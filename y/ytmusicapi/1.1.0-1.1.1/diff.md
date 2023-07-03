# Comparing `tmp/ytmusicapi-1.1.0.tar.gz` & `tmp/ytmusicapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusicapi-1.1.0.tar", last modified: Thu Jun 15 18:28:45 2023, max compression
+gzip compressed data, was "ytmusicapi-1.1.1.tar", last modified: Mon Jul  3 20:56:51 2023, max compression
```

## Comparing `ytmusicapi-1.1.0.tar` & `ytmusicapi-1.1.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.861526 ytmusicapi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/workflows/docsbuild.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/docs/source/setup/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/browser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/headers_auth.json.example
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:28:45.861526 ytmusicapi-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/tests/test.cfg.example
--rw-r--r--   0 runner    (1001) docker     (123)    22845 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/continuations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/locales/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/update_mo.sh
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/update_po.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/albums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/songs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.994015 ytmusicapi-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-03 20:56:51.994015 ytmusicapi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:56:51.994015 ytmusicapi-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/tests/test.cfg.example
+-rw-r--r--   0 runner    (1001) docker     (123)    22949 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/auth/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/auth/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/nl/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.978014 ytmusicapi-1.1.1/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.982014 ytmusicapi-1.1.1/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.990014 ytmusicapi-1.1.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.994015 ytmusicapi-1.1.1/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.994015 ytmusicapi-1.1.1/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-03 20:56:41.000000 ytmusicapi-1.1.1/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:56:51.986014 ytmusicapi-1.1.1/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-03 20:56:51.000000 ytmusicapi-1.1.1/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-03 20:56:51.000000 ytmusicapi-1.1.1/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:56:51.000000 ytmusicapi-1.1.1/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 20:56:51.000000 ytmusicapi-1.1.1/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 20:56:51.000000 ytmusicapi-1.1.1/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 20:56:51.000000 ytmusicapi-1.1.1/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ytmusicapi-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ytmusicapi-1.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/.github/workflows/coverage.yml` & `ytmusicapi-1.1.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/.github/workflows/pythonpublish.yml` & `ytmusicapi-1.1.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/CONTRIBUTING.rst` & `ytmusicapi-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/LICENSE` & `ytmusicapi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/PKG-INFO` & `ytmusicapi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.1.0/README.rst` & `ytmusicapi-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/Makefile` & `ytmusicapi-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/make.bat` & `ytmusicapi-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/source/conf.py` & `ytmusicapi-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/source/faq.rst` & `ytmusicapi-1.1.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/source/index.rst` & `ytmusicapi-1.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/source/reference.rst` & `ytmusicapi-1.1.1/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/source/setup/browser.rst` & `ytmusicapi-1.1.1/docs/source/setup/browser.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/docs/source/usage.rst` & `ytmusicapi-1.1.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/pyproject.toml` & `ytmusicapi-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/tests/README.rst` & `ytmusicapi-1.1.1/tests/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/tests/test.cfg.example` & `ytmusicapi-1.1.1/tests/test.cfg.example`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/tests/test.py` & `ytmusicapi-1.1.1/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,28 +384,31 @@
         self.yt_auth.subscribe_artists(["UCUDVBtnOQi4c7E8jebpjc9Q", "UCiMhD4jzUqG-IgPzUmmytRQ"])
         self.yt_auth.unsubscribe_artists(["UCUDVBtnOQi4c7E8jebpjc9Q", "UCiMhD4jzUqG-IgPzUmmytRQ"])
 
     ###############
     # PLAYLISTS
     ###############
 
-    def test_get_foreign_playlist(self):
+    def test_get_playlist_foreign(self):
         self.assertRaises(Exception, self.yt.get_playlist, "PLABC")
         playlist = self.yt.get_playlist(sample_playlist, limit=300, suggestions_limit=7)
         self.assertGreater(len(playlist['duration']), 5)
         self.assertGreater(len(playlist["tracks"]), 200)
         self.assertNotIn("suggestions", playlist)
 
+        self.yt.get_playlist("RDATgXd-")
+        self.assertGreaterEqual(len(playlist["tracks"]), 100)
+
         playlist = self.yt_oauth.get_playlist("PLj4BSJLnVpNyIjbCWXWNAmybc97FXLlTk",
                                               limit=None,
                                               related=True)
         self.assertGreater(len(playlist["tracks"]), 200)
         self.assertEqual(len(playlist["related"]), 0)
 
-    def test_get_owned_playlist(self):
+    def test_get_playlist_owned(self):
         playlist = self.yt_brand.get_playlist(config["playlists"]["own"],
                                               related=True,
                                               suggestions_limit=21)
         self.assertLess(len(playlist["tracks"]), 100)
         self.assertEqual(len(playlist["suggestions"]), 21)
         self.assertEqual(len(playlist["related"]), 10)
```

### Comparing `ytmusicapi-1.1.0/ytmusicapi/auth/browser.py` & `ytmusicapi-1.1.1/ytmusicapi/auth/browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/auth/headers.py` & `ytmusicapi-1.1.1/ytmusicapi/auth/headers.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,23 +19,21 @@
 
     return input_json
 
 
 def prepare_headers(
     session: requests.Session,
     proxies: Optional[Dict] = None,
-    auth: Optional[str] = None,
+    input_dict: Optional[CaseInsensitiveDict] = None,
 ) -> Dict:
-    if auth:
-        input_json = load_headers_file(auth)
-        input_dict = CaseInsensitiveDict(input_json)
+    if input_dict:
 
         if is_oauth(input_dict):
             oauth = YTMusicOAuth(session, proxies)
-            headers = oauth.load_headers(dict(input_dict), auth)
+            headers = oauth.load_headers(dict(input_dict), input_dict['filepath'])
 
         elif is_browser(input_dict):
             headers = input_dict
 
         elif is_custom_oauth(input_dict):
             headers = input_dict
```

### Comparing `ytmusicapi-1.1.0/ytmusicapi/auth/oauth.py` & `ytmusicapi-1.1.1/ytmusicapi/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/constants.py` & `ytmusicapi-1.1.1/ytmusicapi/constants.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/continuations.py` & `ytmusicapi-1.1.1/ytmusicapi/continuations.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/helpers.py` & `ytmusicapi-1.1.1/ytmusicapi/helpers.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/README.rst` & `ytmusicapi-1.1.1/ytmusicapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/base.pot` & `ytmusicapi-1.1.1/ytmusicapi/locales/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/en/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/es/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/it/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/nl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/nl/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot` & `ytmusicapi-1.1.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po` & `ytmusicapi-1.1.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/_utils.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/browsing.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/explore.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/library.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/playlists.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,22 +128,27 @@
             playlist['author'] = {
                 'name': nav(header, SUBTITLE2),
                 'id': nav(header, SUBTITLE_RUNS + [2] + NAVIGATION_BROWSE_ID, True)
             }
             if run_count == 5:
                 playlist['year'] = nav(header, SUBTITLE3)
 
-        second_subtitle_runs = header['secondSubtitle']['runs']
+        playlist['views'] = None
+        playlist['duration'] = None
+        if 'runs' in header['secondSubtitle']:
+            second_subtitle_runs = header['secondSubtitle']['runs']
+            has_views = (len(second_subtitle_runs) > 3) * 2
+            playlist['views'] = None if not has_views else to_int(second_subtitle_runs[0]['text'])
+            has_duration = (len(second_subtitle_runs) > 1) * 2
+            playlist['duration'] = None if not has_duration else second_subtitle_runs[has_views + has_duration]['text']
+            song_count = second_subtitle_runs[has_views + 0]['text'].split(" ")
+            song_count = to_int(song_count[0]) if len(song_count) > 1 else 0
+        else:
+            song_count = len(results['contents'])
 
-        has_views = (len(second_subtitle_runs) > 3) * 2
-        playlist['views'] = None if not has_views else to_int(second_subtitle_runs[0]['text'])
-        has_duration = (len(second_subtitle_runs) > 1) * 2
-        playlist['duration'] = None if not has_duration else second_subtitle_runs[has_views + has_duration]['text']
-        song_count = second_subtitle_runs[has_views + 0]['text'].split(" ")
-        song_count = to_int(song_count[0]) if len(song_count) > 1 else 0
         playlist['trackCount'] = song_count
 
         request_func = lambda additionalParams: self._send_request(endpoint, body, additionalParams)
 
         # suggestions and related are missing e.g. on liked songs
         section_list = nav(response, SINGLE_COLUMN_TAB + ['sectionListRenderer'])
         playlist['related'] = []
```

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/search.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/mixins/watch.py` & `ytmusicapi-1.1.1/ytmusicapi/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/navigation.py` & `ytmusicapi-1.1.1/ytmusicapi/navigation.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/_utils.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/albums.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/albums.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/browsing.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/explore.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/i18n.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/i18n.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/library.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/search.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/songs.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/songs.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/parsers/watch.py` & `ytmusicapi-1.1.1/ytmusicapi/parsers/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/setup.py` & `ytmusicapi-1.1.1/ytmusicapi/setup.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.1.0/ytmusicapi/ytmusic.py` & `ytmusicapi-1.1.1/ytmusicapi/ytmusic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import requests
 import gettext
 import os
 from functools import partial
 from contextlib import suppress
 from typing import Dict
 
-from ytmusicapi.auth.headers import prepare_headers
+from requests.structures import CaseInsensitiveDict
+from ytmusicapi.auth.headers import load_headers_file, prepare_headers
 from ytmusicapi.parsers.i18n import Parser
 from ytmusicapi.helpers import *
 from ytmusicapi.mixins.browsing import BrowsingMixin
 from ytmusicapi.mixins.search import SearchMixin
 from ytmusicapi.mixins.watch import WatchMixin
 from ytmusicapi.mixins.explore import ExploreMixin
 from ytmusicapi.mixins.library import LibraryMixin
 from ytmusicapi.mixins.playlists import PlaylistsMixin
 from ytmusicapi.mixins.uploads import UploadsMixin
+from ytmusicapi.auth.oauth import YTMusicOAuth, is_oauth
 
 
 class YTMusic(BrowsingMixin, SearchMixin, WatchMixin, ExploreMixin, LibraryMixin, PlaylistsMixin,
               UploadsMixin):
     """
     Allows automated interactions with YouTube Music by emulating the YouTube web client's requests.
     Permits both authenticated and non-authenticated requests.
@@ -64,28 +66,35 @@
             English will be used by default. Available languages can be checked in
             the ytmusicapi/locales directory.
         :param location: Optional. Can be used to change the location of the user.
             No location will be set by default. This means it is determined by the server.
             Available languages can be checked in the FAQ.
         """
         self.auth = auth
+        self.input_dict = None
+        self.is_oauth_auth = False
 
         if isinstance(requests_session, requests.Session):
             self._session = requests_session
         else:
             if requests_session:  # Build a new session.
                 self._session = requests.Session()
                 self._session.request = partial(self._session.request, timeout=30)
             else:  # Use the Requests API module as a "session".
                 self._session = requests.api
 
         self.proxies = proxies
         self.cookies = {'CONSENT': 'YES+1'}
+        if self.auth is not None:
+            input_json = load_headers_file(self.auth)
+            self.input_dict = CaseInsensitiveDict(input_json)
+            self.input_dict['filepath'] = self.auth
+            self.is_oauth_auth = is_oauth(self.input_dict)
 
-        self.headers = prepare_headers(self._session, proxies, auth)
+        self.headers = prepare_headers(self._session, proxies, self.input_dict)
 
         if 'x-goog-visitor-id' not in self.headers:
             self.headers.update(get_visitor_id(self._send_get_request))
 
         # prepare context
         self.context = initialize_context()
 
@@ -117,15 +126,20 @@
         if self.is_browser_auth:
             try:
                 cookie = self.headers.get('cookie')
                 self.sapisid = sapisid_from_cookie(cookie)
             except KeyError:
                 raise Exception("Your cookie is missing the required value __Secure-3PAPISID")
 
+
+
     def _send_request(self, endpoint: str, body: Dict, additionalParams: str = "") -> Dict:
+
+        if self.is_oauth_auth:
+            self.headers = prepare_headers(self._session, self.proxies, self.input_dict) 
         body.update(self.context)
         params = YTM_PARAMS
         if self.is_browser_auth:
             origin = self.headers.get('origin', self.headers.get('x-origin'))
             self.headers["authorization"] = get_authorization(self.sapisid + ' ' + origin)
             params += YTM_PARAMS_KEY
```

### Comparing `ytmusicapi-1.1.0/ytmusicapi.egg-info/PKG-INFO` & `ytmusicapi-1.1.1/ytmusicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.1.0/ytmusicapi.egg-info/SOURCES.txt` & `ytmusicapi-1.1.1/ytmusicapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

