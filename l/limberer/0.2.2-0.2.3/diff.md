# Comparing `tmp/limberer-0.2.2.tar.gz` & `tmp/limberer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.2.2.tar", last modified: Mon Jul  3 07:51:54 2023, max compression
+gzip compressed data, was "limberer-0.2.3.tar", last modified: Mon Jul  3 10:29:43 2023, max compression
```

## Comparing `limberer-0.2.2.tar` & `limberer-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.2/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.2/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.2/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 07:51:54.930336 limberer-0.2.2/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.2/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1121 2023-07-03 06:56:58.000000 limberer-0.2.2/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 07:51:54.930336 limberer-0.2.2/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.926336 limberer-0.2.2/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.926336 limberer-0.2.2/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    10256 2023-07-03 07:50:53.000000 limberer-0.2.2/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5507 2023-07-03 07:10:09.000000 limberer-0.2.2/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1101 2023-06-28 10:57:50.000000 limberer-0.2.2/src/limberer/static/assets/base.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-06-28 10:57:50.000000 limberer-0.2.2/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3582 2023-07-03 07:41:04.000000 limberer-0.2.2/src/limberer/static/assets/theme.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.2/src/limberer/static/custom/custom.css
--rw-r--r--   0 jtd       (1000) jtd       (1000)      282 2023-06-28 04:38:31.000000 limberer-0.2.2/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1210 2023-07-03 07:49:39.000000 limberer-0.2.2/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 07:49:42.000000 limberer-0.2.2/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 07:49:58.000000 limberer-0.2.2/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.2/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      300 2023-07-03 07:49:52.000000 limberer-0.2.2/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.2/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 07:51:54.930336 limberer-0.2.2/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      738 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 07:51:54.000000 limberer-0.2.2/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.690171 limberer-0.2.3/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.3/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.3/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.3/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 10:29:43.690171 limberer-0.2.3/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.3/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1096 2023-07-03 09:00:08.000000 limberer-0.2.3/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 10:29:43.690171 limberer-0.2.3/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.686171 limberer-0.2.3/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.686171 limberer-0.2.3/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    10632 2023-07-03 10:26:57.000000 limberer-0.2.3/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5507 2023-07-03 07:10:09.000000 limberer-0.2.3/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.690171 limberer-0.2.3/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.690171 limberer-0.2.3/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1101 2023-07-03 09:59:46.000000 limberer-0.2.3/src/limberer/static/assets/base.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.2.3/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3918 2023-07-03 10:28:48.000000 limberer-0.2.3/src/limberer/static/assets/theme.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.690171 limberer-0.2.3/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.3/src/limberer/static/custom/custom.css
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      282 2023-06-28 04:38:31.000000 limberer-0.2.3/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.690171 limberer-0.2.3/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1401 2023-07-03 10:28:15.000000 limberer-0.2.3/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 07:49:42.000000 limberer-0.2.3/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.690171 limberer-0.2.3/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 07:49:58.000000 limberer-0.2.3/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.3/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-03 10:28:22.000000 limberer-0.2.3/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.3/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 10:29:43.686171 limberer-0.2.3/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 10:29:43.000000 limberer-0.2.3/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      738 2023-07-03 10:29:43.000000 limberer-0.2.3/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 10:29:43.000000 limberer-0.2.3/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 10:29:43.000000 limberer-0.2.3/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 10:29:43.000000 limberer-0.2.3/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 10:29:43.000000 limberer-0.2.3/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.2.2/LICENSE` & `limberer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/PKG-INFO` & `limberer-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.2/README.md` & `limberer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/pyproject.toml` & `limberer-0.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [project]
 name = "limberer"
-# alternatively, limberr
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
```

### Comparing `limberer-0.2.2/src/limberer/__init__.py` & `limberer-0.2.3/src/limberer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,18 @@
                       help="Name of project to create.")
   create.add_argument('-t', '--template', metavar='<path>', type=str,
                       default="",
                       help='Create from alternative template path instead of the built-in default.')
   build = subparsers.add_parser('build')
   parser.add_argument('-d', '--debug', action='store_true',
                       help='Debug output.')
+  build.add_argument('-E', '--emit-html', metavar='<path>', type=str,
+                     default="",
+                     help='Emit post-processed HTML to <path>.')
+
   build.add_argument('config', metavar='<config>', type=str,
                       help="Path to document toml configuration file.")
   args = parser.parse_args()
   return args
 
 def main():
   args = parse_args()
@@ -229,29 +233,30 @@
       soup = BeautifulSoup(html, 'html.parser')
       _fns = soup.find(id="footnotes")
       if _fns is not None:
         _fns = _fns.extract()
         _fns.ol['start'] = str(footnotecount)
         _fns.ol['style'] = f"counter-reset:list-item {footnotecount}; counter-increment:list-item -1;"
         __fns = [c for c in _fns.ol.children if c != "\n"]
-        footnotecount += len(__fns)
         del _fns['id']
         for __fn in __fns:
           id = __fn['id']
           nid = section_name + "-" + id
           __fn['id'] = nid
           __fnx = soup.find(id=id)
           if __fnx is not None:
             __fnx['id'] = nid
         for _a in soup.find_all(class_="footnote-ref"):
           _a['id'] = section_name + "-" + _a['id']
           _a['href'] = '#' + section_name + "-" + _a['href'][1:]
-          print(_a)
+          _a.sup.string = str(footnotecount - 1 + int(_a.sup.string))
         for _a in _fns.find_all(class_="footnote-back"):
           _a['href'] = '#' + section_name + "-" + _a['href'][1:]
+        _fns.name = 'div'
+        footnotecount += len(__fns)
 
         footnotes = str(_fns)
         html = str(soup)
 
       opts['html'] = html
       opts['footnotes'] = footnotes
       opts['opts'] = opts # we occasionally need top.down.variable.paths to resolve abiguity
@@ -282,14 +287,19 @@
         body += "\n"
 
   config['body'] = body
   report_html = chevron.render(base_template, config)
 
   if args.debug:
     print(report_html)
+  if args.emit_html != "":
+    with open(args.emit_html, 'w') as fd:
+      fd.write(report_html)
+      fd.flush()
+      fd.close()
 
   h = weasyprint.HTML(string=report_html, base_url='./', url_fetcher=fetcher)
   h.write_pdf("./" + '.pdf'.join(fname.rsplit('.toml', 1)))
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `limberer-0.2.2/src/limberer/pf.py` & `limberer-0.2.3/src/limberer/pf.py`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/src/limberer/static/assets/base.css` & `limberer-0.2.3/src/limberer/static/assets/base.css`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/src/limberer/static/assets/logo.svg` & `limberer-0.2.3/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/src/limberer/static/assets/theme.css` & `limberer-0.2.3/src/limberer/static/assets/theme.css`

 * *Files 12% similar despite different names*

```diff
@@ -186,14 +186,26 @@
   align-items: flex-start;
   justify-content: center;
   position: absolute;
   bottom: 0px;
   width: 100%;
 }
 
+article {
+  display: flex;
+  flex-direction: column;
+  height: 8.5in;
+  width: 6.5in;
+}
+
+article>div.article-body {
+  width: 6.5in;
+  flex: 1 1 auto;
+}
+
 article ul {
   list-style: none;
   padding-left: 0;
 }
 
 /*weasyprint currently gets this wrong: https://github.com/Kozea/WeasyPrint/issues/1557*/
 article ol {
@@ -213,25 +225,37 @@
   color: #E6E6FA;
   content: '• ';
   font-size: 10pt;
   padding-right: 1em;
 }
 
 .footnotes {
-  position: absolute;
-  width: 100%;
-  bottom: 0;
+  width: 6.5in;
+  flex: 0 1in auto;
+  min-height: 4rem;
+}
+
+.footnotes hr {
+  border: 1px solid black;
 }
 
 .footnotes ol {
-  padding-left: 0;
-  margin-left: 0;
+  padding-left: 0rem;
+  margin-left: 1.5rem;
 }
 
 .footnotes ol li {
   line-height: 1;
 }
 .footnotes ol li::before {
   content: none;
   line-height: 1;
 }
 
+.footnote-ref {
+  text-decoration: none;
+  color: inherit;
+}
+.footnote-back {
+  text-decoration: none;
+  color: inherit;
+}
```

### Comparing `limberer-0.2.2/src/limberer/static/sections/example.md` & `limberer-0.2.3/src/limberer/static/sections/example.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 ### Not in the ToC due to H3
 
 Hi there.
 
 * some[^aaa]
 * bullets[^bbb]
-* <a href="#example">#Example</a>
-* <a href="#wat" class="title"></a>
+* <a href="#example">#Example</a>[^ccc]
+* <a href="#wat" class="title"></a>[^ddd]
 
 [^aaa]: <https://example.com>
 [^bbb]: wat
+[^ccc]: wat2<br>foo
+[^ddd]: wat3
 
 ## Code Snippet
 
 ```js
 let j = await fetch("https://wat.wat", {
   "headers": {
     "x-test": "foo"
@@ -41,27 +43,32 @@
   </thead>
   <tbody>
     <tr>
       <td>table _body_</td>
       <td>
 * table bullet
       </td>
-      <td>
+<td>
 ```
 test
 ```
 </td>
-      <td>this is actually in the cell to the right, but pandoc seems to think the prior one is part of a code block. if you want more insanity, put a code block in the same cell as the bullet</td>
+      <td>if we place the above `<td>`/`</td>` for the previous cell _with indentation_, pandoc breaks down</td>
     </tr>
     <tr>
       <td>Test</td><td>Hello; world!</td><td></td><td></td>
     </tr>
     <tr>
-      <td><ol><li>Table list</li><li>foo</li></ol></td>
-      <td></td><td></td><td></td>
+      <td><ol><li>Table list</li><li>foo</li></ol></td><td></td><td></td><td></td>
+    </tr>
+    <tr>
+      <td><ol><li>Table list</li><li>foo</li></ol></td><td></td><td></td><td></td>
+    </tr>
+    <tr>
+      <td><ol><li>Table list</li><li>foo</li></ol></td><td></td><td></td><td></td>
     </tr>
     <tr>
-      <td></td><td></td><td></td><td></td>
+      <td><ol><li>Table list</li><li>foo</li></ol></td><td></td><td></td><td></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 --- toc_header_level: 2 --- # Examplely Example
 ***** Hello World - not picked up by the ToC due to inline html *****
 ### Not in the ToC due to H3 Hi there. * some[^aaa] * bullets[^bbb] * #Example
-*  [^aaa]:
-example.com> [^bbb]: wat ## Code Snippet ```js let j = await fetch("https://
-wat.wat", { "headers": { "x-test": "foo" } }).then((res)=>res.json()); ``` ##
-Table Test
+[^ccc] * [^ddd] [^aaa]:
+example.com> [^bbb]: wat [^ccc]: wat2
+foo [^ddd]: wat3 ## Code Snippet ```js let j = await fetch("https://wat.wat",
+{ "headers": { "x-test": "foo" } }).then((res)=>res.json()); ``` ## Table Test
 a                b              c            d
-                                             this is actually in the cell to
-                                             the right, but pandoc seems to
-table _body_     * table bullet ``` test ``` think the prior one is part of a
-                                             code block. if you want more
-                                             insanity, put a code block in the
-                                             same cell as the bullet
+table _body_     * table bullet ``` test ``` if we place the above ` `/`
 Test             Hello; world!
    1. Table list
    2. foo
+   1. Table list
+   2. foo
+   1. Table list
+   2. foo
+   1. Table list
+   2. foo
```

### Comparing `limberer-0.2.2/src/limberer/static/sections/example2.md` & `limberer-0.2.3/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/src/limberer/static/templates/cover.html` & `limberer-0.2.3/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/src/limberer/static/templates/toc.html` & `limberer-0.2.3/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.2/src/limberer.egg-info/PKG-INFO` & `limberer-0.2.3/src/limberer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.2/src/limberer.egg-info/SOURCES.txt` & `limberer-0.2.3/src/limberer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

