# Comparing `tmp/chinese_calendar-1.8.0.tar.gz` & `tmp/chinese_calendar-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chinese_calendar-1.8.0.tar", last modified: Thu Dec  8 16:01:33 2022, max compression
+gzip compressed data, was "chinese_calendar-1.8.1.tar", last modified: Mon Jul  3 09:25:49 2023, max compression
```

## Comparing `chinese_calendar-1.8.0.tar` & `chinese_calendar-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-12-08 16:01:33.120837 chinese_calendar-1.8.0/
--rw-rw-rw-   0        0        0     1066 2022-03-22 15:11:02.000000 chinese_calendar-1.8.0/LICENSE
--rw-rw-rw-   0        0        0     3077 2022-12-08 16:01:33.120837 chinese_calendar-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2329 2022-12-08 16:00:41.000000 chinese_calendar-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2022-12-08 16:01:33.108837 chinese_calendar-1.8.0/chinese_calendar/
--rw-rw-rw-   0        0        0      616 2022-12-08 16:01:03.000000 chinese_calendar-1.8.0/chinese_calendar/__init__.py
--rw-rw-rw-   0        0        0    61744 2022-12-08 15:57:35.000000 chinese_calendar-1.8.0/chinese_calendar/constants.py
--rw-rw-rw-   0        0        0     4541 2022-12-08 15:46:46.000000 chinese_calendar-1.8.0/chinese_calendar/solar_terms.py
--rw-rw-rw-   0        0        0     6867 2022-05-07 09:33:28.000000 chinese_calendar-1.8.0/chinese_calendar/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-08 16:01:33.119837 chinese_calendar-1.8.0/chinese_calendar.egg-info/
--rw-rw-rw-   0        0        0     3077 2022-12-08 16:01:32.000000 chinese_calendar-1.8.0/chinese_calendar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2022-12-08 16:01:33.000000 chinese_calendar-1.8.0/chinese_calendar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-08 16:01:32.000000 chinese_calendar-1.8.0/chinese_calendar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-12-08 16:01:33.000000 chinese_calendar-1.8.0/chinese_calendar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      687 2022-12-08 16:01:33.121835 chinese_calendar-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0      960 2022-12-08 16:01:32.000000 chinese_calendar-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:25:49.041567 chinese_calendar-1.8.1/
+-rw-rw-rw-   0        0        0     1066 2021-08-20 05:42:44.000000 chinese_calendar-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0     3055 2023-07-03 09:25:49.041567 chinese_calendar-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2329 2022-12-12 13:20:20.000000 chinese_calendar-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 09:25:49.035437 chinese_calendar-1.8.1/chinese_calendar/
+-rw-rw-rw-   0        0        0      616 2023-07-03 09:24:10.000000 chinese_calendar-1.8.1/chinese_calendar/__init__.py
+-rw-rw-rw-   0        0        0    61744 2023-07-03 09:20:55.000000 chinese_calendar-1.8.1/chinese_calendar/constants.py
+-rw-rw-rw-   0        0        0     4541 2022-11-14 07:37:19.000000 chinese_calendar-1.8.1/chinese_calendar/solar_terms.py
+-rw-rw-rw-   0        0        0     7136 2023-07-03 09:20:07.000000 chinese_calendar-1.8.1/chinese_calendar/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:25:49.040443 chinese_calendar-1.8.1/chinese_calendar.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-07-03 09:25:49.000000 chinese_calendar-1.8.1/chinese_calendar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-07-03 09:25:49.000000 chinese_calendar-1.8.1/chinese_calendar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:25:49.000000 chinese_calendar-1.8.1/chinese_calendar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 09:25:49.000000 chinese_calendar-1.8.1/chinese_calendar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      435 2023-07-03 09:25:49.042560 chinese_calendar-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-07-03 09:25:48.000000 chinese_calendar-1.8.1/setup.py
```

### Comparing `chinese_calendar-1.8.0/LICENSE` & `chinese_calendar-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chinese_calendar-1.8.0/PKG-INFO` & `chinese_calendar-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: chinese_calendar
-Version: 1.8.0
+Version: 1.8.1
 Summary: check if some day is holiday in China
 Home-page: https://github.com/LKI/chinese-calendar
 Author: Lirian Su
 Author-email: liriansu@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 中国节假日
 
 [![Package](https://img.shields.io/pypi/v/chinesecalendar.svg)](https://pypi.python.org/pypi/chinesecalendar)
 [![Travis](https://img.shields.io/travis/LKI/chinese-calendar.svg)](https://travis-ci.org/LKI/chinese-calendar)
@@ -77,9 +76,7 @@
 2. 修改[节假日定义][scripts/data.py]
 3. 执行[脚本][scripts/__init__.py]自动生成[常量文件][constants.py]
 4. 提交PR
 
 [constants.py]: https://github.com/LKI/chinese-calendar/blob/master/chinese_calendar/constants.py
 [scripts/data.py]: https://github.com/LKI/chinese-calendar/blob/master/chinese_calendar/scripts/data.py
 [scripts/__init__.py]: https://github.com/LKI/chinese-calendar/blob/master/chinese_calendar/scripts/__init__.py
-
-
```

### Comparing `chinese_calendar-1.8.0/README.md` & `chinese_calendar-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `chinese_calendar-1.8.0/chinese_calendar/__init__.py` & `chinese_calendar-1.8.1/chinese_calendar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     get_solar_terms,
     get_workdays,
     is_holiday,
     is_in_lieu,
     is_workday,
 )
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 __all__ = [
     "Holiday",
     "holidays",
     "in_lieu_days",
     "workdays",
     "is_holiday",
     "is_in_lieu",
```

### Comparing `chinese_calendar-1.8.0/chinese_calendar/constants.py` & `chinese_calendar-1.8.1/chinese_calendar/constants.py`

 * *Files identical despite different names*

### Comparing `chinese_calendar-1.8.0/chinese_calendar/solar_terms.py` & `chinese_calendar-1.8.1/chinese_calendar/solar_terms.py`

 * *Files identical despite different names*

### Comparing `chinese_calendar-1.8.0/chinese_calendar/utils.py` & `chinese_calendar-1.8.1/chinese_calendar/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, unicode_literals
 
 import datetime
 
 from chinese_calendar.constants import holidays, in_lieu_days, workdays
-from chinese_calendar.solar_terms import SOLAR_TERMS_C_NUMS, SOLAR_TERMS_DELTA, SOLAR_TERMS_MONTH, SolarTerms
+from chinese_calendar.solar_terms import (
+    SOLAR_TERMS_C_NUMS,
+    SOLAR_TERMS_DELTA,
+    SOLAR_TERMS_MONTH,
+    SolarTerms,
+)
 
 
 def _wrap_date(date):
     """
     transform datetime.datetime into datetime.date
 
     :type date: datetime.date | datetime.datetime
@@ -120,24 +125,28 @@
     """
     start, end = _validate_date(start, end)
     if include_weekends:
         return list(filter(is_holiday, get_dates(start, end)))
     return list(filter(lambda x: x in holidays, get_dates(start, end)))
 
 
-def get_workdays(start, end):
+def get_workdays(start, end, include_weekends=True):
     """
     get workdays between start date and end date. (includes start date and end date)
 
     :type start: datetime.date | datetime.datetime
     :type end:  datetime.date | datetime.datetime
+    :type include_weekends: bool
+    :param include_weekends: False for excluding Saturdays and Sundays
     :rtype: list[datetime.date]
     """
     start, end = _validate_date(start, end)
-    return list(filter(is_workday, get_dates(start, end)))
+    if include_weekends:
+        return list(filter(is_workday, get_dates(start, end)))
+    return list(filter(lambda x: is_workday(x) and x.weekday() < 5, get_dates(start, end)))
 
 
 def find_workday(delta_days=0, date=None):
     """
     find the workday after {delta_days} days.
 
     :type delta_days: int
```

### Comparing `chinese_calendar-1.8.0/chinese_calendar.egg-info/PKG-INFO` & `chinese_calendar-1.8.1/chinese_calendar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: chinese-calendar
-Version: 1.8.0
+Version: 1.8.1
 Summary: check if some day is holiday in China
 Home-page: https://github.com/LKI/chinese-calendar
 Author: Lirian Su
 Author-email: liriansu@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 中国节假日
 
 [![Package](https://img.shields.io/pypi/v/chinesecalendar.svg)](https://pypi.python.org/pypi/chinesecalendar)
 [![Travis](https://img.shields.io/travis/LKI/chinese-calendar.svg)](https://travis-ci.org/LKI/chinese-calendar)
@@ -77,9 +76,7 @@
 2. 修改[节假日定义][scripts/data.py]
 3. 执行[脚本][scripts/__init__.py]自动生成[常量文件][constants.py]
 4. 提交PR
 
 [constants.py]: https://github.com/LKI/chinese-calendar/blob/master/chinese_calendar/constants.py
 [scripts/data.py]: https://github.com/LKI/chinese-calendar/blob/master/chinese_calendar/scripts/data.py
 [scripts/__init__.py]: https://github.com/LKI/chinese-calendar/blob/master/chinese_calendar/scripts/__init__.py
-
-
```

### Comparing `chinese_calendar-1.8.0/setup.py` & `chinese_calendar-1.8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     url="https://github.com/LKI/chinese-calendar",
     license="MIT License",
     packages=["chinese_calendar"],
     install_requires=[],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

