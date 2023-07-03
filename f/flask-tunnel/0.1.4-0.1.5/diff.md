# Comparing `tmp/flask-tunnel-0.1.4.tar.gz` & `tmp/flask-tunnel-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-tunnel-0.1.4.tar", last modified: Mon Jul  3 20:32:00 2023, max compression
+gzip compressed data, was "flask-tunnel-0.1.5.tar", last modified: Mon Jul  3 20:36:32 2023, max compression
```

## Comparing `flask-tunnel-0.1.4.tar` & `flask-tunnel-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:32:00.552971 flask-tunnel-0.1.4/
--rw-rw-rw-   0        0        0     1095 2023-07-03 19:54:11.000000 flask-tunnel-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1302 2023-07-03 20:32:00.552971 flask-tunnel-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-07-03 20:11:08.000000 flask-tunnel-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 20:32:00.551970 flask-tunnel-0.1.4/flask_tunnel.egg-info/
--rw-rw-rw-   0        0        0     1302 2023-07-03 20:32:00.000000 flask-tunnel-0.1.4/flask_tunnel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-03 20:32:00.000000 flask-tunnel-0.1.4/flask_tunnel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:32:00.000000 flask-tunnel-0.1.4/flask_tunnel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 20:32:00.000000 flask-tunnel-0.1.4/flask_tunnel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 20:32:00.000000 flask-tunnel-0.1.4/flask_tunnel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      639 2023-07-03 19:49:25.000000 flask-tunnel-0.1.4/flask_tunnel.py
--rw-rw-rw-   0        0        0       42 2023-07-03 20:32:00.553972 flask-tunnel-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-07-03 20:31:48.000000 flask-tunnel-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:36:32.919209 flask-tunnel-0.1.5/
+-rw-rw-rw-   0        0        0     1095 2023-07-03 19:54:11.000000 flask-tunnel-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1302 2023-07-03 20:36:32.919209 flask-tunnel-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-07-03 20:11:08.000000 flask-tunnel-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 20:36:32.918209 flask-tunnel-0.1.5/flask_tunnel.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-07-03 20:36:32.000000 flask-tunnel-0.1.5/flask_tunnel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-07-03 20:36:32.000000 flask-tunnel-0.1.5/flask_tunnel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 20:36:32.000000 flask-tunnel-0.1.5/flask_tunnel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 20:36:32.000000 flask-tunnel-0.1.5/flask_tunnel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 20:36:32.000000 flask-tunnel-0.1.5/flask_tunnel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      671 2023-07-03 20:36:10.000000 flask-tunnel-0.1.5/flask_tunnel.py
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:36:32.919209 flask-tunnel-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-07-03 20:36:31.000000 flask-tunnel-0.1.5/setup.py
```

### Comparing `flask-tunnel-0.1.4/LICENSE` & `flask-tunnel-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.4/PKG-INFO` & `flask-tunnel-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tunnel
-Version: 0.1.4
+Version: 0.1.5
 Summary: Configurable ngrok tunneling for Flask apps.
 Home-page: https://github.com/Wolfiej-k/flask-tunnel
 Author: Taj Jethwani-Keyser
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `flask-tunnel-0.1.4/README.md` & `flask-tunnel-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `flask-tunnel-0.1.4/flask_tunnel.egg-info/PKG-INFO` & `flask-tunnel-0.1.5/flask_tunnel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tunnel
-Version: 0.1.4
+Version: 0.1.5
 Summary: Configurable ngrok tunneling for Flask apps.
 Home-page: https://github.com/Wolfiej-k/flask-tunnel
 Author: Taj Jethwani-Keyser
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `flask-tunnel-0.1.4/flask_tunnel.py` & `flask-tunnel-0.1.5/flask_tunnel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pyngrok import ngrok, conf
 
 class FlaskTunnel():
     def __init__(self, app, auth: str = None, config: conf.PyngrokConfig = None, **kwargs):
+        ngrok.kill()
+        
         if auth is not None:
             ngrok.set_auth_token(auth)
         
         if config is not None:
             conf.set_default(config)
 
         self.params = kwargs
```

### Comparing `flask-tunnel-0.1.4/setup.py` & `flask-tunnel-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='flask-tunnel',
-    version='0.1.4',
+    version='0.1.5',
     description='Configurable ngrok tunneling for Flask apps.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Taj Jethwani-Keyser',
     url='https://github.com/Wolfiej-k/flask-tunnel',
     py_modules=['flask_tunnel'],
     classifiers=[
```

