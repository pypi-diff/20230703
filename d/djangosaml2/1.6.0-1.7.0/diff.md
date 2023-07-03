# Comparing `tmp/djangosaml2-1.6.0.tar.gz` & `tmp/djangosaml2-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml2-1.6.0.tar", last modified: Mon Jun 19 17:02:21 2023, max compression
+gzip compressed data, was "djangosaml2-1.7.0.tar", last modified: Mon Jul  3 13:25:10 2023, max compression
```

## Comparing `djangosaml2-1.6.0.tar` & `djangosaml2-1.7.0.tar`

### file list

```diff
@@ -1,1590 +1,69 @@
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:01.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.808248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:02.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:04.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:32:55.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:01.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:32:55.000000 djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:10.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.812248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.792248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.816248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:12.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:13.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:06.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:11.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:06.000000 djangosaml2-1.6.0/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:20.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.820248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:21.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.824248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:23.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:16.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:20.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:16.000000 djangosaml2-1.6.0/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.828248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:31.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.832248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:33.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:25.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:30.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:25.000000 djangosaml2-1.6.0/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.7-django2.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.796248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:39.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.836248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:40.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:42.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:35.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:39.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:35.000000 djangosaml2-1.6.0/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.840247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.844247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:50.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:52.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:44.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:49.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:44.000000 djangosaml2-1.6.0/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:58.000000 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:54.000000 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:54.000000 djangosaml2-1.6.0/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    13512 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/CHANGES
--rw-rw-r--   0 wert      (1000) wert      (1000)    11358 2021-01-23 23:44:15.000000 djangosaml2-1.6.0/COPYING
--rw-rw-r--   0 wert      (1000) wert      (1000)      164 2021-01-23 23:44:15.000000 djangosaml2-1.6.0/MANIFEST.in
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)     1681 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/README.md
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      190 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/apps.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    14380 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/backends.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2894 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/cache.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2568 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)       51 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/exceptions.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     3586 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/djangosaml2/middleware.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1045 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/overrides.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      726 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/signals.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/templatetags/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/templatetags/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/templatetags/idplist.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)    43575 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/djangosaml2/tests/__init__.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/
--rw-rw-r--   0 wert      (1000) wert      (1000)      555 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/django_saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    11106 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     5095 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/auth_response.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     4177 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13780 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3565 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3557 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10380 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2466 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/spcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-16 13:28:16.000000 djangosaml2-1.6.0/djangosaml2/tests/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1190 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/urls.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     6333 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/djangosaml2/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    33758 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/djangosaml2/views.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.848247 djangosaml2-1.6.0/djangosaml2.egg-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)   111057 2023-06-19 17:02:21.000000 djangosaml2-1.6.0/djangosaml2.egg-info/SOURCES.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/dependency_links.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/not-zip-safe
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/requires.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)       12 2023-06-19 17:02:20.000000 djangosaml2-1.6.0/djangosaml2.egg-info/top_level.txt
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/docs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/docs/build/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/build/html/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/build/html/contents/
--rw-rw-r--   0 wert      (1000) wert      (1000)    12532 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/developer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     8498 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/faq.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    15228 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/miscellanea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    69252 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/contents/setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     8538 2023-06-19 16:49:08.000000 djangosaml2-1.6.0/docs/build/html/contents/usage.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6153 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/genindex.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    12704 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6552 2023-06-19 16:50:07.000000 djangosaml2-1.6.0/docs/build/html/search.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/docs/source/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.800248 djangosaml2-1.6.0/docs/source/_templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/source/_templates/pplnx_template/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1829 2021-04-04 22:43:59.000000 djangosaml2-1.6.0/docs/source/_templates/pplnx_template/footer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1488 2023-06-19 16:54:37.000000 djangosaml2-1.6.0/docs/source/_templates/pplnx_template/layout.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/source/html/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/docs/source/html/contents/
--rw-rw-r--   0 wert      (1000) wert      (1000)    12532 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/developer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     8498 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/faq.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    15228 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/miscellanea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    69252 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     8538 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/contents/usage.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6153 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/genindex.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    12704 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6552 2023-06-19 16:50:24.000000 djangosaml2-1.6.0/docs/source/html/search.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/htmlfiles/
--rw-rw-r--   0 wert      (1000) wert      (1000)     5400 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/htmlfiles/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6434 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/coverage/htmlfiles/pyfile.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1235 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1716 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2515 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6110 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      448 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3019 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3290 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1502 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      697 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/color_theme_toggle.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      453 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2539 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2241 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2580 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4086 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.852247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2200 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1849 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1899 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      486 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2136 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1257 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1093 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      339 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2096 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      745 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2428 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1366 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      869 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      196 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1587 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      360 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      865 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/div.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/
--rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/
--rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      119 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/div.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       88 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       85 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/ul.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      147 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/label.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      673 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      814 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      712 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.856247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      874 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/div.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      118 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/div.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       82 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       83 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/ul.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      122 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/label.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      684 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      825 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      723 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      426 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11184 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17662 2023-05-01 09:55:03.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)    26094 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/SOURCES.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/dependency_links.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      969 2023-05-01 09:54:30.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/docutils-0.19.dist-info/top_level.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/jeepney/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/jeepney/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     4575 2023-05-07 19:41:47.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:29.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2023-05-01 09:55:04.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.804248 djangosaml2-1.6.0/env/lib/python3.10/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/env/lib/python3.10/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2023-05-01 09:54:28.000000 djangosaml2-1.6.0/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      439 2023-04-05 16:19:28.000000 djangosaml2-1.6.0/pyproject.toml
--rw-rw-r--   0 wert      (1000) wert      (1000)      197 2023-06-19 17:02:21.860247 djangosaml2-1.6.0/setup.cfg
--rw-rw-r--   0 wert      (1000) wert      (1000)     2436 2023-06-19 16:48:07.000000 djangosaml2-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.960576 djangosaml2-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-03 13:25:10.960576 djangosaml2-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.956575 djangosaml2-1.7.0/djangosaml2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.952576 djangosaml2-1.7.0/djangosaml2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.956575 djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/login_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/wayf.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.956575 djangosaml2-1.7.0/djangosaml2/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/templatetags/idplist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.960576 djangosaml2-1.7.0/djangosaml2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    43575 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.960576 djangosaml2-1.7.0/djangosaml2/tests/attribute-maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/attribute-maps/django_saml_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/attribute-maps/saml_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/idpcert.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/idpcert.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/idpcert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/mycert.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/mycert.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/mycert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    13780 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/remote_metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/sp_metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/spcert.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/spcert.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/spcert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33783 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/djangosaml2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.956575 djangosaml2-1.7.0/djangosaml2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-03 13:25:10.000000 djangosaml2-1.7.0/djangosaml2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-03 13:25:10.000000 djangosaml2-1.7.0/djangosaml2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:25:10.000000 djangosaml2-1.7.0/djangosaml2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:25:10.000000 djangosaml2-1.7.0/djangosaml2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 13:25:10.000000 djangosaml2-1.7.0/djangosaml2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 13:25:10.000000 djangosaml2-1.7.0/djangosaml2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.952576 djangosaml2-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.952576 djangosaml2-1.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.952576 djangosaml2-1.7.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:25:10.960576 djangosaml2-1.7.0/docs/source/_templates/pplnx_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/docs/source/_templates/pplnx_template/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/docs/source/_templates/pplnx_template/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 13:25:10.960576 djangosaml2-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-03 13:25:00.000000 djangosaml2-1.7.0/setup.py
```

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.7.0/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.7.0/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.7.0/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.7.0/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.7.0/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.7.0/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.7.0/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata.xml`

 * *Files 1% similar despite different names*

#### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata.xml`

```diff
@@ -23,15 +23,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp1.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -53,15 +53,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp1.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp1.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp2.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -83,15 +83,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp2.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp2.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp3.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -113,11 +113,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp3.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp3.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files 2% similar despite different names*

#### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_one_idp.xml`

```diff
@@ -23,11 +23,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files 3% similar despite different names*

#### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_post_binding.xml`

```diff
@@ -23,11 +23,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files 2% similar despite different names*

#### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.7.0/djangosaml2/tests/remote_metadata_three_idps.xml`

```diff
@@ -23,15 +23,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp1.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp1.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp2.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -53,15 +53,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp2.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp2.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp3.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -83,11 +83,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp3.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp3.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.7.0/djangosaml2/tests/sp_metadata.xml`

 * *Files 5% similar despite different names*

#### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.7.0/djangosaml2/tests/sp_metadata.xml`

```diff
@@ -31,11 +31,11 @@
     <md:Organization>
       <md:OrganizationURL xml:lang="en">http://sp.example.com/</md:OrganizationURL>
       <md:OrganizationName xml:lang="en">Lorenzo's test SP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">sp.example.com</md:OrganizationDisplayName>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.7.0/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.7.0/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.7.0/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/CHANGES` & `djangosaml2-1.7.0/CHANGES`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/COPYING` & `djangosaml2-1.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/PKG-INFO` & `djangosaml2-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.6.0
+Version: 1.7.0
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.6.0/README.md` & `djangosaml2-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/backends.py` & `djangosaml2-1.7.0/djangosaml2/backends.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/cache.py` & `djangosaml2-1.7.0/djangosaml2/cache.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/conf.py` & `djangosaml2-1.7.0/djangosaml2/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/middleware.py` & `djangosaml2-1.7.0/djangosaml2/middleware.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/overrides.py` & `djangosaml2-1.7.0/djangosaml2/overrides.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/signals.py` & `djangosaml2-1.7.0/djangosaml2/signals.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/templatetags/idplist.py` & `djangosaml2-1.7.0/djangosaml2/templatetags/idplist.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/tests/__init__.py` & `djangosaml2-1.7.0/djangosaml2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/django_saml_uri.py` & `djangosaml2-1.7.0/djangosaml2/tests/attribute-maps/django_saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/tests/attribute-maps/saml_uri.py` & `djangosaml2-1.7.0/djangosaml2/tests/attribute-maps/saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/tests/auth_response.py` & `djangosaml2-1.7.0/djangosaml2/tests/auth_response.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/tests/conf.py` & `djangosaml2-1.7.0/djangosaml2/tests/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/urls.py` & `djangosaml2-1.7.0/djangosaml2/urls.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/utils.py` & `djangosaml2-1.7.0/djangosaml2/utils.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/djangosaml2/views.py` & `djangosaml2-1.7.0/djangosaml2/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import base64
 import logging
+from typing import Optional
 from urllib.parse import quote
 
 from django.conf import settings
 from django.core.exceptions import PermissionDenied, SuspiciousOperation
 from django.http import (
     HttpRequest,
     HttpResponse,
@@ -85,14 +86,26 @@
 def _get_subject_id(session):
     try:
         return decode(session["_saml2_subject_id"])
     except KeyError:
         return None
 
 
+def _get_next_path(request: HttpRequest) -> Optional[str]:
+    if "next" in request.GET:
+        next_path = request.GET["next"]
+    elif "RelayState" in request.GET:
+        next_path = request.GET["RelayState"]
+    else:
+        return None
+
+    next_path = validate_referral_url(request, next_path)
+    return next_path
+
+
 class SPConfigMixin:
     """Mixin for some of the SAML views with re-usable methods."""
 
     config_loader_path = None
 
     def get_config_loader_path(self, request: HttpRequest):
         return self.config_loader_path
@@ -134,28 +147,14 @@
     )
     post_binding_form_template = getattr(
         settings,
         "SAML2_CUSTOM_POST_BINDING_FORM_TEMPLATE",
         "djangosaml2/post_binding_form.html",
     )
 
-    def get_next_path(self, request: HttpRequest) -> str:
-        """Returns the path to put in the RelayState to redirect the user to after having logged in.
-        If the user is already logged in (and if allowed), he will redirect to there immediately.
-        """
-
-        next_path = get_fallback_login_redirect_url()
-        if "next" in request.GET:
-            next_path = request.GET["next"]
-        elif "RelayState" in request.GET:
-            next_path = request.GET["RelayState"]
-
-        next_path = validate_referral_url(request, next_path)
-        return next_path
-
     def unknown_idp(self, request, idp):
         msg = f"Error: IdP EntityID {escape(idp)} was not found in metadata"
         logger.error(msg)
         return HttpResponse(msg, status=403)
 
     def load_sso_kwargs_scoping(self, sso_kwargs):
         """Performs IdP Scoping if scoping param is present."""
@@ -181,15 +180,17 @@
         # B) He comes from a view that (incorrectly) send him here because
         #    he does not have enough permissions. That view should have shown
         #    an authorization error in the first place.
         return request.user.is_authenticated
 
     def get(self, request, *args, **kwargs):
         logger.debug("Login process started")
-        next_path = self.get_next_path(request)
+        next_path = _get_next_path(request)
+        if next_path is None:
+            next_path = get_fallback_login_redirect_url()
 
         if self.should_prevent_auth(request):
             # If the SAML_IGNORE_AUTHENTICATED_USERS_ON_LOGIN setting is True
             # (default value), redirect to the next_path. Otherwise, show a
             # configurable authorization error.
             if get_custom_setting("SAML_IGNORE_AUTHENTICATED_USERS_ON_LOGIN", True):
                 return HttpResponseRedirect(next_path)
@@ -818,16 +819,20 @@
     if getattr(settings, "SAML_IGNORE_LOGOUT_ERRORS", False) or (
         response and response.status_ok()
     ):
         logger.debug("Performing django logout.")
 
         auth.logout(request)
 
-        if settings.LOGOUT_REDIRECT_URL is not None:
-            return HttpResponseRedirect(resolve_url(settings.LOGOUT_REDIRECT_URL))
+        next_path = _get_next_path(request)
+        if next_path is not None:
+            return HttpResponseRedirect(next_path)
+        elif settings.LOGOUT_REDIRECT_URL is not None:
+            fallback_url = resolve_url(settings.LOGOUT_REDIRECT_URL)
+            return HttpResponseRedirect(fallback_url)
         else:
             current_site = get_current_site(request)
             return render(
                 request,
                 "registration/logged_out.html",
                 {
                     "site": current_site,
```

### Comparing `djangosaml2-1.6.0/djangosaml2.egg-info/PKG-INFO` & `djangosaml2-1.7.0/djangosaml2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.6.0
+Version: 1.7.0
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.6.0/docs/source/_templates/pplnx_template/footer.html` & `djangosaml2-1.7.0/docs/source/_templates/pplnx_template/footer.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/docs/source/_templates/pplnx_template/layout.html` & `djangosaml2-1.7.0/docs/source/_templates/pplnx_template/layout.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.6.0/setup.py` & `djangosaml2-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return codecs.open(
         os.path.join(os.path.dirname(__file__), *rnames), encoding="utf-8"
     ).read()
 
 
 setup(
     name="djangosaml2",
-    version="1.6.0",
+    version="1.7.0",
     description="pysaml2 integration for Django",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
```

