# Comparing `tmp/python-dict-display-filter-0.9.8.tar.gz` & `tmp/python-dict-display-filter-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dict-display-filter-0.9.8.tar", last modified: Sun Jul  2 14:31:04 2023, max compression
+gzip compressed data, was "python-dict-display-filter-0.9.9.tar", last modified: Mon Jul  3 09:17:23 2023, max compression
```

## Comparing `python-dict-display-filter-0.9.8.tar` & `python-dict-display-filter-0.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/LICENSE
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4177 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3723 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/README.md
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/pydictdisplayfilter/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10804 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/display_filters.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/exceptions.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/factories.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8057 2023-07-02 13:18:01.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/helpers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/models.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4311 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7361 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/slicers.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4177 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      856 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       93 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/requires.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/top_level.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/setup.cfg
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1001 2023-06-30 10:16:10.000000 python-dict-display-filter-0.9.8/setup.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/tests/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/tests/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10562 2023-06-30 09:43:27.000000 python-dict-display-filter-0.9.8/tests/test_dict_display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6105 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/tests/test_display_filter_parser.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/tests/test_slicers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7550 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.8/tests/test_sql_display_filter.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/LICENSE
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4656 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4202 2023-07-03 09:14:46.000000 python-dict-display-filter-0.9.9/README.md
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/pydictdisplayfilter/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    10804 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/display_filters.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/exceptions.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/factories.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7661 2023-07-02 17:42:15.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/helpers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/models.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4311 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7361 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/slicers.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4656 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      856 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       93 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/requires.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/top_level.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/setup.cfg
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1001 2023-07-02 17:35:40.000000 python-dict-display-filter-0.9.9/setup.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/tests/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/tests/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    10562 2023-06-30 09:43:27.000000 python-dict-display-filter-0.9.9/tests/test_dict_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6105 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/tests/test_display_filter_parser.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/tests/test_slicers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7550 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.9/tests/test_sql_display_filter.py
```

### Comparing `python-dict-display-filter-0.9.8/LICENSE` & `python-dict-display-filter-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/PKG-INFO` & `python-dict-display-filter-0.9.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,84 @@
-Metadata-Version: 2.1
-Name: python-dict-display-filter
-Version: 0.9.8
-Summary: A Wireshark-like display filter for dictionaries.
-Home-page: https://github.com/bytebutcher/python-dict-display-filter
-Author: bytebutcher
-Author-email: thomas.engel.web@gmail.com
-License: GPL-3.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
     <img src="https://github.com/bytebutcher/python-dict-display-filter/raw/main/images/python_dict_display_filter_logo.png" alt="python_dict_display_filter Logo"/>
 </p>
 <h1 align="center" style="margin-top: 0px;">Python Dictionary Display Filter</h1>
 <div align="center">
 
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
-Wireshark-like display filter for python dictionaries.
+A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
+manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
+combining operators, membership operators, and more. 
+
+## Table of Contents
+1. [Quick Start](#quick-start)
+2. [Usage](#usage)
+3. [Features](#features)
+4. [Examples](#examples)
+5. [Acknowledgements](#acknowledgements)
+
+## Quick Start
+
+Here's a simple example to get you started. First, install the package:
 
-## Setup
 ```commandline
 pip3 install python-dict-display-filter
 ```
 
-## Usage
+Then, use it to filter a list of dictionaries:
+```
+from pydictdisplayfilter import DictDisplayFilter
+actors = [
+    {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
+    {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
+    {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"}, "gender": "male"},
+    {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
+]
+ddf = DictDisplayFilter(actors)
 
-The basics and the syntax of the display filter are described in the 
-<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
+# This will filter the list to show only male actors born between 1960 and 1965 whose names end with 'e'
+filtered_actors = ddf.filter("gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$")
 
-If you want to see some advanced examples of how ```python-dict-display-filter``` can be put to use checkout the 
-<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md">Examples</a>.
+print(list(filtered_actors))
+[{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
+```
 
-If you want to use ```python-dict-display-filter``` in your own application and customize it to your needs 
-check out the 
-<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/DEVELOPER_GUIDE.md">Developer Guide</a>.
+For more details, please refer to the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Features
-The following overview shows all the supported features of the display filter:
+
+Python Dictionary Display Filter supports a wide range of features, including:
 * **Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```, ```~=```, ```~```, ```&```
 * **Combining Operators:** ```and```, ```or```, ```xor```, ```not``` 
 * **Membership Operators:** ```in```
 * **Types:** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Functions:** ```upper```, ```lower```, ```len```
+* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite```
 
 For a detailed description of the individual features check out the
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Examples 
 
-Initialize ```DictDisplayFilter``` with a list of dictionaries:
-```
-> from pydictdisplayfilter import DictDisplayFilter
-> actors = [
-    {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
-    {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
-    {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"}, "gender": "male"},
-    {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
-]
-> ddf = DictDisplayFilter(actors)
-```
-
-Show only actors with some kind of super-power:
-```
-> ddf.filter("power")
-```
-
-Show only actors which were born before 1965:
-```
-> ddf.filter("age.born < 1965")
-```
-
-Show only female actors:
-```
-> ddf.filter("gender == female")
-```
-
-Show all male actors which are born between 1960 and 1965:
-```
-> ddf.filter("gender == male and (age.born > 1960 and age.born < 1965)")
-```
-
-Show all actors which name contain the character 'e':
-```
-> ddf.filter("name contains e")
-```
+For detailed examples of how the display filter can be utilized, please refer to the following:
 
-Show all actors which name matches a regular expression:
-```
-> ddf.filter("name matches .*e$")
-```
-
-## Inspired by
+* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-filter)
+* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter)
+* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#sqlite-display-filter)
+* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#nmap-display-filter)
 
-* <a href="https://wiki.wireshark.org/DisplayFilters">Wireshark Display Filter</a>
+## Acknowledgements
 
-## Powered by
+This project wouldn't be possible without these awesome projects:
 
+* <a href="https://wiki.wireshark.org/DisplayFilters">wireshark display filter</a>: Display filter for filtering network packages
 * <a href="https://github.com/wolever/parameterized">parameterized</a>: Parameterized testing with any Python test framework
 * <a href="https://github.com/pyparsing/pyparsing/">pyparsing</a>: Creating PEG-parsers made easy
 * <a href="https://github.com/bytebutcher/ipranger/">ipranger</a>: Parsing and matching IPv4-addresses
 * <a href="https://pypi.org/project/python-dateutil/">python-dateutil</a>: Parsing and comparing dates 
-
-
```

#### html2text {}

```diff
@@ -1,44 +1,48 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.8 Summary:
-A Wireshark-like display filter for dictionaries. Home-page: https://
-github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
-email: thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
 
-Wireshark-like display filter for python dictionaries. ## Setup ```commandline
-pip3 install python-dict-display-filter ``` ## Usage The basics and the syntax
-of the display filter are described in the User_Guide. If you want to see some
-advanced examples of how ```python-dict-display-filter``` can be put to use
-checkout the Examples. If you want to use ```python-dict-display-filter``` in
-your own application and customize it to your needs check out the Developer
-Guide. ## Features The following overview shows all the supported features of
-the display filter: * **Comparison Operators:** ```==```, ```!=```, ```<=```,
-```<```, ```>=```, ```>```, ```~=```, ```~```, ```&``` * **Combining Operators:
-** ```and```, ```or```, ```xor```, ```not``` * **Membership Operators:**
-```in``` * **Types:** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-
-```, ```IPv4-```, ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-
-```, ```IPv4-```, ```IPv6-Address``` * **Functions:** ```upper```, ```lower```,
-```len``` For a detailed description of the individual features check out the
-User_Guide. ## Examples Initialize ```DictDisplayFilter``` with a list of
-dictionaries: ``` > from pydictdisplayfilter import DictDisplayFilter > actors
-= [ {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender":
-"male"}, {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender":
-"male", "power": ["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"],
-"age": {"born": "1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"],
-"age": {"born": "1967"}, "gender": "female"} ] > ddf = DictDisplayFilter
-(actors) ``` Show only actors with some kind of super-power: ``` > ddf.filter
-("power") ``` Show only actors which were born before 1965: ``` > ddf.filter
-("age.born < 1965") ``` Show only female actors: ``` > ddf.filter("gender ==
-female") ``` Show all male actors which are born between 1960 and 1965: ``` >
-ddf.filter("gender == male and (age.born > 1960 and age.born < 1965)") ``` Show
-all actors which name contain the character 'e': ``` > ddf.filter("name
-contains e") ``` Show all actors which name matches a regular expression: ``` >
-ddf.filter("name matches .*e$") ``` ## Inspired by * Wireshark_Display_Filter
-## Powered by * parameterized: Parameterized testing with any Python test
-framework * pyparsing: Creating PEG-parsers made easy * ipranger: Parsing and
-matching IPv4-addresses * python-dateutil: Parsing and comparing dates
+A Wireshark-like display filter for Python dictionaries. This tool allows you
+to easily filter, analyze, and manipulate data in Python dictionaries. It
+offers a range of features including comparison operators, combining operators,
+membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
+start) 2. [Usage](#usage) 3. [Features](#features) 4. [Examples](#examples) 5.
+[Acknowledgements](#acknowledgements) ## Quick Start Here's a simple example to
+get you started. First, install the package: ```commandline pip3 install
+python-dict-display-filter ``` Then, use it to filter a list of dictionaries:
+``` from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
+["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
+["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
+["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
+"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
+"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) # This will
+filter the list to show only male actors born between 1960 and 1965 whose names
+end with 'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960
+and age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [
+{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
+``` For more details, please refer to the User_Guide. ## Features Python
+Dictionary Display Filter supports a wide range of features, including: *
+**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
+```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
+```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
+** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
+```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
+**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
+detailed description of the individual features check out the User_Guide. ##
+Examples For detailed examples of how the display filter can be utilized,
+please refer to the following: * [CSV Display Filter](https://github.com/
+bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
+filter) * [JSON Display Filter](https://github.com/bytebutcher/python-dict-
+display-filter/blob/main/docs/EXAMPLES.md#json-display-filter) * [SQLite
+Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/
+main/docs/EXAMPLES.md#sqlite-display-filter) * [Nmap Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+EXAMPLES.md#nmap-display-filter) ## Acknowledgements This project wouldn't be
+possible without these awesome projects: * wireshark_display_filter: Display
+filter for filtering network packages * parameterized: Parameterized testing
+with any Python test framework * pyparsing: Creating PEG-parsers made easy *
+ipranger: Parsing and matching IPv4-addresses * python-dateutil: Parsing and
+comparing dates
```

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/__init__.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/display_filters.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/display_filters.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/__init__.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/common.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/exceptions.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/factories.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/factories.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/helpers.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,58 +11,56 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import cmd
-import itertools
 import logging
 import os
 import time
 import traceback
-from typing import List, Set
+from typing import List
 
-from pydictdisplayfilter import DictDisplayFilter
-from pydictdisplayfilter.display_filters import BaseDisplayFilter
+from pydictdisplayfilter.display_filters import BaseDisplayFilter, DictDisplayFilter
 from pydictdisplayfilter.exceptions import ParserError, EvaluationError
 
 
 class TableError(Exception):
     pass
 
 
 class Table:
     """ Data store with filter capabilities and pretty table printout. """
 
     def __init__(self, display_filter: BaseDisplayFilter):
         self._display_filter = display_filter
 
-    def _make_table(self, data_store) -> List[str]:
+    def _make_table(self, data_store: List[dict]) -> List[str]:
         """ Creates a table including header from the data store. """
         if not data_store:
             return []
         table = [self.fields()]
         column_size = self._calculate_column_size(data_store)
         format_str = ' | '.join(["{{:<{}}}".format(i) for i in column_size])
         for item in data_store:
             table.append(item.values())
         column_size = self._calculate_column_size(data_store)
         table.insert(1, ['-' * i for i in column_size]) # Separating line
         return [""] + [ format_str.format(*item) for item in table ]
 
-    def _calculate_column_size(self, data_store) -> List[int]:
+    def _calculate_column_size(self, data_store: List[dict]) -> List[int]:
         """ Calculates and returns the necessary size of each column in the data store. """
         header = list(data_store[0].keys())
         items = [list(item.values()) for item in data_store]
         return [
             max(len(str(item)) for item in column) for column in zip(*items + [header])
         ]
 
-    def _make_footer(self, items, duration) -> List[str]:
+    def _make_footer(self, items: List[dict], duration: float) -> List[str]:
         """ Creates a footer for the table which prints some statistics. """
         item_count = len(items)
         result = [""]
         if item_count == 0:
             result.append("Empty set ({:.2f} secs)".format(duration))
         else:
             type_name = "row" if item_count == 1 else "rows"
@@ -180,29 +178,21 @@
     """ Data store with filter capabilities and pretty table printout. """
 
     def __init__(self, data_store: List[dict]):
         """ Initializes the DictTable with a data store. """
         self._data_store = data_store
         super().__init__(DictDisplayFilter(data_store))
 
-    def fields(self, thorough: bool = False) -> List[str]:
-        """
-        Returns the field names used in the data store.
-        :param thorough: if enabled, scans each item in the data store for its field names, otherwise only the first
-                         item is looked upon which is usually enough. Disabled by default.
-        """
+    def fields(self) -> List[str]:
+        """ Returns the field names used in the data store. """
         if not self._data_store:
             # No items in data store, so there are no fields to query either.
             return list()
-
-        if not thorough:
-            return list(self._data_store[0].keys())
-        else:
-            return itertools.chain.from_iterable([item.keys() for item in self._data_store])
+        return list(self._data_store[0].keys())
 
 
 class DictDisplayFilterShell(DisplayFilterShell):
     """ A little shell for querying a list of dictionaries using the display filter. """
 
     def __init__(self, data_store: List[dict]):
         """ Initializes the DictDisplayFilterShell with a data store. """
-        super().__init__(DictTable(data_store))
+        super().__init__(DictTable(data_store))
```

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/models.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/models.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/__init__.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/common.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/display_filter.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/pydictdisplayfilter/slicers.py` & `python-dict-display-filter-0.9.9/pydictdisplayfilter/slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/PKG-INFO` & `python-dict-display-filter-0.9.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -20,94 +20,81 @@
 
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
-Wireshark-like display filter for python dictionaries.
+A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
+manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
+combining operators, membership operators, and more. 
+
+## Table of Contents
+1. [Quick Start](#quick-start)
+2. [Usage](#usage)
+3. [Features](#features)
+4. [Examples](#examples)
+5. [Acknowledgements](#acknowledgements)
+
+## Quick Start
+
+Here's a simple example to get you started. First, install the package:
 
-## Setup
 ```commandline
 pip3 install python-dict-display-filter
 ```
 
-## Usage
+Then, use it to filter a list of dictionaries:
+```
+from pydictdisplayfilter import DictDisplayFilter
+actors = [
+    {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
+    {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
+    {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"}, "gender": "male"},
+    {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
+]
+ddf = DictDisplayFilter(actors)
 
-The basics and the syntax of the display filter are described in the 
-<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
+# This will filter the list to show only male actors born between 1960 and 1965 whose names end with 'e'
+filtered_actors = ddf.filter("gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$")
 
-If you want to see some advanced examples of how ```python-dict-display-filter``` can be put to use checkout the 
-<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md">Examples</a>.
+print(list(filtered_actors))
+[{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
+```
 
-If you want to use ```python-dict-display-filter``` in your own application and customize it to your needs 
-check out the 
-<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/DEVELOPER_GUIDE.md">Developer Guide</a>.
+For more details, please refer to the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Features
-The following overview shows all the supported features of the display filter:
+
+Python Dictionary Display Filter supports a wide range of features, including:
 * **Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```, ```~=```, ```~```, ```&```
 * **Combining Operators:** ```and```, ```or```, ```xor```, ```not``` 
 * **Membership Operators:** ```in```
 * **Types:** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Functions:** ```upper```, ```lower```, ```len```
+* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite```
 
 For a detailed description of the individual features check out the
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Examples 
 
-Initialize ```DictDisplayFilter``` with a list of dictionaries:
-```
-> from pydictdisplayfilter import DictDisplayFilter
-> actors = [
-    {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
-    {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
-    {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"}, "gender": "male"},
-    {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
-]
-> ddf = DictDisplayFilter(actors)
-```
-
-Show only actors with some kind of super-power:
-```
-> ddf.filter("power")
-```
-
-Show only actors which were born before 1965:
-```
-> ddf.filter("age.born < 1965")
-```
-
-Show only female actors:
-```
-> ddf.filter("gender == female")
-```
-
-Show all male actors which are born between 1960 and 1965:
-```
-> ddf.filter("gender == male and (age.born > 1960 and age.born < 1965)")
-```
-
-Show all actors which name contain the character 'e':
-```
-> ddf.filter("name contains e")
-```
-
-Show all actors which name matches a regular expression:
-```
-> ddf.filter("name matches .*e$")
-```
+For detailed examples of how the display filter can be utilized, please refer to the following:
 
-## Inspired by
+* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-filter)
+* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter)
+* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#sqlite-display-filter)
+* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#nmap-display-filter)
 
-* <a href="https://wiki.wireshark.org/DisplayFilters">Wireshark Display Filter</a>
+## Acknowledgements
 
-## Powered by
+This project wouldn't be possible without these awesome projects:
 
+* <a href="https://wiki.wireshark.org/DisplayFilters">wireshark display filter</a>: Display filter for filtering network packages
 * <a href="https://github.com/wolever/parameterized">parameterized</a>: Parameterized testing with any Python test framework
 * <a href="https://github.com/pyparsing/pyparsing/">pyparsing</a>: Creating PEG-parsers made easy
 * <a href="https://github.com/bytebutcher/ipranger/">ipranger</a>: Parsing and matching IPv4-addresses
 * <a href="https://pypi.org/project/python-dateutil/">python-dateutil</a>: Parsing and comparing dates
```

#### html2text {}

```diff
@@ -1,44 +1,54 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.8 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.9 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
 email: thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
 
-Wireshark-like display filter for python dictionaries. ## Setup ```commandline
-pip3 install python-dict-display-filter ``` ## Usage The basics and the syntax
-of the display filter are described in the User_Guide. If you want to see some
-advanced examples of how ```python-dict-display-filter``` can be put to use
-checkout the Examples. If you want to use ```python-dict-display-filter``` in
-your own application and customize it to your needs check out the Developer
-Guide. ## Features The following overview shows all the supported features of
-the display filter: * **Comparison Operators:** ```==```, ```!=```, ```<=```,
-```<```, ```>=```, ```>```, ```~=```, ```~```, ```&``` * **Combining Operators:
-** ```and```, ```or```, ```xor```, ```not``` * **Membership Operators:**
-```in``` * **Types:** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-
-```, ```IPv4-```, ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-
-```, ```IPv4-```, ```IPv6-Address``` * **Functions:** ```upper```, ```lower```,
-```len``` For a detailed description of the individual features check out the
-User_Guide. ## Examples Initialize ```DictDisplayFilter``` with a list of
-dictionaries: ``` > from pydictdisplayfilter import DictDisplayFilter > actors
-= [ {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender":
-"male"}, {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender":
-"male", "power": ["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"],
-"age": {"born": "1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"],
-"age": {"born": "1967"}, "gender": "female"} ] > ddf = DictDisplayFilter
-(actors) ``` Show only actors with some kind of super-power: ``` > ddf.filter
-("power") ``` Show only actors which were born before 1965: ``` > ddf.filter
-("age.born < 1965") ``` Show only female actors: ``` > ddf.filter("gender ==
-female") ``` Show all male actors which are born between 1960 and 1965: ``` >
-ddf.filter("gender == male and (age.born > 1960 and age.born < 1965)") ``` Show
-all actors which name contain the character 'e': ``` > ddf.filter("name
-contains e") ``` Show all actors which name matches a regular expression: ``` >
-ddf.filter("name matches .*e$") ``` ## Inspired by * Wireshark_Display_Filter
-## Powered by * parameterized: Parameterized testing with any Python test
-framework * pyparsing: Creating PEG-parsers made easy * ipranger: Parsing and
-matching IPv4-addresses * python-dateutil: Parsing and comparing dates
+A Wireshark-like display filter for Python dictionaries. This tool allows you
+to easily filter, analyze, and manipulate data in Python dictionaries. It
+offers a range of features including comparison operators, combining operators,
+membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
+start) 2. [Usage](#usage) 3. [Features](#features) 4. [Examples](#examples) 5.
+[Acknowledgements](#acknowledgements) ## Quick Start Here's a simple example to
+get you started. First, install the package: ```commandline pip3 install
+python-dict-display-filter ``` Then, use it to filter a list of dictionaries:
+``` from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
+["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
+["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
+["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
+"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
+"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) # This will
+filter the list to show only male actors born between 1960 and 1965 whose names
+end with 'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960
+and age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [
+{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
+``` For more details, please refer to the User_Guide. ## Features Python
+Dictionary Display Filter supports a wide range of features, including: *
+**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
+```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
+```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
+** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
+```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
+**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
+detailed description of the individual features check out the User_Guide. ##
+Examples For detailed examples of how the display filter can be utilized,
+please refer to the following: * [CSV Display Filter](https://github.com/
+bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
+filter) * [JSON Display Filter](https://github.com/bytebutcher/python-dict-
+display-filter/blob/main/docs/EXAMPLES.md#json-display-filter) * [SQLite
+Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/
+main/docs/EXAMPLES.md#sqlite-display-filter) * [Nmap Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+EXAMPLES.md#nmap-display-filter) ## Acknowledgements This project wouldn't be
+possible without these awesome projects: * wireshark_display_filter: Display
+filter for filtering network packages * parameterized: Parameterized testing
+with any Python test framework * pyparsing: Creating PEG-parsers made easy *
+ipranger: Parsing and matching IPv4-addresses * python-dateutil: Parsing and
+comparing dates
```

### Comparing `python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/SOURCES.txt` & `python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/setup.py` & `python-dict-display-filter-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="python-dict-display-filter",
-    version="0.9.8",
+    version="0.9.9",
     description="A Wireshark-like display filter for dictionaries.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bytebutcher/python-dict-display-filter",
     author="bytebutcher",
     author_email="thomas.engel.web@gmail.com",
     license="GPL-3.0",
```

### Comparing `python-dict-display-filter-0.9.8/tests/__init__.py` & `python-dict-display-filter-0.9.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/tests/test_dict_display_filter.py` & `python-dict-display-filter-0.9.9/tests/test_dict_display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/tests/test_display_filter_parser.py` & `python-dict-display-filter-0.9.9/tests/test_display_filter_parser.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/tests/test_slicers.py` & `python-dict-display-filter-0.9.9/tests/test_slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.8/tests/test_sql_display_filter.py` & `python-dict-display-filter-0.9.9/tests/test_sql_display_filter.py`

 * *Files identical despite different names*

