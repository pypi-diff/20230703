# Comparing `tmp/linkit-0.1.7.tar.gz` & `tmp/linkit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkit-0.1.7.tar", last modified: Thu Apr 27 11:19:09 2023, max compression
+gzip compressed data, was "linkit-0.1.8.tar", last modified: Mon Jul  3 09:33:52 2023, max compression
```

## Comparing `linkit-0.1.7.tar` & `linkit-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:09.005290 linkit-0.1.7/
--rw-r--r--   0 christianschuermann   (501) staff       (20)     1064 2023-03-06 15:48:51.000000 linkit-0.1.7/LICENSE
--rw-r--r--   0 christianschuermann   (501) staff       (20)       58 2023-03-06 15:48:51.000000 linkit-0.1.7/MANIFEST.in
--rw-r--r--   0 christianschuermann   (501) staff       (20)     4481 2023-04-27 11:19:09.004935 linkit-0.1.7/PKG-INFO
--rw-r--r--   0 christianschuermann   (501) staff       (20)     3833 2023-03-06 15:48:51.000000 linkit-0.1.7/README.md
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.996087 linkit-0.1.7/linkit/
--rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/__init__.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)       63 2023-04-27 11:16:02.000000 linkit-0.1.7/linkit/__version__.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)       87 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/apps.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     1088 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/form_fields.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     2745 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/link.py
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.998759 linkit-0.1.7/linkit/migrations/
--rw-r--r--   0 christianschuermann   (501) staff       (20)      748 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/migrations/0001_initial.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/migrations/__init__.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     2864 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/model_fields.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)      447 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/models.py
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.987099 linkit-0.1.7/linkit/templates/
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.987302 linkit-0.1.7/linkit/templates/django/
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.987503 linkit-0.1.7/linkit/templates/django/forms/
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.999109 linkit-0.1.7/linkit/templates/django/forms/widgets/
--rw-r--r--   0 christianschuermann   (501) staff       (20)     1523 2023-04-18 13:59:43.000000 linkit-0.1.7/linkit/templates/django/forms/widgets/link.html
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:09.004197 linkit-0.1.7/linkit/types/
--rw-r--r--   0 christianschuermann   (501) staff       (20)      311 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/__init__.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     2673 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/contracts.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     1728 2023-04-18 14:03:16.000000 linkit-0.1.7/linkit/types/file.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)      745 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/input.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     1549 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/manager.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     1136 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/model.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     1156 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/page.py
--rw-r--r--   0 christianschuermann   (501) staff       (20)     5044 2023-04-27 11:17:01.000000 linkit-0.1.7/linkit/widgets.py
-drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.997746 linkit-0.1.7/linkit.egg-info/
--rw-r--r--   0 christianschuermann   (501) staff       (20)     4481 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/PKG-INFO
--rw-r--r--   0 christianschuermann   (501) staff       (20)      582 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/SOURCES.txt
--rw-r--r--   0 christianschuermann   (501) staff       (20)        1 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/dependency_links.txt
--rw-r--r--   0 christianschuermann   (501) staff       (20)        7 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/top_level.txt
--rw-r--r--   0 christianschuermann   (501) staff       (20)       38 2023-04-27 11:19:09.005407 linkit-0.1.7/setup.cfg
--rw-r--r--   0 christianschuermann   (501) staff       (20)     2972 2023-03-06 15:48:51.000000 linkit-0.1.7/setup.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.602911 linkit-0.1.8/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1064 2023-03-06 15:48:51.000000 linkit-0.1.8/LICENSE
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       58 2023-03-06 15:48:51.000000 linkit-0.1.8/MANIFEST.in
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     4480 2023-07-03 09:33:52.602599 linkit-0.1.8/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     3832 2023-06-30 14:09:46.000000 linkit-0.1.8/README.md
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.595425 linkit-0.1.8/linkit/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       63 2023-07-03 09:28:38.000000 linkit-0.1.8/linkit/__version__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       87 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/apps.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1088 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/form_fields.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2745 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/link.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.598582 linkit-0.1.8/linkit/migrations/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      748 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/migrations/0001_initial.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/migrations/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2864 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/model_fields.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      447 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/models.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.589568 linkit-0.1.8/linkit/templates/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.589686 linkit-0.1.8/linkit/templates/django/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.589921 linkit-0.1.8/linkit/templates/django/forms/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.598853 linkit-0.1.8/linkit/templates/django/forms/widgets/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1523 2023-04-18 13:59:43.000000 linkit-0.1.8/linkit/templates/django/forms/widgets/link.html
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.602076 linkit-0.1.8/linkit/types/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      311 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/types/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2673 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/types/contracts.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1727 2023-06-30 14:09:43.000000 linkit-0.1.8/linkit/types/file.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      744 2023-06-30 14:09:43.000000 linkit-0.1.8/linkit/types/input.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1549 2023-03-06 15:48:51.000000 linkit-0.1.8/linkit/types/manager.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1134 2023-06-30 14:10:58.000000 linkit-0.1.8/linkit/types/model.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1155 2023-06-30 14:09:43.000000 linkit-0.1.8/linkit/types/page.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     5044 2023-04-27 11:17:01.000000 linkit-0.1.8/linkit/widgets.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 09:33:52.597464 linkit-0.1.8/linkit.egg-info/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     4480 2023-07-03 09:33:52.000000 linkit-0.1.8/linkit.egg-info/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      582 2023-07-03 09:33:52.000000 linkit-0.1.8/linkit.egg-info/SOURCES.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        1 2023-07-03 09:33:52.000000 linkit-0.1.8/linkit.egg-info/dependency_links.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        7 2023-07-03 09:33:52.000000 linkit-0.1.8/linkit.egg-info/top_level.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       38 2023-07-03 09:33:52.603005 linkit-0.1.8/setup.cfg
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2972 2023-03-06 15:48:51.000000 linkit-0.1.8/setup.py
```

### Comparing `linkit-0.1.7/LICENSE` & `linkit-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/PKG-INFO` & `linkit-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkit
-Version: 0.1.7
+Version: 0.1.8
 Summary: Painless link handling - be it a custom model, file or cms page
 Home-page: https://github.com/dreipol/linkit
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -74,15 +74,15 @@
 
 ```
 
 2. Register the new type, preferably in a `AppConfig` `ready` method:
 
 ````python
 from django.apps import AppConfig
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class ContentConfig(AppConfig):
     name = 'contents'
 
     def ready(self):
         from contents.link_types import NewsLinkType
```

### Comparing `linkit-0.1.7/README.md` & `linkit-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ```
 
 2. Register the new type, preferably in a `AppConfig` `ready` method:
 
 ````python
 from django.apps import AppConfig
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class ContentConfig(AppConfig):
     name = 'contents'
 
     def ready(self):
         from contents.link_types import NewsLinkType
```

### Comparing `linkit-0.1.7/linkit/form_fields.py` & `linkit-0.1.8/linkit/form_fields.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit/link.py` & `linkit-0.1.8/linkit/link.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit/migrations/0001_initial.py` & `linkit-0.1.8/linkit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit/model_fields.py` & `linkit-0.1.8/linkit/model_fields.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit/templates/django/forms/widgets/link.html` & `linkit-0.1.8/linkit/templates/django/forms/widgets/link.html`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit/types/contracts.py` & `linkit-0.1.8/linkit/types/contracts.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit/types/file.py` & `linkit-0.1.8/linkit/types/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from filer.fields.file import AdminFileFormField
 from filer.models import File
 
 from linkit.models import FakeLink
 from linkit.types.contracts import LinkType, TypeForm
```

### Comparing `linkit-0.1.7/linkit/types/input.py` & `linkit-0.1.8/linkit/types/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from django.forms import CharField
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from linkit.types.contracts import LinkType, TypeForm
 
 
 class InputTypeForm(TypeForm):
     input = CharField(label=_('Website'), help_text=_('prefix with https, mailto or tel'), max_length=2048)
```

### Comparing `linkit-0.1.7/linkit/types/manager.py` & `linkit-0.1.8/linkit/types/manager.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit/types/model.py` & `linkit-0.1.8/linkit/types/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from django.forms import ModelChoiceField
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from linkit.types.contracts import TypeForm, LinkType
 
 
 class ModelTypeForm(TypeForm):
     def __init__(self, *args, **kwargs):
         """ Set the queryset and label dynamically based on the properties defined on the link type. """
         super().__init__(*args, **kwargs)
         self.fields['model'].queryset = self.link_type.queryset()
-        self.fields['model'].label = force_text(self.link_type.model._meta.verbose_name)
+        self.fields['model'].label = force_str(self.link_type.model._meta.verbose_name)
 
     model = ModelChoiceField(queryset=None)
 
 
 class ModelLinkType(LinkType):
     model = None
     form_class = ModelTypeForm
```

### Comparing `linkit-0.1.7/linkit/types/page.py` & `linkit-0.1.8/linkit/types/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 from cms.forms.fields import PageSelectFormField
 from cms.models import Page
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from linkit.types.contracts import LinkType, TypeForm
 
 
 class PageTypeForm(TypeForm):
     def __init__(self, *args, **kwargs):
         """ Set the queryset and label dynamically based on the properties defined on the link type. """
```

### Comparing `linkit-0.1.7/linkit/widgets.py` & `linkit-0.1.8/linkit/widgets.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/linkit.egg-info/PKG-INFO` & `linkit-0.1.8/linkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkit
-Version: 0.1.7
+Version: 0.1.8
 Summary: Painless link handling - be it a custom model, file or cms page
 Home-page: https://github.com/dreipol/linkit
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -74,15 +74,15 @@
 
 ```
 
 2. Register the new type, preferably in a `AppConfig` `ready` method:
 
 ````python
 from django.apps import AppConfig
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class ContentConfig(AppConfig):
     name = 'contents'
 
     def ready(self):
         from contents.link_types import NewsLinkType
```

### Comparing `linkit-0.1.7/linkit.egg-info/SOURCES.txt` & `linkit-0.1.8/linkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkit-0.1.7/setup.py` & `linkit-0.1.8/setup.py`

 * *Files identical despite different names*

