# Comparing `tmp/cnvm-0.1.1.tar.gz` & `tmp/cnvm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnvm-0.1.1.tar", max compression
+gzip compressed data, was "cnvm-0.2.0.tar", max compression
```

## Comparing `cnvm-0.1.1.tar` & `cnvm-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-01 12:02:15.724243 cnvm-0.1.1/cnvm/__init__.py
--rw-r--r--   0        0        0     9576 2023-06-01 12:02:15.724243 cnvm-0.1.1/cnvm/collective_variables.py
--rw-r--r--   0        0        0    10290 2023-06-01 12:02:15.724243 cnvm-0.1.1/cnvm/model.py
--rw-r--r--   0        0        0    10221 2023-06-29 14:27:54.206058 cnvm-0.1.1/cnvm/network_generator.py
--rw-r--r--   0        0        0    10105 2023-06-01 12:02:15.725239 cnvm-0.1.1/cnvm/parameters.py
--rw-r--r--   0        0        0     6774 2023-06-01 12:02:15.725239 cnvm-0.1.1/cnvm/utils.py
--rw-r--r--   0        0        0    35823 2022-11-05 17:20:32.769485 cnvm-0.1.1/LICENSE
--rw-r--r--   0        0        0     1158 2023-06-29 15:23:06.929140 cnvm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5643 2023-06-01 12:02:15.723246 cnvm-0.1.1/README.md
--rw-r--r--   0        0        0     6543 1970-01-01 00:00:00.000000 cnvm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      191 2023-07-03 13:15:49.929756 cnvm-0.2.0/cnvm/__init__.py
+-rw-r--r--   0        0        0     3375 2023-07-03 13:17:31.093908 cnvm-0.2.0/cnvm/chemical_langevin_equation.py
+-rw-r--r--   0        0        0     9576 2023-06-01 12:02:15.724243 cnvm-0.2.0/cnvm/collective_variables.py
+-rw-r--r--   0        0        0    10290 2023-06-01 12:02:15.724243 cnvm-0.2.0/cnvm/model.py
+-rw-r--r--   0        0        0    10221 2023-06-29 14:27:54.206058 cnvm-0.2.0/cnvm/network_generator.py
+-rw-r--r--   0        0        0    10105 2023-06-01 12:02:15.725239 cnvm-0.2.0/cnvm/parameters.py
+-rw-r--r--   0        0        0     6774 2023-06-01 12:02:15.725239 cnvm-0.2.0/cnvm/utils.py
+-rw-r--r--   0        0        0    35823 2022-11-05 17:20:32.769485 cnvm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1158 2023-07-03 14:13:15.895067 cnvm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5643 2023-06-01 12:02:15.723246 cnvm-0.2.0/README.md
+-rw-r--r--   0        0        0     6594 1970-01-01 00:00:00.000000 cnvm-0.2.0/PKG-INFO
```

### Comparing `cnvm-0.1.1/cnvm/collective_variables.py` & `cnvm-0.2.0/cnvm/collective_variables.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.1/cnvm/model.py` & `cnvm-0.2.0/cnvm/model.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.1/cnvm/network_generator.py` & `cnvm-0.2.0/cnvm/network_generator.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.1/cnvm/parameters.py` & `cnvm-0.2.0/cnvm/parameters.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.1/cnvm/utils.py` & `cnvm-0.2.0/cnvm/utils.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.1/LICENSE` & `cnvm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.1/pyproject.toml` & `cnvm-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cnvm"
-version = "0.1.1"
+version = "0.2.0"
 description = "Continuous-time Noisy Voter Model (CNVM) of social dynamics."
 license = "GPL-3.0-or-later"
 authors = ["Marvin Lücke"]
 readme = "README.md"
 repository = "https://github.com/lueckem/cnvm"
 keywords = [
     "voter model",
@@ -18,15 +18,15 @@
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<3.12"
 numpy = ">=1.21"
 numba = ">=0.55"
 networkx = ">=2.8.4"
 scipy = ">=1.9.3"
 
 
 [tool.poetry.group.test]
```

### Comparing `cnvm-0.1.1/README.md` & `cnvm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.1/PKG-INFO` & `cnvm-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cnvm
-Version: 0.1.1
+Version: 0.2.0
 Summary: Continuous-time Noisy Voter Model (CNVM) of social dynamics.
 Home-page: https://github.com/lueckem/cnvm
 License: GPL-3.0-or-later
 Keywords: voter model,social dynamics,opinion dynamics,statistical physics,agent-based model,epidemiology,interacting particle system
 Author: Marvin Lücke
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: networkx (>=2.8.4)
 Requires-Dist: numba (>=0.55)
 Requires-Dist: numpy (>=1.21)
 Requires-Dist: scipy (>=1.9.3)
 Project-URL: Repository, https://github.com/lueckem/cnvm
```

