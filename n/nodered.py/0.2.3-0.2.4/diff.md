# Comparing `tmp/nodered.py-0.2.3.tar.gz` & `tmp/nodered.py-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.3.tar", last modified: Sun Jun  4 00:46:33 2023, max compression
+gzip compressed data, was "nodered.py-0.2.4.tar", last modified: Mon Jul  3 07:00:16 2023, max compression
```

## Comparing `nodered.py-0.2.3.tar` & `nodered.py-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.3/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-04 00:46:33.500000 nodered.py-0.2.3/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.3/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.3/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-06-04 00:16:07.000000 nodered.py-0.2.3/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    13016 2023-06-04 00:19:59.000000 nodered.py-0.2.3/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.3/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.3/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.3/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.420000 nodered.py-0.2.3/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.3/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-06-04 00:34:19.000000 nodered.py-0.2.3/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.3/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.420000 nodered.py-0.2.3/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.3/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.3/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.3/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.3/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-06-04 00:46:33.500000 nodered.py-0.2.3/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.3/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.4/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-03 07:00:16.780000 nodered.py-0.2.4/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.4/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.630000 nodered.py-0.2.4/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.4/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-07-03 06:04:11.000000 nodered.py-0.2.4/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    13201 2023-07-03 06:05:41.000000 nodered.py-0.2.4/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.4/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.4/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.4/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.4/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.4/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.4/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.4/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.4/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.4/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.4/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-03 07:00:16.780000 nodered.py-0.2.4/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.4/setup.py
```

### Comparing `nodered.py-0.2.3/LICENSE` & `nodered.py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/PKG-INFO` & `nodered.py-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.3
+Version: 0.2.4
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.3 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.4 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.3/README.md` & `nodered.py-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.4/nodered.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.3
+Version: 0.2.4
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.3 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.4 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.3/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.4/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/noderedpy/_nodered.py` & `nodered.py-0.2.4/noderedpy/_nodered.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         if node_red_dir is None:
             self.node_red_dir = os.path.join(__path__[0], "node-red-starter")
         else:
             self.node_red_dir = node_red_dir = os.path.realpath(node_red_dir)
             if os.path.exists(node_red_dir):
                 if not { "index.js", "package.json" }.issubset(set(os.listdir(node_red_dir))):
                     raise RuntimeError("Target `node_red_dir` is not Node-RED dir format!")
+
+                shutil.copyfile(os.path.join(__path__[0], "node-red-starter", "index.js"), os.path.join(node_red_dir, "index.js"))
             else:
                 os.mkdir(node_red_dir)
                 shutil.copyfile(os.path.join(__path__[0], "node-red-starter", "index.js"), os.path.join(node_red_dir, "index.js"))
                 shutil.copyfile(os.path.join(__path__[0], "node-red-starter", "package.json"), os.path.join(node_red_dir, "package.json"))
 
         # setup Node-RED starter
         subprocess.call(
@@ -75,24 +77,30 @@
             "title": "Node-RED.py",
             "image": None
         })
         menu_theme = editor_theme.pop("menu", {})
         menu_theme.update({
             "menu-item-palette": False
         })
+        palette_theme = editor_theme.pop("palette", {})
+        palette_theme.update({
+            "editable": palette_theme.pop("editable", True)
+        })
         project_feature = editor_theme.pop("projects", {})
         project_feature.update({
-            "enabled": project_feature.pop("enabled", False)
+            "enabled": project_feature.pop("enabled", True)
         })
 
         editor_theme.update({
             "page": page_theme,
             "header": header_theme,
             "menu": menu_theme,
+            "tours": editor_theme.pop("tours", False),
             "userMenu": editor_theme.pop("userMenu", True),
+            "palette": palette_theme,
             "projects": project_feature
         })
 
         return editor_theme
     
     # fill empty auth in auths
     def __default_node_auth(self, node_auths:List[dict]) -> List[dict]:
@@ -198,18 +206,14 @@
                 "port": self.port,
                 "showDefaultCategory": self.show_default_category,
                 "userCategory": list(set([ node.category for node in RED.registered_nodes ])),
                 "editorTheme": self.editor_theme,
                 "adminAuth": self.node_auths
             }, cfw, indent = 4)
 
-        # # save editor_theme
-        # with open(os.path.join(self.node_red_dir, "editorTheme.json"), "w", encoding = "utf-8") as tjw:
-        #     json.dump(self.editor_theme, tjw, indent = 4)
-
         # remove existing nodes
         for node_dir in glob(os.path.join(self.user_dir, "node_modules", "nodered-py-*")):
             shutil.rmtree(node_dir)
 
         # create custom nodes
         for node in RED.registered_nodes:
             node.create(self.user_dir, self.__cache_dir)
```

### Comparing `nodered.py-0.2.3/noderedpy/_property.py` & `nodered.py-0.2.4/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/noderedpy/assets/python-logo.png` & `nodered.py-0.2.4/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/noderedpy/decorator.py` & `nodered.py-0.2.4/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.4/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/noderedpy/templates/__init__.py` & `nodered.py-0.2.4/noderedpy/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/noderedpy/templates/template.html` & `nodered.py-0.2.4/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/noderedpy/templates/template.js` & `nodered.py-0.2.4/noderedpy/templates/template.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.3/setup.py` & `nodered.py-0.2.4/setup.py`

 * *Files identical despite different names*

