# Comparing `tmp/budoux-0.5.1.tar.gz` & `tmp/budoux-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budoux-0.5.1.tar", last modified: Thu Apr 20 03:11:23 2023, max compression
+gzip compressed data, was "budoux-0.5.2.tar", last modified: Mon Jul  3 05:53:46 2023, max compression
```

## Comparing `budoux-0.5.1.tar` & `budoux-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.915552 budoux-0.5.1/
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)    11357 2023-04-20 02:57:14.000000 budoux-0.5.1/LICENSE
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)      129 2023-04-20 02:57:14.000000 budoux-0.5.1/MANIFEST.in
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     9355 2023-04-20 03:11:23.915848 budoux-0.5.1/PKG-INFO
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     8725 2023-04-20 02:57:14.000000 budoux-0.5.1/README.md
-drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.904467 budoux-0.5.1/budoux/
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)      908 2023-04-20 03:11:07.000000 budoux-0.5.1/budoux/__init__.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     3218 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/html_processor.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4977 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/main.py
-drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.909391 budoux-0.5.1/budoux/models/
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)    14434 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/models/ja.json
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)    64385 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/models/zh-hans.json
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)    64671 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/models/zh-hant.json
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4282 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/parser.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/py.typed
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)      124 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/skip_nodes.json
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)      667 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/utils.py
-drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.907347 budoux-0.5.1/budoux.egg-info/
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     9355 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/PKG-INFO
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)      655 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/SOURCES.txt
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)        1 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/dependency_links.txt
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)       44 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/entry_points.txt
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)       77 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/requires.txt
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)       15 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/top_level.txt
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)       90 2023-04-20 02:57:14.000000 budoux-0.5.1/pyproject.toml
-drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.913177 budoux-0.5.1/scripts/
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/__init__.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     3157 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/build_model.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4946 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/encode_data.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4854 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/prepare_knbc.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)    13818 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/train.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     3612 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/translate_model.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     1063 2023-04-20 03:11:23.917767 budoux-0.5.1/setup.cfg
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)      614 2023-04-20 02:57:14.000000 budoux-0.5.1/setup.py
-drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.915032 budoux-0.5.1/tests/
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     2841 2023-04-20 02:57:14.000000 budoux-0.5.1/tests/test_html_processor.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     5601 2023-04-20 02:57:14.000000 budoux-0.5.1/tests/test_main.py
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     5369 2023-04-20 02:57:14.000000 budoux-0.5.1/tests/test_parser.py
+drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:53:46.459712 budoux-0.5.2/
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)    11357 2023-07-03 05:36:07.000000 budoux-0.5.2/LICENSE
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)      129 2023-07-03 05:36:07.000000 budoux-0.5.2/MANIFEST.in
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     9351 2023-07-03 05:53:46.459712 budoux-0.5.2/PKG-INFO
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     8721 2023-07-03 05:36:07.000000 budoux-0.5.2/README.md
+drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:53:46.455711 budoux-0.5.2/budoux/
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)      908 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/__init__.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     3216 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/html_processor.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     4977 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/main.py
+drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:53:46.455711 budoux-0.5.2/budoux/models/
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)    14414 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/models/ja.json
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)    14434 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/models/ja_knbc.json
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)    64385 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/models/zh-hans.json
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)    64671 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/models/zh-hant.json
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     4282 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/parser.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/py.typed
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)      124 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/skip_nodes.json
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)      667 2023-07-03 05:36:07.000000 budoux-0.5.2/budoux/utils.py
+drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:53:46.455711 budoux-0.5.2/budoux.egg-info/
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     9351 2023-07-03 05:53:46.000000 budoux-0.5.2/budoux.egg-info/PKG-INFO
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)      724 2023-07-03 05:53:46.000000 budoux-0.5.2/budoux.egg-info/SOURCES.txt
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)        1 2023-07-03 05:53:46.000000 budoux-0.5.2/budoux.egg-info/dependency_links.txt
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)       44 2023-07-03 05:53:46.000000 budoux-0.5.2/budoux.egg-info/entry_points.txt
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)       71 2023-07-03 05:53:46.000000 budoux-0.5.2/budoux.egg-info/requires.txt
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)       15 2023-07-03 05:53:46.000000 budoux-0.5.2/budoux.egg-info/top_level.txt
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)       90 2023-07-03 05:36:07.000000 budoux-0.5.2/pyproject.toml
+drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:53:46.459712 budoux-0.5.2/scripts/
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:36:07.000000 budoux-0.5.2/scripts/__init__.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     3769 2023-07-03 05:36:07.000000 budoux-0.5.2/scripts/build_model.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     4946 2023-07-03 05:36:07.000000 budoux-0.5.2/scripts/encode_data.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     8536 2023-07-03 05:36:07.000000 budoux-0.5.2/scripts/finetune.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     4854 2023-07-03 05:36:07.000000 budoux-0.5.2/scripts/prepare_knbc.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)    13666 2023-07-03 05:36:07.000000 budoux-0.5.2/scripts/train.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     3612 2023-07-03 05:36:07.000000 budoux-0.5.2/scripts/translate_model.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     1056 2023-07-03 05:53:46.459712 budoux-0.5.2/setup.cfg
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)      614 2023-07-03 05:36:07.000000 budoux-0.5.2/setup.py
+drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2023-07-03 05:53:46.459712 budoux-0.5.2/tests/
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     2833 2023-07-03 05:36:07.000000 budoux-0.5.2/tests/test_html_processor.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     5581 2023-07-03 05:36:07.000000 budoux-0.5.2/tests/test_main.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     5347 2023-07-03 05:36:07.000000 budoux-0.5.2/tests/test_parser.py
+-rw-r-----   0 tushuhei (175101) primarygroup (89939)     1382 2023-07-03 05:36:07.000000 budoux-0.5.2/tests/test_quality.py
```

### Comparing `budoux-0.5.1/LICENSE` & `budoux-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/PKG-INFO` & `budoux-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budoux
-Version: 0.5.1
+Version: 0.5.2
 Summary: BudouX is the successor of Budou
 Author: Shuhei Iitsuka
 Author-email: tushuhei@google.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -94,15 +94,15 @@
 # ['今天', '是', '晴天。']
 ```
 
 You can also translate an HTML string by wrapping phrases with non-breaking markup.
 
 ```python
 print(parser.translate_html_string('今日は<b>とても天気</b>です。'))
-# <span style="word-break: keep-all; overflow-wrap: break-word;">今日は<b ><wbr>とても<wbr>天気</b>です。</span>
+# <span style="word-break: keep-all; overflow-wrap: anywhere;">今日は<b ><wbr>とても<wbr>天気</b>です。</span>
 ```
 
 If you have a custom model, you can use it as follows.
 
 ```python
 with open('/path/to/your/model.json') as f:
   model = json.load(f)
@@ -145,15 +145,15 @@
 ---
 明日は
 曇りでしょう。
 ```
 
 ```shellsession
 $ budoux 本日は晴天です。 -H
-<span style="word-break: keep-all; overflow-wrap: break-word;">本日は<wbr>晴天です。</span>
+<span style="word-break: keep-all; overflow-wrap: anywhere;">本日は<wbr>晴天です。</span>
 ```
 
 If you want to see help, run `budoux -h`.
 
 ```shellsession
 $ budoux -h
 usage: budoux [-h] [-H] [-m JSON | -l LANG] [-d STR] [-V] [TXT]
```

### Comparing `budoux-0.5.1/README.md` & `budoux-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 # ['今天', '是', '晴天。']
 ```
 
 You can also translate an HTML string by wrapping phrases with non-breaking markup.
 
 ```python
 print(parser.translate_html_string('今日は<b>とても天気</b>です。'))
-# <span style="word-break: keep-all; overflow-wrap: break-word;">今日は<b ><wbr>とても<wbr>天気</b>です。</span>
+# <span style="word-break: keep-all; overflow-wrap: anywhere;">今日は<b ><wbr>とても<wbr>天気</b>です。</span>
 ```
 
 If you have a custom model, you can use it as follows.
 
 ```python
 with open('/path/to/your/model.json') as f:
   model = json.load(f)
@@ -126,15 +126,15 @@
 ---
 明日は
 曇りでしょう。
 ```
 
 ```shellsession
 $ budoux 本日は晴天です。 -H
-<span style="word-break: keep-all; overflow-wrap: break-word;">本日は<wbr>晴天です。</span>
+<span style="word-break: keep-all; overflow-wrap: anywhere;">本日は<wbr>晴天です。</span>
 ```
 
 If you want to see help, run `budoux -h`.
 
 ```shellsession
 $ budoux -h
 usage: budoux [-h] [-H] [-m JSON | -l LANG] [-d STR] [-V] [TXT]
```

### Comparing `budoux-0.5.1/budoux/__init__.py` & `budoux-0.5.2/budoux/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """BudouX module."""
 
 from . import parser
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 Parser = parser.Parser
 load_default_japanese_parser = parser.load_default_japanese_parser
 load_default_simplified_chinese_parser = parser.load_default_simplified_chinese_parser
 load_default_traditional_chinese_parser = parser.load_default_traditional_chinese_parser
```

### Comparing `budoux-0.5.1/budoux/html_processor.py` & `budoux-0.5.2/budoux/html_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 import typing
 from html.parser import HTMLParser
 
 from .utils import SEP
 
 HTMLAttr = typing.List[typing.Tuple[str, typing.Union[str, None]]]
-PARENT_CSS_STYLE = 'word-break: keep-all; overflow-wrap: break-word;'
+PARENT_CSS_STYLE = 'word-break: keep-all; overflow-wrap: anywhere;'
 with open(
     os.path.join(os.path.dirname(__file__), 'skip_nodes.json'),
     encoding='utf-8') as f:
   SKIP_NODES: typing.Set[str] = set(json.load(f))
 
 
 class TextContentExtractor(HTMLParser):
```

### Comparing `budoux-0.5.1/budoux/main.py` & `budoux-0.5.2/budoux/main.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/budoux/models/ja.json` & `budoux-0.5.2/budoux/models/ja_knbc.json`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/budoux/models/zh-hans.json` & `budoux-0.5.2/budoux/models/zh-hans.json`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/budoux/models/zh-hant.json` & `budoux-0.5.2/budoux/models/zh-hant.json`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/budoux/parser.py` & `budoux-0.5.2/budoux/parser.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/budoux/utils.py` & `budoux-0.5.2/budoux/utils.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/budoux.egg-info/PKG-INFO` & `budoux-0.5.2/budoux.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budoux
-Version: 0.5.1
+Version: 0.5.2
 Summary: BudouX is the successor of Budou
 Author: Shuhei Iitsuka
 Author-email: tushuhei@google.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -94,15 +94,15 @@
 # ['今天', '是', '晴天。']
 ```
 
 You can also translate an HTML string by wrapping phrases with non-breaking markup.
 
 ```python
 print(parser.translate_html_string('今日は<b>とても天気</b>です。'))
-# <span style="word-break: keep-all; overflow-wrap: break-word;">今日は<b ><wbr>とても<wbr>天気</b>です。</span>
+# <span style="word-break: keep-all; overflow-wrap: anywhere;">今日は<b ><wbr>とても<wbr>天気</b>です。</span>
 ```
 
 If you have a custom model, you can use it as follows.
 
 ```python
 with open('/path/to/your/model.json') as f:
   model = json.load(f)
@@ -145,15 +145,15 @@
 ---
 明日は
 曇りでしょう。
 ```
 
 ```shellsession
 $ budoux 本日は晴天です。 -H
-<span style="word-break: keep-all; overflow-wrap: break-word;">本日は<wbr>晴天です。</span>
+<span style="word-break: keep-all; overflow-wrap: anywhere;">本日は<wbr>晴天です。</span>
 ```
 
 If you want to see help, run `budoux -h`.
 
 ```shellsession
 $ budoux -h
 usage: budoux [-h] [-H] [-m JSON | -l LANG] [-d STR] [-V] [TXT]
```

### Comparing `budoux-0.5.1/budoux.egg-info/SOURCES.txt` & `budoux-0.5.2/budoux.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 budoux.egg-info/PKG-INFO
 budoux.egg-info/SOURCES.txt
 budoux.egg-info/dependency_links.txt
 budoux.egg-info/entry_points.txt
 budoux.egg-info/requires.txt
 budoux.egg-info/top_level.txt
 budoux/models/ja.json
+budoux/models/ja_knbc.json
 budoux/models/zh-hans.json
 budoux/models/zh-hant.json
 scripts/__init__.py
 scripts/build_model.py
 scripts/encode_data.py
+scripts/finetune.py
 scripts/prepare_knbc.py
 scripts/train.py
 scripts/translate_model.py
 tests/test_html_processor.py
 tests/test_main.py
-tests/test_parser.py
+tests/test_parser.py
+tests/test_quality.py
```

### Comparing `budoux-0.5.1/scripts/build_model.py` & `budoux-0.5.2/scripts/build_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     decision_trees.setdefault(feature_group, {})
     decision_trees[feature_group].setdefault(feature_content, 0)
     decision_trees[feature_group][feature_content] += score
   return decision_trees
 
 
 def round_model(model: typing.Dict[str, typing.Dict[str, float]],
-                scale: int = 1000) -> typing.Dict[str, typing.Dict[str, int]]:
+                scale: int) -> typing.Dict[str, typing.Dict[str, int]]:
   """Rounds the scores in the model to integer after scaling.
 
   Args:
     model (Dict[str, Dict[str, float]]): The model to round scores.
     scale (int, optional): A scale factor to multiply scores.
 
   Returns:
@@ -63,30 +63,55 @@
       scaled_score = int(score * scale)
       if abs(scaled_score) > 0:
         model_rounded.setdefault(feature_group, {})
         model_rounded[feature_group][feature_content] = scaled_score
   return model_rounded
 
 
-def main() -> None:
-  parser = argparse.ArgumentParser(description=__doc__)
+def parse_args(
+    test: typing.Optional[typing.List[str]] = None) -> argparse.Namespace:
+  """Parses commandline arguments.
+
+  Args:
+    test (typing.Optional[typing.List[str]], optional): Commandline args for
+      testing. Defaults to None.
+
+  Returns:
+    Parsed arguments (argparse.Namespace).
+  """
+  parser = argparse.ArgumentParser(
+      description=__doc__, formatter_class=argparse.RawTextHelpFormatter)
   parser.add_argument(
       'weight_file', help='A file path for the learned weights.')
   parser.add_argument(
       '-o',
       '--outfile',
       help='A file path to export a model file. (default: model.json)',
-      default='model.json')
-  args = parser.parse_args()
+      default='model.json',
+      type=str)
+  parser.add_argument(
+      '--scale',
+      help='A scale factor for the output scores',
+      default=1000,
+      type=int)
+  if test is None:
+    return parser.parse_args()
+  else:
+    return parser.parse_args(test)
+
+
+def main() -> None:
+  args = parse_args()
   weights_filename = args.weight_file
   model_filename = args.outfile
+  scale = args.scale
   with open(weights_filename) as f:
     weights = f.readlines()
   model = aggregate_scores(weights)
-  model_rounded = round_model(model)
+  model_rounded = round_model(model, scale)
   with open(model_filename, 'w', encoding='utf-8') as f:
     json.dump(model_rounded, f, ensure_ascii=False, separators=(',', ':'))
   print('Model file is exported as', model_filename)
 
 
 if __name__ == '__main__':
   main()
```

### Comparing `budoux-0.5.1/scripts/encode_data.py` & `budoux-0.5.2/scripts/encode_data.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/scripts/prepare_knbc.py` & `budoux-0.5.2/scripts/prepare_knbc.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/scripts/train.py` & `budoux-0.5.2/scripts/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,18 +18,16 @@
 import typing
 from collections import Counter
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.numpy as jnp
-import numpy as np
-import numpy.typing as npt
 
-EPS = np.finfo(float).eps  # type: np.floating[typing.Any]
+EPS: float = jnp.finfo(float).eps
 DEFAULT_OUTPUT_NAME = 'weights.txt'
 DEFAULT_LOG_NAME = 'train.log'
 DEFAULT_FEATURE_THRES = 10
 DEFAULT_ITERATION = 10000
 DEFAULT_OUT_SPAN = 100
 ArgList = typing.Optional[typing.List[str]]
 
@@ -41,122 +39,136 @@
   fn: int
   accuracy: float
   precision: float
   recall: float
   fscore: float
 
 
-def preprocess(
-    entries_filename: str, feature_thres: int
-) -> typing.Tuple[typing.Any, typing.Any, typing.Any, typing.List[str]]:
-  """Loads entries and translates them into JAX arrays. The boolean matrix of
-  the input data is represented by row indices and column indices of True values
-  instead of the matrix itself for memory efficiency, assuming the matrix is
-  highly sparse. Row and column indices are not guaranteed to be sorted.
+class Dataset(NamedTuple):
+  """A dataset tuple.
+
+  X_rows (jax.Array): Row indices of True values in the input data.
+  X_cols (jax.Array): Column indices of True values in the input data.
+  Y (jax.Array): The target output.
+  """
+  X_rows: jax.Array
+  X_cols: jax.Array
+  Y: jax.Array
+
+
+def extract_features(data_path: str, thres: int) -> typing.List[str]:
+  """Extracts a features list from the given encoded data file. This filters out
+     features whose number of occurrences does not exceed the threshold.
 
   Args:
-    entries_filename (str): A file path to the entries file.
-    feature_thres (str): A threshold to filter out features whose frequency is
-      below the given value.
+    data_path (str): The path to the encoded data file that contains the
+      features to be extracted, which is typically a training data file.
+    thres (int): A threshold to filter out features  whose number of occurrences
+      does not exceed the threshold.
 
   Returns:
-    A tuple of following items:
-    - rows (JAX array): Row indices of True values in the input data.
-    - cols (JAX array): Column indices of True values in the input data.
-    - Y (JAX array): The target output data.
-    - features (List[str]): The list of features.
+    A list of features
+  """
+  counter: typing.Counter[str] = Counter()
+  with open(data_path) as f:
+    for row in f:
+      cols = row.strip().split('\t')
+      if len(cols) < 2:
+        continue
+      counter.update(cols[1:])
+  return [item[0] for item in counter.most_common() if item[1] > thres]
+
+
+def load_dataset(data_path: str, findex: typing.Dict[str, int]) -> Dataset:
+  """Loads a dataset from the given encoded data file.
+
+  Args:
+    data_path (str): A file path for the encoded data file.
+    findex (Dict[str, int]): A dictionary that maps a feature to its index.
+
+  Returns:
+    A dataset
   """
-  features_counter: typing.Counter[str] = Counter()
-  X = []
   Y = array.array('B')
-  with open(entries_filename) as f:
+  X_rows = array.array('I')
+  X_cols = array.array('I')
+  with open(data_path) as f:
+    i = 0
     for row in f:
       cols = row.strip().split('\t')
       if len(cols) < 2:
         continue
       Y.append(cols[0] == '1')
-      X.append(cols[1:])
-      features_counter.update(cols[1:])
-  features = [
-      item[0]
-      for item in features_counter.most_common()
-      if item[1] > feature_thres
-  ]
-  feature_index = dict([(feature, i) for i, feature in enumerate(features)])
-  rows = array.array('I')
-  cols = array.array('I')  # type: ignore
-  for i, x in enumerate(X):
-    hit_indices = [feature_index[feat] for feat in x if feat in feature_index]
-    rows.extend(i for _ in range(len(hit_indices)))
-    cols.extend(hit_indices)  # type: ignore
-  return jnp.asarray(rows), jnp.asarray(cols), jnp.asarray(
-      Y, dtype=bool), features
-
-
-def split_data(
-    rows: npt.NDArray[np.int32],
-    cols: npt.NDArray[np.int32],
-    Y: npt.NDArray[np.bool_],
-    split_ratio: float = .9
-) -> typing.Tuple[npt.NDArray[np.int32], npt.NDArray[np.int32],
-                  npt.NDArray[np.int32], npt.NDArray[np.int32],
-                  npt.NDArray[np.bool_], npt.NDArray[np.bool_]]:
-  """Splits a dataset into a training dataset and a test dataset.
+      hit_indices = [findex[feat] for feat in cols[1:] if feat in findex]
+      X_rows.extend(i for _ in range(len(hit_indices)))
+      X_cols.extend(hit_indices)
+      i += 1
+  return Dataset(
+      jnp.asarray(X_rows), jnp.asarray(X_cols), jnp.asarray(Y, dtype=bool))
+
+
+def preprocess(
+    train_data_path: str,
+    feature_thres: int,
+    val_data_path: typing.Optional[str] = None,
+) -> typing.Tuple[Dataset, typing.List[str], typing.Optional[Dataset]]:
+  """Loads entries and translates them into JAX arrays. The boolean matrix of
+  the input data is represented by row indices and column indices of True values
+  instead of the matrix itself for memory efficiency, assuming the matrix is
+  highly sparse. Row and column indices are not guaranteed to be sorted.
 
   Args:
-    rows (numpy.ndarray): Row indices of True values in the input data.
-    cols (numpy.ndarray): Column indices of True values in the input data.
-    Y (numpy.ndarray): The target output.
-    split_ratio (float, optional): The split ratio for the training dataset.
-      The value should be between 0 and 1. The default value is 0.9 (=90% for
-      training).
+    train_data_path (str): A file path to the training data file.
+    feature_thres (str): A threshold to filter out features whose number of
+      occurances does not exceed the value.
+    val_data_path (str, optional): A file path to the validation data file.
 
   Returns:
-    A tuple of:
-    - rows_train (numpy.ndarray): Row indices of True values in the training input data.
-    - cols_train (numpy.ndarray): Column indices of True values in the training input data.
-    - rows_test (numpy.ndarray): Row indices of True values in the test input data.
-    - cols_test (numpy.ndarray): Column indices of True values in the test input data.
-    - Y_train (numpy.ndarray): The training target output.
-    - Y_test (numpy.ndarray): The test target output.
+    A tuple of following items:
+    - train_dataset (Dataset): The training dataset.
+    - features (List[str]): The list of features.
+    - val_dataset (Optional[Dataset]): The validation dataset.
+        This becomes None if val_data_path is None.
   """
-  thres = int(Y.shape[0] * split_ratio)
-  return (rows[rows < thres], cols[rows < thres], rows[rows >= thres] - thres,
-          cols[rows >= thres], Y[:thres], Y[thres:])
+  features = extract_features(train_data_path, feature_thres)
+  feature_index = dict((feature, i) for i, feature in enumerate(features))
+  train_dataset = load_dataset(train_data_path, feature_index)
+  val_dataset = load_dataset(val_data_path,
+                             feature_index) if val_data_path else None
+  return train_dataset, features, val_dataset
 
 
 @partial(jax.jit, static_argnums=[3])
-def pred(scores: npt.NDArray[np.float32], rows: npt.NDArray[np.int32],
-         cols: npt.NDArray[np.int32], N: int) -> npt.NDArray[np.bool_]:
+def pred(scores: jax.Array, rows: jax.Array, cols: jax.Array,
+         N: int) -> jax.Array:
   """Predicts the target output from the learned scores and input entries.
 
   Args:
-    scores (numpy.ndarray): Contribution scores of features.
-    rows (numpy.ndarray): Row indices of True values in the input.
-    cols (numpy.ndarray): Column indices of True values in the input.
+    scores (jax.Array): Contribution scores of features.
+    rows (jax.Array): Row indices of True values in the input.
+    cols (jax.Array): Column indices of True values in the input.
     N (int): The number of input entries.
 
   Returns:
-    res (numpy.ndarray): A prediction of the target.
+    res (jax.Array): A prediction of the target.
   """
   # This is equivalent to scores.dot(2X - 1) = 2 * scores.dot(X) - scores.sum()
   # but in a sparse matrix-friendly way.
-  r: npt.NDArray[np.float32] = 2 * jax.ops.segment_sum(
-      scores.take(cols), rows, N) - scores.sum()
+  r: jax.Array = 2 * jax.ops.segment_sum(scores.take(cols), rows,
+                                         N) - scores.sum()
   return r > 0
 
 
 @jax.jit
-def get_metrics(pred: npt.NDArray[np.bool_],
-                actual: npt.NDArray[np.bool_]) -> Result:
+def get_metrics(pred: jax.Array, actual: jax.Array) -> Result:
   """Gets evaluation metrics from the prediction and the actual target.
 
   Args:
-    pred (numpy.ndarray): A prediction of the target.
-    actual (numpy.ndarray): The actual target.
+    pred (jax.Array): A prediction of the target.
+    actual (jax.Array): The actual target.
 
   Returns:
     result (Result): A result.
   """
   tp: int = jnp.sum(jnp.logical_and(pred == 1, actual == 1))  # type: ignore
   tn: int = jnp.sum(jnp.logical_and(pred == 0, actual == 0))  # type: ignore
   fp: int = jnp.sum(jnp.logical_and(pred == 1, actual == 0))  # type: ignore
@@ -173,31 +185,29 @@
       precision=precision,
       recall=recall,
       fscore=2 * precision * recall / (precision + recall),
   )
 
 
 @jax.jit
-def update(
-    w: npt.NDArray[np.float32], scores: typing.Any, rows: npt.NDArray[np.int32],
-    cols: npt.NDArray[np.int32], Y: npt.NDArray[np.bool_]
-) -> typing.Tuple[typing.Any, typing.Any, int, float]:
+def update(w: jax.Array, scores: jax.Array, rows: jax.Array, cols: jax.Array,
+           Y: jax.Array) -> typing.Tuple[jax.Array, jax.Array, int, float]:
   """Calculates the new weight vector and the contribution scores.
 
   Args:
-    w (numpy.ndarray): A weight vector.
+    w (jax.Array): A weight vector.
     scores (JAX array): Contribution scores of features.
-    rows (numpy.ndarray): Row indices of True values in the input data.
-    cols (numpy.ndarray): Column indices of True values in the input data.
-    Y (numpy.ndarray): The target output.
+    rows (jax.Array): Row indices of True values in the input data.
+    cols (jax.Array): Column indices of True values in the input data.
+    Y (jax.Array): The target output.
 
 
   Returns:
     A tuple of following items:
-    - w (numpy.ndarray): The new weight vector.
+    - w (jax.Array): The new weight vector.
     - scores (JAX array): The new contribution scores.
     - best_feature_index (int): The index of the best feature.
     - score (float): The newly added score for the best feature.
   """
   N = w.shape[0]
   M = scores.shape[0]
   # This is quivalent to w.dot(Y[:, None] ^ X). Note that y ^ x = y + x - 2yx,
@@ -217,88 +227,95 @@
   w = w * jnp.exp(amount * (Y ^ X_best == positivity))
   w = w / w.sum()
   score = amount * (2 * positivity - 1)
   scores = scores.at[best_feature_index].add(score)
   return w, scores, best_feature_index, score
 
 
-def fit(rows_train: npt.NDArray[np.int32], cols_train: npt.NDArray[np.int32],
-        rows_test: npt.NDArray[np.int32], cols_test: npt.NDArray[np.int32],
-        Y_train: npt.NDArray[np.bool_], Y_test: npt.NDArray[np.bool_],
+def fit(dataset_train: Dataset, dataset_val: typing.Optional[Dataset],
         features: typing.List[str], iters: int, weights_filename: str,
-        log_filename: str, out_span: int) -> typing.Any:
+        log_filename: str, out_span: int) -> jax.Array:
   """Trains an AdaBoost binary classifier.
 
   Args:
-    row_train (numpy.ndarray): Row indices of True values in the training input data.
-    col_train (numpy.ndarray): Column indices of True values in the training input data.
-    row_test (numpy.ndarray): Row indices of True values in the test input data.
-    col_test (numpy.ndarray): Column indices of True values in the test input data.
-    Y_train (numpy.ndarray): The training target output.
-    Y_test (numpy.ndarray): The test target output.
+    dataset_train (Dataset): A training dataset.
+    dataset_val (Optional[Dataset]): A validation dataset.
     features (List[str]): Features, which correspond to the columns of entries.
     iters (int): A number of training iterations.
     weights_filename (str): A file path to write the learned weights.
     log_filename (str): A file path to log the accuracy along with training.
     out_span (int): Iteration span to output metics and weights.
 
   Returns:
-    scores (Any): The contribution scores.
+    scores (jax.Array): The contribution scores.
   """
   with open(weights_filename, 'w') as f:
     f.write('')
   with open(log_filename, 'w') as f:
-    f.write(
-        'iter\ttrain_accuracy\ttrain_precision\ttrain_recall\ttrain_fscore\t'
-        'test_accuracy\ttest_precision\ttest_recall\ttest_fscore\n')
+    f.write('iter\ttrain_accuracy\ttrain_precision\ttrain_recall\ttrain_fscore')
+    if dataset_val:
+      f.write('\ttest_accuracy\ttest_precision\ttest_recall\ttest_fscore')
+    f.write('\n')
   print('Outputting learned weights to %s ...' % (weights_filename))
 
   M = len(features)
   scores = jnp.zeros(M)
   feature_score_buffer: typing.List[typing.Tuple[str, float]] = []
-  N_train = Y_train.shape[0]
-  N_test = Y_test.shape[0]
+  N_train = dataset_train.Y.shape[0]
+  N_test = dataset_val.Y.shape[0] if dataset_val else 0
   w = jnp.ones(N_train) / N_train
 
   def output_progress(t: int) -> None:
-    print('=== %s ===' % t)
     with open(weights_filename, 'a') as f:
       f.write('\n'.join('%s\t%.6f' % p for p in feature_score_buffer) + '\n')
     feature_score_buffer.clear()
-    pred_train = pred(scores, rows_train, cols_train, N_train)
-    pred_test = pred(scores, rows_test, cols_test, N_test)
-    metrics_train = get_metrics(pred_train, Y_train)
-    metrics_test = get_metrics(pred_test, Y_test)
-    print()
-    print('train accuracy:\t%.5f' % metrics_train.accuracy)
-    print('train prec.:\t%.5f' % metrics_train.precision)
-    print('train recall:\t%.5f' % metrics_train.recall)
-    print('train fscore:\t%.5f' % metrics_train.fscore)
-    print()
-    print('test accuracy:\t%.5f' % metrics_test.accuracy)
-    print('test prec.:\t%.5f' % metrics_test.precision)
-    print('test recall:\t%.5f' % metrics_test.recall)
-    print('test fscore:\t%.5f' % metrics_test.fscore)
+
+    print('=== %s ===' % t)
     print()
+
     with open(log_filename, 'a') as f:
-      f.write('%d\t%.5f\t%.5f\t%.5f\t%.5f\t%.5f\t%.5f\t%.5f\t%.5f\n' % (
+      pred_train = pred(scores, dataset_train.X_rows, dataset_train.X_cols,
+                        N_train)
+      metrics_train = get_metrics(pred_train, dataset_train.Y)
+      print('train accuracy:\t%.5f' % metrics_train.accuracy)
+      print('train prec.:\t%.5f' % metrics_train.precision)
+      print('train recall:\t%.5f' % metrics_train.recall)
+      print('train fscore:\t%.5f' % metrics_train.fscore)
+      print()
+      f.write('%d\t%.5f\t%.5f\t%.5f\t%.5f' % (
           t,
           metrics_train.accuracy,
           metrics_train.precision,
           metrics_train.recall,
           metrics_train.fscore,
-          metrics_test.accuracy,
-          metrics_test.precision,
-          metrics_test.recall,
-          metrics_test.fscore,
       ))
 
+      if dataset_val:
+        pred_test = pred(scores, dataset_val.X_rows, dataset_val.X_cols, N_test)
+        metrics_test = get_metrics(pred_test, dataset_val.Y)
+        print('test accuracy:\t%.5f' % metrics_test.accuracy)
+        print('test prec.:\t%.5f' % metrics_test.precision)
+        print('test recall:\t%.5f' % metrics_test.recall)
+        print('test fscore:\t%.5f' % metrics_test.fscore)
+        print()
+
+        f.write('\t%.5f\t%.5f\t%.5f\t%.5f' % (
+            metrics_test.accuracy,
+            metrics_test.precision,
+            metrics_test.recall,
+            metrics_test.fscore,
+        ))
+
+      f.write('\n')
+
   for t in range(iters):
-    w, scores, best_feature_index, score = update(w, scores, rows_train,
-                                                  cols_train, Y_train)
+    w, scores, best_feature_index, score = update(w, scores,
+                                                  dataset_train.X_rows,
+                                                  dataset_train.X_cols,
+                                                  dataset_train.Y)
     w.block_until_ready()
     feature = features[best_feature_index]
     feature_score_buffer.append((feature, score))
     if (t + 1) % out_span == 0:
       output_progress(t + 1)
   if len(feature_score_buffer) > 0:
     output_progress(t + 1)
@@ -340,33 +357,35 @@
       type=int,
       default=DEFAULT_ITERATION)
   parser.add_argument(
       '--out-span',
       help=f'Iteration span to output metrics and weights. (default: {DEFAULT_OUT_SPAN})',
       type=int,
       default=DEFAULT_OUT_SPAN)
+  parser.add_argument(
+      '--val-data', help='File path for the encoded validation data.', type=str)
   if test is None:
     return parser.parse_args()
   else:
     return parser.parse_args(test)
 
 
 def main() -> None:
   args = parse_args()
   data_filename: str = args.encoded_train_data
   weights_filename: str = args.output
   log_filename: str = args.log
   feature_thres = int(args.feature_thres)
   iterations = int(args.iter)
   out_span = int(args.out_span)
+  val_data: typing.Optional[str] = args.val_data
 
-  X_rows, X_cols, Y, features = preprocess(data_filename, feature_thres)
-  X_rows_train, X_cols_train, X_rows_test, X_cols_test, Y_train, Y_test = split_data(
-      X_rows, X_cols, Y)
-  fit(X_rows_train, X_cols_train, X_rows_test, X_cols_test, Y_train, Y_test,
-      features, iterations, weights_filename, log_filename, out_span)
+  dataset_train, features, dataset_val = preprocess(data_filename,
+                                                    feature_thres, val_data)
+  fit(dataset_train, dataset_val, features, iterations, weights_filename,
+      log_filename, out_span)
   print('Training done. Export the model by passing %s to build_model.py' %
         (weights_filename))
 
 
 if __name__ == '__main__':
   main()
```

### Comparing `budoux-0.5.1/scripts/translate_model.py` & `budoux-0.5.2/scripts/translate_model.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/setup.cfg` & `budoux-0.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 test_suite = tests
 
 [options.extras_require]
 dev = 
 	build
 	flake8
 	isort
-	numpy
 	mypy
 	pytest
 	toml
 	twine
 	types-setuptools
 	yapf
```

### Comparing `budoux-0.5.1/setup.py` & `budoux-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.1/tests/test_html_processor.py` & `budoux-0.5.2/tests/test_html_processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,30 +49,30 @@
 
 class TestResolve(unittest.TestCase):
 
   def test_with_simple_text_input(self) -> None:
     chunks = ['abc', 'def']
     html = 'abcdef'
     result = html_processor.resolve(chunks, html)
-    expected = '<span style="word-break: keep-all; overflow-wrap: break-word;">abc<wbr>def</span>'
+    expected = '<span style="word-break: keep-all; overflow-wrap: anywhere;">abc<wbr>def</span>'
     self.assertEqual(result, expected)
 
   def test_with_standard_html_input(self) -> None:
     chunks = ['abc', 'def']
     html = 'ab<a href="http://example.com">cd</a>ef'
     result = html_processor.resolve(chunks, html)
-    expected = '<span style="word-break: keep-all; overflow-wrap: break-word;">ab<a href="http://example.com">c<wbr>d</a>ef</span>'
+    expected = '<span style="word-break: keep-all; overflow-wrap: anywhere;">ab<a href="http://example.com">c<wbr>d</a>ef</span>'
     self.assertEqual(result, expected)
 
   def test_with_nodes_to_skip(self) -> None:
     chunks = ['abc', 'def']
     html = "a<button>bcde</button>f"
     result = html_processor.resolve(chunks, html)
-    expected = '<span style="word-break: keep-all; overflow-wrap: break-word;">a<button>bcde</button>f</span>'
+    expected = '<span style="word-break: keep-all; overflow-wrap: anywhere;">a<button>bcde</button>f</span>'
     self.assertEqual(result, expected)
 
   def test_with_nothing_to_split(self) -> None:
     chunks = ['abcdef']
     html = 'abcdef'
     result = html_processor.resolve(chunks, html)
-    expected = '<span style="word-break: keep-all; overflow-wrap: break-word;">abcdef</span>'
+    expected = '<span style="word-break: keep-all; overflow-wrap: anywhere;">abcdef</span>'
     self.assertEqual(result, expected)
```

### Comparing `budoux-0.5.1/tests/test_main.py` & `budoux-0.5.2/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,18 +75,18 @@
     cmdargs = ['-l', 'ja-abc']
     with self.assertRaises(SystemExit) as cm:
       main.parse_args(cmdargs)
 
     self.assertEqual(cm.exception.code, 2)
 
   def test_cmdargs_lang_ja(self) -> None:
-    cmdargs = ['-l', 'ja', '今日はいい天気ですね。']
+    cmdargs = ['-l', 'ja', '今日は良い天気ですね。']
     output = main._main(cmdargs)
 
-    self.assertEqual(output, '今日は\nいい\n天気ですね。')
+    self.assertEqual(output, '今日は\n良い\n天気ですね。')
 
   def test_cmdargs_lang_zh_hans(self) -> None:
     cmdargs = ['-l', 'zh-hans', '今天天气晴朗。']
     output = main._main(cmdargs)
 
     self.assertEqual(output, '今天\n天气\n晴朗。')
 
@@ -125,16 +125,15 @@
     self.assertEqual(cm.exception.code, 2)
 
   def test_cmdargs_single_html(self) -> None:
     cmdargs = ['-H', '今日は<b>とても天気</b>です。']
     output = main._main(cmdargs)
 
     self.assertEqual(
-        output,
-        '<span style="word-break: keep-all; overflow-wrap: break-word;">'
+        output, '<span style="word-break: keep-all; overflow-wrap: anywhere;">'
         '今日は<b><wbr>とても<wbr>天気</b>です。</span>')
 
   def test_cmdargs_multi_html(self) -> None:
     cmdargs = ['-H', '今日は<b>とても天気</b>です。', 'これは<b>テスト</b>です。']
     with self.assertRaises(SystemExit) as cm:
       main._main(cmdargs)
 
@@ -168,15 +167,14 @@
         join(abspath(dirname(__file__)), "in/3.in"),
         "r",
         encoding=sys.getdefaultencoding()) as f:
       sys.stdin = f
       output = main._main(["-H"])
 
     self.assertEqual(
-        output,
-        '<span style="word-break: keep-all; overflow-wrap: break-word;">'
+        output, '<span style="word-break: keep-all; overflow-wrap: anywhere;">'
         'これは<b><wbr>テスト</b>です。<wbr>\n'
         '</span>')
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `budoux-0.5.1/tests/test_parser.py` & `budoux-0.5.2/tests/test_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,49 +57,49 @@
         'UW4': {
             'a': 10000
         },  # means "should separate right before 'a'".
     })
 
     input_html = 'xyzabcd'
     expected_html = (
-        '<span style="word-break: keep-all; overflow-wrap: break-word;">'
+        '<span style="word-break: keep-all; overflow-wrap: anywhere;">'
         'xyz<wbr>abcd</span>')
     output_html = p.translate_html_string(input_html)
     self.assertEqual(
         output_html, expected_html,
         'Should output a html string with a SPAN parent with proper style attributes.'
     )
 
     input_html = 'xyz<script>alert(1);</script>xyzabc'
     expected_html = (
-        '<span style="word-break: keep-all; overflow-wrap: break-word;">'
+        '<span style="word-break: keep-all; overflow-wrap: anywhere;">'
         'xyz<script>alert(1);</script>xyz<wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
     self.assertEqual(output_html, expected_html,
                      'Should pass script tags as is.')
 
     input_html = 'xyz<code>abc</code>abc'
     expected_html = (
-        '<span style="word-break: keep-all; overflow-wrap: break-word;">'
+        '<span style="word-break: keep-all; overflow-wrap: anywhere;">'
         'xyz<code>abc</code><wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
     self.assertEqual(output_html, expected_html,
                      'Should skip some specific tags.')
 
     input_html = 'xyza<a href="#" hidden>bc</a>abc'
     expected_html = (
-        '<span style="word-break: keep-all; overflow-wrap: break-word;">'
+        '<span style="word-break: keep-all; overflow-wrap: anywhere;">'
         'xyz<wbr>a<a href="#" hidden>bc</a><wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
     self.assertEqual(output_html, expected_html,
                      'Should not ruin attributes of child elements.')
 
     input_html = 'xyza🇯🇵🇵🇹abc'
     expected_html = (
-        '<span style="word-break: keep-all; overflow-wrap: break-word;">'
+        '<span style="word-break: keep-all; overflow-wrap: anywhere;">'
         'xyz<wbr>a🇯🇵🇵🇹<wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
     self.assertEqual(output_html, expected_html, 'Should work with emojis.')
 
 
 class TestDefaultParser(unittest.TestCase):
 
@@ -111,16 +111,15 @@
         '使命は、',
         '世界中の',
         '情報を',
         '整理し、',
         '世界中の',
         '人が',
         'アクセスできて',
-        '使えるように',
-        'する',
+        '使えるようにする',
         'ことです。',
     ])
 
   def test_load_default_simplified_chinese_parser(self) -> None:
     p_hans = parser.load_default_simplified_chinese_parser()
     phrases = p_hans.parse('我们的使命是整合全球信息，供大众使用，让人人受益。')
     self.assertListEqual(phrases, [
```

