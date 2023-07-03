# Comparing `tmp/abstra-0.9.0.tar.gz` & `tmp/abstra-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/abstra-0.9.0.tar", last modified: Fri Mar 17 14:49:52 2023, max compression
+gzip compressed data, was "dist/abstra-1.0.0.tar", last modified: Mon Jul  3 18:14:07 2023, max compression
```

## Comparing `abstra-0.9.0.tar` & `abstra-1.0.0.tar`

### file list

```diff
@@ -1,72 +1,888 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-17 14:49:52.000000 abstra-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-17 14:49:37.000000 abstra-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/dashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra/widgets/library/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/AnswerSheetInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CardsInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CheckboxInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ChecklistInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ClickInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CnpjInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CodeInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CpfInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CurrencyInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/DateInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/DropdownInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/EmailInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/FileInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/FileOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/HtmlOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/IframeOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ImageInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ImageOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/KanbanBoardInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/LatexOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/LinkOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ListInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/MarkdownOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/MultipleChoiceInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/NpsInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/NumberInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/NumberSliderInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PandasOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PandasRowSelectionInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PasswordInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PhoneInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PlotlyOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ProgressOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/RatingInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TagInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TextInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TextOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TextareaInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TimeInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ToggleInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/VideoInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/widget_base.py
--rw-r--r--   0 runner    (1001) docker     (123)   280192 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/response_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/widget_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/widget_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 14:49:52.000000 abstra-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-17 14:49:37.000000 abstra-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:07.000000 abstra-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-03 18:14:07.000000 abstra-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-03 18:13:39.000000 abstra-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/dashes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/debug_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra/forms/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40867 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/generated/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/generated/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53225 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/generated/widget_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/list_item_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/page_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/reactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/forms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/tables/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/tables/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra/widgets/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/AnswerSheetInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/CardsInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/CheckboxInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/ChecklistInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/ClickInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/CnpjInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/CodeInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/CpfInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/CurrencyInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/CustomInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/DateInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/DropdownInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/EmailInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/FileInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/FileOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/HtmlOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/IframeOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/ImageInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/ImageOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/KanbanBoardInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/LatexOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/LinkOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/ListInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/MarkdownOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/MultipleChoiceInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/NpsInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/NumberInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/NumberSliderInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/PandasOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/PandasRowSelectionInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/PasswordInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/PhoneInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/PlotlyOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/ProgressOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/RatingInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/RichTextInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/TagInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/TextInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/TextOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/TextareaInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/TimeInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/ToggleInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/VideoInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/library/widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   316387 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/response_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra/widgets/widget_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37444 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_cli/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/dashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/subdomains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/apis/workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/dashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/subdomains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/resources/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/utils/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/utils/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/api/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/apps/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/apps/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/contract/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/contract/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/contract/dashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/contract/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/overloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/runtimes/dashes/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/dashes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/dashes/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/dashes/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/dashes/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/runtimes/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/forms/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/runtimes/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_server/runtimes/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/runtimes/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_statics/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:06.000000 abstra-1.0.0/abstra_statics/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/IfBlock.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:07.000000 abstra-1.0.0/abstra_statics/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AD.d9b7879b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AE.634f1116.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AF.22cf8d2c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AG.e9e66959.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AL.595dc1e0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AM.a13e8ede.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AO.3d382dd3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AR.9e19d442.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AT.7f745c0e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AU.9609169d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AW.8cebd800.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/AZ.00ed0296.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ApiKeys.07320cff.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ApiKeys.565e4da2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BA.20a3c832.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BB.68d11590.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BD.faa434d0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BE.704ec6c4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BF.617a7e60.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BG.aee8effa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BH.91bf6bff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BI.ef2db71e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BJ.6e4e173e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BN.d7e937c6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BO.e482a67a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BR.21ae1f9c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BS.598f106c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BT.4d5713c7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BW.60db8307.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BY.01420a44.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BZ.1f927f51.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.05f1911d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.0686fb5a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.1bd55e3c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.21fd810f.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.467d93ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.7411b00a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.7438db42.css
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.802d214e.css
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.9a7f01c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.ae9a631b.css
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.c350c17f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.dbd772ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.e9f71cf5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.f34770a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.fe1ad1ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/BackButton.ffb72b1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Builds.c48a1805.js
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ButtonWithIcon.35687b29.js
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ButtonWithIcon.59b28959.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CA.10ab164a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CD.03157053.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CF.76b7213b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CG.9bc5f25d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CH.85ab01e7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CI.d6246e4a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CL.1761c997.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CM.2f932da1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CN.a696f3cd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CO.cf732cb4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CR.53cb82e4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CU.1b40bda1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CV.c4cd6eea.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CY.b6d13408.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CZ.e3582ef7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   299145 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CircularLoading.59d7fd3d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   299145 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CircularLoading.89577a16.js
+-rw-r--r--   0 runner    (1001) docker     (123)   298732 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CircularLoading.cef8a22f.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CircularLoading.f81b57b4.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CrudView.20b9da12.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/CrudView.fcb5b6d8.css
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DE.ceca9894.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DJ.30f3c17e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DK.11a412b0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DM.5ac0933e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DO.e16d6925.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DZ.23a5cea1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.0c519322.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.0d379120.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64456 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.22e8f726.js
+-rw-r--r--   0 runner    (1001) docker     (123)    65011 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.283fdca3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.36d1f0a5.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.3e62cf8a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.4295c1bd.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64467 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.7273a648.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.861b2b5b.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.919089d5.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64684 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.92b21de1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64684 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.99796c98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64456 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.9eb4cb4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64696 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.9ed2a800.js
+-rw-r--r--   0 runner    (1001) docker     (123)    65036 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.a8d4191d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64711 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.d3e4535e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64810 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.d496431b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64684 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashEditor.e3dd5d37.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPlayer.3b3076a0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40365 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPlayer.526e44da.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40328 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPlayer.56553644.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPlayer.6b0e40bf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40328 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPlayer.7373a7f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40328 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPlayer.d88d0731.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPlayer.f60035bd.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.2ce870bf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.4ac074a5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.5febe542.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.63921711.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.64450e79.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.6d494ae5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.74617a8b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.94ee56a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DashPreview.cc968db7.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Dashes.27789115.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Dashes.40d56794.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Dashes.4dca928b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Dashes.6fb3fa8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Dashes.8c1d4eac.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Dashes.c740c421.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Dashes.dc83c12f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DropdownMenu.5abf24d0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/DropdownMenu.f9c0b8cd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/EC.f6ea9e10.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/EE.7a6f3b22.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/EG.50036f48.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ER.79d67b90.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ES.48402498.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ET.dd9f04ce.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/EnvVars.d8500348.js
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Error.5cfc41d8.css
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Error.de2ae46c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Error.e6ce10ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Error.fd927673.js
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FI.ef706e32.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FJ.14b2d880.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FM.bdc49a3c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FR.336e90c0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.0225fbda.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.07b05447.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.0f529fb4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.149481b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.1c24c746.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.32bb1fbb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.3c610c3d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.3e4dba2f.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.81e943eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.888dcac0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.8a54b880.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.b0ff8fde.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.cdd43079.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.f2e6ac20.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormEditor.f8ea695c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.07bb010f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.1ecd3c94.js
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.69e549a7.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.91d90ce9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.a576dc7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.b0b40fce.js
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.c6c54868.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.f2da1287.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/FormPreview.fe6a99a8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Forms.084081fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Forms.4ba06962.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Forms.4d214f5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Forms.8f844ffe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Forms.c36934cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Forms.df228d0b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GA.63234e0c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GB.c3c40c55.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GD.f7b9e7b3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GE.1bd3a5e6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GH.9917d988.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GM.ecb91acb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GN.5ecf0991.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GQ.cf218948.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GR.a1d7c3cf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GT.20d8d46d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GW.a701fc41.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/GY.e0b00d54.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HK.1e78a2b0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HN.17063869.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HR.230cef5b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HT.ebd12df1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HU.e1a0940b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Home.1c04d83a.css
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Home.202e3431.js
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Home.3854bdc9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Home.5fc0c856.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.029f2d3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.063b9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.3f455dbc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.468d9d10.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.530f253d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.630dbb87.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.7c51dc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.830a8417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.a3db11d1.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.ae396e80.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.b2f9c960.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.c007bcab.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/HookEditor.dec8afb8.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Hooks.2e477da3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Hooks.46a5d242.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Hooks.5ce1570a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Hooks.5f9e9bd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Hooks.72316ccb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Hooks.a3269158.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Hooks.c18563cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ID.41f81c7b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/IE.125a51ea.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/IL.647b3d1c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/IN.1564e97a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/IQ.0ea6f8c9.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/IR.de331507.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/IS.15daa1ae.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/IT.6fe7f000.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JM.89e4fbca.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JO.6cd1431a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JP.060b0a81.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32174 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.43a8dc96.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.4c734b2f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32343 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.4cef59f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32342 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.632f2855.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.65e83508.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.b644c810.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.c6cf75b2.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.d5473a5a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32442 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.dd1534c0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.e5f4d76c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.e92b89e4.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.e9c87edc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.f75c6c78.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32377 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/JobEditor.fcbe750c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.12becfb9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.8cbedbeb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.8e7fd096.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.8eb4faf3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.bffd2f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.de40f5b3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.ec5025ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Jobs.fbf373ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KE.52a4047f.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KG.34c50057.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KH.c062424c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KM.2f46806a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KP.18264f14.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KR.9d772a89.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KW.3e722fc6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/KZ.66396182.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LA.76acc54e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LB.70c16585.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LC.4081d3cf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LI.066cb02d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LK.d03b9856.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LR.500fa830.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LS.5f5ef57b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LT.5427c16d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LU.a36532df.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LV.a76bad4d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/LY.3347db57.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Login.0394245e.css
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Login.3624d803.js
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MA.7cdae0ec.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MC.fe98c108.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MD.58612331.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ME.3d5b9393.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MG.c6708cda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MK.45498ebc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ML.aa8d8866.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MM.c584fe1e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MN.4f251a51.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MQ.fbed0a4b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MR.11db4d97.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MT.2d20096e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MU.6f4cd188.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MV.9ad63919.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MW.adaba0c4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MX.4c1e987d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MY.53429c98.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/MZ.d1f10678.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Members.fca19282.js
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Modal.29f9eb98.css
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Modal.2ceba592.js
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Modal.5aaf8eba.css
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Modal.8745ec05.js
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Modal.bc20d9b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NA.b01ff39a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NE.1dcaf7e3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NG.97dbee7d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NI.39141b8a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NL.32c9b0e0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NO.55213eaf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NP.08c36460.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NR.b19f253f.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/NZ.f777e447.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Navbar.60d8d8eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Navbar.84f52f8d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/OM.81e030e7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Organization.2cc71128.js
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Organization.48a2e6fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/OrganizationSettings.cfd9b8c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Organizations.6ac1d5ed.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Organizations.7dbd86dc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PA.3074e313.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PE.dc540660.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PG.d1e0c299.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PH.940eb551.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PK.24d03904.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PL.dbb32cb3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PS.bdc0e68d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PT.86ed6e99.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PW.cd26731b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/PY.aed3776c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Passwordless.1696a947.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Passwordless.c981501a.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Player.144caca5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Player.3d55b4fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Player.82401ce5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Player.ab345cf7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Player.b2660e36.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Player.d5eab81a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Player.eb229b81.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Project.d9ec5254.js
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Project.f09233c8.css
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ProjectSettings.5975fb49.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Projects.d4e97876.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/QA.58b347e8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RO.f49289dc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RS.68223037.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RU.7a003302.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RW.46ecbfb0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RuntimeList.106b52b7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RuntimeList.1a694a92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RuntimeList.3913631a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RuntimeList.7704c49f.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/RuntimeList.fb8a1e5e.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SA.e1cb5dd6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SB.eaafb7a5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SC.2849eccf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SD.2cba080b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SE.a22c1896.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SG.7b117d09.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SI.79831723.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SK.0fd2411c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SL.2b3d4f82.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SM.fcacf5d4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SN.a3e19ac5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SO.f3980904.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SR.5542d97f.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SS.91f1d751.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ST.a5b3747c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SV.a43c07ef.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SY.869ac965.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SZ.ca793866.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SaveButton.0f1a1078.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SaveButton.39be38fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SaveButton.3fd01c4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SaveButton.5cd5bd07.css
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SaveButton.90897407.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SaveButton.afacdfe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SaveButton.f1dc522a.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.19c0a661.css
+-rw-r--r--   0 runner    (1001) docker     (123)    45894 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.276efec7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45894 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.295d42a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45890 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.3408553a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45894 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.3a0d0684.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45931 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.63cf6116.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.9b9e4960.css
+-rw-r--r--   0 runner    (1001) docker     (123)    45894 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Settings.a61c6fb4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Sidebar.a295cdc7.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Sidebar.e9cedb40.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.03445c4c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.08de4d8d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.20fc70ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.2dca9a38.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.3078b513.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.41690e74.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.5ee5532f.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.779b6df2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.9a68b5ac.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.cdf4c03b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.de1ab198.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/SmartConsole.fb5bafc1.css
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TC.eae8b06e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TD.c539df50.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TG.ebc933be.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TH.18022161.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TJ.ba058331.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TL.8c67ea11.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TM.f6615c11.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TN.bfd12a95.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TO.53425167.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TR.0ca703a3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TT.1656516e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TZ.809af5c7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TableEditor.12bf9b56.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TableEditor.6b74d645.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TableEditor.73c06e25.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/TableEditor.ea1a2f33.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Tables.02be8cbd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Tables.74d48a4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Tables.ead7e850.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Tooltip.63c4352e.css
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Tooltip.879659d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/UA.a4cbac5d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/UG.1b065c29.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/US.a4361620.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/UY.53b87108.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/UZ.580fb67d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/VC.72a4136b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/VE.52d4ec7c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/VN.85ca6627.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/VU.ff080334.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WS.375cbc97.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WidgetsFrame.015f5931.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WidgetsFrame.1013b5e8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WidgetsFrame.47768dce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24075 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WidgetsFrame.783acd39.css
+-rw-r--r--   0 runner    (1001) docker     (123)    29779 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WidgetsFrame.7e48c68b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29779 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WidgetsFrame.cebd6d3d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/WidgetsFrame.f427edd2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.020de22f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.082a7639.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.19ebbc6c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.1f4b6fe5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.28e97aea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.89631035.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.9e3a8205.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.bb1d171c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.cc950962.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/Workspace.efad2738.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/YE.10f3018f.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ZA.63a587bc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ZM.7ef07ee8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ZW.80d84f56.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/abap.15cc56c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/apex.3097bfba.js
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/asyncComputed.841de1fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/azcli.b70fb9b3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/bat.4e83862e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/bicep.107c4876.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15896 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/broker.22806872.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/broker.64603716.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15896 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/broker.6d8b5367.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/broker.b057aed3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/broker.b9a40809.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/broker.c3576dd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/cameligo.9b7ef084.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/clojure.9b9ce362.js
+-rw-r--r--   0 runner    (1001) docker     (123)    72504 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/codicon.71cccbf1.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/coffee.3343db4b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/color.473bc8ca.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/console.faeffdee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/cpp.5842f29e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/csharp.711e6ef5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/csp.1454e635.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/css.0f39058b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33796 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/cssMode.4686a6ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33796 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/cssMode.57850b5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33796 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/cssMode.d8d026cd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/cypher.8b877bda.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/dart.d9ca4827.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/dashes.8e41d473.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/dashes.b38d2459.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/dashes.da7ff1db.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/dashes.f5f65b41.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/dockerfile.b12c8d75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ecl.5841a83e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   232554 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.053e6919.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.0d83b914.js
+-rw-r--r--   0 runner    (1001) docker     (123)   232554 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.168d39d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83038 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.30d77c87.css
+-rw-r--r--   0 runner    (1001) docker     (123)   231378 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.3b947933.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231240 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.3ebe774c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231378 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.4b26f8d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231240 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.4bfcc5fe.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.6598cb79.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231176 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.807c1a16.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.8cb3438e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231378 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.d3ad0052.js
+-rw-r--r--   0 runner    (1001) docker     (123)   232554 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.db9333ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.f054e8f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2786162 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.main.0ad64f00.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2786162 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.main.8ac4b83d.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2786162 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/editor.main.c431dd7b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/elixir.837d31f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/empty-box.758770e4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/flow9.02cb4afd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/forms.7bc6baea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/forms.a8d20ba7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/freemarker2.4acd8a93.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/freemarker2.c415f147.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/freemarker2.d1c5507e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/fsharp.c6cc3d99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/go.e18cc8fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/graphql.91865f29.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/handlebars.572f33ee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/handlebars.909dda29.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/handlebars.d40eca03.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/hcl.89542f1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/hooks.039c0cd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/hooks.2479f4f4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/hooks.944007d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/html.532be59b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/html.b8b94c67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/html.eea05465.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/htmlMode.3dbe0b56.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/htmlMode.6f056605.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/htmlMode.ff962a6e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/icons.5214a3f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/icons.907f45d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/icons.a63cb90b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/icons.b8ff2c28.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/icons.ea1ef9e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/index.314cf40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/index.7a773bce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    54526 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/index.d20ddea0.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/index.e104c322.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ini.927d4958.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/java.cae92986.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/javascript.6d8bc9e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/javascript.78a20bd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/javascript.d32f3a78.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/jobs.84cb688a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/jobs.987450d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/jobs.9a947645.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/jobs.af366134.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39838 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/jsonMode.8d3520ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39838 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/jsonMode.9f6458aa.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39838 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/jsonMode.aa675433.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/julia.1ab2c6a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/kotlin.567012b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/less.8ff15de1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/lexon.892ac9e8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/liquid.16e8c3fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/liquid.181ccf90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/liquid.3d295eb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/log.1679837e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/log.2520bfaa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/log.7bdc5c83.js
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/logo.084e5d7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/logo.0faadfa2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/lua.84919ba3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/m3.dbd6d890.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/markdown.0bd269fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/member.35180141.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/mips.5b57214f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/msdax.664f04d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/mysql.b3be80b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/objective-c.f61689b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/organization.91baba90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/pascal.63810ab2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/pascaligo.f3c373fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/passwordlessManager.d8088db9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/perl.7a13b920.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/pgsql.231377e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/php.f75fab85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/pla.53add393.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/player.1e51a78a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/player.4d3f1197.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/player.5a355670.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/player.821c820c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/player.a0f983fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/player.da34eff2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/postiats.b78836c4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/powerquery.40e0a8e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/powershell.b2dc53b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    72204 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/primeicons.131bc3bf.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/primeicons.3824be50.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   291454 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/primeicons.5e10f102.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    72280 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/primeicons.90a58d3a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    72380 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/primeicons.ce852338.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/project.eda7f383.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/protobuf.bce7ad87.js
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/pubsub.a0411919.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/pug.e7bd8f2e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/python.8d171686.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/python.9f9d29e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/python.d0665899.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/qsharp.9d22faff.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/r.77bb7e19.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/razor.971e2370.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/razor.9c779edc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/razor.e34ad34f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/redis.d60fd379.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/redshift.3c32617e.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1802039 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/registerWidgets.81004098.js
+-rw-r--r--   0 runner    (1001) docker     (123)    77730 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/registerWidgets.c131d556.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77730 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/registerWidgets.c4c71ee6.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1801973 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/registerWidgets.d12d7cf9.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1801972 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/registerWidgets.fff064a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/restructuredtext.6d30740a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/ruby.10c929d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   159071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/runnerData.12d27e35.js
+-rw-r--r--   0 runner    (1001) docker     (123)   159071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/runnerData.81f4c073.js
+-rw-r--r--   0 runner    (1001) docker     (123)   159085 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/runnerData.9e14dd92.js
+-rw-r--r--   0 runner    (1001) docker     (123)   159071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/runnerData.a1d2b4df.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/rust.abc56d3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/sb.4973b57f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/scala.2026dee1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/scheme.fe55144d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/scss.4ba8f803.js
+-rw-r--r--   0 runner    (1001) docker     (123)   222491 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/sentry.923a3738.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/shell.2643570b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18889 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/solidity.9a85e4e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/sophia.ae3e217e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/sparql.6944fd44.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/sql.4f48b9c1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/st.7c961594.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/swift.23da7225.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/systemverilog.0eef8e45.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/tables.831fc587.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/tables.cffe2d61.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/tables.e9c2644d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/tcl.236460f4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/tsMode.7df1f426.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/tsMode.a7cb20a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/tsMode.babb8407.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/twig.b70b7ae1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/typescript.2cacf20b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/typescript.2fe931e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/typescript.81b312d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/utils.3371dfe5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/utils.ac5c1175.js
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/utils.f91c500c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/vb.5502a104.js
+-rw-r--r--   0 runner    (1001) docker     (123)   256708 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/vue-quill.esm-bundler.6d0a33e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   256708 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/vue-quill.esm-bundler.7582c4d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   256708 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/vue-quill.esm-bundler.94105e4b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/workspaces.252c90d6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/workspaces.32af92db.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/xml.0bac6c8b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/xml.9cd0dbe8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/xml.fca458fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/yaml.35e44807.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/yaml.70e2347a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/assets/yaml.cd75ddf4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/chevron-down-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/chevron-down-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/chevron-up-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/chevron-up-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/circularLoading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/dash-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/dash-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/dash-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/drag-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/drag-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/editor.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1125202 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/player.html
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/thumbnail.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:07.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/AnswerSheetInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CardsInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CheckboxInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/ChecklistInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/ClickInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CnpjInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CodeInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CpfInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CurrencyInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CustomInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/CustomOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/DateInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/DropdownInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/EmailInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/FileInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/FileOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/HtmlOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/IframeOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/ImageInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/ImageOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/KanbanBoardInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   141072 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/LatexOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/LinkOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/ListInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46699 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/MarkdownOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/MultipleChoiceInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/NpsInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/NumberInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/NumberSliderInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/PandasOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/PandasRowSelectionInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/PasswordInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/PhoneInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/PlotlyOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/ProgressOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/RatingInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/RichTextInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/TagInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/TextInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/TextOutput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/TextareaInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/TimeInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/ToggleInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-03 18:13:39.000000 abstra-1.0.0/abstra_statics/dist/widget-thumbs/VideoInput.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:14:07.000000 abstra-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-03 18:13:39.000000 abstra-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:14:07.000000 abstra-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/example_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_compute_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_server_dashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_server_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_server_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 18:13:39.000000 abstra-1.0.0/tests/test_widgets.py
```

### Comparing `abstra-0.9.0/PKG-INFO` & `abstra-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstra
-Version: 0.9.0
+Version: 1.0.0
 Summary: Abstra Lib
 Home-page: https://github.com/abstra-app/abstra-lib
 License: MIT
 Description: [![pypi](https://img.shields.io/pypi/v/abstra.svg)](https://pypi.python.org/pypi/abstra)
         [![PyPI Downloads](https://img.shields.io/pypi/dm/abstra.svg)](https://pypi.org/project/abstra/)
         [![Code check](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml/badge.svg)](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml)
```

### Comparing `abstra-0.9.0/README.md` & `abstra-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/connectors.py` & `abstra-1.0.0/abstra/connectors.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/hooks.py` & `abstra-1.0.0/abstra/hooks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,50 @@
+from io import BytesIO
 import os, json
 
 
-def get_request(local_file="request.json"):
+def _app_json_parse(body: str):
+    return json.loads(body)
+
+
+def _multipart_form_parse(body: str, headers: dict):
+    from multipart import MultipartParser, to_bytes, parse_options_header
+
+    _, options = parse_options_header(headers["Content-Type"])
+    boundary = options["boundary"].encode("utf-8")
+    p = MultipartParser(BytesIO(to_bytes(body)), boundary)  # TODO: direct from fs
+    return [{"name": i.name, "value": i.value} for i in p]
+
+
+def get_raw_request(local_file="request.json"):
     try:
         with open(os.getenv("REQUEST_FILE", local_file)) as f:
             request = json.loads(f.read())
             body = request["body"]
             query = request["query"]
             headers = request["headers"]
-
-        try:
-            if headers["Content-Type"] == "application/json":
-                return json.loads(body), query, headers
-            else:
-                return body, query, headers
-        except Exception:
-            return body, query, headers
+        return body, query, headers
 
     except Exception:
         return None, None, None
 
 
+def get_request(local_file="request.json"):
+    body, query, headers = get_raw_request(local_file)
+    try:
+        if "application/json" in headers["Content-Type"]:
+            return _app_json_parse(body), query, headers
+        elif "multipart/form-data" in headers["Content-Type"]:
+            return _multipart_form_parse(body, headers), query, headers
+        else:
+            return body, query, headers
+    except Exception:
+        return body, query, headers
+
+
 def send_response(body="", status_code=200, headers={}, local_file="response.json"):
     response = {"status_code": status_code, "body": body, "headers": headers}
     path = os.getenv("RESPONSE_FILE", local_file)
     content = json.dumps(response)
     with open(path, "w") as f:
         f.write(content)
```

### Comparing `abstra-0.9.0/abstra/tables.py` & `abstra-1.0.0/abstra/tables.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/__init__.py` & `abstra-1.0.0/abstra/widgets/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 
 from abstra.widgets import library
-from .widget_base import Input, Output  # exported
+from .widget_base import Input, Output
 from .metadata import metadata
 
 
 output_types = [
     w for w in library.__dict__.values() if inspect.isclass(w) and issubclass(w, Output)
 ]
 
@@ -29,14 +29,27 @@
     try:
         prop = _get_prop(widget_type, prop_name)
         return not prop["isKwarg"]
     except:
         return False
 
 
+def _get_broker_prop(widget_type: str, prop_name: str):
+    params = metadata[widget_type]["brokerAPI"]["params"]
+    return [p for p in params if p["argName"] == prop_name][0]
+
+
+def is_broker_prop_form_only(widget_type: str, prop_name: str):
+    try:
+        prop = _get_broker_prop(widget_type, prop_name)
+        return prop["formOnly"]
+    except:
+        return False
+
+
 def get_widget_name(widget_type: str):
     try:
         return metadata[widget_type]["name"]
     except:
         return None
```

### Comparing `abstra-0.9.0/abstra/widgets/apis.py` & `abstra-1.0.0/abstra/widgets/apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import json
-import requests
-import urllib.request
-import urllib.response
+import json, requests, urllib.request, urllib.response, io
 
 
-def upload_file(file):
+def upload_file(file: io.IOBase):
     response = requests.post(
         "https://upload.abstra.cloud/hackerforms/upload",
         data=json.dumps({"filepath": file.name}),
         headers={"content-type": "application/json"},
     )
     response_json = json.loads(response.text)
```

### Comparing `abstra-0.9.0/abstra/widgets/file_utils.py` & `abstra-1.0.0/abstra/widgets/file_utils.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/AnswerSheetInput.py` & `abstra-1.0.0/abstra/widgets/library/AnswerSheetInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/CardsInput.py` & `abstra-1.0.0/abstra/widgets/library/CardsInput.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.label = label
         self.options = options
         self.multiple = kwargs.get("multiple", False)
         self.searchable = kwargs.get("searchable", False)
         self.initial_value = kwargs.get("initial_value", None)
         self.required = kwargs.get("required", True)
         self.hint = kwargs.get("hint", None)
-        self.columns = kwargs.get("columns", 1)
+        self.columns = kwargs.get("columns", 2)
         self.full_width = kwargs.get("full_width", False)
         self.layout = kwargs.get("layout", "list")
         self.disabled = kwargs.get("disabled", False)
 
     def json(self, **kwargs):
         return {
             "type": self.type,
```

### Comparing `abstra-0.9.0/abstra/widgets/library/CheckboxInput.py` & `abstra-1.0.0/abstra/widgets/library/CheckboxInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/ChecklistInput.py` & `abstra-1.0.0/abstra/widgets/library/ChecklistInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/ClickInput.py` & `abstra-1.0.0/abstra/widgets/library/ClickInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/CnpjInput.py` & `abstra-1.0.0/abstra/widgets/library/CnpjInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/CodeInput.py` & `abstra-1.0.0/abstra/widgets/library/CodeInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/CpfInput.py` & `abstra-1.0.0/abstra/widgets/library/CpfInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/CurrencyInput.py` & `abstra-1.0.0/abstra/widgets/library/CurrencyInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/DateInput.py` & `abstra-1.0.0/abstra/widgets/library/DateInput.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+import datetime, time, re
 from ..widget_base import Input
 from typing import Union, Optional
-import datetime
-import time
 
 
 class DateInput(Input):
     type = "date-input"
 
     def __init__(self, key: str, label: str, **kwargs):
         super().__init__(key)
@@ -13,42 +12,40 @@
         self.initial_value = kwargs.get("initial_value", None)
         self.required = kwargs.get("required", True)
         self.hint = kwargs.get("hint", None)
         self.columns = kwargs.get("columns", 1)
         self.full_width = kwargs.get("full_width", False)
         self.disabled = kwargs.get("disabled", False)
 
-    @staticmethod
-    def convert_value(value: Union[datetime.date, time.struct_time, str]) -> str:
-        if isinstance(value, datetime.date):
-            return value.isoformat()
-        elif isinstance(value, time.struct_time):
-            return (
-                datetime.datetime.fromtimestamp(time.mktime(value)).date().isoformat()
-            )
-        return value
-
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "hint": self.hint,
             "label": self.label,
-            "initialValue": DateInput.convert_value(self.initial_value)
-            if self.initial_value
-            else "",
+            "initialValue": DateInput.__revert_value(self.initial_value),
             "required": self.required,
             "columns": self.columns,
             "fullWidth": self.full_width,
             "disabled": self.disabled,
         }
 
     @staticmethod
-    def __revert_value(value: Union[datetime.date, time.struct_time, str]) -> str:
-        return DateInput.convert_value(value)
+    def __revert_value(
+        value: Optional[Union[datetime.date, time.struct_time, str]]
+    ) -> str:
+        if isinstance(value, datetime.date):
+            return value.isoformat()
+        if isinstance(value, time.struct_time):
+            return (
+                datetime.datetime.fromtimestamp(time.mktime(value)).date().isoformat()
+            )
+        if isinstance(value, str) and re.match("^\\d{4}-\\d{2}-\\d{2}$", value):
+            return value
+        return ""
 
     @staticmethod
     def __convert_answer(answer: str) -> Optional[datetime.date]:
         if not answer:
             return None
         try:
             split_answer = answer.split("T")[0].split("-")
```

### Comparing `abstra-0.9.0/abstra/widgets/library/DropdownInput.py` & `abstra-1.0.0/abstra/widgets/library/DropdownInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/EmailInput.py` & `abstra-1.0.0/abstra/widgets/library/EmailInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/FileInput.py` & `abstra-1.0.0/abstra/widgets/library/FileInput.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from io import IOBase
+from typing import Optional, Union, List
+from ..apis import upload_file
 from ..widget_base import Input
 from ..response_types import FileResponse
-from typing import Optional
 
 
 class FileInput(Input):
     type = "file-input"
 
     def __init__(self, key: str, label: str, **kwargs):
         super().__init__(key)
@@ -20,30 +22,46 @@
 
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "hint": self.hint,
             "label": self.label,
-            "initialValue": self.initial_value,
+            "initialValue": FileInput.__revert_value(self.initial_value),
             "required": self.required,
             "columns": self.columns,
             "multiple": self.multiple,
             "fullWidth": self.full_width,
             "disabled": self.disabled,
             "maxFileSize": self.max_file_size,
         }
 
     @staticmethod
-    def __revert_value(value) -> Optional[str]:
+    def __convert_value(value: Union[FileResponse, str, IOBase]) -> str:
+        if isinstance(value, FileResponse):
+            return value.url
+        if isinstance(value, str):
+            return value
+        if isinstance(value, IOBase):
+            return upload_file(value)
+        return ""
+
+    @staticmethod
+    def __revert_value(
+        value: Optional[
+            Union[
+                FileResponse, List[FileResponse], str, List[str], IOBase, List[IOBase]
+            ]
+        ]
+    ) -> Optional[str]:
         if not value:
             return None
         if isinstance(value, list):
-            return [item.url for item in value]
-        return value.url
+            return [FileInput.__convert_value(item) for item in value]
+        return FileInput.__convert_value(value)
 
     @staticmethod
     def __convert_answer(answer) -> Optional[FileResponse]:
         if not answer:
             return None
         if isinstance(answer, list):
             return [FileResponse(item) for item in answer]
```

### Comparing `abstra-0.9.0/abstra/widgets/library/FileOutput.py` & `abstra-1.0.0/abstra/widgets/library/FileOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/IframeOutput.py` & `abstra-1.0.0/abstra/widgets/library/IframeOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/ImageInput.py` & `abstra-1.0.0/abstra/widgets/library/ImageInput.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from io import IOBase
+from typing import Optional, Union, List
+from ..apis import upload_file
 from ..widget_base import Input
 from ..response_types import FileResponse
-from typing import Optional
 
 
 class ImageInput(Input):
     type = "image-input"
 
     def __init__(self, key: str, label: str, **kwargs):
         super().__init__(key)
@@ -20,30 +22,46 @@
 
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "hint": self.hint,
             "label": self.label,
-            "initialValue": self.initial_value,
+            "initialValue": ImageInput.__revert_value(self.initial_value),
             "columns": self.columns,
             "required": self.required,
             "multiple": self.multiple,
             "fullWidth": self.full_width,
             "disabled": self.disabled,
             "maxFileSize": self.max_file_size,
         }
 
     @staticmethod
-    def __revert_value(value) -> Optional[str]:
+    def __convert_value(value: Union[FileResponse, str, IOBase]) -> str:
+        if isinstance(value, FileResponse):
+            return value.url
+        if isinstance(value, str):
+            return value
+        if isinstance(value, IOBase):
+            return upload_file(value)
+        return ""
+
+    @staticmethod
+    def __revert_value(
+        value: Optional[
+            Union[
+                FileResponse, List[FileResponse], str, List[str], IOBase, List[IOBase]
+            ]
+        ]
+    ) -> Optional[str]:
         if not value:
             return None
         if isinstance(value, list):
-            return [item.url for item in value]
-        return value.url
+            return [ImageInput.__convert_value(item) for item in value]
+        return ImageInput.__convert_value(value)
 
     @staticmethod
     def __convert_answer(answer) -> Optional[FileResponse]:
         if not answer:
             return None
         if isinstance(answer, list):
             return [FileResponse(item) for item in answer]
```

### Comparing `abstra-0.9.0/abstra/widgets/library/ImageOutput.py` & `abstra-1.0.0/abstra/widgets/library/ImageOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/KanbanBoardInput.py` & `abstra-1.0.0/abstra/widgets/library/KanbanBoardInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/LinkOutput.py` & `abstra-1.0.0/abstra/widgets/library/LinkOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/ListInput.py` & `abstra-1.0.0/abstra/widgets/library/ListInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/MultipleChoiceInput.py` & `abstra-1.0.0/abstra/widgets/library/MultipleChoiceInput.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return {
             "type": self.type,
             "key": self.key,
             "label": self.label,
             "options": self.options,
             "hint": self.hint,
             "multiple": self.multiple,
-            "initialValue": self.initial_value or ([] if self.multiple else None),
+            "initialValue": self.initial_value,
             "required": self.required and not self.multiple,
             "columns": self.columns,
             "fullWidth": self.full_width,
             "min": self.min,
             "max": self.max,
             "disabled": self.disabled,
         }
```

### Comparing `abstra-0.9.0/abstra/widgets/library/NpsInput.py` & `abstra-1.0.0/abstra/widgets/library/NpsInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/NumberInput.py` & `abstra-1.0.0/abstra/widgets/library/NumberInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/NumberSliderInput.py` & `abstra-1.0.0/abstra/widgets/library/NumberSliderInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/PandasOutput.py` & `abstra-1.0.0/abstra/widgets/library/PandasOutput.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,23 @@
 
     def __init__(self, df: Any, **kwargs):
         self.df = df
         self.columns = kwargs.get("columns", 1)
         self.full_width = kwargs.get("full_width", False)
         self.display_index = kwargs.get("display_index", False)
         self.label = kwargs.get("label", None)
+        self.actions = kwargs.get("actions", [])
+        self.filterable = kwargs.get("filterable", False)
+        self.editable = kwargs.get("editable", False)
 
     def json(self, **kwargs):
         return {
             "type": self.type,
             "table": json.loads(self.df.to_json(orient="table")),
             "columns": self.columns,
             "fullWidth": self.full_width,
             "displayIndex": self.display_index,
             "label": self.label,
+            "actions": self.actions,
+            "filterable": self.filterable,
+            "editable": self.editable,
         }
```

### Comparing `abstra-0.9.0/abstra/widgets/library/PandasRowSelectionInput.py` & `abstra-1.0.0/abstra/widgets/library/PandasRowSelectionInput.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,30 @@
         self.hint = kwargs.get("hint", None)
         self.columns = kwargs.get("columns", 1)
         self.full_width = kwargs.get("full_width", False)
         self.display_index = kwargs.get("display_index", False)
         self.disabled = kwargs.get("disabled", False)
         self.label = kwargs.get("label", None)
         self.multiple = kwargs.get("multiple", True)
+        self.filterable = kwargs.get("filterable", False)
 
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "hint": self.hint,
             "table": json.loads(self.df.to_json(orient="table")),
             "required": self.required,
             "columns": self.columns,
             "fullWidth": self.full_width,
             "displayIndex": self.display_index,
             "disabled": self.disabled,
             "label": self.label,
             "multiple": self.multiple,
+            "filterable": self.filterable,
         }
 
     def convert_answer(self, answer) -> List:
         """
         Returns:
             list: The list of selected rows
         """
```

### Comparing `abstra-0.9.0/abstra/widgets/library/PasswordInput.py` & `abstra-1.0.0/abstra/widgets/library/PasswordInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/PhoneInput.py` & `abstra-1.0.0/abstra/widgets/library/PhoneInput.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..widget_base import Input
-from typing import Optional
+from typing import Optional, Union
 from ..response_types import PhoneResponse
 
 
 class PhoneInput(Input):
     type = "phone-input"
 
     def __init__(self, key: str, label: str, **kwargs):
@@ -13,60 +13,55 @@
         self.required = kwargs.get("required", True)
         self.hint = kwargs.get("hint", None)
         self.placeholder = kwargs.get("placeholder", "")
         self.columns = kwargs.get("columns", 1)
         self.full_width = kwargs.get("full_width", False)
         self.disabled = kwargs.get("disabled", False)
 
-    def _initial_value_to_json(self, initial_value):
-        if isinstance(initial_value, str):
-            return {"countryCode": "+1", "nationalNumber": initial_value}
-        return {
-            "countryCode": initial_value["country_code"]
-            if "country_code" in initial_value
-            else "",
-            "nationalNumber": initial_value["national_number"]
-            if "national_number" in initial_value
-            else "",
-        }
-
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "label": self.label,
-            "initialValue": self._initial_value_to_json(self.initial_value),
+            "initialValue": PhoneInput.__revert_value(self.initial_value),
             "placeholder": self.placeholder,
             "required": self.required,
             "hint": self.hint,
             "columns": self.columns,
             "fullWidth": self.full_width,
             "disabled": self.disabled,
         }
 
     @staticmethod
-    def __revert_value(value: Optional[PhoneResponse]):
-        if not value:
-            return None
-        return {
-            "raw": value.raw,
-            "masked": value.masked,
-            "countryCode": value.country_code,
-            "nationalNumber": value.national_number,
-        }
+    def __revert_value(value: Optional[Union[PhoneResponse, str, dict]]):
+        if isinstance(value, str):
+            return {"countryCode": None, "nationalNumber": value}
+        if isinstance(value, dict):
+            return {
+                "countryCode": value.get("country_code", ""),
+                "nationalNumber": value.get("national_number", ""),
+            }
+        if isinstance(value, PhoneResponse):
+            return {
+                "raw": value.raw,
+                "masked": value.masked,
+                "countryCode": value.country_code,
+                "nationalNumber": value.national_number,
+            }
+        return None
 
     @staticmethod
     def __convert_answer(answer) -> Optional[PhoneResponse]:
         if not answer:
             return None
         return PhoneResponse(
-            masked=answer["masked"],
-            raw=answer["raw"],
-            country_code=answer["countryCode"],
-            national_number=answer["nationalNumber"],
+            masked=answer.get("masked"),
+            raw=answer.get("raw"),
+            country_code=answer.get("countryCode"),
+            national_number=answer.get("nationalNumber"),
         )
 
     def convert_answer(self, answer) -> Optional[PhoneResponse]:
         """
         Returns:
             PhoneResponse: A dict containing the value entered by the user ({"raw": str, "masked": str})
         """
```

### Comparing `abstra-0.9.0/abstra/widgets/library/PlotlyOutput.py` & `abstra-1.0.0/abstra/widgets/library/PlotlyOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/ProgressOutput.py` & `abstra-1.0.0/abstra/widgets/library/ProgressOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/RatingInput.py` & `abstra-1.0.0/abstra/widgets/library/RatingInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/TagInput.py` & `abstra-1.0.0/abstra/widgets/library/TagInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/TextInput.py` & `abstra-1.0.0/abstra/widgets/library/TextInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/TextareaInput.py` & `abstra-1.0.0/abstra/widgets/library/TextareaInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/library/TimeInput.py` & `abstra-1.0.0/abstra/widgets/library/TimeInput.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import datetime, re
 from ..widget_base import Input
-import datetime
-from typing import Optional
+from typing import Optional, Union
 
 
 class TimeInput(Input):
     type = "time-input"
 
     def __init__(self, key: str, label: str, **kwargs):
         super().__init__(key)
@@ -20,24 +20,33 @@
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "label": self.label,
             "format": self.format,
             "hint": self.hint,
-            "initialValue": self.initial_value,
+            "initialValue": TimeInput.__revert_value(self.initial_value),
             "required": self.required,
             "columns": self.columns,
             "fullWidth": self.full_width,
             "disabled": self.disabled,
         }
 
     @staticmethod
-    def __revert_value(value: Optional[datetime.time]):
-        return {"hour": value.hour, "minute": value.minute} if value else None
+    def __revert_value(
+        value: Optional[Union[datetime.time, str, dict]]
+    ) -> Optional[dict]:
+        if isinstance(value, str) and re.match("^\\d{2}:\\d{2}$", value):
+            return {
+                "hour": int(value.split(":")[0]),
+                "minute": int(value.split(":")[1]),
+            }
+        if isinstance(value, datetime.time):
+            return {"hour": value.hour, "minute": value.minute}
+        return None
 
     @staticmethod
     def __convert_answer(answer) -> Optional[datetime.time]:
         return datetime.time(answer["hour"], answer["minute"]) if answer else None
 
     def convert_answer(self, answer) -> Optional[datetime.time]:
         """
```

### Comparing `abstra-0.9.0/abstra/widgets/library/ToggleInput.py` & `abstra-1.0.0/abstra/widgets/library/ToggleInput.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..widget_base import Input
-from typing import Dict
+from typing import Optional, Union
 
 
 class ToggleInput(Input):
     type = "toggle-input"
 
     def __init__(self, key: str, label: str, **kwargs):
         super().__init__(key)
@@ -20,25 +20,27 @@
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "label": self.label,
             "onText": self.on_text,
             "offText": self.off_text,
-            "initialValue": self.initial_value,
+            "initialValue": ToggleInput.__revert_value(self.initial_value),
             "required": self.required,
             "hint": self.hint,
             "columns": self.columns,
             "fullWidth": self.full_width,
             "disabled": self.disabled,
         }
 
     @staticmethod
-    def __revert_value(value: bool) -> str:
-        return "1" if value == True else "0"
+    def __revert_value(value: Optional[Union[bool, str]]) -> str:
+        if value == "1" or value == True:
+            return "1"
+        return "0"
 
     @staticmethod
     def __convert_answer(answer: str) -> str:
         return True if answer == "1" else False
 
     def convert_answer(self, answer: str) -> str:
         return self.__convert_answer(answer)
```

### Comparing `abstra-0.9.0/abstra/widgets/library/VideoInput.py` & `abstra-1.0.0/abstra/widgets/library/VideoInput.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from io import IOBase
+from typing import Optional, Union, List
+from ..apis import upload_file
 from ..widget_base import Input
-from typing import Optional
 from ..response_types import FileResponse
 
 
 class VideoInput(Input):
     type = "video-input"
 
     def __init__(self, key: str, label: str, **kwargs):
@@ -20,38 +22,46 @@
 
     def json(self, **kwargs):
         return {
             "type": self.type,
             "key": self.key,
             "hint": self.hint,
             "label": self.label,
-            "initialValue": self.initial_value,
+            "initialValue": VideoInput.__revert_value(self.initial_value),
             "columns": self.columns,
             "required": self.required,
             "multiple": self.multiple,
             "fullWidth": self.full_width,
             "disabled": self.disabled,
             "maxFileSize": self.max_file_size,
         }
 
     @staticmethod
-    def __revert_value(value) -> Optional[str]:
-        if not value:
-            return None
-        if isinstance(value, list):
-            return [item.url for item in value]
-        return value.url
+    def __convert_value(value: Union[FileResponse, str, IOBase]) -> str:
+        if isinstance(value, FileResponse):
+            return value.url
+        if isinstance(value, str):
+            return value
+        if isinstance(value, IOBase):
+            return upload_file(value)
+        return ""
 
     @staticmethod
-    def __convert_answer(answer) -> Optional[FileResponse]:
-        if not answer:
+    def __revert_value(
+        value: Optional[
+            Union[
+                FileResponse, List[FileResponse], str, List[str], IOBase, List[IOBase]
+            ]
+        ]
+    ) -> Optional[str]:
+        if not value:
             return None
-        if isinstance(answer, list):
-            return [FileResponse(item) for item in answer]
-        return FileResponse(answer)
+        if isinstance(value, list):
+            return [VideoInput.__convert_value(item) for item in value]
+        return VideoInput.__convert_value(value)
 
     def convert_answer(self, answer) -> Optional[FileResponse]:
         """
         Returns:
             FileResponse or FileResponse[]: A dict containing the video uploaded by the user ({"file": file, "url": str, "content": bytes}) or a list of videos in case of multiple flag set as True
         """
         return self.__convert_answer(answer)
```

### Comparing `abstra-0.9.0/abstra/widgets/library/__init__.py` & `abstra-1.0.0/abstra/widgets/library/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from .TextareaInput import TextareaInput
 from .ListInput import ListInput
+from .CustomInput import CustomInput
 from .VideoInput import VideoInput
 from .TagInput import TagInput
 from .PandasOutput import PandasOutput
 from .TimeInput import TimeInput
+from .RichTextInput import RichTextInput
 from .NumberSliderInput import NumberSliderInput
 from .CheckboxInput import CheckboxInput
 from .CnpjInput import CnpjInput
 from .ProgressOutput import ProgressOutput
 from .CpfInput import CpfInput
 from .TextInput import TextInput
 from .PhoneInput import PhoneInput
```

### Comparing `abstra-0.9.0/abstra/widgets/metadata.py` & `abstra-1.0.0/abstra/widgets/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 200,
             "minHeight": 350,
             "initialWidth": 200,
             "initialHeight": 350,
         },
         "pythonAPI": {
@@ -54,14 +55,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -78,14 +80,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list: The values/value selected by the user",
                 }
             ],
@@ -133,14 +143,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -168,46 +179,58 @@
             }
         ],
     },
     "cards-input": {
         "name": "Card display",
         "description": "Read a text value from the user simple text input",
         "type": "cards-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
-            }
+            },
+            {
+                "key": "card-click",
+                "description": "Function or expression to be run when a card is clicked",
+                "payloadSchema": [
+                    {
+                        "key": "card",
+                        "typeName": "Object",
+                        "description": "The card that was clicked",
+                    }
+                ],
+            },
         ],
         "dashProperties": {
-            "minWidth": 530,
-            "minHeight": 352,
-            "initialWidth": 530,
-            "initialHeight": 712,
+            "minWidth": 200,
+            "minHeight": 200,
+            "initialWidth": 400,
+            "initialHeight": 350,
         },
         "pythonAPI": {
             "name": "read_cards",
             "params": [
                 {
                     "argName": "label",
-                    "description": "The text related to this field",
+                    "description": "The text related to this input",
                     "typeName": "str",
                     "isKwarg": False,
                     "default": None,
                     "dashesInitialValue": '"Card Title"',
                 },
                 {
                     "argName": "options",
                     "description": "The options to display to the user, eg. [\n{'title': 'Option 1', 'subtitle': 'Subtitle 1', 'image': 'https://image_1.png', 'description': 'option 1 description', 'topLeftExtra': 'Left 1', 'topRightExtra': 'Right 1' },\n{'title': 'Option 2', 'subtitle': 'Subtitle 2', 'image': 'https://image_2.png', 'description': 'option 2 description', 'topLeftExtra': 'Left 2', 'topRightExtra': 'Right 2' }]",
                     "typeName": "list",
                     "typeDescription": ["list[AbstraCard]"],
                     "isKwarg": False,
                     "default": None,
-                    "dashesInitialValue": '[\n          {\n            "title": "Option 1",\n            "subtitle": "Subtitle 1",\n            "image": "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Mona_Lisa.jpg/396px-Mona_Lisa.jpg",\n            "description": "option 1 description",\n            "topLeftExtra": "Left 1",\n            "topRightExtra": "Right 1",\n          },\n          {\n            "title": "Option 2",\n            "subtitle": "Subtitle 2",\n            "image": "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Mona_Lisa.jpg/396px-Mona_Lisa.jpg",\n            "description": "option 2 description",\n            "topLeftExtra": "Left 2",\n            "topRightExtra": "Right 2",\n          },\n        ]',
+                    "dashesInitialValue": '[\n          {\n            "title": "Option 1",\n            "subtitle": "Subtitle 1",\n            "image": "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Mona_Lisa.jpg/396px-Mona_Lisa.jpg",\n            "description": "option 1 description",\n            "topLeftExtra": "Left 1",\n            "topRightExtra": "Right 1",\n          }\n        ]',
                 },
                 {
                     "argName": "multiple",
                     "description": "Whether the user can select multiple options. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
@@ -226,34 +249,42 @@
                     "description": "Whether to show a search bar. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                 },
                 {
                     "argName": "layout",
-                    "description": "Whether the cards layout should be 'list' or 'grid'. Defaults to 'list'.%%%",
+                    "description": "Whether the cards layout should be 'list' or 'grid'. Defaults to 'list'. The 'grid' only applies to desktop resolutions.",
                     "typeName": "str",
                     "typeDescription": ["str ('list', 'grid')"],
                     "isKwarg": True,
                     "default": "'list'",
                 },
                 {
+                    "argName": "columns",
+                    "typeName": "int",
+                    "description": "When layout is 'grid', how many columns to display",
+                    "isKwarg": True,
+                    "default": "2",
+                },
+                {
                     "argName": "disabled",
                     "description": "whether the input is disabled. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                 },
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -270,14 +301,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list, any: The options/option selected by the user",
                 }
             ],
@@ -368,20 +407,27 @@
                         ],
                         "default": None,
                     },
                 },
                 {
                     "argName": "layout",
                     "typeName": "string",
-                    "description": "Whether the cards layout should be 'list' or 'grid'",
+                    "description": "Whether the cards layout should be 'list' or 'grid'. Defaults to 'list'. The 'grid' only applies to desktop resolutions.",
                     "oneOf": ["list", "grid"],
                     "default": "list",
                     "isOptional": True,
                 },
                 {
+                    "argName": "columns",
+                    "typeName": "number",
+                    "description": "When layout is 'grid', how many columns to display",
+                    "isOptional": True,
+                    "default": "2",
+                },
+                {
                     "argName": "key",
                     "typeName": "string",
                     "description": "The key of the input on the returning object",
                 },
                 {
                     "argName": "disabled",
                     "typeName": "boolean",
@@ -403,20 +449,14 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
-                },
-                {
-                    "argName": "columns",
-                    "typeName": "number",
-                    "description": "number of columns this input will take",
-                    "isOptional": True,
                     "formOnly": True,
                 },
                 {
                     "argName": "fullWidth",
                     "typeName": "boolean",
                     "description": "Whether the widget should take up the full width of the page",
                     "isOptional": True,
@@ -462,14 +502,15 @@
             }
         ],
     },
     "checkbox-input": {
         "name": "Checkbox",
         "description": "Allow users to select an option by interacting with a checkbox",
         "type": "checkbox-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -508,14 +549,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -532,14 +574,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list(str) or list(float): The value entered by the user",
                 }
             ],
@@ -585,14 +635,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -641,14 +692,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 60,
             "minHeight": 32,
             "initialWidth": 222,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -689,14 +741,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -713,14 +766,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list or any: The value entered by the user",
                 }
             ],
@@ -786,14 +847,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -851,14 +913,15 @@
             },
         ],
     },
     "click-input": {
         "name": "Button",
         "description": "Buttons allow users to trigger actions.",
         "type": "click-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "click",
                 "description": "Function or expression to be run when the button is clicked",
                 "payloadSchema": [],
             }
         ],
@@ -890,14 +953,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -906,14 +970,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list(str) or list(float): The value entered by the user",
                 }
             ],
@@ -944,14 +1016,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -972,17 +1045,18 @@
                 "description": "The following example demonstrate some of the available functionality for read_click",
                 "key": "example1",
                 "code": "",
             }
         ],
     },
     "cnpj-input": {
-        "name": "CNPJ field",
+        "name": "CNPJ input",
         "description": "Allow users to insert a CNPJ number into the app.",
         "type": "cnpj-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -1030,14 +1104,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -1054,14 +1129,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list(str) or list(float): The value entered by the user",
                 }
             ],
@@ -1106,14 +1189,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -1140,17 +1224,18 @@
                 "description": "The following example demonstrate some of the available functionality for read_cnpj",
                 "key": "example1",
                 "code": 'from hackerforms import read_cnpj\n\nname = read_cnpj("Insert your CNPJ below")\n',
             }
         ],
     },
     "code-input": {
-        "name": "Code field",
-        "description": "Code field allow users to insert code and reads it.",
+        "name": "Code input",
+        "description": "Code input allow users to insert code and reads it.",
         "type": "code-input",
+        "autoHeight": False,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -1196,14 +1281,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -1220,14 +1306,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "str", "typeDescription": "The value entered by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -1275,14 +1369,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -1307,24 +1402,25 @@
                 "description": "The following example demonstrate some of the available functionality for read_code",
                 "key": "example1",
                 "code": 'from hackerforms import read_code\n\nans = read_code("Show me the code!", language="c")\n',
             }
         ],
     },
     "cpf-input": {
-        "name": "CPF field",
+        "name": "CPF input",
         "description": "Allow users to insert a CPF number into the app.",
         "type": "cpf-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 222,
             "minHeight": 70,
             "initialWidth": 222,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -1365,14 +1461,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -1389,14 +1486,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "str", "typeDescription": "The value entered by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -1438,14 +1543,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -1472,24 +1578,25 @@
                 "description": "The following example demonstrate some of the available functionality for read_cpf",
                 "key": "example1",
                 "code": 'from hackerforms import read_cpf\n\nname = read_cpf("Insert your CPF below")\n',
             }
         ],
     },
     "currency-input": {
-        "name": "Currency field",
-        "description": "Currency field allows users to enter monetary values.",
+        "name": "Currency input",
+        "description": "Currency input allows users to enter monetary values.",
         "type": "currency-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 100,
             "minHeight": 72,
             "initialWidth": 300,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -1556,14 +1663,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -1580,14 +1688,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "float",
                     "typeDescription": "The value entered by the user",
                 }
             ],
@@ -1655,14 +1771,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -1692,25 +1809,198 @@
                 "name": "Basic Example",
                 "description": "The following example demonstrate some of the available functionality for read_currency",
                 "key": "example1",
                 "code": 'from hackerforms import read_currency\n\nread_currency(\n    f"How many credits do you want?", currency="USD", initial_value=10, min=10\n)\n',
             }
         ],
     },
+    "custom-input": {
+        "type": "custom-input",
+        "name": "Custom widget",
+        "description": "Widget with customizable UI and behaviour",
+        "autoHeight": False,
+        "events": [
+            {
+                "key": "custom-event",
+                "description": "Function or expression to be run when custom event is triggered",
+                "payloadSchema": [],
+            },
+            {
+                "key": "change",
+                "description": "Function or expression to be run when the input value changes",
+                "payloadSchema": [],
+            },
+        ],
+        "dashProperties": {
+            "minWidth": 65,
+            "minHeight": 30,
+            "initialWidth": 146,
+            "initialHeight": 32,
+        },
+        "pythonAPI": {
+            "name": "read_custom",
+            "params": [
+                {
+                    "argName": "html_body",
+                    "description": "The HTML body content",
+                    "typeName": "str",
+                    "typeDescription": ["str (HTML snippet)"],
+                    "isKwarg": False,
+                    "default": None,
+                    "dashesInitialValue": '"<h1>Hello World</h1>"',
+                },
+                {
+                    "argName": "initial_value",
+                    "description": "The initial value to be stored in custom widget state.",
+                    "typeName": "Any",
+                    "isKwarg": True,
+                    "default": None,
+                    "formOnly": True,
+                },
+                {
+                    "argName": "label",
+                    "description": "The label to display to the user",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": None,
+                },
+                {
+                    "argName": "html_head",
+                    "description": "The HTML head content",
+                    "typeName": "str",
+                    "typeDescription": ["str (HTML snippet)"],
+                    "isKwarg": True,
+                    "default": None,
+                    "dashesInitialValue": '""',
+                },
+                {
+                    "argName": "css",
+                    "description": "The widget's CSS",
+                    "typeName": "str",
+                    "typeDescription": ["str (CSS snippet)"],
+                    "isKwarg": True,
+                    "default": None,
+                    "dashesInitialValue": '"h1 { color: red; }"',
+                },
+                {
+                    "argName": "js",
+                    "description": "The widget's JavaScript",
+                    "typeName": "str",
+                    "typeDescription": ["str (JavaScript snippet)"],
+                    "isKwarg": True,
+                    "default": None,
+                    "dashesInitialValue": "\"console.log('Hello World')\"",
+                },
+                {
+                    "argName": "full_width",
+                    "description": "Whether the input should use full screen width. Defaults to False.",
+                    "typeName": "bool",
+                    "isKwarg": True,
+                    "default": "False",
+                    "formOnly": True,
+                },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
+            ],
+            "returns": [
+                {"typeName": None, "typeDescription": "any: The custom response"}
+            ],
+        },
+        "brokerAPI": {
+            "params": [
+                {
+                    "argName": "label",
+                    "typeName": "string",
+                    "description": "The label to display to the user",
+                    "isOptional": True,
+                },
+                {
+                    "argName": "initialValue",
+                    "typeName": "any",
+                    "description": "The initial value to be stored in custom widget state.",
+                    "default": None,
+                    "isOptional": True,
+                },
+                {
+                    "argName": "htmlHead",
+                    "typeName": "string",
+                    "description": "The HTML head content",
+                    "isOptional": True,
+                },
+                {
+                    "argName": "htmlBody",
+                    "typeName": "string",
+                    "description": "The HTML body content",
+                },
+                {
+                    "argName": "css",
+                    "typeName": "string",
+                    "description": "The widget's CSS",
+                    "isOptional": True,
+                },
+                {
+                    "argName": "js",
+                    "typeName": "string",
+                    "description": "The widget's JavaScript",
+                    "isOptional": True,
+                },
+                {
+                    "argName": "key",
+                    "typeName": "string",
+                    "description": "The key of the input on the returning object",
+                },
+                {
+                    "argName": "columns",
+                    "typeName": "number",
+                    "description": "number of columns this input will take",
+                    "isOptional": True,
+                    "formOnly": True,
+                },
+                {
+                    "argName": "fullWidth",
+                    "typeName": "boolean",
+                    "description": "Whether the widget should take up the full width of the page",
+                    "isOptional": True,
+                    "formOnly": True,
+                },
+            ]
+        },
+        "examples": [
+            {
+                "props": {
+                    "htmlBody": "<button id='date-btn'>Get current date</button>",
+                    "js": "document.getElementById('date-btn').addEventListener('click',function() {\n    const date = new Date();\n    const day = date.getDate();\n    const month = date.getMonth() + 1;\n    const year = date.getFullYear();\n\n    changeEvent(day + '/' + month + '/' + year);\n});",
+                    "css": "body {\n    margin: 0;\n    padding: 0;\n}\n\n#date-btn {\n    cursor: pointer;\n    background-color: #343b46;\n    border: none;\n    border-radius: 4px;\n    color: white;\n    padding: 15px 32px;\n    text-align: center;\n    text-decoration: none;\n    display: inline-block;\n    font-size: 16px;\n}\n\n#date-btn:hover {\n    background-color: #3e4756;\n}",
+                    "label": "Custom Widget",
+                },
+                "name": "Basic Example",
+                "description": "The following example shows how to create a custom widget with a button that returns the current date.",
+                "key": "example1",
+                "code": 'from hackerforms import read_custom\n\ncurrent_date = read_custom(\n    "<button id=\'date-btn\'>Get current date</button>",\n    label="Custom Widget",\n    js="""\n    document.getElementById(\'date-btn\').addEventListener(\'click\',function() {\n        const date = new Date();\n        const day = date.getDate();\n        const month = date.getMonth() + 1;\n        const year = date.getFullYear();\n\n        changeEvent(day + \'/\' + month + \'/\' + year);\n    });\n    """,\n    css="""\n    body {\n        margin: 0;\n        padding: 0;\n    }\n\n    #date-btn {\n        cursor: pointer;\n        background-color: #343b46;\n        border: none;\n        border-radius: 4px;\n        color: white;\n        padding: 15px 32px;\n        text-align: center;\n        text-decoration: none;\n        display: inline-block;\n        font-size: 16px;\n    }\n\n    #date-btn:hover {\n        background-color: #3e4756;\n    }\n    """,\n)\n',
+            }
+        ],
+    },
     "date-input": {
         "name": "Date picker input",
         "description": "Allow users to select  a date, or a range of dates.*",
         "type": "date-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 200,
             "minHeight": 72,
             "initialWidth": 300,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -1747,14 +2037,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -1771,14 +2062,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "datetime.date",
                     "typeDescription": "The value entered by the user",
                 }
             ],
@@ -1822,14 +2121,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -1853,14 +2153,15 @@
             }
         ],
     },
     "dropdown-input": {
         "name": "Dropdown",
         "description": "Allow users to select one or more options by selecting items in a dropdown",
         "type": "dropdown-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -1922,14 +2223,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -1946,14 +2248,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "str", "typeDescription": "The value selected by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -1995,14 +2305,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -2067,24 +2378,25 @@
                 "description": "Use a dictionary to specify the label and value of each option. The label will be displayed to the user, and the value will be returned by the widget.",
                 "key": "example2",
                 "code": 'from hackerforms import read_dropdown\n\nans = read_dropdown(\n    "Choose a color",\n    [\n        {"label": "Red", "value": "R"},\n        {"label": "Green", "value": "G"},\n        {"label": "Blue", "value": "B"},\n    ],\n)\n# ans = "R", "G" or "B"\n',
             },
         ],
     },
     "email-input": {
-        "name": "Email field",
-        "description": "Email field allow users to enter a valid email address.",
+        "name": "Email input",
+        "description": "Email input allow users to enter a valid email address.",
         "type": "email-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 220,
             "minHeight": 60,
             "initialWidth": 223,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -2130,14 +2442,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -2154,14 +2467,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "str", "typeDescription": "The value entered by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -2209,14 +2530,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -2245,14 +2567,15 @@
             }
         ],
     },
     "file-input": {
         "name": "File upload area",
         "description": "File upload adds a drop-area for users to upload one or more files",
         "type": "file-input",
+        "autoHeight": False,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -2305,14 +2628,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -2329,14 +2653,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "Union[FileResponse, List[FileResponse]]",
                     "typeDescription": "A dict containing the file uploaded by the user FileResponse(file: TemporaryFile, url: str, content: bytes) or a list of FileResponses in case of multiple flag set as True. ⚠️ The url expires after 48 hours",
                 }
             ],
@@ -2346,15 +2678,15 @@
                 {
                     "argName": "label",
                     "typeName": "string",
                     "description": "The label to display above the input",
                 },
                 {
                     "argName": "initialValue",
-                    "typeName": ["string", "array"],
+                    "typeName": ["string", "array", "null"],
                     "description": "The initial value of the input",
                     "default": "",
                 },
                 {
                     "argName": "multiple",
                     "description": "Whether the user will be allowed to upload multiple files. Defaults to False.",
                     "typeName": "boolean",
@@ -2392,14 +2724,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -2415,29 +2748,37 @@
         },
         "examples": [
             {
                 "props": {"label": "Upload your .xlsx file"},
                 "name": "Basic Example",
                 "description": "The following example demonstrate some of the available functionality for read_file",
                 "key": "example1",
-                "code": 'from hackerforms import read_file\n\nfileResponse = read_file("Upload your .xlsx file")\nfile = fileResponse.file  # File object\nurl = fileResponse.url  # Url to the file\ncontent = fileResponse.content  # Raw file content\n',
-            }
+                "code": 'from hackerforms import read_file\n\nfile_response = read_file("Upload your .xlsx file")\nfile = file_response.file  # File object\n',
+            },
+            {
+                "props": {"label": "Upload your file"},
+                "name": "Saving file to a directory on Files storage",
+                "description": "This example shows how to save a file to a directory on Files",
+                "key": "example2",
+                "code": 'from hackerforms import read_file\nimport shutil, os\n\nfile_response = read_file("Upload your file")\n\ndestination_dir = "foo/bar/"\n# Creates directory if it does not exist\nos.makedirs(destination_dir, exist_ok=True)\n\n# Copies file to destination directory\nshutil.copy(file_response.file.name, destination_dir + file_response.name)\n',
+            },
         ],
     },
     "image-input": {
         "name": "Image upload",
         "description": "Image upload adds a drop-area for users to upload one or more image files.",
         "type": "image-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": False,
         "dashProperties": {
             "minWidth": 150,
             "minHeight": 112,
             "initialWidth": 223,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -2483,14 +2824,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -2507,14 +2849,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "Union[FileResponse, List[FileResponse]]",
                     "typeDescription": 'A dict containing the image file uploaded by the user ({"file": file, "url": str, "content": bytes}) or a list of images in case of multiple flag set as True',
                 }
             ],
@@ -2566,14 +2916,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -2595,24 +2946,25 @@
         },
         "examples": [
             {
                 "props": {"label": "Upload your .png image"},
                 "name": "Basic Example",
                 "description": "The following example demonstrate some of the available functionality for read_image",
                 "key": "example1",
-                "code": 'from hackerforms import read_image\n\nfileResponse = read_image("Upload your .png image")\nfile = fileResponse.file  # File object\nurl = fileResponse.url  # Url to the file\ncontent = fileResponse.content  # Raw file content\n',
+                "code": 'from hackerforms import read_image\n\nfile_response = read_image("Upload your .png image")\nfile = file_response.file  # File object\n',
             }
         ],
     },
     "kanban-board-input": {
         "name": "Kanban board",
         "description": "Kanban board",
         "type": "kanban-board-input",
         "dashOnly": True,
         "events": [],
+        "autoHeight": False,
         "dashProperties": {
             "minWidth": 300,
             "minHeight": 500,
             "initialWidth": 500,
             "initialHeight": 500,
         },
         "pythonAPI": {
@@ -2679,14 +3031,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -2779,14 +3132,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 146,
             "minHeight": 32,
             "initialWidth": 146,
             "initialHeight": 32,
         },
         "pythonAPI": {
@@ -2845,14 +3199,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -2869,14 +3224,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "list",
                     "typeDescription": "The values entered by the user",
                 }
             ],
@@ -2943,14 +3306,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -3005,14 +3369,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 60,
             "minHeight": 70,
             "initialWidth": 223,
             "initialHeight": 152,
         },
         "pythonAPI": {
@@ -3074,14 +3439,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -3098,14 +3464,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list or any: The values/value selected by the user",
                 }
             ],
@@ -3172,14 +3546,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -3254,14 +3629,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 120,
             "minHeight": 60,
             "initialWidth": 608,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -3322,14 +3698,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -3346,14 +3723,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "int", "typeDescription": "The value entered by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -3422,14 +3807,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -3454,24 +3840,25 @@
                 "description": "The following example demonstrate some of the available functionality for read_nps",
                 "key": "example1",
                 "code": 'from hackerforms import read_nps\n\nans = read_nps(\n    "How likely are you to recommend Abstra Cloud?",\n    min_hint="No way!",\n    max_hint="Hell yeah!",\n)\n',
             }
         ],
     },
     "number-input": {
-        "name": "Number field",
-        "description": "Number field allow users to enter numeric values.",
+        "name": "Number input",
+        "description": "Number input allow users to enter numeric values.",
         "type": "number-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 120,
             "minHeight": 60,
             "initialWidth": 223,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -3531,14 +3918,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -3555,14 +3943,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "float",
                     "typeDescription": "The value entered by the user",
                 }
             ],
@@ -3624,14 +4020,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -3668,14 +4065,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 120,
             "minHeight": 30,
             "initialWidth": 223,
             "initialHeight": 72,
         },
         "pythonAPI": {
@@ -3728,14 +4126,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -3752,14 +4151,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "float",
                     "typeDescription": "The value entered by the user",
                 }
             ],
@@ -3821,14 +4228,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -3859,14 +4267,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": False,
         "dashProperties": {
             "minWidth": 195,
             "minHeight": 72,
             "initialWidth": 245,
             "initialHeight": 72,
         },
         "pythonAPI": {
@@ -3911,14 +4320,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -3935,14 +4345,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "list", "typeDescription": "The list of selected rows"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -4004,14 +4422,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -4053,24 +4472,25 @@
                 "description": "The following example demonstrate some of the available functionality for read_pandas",
                 "key": "example1",
                 "code": 'from hackerforms import read_pandas_row_selection\nimport pandas as pd\n\ndata = [\n    {"Country": "USA", "Population": "32,700,000"},\n    {"Country": "China", "Population": "1,300,000,000"},\n    {"Country": "Japan", "Population": "126,000,000"},\n]\ndf = pd.DataFrame(data)\nread_pandas_row_selection(df)\n',
             }
         ],
     },
     "password-input": {
-        "name": "Password field",
+        "name": "Password input",
         "type": "password-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
-        "description": "Password field allow users to enter a password before seen the content.",
+        "autoHeight": True,
+        "description": "Password input allow users to enter a password before seen the content.",
         "dashProperties": {
             "minWidth": 120,
             "minHeight": 60,
             "initialWidth": 223,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -4168,14 +4588,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -4192,14 +4613,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "str", "typeDescription": "The value entered by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -4270,15 +4699,15 @@
                     "description": "Allow the user's password manager to automatically enter the password",
                     "default": "current-password",
                     "isOptional": True,
                 },
                 {
                     "argName": "secret",
                     "typeName": "boolean",
-                    "description": "Read-only field that indicates whether the widget response value is secret.",
+                    "description": "Read-only input that indicates whether the widget response value is secret.",
                     "default": True,
                     "isOptional": True,
                 },
                 {
                     "argName": "key",
                     "typeName": "string",
                     "description": "The key of the input on the returning object",
@@ -4304,14 +4733,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -4337,17 +4767,18 @@
                 "description": "The following example demonstrate some of the available functionality for read_password",
                 "key": "example1",
                 "code": 'from hackerforms import read_password\n\nans = read_password("Insert your password below")\n',
             }
         ],
     },
     "phone-input": {
-        "name": "Phone field",
-        "description": "Phone field allow users to enter a valid phone number.",
+        "name": "Phone input",
+        "description": "Phone input allow users to enter a valid phone number.",
         "type": "phone-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -4367,16 +4798,18 @@
                     "isKwarg": False,
                     "default": None,
                     "dashesInitialValue": '"Insert a phone number."',
                 },
                 {
                     "argName": "initial_value",
                     "description": "The initial value to display to the user. If dictionary, it contains two keys: 'country_code' (string with optional + sign or number) and 'national_number' (str or number). Ex: {'country_code': '+55', 'national_number': '21999990000'}. Defaults to \"\".",
-                    "typeName": "Union[str, dict]",
-                    "typeDescription": ["str (000000000000)", "AbstraPhone"],
+                    "typeName": "dict",
+                    "typeDescription": [
+                        'dict ({"country_code": str, "national_number": str})'
+                    ],
                     "isKwarg": True,
                     "default": '""',
                     "formOnly": True,
                 },
                 {
                     "argName": "placeholder",
                     "description": 'The placeholder text to display to the user. Defaults to "".',
@@ -4394,14 +4827,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -4418,14 +4852,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "PhoneResponse",
                     "typeDescription": 'A dict containing the value entered by the user ({"raw": str, "masked": str})',
                 }
             ],
@@ -4481,14 +4923,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -4525,14 +4968,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 120,
             "minHeight": 60,
             "initialWidth": 223,
             "initialHeight": 72,
         },
         "pythonAPI": {
@@ -4579,14 +5023,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -4603,14 +5048,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "float",
                     "typeDescription": "The value entered by the user",
                 }
             ],
@@ -4669,14 +5122,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -4707,17 +5161,195 @@
                 "name": "Custom chars and number of points",
                 "description": "The following example demonstrate some of the available functionality for read_rating",
                 "key": "example2",
                 "code": 'from hackerforms import read_rating\n\nrating = read_rating("How do you evaluate your Python skills?", char="🐍", max=3)\n',
             },
         ],
     },
+    "rich-text-input": {
+        "name": "Rich text input",
+        "type": "rich-text-input",
+        "events": [
+            {
+                "key": "change",
+                "description": "Function or expression to be run when the input value changes",
+                "payloadSchema": [],
+            }
+        ],
+        "description": "Rich text input allows users to type and format textual content.",
+        "autoHeight": False,
+        "dashProperties": {
+            "minWidth": 100,
+            "minHeight": 100,
+            "initialWidth": 200,
+            "initialHeight": 150,
+        },
+        "pythonAPI": {
+            "name": "read_richtext",
+            "params": [
+                {
+                    "argName": "label",
+                    "description": "The label to display to the user",
+                    "typeName": "str",
+                    "isKwarg": False,
+                    "default": None,
+                    "dashesInitialValue": '"Insert your rich text here!"',
+                },
+                {
+                    "argName": "initial_value",
+                    "description": 'The initial value to display to the user. Defaults to "".',
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": '""',
+                    "formOnly": True,
+                },
+                {
+                    "argName": "placeholder",
+                    "description": 'The placeholder text to display to the user. Defaults to "Your rich text here".',
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": '"Your rich text here"',
+                },
+                {
+                    "argName": "disabled",
+                    "description": "whether the input is disabled. Defaults to False.",
+                    "typeName": "bool",
+                    "isKwarg": True,
+                    "default": "False",
+                },
+                {
+                    "argName": "required",
+                    "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
+                    "typeName": "Union[bool, str]",
+                    "typeDescription": ["bool", "str"],
+                    "isKwarg": True,
+                    "default": "True",
+                    "formOnly": True,
+                },
+                {
+                    "argName": "hint",
+                    "description": "A tooltip displayed to the user. Defaults to None.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "None",
+                },
+                {
+                    "argName": "end_program",
+                    "description": "Whether the program should end after the widget is shown. Defaults to False.",
+                    "typeName": "bool",
+                    "isKwarg": True,
+                    "default": "False",
+                    "formOnly": True,
+                },
+                {
+                    "argName": "full_width",
+                    "description": "Whether the input should use full screen width. Defaults to False.",
+                    "typeName": "bool",
+                    "isKwarg": True,
+                    "default": "False",
+                    "formOnly": True,
+                },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
+            ],
+            "returns": [
+                {
+                    "typeName": "str",
+                    "typeDescription": "The rich text value entered by the user",
+                }
+            ],
+        },
+        "brokerAPI": {
+            "params": [
+                {
+                    "argName": "label",
+                    "typeName": "string",
+                    "description": "The label of the input",
+                },
+                {
+                    "argName": "initialValue",
+                    "typeName": "string",
+                    "description": "The initial value of the input",
+                    "default": "",
+                    "isOptional": True,
+                },
+                {
+                    "argName": "key",
+                    "typeName": "string",
+                    "description": "The key of the input on the returning object",
+                },
+                {
+                    "argName": "disabled",
+                    "typeName": "boolean",
+                    "description": "Whether the input is disabled",
+                },
+                {
+                    "argName": "hint",
+                    "typeName": ["string", "null"],
+                    "description": "message describing the input",
+                    "default": None,
+                    "isOptional": True,
+                },
+                {
+                    "argName": "end_program",
+                    "typeName": ["boolean", "null"],
+                    "description": "End program after this widget is shown",
+                    "default": False,
+                    "isOptional": True,
+                },
+                {
+                    "argName": "required",
+                    "typeName": ["boolean", "string"],
+                    "description": "Whether the input is required or not",
+                    "default": True,
+                    "isOptional": True,
+                    "formOnly": True,
+                },
+                {
+                    "argName": "columns",
+                    "typeName": "number",
+                    "description": "number of columns this input will take",
+                    "isOptional": True,
+                    "formOnly": True,
+                },
+                {
+                    "argName": "fullWidth",
+                    "typeName": "boolean",
+                    "description": "Whether the widget should take up the full width of the page",
+                    "isOptional": True,
+                    "formOnly": True,
+                },
+                {
+                    "argName": "placeholder",
+                    "typeName": "string",
+                    "description": "The placeholder text to display in the input",
+                    "default": "Your rich text here",
+                },
+            ]
+        },
+        "examples": [
+            {
+                "props": {"label": "Write here your bio"},
+                "name": "Basic Example",
+                "description": "The following example demonstrate some of the available functionality for read_richtext",
+                "key": "example1",
+                "code": 'read_richtext("Write here your bio")\n',
+            }
+        ],
+    },
     "tag-input": {
         "name": "Tag input",
         "type": "tag-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -4765,14 +5397,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -4789,14 +5422,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": None,
                     "typeDescription": "list(str) or list(float): The value entered by the user",
                 }
             ],
@@ -4848,14 +5489,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -4879,17 +5521,18 @@
                 "description": "The following example demonstrate some of the available functionality for read_tag",
                 "key": "example1",
                 "code": 'from hackerforms import read_tag\n\nans = read_tag(\n    "Type and press enter to add a tag", initial_value=["Red", "Green", "Blue"]\n)\n# ans = ["Red", "Green" or "Blue"]`\n',
             }
         ],
     },
     "text-input": {
-        "name": "Text field",
+        "name": "Text input",
         "description": "Text fields allow users to insert plain text.",
         "type": "text-input",
+        "autoHeight": True,
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
@@ -4942,14 +5585,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -4966,14 +5610,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "str", "typeDescription": "The value entered by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -5022,14 +5674,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -5066,29 +5719,30 @@
                 "description": "The following example shows the usage of the mask property for read widget. In the mask property, the '0' digit represents a numeric value, the 'a' digit represents an alphabetic value and other digits are recognized as part of the value",
                 "key": "example2",
                 "code": 'from hackerforms import read\n\nread("What is your credit card number?", mask="0000 0000 0000 0000")\n',
             },
         ],
     },
     "textarea-input": {
-        "name": "Long text field",
+        "name": "Long text input",
         "type": "textarea-input",
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
-        "description": "Long text field allow users to type longer textual content.",
+        "description": "Long text input allow users to type longer textual content.",
+        "autoHeight": False,
         "dashProperties": {
-            "minWidth": 200,
-            "minHeight": 200,
-            "initialWidth": 223,
-            "initialHeight": 272,
+            "minWidth": 100,
+            "minHeight": 100,
+            "initialWidth": 200,
+            "initialHeight": 150,
         },
         "pythonAPI": {
             "name": "read_textarea",
             "params": [
                 {
                     "argName": "label",
                     "description": "The label to display to the user",
@@ -5122,14 +5776,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -5146,14 +5801,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": "str", "typeDescription": "The value entered by the user"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -5195,14 +5858,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -5240,14 +5904,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "description": "Read a time value from the user",
         "dashProperties": {
             "minWidth": 120,
             "minHeight": 60,
             "initialWidth": 223,
             "initialHeight": 112,
         },
@@ -5288,14 +5953,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -5312,14 +5978,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "datetime.time",
                     "typeDescription": "A datetime.time object representing the value entered by the user",
                 }
             ],
@@ -5371,14 +6045,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -5409,17 +6084,18 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 120,
-            "minHeight": 100,
+            "minHeight": 60,
             "initialWidth": 377,
             "initialHeight": 112,
         },
         "pythonAPI": {
             "name": "read_toggle",
             "params": [
                 {
@@ -5454,14 +6130,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -5478,14 +6155,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {"typeName": None, "typeDescription": "bool: if the toggle was checked"}
             ],
         },
         "brokerAPI": {
             "params": [
@@ -5530,14 +6215,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -5579,14 +6265,15 @@
         "events": [
             {
                 "key": "change",
                 "description": "Function or expression to be run when the input value changes",
                 "payloadSchema": [],
             }
         ],
+        "autoHeight": False,
         "dashProperties": {
             "minWidth": 150,
             "minHeight": 112,
             "initialWidth": 223,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -5633,14 +6320,15 @@
                 {
                     "argName": "required",
                     "description": 'Whether the input is required or not eg. "this field is required". Defaults to True.',
                     "typeName": "Union[bool, str]",
                     "typeDescription": ["bool", "str"],
                     "isKwarg": True,
                     "default": "True",
+                    "formOnly": True,
                 },
                 {
                     "argName": "hint",
                     "description": "A tooltip displayed to the user. Defaults to None.",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": "None",
@@ -5657,14 +6345,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [
                 {
                     "typeName": "Union[FileResponse, List[FileResponse]]",
                     "typeDescription": 'A dict containing the video uploaded by the user ({"file": file, "url": str, "content": bytes}) or a list of videos in case of multiple flag set as True',
                 }
             ],
@@ -5716,14 +6412,15 @@
                 },
                 {
                     "argName": "required",
                     "typeName": ["boolean", "string"],
                     "description": "Whether the input is required or not",
                     "default": True,
                     "isOptional": True,
+                    "formOnly": True,
                 },
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
@@ -5745,22 +6442,23 @@
         },
         "examples": [
             {
                 "props": {"label": "Upload your video"},
                 "name": "Basic Example",
                 "description": "The following example demonstrate some of the available functionality for read_video",
                 "key": "example1",
-                "code": 'from hackerforms import read_video\n\nfileResponse = read_video("Upload your video")\nfile = fileResponse.file  # File object\nurl = fileResponse.url  # Url to the file\ncontent = fileResponse.content  # Raw file content\n',
+                "code": 'from hackerforms import read_video\n\nfile_response = read_video("Upload your video")\nfile = file_response.file  # File object\n',
             }
         ],
     },
     "file-output": {
         "name": "Download file",
         "description": "Show a button for the user to download a file.",
         "type": "file-output",
+        "autoHeight": True,
         "events": [],
         "dashProperties": {
             "minWidth": 65,
             "minHeight": 30,
             "initialWidth": 223,
             "initialHeight": 72,
         },
@@ -5795,14 +6493,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "fileUrl", "typeName": "string", "description": ""},
                 {
@@ -5841,14 +6547,15 @@
         ],
     },
     "html-output": {
         "name": "HTML",
         "description": "Embed HTML to the app.",
         "type": "html-output",
         "events": [],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 65,
             "minHeight": 30,
             "initialWidth": 146,
             "initialHeight": 32,
         },
         "pythonAPI": {
@@ -5875,14 +6582,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "html", "typeName": "string", "description": ""},
                 {
@@ -5914,14 +6629,15 @@
         ],
     },
     "iframe-output": {
         "name": "iframe",
         "description": "Embed content using iframe.",
         "type": "iframe-output",
         "events": [],
+        "autoHeight": False,
         "dashProperties": {
             "minWidth": 377,
             "minHeight": 632,
             "initialWidth": 377,
             "initialHeight": 632,
         },
         "pythonAPI": {
@@ -5964,14 +6680,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "url", "typeName": "string", "description": ""},
                 {
@@ -6017,14 +6741,15 @@
         ],
     },
     "image-output": {
         "name": "Show image",
         "description": "Show an image to the user",
         "type": "image-output",
         "events": [],
+        "autoHeight": False,
         "dashProperties": {
             "minWidth": 60,
             "minHeight": 60,
             "initialWidth": 223,
             "initialHeight": 312,
         },
         "pythonAPI": {
@@ -6065,14 +6790,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "imageUrl", "typeName": "string", "description": ""},
                 {
@@ -6118,14 +6851,15 @@
         ],
     },
     "latex-output": {
         "name": "Show Latex formula",
         "description": "Show an Latex formula to the user",
         "type": "latex-output",
         "events": [],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 60,
             "minHeight": 30,
             "initialWidth": 146,
             "initialHeight": 32,
         },
         "pythonAPI": {
@@ -6152,14 +6886,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {
                     "argName": "text",
@@ -6202,17 +6944,18 @@
         ],
     },
     "link-output": {
         "name": "Link (text URL)",
         "description": "Allow users to see and open content from text links.",
         "type": "link-output",
         "events": [],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 60,
-            "minHeight": 72,
+            "minHeight": 30,
             "initialWidth": 146,
             "initialHeight": 72,
         },
         "pythonAPI": {
             "name": "display_link",
             "params": [
                 {
@@ -6250,14 +6993,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "linkText", "typeName": "string", "description": ""},
                 {"argName": "linkUrl", "typeName": "string", "description": ""},
@@ -6297,14 +7048,15 @@
             }
         ],
     },
     "markdown-output": {
         "name": "Markdown",
         "description": "Show a formatted text to the user",
         "type": "markdown-output",
+        "autoHeight": True,
         "events": [],
         "dashProperties": {
             "minWidth": 60,
             "minHeight": 30,
             "initialWidth": 146,
             "initialHeight": 72,
         },
@@ -6332,14 +7084,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "text", "typeName": "string", "description": ""},
                 {
@@ -6370,26 +7130,43 @@
             }
         ],
     },
     "pandas-output": {
         "name": "Table",
         "description": "Display a pandas dataframe to the user",
         "type": "pandas-output",
+        "autoHeight": False,
         "events": [
             {
                 "key": "row-click",
                 "description": "When clicking on a row",
                 "payloadSchema": [
                     {
                         "key": "row",
                         "typeName": "pandas.Series",
                         "description": "The row that was clicked",
                     }
                 ],
-            }
+            },
+            {
+                "key": "row-edit",
+                "description": "Function or expression to be run when the user edits a cell",
+                "payloadSchema": [],
+            },
+            {
+                "key": "action-click",
+                "description": "Function or expression to be run when the input value changes",
+                "payloadSchema": [
+                    {
+                        "key": "action",
+                        "description": "The action that was clicked",
+                        "typeName": "str",
+                    }
+                ],
+            },
         ],
         "dashProperties": {
             "minWidth": 195,
             "minHeight": 72,
             "initialWidth": 245,
             "initialHeight": 72,
         },
@@ -6415,14 +7192,29 @@
                     "argName": "label",
                     "description": "The label to display to the user",
                     "typeName": "str",
                     "isKwarg": True,
                     "default": None,
                 },
                 {
+                    "argName": "editable",
+                    "description": "Whether the user will be allowed to edit the cells. Defaults to False.",
+                    "typeName": "bool",
+                    "isKwarg": True,
+                    "default": "False",
+                },
+                {
+                    "argName": "actions",
+                    "description": "Actions that can be triggered by table rows",
+                    "typeName": "list",
+                    "typeDescription": ["list[str]"],
+                    "isKwarg": True,
+                    "default": "[]",
+                },
+                {
                     "argName": "end_program",
                     "description": "Whether the program should end after the widget is shown. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
@@ -6430,14 +7222,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {
                     "argName": "table",
@@ -6468,14 +7268,26 @@
                 {
                     "argName": "label",
                     "typeName": "string",
                     "description": "The label to display above the dataframe",
                     "isOptional": True,
                 },
                 {
+                    "argName": "editable",
+                    "typeName": "boolean",
+                    "description": "Whether the user will be allowed to edit the cells",
+                    "default": False,
+                },
+                {
+                    "argName": "actions",
+                    "typeName": "array",
+                    "description": "Actions that can be triggered by table rows",
+                    "isOptional": True,
+                },
+                {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
                 },
                 {
@@ -6509,18 +7321,19 @@
                 "description": "The following example demonstrate some of the available functionality for display_pandas",
                 "key": "example1",
                 "code": "from hackerforms import display_pandas\n\ndisplay_pandas(df)\n",
             }
         ],
     },
     "plotly-output": {
-        "name": "Line chart",
-        "description": "Show a line chart to the user using Plotly",
+        "name": "Plotly graph",
+        "description": "Displays a Plotly figure to the user",
         "type": "plotly-output",
         "events": [],
+        "autoHeight": False,
         "dashProperties": {
             "minWidth": 245,
             "minHeight": 112,
             "initialWidth": 245,
             "initialHeight": 112,
         },
         "pythonAPI": {
@@ -6553,14 +7366,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "figure", "typeName": "any", "description": ""},
                 {
@@ -6601,14 +7422,15 @@
         ],
     },
     "progress-output": {
         "name": "Progress bar",
         "description": "Show a progress bar when loading the app.",
         "type": "progress-output",
         "events": [],
+        "autoHeight": True,
         "dashProperties": {
             "minWidth": 60,
             "minHeight": 30,
             "initialWidth": 300,
             "initialHeight": 32,
         },
         "pythonAPI": {
@@ -6649,14 +7471,22 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {
                     "argName": "current",
@@ -6702,22 +7532,23 @@
                 "code": "from hackerforms import display_progress\n\ndisplay_progress()\n",
             },
             {
                 "props": {"current": 8, "total": 10, "text": "Almost there!"},
                 "name": "Custom fields",
                 "description": "You can customize the current and total number of steps. Also the message of each step",
                 "key": "example2",
-                "code": 'from time import sleep\n\ndisplay_progress(0, 10, "Computing values")\n\n# Do some computation\nsleep(1)\n\ndisplay_progress(8, 10, "Almost there!")\n\n# Do some other computation\nsleep(1)\n\ndisplay("Done")\n',
+                "code": 'from time import sleep\n\nfor i in range(10):\n    display_progress(i, 10, text="Computing values")\n\n    sleep(1)  # Do some computation\n',
             },
         ],
     },
     "text-output": {
         "name": "Text display",
         "description": '"Text display" adds textual information into the app.',
         "type": "text-output",
+        "autoHeight": True,
         "events": [],
         "dashProperties": {
             "minWidth": 60,
             "minHeight": 30,
             "initialWidth": 223,
             "initialHeight": 112,
         },
@@ -6729,14 +7560,21 @@
                     "description": "The text to display to the user",
                     "typeName": "str",
                     "isKwarg": False,
                     "default": None,
                     "dashesInitialValue": '"Your text here!"',
                 },
                 {
+                    "argName": "size",
+                    "description": "The size of the text: 'small', 'medium', 'large'",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "medium",
+                },
+                {
                     "argName": "end_program",
                     "description": "Whether the program should end after the widget is shown. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
@@ -6744,20 +7582,29 @@
                     "argName": "full_width",
                     "description": "Whether the input should use full screen width. Defaults to False.",
                     "typeName": "bool",
                     "isKwarg": True,
                     "default": "False",
                     "formOnly": True,
                 },
+                {
+                    "argName": "button_text",
+                    "description": "What text to display on the button when the widget is not part of a Page. Defaults to 'Next'.",
+                    "typeName": "str",
+                    "isKwarg": True,
+                    "default": "Next",
+                    "formOnly": True,
+                },
             ],
             "returns": [],
         },
         "brokerAPI": {
             "params": [
                 {"argName": "text", "description": "", "typeName": "string"},
+                {"argName": "size", "description": "", "typeName": "string"},
                 {
                     "argName": "columns",
                     "typeName": "number",
                     "description": "number of columns this input will take",
                     "isOptional": True,
                     "formOnly": True,
                 },
```

### Comparing `abstra-0.9.0/abstra/widgets/response_types.py` & `abstra-1.0.0/abstra/widgets/response_types.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/types.py` & `abstra-1.0.0/abstra/widgets/types.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra/widgets/validation.py` & `abstra-1.0.0/abstra/widgets/validation.py`

 * *Files identical despite different names*

### Comparing `abstra-0.9.0/abstra.egg-info/PKG-INFO` & `abstra-1.0.0/abstra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstra
-Version: 0.9.0
+Version: 1.0.0
 Summary: Abstra Lib
 Home-page: https://github.com/abstra-app/abstra-lib
 License: MIT
 Description: [![pypi](https://img.shields.io/pypi/v/abstra.svg)](https://pypi.python.org/pypi/abstra)
         [![PyPI Downloads](https://img.shields.io/pypi/dm/abstra.svg)](https://pypi.org/project/abstra/)
         [![Code check](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml/badge.svg)](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml)
```

