# Comparing `tmp/home_assistant_streamdeck_yaml-2023.5.1.tar.gz` & `tmp/home_assistant_streamdeck_yaml-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_streamdeck_yaml-2023.5.1.tar", last modified: Mon May 22 23:34:56 2023, max compression
+gzip compressed data, was "home_assistant_streamdeck_yaml-2023.7.0.tar", last modified: Mon Jul  3 16:52:57 2023, max compression
```

## Comparing `home_assistant_streamdeck_yaml-2023.5.1.tar` & `home_assistant_streamdeck_yaml-2023.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:34:56.234029 home_assistant_streamdeck_yaml-2023.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.github/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/toc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/update-readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/fireplace.png
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/hogwarts.png
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/netflix.png
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/night_sky.png
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/space-heater.png
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/spotify.png
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/assets/xbox.png
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-05-22 23:34:56.000000 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-22 23:34:56.000000 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:34:56.000000 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-22 23:34:56.000000 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-22 23:34:56.000000 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 23:34:56.000000 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    59997 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/systemd/home-assistant-streamdeck-yaml.service
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/systemd/restart
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/systemd/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/systemd/status
--rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/systemd/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:34:56.238029 home_assistant_streamdeck_yaml-2023.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/tests/state.json
--rw-r--r--   0 runner    (1001) docker     (123)    35391 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-05-22 23:34:37.000000 home_assistant_streamdeck_yaml-2023.5.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:52:57.249857 home_assistant_streamdeck_yaml-2023.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:52:57.241856 home_assistant_streamdeck_yaml-2023.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.github/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:52:57.245856 home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/toc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/update-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-03 16:52:57.249857 home_assistant_streamdeck_yaml-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:52:57.245856 home_assistant_streamdeck_yaml-2023.7.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/fireplace.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/hogwarts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/netflix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/night_sky.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/space-heater.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/assets/xbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:52:57.245856 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-03 16:52:57.000000 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-03 16:52:57.000000 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:52:57.000000 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-03 16:52:57.000000 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 16:52:57.000000 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 16:52:57.000000 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59997 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:52:57.249857 home_assistant_streamdeck_yaml-2023.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:52:57.245856 home_assistant_streamdeck_yaml-2023.7.0/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/systemd/home-assistant-streamdeck-yaml.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/systemd/restart
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/systemd/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/systemd/status
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/systemd/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:52:57.249857 home_assistant_streamdeck_yaml-2023.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/tests/state.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35391 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-07-03 16:52:37.000000 home_assistant_streamdeck_yaml-2023.7.0/tests/test_examples.py
```

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/.github/release.py` & `home_assistant_streamdeck_yaml-2023.7.0/.github/release.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/docker-build.yml` & `home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/pytest.yml` & `home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/release.yml` & `home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/.github/workflows/update-readme.yml` & `home_assistant_streamdeck_yaml-2023.7.0/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/.gitignore` & `home_assistant_streamdeck_yaml-2023.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/.pre-commit-config.yaml` & `home_assistant_streamdeck_yaml-2023.7.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
       - id: mixed-line-ending
   - repo: "https://github.com/ambv/black"
     rev: 23.3.0
     hooks:
       - id: black-jupyter
         language_version: python3
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.269"
+    rev: "v0.0.270"
     hooks:
       - id: ruff
         args: ["--fix"]
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.3.0"
     hooks:
       - id: mypy
```

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/Dockerfile` & `home_assistant_streamdeck_yaml-2023.7.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/LICENSE` & `home_assistant_streamdeck_yaml-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home_assistant_streamdeck_yaml
-Version: 2023.5.1
+Version: 2023.7.0
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/README.md` & `home_assistant_streamdeck_yaml-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/Roboto-Regular.ttf` & `home_assistant_streamdeck_yaml-2023.7.0/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/fireplace.png` & `home_assistant_streamdeck_yaml-2023.7.0/assets/fireplace.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/hogwarts.png` & `home_assistant_streamdeck_yaml-2023.7.0/assets/hogwarts.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/netflix.png` & `home_assistant_streamdeck_yaml-2023.7.0/assets/netflix.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/night_sky.png` & `home_assistant_streamdeck_yaml-2023.7.0/assets/night_sky.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/space-heater.png` & `home_assistant_streamdeck_yaml-2023.7.0/assets/space-heater.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/spotify.png` & `home_assistant_streamdeck_yaml-2023.7.0/assets/spotify.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/assets/xbox.png` & `home_assistant_streamdeck_yaml-2023.7.0/assets/xbox.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/configuration.yaml` & `home_assistant_streamdeck_yaml-2023.7.0/configuration.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-streamdeck-yaml
-Version: 2023.5.1
+Version: 2023.7.0
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt` & `home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/home_assistant_streamdeck_yaml.py` & `home_assistant_streamdeck_yaml-2023.7.0/home_assistant_streamdeck_yaml.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/pyproject.toml` & `home_assistant_streamdeck_yaml-2023.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dynamic = ["version"]
 authors = [{ name = "Bas Nijholt", email = "bas@nijho.lt" }]
 dependencies = [
     "cairosvg",
     "jinja2",
     "lxml",
     "pillow",
-    "pydantic",
+    "pydantic<2",
     "python-dotenv",
     "pyyaml",
     "requests",
     "rich",
     "streamdeck",
     "websockets",
 ]
```

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/systemd/home-assistant-streamdeck-yaml.service` & `home_assistant_streamdeck_yaml-2023.7.0/systemd/home-assistant-streamdeck-yaml.service`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/tests/state.json` & `home_assistant_streamdeck_yaml-2023.7.0/tests/state.json`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/tests/test_app.py` & `home_assistant_streamdeck_yaml-2023.7.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.5.1/tests/test_examples.py` & `home_assistant_streamdeck_yaml-2023.7.0/tests/test_examples.py`

 * *Files identical despite different names*

