# Comparing `tmp/jacktest-0.0.5.tar.gz` & `tmp/jacktest-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacktest-0.0.5.tar", last modified: Mon Jul  3 03:36:55 2023, max compression
+gzip compressed data, was "jacktest-0.0.6.tar", last modified: Mon Jul  3 03:44:28 2023, max compression
```

## Comparing `jacktest-0.0.5.tar` & `jacktest-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:36:55.104024 jacktest-0.0.5/
--rw-r--r--   0 bytedance   (501) staff       (20)     1074 2023-06-29 12:19:57.000000 jacktest-0.0.5/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:36:55.103694 jacktest-0.0.5/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      172 2023-06-29 12:19:40.000000 jacktest-0.0.5/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:36:55.101127 jacktest-0.0.5/jacktest/
--rw-r--r--   0 bytedance   (501) staff       (20)       73 2023-07-03 03:36:27.000000 jacktest-0.0.5/jacktest/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      155 2023-07-03 03:36:00.000000 jacktest-0.0.5/jacktest/print_hi.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:36:55.103142 jacktest-0.0.5/jacktest.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      196 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        9 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-03 03:36:55.104139 jacktest-0.0.5/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     1748 2023-07-03 03:36:50.000000 jacktest-0.0.5/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:44:28.910639 jacktest-0.0.6/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1074 2023-06-29 12:19:57.000000 jacktest-0.0.6/LICENSE
+-rw-r--r--   0 bytedance   (501) staff       (20)      560 2023-07-03 03:44:28.910284 jacktest-0.0.6/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      172 2023-06-29 12:19:40.000000 jacktest-0.0.6/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:44:28.907686 jacktest-0.0.6/jacktest/
+-rw-r--r--   0 bytedance   (501) staff       (20)      101 2023-07-03 03:42:55.000000 jacktest-0.0.6/jacktest/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      179 2023-07-03 03:42:30.000000 jacktest-0.0.6/jacktest/print_hi.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:44:28.909757 jacktest-0.0.6/jacktest.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)      560 2023-07-03 03:44:28.000000 jacktest-0.0.6/jacktest.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      196 2023-07-03 03:44:28.000000 jacktest-0.0.6/jacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-03 03:44:28.000000 jacktest-0.0.6/jacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        9 2023-07-03 03:44:28.000000 jacktest-0.0.6/jacktest.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-03 03:44:28.910768 jacktest-0.0.6/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)     1770 2023-07-03 03:44:10.000000 jacktest-0.0.6/setup.py
```

### Comparing `jacktest-0.0.5/LICENSE` & `jacktest-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jacktest-0.0.5/setup.py` & `jacktest-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# import setuptools
-#
-# with open("README.md", "r") as fh:
-#   long_description = fh.read()
-#
-# setuptools.setup(
-#   name="jacktest",
-#   version="0.0.2",
-#   author="jack",
-#   author_email="jack@example.com",
-#   description="A small example package",
-#   long_description=long_description,
-#   long_description_content_type="text/markdown",
-#   url="https://github.com/pypa/sampleproject",
-#   packages=setuptools.find_packages(),
-#   classifiers=[
-#   "Programming Language :: Python :: 3",
-#   "License :: OSI Approved :: MIT License",
-#   "Operating System :: OS Independent",
-#   ],
-# )
-
+import setuptools
 
-from distutils.core import setup
-from setuptools import find_packages
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
-setup(name='jacktest',  # 包名
-      version='0.0.5',  # 版本号
-      description='A small example package',
-      long_description=long_description,
-      author='jack',
-      author_email='jack@example.com',
-      url='https://github.com/pypa/sampleproject',
-      install_requires=[],
-      license='BSD License',
-      packages=find_packages(),
-      platforms=["all"],
-      classifiers=[
-          'Intended Audience :: Developers',
-          'Operating System :: OS Independent',
-          'Natural Language :: Chinese (Simplified)',
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Topic :: Software Development :: Libraries'
-      ],
-      )
+setuptools.setup(
+  name="jacktest",
+  version="0.0.6",
+  author="jack",
+  author_email="jack@example.com",
+  description="A small example package",
+  long_description=long_description,
+  long_description_content_type="text/markdown",
+  url="https://github.com/pypa/sampleproject",
+  packages=setuptools.find_packages(),
+  classifiers=[
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  ],
+)
+
+#
+# from distutils.core import setup
+# from setuptools import find_packages
+# with open("README.md", "r") as fh:
+#   long_description = fh.read()
+#
+# setup(name='jacktest',  # 包名
+#       version='0.0.5',  # 版本号
+#       description='A small example package',
+#       long_description=long_description,
+#       author='jack',
+#       author_email='jack@example.com',
+#       url='https://github.com/pypa/sampleproject',
+#       install_requires=[],
+#       license='BSD License',
+#       packages=find_packages(),
+#       platforms=["all"],
+#       classifiers=[
+#           'Intended Audience :: Developers',
+#           'Operating System :: OS Independent',
+#           'Natural Language :: Chinese (Simplified)',
+#           'Programming Language :: Python',
+#           'Programming Language :: Python :: 2',
+#           'Programming Language :: Python :: 2.7',
+#           'Programming Language :: Python :: 3',
+#           'Programming Language :: Python :: 3.5',
+#           'Programming Language :: Python :: 3.6',
+#           'Programming Language :: Python :: 3.7',
+#           'Programming Language :: Python :: 3.8',
+#           'Topic :: Software Development :: Libraries'
+#       ],
+#       )
```

