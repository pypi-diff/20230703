# Comparing `tmp/modeldag-0.3.3.tar.gz` & `tmp/modeldag-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modeldag-0.3.3.tar", last modified: Fri Jun 30 08:44:12 2023, max compression
+gzip compressed data, was "modeldag-0.4.0.tar", last modified: Mon Jul  3 10:29:38 2023, max compression
```

## Comparing `modeldag-0.3.3.tar` & `modeldag-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 08:44:12.647832 modeldag-0.3.3/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.3.3/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      725 2023-06-30 08:44:12.647877 modeldag-0.3.3/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     1896 2023-06-30 08:42:53.000000 modeldag-0.3.3/README.md
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 08:44:12.647116 modeldag-0.3.3/modeldag/
--rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-06-30 08:40:07.000000 modeldag-0.3.3/modeldag/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    15196 2023-06-26 15:11:38.000000 modeldag-0.3.3/modeldag/modeldag.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 08:44:12.647734 modeldag-0.3.3/modeldag.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      725 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.3.3/modeldag.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/top_level.txt
--rw-r--r--   0 rigault   (2358) staff       (20)     1004 2023-06-30 08:44:12.648128 modeldag-0.3.3/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.3.3/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 10:29:38.752427 modeldag-0.4.0/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.4.0/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      725 2023-07-03 10:29:38.752487 modeldag-0.4.0/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     1896 2023-06-30 08:42:53.000000 modeldag-0.4.0/README.md
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 10:29:38.751597 modeldag-0.4.0/modeldag/
+-rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-07-03 10:29:13.000000 modeldag-0.4.0/modeldag/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15477 2023-07-03 10:26:51.000000 modeldag-0.4.0/modeldag/modeldag.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 10:29:38.752324 modeldag-0.4.0/modeldag.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      725 2023-07-03 10:29:38.000000 modeldag-0.4.0/modeldag.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-07-03 10:29:38.000000 modeldag-0.4.0/modeldag.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-07-03 10:29:38.000000 modeldag-0.4.0/modeldag.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.4.0/modeldag.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-07-03 10:29:38.000000 modeldag-0.4.0/modeldag.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-07-03 10:29:38.000000 modeldag-0.4.0/modeldag.egg-info/top_level.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)     1004 2023-07-03 10:29:38.752821 modeldag-0.4.0/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.4.0/setup.py
```

### Comparing `modeldag-0.3.3/LICENSE` & `modeldag-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modeldag-0.3.3/PKG-INFO` & `modeldag-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.3.3
+Version: 0.4.0
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `modeldag-0.3.3/README.md` & `modeldag-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `modeldag-0.3.3/modeldag/modeldag.py` & `modeldag-0.4.0/modeldag/modeldag.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,24 @@
             
     @staticmethod
     def draw_from_pdf(pdf, xx, size):
         """ randomly draw from xx N=size elements following the pdf. """
         if type(xx) == str: # assumed r_ input
             xx = eval(f"np.r_[{xx}]")
 
-        return np.random.choice(xx, size=size, p=pdf/pdf.sum())
+        pdf = np.squeeze(pdf) # shape -> (1, size) -> (size,)
+        
+        if len( pdf.shape ) == 2:
+            choices = np.hstack([np.random.choice(xx, size=1, p=pdf_/pdf_.sum())
+                           for pdf_ in pdf])
+        else:
+            choices = np.random.choice(xx, size=size, p=pdf/pdf.sum())
+
+        return choices
+    
 
     def _draw(self, model, size=None, limit_to_entries=None, data=None):
         """ core method converting model into a DataFrame (interp) """
         
         model = deepcopy(model) # safe case
         if size == 0:
             columns = list(np.hstack([v.get("as", name) for name, v in model.items()]))
```

### Comparing `modeldag-0.3.3/modeldag.egg-info/PKG-INFO` & `modeldag-0.4.0/modeldag.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.3.3
+Version: 0.4.0
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `modeldag-0.3.3/setup.cfg` & `modeldag-0.4.0/setup.cfg`

 * *Files identical despite different names*

