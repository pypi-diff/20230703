# Comparing `tmp/sqscraper-0.5.0.tar.gz` & `tmp/sqscraper-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqscraper-0.5.0.tar", last modified: Mon Jun 26 20:10:38 2023, max compression
+gzip compressed data, was "sqscraper-0.6.0.tar", last modified: Mon Jul  3 18:52:42 2023, max compression
```

## Comparing `sqscraper-0.5.0.tar` & `sqscraper-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.641201 sqscraper-0.5.0/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     2312 2023-06-26 20:10:38.640201 sqscraper-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.5.0/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-26 20:09:25.000000 sqscraper-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 20:10:38.641201 sqscraper-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.422496 sqscraper-0.5.0/sqscraper/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.5.0/sqscraper/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.5.0/sqscraper/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.591949 sqscraper-0.5.0/sqscraper/cnbc/
--rw-rw-rw-   0        0        0      117 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/cnbc/__init__.py
--rw-rw-rw-   0        0        0      931 2023-06-20 22:50:22.000000 sqscraper-0.5.0/sqscraper/cnbc/_apps.py
--rw-rw-rw-   0        0        0    12837 2023-06-22 23:17:14.000000 sqscraper-0.5.0/sqscraper/cnbc/_serializer.py
--rw-rw-rw-   0        0        0    17770 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/cnbc/charts.py
--rw-rw-rw-   0        0        0    13041 2023-06-22 23:17:14.000000 sqscraper-0.5.0/sqscraper/cnbc/quote_page.py
--rw-rw-rw-   0        0        0    15205 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/cnbc/summary.py
--rw-rw-rw-   0        0        0      739 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.469369 sqscraper-0.5.0/sqscraper.egg-info/
--rw-rw-rw-   0        0        0     2312 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      483 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 18:52:42.670094 sqscraper-0.6.0/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2210 2023-07-03 18:52:42.670094 sqscraper-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.6.0/README.md
+-rw-rw-rw-   0        0        0     1897 2023-07-03 18:51:27.000000 sqscraper-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 18:52:42.670094 sqscraper-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 18:52:42.634238 sqscraper-0.6.0/sqscraper/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.6.0/sqscraper/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.6.0/sqscraper/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:52:42.670094 sqscraper-0.6.0/sqscraper/cnbc/
+-rw-rw-rw-   0        0        0      154 2023-07-03 18:51:02.000000 sqscraper-0.6.0/sqscraper/cnbc/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-06-20 22:50:22.000000 sqscraper-0.6.0/sqscraper/cnbc/_apps.py
+-rw-rw-rw-   0        0        0    12837 2023-06-22 23:17:14.000000 sqscraper-0.6.0/sqscraper/cnbc/_serializer.py
+-rw-rw-rw-   0        0        0    17770 2023-06-26 20:09:10.000000 sqscraper-0.6.0/sqscraper/cnbc/charts.py
+-rw-rw-rw-   0        0        0     8922 2023-07-03 18:51:02.000000 sqscraper-0.6.0/sqscraper/cnbc/earnings.py
+-rw-rw-rw-   0        0        0    13041 2023-06-22 23:17:14.000000 sqscraper-0.6.0/sqscraper/cnbc/quote_page.py
+-rw-rw-rw-   0        0        0    15026 2023-07-03 18:51:02.000000 sqscraper-0.6.0/sqscraper/cnbc/summary.py
+-rw-rw-rw-   0        0        0      739 2023-06-26 20:09:10.000000 sqscraper-0.6.0/sqscraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:52:42.648375 sqscraper-0.6.0/sqscraper.egg-info/
+-rw-rw-rw-   0        0        0     2210 2023-07-03 18:52:42.000000 sqscraper-0.6.0/sqscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-03 18:52:42.000000 sqscraper-0.6.0/sqscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 18:52:42.000000 sqscraper-0.6.0/sqscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      483 2023-07-03 18:52:42.000000 sqscraper-0.6.0/sqscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 18:52:42.000000 sqscraper-0.6.0/sqscraper.egg-info/top_level.txt
```

### Comparing `sqscraper-0.5.0/LICENSE` & `sqscraper-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqscraper-0.5.0/PKG-INFO` & `sqscraper-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.5.0
+Version: 0.6.0
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,19 +29,17 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQScraper
```

### Comparing `sqscraper-0.5.0/pyproject.toml` & `sqscraper-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqscraper"
-version = "0.5.0"
+version = "0.6.0"
 description = "API wrapper and web scraper for select stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Financial and Insurance Industry",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development"
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 dependencies = [
     "beautifulsoup4==4.12.2",
     "certifi==2023.5.7 ; python_version >= '3.6'",
     "charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'",
     "html5lib==1.1",
     "idna==3.4 ; python_version >= '3.5'",
     "lxml==4.9.2",
```

### Comparing `sqscraper-0.5.0/sqscraper/cnbc/_apps.py` & `sqscraper-0.6.0/sqscraper/cnbc/_apps.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.5.0/sqscraper/cnbc/_serializer.py` & `sqscraper-0.6.0/sqscraper/cnbc/_serializer.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.5.0/sqscraper/cnbc/charts.py` & `sqscraper-0.6.0/sqscraper/cnbc/charts.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.5.0/sqscraper/cnbc/quote_page.py` & `sqscraper-0.6.0/sqscraper/cnbc/quote_page.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.5.0/sqscraper/cnbc/summary.py` & `sqscraper-0.6.0/sqscraper/cnbc/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,54 +299,52 @@
     @property
     def _javascript(self) -> str:
         """
         """
         for element in self._soup.select(
             "div#category > div.subsection > script[type='text/javascript']"
         ):
-            if re.search(r"j1=\[\];.*var growthData=j1;", element.text) is not None:
+            if re.search(r"j1=\[\];", element.text) is not None:
                 return element.text.strip()
         raise ValueError
 
     def _scrape_chart_data(self) -> typing.List[pd.DataFrame]:
         """
         :return:
         """
         data = []
         regex = [
             re.compile(r"^j1=\[\]$"),
             re.compile(r"^j1\[\d\]=\{\}$"),
-            re.compile(r"^j1\[(\d)\]\.name=(.*?)$"),
-            re.compile(r"^j1\[(\d)\]\.prefix=(.*?)$"),
-            re.compile(r"^j1\[(\d)\]\.years=\[\]$"),
-            re.compile(r"^j1\[(\d)\]\.years\[\d\]=\{\}$"),
-            re.compile(r"^j1\[(\d)\]\.years\[(\d)\]\.(.*?)=(.*?)$")
+            re.compile(r"^j1\[(\d)\]\.(.*?)=\"?(.*?)\"?$"),
+            re.compile(r"^j1\[(\d)\]\.(.*?)=\[\]$"),
+            re.compile(r"^j1\[(\d)\]\.(.*?)\[\d\]=\{\}$"),
+            re.compile(r"^j1\[(\d)\]\.(.*?)\[(\d)\]\.(.*?)=\"?(.*?)\"?$")
         ]
+
         for statement in self._javascript.split(";"):
             results = [r.search(statement) for r in regex]
-            nonnull_results = [(i, x) for i, x in enumerate(results) if x is not None]
+            nonnull_results = [(i, x) for (i, x) in enumerate(results) if x is not None]
             if len(nonnull_results) != 1:
                 continue
             idx, res = nonnull_results[0]
 
             if idx == 0:
                 continue
             elif idx == 1:
                 data.append({})
             elif idx == 2:
-                data[int(res.group(1))].setdefault("name", res.group(2).strip("\""))
+                data[int(res.group(1))].setdefault(res.group(2), res.group(3))
             elif idx == 3:
-                data[int(res.group(1))].setdefault("profile", res.group(2).strip("\""))
+                data[int(res.group(1))].setdefault(res.group(2), [])
             elif idx == 4:
-                data[int(res.group(1))].setdefault("years", [])
+                data[int(res.group(1))][res.group(2)].append({})
             elif idx == 5:
-                data[int(res.group(1))]["years"].append({})
-            elif idx == 6:
-                data[int(res.group(1))]["years"][int(res.group(2))].setdefault(
-                    res.group(3), res.group(4).strip("\"")
+                data[int(res.group(1))][res.group(2)][int(res.group(3))].setdefault(
+                    res.group(4), res.group(5)
                 )
 
         dataframes = []
         for i, record in enumerate(data):
             dataframes.append(
                 pd.DataFrame({int(x["FiscalYear"]): x for x in record["years"]})
             )
```

### Comparing `sqscraper-0.5.0/sqscraper/utils.py` & `sqscraper-0.6.0/sqscraper/utils.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.5.0/sqscraper.egg-info/PKG-INFO` & `sqscraper-0.6.0/sqscraper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.5.0
+Version: 0.6.0
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,19 +29,17 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQScraper
```

