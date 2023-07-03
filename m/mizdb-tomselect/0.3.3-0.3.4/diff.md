# Comparing `tmp/mizdb-tomselect-0.3.3.tar.gz` & `tmp/mizdb-tomselect-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizdb-tomselect-0.3.3.tar", last modified: Thu Jun 29 09:26:43 2023, max compression
+gzip compressed data, was "mizdb-tomselect-0.3.4.tar", last modified: Mon Jul  3 10:08:20 2023, max compression
```

## Comparing `mizdb-tomselect-0.3.3.tar` & `mizdb-tomselect-0.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     1064 2023-05-24 06:41:14.000000 mizdb-tomselect-0.3.3/LICENSE
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    10848 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/PKG-INFO
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    10446 2023-06-29 09:22:01.000000 mizdb-tomselect-0.3.3/README.md
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     1601 2023-06-29 09:26:26.000000 mizdb-tomselect-0.3.3/pyproject.toml
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)       38 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/setup.cfg
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.989368 mizdb-tomselect-0.3.3/src/
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.012369 mizdb-tomselect-0.3.3/src/mizdb_tomselect/
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)      123 2023-05-24 06:41:14.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/__init__.py
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.013368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/css/
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)      430 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.013368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/js/
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)   145839 2023-06-29 09:26:40.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.013368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    17697 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    23112 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     4360 2023-06-29 08:29:14.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/views.py
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     6229 2023-06-29 09:22:01.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/widgets.py
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.012369 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    10848 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/PKG-INFO
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)      672 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/SOURCES.txt
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)        1 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/dependency_links.txt
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)        7 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/requires.txt
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)       16 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/top_level.txt
-drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/tests/
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    14349 2023-06-29 09:22:17.000000 mizdb-tomselect-0.3.3/tests/test_e2e.py
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    16071 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/tests/test_views.py
--rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     5000 2023-06-29 09:22:01.000000 mizdb-tomselect-0.3.3/tests/test_widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/
+-rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.4/LICENSE
+-rw-r--r--   0 philip    (1000) philip    (1000)    10852 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)    10450 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/README.md
+-rw-r--r--   0 philip    (1000) philip    (1000)     1601 2023-07-03 10:07:10.000000 mizdb-tomselect-0.3.4/pyproject.toml
+-rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/setup.cfg
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.069904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/
+-rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/__init__.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.070904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)      430 2023-07-03 10:03:55.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.070904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/js/
+-rw-r--r--   0 philip    (1000) philip    (1000)   145719 2023-07-03 10:08:17.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.071904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
+-rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
+-rw-r--r--   0 philip    (1000) philip    (1000)     4366 2023-07-03 10:03:55.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     6229 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.070904 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/
+-rw-r--r--   0 philip    (1000) philip    (1000)    10852 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)      672 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/SOURCES.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/dependency_links.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/requires.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/top_level.txt
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/tests/
+-rw-r--r--   0 philip    (1000) philip    (1000)    14349 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/tests/test_e2e.py
+-rw-r--r--   0 philip    (1000) philip    (1000)    16008 2023-07-03 10:03:55.000000 mizdb-tomselect-0.3.4/tests/test_views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     5000 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/tests/test_widgets.py
```

### Comparing `mizdb-tomselect-0.3.3/LICENSE` & `mizdb-tomselect-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.3/PKG-INFO` & `mizdb-tomselect-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.3.3
+Version: 0.3.4
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -28,19 +28,20 @@
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
 
 ----
+
 ## Installation
 
 Install:
 ```bash
-pip install -U mizdb_tomselect
+pip install -U mizdb-tomselect
 ```
 ## Usage
 
 Add to installed apps:
 ```python
 INSTALLED_APPS = [
     ...
@@ -112,14 +113,16 @@
         <button type="submit" class="btn btn-success">Save</button>
     </form>
 </div>
 </body>
 </html>
 ```
 
+----
+
 ## Widgets
 
 The widgets pass attributes necessary to make autocomplete requests to the
 HTML element via the dataset property. The TomSelect element is then initialized
 from the attributes in the dataset property.
 
 ### MIZSelect
@@ -169,14 +172,15 @@
 
 **Important**: that means that the result visible to TomSelect must have an attribute
 or property with that name or the column will remain empty. 
 The results for TomSelect are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
+----
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
 passed to the widget. The default value for the lookup is `name__icontains`.
@@ -185,15 +189,14 @@
 class MyAutocompleteView(AutocompleteView):
     
     def search(self, request, queryset, q):
         # Filter using your own queryset method:
         return queryset.search(q)
 ```
 
-----
 ### Option creation
 
 To enable option creation in the dropdown, pass the URL pattern name of the 
 add page of the given model to the widget. This will add an 'Add' button to the
 bottom of the dropdown.
 
 ```python
@@ -223,15 +226,14 @@
     def create_object(self, data):
         """Create a new object with the given data."""
         return self.model.objects.create(**{self.create_field: data[self.create_field]})
 ```
 
 Override the view's `create_object` method to change the creation process.
 
-----
 ### Changelist link
 
 The dropdown will include a link to the changelist of the given model if you
 pass in the URL pattern name of the changelist view.
 
 ```python
 # urls.py
@@ -240,15 +242,15 @@
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
     path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
 widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
-----
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
 class Person(models.Model):
@@ -272,14 +274,16 @@
 ```
 This will result in the Person result queryset to be filtered against 
 `city_id` with the current value of the `capitol` formfield.  
 NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
+----
+
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
```

### Comparing `mizdb-tomselect-0.3.3/README.md` & `mizdb-tomselect-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,20 @@
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
 
 ----
+
 ## Installation
 
 Install:
 ```bash
-pip install -U mizdb_tomselect
+pip install -U mizdb-tomselect
 ```
 ## Usage
 
 Add to installed apps:
 ```python
 INSTALLED_APPS = [
     ...
@@ -100,14 +101,16 @@
         <button type="submit" class="btn btn-success">Save</button>
     </form>
 </div>
 </body>
 </html>
 ```
 
+----
+
 ## Widgets
 
 The widgets pass attributes necessary to make autocomplete requests to the
 HTML element via the dataset property. The TomSelect element is then initialized
 from the attributes in the dataset property.
 
 ### MIZSelect
@@ -157,14 +160,15 @@
 
 **Important**: that means that the result visible to TomSelect must have an attribute
 or property with that name or the column will remain empty. 
 The results for TomSelect are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
+----
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
 passed to the widget. The default value for the lookup is `name__icontains`.
@@ -173,15 +177,14 @@
 class MyAutocompleteView(AutocompleteView):
     
     def search(self, request, queryset, q):
         # Filter using your own queryset method:
         return queryset.search(q)
 ```
 
-----
 ### Option creation
 
 To enable option creation in the dropdown, pass the URL pattern name of the 
 add page of the given model to the widget. This will add an 'Add' button to the
 bottom of the dropdown.
 
 ```python
@@ -211,15 +214,14 @@
     def create_object(self, data):
         """Create a new object with the given data."""
         return self.model.objects.create(**{self.create_field: data[self.create_field]})
 ```
 
 Override the view's `create_object` method to change the creation process.
 
-----
 ### Changelist link
 
 The dropdown will include a link to the changelist of the given model if you
 pass in the URL pattern name of the changelist view.
 
 ```python
 # urls.py
@@ -228,15 +230,15 @@
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
     path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
 widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
-----
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
 class Person(models.Model):
@@ -260,14 +262,16 @@
 ```
 This will result in the Person result queryset to be filtered against 
 `city_id` with the current value of the `capitol` formfield.  
 NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
+----
+
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
```

### Comparing `mizdb-tomselect-0.3.3/pyproject.toml` & `mizdb-tomselect-0.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mizdb-tomselect"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Philip Becker", email="yummytea1@gmail.com" },
 ]
 description = "Django autocomplete widgets and views using TomSelect"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js` & `mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4306,22 +4306,22 @@
     function getSettings2(elem) {
         function buildUrl(query, page) {
             let valuesSelect = [elem.dataset.valueField, elem.dataset.labelField];
             if (elem.extraColumns) {
                 valuesSelect = valuesSelect.concat(elem.extraColumns);
             }
             const params = new URLSearchParams({
-                q: encodeURIComponent(query),
+                q: query,
                 p: page,
-                model: encodeURIComponent(elem.dataset.model),
-                sl: encodeURIComponent(elem.dataset.searchLookup),
-                vs: encodeURIComponent(JSON.stringify(valuesSelect))
+                model: elem.dataset.model,
+                sl: elem.dataset.searchLookup,
+                vs: JSON.stringify(valuesSelect)
             });
             if (elem.filterByElem) {
-                params.append("f", encodeURIComponent(`${elem.filterByLookup}=${elem.filterByElem.value}`));
+                params.append("f", `${elem.filterByLookup}=${elem.filterByElem.value}`);
             }
             return `${elem.dataset.autocompleteUrl}?${params.toString()}`;
         }
         elem.extraColumns = elem.hasAttribute("is-tabular") ? JSON.parse(elem.dataset.extraColumns) : [];
         elem.labelColClass = elem.extraColumns.length > 0 && elem.extraColumns.length < 4 ? "col-5" : "col";
         if (elem.dataset.filterBy) {
             const filterBy = JSON.parse(elem.dataset.filterBy);
@@ -4496,15 +4496,15 @@
                 changelistLink.href = changelistURL;
                 changelistLink.target = "_blank";
                 changelistLink.innerHTML = "\xC4nderungsliste";
                 footer.appendChild(changelistLink);
                 ts.on("type", (query) => {
                     if (query) {
                         const queryString = new URLSearchParams({
-                            q: encodeURIComponent(query)
+                            q: query
                         }).toString();
                         changelistLink.href = `${changelistURL}?${queryString}`;
                     } else {
                         changelistLink.href = changelistURL;
                     }
                 });
                 ts.on("blur", () => {
```

### Comparing `mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css` & `mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map` & `mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.3/src/mizdb_tomselect/views.py` & `mizdb-tomselect-0.3.4/src/mizdb_tomselect/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
-from urllib.parse import unquote
 
 from django import http, views
 from django.apps import apps
 from django.contrib.auth import get_permission_codename
+from django.db import transaction
 
 SEARCH_VAR = "q"
 SEARCH_LOOKUP_VAR = "sl"
 FILTERBY_VAR = "f"
 VALUES_VAR = "vs"
 
 PAGE_VAR = "p"
@@ -21,34 +21,34 @@
     page_kwarg = PAGE_VAR
 
     def setup(self, request, *args, **kwargs):
         super().setup(request, *args, **kwargs)
         request_data = getattr(request, request.method)
         self.model = apps.get_model(request_data["model"])
         self.create_field = request_data.get("create-field")
-        self.search_lookup = request.GET.get(SEARCH_LOOKUP_VAR)
+        self.search_lookup = request_data.get(SEARCH_LOOKUP_VAR)
         self.values_select = []
         if VALUES_VAR in request_data:
-            values = unquote(request_data[VALUES_VAR])
-            self.values_select = json.loads(values)
+            self.values_select = json.loads(request_data[VALUES_VAR])
+        self.q = request_data.get(SEARCH_VAR, "")
 
     def apply_filter_by(self, queryset):
         """
         Filter the given queryset against values set by other form fields.
 
         If the widget was set up with a `filter_by` parameter, the request will
         include the `FILTERBY_VAR` parameter, indicating that the results must
         be filtered against the lookup and value provided by `FILTERBY_VAR`.
         If `FILTERBY_VAR` is present but no value is set, return an empty
         queryset.
         """
         if FILTERBY_VAR not in self.request.GET:
             return queryset
         else:
-            lookup, value = unquote(self.request.GET[FILTERBY_VAR]).split("=")
+            lookup, value = self.request.GET[FILTERBY_VAR].split("=")
             if not value:
                 # A filter was set up for this autocomplete, but no filter value
                 # was provided; return an empty queryset.
                 return queryset.none()
             return queryset.filter(**{lookup: value})
 
     def search(self, queryset, q):
@@ -59,26 +59,25 @@
         """Order the result queryset."""
         ordering = self.model._meta.ordering or ["id"]
         return queryset.order_by(*ordering)
 
     def get_queryset(self):
         """Return a queryset of objects that match the search parameters and filters."""
         queryset = super().get_queryset()
-        q = unquote(self.request.GET.get(SEARCH_VAR, ""))
-        if q or FILTERBY_VAR in self.request.GET:
+        if self.q or FILTERBY_VAR in self.request.GET:
             queryset = self.apply_filter_by(queryset)
-            queryset = self.search(queryset, q)
+            queryset = self.search(queryset, self.q)
         return self.order_queryset(queryset)
 
     def get_page_results(self, page):
         """Hook for modifying the result queryset for the given page."""
         return page.object_list
 
     def get_result_values(self, results):
-        """Return a list of key:value pairs for the given results."""
+        """Return a JSON-serializable list of values for the given results."""
         return list(results.values(*self.values_select))
 
     def get(self, request, *args, **kwargs):
         queryset = self.get_queryset()
         page_size = self.get_paginate_by(queryset)
         paginator, page, object_list, has_other_pages = self.paginate_queryset(queryset, page_size)
         data = {
@@ -103,9 +102,10 @@
         return self.model.objects.create(**{self.create_field: data[self.create_field]})
 
     def post(self, request, *args, **kwargs):
         if not self.has_add_permission(request):
             return http.HttpResponseForbidden()
         if request.POST.get(self.create_field) is None:
             return http.HttpResponseBadRequest()
-        obj = self.create_object(request.POST)
+        with transaction.atomic():
+            obj = self.create_object(request.POST)
         return http.JsonResponse({"pk": obj.pk, "text": str(obj)})
```

### Comparing `mizdb-tomselect-0.3.3/src/mizdb_tomselect/widgets.py` & `mizdb-tomselect-0.3.4/src/mizdb_tomselect/widgets.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/PKG-INFO` & `mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.3.3
+Version: 0.3.4
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -28,19 +28,20 @@
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
 
 ----
+
 ## Installation
 
 Install:
 ```bash
-pip install -U mizdb_tomselect
+pip install -U mizdb-tomselect
 ```
 ## Usage
 
 Add to installed apps:
 ```python
 INSTALLED_APPS = [
     ...
@@ -112,14 +113,16 @@
         <button type="submit" class="btn btn-success">Save</button>
     </form>
 </div>
 </body>
 </html>
 ```
 
+----
+
 ## Widgets
 
 The widgets pass attributes necessary to make autocomplete requests to the
 HTML element via the dataset property. The TomSelect element is then initialized
 from the attributes in the dataset property.
 
 ### MIZSelect
@@ -169,14 +172,15 @@
 
 **Important**: that means that the result visible to TomSelect must have an attribute
 or property with that name or the column will remain empty. 
 The results for TomSelect are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
+----
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
 passed to the widget. The default value for the lookup is `name__icontains`.
@@ -185,15 +189,14 @@
 class MyAutocompleteView(AutocompleteView):
     
     def search(self, request, queryset, q):
         # Filter using your own queryset method:
         return queryset.search(q)
 ```
 
-----
 ### Option creation
 
 To enable option creation in the dropdown, pass the URL pattern name of the 
 add page of the given model to the widget. This will add an 'Add' button to the
 bottom of the dropdown.
 
 ```python
@@ -223,15 +226,14 @@
     def create_object(self, data):
         """Create a new object with the given data."""
         return self.model.objects.create(**{self.create_field: data[self.create_field]})
 ```
 
 Override the view's `create_object` method to change the creation process.
 
-----
 ### Changelist link
 
 The dropdown will include a link to the changelist of the given model if you
 pass in the URL pattern name of the changelist view.
 
 ```python
 # urls.py
@@ -240,15 +242,15 @@
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
     path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
 widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
-----
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
 class Person(models.Model):
@@ -272,14 +274,16 @@
 ```
 This will result in the Person result queryset to be filtered against 
 `city_id` with the current value of the `capitol` formfield.  
 NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
+----
+
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
```

### Comparing `mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/SOURCES.txt` & `mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.3/tests/test_e2e.py` & `mizdb-tomselect-0.3.4/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.3/tests/test_views.py` & `mizdb-tomselect-0.3.4/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from unittest.mock import Mock, patch
-from urllib.parse import quote, urlencode
+from urllib.parse import urlencode
 
 import pytest
 from django.contrib.auth import get_permission_codename, get_user_model
 from django.contrib.auth.models import Permission
 from django.db.models.sql.where import NothingNode
 from django.http import HttpResponseBadRequest, HttpResponseForbidden, JsonResponse
 from django.test import Client
@@ -236,20 +236,20 @@
         assert view.create_field == "create_field"
 
     @pytest.mark.parametrize("request_data", [{SEARCH_LOOKUP_VAR: "search_lookup"}])
     def test_setup_sets_search_lookup(self, view, setup_view, request_data):
         """Assert that setup() sets the `search_lookup` attribute."""
         assert view.search_lookup == "search_lookup"
 
-    @pytest.mark.parametrize("request_data", [{VALUES_VAR: quote(json.dumps(["id", "name", "jahr", "num"]))}])
+    @pytest.mark.parametrize("request_data", [{VALUES_VAR: json.dumps(["id", "name", "jahr", "num"])}])
     def test_setup_sets_values_select(self, view, setup_view, request_data):
         """Assert that setup() sets the `values_select` attribute."""
         assert view.values_select == ["id", "name", "jahr", "num"]
 
-    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: quote("magazin_id=1")}])
+    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "magazin_id=1"}])
     def test_apply_filter_by(self, view, request_data):
         """Assert that apply_filter_by applies the expected ^filter to the queryset."""
         queryset = view.apply_filter_by(self.queryset)
         assert len(queryset.query.where.children) == 1
         lookup = queryset.query.where.children[0]
         assert lookup.lhs.target == self.model._meta.get_field("magazin")
         assert lookup.rhs == 1
@@ -259,15 +259,15 @@
         """
         Assert that apply_filter_by returns the queryset unchanged if the
         request does not contain FILTERBY_VAR.
         """
         queryset = view.apply_filter_by(self.queryset)
         assert len(queryset.query.where.children) == 0
 
-    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: quote("magazin_id=")}])
+    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "magazin_id="}])
     def test_apply_filter_by_no_filter_value(self, view, request_data):
         """
         Assert that apply_filter_by returns an empty queryset if no filter
         value is given.
         """
         queryset = view.apply_filter_by(self.queryset)
         assert len(queryset.query.where.children) == 1
@@ -282,40 +282,38 @@
         assert lookup.lhs.target == self.model._meta.get_field("name")
         assert lookup.rhs == "Test"
 
     def test_order_queryset(self, view, setup_view):
         """Assert that order_queryset applies ordering to the queryset."""
         assert view.order_queryset(self.queryset).query.order_by == ("magazin", "name")
 
-    @pytest.mark.parametrize("request_data", [{SEARCH_VAR: quote("Test"), SEARCH_LOOKUP_VAR: "name__icontains"}])
+    @pytest.mark.parametrize("request_data", [{SEARCH_VAR: "Test", SEARCH_LOOKUP_VAR: "name__icontains"}])
     def test_get_queryset_calls_search(self, view, setup_view, request_data):
         """Assert that get_queryset calls search if a search term is given."""
         search_mock = Mock()
         with patch.object(view, "apply_filter_by", new=search_mock):
             view.get_queryset()
             search_mock.assert_called()
 
-    @pytest.mark.parametrize(
-        "request_data", [{FILTERBY_VAR: quote("magazin_id=1"), SEARCH_LOOKUP_VAR: "name__icontains"}]
-    )
+    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "magazin_id=1", SEARCH_LOOKUP_VAR: "name__icontains"}])
     def test_get_queryset_calls_apply_filter_by(self, view, setup_view, request_data):
         """Assert that get_queryset calls apply_filter_by if FILTERBY_VAR is given."""
         apply_filter_by_mock = Mock()
         with patch.object(view, "apply_filter_by", new=apply_filter_by_mock):
             view.get_queryset()
             apply_filter_by_mock.assert_called()
 
     def test_get_queryset_calls_order_queryset(self, view, setup_view):
         """Assert that get_queryset calls order_queryset."""
         order_queryset_mock = Mock()
         with patch.object(view, "order_queryset", new=order_queryset_mock):
             view.get_queryset()
             order_queryset_mock.assert_called()
 
-    @pytest.mark.parametrize("request_data", [{VALUES_VAR: quote(json.dumps(["id", "name", "jahr", "num"]))}])
+    @pytest.mark.parametrize("request_data", [{VALUES_VAR: json.dumps(["id", "name", "jahr", "num"])}])
     def test_get_result_values(self, view, setup_view, request_data, obj):
         """Assert that get_result_values returns a list of queryset values."""
         results = view.get_result_values(self.queryset.filter(pk=obj.pk))
         assert results == [{"id": obj.pk, "name": "Test", "jahr": "3", "num": "1"}]
 
     def test_get(self, view, setup_view, admin_user, obj):
         """Assert that get returns the expected response."""
```

### Comparing `mizdb-tomselect-0.3.3/tests/test_widgets.py` & `mizdb-tomselect-0.3.4/tests/test_widgets.py`

 * *Files identical despite different names*

