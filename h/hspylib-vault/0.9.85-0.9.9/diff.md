# Comparing `tmp/hspylib-vault-0.9.85.tar.gz` & `tmp/hspylib-vault-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-vault-0.9.85.tar", last modified: Mon Jul  3 20:38:22 2023, max compression
+gzip compressed data, was "hspylib-vault-0.9.9.tar", last modified: Tue Feb 22 20:01:27 2022, max compression
```

## Comparing `hspylib-vault-0.9.85.tar` & `hspylib-vault-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:38:22.354514 hspylib-vault-0.9.85/
--rw-r--r--   0 hjunior    (504) staff       (20)       96 2022-06-17 15:16:57.000000 hspylib-vault-0.9.85/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-07-03 20:38:22.353504 hspylib-vault-0.9.85/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      675 2023-07-03 20:38:21.000000 hspylib-vault-0.9.85/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:38:22.295669 hspylib-vault-0.9.85/hspylib_vault.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-07-03 20:38:22.000000 hspylib-vault-0.9.85/hspylib_vault.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      585 2023-07-03 20:38:22.000000 hspylib-vault-0.9.85/hspylib_vault.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-03 20:38:22.000000 hspylib-vault-0.9.85/hspylib_vault.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-07-03 20:38:22.000000 hspylib-vault-0.9.85/hspylib_vault.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-03 20:38:22.000000 hspylib-vault-0.9.85/hspylib_vault.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-03 20:38:22.354709 hspylib-vault-0.9.85/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1854 2023-04-19 22:13:51.000000 hspylib-vault-0.9.85/setup.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:38:22.322429 hspylib-vault-0.9.85/vault/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-03 20:38:21.000000 hspylib-vault-0.9.85/vault/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:58.000000 hspylib-vault-0.9.85/vault/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      180 2023-07-03 20:38:21.000000 hspylib-vault-0.9.85/vault/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5147 2023-04-19 22:13:51.000000 hspylib-vault-0.9.85/vault/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:38:22.338020 hspylib-vault-0.9.85/vault/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      219 2023-07-03 20:38:21.000000 hspylib-vault-0.9.85/vault/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)    13235 2023-06-16 21:19:22.000000 hspylib-vault-0.9.85/vault/core/vault.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1395 2023-04-19 22:18:03.000000 hspylib-vault-0.9.85/vault/core/vault_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1852 2023-04-19 22:18:03.000000 hspylib-vault-0.9.85/vault/core/vault_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2358 2023-04-19 22:18:03.000000 hspylib-vault-0.9.85/vault/core/vault_service.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:38:22.344431 hspylib-vault-0.9.85/vault/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      165 2023-07-03 20:38:21.000000 hspylib-vault-0.9.85/vault/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3466 2023-04-19 22:18:03.000000 hspylib-vault-0.9.85/vault/domain/vault_entry.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:38:22.350182 hspylib-vault-0.9.85/vault/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-03 20:38:21.000000 hspylib-vault-0.9.85/vault/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      839 2023-04-19 22:01:58.000000 hspylib-vault-0.9.85/vault/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:38:22.352219 hspylib-vault-0.9.85/vault/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-11-12 19:14:13.000000 hspylib-vault-0.9.85/vault/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      168 2023-04-19 21:58:35.000000 hspylib-vault-0.9.85/vault/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.651843 hspylib-vault-0.9.9/
+-rw-r--r--   0 hjunior    (504) staff       (20)      125 2022-02-18 20:26:39.000000 hspylib-vault-0.9.9/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)      662 2022-02-22 20:01:27.650723 hspylib-vault-0.9.9/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2022-02-13 18:46:58.000000 hspylib-vault-0.9.9/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.604944 hspylib-vault-0.9.9/hspylib_vault.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)      662 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      704 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       57 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2022-02-22 20:01:27.651948 hspylib-vault-0.9.9/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1557 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.615812 hspylib-vault-0.9.9/vault/
+-rw-r--r--   0 hjunior    (504) staff       (20)        5 2022-02-22 20:01:25.000000 hspylib-vault-0.9.9/vault/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      193 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4384 2022-02-18 21:07:53.000000 hspylib-vault-0.9.9/vault/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.624864 hspylib-vault-0.9.9/vault/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      217 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     8712 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1315 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/core/vault_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2160 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1089 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault_service.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.628367 hspylib-vault-0.9.9/vault/entity/
+-rw-r--r--   0 hjunior    (504) staff       (20)      179 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/entity/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.631698 hspylib-vault-0.9.9/vault/entity/validator/
+-rw-r--r--   0 hjunior    (504) staff       (20)      177 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/entity/validator/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2231 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/entity/validator/entry_validator.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2128 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/entity/vault_entry.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.634841 hspylib-vault-0.9.9/vault/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      165 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      627 2022-02-11 19:26:38.000000 hspylib-vault-0.9.9/vault/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.642361 hspylib-vault-0.9.9/vault/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/resources/application.properties
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.649219 hspylib-vault-0.9.9/vault/resources/log/
+-rw-r--r--   0 hjunior    (504) staff       (20)        0 2022-02-02 16:37:07.000000 hspylib-vault-0.9.9/vault/resources/log/.gitkeep
+-rw-r--r--   0 hjunior    (504) staff       (20)     2572 2022-02-21 23:29:30.000000 hspylib-vault-0.9.9/vault/resources/log/application.log
+-rw-r--r--   0 hjunior    (504) staff       (20)      168 2022-02-18 20:29:20.000000 hspylib-vault-0.9.9/vault/welcome.txt
```

### Comparing `hspylib-vault-0.9.85/hspylib_vault.egg-info/SOURCES.txt` & `hspylib-vault-0.9.9/hspylib_vault.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 setup.py
 hspylib_vault.egg-info/PKG-INFO
 hspylib_vault.egg-info/SOURCES.txt
 hspylib_vault.egg-info/dependency_links.txt
 hspylib_vault.egg-info/requires.txt
 hspylib_vault.egg-info/top_level.txt
 vault/.version
-vault/__classpath__.py
 vault/__init__.py
 vault/__main__.py
 vault/welcome.txt
 vault/core/__init__.py
 vault/core/vault.py
 vault/core/vault_config.py
 vault/core/vault_repository.py
 vault/core/vault_service.py
-vault/domain/__init__.py
-vault/domain/vault_entry.py
+vault/entity/__init__.py
+vault/entity/vault_entry.py
+vault/entity/validator/__init__.py
+vault/entity/validator/entry_validator.py
 vault/exception/__init__.py
 vault/exception/exceptions.py
-vault/resources/application.properties
+vault/resources/application.properties
+vault/resources/log/.gitkeep
+vault/resources/log/application.log
```

### Comparing `hspylib-vault-0.9.85/vault/exception/exceptions.py` & `hspylib-vault-0.9.9/vault/exception/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HsPyLib-Vault
-   @package: vault.exception
+   TODO Purpose of the file
+   @project: HSPyLib
+   hspylib.app.vault.exception
       @file: exceptions.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2023, HsPyLib team
+   Copyright 2021, HSPyLib team
 """
 from hspylib.core.exception.exceptions import HSBaseException
 
 
 class VaultCloseError(HSBaseException):
     """Raised when closing the vault"""
 
 
 class VaultOpenError(HSBaseException):
     """Raised when opening the vault"""
-
-
-class VaultSecurityException(HSBaseException):
-    """Raised when something unexpected happened to vault file"""
-
-
-class VaultExecutionException(HSBaseException):
-    """Raised when something unexpected happened to vault execution"""
```

