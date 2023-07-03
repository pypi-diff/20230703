# Comparing `tmp/neuromorphic_drivers-0.2.1.tar.gz` & `tmp/neuromorphic_drivers-0.2.2.tar.gz`

## Comparing `neuromorphic_drivers-0.2.1.tar` & `neuromorphic_drivers-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/Cargo.toml
--rw-r--r--   0     1001      123    18887 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/de.rs
--rw-r--r--   0     1001      123     5021 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/error.rs
--rw-r--r--   0     1001      123    25754 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/format.rs
--rw-r--r--   0     1001      123    14340 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/lib.rs
--rw-r--r--   0     1001      123    14435 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/ser.rs
--rw-r--r--   0     1001      123    11374 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/trace.rs
--rw-r--r--   0     1001      123    10825 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/value.rs
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123       41 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/.gitignore
--rw-r--r--   0     1001      123     1102 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/LICENSE
--rw-r--r--   0     1001      123      115 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/README.md
--rw-r--r--   0     1001      123    34780 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/build.rs
--rw-r--r--   0     1001      123     1031 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123     2765 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/__init__.py
--rw-r--r--   0     1001      123      802 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/device.py
--rw-r--r--   0     1001      123     5781 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
--rw-r--r--   0     1001      123     6143 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
--rw-r--r--   0     1001      123     8269 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices_types.py
--rw-r--r--   0     1001      123      400 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/enums.py
--rw-r--r--   0     1001      123      701 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/unions.py
--rw-r--r--   0     1001      123     4481 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/mask.py
--rw-r--r--   0     1001      123       91 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/__init__.py
--rw-r--r--   0     1001      123    15358 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/binary.py
--rw-r--r--   0     1001      123     2296 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/bincode.py
--rw-r--r--   0     1001      123     1547 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/type.py
--rw-r--r--   0     1001      123     1091 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/status.py
--rw-r--r--   0     1001      123     1858 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/udev.py
--rw-r--r--   0     1001      123     4497 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/adapters.rs
--rw-r--r--   0     1001      123     1675 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/bytes.rs
--rw-r--r--   0     1001      123    14237 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123     4091 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/structured_array.rs
--rw-r--r--   0     1001      123     6177 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/display.py
--rw-r--r--   0     1001      123     1961 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/external_synchronization.py
--rw-r--r--   0     1001      123      608 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/read_many.py
--rw-r--r--   0     1001      123      687 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/record_raw.py
--rw-r--r--   0     1001      123      336 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/test.py
--rw-r--r--   0     1001      123    19206 2023-07-02 23:56:13.000000 neuromorphic_drivers-0.2.1/Cargo.lock
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/Cargo.toml
+-rw-r--r--   0     1001      123    18887 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/de.rs
+-rw-r--r--   0     1001      123     5021 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/error.rs
+-rw-r--r--   0     1001      123    25754 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/format.rs
+-rw-r--r--   0     1001      123    14340 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/lib.rs
+-rw-r--r--   0     1001      123    14435 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/ser.rs
+-rw-r--r--   0     1001      123    11374 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/trace.rs
+-rw-r--r--   0     1001      123    10825 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/value.rs
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123       41 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/.gitignore
+-rw-r--r--   0     1001      123     1102 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/LICENSE
+-rw-r--r--   0     1001      123      115 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/README.md
+-rw-r--r--   0     1001      123    35531 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/build.rs
+-rw-r--r--   0     1001      123     1031 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123     2765 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/__init__.py
+-rw-r--r--   0     1001      123      802 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/device.py
+-rw-r--r--   0     1001      123     5781 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
+-rw-r--r--   0     1001      123     6143 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
+-rw-r--r--   0     1001      123     8269 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices_types.py
+-rw-r--r--   0     1001      123      400 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/enums.py
+-rw-r--r--   0     1001      123      701 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/unions.py
+-rw-r--r--   0     1001      123     4481 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/mask.py
+-rw-r--r--   0     1001      123       91 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/__init__.py
+-rw-r--r--   0     1001      123    15358 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/binary.py
+-rw-r--r--   0     1001      123     2296 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/bincode.py
+-rw-r--r--   0     1001      123     1547 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/type.py
+-rw-r--r--   0     1001      123     1091 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/status.py
+-rw-r--r--   0     1001      123     1858 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/udev.py
+-rw-r--r--   0     1001      123     4497 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/adapters.rs
+-rw-r--r--   0     1001      123     1675 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/bytes.rs
+-rw-r--r--   0     1001      123    14237 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123     4091 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/structured_array.rs
+-rw-r--r--   0     1001      123     6177 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/display.py
+-rw-r--r--   0     1001      123     1961 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/external_synchronization.py
+-rw-r--r--   0     1001      123      608 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/read_many.py
+-rw-r--r--   0     1001      123      687 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/record_raw.py
+-rw-r--r--   0     1001      123      336 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/test.py
+-rw-r--r--   0     1001      123    19206 2023-07-03 07:28:04.000000 neuromorphic_drivers-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.2/PKG-INFO
```

### Comparing `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/de.rs` & `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/de.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/error.rs` & `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/error.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/format.rs` & `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/format.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/lib.rs` & `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/lib.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/ser.rs` & `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/ser.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/trace.rs` & `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/trace.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/value.rs` & `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/value.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/LICENSE` & `neuromorphic_drivers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/build.rs` & `neuromorphic_drivers-0.2.2/build.rs`

 * *Files 1% similar despite different names*

```diff
@@ -795,10 +795,34 @@
                     "    )",
                 ),
             ).unwrap();
         }
     };
 }
 
+fn macos_link_search_path() -> Option<String> {
+    let output = cc::Build::new()
+        .get_compiler()
+        .to_command()
+        .arg("--print-search-dirs")
+        .output()
+        .unwrap();
+    for line in String::from_utf8_lossy(&output.stdout).lines() {
+        if line.contains("libraries: =") {
+            let path = line.split('=').nth(1).unwrap();
+            if !path.is_empty() {
+                return Some(format!("{}/lib/darwin", path));
+            }
+        }
+    }
+    None
+}
+
 fn main() {
+    if std::env::var("TARGET").unwrap().contains("apple") {
+        if let Some(path) = macos_link_search_path() {
+            println!("cargo:rustc-link-lib=clang_rt.osx");
+            println!("cargo:rustc-link-search={}", path);
+        }
+    }
     generate!(prophesee_evk3_hd, prophesee_evk4);
 }
```

### Comparing `neuromorphic_drivers-0.2.1/pyproject.toml` & `neuromorphic_drivers-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Neuromorphic devices drivers"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "International Centre for Neuromorphic Systems"},
     {name = "Alexandre Marcireau"},
 ]
-version = "0.2.1"
+version = "0.2.2"
 requires-python = ">=3.8"
 dependencies = ["numpy>=1.24"]
 
 [project.urls]
 homepage = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 repository = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 documentation = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
```

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/__init__.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/device.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/device.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices_types.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices_types.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/unions.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/unions.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/mask.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/mask.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/binary.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/binary.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/bincode.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/bincode.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/type.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/type.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/status.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/status.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/udev.py` & `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/udev.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/src/adapters.rs` & `neuromorphic_drivers-0.2.2/src/adapters.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/src/bytes.rs` & `neuromorphic_drivers-0.2.2/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/src/lib.rs` & `neuromorphic_drivers-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/src/structured_array.rs` & `neuromorphic_drivers-0.2.2/src/structured_array.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/tests/display.py` & `neuromorphic_drivers-0.2.2/tests/display.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/tests/external_synchronization.py` & `neuromorphic_drivers-0.2.2/tests/external_synchronization.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/tests/read_many.py` & `neuromorphic_drivers-0.2.2/tests/read_many.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/tests/record_raw.py` & `neuromorphic_drivers-0.2.2/tests/record_raw.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.1/Cargo.lock` & `neuromorphic_drivers-0.2.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -95,17 +95,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "c0aa48fab2893d8a49caa94082ae8488f4e1050d73b367881dcd2198f4199fd8"
 
 [[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
@@ -410,15 +410,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "python"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "bincode",
  "cc",
  "neuromorphic-drivers 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "numpy",
  "paste",
  "pyo3",
```

### Comparing `neuromorphic_drivers-0.2.1/PKG-INFO` & `neuromorphic_drivers-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromorphic_drivers
-Version: 0.2.1
+Version: 0.2.2
 Requires-Dist: numpy >=1.24
 License-File: LICENSE
 Summary: Neuromorphic devices drivers
 Author: International Centre for Neuromorphic Systems, Alexandre Marcireau
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/neuromorphicsystems/neuromorphic-rs/
```

