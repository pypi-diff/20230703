# Comparing `tmp/uniquer-1.0.0.tar.gz` & `tmp/uniquer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniquer-1.0.0.tar", max compression
+gzip compressed data, was "uniquer-1.0.1.tar", max compression
```

## Comparing `uniquer-1.0.0.tar` & `uniquer-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-20 20:06:33.948440 uniquer-1.0.0/LICENSE
--rw-r--r--   0        0        0     1094 2023-06-20 20:06:33.952440 uniquer-1.0.0/README.md
--rw-r--r--   0        0        0     2071 2023-06-20 20:28:36.517290 uniquer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3062 2023-06-20 20:25:37.177959 uniquer-1.0.0/uniquer/__init__.py
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 uniquer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-03 06:56:48.422968 uniquer-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1175 2023-07-03 06:56:48.422968 uniquer-1.0.1/README.md
+-rw-r--r--   0        0        0     2071 2023-07-03 06:56:48.422968 uniquer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3219 2023-07-03 06:56:48.422968 uniquer-1.0.1/uniquer/__init__.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 uniquer-1.0.1/PKG-INFO
```

### Comparing `uniquer-1.0.0/LICENSE` & `uniquer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniquer-1.0.0/README.md` & `uniquer-1.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -8,7 +8,15 @@
 
 # Unique Iteration
 
 * [Documentation](https://uniquer.readthedocs.io/en/latest/)
 * [PyPI](https://pypi.org/project/uniquer/)
 * [Sources](https://github.com/nbiotcloud/uniquer)
 * [Issues](https://github.com/nbiotcloud/uniquer/issues)
+
+## Installation
+
+Installing it is pretty easy:
+
+```bash
+pip install uniquer
+```
```

### Comparing `uniquer-1.0.0/pyproject.toml` & `uniquer-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniquer"
-version = "1.0.0"
+version = "1.0.1"
 description = "Unique Iteration"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `uniquer-1.0.0/uniquer/__init__.py` & `uniquer-1.0.1/uniquer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """
-Unique Iteration.
+Unique Iteration Utilities.
+
+* :any:`unique` - Unique Iterator
+* :any:`uniquetuple` - Create tuple with unique elements
+* :any:`uniquelist` - Create list with unique elements
 """
 
 
 def uniquelist(iterable, key=None):
     """
     Return unique list.
```

### Comparing `uniquer-1.0.0/PKG-INFO` & `uniquer-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniquer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unique Iteration
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -24,7 +24,15 @@
 # Unique Iteration
 
 * [Documentation](https://uniquer.readthedocs.io/en/latest/)
 * [PyPI](https://pypi.org/project/uniquer/)
 * [Sources](https://github.com/nbiotcloud/uniquer)
 * [Issues](https://github.com/nbiotcloud/uniquer/issues)
 
+## Installation
+
+Installing it is pretty easy:
+
+```bash
+pip install uniquer
+```
+
```

