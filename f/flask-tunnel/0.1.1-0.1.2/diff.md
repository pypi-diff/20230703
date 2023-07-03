# Comparing `tmp/flask-tunnel-0.1.1.tar.gz` & `tmp/flask-tunnel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-tunnel-0.1.1.tar", last modified: Mon Jul  3 20:11:35 2023, max compression
+gzip compressed data, was "flask-tunnel-0.1.2.tar", last modified: Mon Jul  3 20:18:52 2023, max compression
```

## Comparing `flask-tunnel-0.1.1.tar` & `flask-tunnel-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:11:35.437207 flask-tunnel-0.1.1/
--rw-rw-rw-   0        0        0     1095 2023-07-03 19:54:11.000000 flask-tunnel-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1302 2023-07-03 20:11:35.437207 flask-tunnel-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-07-03 20:11:08.000000 flask-tunnel-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 20:11:35.436206 flask-tunnel-0.1.1/flask_tunnel.egg-info/
--rw-rw-rw-   0        0        0     1302 2023-07-03 20:11:35.000000 flask-tunnel-0.1.1/flask_tunnel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-03 20:11:35.000000 flask-tunnel-0.1.1/flask_tunnel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:11:35.000000 flask-tunnel-0.1.1/flask_tunnel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 20:11:35.000000 flask-tunnel-0.1.1/flask_tunnel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      639 2023-07-03 19:49:25.000000 flask-tunnel-0.1.1/flask_tunnel.py
--rw-rw-rw-   0        0        0       42 2023-07-03 20:11:35.438208 flask-tunnel-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      586 2023-07-03 20:11:33.000000 flask-tunnel-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:18:52.595620 flask-tunnel-0.1.2/
+-rw-rw-rw-   0        0        0     1095 2023-07-03 19:54:11.000000 flask-tunnel-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1302 2023-07-03 20:18:52.595620 flask-tunnel-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-07-03 20:11:08.000000 flask-tunnel-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 20:18:52.581606 flask-tunnel-0.1.2/flask-tunnel/
+-rw-rw-rw-   0        0        0        0 2023-07-03 20:17:36.000000 flask-tunnel-0.1.2/flask-tunnel/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-03 19:49:25.000000 flask-tunnel-0.1.2/flask-tunnel/flask_tunnel.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:18:52.593618 flask-tunnel-0.1.2/flask_tunnel.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:18:52.595620 flask-tunnel-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      584 2023-07-03 20:18:50.000000 flask-tunnel-0.1.2/setup.py
```

### Comparing `flask-tunnel-0.1.1/LICENSE` & `flask-tunnel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.1/PKG-INFO` & `flask-tunnel-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tunnel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Configurable ngrok tunneling for Flask apps.
 Home-page: https://github.com/Wolfiej-k/flask-tunnel
 Author: Taj Jethwani-Keyser
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `flask-tunnel-0.1.1/README.md` & `flask-tunnel-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.1/flask_tunnel.egg-info/PKG-INFO` & `flask-tunnel-0.1.2/flask_tunnel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tunnel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Configurable ngrok tunneling for Flask apps.
 Home-page: https://github.com/Wolfiej-k/flask-tunnel
 Author: Taj Jethwani-Keyser
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `flask-tunnel-0.1.1/flask_tunnel.py` & `flask-tunnel-0.1.2/flask-tunnel/flask_tunnel.py`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.1/setup.py` & `flask-tunnel-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='flask-tunnel',
-    version='0.1.1',
+    version='0.1.2',
     description='Configurable ngrok tunneling for Flask apps.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Taj Jethwani-Keyser',
     url='https://github.com/Wolfiej-k/flask-tunnel',
-    py_modules=['flask_tunnel'],
+    packages=['flask-tunnel'],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
     ],
     license='MIT'
 )
```

