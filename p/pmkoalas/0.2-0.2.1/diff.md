# Comparing `tmp/pmkoalas-0.2.tar.gz` & `tmp/pmkoalas-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmkoalas-0.2.tar", last modified: Thu Jun 22 03:23:17 2023, max compression
+gzip compressed data, was "pmkoalas-0.2.1.tar", last modified: Mon Jul  3 01:32:14 2023, max compression
```

## Comparing `pmkoalas-0.2.tar` & `pmkoalas-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.334381 pmkoalas-0.2/
--rw-rw-rw-   0        0        0     1095 2022-10-22 22:45:35.000000 pmkoalas-0.2/LICENSE
--rw-rw-rw-   0        0        0     4040 2023-06-22 03:23:17.333383 pmkoalas-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2132 2023-06-22 02:19:40.000000 pmkoalas-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.310191 pmkoalas-0.2/pmkoalas/
--rw-rw-rw-   0        0        0       19 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/__init__.py
--rw-rw-rw-   0        0        0     2705 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/_logging.py
--rw-rw-rw-   0        0        0    11208 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/complex.py
--rw-rw-rw-   0        0        0    17693 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/directly.py
--rw-rw-rw-   0        0        0      706 2023-06-22 03:18:45.000000 pmkoalas-0.2/pmkoalas/dtlog.py
--rw-rw-rw-   0        0        0        0 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/eventlog.py
--rw-rw-rw-   0        0        0     9574 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/export.py
--rw-rw-rw-   0        0        0    10090 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/read.py
--rw-rw-rw-   0        0        0     9240 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/simple.py
--rw-rw-rw-   0        0        0        0 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/work.py
--rw-rw-rw-   0        0        0      192 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/xes.py
--rw-rw-rw-   0        0        0     5221 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/xes_export.py
-drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.326193 pmkoalas-0.2/pmkoalas.egg-info/
--rw-rw-rw-   0        0        0     4040 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      874 2023-06-22 02:19:40.000000 pmkoalas-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 03:23:17.334381 pmkoalas-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.332381 pmkoalas-0.2/tests/
--rw-rw-rw-   0        0        0     3819 2023-06-22 02:26:48.000000 pmkoalas-0.2/tests/test_drelations.py
--rw-rw-rw-   0        0        0     1214 2023-06-22 03:18:45.000000 pmkoalas-0.2/tests/test_dtlog.py
--rw-rw-rw-   0        0        0     3260 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_export_complex.py
--rw-rw-rw-   0        0        0     2278 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_export_simple.py
--rw-rw-rw-   0        0        0     4079 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_read_complex.py
--rw-rw-rw-   0        0        0     1976 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_read_simple.py
--rw-rw-rw-   0        0        0     1577 2023-06-22 02:25:48.000000 pmkoalas-0.2/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:32:14.974150 pmkoalas-0.2.1/
+-rw-rw-rw-   0        0        0     1094 2022-08-18 07:14:37.000000 pmkoalas-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4039 2023-07-03 01:32:14.973153 pmkoalas-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2129 2023-07-03 00:42:02.000000 pmkoalas-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 01:32:14.940240 pmkoalas-0.2.1/pmkoalas/
+-rw-rw-rw-   0        0        0       21 2023-07-03 01:31:50.000000 pmkoalas-0.2.1/pmkoalas/__init__.py
+-rw-rw-rw-   0        0        0     2705 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/_logging.py
+-rw-rw-rw-   0        0        0    11208 2023-07-03 01:29:05.000000 pmkoalas-0.2.1/pmkoalas/complex.py
+-rw-rw-rw-   0        0        0    17693 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/directly.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:32:14.951212 pmkoalas-0.2.1/pmkoalas/discovery/
+-rw-rw-rw-   0        0        0        0 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/discovery/__init__.py
+-rw-rw-rw-   0        0        0    17624 2023-07-03 00:42:02.000000 pmkoalas-0.2.1/pmkoalas/discovery/alpha_miner.py
+-rw-rw-rw-   0        0        0      706 2023-07-03 00:41:52.000000 pmkoalas-0.2.1/pmkoalas/dtlog.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/eventlog.py
+-rw-rw-rw-   0        0        0     9574 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/export.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:32:14.957195 pmkoalas-0.2.1/pmkoalas/models/
+-rw-rw-rw-   0        0        0      784 2023-07-03 00:42:02.000000 pmkoalas-0.2.1/pmkoalas/models/dotutil.py
+-rw-rw-rw-   0        0        0    15224 2023-07-03 00:42:02.000000 pmkoalas-0.2.1/pmkoalas/models/petrinet.py
+-rw-rw-rw-   0        0        0    12758 2023-07-03 00:42:02.000000 pmkoalas-0.2.1/pmkoalas/models/pnfrag.py
+-rw-rw-rw-   0        0        0    10090 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/read.py
+-rw-rw-rw-   0        0        0     9240 2023-07-03 01:29:05.000000 pmkoalas-0.2.1/pmkoalas/simple.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/work.py
+-rw-rw-rw-   0        0        0      192 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/xes.py
+-rw-rw-rw-   0        0        0     5221 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/pmkoalas/xes_export.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:32:14.948219 pmkoalas-0.2.1/pmkoalas.egg-info/
+-rw-rw-rw-   0        0        0     4039 2023-07-03 01:32:14.000000 pmkoalas-0.2.1/pmkoalas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-07-03 01:32:14.000000 pmkoalas-0.2.1/pmkoalas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 01:32:14.000000 pmkoalas-0.2.1/pmkoalas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-03 01:32:14.000000 pmkoalas-0.2.1/pmkoalas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 01:32:14.000000 pmkoalas-0.2.1/pmkoalas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      919 2023-07-03 01:31:57.000000 pmkoalas-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 01:32:14.974150 pmkoalas-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 01:32:14.971157 pmkoalas-0.2.1/tests/
+-rw-rw-rw-   0        0        0     3819 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/tests/test_drelations.py
+-rw-rw-rw-   0        0        0     1214 2023-07-03 00:41:52.000000 pmkoalas-0.2.1/tests/test_dtlog.py
+-rw-rw-rw-   0        0        0     3260 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/tests/test_export_complex.py
+-rw-rw-rw-   0        0        0     2278 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/tests/test_export_simple.py
+-rw-rw-rw-   0        0        0     4079 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/tests/test_read_complex.py
+-rw-rw-rw-   0        0        0     1976 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/tests/test_read_simple.py
+-rw-rw-rw-   0        0        0     1577 2023-06-23 00:51:54.000000 pmkoalas-0.2.1/tests/test_simple.py
```

### Comparing `pmkoalas-0.2/LICENSE` & `pmkoalas-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `pmkoalas-0.2/PKG-INFO` & `pmkoalas-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmkoalas
-Version: 0.2
+Version: 0.2.1
 Summary: A process mining library that focuses on providing pythonic interactions with event logs and languages.
 Author: Adam Burke
 Author-email: Adam Banham <adam_banham@hotmail.com>
 License: MIT License
         
         Copyright (c) 2022 Adam Peter Banham
         
@@ -43,28 +43,27 @@
 `pmkoalas` provides data structures for process mining research in a well-organized pythonic style.
 
 ## Current Features
 * Event log structures
     * Importing and exporting of logs to XES formatted XML
     * Several views/types of log
         * Simplified logs
-            * This type only considers sequences of process 
-            activities, and nothing else.
+            * This type only considers sequences of process activities, and 
+            nothing else.
         * Complex logs
-            * This type considers sequences of events. Where 
-            an event is a mapping of data. This log type can 
-            always be reduced to the simplified type.
-    * Generating logs quickly delimited string
+            * This type considers sequences of events. Where an event is a 
+            mapping of data. This log type can always be reduced to the 
+            simplified type.
+    * Generating logs quickly using delimited strings
         * currently only supports simplified logs
 * Process model structures
     * Petri nets
         * exporting to pnml
         * creating dot files for a net
-        * generation of a net using fragments of desirable 
-        behaviour
+        * generation of a net using fragments of desirable behaviour
 * Process discovery techniques
     * Generating a directly follows language from a log
     * The Alpha miner (original variant)
 
 # Development Information
 To install dependencies:
```

### Comparing `pmkoalas-0.2/README.md` & `pmkoalas-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 `pmkoalas` provides data structures for process mining research in a well-organized pythonic style.
 
 ## Current Features
 * Event log structures
     * Importing and exporting of logs to XES formatted XML
     * Several views/types of log
         * Simplified logs
-            * This type only considers sequences of process 
-            activities, and nothing else.
+            * This type only considers sequences of process activities, and 
+            nothing else.
         * Complex logs
-            * This type considers sequences of events. Where 
-            an event is a mapping of data. This log type can 
-            always be reduced to the simplified type.
-    * Generating logs quickly delimited string
+            * This type considers sequences of events. Where an event is a 
+            mapping of data. This log type can always be reduced to the 
+            simplified type.
+    * Generating logs quickly using delimited strings
         * currently only supports simplified logs
 * Process model structures
     * Petri nets
         * exporting to pnml
         * creating dot files for a net
-        * generation of a net using fragments of desirable 
-        behaviour
+        * generation of a net using fragments of desirable behaviour
 * Process discovery techniques
     * Generating a directly follows language from a log
     * The Alpha miner (original variant)
 
 # Development Information
 To install dependencies:
```

### Comparing `pmkoalas-0.2/pmkoalas/_logging.py` & `pmkoalas-0.2.1/pmkoalas/_logging.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas/complex.py` & `pmkoalas-0.2.1/pmkoalas/complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas/directly.py` & `pmkoalas-0.2.1/pmkoalas/directly.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas/dtlog.py` & `pmkoalas-0.2.1/pmkoalas/dtlog.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas/export.py` & `pmkoalas-0.2.1/pmkoalas/export.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas/read.py` & `pmkoalas-0.2.1/pmkoalas/read.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas/simple.py` & `pmkoalas-0.2.1/pmkoalas/simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas/xes_export.py` & `pmkoalas-0.2.1/pmkoalas/xes_export.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/pmkoalas.egg-info/PKG-INFO` & `pmkoalas-0.2.1/pmkoalas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmkoalas
-Version: 0.2
+Version: 0.2.1
 Summary: A process mining library that focuses on providing pythonic interactions with event logs and languages.
 Author: Adam Burke
 Author-email: Adam Banham <adam_banham@hotmail.com>
 License: MIT License
         
         Copyright (c) 2022 Adam Peter Banham
         
@@ -43,28 +43,27 @@
 `pmkoalas` provides data structures for process mining research in a well-organized pythonic style.
 
 ## Current Features
 * Event log structures
     * Importing and exporting of logs to XES formatted XML
     * Several views/types of log
         * Simplified logs
-            * This type only considers sequences of process 
-            activities, and nothing else.
+            * This type only considers sequences of process activities, and 
+            nothing else.
         * Complex logs
-            * This type considers sequences of events. Where 
-            an event is a mapping of data. This log type can 
-            always be reduced to the simplified type.
-    * Generating logs quickly delimited string
+            * This type considers sequences of events. Where an event is a 
+            mapping of data. This log type can always be reduced to the 
+            simplified type.
+    * Generating logs quickly using delimited strings
         * currently only supports simplified logs
 * Process model structures
     * Petri nets
         * exporting to pnml
         * creating dot files for a net
-        * generation of a net using fragments of desirable 
-        behaviour
+        * generation of a net using fragments of desirable behaviour
 * Process discovery techniques
     * Generating a directly follows language from a log
     * The Alpha miner (original variant)
 
 # Development Information
 To install dependencies:
```

### Comparing `pmkoalas-0.2/pmkoalas.egg-info/SOURCES.txt` & `pmkoalas-0.2.1/pmkoalas.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 pmkoalas/xes.py
 pmkoalas/xes_export.py
 pmkoalas.egg-info/PKG-INFO
 pmkoalas.egg-info/SOURCES.txt
 pmkoalas.egg-info/dependency_links.txt
 pmkoalas.egg-info/requires.txt
 pmkoalas.egg-info/top_level.txt
+pmkoalas/discovery/__init__.py
+pmkoalas/discovery/alpha_miner.py
+pmkoalas/models/dotutil.py
+pmkoalas/models/petrinet.py
+pmkoalas/models/pnfrag.py
 tests/test_drelations.py
 tests/test_dtlog.py
 tests/test_export_complex.py
 tests/test_export_simple.py
 tests/test_read_complex.py
 tests/test_read_simple.py
 tests/test_simple.py
```

### Comparing `pmkoalas-0.2/pyproject.toml` & `pmkoalas-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmkoalas"
-version = "0.2"
+version = "0.2.1"
 authors = [
   { name="Adam Banham", email="adam_banham@hotmail.com" },
   { name="Adam Burke" },
 ]
 description = "A process mining library that focuses on providing pythonic interactions with event logs and languages."
 readme = "README.md"
 license = { file="LICENSE" }
@@ -25,13 +25,15 @@
 [project.optional-dependencies]
 dev = [ 
   'xmlschema'
 ]
 
 [tool.setuptools]
 packages = [
-"pmkoalas"
+"pmkoalas",
+"pmkoalas.discovery",
+"pmkoalas.models"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/AdamBanham/koalas"
 "Bug Tracker" = "https://github.com/AdamBanham/koalas/issues"
```

### Comparing `pmkoalas-0.2/tests/test_drelations.py` & `pmkoalas-0.2.1/tests/test_drelations.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/tests/test_dtlog.py` & `pmkoalas-0.2.1/tests/test_dtlog.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/tests/test_export_complex.py` & `pmkoalas-0.2.1/tests/test_export_complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/tests/test_export_simple.py` & `pmkoalas-0.2.1/tests/test_export_simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/tests/test_read_complex.py` & `pmkoalas-0.2.1/tests/test_read_complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/tests/test_read_simple.py` & `pmkoalas-0.2.1/tests/test_read_simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.2/tests/test_simple.py` & `pmkoalas-0.2.1/tests/test_simple.py`

 * *Files identical despite different names*

