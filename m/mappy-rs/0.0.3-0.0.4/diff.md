# Comparing `tmp/mappy_rs-0.0.3.tar.gz` & `tmp/mappy_rs-0.0.4.tar.gz`

## Comparing `mappy_rs-0.0.3.tar` & `mappy_rs-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 mappy_rs-0.0.3/Cargo.toml
--rw-r--r--   0     1001      123     3431 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/.github/CONTRIBUTING.md
--rw-r--r--   0     1001      123      499 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/.github/dependabot.yml
--rw-r--r--   0     1001      123     1749 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     2218 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/.github/workflows/check.yml
--rw-r--r--   0     1001      123     4456 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/.gitignore
--rw-r--r--   0     1001      123      738 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     1088 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/LICENSE.MD
--rw-r--r--   0     1001      123     4892 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/README.md
--rw-r--r--   0     1001      123   187724 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/img/crab_map.webp
--rw-r--r--   0     1001      123     1171 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/pyproject.toml
--rw-r--r--   0     1001      123        0 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/resources/benchmarking/fastq/.gitkeep
--rw-r--r--   0     1001      123        0 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/resources/benchmarking/index/.gitkeep
--rw-r--r--   0     1001      123     1721 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/resources/test/test.fa
--rw-r--r--   0     1001      123   136470 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/resources/test/test.mmi
--rwxr-xr-x   0     1001      123      839 2023-03-09 11:39:04.000000 mappy_rs-0.0.3/run-maturin-action.sh
--rw-r--r--   0     1001      123    32694 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/src/lib.rs
--rw-r--r--   0     1001      123     2140 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/tests/benchmark.py
--rw-r--r--   0     1001      123     5177 2023-03-09 11:38:25.000000 mappy_rs-0.0.3/tests/python_test.py
--rw-r--r--   0        0        0    16907 2023-03-09 11:40:30.000000 mappy_rs-0.0.3/Cargo.lock
--rw-r--r--   0        0        0     6028 1970-01-01 00:00:00.000000 mappy_rs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 mappy_rs-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      123     3431 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/.github/CONTRIBUTING.md
+-rw-r--r--   0     1001      123      499 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/.github/dependabot.yml
+-rw-r--r--   0     1001      123     1749 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     2228 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/.github/workflows/check.yml
+-rw-r--r--   0     1001      123     4486 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/.gitignore
+-rw-r--r--   0     1001      123      738 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     1088 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/LICENSE.MD
+-rw-r--r--   0     1001      123     5013 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/README.md
+-rw-r--r--   0     1001      123   187724 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/img/crab_map.webp
+-rw-r--r--   0     1001      123     1419 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/pyproject.toml
+-rw-r--r--   0     1001      123        0 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/resources/benchmarking/fastq/.gitkeep
+-rw-r--r--   0     1001      123        0 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/resources/benchmarking/index/.gitkeep
+-rw-r--r--   0     1001      123     1721 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/resources/test/test.fa
+-rw-r--r--   0     1001      123   136470 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/resources/test/test.mmi
+-rwxr-xr-x   0     1001      123      839 2023-07-03 14:47:08.000000 mappy_rs-0.0.4/run-maturin-action.sh
+-rw-r--r--   0     1001      123    40859 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      123     2230 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/tests/benchmark.py
+-rw-r--r--   0     1001      123     4369 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/tests/memory.py
+-rw-r--r--   0     1001      123     5177 2023-07-03 14:46:28.000000 mappy_rs-0.0.4/tests/python_test.py
+-rw-r--r--   0        0        0    18771 2023-07-03 14:47:53.000000 mappy_rs-0.0.4/Cargo.lock
+-rw-r--r--   0        0        0     6401 1970-01-01 00:00:00.000000 mappy_rs-0.0.4/PKG-INFO
```

### Comparing `mappy_rs-0.0.3/Cargo.toml` & `mappy_rs-0.0.4/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "mappy-rs"
-version = "0.0.3"
+version = "0.0.4"
 edition = "2021"
 authors = ["Rory Munro <roryjmunro1@gmail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python Bindings to multithreaded rust minimap2"
 repository = "https://github.com/alexomics/mm2_rs"
 categories = ["science"]
 keywords = ["bioinformatics", "fasta", "alignment", "fastq"]
@@ -17,19 +17,20 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "mappy_rs"
 
 [dependencies]
 libc = "0.2"
 pyo3 = { version = "0.18" }
-minimap2-sys = "0.1.10"
-minimap2 = "0.1.11"
+minimap2-sys = "0.1.12+minimap2.2.26"
+minimap2 = {git = "https://github.com/jguhlin/minimap2-rs.git", rev = "037abe5"}
 crossbeam = "0.8.2"
-threadpool = "1.0.0"
 fnv = "1.0.7"
+ctrlc = {version = "3.4.0", features = ["termination"] }
+itertools = "0.10.5"
 
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
 
 [profile.release]
 opt-level = 3
```

### Comparing `mappy_rs-0.0.3/.github/CONTRIBUTING.md` & `mappy_rs-0.0.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/.github/workflows/CI.yml` & `mappy_rs-0.0.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/.github/workflows/check.yml` & `mappy_rs-0.0.4/.github/workflows/check.yml`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         run: "pytest"
 
   msrv:
     runs-on: "ubuntu-latest"
     needs: ["cargo-test", "python-test"]
     strategy:
       matrix:
-        msrv: ["1.58.1"]
+        msrv: ["1.63.0", "1.64.0"]
     name: "ubuntu / ${{ matrix.msrv }}"
     steps:
       - uses: "actions/checkout@v3"
       - uses: "dtolnay/rust-toolchain@master"
         with:
           toolchain: "${{ matrix.msrv }}"
       - name: "cargo +${{ matrix.msrv }} check"
```

### Comparing `mappy_rs-0.0.3/.gitignore` & `mappy_rs-0.0.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 /target
+/bytehound
+*.dat
+*.html
+*.bin
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 
 # C extensions
```

### Comparing `mappy_rs-0.0.3/.pre-commit-config.yaml` & `mappy_rs-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/LICENSE.MD` & `mappy_rs-0.0.4/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/README.md` & `mappy_rs-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Mappy-rs
 [![build](https://github.com/Adoni5/mappy-rs/actions/workflows/CI.yml/badge.svg)](https://github.com/Adoni5/mappy-rs/actions/workflows/CI.yml)
 [![CI](https://github.com/Adoni5/mappy-rs/actions/workflows/check.yml/badge.svg)](https://github.com/Adoni5/mappy-rs/actions/workflows/check.yml)
 
 
-![A map with a crab on it](img/crab_map.webp)
+![A map with a crab on it](https://github.com/Adoni5/mappy-rs/blob/main/img/crab_map.webp)
 
 A multi-threaded minimap2 aligner for python. Built for [readfish](https://github.com/LooseLab/readfish/) compatibility.
 
-Heavily leaning on and inspired by Joeseph Guhlin's minimap2-rs [repository](https://github.com/jguhlin/minimap2-rs). They also have a more heavily featured python client, however this one simply multi threads and maps.
+Heavily leaning on and inspired by Joeseph Guhlin's minimap2-rs [repository](https://github.com/jguhlin/minimap2-rs). They also have a more heavily featured python client, which also provides multithreaded alignment. This client provides a more simple streaming interface for use in pipelines.
 
 `pip install mappy-rs`
 
 ## Developers
 Start with some Docs on Py03 - https://pyo3.rs/latest/
 
 If you wish to contribute, have a look at [CONTRIBUTING.md](.github/CONTRIBUTING.md)
@@ -38,29 +38,29 @@
 Then in your python shell of choice:
 
 ```python
 import mappy_rs
 aligner = mappy_rs.Aligner("resources/test/test.mmi")
 ```
 
-The current iteration of `mappy-rs` serves as a drop in for `mappy`, implementing all the same methods. However if this is the use case, you may well be better off using `mappy`, as the extra level of Rust betwene your python and C++ may well add slighly slower performance.
+The current iteration of `mappy-rs` serves as a drop in for `mappy`, implementing all the same methods. However if this is the use case, you may well be better off using `mappy`, as the extra level of Rust between your python and C++ may well add slightly slower performance.
 
 ### Multithreading
 In order to use multi threading, one must first enable it.
 
 ```python
 import mappy_rs
 aligner = mappy_rs.Aligner("resources/test/test.mmi")
 # Use 10 threads
 aligner.enable_threading(10)
 ```
 
 Enabling threading makes the `map_batch` method available.
 This method requires a list or iterable of dictionaries, which can have any number of keys and depth, but **must** contain the key `seq` with a string value in the top-level dictionary.
-Currently, the maximum batch size tobe iterated in one call is 20000.
+Currently, the maximum batch size to be iterated in one call is 20000.
 
 For example:
 
 ```python
 import mappy_rs
 aligner = mappy_rs.Aligner("resources/test/test.mmi")
 aligner.enable_threading(10)
```

### Comparing `mappy_rs-0.0.3/img/crab_map.webp` & `mappy_rs-0.0.4/img/crab_map.webp`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/resources/test/test.fa` & `mappy_rs-0.0.4/resources/test/test.fa`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/resources/test/test.mmi` & `mappy_rs-0.0.4/resources/test/test.mmi`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/run-maturin-action.sh` & `mappy_rs-0.0.4/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/src/lib.rs` & `mappy_rs-0.0.4/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 //! Serves as a drop in for mappy in single threaded mode.
 //! Designed for use with readfish https://github.com/LooseLab/readfish/
 #![deny(missing_docs)]
 #![deny(clippy::missing_docs_in_private_items)]
 
 use crossbeam::channel::{bounded, Receiver, RecvError, Sender};
 use crossbeam::queue::ArrayQueue;
-use crossbeam::utils::Backoff;
 use fnv::FnvHashMap;
+use itertools::all;
 use pyo3::exceptions::{
     PyKeyError, PyNotImplementedError, PyRuntimeError, PyTypeError, PyValueError,
 };
 use pyo3::prelude::*;
 use pyo3::pyclass::IterNextOutput;
 use pyo3::types::{PyIterator, PyList, PySequence, PyTuple};
 use pyo3::FromPyObject;
 use std::collections::HashMap;
 use std::fmt::{Display, Formatter};
+use std::mem;
 use std::sync::{Arc, Mutex};
+use std::time::Duration;
 
 /// Strand enum
 #[pyclass]
 #[derive(Debug, PartialEq, Eq, Copy, Clone)]
 pub enum Strand {
     /// Maps to the forward strand
     Forward,
     /// Maps to the Reverse strand
     Reverse,
 }
 
 /// Enum containing results from multithreaded Alignment
 #[derive(Debug)]
 enum WorkQueue<T> {
-    /// Lemme see you work work wokr work, shorty sumthin sumthin
+    /// Lemme see you work work work work, shorty sumthin sumthin
     Work(T),
     /// The threads are finished
     Done,
     /// Result of multi threaded mapping queue
     Result(T),
     /// All threads have finished
     Finished,
@@ -279,23 +281,32 @@
     #[getter(is_primary)]
     fn get_is_primary(&self) -> PyResult<bool> {
         Ok(self.is_primary)
     }
 }
 
 /// Aligner struct, mimicking minimap2's python interface
-#[pyclass]
-#[derive(Clone)]
+#[pyclass(unsendable)]
+#[allow(clippy::type_complexity)]
+
 pub struct Aligner {
     /// Inner minimap2::Aligner
     pub aligner: minimap2::Aligner,
     /// Number of mapping threads
     n_threads: usize,
+    /// thread handles
+    _handles: Arc<Mutex<Vec<std::thread::JoinHandle<()>>>>,
+    /// stop the threads
+    stop: Arc<Mutex<bool>>,
+    /// Work queue stores strings to map and ids to get the corresponding dict back
+    work_queue: Arc<ArrayQueue<WorkQueue<(usize, String)>>>,
+    /// Results of the threads go here
+    results_queue: Arc<ArrayQueue<WorkQueue<(Vec<Mapping>, usize)>>>,
 }
-unsafe impl Send for Aligner {}
+// unsafe impl Send for Aligner {}
 
 #[pymethods]
 impl Aligner {
     /// Initialise a new Py Class Aligner
     /// Aligner struct, mimicking minimap2's python interface
     #[new]
     #[pyo3(signature = (fn_idx_in=None, preset=None, k=None, w=None, min_cnt=None, min_chain_score=None, min_dp_score=None, bw=None, best_n=None, n_threads=3, fn_idx_out=None, max_frag_len=None, extra_flags=None, seq=None, scoring=None))]
@@ -313,14 +324,16 @@
         n_threads: usize,
         fn_idx_out: Option<std::path::PathBuf>,
         max_frag_len: Option<usize>,
         extra_flags: Option<usize>,
         seq: Option<String>,
         scoring: Option<&PyTuple>,
     ) -> PyResult<Self> {
+        // handle ctrl c signal to kill threads - development use only!
+        println!("{n_threads}");
         let mut mapopts = minimap2::MapOpt::default();
         let mut idxopts = minimap2::IdxOpt::default();
         unsafe { minimap2_sys::mm_set_opt(std::ptr::null(), &mut idxopts, &mut mapopts) };
         if let Some(preset) = preset {
             let _preset = std::ffi::CString::new(preset).unwrap();
             unsafe {
                 minimap2_sys::mm_set_opt(_preset.as_ptr() as *const i8, &mut idxopts, &mut mapopts)
@@ -402,25 +415,30 @@
                 // Close the reader
                 minimap2_sys::mm_idx_reader_close(idx_reader);
                 // Set index opts
                 minimap2_sys::mm_mapopt_update(&mut mapopts, *idx.as_ptr());
                 // Idx index name
                 minimap2_sys::mm_idx_index_name(idx.assume_init());
             };
-
-            return Ok(Aligner {
+            let al = Aligner {
                 aligner: minimap2::Aligner {
                     mapopt: mapopts,
                     idxopt: idxopts,
                     threads: n_threads,
                     idx: Some(unsafe { *idx.assume_init() }),
                     idx_reader: Some(unsafe { *idx_reader }),
                 },
                 n_threads: 0,
-            });
+                _handles: Arc::new(Mutex::new(vec![])),
+                stop: Arc::new(Mutex::new(false)),
+                work_queue: Arc::new(ArrayQueue::<WorkQueue<(usize, String)>>::new(50000)),
+                results_queue: Arc::new(ArrayQueue::<WorkQueue<(Vec<Mapping>, usize)>>::new(50000)),
+            };
+            // al.setup_signal();
+            return Ok(al);
         }
         Err(PyRuntimeError::new_err("Did not create or open an index"))
     }
 
     /// Return the sequence names contained within an index as a list.
     #[getter]
     fn seq_names(&self) -> PyResult<Vec<String>> {
@@ -485,32 +503,143 @@
                         target_start: m.target_start,              // i32,
                         target_end: m.target_end,                  // i32,
                         match_len: m.match_len,                    // i32,
                         block_len: m.block_len,                    // i32,
                         mapq: m.mapq,                              // u32,
                         is_primary: m.is_primary,                  // bool
                         cigar: a.cigar.unwrap_or_default(),        // Vec<(u32, u8)>
-                        NM: a.nm,
-                        MD: a.md,
-                        cs: a.cs,
+                        NM: a.nm,                                  // i32
+                        MD: a.md,                                  // Option<String>
+                        cs: a.cs,                                  // Option<String>
                     }
                 })
                 .collect()),
             Err(e) => Err(PyRuntimeError::new_err(e)),
         }
     }
 
+    /// Map a single read, blocking
+    #[pyo3(signature = (_seq, seq2=None, _cs=false, _MD=false), text_signature = "(_seq, seq2=None, _cs=False, _MD=False)")]
+    #[allow(non_snake_case)]
+    fn map_no_op(
+        &self,
+        _seq: String,
+        seq2: Option<String>,
+        _cs: bool,
+        _MD: bool,
+    ) -> PyResult<Vec<Mapping>> {
+        // TODO: PyIterProtocol to map single reads and return as a generator
+        if let Some(_seq2) = seq2 {
+            return Err(PyNotImplementedError::new_err(
+                "Using `seq2` is not implemented",
+            ));
+        }
+        Ok(self.no_op_map())
+    }
+
     ///  Enable multi threading on this mappy instance.
     ///
     /// Example
     /// -------
     /// `aligner::enable_threading(8)`
     #[pyo3(signature = (n_threads), text_signature = "(n_threads=8)")]
     fn enable_threading(&mut self, n_threads: usize) -> PyResult<()> {
         self.n_threads = n_threads;
+        let dones = Arc::new(Mutex::new(vec![false; n_threads]));
+        for i in 0..n_threads {
+            let _aligner = self.aligner.clone();
+            let stop = Arc::clone(&self.stop);
+            let wq = Arc::clone(&self.work_queue);
+            let rq = Arc::clone(&self.results_queue);
+            let thread_number = i;
+            let done_ref = Arc::clone(&dones);
+
+            // start the threads
+            std::thread::spawn(move || {
+                loop {
+                    // STOP SIGNAL RECEVIED SIGINT/SIGTERM
+                    if *stop.lock().unwrap() {
+                        break;
+                    }
+                    let wait_as_done = {
+                        let mut dr: std::sync::MutexGuard<'_, Vec<bool>> = done_ref.lock().unwrap();
+                        let done = *dr.get(thread_number).unwrap();
+                        let all_done = all(dr.iter(), |elt| *elt);
+                        if all_done {
+                            // everythread has sent a done, so set them all to not done again
+                            for b in dr.iter_mut() {
+                                *b = !*b;
+                            }
+                        }
+                        done & !all_done
+                    };
+                    // this thread has sent a done and not all other threads are fininshed
+                    if wait_as_done {
+                        std::thread::sleep(Duration::from_millis(1));
+                        continue;
+                    }
+                    match wq.pop() {
+                        None => std::thread::sleep(Duration::from_millis(10)),
+                        Some(work_item) => {
+                            match work_item {
+                                WorkQueue::Done => {
+                                    rq.push(WorkQueue::Done).unwrap();
+                                    {
+                                        done_ref.lock().unwrap()[thread_number] = true;
+                                    }
+                                }
+                                WorkQueue::Work((id_num, seq)) => {
+                                    match _aligner.map(
+                                        seq.as_bytes(),
+                                        true,
+                                        false,
+                                        Some(_aligner.mapopt.max_frag_len as usize),
+                                        None,
+                                    ) {
+                                        Ok(_mappings) => {
+                                            mem::drop(seq);
+                                            let mappings: Vec<Mapping> = _mappings
+                                                .into_iter()
+                                                .map(|m| {
+                                                    let a = m.alignment.unwrap();
+                                                    Mapping {
+                                                        query_start: m.query_start,                // i32,
+                                                        query_end: m.query_end, // i32,
+                                                        strand: Strand::from_mm2_strand(m.strand), // Strand,
+                                                        target_name: m.target_name.unwrap(), // String,
+                                                        target_len: m.target_len,            // i32,
+                                                        target_start: m.target_start,        // i32,
+                                                        target_end: m.target_end,            // i32,
+                                                        match_len: m.match_len,              // i32,
+                                                        block_len: m.block_len,              // i32,
+                                                        mapq: m.mapq,                        // u32,
+                                                        is_primary: m.is_primary,            // bool
+                                                        cigar: a.cigar.unwrap_or_default(), // Vec<(u32, u8)>
+                                                        NM: a.nm,
+                                                        MD: a.md,
+                                                        cs: a.cs,
+                                                    }
+                                                })
+                                                .collect();
+                                            rq.push(WorkQueue::Result((mappings, id_num))).unwrap();
+                                        }
+                                        Err(_) => {
+                                            eprintln!("Failed to map sequence in threaded implementation.")
+                                        }
+                                    }
+                                }
+                                _ => {
+                                    println!("What is this doing in the work queue")
+                                }
+                            }
+                        }
+                    }
+                }
+            });
+        }
         Ok(())
     }
 
     /// Align a sequence with optional Metadata tuple. If provided, the tuple MUST be in the shape of (channel_number: int, read_id: str)
     fn map_batch(&self, seqs: &PyAny) -> PyResult<AlignmentBatchResultIter> {
         let mut res = AlignmentBatchResultIter::new();
         // Set the number of threads
@@ -528,29 +657,58 @@
     }
 
     /// Get the k value from the index.
     #[getter]
     fn k(&self) -> PyResult<i32> {
         Ok(self.aligner.idx.unwrap().k)
     }
-
     /// Get the w value form the index.
     #[getter]
     fn w(&self) -> PyResult<i32> {
         Ok(self.aligner.idx.unwrap().w)
     }
 
     /// Get the number of sequences present in the index
     #[getter]
     fn n_seq(&self) -> PyResult<u32> {
         Ok(self.aligner.idx.unwrap().n_seq)
     }
 }
 
 impl Aligner {
+    /// Instead of calling out to the ALigner, return a predefined dummy mapping
+    pub fn no_op_map(&self) -> Vec<Mapping> {
+        vec![Mapping {
+            query_start: 0,                                             // i32,
+            query_end: 1000,                                            // i32,
+            strand: Strand::from_mm2_strand(minimap2::Strand::Forward), // Strand,
+            target_name: String::from("Hello"),                         // String,
+            target_len: 101010,                                         // i32,
+            target_start: 10,                                           // i32,
+            target_end: 1010,                                           // i32,
+            match_len: 1000,                                            // i32,
+            block_len: 1000,                                            // i32,
+            mapq: 60,                                                   // u32,
+            is_primary: true,                                           // bool
+            cigar: vec![],                                              // Vec<(u32, u8)>
+            NM: 0,
+            MD: None,
+            cs: Some(String::from("Cigar string")),
+        }]
+    }
+    /// Setup signal catching for ctrl c to stop threads
+    pub fn setup_signal(&self) {
+        let stop = Arc::clone(&self.stop);
+        ctrlc::set_handler(move || {
+            println!("Signal intercepted");
+            *stop.lock().unwrap() = true;
+            std::process::exit(0);
+        })
+        .expect("Failed to set signal listener");
+    }
     /// Private function
     /// Get a sequence or subsequence of a contig loaded into the index.
     pub fn _get_index_seq(&self, name: String, start: i32, mut end: i32) -> Result<String, &str> {
         if !self.aligner.has_index() {
             return Err("No index");
         }
         if (self.aligner.mapopt.flag & minimap2_sys::MM_F_CIGAR as i64 != 0)
@@ -609,14 +767,15 @@
             }
         }
         Ok(std::string::String::from_utf8(seq_buf).unwrap())
     }
 
     /// Align a batch of reads provided in an iterator, using a threadpool with the number of threads specified by
     /// .enable_threading()
+    #[allow(clippy::type_complexity)]
     pub fn _map_batch(&self, res: &mut AlignmentBatchResultIter, seqs: &PyAny) -> PyResult<()> {
         if self.n_threads == 0_usize {
             return Err(PyRuntimeError::new_err(
                 "Multi threading not enabled on this instance. Please call `.enable_threading()`",
             ));
         }
         match seqs.extract() {
@@ -626,96 +785,94 @@
             Ok(SupportedTypes::Sequence(_)) => (),
             _ => {
                 return Err(PyTypeError::new_err(
                     "Unsupported batch type, pass a list, iter, generator or tuple",
                 ))
             }
         };
-        for _ in 0..self.n_threads {
-            let work_queue: Arc<ArrayQueue<WorkQueue<(usize, String)>>> =
-                Arc::clone(&res.work_queue);
-            let results_tx = res.tx.clone();
-            let aligner = self.clone();
-            let counter = Arc::clone(&res._n_finished_threads);
-            let n_threads = res._n_threads;
-            std::thread::spawn(move || {
-                loop {
-                    // new backoff
-                    let backoff = Backoff::new();
-                    // pop returns None if the queue is empty, which is possible at the start as data hasn't been added below
-                    match work_queue.pop() {
-                        // We
-                        Some(worky) => match worky {
-                            WorkQueue::Done => {
-                                // This thread has finished
-                                // Lock the mutex and increment
-                                let mut num = counter.lock().unwrap();
-                                *num += 1;
-                                // ALL threads have finished
-                                if *num == n_threads {
-                                    results_tx.send(WorkQueue::Finished).unwrap();
-                                }
+        let results_queue: Arc<ArrayQueue<WorkQueue<(Vec<Mapping>, usize)>>> =
+            Arc::clone(&self.results_queue);
+        let results_tx = res.tx.clone();
+        let counter = Arc::clone(&res._n_finished_threads);
+        let n_threads = res._n_threads;
+        std::thread::spawn(move || {
+            loop {
+                //             // pop returns None if the queue is empty, which is possible at the start as data hasn't been added below
+                match results_queue.pop() {
+                    //                 // We
+                    Some(worky) => match worky {
+                        // each thread can only see one workqueue DONE
+                        WorkQueue::Done => {
+                            // This thread has finished
+                            // Lock the mutex and increment
+                            let mut num = counter.lock().unwrap();
+                            *num += 1;
+                            // println!("{num}");
+                            // ALL threads have finished
+                            if *num == n_threads {
+                                results_tx.send(WorkQueue::Finished).unwrap();
+                                // reset number of finshed threads
                                 break;
                             }
-                            WorkQueue::Work((id_num, seq)) => {
-                                let maps = aligner.map(seq, None, true, true).unwrap();
-                                match results_tx.send(WorkQueue::Result((maps, id_num))) {
-                                    Ok(()) => {}
-                                    Err(e) => {
-                                        eprintln!("Internal error returning data. {e}");
-                                    }
+                        }
+                        WorkQueue::Result(result) => {
+                            let id = result.1;
+                            match results_tx.send(WorkQueue::Result(result)) {
+                                Ok(()) => {}
+                                Err(e) => {
+                                    eprintln!("Internal error returning data. {e} {id}");
                                 }
                             }
-                            _ => {
-                                eprintln!("Wrong WorkQueue arm seen in worker thread.")
-                            }
-                        },
-                        // Todo Crossbeam backoff rather than continue
-                        None => {
-                            backoff.snooze();
                         }
+                        _ => {
+                            eprintln!("Wrong WorkQueue arm seen in worker thread.")
+                        }
+                    },
+                    // Todo Crossbeam backoff rather than continue
+                    None => {
+                        std::thread::sleep(Duration::from_millis(5));
                     }
-                    // (id_num, seq): (usize, String)
                 }
-            });
-        }
+                //             // (id_num, seq): (usize, String)
+            }
+        });
         let iter = match seqs.iter() {
             Ok(it) => it,
             _ => return Err(PyTypeError::new_err("Could not iterate batch")),
         };
-        let work_queue: Arc<ArrayQueue<WorkQueue<(usize, String)>>> = Arc::clone(&res.work_queue);
-        for (id_num, py_dicts) in iter.enumerate() {
-            let py_dict = py_dicts?;
+        let work_queue: Arc<ArrayQueue<WorkQueue<(usize, String)>>> = Arc::clone(&self.work_queue);
+        for (id_num, py_dict) in iter.enumerate() {
+            let py_dict = py_dict?;
             let data: HashMap<String, Py<PyAny>> = match py_dict.extract() {
                 Ok(x) => x,
                 _ => {
                     return Err(PyTypeError::new_err(
                         "Element in iterable is not a dictionary",
                     ))
                 }
             };
             res.data.insert(id_num, data);
             let seq: String = match py_dict.get_item("seq") {
-                Ok(seq) => match seq.extract() {
-                    Ok(seq) => seq,
+                Ok(seq) => match seq.extract::<String>() {
+                    Ok(seq) => seq.clone(),
                     _ => return Err(PyValueError::new_err("`seq` must be a string")),
                 },
                 _ => {
                     return Err(PyKeyError::new_err(
                         "AHHH Key 🗝️  not found in iterated dictionary",
                     ))
                 }
             };
-
             work_queue.push(WorkQueue::Work((id_num, seq))).unwrap();
         }
-        // Now we add 4 dones, one for each thread. When the threads see this they know to close as there is no more data
+        // Now we add n_thread dones, one for each thread. When the threads see this they know to close as there is no more data
         for _ in 0..self.n_threads {
             work_queue.push(WorkQueue::Done).unwrap();
         }
+
         Ok(())
     }
 }
 
 /// Python iterable types that are accepted by the `Aligner.map_batch()` function
 #[derive(FromPyObject)]
 enum SupportedTypes<'py> {
@@ -734,16 +891,14 @@
 pub struct AlignmentBatchResultIter {
     /// Sender of results into this scope
     tx: Sender<WorkQueue<(Vec<Mapping>, usize)>>,
     /// Receive the sent data
     rx: Receiver<WorkQueue<(Vec<Mapping>, usize)>>,
     /// HashMap for caching sent data
     data: FnvHashMap<usize, HashMap<String, Py<PyAny>>>,
-    /// ArrayQueue for work
-    work_queue: Arc<ArrayQueue<WorkQueue<(usize, String)>>>,
     /// Number of threads, which checks against the number offinished threads
     _n_threads: usize,
     /// Number of finished threads, used to know when to close the receiver. Is unlocked in the worker threads.
     _n_finished_threads: Arc<Mutex<usize>>,
 }
 
 impl Default for AlignmentBatchResultIter {
@@ -760,15 +915,14 @@
     #[new]
     pub fn new() -> Self {
         let (tx, rx) = bounded(20000);
         AlignmentBatchResultIter {
             tx,
             rx,
             data: FnvHashMap::default(),
-            work_queue: Arc::new(ArrayQueue::<WorkQueue<(usize, String)>>::new(50000)),
             _n_threads: 0_usize,
             _n_finished_threads: Arc::new(Mutex::new(0_usize)),
         }
     }
 
     /// Set the number of threads on this mappy_rs instance
     pub fn set_n_threads(&mut self, n_threads: usize) {
@@ -778,35 +932,31 @@
     /// Returns the Iterable, in this case the struct itself.
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
 
     /// Returns the next element in the Iterator.
     #[allow(clippy::type_complexity)]
-    fn __next__(
-        &mut self,
-    ) -> IterNextOutput<(Vec<Mapping>, HashMap<String, Py<PyAny>>), &'static str> {
+    fn __next__(&mut self) -> IterNextOutput<(Vec<Mapping>, HashMap<String, Py<PyAny>>), &str> {
         let try_recv = self.rx.recv();
         match try_recv {
             Ok(work_queue_member) => match work_queue_member {
-                WorkQueue::Finished => {
-                    IterNextOutput::Return("Home you're finished, 'cause I am...")
-                }
+                WorkQueue::Finished => IterNextOutput::Return("Finished"),
                 WorkQueue::Result((mapping, id_num)) => {
                     let data = self.data.remove(&id_num).unwrap();
                     IterNextOutput::Yield((mapping, data))
                 }
                 _ => {
                     eprintln!("Received wrong variant as a Result");
-                    IterNextOutput::Return("Home you're finished, 'cause I have exploded...")
+                    IterNextOutput::Return("Wrong variant")
                 }
             },
             Err(RecvError) => {
                 eprintln!("Receiver Error");
-                IterNextOutput::Return("Home you're finished, 'cause I have exploded...")
+                IterNextOutput::Return("Receiver error - channel was closed")
             }
         }
     }
 }
 
 /// Initialise the python module and add the Aligner class.
 #[pymodule]
```

### Comparing `mappy_rs-0.0.3/tests/benchmark.py` & `mappy_rs-0.0.4/tests/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 from pathlib import Path
 
 RESOURCES = (
     Path(__file__).parent.resolve().parent.resolve() / "resources/benchmarking"
 )
 FASTQ_PATH = RESOURCES / "fastq"
-INDEX_PATH = RESOURCES / "index/hg38.mmi"
+INDEX_PATH = RESOURCES / "index/hg38_simple.mmi"
 _FILE_SUFFIXES = set([".fq", ".fastq", ".fastq.gz", ".fq.qz"])
 
 
 def _gen_fastq(path: Path):
     """
     Generator returning fastq records from either a directory fo Fastq or a
     single Fastq file
@@ -38,20 +38,20 @@
 @pytest.fixture
 def mappy_al_rs():
     return mappy_rs.Aligner(str(INDEX_PATH))
 
 
 @pytest.fixture
 def mappy_al():
-    return mp.Aligner(str(INDEX_PATH))
+    yield mp.Aligner(str(INDEX_PATH))
 
 
 @pytest.fixture
 def aligner(request):
-    return request.getfixturevalue(request.param)
+    yield request.getfixturevalue(request.param)
 
 
 def align_multi(al, fasta):
     """
     Parameters
     ----------
     al: mappy_rs.Aligner
@@ -70,19 +70,21 @@
         n += 1
     return n
 
 
 @pytest.mark.parametrize("aligner", ["mappy_al", "mappy_al_rs"], indirect=True)
 def test_classic_mappy(benchmark, aligner, fasta):
     n = benchmark.pedantic(
-        _align, args=(aligner, fasta), iterations=1, rounds=5
+        _align, args=(aligner, fasta), iterations=1, rounds=1
     )
     assert N_READS == n
+    print("Finished classic mappy round")
 
 
 @pytest.mark.parametrize("threads", list(range(1, 6)))
 def test_benchmark_multi(threads, benchmark, mappy_al_rs, fasta):
     mappy_al_rs.enable_threading(threads)
     n = benchmark.pedantic(
-        align_multi, args=(mappy_al_rs, fasta), iterations=1, rounds=5
+        align_multi, args=(mappy_al_rs, fasta), iterations=1, rounds=1
     )
     assert N_READS == n
+    print("Finished threaded mappy round")
```

### Comparing `mappy_rs-0.0.3/tests/python_test.py` & `mappy_rs-0.0.4/tests/python_test.py`

 * *Files identical despite different names*

### Comparing `mappy_rs-0.0.3/Cargo.lock` & `mappy_rs-0.0.4/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,48 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bytelines"
@@ -69,17 +93,17 @@
  "crossbeam-epoch",
  "crossbeam-queue",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -90,22 +114,22 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-queue"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -113,193 +137,216 @@
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "ctrlc"
+version = "3.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a011bbe2c35ce9c1f143b7af6f94f29a167beb4cd1d29e6740ce836f723120e"
+dependencies = [
+ "nix",
+ "windows-sys",
+]
+
+[[package]]
+name = "either"
+version = "1.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+
+[[package]]
 name = "fffx"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7ca98dd80388586fe34f240e19d44ee7e094cf75bdc9bd81ff72d5b5230d52f"
 dependencies = [
  "bytelines",
  "flate2",
  "simdutf8",
  "static_assertions",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "libz-sys",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "futures"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e2792b0ff0340399d58445b88fd9770e3489eff258a4cbc1523418f12abf84"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e5317663a9089767a1ec00a487df42e0ca174b61b4483213ac24448e4664df5"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec90ff4d0fe1f57d600049061dc6bb68ed03c7d2fbd697274c41805dcb3f8608"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8de0a35a6ab97ec8869e32a2473f4b1324459e14c29275d14b10cb1fd19b50e"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfb8371b6fb2aeb2d280374607aeabfc99d95c72edfe51692e42d3d7f0d08531"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95a73af87da33b5acf53acfebdc339fe592ecf5357ac7c0a7734ab9d8c876a70"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f310820bb3e8cfd46c80db4d7fb8353e15dfff853a127158425f31e0be6c8364"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf79a1bf610b10f42aea489289c5a2c478a786509693b80cd39c44ccd936366"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c1d6de3acfef38d2be4b1f543f553131788603495be83da675e180c8d6b7bd1"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
-name = "hermit-abi"
-version = "0.2.6"
+name = "gimli"
+version = "0.27.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libz-sys"
-version = "1.1.8"
+version = "1.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "mappy-rs"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "crossbeam",
+ "ctrlc",
  "fnv",
+ "itertools",
  "libc",
  "minimap2",
  "minimap2-sys",
  "pyo3",
- "threadpool",
 ]
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
@@ -310,193 +357,218 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "minimap2"
-version = "0.1.11"
+name = "memoffset"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acce515adeecaa1ecce83f92fd55dae6d6bbd96731d9c053b2b3a90d1a535e58"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "minimap2"
+version = "0.1.13+minimap2.2.26"
+source = "git+https://github.com/jguhlin/minimap2-rs.git?rev=037abe5#037abe545adb8e05ecd143b4c6d2cb2ecb6dff13"
 dependencies = [
  "bytelines",
  "fffx",
  "flate2",
  "libc",
  "minimap2-sys",
  "simdutf8",
 ]
 
 [[package]]
 name = "minimap2-sys"
-version = "0.1.10"
+version = "0.1.12+minimap2.2.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1f276571c6759045a1f4a4698aec870c40a1c69698edf788f1b439ce9b0483f"
+checksum = "e4797b6c7ddec7f2c15c51ed41324611297d3edff138d73ac1b8611e40298d35"
 dependencies = [
  "cc",
  "libc",
  "libz-sys",
  "pkg-config",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
-name = "num_cpus"
-version = "1.15.0"
+name = "nix"
+version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
 dependencies = [
- "hermit-abi",
+ "bitflags",
+ "cfg-if",
  "libc",
+ "static_assertions",
+]
+
+[[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "simdutf8"
@@ -533,46 +605,47 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.6"
+name = "syn"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
-name = "threadpool"
-version = "1.8.1"
+name = "target-lexicon"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
-dependencies = [
- "num_cpus",
-]
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
- "memchr",
  "pin-project-lite",
- "windows-sys",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -580,70 +653,70 @@
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `mappy_rs-0.0.3/PKG-INFO` & `mappy_rs-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 Metadata-Version: 2.1
 Name: mappy-rs
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest; extra == 'tests'
-Requires-Dist: mappy-rs[tests]; extra == 'dev'
-Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: mappy_rs[dev]; extra == 'benchmark'
 Requires-Dist: pytest-benchmark[histogram]; extra == 'benchmark'
 Requires-Dist: mappy; extra == 'benchmark'
+Requires-Dist: mappy-rs[tests]; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: tests
-Provides-Extra: dev
 Provides-Extra: benchmark
+Provides-Extra: dev
 License-File: LICENSE.MD
 Summary: A multithreaded python wrapper for rust bindings of minimap2.
 Keywords: alignment,bioinformatics,python,rust,minimap2
 Author: Rory Munro <roryjmunro1@gmail.com>
-Author-email: Rory Munro <rory.munro@nottingham.ac.uk>, Aelxander Payne <alexander.payne@nottingham.ac.uk>
+Author-email: Rory Munro <rory.munro@nottingham.ac.uk>, Alexander Payne <alexander.payne@nottingham.ac.uk>
 Maintainer-email: Rory Munro <rory.munro@nottingham.ac.uk>
 License: BSD 3-Clause License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/alexomics/mm2_rs
 
 # Mappy-rs
 [![build](https://github.com/Adoni5/mappy-rs/actions/workflows/CI.yml/badge.svg)](https://github.com/Adoni5/mappy-rs/actions/workflows/CI.yml)
 [![CI](https://github.com/Adoni5/mappy-rs/actions/workflows/check.yml/badge.svg)](https://github.com/Adoni5/mappy-rs/actions/workflows/check.yml)
 
 
-![A map with a crab on it](img/crab_map.webp)
+![A map with a crab on it](https://github.com/Adoni5/mappy-rs/blob/main/img/crab_map.webp)
 
 A multi-threaded minimap2 aligner for python. Built for [readfish](https://github.com/LooseLab/readfish/) compatibility.
 
-Heavily leaning on and inspired by Joeseph Guhlin's minimap2-rs [repository](https://github.com/jguhlin/minimap2-rs). They also have a more heavily featured python client, however this one simply multi threads and maps.
+Heavily leaning on and inspired by Joeseph Guhlin's minimap2-rs [repository](https://github.com/jguhlin/minimap2-rs). They also have a more heavily featured python client, which also provides multithreaded alignment. This client provides a more simple streaming interface for use in pipelines.
 
 `pip install mappy-rs`
 
 ## Developers
 Start with some Docs on Py03 - https://pyo3.rs/latest/
 
 If you wish to contribute, have a look at [CONTRIBUTING.md](.github/CONTRIBUTING.md)
@@ -64,29 +69,29 @@
 Then in your python shell of choice:
 
 ```python
 import mappy_rs
 aligner = mappy_rs.Aligner("resources/test/test.mmi")
 ```
 
-The current iteration of `mappy-rs` serves as a drop in for `mappy`, implementing all the same methods. However if this is the use case, you may well be better off using `mappy`, as the extra level of Rust betwene your python and C++ may well add slighly slower performance.
+The current iteration of `mappy-rs` serves as a drop in for `mappy`, implementing all the same methods. However if this is the use case, you may well be better off using `mappy`, as the extra level of Rust between your python and C++ may well add slightly slower performance.
 
 ### Multithreading
 In order to use multi threading, one must first enable it.
 
 ```python
 import mappy_rs
 aligner = mappy_rs.Aligner("resources/test/test.mmi")
 # Use 10 threads
 aligner.enable_threading(10)
 ```
 
 Enabling threading makes the `map_batch` method available.
 This method requires a list or iterable of dictionaries, which can have any number of keys and depth, but **must** contain the key `seq` with a string value in the top-level dictionary.
-Currently, the maximum batch size tobe iterated in one call is 20000.
+Currently, the maximum batch size to be iterated in one call is 20000.
 
 For example:
 
 ```python
 import mappy_rs
 aligner = mappy_rs.Aligner("resources/test/test.mmi")
 aligner.enable_threading(10)
```

