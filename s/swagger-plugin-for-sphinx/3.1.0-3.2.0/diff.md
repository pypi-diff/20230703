# Comparing `tmp/swagger-plugin-for-sphinx-3.1.0.tar.gz` & `tmp/swagger-plugin-for-sphinx-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagger-plugin-for-sphinx-3.1.0.tar", last modified: Mon Jun  5 14:00:52 2023, max compression
+gzip compressed data, was "swagger-plugin-for-sphinx-3.2.0.tar", last modified: Mon Jul  3 14:21:36 2023, max compression
```

## Comparing `swagger-plugin-for-sphinx-3.1.0.tar` & `swagger-plugin-for-sphinx-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/swagger.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:21:36.590305 swagger-plugin-for-sphinx-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 14:21:36.590305 swagger-plugin-for-sphinx-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:21:36.590305 swagger-plugin-for-sphinx-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:21:36.590305 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx/swagger.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:21:36.590305 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 14:21:36.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 14:21:36.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:21:36.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 14:21:36.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 14:21:36.000000 swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:21:36.590305 swagger-plugin-for-sphinx-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-03 14:21:08.000000 swagger-plugin-for-sphinx-3.2.0/tests/test_plugin.py
```

### Comparing `swagger-plugin-for-sphinx-3.1.0/LICENSE` & `swagger-plugin-for-sphinx-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swagger-plugin-for-sphinx-3.1.0/PKG-INFO` & `swagger-plugin-for-sphinx-3.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagger-plugin-for-sphinx
-Version: 3.1.0
+Version: 3.2.0
 Summary: Sphinx plugin which renders a OpenAPI specification with Swagger
 Author-email: Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Issue Tracker, https://github.com/SAP/swagger-plugin-for-sphinx/issues
 Project-URL: Changelog, https://github.com/SAP/swagger-plugin-for-sphinx/blob/main/CHANGELOG.md
 Keywords: sphinx,swagger,plugin,openapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,50 +40,66 @@
 ## Install
 
 Just run `pip install swagger-plugin-for-sphinx`
 
 
 ## Usage
 
+### Enable the plugin
+
 First, add the plugin to the extensions list:
 ```python
 extensions = ["swagger_plugin_for_sphinx"]
 ```
 
+### Global configuration
+
 Then add the main configuration for swagger:
 ```python
 swagger_present_uri = ""
 swagger_bundle_uri = ""
 swagger_css_uri = ""
 ```
 These correspond to the modules explained [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/installation.md).
 By default, the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
 
+
+### Standalone page
 As a last step, define the swagger configuration as follows:
 ```python
 swagger = [
     {
         "name": "Service API",
         "page": "openapi",
+        "id": "my-page",
         "options": {
             "url": "openapi.yaml",
         },
     }
 ]
 ```
 Each item on the list will generate a new swagger HTML page.
 The `name` is the HTML page name and `page` defines the file name without an extension. This needs to be included in the TOC.
 The `options` are then used for the `SwaggerUIBundle` as defined [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md).
 Please don't specify the `dom_id` since it's hardcoded in the HTML page.
+If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
+To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
 
-In the sphinx build, an HTML page is created and put into the `_static` directory of the build.
+## Inline swagger page
+To include a swagger page into a sphinx page use the directive ``inline-swagger``:
 
-If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
+```rst
+.. inline-swagger::
+    :id: my-page
+```
 
-To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
+The ``id`` links to an existing configuration in ``conf.py`` as shows above.
+In this case, the configuration ``page`` will be ignored.
+Behind the scenes, a swagger HTML page is generated and then inserted using the ``.. raw::``
+directive.
 
 ## Build and Publish
 
 This project uses `setuptools` as the dependency management and build tool.
 To publish a new release, follow these steps:
 * Update the version in the `pyproject.toml`
 * Add an entry in the changelog
```

### Comparing `swagger-plugin-for-sphinx-3.1.0/README.md` & `swagger-plugin-for-sphinx-3.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,50 +10,66 @@
 ## Install
 
 Just run `pip install swagger-plugin-for-sphinx`
 
 
 ## Usage
 
+### Enable the plugin
+
 First, add the plugin to the extensions list:
 ```python
 extensions = ["swagger_plugin_for_sphinx"]
 ```
 
+### Global configuration
+
 Then add the main configuration for swagger:
 ```python
 swagger_present_uri = ""
 swagger_bundle_uri = ""
 swagger_css_uri = ""
 ```
 These correspond to the modules explained [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/installation.md).
 By default, the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
 
+
+### Standalone page
 As a last step, define the swagger configuration as follows:
 ```python
 swagger = [
     {
         "name": "Service API",
         "page": "openapi",
+        "id": "my-page",
         "options": {
             "url": "openapi.yaml",
         },
     }
 ]
 ```
 Each item on the list will generate a new swagger HTML page.
 The `name` is the HTML page name and `page` defines the file name without an extension. This needs to be included in the TOC.
 The `options` are then used for the `SwaggerUIBundle` as defined [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md).
 Please don't specify the `dom_id` since it's hardcoded in the HTML page.
+If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
+To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
 
-In the sphinx build, an HTML page is created and put into the `_static` directory of the build.
+## Inline swagger page
+To include a swagger page into a sphinx page use the directive ``inline-swagger``:
 
-If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
+```rst
+.. inline-swagger::
+    :id: my-page
+```
 
-To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
+The ``id`` links to an existing configuration in ``conf.py`` as shows above.
+In this case, the configuration ``page`` will be ignored.
+Behind the scenes, a swagger HTML page is generated and then inserted using the ``.. raw::``
+directive.
 
 ## Build and Publish
 
 This project uses `setuptools` as the dependency management and build tool.
 To publish a new release, follow these steps:
 * Update the version in the `pyproject.toml`
 * Add an entry in the changelog
```

### Comparing `swagger-plugin-for-sphinx-3.1.0/pyproject.toml` & `swagger-plugin-for-sphinx-3.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swagger-plugin-for-sphinx"
-version = "3.1.0"
+version = "3.2.0"
 description = "Sphinx plugin which renders a OpenAPI specification with Swagger"
 authors = [{ name = "Kai Mueller", email = "kai.mueller01@sap.com"}]
 readme = "README.md"
 keywords = ["sphinx", "swagger", "plugin", "openapi"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
@@ -27,14 +27,15 @@
     "Topic :: Documentation :: Sphinx",
     "Typing :: Typed"
 ]
 requires-python = ">=3.8,<4"
 dependencies = [
     "sphinx>=6.0,<8",
     "jinja2~=3.0",
+    "docutils",
 ]
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Issue Tracker" = "https://github.com/SAP/swagger-plugin-for-sphinx/issues"
@@ -49,14 +50,15 @@
     "coverage==7.2.0",
     "diff-cover==7.5.0",
     "pytest-cov==4.1.0",
     "black==23.3.0",
     "isort==5.12.0",
     "flake8==6.0.0",
     "mypy==1.3.0",
+    "types-docutils==0.20.0.1"
 ]
 
 [tool.setuptools.packages.find]
 include = ["swagger_plugin_for_sphinx"]
 
 [tool.setuptools.package-data]
 swagger_plugin_for_sphinx = ["py.typed", "*.j2"]
```

### Comparing `swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/swagger.j2` & `swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx/swagger.j2`

 * *Files identical despite different names*

### Comparing `swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO` & `swagger-plugin-for-sphinx-3.2.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagger-plugin-for-sphinx
-Version: 3.1.0
+Version: 3.2.0
 Summary: Sphinx plugin which renders a OpenAPI specification with Swagger
 Author-email: Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Issue Tracker, https://github.com/SAP/swagger-plugin-for-sphinx/issues
 Project-URL: Changelog, https://github.com/SAP/swagger-plugin-for-sphinx/blob/main/CHANGELOG.md
 Keywords: sphinx,swagger,plugin,openapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,50 +40,66 @@
 ## Install
 
 Just run `pip install swagger-plugin-for-sphinx`
 
 
 ## Usage
 
+### Enable the plugin
+
 First, add the plugin to the extensions list:
 ```python
 extensions = ["swagger_plugin_for_sphinx"]
 ```
 
+### Global configuration
+
 Then add the main configuration for swagger:
 ```python
 swagger_present_uri = ""
 swagger_bundle_uri = ""
 swagger_css_uri = ""
 ```
 These correspond to the modules explained [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/installation.md).
 By default, the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
 
+
+### Standalone page
 As a last step, define the swagger configuration as follows:
 ```python
 swagger = [
     {
         "name": "Service API",
         "page": "openapi",
+        "id": "my-page",
         "options": {
             "url": "openapi.yaml",
         },
     }
 ]
 ```
 Each item on the list will generate a new swagger HTML page.
 The `name` is the HTML page name and `page` defines the file name without an extension. This needs to be included in the TOC.
 The `options` are then used for the `SwaggerUIBundle` as defined [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md).
 Please don't specify the `dom_id` since it's hardcoded in the HTML page.
+If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
+To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
 
-In the sphinx build, an HTML page is created and put into the `_static` directory of the build.
+## Inline swagger page
+To include a swagger page into a sphinx page use the directive ``inline-swagger``:
 
-If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
+```rst
+.. inline-swagger::
+    :id: my-page
+```
 
-To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
+The ``id`` links to an existing configuration in ``conf.py`` as shows above.
+In this case, the configuration ``page`` will be ignored.
+Behind the scenes, a swagger HTML page is generated and then inserted using the ``.. raw::``
+directive.
 
 ## Build and Publish
 
 This project uses `setuptools` as the dependency management and build tool.
 To publish a new release, follow these steps:
 * Update the version in the `pyproject.toml`
 * Add an entry in the changelog
```

### Comparing `swagger-plugin-for-sphinx-3.1.0/tests/test_plugin.py` & `swagger-plugin-for-sphinx-3.2.0/tests/test_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -107,14 +107,42 @@
     </body>
 </html>"""
     )
 
     assert expected == html
 
 
+def test_inline(sphinx_runner: SphinxRunner, tmp_path: Path) -> None:
+    docs = tmp_path / "docs"
+    api_file = docs / "api.rst"
+    api_file.write_text(
+        "API\n===\n\n.. inline-swagger::\n    :id: myid\n", encoding="utf-8"
+    )
+
+    sphinx_runner(
+        swagger=[
+            {"name": "API1", "page": "openapi", "options": {"url": "openapi.yaml"}},
+            {"name": "API2", "id": "myid", "options": {"url": "openapi.yaml"}},
+        ]
+    )
+
+    build = tmp_path / "build"
+    static = build / "_static"
+
+    assert (static / "swagger-ui.css").is_file()
+    assert (static / "swagger-ui-bundle.js").is_file()
+    assert (static / "swagger-ui-standalone-preset.js").is_file()
+
+    with open(build / "api.html", encoding="utf-8") as file:
+        html = file.read()
+
+    assert '<script src="_static/sphinx_highlight.js">' in html
+    assert "window.ui = SwaggerUIBundle(config);" in html
+
+
 @pytest.mark.parametrize(
     "present_uri,bundle_uri,css_uri,expected_present_uri,expected_bundle_uri,expected_css_uri",
     [
         (
             None,
             None,
             None,
```

#### html2text {}

 * *error from `html2text {}` (b):*

 * *File "/tmp/diffoscope_vrp6lnvt_/tmp87nipxkh_TarContainer/0/18.py", line 186, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_vrp6lnvt_/tmp87nipxkh_TarContainer/0/18.py", line 186, column 0: CDATA terminal not found*

```diff
@@ -21,24 +21,17 @@
 "page": "openapi", "options": { "url": "openapi.yaml", }, } ] ) build =
 tmp_path / "build" static = build / "_static" assert (static / "swagger-
 ui.css").is_file() assert (static / "swagger-ui-bundle.js").is_file() assert
 (static / "swagger-ui-standalone-preset.js").is_file() with open(build /
 "openapi.html", encoding="utf-8") as file: html = file.read() base_url =
 "https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest" expected = dedent( f"""
 
-""" ) assert expected == html @pytest.mark.parametrize
-(
-"present_uri,bundle_uri,css_uri,expected_present_uri,expected_bundle_uri,expected_css_uri",
-[ ( None, None, None, "https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest/
-swagger-ui-standalone-preset.js", "https://cdn.jsdelivr.net/npm/swagger-ui-
-dist@latest/swagger-ui-bundle.js", "https://cdn.jsdelivr.net/npm/swagger-ui-
-dist@latest/swagger-ui.css", ), ( "foo-present", "foo-bundle", "foo-css", "foo-
-present", "foo-bundle", "foo-css", ), ], ) def test_custom_urls( mocker:
-MockerFixture, tmp_path: Path, sphinx_runner: SphinxRunner, present_uri: str |
-None, bundle_uri: str | None, css_uri: str | None, expected_present_uri: str,
-expected_bundle_uri: str, expected_css_uri: str, ) -> None: urlretrieve =
-mocker.patch.object(urllib.request, "urlretrieve") sphinx_runner([],
-present_uri, bundle_uri, css_uri) base_path = str(tmp_path) + "/build/_static"
-assert urlretrieve.call_args_list == [ mocker.call( expected_present_uri, f"
-{base_path}/swagger-ui-standalone-preset.js" ), mocker.call
-(expected_bundle_uri, f"{base_path}/swagger-ui-bundle.js"), mocker.call
-(expected_css_uri, f"{base_path}/swagger-ui.css"), ]
+""" ) assert expected == html def test_inline(sphinx_runner: SphinxRunner,
+tmp_path: Path) -> None: docs = tmp_path / "docs" api_file = docs / "api.rst"
+api_file.write_text( "API\n===\n\n.. inline-swagger::\n :id: myid\n",
+encoding="utf-8" ) sphinx_runner( swagger=[ {"name": "API1", "page": "openapi",
+"options": {"url": "openapi.yaml"}}, {"name": "API2", "id": "myid", "options":
+{"url": "openapi.yaml"}}, ] ) build = tmp_path / "build" static = build /
+"_static" assert (static / "swagger-ui.css").is_file() assert (static /
+"swagger-ui-bundle.js").is_file() assert (static / "swagger-ui-standalone-
+preset.js").is_file() with open(build / "api.html", encoding="utf-8") as file:
+html = file.read() assert '
```

