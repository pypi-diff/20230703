# Comparing `tmp/django_flatpickr-2.0.0.tar.gz` & `tmp/django_flatpickr-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_flatpickr-2.0.0.tar", max compression
+gzip compressed data, was "django_flatpickr-2.0.1.tar", max compression
```

## Comparing `django_flatpickr-2.0.0.tar` & `django_flatpickr-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1068 2022-10-23 10:35:54.134899 django_flatpickr-2.0.0/LICENSE
--rw-r--r--   0        0        0     8324 2022-10-23 10:35:54.134899 django_flatpickr-2.0.0/README.rst
--rw-r--r--   0        0        0     3595 2022-10-23 10:36:06.046816 django_flatpickr-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       59 2022-10-23 10:36:06.082816 django_flatpickr-2.0.0/src/django_flatpickr/__init__.py
--rw-r--r--   0        0        0     2547 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/_base.py
--rw-r--r--   0        0        0      994 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/_config.py
--rw-r--r--   0        0        0      910 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/_media.py
--rw-r--r--   0        0        0        0 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/py.typed
--rw-r--r--   0        0        0     2972 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/schemas.py
--rw-r--r--   0        0        0     1777 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/settings.py
--rw-r--r--   0        0        0     6219 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/static/django_flatpickr/js/django-flatpickr.js
--rw-r--r--   0        0        0       86 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/templates/django_flatpickr/input.html
--rw-r--r--   0        0        0     1477 2022-10-23 10:35:54.138899 django_flatpickr-2.0.0/src/django_flatpickr/widgets.py
--rw-r--r--   0        0        0     9563 1970-01-01 00:00:00.000000 django_flatpickr-2.0.0/setup.py
--rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 django_flatpickr-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/LICENSE
+-rw-r--r--   0        0        0     8324 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/README.rst
+-rw-r--r--   0        0        0     3616 2023-07-03 05:15:57.646426 django_flatpickr-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-03 05:15:57.682426 django_flatpickr-2.0.1/src/django_flatpickr/__init__.py
+-rw-r--r--   0        0        0     2547 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/_base.py
+-rw-r--r--   0        0        0      994 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/_config.py
+-rw-r--r--   0        0        0      910 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/_media.py
+-rw-r--r--   0        0        0        0 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/py.typed
+-rw-r--r--   0        0        0     2972 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/schemas.py
+-rw-r--r--   0        0        0     1777 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/settings.py
+-rw-r--r--   0        0        0     6219 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/static/django_flatpickr/js/django-flatpickr.js
+-rw-r--r--   0        0        0       86 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/templates/django_flatpickr/input.html
+-rw-r--r--   0        0        0     1609 2023-07-03 05:15:42.630474 django_flatpickr-2.0.1/src/django_flatpickr/widgets.py
+-rw-r--r--   0        0        0     9754 1970-01-01 00:00:00.000000 django_flatpickr-2.0.1/PKG-INFO
```

### Comparing `django_flatpickr-2.0.0/LICENSE` & `django_flatpickr-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_flatpickr-2.0.0/README.rst` & `django_flatpickr-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `django_flatpickr-2.0.0/pyproject.toml` & `django_flatpickr-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "django-flatpickr"
-version = "2.0.0"
+version = "2.0.1"
 description = """\
     Flatpickr based DatePickerInput, TimePickerInput and \
     DateTimePickerInput with date-range-picker functionality \
     for django >= 2.0\
     """
 authors = ["Munim Munna <6266677+monim67@users.noreply.github.com>"]
 repository = "https://github.com/monim67/django-flatpickr"
 license = "MIT"
 readme = "README.rst"
-packages = [{ include = "*", from = "src" }]
+packages = [{ include = "django_flatpickr", from = "src" }]
 keywords = [
     "django",
     "flatpickr",
     "date-picker",
     "time-picker",
     "datetime-picker",
     "date-range-picker",
@@ -31,15 +31,15 @@
     "Framework :: Django :: 3.0",
     "Framework :: Django :: 4.0",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 Django = ">=2,<5"
-pydantic = "*"
+pydantic = "<2"
 typing-extensions = "*"
 
 [tool.poetry.group.build.dependencies]
 pytest-django = "^4.5.2"
 pytest-dotenv = "^0.5.2"
 black = "^22.6.0"
 isort = "^5.10.1"
@@ -111,15 +111,15 @@
     "**/site-packages/django_flatpickr",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py{310,39,38,37}
+envlist = py{3.11,310,39,38,37}
 
 [testenv]
 allowlist_externals = poetry
 skip_install = true
 commands =
     poetry install --no-root --only build
     pip install -c tests/pip-constraints.txt .
```

### Comparing `django_flatpickr-2.0.0/src/django_flatpickr/_base.py` & `django_flatpickr-2.0.1/src/django_flatpickr/_base.py`

 * *Files identical despite different names*

### Comparing `django_flatpickr-2.0.0/src/django_flatpickr/_config.py` & `django_flatpickr-2.0.1/src/django_flatpickr/_config.py`

 * *Files identical despite different names*

### Comparing `django_flatpickr-2.0.0/src/django_flatpickr/_media.py` & `django_flatpickr-2.0.1/src/django_flatpickr/_media.py`

 * *Files identical despite different names*

### Comparing `django_flatpickr-2.0.0/src/django_flatpickr/schemas.py` & `django_flatpickr-2.0.1/src/django_flatpickr/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     altFormat: Optional[str]
     altInput: bool = True
     altInputClass: Optional[str]
     ariaDateFormat: Optional[str]
     clickOpens: Optional[bool]
     dateFormat: Optional[str]
     defaultDate: Optional[str]
-    defaultHour: Optional[int] = Field(ge=1, le=12)
+    defaultHour: Optional[int] = Field(ge=0, le=23)
     defaultMinute: Optional[int] = Field(ge=0, le=59)
     disable: Optional[List[str]]
     disableMobile: Optional[bool]
     enable: Optional[List[str]]
     enableSeconds: Optional[bool]
     enableTime: Optional[bool]
     hourIncrement: Optional[int] = Field(ge=1, le=12)
```

### Comparing `django_flatpickr-2.0.0/src/django_flatpickr/settings.py` & `django_flatpickr-2.0.1/src/django_flatpickr/settings.py`

 * *Files identical despite different names*

### Comparing `django_flatpickr-2.0.0/src/django_flatpickr/static/django_flatpickr/js/django-flatpickr.js` & `django_flatpickr-2.0.1/src/django_flatpickr/static/django_flatpickr/js/django-flatpickr.js`

 * *Files identical despite different names*

### Comparing `django_flatpickr-2.0.0/src/django_flatpickr/widgets.py` & `django_flatpickr-2.0.1/src/django_flatpickr/widgets.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 )
 
 
 class DatePickerInput(BasePickerInput):
     """Widget for DateField to display a Date-Picker Calendar.
 
     Args:
-        - attrs (dict): HTML attributes of rendered HTML input
-        - options (dict): Options to customize the widget, see Docs
+        attrs: HTML attributes of rendered HTML input
+        options: Options to customize the widget, see Docs
+        range_from: Name of input to link for range selection
     """
 
     picker_type = "DATE"
     datetime_format = "%Y-%m-%d"
     format_key = "DATE_INPUT_FORMATS"
 
 
 class TimePickerInput(BasePickerInput):
     """Widget for TimeField to display a Time-Picker Calendar.
 
     Args:
-        - attrs (dict): HTML attributes of rendered HTML input
-        - options (dict): Options to customize the widget, see Docs
+        attrs: HTML attributes of rendered HTML input
+        options: Options to customize the widget, see Docs
+        range_from: Name of input to link for range selection
     """
 
     picker_type = "TIME"
     datetime_format = "%H:%M:%S"
     format_key = "TIME_INPUT_FORMATS"
     _option_overrides = {
         "dateFormat": "H:i:S",
@@ -40,16 +42,17 @@
     }
 
 
 class DateTimePickerInput(BasePickerInput):
     """Widget for DateTimeField to display a DateTime-Picker Calendar.
 
     Args:
-        - attrs (dict): HTML attributes of rendered HTML input
-        - options (dict): Options to customize the widget, see Docs
+        attrs: HTML attributes of rendered HTML input
+        options: Options to customize the widget, see Docs
+        range_from: Name of input to link for range selection
     """
 
     picker_type = "DATETIME"
     datetime_format = "%Y-%m-%d %H:%M:%S"
     format_key = "DATETIME_INPUT_FORMATS"
     _option_overrides = {
         "dateFormat": "Y-m-d H:i:S",
```

### Comparing `django_flatpickr-2.0.0/PKG-INFO` & `django_flatpickr-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flatpickr
-Version: 2.0.0
+Version: 2.0.1
 Summary: Flatpickr based DatePickerInput, TimePickerInput and DateTimePickerInput with date-range-picker functionality for django >= 2.0
 Home-page: https://github.com/monim67/django-flatpickr
 License: MIT
 Keywords: django,flatpickr,date-picker,time-picker,datetime-picker,date-range-picker
 Author: Munim Munna
 Author-email: 6266677+monim67@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: Django (>=2,<5)
-Requires-Dist: pydantic
+Requires-Dist: pydantic (<2)
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/monim67/django-flatpickr
 Description-Content-Type: text/x-rst
 
 django-flatpickr
 ================
```

