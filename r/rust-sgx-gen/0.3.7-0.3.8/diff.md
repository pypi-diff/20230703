# Comparing `tmp/rust-sgx-gen-0.3.7.tar.gz` & `tmp/rust-sgx-gen-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rust-sgx-gen-0.3.7.tar", last modified: Mon Jan 16 15:07:35 2023, max compression
+gzip compressed data, was "rust-sgx-gen-0.3.8.tar", last modified: Mon Jul  3 12:58:28 2023, max compression
```

## Comparing `rust-sgx-gen-0.3.7.tar` & `rust-sgx-gen-0.3.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 15:07:35.818962 rust-sgx-gen-0.3.7/
--rw-r--r--   0 root         (0) root         (0)     1076 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       37 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6966 2023-01-16 15:07:35.818962 rust-sgx-gen-0.3.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5339 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 15:07:35.814962 rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6966 2023-01-16 15:07:35.000000 rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-01-16 15:07:35.000000 rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-16 15:07:35.000000 rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-01-16 15:07:35.000000 rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-16 15:07:35.000000 rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-16 15:07:35.000000 rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 15:07:35.814962 rust-sgx-gen-0.3.7/rustsgxgen/
--rw-r--r--   0 root         (0) root         (0)       59 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/conf.py
--rw-r--r--   0 root         (0) root         (0)     5861 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/generator.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/initialization.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 15:07:35.814962 rust-sgx-gen-0.3.7/rustsgxgen/stubs/
--rw-r--r--   0 root         (0) root         (0)     2865 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/README.md
--rw-r--r--   0 root         (0) root         (0)    20096 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/__authentic_execution.rs
--rw-r--r--   0 root         (0) root         (0)      293 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/common_deps.toml
--rw-r--r--   0 root         (0) root         (0)     1272 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/constants.rs
--rw-r--r--   0 root         (0) root         (0)       93 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/main.rs
--rw-r--r--   0 root         (0) root         (0)      360 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/mods_uses.rs
--rw-r--r--   0 root         (0) root         (0)      117 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/output.rs
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/request.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 15:07:35.814962 rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_native/
--rw-r--r--   0 root         (0) root         (0)     1783 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_native/__run.rs
--rw-r--r--   0 root         (0) root         (0)       25 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_native/dependencies.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 15:07:35.814962 rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_sgx/
--rw-r--r--   0 root         (0) root         (0)     2796 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_sgx/__run.rs
--rw-r--r--   0 root         (0) root         (0)      325 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_sgx/dependencies.toml
--rw-r--r--   0 root         (0) root         (0)     4541 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/rustsgxgen/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-16 15:07:35.818962 rust-sgx-gen-0.3.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      956 2023-01-16 15:05:47.000000 rust-sgx-gen-0.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:58:28.174106 rust-sgx-gen-0.3.8/
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-07-03 12:58:28.174106 rust-sgx-gen-0.3.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:58:28.170106 rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-07-03 12:58:28.000000 rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-03 12:58:28.000000 rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:58:28.000000 rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-03 12:58:28.000000 rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 12:58:28.000000 rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-03 12:58:28.000000 rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:58:28.170106 rust-sgx-gen-0.3.8/rustsgxgen/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5861 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/generator.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/initialization.py
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:58:28.174106 rust-sgx-gen-0.3.8/rustsgxgen/stubs/
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/README.md
+-rw-r--r--   0 root         (0) root         (0)    20130 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/__authentic_execution.rs
+-rw-r--r--   0 root         (0) root         (0)      293 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/common_deps.toml
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/constants.rs
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/main.rs
+-rw-r--r--   0 root         (0) root         (0)      360 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/mods_uses.rs
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/output.rs
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/request.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:58:28.174106 rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_native/
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_native/__run.rs
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_native/dependencies.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:58:28.174106 rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_sgx/
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_sgx/__run.rs
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_sgx/dependencies.toml
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/rustsgxgen/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:58:28.174106 rust-sgx-gen-0.3.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-03 12:56:29.000000 rust-sgx-gen-0.3.8/setup.py
```

### Comparing `rust-sgx-gen-0.3.7/LICENSE` & `rust-sgx-gen-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/PKG-INFO` & `rust-sgx-gen-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rust-sgx-gen
-Version: 0.3.7
+Version: 0.3.8
 Summary: Rust code generator for the Authentic Execution framework
 Home-page: https://github.com/AuthenticExecution/rust-sgx-gen
 Author: Gianluca Scopelliti
 Author-email: gianlu.1033@gmail.com
 License: UNKNOWN
 Description: # rust-sgx-gen
```

### Comparing `rust-sgx-gen-0.3.7/README.md` & `rust-sgx-gen-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/PKG-INFO` & `rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rust-sgx-gen
-Version: 0.3.7
+Version: 0.3.8
 Summary: Rust code generator for the Authentic Execution framework
 Home-page: https://github.com/AuthenticExecution/rust-sgx-gen
 Author: Gianluca Scopelliti
 Author-email: gianlu.1033@gmail.com
 License: UNKNOWN
 Description: # rust-sgx-gen
```

### Comparing `rust-sgx-gen-0.3.7/rust_sgx_gen.egg-info/SOURCES.txt` & `rust-sgx-gen-0.3.8/rust_sgx_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/conf.py` & `rust-sgx-gen-0.3.8/rustsgxgen/conf.py`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/generator.py` & `rust-sgx-gen-0.3.8/rustsgxgen/generator.py`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/initialization.py` & `rust-sgx-gen-0.3.8/rustsgxgen/initialization.py`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/runner.py` & `rust-sgx-gen-0.3.8/rustsgxgen/runner.py`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/stubs/README.md` & `rust-sgx-gen-0.3.8/rustsgxgen/stubs/README.md`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/stubs/__authentic_execution.rs` & `rust-sgx-gen-0.3.8/rustsgxgen/stubs/__authentic_execution.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 pub mod authentic_execution {
     extern crate base64;
     extern crate reactive_crypto;
     extern crate reactive_net;
+    extern crate sgx_attestation;
 
     use std::collections::{HashMap, HashSet};
     use std::sync::Mutex;
     use std::net::TcpStream;
 
     use reactive_net::{ResultCode, CommandCode, ResultMessage, CommandMessage, EntrypointID};
     use reactive_crypto::Encryption;
```

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/stubs/constants.rs` & `rust-sgx-gen-0.3.8/rustsgxgen/stubs/constants.rs`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_native/__run.rs` & `rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_native/__run.rs`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/stubs/runner_sgx/__run.rs` & `rust-sgx-gen-0.3.8/rustsgxgen/stubs/runner_sgx/__run.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 use std::net::{TcpListener, TcpStream};
 use crate::{debug, info, error};
 use crate::__authentic_execution::authentic_execution::{MODULE_NAME, EM_PORT, MODULE_ID, NUM_THREADS, handle_entrypoint};
 extern crate base64;
 use threadpool::ThreadPool;
 
-use ra_enclave::EnclaveRaContext;
-
 lazy_static! {
     pub static ref MODULE_KEY: String = remote_attestation().unwrap();
     pub static ref SP_VKEY_PEM: &'static str = "__SP_VKEY_PEM__";
 }
 
 
 fn handle_client(mut stream: TcpStream) {
@@ -27,41 +25,27 @@
         error!("{}", e);
     }
 }
 
 
 fn remote_attestation() -> std::io::Result<String> {
     info!("Waiting for attestation");
-
     let port = *EM_PORT + *MODULE_ID;
-    let listener = TcpListener::bind(("0.0.0.0", port))?;
-
-    let mut stream = listener.accept()?.0;
-
-    debug!("Connected to ra_client");
-    let context = match EnclaveRaContext::init(*SP_VKEY_PEM) {
-        Ok(c) => c,
-        Err(e) => {
-            error!("{:?}", e);
-            panic!("{:?}", e);
-        }
-    };
 
-    debug!("Starting attestation process");
-    let result = match context.do_attestation(&mut stream) {
+    let result = match sgx_attestation::do_attestation(port, *SP_VKEY_PEM) {
         Ok(r) => r,
         Err(e) => {
             error!("{:?}", e);
             panic!("{:?}", e);
         }
     };
 
     info!("Remote attestation succeeded");
 
-    Ok(base64::encode(&result.1))
+    Ok(base64::encode(&result))
 }
 
 fn run_single_thread(listener : TcpListener) {
     for stream in listener.incoming() {
         //debug!("Received connection");
         match stream {
             Ok(s)   => handle_client(s),
```

### Comparing `rust-sgx-gen-0.3.7/rustsgxgen/utils.py` & `rust-sgx-gen-0.3.8/rustsgxgen/utils.py`

 * *Files identical despite different names*

### Comparing `rust-sgx-gen-0.3.7/setup.py` & `rust-sgx-gen-0.3.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name="rust-sgx-gen",
-    version="0.3.7",
+    version="0.3.8",
     author="Gianluca Scopelliti",
     author_email="gianlu.1033@gmail.com",
     description="Rust code generator for the Authentic Execution framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AuthenticExecution/rust-sgx-gen",
     packages=setuptools.find_packages(),
```

