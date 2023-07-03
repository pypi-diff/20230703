# Comparing `tmp/collective.volto.blocksfield-1.0.3.tar.gz` & `tmp/collective.volto.blocksfield-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.volto.blocksfield-1.0.3.tar", last modified: Tue May 31 08:03:57 2022, max compression
+gzip compressed data, was "collective.volto.blocksfield-2.0.0.tar", last modified: Mon Jul  3 09:30:25 2023, max compression
```

## Comparing `collective.volto.blocksfield-1.0.3.tar` & `collective.volto.blocksfield-2.0.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.963969 collective.volto.blocksfield-1.0.3/
--rw-r--r--   0 cekk       (501) staff       (20)     1926 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/.gitlab-ci.yml
--rw-r--r--   0 cekk       (501) staff       (20)     1213 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/.travis.yml
--rw-r--r--   0 cekk       (501) staff       (20)      434 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      679 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      109 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     3882 2022-05-31 08:03:57.964112 collective.volto.blocksfield-1.0.3/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     1406 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.953445 collective.volto.blocksfield-1.0.3/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7947 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)      107 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       50 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      321 2022-05-31 08:03:57.964566 collective.volto.blocksfield-1.0.3/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2571 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.947471 collective.volto.blocksfield-1.0.3/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.953680 collective.volto.blocksfield-1.0.3/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.956031 collective.volto.blocksfield-1.0.3/src/collective/volto/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.957976 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/
--rw-r--r--   0 cekk       (501) staff       (20)      145 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.958835 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/adapters/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/adapters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      347 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/adapters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1569 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/adapters/searchabletext_indexers.py
--rw-r--r--   0 cekk       (501) staff       (20)      444 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      903 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/field.py
--rw-r--r--   0 cekk       (501) staff       (20)      156 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.959981 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/collective.volto.blocksfield.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.948343 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.960470 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)       28 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/en/LC_MESSAGES/collective.volto.blocksfield.mo
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/en/LC_MESSAGES/collective.volto.blocksfield.po
--rw-r--r--   0 cekk       (501) staff       (20)     1764 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      521 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      260 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.960896 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      297 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.961930 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1378 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      720 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1517 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/dxfields.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.962864 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/serializers/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/serializers/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      843 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/serializers/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      452 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/serializers/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1577 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/serializers/dxfields.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.963580 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/types/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/types/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      635 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/types/adapters.py
--rw-r--r--   0 cekk       (501) staff       (20)      227 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/types/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      629 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1324 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.963811 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-05-31 08:03:57.955801 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     3882 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2569 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      153 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       28 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      173 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2022-05-31 08:03:57.000000 collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.188479 collective.volto.blocksfield-2.0.0/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1926 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/.gitlab-ci.yml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1213 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/.travis.yml
+-rw-r--r--   0 lucabel    (501) staff       (20)      621 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       73 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      586 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      679 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      109 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)     3226 2023-07-03 09:30:25.188579 collective.volto.blocksfield-2.0.0/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     1406 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       27 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/constraints.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/constraints_plone52.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.176992 collective.volto.blocksfield-2.0.0/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7947 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      107 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       50 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      321 2023-07-03 09:30:25.188980 collective.volto.blocksfield-2.0.0/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2571 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.171398 collective.volto.blocksfield-2.0.0/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.177327 collective.volto.blocksfield-2.0.0/src/collective/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.180183 collective.volto.blocksfield-2.0.0/src/collective/volto/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.181933 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/
+-rw-r--r--   0 lucabel    (501) staff       (20)      145 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.182585 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      257 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1566 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/adapters/searchabletext_indexers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      444 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      903 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/field.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      156 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.183682 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/collective.volto.blocksfield.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.172120 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.183930 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/en/LC_MESSAGES/collective.volto.blocksfield.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     1764 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      521 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      260 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.185042 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      297 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.186294 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1378 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/blocks.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      720 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1517 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/dxfields.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.187415 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/serializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      843 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/serializers/blocks.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      452 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/serializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1577 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/serializers/dxfields.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.188096 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      635 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/types/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      227 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      629 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1324 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.188330 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:24.000000 collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/tests/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-03 09:30:25.179953 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3226 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     2481 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      133 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       28 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      173 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       11 2023-07-03 09:30:25.000000 collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/top_level.txt
```

### Comparing `collective.volto.blocksfield-1.0.3/.gitlab-ci.yml` & `collective.volto.blocksfield-2.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/.travis.yml` & `collective.volto.blocksfield-2.0.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/DEVELOP.rst` & `collective.volto.blocksfield-2.0.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/LICENSE.GPL` & `collective.volto.blocksfield-2.0.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/LICENSE.rst` & `collective.volto.blocksfield-2.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/README.rst` & `collective.volto.blocksfield-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/docs/conf.py` & `collective.volto.blocksfield-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/setup.py` & `collective.volto.blocksfield-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='collective.volto.blocksfield',
-    version='1.0.3',
+    version='2.0.0',
     description="Field that allows to use blocks instead rich text",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/adapters/searchabletext_indexers.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/adapters/searchabletext_indexers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
-from collective.dexteritytextindexer.converters import (
-    DefaultDexterityTextIndexFieldConverter,
+
+from plone.app.dexterity.textindexer.converters import (
+DefaultDexterityTextIndexFieldConverter,
 )
-from collective.dexteritytextindexer.interfaces import (
+from plone.app.dexterity.textindexer.interfaces import (
     IDexterityTextIndexFieldConverter,
 )
 from collective.volto.blocksfield.interfaces import IBlocksField
 from plone.dexterity.interfaces import IDexterityContent
 from plone.restapi.interfaces import IBlockSearchableText
 from z3c.form.interfaces import IWidget
 from zope.component import adapter
```

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/field.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/field.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/README.rst` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/update.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/locales/update.sh` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/blocks.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/blocks.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/configure.zcml` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/deserializers/dxfields.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/deserializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/serializers/blocks.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/serializers/blocks.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/serializers/dxfields.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/serializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/restapi/types/adapters.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/restapi/types/adapters.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/setuphandlers.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective/volto/blocksfield/testing.py` & `collective.volto.blocksfield-2.0.0/src/collective/volto/blocksfield/testing.py`

 * *Files identical despite different names*

### Comparing `collective.volto.blocksfield-1.0.3/src/collective.volto.blocksfield.egg-info/SOURCES.txt` & `collective.volto.blocksfield-2.0.0/src/collective.volto.blocksfield.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 src/collective/volto/blocksfield/adapters/configure.zcml
 src/collective/volto/blocksfield/adapters/searchabletext_indexers.py
 src/collective/volto/blocksfield/locales/README.rst
 src/collective/volto/blocksfield/locales/__init__.py
 src/collective/volto/blocksfield/locales/collective.volto.blocksfield.pot
 src/collective/volto/blocksfield/locales/update.py
 src/collective/volto/blocksfield/locales/update.sh
-src/collective/volto/blocksfield/locales/en/LC_MESSAGES/collective.volto.blocksfield.mo
 src/collective/volto/blocksfield/locales/en/LC_MESSAGES/collective.volto.blocksfield.po
 src/collective/volto/blocksfield/restapi/__init__.py
 src/collective/volto/blocksfield/restapi/configure.zcml
 src/collective/volto/blocksfield/restapi/deserializers/__init__.py
 src/collective/volto/blocksfield/restapi/deserializers/blocks.py
 src/collective/volto/blocksfield/restapi/deserializers/configure.zcml
 src/collective/volto/blocksfield/restapi/deserializers/dxfields.py
```

