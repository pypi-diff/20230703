# Comparing `tmp/crispy-bulma-0.8.3.tar.gz` & `tmp/crispy-bulma-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispy-bulma-0.8.3.tar", last modified: Tue Jan 31 10:23:52 2023, max compression
+gzip compressed data, was "crispy-bulma-0.9.0.tar", last modified: Sun Mar  5 18:54:40 2023, max compression
```

## Comparing `crispy-bulma-0.8.3.tar` & `crispy-bulma-0.9.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.977818 crispy-bulma-0.8.3/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3706 2022-05-19 19:07:40.000000 crispy-bulma-0.8.3/CONTRIBUTING.rst
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3296 2023-01-31 10:22:57.000000 crispy-bulma-0.8.3/HISTORY.rst
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1159 2022-04-05 21:56:48.000000 crispy-bulma-0.8.3/LICENSE
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      202 2022-04-08 19:46:57.000000 crispy-bulma-0.8.3/MANIFEST.in
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     9944 2023-01-31 10:23:52.977818 crispy-bulma-0.8.3/PKG-INFO
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3227 2023-01-29 21:00:49.000000 crispy-bulma-0.8.3/README.rst
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.969817 crispy-bulma-0.8.3/crispy_bulma/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      133 2023-01-31 10:23:11.000000 crispy-bulma-0.8.3/crispy_bulma/__init__.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     2885 2022-04-28 10:15:19.000000 crispy-bulma-0.8.3/crispy_bulma/bulma.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      296 2022-04-12 16:39:04.000000 crispy-bulma-0.8.3/crispy_bulma/forms.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     8956 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/crispy_bulma/layout.py
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.969817 crispy-bulma-0.8.3/crispy_bulma/templates/
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.973817 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      253 2021-05-22 12:38:25.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/display_form.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      325 2021-05-22 12:38:25.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/errors.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     2128 2022-12-29 21:22:43.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/field.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      181 2022-05-19 19:07:40.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/inputs.html
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.973817 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1083 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/baseinput.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      727 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/button.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      426 2022-04-15 18:44:39.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/checkboxinput.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      662 2022-05-19 19:07:40.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/checkboxselectmultiple.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      750 2022-04-16 18:53:31.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/checkboxselectmultiple_inline.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      168 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/div.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      236 2021-05-22 12:38:25.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/field_errors.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      230 2021-05-22 12:38:25.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/field_errors_block.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      356 2022-12-29 21:32:28.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/formgroup.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      116 2022-04-12 17:34:33.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/help_text.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      659 2022-12-14 22:57:28.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/input_with_icon.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      585 2022-05-19 19:07:40.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/radioselect.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      671 2022-05-19 19:07:40.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/radioselect_inline.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      222 2023-01-31 10:22:57.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/select.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      304 2022-04-16 21:03:09.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/uni_form.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      455 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/whole_uni_form.html
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.973817 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/widgets/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1121 2023-01-22 20:11:25.000000 crispy-bulma-0.8.3/crispy_bulma/templates/bulma/widgets/file_upload_input.html
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.973817 crispy-bulma-0.8.3/crispy_bulma/templatetags/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        0 2022-04-14 08:47:04.000000 crispy-bulma-0.8.3/crispy_bulma/templatetags/__init__.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     5409 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/crispy_bulma/templatetags/crispy_forms_bulma_field.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      148 2022-12-29 19:37:34.000000 crispy-bulma-0.8.3/crispy_bulma/widgets.py
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.969817 crispy-bulma-0.8.3/crispy_bulma.egg-info/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     9944 2023-01-31 10:23:52.000000 crispy-bulma-0.8.3/crispy_bulma.egg-info/PKG-INFO
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3512 2023-01-31 10:23:52.000000 crispy-bulma-0.8.3/crispy_bulma.egg-info/SOURCES.txt
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        1 2023-01-31 10:23:52.000000 crispy-bulma-0.8.3/crispy_bulma.egg-info/dependency_links.txt
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        1 2023-01-31 10:23:52.000000 crispy-bulma-0.8.3/crispy_bulma.egg-info/not-zip-safe
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       69 2023-01-31 10:23:52.000000 crispy-bulma-0.8.3/crispy_bulma.egg-info/requires.txt
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       13 2023-01-31 10:23:52.000000 crispy-bulma-0.8.3/crispy_bulma.egg-info/top_level.txt
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      843 2023-01-31 10:23:52.977818 crispy-bulma-0.8.3/setup.cfg
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     2030 2023-01-31 10:23:11.000000 crispy-bulma-0.8.3/setup.py
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.973817 crispy-bulma-0.8.3/tests/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        0 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/__init__.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     7860 2022-12-14 23:53:01.000000 crispy-bulma-0.8.3/tests/forms.py
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.977818 crispy-bulma-0.8.3/tests/results/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      263 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/alert.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      525 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/results/field_with_buttons.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      587 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/results/field_with_buttons_failing.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       44 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/flat_attrs.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      331 2022-04-12 17:34:33.000000 crispy-bulma-0.8.3/tests/results/help_text_escape.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1244 2022-05-10 14:13:23.000000 crispy-bulma-0.8.3/tests/results/row.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      943 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/results/test_bootstrap5_form_inline.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      183 2022-04-28 09:16:38.000000 crispy-bulma-0.8.3/tests/results/test_button.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      351 2022-04-28 10:15:19.000000 crispy-bulma-0.8.3/tests/results/test_button_horizontal.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      263 2022-04-12 17:34:33.000000 crispy-bulma-0.8.3/tests/results/test_checkbox.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      827 2022-04-14 09:51:15.000000 crispy-bulma-0.8.3/tests/results/test_checkboxes.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1158 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_clearable_file_field.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      673 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_clearable_file_field_failing.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      339 2022-04-12 15:53:00.000000 crispy-bulma-0.8.3/tests/results/test_email_field.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      459 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_file_field.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      649 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_file_field_failing.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      971 2022-12-29 21:32:28.000000 crispy-bulma-0.8.3/tests/results/test_form_group.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1348 2022-12-29 21:32:28.000000 crispy-bulma-0.8.3/tests/results/test_form_group_horizontal.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      498 2022-04-12 21:35:00.000000 crispy-bulma-0.8.3/tests/results/test_form_horizontal.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1768 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_grouped_checkboxes.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1990 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_grouped_checkboxes_failing.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1379 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_grouped_radios.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     2034 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/results/test_grouped_radios_failing.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      157 2022-04-28 09:16:38.000000 crispy-bulma-0.8.3/tests/results/test_hidden.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      847 2022-04-16 18:53:31.000000 crispy-bulma-0.8.3/tests/results/test_inline_checkboxes.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      697 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/results/test_inline_field.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      910 2022-04-16 18:53:31.000000 crispy-bulma-0.8.3/tests/results/test_inline_radios.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      589 2022-12-14 23:00:56.000000 crispy-bulma-0.8.3/tests/results/test_input_with_icon.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1926 2022-11-08 18:33:34.000000 crispy-bulma-0.8.3/tests/results/test_prepended_appended_select.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1547 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/results/test_prepended_appended_text.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      878 2022-04-14 09:51:29.000000 crispy-bulma-0.8.3/tests/results/test_radio.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      214 2022-04-28 09:16:38.000000 crispy-bulma-0.8.3/tests/results/test_reset.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      495 2022-04-14 09:51:20.000000 crispy-bulma-0.8.3/tests/results/test_select.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      695 2022-04-14 10:02:42.000000 crispy-bulma-0.8.3/tests/results/test_selectmultiple.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      219 2022-04-28 09:16:38.000000 crispy-bulma-0.8.3/tests/results/test_submit.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      365 2022-04-28 10:15:19.000000 crispy-bulma-0.8.3/tests/results/test_submit_horizontal.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     8457 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/results/test_tabular_formset_layout.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     6966 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/results/test_tabular_formset_layout_failing.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      388 2022-04-12 17:34:33.000000 crispy-bulma-0.8.3/tests/results/test_text_area.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      313 2022-04-12 17:34:33.000000 crispy-bulma-0.8.3/tests/results/test_text_input.html
-drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-01-31 10:23:52.977818 crispy-bulma-0.8.3/tests/templates/
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       48 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/templates/crispy_render_template.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       63 2022-04-16 21:03:09.000000 crispy-bulma-0.8.3/tests/templates/custom_field_template.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       75 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/templates/custom_form_template.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      152 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/templates/custom_form_template_with_context.html
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)    19959 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/test_form_helper.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)    17262 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/test_layout.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)    13206 2023-01-29 17:10:32.000000 crispy-bulma-0.8.3/tests/test_layout_objects.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1569 2022-04-07 18:49:49.000000 crispy-bulma-0.8.3/tests/test_settings.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     6266 2023-01-29 20:04:20.000000 crispy-bulma-0.8.3/tests/test_tags.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      151 2022-04-04 14:34:21.000000 crispy-bulma-0.8.3/tests/urls.py
--rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1358 2022-11-08 18:33:34.000000 crispy-bulma-0.8.3/tests/utils.py
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.763406 crispy-bulma-0.9.0/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3706 2022-05-19 19:07:40.000000 crispy-bulma-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3474 2023-03-05 18:36:03.000000 crispy-bulma-0.9.0/HISTORY.rst
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1159 2022-04-05 21:56:48.000000 crispy-bulma-0.9.0/LICENSE
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      202 2022-04-08 19:46:57.000000 crispy-bulma-0.9.0/MANIFEST.in
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     7986 2023-03-05 18:54:40.763406 crispy-bulma-0.9.0/PKG-INFO
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3059 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/README.rst
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.759406 crispy-bulma-0.9.0/crispy_bulma/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      133 2023-03-05 18:53:35.000000 crispy-bulma-0.9.0/crispy_bulma/__init__.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     2885 2022-04-28 10:15:19.000000 crispy-bulma-0.9.0/crispy_bulma/bulma.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      296 2022-04-12 16:39:04.000000 crispy-bulma-0.9.0/crispy_bulma/forms.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     8768 2023-03-05 18:31:24.000000 crispy-bulma-0.9.0/crispy_bulma/layout.py
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.755406 crispy-bulma-0.9.0/crispy_bulma/templates/
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.759406 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      253 2021-05-22 12:38:25.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/display_form.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      325 2021-05-22 12:38:25.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/errors.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     2128 2022-12-29 21:22:43.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/field.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      181 2022-05-19 19:07:40.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/inputs.html
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.759406 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      990 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/baseinput.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      722 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/button.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      426 2022-04-15 18:44:39.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/checkboxinput.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      662 2022-05-19 19:07:40.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/checkboxselectmultiple.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      750 2022-04-16 18:53:31.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/checkboxselectmultiple_inline.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      158 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/div.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      236 2021-05-22 12:38:25.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/field_errors.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      230 2021-05-22 12:38:25.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/field_errors_block.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      351 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/formgroup.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      116 2022-04-12 17:34:33.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/help_text.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      659 2022-12-14 22:57:28.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/input_with_icon.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      585 2022-05-19 19:07:40.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/radioselect.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      671 2022-05-19 19:07:40.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/radioselect_inline.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      222 2023-03-05 11:45:00.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/select.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      304 2022-04-16 21:03:09.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/uni_form.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      450 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/whole_uni_form.html
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.759406 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/widgets/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1121 2023-01-22 20:11:25.000000 crispy-bulma-0.9.0/crispy_bulma/templates/bulma/widgets/file_upload_input.html
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.759406 crispy-bulma-0.9.0/crispy_bulma/templatetags/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        0 2022-04-14 08:47:04.000000 crispy-bulma-0.9.0/crispy_bulma/templatetags/__init__.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     5409 2023-03-05 17:54:35.000000 crispy-bulma-0.9.0/crispy_bulma/templatetags/crispy_forms_bulma_field.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      148 2022-12-29 19:37:34.000000 crispy-bulma-0.9.0/crispy_bulma/widgets.py
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.759406 crispy-bulma-0.9.0/crispy_bulma.egg-info/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     7986 2023-03-05 18:54:40.000000 crispy-bulma-0.9.0/crispy_bulma.egg-info/PKG-INFO
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     3527 2023-03-05 18:54:40.000000 crispy-bulma-0.9.0/crispy_bulma.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        1 2023-03-05 18:54:40.000000 crispy-bulma-0.9.0/crispy_bulma.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        1 2023-03-05 18:54:40.000000 crispy-bulma-0.9.0/crispy_bulma.egg-info/not-zip-safe
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       66 2023-03-05 18:54:40.000000 crispy-bulma-0.9.0/crispy_bulma.egg-info/requires.txt
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       13 2023-03-05 18:54:40.000000 crispy-bulma-0.9.0/crispy_bulma.egg-info/top_level.txt
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      380 2023-03-05 18:52:30.000000 crispy-bulma-0.9.0/pyproject.toml
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      517 2023-03-05 18:54:40.763406 crispy-bulma-0.9.0/setup.cfg
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1989 2023-03-05 18:53:35.000000 crispy-bulma-0.9.0/setup.py
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.759406 crispy-bulma-0.9.0/tests/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)        0 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/__init__.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     7860 2023-03-05 18:31:24.000000 crispy-bulma-0.9.0/tests/forms.py
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.763406 crispy-bulma-0.9.0/tests/results/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      263 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/alert.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      506 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/results/field_with_buttons.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      568 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/results/field_with_buttons_failing.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       44 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/flat_attrs.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      331 2022-04-12 17:34:33.000000 crispy-bulma-0.9.0/tests/results/help_text_escape.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1244 2022-05-10 14:13:23.000000 crispy-bulma-0.9.0/tests/results/row.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      883 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/results/test_bootstrap5_form_inline.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      183 2022-04-28 09:16:38.000000 crispy-bulma-0.9.0/tests/results/test_button.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      351 2022-04-28 10:15:19.000000 crispy-bulma-0.9.0/tests/results/test_button_horizontal.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      263 2022-04-12 17:34:33.000000 crispy-bulma-0.9.0/tests/results/test_checkbox.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      827 2022-04-14 09:51:15.000000 crispy-bulma-0.9.0/tests/results/test_checkboxes.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1158 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_clearable_file_field.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      673 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_clearable_file_field_failing.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      339 2022-04-12 15:53:00.000000 crispy-bulma-0.9.0/tests/results/test_email_field.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      459 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_file_field.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      649 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_file_field_failing.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      971 2022-12-29 21:32:28.000000 crispy-bulma-0.9.0/tests/results/test_form_group.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1348 2022-12-29 21:32:28.000000 crispy-bulma-0.9.0/tests/results/test_form_group_horizontal.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      498 2022-04-12 21:35:00.000000 crispy-bulma-0.9.0/tests/results/test_form_horizontal.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1768 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_grouped_checkboxes.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1990 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_grouped_checkboxes_failing.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1379 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_grouped_radios.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     2034 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/results/test_grouped_radios_failing.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      157 2022-04-28 09:16:38.000000 crispy-bulma-0.9.0/tests/results/test_hidden.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      847 2022-04-16 18:53:31.000000 crispy-bulma-0.9.0/tests/results/test_inline_checkboxes.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      678 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/results/test_inline_field.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      910 2022-04-16 18:53:31.000000 crispy-bulma-0.9.0/tests/results/test_inline_radios.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      589 2022-12-14 23:00:56.000000 crispy-bulma-0.9.0/tests/results/test_input_with_icon.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1926 2022-11-08 18:33:34.000000 crispy-bulma-0.9.0/tests/results/test_prepended_appended_select.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1488 2023-03-05 18:23:21.000000 crispy-bulma-0.9.0/tests/results/test_prepended_appended_text.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      878 2022-04-14 09:51:29.000000 crispy-bulma-0.9.0/tests/results/test_radio.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      214 2022-04-28 09:16:38.000000 crispy-bulma-0.9.0/tests/results/test_reset.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      495 2022-04-14 09:51:20.000000 crispy-bulma-0.9.0/tests/results/test_select.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      695 2022-04-14 10:02:42.000000 crispy-bulma-0.9.0/tests/results/test_selectmultiple.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      219 2022-04-28 09:16:38.000000 crispy-bulma-0.9.0/tests/results/test_submit.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      365 2022-04-28 10:15:19.000000 crispy-bulma-0.9.0/tests/results/test_submit_horizontal.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     8058 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/results/test_tabular_formset_layout.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     6767 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/results/test_tabular_formset_layout_failing.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      388 2022-04-12 17:34:33.000000 crispy-bulma-0.9.0/tests/results/test_text_area.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      313 2022-04-12 17:34:33.000000 crispy-bulma-0.9.0/tests/results/test_text_input.html
+drwxrwxr-x   0 ckrybu    (1000) ckrybu    (1000)        0 2023-03-05 18:54:40.763406 crispy-bulma-0.9.0/tests/templates/
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       48 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/templates/crispy_render_template.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       63 2022-04-16 21:03:09.000000 crispy-bulma-0.9.0/tests/templates/custom_field_template.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)       71 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/templates/custom_form_template.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      148 2023-03-05 18:18:20.000000 crispy-bulma-0.9.0/tests/templates/custom_form_template_with_context.html
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)    19317 2023-03-05 18:31:24.000000 crispy-bulma-0.9.0/tests/test_form_helper.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)    17262 2023-03-05 18:31:24.000000 crispy-bulma-0.9.0/tests/test_layout.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)    13206 2023-03-05 18:31:24.000000 crispy-bulma-0.9.0/tests/test_layout_objects.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1569 2022-04-07 18:49:49.000000 crispy-bulma-0.9.0/tests/test_settings.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     6140 2023-03-05 18:31:24.000000 crispy-bulma-0.9.0/tests/test_tags.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)      151 2022-04-04 14:34:21.000000 crispy-bulma-0.9.0/tests/urls.py
+-rw-rw-r--   0 ckrybu    (1000) ckrybu    (1000)     1358 2023-03-05 18:31:24.000000 crispy-bulma-0.9.0/tests/utils.py
```

### Comparing `crispy-bulma-0.8.3/CONTRIBUTING.rst` & `crispy-bulma-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/HISTORY.rst` & `crispy-bulma-0.9.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 =======
 History
 =======
 
 
+0.9.0 (2023-03-05)
+------------------
+
+* Drop support for django-crispy-forms 1.12.0, 1.13.0 and 1.14.0
+* Add support for django-crispy-forms 2.0
+* Drop support for Django 2.2
+
+
 0.8.3 (2023-01-31)
 ------------------
 
 * Fix Select widget error state rendering (the red border was missing).
 
 
 0.8.2 (2023-01-29)
```

### Comparing `crispy-bulma-0.8.3/LICENSE` & `crispy-bulma-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/README.rst` & `crispy-bulma-0.9.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -26,25 +26,22 @@
 
 
 Requirements
 ------------
 
 Officially supported versions:
 
-* Django: 2.2, 3.2, 4.0, 4.1
+* Django: 3.2, 4.0, 4.1
 * Python 3.7, 3.8, 3.9, 3.10, 3.11
-* django-crispy-forms 1.12, 1.13, 1.14
+* django-crispy-forms 2.0
 * Bulma.css 0.9.4
 
-**Note: Django 4.0+ requires version 0.6.0+ and django-crispy-forms version 1.13+.**
+**Django 4.0+ requires crispy-bulma version 0.6.0+ and django-crispy-forms version 1.13+.**
 
-Older versions might work, but are not officially supported.
-For example django-crispy-forms >= 1.9.0, Bulma >= 0.7.5 and Django 3.0/3.1 are still likely to work.
-
-If you depend on django-crispy-forms < 1.12.0 use the 0.4.0 version.
+**For django-crispy-forms versions older than 2.0 use crispy-bulma<=0.8.3**
 
 
 Quickstart
 ----------
 
 Install this plugin using `pip`::
```

### Comparing `crispy-bulma-0.8.3/crispy_bulma/bulma.py` & `crispy-bulma-0.9.0/crispy_bulma/bulma.py`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/layout.py` & `crispy-bulma-0.9.0/crispy_bulma/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,25 +51,23 @@
 
 
 class BulmaBaseInput(BaseInput):
     def __init__(self, *args, **kwargs):
         self.control_class = kwargs.pop("control_class", None)
         super().__init__(*args, **kwargs)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK, **kwargs):
+    def render(self, form, context, template_pack=TEMPLATE_PACK, **kwargs):
         """
         Renders an `<input />` if container is used as a Layout object.
         Input button value can be a variable in context.
 
         """
         if self.control_class:
             context["control_class"] = self.control_class
-        return super().render(
-            form, form_style, context, template_pack=template_pack, **kwargs
-        )
+        return super().render(form, context, template_pack=template_pack, **kwargs)
 
 
 class Submit(BulmaBaseInput):
     """
     Used to create a Submit button descriptor for the {% crispy %} template tag.
     >>> submit = Submit("Search the Site", "search this site")
 
@@ -100,15 +98,15 @@
             kwargs["id"] = kwargs.pop("css_id")
         kwargs["class"] = self.field_classes
         if "css_class" in kwargs:
             kwargs["class"] += " %s" % kwargs.pop("css_class")
 
         self.flat_attrs = flatatt(kwargs)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK, **kwargs):
+    def render(self, form, context, template_pack=TEMPLATE_PACK, **kwargs):
         self.content = Template(str(self.content)).render(context)
         template = self.get_template_name(template_pack)
 
         extra_context = {"button": self}
         if self.control_class:
             extra_context["control_class"] = self.control_class
 
@@ -198,35 +196,28 @@
     def __init__(self, field, icon_prepend=None, icon_append=None, *args, **kwargs):
         self.field = field
         self.icon_prepend = icon_prepend
         self.icon_append = icon_append
         super().__init__(*args, **kwargs)
 
     def render(
-        self,
-        form,
-        form_style,
-        context,
-        template_pack=TEMPLATE_PACK,
-        extra_context=None,
-        **kwargs
+        self, form, context, template_pack=TEMPLATE_PACK, extra_context=None, **kwargs
     ):
         extra_context = extra_context.copy() if extra_context is not None else {}
         extra_context.update(
             {
                 "icon_prepend": self.icon_prepend,
                 "icon_append": self.icon_append,
             }
         )
         template = self.get_template_name(template_pack)
 
         return render_field(
             self.field,
             form,
-            form_style,
             context,
             template=template,
             template_pack=template_pack,
             extra_context=extra_context,
             attrs=self.attrs,
             **kwargs
         )
@@ -270,20 +261,18 @@
     def __init__(self, *fields, css_id=None, css_class=None, template=None, **kwargs):
         self.fields = list(fields)
         self.id = css_id
         self.css_class = css_class
         self.template = template or self.template
         self.flat_attrs = flatatt(kwargs)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK, **kwargs):
+    def render(self, form, context, template_pack=TEMPLATE_PACK, **kwargs):
         # TODO use extra_context
         # There seem to be a bug in crispy_forms, the `extra_context` kwarg is not being
         # passed on to `field.render` in `render_field` which is called by `get_rendered_fields`.
         # Right now `exclude_field_wrapper` is being passed on also to `formgroup.html`,
         # but it does not break anything.
         context["exclude_field_wrapper"] = True
-        html = self.get_rendered_fields(
-            form, form_style, context, template_pack, **kwargs
-        )
+        html = self.get_rendered_fields(form, context, template_pack, **kwargs)
         template = self.get_template_name(template_pack)
         context.update({"formgroup": self, "fields_output": html})
         return render_to_string(template, context.flatten())
```

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/field.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/field.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/baseinput.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/baseinput.html`

 * *Files 26% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 <div class="control{% if control_class %} {{ control_class }}{% endif %}">
   <input type="{{ input.input_type }}"
     name="{% if input.name|wordcount > 1 %}{{ input.name|slugify }}{% else %}{{ input.name }}{% endif %}"
     value="{{ input.value }}"
     {% if input.input_type != "hidden" %}
         class="{{ input.field_classes }}"
-        id="{% if input.id %}{{ input.id }}{% else %}{{ input.input_type }}-id-{{ input.name|slugify }}{% endif %}"
+        id="{{ input.id }}"
     {% endif %}
-    {{ input.flat_attrs|safe }}
+    {{ input.flat_attrs }}
     />
 </div>
 
 {% if not exclude_field_wrapper %}
 {% if form_horizontal %}
   </div>
 </div>
```

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/button.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/button.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 </div>
 <div class="field-body">
   <div class="field">
 {% endif %}
 {% endif %}
 
 <div class="control{% if control_class %} {{ control_class }}{% endif %}">
-  <button {{ button.flat_attrs|safe }}>{{ button.content|safe }}</button>
+  <button {{ button.flat_attrs }}>{{ button.content|safe }}</button>
 </div>
 
 {% if not exclude_field_wrapper %}
 {% if form_horizontal %}
   </div>
 </div>
 {% endif %}
```

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/checkboxselectmultiple.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/checkboxselectmultiple.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/checkboxselectmultiple_inline.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/checkboxselectmultiple_inline.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/input_with_icon.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/input_with_icon.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/radioselect.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/radioselect.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/layout/radioselect_inline.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/layout/radioselect_inline.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templates/bulma/widgets/file_upload_input.html` & `crispy-bulma-0.9.0/crispy_bulma/templates/bulma/widgets/file_upload_input.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma/templatetags/crispy_forms_bulma_field.py` & `crispy-bulma-0.9.0/crispy_bulma/templatetags/crispy_forms_bulma_field.py`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/crispy_bulma.egg-info/SOURCES.txt` & `crispy-bulma-0.9.0/crispy_bulma.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 crispy_bulma/__init__.py
 crispy_bulma/bulma.py
 crispy_bulma/forms.py
 crispy_bulma/layout.py
 crispy_bulma/widgets.py
```

### Comparing `crispy-bulma-0.8.3/setup.cfg` & `crispy-bulma-0.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,16 @@
 [bumpversion]
-current_version = 0.8.3
+current_version = 0.9.0
 commit = True
 tag = True
 
 [metadata]
 license_file = LICENSE
 description_file = README.rst
 
-[isort]
-profile = black
-default_section = THIRDPARTY
-known_django = django
-known_first_party = crispy_bulma,crispy_forms
-sections = FUTURE,STDLIB,THIRDPARTY,DJANGO,FIRSTPARTY,LOCALFOLDER
-skip = .tox,docs
-
-[tool:pytest]
-django_settings_module = tests.test_settings
-norecursedirs = .git .tox docs
-collect_ignore = ["setup.py"]
-
 [flake8]
 exclude = .tox,docs
 max-line-length = 119
 statistics = True
 count = True
 select = C,E,F,W,B
 ignore = E203, W503
```

### Comparing `crispy-bulma-0.8.3/setup.py` & `crispy-bulma-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,39 +7,38 @@
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 
 setup(
     name="crispy-bulma",
-    version="0.8.3",
+    version="0.9.0",
     description="Bulma template pack for django-crispy-forms",
     long_description=readme + "\n\n" + history,
     author="Christoph Krybus",
     author_email="chris@ckrybus.com",
     keywords=["forms", "django", "crispy", "bulma"],
     url="https://github.com/ckrybus/crispy-bulma",
     license="MIT",
     packages=["crispy_bulma"],
-    install_requires=["Django>=2.2", "django-crispy-forms>=1.12.0"],
+    install_requires=["Django>=3.2", "django-crispy-forms>=2.0"],
     extras_require={"test": ["pytest", "pytest-django"]},
     tests_require=["crispy-bulma[test]"],
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://crispy-bulma.readthedocs.io/en/latest/",
         "Source": "https://github.com/ckrybus/crispy-bulma",
         "Changelog": "https://github.com/ckrybus/crispy-bulma/blob/main/HISTORY.rst",
     },
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `crispy-bulma-0.8.3/tests/forms.py` & `crispy-bulma-0.9.0/tests/forms.py`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/field_with_buttons.html` & `crispy-bulma-0.9.0/tests/results/field_with_buttons_failing.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <form method="post">
 	<div class=" col-md">
-		<div class="mb-3"><label class=" form-label requiredField" for="id_email">email<span
+		<div class="mb-3"><label class=" form-label requiredField" for="id_email">Email<span
 					class="asteriskField">*</span></label>
 			<div>
-				<div class="input-group"><input class="form-control inputtext textInput textinput" id="id_email"
-						maxlength="30" name="email" required type="text"><a class="btn btn-primary"
-						role="button">click me</a></div>
-				<small class="form-text text-muted" id="hint_id_email">Insert your email</small>
+				<div class="input-group"><input class="form-control inputtext is-invalid"
+						id="id_email" maxlength="20" name="email" required type="text"><button
+						class="btn btn-outline-secondary" type="button">Go!</button></div>
+				<p class="mb-0 text-danger" id="error_1_id_email"><small><strong>This field is
+							required.</strong></small></p>
 			</div>
 		</div>
 	</div>
-</form>
+</form>
```

### Comparing `crispy-bulma-0.8.3/tests/results/row.html` & `crispy-bulma-0.9.0/tests/results/row.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_bootstrap5_form_inline.html` & `crispy-bulma-0.9.0/tests/results/test_bootstrap5_form_inline.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <form class="row row-cols-lg-auto" method="post">
     <div id="div_id_email">
         <label class="visually-hidden" for="id_email">
             email
-        </label><input class="form-control inputtext textInput textinput" id="id_email" maxlength="30" name="email"
+        </label><input class="form-control inputtext" id="id_email" maxlength="30" name="email"
             placeholder="email" required type="text">
     </div>
     <div id="div_id_password1">
         <label class="visually-hidden" for="id_password1">
             password
-        </label><input class="form-control textInput textinput" id="id_password1" maxlength="30" name="password1"
+        </label><input class="form-control" id="id_password1" maxlength="30" name="password1"
             placeholder="password" required type="password">
     </div>
     <div id="div_id_last_name">
         <label class="visually-hidden" for="id_last_name">
             last name
-        </label><input class="form-control inputtext textInput textinput" id="id_last_name" maxlength="5"
+        </label><input class="form-control inputtext" id="id_last_name" maxlength="5"
             name="last_name" placeholder="last name" required type="text">
     </div>
 </form>
```

### Comparing `crispy-bulma-0.8.3/tests/results/test_checkboxes.html` & `crispy-bulma-0.9.0/tests/results/test_checkboxes.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_clearable_file_field.html` & `crispy-bulma-0.9.0/tests/results/test_clearable_file_field.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_clearable_file_field_failing.html` & `crispy-bulma-0.9.0/tests/results/test_clearable_file_field_failing.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_file_field_failing.html` & `crispy-bulma-0.9.0/tests/results/test_file_field_failing.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_form_group.html` & `crispy-bulma-0.9.0/tests/results/test_form_group.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_form_group_horizontal.html` & `crispy-bulma-0.9.0/tests/results/test_form_group_horizontal.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_grouped_checkboxes.html` & `crispy-bulma-0.9.0/tests/results/test_grouped_checkboxes.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_grouped_checkboxes_failing.html` & `crispy-bulma-0.9.0/tests/results/test_grouped_checkboxes_failing.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_grouped_radios.html` & `crispy-bulma-0.9.0/tests/results/test_grouped_radios.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_grouped_radios_failing.html` & `crispy-bulma-0.9.0/tests/results/test_grouped_radios_failing.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_inline_checkboxes.html` & `crispy-bulma-0.9.0/tests/results/test_inline_checkboxes.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_inline_field.html` & `crispy-bulma-0.9.0/tests/results/test_inline_field.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <form class="align-items-center row row-cols-lg-auto" method="post">
     <div class="col-4" id="div_id_first_name">
         <label class="visually-hidden" for="id_first_name">
             first name
-        </label><input class="form-control inputtext textInput textinput" id="id_first_name" maxlength="5"
+        </label><input class="form-control inputtext" id="id_first_name" maxlength="5"
             name="first_name" placeholder="first name" required type="text">
     </div>
     <div class="col-4 form-check form-check-inline" id="div_id_is_company">
         <input class="checkboxinput form-check-input" id="id_is_company" name="is_company" type="checkbox"><label
             class="form-check-label" for="id_is_company">
             company
         </label>
     </div>
-</form>
+</form>
```

### Comparing `crispy-bulma-0.8.3/tests/results/test_inline_radios.html` & `crispy-bulma-0.9.0/tests/results/test_inline_radios.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_input_with_icon.html` & `crispy-bulma-0.9.0/tests/results/test_input_with_icon.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_prepended_appended_select.html` & `crispy-bulma-0.9.0/tests/results/test_prepended_appended_select.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_radio.html` & `crispy-bulma-0.9.0/tests/results/test_radio.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_selectmultiple.html` & `crispy-bulma-0.9.0/tests/results/test_selectmultiple.html`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/results/test_tabular_formset_layout.html` & `crispy-bulma-0.9.0/tests/results/test_tabular_formset_layout.html`

 * *Files 12% similar despite different names*

```diff
@@ -25,87 +25,87 @@
     <tr class="d-none empty-form">
         <div class="mb-3">
         <td id="div_id_form-__prefix__-is_company" class="mb-3"> <input type="checkbox"
             name="form-__prefix__-is_company" class="checkboxinput form-check-input"
             id="id_form-__prefix__-is_company"> </td>
         </div>
         <td id="div_id_form-__prefix__-email" class="mb-3"> <input type="text" name="form-__prefix__-email"
-            maxlength="30" class="textinput textInput inputtext form-control" id="id_form-__prefix__-email"> <small
+            maxlength="30" class="inputtext form-control" id="id_form-__prefix__-email"> <small
             id="hint_id_form-__prefix__-email" class="form-text text-muted">Insert your email</small> </td>
         <td id="div_id_form-__prefix__-password1" class="mb-3"> <input type="password"
-            name="form-__prefix__-password1" maxlength="30" class="textinput textInput form-control"
+            name="form-__prefix__-password1" maxlength="30" class="form-control"
             id="id_form-__prefix__-password1"> </td>
         <td id="div_id_form-__prefix__-password2" class="mb-3"> <input type="password"
-            name="form-__prefix__-password2" maxlength="30" class="textinput textInput form-control"
+            name="form-__prefix__-password2" maxlength="30" class="form-control"
             id="id_form-__prefix__-password2"> </td>
         <td id="div_id_form-__prefix__-first_name" class="mb-3"> <input type="text" name="form-__prefix__-first_name"
-            maxlength="5" class="textinput textInput inputtext form-control" id="id_form-__prefix__-first_name"> </td>
+            maxlength="5" class="inputtext form-control" id="id_form-__prefix__-first_name"> </td>
         <td id="div_id_form-__prefix__-last_name" class="mb-3"> <input type="text" name="form-__prefix__-last_name"
-            maxlength="5" class="textinput textInput inputtext form-control" id="id_form-__prefix__-last_name"> </td>
+            maxlength="5" class="inputtext form-control" id="id_form-__prefix__-last_name"> </td>
         <td id="div_id_form-__prefix__-datetime_field" class="mb-3"> <input type="text"
             name="form-__prefix__-datetime_field_0" class="dateinput form-control"
             id="id_form-__prefix__-datetime_field_0"><input type="text" name="form-__prefix__-datetime_field_1"
             class="timeinput form-control" id="id_form-__prefix__-datetime_field_1"> </td>
     </tr>
     <tr>
         <div class="mb-3">
         <td id="div_id_form-0-is_company" class="mb-3"> <input type="checkbox" name="form-0-is_company"
             class="checkboxinput form-check-input" id="id_form-0-is_company"> </td>
         </div>
         <td id="div_id_form-0-email" class="mb-3"> <input type="text" name="form-0-email" maxlength="30"
-            class="textinput textInput inputtext form-control" id="id_form-0-email"> <small id="hint_id_form-0-email"
+            class="inputtext form-control" id="id_form-0-email"> <small id="hint_id_form-0-email"
             class="form-text text-muted">Insert your email</small> </td>
         <td id="div_id_form-0-password1" class="mb-3"> <input type="password" name="form-0-password1" maxlength="30"
-            class="textinput textInput form-control" id="id_form-0-password1"> </td>
+            class="form-control" id="id_form-0-password1"> </td>
         <td id="div_id_form-0-password2" class="mb-3"> <input type="password" name="form-0-password2" maxlength="30"
-            class="textinput textInput form-control" id="id_form-0-password2"> </td>
+            class="form-control" id="id_form-0-password2"> </td>
         <td id="div_id_form-0-first_name" class="mb-3"> <input type="text" name="form-0-first_name" maxlength="5"
-            class="textinput textInput inputtext form-control" id="id_form-0-first_name"> </td>
+            class="inputtext form-control" id="id_form-0-first_name"> </td>
         <td id="div_id_form-0-last_name" class="mb-3"> <input type="text" name="form-0-last_name" maxlength="5"
-            class="textinput textInput inputtext form-control" id="id_form-0-last_name"> </td>
+            class="inputtext form-control" id="id_form-0-last_name"> </td>
         <td id="div_id_form-0-datetime_field" class="mb-3"> <input type="text" name="form-0-datetime_field_0"
             class="dateinput form-control" id="id_form-0-datetime_field_0"><input type="text"
             name="form-0-datetime_field_1" class="timeinput form-control" id="id_form-0-datetime_field_1"> </td>
     </tr>
     <tr>
         <div class="mb-3">
         <td id="div_id_form-1-is_company" class="mb-3"> <input type="checkbox" name="form-1-is_company"
             class="checkboxinput form-check-input" id="id_form-1-is_company"> </td>
         </div>
         <td id="div_id_form-1-email" class="mb-3"> <input type="text" name="form-1-email" maxlength="30"
-            class="textinput textInput inputtext form-control" id="id_form-1-email"> <small id="hint_id_form-1-email"
+            class="inputtext form-control" id="id_form-1-email"> <small id="hint_id_form-1-email"
             class="form-text text-muted">Insert your email</small> </td>
         <td id="div_id_form-1-password1" class="mb-3"> <input type="password" name="form-1-password1" maxlength="30"
-            class="textinput textInput form-control" id="id_form-1-password1"> </td>
+            class="form-control" id="id_form-1-password1"> </td>
         <td id="div_id_form-1-password2" class="mb-3"> <input type="password" name="form-1-password2" maxlength="30"
-            class="textinput textInput form-control" id="id_form-1-password2"> </td>
+            class="form-control" id="id_form-1-password2"> </td>
         <td id="div_id_form-1-first_name" class="mb-3"> <input type="text" name="form-1-first_name" maxlength="5"
-            class="textinput textInput inputtext form-control" id="id_form-1-first_name"> </td>
+            class="inputtext form-control" id="id_form-1-first_name"> </td>
         <td id="div_id_form-1-last_name" class="mb-3"> <input type="text" name="form-1-last_name" maxlength="5"
-            class="textinput textInput inputtext form-control" id="id_form-1-last_name"> </td>
+            class="inputtext form-control" id="id_form-1-last_name"> </td>
         <td id="div_id_form-1-datetime_field" class="mb-3"> <input type="text" name="form-1-datetime_field_0"
             class="dateinput form-control" id="id_form-1-datetime_field_0"><input type="text"
             name="form-1-datetime_field_1" class="timeinput form-control" id="id_form-1-datetime_field_1"> </td>
     </tr>
     <tr>
         <div class="mb-3">
         <td id="div_id_form-2-is_company" class="mb-3"> <input type="checkbox" name="form-2-is_company"
             class="checkboxinput form-check-input" id="id_form-2-is_company"> </td>
         </div>
         <td id="div_id_form-2-email" class="mb-3"> <input type="text" name="form-2-email" maxlength="30"
-            class="textinput textInput inputtext form-control" id="id_form-2-email"> <small id="hint_id_form-2-email"
+            class="inputtext form-control" id="id_form-2-email"> <small id="hint_id_form-2-email"
             class="form-text text-muted">Insert your email</small> </td>
         <td id="div_id_form-2-password1" class="mb-3"> <input type="password" name="form-2-password1" maxlength="30"
-            class="textinput textInput form-control" id="id_form-2-password1"> </td>
+            class="form-control" id="id_form-2-password1"> </td>
         <td id="div_id_form-2-password2" class="mb-3"> <input type="password" name="form-2-password2" maxlength="30"
-            class="textinput textInput form-control" id="id_form-2-password2"> </td>
+            class="form-control" id="id_form-2-password2"> </td>
         <td id="div_id_form-2-first_name" class="mb-3"> <input type="text" name="form-2-first_name" maxlength="5"
-            class="textinput textInput inputtext form-control" id="id_form-2-first_name"> </td>
+            class="inputtext form-control" id="id_form-2-first_name"> </td>
         <td id="div_id_form-2-last_name" class="mb-3"> <input type="text" name="form-2-last_name" maxlength="5"
-            class="textinput textInput inputtext form-control" id="id_form-2-last_name"> </td>
+            class="inputtext form-control" id="id_form-2-last_name"> </td>
         <td id="div_id_form-2-datetime_field" class="mb-3"> <input type="text" name="form-2-datetime_field_0"
             class="dateinput form-control" id="id_form-2-datetime_field_0"><input type="text"
             name="form-2-datetime_field_1" class="timeinput form-control" id="id_form-2-datetime_field_1"> </td>
     </tr>
     </tbody>
 </table>
-</form>
+</form>
```

### Comparing `crispy-bulma-0.8.3/tests/results/test_tabular_formset_layout_failing.html` & `crispy-bulma-0.9.0/tests/results/test_tabular_formset_layout_failing.html`

 * *Files 8% similar despite different names*

```diff
@@ -25,28 +25,28 @@
             <tr class="d-none empty-form">
                 <div class="mb-3">
                     <td class="mb-3" id="div_id_form-__prefix__-is_company"><input
                             class="checkboxinput form-check-input" id="id_form-__prefix__-is_company"
                             name="form-__prefix__-is_company" type="checkbox"></td>
                 </div>
                 <td class="mb-3" id="div_id_form-__prefix__-email"><input
-                        class="form-control inputtext textInput textinput" id="id_form-__prefix__-email" maxlength="30"
+                        class="form-control inputtext" id="id_form-__prefix__-email" maxlength="30"
                         name="form-__prefix__-email" type="text"><small class="form-text text-muted"
                         id="hint_id_form-__prefix__-email">Insert your email</small></td>
-                <td class="mb-3" id="div_id_form-__prefix__-password1"><input class="form-control textInput textinput"
+                <td class="mb-3" id="div_id_form-__prefix__-password1"><input class="form-control"
                         id="id_form-__prefix__-password1" maxlength="30" name="form-__prefix__-password1"
                         type="password"></td>
-                <td class="mb-3" id="div_id_form-__prefix__-password2"><input class="form-control textInput textinput"
+                <td class="mb-3" id="div_id_form-__prefix__-password2"><input class="form-control"
                         id="id_form-__prefix__-password2" maxlength="30" name="form-__prefix__-password2"
                         type="password"></td>
                 <td class="mb-3" id="div_id_form-__prefix__-first_name"><input
-                        class="form-control inputtext textInput textinput" id="id_form-__prefix__-first_name"
+                        class="form-control inputtext" id="id_form-__prefix__-first_name"
                         maxlength="5" name="form-__prefix__-first_name" type="text"></td>
                 <td class="mb-3" id="div_id_form-__prefix__-last_name"><input
-                        class="form-control inputtext textInput textinput" id="id_form-__prefix__-last_name"
+                        class="form-control inputtext" id="id_form-__prefix__-last_name"
                         maxlength="5" name="form-__prefix__-last_name" type="text"></td>
                 <td class="mb-3" id="div_id_form-__prefix__-datetime_field"><input class="dateinput form-control"
                         id="id_form-__prefix__-datetime_field_0" name="form-__prefix__-datetime_field_0"
                         type="text"><input class="form-control timeinput" id="id_form-__prefix__-datetime_field_1"
                         name="form-__prefix__-datetime_field_1" type="text"></td>
             </tr>
             <div class="alert alert-block alert-danger">
@@ -56,36 +56,36 @@
             </div>
             <tr>
                 <div class="mb-3">
                     <td class="mb-3" id="div_id_form-0-is_company"><input class="checkboxinput form-check-input"
                             id="id_form-0-is_company" name="form-0-is_company" type="checkbox"></td>
                 </div>
                 <td class="mb-3" id="div_id_form-0-email"><input
-                        class="form-control inputtext is-invalid textInput textinput" id="id_form-0-email"
+                        class="form-control inputtext is-invalid" id="id_form-0-email"
                         maxlength="30" name="form-0-email" type="text"><span class="invalid-feedback"
                         id="error_1_id_form-0-email"><strong>This field is required.</strong></span><small
                         class="form-text text-muted" id="hint_id_form-0-email">Insert your email</small></td>
-                <td class="mb-3" id="div_id_form-0-password1"><input class="form-control is-invalid textInput textinput"
+                <td class="mb-3" id="div_id_form-0-password1"><input class="form-control is-invalid"
                         id="id_form-0-password1" maxlength="30" name="form-0-password1" type="password"><span
                         class="invalid-feedback" id="error_1_id_form-0-password1"><strong>This field is
                             required.</strong></span></td>
-                <td class="mb-3" id="div_id_form-0-password2"><input class="form-control is-invalid textInput textinput"
+                <td class="mb-3" id="div_id_form-0-password2"><input class="form-control is-invalid"
                         id="id_form-0-password2" maxlength="30" name="form-0-password2" type="password"><span
                         class="invalid-feedback" id="error_1_id_form-0-password2"><strong>This field is
                             required.</strong></span></td>
                 <td class="mb-3" id="div_id_form-0-first_name"><input
-                        class="form-control inputtext is-invalid textInput textinput" id="id_form-0-first_name"
+                        class="form-control inputtext is-invalid" id="id_form-0-first_name"
                         maxlength="5" name="form-0-first_name" type="text"><span class="invalid-feedback"
                         id="error_1_id_form-0-first_name"><strong>This field is required.</strong></span></td>
                 <td class="mb-3" id="div_id_form-0-last_name"><input
-                        class="form-control inputtext is-invalid textInput textinput" id="id_form-0-last_name"
+                        class="form-control inputtext is-invalid" id="id_form-0-last_name"
                         maxlength="5" name="form-0-last_name" type="text"><span class="invalid-feedback"
                         id="error_1_id_form-0-last_name"><strong>This field is required.</strong></span></td>
                 <td class="mb-3" id="div_id_form-0-datetime_field"><input class="dateinput form-control is-invalid"
                         id="id_form-0-datetime_field_0" name="form-0-datetime_field_0" type="text"><input
                         class="form-control is-invalid timeinput" id="id_form-0-datetime_field_1"
                         name="form-0-datetime_field_1" type="text"><span class="invalid-feedback"
                         id="error_1_id_form-0-datetime_field"><strong>This field is required.</strong></span></td>
             </tr>
         </tbody>
     </table>
-</form>
+</form>
```

### Comparing `crispy-bulma-0.8.3/tests/test_form_helper.py` & `crispy-bulma-0.9.0/tests/test_form_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 def test_invalid_form_method():
     form_helper = FormHelper()
     with pytest.raises(FormHelpersException):
         form_helper.form_method = "superPost"
 
 
-def test_form_with_helper_without_layout(settings):
+def test_form_with_helper_without_layout():
     form_helper = FormHelper()
     form_helper.form_id = "this-form-rocks"
     form_helper.form_class = "forms-that-rock"
     form_helper.form_method = "GET"
     form_helper.form_action = "simpleAction"
     form_helper.form_error_title = "ERRORS"
 
@@ -124,17 +124,14 @@
     # Lets make sure everything loads right
     assert html.count("<form") == 1
     assert "forms-that-rock" in html
     assert 'method="get"' in html
     assert 'id="this-form-rocks"' in html
     assert 'action="%s"' % reverse("simpleAction") in html
 
-    if settings.CRISPY_TEMPLATE_PACK == "uni_form":
-        assert 'class="uniForm' in html
-
     assert "ERRORS" in html
     assert "<li>Passwords dont match</li>" in html
 
     # now lets remove the form tag and render it again. All the True items above
     # should now be false because the form tag is removed.
     form_helper.form_tag = False
     html = template.render(c)
@@ -173,29 +170,14 @@
 
     # Ensure errors were not rendered
     assert "<li>Passwords dont match</li>" not in html
     assert str(_("This field is required.")) not in html
     assert "error" not in html
 
 
-def test_html5_required():
-    form = SampleForm()
-    form.helper = FormHelper()
-    form.helper.html5_required = True
-    html = render_crispy_form(form)
-    # 6 out of 7 fields are required and an extra one for the
-    # SplitDateTimeWidget makes 7.
-    assert len(re.findall(r"\brequired\b", html)) == 7
-
-    form = SampleForm()
-    form.helper = FormHelper()
-    form.helper.html5_required = False
-    html = render_crispy_form(form)
-
-
 def test_media_is_included_by_default_with_bulma():
     form = SampleFormWithMedia()
     form.helper = FormHelper()
     form.helper.template_pack = "bulma"
     html = render_crispy_form(form)
     assert "test.css" in html
     assert "test.js" in html
@@ -291,15 +273,15 @@
 
     settings.CRISPY_FAIL_SILENTLY = settings.TEMPLATE_DEBUG = False
     with pytest.raises(TypeError):
         template.render(c)
 
 
 @pytest.mark.skip(reason="formset")
-def test_formset_with_helper_without_layout(settings):
+def test_formset_with_helper_without_layout():
     template = Template(
         """
         {% load crispy_forms_tags %}
         {% crispy testFormSet formset_helper %}
     """
     )
 
@@ -329,16 +311,14 @@
     assert "form-INITIAL_FORMS" in html
     assert "form-MAX_NUM_FORMS" in html
 
     assert "formsets-that-rock" in html
     assert 'method="post"' in html
     assert 'id="thisFormsetRocks"' in html
     assert 'action="%s"' % reverse("simpleAction") in html
-    if settings.CRISPY_TEMPLATE_PACK == "uni_form":
-        assert 'class="uniForm' in html
 
 
 def test_CSRF_token_POST_form():
     form_helper = FormHelper()
     template = Template(
         """
         {% load crispy_forms_tags %}
```

### Comparing `crispy-bulma-0.8.3/tests/test_layout.py` & `crispy-bulma-0.9.0/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/test_layout_objects.py` & `crispy-bulma-0.9.0/tests/test_layout_objects.py`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/test_settings.py` & `crispy-bulma-0.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `crispy-bulma-0.8.3/tests/test_tags.py` & `crispy-bulma-0.9.0/tests/test_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 
-import django
 from django.forms.boundfield import BoundField
 from django.forms.formsets import formset_factory
 from django.template import Context, Template
 from django.test import override_settings
 
 from crispy_forms.exceptions import CrispyError
 from crispy_forms.templatetags.crispy_forms_field import crispy_addon
@@ -95,18 +94,15 @@
         }
     )
     formset.is_valid()
 
     c = Context({"formset": formset})
     html = template.render(c)
     assert "errorMsg" in html or "alert" in html
-    if django.VERSION < (3, 2):
-        assert "<li>Please submit 1 or fewer forms.</li>" in html
-    else:
-        assert "<li>Please submit at most 1 form.</li>" in html
+    assert "<li>Please submit at most 1 form.</li>" in html
     assert "<h3>" not in html
 
 
 def test_as_crispy_field_non_field(settings):
     template = Template(
         """
         {% load crispy_forms_tags %}
```

### Comparing `crispy-bulma-0.8.3/tests/utils.py` & `crispy-bulma-0.9.0/tests/utils.py`

 * *Files identical despite different names*

