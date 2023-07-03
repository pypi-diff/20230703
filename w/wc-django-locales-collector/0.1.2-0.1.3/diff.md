# Comparing `tmp/wc-django-locales-collector-0.1.2.tar.gz` & `tmp/wc-django-locales-collector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-locales-collector-0.1.2.tar", last modified: Thu Dec 22 11:37:12 2022, max compression
+gzip compressed data, was "wc-django-locales-collector-0.1.3.tar", last modified: Mon Jul  3 09:02:23 2023, max compression
```

## Comparing `wc-django-locales-collector-0.1.2.tar` & `wc-django-locales-collector-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-22 11:37:12.773189 wc-django-locales-collector-0.1.2/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      363 2022-12-22 11:33:36.000000 wc-django-locales-collector-0.1.2/CHANGELOG.md
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1072 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/LICENSE
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)       88 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/MANIFEST.in
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1260 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2910 2022-12-22 11:37:12.773189 wc-django-locales-collector-0.1.2/PKG-INFO
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1366 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/README.md
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)       79 2022-12-22 11:37:12.773189 wc-django-locales-collector-0.1.2/setup.cfg
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1600 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/setup.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      562 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-22 11:37:12.769189 wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     2910 2022-12-22 11:37:12.000000 wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/PKG-INFO
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      784 2022-12-22 11:37:12.000000 wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/SOURCES.txt
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)        1 2022-12-22 11:37:12.000000 wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/dependency_links.txt
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      153 2022-12-22 11:37:12.000000 wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/requires.txt
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)       22 2022-12-22 11:37:12.000000 wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-22 11:37:12.769189 wc-django-locales-collector-0.1.2/wcd_locales_collector/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      137 2022-12-22 11:29:41.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/__init__.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      364 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/apps.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      440 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/conf.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)       57 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/discovery.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1153 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/helpers.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-22 11:37:12.769189 wc-django-locales-collector-0.1.2/wcd_locales_collector/management/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/management/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-22 11:37:12.769189 wc-django-locales-collector-0.1.2/wcd_locales_collector/management/commands/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/management/commands/__init__.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1458 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/management/commands/collectlocales.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-22 11:37:12.773189 wc-django-locales-collector-0.1.2/wcd_locales_collector/services/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/services/__init__.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1758 2022-12-22 09:25:21.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/services/collector.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      895 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.2/wcd_locales_collector/services/pathifier.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      489 2023-07-03 09:01:13.000000 wc-django-locales-collector-0.1.3/CHANGELOG.md
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1072 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/LICENSE
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       88 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/MANIFEST.in
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1260 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2448 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/PKG-INFO
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1366 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/README.md
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       79 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/setup.cfg
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1600 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/setup.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      562 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     2448 2023-07-03 09:02:23.000000 wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/PKG-INFO
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      784 2023-07-03 09:02:23.000000 wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/SOURCES.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        1 2023-07-03 09:02:23.000000 wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/dependency_links.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      153 2023-07-03 09:02:23.000000 wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/requires.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       22 2023-07-03 09:02:23.000000 wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/wcd_locales_collector/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      137 2023-07-03 08:59:38.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      364 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/apps.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      440 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/conf.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       57 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/discovery.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1153 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/helpers.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/wcd_locales_collector/management/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/management/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/wcd_locales_collector/management/commands/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/management/commands/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1458 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/management/commands/collectlocales.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 09:02:23.221445 wc-django-locales-collector-0.1.3/wcd_locales_collector/services/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/services/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2587 2023-07-03 08:59:32.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/services/collector.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      895 2022-09-20 08:50:23.000000 wc-django-locales-collector-0.1.3/wcd_locales_collector/services/pathifier.py
```

### Comparing `wc-django-locales-collector-0.1.2/LICENSE` & `wc-django-locales-collector-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/Makefile` & `wc-django-locales-collector-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/PKG-INFO` & `wc-django-locales-collector-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,92 @@
 Metadata-Version: 2.1
 Name: wc-django-locales-collector
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django app that collect thirdparty translations into local folder.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Description: # WebCase locales collector
-        
-        Collects locales from any python third parties to some local folder. It's useful for a more easier local translations management.
-        
-        ## Installation
-        
-        ```sh
-        pip install wc-django-locales-collector
-        ```
-        
-        In `settings.py`:
-        
-        ```python
-        
-        INSTALLED_APPS += [
-          'wcd_locales_collector',
-        ]
-        
-        WCD_LOCALES_COLLECTOR = {
-          # List of modules for which locales will be collected.
-          'MODULES': [
-            # For example:
-            'rest_framework',
-          ],
-          # Path to save collected locales.
-          'PATH' = BASE_ROOT / 'exported_locale'
-        }
-        
-        # All root options could also be provided as standalone ones(for overriding, etc.):
-        WCD_LOCALES_COLLECTOR_PATH = BASE_ROOT / 'replaced_locale'
-        
-        # ...
-        
-        # Your static `LOCALE_PATHS` config should be wrapped by paths extender.
-        # If it's not, then all exported locales will not be applied.
-        from wcd_locales_collector.helpers import locale_paths_extender
-        
-        LOCALE_PATHS = locale_paths_extender(LOCALE_PATHS)
-        
-        # OR!
-        # If you have some issues with that approach - you can extend `LOCALE_PATHS`
-        # manually:
-        from wcd_locales_collector.services import pathifier
-        
-        LOCALE_PATHS = LOCALE_PATHS + pathifier.get_modules_result_paths(
-          WCD_LOCALES_COLLECTOR['MODULES'], WCD_LOCALES_COLLECTOR_PATH
-        )
-        ```
-        
-        ## Usage
-        
-        ```python
-        python manage.py collectlocales
-        ```
-        
-        That's it. You have collected all locales from all provided apps into a separate folder.
-        # Changelog
-        All notable changes to this project will be documented in this file.
-        
-        The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-        and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-        
-        ## [Unreleased]
-        
-        ## [0.1.2]
-        ### Fixed
-        - Initial merge issue with unicode symbols.
-        
-        ## [0.1.0]
-        Initial version.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# WebCase locales collector
+
+Collects locales from any python third parties to some local folder. It's useful for a more easier local translations management.
+
+## Installation
+
+```sh
+pip install wc-django-locales-collector
+```
+
+In `settings.py`:
+
+```python
+
+INSTALLED_APPS += [
+  'wcd_locales_collector',
+]
+
+WCD_LOCALES_COLLECTOR = {
+  # List of modules for which locales will be collected.
+  'MODULES': [
+    # For example:
+    'rest_framework',
+  ],
+  # Path to save collected locales.
+  'PATH' = BASE_ROOT / 'exported_locale'
+}
+
+# All root options could also be provided as standalone ones(for overriding, etc.):
+WCD_LOCALES_COLLECTOR_PATH = BASE_ROOT / 'replaced_locale'
+
+# ...
+
+# Your static `LOCALE_PATHS` config should be wrapped by paths extender.
+# If it's not, then all exported locales will not be applied.
+from wcd_locales_collector.helpers import locale_paths_extender
+
+LOCALE_PATHS = locale_paths_extender(LOCALE_PATHS)
+
+# OR!
+# If you have some issues with that approach - you can extend `LOCALE_PATHS`
+# manually:
+from wcd_locales_collector.services import pathifier
+
+LOCALE_PATHS = LOCALE_PATHS + pathifier.get_modules_result_paths(
+  WCD_LOCALES_COLLECTOR['MODULES'], WCD_LOCALES_COLLECTOR_PATH
+)
+```
+
+## Usage
+
+```python
+python manage.py collectlocales
+```
+
+That's it. You have collected all locales from all provided apps into a separate folder.
+# Changelog
+All notable changes to this project will be documented in this file.
+
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+
+## [Unreleased]
+
+## [0.1.3]
+### Added
+- Automatic mo2po sources conversion if library doesn't have po files but ships with compiled mo files.
+
+## [0.1.2]
+### Fixed
+- Initial merge issue with unicode symbols.
+
+## [0.1.0]
+Initial version.
```

### Comparing `wc-django-locales-collector-0.1.2/README.md` & `wc-django-locales-collector-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/setup.py` & `wc-django-locales-collector-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/tox.ini` & `wc-django-locales-collector-0.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/PKG-INFO` & `wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,92 @@
 Metadata-Version: 2.1
 Name: wc-django-locales-collector
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django app that collect thirdparty translations into local folder.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Description: # WebCase locales collector
-        
-        Collects locales from any python third parties to some local folder. It's useful for a more easier local translations management.
-        
-        ## Installation
-        
-        ```sh
-        pip install wc-django-locales-collector
-        ```
-        
-        In `settings.py`:
-        
-        ```python
-        
-        INSTALLED_APPS += [
-          'wcd_locales_collector',
-        ]
-        
-        WCD_LOCALES_COLLECTOR = {
-          # List of modules for which locales will be collected.
-          'MODULES': [
-            # For example:
-            'rest_framework',
-          ],
-          # Path to save collected locales.
-          'PATH' = BASE_ROOT / 'exported_locale'
-        }
-        
-        # All root options could also be provided as standalone ones(for overriding, etc.):
-        WCD_LOCALES_COLLECTOR_PATH = BASE_ROOT / 'replaced_locale'
-        
-        # ...
-        
-        # Your static `LOCALE_PATHS` config should be wrapped by paths extender.
-        # If it's not, then all exported locales will not be applied.
-        from wcd_locales_collector.helpers import locale_paths_extender
-        
-        LOCALE_PATHS = locale_paths_extender(LOCALE_PATHS)
-        
-        # OR!
-        # If you have some issues with that approach - you can extend `LOCALE_PATHS`
-        # manually:
-        from wcd_locales_collector.services import pathifier
-        
-        LOCALE_PATHS = LOCALE_PATHS + pathifier.get_modules_result_paths(
-          WCD_LOCALES_COLLECTOR['MODULES'], WCD_LOCALES_COLLECTOR_PATH
-        )
-        ```
-        
-        ## Usage
-        
-        ```python
-        python manage.py collectlocales
-        ```
-        
-        That's it. You have collected all locales from all provided apps into a separate folder.
-        # Changelog
-        All notable changes to this project will be documented in this file.
-        
-        The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-        and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-        
-        ## [Unreleased]
-        
-        ## [0.1.2]
-        ### Fixed
-        - Initial merge issue with unicode symbols.
-        
-        ## [0.1.0]
-        Initial version.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# WebCase locales collector
+
+Collects locales from any python third parties to some local folder. It's useful for a more easier local translations management.
+
+## Installation
+
+```sh
+pip install wc-django-locales-collector
+```
+
+In `settings.py`:
+
+```python
+
+INSTALLED_APPS += [
+  'wcd_locales_collector',
+]
+
+WCD_LOCALES_COLLECTOR = {
+  # List of modules for which locales will be collected.
+  'MODULES': [
+    # For example:
+    'rest_framework',
+  ],
+  # Path to save collected locales.
+  'PATH' = BASE_ROOT / 'exported_locale'
+}
+
+# All root options could also be provided as standalone ones(for overriding, etc.):
+WCD_LOCALES_COLLECTOR_PATH = BASE_ROOT / 'replaced_locale'
+
+# ...
+
+# Your static `LOCALE_PATHS` config should be wrapped by paths extender.
+# If it's not, then all exported locales will not be applied.
+from wcd_locales_collector.helpers import locale_paths_extender
+
+LOCALE_PATHS = locale_paths_extender(LOCALE_PATHS)
+
+# OR!
+# If you have some issues with that approach - you can extend `LOCALE_PATHS`
+# manually:
+from wcd_locales_collector.services import pathifier
+
+LOCALE_PATHS = LOCALE_PATHS + pathifier.get_modules_result_paths(
+  WCD_LOCALES_COLLECTOR['MODULES'], WCD_LOCALES_COLLECTOR_PATH
+)
+```
+
+## Usage
+
+```python
+python manage.py collectlocales
+```
+
+That's it. You have collected all locales from all provided apps into a separate folder.
+# Changelog
+All notable changes to this project will be documented in this file.
+
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+
+## [Unreleased]
+
+## [0.1.3]
+### Added
+- Automatic mo2po sources conversion if library doesn't have po files but ships with compiled mo files.
+
+## [0.1.2]
+### Fixed
+- Initial merge issue with unicode symbols.
+
+## [0.1.0]
+Initial version.
```

### Comparing `wc-django-locales-collector-0.1.2/wc_django_locales_collector.egg-info/SOURCES.txt` & `wc-django-locales-collector-0.1.3/wc_django_locales_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/wcd_locales_collector/helpers.py` & `wc-django-locales-collector-0.1.3/wcd_locales_collector/helpers.py`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/wcd_locales_collector/management/commands/collectlocales.py` & `wc-django-locales-collector-0.1.3/wcd_locales_collector/management/commands/collectlocales.py`

 * *Files identical despite different names*

### Comparing `wc-django-locales-collector-0.1.2/wcd_locales_collector/services/collector.py` & `wc-django-locales-collector-0.1.3/wcd_locales_collector/services/collector.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 MSGMERGE_DEFAULT_ARGS = [
     'msgmerge', '-q', '--previous',
 ]
 MSGCAT_DEFAULT_ARGS = [
     'msgcat', '--to-code=utf-8', '--use-first',
 ]
+MSGUNFMT_DEFAULT_ARGS = [
+    'msgunfmt',
+]
 
 
 def merge(path_from: str, path_to: str):
     os.makedirs(os.path.dirname(path_to), exist_ok=True)
 
     if not os.path.exists(path_to):
         shutil.copy(path_from, path_to)
@@ -37,14 +40,22 @@
 
     # Merging filled source data to an empty new.
     return popen_wrapper(
         MSGCAT_DEFAULT_ARGS + [path_to, path_from, '-o', path_to],
     )
 
 
+def uncompile(path_from: str, path_to: str):
+    _, errors, status = popen_wrapper(
+        MSGUNFMT_DEFAULT_ARGS + [path_from, '-o', path_to],
+    )
+
+    return os.path.exists(path_to)
+
+
 def collect_locales(
     modules: List[str],
     result_path: str,
     report_error: lambda *args: logger.warning(*args)
 ):
     result_path = os.path.abspath(result_path)
 
@@ -56,16 +67,34 @@
             continue
 
         module_path = pathifier.get_module_result_path(module, result_path)
 
         for root, dirs, files in os.walk(path):
             dir = os.path.join(module_path, root.replace(path, ''))
 
-            for file in files:
-                if file.endswith('.po'):
-                    file_path = os.path.join(root, file)
-                    new_path = os.path.join(dir, file)
+            rmfiles = []
+            pofiles = [file for file in files if file.endswith('.po')]
+
+            if len(pofiles) == 0:
+                mofiles = [file for file in files if file.endswith('.mo')]
+
+                for file in mofiles:
+                    filepath = os.path.join(root, file)
+                    path_to = filepath[:-3] + '.po'
+                    result = uncompile(filepath, path_to)
+
+                    if result:
+                        pofiles.append(file[:-3] + '.po')
+                        rmfiles.append(path_to)
+
+            for file in pofiles:
+                file_path = os.path.join(root, file)
+                new_path = os.path.join(dir, file)
+
+                _, errors, status = merge(file_path, new_path)
 
-                    _, errors, status = merge(file_path, new_path)
+                if status != 0:
+                    report_error(errors)
 
-                    if status != 0:
-                        report_error(errors)
+            if len(rmfiles):
+                for rmfile in rmfiles:
+                    os.unlink(rmfile)
```

### Comparing `wc-django-locales-collector-0.1.2/wcd_locales_collector/services/pathifier.py` & `wc-django-locales-collector-0.1.3/wcd_locales_collector/services/pathifier.py`

 * *Files identical despite different names*

