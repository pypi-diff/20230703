# Comparing `tmp/django-pfx-1.2.dev82.tar.gz` & `tmp/django-pfx-1.2.dev84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pfx-1.2.dev82.tar", last modified: Thu Jun 29 15:29:03 2023, max compression
+gzip compressed data, was "django-pfx-1.2.dev84.tar", last modified: Mon Jul  3 09:13:38 2023, max compression
```

## Comparing `django-pfx-1.2.dev82.tar` & `django-pfx-1.2.dev84.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.704982 django-pfx-1.2.dev82/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-29 15:29:03.704982 django-pfx-1.2.dev82/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.683982 django-pfx-1.2.dev82/django_pfx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-29 15:29:03.000000 django-pfx-1.2.dev82/django_pfx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3417 2023-06-29 15:29:03.000000 django-pfx-1.2.dev82/django_pfx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 15:29:03.000000 django-pfx-1.2.dev82/django_pfx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-29 15:29:03.000000 django-pfx-1.2.dev82/django_pfx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 15:29:03.000000 django-pfx-1.2.dev82/django_pfx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.684982 django-pfx-1.2.dev82/img/
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/img/pfx.png
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/img/pfx.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.684982 django-pfx-1.2.dev82/pfx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.686982 django-pfx-1.2.dev82/pfx/pfxcore/
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.686982 django-pfx-1.2.dev82/pfx/pfxcore/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/apidoc/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/apidoc/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/apidoc/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.687982 django-pfx-1.2.dev82/pfx/pfxcore/decorator/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/decorator/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.687982 django-pfx-1.2.dev82/pfx/pfxcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/http/json_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.678982 django-pfx-1.2.dev82/pfx/pfxcore/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.678982 django-pfx-1.2.dev82/pfx/pfxcore/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.688982 django-pfx-1.2.dev82/pfx/pfxcore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3331 2023-06-29 15:28:59.000000 django-pfx-1.2.dev82/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     5332 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.688982 django-pfx-1.2.dev82/pfx/pfxcore/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.688982 django-pfx-1.2.dev82/pfx/pfxcore/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7237 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/management/commands/makeapidoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.689982 django-pfx-1.2.dev82/pfx/pfxcore/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/middleware/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/middleware/locale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.690982 django-pfx-1.2.dev82/pfx/pfxcore/models/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/models/cache_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/models/not_null_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3419 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/models/pfx_models.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/models/user_filtered_queryset_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.690982 django-pfx-1.2.dev82/pfx/pfxcore/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/serializers/json.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.691982 django-pfx-1.2.dev82/pfx/pfxcore/storage/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/storage/s3_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.679982 django-pfx-1.2.dev82/pfx/pfxcore/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.691982 django-pfx-1.2.dev82/pfx/pfxcore/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/templates/registration/welcome_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/templates/registration/welcome_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)    10198 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/test.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.693982 django-pfx-1.2.dev82/pfx/pfxcore/views/
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11581 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/authentication_views.py
--rw-rw-rw-   0 root         (0) root         (0)    12218 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/filters_views.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/locale_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.697982 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/date_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/list_count.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/list_items.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/list_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/list_order.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/list_search.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/media_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/meta_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/meta_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/meta_orders.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/subset.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/subset_limit.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/subset_offset.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/subset_page.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/subset_page_size.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/subset_page_subset.py
--rw-rw-rw-   0 root         (0) root         (0)    27547 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pfx/pfxcore/views/rest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      440 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/runtest.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-29 15:29:03.704982 django-pfx-1.2.dev82/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.697982 django-pfx-1.2.dev82/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6487 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.699982 django-pfx-1.2.dev82/tests/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/settings/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/settings/dev.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/settings/dev_custom_example.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/settings/dev_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:29:03.703982 django-pfx-1.2.dev82/tests/tests/
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/basic_api_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    46979 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/basic_api_test.py
--rw-rw-rw-   0 root         (0) root         (0)    18097 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_api_doc.py
--rw-rw-rw-   0 root         (0) root         (0)    29106 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     9909 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_locale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_perm_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_perms_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_timezone_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_user_queryset.py
--rw-rw-rw-   0 root         (0) root         (0)     3558 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_view_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/tests/test_view_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8416 2023-06-29 15:28:19.000000 django-pfx-1.2.dev82/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.533832 django-pfx-1.2.dev84/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 09:13:38.533832 django-pfx-1.2.dev84/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.517832 django-pfx-1.2.dev84/django_pfx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.518832 django-pfx-1.2.dev84/img/
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/img/pfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/img/pfx.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.518832 django-pfx-1.2.dev84/pfx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.519832 django-pfx-1.2.dev84/pfx/pfxcore/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.520832 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.520832 django-pfx-1.2.dev84/pfx/pfxcore/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/decorator/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.521832 django-pfx-1.2.dev84/pfx/pfxcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/http/json_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.513831 django-pfx-1.2.dev84/pfx/pfxcore/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.513831 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.521832 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-07-03 09:13:34.000000 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5332 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.521832 django-pfx-1.2.dev84/pfx/pfxcore/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.522832 django-pfx-1.2.dev84/pfx/pfxcore/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7568 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/management/commands/makeapidoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.522832 django-pfx-1.2.dev84/pfx/pfxcore/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/middleware/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/middleware/locale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.523832 django-pfx-1.2.dev84/pfx/pfxcore/models/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/cache_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/not_null_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3419 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/pfx_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/user_filtered_queryset_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.523832 django-pfx-1.2.dev84/pfx/pfxcore/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/serializers/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.524832 django-pfx-1.2.dev84/pfx/pfxcore/storage/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/storage/s3_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.514832 django-pfx-1.2.dev84/pfx/pfxcore/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.524832 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/welcome_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/welcome_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)    10198 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.525832 django-pfx-1.2.dev84/pfx/pfxcore/views/
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11581 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/authentication_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    12218 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/filters_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/locale_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.528832 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/date_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_order.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/media_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/meta_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/meta_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/meta_orders.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_offset.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_page_size.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_page_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27547 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/rest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      440 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/runtest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-03 09:13:38.534832 django-pfx-1.2.dev84/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.529832 django-pfx-1.2.dev84/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.530832 django-pfx-1.2.dev84/tests/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/dev_custom_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/dev_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.533832 django-pfx-1.2.dev84/tests/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/basic_api_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    46979 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/basic_api_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    18097 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_api_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)    29106 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9909 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_locale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_perm_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_perms_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_timezone_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_user_queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3558 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_view_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_view_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8416 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/views.py
```

### Comparing `django-pfx-1.2.dev82/.gitlab-ci.yml` & `django-pfx-1.2.dev84/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/LICENSE` & `django-pfx-1.2.dev84/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/PKG-INFO` & `django-pfx-1.2.dev84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev82
+Version: 1.2.dev84
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev82/README.md` & `django-pfx-1.2.dev84/README.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/django_pfx.egg-info/PKG-INFO` & `django-pfx-1.2.dev84/django_pfx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev82
+Version: 1.2.dev84
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev82/django_pfx.egg-info/SOURCES.txt` & `django-pfx-1.2.dev84/django_pfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/img/pfx.png` & `django-pfx-1.2.dev84/img/pfx.png`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/img/pfx.svg` & `django-pfx-1.2.dev84/img/pfx.svg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/apidoc/parameters.py` & `django-pfx-1.2.dev84/pfx/pfxcore/apidoc/parameters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/apidoc/schema.py` & `django-pfx-1.2.dev84/pfx/pfxcore/apidoc/schema.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/decorator/rest.py` & `django-pfx-1.2.dev84/pfx/pfxcore/decorator/rest.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/exceptions.py` & `django-pfx-1.2.dev84/pfx/pfxcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/fields.py` & `django-pfx-1.2.dev84/pfx/pfxcore/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo` & `django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/management/commands/makeapidoc.py` & `django-pfx-1.2.dev84/pfx/pfxcore/management/commands/makeapidoc.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,18 +184,26 @@
 
 
 class Command(BaseCommand):
     help = 'Generate OpenAPI documentation'
 
     def add_arguments(self, parser):
         parser.add_argument("groups", nargs="*", type=str)
+        parser.add_argument(
+            "-f", "--format", dest="format", choices=['json', 'yaml'],
+            default="json", type=str)
 
     def handle(self, *args, groups=None, **options):
         spec = get_spec(set(groups))
 
-        path = Path(settings.PFX_OPENAPI_PATH)
+        path = Path(
+            settings.PFX_OPENAPI_PATH,
+            f'{settings.PFX_OPENAPI_FILENAME}.{options["format"]}')
         path.parent.mkdir(parents=True, exist_ok=True)
         with open(path, "w") as outfile:
-            json.dump(spec.to_dict(), outfile, indent=2)
+            if options["format"] == 'yaml':
+                outfile.write(spec.to_yaml())
+            else:
+                json.dump(spec.to_dict(), outfile, indent=2)
 
         self.stdout.write(self.style.SUCCESS(
             f"OpenAPI documentation generated: {path}"))
```

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/middleware/authentication.py` & `django-pfx-1.2.dev84/pfx/pfxcore/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/middleware/locale.py` & `django-pfx-1.2.dev84/pfx/pfxcore/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/models/cache_mixins.py` & `django-pfx-1.2.dev84/pfx/pfxcore/models/cache_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/models/pfx_models.py` & `django-pfx-1.2.dev84/pfx/pfxcore/models/pfx_models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/shortcuts.py` & `django-pfx-1.2.dev84/pfx/pfxcore/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/storage/s3_storage.py` & `django-pfx-1.2.dev84/pfx/pfxcore/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/test.py` & `django-pfx-1.2.dev84/pfx/pfxcore/test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/__init__.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/authentication_views.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/authentication_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/fields.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/filters_views.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/filters_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/locale_views.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/locale_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/__init__.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/date_format.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/date_format.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/groups.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/list_order.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_order.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/parameters/subset.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/pfx/pfxcore/views/rest_views.py` & `django-pfx-1.2.dev84/pfx/pfxcore/views/rest_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/setup.cfg` & `django-pfx-1.2.dev84/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/models.py` & `django-pfx-1.2.dev84/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/settings/common.py` & `django-pfx-1.2.dev84/tests/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/settings/dev_custom_example.py` & `django-pfx-1.2.dev84/tests/settings/dev_custom_example.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/__init__.py` & `django-pfx-1.2.dev84/tests/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/basic_api_errors.py` & `django-pfx-1.2.dev84/tests/tests/basic_api_errors.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/basic_api_test.py` & `django-pfx-1.2.dev84/tests/tests/basic_api_test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_api_doc.py` & `django-pfx-1.2.dev84/tests/tests/test_api_doc.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_auth_api.py` & `django-pfx-1.2.dev84/tests/tests/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_cache.py` & `django-pfx-1.2.dev84/tests/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_fields.py` & `django-pfx-1.2.dev84/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_filters.py` & `django-pfx-1.2.dev84/tests/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_locale_api.py` & `django-pfx-1.2.dev84/tests/tests/test_locale_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_perm_tests.py` & `django-pfx-1.2.dev84/tests/tests/test_perm_tests.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_perms_api.py` & `django-pfx-1.2.dev84/tests/tests/test_perms_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_shortcuts.py` & `django-pfx-1.2.dev84/tests/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_timezone_middleware.py` & `django-pfx-1.2.dev84/tests/tests/test_timezone_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_tools.py` & `django-pfx-1.2.dev84/tests/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_user_queryset.py` & `django-pfx-1.2.dev84/tests/tests/test_user_queryset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_view_decorators.py` & `django-pfx-1.2.dev84/tests/tests/test_view_decorators.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/tests/test_view_fields.py` & `django-pfx-1.2.dev84/tests/tests/test_view_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/urls.py` & `django-pfx-1.2.dev84/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev82/tests/views.py` & `django-pfx-1.2.dev84/tests/views.py`

 * *Files identical despite different names*

