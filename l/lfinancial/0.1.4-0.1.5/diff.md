# Comparing `tmp/lfinancial-0.1.4.tar.gz` & `tmp/lfinancial-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.1.4.tar", last modified: Thu Jun 29 12:56:39 2023, max compression
+gzip compressed data, was "lfinancial-0.1.5.tar", last modified: Mon Jul  3 11:43:36 2023, max compression
```

## Comparing `lfinancial-0.1.4.tar` & `lfinancial-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:56:39.883035 lfinancial-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 12:56:18.000000 lfinancial-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-29 12:56:39.883035 lfinancial-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-29 12:56:18.000000 lfinancial-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:56:39.883035 lfinancial-0.1.4/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 12:56:18.000000 lfinancial-0.1.4/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-29 12:56:18.000000 lfinancial-0.1.4/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-29 12:56:18.000000 lfinancial-0.1.4/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:56:39.883035 lfinancial-0.1.4/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-29 12:56:39.000000 lfinancial-0.1.4/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-29 12:56:39.000000 lfinancial-0.1.4/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:56:39.000000 lfinancial-0.1.4/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 12:56:39.000000 lfinancial-0.1.4/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:56:39.883035 lfinancial-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 12:56:18.000000 lfinancial-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:56:39.883035 lfinancial-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-29 12:56:18.000000 lfinancial-0.1.4/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:36.187574 lfinancial-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-03 11:43:19.000000 lfinancial-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 11:43:36.187574 lfinancial-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 11:43:19.000000 lfinancial-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:36.183574 lfinancial-0.1.5/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 11:43:19.000000 lfinancial-0.1.5/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-03 11:43:19.000000 lfinancial-0.1.5/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-03 11:43:19.000000 lfinancial-0.1.5/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:36.187574 lfinancial-0.1.5/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 11:43:36.000000 lfinancial-0.1.5/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-03 11:43:36.000000 lfinancial-0.1.5/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:43:36.000000 lfinancial-0.1.5/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 11:43:36.000000 lfinancial-0.1.5/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:43:36.187574 lfinancial-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-03 11:43:19.000000 lfinancial-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:36.187574 lfinancial-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 11:43:19.000000 lfinancial-0.1.5/tests/test_document.py
```

### Comparing `lfinancial-0.1.4/LICENSE.txt` & `lfinancial-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.4/PKG-INFO` & `lfinancial-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -69,8 +69,11 @@
 # 13851695115
 
 f.area_code()
 # +86
 
 f.high_risk_country()
 # MA
+
+f.email()
+# q0o58mkgq3@gmail.com
 ```
```

### Comparing `lfinancial-0.1.4/README.md` & `lfinancial-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,8 +57,11 @@
 # 13851695115
 
 f.area_code()
 # +86
 
 f.high_risk_country()
 # MA
+
+f.email()
+# q0o58mkgq3@gmail.com
 ```
```

### Comparing `lfinancial-0.1.4/lfinancial/factory.py` & `lfinancial-0.1.5/lfinancial/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from lfinancial.generators.contry import CountryGenerator
 from lfinancial.generators.document import IDCodeGenerator
+from lfinancial.generators.mail import EmailGenerator
 from lfinancial.generators.name import NameGenerator
 from lfinancial.generators.phone import PhoneGenerator
 
 
 class GeneratorFactory:
     def __init__(self):
         self.generators = {
@@ -16,14 +17,15 @@
             "middle_name": NameGenerator(),
             "last_name": NameGenerator(),
             "cn_name": NameGenerator(),
             "kana_name": NameGenerator(),
             "cellphone": PhoneGenerator(),
             "area_code": PhoneGenerator(),
             "high_risk": CountryGenerator(),
+            "email": EmailGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.1.4/lfinancial/financial.py` & `lfinancial-0.1.5/lfinancial/financial.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 
     def area_code(self, country=None):
         return self._generate("area_code", country)
 
     def high_risk_country(self, country=None):
         return self._generate("high_risk", country)
 
+    def email(self, suffix=None):
+        return self._generate("email", suffix)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
@@ -60,7 +63,8 @@
     print(f.middle_name())
     print(f.last_name())
     print(f.kana_name())
     print(f.cn_name())
     print(f.cellphone())
     print(f.area_code())
     print(f.high_risk_country())
+    print(f.email())
```

### Comparing `lfinancial-0.1.4/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.1.5/lfinancial.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -69,8 +69,11 @@
 # 13851695115
 
 f.area_code()
 # +86
 
 f.high_risk_country()
 # MA
+
+f.email()
+# q0o58mkgq3@gmail.com
 ```
```

### Comparing `lfinancial-0.1.4/setup.py` & `lfinancial-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='lfinancial',
-    version='0.1.4',
+    version='0.1.5',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=['lfinancial'],
```

