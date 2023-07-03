# Comparing `tmp/ra2mix-0.0.5.tar.gz` & `tmp/ra2mix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ra2mix-0.0.5.tar", last modified: Sun Jul  2 15:59:02 2023, max compression
+gzip compressed data, was "ra2mix-0.0.6.tar", last modified: Mon Jul  3 01:04:28 2023, max compression
```

## Comparing `ra2mix-0.0.5.tar` & `ra2mix-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:59:02.267485 ra2mix-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 15:58:53.000000 ra2mix-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 15:59:02.267485 ra2mix-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 15:58:53.000000 ra2mix-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 15:58:53.000000 ra2mix-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:59:02.267485 ra2mix-0.0.5/ra2mix/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 15:58:53.000000 ra2mix-0.0.5/ra2mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 15:58:53.000000 ra2mix-0.0.5/ra2mix/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-02 15:58:53.000000 ra2mix-0.0.5/ra2mix/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-02 15:58:53.000000 ra2mix-0.0.5/ra2mix/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-02 15:58:53.000000 ra2mix-0.0.5/ra2mix/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:59:02.267485 ra2mix-0.0.5/ra2mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 15:59:02.000000 ra2mix-0.0.5/ra2mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-02 15:59:02.000000 ra2mix-0.0.5/ra2mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:59:02.000000 ra2mix-0.0.5/ra2mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-02 15:59:02.000000 ra2mix-0.0.5/ra2mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 15:59:02.000000 ra2mix-0.0.5/ra2mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:59:02.267485 ra2mix-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:04:28.823609 ra2mix-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 01:04:19.000000 ra2mix-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 01:04:28.823609 ra2mix-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-03 01:04:19.000000 ra2mix-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 01:04:19.000000 ra2mix-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:04:28.823609 ra2mix-0.0.6/ra2mix/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:04:28.823609 ra2mix-0.0.6/ra2mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:04:28.823609 ra2mix-0.0.6/setup.cfg
```

### Comparing `ra2mix-0.0.5/LICENSE` & `ra2mix-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.5/PKG-INFO` & `ra2mix-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra2mix
-Version: 0.0.5
+Version: 0.0.6
 Summary: ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files
 Author-email: nyte_owl <nyteowldev@gmail.com>
 Project-URL: Homepage, https://github.com/endless-creation/ra2mix
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ra2mix-0.0.5/pyproject.toml` & `ra2mix-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "ra2mix"
 authors = [
     {name = "nyte_owl", email = "nyteowldev@gmail.com"}
 ]
 description = "ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
     "crc"
 ]
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `ra2mix-0.0.5/ra2mix/checksum.py` & `ra2mix-0.0.6/ra2mix/checksum.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import struct
+
 from crc import Calculator, Crc32
 
 
 def obfuscate_filename(filename: str) -> str:
     filename_length = len(filename)
     obfuscated_name = filename.upper()
     salt = filename_length & 0xFFFFFFFC
@@ -12,8 +14,13 @@
             obfuscated_name += obfuscated_name[salt]
     return obfuscated_name
 
 
 def ra2_crc(filename: str) -> int:
     obfuscated_name = obfuscate_filename(filename)
     binary_data = obfuscated_name.encode()
-    return Calculator(Crc32.CRC32).checksum(binary_data)
+    crc = Calculator(Crc32.CRC32).checksum(binary_data)
+
+    # CRC must be interpreted as a 32-bit signed integer for proper sorting
+    # in mix file header/body
+    (signed_crc,) = struct.unpack("=i", struct.pack("=I", crc))
+    return signed_crc
```

### Comparing `ra2mix-0.0.5/ra2mix/reader.py` & `ra2mix-0.0.6/ra2mix/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 def get_file_entries(header: Header, mix_data: bytes) -> list[FileEntry]:
     file_entries = []
     for i in range(header.file_count):
         start = 10 + (i * const.FILE_ENTRY_SIZE)
         end = start + const.FILE_ENTRY_SIZE
         # print(binascii.b2a_hex(mix_data[start:end], ":"))
 
-        # ID is unpacked as an unsigned integer because the CRC computer creates
-        # unsigned integers; they need to match for comparison sake
-        file_entries.append(FileEntry._make(struct.unpack("=3I", mix_data[start:end])))
+        file_entries.append(FileEntry._make(struct.unpack("=iII", mix_data[start:end])))
 
     return file_entries
 
 
 def get_filenames_from_mix_db(mix_db_file_data: bytes) -> list[str]:
     filenames = []
     end = (start := const.XCC_HEADER_SIZE)
@@ -44,40 +42,46 @@
 
 def get_file_map(file_entries: list[FileEntry], mix_data: bytes):
     if len(file_entries) == 1:
         return {}
 
     MIX_DB_ID = ra2_crc(const.MIX_DB_FILENAME)
 
-    BODY_START = const.HEADER_SIZE + (const.FILE_ENTRY_SIZE * len(file_entries))
+    body_start = const.HEADER_SIZE + (const.FILE_ENTRY_SIZE * len(file_entries))
     for file_entry in file_entries:
         if file_entry.id != MIX_DB_ID:
             continue
         mix_db_file_entry = file_entry
         break
 
-    mix_body_data = mix_data[BODY_START:]
+    mix_body_data = mix_data[body_start:]
     mix_db_file_data = get_file_data_from_mix_body(mix_db_file_entry, mix_body_data)
 
     filenames = get_filenames_from_mix_db(mix_db_file_data)
     filename_id_map = {ra2_crc(filename): filename for filename in filenames}
     # print(f"{filename_id_map=}")
 
     filemap = {}
     for file_entry in file_entries:
         file_data = get_file_data_from_mix_body(file_entry, mix_body_data)
         filemap[filename_id_map[file_entry.id]] = file_data
 
     return filemap
 
 
-def read(mix_filepath: str) -> dict[str, bytes]:
+def read_file_info(mix_filepath: str) -> Header:
     with open(mix_filepath, "rb") as fp:
         mix_data = fp.read()
 
     header = Header._make(struct.unpack("=I H I", mix_data[: const.HEADER_SIZE]))
     if (header.flags & 2) != 0:
         raise NotImplementedError("Cannot parse encrypted mix header")
 
     file_entries = get_file_entries(header, mix_data)
 
+    return header, file_entries, mix_data
+
+
+def read(mix_filepath: str) -> dict[str, bytes]:
+    _, file_entries, mix_data = read_file_info(mix_filepath)
+
     return get_file_map(file_entries, mix_data)
```

### Comparing `ra2mix-0.0.5/ra2mix/writer.py` & `ra2mix-0.0.6/ra2mix/writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 def get_mix_db_data(filenames: list[str], game: const.XCCGame):
     num_files = len(filenames)
     db_size_in_bytes = (
         const.XCC_HEADER_SIZE
         + sum([len(filename) for filename in filenames])
         + num_files
     )
-    print(db_size_in_bytes)
 
     bytes_data = struct.pack("=32s", const.XCC_ID_BYTES) + struct.pack(
         "=5I",
         db_size_in_bytes,
         const.XCC_FILE_TYPE,
         const.XCC_FILE_VERSION,
         game.value,
@@ -56,29 +55,32 @@
 
         file_map = {}
         for path in paths:
             file_map[path.name] = path.read_bytes()
 
     filenames = list(file_map.keys())
     filenames.append(const.MIX_DB_FILENAME)
-    print(filenames)
 
     db_data = get_mix_db_data(filenames, game)
 
     file_map[const.MIX_DB_FILENAME] = db_data
 
-    return file_map
+    filetypes = {}
+    for filename in file_map.keys():
+        filetype = filename.split(".")[-1]
+        if filetype in filetypes:
+            filetypes[filetype] = filetypes[filetype] + 1
+        else:
+            filetypes[filetype] = 1
 
+    print("The following files will be written to the .mix file:")
+    for filetype, count in filetypes.items():
+        print(f"\t*.{filetype}: {count}")
 
-def packed_id(filename: str):
-    crc = ra2_crc(filename)
-    # CRC must be interpreted as a 32-bit signed integer for proper sorting
-    # in mix file header/body
-    (pid,) = struct.unpack("=i", struct.pack("=I", crc))
-    return pid
+    return file_map
 
 
 class FileInfo(TypedDict):
     file_id: int
     data: bytes
 
 
@@ -101,34 +103,34 @@
     file_map: dict[str, bytes] | None = None,
     folder_path: str | None = None,
     filepaths: list[str] | None = None,
 ) -> bytes:
     file_map = coalesce_input_files(game, file_map, folder_path, filepaths)
 
     file_information_list = [
-        FileInfo(file_id=packed_id(filename), data=data)
+        FileInfo(file_id=ra2_crc(filename), data=data)
         for filename, data in file_map.items()
     ]
     sorted_file_info_list = sorted(
         file_information_list, key=lambda file_info: file_info["file_id"]
     )
 
-    print(f"Sorted file info: {sorted_file_info_list}")
-
     offset = 0
     file_entry_data = b""
     body_data = b""
+    print("Generating .mix data")
     for file_info in sorted_file_info_list:
         size = len(file_info["data"])
 
         file_entry_data += struct.pack("=iII", file_info["file_id"], offset, size)
         body_data += file_info["data"]
 
         offset += size
 
     mix_data = create_mix_header(file_map) + file_entry_data + body_data
 
     if mix_filepath is not None:
+        print(f"Writing mix data to file {mix_filepath}")
         with open(mix_filepath, "wb") as fp:
             fp.write(mix_data)
 
     return mix_data
```

### Comparing `ra2mix-0.0.5/ra2mix.egg-info/PKG-INFO` & `ra2mix-0.0.6/ra2mix.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra2mix
-Version: 0.0.5
+Version: 0.0.6
 Summary: ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files
 Author-email: nyte_owl <nyteowldev@gmail.com>
 Project-URL: Homepage, https://github.com/endless-creation/ra2mix
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

