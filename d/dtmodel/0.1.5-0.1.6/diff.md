# Comparing `tmp/dtmodel-0.1.5.tar.gz` & `tmp/dtmodel-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtmodel-0.1.5.tar", max compression
+gzip compressed data, was "dtmodel-0.1.6.tar", max compression
```

## Comparing `dtmodel-0.1.5.tar` & `dtmodel-0.1.6.tar`

### file list

```diff
@@ -1,60 +1,90 @@
--rw-r--r--   0        0        0     1324 2023-06-02 17:19:45.034575 dtmodel-0.1.5/dtmodel/.env
--rw-r--r--   0        0        0      111 2023-06-18 01:40:16.194312 dtmodel-0.1.5/dtmodel/__init__.py
--rw-r--r--   0        0        0      115 2023-06-12 21:18:03.013541 dtmodel-0.1.5/dtmodel/bases/__init__.py
--rw-r--r--   0        0        0      304 2023-06-12 21:29:50.059622 dtmodel-0.1.5/dtmodel/bases/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3568 2023-06-18 01:53:17.356709 dtmodel-0.1.5/dtmodel/bases/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0     4612 2023-06-18 01:53:17.350580 dtmodel-0.1.5/dtmodel/bases/__pycache__/general.cpython-39.pyc
--rw-r--r--   0        0        0     1585 2023-06-18 01:53:17.354237 dtmodel-0.1.5/dtmodel/bases/__pycache__/medical.cpython-39.pyc
--rw-r--r--   0        0        0     5829 2023-06-18 01:53:17.340964 dtmodel-0.1.5/dtmodel/bases/__pycache__/people.cpython-39.pyc
--rw-r--r--   0        0        0      590 2023-06-18 01:53:17.338722 dtmodel-0.1.5/dtmodel/bases/__pycache__/self_key.cpython-39.pyc
--rw-r--r--   0        0        0     2576 2023-06-18 01:52:52.973390 dtmodel-0.1.5/dtmodel/bases/facility.py
--rw-r--r--   0        0        0     2681 2023-06-18 01:52:52.975168 dtmodel-0.1.5/dtmodel/bases/general.py
--rw-r--r--   0        0        0      985 2023-06-18 01:52:52.959320 dtmodel-0.1.5/dtmodel/bases/medical.py
--rw-r--r--   0        0        0     3639 2023-06-18 01:52:52.969538 dtmodel-0.1.5/dtmodel/bases/people.py
--rw-r--r--   0        0        0      229 2023-06-18 01:52:52.971125 dtmodel-0.1.5/dtmodel/bases/self_key.py
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtmodel-0.1.5/dtmodel/dtfield/__init__.py
--rw-r--r--   0        0        0      307 2023-06-18 01:50:26.938270 dtmodel-0.1.5/dtmodel/dtfield/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1869 2023-06-18 01:50:26.939028 dtmodel-0.1.5/dtmodel/dtfield/__pycache__/_imports.cpython-39.pyc
--rw-r--r--   0        0        0     2335 2023-06-18 01:53:16.933540 dtmodel-0.1.5/dtmodel/dtfield/__pycache__/base_enum.cpython-39.pyc
--rw-r--r--   0        0        0    30868 2023-06-18 01:53:16.939247 dtmodel-0.1.5/dtmodel/dtfield/__pycache__/engine.cpython-39.pyc
--rw-r--r--   0        0        0     3745 2023-06-18 01:50:27.077581 dtmodel-0.1.5/dtmodel/dtfield/__pycache__/functions.cpython-39.pyc
--rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtmodel-0.1.5/dtmodel/dtfield/_imports.py
--rw-r--r--   0        0        0     1397 2023-06-18 01:52:52.967512 dtmodel-0.1.5/dtmodel/dtfield/base_enum.py
--rw-r--r--   0        0        0    25945 2023-06-18 01:52:52.963373 dtmodel-0.1.5/dtmodel/dtfield/engine.py
--rw-r--r--   0        0        0     2762 2023-06-18 01:57:36.117036 dtmodel-0.1.5/dtmodel/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtmodel-0.1.5/dtmodel/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      348 2023-06-18 01:50:44.667250 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      451 2023-06-18 01:50:44.668027 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      785 2023-06-18 01:50:44.669834 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1744 2023-06-18 01:53:05.781277 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      534 2023-06-18 01:50:44.668475 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1288 2023-06-18 01:50:44.669455 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      810 2023-06-18 01:50:44.668902 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11660 2023-06-18 01:53:16.932211 dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtmodel-0.1.5/dtmodel/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtmodel-0.1.5/dtmodel/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1551 2023-06-18 01:53:05.630079 dtmodel-0.1.5/dtmodel/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtmodel-0.1.5/dtmodel/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtmodel-0.1.5/dtmodel/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtmodel-0.1.5/dtmodel/dtfield/parse/string.py
--rw-r--r--   0        0        0    10847 2023-06-18 01:53:16.713627 dtmodel-0.1.5/dtmodel/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0       68 2023-06-13 17:57:46.458805 dtmodel-0.1.5/dtmodel/enums/__init__.py
--rw-r--r--   0        0        0      265 2023-06-13 17:57:46.843945 dtmodel-0.1.5/dtmodel/enums/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1212 2023-06-18 01:53:17.343146 dtmodel-0.1.5/dtmodel/enums/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0      595 2023-06-18 01:53:17.344418 dtmodel-0.1.5/dtmodel/enums/__pycache__/medical.cpython-39.pyc
--rw-r--r--   0        0        0      738 2023-06-18 01:53:17.342218 dtmodel-0.1.5/dtmodel/enums/__pycache__/person.cpython-39.pyc
--rw-r--r--   0        0        0      789 2023-06-18 01:52:52.978073 dtmodel-0.1.5/dtmodel/enums/facility.py
--rw-r--r--   0        0        0      278 2023-06-18 01:52:52.965722 dtmodel-0.1.5/dtmodel/enums/medical.py
--rw-r--r--   0        0        0      328 2023-06-18 01:52:52.976595 dtmodel-0.1.5/dtmodel/enums/person.py
--rw-r--r--   0        0        0     1224 2023-06-12 19:51:27.475674 dtmodel-0.1.5/dtmodel/functions.py
--rw-r--r--   0        0        0       70 2023-06-12 03:19:07.376538 dtmodel-0.1.5/dtmodel/models/__init__.py
--rw-r--r--   0        0        0      266 2023-06-12 03:25:45.653987 dtmodel-0.1.5/dtmodel/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1918 2023-06-18 01:53:30.394045 dtmodel-0.1.5/dtmodel/models/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0     2129 2023-06-18 01:53:36.512967 dtmodel-0.1.5/dtmodel/models/__pycache__/medical.cpython-39.pyc
--rw-r--r--   0        0        0     3244 2023-06-18 01:53:24.789227 dtmodel-0.1.5/dtmodel/models/__pycache__/people.cpython-39.pyc
--rw-r--r--   0        0        0     1241 2023-06-18 01:53:30.161686 dtmodel-0.1.5/dtmodel/models/facility.py
--rw-r--r--   0        0        0     2087 2023-06-18 01:53:36.272660 dtmodel-0.1.5/dtmodel/models/medical.py
--rw-r--r--   0        0        0     2086 2023-06-18 01:53:24.548063 dtmodel-0.1.5/dtmodel/models/people.py
--rw-r--r--   0        0        0      468 2023-06-18 01:57:36.114761 dtmodel-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      909 2023-06-18 01:58:02.378126 dtmodel-0.1.5/setup.py
--rw-r--r--   0        0        0      669 2023-06-18 01:58:02.378349 dtmodel-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1530 2023-06-19 12:57:49.406373 dtmodel-0.1.6/dtmodel/.env
+-rw-r--r--   0        0        0      361 2023-07-02 20:55:40.149138 dtmodel-0.1.6/dtmodel/__init__.py
+-rw-r--r--   0        0        0    19163 2023-07-02 20:55:40.157390 dtmodel-0.1.6/dtmodel/app.py
+-rw-r--r--   0        0        0       92 2023-06-19 02:27:09.410134 dtmodel-0.1.6/dtmodel/base/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-19 02:27:09.538046 dtmodel-0.1.6/dtmodel/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    23096 2023-07-01 17:22:38.099690 dtmodel-0.1.6/dtmodel/base/__pycache__/_base.cpython-39.pyc
+-rw-r--r--   0        0        0     2038 2023-06-19 02:56:24.980207 dtmodel-0.1.6/dtmodel/base/__pycache__/_imports.cpython-39.pyc
+-rw-r--r--   0        0        0     1372 2023-07-02 21:00:08.299182 dtmodel-0.1.6/dtmodel/base/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0     2338 2023-06-26 03:40:29.545636 dtmodel-0.1.6/dtmodel/base/__pycache__/base_enum.cpython-39.pyc
+-rw-r--r--   0        0        0    20373 2023-07-01 16:49:17.465715 dtmodel-0.1.6/dtmodel/base/_base.py
+-rw-r--r--   0        0        0     2309 2023-06-19 02:56:24.903864 dtmodel-0.1.6/dtmodel/base/_imports.py
+-rw-r--r--   0        0        0      706 2023-07-02 20:55:40.152007 dtmodel-0.1.6/dtmodel/base/_types.py
+-rw-r--r--   0        0        0     1418 2023-06-26 03:40:28.999106 dtmodel-0.1.6/dtmodel/base/base_enum.py
+-rw-r--r--   0        0        0     2601 2023-06-29 13:00:08.969082 dtmodel-0.1.6/dtmodel/descriptor.py
+-rw-r--r--   0        0        0       91 2023-07-02 21:00:18.235157 dtmodel-0.1.6/dtmodel/endpoint/__init__.py
+-rw-r--r--   0        0        0      286 2023-07-02 21:00:18.462128 dtmodel-0.1.6/dtmodel/endpoint/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9307 2023-07-02 21:00:08.310575 dtmodel-0.1.6/dtmodel/endpoint/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0      536 2023-06-19 13:16:20.299765 dtmodel-0.1.6/dtmodel/endpoint/__pycache__/middleware.cpython-39.pyc
+-rw-r--r--   0        0        0     1887 2023-07-02 14:32:50.332935 dtmodel-0.1.6/dtmodel/endpoint/__pycache__/path.cpython-39.pyc
+-rw-r--r--   0        0        0    16338 2023-07-02 20:55:40.159985 dtmodel-0.1.6/dtmodel/endpoint/base.py
+-rw-r--r--   0        0        0     1867 2023-07-02 20:34:45.529987 dtmodel-0.1.6/dtmodel/endpoint/functions.py
+-rw-r--r--   0        0        0      310 2023-06-19 04:20:31.267696 dtmodel-0.1.6/dtmodel/endpoint/middleware.py
+-rw-r--r--   0        0        0     1499 2023-07-02 14:32:50.116794 dtmodel-0.1.6/dtmodel/endpoint/path.py
+-rw-r--r--   0        0        0       41 2023-06-21 02:17:03.066726 dtmodel-0.1.6/dtmodel/endpoint/templates/__init__.py
+-rw-r--r--   0        0        0      255 2023-06-21 02:17:03.852925 dtmodel-0.1.6/dtmodel/endpoint/templates/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      214 2023-06-21 22:25:52.145758 dtmodel-0.1.6/dtmodel/endpoint/templates/__pycache__/detail.cpython-39.pyc
+-rw-r--r--   0        0        0     1167 2023-06-23 04:20:11.340397 dtmodel-0.1.6/dtmodel/endpoint/templates/__pycache__/form.cpython-39.pyc
+-rw-r--r--   0        0        0     4365 2023-07-01 17:22:38.206019 dtmodel-0.1.6/dtmodel/endpoint/templates/__pycache__/render.cpython-39.pyc
+-rw-r--r--   0        0        0      463 2023-06-21 22:25:51.755167 dtmodel-0.1.6/dtmodel/endpoint/templates/detail.py
+-rw-r--r--   0        0        0      714 2023-06-23 04:20:10.647029 dtmodel-0.1.6/dtmodel/endpoint/templates/form.py
+-rw-r--r--   0        0        0     4428 2023-07-02 20:34:45.522701 dtmodel-0.1.6/dtmodel/endpoint/templates/render.py
+-rw-r--r--   0        0        0    10220 2023-06-28 15:08:05.433846 dtmodel-0.1.6/dtmodel/functions.py
+-rw-r--r--   0        0        0       82 2023-07-02 20:55:40.146256 dtmodel-0.1.6/dtmodel/micro/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-02 21:00:18.520101 dtmodel-0.1.6/dtmodel/micro/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2036 2023-07-02 21:00:18.520749 dtmodel-0.1.6/dtmodel/micro/__pycache__/_base.cpython-39.pyc
+-rw-r--r--   0        0        0      200 2023-07-02 21:00:18.521336 dtmodel-0.1.6/dtmodel/micro/__pycache__/_html.cpython-39.pyc
+-rw-r--r--   0        0        0      200 2023-07-02 21:00:18.521575 dtmodel-0.1.6/dtmodel/micro/__pycache__/_json.cpython-39.pyc
+-rw-r--r--   0        0        0      199 2023-07-02 21:00:18.521074 dtmodel-0.1.6/dtmodel/micro/__pycache__/dash.cpython-39.pyc
+-rw-r--r--   0        0        0     1601 2023-07-02 20:55:40.154073 dtmodel-0.1.6/dtmodel/micro/_base.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:35:13.165891 dtmodel-0.1.6/dtmodel/micro/_html.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:35:07.637707 dtmodel-0.1.6/dtmodel/micro/_json.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:34:51.253145 dtmodel-0.1.6/dtmodel/micro/dash.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:35:53.351398 dtmodel-0.1.6/dtmodel/micro/primary.py
+-rw-r--r--   0        0        0    12412 2023-07-01 19:02:13.143054 dtmodel-0.1.6/dtmodel/model.py
+-rw-r--r--   0        0        0      112 2023-06-19 02:27:09.414992 dtmodel-0.1.6/dtmodel/models/__init__.py
+-rw-r--r--   0        0        0      300 2023-06-19 02:27:09.719330 dtmodel-0.1.6/dtmodel/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2905 2023-06-26 05:49:13.287146 dtmodel-0.1.6/dtmodel/models/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0     8064 2023-06-30 02:50:42.590465 dtmodel-0.1.6/dtmodel/models/__pycache__/medical.cpython-39.pyc
+-rw-r--r--   0        0        0     3498 2023-07-02 21:00:18.510832 dtmodel-0.1.6/dtmodel/models/__pycache__/people.cpython-39.pyc
+-rw-r--r--   0        0        0      115 2023-06-12 21:18:03.013541 dtmodel-0.1.6/dtmodel/models/bases/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-19 02:20:39.735347 dtmodel-0.1.6/dtmodel/models/bases/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4010 2023-06-26 06:09:38.146063 dtmodel-0.1.6/dtmodel/models/bases/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0     6909 2023-06-29 03:44:26.692711 dtmodel-0.1.6/dtmodel/models/bases/__pycache__/general.cpython-39.pyc
+-rw-r--r--   0        0        0    10667 2023-06-29 18:55:43.022147 dtmodel-0.1.6/dtmodel/models/bases/__pycache__/medical.cpython-39.pyc
+-rw-r--r--   0        0        0     6996 2023-06-26 15:26:47.199883 dtmodel-0.1.6/dtmodel/models/bases/__pycache__/people.cpython-39.pyc
+-rw-r--r--   0        0        0      655 2023-06-26 00:35:31.739762 dtmodel-0.1.6/dtmodel/models/bases/__pycache__/self_key.cpython-39.pyc
+-rw-r--r--   0        0        0     2916 2023-06-26 06:09:37.411409 dtmodel-0.1.6/dtmodel/models/bases/facility.py
+-rw-r--r--   0        0        0     4282 2023-06-29 03:44:26.070566 dtmodel-0.1.6/dtmodel/models/bases/general.py
+-rw-r--r--   0        0        0     6797 2023-06-29 18:55:42.343033 dtmodel-0.1.6/dtmodel/models/bases/medical.py
+-rw-r--r--   0        0        0     4553 2023-06-26 15:26:46.569162 dtmodel-0.1.6/dtmodel/models/bases/people.py
+-rw-r--r--   0        0        0      279 2023-06-26 00:35:31.055604 dtmodel-0.1.6/dtmodel/models/bases/self_key.py
+-rw-r--r--   0        0        0       68 2023-06-13 17:57:46.458805 dtmodel-0.1.6/dtmodel/models/enums/__init__.py
+-rw-r--r--   0        0        0      272 2023-06-19 02:23:11.672713 dtmodel-0.1.6/dtmodel/models/enums/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1216 2023-06-19 12:37:15.474782 dtmodel-0.1.6/dtmodel/models/enums/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0      626 2023-06-25 13:52:41.415503 dtmodel-0.1.6/dtmodel/models/enums/__pycache__/medical.cpython-39.pyc
+-rw-r--r--   0        0        0      742 2023-06-19 12:37:15.473906 dtmodel-0.1.6/dtmodel/models/enums/__pycache__/person.cpython-39.pyc
+-rw-r--r--   0        0        0      786 2023-06-19 04:20:31.277660 dtmodel-0.1.6/dtmodel/models/enums/facility.py
+-rw-r--r--   0        0        0      303 2023-06-25 13:52:40.721450 dtmodel-0.1.6/dtmodel/models/enums/medical.py
+-rw-r--r--   0        0        0      325 2023-06-19 04:20:31.291877 dtmodel-0.1.6/dtmodel/models/enums/person.py
+-rw-r--r--   0        0        0     2214 2023-06-26 05:49:12.466739 dtmodel-0.1.6/dtmodel/models/facility.py
+-rw-r--r--   0        0        0     6846 2023-06-30 02:50:41.845137 dtmodel-0.1.6/dtmodel/models/medical.py
+-rw-r--r--   0        0        0     2409 2023-07-02 20:55:40.143060 dtmodel-0.1.6/dtmodel/models/people.py
+-rw-r--r--   0        0        0      139 2023-06-19 02:56:24.897397 dtmodel-0.1.6/dtmodel/parse/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-19 02:56:25.267120 dtmodel-0.1.6/dtmodel/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-18 19:03:56.455215 dtmodel-0.1.6/dtmodel/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1777 2023-06-26 02:56:37.269664 dtmodel-0.1.6/dtmodel/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-18 19:03:56.454017 dtmodel-0.1.6/dtmodel/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-18 19:03:56.454879 dtmodel-0.1.6/dtmodel/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-18 19:03:56.454360 dtmodel-0.1.6/dtmodel/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11323 2023-06-19 12:37:15.469170 dtmodel-0.1.6/dtmodel/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtmodel-0.1.6/dtmodel/parse/dates.py
+-rw-r--r--   0        0        0     1622 2023-06-26 02:56:36.643982 dtmodel-0.1.6/dtmodel/parse/json_encoder.py
+-rw-r--r--   0        0        0      372 2023-06-19 02:56:24.901051 dtmodel-0.1.6/dtmodel/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtmodel-0.1.6/dtmodel/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtmodel-0.1.6/dtmodel/parse/string.py
+-rw-r--r--   0        0        0    10883 2023-06-19 04:20:31.308863 dtmodel-0.1.6/dtmodel/parse/type_hint.py
+-rw-r--r--   0        0        0     2716 2023-07-02 22:16:54.734859 dtmodel-0.1.6/dtmodel/regex.py
+-rw-r--r--   0        0        0      629 2023-07-02 22:20:02.378405 dtmodel-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1100 2023-07-02 22:20:07.283291 dtmodel-0.1.6/setup.py
+-rw-r--r--   0        0        0      669 2023-07-02 22:20:07.283510 dtmodel-0.1.6/PKG-INFO
```

### Comparing `dtmodel-0.1.5/dtmodel/.env` & `dtmodel-0.1.6/dtmodel/.env`

 * *Files 22% similar despite different names*

```diff
@@ -21,8 +21,14 @@
 MEMED_API_KEY=iJGiB4kjDGOLeDFPWMG3no9VnN7Abpqe3w1jEFm6olkhkZD6oSfSmYCm
 MEMED_SECRET_KEY=Xe8M5GvBGCr4FStKfxXKisRo3SfYKI7KrTMkJpCAstzu2yXVN4av5nmL
 MEMED_FRONTEND_DOMAIN=integrations.memed.com.br
 MEMED_API_DOMAIN=integrations.api.memed.com.br
 GOOGLE_API_KEY=AIzaSyABE4zPjeCerBYow0Ehf115S8GyDRrfaZQ
 GOOGLE_APP_NAME=essencia-deta
 DETA_TOKEN=1rfGomYm_zG61cwoWjhfTCY7FBZWEbjVvJiPWXyBi
+FACILITY_NAME='Essência Psiquiatria'
+FACILITY_ADDRESS='R. Rodrigues Tomáz, 95'
+FACILITY_CITY=Anápolis/GO
+FACILITY_EMAIL=contato@essencia.me
+FACILITY_PHONE=+55(62)3979-0777
+AUTHOR='Daniel Victor Arantes'
```

### Comparing `dtmodel-0.1.5/dtmodel/bases/facility.py` & `dtmodel-0.1.6/dtmodel/models/bases/facility.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 __all__ = [
         'FacilityKey',
         'ServiceKey',
         'ServiceTypeBase',
-        'Payment'
+        'Payment',
+        'ServiceDate',
 ]
-
-from dtmodel.dtfield import dataclass, Validator, ContextBase, datetime, Decimal, ModelMap
-from ..enums import *
+from dtmodel.base import *
+from dtmodel.descriptor import *
+from dtmodel.models.enums import *
 
 @dataclass
-class FacilityKey(ContextBase):
-    facility_key: str = Validator(compare=False, label='Empresa', table='Facility', item_name='facility', default=None)
+class FacilityKey:
+    facility_key: Key = KeyValidator(compare=False, label='empresa', table='Facility', item_name='facility', default=None)
     
     
 @dataclass
-class ServiceKey(ContextBase):
-    service_key: str = Validator(compare=False, label='Serviço', table='Service', item_name='service')
-    
-    
+class ServiceKey:
+    service_key: Key = KeyValidator(compare=False, label='serviço', table='Service', item_name='service')
+
+
+@dataclass
+class ServiceDate:
+    service_date: datetime.date = DateValidator(default_factory=datetime.date.today, label='data do serviço')
+
+
 @dataclass
-class ServiceTypeBase(ContextBase):
-    type: ServiceType = Validator(hash=True)
+class ServiceTypeBase:
+    type: ServiceType = EnumValidator(hash=True, label='tipo de serviço')
 
 
 @dataclass
-class Payment(ContextBase):
-    payment_method: PaymentMethod = Validator(default='DI')
-    payment_value: Decimal = Validator(default=Decimal('0.0'))
-    payment_date: datetime.date = Validator(default_factory=datetime.date.today)
+class Payment:
+    payment_method: PaymentMethod = EnumValidator(default='CA', label='método de pagamento', field_size='col-sm-12 col-md-4')
+    payment_value: Decimal = NumberValidator(default=Decimal('0.0'), label='valor do pagamento', step=0.01, min=0, field_size='col-sm-12 col-md-4')
+    payment_date: datetime.date = DateValidator(default_factory=datetime.date.today, label='data de pagamento', field_size='col-sm-12 col-md-4')
     
     @classmethod
     async def total_payment(cls):
         return float(sum([Decimal(i.get('payment_value')) for i in await cls.fetch_all()])).__round__(2)
     
     
     @classmethod
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/__pycache__/_imports.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/base/__pycache__/_imports.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Jun 12 14:04:46 2023 UTC, .py size: 2014 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 fe25 8764 de07 0000  a........%.d....
+00000000: 610d 0d0a 0000 0000 d8c3 8f64 0509 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 6c01 0000 6700  .....@...sl...g.
+00000020: 0006 0000 0040 0000 0073 7401 0000 6700  .....@...st...g.
 00000030: 6400 a201 5a00 6401 6402 6c01 5a01 6401  d...Z.d.d.l.Z.d.
 00000040: 6402 6c02 5a02 6401 6402 6c03 5a03 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 5a04 6401 6402 6c05 5a05 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c06 6d07 5a07 0100 6401 6404 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 6d0a 5a0a 0100 6401 6405 6c0b  m.Z.m.Z...d.d.l.
 00000080: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000090: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
@@ -18,100 +18,111 @@
 00000110: 0100 6401 640a 6c2c 6d2d 5a2d 6d2e 5a2e  ..d.d.l,m-Z-m.Z.
 00000120: 6d2f 5a2f 6d30 5a30 6d31 5a31 6d32 5a32  m/Z/m0Z0m1Z1m2Z2
 00000130: 6d33 5a33 6d34 5a34 6d35 5a35 0100 6401  m3Z3m4Z4m5Z5..d.
 00000140: 640b 6c36 6d37 5a37 0100 6401 640c 6c38  d.l6m7Z7..d.d.l8
 00000150: 6d39 5a39 0100 6401 640d 6c3a 6d3b 5a3b  m9Z9..d.d.l:m;Z;
 00000160: 0100 6401 640e 6c3c 6d3d 5a3d 0100 6401  ..d.d.l<m=Z=..d.
 00000170: 640f 6c3e 6d3f 5a3f 6d40 5a40 6d41 5a41  d.l>m?Z?m@Z@mAZA
-00000180: 6d42 5a42 0100 6529 6532 6410 6410 6410  mBZB..e)e2d.d.d.
-00000190: 6411 8d04 5a43 6402 5300 2912 2936 da08  d...ZCd.S.).)6..
-000001a0: 6461 7465 7469 6d65 da11 6372 6561 7465  datetime..create
-000001b0: 5f74 6173 6b5f 6772 6f75 70da 0445 6e75  _task_group..Enu
-000001c0: 6dda 0555 6e69 6f6e da08 4f70 7469 6f6e  m..Union..Option
-000001d0: 616c da03 416e 79da 0843 616c 6c61 626c  al..Any..Callabl
-000001e0: 65da 0754 7970 6556 6172 da08 4974 6572  e..TypeVar..Iter
-000001f0: 6162 6c65 da04 5479 7065 da0a 4e61 6d65  able..Type..Name
-00000200: 6454 7570 6c65 da0a 5573 6572 5374 7269  dTuple..UserStri
-00000210: 6e67 da08 5573 6572 4469 6374 da08 5573  ng..UserDict..Us
-00000220: 6572 4c69 7374 da05 6465 7175 65da 0b64  erList..deque..d
-00000230: 6566 6175 6c74 6469 6374 da08 4368 6169  efaultdict..Chai
-00000240: 6e4d 6170 da07 436f 6e74 6578 74da 0a43  nMap..Context..C
-00000250: 6f6e 7465 7874 5661 72da 0c63 6f70 795f  ontextVar..copy_
-00000260: 636f 6e74 6578 74da 0577 7261 7073 da0d  context..wraps..
-00000270: 7061 7274 6961 6c6d 6574 686f 64da 0563  partialmethod..c
-00000280: 6163 6865 da07 7061 7274 6961 6cda 074d  ache..partial..M
-00000290: 6170 7069 6e67 da0a 6765 745f 6f72 6967  apping..get_orig
-000002a0: 696e da0e 6765 745f 7479 7065 5f68 696e  in..get_type_hin
-000002b0: 7473 da08 6765 745f 6172 6773 da04 5365  ts..get_args..Se
-000002c0: 6c66 da09 6461 7461 636c 6173 73da 0566  lf..dataclass..f
-000002d0: 6965 6c64 da06 6669 656c 6473 da07 4d49  ield..fields..MI
-000002e0: 5353 494e 47da 0546 6965 6c64 da0c 6973  SSING..Field..is
-000002f0: 5f64 6174 6163 6c61 7373 da07 4465 6369  _dataclass..Deci
-00000300: 6d61 6cda 0843 6c61 7373 5661 72da 0749  mal..ClassVar..I
-00000310: 6e69 7456 6172 da03 4142 43da 0e61 6273  nitVar..ABC..abs
-00000320: 7472 6163 746d 6574 686f 64da 0767 726f  tractmethod..gro
-00000330: 7570 6279 da04 6a73 6f6e da07 6173 796e  upby..json..asyn
-00000340: 6369 6fda 0775 7669 636f 726e da08 5265  cio..uvicorn..Re
-00000350: 7370 6f6e 7365 da0c 4854 4d4c 5265 7370  sponse..HTMLResp
-00000360: 6f6e 7365 da0c 4a53 4f4e 5265 7370 6f6e  onse..JSONRespon
-00000370: 7365 da10 5265 6469 7265 6374 5265 7370  se..RedirectResp
-00000380: 6f6e 7365 da07 5265 7175 6573 74da 0272  onse..Request..r
-00000390: 65da 0661 7364 6963 74da 0761 7374 7570  e..asdict..astup
-000003a0: 6c65 da08 5072 6f74 6f63 6f6c da0d 6465  le..Protocol..de
-000003b0: 7363 6461 7461 636c 6173 73e9 0000 0000  scdataclass.....
-000003c0: 4e29 0172 0300 0000 2902 7227 0000 0072  N).r....).r'...r
-000003d0: 2800 0000 290e 7204 0000 0072 0500 0000  (...).r....r....
-000003e0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-000003f0: 0900 0000 720a 0000 0072 0b00 0000 7219  ....r....r....r.
-00000400: 0000 0072 1b00 0000 721c 0000 0072 1a00  ...r....r....r..
-00000410: 0000 7225 0000 0072 3500 0000 2906 720c  ..r%...r5...).r.
-00000420: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
-00000430: 0000 7210 0000 0072 1100 0000 2903 7212  ..r....r....).r.
-00000440: 0000 0072 1300 0000 7214 0000 0029 0472  ...r....r....).r
-00000450: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00000460: 0000 0029 0172 2900 0000 2909 7220 0000  ...).r)...).r ..
-00000470: 0072 2100 0000 721f 0000 0072 2200 0000  .r!...r....r"...
-00000480: 7223 0000 0072 1e00 0000 7226 0000 0072  r#...r....r&...r
-00000490: 3300 0000 7234 0000 0029 0172 2400 0000  3...r4...).r$...
-000004a0: 2901 7202 0000 0029 0172 1d00 0000 2901  ).r....).r....).
-000004b0: 7231 0000 0029 0472 2d00 0000 722e 0000  r1...).r-...r...
-000004c0: 0072 2f00 0000 7230 0000 0046 2903 da02  .r/...r0...F)...
-000004d0: 6571 da04 7265 7072 da05 6f72 6465 7229  eq..repr..order)
-000004e0: 44da 075f 5f61 6c6c 5f5f 7201 0000 0072  D..__all__r....r
-000004f0: 2a00 0000 722b 0000 0072 3200 0000 722c  *...r+...r2...r,
-00000500: 0000 00da 0465 6e75 6d72 0300 0000 da03  .....enumr......
-00000510: 6162 6372 2700 0000 7228 0000 00da 0674  abcr'...r(.....t
-00000520: 7970 696e 6772 0400 0000 7205 0000 0072  ypingr....r....r
-00000530: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
-00000540: 0000 0072 0a00 0000 720b 0000 0072 1900  ...r....r....r..
-00000550: 0000 721b 0000 0072 1c00 0000 721a 0000  ..r....r....r...
-00000560: 0072 2500 0000 7235 0000 00da 0b63 6f6c  .r%...r5.....col
-00000570: 6c65 6374 696f 6e73 720c 0000 0072 0d00  lectionsr....r..
-00000580: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000590: 0072 1100 0000 5a0b 636f 6e74 6578 7476  .r....Z.contextv
-000005a0: 6172 7372 1200 0000 7213 0000 0072 1400  arsr....r....r..
-000005b0: 0000 da09 6675 6e63 746f 6f6c 7372 1500  ....functoolsr..
-000005c0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-000005d0: 00da 0969 7465 7274 6f6f 6c73 7229 0000  ...itertoolsr)..
-000005e0: 005a 0b64 6174 6163 6c61 7373 6573 7220  .Z.dataclassesr 
-000005f0: 0000 0072 2100 0000 721f 0000 0072 2200  ...r!...r....r".
-00000600: 0000 7223 0000 0072 1e00 0000 7226 0000  ..r#...r....r&..
-00000610: 0072 3300 0000 7234 0000 005a 0764 6563  .r3...r4...Z.dec
-00000620: 696d 616c 7224 0000 005a 0561 6e79 696f  imalr$...Z.anyio
-00000630: 7202 0000 005a 1174 7970 696e 675f 6578  r....Z.typing_ex
-00000640: 7465 6e73 696f 6e73 721d 0000 005a 1273  tensionsr....Z.s
-00000650: 7461 726c 6574 7465 2e72 6571 7565 7374  tarlette.request
-00000660: 7372 3100 0000 5a13 7374 6172 6c65 7474  sr1...Z.starlett
-00000670: 652e 7265 7370 6f6e 7365 7372 2d00 0000  e.responsesr-...
-00000680: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00000690: 3600 0000 a900 7242 0000 0072 4200 0000  6.....rB...rB...
-000006a0: fa72 2f55 7365 7273 2f64 616e 6965 6c61  .r/Users/daniela
-000006b0: 7261 6e74 6573 2f4c 6962 7261 7279 2f4d  rantes/Library/M
-000006c0: 6f62 696c 6520 446f 6375 6d65 6e74 732f  obile Documents/
-000006d0: 636f 6d7e 6170 706c 657e 436c 6f75 6444  com~apple~CloudD
-000006e0: 6f63 732f 4d79 2041 7070 732f 7079 7069  ocs/My Apps/pypi
-000006f0: 2f64 746d 6f64 656c 2f64 746d 6f64 656c  /dtmodel/dtmodel
-00000700: 2f64 7466 6965 6c64 2f5f 696d 706f 7274  /dtfield/_import
-00000710: 732e 7079 da08 3c6d 6f64 756c 653e 0100  s.py..<module>..
-00000720: 0000 7326 0000 0008 3908 0108 0108 0108  ..s&....9.......
-00000730: 0108 010c 0110 0140 0220 0114 0118 010c  .......@. ......
-00000740: 012c 010c 010c 010c 010c 0118 04         .,...........
+00000180: 6d42 5a42 0100 6401 6410 6c43 5400 6529  mBZB..d.d.lCT.e)
+00000190: 6532 6411 6411 6411 6412 8d04 5a44 6402  e2d.d.d.d...ZDd.
+000001a0: 5300 2913 2943 da08 6461 7465 7469 6d65  S.).)C..datetime
+000001b0: da11 6372 6561 7465 5f74 6173 6b5f 6772  ..create_task_gr
+000001c0: 6f75 70da 0445 6e75 6dda 0555 6e69 6f6e  oup..Enum..Union
+000001d0: da08 4f70 7469 6f6e 616c da03 416e 79da  ..Optional..Any.
+000001e0: 0843 616c 6c61 626c 65da 0754 7970 6556  .Callable..TypeV
+000001f0: 6172 da08 4974 6572 6162 6c65 da04 5479  ar..Iterable..Ty
+00000200: 7065 da0a 4e61 6d65 6454 7570 6c65 da0a  pe..NamedTuple..
+00000210: 5573 6572 5374 7269 6e67 da08 5573 6572  UserString..User
+00000220: 4469 6374 da08 5573 6572 4c69 7374 da05  Dict..UserList..
+00000230: 6465 7175 65da 0b64 6566 6175 6c74 6469  deque..defaultdi
+00000240: 6374 da08 4368 6169 6e4d 6170 da07 436f  ct..ChainMap..Co
+00000250: 6e74 6578 74da 0a43 6f6e 7465 7874 5661  ntext..ContextVa
+00000260: 72da 0c63 6f70 795f 636f 6e74 6578 74da  r..copy_context.
+00000270: 0577 7261 7073 da0d 7061 7274 6961 6c6d  .wraps..partialm
+00000280: 6574 686f 64da 0563 6163 6865 da07 7061  ethod..cache..pa
+00000290: 7274 6961 6cda 074d 6170 7069 6e67 da0a  rtial..Mapping..
+000002a0: 6765 745f 6f72 6967 696e da0e 6765 745f  get_origin..get_
+000002b0: 7479 7065 5f68 696e 7473 da08 6765 745f  type_hints..get_
+000002c0: 6172 6773 da04 5365 6c66 da09 6461 7461  args..Self..data
+000002d0: 636c 6173 73da 0566 6965 6c64 da06 6669  class..field..fi
+000002e0: 656c 6473 da07 4d49 5353 494e 47da 0546  elds..MISSING..F
+000002f0: 6965 6c64 da0c 6973 5f64 6174 6163 6c61  ield..is_datacla
+00000300: 7373 da07 4465 6369 6d61 6cda 0843 6c61  ss..Decimal..Cla
+00000310: 7373 5661 72da 0749 6e69 7456 6172 da03  ssVar..InitVar..
+00000320: 4142 43da 0e61 6273 7472 6163 746d 6574  ABC..abstractmet
+00000330: 686f 64da 0767 726f 7570 6279 da04 6a73  hod..groupby..js
+00000340: 6f6e da07 6173 796e 6369 6fda 0775 7669  on..asyncio..uvi
+00000350: 636f 726e da08 5265 7370 6f6e 7365 da0c  corn..Response..
+00000360: 4854 4d4c 5265 7370 6f6e 7365 da0c 4a53  HTMLResponse..JS
+00000370: 4f4e 5265 7370 6f6e 7365 da10 5265 6469  ONResponse..Redi
+00000380: 7265 6374 5265 7370 6f6e 7365 da07 5265  rectResponse..Re
+00000390: 7175 6573 74da 0272 65da 0661 7364 6963  quest..re..asdic
+000003a0: 74da 0761 7374 7570 6c65 da08 5072 6f74  t..astuple..Prot
+000003b0: 6f63 6f6c da0d 6465 7363 6461 7461 636c  ocol..descdatacl
+000003c0: 6173 735a 0944 6574 6151 7565 7279 5a08  assZ.DetaQueryZ.
+000003d0: 4465 7461 4261 7365 5a08 4578 7069 7265  DetaBaseZ.Expire
+000003e0: 4174 5a08 4578 7069 7265 496e 5a0b 4578  AtZ.ExpireInZ.Ex
+000003f0: 6973 7450 6172 616d 735a 084a 736f 6e61  istParamsZ.Jsona
+00000400: 626c 655a 0c4a 736f 6e53 6571 7565 6e63  bleZ.JsonSequenc
+00000410: 655a 0d4a 736f 6e50 7269 6d69 7469 7665  eZ.JsonPrimitive
+00000420: 5a0b 5365 6172 6368 5061 7261 6d5a 0744  Z.SearchParamZ.D
+00000430: 6574 614b 6579 5a08 4465 7461 4461 7461  etaKeyZ.DetaData
+00000440: 5a0a 4465 7461 436f 6e66 6967 5a06 636f  Z.DetaConfigZ.co
+00000450: 6e66 6967 e900 0000 004e 2901 7203 0000  nfig.....N).r...
+00000460: 0029 0272 2700 0000 7228 0000 0029 0e72  .).r'...r(...).r
+00000470: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00000480: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00000490: 0000 720b 0000 0072 1900 0000 721b 0000  ..r....r....r...
+000004a0: 0072 1c00 0000 721a 0000 0072 2500 0000  .r....r....r%...
+000004b0: 7235 0000 0029 0672 0c00 0000 720d 0000  r5...).r....r...
+000004c0: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
+000004d0: 7211 0000 0029 0372 1200 0000 7213 0000  r....).r....r...
+000004e0: 0072 1400 0000 2904 7215 0000 0072 1600  .r....).r....r..
+000004f0: 0000 7217 0000 0072 1800 0000 2901 7229  ..r....r....).r)
+00000500: 0000 0029 0972 2000 0000 7221 0000 0072  ...).r ...r!...r
+00000510: 1f00 0000 7222 0000 0072 2300 0000 721e  ....r"...r#...r.
+00000520: 0000 0072 2600 0000 7233 0000 0072 3400  ...r&...r3...r4.
+00000530: 0000 2901 7224 0000 0029 0172 0200 0000  ..).r$...).r....
+00000540: 2901 721d 0000 0029 0172 3100 0000 2904  ).r....).r1...).
+00000550: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
+00000560: 3000 0000 2901 da01 2a46 2903 da02 6571  0...)...*F)...eq
+00000570: da04 7265 7072 da05 6f72 6465 7229 45da  ..repr..order)E.
+00000580: 075f 5f61 6c6c 5f5f 7201 0000 0072 2a00  .__all__r....r*.
+00000590: 0000 722b 0000 0072 3200 0000 722c 0000  ..r+...r2...r,..
+000005a0: 00da 0465 6e75 6d72 0300 0000 da03 6162  ...enumr......ab
+000005b0: 6372 2700 0000 7228 0000 00da 0674 7970  cr'...r(.....typ
+000005c0: 696e 6772 0400 0000 7205 0000 0072 0600  ingr....r....r..
+000005d0: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+000005e0: 0072 0a00 0000 720b 0000 0072 1900 0000  .r....r....r....
+000005f0: 721b 0000 0072 1c00 0000 721a 0000 0072  r....r....r....r
+00000600: 2500 0000 7235 0000 00da 0b63 6f6c 6c65  %...r5.....colle
+00000610: 6374 696f 6e73 720c 0000 0072 0d00 0000  ctionsr....r....
+00000620: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000630: 1100 0000 5a0b 636f 6e74 6578 7476 6172  ....Z.contextvar
+00000640: 7372 1200 0000 7213 0000 0072 1400 0000  sr....r....r....
+00000650: da09 6675 6e63 746f 6f6c 7372 1500 0000  ..functoolsr....
+00000660: 7216 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00000670: 0969 7465 7274 6f6f 6c73 7229 0000 005a  .itertoolsr)...Z
+00000680: 0b64 6174 6163 6c61 7373 6573 7220 0000  .dataclassesr ..
+00000690: 0072 2100 0000 721f 0000 0072 2200 0000  .r!...r....r"...
+000006a0: 7223 0000 0072 1e00 0000 7226 0000 0072  r#...r....r&...r
+000006b0: 3300 0000 7234 0000 005a 0764 6563 696d  3...r4...Z.decim
+000006c0: 616c 7224 0000 005a 0561 6e79 696f 7202  alr$...Z.anyior.
+000006d0: 0000 005a 1174 7970 696e 675f 6578 7465  ...Z.typing_exte
+000006e0: 6e73 696f 6e73 721d 0000 005a 1273 7461  nsionsr....Z.sta
+000006f0: 726c 6574 7465 2e72 6571 7565 7374 7372  rlette.requestsr
+00000700: 3100 0000 5a13 7374 6172 6c65 7474 652e  1...Z.starlette.
+00000710: 7265 7370 6f6e 7365 7372 2d00 0000 722e  responsesr-...r.
+00000720: 0000 0072 2f00 0000 7230 0000 005a 0664  ...r/...r0...Z.d
+00000730: 7462 6173 6572 3600 0000 a900 7243 0000  tbaser6.....rC..
+00000740: 0072 4300 0000 fa73 2f55 7365 7273 2f64  .rC....s/Users/d
+00000750: 616e 6965 6c61 7261 6e74 6573 2f4c 6962  anielarantes/Lib
+00000760: 7261 7279 2f4d 6f62 696c 6520 446f 6375  rary/Mobile Docu
+00000770: 6d65 6e74 732f 636f 6d7e 6170 706c 657e  ments/com~apple~
+00000780: 436c 6f75 6444 6f63 732f 4d79 2041 7070  CloudDocs/My App
+00000790: 732f 7079 7069 2f64 746d 6f64 656c 2f64  s/pypi/dtmodel/d
+000007a0: 746d 6f64 656c 2f61 6273 7472 6163 742f  tmodel/abstract/
+000007b0: 5f69 6d70 6f72 7473 2e70 79da 083c 6d6f  _imports.py..<mo
+000007c0: 6475 6c65 3e01 0000 0073 2800 0000 0846  dule>....s(....F
+000007d0: 0801 0801 0801 0801 0801 0c01 1001 4002  ..............@.
+000007e0: 2001 1401 1801 0c01 2c01 0c01 0c01 0c01   .......,.......
+000007f0: 0c01 1801 0803                           ......
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/__pycache__/base_enum.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/base/__pycache__/base_enum.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 18 01:52:52 2023 UTC, .py size: 1397 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7463 8e64 7505 0000  a.......tc.du...
+00000000: 610d 0d0a 0000 0000 ac08 9964 8a05 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6701 5a00 6401 6402 6c01 6d02 5a02 0100  g.Z.d.d.l.m.Z...
 00000040: 4700 6403 6400 8400 6400 6502 8303 5a03  G.d.d...d.e...Z.
 00000050: 6404 5300 2905 da08 4261 7365 456e 756d  d.S.)...BaseEnum
 00000060: e900 0000 0029 01da 0445 6e75 6d63 0000  .....)...Enumc..
 00000070: 0000 0000 0000 0000 0000 0000 0000 0500  ................
@@ -21,126 +21,127 @@
 00000140: 0200 0000 0400 0000 4300 0000 731e 0000  ........C...s...
 00000150: 0074 007c 0174 017c 0083 0183 0272 1a7c  .t.|.t.|.....r.|
 00000160: 006a 027c 016a 026b 0253 0074 0353 00a9  .j.|.j.k.S.t.S..
 00000170: 014e 2904 da0a 6973 696e 7374 616e 6365  .N)...isinstance
 00000180: da04 7479 7065 da04 6e61 6d65 da0e 4e6f  ..type..name..No
 00000190: 7449 6d70 6c65 6d65 6e74 6564 a902 da04  tImplemented....
 000001a0: 7365 6c66 da05 6f74 6865 72a9 0072 0c00  self..other..r..
-000001b0: 0000 fa73 2f55 7365 7273 2f64 616e 6965  ...s/Users/danie
+000001b0: 0000 fa70 2f55 7365 7273 2f64 616e 6965  ...p/Users/danie
 000001c0: 6c61 7261 6e74 6573 2f4c 6962 7261 7279  larantes/Library
 000001d0: 2f4d 6f62 696c 6520 446f 6375 6d65 6e74  /Mobile Document
 000001e0: 732f 636f 6d7e 6170 706c 657e 436c 6f75  s/com~apple~Clou
 000001f0: 6444 6f63 732f 4d79 2041 7070 732f 7079  dDocs/My Apps/py
 00000200: 7069 2f64 746d 6f64 656c 2f64 746d 6f64  pi/dtmodel/dtmod
-00000210: 656c 2f64 7466 6965 6c64 2f62 6173 655f  el/dtfield/base_
-00000220: 656e 756d 2e70 79da 065f 5f65 715f 5f09  enum.py..__eq__.
-00000230: 0000 0073 0600 0000 0001 0e01 0c01 7a0f  ...s..........z.
-00000240: 4261 7365 456e 756d 2e5f 5f65 715f 5f63  BaseEnum.__eq__c
-00000250: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000260: 0400 0000 4300 0000 731e 0000 0074 007c  ....C...s....t.|
-00000270: 0174 017c 0083 0183 0272 1a7c 006a 027c  .t.|.....r.|.j.|
-00000280: 016a 026b 0053 0074 0353 0072 0400 0000  .j.k.S.t.S.r....
-00000290: 2904 7205 0000 0072 0600 0000 da05 7661  ).r....r......va
-000002a0: 6c75 6572 0800 0000 7209 0000 0072 0c00  luer....r....r..
-000002b0: 0000 720c 0000 0072 0d00 0000 da06 5f5f  ..r....r......__
-000002c0: 6c74 5f5f 0e00 0000 7306 0000 0000 010e  lt__....s.......
-000002d0: 010c 017a 0f42 6173 6545 6e75 6d2e 5f5f  ...z.BaseEnum.__
-000002e0: 6c74 5f5f 6301 0000 0000 0000 0000 0000  lt__c...........
-000002f0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000300: 0000 7c00 6a00 5300 7204 0000 0029 01da  ..|.j.S.r....)..
-00000310: 085f 5f6e 616d 655f 5fa9 01da 0363 6c73  .__name__....cls
-00000320: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000330: 0574 6162 6c65 1300 0000 7302 0000 0000  .table....s.....
-00000340: 027a 0e42 6173 6545 6e75 6d2e 7461 626c  .z.BaseEnum.tabl
-00000350: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000360: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-00000370: 006a 0053 0072 0400 0000 a901 7207 0000  .j.S.r......r...
-00000380: 00a9 0172 0a00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000390: 0000 720d 0000 00da 046a 736f 6e17 0000  ..r......json...
-000003a0: 0073 0200 0000 0001 7a0d 4261 7365 456e  .s......z.BaseEn
-000003b0: 756d 2e6a 736f 6e63 0100 0000 0000 0000  um.jsonc........
-000003c0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000003d0: 7306 0000 007c 006a 0053 0072 0400 0000  s....|.j.S.r....
-000003e0: 7215 0000 0072 1600 0000 720c 0000 0072  r....r....r....r
-000003f0: 0c00 0000 720d 0000 00da 036b 6579 1a00  ....r......key..
-00000400: 0000 7302 0000 0000 027a 0c42 6173 6545  ..s......z.BaseE
-00000410: 6e75 6d2e 6b65 7963 0100 0000 0000 0000  num.keyc........
-00000420: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000430: 7306 0000 007c 006a 0053 0072 0400 0000  s....|.j.S.r....
-00000440: a901 720f 0000 0072 1600 0000 720c 0000  ..r....r....r...
-00000450: 0072 0c00 0000 720d 0000 00da 075f 5f73  .r....r......__s
-00000460: 7472 5f5f 1e00 0000 7302 0000 0000 017a  tr__....s......z
-00000470: 1042 6173 6545 6e75 6d2e 5f5f 7374 725f  .BaseEnum.__str_
-00000480: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00000490: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-000004a0: 006a 0053 0072 0400 0000 7219 0000 0072  .j.S.r....r....r
-000004b0: 1600 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000004c0: 0000 00da 0764 6973 706c 6179 2100 0000  .....display!...
-000004d0: 7302 0000 0000 027a 1042 6173 6545 6e75  s......z.BaseEnu
-000004e0: 6d2e 6469 7370 6c61 7963 0100 0000 0000  m.displayc......
-000004f0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000500: 0000 730a 0000 007c 006a 00a0 01a1 0053  ..s....|.j.....S
-00000510: 0072 0400 0000 2902 da0b 5f5f 6d65 6d62  .r....)...__memb
-00000520: 6572 735f 5fda 0676 616c 7565 7372 1200  ers__..valuesr..
-00000530: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000540: 00da 076d 656d 6265 7273 2500 0000 7302  ...members%...s.
-00000550: 0000 0000 027a 1042 6173 6545 6e75 6d2e  .....z.BaseEnum.
-00000560: 6d65 6d62 6572 734e 4629 02da 0469 7465  membersNF)...ite
-00000570: 6dda 0873 656c 6563 7465 6463 0300 0000  m..selectedc....
-00000580: 0000 0000 0000 0000 0300 0000 0b00 0000  ................
-00000590: 4300 0000 7344 0000 007c 0173 0864 0153  C...sD...|.s.d.S
-000005a0: 0064 0274 007c 0183 016a 019b 0064 037c  .d.t.|...j...d.|
-000005b0: 016a 029b 0064 047c 016a 029b 0064 057c  .j...d.|.j...d.|
-000005c0: 0264 0675 0072 3264 076e 0264 089b 0064  .d.u.r2d.n.d...d
-000005d0: 097c 016a 039b 0064 0a9d 0b53 0029 0b4e  .|.j...d...S.).N
-000005e0: 7a11 3c6f 7074 696f 6e3e 3c2f 6f70 7469  z.<option></opti
-000005f0: 6f6e 3e7a 0c3c 6f70 7469 6f6e 2069 643d  on>z.<option id=
-00000600: 22da 012e 7a09 2220 7661 6c75 653d 227a  "...z." value="z
-00000610: 0222 2054 7220 0000 00da 00da 013e 7a09  ." Tr .......>z.
-00000620: 3c2f 6f70 7469 6f6e 3e29 0472 0600 0000  </option>).r....
-00000630: 7211 0000 0072 1800 0000 721b 0000 0029  r....r....r....)
-00000640: 0372 1300 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00000650: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000660: 066f 7074 696f 6e29 0000 0073 0e00 0000  .option)...s....
-00000670: 0002 0401 0401 1e01 0eff 0401 04ff 7a0f  ..............z.
-00000680: 4261 7365 456e 756d 2e6f 7074 696f 6e29  BaseEnum.option)
-00000690: 01da 0764 6566 6175 6c74 6302 0000 0000  ...defaultc.....
-000006a0: 0000 0000 0000 0002 0000 0006 0000 0003  ................
-000006b0: 0000 0073 3c00 0000 8801 7214 7400 8801  ...s<.....r.t...
-000006c0: 8800 8302 7214 8801 6a01 8901 6401 a002  ....r...j...d...
-000006d0: 8800 a003 a100 6701 8700 8701 6602 6402  ......g.....f.d.
-000006e0: 6403 8408 8800 a004 a100 4400 8301 a201  d.........D.....
-000006f0: a101 5300 2904 4e72 2200 0000 6301 0000  ..S.).Nr"...c...
-00000700: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-00000710: 0013 0000 0073 1e00 0000 6700 7c00 5d16  .....s....g.|.].
-00000720: 7d01 8800 a000 7c01 7c01 6a01 8801 6b02  }.....|.|.j...k.
-00000730: a102 9102 7104 5300 720c 0000 0029 0272  ....q.S.r....).r
-00000740: 2400 0000 7218 0000 0029 02da 022e 30da  $...r....)....0.
-00000750: 066d 656d 6265 72a9 0272 1300 0000 7225  .member..r....r%
-00000760: 0000 0072 0c00 0000 720d 0000 00da 0a3c  ...r....r......<
-00000770: 6c69 7374 636f 6d70 3e35 0000 00f3 0000  listcomp>5......
-00000780: 0000 7a24 4261 7365 456e 756d 2e6f 7074  ..z$BaseEnum.opt
-00000790: 696f 6e73 2e3c 6c6f 6361 6c73 3e2e 3c6c  ions.<locals>.<l
-000007a0: 6973 7463 6f6d 703e 2905 7205 0000 0072  istcomp>).r....r
-000007b0: 0700 0000 da04 6a6f 696e 7224 0000 0072  ......joinr$...r
-000007c0: 1e00 0000 7228 0000 0072 0c00 0000 7228  ....r(...r....r(
-000007d0: 0000 0072 0d00 0000 da07 6f70 7469 6f6e  ...r......option
-000007e0: 7330 0000 0073 0800 0000 0002 0401 0a01  s0...s..........
-000007f0: 0601 7a10 4261 7365 456e 756d 2e6f 7074  ..z.BaseEnum.opt
-00000800: 696f 6e73 2902 4e46 2901 4e29 1272 1100  ions).NF).N).r..
-00000810: 0000 da0a 5f5f 6d6f 6475 6c65 5f5f da0c  ....__module__..
-00000820: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00000830: 646f 635f 5f72 0e00 0000 7210 0000 00da  doc__r....r.....
-00000840: 0b63 6c61 7373 6d65 7468 6f64 7214 0000  .classmethodr...
-00000850: 0072 1700 0000 da08 7072 6f70 6572 7479  .r......property
-00000860: 7218 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000870: 1e00 0000 da04 626f 6f6c 7224 0000 00da  ......boolr$....
-00000880: 0373 7472 722c 0000 0072 0c00 0000 720c  .strr,...r....r.
-00000890: 0000 0072 0c00 0000 720d 0000 0072 0100  ...r....r....r..
-000008a0: 0000 0600 0000 7322 0000 0008 0104 0208  ......s"........
-000008b0: 0508 0502 010a 0308 0302 010a 0308 0302  ................
-000008c0: 010a 0302 010a 0302 0114 0602 014e 2904  .............N).
-000008d0: da07 5f5f 616c 6c5f 5f5a 0f64 746d 6f64  ..__all__Z.dtmod
-000008e0: 656c 2e64 7466 6965 6c64 7203 0000 0072  el.dtfieldr....r
-000008f0: 0100 0000 720c 0000 0072 0c00 0000 720c  ....r....r....r.
-00000900: 0000 0072 0d00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000910: 653e 0100 0000 7304 0000 0006 030c 02    e>....s........
+00000210: 656c 2f62 6173 652f 6261 7365 5f65 6e75  el/base/base_enu
+00000220: 6d2e 7079 da06 5f5f 6571 5f5f 0900 0000  m.py..__eq__....
+00000230: 7306 0000 0000 010e 010c 017a 0f42 6173  s..........z.Bas
+00000240: 6545 6e75 6d2e 5f5f 6571 5f5f 6302 0000  eEnum.__eq__c...
+00000250: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000260: 0043 0000 0073 1e00 0000 7400 7c01 7401  .C...s....t.|.t.
+00000270: 7c00 8301 8302 721a 7c00 6a02 7c01 6a02  |.....r.|.j.|.j.
+00000280: 6b00 5300 7403 5300 7204 0000 0029 0472  k.S.t.S.r....).r
+00000290: 0500 0000 7206 0000 00da 0576 616c 7565  ....r......value
+000002a0: 7208 0000 0072 0900 0000 720c 0000 0072  r....r....r....r
+000002b0: 0c00 0000 720d 0000 00da 065f 5f6c 745f  ....r......__lt_
+000002c0: 5f0e 0000 0073 0600 0000 0001 0e01 0c01  _....s..........
+000002d0: 7a0f 4261 7365 456e 756d 2e5f 5f6c 745f  z.BaseEnum.__lt_
+000002e0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+000002f0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00000300: 006a 0053 0072 0400 0000 2901 da08 5f5f  .j.S.r....)...__
+00000310: 6e61 6d65 5f5f a901 da03 636c 7372 0c00  name__....clsr..
+00000320: 0000 720c 0000 0072 0d00 0000 da05 7461  ..r....r......ta
+00000330: 626c 6513 0000 0073 0200 0000 0002 7a0e  ble....s......z.
+00000340: 4261 7365 456e 756d 2e74 6162 6c65 6301  BaseEnum.tablec.
+00000350: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000360: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+00000370: 5300 7204 0000 00a9 0172 0700 0000 a901  S.r......r......
+00000380: 720a 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000390: 0d00 0000 da04 6a73 6f6e 1700 0000 7302  ......json....s.
+000003a0: 0000 0000 017a 0d42 6173 6545 6e75 6d2e  .....z.BaseEnum.
+000003b0: 6a73 6f6e 6301 0000 0000 0000 0000 0000  jsonc...........
+000003c0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+000003d0: 0000 7c00 6a00 5300 7204 0000 0072 1500  ..|.j.S.r....r..
+000003e0: 0000 7216 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+000003f0: 0072 0d00 0000 da03 6b65 791a 0000 0073  .r......key....s
+00000400: 0200 0000 0002 7a0c 4261 7365 456e 756d  ......z.BaseEnum
+00000410: 2e6b 6579 6301 0000 0000 0000 0000 0000  .keyc...........
+00000420: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+00000430: 0000 7c00 6a00 5300 7204 0000 00a9 0172  ..|.j.S.r......r
+00000440: 0f00 0000 7216 0000 0072 0c00 0000 720c  ....r....r....r.
+00000450: 0000 0072 0d00 0000 da07 5f5f 7374 725f  ...r......__str_
+00000460: 5f1e 0000 0073 0200 0000 0001 7a10 4261  _....s......z.Ba
+00000470: 7365 456e 756d 2e5f 5f73 7472 5f5f 6301  seEnum.__str__c.
+00000480: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000490: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+000004a0: 5300 7204 0000 0072 1900 0000 7216 0000  S.r....r....r...
+000004b0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000004c0: da07 6469 7370 6c61 7921 0000 0073 0200  ..display!...s..
+000004d0: 0000 0002 7a10 4261 7365 456e 756d 2e64  ....z.BaseEnum.d
+000004e0: 6973 706c 6179 6301 0000 0000 0000 0000  isplayc.........
+000004f0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000500: 0a00 0000 7c00 6a00 a001 a100 5300 7204  ....|.j.....S.r.
+00000510: 0000 0029 02da 0b5f 5f6d 656d 6265 7273  ...)...__members
+00000520: 5f5f da06 7661 6c75 6573 7212 0000 0072  __..valuesr....r
+00000530: 0c00 0000 720c 0000 0072 0d00 0000 da07  ....r....r......
+00000540: 6d65 6d62 6572 7325 0000 0073 0200 0000  members%...s....
+00000550: 0002 7a10 4261 7365 456e 756d 2e6d 656d  ..z.BaseEnum.mem
+00000560: 6265 7273 4e46 2902 da04 6974 656d da08  bersNF)...item..
+00000570: 7365 6c65 6374 6564 6303 0000 0000 0000  selectedc.......
+00000580: 0000 0000 0003 0000 000b 0000 0043 0000  .............C..
+00000590: 0073 4400 0000 7c01 7308 6401 5300 6402  .sD...|.s.d.S.d.
+000005a0: 7400 7c01 8301 6a01 9b00 6403 7c01 6a02  t.|...j...d.|.j.
+000005b0: 9b00 6404 7c01 6a02 9b00 6405 7c02 6406  ..d.|.j...d.|.d.
+000005c0: 7500 7232 6407 6e02 6408 9b00 6409 7c01  u.r2d.n.d...d.|.
+000005d0: 6a03 9b00 640a 9d0b 5300 290b 4e7a 113c  j...d...S.).Nz.<
+000005e0: 6f70 7469 6f6e 3e3c 2f6f 7074 696f 6e3e  option></option>
+000005f0: 7a0c 3c6f 7074 696f 6e20 6964 3d22 da01  z.<option id="..
+00000600: 2e7a 0922 2076 616c 7565 3d22 7a02 2220  .z." value="z." 
+00000610: 5472 2000 0000 da00 da01 3e7a 093c 2f6f  Tr .......>z.</o
+00000620: 7074 696f 6e3e 2904 7206 0000 0072 1100  ption>).r....r..
+00000630: 0000 7218 0000 0072 1b00 0000 2903 7213  ..r....r....).r.
+00000640: 0000 0072 1f00 0000 7220 0000 0072 0c00  ...r....r ...r..
+00000650: 0000 720c 0000 0072 0d00 0000 da06 6f70  ..r....r......op
+00000660: 7469 6f6e 2900 0000 730e 0000 0000 0204  tion)...s.......
+00000670: 0104 011e 010e ff04 0104 ff7a 0f42 6173  ...........z.Bas
+00000680: 6545 6e75 6d2e 6f70 7469 6f6e 2901 da07  eEnum.option)...
+00000690: 6465 6661 756c 7463 0200 0000 0000 0000  defaultc........
+000006a0: 0000 0000 0200 0000 0600 0000 0300 0000  ................
+000006b0: 7344 0000 0074 0088 0183 0101 0088 0172  sD...t.........r
+000006c0: 1c74 0188 0188 0083 0272 1c88 016a 0289  .t.......r...j..
+000006d0: 0164 01a0 0388 00a0 04a1 0067 0187 0087  .d.........g....
+000006e0: 0166 0264 0264 0384 0888 00a0 05a1 0044  .f.d.d.........D
+000006f0: 0083 01a2 01a1 0153 0029 044e 7222 0000  .......S.).Nr"..
+00000700: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000710: 0000 0700 0000 1300 0000 731e 0000 0067  ..........s....g
+00000720: 007c 005d 167d 0188 00a0 007c 017c 016a  .|.].}.....|.|.j
+00000730: 0188 016b 02a1 0291 0271 0453 0072 0c00  ...k.....q.S.r..
+00000740: 0000 2902 7224 0000 0072 1800 0000 2902  ..).r$...r....).
+00000750: da02 2e30 da06 6d65 6d62 6572 a902 7213  ...0..member..r.
+00000760: 0000 0072 2500 0000 720c 0000 0072 0d00  ...r%...r....r..
+00000770: 0000 da0a 3c6c 6973 7463 6f6d 703e 3700  ....<listcomp>7.
+00000780: 0000 f300 0000 007a 2442 6173 6545 6e75  .......z$BaseEnu
+00000790: 6d2e 6f70 7469 6f6e 732e 3c6c 6f63 616c  m.options.<local
+000007a0: 733e 2e3c 6c69 7374 636f 6d70 3e29 06da  s>.<listcomp>)..
+000007b0: 0570 7269 6e74 7205 0000 0072 0700 0000  .printr....r....
+000007c0: da04 6a6f 696e 7224 0000 0072 1e00 0000  ..joinr$...r....
+000007d0: 7228 0000 0072 0c00 0000 7228 0000 0072  r(...r....r(...r
+000007e0: 0d00 0000 da07 6f70 7469 6f6e 7330 0000  ......options0..
+000007f0: 0073 0a00 0000 0002 0802 0401 0a01 0601  .s..............
+00000800: 7a10 4261 7365 456e 756d 2e6f 7074 696f  z.BaseEnum.optio
+00000810: 6e73 2902 4e46 2901 4e29 1272 1100 0000  ns).NF).N).r....
+00000820: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000830: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000840: 635f 5f72 0e00 0000 7210 0000 00da 0b63  c__r....r......c
+00000850: 6c61 7373 6d65 7468 6f64 7214 0000 0072  lassmethodr....r
+00000860: 1700 0000 da08 7072 6f70 6572 7479 7218  ......propertyr.
+00000870: 0000 0072 1a00 0000 721b 0000 0072 1e00  ...r....r....r..
+00000880: 0000 da04 626f 6f6c 7224 0000 00da 0373  ....boolr$.....s
+00000890: 7472 722d 0000 0072 0c00 0000 720c 0000  trr-...r....r...
+000008a0: 0072 0c00 0000 720d 0000 0072 0100 0000  .r....r....r....
+000008b0: 0600 0000 7322 0000 0008 0104 0208 0508  ....s"..........
+000008c0: 0502 010a 0308 0302 010a 0308 0302 010a  ................
+000008d0: 0302 010a 0302 0114 0602 014e 2904 da07  ...........N)...
+000008e0: 5f5f 616c 6c5f 5fda 0465 6e75 6d72 0300  __all__..enumr..
+000008f0: 0000 7201 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000900: 0072 0c00 0000 720d 0000 00da 083c 6d6f  .r....r......<mo
+00000910: 6475 6c65 3e01 0000 0073 0400 0000 0603  dule>....s......
+00000920: 0c02                                     ..
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/_imports.py` & `dtmodel-0.1.6/dtmodel/base/_imports.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,15 +48,28 @@
         'JSONResponse',
         'RedirectResponse',
         'Request',
         're',
         'asdict',
         'astuple',
         'Protocol',
-        'descdataclass'
+        'descdataclass',
+        'DetaQuery',
+        'DetaBase',
+        'ExpireAt',
+        'ExpireIn',
+        'ExistParams',
+        'Jsonable',
+        'JsonSequence',
+        'JsonPrimitive',
+        'SearchParam',
+        'DetaKey',
+        'DetaData',
+        'DetaConfig',
+        'config'
 ]
 
 import datetime
 import json
 import asyncio
 import re
 import uvicorn
@@ -70,11 +83,11 @@
 from itertools import groupby
 from dataclasses import fields, MISSING, field, Field, is_dataclass, dataclass, InitVar, asdict, astuple
 from decimal import Decimal
 from anyio import create_task_group
 from typing_extensions import Self
 from starlette.requests import Request
 from starlette.responses import Response, HTMLResponse, JSONResponse, RedirectResponse
-
+from dtbase import *
 
 
 descdataclass = partial(dataclass, eq=False, repr=False, order=False)
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/base_enum.py` & `dtmodel-0.1.6/dtmodel/base/base_enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __all__ = ['BaseEnum']
 
 
-from dtmodel.dtfield import Enum
+from enum import Enum
 
 class BaseEnum(Enum):
     """Enum base model class"""
     
     def __eq__(self, other):
         if isinstance(other, type(self)):
             return self.name == other.name
@@ -43,12 +43,14 @@
         if not item:
             return '<option></option>'
         return f'<option id="{type(item).__name__}.{item.key}" value="{item.key}" ' \
                f'{"selected" if selected is True else ""}>{item.display}</option>'
     
     @classmethod
     def options(cls, default: str = None):
+        print(default)
+        
         if default:
             if isinstance(default, cls):
                 default = default.name
         return ''.join([cls.option(), *[cls.option(member, member.key == default) for member in cls.members()]])
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/parse/__pycache__/dates.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 11 02:28:20 2023 UTC, .py size: 694 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,35 @@
 000000e0: 7c00 8301 7401 6a01 7500 7226 7c00 6a02  |...t.j.u.r&|.j.
 000000f0: 5300 7403 7c00 7404 8302 723c 7401 6a02  S.t.|.t...r<t.j.
 00000100: a005 7c00 a101 5300 7c00 5300 a901 4e29  ..|...S.|.S...N)
 00000110: 06da 0474 7970 65da 0864 6174 6574 696d  ...type..datetim
 00000120: 65da 0464 6174 65da 0a69 7369 6e73 7461  e..date..isinsta
 00000130: 6e63 65da 0373 7472 da0d 6672 6f6d 6973  nce..str..fromis
 00000140: 6f66 6f72 6d61 74a9 0172 0500 0000 a900  oformat..r......
-00000150: 720f 0000 00fa 752f 5573 6572 732f 6461  r.....u/Users/da
+00000150: 720f 0000 00fa 6d2f 5573 6572 732f 6461  r.....m/Users/da
 00000160: 6e69 656c 6172 616e 7465 732f 4c69 6272  nielarantes/Libr
 00000170: 6172 792f 4d6f 6269 6c65 2044 6f63 756d  ary/Mobile Docum
 00000180: 656e 7473 2f63 6f6d 7e61 7070 6c65 7e43  ents/com~apple~C
 00000190: 6c6f 7564 446f 6373 2f4d 7920 4170 7073  loudDocs/My Apps
 000001a0: 2f70 7970 692f 6474 6d6f 6465 6c2f 6474  /pypi/dtmodel/dt
-000001b0: 6d6f 6465 6c2f 6474 6669 656c 642f 7061  model/dtfield/pa
-000001c0: 7273 652f 6461 7465 732e 7079 7201 0000  rse/dates.pyr...
-000001d0: 0007 0000 0073 0e00 0000 0001 0e01 0401  .....s..........
-000001e0: 0e01 0601 0a01 0c01 6301 0000 0000 0000  ........c.......
-000001f0: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-00000200: 0073 4e00 0000 7400 7c00 8301 7401 6a02  .sN...t.|...t.j.
-00000210: 7500 7222 7401 a001 7c00 6a03 7c00 6a04  u.r"t...|.j.|.j.
-00000220: 7c00 6a02 a103 5300 7400 7c00 8301 7401  |.j...S.t.|...t.
-00000230: 6a01 7500 7234 7c00 5300 7405 7c00 7406  j.u.r4|.S.t.|.t.
-00000240: 8302 724a 7401 6a01 a007 7c00 a101 5300  ..rJt.j...|...S.
-00000250: 7c00 5300 7207 0000 0029 0872 0800 0000  |.S.r....).r....
-00000260: 7209 0000 0072 0a00 0000 da04 7965 6172  r....r......year
-00000270: da05 6d6f 6e74 6872 0b00 0000 720c 0000  ..monthr....r...
-00000280: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000290: 720f 0000 0072 1000 0000 7202 0000 0011  r....r....r.....
-000002a0: 0000 0073 0e00 0000 0001 0e01 1401 0e01  ...s............
-000002b0: 0401 0a01 0c01 2907 da07 5f5f 616c 6c5f  ......)...__all_
-000002c0: 5fda 0674 7970 696e 6772 0400 0000 7209  _..typingr....r.
-000002d0: 0000 0072 0a00 0000 7201 0000 0072 0200  ...r....r....r..
-000002e0: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-000002f0: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000300: 0100 0000 7308 0000 0008 020c 0108 0312  ....s...........
-00000310: 0a                                       .
+000001b0: 6d6f 6465 6c2f 7061 7273 652f 6461 7465  model/parse/date
+000001c0: 732e 7079 7201 0000 0007 0000 0073 0e00  s.pyr........s..
+000001d0: 0000 0001 0e01 0401 0e01 0601 0a01 0c01  ................
+000001e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000001f0: 0005 0000 0043 0000 0073 4e00 0000 7400  .....C...sN...t.
+00000200: 7c00 8301 7401 6a02 7500 7222 7401 a001  |...t.j.u.r"t...
+00000210: 7c00 6a03 7c00 6a04 7c00 6a02 a103 5300  |.j.|.j.|.j...S.
+00000220: 7400 7c00 8301 7401 6a01 7500 7234 7c00  t.|...t.j.u.r4|.
+00000230: 5300 7405 7c00 7406 8302 724a 7401 6a01  S.t.|.t...rJt.j.
+00000240: a007 7c00 a101 5300 7c00 5300 7207 0000  ..|...S.|.S.r...
+00000250: 0029 0872 0800 0000 7209 0000 0072 0a00  .).r....r....r..
+00000260: 0000 da04 7965 6172 da05 6d6f 6e74 6872  ....year..monthr
+00000270: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
+00000280: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+00000290: 0000 7202 0000 0011 0000 0073 0e00 0000  ..r........s....
+000002a0: 0001 0e01 1401 0e01 0401 0a01 0c01 2907  ..............).
+000002b0: da07 5f5f 616c 6c5f 5fda 0674 7970 696e  ..__all__..typin
+000002c0: 6772 0400 0000 7209 0000 0072 0a00 0000  gr....r....r....
+000002d0: 7201 0000 0072 0200 0000 720f 0000 0072  r....r....r....r
+000002e0: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+000002f0: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000300: 0008 020c 0108 0312 0a                   .........
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 18 01:53:05 2023 UTC, .py size: 1551 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8163 8e64 0f06 0000  a........c.d....
+00000000: 610d 0d0a 0000 0000 64fe 9864 5606 0000  a.......d..dV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6700  .....@...sb...g.
 00000030: 6400 a201 5a00 6401 6402 6c01 5400 6401  d...Z.d.d.l.T.d.
 00000040: 6403 6c02 6d03 5a03 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6504 6a05 8303 5a06 6507 6503  ..d.e.j...Z.e.e.
 00000060: 6406 9c02 6407 6408 8404 5a08 6509 6507  d...d.d...Z.e.e.
 00000070: 6406 9c02 6409 640a 8404 5a0a 6509 6503  d...d.d...Z.e.e.
@@ -12,98 +12,101 @@
 000000b0: 6f6e 5f6c 6f61 6473 da0b 4a73 6f6e 456e  on_loads..JsonEn
 000000c0: 636f 6465 72e9 0000 0000 2901 da01 2a29  coder.....)...*)
 000000d0: 01da 084a 736f 6e61 626c 6563 0000 0000  ...Jsonablec....
 000000e0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
 000000f0: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
 00000100: 0264 0164 0284 005a 0364 0353 0029 0472  .d.d...Z.d.S.).r
 00000110: 0400 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000120: 0002 0000 0004 0000 0043 0000 0073 ec00  .........C...s..
+00000120: 0002 0000 0004 0000 0043 0000 0073 0401  .........C...s..
 00000130: 0000 7400 7c01 7401 6a01 8302 721c 7c01  ..t.|.t.j...r.|.
 00000140: a002 a100 6400 6401 8502 1900 5300 7400  ....d.d.....S.t.
 00000150: 7c01 7401 6a03 8302 7230 7c01 a002 a100  |.t.j...r0|.....
 00000160: 5300 7400 7c01 7404 8302 7240 7c01 6a05  S.t.|.t...r@|.j.
 00000170: 5300 7400 7c01 7406 8302 7256 7c01 6a07  S.t.|.t...rV|.j.
 00000180: 6402 6403 8d01 5300 7400 7c01 7408 8302  d.d...S.t.|.t...
 00000190: 7268 7409 7c01 8301 5300 7400 7c01 740a  rht.|...S.t.|.t.
 000001a0: 740b 6602 8302 7284 6404 6405 8400 7c01  t.f...r.d.d...|.
 000001b0: 4400 8301 5300 7400 7c01 740c 8302 7296  D...S.t.|.t...r.
 000001c0: 740d 7c01 8301 5300 7400 7c01 740e 740f  t.|...S.t.|.t.t.
 000001d0: 6602 8302 72ae 7409 7c01 6a10 8301 5300  f...r.t.|.j...S.
 000001e0: 7411 7c01 6406 8302 72c0 7c01 a012 a100  t.|.d...r.|.....
 000001f0: 5300 7413 7c01 8301 72de 7400 7c01 7414  S.t.|...r.t.|.t.
 00000200: 8302 73de 7409 7415 7c01 8301 8301 5300  ..s.t.t.|.....S.
-00000210: 7416 6a17 a018 7c00 7c01 a102 5300 2907  t.j...|.|...S.).
-00000220: 4ee9 1000 0000 7a05 7574 662d 3829 01da  N.....z.utf-8)..
-00000230: 0865 6e63 6f64 696e 6763 0100 0000 0000  .encodingc......
-00000240: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00000250: 0000 7314 0000 0067 007c 005d 0c7d 0174  ..s....g.|.].}.t
-00000260: 007c 0183 0191 0271 0453 00a9 0029 0172  .|.....q.S...).r
-00000270: 0200 0000 2902 da02 2e30 da04 6974 656d  ....)....0..item
-00000280: 720a 0000 0072 0a00 0000 fa7c 2f55 7365  r....r.....|/Use
-00000290: 7273 2f64 616e 6965 6c61 7261 6e74 6573  rs/danielarantes
-000002a0: 2f4c 6962 7261 7279 2f4d 6f62 696c 6520  /Library/Mobile 
-000002b0: 446f 6375 6d65 6e74 732f 636f 6d7e 6170  Documents/com~ap
-000002c0: 706c 657e 436c 6f75 6444 6f63 732f 4d79  ple~CloudDocs/My
-000002d0: 2041 7070 732f 7079 7069 2f64 746d 6f64   Apps/pypi/dtmod
-000002e0: 656c 2f64 746d 6f64 656c 2f64 7466 6965  el/dtmodel/dtfie
-000002f0: 6c64 2f70 6172 7365 2f6a 736f 6e5f 656e  ld/parse/json_en
-00000300: 636f 6465 722e 7079 da0a 3c6c 6973 7463  coder.py..<listc
-00000310: 6f6d 703e 1f00 0000 f300 0000 007a 274a  omp>.........z'J
-00000320: 736f 6e45 6e63 6f64 6572 2e64 6566 6175  sonEncoder.defau
-00000330: 6c74 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  lt.<locals>.<lis
-00000340: 7463 6f6d 703e da06 6173 6a73 6f6e 2919  tcomp>..asjson).
-00000350: da0a 6973 696e 7374 616e 6365 da08 6461  ..isinstance..da
-00000360: 7465 7469 6d65 da09 6973 6f66 6f72 6d61  tetime..isoforma
-00000370: 74da 0464 6174 65da 0445 6e75 6dda 046e  t..date..Enum..n
-00000380: 616d 65da 0562 7974 6573 da06 6465 636f  ame..bytes..deco
-00000390: 6465 da04 6469 6374 7202 0000 00da 046c  de..dictr......l
-000003a0: 6973 74da 0574 7570 6c65 da0a 5573 6572  ist..tuple..User
-000003b0: 5374 7269 6e67 da03 7374 72da 0855 7365  String..str..Use
-000003c0: 7244 6963 74da 0855 7365 724c 6973 74da  rDict..UserList.
-000003d0: 0464 6174 61da 0768 6173 6174 7472 7210  .data..hasattrr.
-000003e0: 0000 00da 0c69 735f 6461 7461 636c 6173  .....is_dataclas
-000003f0: 73da 0474 7970 65da 0661 7364 6963 74da  s..type..asdict.
-00000400: 046a 736f 6eda 0b4a 534f 4e45 6e63 6f64  .json..JSONEncod
-00000410: 6572 da07 6465 6661 756c 7429 02da 0473  er..default)...s
-00000420: 656c 66da 036f 626a 720a 0000 0072 0a00  elf..objr....r..
-00000430: 0000 720d 0000 0072 2700 0000 1300 0000  ..r....r'.......
-00000440: 732a 0000 0000 010c 0110 010c 0108 010a  s*..............
-00000450: 0106 010a 010c 010a 0108 010e 010e 010a  ................
-00000460: 0108 010e 010a 010a 0108 0112 010c 017a  ...............z
-00000470: 134a 736f 6e45 6e63 6f64 6572 2e64 6566  .JsonEncoder.def
-00000480: 6175 6c74 4e29 04da 085f 5f6e 616d 655f  aultN)...__name_
-00000490: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000004a0: 5f71 7561 6c6e 616d 655f 5f72 2700 0000  _qualname__r'...
-000004b0: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-000004c0: 0d00 0000 7204 0000 0012 0000 0073 0200  ....r........s..
-000004d0: 0000 0801 7204 0000 0029 0272 2900 0000  ....r....).r)...
-000004e0: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-000004f0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000500: 0073 0a00 0000 7400 a001 7c00 a101 5300  .s....t...|...S.
-00000510: a901 4e29 0272 2500 0000 da05 6c6f 6164  ..N).r%.....load
-00000520: 73a9 0172 2900 0000 720a 0000 0072 0a00  s..r)...r....r..
-00000530: 0000 720d 0000 0072 0300 0000 2b00 0000  ..r....r....+...
-00000540: 7302 0000 0000 0172 0300 0000 6301 0000  s......r....c...
-00000550: 0000 0000 0000 0000 0001 0000 0006 0000  ................
-00000560: 0043 0000 0073 1200 0000 7400 6a01 7c00  .C...s....t.j.|.
-00000570: 7402 6401 6402 6403 8d04 5300 2904 4ee9  t.d.d.d...S.).N.
-00000580: 0200 0000 4629 03da 0363 6c73 da06 696e  ....F)...cls..in
-00000590: 6465 6e74 da0c 656e 7375 7265 5f61 7363  dent..ensure_asc
-000005a0: 6969 2903 7225 0000 00da 0564 756d 7073  ii).r%.....dumps
-000005b0: 7204 0000 0072 3000 0000 720a 0000 0072  r....r0...r....r
-000005c0: 0a00 0000 720d 0000 0072 0100 0000 2f00  ....r....r..../.
-000005d0: 0000 7302 0000 0000 0172 0100 0000 6301  ..s......r....c.
-000005e0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-000005f0: 0000 0043 0000 0073 0c00 0000 7400 7401  ...C...s....t.t.
-00000600: 7c00 8301 8301 5300 722e 0000 0029 0272  |.....S.r....).r
-00000610: 0300 0000 7201 0000 0072 3000 0000 720a  ....r....r0...r.
-00000620: 0000 0072 0a00 0000 720d 0000 0072 0200  ...r....r....r..
-00000630: 0000 3300 0000 7302 0000 0000 0172 0200  ..3...s......r..
-00000640: 0000 4e29 0cda 075f 5f61 6c6c 5f5f 5a18  ..N)...__all__Z.
-00000650: 6474 6d6f 6465 6c2e 6474 6669 656c 642e  dtmodel.dtfield.
-00000660: 5f69 6d70 6f72 7473 da06 6474 6261 7365  _imports..dtbase
-00000670: 7207 0000 0072 2500 0000 7226 0000 0072  r....r%...r&...r
-00000680: 0400 0000 721d 0000 0072 0300 0000 da03  ....r....r......
-00000690: 416e 7972 0100 0000 7202 0000 0072 0a00  Anyr....r....r..
-000006a0: 0000 720a 0000 0072 0a00 0000 720d 0000  ..r....r....r...
-000006b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000006c0: 0c00 0000 080d 0801 0c03 1219 1004 1004  ................
+00000210: 7400 7c01 7416 8302 9000 72f6 740d 7417  t.|.t.....r.t.t.
+00000220: 7c01 8301 8301 5300 7418 6a19 a01a 7c00  |.....S.t.j...|.
+00000230: 7c01 a102 5300 2907 4ee9 1000 0000 7a05  |...S.).N.....z.
+00000240: 7574 662d 3829 01da 0865 6e63 6f64 696e  utf-8)...encodin
+00000250: 6763 0100 0000 0000 0000 0000 0000 0200  gc..............
+00000260: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00000270: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
+00000280: 0453 00a9 0029 0172 0200 0000 2902 da02  .S...).r....)...
+00000290: 2e30 da04 6974 656d 720a 0000 0072 0a00  .0..itemr....r..
+000002a0: 0000 fa74 2f55 7365 7273 2f64 616e 6965  ...t/Users/danie
+000002b0: 6c61 7261 6e74 6573 2f4c 6962 7261 7279  larantes/Library
+000002c0: 2f4d 6f62 696c 6520 446f 6375 6d65 6e74  /Mobile Document
+000002d0: 732f 636f 6d7e 6170 706c 657e 436c 6f75  s/com~apple~Clou
+000002e0: 6444 6f63 732f 4d79 2041 7070 732f 7079  dDocs/My Apps/py
+000002f0: 7069 2f64 746d 6f64 656c 2f64 746d 6f64  pi/dtmodel/dtmod
+00000300: 656c 2f70 6172 7365 2f6a 736f 6e5f 656e  el/parse/json_en
+00000310: 636f 6465 722e 7079 da0a 3c6c 6973 7463  coder.py..<listc
+00000320: 6f6d 703e 1f00 0000 f300 0000 007a 274a  omp>.........z'J
+00000330: 736f 6e45 6e63 6f64 6572 2e64 6566 6175  sonEncoder.defau
+00000340: 6c74 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  lt.<locals>.<lis
+00000350: 7463 6f6d 703e da06 6173 6a73 6f6e 291b  tcomp>..asjson).
+00000360: da0a 6973 696e 7374 616e 6365 da08 6461  ..isinstance..da
+00000370: 7465 7469 6d65 da09 6973 6f66 6f72 6d61  tetime..isoforma
+00000380: 74da 0464 6174 65da 0445 6e75 6dda 046e  t..date..Enum..n
+00000390: 616d 65da 0562 7974 6573 da06 6465 636f  ame..bytes..deco
+000003a0: 6465 da04 6469 6374 7202 0000 00da 046c  de..dictr......l
+000003b0: 6973 74da 0574 7570 6c65 da0a 5573 6572  ist..tuple..User
+000003c0: 5374 7269 6e67 da03 7374 72da 0855 7365  String..str..Use
+000003d0: 7244 6963 74da 0855 7365 724c 6973 74da  rDict..UserList.
+000003e0: 0464 6174 61da 0768 6173 6174 7472 7210  .data..hasattrr.
+000003f0: 0000 00da 0c69 735f 6461 7461 636c 6173  .....is_dataclas
+00000400: 73da 0474 7970 65da 0661 7364 6963 74da  s..type..asdict.
+00000410: 0744 6563 696d 616c da05 666c 6f61 74da  .Decimal..float.
+00000420: 046a 736f 6eda 0b4a 534f 4e45 6e63 6f64  .json..JSONEncod
+00000430: 6572 da07 6465 6661 756c 7429 02da 0473  er..default)...s
+00000440: 656c 66da 036f 626a 720a 0000 0072 0a00  elf..objr....r..
+00000450: 0000 720d 0000 0072 2900 0000 1300 0000  ..r....r).......
+00000460: 732e 0000 0000 010c 0110 010c 0108 010a  s...............
+00000470: 0106 010a 010c 010a 0108 010e 010e 010a  ................
+00000480: 0108 010e 010a 010a 0108 0112 010c 010c  ................
+00000490: 010c 017a 134a 736f 6e45 6e63 6f64 6572  ...z.JsonEncoder
+000004a0: 2e64 6566 6175 6c74 4e29 04da 085f 5f6e  .defaultN)...__n
+000004b0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+000004c0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+000004d0: 2900 0000 720a 0000 0072 0a00 0000 720a  )...r....r....r.
+000004e0: 0000 0072 0d00 0000 7204 0000 0012 0000  ...r....r.......
+000004f0: 0073 0200 0000 0801 7204 0000 0029 0272  .s......r....).r
+00000500: 2b00 0000 da06 7265 7475 726e 6301 0000  +.....returnc...
+00000510: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000520: 0043 0000 0073 0a00 0000 7400 a001 7c00  .C...s....t...|.
+00000530: a101 5300 a901 4e29 0272 2700 0000 da05  ..S...N).r'.....
+00000540: 6c6f 6164 73a9 0172 2b00 0000 720a 0000  loads..r+...r...
+00000550: 0072 0a00 0000 720d 0000 0072 0300 0000  .r....r....r....
+00000560: 2d00 0000 7302 0000 0000 0172 0300 0000  -...s......r....
+00000570: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000580: 0006 0000 0043 0000 0073 1200 0000 7400  .....C...s....t.
+00000590: 6a01 7c00 7402 6401 6402 6403 8d04 5300  j.|.t.d.d.d...S.
+000005a0: 2904 4ee9 0200 0000 4629 03da 0363 6c73  ).N.....F)...cls
+000005b0: da06 696e 6465 6e74 da0c 656e 7375 7265  ..indent..ensure
+000005c0: 5f61 7363 6969 2903 7227 0000 00da 0564  _ascii).r'.....d
+000005d0: 756d 7073 7204 0000 0072 3200 0000 720a  umpsr....r2...r.
+000005e0: 0000 0072 0a00 0000 720d 0000 0072 0100  ...r....r....r..
+000005f0: 0000 3100 0000 7302 0000 0000 0172 0100  ..1...s......r..
+00000600: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000610: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
+00000620: 7400 7401 7c00 8301 8301 5300 7230 0000  t.t.|.....S.r0..
+00000630: 0029 0272 0300 0000 7201 0000 0072 3200  .).r....r....r2.
+00000640: 0000 720a 0000 0072 0a00 0000 720d 0000  ..r....r....r...
+00000650: 0072 0200 0000 3500 0000 7302 0000 0000  .r....5...s.....
+00000660: 0172 0200 0000 4e29 0cda 075f 5f61 6c6c  .r....N)...__all
+00000670: 5f5f da15 6474 6d6f 6465 6c2e 6261 7365  __..dtmodel.base
+00000680: 2e5f 696d 706f 7274 73da 0664 7462 6173  ._imports..dtbas
+00000690: 6572 0700 0000 7227 0000 0072 2800 0000  er....r'...r(...
+000006a0: 7204 0000 0072 1d00 0000 7203 0000 00da  r....r....r.....
+000006b0: 0341 6e79 7201 0000 0072 0200 0000 720a  .Anyr....r....r.
+000006c0: 0000 0072 0a00 0000 720a 0000 0072 0d00  ...r....r....r..
+000006d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000006e0: 730c 0000 0008 0d08 010c 0312 1b10 0410  s...............
+000006f0: 04                                       .
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/parse/__pycache__/null.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 11 02:36:40 2023 UTC, .py size: 346 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -11,24 +11,23 @@
 000000a0: 0100 0000 0900 0000 4300 0000 733c 0000  ........C...s<..
 000000b0: 0074 007c 0064 0075 007c 0064 016b 027c  .t.|.d.u.|.d.k.|
 000000c0: 0064 026b 027c 0067 006b 027c 0069 006b  .d.k.|.g.k.|.i.k
 000000d0: 027c 0074 0183 006b 027c 0074 026b 0267  .|.t...k.|.t.k.g
 000000e0: 0783 0172 3864 0353 0064 0453 0029 054e  ...r8d.S.d.S.).N
 000000f0: da00 f300 0000 0054 4629 03da 0361 6e79  .......TF)...any
 00000100: da04 6469 6374 7204 0000 0029 0172 0500  ..dictr....).r..
-00000110: 0000 a900 720b 0000 00fa 742f 5573 6572  ....r.....t/User
+00000110: 0000 a900 720b 0000 00fa 6c2f 5573 6572  ....r.....l/User
 00000120: 732f 6461 6e69 656c 6172 616e 7465 732f  s/danielarantes/
 00000130: 4c69 6272 6172 792f 4d6f 6269 6c65 2044  Library/Mobile D
 00000140: 6f63 756d 656e 7473 2f63 6f6d 7e61 7070  ocuments/com~app
 00000150: 6c65 7e43 6c6f 7564 446f 6373 2f4d 7920  le~CloudDocs/My 
 00000160: 4170 7073 2f70 7970 692f 6474 6d6f 6465  Apps/pypi/dtmode
-00000170: 6c2f 6474 6d6f 6465 6c2f 6474 6669 656c  l/dtmodel/dtfiel
-00000180: 642f 7061 7273 652f 6e75 6c6c 2e70 7972  d/parse/null.pyr
-00000190: 0100 0000 0700 0000 7316 0000 0000 0102  ........s.......
-000001a0: 0106 0106 0106 0106 0106 0108 0106 f90a  ................
-000001b0: 0802 f84e 2907 da07 5f5f 616c 6c5f 5fda  ...N)...__all__.
-000001c0: 0674 7970 696e 6772 0300 0000 da0b 6461  .typingr......da
-000001d0: 7461 636c 6173 7365 7372 0400 0000 da04  taclassesr......
-000001e0: 626f 6f6c 7201 0000 0072 0b00 0000 720b  boolr....r....r.
-000001f0: 0000 0072 0b00 0000 720c 0000 00da 083c  ...r....r......<
-00000200: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
-00000210: 0602 0c01 0c03                           ......
+00000170: 6c2f 6474 6d6f 6465 6c2f 7061 7273 652f  l/dtmodel/parse/
+00000180: 6e75 6c6c 2e70 7972 0100 0000 0700 0000  null.pyr........
+00000190: 7316 0000 0000 0102 0106 0106 0106 0106  s...............
+000001a0: 0106 0108 0106 f90a 0802 f84e 2907 da07  ...........N)...
+000001b0: 5f5f 616c 6c5f 5fda 0674 7970 696e 6772  __all__..typingr
+000001c0: 0300 0000 da0b 6461 7461 636c 6173 7365  ......dataclasse
+000001d0: 7372 0400 0000 da04 626f 6f6c 7201 0000  sr......boolr...
+000001e0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
+000001f0: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000200: 0000 0073 0600 0000 0602 0c01 0c03       ...s..........
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/parse/__pycache__/number.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 11 02:29:46 2023 UTC, .py size: 1260 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -23,59 +23,58 @@
 00000160: 7402 7c00 8301 5300 7c00 5300 2904 4efa  t.|...S.|.S.).N.
 00000170: 012c da01 2e72 0400 0000 290b da0a 6973  .,...r....)...is
 00000180: 696e 7374 616e 6365 da03 7374 72da 0369  instance..str..i
 00000190: 6e74 da05 666c 6f61 74da 0272 65da 0373  nt..float..re..s
 000001a0: 7562 da09 5f5f 726f 756e 645f 5fda 0864  ub..__round__..d
 000001b0: 6174 6574 696d 65da 0464 6174 65da 0974  atetime..date..t
 000001c0: 6f6f 7264 696e 616c da04 626f 6f6c a901  oordinal..bool..
-000001d0: 7207 0000 00a9 0072 1700 0000 fa76 2f55  r......r.....v/U
+000001d0: 7207 0000 00a9 0072 1700 0000 fa6e 2f55  r......r.....n/U
 000001e0: 7365 7273 2f64 616e 6965 6c61 7261 6e74  sers/danielarant
 000001f0: 6573 2f4c 6962 7261 7279 2f4d 6f62 696c  es/Library/Mobil
 00000200: 6520 446f 6375 6d65 6e74 732f 636f 6d7e  e Documents/com~
 00000210: 6170 706c 657e 436c 6f75 6444 6f63 732f  apple~CloudDocs/
 00000220: 4d79 2041 7070 732f 7079 7069 2f64 746d  My Apps/pypi/dtm
-00000230: 6f64 656c 2f64 746d 6f64 656c 2f64 7466  odel/dtmodel/dtf
-00000240: 6965 6c64 2f70 6172 7365 2f6e 756d 6265  ield/parse/numbe
-00000250: 722e 7079 7201 0000 0009 0000 0073 1200  r.pyr........s..
-00000260: 0000 0001 0a01 1c01 0a01 0801 1201 0801  ................
-00000270: 0a01 0801 7201 0000 0063 0100 0000 0000  ....r....c......
-00000280: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
-00000290: 0000 7368 0000 0074 007c 0074 0183 0272  ..sh...t.|.t...r
-000002a0: 2274 0274 03a0 0464 0164 027c 00a1 0383  "t.t...d.d.|....
-000002b0: 01a0 0564 03a1 0153 0074 007c 0074 0683  ...d...S.t.|.t..
-000002c0: 0272 3474 027c 0083 0153 0074 007c 0074  .r4t.|...S.t.|.t
-000002d0: 076a 0774 076a 0866 0283 0272 5274 027c  .j.t.j.f...rRt.|
-000002e0: 00a0 09a1 0083 0153 0074 007c 0074 0a83  .......S.t.|.t..
-000002f0: 0272 6474 027c 0083 0153 007c 0053 0029  .rdt.|...S.|.S.)
-00000300: 044e 7209 0000 0072 0a00 0000 e902 0000  .Nr....r........
-00000310: 0029 0b72 0b00 0000 720c 0000 0072 0e00  .).r....r....r..
-00000320: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000330: 0072 0d00 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000340: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000350: 1700 0000 7217 0000 0072 1800 0000 7202  ....r....r....r.
-00000360: 0000 0015 0000 0073 1200 0000 0001 0a01  .......s........
-00000370: 1801 0a01 0801 1201 0c01 0a01 0801 7202  ..............r.
-00000380: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000390: 0100 0000 0600 0000 4300 0000 736a 0000  ........C...sj..
-000003a0: 0074 007c 0074 0183 0272 1c74 0274 03a0  .t.|.t...r.t.t..
-000003b0: 0464 0164 027c 00a1 0383 0153 0074 007c  .d.d.|.....S.t.|
-000003c0: 0074 0583 0272 3674 0274 0174 067c 0083  .t...r6t.t.t.|..
-000003d0: 0183 0183 0153 0074 007c 0074 076a 0774  .....S.t.|.t.j.t
-000003e0: 076a 0866 0283 0272 5474 027c 00a0 09a1  .j.f...rTt.|....
-000003f0: 0083 0153 0074 007c 0074 0a83 0272 6674  ...S.t.|.t...rft
-00000400: 027c 0083 0153 007c 0053 0029 034e 7209  .|...S.|.S.).Nr.
-00000410: 0000 0072 0a00 0000 290b 720b 0000 0072  ...r....).r....r
-00000420: 0c00 0000 7206 0000 0072 0f00 0000 7210  ....r....r....r.
-00000430: 0000 0072 0d00 0000 720e 0000 0072 1200  ...r....r....r..
-00000440: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000450: 0072 1600 0000 7217 0000 0072 1700 0000  .r....r....r....
-00000460: 7218 0000 0072 0300 0000 2000 0000 7312  r....r.... ...s.
-00000470: 0000 0000 010a 0112 010a 0110 0112 010c  ................
-00000480: 010a 0108 0172 0300 0000 290c da07 5f5f  .....r....)...__
-00000490: 616c 6c5f 5f72 0f00 0000 da06 7479 7069  all__r......typi
-000004a0: 6e67 7205 0000 00da 0764 6563 696d 616c  ngr......decimal
-000004b0: 7206 0000 0072 1200 0000 720d 0000 0072  r....r....r....r
-000004c0: 0100 0000 720e 0000 0072 0200 0000 7203  ....r....r....r.
-000004d0: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-000004e0: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000004f0: 3e01 0000 0073 0e00 0000 0802 0801 0c01  >....s..........
-00000500: 0c01 0803 100c 100b                      ........
+00000230: 6f64 656c 2f64 746d 6f64 656c 2f70 6172  odel/dtmodel/par
+00000240: 7365 2f6e 756d 6265 722e 7079 7201 0000  se/number.pyr...
+00000250: 0009 0000 0073 1200 0000 0001 0a01 1c01  .....s..........
+00000260: 0a01 0801 1201 0801 0a01 0801 7201 0000  ............r...
+00000270: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000280: 0000 0600 0000 4300 0000 7368 0000 0074  ......C...sh...t
+00000290: 007c 0074 0183 0272 2274 0274 03a0 0464  .|.t...r"t.t...d
+000002a0: 0164 027c 00a1 0383 01a0 0564 03a1 0153  .d.|.......d...S
+000002b0: 0074 007c 0074 0683 0272 3474 027c 0083  .t.|.t...r4t.|..
+000002c0: 0153 0074 007c 0074 076a 0774 076a 0866  .S.t.|.t.j.t.j.f
+000002d0: 0283 0272 5274 027c 00a0 09a1 0083 0153  ...rRt.|.......S
+000002e0: 0074 007c 0074 0a83 0272 6474 027c 0083  .t.|.t...rdt.|..
+000002f0: 0153 007c 0053 0029 044e 7209 0000 0072  .S.|.S.).Nr....r
+00000300: 0a00 0000 e902 0000 0029 0b72 0b00 0000  .........).r....
+00000310: 720c 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00000320: 1000 0000 7211 0000 0072 0d00 0000 7212  ....r....r....r.
+00000330: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+00000340: 0000 7216 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00000350: 0072 1800 0000 7202 0000 0015 0000 0073  .r....r........s
+00000360: 1200 0000 0001 0a01 1801 0a01 0801 1201  ................
+00000370: 0c01 0a01 0801 7202 0000 0063 0100 0000  ......r....c....
+00000380: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00000390: 4300 0000 736a 0000 0074 007c 0074 0183  C...sj...t.|.t..
+000003a0: 0272 1c74 0274 03a0 0464 0164 027c 00a1  .r.t.t...d.d.|..
+000003b0: 0383 0153 0074 007c 0074 0583 0272 3674  ...S.t.|.t...r6t
+000003c0: 0274 0174 067c 0083 0183 0183 0153 0074  .t.t.|.......S.t
+000003d0: 007c 0074 076a 0774 076a 0866 0283 0272  .|.t.j.t.j.f...r
+000003e0: 5474 027c 00a0 09a1 0083 0153 0074 007c  Tt.|.......S.t.|
+000003f0: 0074 0a83 0272 6674 027c 0083 0153 007c  .t...rft.|...S.|
+00000400: 0053 0029 034e 7209 0000 0072 0a00 0000  .S.).Nr....r....
+00000410: 290b 720b 0000 0072 0c00 0000 7206 0000  ).r....r....r...
+00000420: 0072 0f00 0000 7210 0000 0072 0d00 0000  .r....r....r....
+00000430: 720e 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000440: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
+00000450: 0000 0072 1700 0000 7218 0000 0072 0300  ...r....r....r..
+00000460: 0000 2000 0000 7312 0000 0000 010a 0112  .. ...s.........
+00000470: 010a 0110 0112 010c 010a 0108 0172 0300  .............r..
+00000480: 0000 290c da07 5f5f 616c 6c5f 5f72 0f00  ..)...__all__r..
+00000490: 0000 da06 7479 7069 6e67 7205 0000 00da  ....typingr.....
+000004a0: 0764 6563 696d 616c 7206 0000 0072 1200  .decimalr....r..
+000004b0: 0000 720d 0000 0072 0100 0000 720e 0000  ..r....r....r...
+000004c0: 0072 0200 0000 7203 0000 0072 1700 0000  .r....r....r....
+000004d0: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+000004e0: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
+000004f0: 0000 0802 0801 0c01 0c01 0803 100c 100b  ................
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/parse/__pycache__/string.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 11 02:34:21 2023 UTC, .py size: 627 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -17,35 +17,35 @@
 00000100: 5300 7408 7c00 8301 5300 a903 4e7a 0575  S.t.|...S...Nz.u
 00000110: 7466 2d38 da03 6b65 7929 09da 0a69 7369  tf-8..key)...isi
 00000120: 6e73 7461 6e63 65da 0864 6174 6574 696d  nstance..datetim
 00000130: 65da 0464 6174 65da 0969 736f 666f 726d  e..date..isoform
 00000140: 6174 da05 6279 7465 73da 0664 6563 6f64  at..bytes..decod
 00000150: 65da 0768 6173 6174 7472 7208 0000 00da  e..hasattrr.....
 00000160: 0373 7472 a901 7205 0000 00a9 0072 1200  .str..r......r..
-00000170: 0000 fa76 2f55 7365 7273 2f64 616e 6965  ...v/Users/danie
+00000170: 0000 fa6e 2f55 7365 7273 2f64 616e 6965  ...n/Users/danie
 00000180: 6c61 7261 6e74 6573 2f4c 6962 7261 7279  larantes/Library
 00000190: 2f4d 6f62 696c 6520 446f 6375 6d65 6e74  /Mobile Document
 000001a0: 732f 636f 6d7e 6170 706c 657e 436c 6f75  s/com~apple~Clou
 000001b0: 6444 6f63 732f 4d79 2041 7070 732f 7079  dDocs/My Apps/py
 000001c0: 7069 2f64 746d 6f64 656c 2f64 746d 6f64  pi/dtmodel/dtmod
-000001d0: 656c 2f64 7466 6965 6c64 2f70 6172 7365  el/dtfield/parse
-000001e0: 2f73 7472 696e 672e 7079 7201 0000 0007  /string.pyr.....
-000001f0: 0000 0073 0e00 0000 0001 1201 0801 0a01  ...s............
-00000200: 0a01 0a01 0601 6301 0000 0000 0000 0000  ......c.........
-00000210: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00000220: 4800 0000 7400 7c00 7401 6a01 7401 6a02  H...t.|.t.j.t.j.
-00000230: 6602 8302 7220 7c00 a003 a100 a004 6401  f...r |.......d.
-00000240: a101 5300 7405 7c00 6402 8302 723a 7406  ..S.t.|.d...r:t.
-00000250: 7c00 6a07 8301 a004 6401 a101 5300 7406  |.j.....d...S.t.
-00000260: 7c00 8301 a004 6401 a101 5300 7207 0000  |.....d...S.r...
-00000270: 0029 0872 0900 0000 720a 0000 0072 0b00  .).r....r....r..
-00000280: 0000 720c 0000 00da 0665 6e63 6f64 6572  ..r......encoder
-00000290: 0f00 0000 7210 0000 0072 0800 0000 7211  ....r....r....r.
-000002a0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-000002b0: 0000 7202 0000 0011 0000 0073 0a00 0000  ..r........s....
-000002c0: 0001 1201 0e01 0a01 1001 2908 da07 5f5f  ..........)...__
-000002d0: 616c 6c5f 5fda 0674 7970 696e 6772 0400  all__..typingr..
-000002e0: 0000 720a 0000 0072 1000 0000 7201 0000  ..r....r....r...
-000002f0: 0072 0d00 0000 7202 0000 0072 1200 0000  .r....r....r....
-00000300: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000310: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-00000320: 0000 0802 0c01 0803 100a                 ..........
+000001d0: 656c 2f70 6172 7365 2f73 7472 696e 672e  el/parse/string.
+000001e0: 7079 7201 0000 0007 0000 0073 0e00 0000  pyr........s....
+000001f0: 0001 1201 0801 0a01 0a01 0a01 0601 6301  ..............c.
+00000200: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000210: 0000 0043 0000 0073 4800 0000 7400 7c00  ...C...sH...t.|.
+00000220: 7401 6a01 7401 6a02 6602 8302 7220 7c00  t.j.t.j.f...r |.
+00000230: a003 a100 a004 6401 a101 5300 7405 7c00  ......d...S.t.|.
+00000240: 6402 8302 723a 7406 7c00 6a07 8301 a004  d...r:t.|.j.....
+00000250: 6401 a101 5300 7406 7c00 8301 a004 6401  d...S.t.|.....d.
+00000260: a101 5300 7207 0000 0029 0872 0900 0000  ..S.r....).r....
+00000270: 720a 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000280: 0665 6e63 6f64 6572 0f00 0000 7210 0000  .encoder....r...
+00000290: 0072 0800 0000 7211 0000 0072 1200 0000  .r....r....r....
+000002a0: 7212 0000 0072 1300 0000 7202 0000 0011  r....r....r.....
+000002b0: 0000 0073 0a00 0000 0001 1201 0e01 0a01  ...s............
+000002c0: 1001 2908 da07 5f5f 616c 6c5f 5fda 0674  ..)...__all__..t
+000002d0: 7970 696e 6772 0400 0000 720a 0000 0072  ypingr....r....r
+000002e0: 1000 0000 7201 0000 0072 0d00 0000 7202  ....r....r....r.
+000002f0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+00000300: 0000 7213 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000310: 3e01 0000 0073 0800 0000 0802 0c01 0803  >....s..........
+00000320: 100a                                     ..
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 18 01:53:16 2023 UTC, .py size: 10847 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,729 +1,708 @@
-00000000: 610d 0d0a 0000 0000 8c63 8e64 5f2a 0000  a........c.d_*..
+00000000: 610d 0d0a 0000 0000 8fd7 8f64 832a 0000  a..........d.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 7601 0000 6700  .....@...sv...g.
-00000030: 6400 a201 5a00 6401 6402 6c01 5400 6403  d...Z.d.d.l.T.d.
-00000040: 6402 6c02 5400 6404 6402 6c03 5400 6504  d.l.T.d.d.l.T.e.
-00000050: 6505 6506 6507 6508 6405 6605 1900 5a09  e.e.e.e.d.f...Z.
-00000060: 6504 650a 650b 6505 6506 6507 6508 6606  e.e.e.e.e.e.e.f.
-00000070: 1900 5a0c 6504 6505 6405 6602 1900 5a0d  ..Z.e.e.d.f...Z.
-00000080: 6504 6505 6405 6602 1900 5a0e 6504 650f  e.e.d.f...Z.e.e.
-00000090: 6a0f 6507 6506 6405 6604 1900 5a10 650b  j.e.e.d.f...Z.e.
-000000a0: 6509 1900 5a11 650a 6505 6504 6511 6509  e...Z.e.e.e.e.e.
-000000b0: 6602 1900 6602 1900 5a12 6504 6512 6511  f...f...Z.e.e.e.
-000000c0: 6509 6603 1900 5a13 6504 650a 6505 6509  e.f...Z.e.e.e.e.
-000000d0: 6602 1900 650b 650a 6505 6509 6602 1900  f...e.e.e.e.f...
-000000e0: 1900 6602 1900 5a14 6504 650b 6505 1900  ..f...Z.e.e.e...
-000000f0: 6505 6602 1900 5a15 6505 5a16 6517 6518  e.f...Z.e.Z.e.e.
-00000100: 1900 5a19 6504 6518 6519 6602 1900 5a1a  ..Z.e.e.e.f...Z.
-00000110: 6517 650b 651b 651c 651d 6605 5a1e 650a  e.e.e.e.e.f.Z.e.
-00000120: 651f 6520 6603 5a21 6522 6406 8301 5a23  e.e f.Z!e"d...Z#
-00000130: 6522 6407 8301 5a24 6504 6523 6524 6602  e"d...Z$e.e#e$f.
-00000140: 1900 5a25 6522 6408 8301 5a26 6522 6409  ..Z%e"d...Z&e"d.
-00000150: 6506 6507 6527 8304 5a28 4700 640a 640b  e.e.e'..Z(G.d.d.
-00000160: 8400 640b 6529 8303 5a2a 4700 640c 640d  ..d.e)..Z*G.d.d.
-00000170: 8400 640d 6529 8303 5a2b 4700 640e 640f  ..d.e)..Z+G.d.d.
-00000180: 8400 640f 652c 8303 5a2d 4700 6410 6411  ..d.e,..Z-G.d.d.
-00000190: 8400 6411 8302 5a2e 6412 6413 8400 5a2f  ..d...Z.d.d...Z/
-000001a0: 6405 5300 2914 2903 da08 5479 7065 4869  d.S.).)...TypeHi
-000001b0: 6e74 da06 7061 7273 6572 da06 5061 7273  nt..parser..Pars
-000001c0: 6572 e902 0000 0029 01da 012a e901 0000  er.....)...*....
-000001d0: 00e9 0000 0000 4eda 0b50 6172 7365 7245  ......N..ParserE
-000001e0: 6e74 7279 da0c 5061 7273 6572 5265 7375  ntry..ParserResu
-000001f0: 6c74 da0b 4765 6e65 7269 6354 7970 65da  lt..GenericType.
-00000200: 064e 756d 6265 7263 0000 0000 0000 0000  .Numberc........
-00000210: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000220: 7324 0000 0065 005a 0164 005a 0265 0365  s$...e.Z.d.Z.e.e
-00000230: 0465 0365 0566 0219 0064 019c 0264 0264  .e.e.f...d...d.d
-00000240: 0384 045a 0664 0453 0029 05da 0e50 6172  ...Z.d.S.)...Par
-00000250: 7365 7250 726f 746f 636f 6ca9 02da 0576  serProtocol....v
-00000260: 616c 7565 da06 7265 7475 726e 6302 0000  alue..returnc...
-00000270: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-00000280: 0043 0000 0073 0400 0000 6400 5300 a901  .C...s....d.S...
-00000290: 4ea9 00a9 02da 0473 656c 6672 0e00 0000  N......selfr....
-000002a0: 7211 0000 0072 1100 0000 fa79 2f55 7365  r....r.....y/Use
-000002b0: 7273 2f64 616e 6965 6c61 7261 6e74 6573  rs/danielarantes
-000002c0: 2f4c 6962 7261 7279 2f4d 6f62 696c 6520  /Library/Mobile 
-000002d0: 446f 6375 6d65 6e74 732f 636f 6d7e 6170  Documents/com~ap
-000002e0: 706c 657e 436c 6f75 6444 6f63 732f 4d79  ple~CloudDocs/My
-000002f0: 2041 7070 732f 7079 7069 2f64 746d 6f64   Apps/pypi/dtmod
-00000300: 656c 2f64 746d 6f64 656c 2f64 7466 6965  el/dtmodel/dtfie
-00000310: 6c64 2f70 6172 7365 2f74 7970 655f 6869  ld/parse/type_hi
-00000320: 6e74 2e70 79da 085f 5f63 616c 6c5f 5f24  nt.py..__call__$
-00000330: 0000 0073 0200 0000 0001 7a17 5061 7273  ...s......z.Pars
-00000340: 6572 5072 6f74 6f63 6f6c 2e5f 5f63 616c  erProtocol.__cal
-00000350: 6c5f 5f4e 2907 da08 5f5f 6e61 6d65 5f5f  l__N)...__name__
-00000360: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000370: 7175 616c 6e61 6d65 5f5f 7208 0000 00da  qualname__r.....
-00000380: 0555 6e69 6f6e 7209 0000 0072 1500 0000  .Unionr....r....
-00000390: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-000003a0: 1400 0000 720c 0000 0023 0000 0073 0200  ....r....#...s..
-000003b0: 0000 0801 720c 0000 0063 0000 0000 0000  ....r....c......
-000003c0: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-000003d0: 0000 731e 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
-000003e0: 0365 0465 0364 019c 0364 0264 0384 045a  .e.e.d...d.d...Z
-000003f0: 0564 0453 0029 05da 1156 616c 6964 6174  .d.S.)...Validat
-00000400: 6f72 5072 6f74 6f63 6f6c 2903 720e 0000  orProtocol).r...
-00000410: 00da 0574 7970 6573 720f 0000 0063 0300  ...typesr....c..
-00000420: 0000 0000 0000 0000 0000 0300 0000 0100  ................
-00000430: 0000 4300 0000 7304 0000 0064 0053 0072  ..C...s....d.S.r
-00000440: 1000 0000 7211 0000 0029 0372 1300 0000  ....r....).r....
-00000450: 720e 0000 0072 1b00 0000 7211 0000 0072  r....r....r....r
-00000460: 1100 0000 7214 0000 0072 1500 0000 2900  ....r....r....).
-00000470: 0000 7302 0000 0000 017a 1a56 616c 6964  ..s......z.Valid
-00000480: 6174 6f72 5072 6f74 6f63 6f6c 2e5f 5f63  atorProtocol.__c
-00000490: 616c 6c5f 5f4e 2906 7216 0000 0072 1700  all__N).r....r..
-000004a0: 0000 7218 0000 0072 0a00 0000 da05 5479  ..r....r......Ty
-000004b0: 7065 7372 1500 0000 7211 0000 0072 1100  pesr....r....r..
-000004c0: 0000 7211 0000 0072 1400 0000 721a 0000  ..r....r....r...
-000004d0: 0028 0000 0073 0200 0000 0801 721a 0000  .(...s......r...
-000004e0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000004f0: 0000 0600 0000 4000 0000 73aa 0100 0065  ......@...s....e
-00000500: 005a 0164 005a 0265 0365 0465 0565 0619  .Z.d.Z.e.e.e.e..
-00000510: 0064 019c 0264 0264 0384 0483 015a 0765  .d...d.d.....Z.e
-00000520: 0365 0465 0565 0619 0065 0864 049c 0364  .e.e.e...e.d...d
-00000530: 0564 0684 0483 015a 0965 0365 0565 0619  .d.....Z.e.e.e..
-00000540: 0065 0a64 079c 0264 0864 0984 0483 015a  .e.d...d.d.....Z
-00000550: 0b65 0365 0465 0565 0c65 0519 0065 0864  .e.e.e.e.e...e.d
-00000560: 0a9c 0464 0b64 0c84 0483 015a 0d65 0365  ...d.d.....Z.e.e
-00000570: 0465 0e65 0f65 1066 0219 0065 0c65 0519  .e.e.e.f...e.e..
-00000580: 0065 0864 0a9c 0464 0d64 0e84 0483 015a  .e.d...d.d.....Z
-00000590: 1165 0365 0465 0665 0864 0f9c 0364 1064  .e.e.e.e.d...d.d
-000005a0: 1184 0483 015a 1265 0365 0465 0864 129c  .....Z.e.e.e.d..
-000005b0: 0264 1364 1484 0483 015a 1365 0365 0465  .d.d.....Z.e.e.e
-000005c0: 0864 129c 0264 1564 1684 0483 015a 1465  .d...d.d.....Z.e
-000005d0: 0365 0465 0864 129c 0264 1764 1884 0483  .e.e.d...d.d....
-000005e0: 015a 1565 0365 0465 0864 129c 0264 1964  .Z.e.e.e.d...d.d
-000005f0: 1a84 0483 015a 1665 0364 1b64 1c84 0083  .....Z.e.d.d....
-00000600: 015a 1765 0365 0f65 0564 1d19 0064 1e9c  .Z.e.e.e.d...d..
-00000610: 0264 1f64 2084 0483 015a 1865 0364 2164  .d.d ....Z.e.d!d
-00000620: 2284 0083 015a 1965 0365 0465 0864 129c  "....Z.e.e.e.d..
-00000630: 0264 2364 2484 0483 015a 1a65 0365 0465  .d#d$....Z.e.e.e
-00000640: 0565 1b19 0065 0864 259c 0364 2664 2784  .e...e.d%..d&d'.
-00000650: 0483 015a 1c65 0365 0465 0864 129c 0264  ...Z.e.e.e.d...d
-00000660: 2864 2984 0483 015a 1d65 0365 0465 0864  (d)....Z.e.e.e.d
-00000670: 129c 0264 2a64 2b84 0483 015a 1e65 0365  ...d*d+....Z.e.e
-00000680: 0465 0864 129c 0264 2c64 2d84 0483 015a  .e.d...d,d-....Z
-00000690: 1f65 0365 0465 0864 129c 0264 2e64 2f84  .e.e.e.d...d.d/.
-000006a0: 0483 015a 2064 3053 0029 3172 0300 0000  ...Z d0S.)1r....
-000006b0: 2902 720e 0000 00da 0963 6173 745f 7479  ).r......cast_ty
-000006c0: 7065 6303 0000 0000 0000 0000 0000 0003  pec.............
-000006d0: 0000 0004 0000 0043 0000 0073 0c00 0000  .......C...s....
-000006e0: 7c00 a000 7c01 7c02 a102 5300 7210 0000  |...|.|...S.r...
-000006f0: 0029 01da 0770 726f 6365 7373 2903 da03  .)...process)...
-00000700: 636c 7372 0e00 0000 721d 0000 0072 1100  clsr....r....r..
-00000710: 0000 7211 0000 0072 1400 0000 da03 6765  ..r....r......ge
-00000720: 742e 0000 0073 0200 0000 0002 7a0a 5061  t....s......z.Pa
-00000730: 7273 6572 2e67 6574 2903 720e 0000 0072  rser.get).r....r
-00000740: 1d00 0000 720f 0000 0063 0300 0000 0000  ....r....c......
-00000750: 0000 0000 0000 0500 0000 0a00 0000 4300  ..............C.
-00000760: 0000 73c6 0000 0074 007c 0283 017d 037c  ..s....t.|...}.|
-00000770: 03a0 017c 01a1 0172 167c 0153 007a 7a7c  ...|...r.|.S.zz|
-00000780: 036a 0272 4c74 037c 017c 0283 0272 2e7c  .j.rLt.|.|...r.|
-00000790: 0157 0053 0074 047c 0183 0172 3c57 0064  .W.S.t.|...r<W.d
-000007a0: 0153 007c 00a0 057c 02a1 017c 0183 0157  .S.|...|...|...W
-000007b0: 0053 007c 036a 0672 667c 00a0 077c 017c  .S.|.j.rf|...|.|
-000007c0: 036a 087c 036a 09a1 0357 0053 007c 036a  .j.|.j...W.S.|.j
-000007d0: 0a72 807c 00a0 0b7c 017c 036a 087c 036a  .r.|...|.|.j.|.j
-000007e0: 09a1 0357 0053 007c 00a0 0c7c 017c 02a1  ...W.S.|...|.|..
-000007f0: 0257 0053 0057 006e 3004 0074 0d79 c001  .W.S.W.n0..t.y..
-00000800: 007d 0401 007a 1874 0e7c 0483 0101 007c  .}...z.t.|.....|
-00000810: 0157 0006 0059 0064 007d 047e 0453 0064  .W...Y.d.}.~.S.d
-00000820: 007d 047e 0430 0030 0064 0053 0029 024e  .}.~.0.0.d.S.).N
-00000830: da00 290f 7201 0000 00da 0a63 6865 636b  ..).r......check
-00000840: 5f74 7970 65da 0e69 735f 7369 6d70 6c65  _type..is_simple
-00000850: 5f74 7970 65da 0a69 7369 6e73 7461 6e63  _type..isinstanc
-00000860: 65da 0769 735f 6e75 6c6c da0d 7369 6d70  e..is_null..simp
-00000870: 6c65 5f65 6e67 696e 65da 0b69 735f 7365  le_engine..is_se
-00000880: 7175 656e 6365 da0f 7365 7175 656e 6365  quence..sequence
-00000890: 5f65 6e67 696e 65da 066f 7269 6769 6eda  _engine..origin.
-000008a0: 0461 7267 73da 0a69 735f 6d61 7070 696e  .args..is_mappin
-000008b0: 67da 0e6d 6170 7069 6e67 5f65 6e67 696e  g..mapping_engin
-000008c0: 65da 0e67 656e 6572 6963 5f65 6e67 696e  e..generic_engin
-000008d0: 65da 0a56 616c 7565 4572 726f 72da 0570  e..ValueError..p
-000008e0: 7269 6e74 2905 721f 0000 0072 0e00 0000  rint).r....r....
-000008f0: 721d 0000 005a 0d63 6173 745f 616e 616c  r....Z.cast_anal
-00000900: 7973 6973 da01 6572 1100 0000 7211 0000  ysis..er....r...
-00000910: 0072 1400 0000 721e 0000 0032 0000 0073  .r....r....2...s
-00000920: 2400 0000 0002 0801 0a01 0401 0201 0601  $...............
-00000930: 0a01 0601 0801 0601 1001 0601 1401 0601  ................
-00000940: 1402 1201 0e01 0801 7a0e 5061 7273 6572  ........z.Parser
-00000950: 2e70 726f 6365 7373 2902 721d 0000 0072  .process).r....r
-00000960: 0f00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000970: 0002 0000 0004 0000 0003 0000 0073 c400  .............s..
-00000980: 0000 8800 7400 7500 720e 8801 6a01 5300  ....t.u.r...j.S.
-00000990: 8800 7402 7500 721c 8801 6a03 5300 8800  ..t.u.r...j.S...
-000009a0: 7404 7500 722a 8801 6a05 5300 8800 7406  t.u.r*..j.S...t.
-000009b0: 6a07 7500 723a 8801 6a08 5300 8800 7406  j.u.r:..j.S...t.
-000009c0: 6a06 7500 724a 8801 6a09 5300 8800 740a  j.u.rJ..j.S...t.
-000009d0: 7500 7258 8801 6a0b 5300 8800 740c 7500  u.rX..j.S...t.u.
-000009e0: 7266 8801 6a0d 5300 8800 740e 7500 7274  rf..j.S...t.u.rt
-000009f0: 8801 6a0f 5300 8800 7410 7500 7282 8801  ..j.S...t.u.r...
-00000a00: 6a11 5300 8800 7412 7500 7290 8801 6a13  j.S...t.u.r...j.
-00000a10: 5300 7414 8800 6401 8302 72a0 8801 6a01  S.t...d...r...j.
-00000a20: 5300 7415 8800 7416 7417 6602 8302 72bc  S.t...t.t.f...r.
-00000a30: 8700 8701 6602 6402 6403 8408 5300 8800  ....f.d.d...S...
-00000a40: 5300 6400 5300 2904 4e5a 0643 5458 5641  S.d.S.).NZ.CTXVA
-00000a50: 5263 0100 0000 0000 0000 0000 0000 0100  Rc..............
-00000a60: 0000 0400 0000 1300 0000 730c 0000 0088  ..........s.....
-00000a70: 01a0 007c 0088 00a1 0253 0072 1000 0000  ...|.....S.r....
-00000a80: 2901 da0b 656e 756d 5f65 6e67 696e 6529  )...enum_engine)
-00000a90: 0172 0e00 0000 a902 721d 0000 0072 1f00  .r......r....r..
-00000aa0: 0000 7211 0000 0072 1400 0000 da08 3c6c  ..r....r......<l
-00000ab0: 616d 6264 613e 6100 0000 f300 0000 007a  ambda>a........z
-00000ac0: 2650 6172 7365 722e 7369 6d70 6c65 5f65  &Parser.simple_e
-00000ad0: 6e67 696e 652e 3c6c 6f63 616c 733e 2e3c  ngine.<locals>.<
-00000ae0: 6c61 6d62 6461 3e29 18da 0373 7472 da0a  lambda>)...str..
-00000af0: 7374 725f 656e 6769 6e65 da03 696e 74da  str_engine..int.
-00000b00: 0a69 6e74 5f65 6e67 696e 65da 0566 6c6f  .int_engine..flo
-00000b10: 6174 da0c 666c 6f61 745f 656e 6769 6e65  at..float_engine
-00000b20: da08 6461 7465 7469 6d65 da04 6461 7465  ..datetime..date
-00000b30: da0b 6461 7465 5f65 6e67 696e 65da 0f64  ..date_engine..d
-00000b40: 6174 6574 696d 655f 656e 6769 6e65 da05  atetime_engine..
-00000b50: 6279 7465 73da 0c62 7974 6573 5f65 6e67  bytes..bytes_eng
-00000b60: 696e 65da 0744 6563 696d 616c da0e 6465  ine..Decimal..de
-00000b70: 6369 6d61 6c5f 656e 6769 6e65 da04 6c69  cimal_engine..li
-00000b80: 7374 da0b 6c69 7374 5f65 6e67 696e 65da  st..list_engine.
-00000b90: 0373 6574 da0a 7365 745f 656e 6769 6e65  .set..set_engine
-00000ba0: da05 7475 706c 65da 0c74 7570 6c65 5f65  ..tuple..tuple_e
-00000bb0: 6e67 696e 65da 0768 6173 6174 7472 da0a  ngine..hasattr..
-00000bc0: 6973 7375 6263 6c61 7373 da08 4261 7365  issubclass..Base
-00000bd0: 456e 756d da04 456e 756d 2902 721f 0000  Enum..Enum).r...
-00000be0: 0072 1d00 0000 7211 0000 0072 3200 0000  .r....r....r2...
-00000bf0: 7214 0000 0072 2600 0000 4800 0000 7332  r....r&...H...s2
-00000c00: 0000 0000 0208 0106 0108 0106 0108 0106  ................
-00000c10: 010a 0106 010a 0106 0108 0106 0108 0106  ................
-00000c20: 0108 0106 0108 0106 0108 0106 010a 0106  ................
-00000c30: 010e 010e 027a 1450 6172 7365 722e 7369  .....z.Parser.si
-00000c40: 6d70 6c65 5f65 6e67 696e 6529 0472 0e00  mple_engine).r..
-00000c50: 0000 7229 0000 0072 2a00 0000 720f 0000  ..r)...r*...r...
-00000c60: 0063 0400 0000 0000 0000 0000 0000 0400  .c..............
-00000c70: 0000 0600 0000 0300 0000 738e 0000 007c  ..........s....|
-00000c80: 0274 0075 0072 4074 017c 0174 0074 0274  .t.u.r@t.|.t.t.t
-00000c90: 0366 0383 0272 2c87 0087 0166 0264 0164  .f...r,....f.d.d
-00000ca0: 0284 087c 0144 0083 0153 0088 01a0 047c  ...|.D...S.....|
-00000cb0: 0188 0064 0319 00a1 0267 0153 006e 4a7c  ...d.....g.S.nJ|
-00000cc0: 0274 0374 0266 0276 0072 8a74 017c 0174  .t.t.f.v.r.t.|.t
-00000cd0: 0074 0274 0366 0383 0272 747c 0287 0087  .t.t.f...rt|....
-00000ce0: 0166 0264 0464 0284 087c 0144 0083 0183  .f.d.d...|.D....
-00000cf0: 0153 007c 0288 01a0 047c 0188 0064 0319  .S.|.....|...d..
-00000d00: 00a1 0267 0183 0153 0064 0053 0029 054e  ...g...S.d.S.).N
-00000d10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000d20: 0007 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
-00000d30: 7c00 5d14 7d01 8801 a000 7c01 8800 6400  |.].}.....|...d.
-00000d40: 1900 a102 9102 7104 5300 a901 7207 0000  ......q.S...r...
-00000d50: 00a9 0172 2000 0000 a902 da02 2e30 da04  ...r ........0..
-00000d60: 6974 656d a902 722a 0000 0072 1f00 0000  item..r*...r....
-00000d70: 7211 0000 0072 1400 0000 da0a 3c6c 6973  r....r......<lis
-00000d80: 7463 6f6d 703e 6900 0000 7234 0000 007a  tcomp>i...r4...z
-00000d90: 2a50 6172 7365 722e 7365 7175 656e 6365  *Parser.sequence
-00000da0: 5f65 6e67 696e 652e 3c6c 6f63 616c 733e  _engine.<locals>
-00000db0: 2e3c 6c69 7374 636f 6d70 3e72 0700 0000  .<listcomp>r....
-00000dc0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000dd0: 0007 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
-00000de0: 7c00 5d14 7d01 8801 a000 7c01 8800 6400  |.].}.....|...d.
-00000df0: 1900 a102 9102 7104 5300 724d 0000 0072  ......q.S.rM...r
-00000e00: 4e00 0000 724f 0000 0072 5200 0000 7211  N...rO...rR...r.
-00000e10: 0000 0072 1400 0000 7253 0000 006e 0000  ...r....rS...n..
-00000e20: 0072 3400 0000 2905 7243 0000 0072 2400  .r4...).rC...r$.
-00000e30: 0000 7247 0000 0072 4500 0000 7220 0000  ..rG...rE...r ..
-00000e40: 00a9 0472 1f00 0000 720e 0000 0072 2900  ...r....r....r).
-00000e50: 0000 722a 0000 0072 1100 0000 7252 0000  ..r*...r....rR..
-00000e60: 0072 1400 0000 7228 0000 0065 0000 0073  .r....r(...e...s
-00000e70: 1000 0000 0002 0801 1001 1402 1401 0c01  ................
-00000e80: 1001 1802 7a16 5061 7273 6572 2e73 6571  ....z.Parser.seq
-00000e90: 7565 6e63 655f 656e 6769 6e65 6304 0000  uence_enginec...
-00000ea0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00000eb0: 0003 0000 0073 6600 0000 7c02 7400 7500  .....sf...|.t.u.
-00000ec0: 7230 7401 7c01 7402 7400 6602 8302 7262  r0t.|.t.t.f...rb
-00000ed0: 8700 8701 6602 6401 6402 8408 7c01 a003  ....f.d.d...|...
-00000ee0: a100 4400 8301 5300 6e32 7c02 7402 7500  ..D...S.n2|.t.u.
-00000ef0: 7262 7401 7c01 7402 7400 6602 8302 7262  rbt.|.t.t.f...rb
-00000f00: 7402 8700 8701 6602 6403 6402 8408 7c01  t.....f.d.d...|.
-00000f10: a003 a100 4400 8301 8301 5300 6400 5300  ....D.....S.d.S.
-00000f20: 2904 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000f30: 0300 0000 0800 0000 1300 0000 732e 0000  ............s...
-00000f40: 0069 007c 005d 265c 027d 017d 0288 01a0  .i.|.]&\.}.}....
-00000f50: 007c 0188 0064 0019 00a1 0288 01a0 007c  .|...d.........|
-00000f60: 0288 0064 0119 00a1 0293 0271 0453 00a9  ...d.......q.S..
-00000f70: 0272 0700 0000 e9ff ffff ff72 4e00 0000  .r.........rN...
-00000f80: a903 7250 0000 00da 016b da01 7672 5200  ..rP.....k..vrR.
-00000f90: 0000 7211 0000 0072 1400 0000 da0a 3c64  ..r....r......<d
-00000fa0: 6963 7463 6f6d 703e 7600 0000 7234 0000  ictcomp>v...r4..
-00000fb0: 007a 2950 6172 7365 722e 6d61 7070 696e  .z)Parser.mappin
-00000fc0: 675f 656e 6769 6e65 2e3c 6c6f 6361 6c73  g_engine.<locals
-00000fd0: 3e2e 3c64 6963 7463 6f6d 703e 6301 0000  >.<dictcomp>c...
-00000fe0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-00000ff0: 0013 0000 0073 2e00 0000 6900 7c00 5d26  .....s....i.|.]&
-00001000: 5c02 7d01 7d02 8801 a000 7c01 8800 6400  \.}.}.....|...d.
-00001010: 1900 a102 8801 a000 7c02 8800 6401 1900  ........|...d...
-00001020: a102 9302 7104 5300 7255 0000 0072 4e00  ....q.S.rU...rN.
-00001030: 0000 7257 0000 0072 5200 0000 7211 0000  ..rW...rR...r...
-00001040: 0072 1400 0000 725a 0000 0079 0000 0072  .r....rZ...y...r
-00001050: 3400 0000 2904 da04 6469 6374 7224 0000  4...)...dictr$..
-00001060: 00da 0843 6861 696e 4d61 70da 0569 7465  ...ChainMap..ite
-00001070: 6d73 7254 0000 0072 1100 0000 7252 0000  msrT...r....rR..
-00001080: 0072 1400 0000 722c 0000 0072 0000 0073  .r....r,...r...s
-00001090: 0c00 0000 0002 0801 0e01 1a01 0801 0e01  ................
-000010a0: 7a15 5061 7273 6572 2e6d 6170 7069 6e67  z.Parser.mapping
-000010b0: 5f65 6e67 696e 6529 0372 0e00 0000 da07  _engine).r......
-000010c0: 6765 6e65 7269 6372 0f00 0000 6303 0000  genericr....c...
-000010d0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-000010e0: 0043 0000 0073 1600 0000 7c02 7400 7500  .C...s....|.t.u.
-000010f0: 7212 7c00 a001 7c01 a101 5300 6400 5300  r.|...|...S.d.S.
-00001100: 7210 0000 0029 0272 0b00 0000 da0d 6e75  r....).r......nu
-00001110: 6d62 6572 5f65 6e67 696e 6529 0372 1f00  mber_engine).r..
-00001120: 0000 720e 0000 0072 5e00 0000 7211 0000  ..r....r^...r...
-00001130: 0072 1100 0000 7214 0000 0072 2d00 0000  .r....r....r-...
-00001140: 7b00 0000 7304 0000 0000 0208 017a 1550  {...s........z.P
-00001150: 6172 7365 722e 6765 6e65 7269 635f 656e  arser.generic_en
-00001160: 6769 6e65 720d 0000 0063 0200 0000 0000  giner....c......
-00001170: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00001180: 0000 732a 0000 0074 007c 0174 0174 0266  ..s*...t.|.t.t.f
-00001190: 0283 0272 1667 007c 01a2 0153 0074 007c  ...r.g.|...S.t.|
-000011a0: 0174 0383 0272 247c 0153 007c 0167 0153  .t...r$|.S.|.g.S
-000011b0: 0072 1000 0000 2904 7224 0000 0072 4500  .r....).r$...rE.
-000011c0: 0000 7247 0000 0072 4300 0000 a902 721f  ..rG...rC.....r.
-000011d0: 0000 0072 0e00 0000 7211 0000 0072 1100  ...r....r....r..
-000011e0: 0000 7214 0000 0072 4400 0000 8000 0000  ..r....rD.......
-000011f0: 7306 0000 0000 020e 0108 017a 1250 6172  s..........z.Par
-00001200: 7365 722e 6c69 7374 5f65 6e67 696e 6563  ser.list_enginec
-00001210: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001220: 0400 0000 4300 0000 732a 0000 0074 007c  ....C...s*...t.|
-00001230: 0174 0174 0266 0283 0272 1669 007c 01a5  .t.t.f...r.i.|..
-00001240: 0153 0074 007c 0174 0383 0272 247c 0153  .S.t.|.t...r$|.S
-00001250: 007c 0168 0153 0072 1000 0000 2904 7224  .|.h.S.r....).r$
-00001260: 0000 0072 4300 0000 7247 0000 0072 4500  ...rC...rG...rE.
-00001270: 0000 7260 0000 0072 1100 0000 7211 0000  ..r`...r....r...
-00001280: 0072 1400 0000 7246 0000 0086 0000 0073  .r....rF.......s
-00001290: 0600 0000 0002 0e01 0801 7a11 5061 7273  ..........z.Pars
-000012a0: 6572 2e73 6574 5f65 6e67 696e 6563 0200  er.set_enginec..
-000012b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000012c0: 0000 4300 0000 7332 0000 0074 007c 0174  ..C...s2...t.|.t
-000012d0: 0174 0266 0283 0272 1a74 0367 007c 01a2  .t.f...r.t.g.|..
-000012e0: 0183 0153 0074 007c 0174 0383 0272 287c  ...S.t.|.t...r(|
-000012f0: 0153 0074 037c 0167 0183 0153 0072 1000  .S.t.|.g...S.r..
-00001300: 0000 2904 7224 0000 0072 4300 0000 7245  ..).r$...rC...rE
-00001310: 0000 0072 4700 0000 7260 0000 0072 1100  ...rG...r`...r..
-00001320: 0000 7211 0000 0072 1400 0000 7248 0000  ..r....r....rH..
-00001330: 008c 0000 0073 0600 0000 0002 0e01 0c01  .....s..........
-00001340: 7a13 5061 7273 6572 2e74 7570 6c65 5f65  z.Parser.tuple_e
-00001350: 6e67 696e 6563 0200 0000 0000 0000 0000  nginec..........
-00001360: 0000 0200 0000 0200 0000 4300 0000 7308  ..........C...s.
-00001370: 0000 0074 007c 0183 0153 0072 1000 0000  ...t.|...S.r....
-00001380: 2901 7235 0000 0072 6000 0000 7211 0000  ).r5...r`...r...
-00001390: 0072 1100 0000 7214 0000 0072 3600 0000  .r....r....r6...
-000013a0: 9200 0000 7302 0000 0000 027a 1150 6172  ....s......z.Par
-000013b0: 7365 722e 7374 725f 656e 6769 6e65 6302  ser.str_enginec.
-000013c0: 0000 0000 0000 0000 0000 0002 0000 0007  ................
-000013d0: 0000 0043 0000 0073 5600 0000 7400 7c01  ...C...sV...t.|.
-000013e0: 7401 8302 7226 7402 7403 7404 a005 6401  t...r&t.t.t...d.
-000013f0: 6402 7c01 a103 8301 a006 6403 a101 8301  d.|.......d.....
-00001400: 5300 7400 7c01 7407 8302 7238 7402 7c01  S.t.|.t...r8t.|.
-00001410: 8301 5300 7400 7c01 7408 6a09 7408 6a08  ..S.t.|.t.j.t.j.
-00001420: 6602 8302 7252 7c01 a00a a100 5300 7c01  f...rR|.....S.|.
-00001430: 5300 2904 4efa 012c da01 2e72 0700 0000  S.).N..,...r....
-00001440: 290b 7224 0000 0072 3500 0000 7237 0000  ).r$...r5...r7..
-00001450: 0072 3900 0000 da02 7265 da03 7375 62da  .r9.....re..sub.
-00001460: 095f 5f72 6f75 6e64 5f5f 7241 0000 0072  .__round__rA...r
-00001470: 3b00 0000 723c 0000 00da 0974 6f6f 7264  ;...r<.....toord
-00001480: 696e 616c 7260 0000 0072 1100 0000 7211  inalr`...r....r.
-00001490: 0000 0072 1400 0000 7238 0000 0096 0000  ...r....r8......
-000014a0: 0073 0e00 0000 0002 0a01 1c01 0a01 0801  .s..............
-000014b0: 1201 0801 7a11 5061 7273 6572 2e69 6e74  ....z.Parser.int
-000014c0: 5f65 6e67 696e 655a 0b43 6f6e 7465 7874  _engineZ.Context
-000014d0: 4261 7365 2902 720e 0000 00da 0a6d 6f64  Base).r......mod
-000014e0: 656c 5f74 7970 6563 0300 0000 0000 0000  el_typec........
-000014f0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00001500: 7310 0000 007c 026a 0066 0069 007c 01a4  s....|.j.f.i.|..
-00001510: 018e 0153 0072 1000 0000 2901 5a0b 7361  ...S.r....).Z.sa
-00001520: 6665 5f63 7265 6174 6529 0372 1f00 0000  fe_create).r....
-00001530: 720e 0000 0072 6700 0000 7211 0000 0072  r....rg...r....r
-00001540: 1100 0000 7214 0000 00da 0d63 6f6e 7465  ....r......conte
-00001550: 7874 5f6d 6f64 656c a000 0000 7302 0000  xt_model....s...
-00001560: 0000 027a 1450 6172 7365 722e 636f 6e74  ...z.Parser.cont
-00001570: 6578 745f 6d6f 6465 6c63 0200 0000 0000  ext_modelc......
-00001580: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-00001590: 0000 7366 0000 0074 007c 0174 0183 0272  ..sf...t.|.t...r
-000015a0: 1c74 0274 03a0 0464 0164 027c 01a1 0383  .t.t...d.d.|....
-000015b0: 0153 0074 007c 0174 0583 0272 2e74 027c  .S.t.|.t...r.t.|
-000015c0: 0183 0153 0074 007c 0174 0683 0272 4074  ...S.t.|.t...r@t
-000015d0: 027c 0183 0153 0074 007c 0174 0783 0272  .|...S.t.|.t...r
-000015e0: 6274 0274 03a0 0464 0164 027c 01a0 0864  bt.t...d.d.|...d
-000015f0: 03a1 01a1 0383 0153 007c 0153 0029 044e  .......S.|.S.).N
-00001600: 7261 0000 0072 6200 0000 fa05 7574 662d  ra...rb.....utf-
-00001610: 3829 0972 2400 0000 7235 0000 0072 3900  8).r$...r5...r9.
-00001620: 0000 7263 0000 0072 6400 0000 7237 0000  ..rc...rd...r7..
-00001630: 0072 4100 0000 723f 0000 00da 0664 6563  .rA...r?.....dec
-00001640: 6f64 6572 6000 0000 7211 0000 0072 1100  oder`...r....r..
-00001650: 0000 7214 0000 0072 3a00 0000 a400 0000  ..r....r:.......
-00001660: 7312 0000 0000 020a 0112 010a 0108 010a  s...............
-00001670: 0108 010a 0118 017a 1350 6172 7365 722e  .......z.Parser.
-00001680: 666c 6f61 745f 656e 6769 6e65 6302 0000  float_enginec...
-00001690: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000016a0: 0043 0000 0073 4400 0000 7400 7c01 7401  .C...sD...t.|.t.
-000016b0: 8302 7216 7402 6a03 a004 7c01 a101 5300  ..r.t.j...|...S.
-000016c0: 7400 7c01 7402 6a02 8302 722a 7c01 a003  t.|.t.j...r*|...
-000016d0: a100 5300 7400 7c01 7405 8302 7240 7402  ..S.t.|.t...r@t.
-000016e0: 6a03 a006 7c01 a101 5300 6400 5300 7210  j...|...S.d.S.r.
-000016f0: 0000 0029 0772 2400 0000 7235 0000 0072  ...).r$...r5...r
-00001700: 3b00 0000 723c 0000 00da 0d66 726f 6d69  ;...r<.....fromi
-00001710: 736f 666f 726d 6174 7237 0000 00da 0b66  soformatr7.....f
-00001720: 726f 6d6f 7264 696e 616c 7260 0000 0072  romordinalr`...r
-00001730: 1100 0000 7211 0000 0072 1400 0000 723d  ....r....r....r=
-00001740: 0000 00b0 0000 0073 0c00 0000 0002 0a01  .......s........
-00001750: 0c01 0c01 0801 0a01 7a12 5061 7273 6572  ........z.Parser
-00001760: 2e64 6174 655f 656e 6769 6e65 2903 720e  .date_engine).r.
-00001770: 0000 00da 0965 6e75 6d5f 7479 7065 720f  .....enum_typer.
-00001780: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00001790: 0400 0000 0a00 0000 4300 0000 7344 0000  ........C...sD..
-000017a0: 007a 0a7c 027c 0119 0057 0053 0004 0074  .z.|.|...W.S...t
-000017b0: 0079 3e01 007d 0301 007a 1c74 017c 0383  .y>..}...z.t.|..
-000017c0: 0101 007c 027c 0183 0157 0006 0059 0064  ...|.|...W...Y.d
-000017d0: 007d 037e 0353 0064 007d 037e 0330 0030  .}.~.S.d.}.~.0.0
-000017e0: 0064 0053 0072 1000 0000 2902 da0d 4261  .d.S.r....)...Ba
-000017f0: 7365 4578 6365 7074 696f 6e72 2f00 0000  seExceptionr/...
-00001800: 2904 721f 0000 0072 0e00 0000 726d 0000  ).r....r....rm..
-00001810: 0072 3000 0000 7211 0000 0072 1100 0000  .r0...r....r....
-00001820: 7214 0000 0072 3100 0000 b900 0000 730a  r....r1.......s.
-00001830: 0000 0000 0202 010a 010e 0108 017a 1250  .............z.P
-00001840: 6172 7365 722e 656e 756d 5f65 6e67 696e  arser.enum_engin
-00001850: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00001860: 0000 0400 0000 4300 0000 734c 0000 0074  ......C...sL...t
-00001870: 007c 0174 0183 0272 1674 026a 02a0 037c  .|.t...r.t.j...|
-00001880: 01a1 0153 0074 007c 0174 026a 0483 0272  ...S.t.|.t.j...r
-00001890: 3274 026a 02a0 057c 01a0 06a1 00a1 0153  2t.j...|.......S
-000018a0: 0074 007c 0174 0783 0272 4874 026a 02a0  .t.|.t...rHt.j..
-000018b0: 057c 01a1 0153 0064 0053 0072 1000 0000  .|...S.d.S.r....
-000018c0: 2908 7224 0000 0072 3500 0000 723b 0000  ).r$...r5...r;..
-000018d0: 0072 6b00 0000 723c 0000 0072 6c00 0000  .rk...r<...rl...
-000018e0: 7266 0000 0072 3700 0000 7260 0000 0072  rf...r7...r`...r
-000018f0: 1100 0000 7211 0000 0072 1400 0000 723e  ....r....r....r>
-00001900: 0000 00c1 0000 0073 0c00 0000 0002 0a01  .......s........
-00001910: 0c01 0c01 1001 0a01 7a16 5061 7273 6572  ........z.Parser
-00001920: 2e64 6174 6574 696d 655f 656e 6769 6e65  .datetime_engine
-00001930: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001940: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-00001950: 7c01 8301 a001 6401 a101 5300 2902 4e72  |.....d...S.).Nr
-00001960: 6900 0000 2902 7235 0000 00da 0665 6e63  i...).r5.....enc
-00001970: 6f64 6572 6000 0000 7211 0000 0072 1100  oder`...r....r..
-00001980: 0000 7214 0000 0072 4000 0000 ca00 0000  ..r....r@.......
-00001990: 7302 0000 0000 027a 1350 6172 7365 722e  s......z.Parser.
-000019a0: 6279 7465 735f 656e 6769 6e65 6302 0000  bytes_enginec...
-000019b0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-000019c0: 0043 0000 0073 5000 0000 7400 7c01 7401  .C...sP...t.|.t.
-000019d0: 8302 721c 7402 7403 a004 6401 6402 7c01  ..r.t.t...d.d.|.
-000019e0: a103 8301 5300 7400 7c01 7405 8302 7232  ....S.t.|.t...r2
-000019f0: 7402 7401 7c01 8301 8301 5300 7400 7c01  t.t.|.....S.t.|.
-00001a00: 7406 8302 724c 7402 7401 7405 7c01 8301  t...rLt.t.t.|...
-00001a10: 8301 8301 5300 6400 5300 2903 4efa 035c  ....S.d.S.).N..\
-00001a20: 2e2c 7262 0000 0029 0772 2400 0000 7235  .,rb...).r$...r5
-00001a30: 0000 0072 4100 0000 7263 0000 0072 6400  ...rA...rc...rd.
-00001a40: 0000 7239 0000 0072 3700 0000 7260 0000  ..r9...r7...r`..
-00001a50: 0072 1100 0000 7211 0000 0072 1400 0000  .r....r....r....
-00001a60: 7242 0000 00ce 0000 0073 0c00 0000 0002  rB.......s......
-00001a70: 0a01 1201 0a01 0c01 0a01 7a15 5061 7273  ..........z.Pars
-00001a80: 6572 2e64 6563 696d 616c 5f65 6e67 696e  er.decimal_engin
-00001a90: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00001aa0: 0000 0400 0000 4300 0000 734e 0000 0074  ......C...sN...t
-00001ab0: 007c 0174 0183 0272 3074 02a0 0364 017c  .|.t...r0t...d.|
-00001ac0: 01a1 0272 227c 00a0 047c 0174 05a1 0253  ...r"|...|.t...S
-00001ad0: 007c 00a0 047c 0174 06a1 0253 006e 1a74  .|...|.t...S.n.t
-00001ae0: 007c 0174 076a 0874 076a 0766 0283 0272  .|.t.j.t.j.f...r
-00001af0: 4a7c 01a0 09a1 0053 0064 0053 0029 024e  J|.....S.d.S.).N
-00001b00: 7270 0000 0029 0a72 2400 0000 7235 0000  rp...).r$...r5..
-00001b10: 0072 6300 0000 da05 6d61 7463 6872 2000  .rc.....matchr .
-00001b20: 0000 7239 0000 0072 3700 0000 723b 0000  ..r9...r7...r;..
-00001b30: 0072 3c00 0000 7266 0000 0072 6000 0000  .r<...rf...r`...
-00001b40: 7211 0000 0072 1100 0000 7214 0000 0072  r....r....r....r
-00001b50: 5f00 0000 d700 0000 730c 0000 0000 020a  _.......s.......
-00001b60: 010c 010c 020e 0112 017a 1450 6172 7365  .........z.Parse
-00001b70: 722e 6e75 6d62 6572 5f65 6e67 696e 654e  r.number_engineN
-00001b80: 2921 7216 0000 0072 1700 0000 7218 0000  )!r....r....r...
-00001b90: 00da 0b63 6c61 7373 6d65 7468 6f64 7208  ...classmethodr.
-00001ba0: 0000 00da 0474 7970 6572 0900 0000 7220  .....typer....r 
-00001bb0: 0000 00da 0c50 6172 7365 7252 6574 7572  .....ParserRetur
-00001bc0: 6e72 1e00 0000 720c 0000 0072 2600 0000  nr....r....r&...
-00001bd0: 7247 0000 0072 2800 0000 7219 0000 0072  rG...r(...r....r
-00001be0: 5b00 0000 725c 0000 0072 2c00 0000 722d  [...r\...r,...r-
-00001bf0: 0000 0072 4400 0000 7246 0000 0072 4800  ...rD...rF...rH.
-00001c00: 0000 7236 0000 0072 3800 0000 7268 0000  ..r6...r8...rh..
-00001c10: 0072 3a00 0000 723d 0000 0072 4b00 0000  .r:...r=...rK...
-00001c20: 7231 0000 0072 3e00 0000 7240 0000 0072  r1...r>...r@...r
-00001c30: 4200 0000 725f 0000 0072 1100 0000 7211  B...r_...r....r.
-00001c40: 0000 0072 1100 0000 7214 0000 0072 0300  ...r....r....r..
-00001c50: 0000 2d00 0000 734c 0000 0008 0102 0116  ..-...sL........
-00001c60: 0302 0118 1502 0116 1c02 011a 0c02 0122  ..............."
-00001c70: 0802 0114 0402 0112 0502 0112 0502 0112  ................
-00001c80: 0502 0112 0302 010a 0902 0116 0302 010a  ................
-00001c90: 0b02 0112 0802 0118 0702 0112 0802 0112  ................
-00001ca0: 0302 0112 0802 0172 0300 0000 6300 0000  .......r....c...
-00001cb0: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00001cc0: 0040 0000 0073 dc00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00001cd0: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-00001ce0: 5a04 6505 6506 6507 1900 6405 9c01 6406  Z.e.e.e...d...d.
-00001cf0: 6407 8404 8301 5a08 6505 6408 6409 8400  d.....Z.e.d.d...
-00001d00: 8301 5a09 6505 640a 640b 8400 8301 5a0a  ..Z.e.d.d.....Z.
-00001d10: 6505 640c 640d 8400 8301 5a0b 6505 640e  e.d.d.....Z.e.d.
-00001d20: 640f 8400 8301 5a0c 6505 6410 6411 8400  d.....Z.e.d.d...
-00001d30: 8301 5a0d 6505 650e 6405 9c01 6412 6413  ..Z.e.e.d...d.d.
-00001d40: 8404 8301 5a0f 6505 6414 6415 8400 8301  ....Z.e.d.d.....
-00001d50: 5a10 6505 6416 6417 8400 8301 5a11 6505  Z.e.d.d.....Z.e.
-00001d60: 6418 6419 8400 8301 5a12 6505 641a 641b  d.d.....Z.e.d.d.
-00001d70: 8400 8301 5a13 6505 641c 641d 8400 8301  ....Z.e.d.d.....
-00001d80: 5a14 6515 650e 641e 9c02 641f 6420 8404  Z.e.e.d...d.d ..
-00001d90: 5a16 6517 6518 641e 9c02 6421 6422 8404  Z.e.e.d...d!d"..
-00001da0: 5a19 6423 5300 2924 7201 0000 0063 0200  Z.d#S.)$r....c..
-00001db0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00001dc0: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-00001dd0: 0064 0053 0072 1000 0000 2901 da09 7479  .d.S.r....)...ty
-00001de0: 7065 5f68 696e 7429 0272 1300 0000 7275  pe_hint).r....ru
-00001df0: 0000 0072 1100 0000 7211 0000 0072 1400  ...r....r....r..
-00001e00: 0000 da08 5f5f 696e 6974 5f5f e500 0000  ....__init__....
-00001e10: 7302 0000 0000 017a 1154 7970 6548 696e  s......z.TypeHin
-00001e20: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
-00001e30: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00001e40: 0000 0073 1800 0000 7400 7c00 8301 6a01  ...s....t.|...j.
-00001e50: 9b00 6401 7c00 6a02 9b00 6402 9d04 5300  ..d.|.j...d...S.
-00001e60: 2903 4efa 0128 fa01 2929 0372 7300 0000  ).N..(..)).rs...
-00001e70: 7216 0000 0072 7500 0000 a901 7213 0000  r....ru.....r...
-00001e80: 0072 1100 0000 7211 0000 0072 1400 0000  .r....r....r....
-00001e90: da07 5f5f 7374 725f 5fe8 0000 0073 0200  ..__str__....s..
-00001ea0: 0000 0001 7a10 5479 7065 4869 6e74 2e5f  ....z.TypeHint._
-00001eb0: 5f73 7472 5f5f 2901 720f 0000 0063 0100  _str__).r....c..
-00001ec0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00001ed0: 0000 4300 0000 7318 0000 0074 0064 0164  ..C...s....t.d.d
-00001ee0: 0284 0074 017c 006a 0283 0144 0083 0183  ...t.|.j...D....
-00001ef0: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-00001f00: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-00001f10: 2600 0000 6700 7c00 5d1e 7d01 7400 7c01  &...g.|.].}.t.|.
-00001f20: 7401 8302 7204 7c01 7401 6400 8301 7501  t...r.|.t.d...u.
-00001f30: 7204 7c01 9102 7104 5300 7210 0000 00a9  r.|...q.S.r.....
-00001f40: 0272 2400 0000 7273 0000 0029 0272 5000  .r$...rs...).rP.
-00001f50: 0000 da01 7472 1100 0000 7211 0000 0072  ....tr....r....r
-00001f60: 1400 0000 7253 0000 00ed 0000 0072 3400  ....rS.......r4.
-00001f70: 0000 7a21 5479 7065 4869 6e74 2e61 7267  ..z!TypeHint.arg
-00001f80: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-00001f90: 636f 6d70 3e29 0372 4700 0000 da08 6765  comp>).rG.....ge
-00001fa0: 745f 6172 6773 7275 0000 0072 7900 0000  t_argsru...ry...
-00001fb0: 7211 0000 0072 1100 0000 7214 0000 0072  r....r....r....r
-00001fc0: 2a00 0000 eb00 0000 7302 0000 0000 027a  *.......s......z
-00001fd0: 0d54 7970 6548 696e 742e 6172 6773 6301  .TypeHint.argsc.
-00001fe0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001ff0: 0000 0043 0000 0073 1400 0000 7400 6401  ...C...s....t.d.
-00002000: 6402 8400 7c00 6a01 4400 8301 8301 5300  d...|.j.D.....S.
-00002010: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00002020: 0200 0000 0500 0000 5300 0000 7318 0000  ........S...s...
-00002030: 0067 007c 005d 107d 0174 007c 0174 0183  .g.|.].}.t.|.t..
-00002040: 020c 0091 0271 0453 0072 1100 0000 727b  .....q.S.r....r{
-00002050: 0000 0072 4f00 0000 7211 0000 0072 1100  ...rO...r....r..
-00002060: 0000 7214 0000 0072 5300 0000 f100 0000  ..r....rS.......
-00002070: 7234 0000 007a 2c54 7970 6548 696e 742e  r4...z,TypeHint.
-00002080: 6973 5f61 7267 735f 6765 6e65 7269 632e  is_args_generic.
-00002090: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000020a0: 6d70 3e29 02da 0361 6c6c 722a 0000 0072  mp>)...allr*...r
-000020b0: 7900 0000 7211 0000 0072 1100 0000 7214  y...r....r....r.
-000020c0: 0000 00da 0f69 735f 6172 6773 5f67 656e  .....is_args_gen
-000020d0: 6572 6963 ef00 0000 7302 0000 0000 027a  eric....s......z
-000020e0: 1854 7970 6548 696e 742e 6973 5f61 7267  .TypeHint.is_arg
-000020f0: 735f 6765 6e65 7269 6363 0100 0000 0000  s_genericc......
-00002100: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00002110: 0000 730a 0000 0074 007c 006a 0183 0153  ..s....t.|.j...S
-00002120: 0072 1000 0000 2902 da0a 6765 745f 6f72  .r....)...get_or
-00002130: 6967 696e 7275 0000 0072 7900 0000 7211  iginru...ry...r.
-00002140: 0000 0072 1100 0000 7214 0000 0072 2900  ...r....r....r).
-00002150: 0000 f300 0000 7302 0000 0000 027a 0f54  ......s......z.T
-00002160: 7970 6548 696e 742e 6f72 6967 696e 6301  ypeHint.originc.
-00002170: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00002180: 0000 0043 0000 0073 0a00 0000 7c00 6a00  ...C...s....|.j.
-00002190: 7401 7600 5300 7210 0000 0029 0272 2900  t.v.S.r....).r).
-000021a0: 0000 da12 5475 706c 6553 6571 7565 6e63  ....TupleSequenc
-000021b0: 6554 7970 6573 7279 0000 0072 1100 0000  eTypesry...r....
-000021c0: 7211 0000 0072 1400 0000 7227 0000 00f7  r....r....r'....
-000021d0: 0000 0073 0200 0000 0002 7a14 5479 7065  ...s......z.Type
-000021e0: 4869 6e74 2e69 735f 7365 7175 656e 6365  Hint.is_sequence
-000021f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002200: 0002 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
-00002210: 6a00 7401 7600 5300 7210 0000 0029 0272  j.t.v.S.r....).r
-00002220: 2900 0000 da0d 5475 706c 654d 6170 5479  ).....TupleMapTy
-00002230: 7065 7372 7900 0000 7211 0000 0072 1100  pesry...r....r..
-00002240: 0000 7214 0000 0072 2b00 0000 fb00 0000  ..r....r+.......
-00002250: 7302 0000 0000 027a 1354 7970 6548 696e  s......z.TypeHin
-00002260: 742e 6973 5f6d 6170 7069 6e67 6301 0000  t.is_mappingc...
-00002270: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00002280: 0043 0000 0073 0e00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00002290: 7402 8302 0c00 5300 7210 0000 0029 0372  t.....S.r....).r
-000022a0: 2400 0000 7229 0000 0072 7300 0000 7279  $...r)...rs...ry
-000022b0: 0000 0072 1100 0000 7211 0000 0072 1400  ...r....r....r..
-000022c0: 0000 da0a 6973 5f67 656e 6572 6963 ff00  ....is_generic..
-000022d0: 0000 7302 0000 0000 027a 1354 7970 6548  ..s......z.TypeH
-000022e0: 696e 742e 6973 5f67 656e 6572 6963 6301  int.is_genericc.
-000022f0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00002300: 0000 0043 0000 0073 1400 0000 7c00 6a00  ...C...s....|.j.
-00002310: 0c00 6f12 7401 7c00 6a02 7403 8302 5300  ..o.t.|.j.t...S.
-00002320: 7210 0000 0029 0472 2a00 0000 7224 0000  r....).r*...r$..
-00002330: 0072 7500 0000 7273 0000 0072 7900 0000  .ru...rs...ry...
-00002340: 7211 0000 0072 1100 0000 7214 0000 0072  r....r....r....r
-00002350: 2300 0000 0301 0000 7302 0000 0000 027a  #.......s......z
-00002360: 1754 7970 6548 696e 742e 6973 5f73 696d  .TypeHint.is_sim
-00002370: 706c 655f 7479 7065 6301 0000 0000 0000  ple_typec.......
-00002380: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00002390: 0073 0e00 0000 7400 6400 8301 7c00 6a01  .s....t.d...|.j.
-000023a0: 7600 5300 7210 0000 0029 0272 7300 0000  v.S.r....).rs...
-000023b0: 722a 0000 0072 7900 0000 7211 0000 0072  r*...ry...r....r
-000023c0: 1100 0000 7214 0000 00da 0b69 735f 6f70  ....r......is_op
-000023d0: 7469 6f6e 616c 0701 0000 7302 0000 0000  tional....s.....
-000023e0: 027a 1454 7970 6548 696e 742e 6973 5f6f  .z.TypeHint.is_o
-000023f0: 7074 696f 6e61 6c63 0100 0000 0000 0000  ptionalc........
-00002400: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00002410: 7328 0000 007c 006a 0072 0c7c 006a 0153  s(...|.j.r.|.j.S
-00002420: 007c 006a 0273 187c 006a 0372 1e7c 006a  .|.j.s.|.j.r.|.j
-00002430: 0453 007c 006a 0553 0064 0053 0072 1000  .S.|.j.S.d.S.r..
-00002440: 0000 2906 7223 0000 0072 7500 0000 722b  ..).r#...ru...r+
-00002450: 0000 0072 2700 0000 7229 0000 0072 2a00  ...r'...r)...r*.
-00002460: 0000 7279 0000 0072 1100 0000 7211 0000  ..ry...r....r...
-00002470: 0072 1400 0000 da0d 6578 7065 6374 6564  .r......expected
-00002480: 5f74 7970 650b 0100 0073 0a00 0000 0002  _type....s......
-00002490: 0601 0601 0c01 0602 7a16 5479 7065 4869  ........z.TypeHi
-000024a0: 6e74 2e65 7870 6563 7465 645f 7479 7065  nt.expected_type
-000024b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000024c0: 0003 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
-000024d0: 7c00 6a01 7402 8302 5300 7210 0000 0029  |.j.t...S.r....)
-000024e0: 0372 4a00 0000 7275 0000 00da 0855 7365  .rJ...ru.....Use
-000024f0: 7244 6963 7472 7900 0000 7211 0000 0072  rDictry...r....r
-00002500: 1100 0000 7214 0000 00da 0d69 735f 6469  ....r......is_di
-00002510: 6374 5f6d 6f64 656c 1401 0000 7302 0000  ct_model....s...
-00002520: 0000 027a 1654 7970 6548 696e 742e 6973  ...z.TypeHint.is
-00002530: 5f64 6963 745f 6d6f 6465 6c63 0100 0000  _dict_modelc....
-00002540: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00002550: 4300 0000 730a 0000 0074 007c 006a 0183  C...s....t.|.j..
-00002560: 0153 0072 1000 0000 2902 da0c 6973 5f64  .S.r....)...is_d
-00002570: 6174 6163 6c61 7373 7275 0000 0072 7900  ataclassru...ry.
-00002580: 0000 7211 0000 0072 1100 0000 7214 0000  ..r....r....r...
-00002590: 0072 8800 0000 1801 0000 7302 0000 0000  .r........s.....
-000025a0: 027a 1554 7970 6548 696e 742e 6973 5f64  .z.TypeHint.is_d
-000025b0: 6174 6163 6c61 7373 6301 0000 0000 0000  ataclassc.......
-000025c0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-000025d0: 0073 0e00 0000 7c00 6a00 7401 7402 1900  .s....|.j.t.t...
-000025e0: 6b02 5300 7210 0000 0029 0372 7500 0000  k.S.r....).ru...
-000025f0: 7243 0000 0072 3500 0000 7279 0000 0072  rC...r5...ry...r
-00002600: 1100 0000 7211 0000 0072 1400 0000 da0e  ....r....r......
-00002610: 6973 5f73 7472 696e 675f 6c69 7374 1c01  is_string_list..
-00002620: 0000 7302 0000 0000 027a 1754 7970 6548  ..s......z.TypeH
-00002630: 696e 742e 6973 5f73 7472 696e 675f 6c69  int.is_string_li
-00002640: 7374 720d 0000 0063 0200 0000 0000 0000  str....c........
-00002650: 0000 0000 0200 0000 0400 0000 0300 0000  ................
-00002660: 73de 0000 0088 006a 0072 5688 006a 0172  s......j.rV..j.r
-00002670: 1874 027c 0188 006a 0383 0253 0088 006a  .t.|...j...S...j
-00002680: 0472 2874 027c 0174 0583 0253 0088 006a  .r(t.|.t...S...j
-00002690: 0672 4a74 027c 0174 0783 026f 4874 0864  .rJt.|.t...oHt.d
-000026a0: 0164 0284 007c 0144 0083 0183 0153 0074  .d...|.D.....S.t
-000026b0: 027c 0188 006a 0383 0253 0088 006a 0972  .|...j...S...j.r
-000026c0: 6874 027c 0188 006a 0a83 0253 0088 006a  ht.|...j...S...j
-000026d0: 0b72 9074 027c 0188 006a 0c83 026f 8e74  .r.t.|...j...o.t
-000026e0: 0887 0066 0164 0364 0284 087c 0144 0083  ...f.d.d...|.D..
-000026f0: 0183 0153 0088 006a 0d72 d674 027c 0188  ...S...j.r.t.|..
-00002700: 006a 0c83 026f d474 0887 0066 0164 0464  .j...o.t...f.d.d
-00002710: 0284 087c 01a0 0ea1 0044 0083 0183 016f  ...|.....D.....o
-00002720: d474 0887 0066 0164 0564 0284 087c 01a0  .t...f.d.d...|..
-00002730: 0fa1 0044 0083 0183 0153 0064 0653 0064  ...D.....S.d.S.d
-00002740: 0053 0029 074e 6301 0000 0000 0000 0000  .S.).Nc.........
-00002750: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-00002760: 1600 0000 6700 7c00 5d0e 7d01 7400 7c01  ....g.|.].}.t.|.
-00002770: 7401 8302 9102 7104 5300 7211 0000 0029  t.....q.S.r....)
-00002780: 0272 2400 0000 7235 0000 0072 4f00 0000  .r$...r5...rO...
-00002790: 7211 0000 0072 1100 0000 7214 0000 0072  r....r....r....r
-000027a0: 5300 0000 2701 0000 7234 0000 007a 2754  S...'...r4...z'T
-000027b0: 7970 6548 696e 742e 6368 6563 6b5f 7479  ypeHint.check_ty
-000027c0: 7065 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  pe.<locals>.<lis
-000027d0: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
-000027e0: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-000027f0: 1800 0000 6700 7c00 5d10 7d01 7400 7c01  ....g.|.].}.t.|.
-00002800: 8800 6a01 8302 9102 7104 5300 7211 0000  ..j.....q.S.r...
-00002810: 00a9 0272 2400 0000 722a 0000 0072 4f00  ...r$...r*...rO.
-00002820: 0000 7279 0000 0072 1100 0000 7214 0000  ..ry...r....r...
-00002830: 0072 5300 0000 2c01 0000 7234 0000 0063  .rS...,...r4...c
-00002840: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00002850: 0800 0000 1300 0000 7324 0000 0067 007c  ........s$...g.|
-00002860: 005d 1c7d 0174 007c 0174 0188 006a 0264  .].}.t.|.t...j.d
-00002870: 0064 0185 0219 0083 0183 0291 0271 0453  .d...........q.S
-00002880: 0029 0272 0600 0000 4e29 0372 2400 0000  .).r....N).r$...
-00002890: 7247 0000 0072 2a00 0000 724f 0000 0072  rG...r*...rO...r
-000028a0: 7900 0000 7211 0000 0072 1400 0000 7253  y...r....r....rS
-000028b0: 0000 002f 0100 0072 3400 0000 6301 0000  .../...r4...c...
-000028c0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-000028d0: 0013 0000 0073 1c00 0000 6700 7c00 5d14  .....s....g.|.].
-000028e0: 7d01 7400 7c01 8800 6a01 6400 1900 8302  }.t.|...j.d.....
-000028f0: 9102 7104 5300 724d 0000 0072 8a00 0000  ..q.S.rM...r....
-00002900: 724f 0000 0072 7900 0000 7211 0000 0072  rO...ry...r....r
-00002910: 1400 0000 7253 0000 0030 0100 0072 3400  ....rS...0...r4.
-00002920: 0000 4629 1072 2300 0000 7288 0000 0072  ..F).r#...r....r
-00002930: 2400 0000 7275 0000 0072 8700 0000 725b  $...ru...r....r[
-00002940: 0000 0072 8900 0000 7243 0000 0072 7e00  ...r....rC...r~.
-00002950: 0000 7283 0000 0072 2a00 0000 7227 0000  ..r....r*...r'..
-00002960: 0072 2900 0000 722b 0000 00da 0676 616c  .r)...r+.....val
-00002970: 7565 73da 046b 6579 7372 1200 0000 7211  ues..keysr....r.
-00002980: 0000 0072 7900 0000 7214 0000 0072 2200  ...ry...r....r".
-00002990: 0000 2001 0000 732a 0000 0000 0106 0106  .. ...s*........
-000029a0: 010c 0106 010a 0106 011c 010c 0106 010c  ................
-000029b0: 0106 0122 0106 010e 0114 ff04 0102 0114  ..."............
-000029c0: ff02 ff02 047a 1354 7970 6548 696e 742e  .....z.TypeHint.
-000029d0: 6368 6563 6b5f 7479 7065 6302 0000 0000  check_typec.....
-000029e0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-000029f0: 0000 0073 1c00 0000 7c00 a000 7c01 a101  ...s....|...|...
-00002a00: 720e 7c01 5300 7401 a002 7c01 7c00 6a03  r.|.S.t...|.|.j.
-00002a10: a102 5300 7210 0000 0029 0472 2200 0000  ..S.r....).r"...
-00002a20: 7203 0000 0072 2000 0000 7275 0000 0072  r....r ...ru...r
-00002a30: 1200 0000 7211 0000 0072 1100 0000 7214  ....r....r....r.
-00002a40: 0000 00da 0570 6172 7365 3501 0000 7306  .....parse5...s.
-00002a50: 0000 0000 010a 0104 017a 0e54 7970 6548  .........z.TypeH
-00002a60: 696e 742e 7061 7273 654e 291a 7216 0000  int.parseN).r...
-00002a70: 0072 1700 0000 7218 0000 0072 7600 0000  .r....r....rv...
-00002a80: 727a 0000 00da 0870 726f 7065 7274 7972  rz.....propertyr
-00002a90: 4700 0000 7273 0000 0072 2a00 0000 727f  G...rs...r*...r.
-00002aa0: 0000 0072 2900 0000 7227 0000 0072 2b00  ...r)...r'...r+.
-00002ab0: 0000 7283 0000 00da 0462 6f6f 6c72 2300  ..r......boolr#.
-00002ac0: 0000 7284 0000 0072 8500 0000 7287 0000  ..r....r....r...
-00002ad0: 0072 8800 0000 7289 0000 00da 0341 6e79  .r....r......Any
-00002ae0: 7222 0000 0072 0800 0000 7209 0000 0072  r"...r....r....r
-00002af0: 8d00 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
-00002b00: 0000 0072 1400 0000 7201 0000 00e4 0000  ...r....r.......
-00002b10: 0073 3800 0000 0801 0803 0803 0201 1403  .s8.............
-00002b20: 0201 0a03 0201 0a03 0201 0a03 0201 0a03  ................
-00002b30: 0201 0a03 0201 1003 0201 0a03 0201 0a08  ................
-00002b40: 0201 0a03 0201 0a03 0201 0a03 1015 7201  ..............r.
-00002b50: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00002b60: 0200 0000 0400 0000 4300 0000 730c 0000  ........C...s...
-00002b70: 0074 00a0 017c 007c 01a1 0253 0072 1000  .t...|.|...S.r..
-00002b80: 0000 2902 7203 0000 0072 2000 0000 2902  ..).r....r ...).
-00002b90: 720e 0000 0072 7500 0000 7211 0000 0072  r....ru...r....r
-00002ba0: 1100 0000 7214 0000 0072 0200 0000 3b01  ....r....r....;.
-00002bb0: 0000 7302 0000 0000 0172 0200 0000 2930  ..s......r....)0
-00002bc0: da07 5f5f 616c 6c5f 5fda 085f 696d 706f  ..__all__.._impo
-00002bd0: 7274 73da 046e 756c 6c5a 1964 746d 6f64  rts..nullZ.dtmod
-00002be0: 656c 2e64 7466 6965 6c64 2e62 6173 655f  el.dtfield.base_
-00002bf0: 656e 756d 7219 0000 0072 3500 0000 7239  enumr....r5...r9
-00002c00: 0000 0072 3700 0000 728f 0000 00da 0d4a  ...r7...r......J
-00002c10: 736f 6e50 7269 6d69 7469 7665 725b 0000  sonPrimitiver[..
-00002c20: 0072 4300 0000 da08 4465 7461 4461 7461  .rC.....DetaData
-00002c30: da07 4465 7461 4b65 79da 0845 7870 6972  ..DetaKey..Expir
-00002c40: 6549 6e72 3b00 0000 da08 4578 7069 7265  eInr;.....Expire
-00002c50: 4174 da0c 4a73 6f6e 5365 7175 656e 6365  At..JsonSequence
-00002c60: da08 4a73 6f6e 4469 6374 da08 4a73 6f6e  ..JsonDict..Json
-00002c70: 6162 6c65 da09 4465 7461 5175 6572 79da  able..DetaQuery.
-00002c80: 0b45 7869 7374 5061 7261 6d73 da0b 5365  .ExistParams..Se
-00002c90: 6172 6368 5061 7261 6d72 4700 0000 7273  archParamrG...rs
-00002ca0: 0000 005a 0854 7970 6541 7267 7372 1c00  ...Z.TypeArgsr..
-00002cb0: 0000 7245 0000 00da 0564 6571 7565 da08  ..rE.....deque..
-00002cc0: 5573 6572 4c69 7374 7281 0000 0072 8600  UserListr....r..
-00002cd0: 0000 725c 0000 0072 8200 0000 da07 5479  ..r\...r......Ty
-00002ce0: 7065 5661 7272 0800 0000 7209 0000 0072  peVarr....r....r
-00002cf0: 7400 0000 720a 0000 0072 4100 0000 720b  t...r....rA...r.
-00002d00: 0000 00da 0850 726f 746f 636f 6c72 0c00  .....Protocolr..
-00002d10: 0000 721a 0000 00da 0341 4243 7203 0000  ..r......ABCr...
-00002d20: 0072 0100 0000 7202 0000 0072 1100 0000  .r....r....r....
-00002d30: 7211 0000 0072 1100 0000 7214 0000 00da  r....r....r.....
-00002d40: 083c 6d6f 6475 6c65 3e01 0000 0073 3a00  .<module>....s:.
-00002d50: 0000 0807 0801 0801 0803 1201 1401 0c01  ................
-00002d60: 0c01 1201 0801 1401 0e01 2001 1001 0401  .......... .....
-00002d70: 0801 0c01 0e01 0a01 0801 0801 0c01 0801  ................
-00002d80: 0e03 1005 1005 107f 0038 0e57            .........8.W
+00000020: 0005 0000 0040 0000 0073 c800 0000 6700  .....@...s....g.
+00000030: 6400 a201 5a00 6401 6402 6c01 5400 6401  d...Z.d.d.l.T.d.
+00000040: 6402 6c02 5400 6401 6402 6c03 5400 6504  d.l.T.d.d.l.T.e.
+00000050: 6505 1900 5a06 6507 6505 6506 6602 1900  e...Z.e.e.e.f...
+00000060: 5a08 6504 6509 650a 650b 650c 6605 5a0d  Z.e.e.e.e.e.f.Z.
+00000070: 650e 650f 6510 6603 5a11 6512 6403 8301  e.e.e.f.Z.e.d...
+00000080: 5a13 6512 6404 8301 5a14 6507 6513 6514  Z.e.d...Z.e.e.e.
+00000090: 6602 1900 5a15 6512 6405 8301 5a16 6512  f...Z.e.d...Z.e.
+000000a0: 6406 6517 6518 6519 8304 5a1a 4700 6407  d.e.e.e...Z.G.d.
+000000b0: 6408 8400 6408 651b 8303 5a1c 4700 6409  d...d.e...Z.G.d.
+000000c0: 640a 8400 640a 651b 8303 5a1d 4700 640b  d...d.e...Z.G.d.
+000000d0: 640c 8400 640c 651e 8303 5a1f 4700 640d  d...d.e...Z.G.d.
+000000e0: 640e 8400 640e 8302 5a20 640f 6410 8400  d...d...Z d.d...
+000000f0: 5a21 6411 5300 2912 2903 da08 5479 7065  Z!d.S.).)...Type
+00000100: 4869 6e74 da06 7061 7273 6572 da06 5061  Hint..parser..Pa
+00000110: 7273 6572 e900 0000 0029 01da 012a da0b  rser.....)...*..
+00000120: 5061 7273 6572 456e 7472 79da 0c50 6172  ParserEntry..Par
+00000130: 7365 7252 6573 756c 74da 0b47 656e 6572  serResult..Gener
+00000140: 6963 5479 7065 da06 4e75 6d62 6572 6300  icType..Numberc.
+00000150: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000160: 0000 0040 0000 0073 2400 0000 6500 5a01  ...@...s$...e.Z.
+00000170: 6400 5a02 6503 6504 6503 6505 6602 1900  d.Z.e.e.e.e.f...
+00000180: 6401 9c02 6402 6403 8404 5a06 6404 5300  d...d.d...Z.d.S.
+00000190: 2905 da0e 5061 7273 6572 5072 6f74 6f63  )...ParserProtoc
+000001a0: 6f6c a902 da05 7661 6c75 65da 0672 6574  ol....value..ret
+000001b0: 7572 6e63 0200 0000 0000 0000 0000 0000  urnc............
+000001c0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000001d0: 0064 0053 00a9 014e a900 a902 da04 7365  .d.S...N......se
+000001e0: 6c66 720c 0000 0072 0f00 0000 720f 0000  lfr....r....r...
+000001f0: 00fa 712f 5573 6572 732f 6461 6e69 656c  ..q/Users/daniel
+00000200: 6172 616e 7465 732f 4c69 6272 6172 792f  arantes/Library/
+00000210: 4d6f 6269 6c65 2044 6f63 756d 656e 7473  Mobile Documents
+00000220: 2f63 6f6d 7e61 7070 6c65 7e43 6c6f 7564  /com~apple~Cloud
+00000230: 446f 6373 2f4d 7920 4170 7073 2f70 7970  Docs/My Apps/pyp
+00000240: 692f 6474 6d6f 6465 6c2f 6474 6d6f 6465  i/dtmodel/dtmode
+00000250: 6c2f 7061 7273 652f 7479 7065 5f68 696e  l/parse/type_hin
+00000260: 742e 7079 da08 5f5f 6361 6c6c 5f5f 2400  t.py..__call__$.
+00000270: 0000 7302 0000 0000 017a 1750 6172 7365  ..s......z.Parse
+00000280: 7250 726f 746f 636f 6c2e 5f5f 6361 6c6c  rProtocol.__call
+00000290: 5f5f 4e29 07da 085f 5f6e 616d 655f 5fda  __N)...__name__.
+000002a0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000002b0: 7561 6c6e 616d 655f 5f72 0600 0000 da05  ualname__r......
+000002c0: 556e 696f 6e72 0700 0000 7213 0000 0072  Unionr....r....r
+000002d0: 0f00 0000 720f 0000 0072 0f00 0000 7212  ....r....r....r.
+000002e0: 0000 0072 0a00 0000 2300 0000 7302 0000  ...r....#...s...
+000002f0: 0008 0172 0a00 0000 6300 0000 0000 0000  ...r....c.......
+00000300: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000310: 0073 1e00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+00000320: 6504 6503 6401 9c03 6402 6403 8404 5a05  e.e.d...d.d...Z.
+00000330: 6404 5300 2905 da11 5661 6c69 6461 746f  d.S.)...Validato
+00000340: 7250 726f 746f 636f 6c29 0372 0c00 0000  rProtocol).r....
+00000350: da05 7479 7065 7372 0d00 0000 6303 0000  ..typesr....c...
+00000360: 0000 0000 0000 0000 0003 0000 0001 0000  ................
+00000370: 0043 0000 0073 0400 0000 6400 5300 720e  .C...s....d.S.r.
+00000380: 0000 0072 0f00 0000 2903 7211 0000 0072  ...r....).r....r
+00000390: 0c00 0000 7219 0000 0072 0f00 0000 720f  ....r....r....r.
+000003a0: 0000 0072 1200 0000 7213 0000 0029 0000  ...r....r....)..
+000003b0: 0073 0200 0000 0001 7a1a 5661 6c69 6461  .s......z.Valida
+000003c0: 746f 7250 726f 746f 636f 6c2e 5f5f 6361  torProtocol.__ca
+000003d0: 6c6c 5f5f 4e29 0672 1400 0000 7215 0000  ll__N).r....r...
+000003e0: 0072 1600 0000 7208 0000 00da 0554 7970  .r....r......Typ
+000003f0: 6573 7213 0000 0072 0f00 0000 720f 0000  esr....r....r...
+00000400: 0072 0f00 0000 7212 0000 0072 1800 0000  .r....r....r....
+00000410: 2800 0000 7302 0000 0008 0172 1800 0000  (...s......r....
+00000420: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000430: 0006 0000 0040 0000 0073 aa01 0000 6500  .....@...s....e.
+00000440: 5a01 6400 5a02 6503 6504 6505 6506 1900  Z.d.Z.e.e.e.e...
+00000450: 6401 9c02 6402 6403 8404 8301 5a07 6503  d...d.d.....Z.e.
+00000460: 6504 6505 6506 1900 6508 6404 9c03 6405  e.e.e...e.d...d.
+00000470: 6406 8404 8301 5a09 6503 6505 6506 1900  d.....Z.e.e.e...
+00000480: 650a 6407 9c02 6408 6409 8404 8301 5a0b  e.d...d.d.....Z.
+00000490: 6503 6504 6505 650c 6505 1900 6508 640a  e.e.e.e.e...e.d.
+000004a0: 9c04 640b 640c 8404 8301 5a0d 6503 6504  ..d.d.....Z.e.e.
+000004b0: 650e 650f 6510 6602 1900 650c 6505 1900  e.e.e.f...e.e...
+000004c0: 6508 640a 9c04 640d 640e 8404 8301 5a11  e.d...d.d.....Z.
+000004d0: 6503 6504 6506 6508 640f 9c03 6410 6411  e.e.e.e.d...d.d.
+000004e0: 8404 8301 5a12 6503 6504 6508 6412 9c02  ....Z.e.e.e.d...
+000004f0: 6413 6414 8404 8301 5a13 6503 6504 6508  d.d.....Z.e.e.e.
+00000500: 6412 9c02 6415 6416 8404 8301 5a14 6503  d...d.d.....Z.e.
+00000510: 6504 6508 6412 9c02 6417 6418 8404 8301  e.e.d...d.d.....
+00000520: 5a15 6503 6504 6508 6412 9c02 6419 641a  Z.e.e.e.d...d.d.
+00000530: 8404 8301 5a16 6503 641b 641c 8400 8301  ....Z.e.d.d.....
+00000540: 5a17 6503 650f 6505 641d 1900 641e 9c02  Z.e.e.e.d...d...
+00000550: 641f 6420 8404 8301 5a18 6503 6421 6422  d.d ....Z.e.d!d"
+00000560: 8400 8301 5a19 6503 6504 6508 6412 9c02  ....Z.e.e.e.d...
+00000570: 6423 6424 8404 8301 5a1a 6503 6504 6505  d#d$....Z.e.e.e.
+00000580: 651b 1900 6508 6425 9c03 6426 6427 8404  e...e.d%..d&d'..
+00000590: 8301 5a1c 6503 6504 6508 6412 9c02 6428  ..Z.e.e.e.d...d(
+000005a0: 6429 8404 8301 5a1d 6503 6504 6508 6412  d)....Z.e.e.e.d.
+000005b0: 9c02 642a 642b 8404 8301 5a1e 6503 6504  ..d*d+....Z.e.e.
+000005c0: 6508 6412 9c02 642c 642d 8404 8301 5a1f  e.d...d,d-....Z.
+000005d0: 6503 6504 6508 6412 9c02 642e 642f 8404  e.e.e.d...d.d/..
+000005e0: 8301 5a20 6430 5300 2931 7203 0000 0029  ..Z d0S.)1r....)
+000005f0: 0272 0c00 0000 da09 6361 7374 5f74 7970  .r......cast_typ
+00000600: 6563 0300 0000 0000 0000 0000 0000 0300  ec..............
+00000610: 0000 0400 0000 4300 0000 730c 0000 007c  ......C...s....|
+00000620: 00a0 007c 017c 02a1 0253 0072 0e00 0000  ...|.|...S.r....
+00000630: 2901 da07 7072 6f63 6573 7329 03da 0363  )...process)...c
+00000640: 6c73 720c 0000 0072 1b00 0000 720f 0000  lsr....r....r...
+00000650: 0072 0f00 0000 7212 0000 00da 0367 6574  .r....r......get
+00000660: 2e00 0000 7302 0000 0000 027a 0a50 6172  ....s......z.Par
+00000670: 7365 722e 6765 7429 0372 0c00 0000 721b  ser.get).r....r.
+00000680: 0000 0072 0d00 0000 6303 0000 0000 0000  ...r....c.......
+00000690: 0000 0000 0005 0000 000a 0000 0043 0000  .............C..
+000006a0: 0073 c600 0000 7400 7c02 8301 7d03 7c03  .s....t.|...}.|.
+000006b0: a001 7c01 a101 7216 7c01 5300 7a7a 7c03  ..|...r.|.S.zz|.
+000006c0: 6a02 724c 7403 7c01 7c02 8302 722e 7c01  j.rLt.|.|...r.|.
+000006d0: 5700 5300 7404 7c01 8301 723c 5700 6401  W.S.t.|...r<W.d.
+000006e0: 5300 7c00 a005 7c02 a101 7c01 8301 5700  S.|...|...|...W.
+000006f0: 5300 7c03 6a06 7266 7c00 a007 7c01 7c03  S.|.j.rf|...|.|.
+00000700: 6a08 7c03 6a09 a103 5700 5300 7c03 6a0a  j.|.j...W.S.|.j.
+00000710: 7280 7c00 a00b 7c01 7c03 6a08 7c03 6a09  r.|...|.|.j.|.j.
+00000720: a103 5700 5300 7c00 a00c 7c01 7c02 a102  ..W.S.|...|.|...
+00000730: 5700 5300 5700 6e30 0400 740d 79c0 0100  W.S.W.n0..t.y...
+00000740: 7d04 0100 7a18 740e 7c04 8301 0100 7c01  }...z.t.|.....|.
+00000750: 5700 0600 5900 6400 7d04 7e04 5300 6400  W...Y.d.}.~.S.d.
+00000760: 7d04 7e04 3000 3000 6400 5300 2902 4eda  }.~.0.0.d.S.).N.
+00000770: 0029 0f72 0100 0000 da0a 6368 6563 6b5f  .).r......check_
+00000780: 7479 7065 da0e 6973 5f73 696d 706c 655f  type..is_simple_
+00000790: 7479 7065 da0a 6973 696e 7374 616e 6365  type..isinstance
+000007a0: da07 6973 5f6e 756c 6cda 0d73 696d 706c  ..is_null..simpl
+000007b0: 655f 656e 6769 6e65 da0b 6973 5f73 6571  e_engine..is_seq
+000007c0: 7565 6e63 65da 0f73 6571 7565 6e63 655f  uence..sequence_
+000007d0: 656e 6769 6e65 da06 6f72 6967 696e da04  engine..origin..
+000007e0: 6172 6773 da0a 6973 5f6d 6170 7069 6e67  args..is_mapping
+000007f0: da0e 6d61 7070 696e 675f 656e 6769 6e65  ..mapping_engine
+00000800: da0e 6765 6e65 7269 635f 656e 6769 6e65  ..generic_engine
+00000810: da0a 5661 6c75 6545 7272 6f72 da05 7072  ..ValueError..pr
+00000820: 696e 7429 0572 1d00 0000 720c 0000 0072  int).r....r....r
+00000830: 1b00 0000 5a0d 6361 7374 5f61 6e61 6c79  ....Z.cast_analy
+00000840: 7369 73da 0165 720f 0000 0072 0f00 0000  sis..er....r....
+00000850: 7212 0000 0072 1c00 0000 3200 0000 7324  r....r....2...s$
+00000860: 0000 0000 0208 010a 0104 0102 0106 010a  ................
+00000870: 0106 0108 0106 0110 0106 0114 0106 0114  ................
+00000880: 0212 010e 0108 017a 0e50 6172 7365 722e  .......z.Parser.
+00000890: 7072 6f63 6573 7329 0272 1b00 0000 720d  process).r....r.
+000008a0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000008b0: 0200 0000 0400 0000 0300 0000 73c4 0000  ............s...
+000008c0: 0088 0074 0075 0072 0e88 016a 0153 0088  ...t.u.r...j.S..
+000008d0: 0074 0275 0072 1c88 016a 0353 0088 0074  .t.u.r...j.S...t
+000008e0: 0475 0072 2a88 016a 0553 0088 0074 066a  .u.r*..j.S...t.j
+000008f0: 0775 0072 3a88 016a 0853 0088 0074 066a  .u.r:..j.S...t.j
+00000900: 0675 0072 4a88 016a 0953 0088 0074 0a75  .u.rJ..j.S...t.u
+00000910: 0072 5888 016a 0b53 0088 0074 0c75 0072  .rX..j.S...t.u.r
+00000920: 6688 016a 0d53 0088 0074 0e75 0072 7488  f..j.S...t.u.rt.
+00000930: 016a 0f53 0088 0074 1075 0072 8288 016a  .j.S...t.u.r...j
+00000940: 1153 0088 0074 1275 0072 9088 016a 1353  .S...t.u.r...j.S
+00000950: 0074 1488 0064 0183 0272 a088 016a 0153  .t...d...r...j.S
+00000960: 0074 1588 0074 1674 1766 0283 0272 bc87  .t...t.t.f...r..
+00000970: 0087 0166 0264 0264 0384 0853 0088 0053  ...f.d.d...S...S
+00000980: 0064 0053 0029 044e 5a06 4354 5856 4152  .d.S.).NZ.CTXVAR
+00000990: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000009a0: 0004 0000 0013 0000 0073 0c00 0000 8801  .........s......
+000009b0: a000 7c00 8800 a102 5300 720e 0000 0029  ..|.....S.r....)
+000009c0: 01da 0b65 6e75 6d5f 656e 6769 6e65 2901  ...enum_engine).
+000009d0: 720c 0000 00a9 0272 1b00 0000 721d 0000  r......r....r...
+000009e0: 0072 0f00 0000 7212 0000 00da 083c 6c61  .r....r......<la
+000009f0: 6d62 6461 3e61 0000 00f3 0000 0000 7a26  mbda>a........z&
+00000a00: 5061 7273 6572 2e73 696d 706c 655f 656e  Parser.simple_en
+00000a10: 6769 6e65 2e3c 6c6f 6361 6c73 3e2e 3c6c  gine.<locals>.<l
+00000a20: 616d 6264 613e 2918 da03 7374 72da 0a73  ambda>)...str..s
+00000a30: 7472 5f65 6e67 696e 65da 0369 6e74 da0a  tr_engine..int..
+00000a40: 696e 745f 656e 6769 6e65 da05 666c 6f61  int_engine..floa
+00000a50: 74da 0c66 6c6f 6174 5f65 6e67 696e 65da  t..float_engine.
+00000a60: 0864 6174 6574 696d 65da 0464 6174 65da  .datetime..date.
+00000a70: 0b64 6174 655f 656e 6769 6e65 da0f 6461  .date_engine..da
+00000a80: 7465 7469 6d65 5f65 6e67 696e 65da 0562  tetime_engine..b
+00000a90: 7974 6573 da0c 6279 7465 735f 656e 6769  ytes..bytes_engi
+00000aa0: 6e65 da07 4465 6369 6d61 6cda 0e64 6563  ne..Decimal..dec
+00000ab0: 696d 616c 5f65 6e67 696e 65da 046c 6973  imal_engine..lis
+00000ac0: 74da 0b6c 6973 745f 656e 6769 6e65 da03  t..list_engine..
+00000ad0: 7365 74da 0a73 6574 5f65 6e67 696e 65da  set..set_engine.
+00000ae0: 0574 7570 6c65 da0c 7475 706c 655f 656e  .tuple..tuple_en
+00000af0: 6769 6e65 da07 6861 7361 7474 72da 0a69  gine..hasattr..i
+00000b00: 7373 7562 636c 6173 73da 0842 6173 6545  ssubclass..BaseE
+00000b10: 6e75 6dda 0445 6e75 6d29 0272 1d00 0000  num..Enum).r....
+00000b20: 721b 0000 0072 0f00 0000 7230 0000 0072  r....r....r0...r
+00000b30: 1200 0000 7224 0000 0048 0000 0073 3200  ....r$...H...s2.
+00000b40: 0000 0002 0801 0601 0801 0601 0801 0601  ................
+00000b50: 0a01 0601 0a01 0601 0801 0601 0801 0601  ................
+00000b60: 0801 0601 0801 0601 0801 0601 0a01 0601  ................
+00000b70: 0e01 0e02 7a14 5061 7273 6572 2e73 696d  ....z.Parser.sim
+00000b80: 706c 655f 656e 6769 6e65 2904 720c 0000  ple_engine).r...
+00000b90: 0072 2700 0000 7228 0000 0072 0d00 0000  .r'...r(...r....
+00000ba0: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00000bb0: 0006 0000 0003 0000 0073 8e00 0000 7c02  .........s....|.
+00000bc0: 7400 7500 7240 7401 7c01 7400 7402 7403  t.u.r@t.|.t.t.t.
+00000bd0: 6603 8302 722c 8700 8701 6602 6401 6402  f...r,....f.d.d.
+00000be0: 8408 7c01 4400 8301 5300 8801 a004 7c01  ..|.D...S.....|.
+00000bf0: 8800 6403 1900 a102 6701 5300 6e4a 7c02  ..d.....g.S.nJ|.
+00000c00: 7403 7402 6602 7600 728a 7401 7c01 7400  t.t.f.v.r.t.|.t.
+00000c10: 7402 7403 6603 8302 7274 7c02 8700 8701  t.t.f...rt|.....
+00000c20: 6602 6404 6402 8408 7c01 4400 8301 8301  f.d.d...|.D.....
+00000c30: 5300 7c02 8801 a004 7c01 8800 6403 1900  S.|.....|...d...
+00000c40: a102 6701 8301 5300 6400 5300 2905 4e63  ..g...S.d.S.).Nc
+00000c50: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000c60: 0700 0000 1300 0000 731c 0000 0067 007c  ........s....g.|
+00000c70: 005d 147d 0188 01a0 007c 0188 0064 0019  .].}.....|...d..
+00000c80: 00a1 0291 0271 0453 00a9 0172 0400 0000  .....q.S...r....
+00000c90: a901 721e 0000 00a9 02da 022e 30da 0469  ..r.........0..i
+00000ca0: 7465 6da9 0272 2800 0000 721d 0000 0072  tem..r(...r....r
+00000cb0: 0f00 0000 7212 0000 00da 0a3c 6c69 7374  ....r......<list
+00000cc0: 636f 6d70 3e69 0000 0072 3200 0000 7a2a  comp>i...r2...z*
+00000cd0: 5061 7273 6572 2e73 6571 7565 6e63 655f  Parser.sequence_
+00000ce0: 656e 6769 6e65 2e3c 6c6f 6361 6c73 3e2e  engine.<locals>.
+00000cf0: 3c6c 6973 7463 6f6d 703e 7204 0000 0063  <listcomp>r....c
+00000d00: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000d10: 0700 0000 1300 0000 731c 0000 0067 007c  ........s....g.|
+00000d20: 005d 147d 0188 01a0 007c 0188 0064 0019  .].}.....|...d..
+00000d30: 00a1 0291 0271 0453 0072 4b00 0000 724c  .....q.S.rK...rL
+00000d40: 0000 0072 4d00 0000 7250 0000 0072 0f00  ...rM...rP...r..
+00000d50: 0000 7212 0000 0072 5100 0000 6e00 0000  ..r....rQ...n...
+00000d60: 7232 0000 0029 0572 4100 0000 7222 0000  r2...).rA...r"..
+00000d70: 0072 4500 0000 7243 0000 0072 1e00 0000  .rE...rC...r....
+00000d80: a904 721d 0000 0072 0c00 0000 7227 0000  ..r....r....r'..
+00000d90: 0072 2800 0000 720f 0000 0072 5000 0000  .r(...r....rP...
+00000da0: 7212 0000 0072 2600 0000 6500 0000 7310  r....r&...e...s.
+00000db0: 0000 0000 0208 0110 0114 0214 010c 0110  ................
+00000dc0: 0118 027a 1650 6172 7365 722e 7365 7175  ...z.Parser.sequ
+00000dd0: 656e 6365 5f65 6e67 696e 6563 0400 0000  ence_enginec....
+00000de0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000df0: 0300 0000 7366 0000 007c 0274 0075 0072  ....sf...|.t.u.r
+00000e00: 3074 017c 0174 0274 0066 0283 0272 6287  0t.|.t.t.f...rb.
+00000e10: 0087 0166 0264 0164 0284 087c 01a0 03a1  ...f.d.d...|....
+00000e20: 0044 0083 0153 006e 327c 0274 0275 0072  .D...S.n2|.t.u.r
+00000e30: 6274 017c 0174 0274 0066 0283 0272 6274  bt.|.t.t.f...rbt
+00000e40: 0287 0087 0166 0264 0364 0284 087c 01a0  .....f.d.d...|..
+00000e50: 03a1 0044 0083 0183 0153 0064 0053 0029  ...D.....S.d.S.)
+00000e60: 044e 6301 0000 0000 0000 0000 0000 0003  .Nc.............
+00000e70: 0000 0008 0000 0013 0000 0073 2e00 0000  ...........s....
+00000e80: 6900 7c00 5d26 5c02 7d01 7d02 8801 a000  i.|.]&\.}.}.....
+00000e90: 7c01 8800 6400 1900 a102 8801 a000 7c02  |...d.........|.
+00000ea0: 8800 6401 1900 a102 9302 7104 5300 a902  ..d.......q.S...
+00000eb0: 7204 0000 00e9 ffff ffff 724c 0000 00a9  r.........rL....
+00000ec0: 0372 4e00 0000 da01 6bda 0176 7250 0000  .rN.....k..vrP..
+00000ed0: 0072 0f00 0000 7212 0000 00da 0a3c 6469  .r....r......<di
+00000ee0: 6374 636f 6d70 3e76 0000 0072 3200 0000  ctcomp>v...r2...
+00000ef0: 7a29 5061 7273 6572 2e6d 6170 7069 6e67  z)Parser.mapping
+00000f00: 5f65 6e67 696e 652e 3c6c 6f63 616c 733e  _engine.<locals>
+00000f10: 2e3c 6469 6374 636f 6d70 3e63 0100 0000  .<dictcomp>c....
+00000f20: 0000 0000 0000 0000 0300 0000 0800 0000  ................
+00000f30: 1300 0000 732e 0000 0069 007c 005d 265c  ....s....i.|.]&\
+00000f40: 027d 017d 0288 01a0 007c 0188 0064 0019  .}.}.....|...d..
+00000f50: 00a1 0288 01a0 007c 0288 0064 0119 00a1  .......|...d....
+00000f60: 0293 0271 0453 0072 5300 0000 724c 0000  ...q.S.rS...rL..
+00000f70: 0072 5500 0000 7250 0000 0072 0f00 0000  .rU...rP...r....
+00000f80: 7212 0000 0072 5800 0000 7900 0000 7232  r....rX...y...r2
+00000f90: 0000 0029 04da 0464 6963 7472 2200 0000  ...)...dictr"...
+00000fa0: da08 4368 6169 6e4d 6170 da05 6974 656d  ..ChainMap..item
+00000fb0: 7372 5200 0000 720f 0000 0072 5000 0000  srR...r....rP...
+00000fc0: 7212 0000 0072 2a00 0000 7200 0000 730c  r....r*...r...s.
+00000fd0: 0000 0000 0208 010e 011a 0108 010e 017a  ...............z
+00000fe0: 1550 6172 7365 722e 6d61 7070 696e 675f  .Parser.mapping_
+00000ff0: 656e 6769 6e65 2903 720c 0000 00da 0767  engine).r......g
+00001000: 656e 6572 6963 720d 0000 0063 0300 0000  enericr....c....
+00001010: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00001020: 4300 0000 7316 0000 007c 0274 0075 0072  C...s....|.t.u.r
+00001030: 127c 00a0 017c 01a1 0153 0064 0053 0072  .|...|...S.d.S.r
+00001040: 0e00 0000 2902 7209 0000 00da 0d6e 756d  ....).r......num
+00001050: 6265 725f 656e 6769 6e65 2903 721d 0000  ber_engine).r...
+00001060: 0072 0c00 0000 725c 0000 0072 0f00 0000  .r....r\...r....
+00001070: 720f 0000 0072 1200 0000 722b 0000 007b  r....r....r+...{
+00001080: 0000 0073 0400 0000 0002 0801 7a15 5061  ...s........z.Pa
+00001090: 7273 6572 2e67 656e 6572 6963 5f65 6e67  rser.generic_eng
+000010a0: 696e 6572 0b00 0000 6302 0000 0000 0000  iner....c.......
+000010b0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000010c0: 0073 2a00 0000 7400 7c01 7401 7402 6602  .s*...t.|.t.t.f.
+000010d0: 8302 7216 6700 7c01 a201 5300 7400 7c01  ..r.g.|...S.t.|.
+000010e0: 7403 8302 7224 7c01 5300 7c01 6701 5300  t...r$|.S.|.g.S.
+000010f0: 720e 0000 0029 0472 2200 0000 7243 0000  r....).r"...rC..
+00001100: 0072 4500 0000 7241 0000 00a9 0272 1d00  .rE...rA.....r..
+00001110: 0000 720c 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00001120: 0072 1200 0000 7242 0000 0080 0000 0073  .r....rB.......s
+00001130: 0600 0000 0002 0e01 0801 7a12 5061 7273  ..........z.Pars
+00001140: 6572 2e6c 6973 745f 656e 6769 6e65 6302  er.list_enginec.
+00001150: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001160: 0000 0043 0000 0073 2a00 0000 7400 7c01  ...C...s*...t.|.
+00001170: 7401 7402 6602 8302 7216 6900 7c01 a501  t.t.f...r.i.|...
+00001180: 5300 7400 7c01 7403 8302 7224 7c01 5300  S.t.|.t...r$|.S.
+00001190: 7c01 6801 5300 720e 0000 0029 0472 2200  |.h.S.r....).r".
+000011a0: 0000 7241 0000 0072 4500 0000 7243 0000  ..rA...rE...rC..
+000011b0: 0072 5e00 0000 720f 0000 0072 0f00 0000  .r^...r....r....
+000011c0: 7212 0000 0072 4400 0000 8600 0000 7306  r....rD.......s.
+000011d0: 0000 0000 020e 0108 017a 1150 6172 7365  .........z.Parse
+000011e0: 722e 7365 745f 656e 6769 6e65 6302 0000  r.set_enginec...
+000011f0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00001200: 0043 0000 0073 3200 0000 7400 7c01 7401  .C...s2...t.|.t.
+00001210: 7402 6602 8302 721a 7403 6700 7c01 a201  t.f...r.t.g.|...
+00001220: 8301 5300 7400 7c01 7403 8302 7228 7c01  ..S.t.|.t...r(|.
+00001230: 5300 7403 7c01 6701 8301 5300 720e 0000  S.t.|.g...S.r...
+00001240: 0029 0472 2200 0000 7241 0000 0072 4300  .).r"...rA...rC.
+00001250: 0000 7245 0000 0072 5e00 0000 720f 0000  ..rE...r^...r...
+00001260: 0072 0f00 0000 7212 0000 0072 4600 0000  .r....r....rF...
+00001270: 8c00 0000 7306 0000 0000 020e 010c 017a  ....s..........z
+00001280: 1350 6172 7365 722e 7475 706c 655f 656e  .Parser.tuple_en
+00001290: 6769 6e65 6302 0000 0000 0000 0000 0000  ginec...........
+000012a0: 0002 0000 0002 0000 0043 0000 0073 0800  .........C...s..
+000012b0: 0000 7400 7c01 8301 5300 720e 0000 0029  ..t.|...S.r....)
+000012c0: 0172 3300 0000 725e 0000 0072 0f00 0000  .r3...r^...r....
+000012d0: 720f 0000 0072 1200 0000 7234 0000 0092  r....r....r4....
+000012e0: 0000 0073 0200 0000 0002 7a11 5061 7273  ...s......z.Pars
+000012f0: 6572 2e73 7472 5f65 6e67 696e 6563 0200  er.str_enginec..
+00001300: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00001310: 0000 4300 0000 7356 0000 0074 007c 0174  ..C...sV...t.|.t
+00001320: 0183 0272 2674 0274 0374 04a0 0564 0164  ...r&t.t.t...d.d
+00001330: 027c 01a1 0383 01a0 0664 03a1 0183 0153  .|.......d.....S
+00001340: 0074 007c 0174 0783 0272 3874 027c 0183  .t.|.t...r8t.|..
+00001350: 0153 0074 007c 0174 086a 0974 086a 0866  .S.t.|.t.j.t.j.f
+00001360: 0283 0272 527c 01a0 0aa1 0053 007c 0153  ...rR|.....S.|.S
+00001370: 0029 044e fa01 2cda 012e 7204 0000 0029  .).N..,...r....)
+00001380: 0b72 2200 0000 7233 0000 0072 3500 0000  .r"...r3...r5...
+00001390: 7237 0000 00da 0272 65da 0373 7562 da09  r7.....re..sub..
+000013a0: 5f5f 726f 756e 645f 5f72 3f00 0000 7239  __round__r?...r9
+000013b0: 0000 0072 3a00 0000 da09 746f 6f72 6469  ...r:.....toordi
+000013c0: 6e61 6c72 5e00 0000 720f 0000 0072 0f00  nalr^...r....r..
+000013d0: 0000 7212 0000 0072 3600 0000 9600 0000  ..r....r6.......
+000013e0: 730e 0000 0000 020a 011c 010a 0108 0112  s...............
+000013f0: 0108 017a 1150 6172 7365 722e 696e 745f  ...z.Parser.int_
+00001400: 656e 6769 6e65 5a05 4d6f 6465 6c29 0272  engineZ.Model).r
+00001410: 0c00 0000 da0a 6d6f 6465 6c5f 7479 7065  ......model_type
+00001420: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00001430: 0004 0000 0043 0000 0073 1000 0000 7c02  .....C...s....|.
+00001440: 6a00 6600 6900 7c01 a401 8e01 5300 720e  j.f.i.|.....S.r.
+00001450: 0000 0029 01da 0b73 6166 655f 6372 6561  ...)...safe_crea
+00001460: 7465 2903 721d 0000 0072 0c00 0000 7265  te).r....r....re
+00001470: 0000 0072 0f00 0000 720f 0000 0072 1200  ...r....r....r..
+00001480: 0000 da0d 636f 6e74 6578 745f 6d6f 6465  ....context_mode
+00001490: 6ca0 0000 0073 0200 0000 0002 7a14 5061  l....s......z.Pa
+000014a0: 7273 6572 2e63 6f6e 7465 7874 5f6d 6f64  rser.context_mod
+000014b0: 656c 6302 0000 0000 0000 0000 0000 0002  elc.............
+000014c0: 0000 0008 0000 0043 0000 0073 6600 0000  .......C...sf...
+000014d0: 7400 7c01 7401 8302 721c 7402 7403 a004  t.|.t...r.t.t...
+000014e0: 6401 6402 7c01 a103 8301 5300 7400 7c01  d.d.|.....S.t.|.
+000014f0: 7405 8302 722e 7402 7c01 8301 5300 7400  t...r.t.|...S.t.
+00001500: 7c01 7406 8302 7240 7402 7c01 8301 5300  |.t...r@t.|...S.
+00001510: 7400 7c01 7407 8302 7262 7402 7403 a004  t.|.t...rbt.t...
+00001520: 6401 6402 7c01 a008 6403 a101 a103 8301  d.d.|...d.......
+00001530: 5300 7c01 5300 2904 4e72 5f00 0000 7260  S.|.S.).Nr_...r`
+00001540: 0000 00fa 0575 7466 2d38 2909 7222 0000  .....utf-8).r"..
+00001550: 0072 3300 0000 7237 0000 0072 6100 0000  .r3...r7...ra...
+00001560: 7262 0000 0072 3500 0000 723f 0000 0072  rb...r5...r?...r
+00001570: 3d00 0000 da06 6465 636f 6465 725e 0000  =.....decoder^..
+00001580: 0072 0f00 0000 720f 0000 0072 1200 0000  .r....r....r....
+00001590: 7238 0000 00a4 0000 0073 1200 0000 0002  r8.......s......
+000015a0: 0a01 1201 0a01 0801 0a01 0801 0a01 1801  ................
+000015b0: 7a13 5061 7273 6572 2e66 6c6f 6174 5f65  z.Parser.float_e
+000015c0: 6e67 696e 6563 0200 0000 0000 0000 0000  nginec..........
+000015d0: 0000 0200 0000 0300 0000 4300 0000 7344  ..........C...sD
+000015e0: 0000 0074 007c 0174 0183 0272 1674 026a  ...t.|.t...r.t.j
+000015f0: 03a0 047c 01a1 0153 0074 007c 0174 026a  ...|...S.t.|.t.j
+00001600: 0283 0272 2a7c 01a0 03a1 0053 0074 007c  ...r*|.....S.t.|
+00001610: 0174 0583 0272 4074 026a 03a0 067c 01a1  .t...r@t.j...|..
+00001620: 0153 0064 0053 0072 0e00 0000 2907 7222  .S.d.S.r....).r"
+00001630: 0000 0072 3300 0000 7239 0000 0072 3a00  ...r3...r9...r:.
+00001640: 0000 da0d 6672 6f6d 6973 6f66 6f72 6d61  ....fromisoforma
+00001650: 7472 3500 0000 da0b 6672 6f6d 6f72 6469  tr5.....fromordi
+00001660: 6e61 6c72 5e00 0000 720f 0000 0072 0f00  nalr^...r....r..
+00001670: 0000 7212 0000 0072 3b00 0000 b000 0000  ..r....r;.......
+00001680: 730c 0000 0000 020a 010c 010c 0108 010a  s...............
+00001690: 017a 1250 6172 7365 722e 6461 7465 5f65  .z.Parser.date_e
+000016a0: 6e67 696e 6529 0372 0c00 0000 da09 656e  ngine).r......en
+000016b0: 756d 5f74 7970 6572 0d00 0000 6303 0000  um_typer....c...
+000016c0: 0000 0000 0000 0000 0004 0000 000a 0000  ................
+000016d0: 0043 0000 0073 4400 0000 7a0a 7c02 7c01  .C...sD...z.|.|.
+000016e0: 1900 5700 5300 0400 7400 793e 0100 7d03  ..W.S...t.y>..}.
+000016f0: 0100 7a1c 7401 7c03 8301 0100 7c02 7c01  ..z.t.|.....|.|.
+00001700: 8301 5700 0600 5900 6400 7d03 7e03 5300  ..W...Y.d.}.~.S.
+00001710: 6400 7d03 7e03 3000 3000 6400 5300 720e  d.}.~.0.0.d.S.r.
+00001720: 0000 0029 02da 0d42 6173 6545 7863 6570  ...)...BaseExcep
+00001730: 7469 6f6e 722d 0000 0029 0472 1d00 0000  tionr-...).r....
+00001740: 720c 0000 0072 6c00 0000 722e 0000 0072  r....rl...r....r
+00001750: 0f00 0000 720f 0000 0072 1200 0000 722f  ....r....r....r/
+00001760: 0000 00b9 0000 0073 0a00 0000 0002 0201  .......s........
+00001770: 0a01 0e01 0801 7a12 5061 7273 6572 2e65  ......z.Parser.e
+00001780: 6e75 6d5f 656e 6769 6e65 6302 0000 0000  num_enginec.....
+00001790: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000017a0: 0000 0073 4c00 0000 7400 7c01 7401 8302  ...sL...t.|.t...
+000017b0: 7216 7402 6a02 a003 7c01 a101 5300 7400  r.t.j...|...S.t.
+000017c0: 7c01 7402 6a04 8302 7232 7402 6a02 a005  |.t.j...r2t.j...
+000017d0: 7c01 a006 a100 a101 5300 7400 7c01 7407  |.......S.t.|.t.
+000017e0: 8302 7248 7402 6a02 a005 7c01 a101 5300  ..rHt.j...|...S.
+000017f0: 6400 5300 720e 0000 0029 0872 2200 0000  d.S.r....).r"...
+00001800: 7233 0000 0072 3900 0000 726a 0000 0072  r3...r9...rj...r
+00001810: 3a00 0000 726b 0000 0072 6400 0000 7235  :...rk...rd...r5
+00001820: 0000 0072 5e00 0000 720f 0000 0072 0f00  ...r^...r....r..
+00001830: 0000 7212 0000 0072 3c00 0000 c100 0000  ..r....r<.......
+00001840: 730c 0000 0000 020a 010c 010c 0110 010a  s...............
+00001850: 017a 1650 6172 7365 722e 6461 7465 7469  .z.Parser.dateti
+00001860: 6d65 5f65 6e67 696e 6563 0200 0000 0000  me_enginec......
+00001870: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00001880: 0000 730e 0000 0074 007c 0183 01a0 0164  ..s....t.|.....d
+00001890: 01a1 0153 0029 024e 7268 0000 0029 0272  ...S.).Nrh...).r
+000018a0: 3300 0000 da06 656e 636f 6465 725e 0000  3.....encoder^..
+000018b0: 0072 0f00 0000 720f 0000 0072 1200 0000  .r....r....r....
+000018c0: 723e 0000 00ca 0000 0073 0200 0000 0002  r>.......s......
+000018d0: 7a13 5061 7273 6572 2e62 7974 6573 5f65  z.Parser.bytes_e
+000018e0: 6e67 696e 6563 0200 0000 0000 0000 0000  nginec..........
+000018f0: 0000 0200 0000 0600 0000 4300 0000 7350  ..........C...sP
+00001900: 0000 0074 007c 0174 0183 0272 1c74 0274  ...t.|.t...r.t.t
+00001910: 03a0 0464 0164 027c 01a1 0383 0153 0074  ...d.d.|.....S.t
+00001920: 007c 0174 0583 0272 3274 0274 017c 0183  .|.t...r2t.t.|..
+00001930: 0183 0153 0074 007c 0174 0683 0272 4c74  ...S.t.|.t...rLt
+00001940: 0274 0174 057c 0183 0183 0183 0153 0064  .t.t.|.......S.d
+00001950: 0053 0029 034e fa03 5c2e 2c72 6000 0000  .S.).N..\.,r`...
+00001960: 2907 7222 0000 0072 3300 0000 723f 0000  ).r"...r3...r?..
+00001970: 0072 6100 0000 7262 0000 0072 3700 0000  .ra...rb...r7...
+00001980: 7235 0000 0072 5e00 0000 720f 0000 0072  r5...r^...r....r
+00001990: 0f00 0000 7212 0000 0072 4000 0000 ce00  ....r....r@.....
+000019a0: 0000 730c 0000 0000 020a 0112 010a 010c  ..s.............
+000019b0: 010a 017a 1550 6172 7365 722e 6465 6369  ...z.Parser.deci
+000019c0: 6d61 6c5f 656e 6769 6e65 6302 0000 0000  mal_enginec.....
+000019d0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000019e0: 0000 0073 4e00 0000 7400 7c01 7401 8302  ...sN...t.|.t...
+000019f0: 7230 7402 a003 6401 7c01 a102 7222 7c00  r0t...d.|...r"|.
+00001a00: a004 7c01 7405 a102 5300 7c00 a004 7c01  ..|.t...S.|...|.
+00001a10: 7406 a102 5300 6e1a 7400 7c01 7407 6a08  t...S.n.t.|.t.j.
+00001a20: 7407 6a07 6602 8302 724a 7c01 a009 a100  t.j.f...rJ|.....
+00001a30: 5300 6400 5300 2902 4e72 6f00 0000 290a  S.d.S.).Nro...).
+00001a40: 7222 0000 0072 3300 0000 7261 0000 00da  r"...r3...ra....
+00001a50: 056d 6174 6368 721e 0000 0072 3700 0000  .matchr....r7...
+00001a60: 7235 0000 0072 3900 0000 723a 0000 0072  r5...r9...r:...r
+00001a70: 6400 0000 725e 0000 0072 0f00 0000 720f  d...r^...r....r.
+00001a80: 0000 0072 1200 0000 725d 0000 00d7 0000  ...r....r]......
+00001a90: 0073 0c00 0000 0002 0a01 0c01 0c02 0e01  .s..............
+00001aa0: 1201 7a14 5061 7273 6572 2e6e 756d 6265  ..z.Parser.numbe
+00001ab0: 725f 656e 6769 6e65 4e29 2172 1400 0000  r_engineN)!r....
+00001ac0: 7215 0000 0072 1600 0000 da0b 636c 6173  r....r......clas
+00001ad0: 736d 6574 686f 6472 0600 0000 da04 7479  smethodr......ty
+00001ae0: 7065 7207 0000 0072 1e00 0000 da0c 5061  per....r......Pa
+00001af0: 7273 6572 5265 7475 726e 721c 0000 0072  rserReturnr....r
+00001b00: 0a00 0000 7224 0000 0072 4500 0000 7226  ....r$...rE...r&
+00001b10: 0000 0072 1700 0000 7259 0000 0072 5a00  ...r....rY...rZ.
+00001b20: 0000 722a 0000 0072 2b00 0000 7242 0000  ..r*...r+...rB..
+00001b30: 0072 4400 0000 7246 0000 0072 3400 0000  .rD...rF...r4...
+00001b40: 7236 0000 0072 6700 0000 7238 0000 0072  r6...rg...r8...r
+00001b50: 3b00 0000 7249 0000 0072 2f00 0000 723c  ;...rI...r/...r<
+00001b60: 0000 0072 3e00 0000 7240 0000 0072 5d00  ...r>...r@...r].
+00001b70: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00001b80: 0072 1200 0000 7203 0000 002d 0000 0073  .r....r....-...s
+00001b90: 4c00 0000 0801 0201 1603 0201 1815 0201  L...............
+00001ba0: 161c 0201 1a0c 0201 2208 0201 1404 0201  ........".......
+00001bb0: 1205 0201 1205 0201 1205 0201 1203 0201  ................
+00001bc0: 0a09 0201 1603 0201 0a0b 0201 1208 0201  ................
+00001bd0: 1807 0201 1208 0201 1203 0201 1208 0201  ................
+00001be0: 7203 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00001bf0: 0000 0000 0000 0400 0000 4000 0000 73dc  ..........@...s.
+00001c00: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00001c10: 005a 0364 0364 0484 005a 0465 0565 0665  .Z.d.d...Z.e.e.e
+00001c20: 0719 0064 059c 0164 0664 0784 0483 015a  ...d...d.d.....Z
+00001c30: 0865 0564 0864 0984 0083 015a 0965 0564  .e.d.d.....Z.e.d
+00001c40: 0a64 0b84 0083 015a 0a65 0564 0c64 0d84  .d.....Z.e.d.d..
+00001c50: 0083 015a 0b65 0564 0e64 0f84 0083 015a  ...Z.e.d.d.....Z
+00001c60: 0c65 0564 1064 1184 0083 015a 0d65 0565  .e.d.d.....Z.e.e
+00001c70: 0e64 059c 0164 1264 1384 0483 015a 0f65  .d...d.d.....Z.e
+00001c80: 0564 1464 1584 0083 015a 1065 0564 1664  .d.d.....Z.e.d.d
+00001c90: 1784 0083 015a 1165 0564 1864 1984 0083  .....Z.e.d.d....
+00001ca0: 015a 1265 0564 1a64 1b84 0083 015a 1365  .Z.e.d.d.....Z.e
+00001cb0: 0564 1c64 1d84 0083 015a 1465 1565 0e64  .d.d.....Z.e.e.d
+00001cc0: 1e9c 0264 1f64 2084 045a 1665 1765 1864  ...d.d ..Z.e.e.d
+00001cd0: 1e9c 0264 2164 2284 045a 1964 2353 0029  ...d!d"..Z.d#S.)
+00001ce0: 2472 0100 0000 6302 0000 0000 0000 0000  $r....c.........
+00001cf0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00001d00: 0a00 0000 7c01 7c00 5f00 6400 5300 720e  ....|.|._.d.S.r.
+00001d10: 0000 0029 01da 0974 7970 655f 6869 6e74  ...)...type_hint
+00001d20: 2902 7211 0000 0072 7400 0000 720f 0000  ).r....rt...r...
+00001d30: 0072 0f00 0000 7212 0000 00da 085f 5f69  .r....r......__i
+00001d40: 6e69 745f 5fe5 0000 0073 0200 0000 0001  nit__....s......
+00001d50: 7a11 5479 7065 4869 6e74 2e5f 5f69 6e69  z.TypeHint.__ini
+00001d60: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00001d70: 0100 0000 0400 0000 4300 0000 7318 0000  ........C...s...
+00001d80: 0074 007c 0083 016a 019b 0064 017c 006a  .t.|...j...d.|.j
+00001d90: 029b 0064 029d 0453 0029 034e fa01 28fa  ...d...S.).N..(.
+00001da0: 0129 2903 7272 0000 0072 1400 0000 7274  .)).rr...r....rt
+00001db0: 0000 00a9 0172 1100 0000 720f 0000 0072  .....r....r....r
+00001dc0: 0f00 0000 7212 0000 00da 075f 5f73 7472  ....r......__str
+00001dd0: 5f5f e800 0000 7302 0000 0000 017a 1054  __....s......z.T
+00001de0: 7970 6548 696e 742e 5f5f 7374 725f 5f29  ypeHint.__str__)
+00001df0: 0172 0d00 0000 6301 0000 0000 0000 0000  .r....c.........
+00001e00: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00001e10: 1800 0000 7400 6401 6402 8400 7401 7c00  ....t.d.d...t.|.
+00001e20: 6a02 8301 4400 8301 8301 5300 2903 4e63  j...D.....S.).Nc
+00001e30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001e40: 0500 0000 5300 0000 7326 0000 0067 007c  ....S...s&...g.|
+00001e50: 005d 1e7d 0174 007c 0174 0183 0272 047c  .].}.t.|.t...r.|
+00001e60: 0174 0164 0083 0175 0172 047c 0191 0271  .t.d...u.r.|...q
+00001e70: 0453 0072 0e00 0000 a902 7222 0000 0072  .S.r......r"...r
+00001e80: 7200 0000 2902 724e 0000 00da 0174 720f  r...).rN.....tr.
+00001e90: 0000 0072 0f00 0000 7212 0000 0072 5100  ...r....r....rQ.
+00001ea0: 0000 ed00 0000 7232 0000 007a 2154 7970  ......r2...z!Typ
+00001eb0: 6548 696e 742e 6172 6773 2e3c 6c6f 6361  eHint.args.<loca
+00001ec0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2903  ls>.<listcomp>).
+00001ed0: 7245 0000 00da 0867 6574 5f61 7267 7372  rE.....get_argsr
+00001ee0: 7400 0000 7278 0000 0072 0f00 0000 720f  t...rx...r....r.
+00001ef0: 0000 0072 1200 0000 7228 0000 00eb 0000  ...r....r(......
+00001f00: 0073 0200 0000 0002 7a0d 5479 7065 4869  .s......z.TypeHi
+00001f10: 6e74 2e61 7267 7363 0100 0000 0000 0000  nt.argsc........
+00001f20: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00001f30: 7314 0000 0074 0064 0164 0284 007c 006a  s....t.d.d...|.j
+00001f40: 0144 0083 0183 0153 0029 034e 6301 0000  .D.....S.).Nc...
+00001f50: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001f60: 0053 0000 0073 1800 0000 6700 7c00 5d10  .S...s....g.|.].
+00001f70: 7d01 7400 7c01 7401 8302 0c00 9102 7104  }.t.|.t.......q.
+00001f80: 5300 720f 0000 0072 7a00 0000 724d 0000  S.r....rz...rM..
+00001f90: 0072 0f00 0000 720f 0000 0072 1200 0000  .r....r....r....
+00001fa0: 7251 0000 00f1 0000 0072 3200 0000 7a2c  rQ.......r2...z,
+00001fb0: 5479 7065 4869 6e74 2e69 735f 6172 6773  TypeHint.is_args
+00001fc0: 5f67 656e 6572 6963 2e3c 6c6f 6361 6c73  _generic.<locals
+00001fd0: 3e2e 3c6c 6973 7463 6f6d 703e 2902 da03  >.<listcomp>)...
+00001fe0: 616c 6c72 2800 0000 7278 0000 0072 0f00  allr(...rx...r..
+00001ff0: 0000 720f 0000 0072 1200 0000 da0f 6973  ..r....r......is
+00002000: 5f61 7267 735f 6765 6e65 7269 63ef 0000  _args_generic...
+00002010: 0073 0200 0000 0002 7a18 5479 7065 4869  .s......z.TypeHi
+00002020: 6e74 2e69 735f 6172 6773 5f67 656e 6572  nt.is_args_gener
+00002030: 6963 6301 0000 0000 0000 0000 0000 0001  icc.............
+00002040: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00002050: 7400 7c00 6a01 8301 5300 720e 0000 0029  t.|.j...S.r....)
+00002060: 02da 0a67 6574 5f6f 7269 6769 6e72 7400  ...get_originrt.
+00002070: 0000 7278 0000 0072 0f00 0000 720f 0000  ..rx...r....r...
+00002080: 0072 1200 0000 7227 0000 00f3 0000 0073  .r....r'.......s
+00002090: 0200 0000 0002 7a0f 5479 7065 4869 6e74  ......z.TypeHint
+000020a0: 2e6f 7269 6769 6e63 0100 0000 0000 0000  .originc........
+000020b0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000020c0: 730a 0000 007c 006a 0074 0176 0053 0072  s....|.j.t.v.S.r
+000020d0: 0e00 0000 2902 7227 0000 00da 1254 7570  ....).r'.....Tup
+000020e0: 6c65 5365 7175 656e 6365 5479 7065 7372  leSequenceTypesr
+000020f0: 7800 0000 720f 0000 0072 0f00 0000 7212  x...r....r....r.
+00002100: 0000 0072 2500 0000 f700 0000 7302 0000  ...r%.......s...
+00002110: 0000 027a 1454 7970 6548 696e 742e 6973  ...z.TypeHint.is
+00002120: 5f73 6571 7565 6e63 6563 0100 0000 0000  _sequencec......
+00002130: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00002140: 0000 730a 0000 007c 006a 0074 0176 0053  ..s....|.j.t.v.S
+00002150: 0072 0e00 0000 2902 7227 0000 00da 0d54  .r....).r'.....T
+00002160: 7570 6c65 4d61 7054 7970 6573 7278 0000  upleMapTypesrx..
+00002170: 0072 0f00 0000 720f 0000 0072 1200 0000  .r....r....r....
+00002180: 7229 0000 00fb 0000 0073 0200 0000 0002  r).......s......
+00002190: 7a13 5479 7065 4869 6e74 2e69 735f 6d61  z.TypeHint.is_ma
+000021a0: 7070 696e 6763 0100 0000 0000 0000 0000  ppingc..........
+000021b0: 0000 0100 0000 0300 0000 4300 0000 730e  ..........C...s.
+000021c0: 0000 0074 007c 006a 0174 0283 020c 0053  ...t.|.j.t.....S
+000021d0: 0072 0e00 0000 2903 7222 0000 0072 2700  .r....).r"...r'.
+000021e0: 0000 7272 0000 0072 7800 0000 720f 0000  ..rr...rx...r...
+000021f0: 0072 0f00 0000 7212 0000 00da 0a69 735f  .r....r......is_
+00002200: 6765 6e65 7269 63ff 0000 0073 0200 0000  generic....s....
+00002210: 0002 7a13 5479 7065 4869 6e74 2e69 735f  ..z.TypeHint.is_
+00002220: 6765 6e65 7269 6363 0100 0000 0000 0000  genericc........
+00002230: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00002240: 7314 0000 007c 006a 000c 006f 1274 017c  s....|.j...o.t.|
+00002250: 006a 0274 0383 0253 0072 0e00 0000 2904  .j.t...S.r....).
+00002260: 7228 0000 0072 2200 0000 7274 0000 0072  r(...r"...rt...r
+00002270: 7200 0000 7278 0000 0072 0f00 0000 720f  r...rx...r....r.
+00002280: 0000 0072 1200 0000 7221 0000 0003 0100  ...r....r!......
+00002290: 0073 0200 0000 0002 7a17 5479 7065 4869  .s......z.TypeHi
+000022a0: 6e74 2e69 735f 7369 6d70 6c65 5f74 7970  nt.is_simple_typ
+000022b0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+000022c0: 0000 0200 0000 4300 0000 730e 0000 0074  ......C...s....t
+000022d0: 0064 0083 017c 006a 0176 0053 0072 0e00  .d...|.j.v.S.r..
+000022e0: 0000 2902 7272 0000 0072 2800 0000 7278  ..).rr...r(...rx
+000022f0: 0000 0072 0f00 0000 720f 0000 0072 1200  ...r....r....r..
+00002300: 0000 da0b 6973 5f6f 7074 696f 6e61 6c07  ....is_optional.
+00002310: 0100 0073 0200 0000 0002 7a14 5479 7065  ...s......z.Type
+00002320: 4869 6e74 2e69 735f 6f70 7469 6f6e 616c  Hint.is_optional
+00002330: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002340: 0001 0000 0043 0000 0073 2800 0000 7c00  .....C...s(...|.
+00002350: 6a00 720c 7c00 6a01 5300 7c00 6a02 7318  j.r.|.j.S.|.j.s.
+00002360: 7c00 6a03 721e 7c00 6a04 5300 7c00 6a05  |.j.r.|.j.S.|.j.
+00002370: 5300 6400 5300 720e 0000 0029 0672 2100  S.d.S.r....).r!.
+00002380: 0000 7274 0000 0072 2900 0000 7225 0000  ..rt...r)...r%..
+00002390: 0072 2700 0000 7228 0000 0072 7800 0000  .r'...r(...rx...
+000023a0: 720f 0000 0072 0f00 0000 7212 0000 00da  r....r....r.....
+000023b0: 0d65 7870 6563 7465 645f 7479 7065 0b01  .expected_type..
+000023c0: 0000 730a 0000 0000 0206 0106 010c 0106  ..s.............
+000023d0: 027a 1654 7970 6548 696e 742e 6578 7065  .z.TypeHint.expe
+000023e0: 6374 6564 5f74 7970 6563 0100 0000 0000  cted_typec......
+000023f0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00002400: 0000 730c 0000 0074 007c 006a 0174 0283  ..s....t.|.j.t..
+00002410: 0253 0072 0e00 0000 2903 7248 0000 0072  .S.r....).rH...r
+00002420: 7400 0000 da08 5573 6572 4469 6374 7278  t.....UserDictrx
+00002430: 0000 0072 0f00 0000 720f 0000 0072 1200  ...r....r....r..
+00002440: 0000 da0d 6973 5f64 6963 745f 6d6f 6465  ....is_dict_mode
+00002450: 6c14 0100 0073 0200 0000 0002 7a16 5479  l....s......z.Ty
+00002460: 7065 4869 6e74 2e69 735f 6469 6374 5f6d  peHint.is_dict_m
+00002470: 6f64 656c 6301 0000 0000 0000 0000 0000  odelc...........
+00002480: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00002490: 0000 7400 7c00 6a01 8301 5300 720e 0000  ..t.|.j...S.r...
+000024a0: 0029 02da 0c69 735f 6461 7461 636c 6173  .)...is_dataclas
+000024b0: 7372 7400 0000 7278 0000 0072 0f00 0000  srt...rx...r....
+000024c0: 720f 0000 0072 1200 0000 7287 0000 0018  r....r....r.....
+000024d0: 0100 0073 0200 0000 0002 7a15 5479 7065  ...s......z.Type
+000024e0: 4869 6e74 2e69 735f 6461 7461 636c 6173  Hint.is_dataclas
+000024f0: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+00002500: 0000 0300 0000 4300 0000 730e 0000 007c  ......C...s....|
+00002510: 006a 0074 0174 0219 006b 0253 0072 0e00  .j.t.t...k.S.r..
+00002520: 0000 2903 7274 0000 0072 4100 0000 7233  ..).rt...rA...r3
+00002530: 0000 0072 7800 0000 720f 0000 0072 0f00  ...rx...r....r..
+00002540: 0000 7212 0000 00da 0e69 735f 7374 7269  ..r......is_stri
+00002550: 6e67 5f6c 6973 741c 0100 0073 0200 0000  ng_list....s....
+00002560: 0002 7a17 5479 7065 4869 6e74 2e69 735f  ..z.TypeHint.is_
+00002570: 7374 7269 6e67 5f6c 6973 7472 0b00 0000  string_listr....
+00002580: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00002590: 0004 0000 0003 0000 0073 de00 0000 8800  .........s......
+000025a0: 6a00 7256 8800 6a01 7218 7402 7c01 8800  j.rV..j.r.t.|...
+000025b0: 6a03 8302 5300 8800 6a04 7228 7402 7c01  j...S...j.r(t.|.
+000025c0: 7405 8302 5300 8800 6a06 724a 7402 7c01  t...S...j.rJt.|.
+000025d0: 7407 8302 6f48 7408 6401 6402 8400 7c01  t...oHt.d.d...|.
+000025e0: 4400 8301 8301 5300 7402 7c01 8800 6a03  D.....S.t.|...j.
+000025f0: 8302 5300 8800 6a09 7268 7402 7c01 8800  ..S...j.rht.|...
+00002600: 6a0a 8302 5300 8800 6a0b 7290 7402 7c01  j...S...j.r.t.|.
+00002610: 8800 6a0c 8302 6f8e 7408 8700 6601 6403  ..j...o.t...f.d.
+00002620: 6402 8408 7c01 4400 8301 8301 5300 8800  d...|.D.....S...
+00002630: 6a0d 72d6 7402 7c01 8800 6a0c 8302 6fd4  j.r.t.|...j...o.
+00002640: 7408 8700 6601 6404 6402 8408 7c01 a00e  t...f.d.d...|...
+00002650: a100 4400 8301 8301 6fd4 7408 8700 6601  ..D.....o.t...f.
+00002660: 6405 6402 8408 7c01 a00f a100 4400 8301  d.d...|.....D...
+00002670: 8301 5300 6406 5300 6400 5300 2907 4e63  ..S.d.S.d.S.).Nc
+00002680: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00002690: 0500 0000 5300 0000 7316 0000 0067 007c  ....S...s....g.|
+000026a0: 005d 0e7d 0174 007c 0174 0183 0291 0271  .].}.t.|.t.....q
+000026b0: 0453 0072 0f00 0000 2902 7222 0000 0072  .S.r....).r"...r
+000026c0: 3300 0000 724d 0000 0072 0f00 0000 720f  3...rM...r....r.
+000026d0: 0000 0072 1200 0000 7251 0000 0027 0100  ...r....rQ...'..
+000026e0: 0072 3200 0000 7a27 5479 7065 4869 6e74  .r2...z'TypeHint
+000026f0: 2e63 6865 636b 5f74 7970 652e 3c6c 6f63  .check_type.<loc
+00002700: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
+00002710: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00002720: 0500 0000 1300 0000 7318 0000 0067 007c  ........s....g.|
+00002730: 005d 107d 0174 007c 0188 006a 0183 0291  .].}.t.|...j....
+00002740: 0271 0453 0072 0f00 0000 a902 7222 0000  .q.S.r......r"..
+00002750: 0072 2800 0000 724d 0000 0072 7800 0000  .r(...rM...rx...
+00002760: 720f 0000 0072 1200 0000 7251 0000 002c  r....r....rQ...,
+00002770: 0100 0072 3200 0000 6301 0000 0000 0000  ...r2...c.......
+00002780: 0000 0000 0002 0000 0008 0000 0013 0000  ................
+00002790: 0073 2400 0000 6700 7c00 5d1c 7d01 7400  .s$...g.|.].}.t.
+000027a0: 7c01 7401 8800 6a02 6400 6401 8502 1900  |.t...j.d.d.....
+000027b0: 8301 8302 9102 7104 5300 2902 e901 0000  ......q.S.).....
+000027c0: 004e 2903 7222 0000 0072 4500 0000 7228  .N).r"...rE...r(
+000027d0: 0000 0072 4d00 0000 7278 0000 0072 0f00  ...rM...rx...r..
+000027e0: 0000 7212 0000 0072 5100 0000 2f01 0000  ..r....rQ.../...
+000027f0: 7232 0000 0063 0100 0000 0000 0000 0000  r2...c..........
+00002800: 0000 0200 0000 0600 0000 1300 0000 731c  ..............s.
+00002810: 0000 0067 007c 005d 147d 0174 007c 0188  ...g.|.].}.t.|..
+00002820: 006a 0164 0019 0083 0291 0271 0453 0072  .j.d.......q.S.r
+00002830: 4b00 0000 7289 0000 0072 4d00 0000 7278  K...r....rM...rx
+00002840: 0000 0072 0f00 0000 7212 0000 0072 5100  ...r....r....rQ.
+00002850: 0000 3001 0000 7232 0000 0046 2910 7221  ..0...r2...F).r!
+00002860: 0000 0072 8700 0000 7222 0000 0072 7400  ...r....r"...rt.
+00002870: 0000 7286 0000 0072 5900 0000 7288 0000  ..r....rY...r...
+00002880: 0072 4100 0000 727d 0000 0072 8200 0000  .rA...r}...r....
+00002890: 7228 0000 0072 2500 0000 7227 0000 0072  r(...r%...r'...r
+000028a0: 2900 0000 da06 7661 6c75 6573 da04 6b65  ).....values..ke
+000028b0: 7973 7210 0000 0072 0f00 0000 7278 0000  ysr....r....rx..
+000028c0: 0072 1200 0000 7220 0000 0020 0100 0073  .r....r ... ...s
+000028d0: 2a00 0000 0001 0601 0601 0c01 0601 0a01  *...............
+000028e0: 0601 1c01 0c01 0601 0c01 0601 2201 0601  ............"...
+000028f0: 0e01 14ff 0401 0201 14ff 02ff 0204 7a13  ..............z.
+00002900: 5479 7065 4869 6e74 2e63 6865 636b 5f74  TypeHint.check_t
+00002910: 7970 6563 0200 0000 0000 0000 0000 0000  ypec............
+00002920: 0200 0000 0400 0000 4300 0000 731c 0000  ........C...s...
+00002930: 007c 00a0 007c 01a1 0172 0e7c 0153 0074  .|...|...r.|.S.t
+00002940: 01a0 027c 017c 006a 03a1 0253 0072 0e00  ...|.|.j...S.r..
+00002950: 0000 2904 7220 0000 0072 0300 0000 721e  ..).r ...r....r.
+00002960: 0000 0072 7400 0000 7210 0000 0072 0f00  ...rt...r....r..
+00002970: 0000 720f 0000 0072 1200 0000 da05 7061  ..r....r......pa
+00002980: 7273 6535 0100 0073 0600 0000 0001 0a01  rse5...s........
+00002990: 0401 7a0e 5479 7065 4869 6e74 2e70 6172  ..z.TypeHint.par
+000029a0: 7365 4e29 1a72 1400 0000 7215 0000 0072  seN).r....r....r
+000029b0: 1600 0000 7275 0000 0072 7900 0000 da08  ....ru...ry.....
+000029c0: 7072 6f70 6572 7479 7245 0000 0072 7200  propertyrE...rr.
+000029d0: 0000 7228 0000 0072 7e00 0000 7227 0000  ..r(...r~...r'..
+000029e0: 0072 2500 0000 7229 0000 0072 8200 0000  .r%...r)...r....
+000029f0: da04 626f 6f6c 7221 0000 0072 8300 0000  ..boolr!...r....
+00002a00: 7284 0000 0072 8600 0000 7287 0000 0072  r....r....r....r
+00002a10: 8800 0000 da03 416e 7972 2000 0000 7206  ......Anyr ...r.
+00002a20: 0000 0072 0700 0000 728d 0000 0072 0f00  ...r....r....r..
+00002a30: 0000 720f 0000 0072 0f00 0000 7212 0000  ..r....r....r...
+00002a40: 0072 0100 0000 e400 0000 7338 0000 0008  .r........s8....
+00002a50: 0108 0308 0302 0114 0302 010a 0302 010a  ................
+00002a60: 0302 010a 0302 010a 0302 010a 0302 0110  ................
+00002a70: 0302 010a 0302 010a 0802 010a 0302 010a  ................
+00002a80: 0302 010a 0310 1572 0100 0000 6302 0000  .......r....c...
+00002a90: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00002aa0: 0043 0000 0073 0c00 0000 7400 a001 7c00  .C...s....t...|.
+00002ab0: 7c01 a102 5300 720e 0000 0029 0272 0300  |...S.r....).r..
+00002ac0: 0000 721e 0000 0029 0272 0c00 0000 7274  ..r....).r....rt
+00002ad0: 0000 0072 0f00 0000 720f 0000 0072 1200  ...r....r....r..
+00002ae0: 0000 7202 0000 003b 0100 0073 0200 0000  ..r....;...s....
+00002af0: 0001 7202 0000 004e 2922 da07 5f5f 616c  ..r....N)"..__al
+00002b00: 6c5f 5fda 1564 746d 6f64 656c 2e62 6173  l__..dtmodel.bas
+00002b10: 652e 5f69 6d70 6f72 7473 da11 6474 6d6f  e._imports..dtmo
+00002b20: 6465 6c2e 6675 6e63 7469 6f6e 73da 1664  del.functions..d
+00002b30: 746d 6f64 656c 2e62 6173 652e 6261 7365  tmodel.base.base
+00002b40: 5f65 6e75 6d72 4500 0000 7272 0000 005a  _enumrE...rr...Z
+00002b50: 0854 7970 6541 7267 7372 1700 0000 721a  .TypeArgsr....r.
+00002b60: 0000 0072 4100 0000 7243 0000 00da 0564  ...rA...rC.....d
+00002b70: 6571 7565 da08 5573 6572 4c69 7374 7280  eque..UserListr.
+00002b80: 0000 0072 5900 0000 7285 0000 0072 5a00  ...rY...r....rZ.
+00002b90: 0000 7281 0000 00da 0754 7970 6556 6172  ..r......TypeVar
+00002ba0: 7206 0000 0072 0700 0000 7273 0000 0072  r....r....rs...r
+00002bb0: 0800 0000 7237 0000 0072 3500 0000 723f  ....r7...r5...r?
+00002bc0: 0000 0072 0900 0000 da08 5072 6f74 6f63  ...r......Protoc
+00002bd0: 6f6c 720a 0000 0072 1800 0000 da03 4142  olr....r......AB
+00002be0: 4372 0300 0000 7201 0000 0072 0200 0000  Cr....r....r....
+00002bf0: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00002c00: 1200 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00002c10: 0000 7324 0000 0008 0708 0108 0108 0e08  ..s$............
+00002c20: 010c 010e 010a 0108 0108 010c 0108 010e  ................
+00002c30: 0310 0510 0510 7f00 380e 57              ........8.W
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/dates.py` & `dtmodel-0.1.6/dtmodel/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/json_encoder.py` & `dtmodel-0.1.6/dtmodel/parse/json_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # import json
 # import datetime
 # from enum import Enum
 # from dataclasses import asdict, is_dataclass
 # from collections import UserString, UserList, UserDict
 # from typing import Any
-from dtmodel.dtfield._imports import *
+from dtmodel.base._imports import *
 from dtbase import Jsonable
 
 
 class JsonEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime.datetime):
             return obj.isoformat()[:16]
@@ -33,14 +33,16 @@
             return str(obj)
         elif isinstance(obj, (UserDict, UserList)):
             return json_parse(obj.data)
         elif hasattr(obj, 'asjson'):
             return obj.asjson()
         elif is_dataclass(obj) and not isinstance(obj, type):
             return json_parse(asdict(obj))
+        elif isinstance(obj, Decimal):
+            return str(float(obj))
         return json.JSONEncoder.default(self, obj)
 
 
 def json_loads(obj: str) -> Jsonable:
     return json.loads(obj)
```

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/number.py` & `dtmodel-0.1.6/dtmodel/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/string.py` & `dtmodel-0.1.6/dtmodel/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.5/dtmodel/dtfield/parse/type_hint.py` & `dtmodel-0.1.6/dtmodel/parse/type_hint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 __all__ = [
         'TypeHint',
         'parser',
         'Parser'
 ]
 
 
-from .._imports import *
-from .null import *
-from dtmodel.dtfield.base_enum import *
-
-
-JsonPrimitive = Union[str, float, int, bool, None]
-DetaData = Union[dict, list, str, float, int, bool]
-DetaKey = Union[str, None]
-ExpireIn = Union[str, None]
-ExpireAt = Union[datetime.datetime, int, float, None]
-JsonSequence = list[JsonPrimitive]
-JsonDict = dict[str, Union[JsonSequence, JsonPrimitive]]
-Jsonable = Union[JsonDict, JsonSequence, JsonPrimitive]
-DetaQuery = Union[dict[str, JsonPrimitive], list[dict[str, JsonPrimitive]]]
-ExistParams = Union[list[str], str]
-SearchParam = str
+from dtmodel.base._imports import *
+from dtmodel.functions import *
+from dtmodel.base.base_enum import *
+
+
+# JsonPrimitive = Union[str, float, int, bool, None]
+# DetaData = Union[dict, list, str, float, int, bool]
+# DetaKey = Union[str, None]
+# ExpireIn = Union[str, None]
+# ExpireAt = Union[datetime.datetime, int, float, None]
+# JsonSequence = list[JsonPrimitive]
+# JsonDict = dict[str, Union[JsonSequence, JsonPrimitive]]
+# Jsonable = Union[JsonDict, JsonSequence, JsonPrimitive]
+# DetaQuery = Union[dict[str, JsonPrimitive], list[dict[str, JsonPrimitive]]]
+# ExistParams = Union[list[str], str]
+# SearchParam = str
 TypeArgs = tuple[type]
 Types = Union[type, TypeArgs]
 TupleSequenceTypes = (tuple, list, set, deque, UserList)
 TupleMapTypes = (dict, UserDict, ChainMap)
 ParserEntry = TypeVar('ParserEntry')
 ParserResult = TypeVar('ParserResult')
 ParserReturn = Union[ParserEntry, ParserResult]
@@ -154,15 +154,15 @@
         elif isinstance(value, Decimal):
             return int(value)
         elif isinstance(value, (datetime.date, datetime.datetime)):
             return value.toordinal()
         return value
     
     @classmethod
-    def context_model(cls, value: dict, model_type: type['ContextBase']):
+    def context_model(cls, value: dict, model_type: type['Model']):
         return model_type.safe_create(**value)
         
     @classmethod
     def float_engine(cls, value):
         if isinstance(value, str):
             return float(re.sub(r',', '.', value))
         elif isinstance(value, int):
```

### Comparing `dtmodel-0.1.5/dtmodel/enums/__pycache__/facility.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/models/enums/__pycache__/facility.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 18 01:52:52 2023 UTC, .py size: 789 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7463 8e64 1503 0000  a.......tc.d....
+00000000: 610d 0d0a 0000 0000 8fd7 8f64 1203 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6702 5a00 6402 6403 6c01 6d02 5a02  d.g.Z.d.d.l.m.Z.
 00000040: 0100 4700 6404 6400 8400 6400 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 4700 6405 6401 8400 6401 6502 8303  Z.G.d.d...d.e...
 00000060: 5a04 6406 5300 2907 da0d 5061 796d 656e  Z.d.S.)...Paymen
 00000070: 744d 6574 686f 64da 0b53 6572 7669 6365  tMethod..Service
@@ -18,59 +18,59 @@
 00000110: 44c3 a962 6974 6f75 1800 0000 5472 616e  D..bitou....Tran
 00000120: 7366 6572 c3aa 6e63 6961 2042 616e 63c3  sfer..ncia Banc.
 00000130: a172 6961 5a03 5069 785a 0643 6865 7175  .riaZ.PixZ.Chequ
 00000140: 654e 2909 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
 00000150: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000160: 616c 6e61 6d65 5f5f da02 4341 da02 4352  alname__..CA..CR
 00000170: 5a02 4445 5a02 5452 5a02 5049 5a02 4348  Z.DEZ.TRZ.PIZ.CH
-00000180: a900 720a 0000 0072 0a00 0000 fa70 2f55  ..r....r.....p/U
+00000180: a900 720a 0000 0072 0a00 0000 fa77 2f55  ..r....r.....w/U
 00000190: 7365 7273 2f64 616e 6965 6c61 7261 6e74  sers/danielarant
 000001a0: 6573 2f4c 6962 7261 7279 2f4d 6f62 696c  es/Library/Mobil
 000001b0: 6520 446f 6375 6d65 6e74 732f 636f 6d7e  e Documents/com~
 000001c0: 6170 706c 657e 436c 6f75 6444 6f63 732f  apple~CloudDocs/
 000001d0: 4d79 2041 7070 732f 7079 7069 2f64 746d  My Apps/pypi/dtm
-000001e0: 6f64 656c 2f64 746d 6f64 656c 2f65 6e75  odel/dtmodel/enu
-000001f0: 6d73 2f66 6163 696c 6974 792e 7079 7201  ms/facility.pyr.
-00000200: 0000 0009 0000 0073 0c00 0000 0801 0401  .......s........
-00000210: 0401 0401 0401 0401 6300 0000 0000 0000  ........c.......
-00000220: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00000230: 0073 4c00 0000 6500 5a01 6400 5a02 6401  .sL...e.Z.d.Z.d.
-00000240: 5a03 6402 5a04 6403 5a05 6404 5a06 6405  Z.d.Z.d.Z.d.Z.d.
-00000250: 5a07 6406 5a08 6407 5a09 6408 5a0a 6409  Z.d.Z.d.Z.d.Z.d.
-00000260: 5a0b 640a 5a0c 640b 5a0d 640c 5a0e 640d  Z.d.Z.d.Z.d.Z.d.
-00000270: 5a0f 640e 5a10 640f 5a11 6410 5a12 6411  Z.d.Z.d.Z.d.Z.d.
-00000280: 5300 2912 7202 0000 007a 1043 6f6e 7375  S.).r....z.Consu
-00000290: 6c74 6120 496e 6963 6961 6c7a 1043 6f6e  lta Inicialz.Con
-000002a0: 7375 6c74 6120 5265 6775 6c61 727a 1043  sulta Regularz.C
-000002b0: 6f6e 7375 6c74 6120 456e 6361 6978 657a  onsulta Encaixez
-000002c0: 1143 6f6e 7375 6c74 6120 436f 7274 6573  .Consulta Cortes
-000002d0: 6961 7a0e 436f 6e73 756c 7461 2042 7265  iaz.Consulta Bre
-000002e0: 7665 7a13 5265 746f 726e 6f20 6465 2043  vez.Retorno de C
-000002f0: 6f6e 7375 6c74 617a 1156 6973 6974 6120  onsultaz.Visita 
-00000300: 486f 7370 6974 616c 6172 7a11 5465 7261  Hospitalarz.Tera
-00000310: 7069 6120 4173 7369 7374 6964 617a 1156  pia Assistidaz.V
-00000320: 6973 6974 6120 446f 6d69 6369 6c69 6172  isita Domiciliar
-00000330: 7511 0000 0041 6365 7274 6f20 6465 2044  u....Acerto de D
-00000340: c3a9 6269 746f 7515 0000 0053 7570 6f72  ..bitou....Supor
-00000350: 7465 2064 6520 4c6f 67c3 ad73 7469 6361  te de Log..stica
-00000360: 7a0f 416c 7567 7565 6c20 6465 2053 616c  z.Aluguel de Sal
-00000370: 6175 0f00 0000 416c 7567 7565 6c20 4469  au....Aluguel Di
-00000380: c3a1 7269 6f75 1200 0000 5365 7373 c3a3  ..riou....Sess..
-00000390: 6f20 6465 2054 6572 6170 6961 750e 0000  o de Terapiau...
-000003a0: 004f 7574 726f 2053 6572 7669 c3a7 6f7a  .Outro Servi..oz
-000003b0: 1056 656e 6461 2064 6520 5072 6f64 7574  .Venda de Produt
-000003c0: 6f4e 2913 7205 0000 0072 0600 0000 7207  oN).r....r....r.
-000003d0: 0000 005a 0243 495a 0243 4f5a 0243 455a  ...Z.CIZ.COZ.CEZ
-000003e0: 0243 435a 0243 505a 0252 545a 0256 485a  .CCZ.CPZ.RTZ.VHZ
-000003f0: 0253 415a 0256 445a 0241 445a 0253 55da  .SAZ.VDZ.ADZ.SU.
-00000400: 0241 4c5a 0241 435a 0253 455a 024f 535a  .ALZ.ACZ.SEZ.OSZ
-00000410: 0256 4572 0a00 0000 720a 0000 0072 0a00  .VEr....r....r..
-00000420: 0000 720b 0000 0072 0200 0000 1300 0000  ..r....r........
-00000430: 7320 0000 0008 0104 0104 0104 0104 0104  s ..............
-00000440: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00000450: 0104 0104 014e 2905 da07 5f5f 616c 6c5f  .....N)...__all_
-00000460: 5fda 1964 746d 6f64 656c 2e64 7466 6965  _..dtmodel.dtfie
-00000470: 6c64 2e62 6173 655f 656e 756d 7204 0000  ld.base_enumr...
-00000480: 0072 0100 0000 7202 0000 0072 0a00 0000  .r....r....r....
-00000490: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-000004a0: 083c 6d6f 6475 6c65 3e02 0000 0073 0a00  .<module>....s..
-000004b0: 0000 0201 02fe 0405 0c03 100a            ............
+000001e0: 6f64 656c 2f64 746d 6f64 656c 2f6d 6f64  odel/dtmodel/mod
+000001f0: 656c 732f 656e 756d 732f 6661 6369 6c69  els/enums/facili
+00000200: 7479 2e70 7972 0100 0000 0900 0000 730c  ty.pyr........s.
+00000210: 0000 0008 0104 0104 0104 0104 0104 0163  ...............c
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0100 0000 4000 0000 734c 0000 0065 005a  ....@...sL...e.Z
+00000240: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
+00000250: 0564 045a 0664 055a 0764 065a 0864 075a  .d.Z.d.Z.d.Z.d.Z
+00000260: 0964 085a 0a64 095a 0b64 0a5a 0c64 0b5a  .d.Z.d.Z.d.Z.d.Z
+00000270: 0d64 0c5a 0e64 0d5a 0f64 0e5a 1064 0f5a  .d.Z.d.Z.d.Z.d.Z
+00000280: 1164 105a 1264 1153 0029 1272 0200 0000  .d.Z.d.S.).r....
+00000290: 7a10 436f 6e73 756c 7461 2049 6e69 6369  z.Consulta Inici
+000002a0: 616c 7a10 436f 6e73 756c 7461 2052 6567  alz.Consulta Reg
+000002b0: 756c 6172 7a10 436f 6e73 756c 7461 2045  ularz.Consulta E
+000002c0: 6e63 6169 7865 7a11 436f 6e73 756c 7461  ncaixez.Consulta
+000002d0: 2043 6f72 7465 7369 617a 0e43 6f6e 7375   Cortesiaz.Consu
+000002e0: 6c74 6120 4272 6576 657a 1352 6574 6f72  lta Brevez.Retor
+000002f0: 6e6f 2064 6520 436f 6e73 756c 7461 7a11  no de Consultaz.
+00000300: 5669 7369 7461 2048 6f73 7069 7461 6c61  Visita Hospitala
+00000310: 727a 1154 6572 6170 6961 2041 7373 6973  rz.Terapia Assis
+00000320: 7469 6461 7a11 5669 7369 7461 2044 6f6d  tidaz.Visita Dom
+00000330: 6963 696c 6961 7275 1100 0000 4163 6572  iciliaru....Acer
+00000340: 746f 2064 6520 44c3 a962 6974 6f75 1500  to de D..bitou..
+00000350: 0000 5375 706f 7274 6520 6465 204c 6f67  ..Suporte de Log
+00000360: c3ad 7374 6963 617a 0f41 6c75 6775 656c  ..sticaz.Aluguel
+00000370: 2064 6520 5361 6c61 750f 0000 0041 6c75   de Salau....Alu
+00000380: 6775 656c 2044 69c3 a172 696f 7512 0000  guel Di..riou...
+00000390: 0053 6573 73c3 a36f 2064 6520 5465 7261  .Sess..o de Tera
+000003a0: 7069 6175 0e00 0000 4f75 7472 6f20 5365  piau....Outro Se
+000003b0: 7276 69c3 a76f 7a10 5665 6e64 6120 6465  rvi..oz.Venda de
+000003c0: 2050 726f 6475 746f 4e29 1372 0500 0000   ProdutoN).r....
+000003d0: 7206 0000 0072 0700 0000 5a02 4349 5a02  r....r....Z.CIZ.
+000003e0: 434f 5a02 4345 5a02 4343 5a02 4350 5a02  COZ.CEZ.CCZ.CPZ.
+000003f0: 5254 5a02 5648 5a02 5341 5a02 5644 5a02  RTZ.VHZ.SAZ.VDZ.
+00000400: 4144 5a02 5355 da02 414c 5a02 4143 5a02  ADZ.SU..ALZ.ACZ.
+00000410: 5345 5a02 4f53 5a02 5645 720a 0000 0072  SEZ.OSZ.VEr....r
+00000420: 0a00 0000 720a 0000 0072 0b00 0000 7202  ....r....r....r.
+00000430: 0000 0013 0000 0073 2000 0000 0801 0401  .......s .......
+00000440: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00000450: 0401 0401 0401 0401 0401 0401 4e29 05da  ............N)..
+00000460: 075f 5f61 6c6c 5f5f da16 6474 6d6f 6465  .__all__..dtmode
+00000470: 6c2e 6261 7365 2e62 6173 655f 656e 756d  l.base.base_enum
+00000480: 7204 0000 0072 0100 0000 7202 0000 0072  r....r....r....r
+00000490: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000004a0: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
+000004b0: 0073 0a00 0000 0201 02fe 0405 0c03 100a  .s..............
```

### Comparing `dtmodel-0.1.5/dtmodel/enums/__pycache__/medical.cpython-39.pyc` & `dtmodel-0.1.6/dtmodel/models/enums/__pycache__/medical.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 18 01:52:52 2023 UTC, .py size: 278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-00000000: 610d 0d0a 0000 0000 7463 8e64 1601 0000  a.......tc.d....
+00000000: 610d 0d0a 0000 0000 a846 9864 2f01 0000  a........F.d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6701 5a00 6401 6402 6c01 6d02 5a02 0100  g.Z.d.d.l.m.Z...
 00000040: 4700 6403 6400 8400 6400 6502 8303 5a03  G.d.d...d.e...Z.
-00000050: 6404 5300 2905 da09 5669 7369 7454 7970  d.S.)...VisitTyp
-00000060: 65e9 0000 0000 2901 da08 4261 7365 456e  e.....)...BaseEn
-00000070: 756d 6300 0000 0000 0000 0000 0000 0000  umc.............
-00000080: 0000 0001 0000 0040 0000 0073 2c00 0000  .......@...s,...
-00000090: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-000000a0: 6403 5a05 6404 5a06 6405 5a07 6406 5a08  d.Z.d.Z.d.Z.d.Z.
-000000b0: 6407 5a09 6408 5a0a 6409 5300 290a 7201  d.Z.d.Z.d.S.).r.
-000000c0: 0000 005a 0749 6e69 6369 616c 5a0a 5365  ...Z.InicialZ.Se
-000000d0: 6775 696d 656e 746f 5a07 456e 6361 6978  guimentoZ.Encaix
-000000e0: 655a 0843 6f72 7465 7369 615a 0542 7265  eZ.CortesiaZ.Bre
-000000f0: 7665 5a07 5265 746f 726e 6f5a 0a48 6f73  veZ.RetornoZ.Hos
-00000100: 7069 7461 6c61 725a 0a44 6f6d 6963 696c  pitalarZ.Domicil
-00000110: 6961 724e 290b da08 5f5f 6e61 6d65 5f5f  iarN)...__name__
-00000120: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000130: 7175 616c 6e61 6d65 5f5f da02 4349 da02  qualname__..CI..
-00000140: 434f da02 4345 da02 4343 da02 4350 da02  CO..CE..CC..CP..
-00000150: 5254 da02 5648 da02 5644 a900 720f 0000  RT..VH..VD..r...
-00000160: 0072 0f00 0000 fa6f 2f55 7365 7273 2f64  .r.....o/Users/d
-00000170: 616e 6965 6c61 7261 6e74 6573 2f4c 6962  anielarantes/Lib
-00000180: 7261 7279 2f4d 6f62 696c 6520 446f 6375  rary/Mobile Docu
-00000190: 6d65 6e74 732f 636f 6d7e 6170 706c 657e  ments/com~apple~
-000001a0: 436c 6f75 6444 6f63 732f 4d79 2041 7070  CloudDocs/My App
-000001b0: 732f 7079 7069 2f64 746d 6f64 656c 2f64  s/pypi/dtmodel/d
-000001c0: 746d 6f64 656c 2f65 6e75 6d73 2f6d 6564  tmodel/enums/med
-000001d0: 6963 616c 2e70 7972 0100 0000 0900 0000  ical.pyr........
-000001e0: 7310 0000 0008 0104 0104 0104 0104 0104  s...............
-000001f0: 0104 0104 014e 2904 da07 5f5f 616c 6c5f  .....N)...__all_
-00000200: 5fda 1964 746d 6f64 656c 2e64 7466 6965  _..dtmodel.dtfie
-00000210: 6c64 2e62 6173 655f 656e 756d 7203 0000  ld.base_enumr...
-00000220: 0072 0100 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00000230: 720f 0000 0072 1000 0000 da08 3c6d 6f64  r....r......<mod
-00000240: 756c 653e 0200 0000 7306 0000 0002 ff04  ule>....s.......
-00000250: 040c 04                                  ...
+00000050: 6404 5300 2905 da0d 5669 7369 7454 7970  d.S.)...VisitTyp
+00000060: 6545 6e75 6de9 0000 0000 2901 da08 4261  eEnum.....)...Ba
+00000070: 7365 456e 756d 6300 0000 0000 0000 0000  seEnumc.........
+00000080: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+00000090: 3000 0000 6500 5a01 6400 5a02 6401 5a03  0...e.Z.d.Z.d.Z.
+000000a0: 6402 5a04 6403 5a05 6404 5a06 6405 5a07  d.Z.d.Z.d.Z.d.Z.
+000000b0: 6406 5a08 6407 5a09 6408 5a0a 6409 5a0b  d.Z.d.Z.d.Z.d.Z.
+000000c0: 640a 5300 290b 7201 0000 005a 0749 6e69  d.S.).r....Z.Ini
+000000d0: 6369 616c 5a0a 5365 6775 696d 656e 746f  cialZ.Seguimento
+000000e0: 5a07 456e 6361 6978 655a 0843 6f72 7465  Z.EncaixeZ.Corte
+000000f0: 7369 615a 0542 7265 7665 5a07 5265 746f  siaZ.BreveZ.Reto
+00000100: 726e 6f5a 0a48 6f73 7069 7461 6c61 725a  rnoZ.HospitalarZ
+00000110: 0a44 6f6d 6963 696c 6961 7275 0800 0000  .Domiciliaru....
+00000120: 5265 7669 73c3 a36f 4e29 0cda 085f 5f6e  Revis..oN)...__n
+00000130: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000140: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000150: 0243 49da 0243 4fda 0243 45da 0243 43da  .CI..CO..CE..CC.
+00000160: 0243 50da 0252 54da 0256 48da 0256 445a  .CP..RT..VH..VDZ
+00000170: 0252 56a9 0072 0f00 0000 720f 0000 00fa  .RV..r....r.....
+00000180: 762f 5573 6572 732f 6461 6e69 656c 6172  v/Users/danielar
+00000190: 616e 7465 732f 4c69 6272 6172 792f 4d6f  antes/Library/Mo
+000001a0: 6269 6c65 2044 6f63 756d 656e 7473 2f63  bile Documents/c
+000001b0: 6f6d 7e61 7070 6c65 7e43 6c6f 7564 446f  om~apple~CloudDo
+000001c0: 6373 2f4d 7920 4170 7073 2f70 7970 692f  cs/My Apps/pypi/
+000001d0: 6474 6d6f 6465 6c2f 6474 6d6f 6465 6c2f  dtmodel/dtmodel/
+000001e0: 6d6f 6465 6c73 2f65 6e75 6d73 2f6d 6564  models/enums/med
+000001f0: 6963 616c 2e70 7972 0100 0000 0900 0000  ical.pyr........
+00000200: 7312 0000 0008 0104 0104 0104 0104 0104  s...............
+00000210: 0104 0104 0104 014e 2904 da07 5f5f 616c  .......N)...__al
+00000220: 6c5f 5fda 1664 746d 6f64 656c 2e62 6173  l__..dtmodel.bas
+00000230: 652e 6261 7365 5f65 6e75 6d72 0300 0000  e.base_enumr....
+00000240: 7201 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00000250: 0f00 0000 7210 0000 00da 083c 6d6f 6475  ....r......<modu
+00000260: 6c65 3e02 0000 0073 0600 0000 02ff 0404  le>....s........
+00000270: 0c04                                     ..
```

### Comparing `dtmodel-0.1.5/dtmodel/enums/facility.py` & `dtmodel-0.1.6/dtmodel/models/enums/facility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __all__ = [
         'PaymentMethod',
         'ServiceType'
 ]
 
-from dtmodel.dtfield.base_enum import BaseEnum
+from dtmodel.base.base_enum import BaseEnum
 
 
 class PaymentMethod(BaseEnum):
     CA = 'Dinheiro'
     CR = 'Cartão de Crédito'
     DE = 'Cartão De Débito'
     TR = 'Transferência Bancária'
```

### Comparing `dtmodel-0.1.5/dtmodel/models/people.py` & `dtmodel-0.1.6/dtmodel/models/people.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,25 @@
         'Doctor',
         'Therapist',
         'Employee',
         'User',
         'Patient'
 ]
 
-import datetime
-
-from dtmodel.dtfield import context_model, dataclass, is_null, normalize_lower, descdataclass
+from dtmodel.base._imports import *
+from dtmodel.model import context_model
 import bcrypt
-from ..bases import *
+from dtmodel.models.bases import *
 from ..functions import *
 
 @context_model
 @descdataclass
-class Person(SelfKey, PersonCode, SocialName, PersonBase):
+class Person(SelfKey, PersonCode, GenderIdentity, CPF, PersonBase):
+    EXIST_PARAMS = ['code', 'cpf']
+    SINGULAR = 'Pessoa'
     
     @property
     def  age(self):
         return years(self.bdate, datetime.date.today())
     
     @property
     def fullname(self):
@@ -37,50 +38,59 @@
     def __str__(self):
         return self.social_name if not is_null(self.social_name) else self.fullname
 
 
 
 @context_model
 @descdataclass
-class Patient(SelfKey, Address, Email, Phone, PersonKey):
+class Patient(SelfKey, Address, Email, Phone,  Profile):
+    EXIST_PARAMS = 'person_key'
+    SINGULAR = 'Paciente'
+
     def __str__(self):
         return self.person.__str__()
     
     def __lt__(self, other):
         return normalize_lower(str(self)) < normalize_lower(str(other))
     
     
 @descdataclass
-class Provider(SelfKey, Address, Email, Phone, Register, PersonKey):
-    
+class Provider(SelfKey, Address, Email, Phone, Register, Profile):
+
     def __str__(self):
         return '{} {}'.format('Dr.' if self.person.gender.name == 'M' else 'Dra.', self.person.short_name)
 
 
 @context_model
 @descdataclass
 class Doctor(Provider):
-    pass
+    EXIST_PARAMS = 'person_key'
+    SINGULAR = 'Médico'
 
 
 @context_model
 @descdataclass
 class Therapist(Provider):
-    pass
+    EXIST_PARAMS = 'person_key'
+    SINGULAR = 'Terapeuta'
 
 
 @context_model
 @descdataclass
 class Employee(SelfKey, WorkActivity, Address, Email, Phone, Salary, PersonKey):
-    pass
+    EXIST_PARAMS = 'person_key'
+    SINGULAR = 'Funcionário'
 
 
 @context_model
 @descdataclass
 class User(SelfKey, PasswordRepeat, Password, ProfileKey, Username):
+    EXIST_PARAMS = ['username', 'profile_key']
+    SINGULAR = 'Usuário'
+
     
     def __post_init__(self, password_repeat: bytes = None):
         if not is_null(password_repeat):
             if isinstance(password_repeat, str):
                 password_repeat = password_repeat.encode('utf-8')
                 assert self.password == password_repeat
                 self.password = bcrypt.hashpw(self.password, bcrypt.gensalt())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dtmodel-0.1.5/PKG-INFO` & `dtmodel-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtmodel
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

