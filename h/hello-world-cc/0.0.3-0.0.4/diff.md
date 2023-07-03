# Comparing `tmp/hello_world_cc-0.0.3.tar.gz` & `tmp/hello_world_cc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_world_cc-0.0.3.tar", last modified: Mon Jul  3 04:18:10 2023, max compression
+gzip compressed data, was "hello_world_cc-0.0.4.tar", last modified: Mon Jul  3 15:10:39 2023, max compression
```

## Comparing `hello_world_cc-0.0.3.tar` & `hello_world_cc-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 04:18:10.753592 hello_world_cc-0.0.3/
--rw-r--r--   0 chenchen   (501) staff       (20)     3078 2023-06-28 07:04:50.000000 hello_world_cc-0.0.3/.gitignore
--rw-r--r--   0 chenchen   (501) staff       (20)    11357 2023-06-28 07:04:50.000000 hello_world_cc-0.0.3/LICENSE
--rw-r--r--   0 chenchen   (501) staff       (20)    13902 2023-07-03 04:18:10.753392 hello_world_cc-0.0.3/PKG-INFO
--rw-r--r--   0 chenchen   (501) staff       (20)      679 2023-07-03 02:58:22.000000 hello_world_cc-0.0.3/README.md
-drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 04:18:10.752566 hello_world_cc-0.0.3/hello_world_cc.egg-info/
--rw-r--r--   0 chenchen   (501) staff       (20)    13902 2023-07-03 04:18:10.000000 hello_world_cc-0.0.3/hello_world_cc.egg-info/PKG-INFO
--rw-r--r--   0 chenchen   (501) staff       (20)      276 2023-07-03 04:18:10.000000 hello_world_cc-0.0.3/hello_world_cc.egg-info/SOURCES.txt
--rw-r--r--   0 chenchen   (501) staff       (20)        1 2023-07-03 04:18:10.000000 hello_world_cc-0.0.3/hello_world_cc.egg-info/dependency_links.txt
--rw-r--r--   0 chenchen   (501) staff       (20)       19 2023-07-03 04:18:10.000000 hello_world_cc-0.0.3/hello_world_cc.egg-info/requires.txt
--rw-r--r--   0 chenchen   (501) staff       (20)       11 2023-07-03 04:18:10.000000 hello_world_cc-0.0.3/hello_world_cc.egg-info/top_level.txt
-drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 04:18:10.753014 hello_world_cc-0.0.3/helloworld/
--rw-r--r--   0 chenchen   (501) staff       (20)       67 2023-07-03 02:58:22.000000 hello_world_cc-0.0.3/helloworld/__init__.py
--rw-r--r--   0 chenchen   (501) staff       (20)     3852 2023-07-03 02:58:22.000000 hello_world_cc-0.0.3/helloworld/client.py
--rw-r--r--   0 chenchen   (501) staff       (20)      558 2023-07-03 04:16:46.000000 hello_world_cc-0.0.3/pyproject.toml
--rw-r--r--   0 chenchen   (501) staff       (20)       38 2023-07-03 04:18:10.753649 hello_world_cc-0.0.3/setup.cfg
+drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:10:39.760633 hello_world_cc-0.0.4/
+-rw-r--r--   0 chenchen   (501) staff       (20)     3078 2023-06-28 07:04:50.000000 hello_world_cc-0.0.4/.gitignore
+-rw-r--r--   0 chenchen   (501) staff       (20)    11357 2023-06-28 07:04:50.000000 hello_world_cc-0.0.4/LICENSE
+-rw-r--r--   0 chenchen   (501) staff       (20)    13888 2023-07-03 15:10:39.760220 hello_world_cc-0.0.4/PKG-INFO
+-rw-r--r--   0 chenchen   (501) staff       (20)      679 2023-07-03 10:57:13.000000 hello_world_cc-0.0.4/README.md
+-rw-r--r--   0 chenchen   (501) staff       (20)     3852 2023-07-03 15:03:22.000000 hello_world_cc-0.0.4/client.py
+drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:10:39.759859 hello_world_cc-0.0.4/hello_world_cc.egg-info/
+-rw-r--r--   0 chenchen   (501) staff       (20)    13888 2023-07-03 15:10:39.000000 hello_world_cc-0.0.4/hello_world_cc.egg-info/PKG-INFO
+-rw-r--r--   0 chenchen   (501) staff       (20)      242 2023-07-03 15:10:39.000000 hello_world_cc-0.0.4/hello_world_cc.egg-info/SOURCES.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)        1 2023-07-03 15:10:39.000000 hello_world_cc-0.0.4/hello_world_cc.egg-info/dependency_links.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)       19 2023-07-03 15:10:39.000000 hello_world_cc-0.0.4/hello_world_cc.egg-info/requires.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)        7 2023-07-03 15:10:39.000000 hello_world_cc-0.0.4/hello_world_cc.egg-info/top_level.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)      431 2023-07-03 15:10:29.000000 hello_world_cc-0.0.4/pyproject.toml
+-rw-r--r--   0 chenchen   (501) staff       (20)       38 2023-07-03 15:10:39.760705 hello_world_cc-0.0.4/setup.cfg
```

### Comparing `hello_world_cc-0.0.3/.gitignore` & `hello_world_cc-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hello_world_cc-0.0.3/LICENSE` & `hello_world_cc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hello_world_cc-0.0.3/PKG-INFO` & `hello_world_cc-0.0.4/hello_world_cc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
-Name: hello_world_cc
-Version: 0.0.3
-Summary: a Hello World Test Module
+Name: hello-world-cc
+Version: 0.0.4
+Summary: the Official W3bstream Client for Python
+Author: haaai
 Author-email: chenchen <chen1233216@hotmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -201,16 +202,14 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Keywords: w3bstream
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
```

### Comparing `hello_world_cc-0.0.3/README.md` & `hello_world_cc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hello_world_cc-0.0.3/hello_world_cc.egg-info/PKG-INFO` & `hello_world_cc-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
-Name: hello-world-cc
-Version: 0.0.3
-Summary: a Hello World Test Module
+Name: hello_world_cc
+Version: 0.0.4
+Summary: the Official W3bstream Client for Python
+Author: haaai
 Author-email: chenchen <chen1233216@hotmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -201,16 +202,14 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Keywords: w3bstream
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
```

### Comparing `hello_world_cc-0.0.3/helloworld/client.py` & `hello_world_cc-0.0.4/client.py`

 * *Files identical despite different names*

