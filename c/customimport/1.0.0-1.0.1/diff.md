# Comparing `tmp/customimport-1.0.0.tar.gz` & `tmp/customimport-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customimport-1.0.0.tar", last modified: Sun Jul  2 19:18:09 2023, max compression
+gzip compressed data, was "customimport-1.0.1.tar", last modified: Mon Jul  3 09:41:55 2023, max compression
```

## Comparing `customimport-1.0.0.tar` & `customimport-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 19:18:09.485213 customimport-1.0.0/
--rw-rw-rw-   0        0        0     1546 2023-07-02 19:10:48.000000 customimport-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      243 2023-07-02 19:18:09.484212 customimport-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2784 2023-07-02 19:15:18.000000 customimport-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 19:18:09.482233 customimport-1.0.0/customimport.egg-info/
--rw-rw-rw-   0        0        0      243 2023-07-02 19:18:09.000000 customimport-1.0.0/customimport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-02 19:18:09.000000 customimport-1.0.0/customimport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 19:18:09.000000 customimport-1.0.0/customimport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 19:18:09.000000 customimport-1.0.0/customimport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 19:18:09.485213 customimport-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      319 2023-07-02 18:58:02.000000 customimport-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:41:55.322291 customimport-1.0.1/
+-rw-rw-rw-   0        0        0     1546 2023-07-02 19:10:48.000000 customimport-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      293 2023-07-03 09:41:55.321292 customimport-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2822 2023-07-02 22:27:38.000000 customimport-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 09:41:55.319289 customimport-1.0.1/customimport.egg-info/
+-rw-rw-rw-   0        0        0      293 2023-07-03 09:41:55.000000 customimport-1.0.1/customimport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-07-03 09:41:55.000000 customimport-1.0.1/customimport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:41:55.000000 customimport-1.0.1/customimport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:41:55.000000 customimport-1.0.1/customimport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      474 2023-07-03 09:41:39.000000 customimport-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 09:41:55.322291 customimport-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      349 2023-07-03 09:41:39.000000 customimport-1.0.1/setup.py
```

### Comparing `customimport-1.0.0/LICENSE` & `customimport-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `customimport-1.0.0/README.md` & `customimport-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Custom importing library
 
+```
+pip install customimport
+```
+
 ### Importing a function from n different code files depending on the running operating system.
 Let's say this is our project structure:
 ```
 main/
   -> main.py
   -> linux.py
   -> windows/
```

