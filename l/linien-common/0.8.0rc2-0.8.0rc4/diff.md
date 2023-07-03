# Comparing `tmp/linien-common-0.8.0rc2.tar.gz` & `tmp/linien-common-0.8.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-common-0.8.0rc2.tar", last modified: Mon Jul  3 12:44:39 2023, max compression
+gzip compressed data, was "linien-common-0.8.0rc4.tar", last modified: Mon Jul  3 13:54:51 2023, max compression
```

## Comparing `linien-common-0.8.0rc2.tar` & `linien-common-0.8.0rc4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:44:39.823587 linien-common-0.8.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 12:44:39.823587 linien-common-0.8.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:44:39.819586 linien-common-0.8.0rc2/linien_common/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 12:44:27.000000 linien-common-0.8.0rc2/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-03 12:44:27.000000 linien-common-0.8.0rc2/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 12:44:27.000000 linien-common-0.8.0rc2/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-03 12:44:27.000000 linien-common-0.8.0rc2/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:44:39.823587 linien-common-0.8.0rc2/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 12:44:39.000000 linien-common-0.8.0rc2/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 12:44:39.000000 linien-common-0.8.0rc2/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:44:39.000000 linien-common-0.8.0rc2/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 12:44:39.000000 linien-common-0.8.0rc2/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:44:39.000000 linien-common-0.8.0rc2/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:44:39.823587 linien-common-0.8.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-03 12:44:27.000000 linien-common-0.8.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:51.258747 linien-common-0.8.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 13:54:51.258747 linien-common-0.8.0rc4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:51.258747 linien-common-0.8.0rc4/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 13:54:39.000000 linien-common-0.8.0rc4/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-03 13:54:39.000000 linien-common-0.8.0rc4/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-03 13:54:39.000000 linien-common-0.8.0rc4/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 13:54:39.000000 linien-common-0.8.0rc4/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-03 13:54:39.000000 linien-common-0.8.0rc4/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:51.258747 linien-common-0.8.0rc4/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 13:54:51.000000 linien-common-0.8.0rc4/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-03 13:54:51.000000 linien-common-0.8.0rc4/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:54:51.000000 linien-common-0.8.0rc4/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 13:54:51.000000 linien-common-0.8.0rc4/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 13:54:51.000000 linien-common-0.8.0rc4/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:54:51.258747 linien-common-0.8.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-03 13:54:39.000000 linien-common-0.8.0rc4/setup.py
```

### Comparing `linien-common-0.8.0rc2/PKG-INFO` & `linien-common-0.8.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 0.8.0rc2
+Version: 0.8.0rc4
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-0.8.0rc2/linien_common/common.py` & `linien-common-0.8.0rc4/linien_common/common.py`

 * *Files identical despite different names*

### Comparing `linien-common-0.8.0rc2/linien_common/config.py` & `linien-common-0.8.0rc4/linien_common/config.py`

 * *Files identical despite different names*

### Comparing `linien-common-0.8.0rc2/linien_common/influxdb.py` & `linien-common-0.8.0rc4/linien_common/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-common-0.8.0rc2/linien_common.egg-info/PKG-INFO` & `linien-common-0.8.0rc4/linien_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 0.8.0rc2
+Version: 0.8.0rc4
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-0.8.0rc2/setup.py` & `linien-common-0.8.0rc4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
 setup(
     name="linien-common",
-    version="0.8.0rc2",
+    version="0.8.0rc4",
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
     maintainer_email="leykauf@physik.hu-berlin.de",
     description="Shared components of the Linien spectroscopy lock application.",
     long_description="Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.",  # noqa: E501
     long_description_content_type="text/markdown",
```

