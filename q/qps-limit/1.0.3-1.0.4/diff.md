# Comparing `tmp/qps_limit-1.0.3-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4975 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jun-27 11:02 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     4655 b- defN 23-Jun-27 11:02 qps_limit/limiter.py
--rw-rw-r--  2.0 unx     4335 b- defN 23-Jun-27 10:58 qps_limit/run.py
--rw-rw-r--  2.0 unx     2509 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/RECORD
-8 files, 12388 bytes uncompressed, 3891 bytes compressed:  68.6%
+Zip file size: 5253 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jul-03 12:54 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     5244 b- defN 23-Jul-03 12:53 qps_limit/limiter.py
+-rw-rw-r--  2.0 unx     5459 b- defN 23-Jul-03 12:36 qps_limit/run.py
+-rw-rw-r--  2.0 unx     2609 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/RECORD
+8 files, 14201 bytes uncompressed, 4169 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.3.dist-info/METADATA
+Filename: qps_limit-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.3.dist-info/WHEEL
+Filename: qps_limit-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.3.dist-info/top_level.txt
+Filename: qps_limit-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.3.dist-info/zip-safe
+Filename: qps_limit-1.0.4.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.3.dist-info/RECORD
+Filename: qps_limit-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 from .run import batch_run, async_batch_run
 from .limiter import Limiter
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## qps_limit/limiter.py

```diff
@@ -22,34 +22,33 @@
         callback: Optional[Callable] = None,
         progress: bool = True,
         ordered: bool = True,
         verbose: bool = False,
         max_workers: int = 128,
         warmup_steps: int = 1
     ) -> Callable:
-        multiprocessing.set_start_method('fork')
+        try:
+            multiprocessing.set_start_method('fork')
+        except RuntimeError:
+            if self.verbose:
+                print("multiprocessing set_start_method error")
 
         self.func = func
         self.params = params
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
         self.callback = callback
         self.progress = progress
         self.ordered = ordered
         self.verbose = verbose
 
-        self.count_iterator, self.param_iterator = itertools.tee(self.params(), 2)
-        counter = itertools.count()
-        collections.deque(zip(self.count_iterator, counter), maxlen=0)
-        self.count = next(counter)
         if self.verbose:
-            print("find {} data, warmup workers with {} data".format(self.count, warmup_steps))
-
-        self.param_iterator, warmup_param_iterator = itertools.tee(self.param_iterator, 2)
+            print("warmup worker nodes with {} data".format(warmup_steps))
+        self.param_iterator, warmup_param_iterator = itertools.tee(self.params(), 2)
         warmup_param_iterator = itertools.islice(warmup_param_iterator, warmup_steps)
         warmup_start_time = time.time()
         batch_run(
             func=self.func,
             params=warmup_param_iterator,
             max_qps=None,
             max_workers=1
@@ -60,33 +59,34 @@
             self.max_workers = max_workers
         else:
             self.max_workers = min(max_workers, self.worker_max_qps * math.ceil(avg_worker_time))
         if self.verbose:
             print("avg worker time: {:.2f}s -> set worker num: {}".format(avg_worker_time, self.max_workers))
 
         if self.ordered:
-            self.dict = multiprocessing.Manager().dict()
+            self.res_dict = multiprocessing.Manager().dict()
         else:
-            self.queue = multiprocessing.Queue()
+            self.res_queue = multiprocessing.Queue()
 
-        self.workers = []
-        if self.progress:
-            self.progress_queue = multiprocessing.Queue()
-            self.workers.append(multiprocessing.Process(target=self._progress_worker))
-        else:
-            self.progress_queue = None
+        self.job_value = multiprocessing.Value('i', 0)
+        self.worker_value = multiprocessing.Value('i', 0)
+        self.worker_event = multiprocessing.Event()
+        self.job_queue = multiprocessing.Queue() if self.progress else None
 
+        self.workers = []
         for mod in range(self.num_workers):
-            self.workers.append(multiprocessing.Process(target=self._worker, args=(mod,)))
+            self.workers.append(multiprocessing.Process(target=self._worker, args=(mod, )))
 
     def _progress_worker(self):
-        progress_bar = tqdm(total=self.count, desc=self.func.__name__)
+        if self.job_queue is None:
+            return
+        progress_bar = tqdm(total=self.job_count, desc=self.func.__name__)
         progress_cnt = 0
-        while progress_cnt < self.count:
-            progress_bar.update(self.progress_queue.get())
+        while progress_cnt < self.job_count:
+            progress_bar.update(self.job_queue.get())
             progress_cnt += 1
 
     def _worker(self, mod: int):
         def make_worker_iterator():
             for idx, (args, kwargs) in enumerate(self.param_iterator):
                 if idx % self.num_workers == mod:
                     yield args, kwargs
@@ -94,39 +94,52 @@
         batch_run_func = batch_run if not self.streaming else streaming_batch_run
         for idx, res in batch_run_func(
             func=self.func,
             params=make_worker_iterator(),
             max_qps=self.worker_max_qps,
             max_workers=self.max_workers,
             callback=self.callback,
-            progress_queue=self.progress_queue
+            job_queue=self.job_queue,
+            job_value=self.job_value,
+            worker_value=self.worker_value,
+            worker_event=self.worker_event
         ):
             real_idx = idx * self.num_workers + mod
             if self.ordered:
-                self.dict[real_idx] = res
+                self.res_dict[real_idx] = res
             else:
-                self.queue.put((real_idx, res))
+                self.res_queue.put((real_idx, res))
 
     def __call__(self):
         start_time = time.time()
         for worker in self.workers:
             worker.start()
-        consume = 0
-        while consume < self.count:
+        while True:
+            if self.worker_value.value == self.num_workers:
+                break
+        if self.verbose:
+            print("receive {} data from {} worker nodes".format(self.job_value.value, self.worker_value.value))
+        self.job_count = self.job_value.value
+        progress_worker = multiprocessing.Process(target=self._progress_worker)
+        progress_worker.start()
+        self.worker_event.set()
+        job_done = 0
+        while job_done < self.job_count:
             if self.ordered:
-                while consume not in self.dict:
+                while job_done not in self.res_dict:
                     pass
-                yield (consume, self.dict[consume])
-                del self.dict[consume]
+                yield (job_done, self.res_dict[job_done])
+                del self.res_dict[job_done]
             else:
-                yield self.queue.get()
-            consume += 1
-        assert consume == self.count
+                yield self.res_queue.get()
+            job_done += 1
+        assert job_done == self.job_count
         for worker in self.workers:
             worker.join()
+        progress_worker.join()
         end_time = time.time()
         if self.verbose:
             print('elapsed time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
                 end_time - start_time,
-                self.count / (end_time - start_time),
+                self.job_count / (end_time - start_time),
                 self.worker_max_qps * self.num_workers if self.worker_max_qps else float("inf"))
             )
```

## qps_limit/run.py

```diff
@@ -17,15 +17,18 @@
 async def async_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
     max_qps: Optional[float] = None,
     max_workers: int = 128,
     callback: Optional[Callable] = None,
-    progress_queue: Optional[multiprocessing.Queue] = None
+    job_queue: Optional[multiprocessing.Queue] = None,
+    job_value: Optional[multiprocessing.Value] = None,
+    worker_value: Optional[multiprocessing.Value] = None,
+    worker_event: Optional[multiprocessing.Event] = None
 ):
     if max_qps is not None:
         limiter = get_limiter(max_qps)
 
         async def limited_func(*args, **kwargs):
             async with limiter:
                 return await func(*args, **kwargs)
@@ -42,46 +45,63 @@
     queue = asyncio.Queue()
     jobs_cnt = 0
 
     for idx, param in enumerate(params):
         await queue.put((idx, param))
         jobs_cnt += 1
 
+    if job_value:
+        with job_value.get_lock():
+            job_value.value += jobs_cnt
+
+    if worker_value:
+        with worker_value.get_lock():
+            worker_value.value += 1
+
     async def worker():
         while not queue.empty():
             _idx, _param = await queue.get()
             result.append((_idx, await callback_func(*_param[0], **_param[1])))
-            if progress_queue:
-                progress_queue.put_nowait(1)
+            if job_queue:
+                job_queue.put_nowait(1)
+
+    if worker_event:
+        worker_event.wait()
 
     await asyncio.gather(*[worker() for _ in range(max_workers)])
     assert len(result) == jobs_cnt
     return result
 
 
 def batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
     max_qps: Optional[float] = None,
     max_workers: int = 128,
     callback: Optional[Callable] = None,
-    progress_queue: Optional[multiprocessing.Queue] = None
+    job_queue: Optional[multiprocessing.Queue] = None,
+    job_value: Optional[multiprocessing.Value] = None,
+    worker_value: Optional[multiprocessing.Value] = None,
+    worker_event: Optional[multiprocessing.Event] = None
 ):
     return asyncio.new_event_loop().run_until_complete(async_batch_run(**locals()))
 
 
 async def async_streaming_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
     max_qps: Optional[float] = None,
     max_workers: int = 128,
     callback: Optional[Callable] = None,
-    progress_queue: Optional[multiprocessing.Queue] = None
+    job_queue: Optional[multiprocessing.Queue] = None,
+    job_value: Optional[multiprocessing.Value] = None,
+    worker_value: Optional[multiprocessing.Value] = None,
+    worker_event: Optional[multiprocessing.Event] = None
 ):
     if max_qps is not None:
         limiter = get_limiter(max_qps)
 
         async def limited_func(*args, **kwargs):
             async with limiter:
                 return await func(*args, **kwargs)
@@ -98,21 +118,32 @@
     result = asyncio.Queue()
     jobs_cnt = 0
 
     for idx, param in enumerate(params):
         await queue.put((idx, param))
         jobs_cnt += 1
 
+    if job_value:
+        with job_value.get_lock():
+            job_value.value += jobs_cnt
+
+    if worker_value:
+        with worker_value.get_lock():
+            worker_value.value += 1
+
     async def worker():
         while not queue.empty():
             _idx, _param = await queue.get()
             _res = await callback_func(*_param[0], **_param[1])
             await result.put((_idx, _res))
-            if progress_queue:
-                progress_queue.put_nowait(1)
+            if job_queue:
+                job_queue.put_nowait(1)
+
+    if worker_event:
+        worker_event.wait()
 
     asyncio.gather(*[worker() for _ in range(max_workers)])
     jobs_consume = 0
     while jobs_consume < jobs_cnt:
         yield await result.get()
         jobs_consume += 1
     assert jobs_consume == jobs_cnt
@@ -121,15 +152,18 @@
 def streaming_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
     max_qps: Optional[float] = None,
     max_workers: int = 128,
     callback: Optional[Callable] = None,
-    progress_queue: Optional[multiprocessing.Queue] = None
+    job_queue: Optional[multiprocessing.Queue] = None,
+    job_value: Optional[multiprocessing.Value] = None,
+    worker_value: Optional[multiprocessing.Value] = None,
+    worker_event: Optional[multiprocessing.Event] = None
 ):
     async_generator = async_streaming_batch_run(**locals())
 
     def iter_over_async(ait, loop):
         ait = ait.__aiter__()
 
         async def get_next():
```

## Comparing `qps_limit-1.0.3.dist-info/METADATA` & `qps_limit-1.0.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.3
+Version: 1.0.4
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -20,14 +20,16 @@
 Requires-Dist: tqdm
 Requires-Dist: aiolimiter
 
 ## QPS Limit
 
 Run functions under any limited rate using `multiprocessing` + `asyncio`
 
+Available on Unix (i.e. Linux, MacOS) only, as the default multiprocessing start method is `fork`.
+
 ### Installation
 
 ```bash
 pip install qps-limit
 ```
 
 or install manually via git
```

