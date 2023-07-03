# Comparing `tmp/OpenFisca-Country-Template-6.0.1.tar.gz` & `tmp/OpenFisca-Country-Template-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Country-Template-6.0.1.tar", last modified: Wed Jun 14 14:26:13 2023, max compression
+gzip compressed data, was "OpenFisca-Country-Template-6.0.2.tar", last modified: Mon Jul  3 11:19:48 2023, max compression
```

## Comparing `OpenFisca-Country-Template-6.0.1.tar` & `OpenFisca-Country-Template-6.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.611308 OpenFisca-Country-Template-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    17989 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.607308 OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9398 2023-06-14 14:26:13.000000 OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-06-14 14:26:13.000000 OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:26:13.000000 OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-14 14:26:13.000000 OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-14 14:26:13.000000 OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9398 2023-06-14 14:26:13.611308 OpenFisca-Country-Template-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8527 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.607308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.603307 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.607308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/benefits/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/benefits/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/benefits/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/benefits/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.607308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/benefits/parenting_allowance/
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.607308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/general/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/general/age_of_majority.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/general/age_of_retirement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.607308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/taxes/
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/taxes/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.607308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/add_dynamic_variable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/add_new_tax.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/flat_social_security_contribution.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/modify_social_security_taxation.py
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/removal_basic_income.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.611308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/situation_examples/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/situation_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/situation_examples/couple.json
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/situation_examples/housing.json
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/situation_examples/single.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.611308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/age.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/disposable_income.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.611308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/reforms/add_new_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.611308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/situations/
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/situations/income_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/situations/parenting_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:26:13.611308 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/benefits.py
--rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/demographics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/housing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/income.py
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/taxes.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-14 14:26:13.615308 OpenFisca-Country-Template-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-06-14 14:25:45.000000 OpenFisca-Country-Template-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.966235 OpenFisca-Country-Template-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    18207 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9398 2023-07-03 11:19:48.000000 OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-07-03 11:19:48.000000 OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 11:19:48.000000 OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-03 11:19:48.000000 OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-03 11:19:48.000000 OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9398 2023-07-03 11:19:48.966235 OpenFisca-Country-Template-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8527 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.954235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/benefits/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/benefits/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/benefits/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/benefits/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/benefits/parenting_allowance/
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/general/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/general/age_of_majority.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/general/age_of_retirement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/taxes/
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/taxes/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/add_dynamic_variable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/add_new_tax.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/flat_social_security_contribution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/modify_social_security_taxation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/removal_basic_income.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.962235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/situation_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/situation_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/situation_examples/couple.json
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/situation_examples/housing.json
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/situation_examples/single.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.966235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/disposable_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.966235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/reforms/add_new_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.966235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/situations/
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/situations/income_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/situations/parenting_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:19:48.966235 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/benefits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/demographics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/housing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/income.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/taxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 11:19:48.966235 OpenFisca-Country-Template-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-03 11:19:25.000000 OpenFisca-Country-Template-6.0.2/setup.py
```

### Comparing `OpenFisca-Country-Template-6.0.1/CHANGELOG.md` & `OpenFisca-Country-Template-6.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+### 6.0.2 [#132](https://github.com/openfisca/country-template/pull/132)
+
+* Technical improvement.
+* Impacted areas: template setup script
+* Details:
+  - Allows country-template to pass `check-style` makefile command
+
 ### 6.0.1 [#134](https://github.com/openfisca/country-template/pull/134)
 
 * Technical improvement.
 * Impacted areas: template replacement script
 * Details:
   - Avoid `sed: RE error: illegal byte sequence` error when template contains `.DS_Store` files after GUI navigation in macOS
```

### Comparing `OpenFisca-Country-Template-6.0.1/LICENSE` & `OpenFisca-Country-Template-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/PKG-INFO` & `OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Country-Template
-Version: 6.0.1
+Version: 6.0.2
 Summary: OpenFisca tax and benefit system for Country-Template
 Home-page: https://github.com/openfisca/country-template
 Author: OpenFisca Team
 Author-email: contact@openfisca.org
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `OpenFisca-Country-Template-6.0.1/OpenFisca_Country_Template.egg-info/SOURCES.txt` & `OpenFisca-Country-Template-6.0.2/OpenFisca_Country_Template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/PKG-INFO` & `OpenFisca-Country-Template-6.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Country-Template
-Version: 6.0.1
+Version: 6.0.2
 Summary: OpenFisca tax and benefit system for Country-Template
 Home-page: https://github.com/openfisca/country-template
 Author: OpenFisca Team
 Author-email: contact@openfisca.org
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `OpenFisca-Country-Template-6.0.1/README.md` & `OpenFisca-Country-Template-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/__init__.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/entities.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/entities.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/parameters/taxes/social_security_contribution.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/parameters/taxes/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/add_dynamic_variable.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/add_dynamic_variable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/add_new_tax.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/add_new_tax.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/flat_social_security_contribution.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/flat_social_security_contribution.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/modify_social_security_taxation.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/modify_social_security_taxation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/reforms/removal_basic_income.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/reforms/removal_basic_income.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/situation_examples/couple.json` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/situation_examples/couple.json`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/age.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/age.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/basic_income.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/basic_income.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/disposable_income.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/disposable_income.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/housing_tax.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/housing_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/reforms/add_new_tax.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/reforms/add_new_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/situations/income_tax.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/situations/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/situations/parenting_allowance.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/situations/parenting_allowance.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/tests/social_security_contribution.yaml` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/tests/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/benefits.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/benefits.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/demographics.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/demographics.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/housing.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/housing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/income.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/income.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/stats.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/stats.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/openfisca_country_template/variables/taxes.py` & `OpenFisca-Country-Template-6.0.2/openfisca_country_template/variables/taxes.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/setup.cfg` & `OpenFisca-Country-Template-6.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.1/setup.py` & `OpenFisca-Country-Template-6.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the contents of our README file for PyPi
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()  # pylint: disable=W1514
 
 setup(
     name = "OpenFisca-Country-Template",
-    version = "6.0.1",
+    version = "6.0.2",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.org",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

