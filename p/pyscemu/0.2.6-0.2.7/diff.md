# Comparing `tmp/pyscemu-0.2.6.tar.gz` & `tmp/pyscemu-0.2.7.tar.gz`

## Comparing `pyscemu-0.2.6.tar` & `pyscemu-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.6/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.6/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.6/.gitignore
--rw-r--r--   0     1000     1000    11699 2023-05-10 08:42:26.000000 pyscemu-0.2.6/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.6/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.6/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.6/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.6/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.6/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.6/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.6/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.6/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.6/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.6/pyproject.toml
--rw-r--r--   0     1000     1000    26649 2023-06-21 15:56:51.000000 pyscemu-0.2.6/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-06-22 08:41:07.000000 pyscemu-0.2.6/Cargo.lock
--rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.7/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.7/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.7/.gitignore
+-rw-r--r--   0     1000     1000    11773 2023-07-03 19:42:43.000000 pyscemu-0.2.7/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.7/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.7/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.7/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.7/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.7/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.7/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.7/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.7/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.7/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.7/pyproject.toml
+-rw-r--r--   0     1000     1000    26776 2023-07-03 19:39:30.000000 pyscemu-0.2.7/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-07-03 20:01:07.000000 pyscemu-0.2.7/Cargo.lock
+-rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.7/PKG-INFO
```

### Comparing `pyscemu-0.2.6/.github/workflows/CI.yml` & `pyscemu-0.2.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/.gitignore` & `pyscemu-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/DOCUMENTATION.md` & `pyscemu-0.2.7/DOCUMENTATION.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
     # It is necessary to load the 32bits or 64bits maps folder for having a realistic memory layout.
     # The maps can be downloaded from the https://github.com/sha0coder/scemu
 emu.load_maps(folder:str)
 
     # Load the binary to be emulated.
 emu.load_binary(filename:str)
+    # Load the bytes to be emulated.
+emu.load_code_bytes(bytes:bytearray)
 ```
 
 optionally is possible to change entry point and base address
 
 ```python
 
     # change the default entry point.
```

### Comparing `pyscemu-0.2.6/README.md` & `pyscemu-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/examples/danabot_rsa.ipynb` & `pyscemu-0.2.7/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/examples/raccoon_strings.ipynb` & `pyscemu-0.2.7/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/examples/scripts/raccoon_strings.py` & `pyscemu-0.2.7/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/examples/scripts/test.py` & `pyscemu-0.2.7/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/examples/scripts/xloader_dexor.py` & `pyscemu-0.2.7/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/examples/xloader_keygen.ipynb` & `pyscemu-0.2.7/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.6/src/lib.rs` & `pyscemu-0.2.7/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,19 @@
     }
 
     /// Load the binary to be emulated.
     fn load_binary(&mut self, filename: &str) {
         self.emu.load_code(filename);
     }
 
+    /// Load code from bytes
+    fn load_code_bytes(&mut self, bytes: &[u8]) {
+        self.emu.load_code_bytes(bytes);
+    }
+
     /// allocate a buffer on the emulated process address space.  
     fn alloc(&mut self, name:&str, size:u64) -> PyResult<u64> {
         return Ok(self.emu.alloc(name, size));
     }
 
 
     /// push a 32bits value to the stack.
```

### Comparing `pyscemu-0.2.6/Cargo.lock` & `pyscemu-0.2.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7884c09bc473386eec552c11d73d4420363e7dac4023ecfd19b7e878efa31c18"
+checksum = "8eedf686dbb13ada4843b35ab8590fff629c2823e6c30bd22a8b35ef5bc8c24c"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.2.6"
+version = "0.2.7"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.2.6/PKG-INFO` & `pyscemu-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.2.6
+Version: 0.2.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

