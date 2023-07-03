# Comparing `tmp/django-slick-reporting-0.9.0.tar.gz` & `tmp/django-slick-reporting-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-slick-reporting-0.9.0.tar", last modified: Wed Jun  7 08:55:44 2023, max compression
+gzip compressed data, was "django-slick-reporting-1.0.0.tar", last modified: Mon Jul  3 11:45:21 2023, max compression
```

## Comparing `django-slick-reporting-0.9.0.tar` & `django-slick-reporting-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-0.9.0/LICENSE.md
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-0.9.0/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9292 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7605 2023-06-05 12:49:44.000000 django-slick-reporting-0.9.0/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.696882 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9292 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1285 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/SOURCES.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/dependency_links.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/requires.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/top_level.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       38 2023-06-05 11:59:25.000000 django-slick-reporting-0.9.0/setup.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-06-07 08:55:39.000000 django-slick-reporting-0.9.0/slick_reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1638 2023-06-06 12:54:30.000000 django-slick-reporting-0.9.0/slick_reporting/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      214 2023-06-06 12:41:34.000000 django-slick-reporting-0.9.0/slick_reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/decorators.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    17166 2023-06-06 12:41:34.000000 django-slick-reporting-0.9.0/slick_reporting/fields.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      198 2023-06-06 12:40:41.000000 django-slick-reporting-0.9.0/slick_reporting/form_factory.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    11412 2023-06-06 12:36:51.000000 django-slick-reporting-0.9.0/slick_reporting/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    38650 2023-06-06 12:41:56.000000 django-slick-reporting-0.9.0/slick_reporting/generator.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1565 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1693 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/registry.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.696882 django-slick-reporting-0.9.0/slick_reporting/static/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7123 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    19417 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/main.js
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.696882 django-slick-reporting-0.9.0/slick_reporting/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1624 2023-06-04 13:48:28.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/base.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2382 2023-06-04 14:00:22.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/js_resources.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4841 2023-06-04 14:16:10.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/simple_report.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/table.html
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-0.9.0/slick_reporting/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2023-06-05 11:59:25.000000 django-slick-reporting-0.9.0/slick_reporting/templatetags/slick_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    18181 2023-06-06 12:42:49.000000 django-slick-reporting-0.9.0/slick_reporting/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.852533 django-slick-reporting-1.0.0/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-1.0.0/LICENSE.md
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-1.0.0/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9292 2023-07-03 11:45:21.852533 django-slick-reporting-1.0.0/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7605 2023-06-11 07:20:46.000000 django-slick-reporting-1.0.0/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.848533 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9292 2023-07-03 11:45:21.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1285 2023-07-03 11:45:21.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/SOURCES.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-07-03 11:45:21.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/dependency_links.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-07-03 11:45:21.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/requires.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-07-03 11:45:21.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-1.0.0/django_slick_reporting.egg-info/top_level.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-07-03 11:45:21.852533 django-slick-reporting-1.0.0/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       38 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.852533 django-slick-reporting-1.0.0/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-07-03 11:45:19.000000 django-slick-reporting-1.0.0/slick_reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1638 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/slick_reporting/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      214 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/slick_reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2023-05-30 09:54:31.000000 django-slick-reporting-1.0.0/slick_reporting/decorators.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    17819 2023-06-09 14:53:23.000000 django-slick-reporting-1.0.0/slick_reporting/fields.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      198 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/slick_reporting/form_factory.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    11412 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/slick_reporting/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    41706 2023-06-09 15:03:00.000000 django-slick-reporting-1.0.0/slick_reporting/generator.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1565 2023-05-30 09:54:31.000000 django-slick-reporting-1.0.0/slick_reporting/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1693 2023-05-30 09:54:31.000000 django-slick-reporting-1.0.0/slick_reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.848533 django-slick-reporting-1.0.0/slick_reporting/static/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.852533 django-slick-reporting-1.0.0/slick_reporting/static/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7123 2023-05-30 09:54:31.000000 django-slick-reporting-1.0.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    19417 2023-05-30 09:54:31.000000 django-slick-reporting-1.0.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-1.0.0/slick_reporting/static/slick_reporting/main.js
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.848533 django-slick-reporting-1.0.0/slick_reporting/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.852533 django-slick-reporting-1.0.0/slick_reporting/templates/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      770 2023-06-11 08:21:07.000000 django-slick-reporting-1.0.0/slick_reporting/templates/slick_reporting/base.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2382 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/slick_reporting/templates/slick_reporting/js_resources.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4841 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/slick_reporting/templates/slick_reporting/simple_report.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-1.0.0/slick_reporting/templates/slick_reporting/table.html
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-03 11:45:21.852533 django-slick-reporting-1.0.0/slick_reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-1.0.0/slick_reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2023-06-07 08:58:21.000000 django-slick-reporting-1.0.0/slick_reporting/templatetags/slick_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    18254 2023-06-09 14:53:23.000000 django-slick-reporting-1.0.0/slick_reporting/views.py
```

### Comparing `django-slick-reporting-0.9.0/LICENSE.md` & `django-slick-reporting-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/PKG-INFO` & `django-slick-reporting-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.9.0
+Version: 1.0.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
@@ -55,23 +55,22 @@
 
 
 Django Slick Reporting
 ======================
 
 A one stop reports engine with batteries included.
 
-This is project is an extract of the reporting engine of `Django ERP Framework <https://github.com/RamezIssac/django-erp-framework>`_
-
 Features
 --------
 
 - Effortlessly create Simple, Grouped, Time series and Crosstab reports in a handful of code lines.
-- Create your Custom Calculation easily, which will be integrated with the above reports types
+- Create Chart(s) for your reports with a single line of code.
+- Create Custom complex Calculation.
 - Optimized for speed.
-- Batteries included! Highcharts & Chart.js charting capabilities , DataTable.net & easily customizable Bootstrap form.
+- Easily extendable.
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install django-slick-reporting.
 
 .. code-block:: console
@@ -90,15 +89,15 @@
 
     # in your urls.py
     path("path-to-report", TotalProductSales.as_view())
 
 
     # in views.py
     from django.db.models import Sum
-    from slick_reporting.views import ReportView
+    from slick_reporting.views import ReportView, Chart
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
 
     class TotalProductSales(ReportView):
 
         report_model = MySalesItems
@@ -107,32 +106,32 @@
         columns = [
             "title",
             SlickReportField.create(Sum, "quantity"),
             SlickReportField.create(Sum, "value", name="sum__value"),
         ]
 
         chart_settings = [
-            {
-                "type": "column",
-                "data_source": ["sum__value"],
-                "plot_total": False,
-                "title_source": "title",
-                "title": _("Detailed Columns"),
-            },
+            Chart(
+                "Total sold $",
+                Chart.BAR,
+                data_source="value__sum",
+                title_source="title",
+            ),
         ]
 
 
-To get something like this
+To get something this
 
 .. image:: https://i.ibb.co/SvxTM23/Selection-294.png
     :target: https://i.ibb.co/SvxTM23/Selection-294.png
     :alt: Shipped in View Page
 
 
-You can do a monthly time series :
+Time Series
+-----------
 
 
 .. code-block:: python
 
     # in views.py
     from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
@@ -141,52 +140,96 @@
 
     class MonthlyProductSales(ReportView):
         report_model = MySalesItems
         date_field = "date_placed"
         group_by = "product"
         columns = ["name", "sku"]
 
-        # Analogy for time series
-        time_series_pattern = "monthly"
+        # Settings for creating time series report
+        time_series_pattern = (
+            "monthly"  # or "yearly" , "weekly" , "daily" , others and custom patterns
+        )
         time_series_columns = [
-            SlickReportField.create(Sum, "quantity", name="sum__quantity")
+            SlickReportField.create(
+                Sum, "value", verbose_name=_("Sales Value"), name="value"
+            )
+        ]
+
+        chart_settings = [
+            Chart(
+                _("Total Sales Monthly"),
+                Chart.PIE,
+                data_source=["value"],
+                title_source=["name"],
+                plot_total=True,
+            ),
         ]
 
 
-This would return a table looking something like this:
+.. image:: https://github.com/ra-systems/django-slick-reporting/blob/develop/docs/source/report_view/_static/timeseries.png?raw=true
+    :alt: Time Series Report
+    :align: center
+
+Cross Tab
+---------
+
+.. code-block:: python
+
+        # in views.py
+        from slick_reporting.views import ReportView
+        from slick_reporting.fields import SlickReportField
+        from .models import MySalesItems
+
+
+        class MyCrosstabReport(ReportView):
 
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product Name | SKU                  | Total Quantity  | Total Quantity | Total Quantity in ... | Total Quantity in December 20 |
-|              |                      | in Jan 20       | in Feb 20      |                       |                               |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 1    | <from product model> | 10              | 15             | ...                   | 14                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 2    | <from product model> | 11              | 12             | ...                   | 12                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 3    | <from product model> | 17              | 12             | ...                   | 17                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
+            crosstab_field = "client"
+            crosstab_ids = [1, 2, 3]
+            crosstab_columns = [
+                SlickReportField.create(Sum, "value", verbose_name=_("Value for")),
+            ]
+            crosstab_compute_remainder = True
 
-*This example code assumes your "MySalesItems" model contains the fields `product` as foreign key,  `quantity` as number , and `date_placed` as a date field. It also assumes your `Product` model has an SKU field.. Change those to better suit your structure.*
+            columns = [
+                "some_optional_field",
+                # You can customize where the crosstab columns are displayed in relation to the other columns
+                "__crosstab__",
+                # This is the same as the Same as the calculation in the crosstab, but this one will be on the whole set. IE total value
+                SlickReportField.create(Sum, "value", verbose_name=_("Total Value")),
+            ]
 
 
---
+.. image:: https://github.com/ra-systems/django-slick-reporting/blob/develop/docs/source/report_view/_static/crosstab.png?raw=true
+   :alt: Homepage
+   :align: center
 
-**On a low level**
 
+Low level
+---------
+
+The view is a wrapper over the `ReportGenerator` class, which is the core of the reporting engine.
 You can interact with the `ReportGenerator` using same syntax as used with the `ReportView` .
 
 .. code-block:: python
 
     from slick_reporting.generator import ReportGenerator
     from .models import MySalesModel
 
-    report = ReportGenerator(
+
+    class MyReport(ReportGenerator):
+        report_model = MySalesModel
+        group_by = "product"
+        columns = ["title", "__total__"]
+
+
+    # OR
+    my_report = ReportGenerator(
         report_model=MySalesModel, group_by="product", columns=["title", "__total__"]
     )
-    report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
+    my_report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
 
 
 This is just a scratch, for more please visit the documentation 
 
 Batteries Included
 ------------------
 
@@ -217,15 +260,14 @@
 ----------
 
 This project is young and can use your support.
 
 Some of the ideas / features that ought be added
 
 * Support Other backends like SQL Alchemy & Pandas
-* Support Time Series and Crosstab at the same time
 
 
 Running tests
 -----------------
 Create a virtual environment (maybe with `virtual slick_reports_test`), activate it; Then ,
  
 .. code-block:: console
```

### Comparing `django-slick-reporting-0.9.0/README.rst` & `django-slick-reporting-1.0.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -17,23 +17,22 @@
 
 
 Django Slick Reporting
 ======================
 
 A one stop reports engine with batteries included.
 
-This is project is an extract of the reporting engine of `Django ERP Framework <https://github.com/RamezIssac/django-erp-framework>`_
-
 Features
 --------
 
 - Effortlessly create Simple, Grouped, Time series and Crosstab reports in a handful of code lines.
-- Create your Custom Calculation easily, which will be integrated with the above reports types
+- Create Chart(s) for your reports with a single line of code.
+- Create Custom complex Calculation.
 - Optimized for speed.
-- Batteries included! Highcharts & Chart.js charting capabilities , DataTable.net & easily customizable Bootstrap form.
+- Easily extendable.
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install django-slick-reporting.
 
 .. code-block:: console
@@ -52,15 +51,15 @@
 
     # in your urls.py
     path("path-to-report", TotalProductSales.as_view())
 
 
     # in views.py
     from django.db.models import Sum
-    from slick_reporting.views import ReportView
+    from slick_reporting.views import ReportView, Chart
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
 
     class TotalProductSales(ReportView):
 
         report_model = MySalesItems
@@ -69,32 +68,32 @@
         columns = [
             "title",
             SlickReportField.create(Sum, "quantity"),
             SlickReportField.create(Sum, "value", name="sum__value"),
         ]
 
         chart_settings = [
-            {
-                "type": "column",
-                "data_source": ["sum__value"],
-                "plot_total": False,
-                "title_source": "title",
-                "title": _("Detailed Columns"),
-            },
+            Chart(
+                "Total sold $",
+                Chart.BAR,
+                data_source="value__sum",
+                title_source="title",
+            ),
         ]
 
 
-To get something like this
+To get something this
 
 .. image:: https://i.ibb.co/SvxTM23/Selection-294.png
     :target: https://i.ibb.co/SvxTM23/Selection-294.png
     :alt: Shipped in View Page
 
 
-You can do a monthly time series :
+Time Series
+-----------
 
 
 .. code-block:: python
 
     # in views.py
     from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
@@ -103,52 +102,96 @@
 
     class MonthlyProductSales(ReportView):
         report_model = MySalesItems
         date_field = "date_placed"
         group_by = "product"
         columns = ["name", "sku"]
 
-        # Analogy for time series
-        time_series_pattern = "monthly"
+        # Settings for creating time series report
+        time_series_pattern = (
+            "monthly"  # or "yearly" , "weekly" , "daily" , others and custom patterns
+        )
         time_series_columns = [
-            SlickReportField.create(Sum, "quantity", name="sum__quantity")
+            SlickReportField.create(
+                Sum, "value", verbose_name=_("Sales Value"), name="value"
+            )
+        ]
+
+        chart_settings = [
+            Chart(
+                _("Total Sales Monthly"),
+                Chart.PIE,
+                data_source=["value"],
+                title_source=["name"],
+                plot_total=True,
+            ),
         ]
 
 
-This would return a table looking something like this:
+.. image:: https://github.com/ra-systems/django-slick-reporting/blob/develop/docs/source/report_view/_static/timeseries.png?raw=true
+    :alt: Time Series Report
+    :align: center
+
+Cross Tab
+---------
+
+.. code-block:: python
+
+        # in views.py
+        from slick_reporting.views import ReportView
+        from slick_reporting.fields import SlickReportField
+        from .models import MySalesItems
+
+
+        class MyCrosstabReport(ReportView):
 
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product Name | SKU                  | Total Quantity  | Total Quantity | Total Quantity in ... | Total Quantity in December 20 |
-|              |                      | in Jan 20       | in Feb 20      |                       |                               |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 1    | <from product model> | 10              | 15             | ...                   | 14                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 2    | <from product model> | 11              | 12             | ...                   | 12                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 3    | <from product model> | 17              | 12             | ...                   | 17                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
+            crosstab_field = "client"
+            crosstab_ids = [1, 2, 3]
+            crosstab_columns = [
+                SlickReportField.create(Sum, "value", verbose_name=_("Value for")),
+            ]
+            crosstab_compute_remainder = True
 
-*This example code assumes your "MySalesItems" model contains the fields `product` as foreign key,  `quantity` as number , and `date_placed` as a date field. It also assumes your `Product` model has an SKU field.. Change those to better suit your structure.*
+            columns = [
+                "some_optional_field",
+                # You can customize where the crosstab columns are displayed in relation to the other columns
+                "__crosstab__",
+                # This is the same as the Same as the calculation in the crosstab, but this one will be on the whole set. IE total value
+                SlickReportField.create(Sum, "value", verbose_name=_("Total Value")),
+            ]
 
 
---
+.. image:: https://github.com/ra-systems/django-slick-reporting/blob/develop/docs/source/report_view/_static/crosstab.png?raw=true
+   :alt: Homepage
+   :align: center
 
-**On a low level**
 
+Low level
+---------
+
+The view is a wrapper over the `ReportGenerator` class, which is the core of the reporting engine.
 You can interact with the `ReportGenerator` using same syntax as used with the `ReportView` .
 
 .. code-block:: python
 
     from slick_reporting.generator import ReportGenerator
     from .models import MySalesModel
 
-    report = ReportGenerator(
+
+    class MyReport(ReportGenerator):
+        report_model = MySalesModel
+        group_by = "product"
+        columns = ["title", "__total__"]
+
+
+    # OR
+    my_report = ReportGenerator(
         report_model=MySalesModel, group_by="product", columns=["title", "__total__"]
     )
-    report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
+    my_report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
 
 
 This is just a scratch, for more please visit the documentation 
 
 Batteries Included
 ------------------
 
@@ -179,15 +222,14 @@
 ----------
 
 This project is young and can use your support.
 
 Some of the ideas / features that ought be added
 
 * Support Other backends like SQL Alchemy & Pandas
-* Support Time Series and Crosstab at the same time
 
 
 Running tests
 -----------------
 Create a virtual environment (maybe with `virtual slick_reports_test`), activate it; Then ,
  
 .. code-block:: console
```

### Comparing `django-slick-reporting-0.9.0/django_slick_reporting.egg-info/PKG-INFO` & `django-slick-reporting-1.0.0/django_slick_reporting.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.9.0
+Version: 1.0.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
@@ -55,23 +55,22 @@
 
 
 Django Slick Reporting
 ======================
 
 A one stop reports engine with batteries included.
 
-This is project is an extract of the reporting engine of `Django ERP Framework <https://github.com/RamezIssac/django-erp-framework>`_
-
 Features
 --------
 
 - Effortlessly create Simple, Grouped, Time series and Crosstab reports in a handful of code lines.
-- Create your Custom Calculation easily, which will be integrated with the above reports types
+- Create Chart(s) for your reports with a single line of code.
+- Create Custom complex Calculation.
 - Optimized for speed.
-- Batteries included! Highcharts & Chart.js charting capabilities , DataTable.net & easily customizable Bootstrap form.
+- Easily extendable.
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install django-slick-reporting.
 
 .. code-block:: console
@@ -90,15 +89,15 @@
 
     # in your urls.py
     path("path-to-report", TotalProductSales.as_view())
 
 
     # in views.py
     from django.db.models import Sum
-    from slick_reporting.views import ReportView
+    from slick_reporting.views import ReportView, Chart
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
 
     class TotalProductSales(ReportView):
 
         report_model = MySalesItems
@@ -107,32 +106,32 @@
         columns = [
             "title",
             SlickReportField.create(Sum, "quantity"),
             SlickReportField.create(Sum, "value", name="sum__value"),
         ]
 
         chart_settings = [
-            {
-                "type": "column",
-                "data_source": ["sum__value"],
-                "plot_total": False,
-                "title_source": "title",
-                "title": _("Detailed Columns"),
-            },
+            Chart(
+                "Total sold $",
+                Chart.BAR,
+                data_source="value__sum",
+                title_source="title",
+            ),
         ]
 
 
-To get something like this
+To get something this
 
 .. image:: https://i.ibb.co/SvxTM23/Selection-294.png
     :target: https://i.ibb.co/SvxTM23/Selection-294.png
     :alt: Shipped in View Page
 
 
-You can do a monthly time series :
+Time Series
+-----------
 
 
 .. code-block:: python
 
     # in views.py
     from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
@@ -141,52 +140,96 @@
 
     class MonthlyProductSales(ReportView):
         report_model = MySalesItems
         date_field = "date_placed"
         group_by = "product"
         columns = ["name", "sku"]
 
-        # Analogy for time series
-        time_series_pattern = "monthly"
+        # Settings for creating time series report
+        time_series_pattern = (
+            "monthly"  # or "yearly" , "weekly" , "daily" , others and custom patterns
+        )
         time_series_columns = [
-            SlickReportField.create(Sum, "quantity", name="sum__quantity")
+            SlickReportField.create(
+                Sum, "value", verbose_name=_("Sales Value"), name="value"
+            )
+        ]
+
+        chart_settings = [
+            Chart(
+                _("Total Sales Monthly"),
+                Chart.PIE,
+                data_source=["value"],
+                title_source=["name"],
+                plot_total=True,
+            ),
         ]
 
 
-This would return a table looking something like this:
+.. image:: https://github.com/ra-systems/django-slick-reporting/blob/develop/docs/source/report_view/_static/timeseries.png?raw=true
+    :alt: Time Series Report
+    :align: center
+
+Cross Tab
+---------
+
+.. code-block:: python
+
+        # in views.py
+        from slick_reporting.views import ReportView
+        from slick_reporting.fields import SlickReportField
+        from .models import MySalesItems
+
+
+        class MyCrosstabReport(ReportView):
 
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product Name | SKU                  | Total Quantity  | Total Quantity | Total Quantity in ... | Total Quantity in December 20 |
-|              |                      | in Jan 20       | in Feb 20      |                       |                               |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 1    | <from product model> | 10              | 15             | ...                   | 14                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 2    | <from product model> | 11              | 12             | ...                   | 12                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
-| Product 3    | <from product model> | 17              | 12             | ...                   | 17                            |
-+--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
+            crosstab_field = "client"
+            crosstab_ids = [1, 2, 3]
+            crosstab_columns = [
+                SlickReportField.create(Sum, "value", verbose_name=_("Value for")),
+            ]
+            crosstab_compute_remainder = True
 
-*This example code assumes your "MySalesItems" model contains the fields `product` as foreign key,  `quantity` as number , and `date_placed` as a date field. It also assumes your `Product` model has an SKU field.. Change those to better suit your structure.*
+            columns = [
+                "some_optional_field",
+                # You can customize where the crosstab columns are displayed in relation to the other columns
+                "__crosstab__",
+                # This is the same as the Same as the calculation in the crosstab, but this one will be on the whole set. IE total value
+                SlickReportField.create(Sum, "value", verbose_name=_("Total Value")),
+            ]
 
 
---
+.. image:: https://github.com/ra-systems/django-slick-reporting/blob/develop/docs/source/report_view/_static/crosstab.png?raw=true
+   :alt: Homepage
+   :align: center
 
-**On a low level**
 
+Low level
+---------
+
+The view is a wrapper over the `ReportGenerator` class, which is the core of the reporting engine.
 You can interact with the `ReportGenerator` using same syntax as used with the `ReportView` .
 
 .. code-block:: python
 
     from slick_reporting.generator import ReportGenerator
     from .models import MySalesModel
 
-    report = ReportGenerator(
+
+    class MyReport(ReportGenerator):
+        report_model = MySalesModel
+        group_by = "product"
+        columns = ["title", "__total__"]
+
+
+    # OR
+    my_report = ReportGenerator(
         report_model=MySalesModel, group_by="product", columns=["title", "__total__"]
     )
-    report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
+    my_report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
 
 
 This is just a scratch, for more please visit the documentation 
 
 Batteries Included
 ------------------
 
@@ -217,15 +260,14 @@
 ----------
 
 This project is young and can use your support.
 
 Some of the ideas / features that ought be added
 
 * Support Other backends like SQL Alchemy & Pandas
-* Support Time Series and Crosstab at the same time
 
 
 Running tests
 -----------------
 Create a virtual environment (maybe with `virtual slick_reports_test`), activate it; Then ,
  
 .. code-block:: console
```

### Comparing `django-slick-reporting-0.9.0/django_slick_reporting.egg-info/SOURCES.txt` & `django-slick-reporting-1.0.0/django_slick_reporting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/setup.cfg` & `django-slick-reporting-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/app_settings.py` & `django-slick-reporting-1.0.0/slick_reporting/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/decorators.py` & `django-slick-reporting-1.0.0/slick_reporting/decorators.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/fields.py` & `django-slick-reporting-1.0.0/slick_reporting/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     report_model = None
     """The model on which the computation would occur"""
 
     queryset = None
     """The queryset on which the computation would occur"""
 
     group_by = None
+    group_by_custom_querysets = None
     plus_side_q = None
     minus_side_q = None
 
     base_kwargs_filters = None
     base_q_filters = None
 
     _require_classes = None
@@ -101,25 +102,30 @@
         minus_side_q=None,
         report_model=None,
         queryset=None,
         calculation_field=None,
         calculation_method=None,
         date_field="",
         group_by=None,
+        group_by_custom_querysets=None,
     ):
         super(SlickReportField, self).__init__()
         self.date_field = date_field
         self.report_model = self.report_model or report_model
         self.queryset = self.queryset or queryset
         self.queryset = (
             self.report_model._default_manager.all()
             if self.queryset is None
             else self.queryset
         )
 
+        self.group_by_custom_querysets = (
+            self.group_by_custom_querysets or group_by_custom_querysets
+        )
+
         self.calculation_field = (
             calculation_field if calculation_field else self.calculation_field
         )
         self.calculation_method = (
             calculation_method if calculation_method else self.calculation_method
         )
         self.plus_side_q = self.plus_side_q or plus_side_q
@@ -144,15 +150,20 @@
         return qs.filter(*self.plus_side_q)
 
     def apply_q_minus_filter(self, qs):
         return qs.filter(*self.minus_side_q)
 
     def apply_aggregation(self, queryset, group_by=""):
         annotation = self.calculation_method(self.calculation_field)
-        if group_by:
+        if self.group_by_custom_querysets:
+            output = []
+            for group_by_query in self.group_by_custom_querysets:
+                output.append(group_by_query.aggregate(annotation))
+            return output
+        elif group_by:
             queryset = queryset.values(group_by).annotate(annotation)
         else:
             queryset = queryset.aggregate(annotation)
         return queryset
 
     def init_preparation(self, q_filters=None, kwargs_filters=None, **kwargs):
         """
@@ -166,15 +177,14 @@
 
         dep_values = self._prepare_dependencies(q_filters, kwargs_filters.copy())
 
         debit_results, credit_results = self.prepare(
             q_filters, kwargs_filters, **kwargs
         )
         self._cache = debit_results, credit_results, dep_values
-        return self._cache
 
     def prepare(self, q_filters=None, kwargs_filters=None, **kwargs):
         """
         This is the first hook where you can customize the calculation away from the Django Query aggregation method
         This method et called with all available parameters , so you can prepare the results for the whole set and save
         it in a local cache (like self._cache) .
         The flow will later call the method `resolve`,  giving you the id, for you to return it respective calculation
@@ -281,27 +291,34 @@
             if name and d != name:
                 continue
             d_instance = dependencies_value[d]["instance"]
             dep_results[d] = d_instance.resolve(current_obj)
         return dep_results
 
     def extract_data(self, cached, current_obj):
-        group_by = "" if self.prevent_group_by else self.group_by
+        group_by = (
+            ""
+            if self.prevent_group_by
+            else (self.group_by or self.group_by_custom_querysets)
+        )
         debit_value = 0
         credit_value = 0
         annotation = self.get_annotation_name()
 
         cached_debit, cached_credit, dependencies_value = cached
 
         if cached_debit or cached_credit:
             debit = None
             if cached_debit is not None:
                 if not group_by:
                     x = list(cached_debit.keys())[0]
                     debit_value = cached_debit[x]
+                elif self.group_by_custom_querysets:
+                    debit = cached_debit[int(current_obj)]
+                    debit_value = debit[annotation]
                 else:
                     for i, x in enumerate(cached_debit):
                         if str(x[group_by]) == current_obj:
                             debit = cached_debit[i]
                             break
                     if debit:
                         debit_value = debit[annotation]
```

### Comparing `django-slick-reporting-0.9.0/slick_reporting/forms.py` & `django-slick-reporting-1.0.0/slick_reporting/forms.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/generator.py` & `django-slick-reporting-1.0.0/slick_reporting/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,18 @@
     """If set, the report will use this field to filter the end date, default to date_field"""
 
     print_flag = None
 
     group_by = None
     """The field to use for grouping, if not set then the report is expected to be a sub version of the report model"""
 
+    group_by_custom_querysets = None
+    """A List of querysets representing different group by options"""
+    group_by_custom_querysets_column_verbose_name = ""
+
     columns = None
     """A list of column names.
     Columns names can be 
 
     1. A Computation Field
 
     2. If group_by is set, then any field on the group_by model
@@ -119,14 +123,16 @@
 
     crosstab_columns = None
     """The computation fields which will be computed for each crosstab-ed ids """
 
     crosstab_ids = None
     """A list is the ids to create a crosstab report on"""
 
+    crosstab_ids_custom_filters = None
+
     crosstab_compute_remainder = True
     """Include an an extra crosstab_columns for the outer group ( ie: all expects those `crosstab_ids`) """
 
     limit_records = None
     """Serves are a main limit to  the returned data of the report_model.
     Can be beneficial if the results may be huge.
     """
@@ -148,21 +154,23 @@
         main_queryset=None,
         start_date=None,
         end_date=None,
         date_field=None,
         q_filters=None,
         kwargs_filters=None,
         group_by=None,
+        group_by_custom_querysets=None,
         columns=None,
         time_series_pattern=None,
         time_series_columns=None,
         time_series_custom_dates=None,
         crosstab_field=None,
         crosstab_columns=None,
         crosstab_ids=None,
+        crosstab_ids_custom_filters=None,
         crosstab_compute_remainder=None,
         swap_sign=False,
         show_empty_records=None,
         print_flag=False,
         doc_type_plus_list=None,
         doc_type_minus_list=None,
         limit_records=False,
@@ -236,14 +244,18 @@
 
         self.q_filters = q_filters or []
         self.kwargs_filters = kwargs_filters or {}
         self.crosstab_field = self.crosstab_field or crosstab_field
 
         self.crosstab_columns = crosstab_columns or self.crosstab_columns or []
         self.crosstab_ids = self.crosstab_ids or crosstab_ids or []
+        self.crosstab_ids_custom_filters = (
+            self.crosstab_ids_custom_filters or crosstab_ids_custom_filters or []
+        )
+
         self.crosstab_compute_remainder = (
             self.crosstab_compute_remainder
             if crosstab_compute_remainder is None
             else crosstab_compute_remainder
         )
 
         self.format_row = format_row_func or self._default_format_row
@@ -253,14 +265,18 @@
         )
         # todo revise & move somewhere nicer, List Report need to override the resetting of order
         main_queryset = self._remove_order(main_queryset)
 
         self.columns = columns or self.columns or []
         self.group_by = group_by or self.group_by
 
+        self.group_by_custom_querysets = (
+            group_by_custom_querysets or self.group_by_custom_querysets or []
+        )
+
         self.time_series_pattern = self.time_series_pattern or time_series_pattern
         self.time_series_columns = self.time_series_columns or time_series_columns
         self.time_series_custom_dates = (
             self.time_series_custom_dates or time_series_custom_dates
         )
         self.container_class = container_class
 
@@ -311,23 +327,26 @@
         self.doc_type_minus_list = (
             list(doc_type_minus_list) if doc_type_minus_list else doc_types[1]
         )
 
         self.swap_sign = self.swap_sign or swap_sign
         self.limit_records = self.limit_records or limit_records
 
-        # in case of a group by, do we show a grouped by model data regardless of their appearance in the results
-        # a client who didn't make a transaction during the date period.
+        # todo delete this
         self.show_empty_records = False  # show_empty_records if show_empty_records else self.show_empty_records
-        # Looks like this options is harder then what i thought as it interfere with the usual filtering of the report
 
         # Preparing actions
         self._parse()
-        if self.group_by:
+        if self.group_by_custom_querysets:
+            self.main_queryset = [
+                {"__index__": i} for i, v in enumerate(self.group_by_custom_querysets)
+            ]
+        elif self.group_by:
             self.main_queryset = self._apply_queryset_options(main_queryset)
+
             if type(self.group_by_field) is ForeignKey:
                 ids = self.main_queryset.values_list(
                     self.group_by_field_attname
                 ).distinct()
                 # uses the same logic that is in Django's query.py when fields is empty in values() call
                 concrete_fields = [
                     f.name
@@ -380,32 +399,35 @@
 
         if filters:
             query = query.filter(**filters)
         if fields:
             return query.values(*fields)
         return query.values()
 
-    def _construct_crosstab_filter(self, col_data):
+    def _construct_crosstab_filter(self, col_data, queryset_filters=None):
         """
         In charge of adding the needed crosstab filter, specific to the case of is_remainder or not
         :param col_data:
         :return:
         """
+        if queryset_filters:
+            return queryset_filters[0], queryset_filters[1]
+
         if "__" in col_data["crosstab_field"]:
             column_name = col_data["crosstab_field"]
         else:
             field = get_field_from_query_text(
                 col_data["crosstab_field"], self.report_model
             )
             column_name = field.column
-        if col_data["is_remainder"]:
+        if col_data["is_remainder"] and not queryset_filters:
             filters = [~Q(**{f"{column_name}__in": self.crosstab_ids})]
         else:
             filters = [Q(**{f"{column_name}": col_data["id"]})]
-        return filters
+        return filters, {}
 
     def _prepare_report_dependencies(self):
         from .fields import SlickReportField
 
         all_columns = (
             ("normal", self._parsed_columns),
             ("time_series", self._time_series_parsed_columns),
@@ -452,32 +474,41 @@
                 report_class = klass(
                     self.doc_type_plus_list,
                     self.doc_type_minus_list,
                     group_by=self.group_by,
                     report_model=self.report_model,
                     date_field=self.date_field,
                     queryset=self.queryset,
+                    group_by_custom_querysets=self.group_by_custom_querysets,
                 )
 
                 q_filters = None
                 date_filter = {
-                    f"{self.date_field}__gte": col_data.get(
+                    f"{self.start_date_field_name}__gte": col_data.get(
                         "start_date", self.start_date
                     ),
-                    f"{self.date_field}__lt": col_data.get("end_date", self.end_date),
+                    f"{self.end_date_field_name}__lt": col_data.get(
+                        "end_date", self.end_date
+                    ),
                 }
                 date_filter.update(self.kwargs_filters)
-                if window == "crosstab":
-                    q_filters = self._construct_crosstab_filter(col_data)
+                if (
+                    window == "crosstab"
+                    or col_data.get("computation_flag", "") == "crosstab"
+                ):
+                    q_filters, kw_filters = col_data["queryset_filters"]
+                    date_filter.update(kw_filters)
 
                 report_class.init_preparation(q_filters, date_filter)
                 self.report_fields_classes[name] = report_class
 
-    @staticmethod
-    def get_primary_key_name(model):
+    # @staticmethod
+    def get_primary_key_name(self, model):
+        if self.group_by_custom_querysets:
+            return "__index__"
         for field in model._meta.fields:
             if field.primary_key:
                 return field.attname
         return ""
 
     def _get_record_data(self, obj, columns):
         """
@@ -485,15 +516,18 @@
         :param obj: current row
         :param: columns： The columns we iterate on
         :return: a dict object containing all needed data
         """
 
         data = {}
         group_by_val = None
-        if self.group_by:
+        if self.group_by_custom_querysets:
+            group_by_val = str(obj["__index__"])
+
+        elif self.group_by:
             if self.group_by_field.related_model and "__" not in self.group_by:
                 primary_key_name = self.get_primary_key_name(
                     self.group_by_field.related_model
                 )
             else:
                 primary_key_name = self.group_by_field_attname
 
@@ -506,17 +540,19 @@
 
                 if col_data.get("source", "") == "attribute_field":
                     data[name] = col_data["ref"](self, obj, data)
                 elif col_data.get("source", "") == "container_class_attribute_field":
                     data[name] = col_data["ref"](obj, data)
 
                 elif (
-                    col_data.get("source", "") == "magic_field" and self.group_by
+                    col_data.get("source", "") == "magic_field"
+                    and (self.group_by or self.group_by_custom_querysets)
                 ) or (self.time_series_pattern and not self.group_by):
                     source = self._report_fields_dependencies[window].get(name, False)
+
                     if source:
                         computation_class = self.report_fields_classes[source]
                         value = computation_class.get_dependency_value(
                             group_by_val, col_data["ref"].name
                         )
                     else:
                         try:
@@ -555,24 +591,35 @@
         Hook where you can format row values like properly format a date
         :param row_obj:
         :return:
         """
         return row_obj
 
     @classmethod
-    def check_columns(cls, columns, group_by, report_model, container_class=None):
+    def check_columns(
+        cls,
+        columns,
+        group_by,
+        report_model,
+        container_class=None,
+        group_by_custom_querysets=None,
+    ):
         """
         Check and parse the columns, throw errors in case an item in the columns cant not identified
         :param columns: List of columns
         :param group_by: group by field if any
         :param report_model: the report model
         :param container_class: a class to search for custom columns attribute in, typically the ReportView
         :return: List of dict, each dict contains relevant data to the respective field in `columns`
         """
         group_by_model = None
+        if group_by_custom_querysets:
+            if "__index__" not in columns:
+                columns.insert(0, "__index__")
+
         if group_by:
             try:
                 group_by_field = [
                     x
                     for x in report_model._meta.get_fields()
                     if x.name == group_by.split("__")[0]
                 ][0]
@@ -633,14 +680,27 @@
                     "source": "magic_field",
                     "ref": magic_field_class,
                     "type": magic_field_class.type,
                     "is_summable": magic_field_class.is_summable,
                 }
             else:
                 # A database field
+                if group_by_custom_querysets and col == "__index__":
+                    # group by custom queryset special case: which is the index
+                    col_data = {
+                        "name": col,
+                        "verbose_name": cls.group_by_custom_querysets_column_verbose_name,
+                        "source": "database",
+                        "ref": "",
+                        "type": "text",
+                    }
+                    col_data.update(options)
+                    parsed_columns.append(col_data)
+                    continue
+
                 model_to_use = (
                     group_by_model
                     if group_by and "__" not in group_by
                     else report_model
                 )
                 group_by_str = str(group_by)
                 if "__" in group_by_str:
@@ -674,19 +734,23 @@
                 }
             col_data.update(options)
             parsed_columns.append(col_data)
         return parsed_columns
 
     def _parse(self):
         self.parsed_columns = self.check_columns(
-            self.columns, self.group_by, self.report_model, self.container_class
+            self.columns,
+            self.group_by,
+            self.report_model,
+            self.container_class,
+            self.group_by_custom_querysets,
         )
         self._parsed_columns = list(self.parsed_columns)
-        self._time_series_parsed_columns = self.get_time_series_parsed_columns()
         self._crosstab_parsed_columns = self.get_crosstab_parsed_columns()
+        self._time_series_parsed_columns = self.get_time_series_parsed_columns()
 
     def get_database_columns(self):
         return [
             col["name"]
             for col in self.parsed_columns
             if "source" in col and col["source"] == "database"
         ]
@@ -747,14 +811,26 @@
                         "ref": magic_field_class,
                         "start_date": dt[0],
                         "end_date": dt[1],
                         "source": "magic_field" if magic_field_class else "",
                         "is_summable": magic_field_class.is_summable,
                     }
                 )
+
+            # append the crosstab fields, if they exist, on the time_series
+            if self._crosstab_parsed_columns:
+                for parsed_col in self._crosstab_parsed_columns:
+                    parsed_col = parsed_col.copy()
+                    parsed_col["name"] = (
+                        parsed_col["name"] + "TS" + dt[1].strftime("%Y%m%d")
+                    )
+                    parsed_col["start_date"] = dt[0]
+                    parsed_col["end_date"] = dt[1]
+                    _values.append(parsed_col)
+
         return _values
 
     def get_time_series_field_verbose_name(
         self, computation_class, date_period, index, series, pattern=None
     ):
         """
         Sent the column data to construct a verbose name.
@@ -819,45 +895,57 @@
 
     def get_crosstab_parsed_columns(self):
         """
         Return a list of the columns analyzed , with reference to computation field and everything
         :return:
         """
         report_columns = self.crosstab_columns or []
-        ids = list(self.crosstab_ids)
-        if self.crosstab_compute_remainder:
+
+        ids = list(self.crosstab_ids) or list(self.crosstab_ids_custom_filters)
+        if self.crosstab_compute_remainder and not self.crosstab_ids_custom_filters:
             ids.append("----")
         output_cols = []
+
         ids_length = len(ids) - 1
-        for counter, id in enumerate(ids):
+        for counter, crosstab_id in enumerate(ids):
+            queryset_filters = None
+
+            if self.crosstab_ids_custom_filters:
+                queryset_filters = crosstab_id
+                crosstab_id = counter
+
             for col in report_columns:
                 magic_field_class = None
                 if type(col) is str:
                     magic_field_class = field_registry.get_field_by_name(col)
                 elif issubclass(col, SlickReportField):
                     magic_field_class = col
 
-                output_cols.append(
-                    {
-                        "name": f"{magic_field_class.name}CT{id}",
-                        "original_name": magic_field_class.name,
-                        "verbose_name": self.get_crosstab_field_verbose_name(
-                            magic_field_class, self.crosstab_field, id
-                        ),
-                        "ref": magic_field_class,
-                        "id": id,
-                        "crosstab_field": self.crosstab_field,
-                        "is_remainder": counter == ids_length
-                        if self.crosstab_compute_remainder
-                        else False,
-                        "source": "magic_field" if magic_field_class else "",
-                        "is_summable": magic_field_class.is_summable,
-                    }
+                crosstab_column = {
+                    "name": f"{magic_field_class.name}CT{crosstab_id}",
+                    "original_name": magic_field_class.name,
+                    "verbose_name": self.get_crosstab_field_verbose_name(
+                        magic_field_class, self.crosstab_field, crosstab_id
+                    ),
+                    "ref": magic_field_class,
+                    "id": crosstab_id,
+                    "crosstab_field": self.crosstab_field,
+                    "is_remainder": counter == ids_length
+                    if self.crosstab_compute_remainder
+                    else False,
+                    "source": "magic_field" if magic_field_class else "",
+                    "is_summable": magic_field_class.is_summable,
+                    "computation_flag": "crosstab",  # a flag, todo find a better way probably
+                }
+                crosstab_column["queryset_filters"] = self._construct_crosstab_filter(
+                    crosstab_column, queryset_filters
                 )
 
+                output_cols.append(crosstab_column)
+
         return output_cols
 
     def get_crosstab_field_verbose_name(self, computation_class, model, id):
         """
         Hook to change the crosstab field verbose name, default it delegate this function to the ReportField
         :param computation_class: ReportField Class
         :param model: the model name as string
```

### Comparing `django-slick-reporting-0.9.0/slick_reporting/helpers.py` & `django-slick-reporting-1.0.0/slick_reporting/helpers.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/registry.py` & `django-slick-reporting-1.0.0/slick_reporting/registry.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js` & `django-slick-reporting-1.0.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js` & `django-slick-reporting-1.0.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/main.js` & `django-slick-reporting-1.0.0/slick_reporting/static/slick_reporting/main.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/js_resources.html` & `django-slick-reporting-1.0.0/slick_reporting/templates/slick_reporting/js_resources.html`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/simple_report.html` & `django-slick-reporting-1.0.0/slick_reporting/templates/slick_reporting/simple_report.html`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/templatetags/slick_reporting_tags.py` & `django-slick-reporting-1.0.0/slick_reporting/templatetags/slick_reporting_tags.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.9.0/slick_reporting/views.py` & `django-slick-reporting-1.0.0/slick_reporting/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,15 @@
         # sanity check, raises error if the columns or date fields is not set
         if cls.columns:
             cls.report_generator_class.check_columns(
                 cls.columns,
                 cls.group_by,
                 cls.get_report_model(),
                 container_class=cls,
+                group_by_custom_querysets=cls.group_by_custom_querysets,
             )
 
         super().__init_subclass__()
 
 
 class SlickReportingListViewMixin:
     report_generator_class = ListViewReportGenerator
```

