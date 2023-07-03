# Comparing `tmp/flask-tunnel-0.1.2.tar.gz` & `tmp/flask-tunnel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-tunnel-0.1.2.tar", last modified: Mon Jul  3 20:18:52 2023, max compression
+gzip compressed data, was "flask-tunnel-0.1.3.tar", last modified: Mon Jul  3 20:25:14 2023, max compression
```

## Comparing `flask-tunnel-0.1.2.tar` & `flask-tunnel-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:18:52.595620 flask-tunnel-0.1.2/
--rw-rw-rw-   0        0        0     1095 2023-07-03 19:54:11.000000 flask-tunnel-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1302 2023-07-03 20:18:52.595620 flask-tunnel-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-07-03 20:11:08.000000 flask-tunnel-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 20:18:52.581606 flask-tunnel-0.1.2/flask-tunnel/
--rw-rw-rw-   0        0        0        0 2023-07-03 20:17:36.000000 flask-tunnel-0.1.2/flask-tunnel/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-03 19:49:25.000000 flask-tunnel-0.1.2/flask-tunnel/flask_tunnel.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:18:52.593618 flask-tunnel-0.1.2/flask_tunnel.egg-info/
--rw-rw-rw-   0        0        0     1302 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 20:18:52.000000 flask-tunnel-0.1.2/flask_tunnel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 20:18:52.595620 flask-tunnel-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      584 2023-07-03 20:18:50.000000 flask-tunnel-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:25:14.121132 flask-tunnel-0.1.3/
+-rw-rw-rw-   0        0        0     1095 2023-07-03 19:54:11.000000 flask-tunnel-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1302 2023-07-03 20:25:14.120132 flask-tunnel-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-07-03 20:11:08.000000 flask-tunnel-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 20:25:14.099113 flask-tunnel-0.1.3/flask-tunnel/
+-rw-rw-rw-   0        0        0        0 2023-07-03 20:17:36.000000 flask-tunnel-0.1.3/flask-tunnel/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-03 19:49:25.000000 flask-tunnel-0.1.3/flask-tunnel/flask_tunnel.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:25:14.119131 flask-tunnel-0.1.3/flask_tunnel.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-07-03 20:25:14.000000 flask-tunnel-0.1.3/flask_tunnel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-03 20:25:14.000000 flask-tunnel-0.1.3/flask_tunnel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 20:25:14.000000 flask-tunnel-0.1.3/flask_tunnel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 20:25:14.000000 flask-tunnel-0.1.3/flask_tunnel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 20:25:14.000000 flask-tunnel-0.1.3/flask_tunnel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:25:14.121132 flask-tunnel-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      619 2023-07-03 20:25:12.000000 flask-tunnel-0.1.3/setup.py
```

### Comparing `flask-tunnel-0.1.2/LICENSE` & `flask-tunnel-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.2/PKG-INFO` & `flask-tunnel-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tunnel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Configurable ngrok tunneling for Flask apps.
 Home-page: https://github.com/Wolfiej-k/flask-tunnel
 Author: Taj Jethwani-Keyser
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `flask-tunnel-0.1.2/README.md` & `flask-tunnel-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.2/flask-tunnel/flask_tunnel.py` & `flask-tunnel-0.1.3/flask-tunnel/flask_tunnel.py`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.2/flask_tunnel.egg-info/PKG-INFO` & `flask-tunnel-0.1.3/flask_tunnel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tunnel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Configurable ngrok tunneling for Flask apps.
 Home-page: https://github.com/Wolfiej-k/flask-tunnel
 Author: Taj Jethwani-Keyser
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `flask-tunnel-0.1.2/setup.py` & `flask-tunnel-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='flask-tunnel',
-    version='0.1.2',
+    version='0.1.3',
     description='Configurable ngrok tunneling for Flask apps.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Taj Jethwani-Keyser',
     url='https://github.com/Wolfiej-k/flask-tunnel',
     packages=['flask-tunnel'],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
     ],
+    install_requires=['pyngrok'],
     license='MIT'
 )
```

