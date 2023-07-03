# Comparing `tmp/limberer-0.2.1.tar.gz` & `tmp/limberer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.2.1.tar", last modified: Wed Jun 28 22:57:08 2023, max compression
+gzip compressed data, was "limberer-0.2.2.tar", last modified: Mon Jul  3 07:51:54 2023, max compression
```

## Comparing `limberer-0.2.1.tar` & `limberer-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.1/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.1/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.1/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-06-28 22:57:08.475502 limberer-0.2.1/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.1/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1101 2023-06-28 22:56:00.000000 limberer-0.2.1/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-06-28 22:57:08.475502 limberer-0.2.1/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     8453 2023-06-28 22:55:11.000000 limberer-0.2.1/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5425 2023-06-28 13:20:04.000000 limberer-0.2.1/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1101 2023-06-28 10:57:50.000000 limberer-0.2.1/src/limberer/static/assets/base.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-06-28 10:57:50.000000 limberer-0.2.1/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3316 2023-06-28 10:57:50.000000 limberer-0.2.1/src/limberer/static/assets/theme.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.1/src/limberer/static/custom/custom.css
--rw-r--r--   0 jtd       (1000) jtd       (1000)      282 2023-06-28 04:38:31.000000 limberer-0.2.1/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1155 2023-06-28 13:19:41.000000 limberer-0.2.1/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1571 2023-06-28 13:19:41.000000 limberer-0.2.1/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      317 2023-06-28 13:19:57.000000 limberer-0.2.1/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.1/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      275 2023-06-28 13:19:57.000000 limberer-0.2.1/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.1/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-06-28 22:57:08.475502 limberer-0.2.1/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-06-28 22:57:08.000000 limberer-0.2.1/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      738 2023-06-28 22:57:08.000000 limberer-0.2.1/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-06-28 22:57:08.000000 limberer-0.2.1/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-06-28 22:57:08.000000 limberer-0.2.1/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       49 2023-06-28 22:57:08.000000 limberer-0.2.1/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-06-28 22:57:08.000000 limberer-0.2.1/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.2/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.2/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.2/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 07:51:54.930336 limberer-0.2.2/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.2/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1121 2023-07-03 06:56:58.000000 limberer-0.2.2/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 07:51:54.930336 limberer-0.2.2/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.926336 limberer-0.2.2/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.926336 limberer-0.2.2/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    10256 2023-07-03 07:50:53.000000 limberer-0.2.2/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5507 2023-07-03 07:10:09.000000 limberer-0.2.2/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1101 2023-06-28 10:57:50.000000 limberer-0.2.2/src/limberer/static/assets/base.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-06-28 10:57:50.000000 limberer-0.2.2/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3582 2023-07-03 07:41:04.000000 limberer-0.2.2/src/limberer/static/assets/theme.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.2/src/limberer/static/custom/custom.css
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      282 2023-06-28 04:38:31.000000 limberer-0.2.2/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1210 2023-07-03 07:49:39.000000 limberer-0.2.2/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 07:49:42.000000 limberer-0.2.2/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 07:49:58.000000 limberer-0.2.2/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.2/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      300 2023-07-03 07:49:52.000000 limberer-0.2.2/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.2/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      738 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.2.1/LICENSE` & `limberer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.2.1/PKG-INFO` & `limberer-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.1/README.md` & `limberer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.1/pyproject.toml` & `limberer-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "limberer"
 # alternatively, limberr
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
@@ -20,14 +20,15 @@
 dependencies = [
   "panflute",
   "chevron",
   "weasyprint",
   "toml",
   "markdown",
   "pillow",
+  "beautifulsoup4",
 ]
 
 [project.urls]
 repository = "https://github.com/ChaosData/limberer"
 
 [build-system]
 requires = ["setuptools>=61.0"]
```

### Comparing `limberer-0.2.1/src/limberer/__init__.py` & `limberer-0.2.2/src/limberer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 import toml
 from collections.abc import Callable
 import chevron
 import weasyprint
 import markdown # temporary
 import subprocess
 import io
+from bs4 import BeautifulSoup
 
 from .pf import entrypoint
 
 # disable remote url resolution and path traversal
 def fetcher(url):
   u = None
   if url.startswith("file://"):
@@ -69,38 +70,48 @@
   return r
 chevron.renderer._get_key = fake_get_key
 # >>> chevron.render('Hello, {{#mustache}}{{#__class__.__bases__}}{{#__subclasses__}}{{.}}{{/__subclasses__}}{{/__class__.__bases__}}{{/mustache}}!', {'mustache': 'World'})
 # 'Hello, no soup for you.!'
 # >>> chevron.render('Hello, {{#mustache}}{{#upper}}{{.}}{{/upper}}{{/mustache}}!', {'mustache': 'world'})
 # 'Hello, no soup for you!!'
 
-def convert(path, opts, toc):
+
+footnotecount = 1
+
+
+def convert(path, opts, toc, args):
   #print("convert(" + repr(path) + ")")
   proc1 = subprocess.run(['pandoc', '-t', 'json', path], capture_output=True)
   if proc1.returncode != 0:
     sys.stderr.write("error running initial pandoc command: \n")
     sys.stderr.buffer.write(proc1.stderr)
     sys.stderr.write("\n")
     sys.exit(1)
   o1 = proc1.stdout.decode('utf-8')
 
+  if args.debug:
+    print(o1)
+
   # run the panflute filter
   sys.argv = ["html"]
   iw = io.StringIO(o1)
   ow = io.StringIO("")
 
   headers = []
   _headers = []
   r = entrypoint(iw, ow, _headers)
   ow.seek(0)
   o2 = ow.read()
 
   if len(_headers) == 1:
     headers = _headers[0]
 
+  if "columns" in opts:
+    toc.append(opts | {"name": opts['section_name'] + "-columns-title", "issubsection": False})
+
   #print(repr(headers))
   header_level = int(opts.get('toc_header_level', ['1'])[0])
 
   for h in headers:
     if h.level <= header_level:
       toc.append(opts | {"name": h.identifier, "issubsection": h.level != 1})
 
@@ -127,15 +138,17 @@
                                      title='subcommands',
                                      description='valid subcommands',
                                      help='additional help')
 
   create = subparsers.add_parser('create')
   create.add_argument('project', metavar='<project>', type=str,
                       help="Name of project to create.")
-
+  create.add_argument('-t', '--template', metavar='<path>', type=str,
+                      default="",
+                      help='Create from alternative template path instead of the built-in default.')
   build = subparsers.add_parser('build')
   parser.add_argument('-d', '--debug', action='store_true',
                       help='Debug output.')
   build.add_argument('config', metavar='<config>', type=str,
                       help="Path to document toml configuration file.")
   args = parser.parse_args()
   return args
@@ -151,22 +164,33 @@
       sys.stderr.write(f"error: path '{projpath}' already exists.\n")
       sys.exit(1)
     absprojpath = os.path.abspath(projpath)
     os.makedirs(os.path.dirname(absprojpath), exist_ok=True)
 
     modpath = os.path.dirname(os.path.abspath(__file__))
     staticpath = os.path.join(modpath, "static")
-
-    shutil.copytree(staticpath, absprojpath)
+    templatepath = None
+    if args.template == "":
+      templatepath = staticpath
+    else:
+      templatepath = args.template
+    shutil.copytree(templatepath, absprojpath)
 
     projname = os.path.basename(absprojpath)
-    os.rename(os.path.join(absprojpath, "project.toml"),
-              os.path.join(absprojpath, projname + ".toml"))
+    if os.path.exists(os.path.join(absprojpath, "project.toml")):
+      os.rename(os.path.join(absprojpath, "project.toml"),
+                os.path.join(absprojpath, projname + ".toml"))
+    else:
+      print("project.toml not found in template path " + repr(args.template) + ".... using default.")
+      shutil.copyfile(os.path.join(staticpath, "project.toml"),
+                os.path.join(absprojpath, projname + ".toml"))
 
 def build(args):
+  global footnotecount
+
   config = args.config
   if not os.path.exists(config):
     sys.stderr.write(f"error: '{config}' not found.\n")
     sys.exit(1)
   if not os.path.isfile(config):
     sys.stderr.write(f"error: '{config}' is not a file.\n")
     sys.exit(1)
@@ -195,26 +219,51 @@
       section_path = 'sections/{}.md'.format(section['name'])
       content = open(section_path, 'rb').read()
       #print(repr(content))
       content = content.decode('utf-8')
       md = markdown.Markdown(extensions=["meta"])
       html = md.convert(content)
       opts = md.Meta | section
-      html = convert(section_path, opts, toc)
+      opts['section_name'] = section_name
+      html = convert(section_path, opts, toc, args)
+      footnotes = ""
+      soup = BeautifulSoup(html, 'html.parser')
+      _fns = soup.find(id="footnotes")
+      if _fns is not None:
+        _fns = _fns.extract()
+        _fns.ol['start'] = str(footnotecount)
+        _fns.ol['style'] = f"counter-reset:list-item {footnotecount}; counter-increment:list-item -1;"
+        __fns = [c for c in _fns.ol.children if c != "\n"]
+        footnotecount += len(__fns)
+        del _fns['id']
+        for __fn in __fns:
+          id = __fn['id']
+          nid = section_name + "-" + id
+          __fn['id'] = nid
+          __fnx = soup.find(id=id)
+          if __fnx is not None:
+            __fnx['id'] = nid
+        for _a in soup.find_all(class_="footnote-ref"):
+          _a['id'] = section_name + "-" + _a['id']
+          _a['href'] = '#' + section_name + "-" + _a['href'][1:]
+          print(_a)
+        for _a in _fns.find_all(class_="footnote-back"):
+          _a['href'] = '#' + section_name + "-" + _a['href'][1:]
+
+        footnotes = str(_fns)
+        html = str(soup)
+
       opts['html'] = html
+      opts['footnotes'] = footnotes
       opts['opts'] = opts # we occasionally need top.down.variable.paths to resolve abiguity
       template = section_template
       if "alt" in section:
         template = open('templates/{}.html'.format(section['alt']), 'r').read()
-      #r = chevron.render(template, {"name": section['name'], "html": html})
-      #print(opts)
       r = chevron.render(template, opts)
       sections.append(r)
-      #if "title" in section:
-        #toc.append(opts | {"issubsection": False})
     elif section['type'] == 'toc':
       # defer until after we get through everything else
       sections.append(section)
     else:
       # assume in templates/
       template = open('templates/{}.html'.format(section['type']), 'r').read()
       r = chevron.render(template, config)
```

### Comparing `limberer-0.2.1/src/limberer/pf.py` & `limberer-0.2.2/src/limberer/pf.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import subprocess
 import os
 import platform
 import base64
 from PIL import Image
 
 titlecounter = 0
-
 headers = []
 
 def stringify(content):
   out = []
   for part in content:
     if isinstance(part, pf.Str):
       out.append(str(part)[4:-1])
@@ -53,14 +52,17 @@
   if isinstance(elem, pf.Doc):
     pass
   elif isinstance(elem, pf.Header):
     #with open("/tmp/log.txt", "a") as fd:
     #  fd.write(repr(elem) + "\n")
     headers.append(elem)
     elem.identifier = elem.identifier + str(len(headers))
+  #elif isinstance(elem, pf.Note):
+  #  print("footnote: " + repr(elem))
+  #  pass
   elif isinstance(elem, pf.CodeBlock):
     code = elem.text.encode()
     classes = elem.classes
 
     lang = 'txt' if len(classes) == 0 else classes[0]
     if lang in ['bash', 'sh', 'console']:
       proc = subprocess.run(['highlight', '--list-scripts=langs'], capture_output=True)
```

### Comparing `limberer-0.2.1/src/limberer/static/assets/base.css` & `limberer-0.2.2/src/limberer/static/assets/base.css`

 * *Files identical despite different names*

### Comparing `limberer-0.2.1/src/limberer/static/assets/logo.svg` & `limberer-0.2.2/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.2.1/src/limberer/static/assets/theme.css` & `limberer-0.2.2/src/limberer/static/assets/theme.css`

 * *Files 8% similar despite different names*

```diff
@@ -186,33 +186,52 @@
   align-items: flex-start;
   justify-content: center;
   position: absolute;
   bottom: 0px;
   width: 100%;
 }
 
-ul {
+article ul {
   list-style: none;
   padding-left: 0;
 }
 
 /*weasyprint currently gets this wrong: https://github.com/Kozea/WeasyPrint/issues/1557*/
-ol {
+article ol {
   list-style-position: outside;
   padding-left: 0;
   margin-left: 1rem;
 }
-ol li::before {
+article ol li::before {
   content: "\00a0\00a0\00a0";
 }
 
-li {
+article li {
   line-height: 1.5;
 }
 
-ul li::before {
+article ul li::before {
   color: #E6E6FA;
   content: '• ';
   font-size: 10pt;
   padding-right: 1em;
 }
 
+.footnotes {
+  position: absolute;
+  width: 100%;
+  bottom: 0;
+}
+
+.footnotes ol {
+  padding-left: 0;
+  margin-left: 0;
+}
+
+.footnotes ol li {
+  line-height: 1;
+}
+.footnotes ol li::before {
+  content: none;
+  line-height: 1;
+}
+
```

### Comparing `limberer-0.2.1/src/limberer/static/sections/example.md` & `limberer-0.2.2/src/limberer/static/sections/example.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 
 <h2 id="wat">Hello World - not picked up by the ToC due to inline html</h2>
 
 ### Not in the ToC due to H3
 
 Hi there.
 
-* some
-* bullets
+* some[^aaa]
+* bullets[^bbb]
 * <a href="#example">#Example</a>
 * <a href="#wat" class="title"></a>
 
+[^aaa]: <https://example.com>
+[^bbb]: wat
+
 ## Code Snippet
 
 ```js
 let j = await fetch("https://wat.wat", {
   "headers": {
     "x-test": "foo"
   }
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
 --- toc_header_level: 2 --- # Examplely Example
 ***** Hello World - not picked up by the ToC due to inline html *****
-### Not in the ToC due to H3 Hi there. * some * bullets * #Example *  ## Code
-Snippet ```js let j = await fetch("https://wat.wat", { "headers": { "x-test":
-"foo" } }).then((res)=>res.json()); ``` ## Table Test
+### Not in the ToC due to H3 Hi there. * some[^aaa] * bullets[^bbb] * #Example
+*  [^aaa]:
+example.com> [^bbb]: wat ## Code Snippet ```js let j = await fetch("https://
+wat.wat", { "headers": { "x-test": "foo" } }).then((res)=>res.json()); ``` ##
+Table Test
 a                b              c            d
                                              this is actually in the cell to
                                              the right, but pandoc seems to
 table _body_     * table bullet ``` test ``` think the prior one is part of a
                                              code block. if you want more
                                              insanity, put a code block in the
                                              same cell as the bullet
```

### Comparing `limberer-0.2.1/src/limberer/static/sections/example2.md` & `limberer-0.2.2/src/limberer/static/sections/example2.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 columns: true
 ---
 
 ## AAA
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam volutpat faucibus vestibulum.
 Mauris varius orci quam. Nam dui mauris, dictum at elementum at, mollis pulvinar est.
-Nunc lobortis pharetra erat, id rutrum lorem malesuada in.
+Nunc lobortis pharetra erat, id rutrum lorem malesuada in.[^ccc]
+
+[^ccc]: foo
 
 ## BBB
 
 Phasellus id nisl nec arcu tempor ultricies non id tortor. Mauris ex nibh, viverra vitae nisi eget, placerat pharetra est.
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed id maximus diam. Cras molestie nisl vitae iaculis convallis.
 Vivamus molestie vitae nisl sed interdum. Nunc aliquam massa rhoncus finibus convallis.
 Vivamus sed vulputate risus. Nunc dignissim magna velit, quis lobortis ex volutpat eget.
-Proin dictum mauris condimentum consequat faucibus.
+Proin dictum mauris condimentum consequat faucibus.[^2]
+
+[^2]: bar
 
 ## CCC
 
 * Foo
 * Bar
 * Baz
```

### Comparing `limberer-0.2.1/src/limberer/static/templates/cover.html` & `limberer-0.2.2/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.1/src/limberer/static/templates/toc.html` & `limberer-0.2.2/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.1/src/limberer.egg-info/PKG-INFO` & `limberer-0.2.2/src/limberer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.1/src/limberer.egg-info/SOURCES.txt` & `limberer-0.2.2/src/limberer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

