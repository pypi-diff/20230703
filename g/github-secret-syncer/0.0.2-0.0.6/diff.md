# Comparing `tmp/github-secret-syncer-0.0.2.tar.gz` & `tmp/github-secret-syncer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-secret-syncer-0.0.2.tar", last modified: Fri Jun 30 18:33:30 2023, max compression
+gzip compressed data, was "github-secret-syncer-0.0.6.tar", last modified: Mon Jul  3 08:33:42 2023, max compression
```

## Comparing `github-secret-syncer-0.0.2.tar` & `github-secret-syncer-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-30 18:33:30.841631 github-secret-syncer-0.0.2/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.2/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)      559 2023-06-30 18:33:30.841498 github-secret-syncer-0.0.2/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)     1079 2023-06-30 18:18:09.000000 github-secret-syncer-0.0.2/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-30 18:33:30.840829 github-secret-syncer-0.0.2/github_secret_syncer/
--rw-r--r--   0 j3ymac     (501) staff       (20)     4623 2023-06-30 18:17:38.000000 github-secret-syncer-0.0.2/github_secret_syncer/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-30 18:33:30.841349 github-secret-syncer-0.0.2/github_secret_syncer.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)      559 2023-06-30 18:33:30.000000 github-secret-syncer-0.0.2/github_secret_syncer.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      235 2023-06-30 18:33:30.000000 github-secret-syncer-0.0.2/github_secret_syncer.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-06-30 18:33:30.000000 github-secret-syncer-0.0.2/github_secret_syncer.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-06-30 18:33:30.000000 github-secret-syncer-0.0.2/github_secret_syncer.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-06-30 18:33:30.841672 github-secret-syncer-0.0.2/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      697 2023-06-30 18:18:18.000000 github-secret-syncer-0.0.2/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:33:42.112405 github-secret-syncer-0.0.6/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.6/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1223 2023-07-03 08:33:42.112264 github-secret-syncer-0.0.6/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      741 2023-07-01 07:55:17.000000 github-secret-syncer-0.0.6/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:33:42.111489 github-secret-syncer-0.0.6/github_secret_syncer/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     4623 2023-06-30 18:17:38.000000 github-secret-syncer-0.0.6/github_secret_syncer/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:33:42.112046 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1223 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      235 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-03 08:33:42.112454 github-secret-syncer-0.0.6/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      733 2023-07-01 07:55:22.000000 github-secret-syncer-0.0.6/setup.py
```

### Comparing `github-secret-syncer-0.0.2/LICENSE` & `github-secret-syncer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.2/github_secret_syncer/__init__.py` & `github-secret-syncer-0.0.6/github_secret_syncer/__init__.py`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.2/setup.py` & `github-secret-syncer-0.0.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import setuptools
+from pathlib import Path
 
+base_dir = Path(__file__).parent.resolve()
+long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="github-secret-syncer",
-    version="0.0.2",
+    version="0.0.6",
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="Github Secret Syncer.",
-    long_description=(
-        "# Github Secret Syncer..\n"
-        "\n"
-        "Synchronize Github secrets with local `.env` file.\n"
-    ),
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thejimmylin/github-secret-syncer",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

