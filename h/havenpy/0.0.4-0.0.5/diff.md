# Comparing `tmp/havenpy-0.0.4.tar.gz` & `tmp/havenpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "havenpy-0.0.4.tar", last modified: Thu Jun 29 14:38:50 2023, max compression
+gzip compressed data, was "havenpy-0.0.5.tar", last modified: Sun Jul  2 23:02:11 2023, max compression
```

## Comparing `havenpy-0.0.4.tar` & `havenpy-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.312173 havenpy-0.0.4/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-06-29 14:38:50.312052 havenpy-0.0.4/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-06 11:14:59.000000 havenpy-0.0.4/README.md
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.310522 havenpy-0.0.4/havenpy/
--rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-06 11:52:59.000000 havenpy-0.0.4/havenpy/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-07 11:20:36.000000 havenpy-0.0.4/havenpy/interceptor.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.311751 havenpy-0.0.4/havenpy/pb/
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-29 14:21:05.000000 havenpy-0.0.4/havenpy/pb/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     4223 2023-06-29 14:21:05.000000 havenpy-0.0.4/havenpy/pb/manager_pb2.py
--rw-r--r--   0 konsti     (501) staff       (20)    13059 2023-06-29 14:21:05.000000 havenpy-0.0.4/havenpy/pb/manager_pb2_grpc.py
--rw-r--r--   0 konsti     (501) staff       (20)     2317 2023-06-29 07:31:37.000000 havenpy-0.0.4/havenpy/run.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.311331 havenpy-0.0.4/havenpy.egg-info/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)      310 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/SOURCES.txt
--rw-r--r--   0 konsti     (501) staff       (20)        1 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/dependency_links.txt
--rw-r--r--   0 konsti     (501) staff       (20)       32 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/requires.txt
--rw-r--r--   0 konsti     (501) staff       (20)        8 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/top_level.txt
--rw-r--r--   0 konsti     (501) staff       (20)       38 2023-06-29 14:38:50.312213 havenpy-0.0.4/setup.cfg
--rw-r--r--   0 konsti     (501) staff       (20)      314 2023-06-29 14:37:33.000000 havenpy-0.0.4/setup.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.553473 havenpy-0.0.5/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-02 23:02:11.553354 havenpy-0.0.5/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-30 05:08:05.000000 havenpy-0.0.5/README.md
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.551757 havenpy-0.0.5/havenpy/
+-rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-30 05:08:05.000000 havenpy-0.0.5/havenpy/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-30 05:08:05.000000 havenpy-0.0.5/havenpy/interceptor.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.553065 havenpy-0.0.5/havenpy/pb/
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-07-02 03:44:58.000000 havenpy-0.0.5/havenpy/pb/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     4535 2023-07-02 06:06:39.000000 havenpy-0.0.5/havenpy/pb/manager_pb2.py
+-rw-r--r--   0 konsti     (501) staff       (20)    13059 2023-07-02 03:44:58.000000 havenpy-0.0.5/havenpy/pb/manager_pb2_grpc.py
+-rw-r--r--   0 konsti     (501) staff       (20)     2474 2023-07-02 22:41:14.000000 havenpy-0.0.5/havenpy/run.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.552472 havenpy-0.0.5/havenpy.egg-info/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)      310 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        1 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       32 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/requires.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        8 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/top_level.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       38 2023-07-02 23:02:11.553514 havenpy-0.0.5/setup.cfg
+-rw-r--r--   0 konsti     (501) staff       (20)      314 2023-07-02 23:02:07.000000 havenpy-0.0.5/setup.py
```

### Comparing `havenpy-0.0.4/havenpy/interceptor.py` & `havenpy-0.0.5/havenpy/interceptor.py`

 * *Files identical despite different names*

### Comparing `havenpy-0.0.4/havenpy/pb/manager_pb2.py` & `havenpy-0.0.5/havenpy/pb/manager_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,45 +9,45 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmanager.proto\x12\x05haven\"\x07\n\x05\x45mpty\"2\n\x0cSetupRequest\x12\x15\n\x08key_file\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_key_file\"5\n\x07Message\x12\x19\n\x04role\x18\x01 \x01(\x0e\x32\x0b.haven.Role\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"N\n\x15\x43hatCompletionRequest\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12 \n\x08messages\x18\x02 \x03(\x0b\x32\x0e.haven.Message\"&\n\x16\x43hatCompletionResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"2\n\x12ListModelsResponse\x12\x1c\n\x06models\x18\x01 \x03(\x0b\x32\x0c.haven.Model\"<\n\x06Worker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12\x1d\n\x06status\x18\x02 \x01(\x0e\x32\r.haven.Status\"5\n\x13ListWorkersResponse\x12\x1e\n\x07workers\x18\x01 \x03(\x0b\x32\r.haven.Worker\"\xcc\x01\n\x1c\x43reateInferenceWorkerRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x14\n\x0cquantization\x18\x02 \x01(\t\x12\x18\n\x0bworker_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x08gpu_type\x18\x04 \x01(\x0e\x32\x0e.haven.GpuTypeH\x01\x88\x01\x01\x12\x16\n\tgpu_count\x18\x06 \x01(\x05H\x02\x88\x01\x01\x42\x0e\n\x0c_worker_nameB\x0b\n\t_gpu_typeB\x0c\n\n_gpu_count\"&\n\x0fInferenceWorker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t*\x1f\n\x04Role\x12\r\n\tASSISTANT\x10\x00\x12\x08\n\x04USER\x10\x01*<\n\x06Status\x12\n\n\x06ONLINE\x10\x00\x12\x0f\n\x0bUNREACHABLE\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\t\n\x05\x45RROR\x10\x03**\n\x07GpuType\x12\x08\n\x04\x41\x31\x30\x30\x10\x00\x12\r\n\tA100_80GB\x10\x01\x12\x06\n\x02T4\x10\x02\x32\xb4\x04\n\x05Haven\x12,\n\x05Setup\x12\x13.haven.SetupRequest\x1a\x0c.haven.Empty\"\x00\x12Q\n\x0e\x43hatCompletion\x12\x1c.haven.ChatCompletionRequest\x1a\x1d.haven.ChatCompletionResponse\"\x00\x30\x01\x12\x37\n\nListModels\x12\x0c.haven.Empty\x1a\x19.haven.ListModelsResponse\"\x00\x12\x39\n\x0bListWorkers\x12\x0c.haven.Empty\x1a\x1a.haven.ListWorkersResponse\"\x00\x12V\n\x15\x43reateInferenceWorker\x12#.haven.CreateInferenceWorkerRequest\x1a\x16.haven.InferenceWorker\"\x00\x12H\n\x14PauseInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15ResumeInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15\x44\x65leteInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmanager.proto\x12\x05haven\"\x07\n\x05\x45mpty\"2\n\x0cSetupRequest\x12\x15\n\x08key_file\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_key_file\"5\n\x07Message\x12\x19\n\x04role\x18\x01 \x01(\x0e\x32\x0b.haven.Role\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"\xdc\x01\n\x15\x43hatCompletionRequest\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12 \n\x08messages\x18\x02 \x03(\x0b\x32\x0e.haven.Message\x12\x17\n\nmax_tokens\x18\x03 \x01(\x05H\x00\x88\x01\x01\x12\x12\n\x05top_p\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05top_k\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x18\n\x0btemperature\x18\x06 \x01(\x02H\x03\x88\x01\x01\x42\r\n\x0b_max_tokensB\x08\n\x06_top_pB\x08\n\x06_top_kB\x0e\n\x0c_temperature\"&\n\x16\x43hatCompletionResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"2\n\x12ListModelsResponse\x12\x1c\n\x06models\x18\x01 \x03(\x0b\x32\x0c.haven.Model\"<\n\x06Worker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12\x1d\n\x06status\x18\x02 \x01(\x0e\x32\r.haven.Status\"5\n\x13ListWorkersResponse\x12\x1e\n\x07workers\x18\x01 \x03(\x0b\x32\r.haven.Worker\"\xcc\x01\n\x1c\x43reateInferenceWorkerRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x14\n\x0cquantization\x18\x02 \x01(\t\x12\x18\n\x0bworker_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x08gpu_type\x18\x04 \x01(\x0e\x32\x0e.haven.GpuTypeH\x01\x88\x01\x01\x12\x16\n\tgpu_count\x18\x06 \x01(\x05H\x02\x88\x01\x01\x42\x0e\n\x0c_worker_nameB\x0b\n\t_gpu_typeB\x0c\n\n_gpu_count\"&\n\x0fInferenceWorker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t*\x1f\n\x04Role\x12\r\n\tASSISTANT\x10\x00\x12\x08\n\x04USER\x10\x01*<\n\x06Status\x12\n\n\x06ONLINE\x10\x00\x12\x0f\n\x0bUNREACHABLE\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\t\n\x05\x45RROR\x10\x03**\n\x07GpuType\x12\x08\n\x04\x41\x31\x30\x30\x10\x00\x12\r\n\tA100_80GB\x10\x01\x12\x06\n\x02T4\x10\x02\x32\xb4\x04\n\x05Haven\x12,\n\x05Setup\x12\x13.haven.SetupRequest\x1a\x0c.haven.Empty\"\x00\x12Q\n\x0e\x43hatCompletion\x12\x1c.haven.ChatCompletionRequest\x1a\x1d.haven.ChatCompletionResponse\"\x00\x30\x01\x12\x37\n\nListModels\x12\x0c.haven.Empty\x1a\x19.haven.ListModelsResponse\"\x00\x12\x39\n\x0bListWorkers\x12\x0c.haven.Empty\x1a\x1a.haven.ListWorkersResponse\"\x00\x12V\n\x15\x43reateInferenceWorker\x12#.haven.CreateInferenceWorkerRequest\x1a\x16.haven.InferenceWorker\"\x00\x12H\n\x14PauseInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15ResumeInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15\x44\x65leteInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'manager_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _ROLE._serialized_start=699
-  _ROLE._serialized_end=730
-  _STATUS._serialized_start=732
-  _STATUS._serialized_end=792
-  _GPUTYPE._serialized_start=794
-  _GPUTYPE._serialized_end=836
+  _ROLE._serialized_start=842
+  _ROLE._serialized_end=873
+  _STATUS._serialized_start=875
+  _STATUS._serialized_end=935
+  _GPUTYPE._serialized_start=937
+  _GPUTYPE._serialized_end=979
   _EMPTY._serialized_start=24
   _EMPTY._serialized_end=31
   _SETUPREQUEST._serialized_start=33
   _SETUPREQUEST._serialized_end=83
   _MESSAGE._serialized_start=85
   _MESSAGE._serialized_end=138
-  _CHATCOMPLETIONREQUEST._serialized_start=140
-  _CHATCOMPLETIONREQUEST._serialized_end=218
-  _CHATCOMPLETIONRESPONSE._serialized_start=220
-  _CHATCOMPLETIONRESPONSE._serialized_end=258
-  _MODEL._serialized_start=260
-  _MODEL._serialized_end=281
-  _LISTMODELSRESPONSE._serialized_start=283
-  _LISTMODELSRESPONSE._serialized_end=333
-  _WORKER._serialized_start=335
-  _WORKER._serialized_end=395
-  _LISTWORKERSRESPONSE._serialized_start=397
-  _LISTWORKERSRESPONSE._serialized_end=450
-  _CREATEINFERENCEWORKERREQUEST._serialized_start=453
-  _CREATEINFERENCEWORKERREQUEST._serialized_end=657
-  _INFERENCEWORKER._serialized_start=659
-  _INFERENCEWORKER._serialized_end=697
-  _HAVEN._serialized_start=839
-  _HAVEN._serialized_end=1403
+  _CHATCOMPLETIONREQUEST._serialized_start=141
+  _CHATCOMPLETIONREQUEST._serialized_end=361
+  _CHATCOMPLETIONRESPONSE._serialized_start=363
+  _CHATCOMPLETIONRESPONSE._serialized_end=401
+  _MODEL._serialized_start=403
+  _MODEL._serialized_end=424
+  _LISTMODELSRESPONSE._serialized_start=426
+  _LISTMODELSRESPONSE._serialized_end=476
+  _WORKER._serialized_start=478
+  _WORKER._serialized_end=538
+  _LISTWORKERSRESPONSE._serialized_start=540
+  _LISTWORKERSRESPONSE._serialized_end=593
+  _CREATEINFERENCEWORKERREQUEST._serialized_start=596
+  _CREATEINFERENCEWORKERREQUEST._serialized_end=800
+  _INFERENCEWORKER._serialized_start=802
+  _INFERENCEWORKER._serialized_end=840
+  _HAVEN._serialized_start=982
+  _HAVEN._serialized_end=1546
 # @@protoc_insertion_point(module_scope)
```

### Comparing `havenpy-0.0.4/havenpy/pb/manager_pb2_grpc.py` & `havenpy-0.0.5/havenpy/pb/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `havenpy-0.0.4/havenpy/run.py` & `havenpy-0.0.5/havenpy/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 		channel = grpc.intercept_channel(channel, interceptor)
 		self.client = manager_pb2_grpc.HavenStub(channel)
 
 	def setup(self, key_file: str) -> manager_pb2.Empty:
 		request = manager_pb2.SetupRequest(key_file=key_file)
 		return self.client.Setup(request)
 
-	def chat_completion(self, worker_name: str, messages: List[manager_pb2.Message], stream: bool = False) -> manager_pb2.ChatCompletionResponse or str:
-		request = manager_pb2.ChatCompletionRequest(worker_name=worker_name, messages=messages)
+	def chat_completion(self, worker_name: str, messages: List[manager_pb2.Message], stream: bool = False, max_tokens: int = -1, top_p: float = -1, top_k: int = -1, temperature: float = -1) -> manager_pb2.ChatCompletionResponse or str:
+		request = manager_pb2.ChatCompletionRequest(worker_name=worker_name, messages=messages, max_tokens=max_tokens, top_p=top_p, top_k=top_k, temperature=temperature)
 		responseStream: manager_pb2.ChatCompletionResponse = self.client.ChatCompletion(request)
 
 		if stream:
 			return responseStream
 		
 		res: str = ""
 		for response in responseStream:
```

