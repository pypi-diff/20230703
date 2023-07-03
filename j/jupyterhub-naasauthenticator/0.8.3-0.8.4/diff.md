# Comparing `tmp/jupyterhub-naasauthenticator-0.8.3.tar.gz` & `tmp/jupyterhub-naasauthenticator-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-naasauthenticator-0.8.3.tar", last modified: Sat Jul  1 07:56:06 2023, max compression
+gzip compressed data, was "jupyterhub-naasauthenticator-0.8.4.tar", last modified: Mon Jul  3 07:27:55 2023, max compression
```

## Comparing `jupyterhub-naasauthenticator-0.8.3.tar` & `jupyterhub-naasauthenticator-0.8.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/
--rw-r--r--   0 root         (0) root         (0)     1510 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      166 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1121 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      789 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.580546 jupyterhub-naasauthenticator-0.8.3/docs/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.588546 jupyterhub-naasauthenticator-0.8.3/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   188847 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/authorization_area.png
--rw-r--r--   0 root         (0) root         (0)  2487640 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/block_user_failed_logins.png
--rw-r--r--   0 root         (0) root         (0)   161847 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/change-password.png
--rw-r--r--   0 root         (0) root         (0)    85574 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/login-two-factor-auth.png
--rw-r--r--   0 root         (0) root         (0)  1355938 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/native_auth_flow.png
--rw-r--r--   0 root         (0) root         (0)    91790 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/signup-two-factor-auth.png
--rw-r--r--   0 root         (0) root         (0)    78767 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/wrong_signup.png
--rw-r--r--   0 root         (0) root         (0)     5390 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     4785 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/options.rst
--rw-r--r--   0 root         (0) root         (0)     2979 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/quickstart.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.588546 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1121 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1462 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.588546 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76508 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/common-credentials.txt
--rw-r--r--   0 root         (0) root         (0)    18595 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/handlers.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/naasauthenticator.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/orm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/admin.html
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/autorization-area.html
--rw-r--r--   0 root         (0) root         (0)     1561 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/change-password.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/home.html
--rw-r--r--   0 root         (0) root         (0)     6580 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/native-login.html
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/not_running.html
--rw-r--r--   0 root         (0) root         (0)     3502 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/page.html
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/reset-password.html
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/spawn.html
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/spawn_pending.html
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/stop_pending.html
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/token.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7607 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_authenticator.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_orm.py
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      874 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:27:55.337815 jupyterhub-naasauthenticator-0.8.4/
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-03 07:27:55.337815 jupyterhub-naasauthenticator-0.8.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      789 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:27:55.321815 jupyterhub-naasauthenticator-0.8.4/docs/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:27:55.329815 jupyterhub-naasauthenticator-0.8.4/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   188847 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/_static/authorization_area.png
+-rw-r--r--   0 root         (0) root         (0)  2487640 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/_static/block_user_failed_logins.png
+-rw-r--r--   0 root         (0) root         (0)   161847 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/_static/change-password.png
+-rw-r--r--   0 root         (0) root         (0)    85574 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/_static/login-two-factor-auth.png
+-rw-r--r--   0 root         (0) root         (0)  1355938 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/_static/native_auth_flow.png
+-rw-r--r--   0 root         (0) root         (0)    91790 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/_static/signup-two-factor-auth.png
+-rw-r--r--   0 root         (0) root         (0)    78767 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/_static/wrong_signup.png
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/options.rst
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/docs/quickstart.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:27:55.329815 jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-03 07:27:55.000000 jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-07-03 07:27:55.000000 jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 07:27:55.000000 jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-03 07:27:55.000000 jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 07:27:55.000000 jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:27:55.333815 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76508 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/common-credentials.txt
+-rw-r--r--   0 root         (0) root         (0)    18595 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/handlers.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/naasauthenticator.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/orm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:27:55.337815 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/admin.html
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/autorization-area.html
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/change-password.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/home.html
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/native-login.html
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/not_running.html
+-rw-r--r--   0 root         (0) root         (0)     3502 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/page.html
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/reset-password.html
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/spawn.html
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/spawn_pending.html
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/stop_pending.html
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/token.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:27:55.337815 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7607 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/tests/test_authenticator.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/naasauthenticator/tests/test_orm.py
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-03 07:27:55.337815 jupyterhub-naasauthenticator-0.8.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      874 2023-07-03 07:27:07.000000 jupyterhub-naasauthenticator-0.8.4/setup.py
```

### Comparing `jupyterhub-naasauthenticator-0.8.3/LICENSE` & `jupyterhub-naasauthenticator-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/PKG-INFO` & `jupyterhub-naasauthenticator-0.8.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-naasauthenticator
-Version: 0.8.3
+Version: 0.8.4
 Summary: JupyterHub Native Authenticator
 Home-page: https://github.com/cashstory/naasauthenticator
 Author: Martin DONADIEU
 Author-email: bob@cashstory.com
 License: 3 Clause BSD
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `jupyterhub-naasauthenticator-0.8.3/README.md` & `jupyterhub-naasauthenticator-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/Makefile` & `jupyterhub-naasauthenticator-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/_static/authorization_area.png` & `jupyterhub-naasauthenticator-0.8.4/docs/_static/authorization_area.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/_static/block_user_failed_logins.png` & `jupyterhub-naasauthenticator-0.8.4/docs/_static/block_user_failed_logins.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/_static/change-password.png` & `jupyterhub-naasauthenticator-0.8.4/docs/_static/change-password.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/_static/login-two-factor-auth.png` & `jupyterhub-naasauthenticator-0.8.4/docs/_static/login-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/_static/native_auth_flow.png` & `jupyterhub-naasauthenticator-0.8.4/docs/_static/native_auth_flow.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/_static/signup-two-factor-auth.png` & `jupyterhub-naasauthenticator-0.8.4/docs/_static/signup-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/_static/wrong_signup.png` & `jupyterhub-naasauthenticator-0.8.4/docs/_static/wrong_signup.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/conf.py` & `jupyterhub-naasauthenticator-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/index.rst` & `jupyterhub-naasauthenticator-0.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/make.bat` & `jupyterhub-naasauthenticator-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/options.rst` & `jupyterhub-naasauthenticator-0.8.4/docs/options.rst`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/docs/quickstart.rst` & `jupyterhub-naasauthenticator-0.8.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/PKG-INFO` & `jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-naasauthenticator
-Version: 0.8.3
+Version: 0.8.4
 Summary: JupyterHub Native Authenticator
 Home-page: https://github.com/cashstory/naasauthenticator
 Author: Martin DONADIEU
 Author-email: bob@cashstory.com
 License: 3 Clause BSD
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/SOURCES.txt` & `jupyterhub-naasauthenticator-0.8.4/jupyterhub_naasauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/common-credentials.txt` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/common-credentials.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/handlers.py` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/naasauthenticator.py` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/naasauthenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/orm.py` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/autorization-area.html` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/autorization-area.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/change-password.html` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/change-password.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/native-login.html` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/native-login.html`

 * *Files 2% similar despite different names*

```diff
@@ -119,21 +119,21 @@
             </a>
             <a id="github-button" href="{{auth_url}}/login/github?next={{next}}" class="btn btn-block custom-button">
                 <img src="{{base_url}}/static/images/custom/github.svg" alt="Github logo" class="icon"> Continue with Github
             </a>
             <a id="linkedin-button" href="{{auth_url}}/login/linkedin?next={{next}}" class="btn btn-block custom-button">
                 <img src="{{base_url}}/static/images/custom/linkedin.svg" alt="Linkedins logo" class="icon"> Continue with Linkedin
             </a>
-            {% if landing_url %}
+            <!-- {% if landing_url %}
             <div style="padding-top: 25px">
                 <p style="text-align: center;">
                     Need account? <a href="{{ landing_url }}" target="_blank">Create one</a>
                 </p>
             </div>
-            {% endif %}
+            {% endif %} -->
             <div class="separator">
                 <span class="separator-text">or</span>
             </div>
             <p style="text-align: center"> For legacy users </p>
 
             <label for="username_input">Username</label>
             <input id="username_input" type="text" autocapitalize="off" autocorrect="off" class="form-control custom-input"
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
 {% extends "page.html" %} {% block nav_bar %} {% endblock %} {% block main %}
 {% if announcement_login %} {% set announcement = announcement_login %} {%
 endif %}
 _[Naas]
  {% if login_error %}
 {{login_error}}
 {% endif %} [Google_logo]_Continue_with_Google [Github_logo]_Continue_with
-Github [Linkedins_logo]_Continue_with_Linkedin {% if landing_url %}
-Need account? Create_one
-{% endif %}
+Github [Linkedins_logo]_Continue_with_Linkedin
 or
 For legacy users
 Username [username            ]
 Password Forgot_Password?  [********************]   ð    [Login]
 By continuing, you agree with Naas's Terms_of_Service.
 and Privacy_Policy
 {% endblock %} {% block script %} {{ super() }}
```

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/page.html` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/page.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/reset-password.html` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/reset-password.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/spawn_pending.html` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/templates/spawn_pending.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_authenticator.py` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_orm.py` & `jupyterhub-naasauthenticator-0.8.4/naasauthenticator/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.8.3/setup.py` & `jupyterhub-naasauthenticator-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="jupyterhub-naasauthenticator",
-    version="0.8.3",
+    version="0.8.4",
     description="JupyterHub Native Authenticator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cashstory/naasauthenticator",
     author="Martin DONADIEU",
     author_email="bob@cashstory.com",
     license="3 Clause BSD",
```

