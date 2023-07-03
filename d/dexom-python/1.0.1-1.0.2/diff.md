# Comparing `tmp/dexom_python-1.0.1.tar.gz` & `tmp/dexom_python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexom_python-1.0.1.tar", max compression
+gzip compressed data, was "dexom_python-1.0.2.tar", max compression
```

## Comparing `dexom_python-1.0.1.tar` & `dexom_python-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35086 2023-04-17 07:19:51.515506 dexom_python-1.0.1/LICENSE
--rw-r--r--   0        0        0    12001 2023-04-17 07:19:51.515506 dexom_python-1.0.1/README.md
--rw-r--r--   0        0        0      559 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/__init__.py
--rw-r--r--   0        0        0     6006 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/Snakefile
--rw-r--r--   0        0        0        0 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/__init__.py
--rw-r--r--   0        0        0     2741 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/cluster_config.yaml
--rw-r--r--   0        0        0      452 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/cluster_install_dexom_python.sh
--rw-r--r--   0        0        0        0 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/legacy/__init__.py
--rw-r--r--   0        0        0     7487 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/legacy/dexom_cluster_results.py
--rw-r--r--   0        0        0    16971 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/legacy/write_cluster_scripts.py
--rw-r--r--   0        0        0     1006 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/slurm_example_gpr.sh
--rw-r--r--   0        0        0     1253 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/snakemake_utils.smk
--rw-r--r--   0        0        0     1145 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/solution_compilation.py
--rw-r--r--   0        0        0      803 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/submit.py
--rw-r--r--   0        0        0      436 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/cluster_utils/submit_slurm.sh
--rw-r--r--   0        0        0      423 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/default_parameter_values.py
--rw-r--r--   0        0        0      219 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/__init__.py
--rw-r--r--   0        0        0    11182 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/diversity_enum_functions.py
--rw-r--r--   0        0        0     7662 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/enumeration.py
--rw-r--r--   0        0        0     9335 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/icut_functions.py
--rw-r--r--   0        0        0    11129 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/maxdist_functions.py
--rw-r--r--   0        0        0    13950 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/rxn_enum_functions.py
--rw-r--r--   0        0        0    10988 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/gpr_rules.py
--rw-r--r--   0        0        0    11789 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/imat_functions.py
--rw-r--r--   0        0        0     2487 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/main.py
--rw-r--r--   0        0        0     7382 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/model_functions.py
--rw-r--r--   0        0        0     7925 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/pathway_enrichment.py
--rw-r--r--   0        0        0     8878 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/result_functions.py
--rw-r--r--   0        0        0    10064 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/toy_models.py
--rw-r--r--   0        0        0      696 2023-04-17 07:19:51.547509 dexom_python-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12992 1970-01-01 00:00:00.000000 dexom_python-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35086 2023-07-03 07:28:33.001593 dexom_python-1.0.2/LICENSE
+-rw-r--r--   0        0        0    12002 2023-07-03 07:28:33.001593 dexom_python-1.0.2/README.md
+-rw-r--r--   0        0        0      559 2023-07-03 07:28:33.001593 dexom_python-1.0.2/dexom_python/__init__.py
+-rw-r--r--   0        0        0     6006 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/Snakefile
+-rw-r--r--   0        0        0        0 2023-07-03 07:28:33.097595 dexom_python-1.0.2/dexom_python/cluster_utils/__init__.py
+-rw-r--r--   0        0        0     2741 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/cluster_config.yaml
+-rw-r--r--   0        0        0      452 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/cluster_install_dexom_python.sh
+-rw-r--r--   0        0        0        0 2023-07-03 07:28:33.097595 dexom_python-1.0.2/dexom_python/cluster_utils/legacy/__init__.py
+-rw-r--r--   0        0        0     7487 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/legacy/dexom_cluster_results.py
+-rw-r--r--   0        0        0    16971 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/legacy/write_cluster_scripts.py
+-rw-r--r--   0        0        0     1006 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/slurm_example_gpr.sh
+-rw-r--r--   0        0        0     1253 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/snakemake_utils.smk
+-rw-r--r--   0        0        0     1145 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/solution_compilation.py
+-rw-r--r--   0        0        0      803 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/submit.py
+-rw-r--r--   0        0        0      436 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/cluster_utils/submit_slurm.sh
+-rw-r--r--   0        0        0      423 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/default_parameter_values.py
+-rw-r--r--   0        0        0      219 2023-07-03 07:28:33.005593 dexom_python-1.0.2/dexom_python/enum_functions/__init__.py
+-rw-r--r--   0        0        0    11182 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/enum_functions/diversity_enum_functions.py
+-rw-r--r--   0        0        0     7662 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/enum_functions/enumeration.py
+-rw-r--r--   0        0        0     9335 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/enum_functions/icut_functions.py
+-rw-r--r--   0        0        0    11129 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/enum_functions/maxdist_functions.py
+-rw-r--r--   0        0        0    13950 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/enum_functions/rxn_enum_functions.py
+-rw-r--r--   0        0        0    10988 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/gpr_rules.py
+-rw-r--r--   0        0        0    11789 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/imat_functions.py
+-rw-r--r--   0        0        0     2487 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/main.py
+-rw-r--r--   0        0        0     7382 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/model_functions.py
+-rw-r--r--   0        0        0     7925 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/pathway_enrichment.py
+-rw-r--r--   0        0        0     8878 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/result_functions.py
+-rw-r--r--   0        0        0    10064 2023-07-03 07:28:33.009593 dexom_python-1.0.2/dexom_python/toy_models.py
+-rw-r--r--   0        0        0      721 2023-07-03 07:28:33.029594 dexom_python-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13055 1970-01-01 00:00:00.000000 dexom_python-1.0.2/PKG-INFO
```

### Comparing `dexom_python-1.0.1/LICENSE` & `dexom_python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/README.md` & `dexom_python-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 To view changes between versions, see [changelog](docs/changelog.rst)
 
 API documentation is available here: https://dexom-python.readthedocs.io/en/stable/  
 All of the commandline scripts can be called with the `-h` option to display help messages.
 
 ## Requirements
-- Python 3.7 - 3.9
+- Python 3.7 - 3.10
 - CPLEX 12.10 - 22.10
 
 ### Installing CPLEX
 
 [Free license (Trial version)](https://www.ibm.com/analytics/cplex-optimizer): this version is limited to 1000 variables and 1000 constraints, and is therefore not useable on larger models
 
 [Academic license](https://www.ibm.com/academic/technology/data-science): for this, you must sign up using an academic email address.
```

### Comparing `dexom_python-1.0.1/dexom_python/__init__.py` & `dexom_python-1.0.2/dexom_python/__init__.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/Snakefile` & `dexom_python-1.0.2/dexom_python/cluster_utils/Snakefile`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/cluster_config.yaml` & `dexom_python-1.0.2/dexom_python/cluster_utils/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/legacy/dexom_cluster_results.py` & `dexom_python-1.0.2/dexom_python/cluster_utils/legacy/dexom_cluster_results.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/legacy/write_cluster_scripts.py` & `dexom_python-1.0.2/dexom_python/cluster_utils/legacy/write_cluster_scripts.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/slurm_example_gpr.sh` & `dexom_python-1.0.2/dexom_python/cluster_utils/slurm_example_gpr.sh`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/snakemake_utils.smk` & `dexom_python-1.0.2/dexom_python/cluster_utils/snakemake_utils.smk`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/solution_compilation.py` & `dexom_python-1.0.2/dexom_python/cluster_utils/solution_compilation.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/cluster_utils/submit.py` & `dexom_python-1.0.2/dexom_python/cluster_utils/submit.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/enum_functions/diversity_enum_functions.py` & `dexom_python-1.0.2/dexom_python/enum_functions/diversity_enum_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/enum_functions/enumeration.py` & `dexom_python-1.0.2/dexom_python/enum_functions/enumeration.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/enum_functions/icut_functions.py` & `dexom_python-1.0.2/dexom_python/enum_functions/icut_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/enum_functions/maxdist_functions.py` & `dexom_python-1.0.2/dexom_python/enum_functions/maxdist_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/enum_functions/rxn_enum_functions.py` & `dexom_python-1.0.2/dexom_python/enum_functions/rxn_enum_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/gpr_rules.py` & `dexom_python-1.0.2/dexom_python/gpr_rules.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/imat_functions.py` & `dexom_python-1.0.2/dexom_python/imat_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/main.py` & `dexom_python-1.0.2/dexom_python/main.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/model_functions.py` & `dexom_python-1.0.2/dexom_python/model_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/pathway_enrichment.py` & `dexom_python-1.0.2/dexom_python/pathway_enrichment.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/result_functions.py` & `dexom_python-1.0.2/dexom_python/result_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/dexom_python/toy_models.py` & `dexom_python-1.0.2/dexom_python/toy_models.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0.1/pyproject.toml` & `dexom_python-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "dexom_python"
-version = "1.0.1"
+version = "1.0.2"
 description = "DEXOM implementation in python using cobrapy"
 authors = ["Maximilian Stingl <maximilian.stingl@inrae.fr>"]
 license = "GPL-3.0"
 readme="README.md"
 include=["LICENSE"]
 repository = "https://forgemia.inra.fr/metexplore/cbm/dexom-python"
 homepage = "https://forgemia.inra.fr/metexplore/cbm/dexom-python"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.10"
+python = ">=3.7,<3.11"
 cobra = "^0.26.3"
-numpy = "1.20"
+numpy = ">=1.20,<1.24"
 six = "^1.16"
-scipy = "1.7"
+scipy = "^1.7"
 symengine = "^0.9.2"
 matplotlib = "^3.5.1"
 scikit-learn = "^1.0.2"
 statsmodels = "^0.13.2"
 
 [tool.poetry.dev-dependencies]
+pytest = "^7.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dexom_python-1.0.1/PKG-INFO` & `dexom_python-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: dexom-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: DEXOM implementation in python using cobrapy
 Home-page: https://forgemia.inra.fr/metexplore/cbm/dexom-python
 License: GPL-3.0
 Author: Maximilian Stingl
 Author-email: maximilian.stingl@inrae.fr
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cobra (>=0.26.3,<0.27.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
-Requires-Dist: numpy (==1.20)
+Requires-Dist: numpy (>=1.20,<1.24)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
-Requires-Dist: scipy (==1.7)
+Requires-Dist: scipy (>=1.7,<2.0)
 Requires-Dist: six (>=1.16,<2.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: symengine (>=0.9.2,<0.10.0)
 Project-URL: Repository, https://forgemia.inra.fr/metexplore/cbm/dexom-python
 Description-Content-Type: text/markdown
 
 # DEXOM in python
@@ -41,15 +42,15 @@
 
 To view changes between versions, see [changelog](docs/changelog.rst)
 
 API documentation is available here: https://dexom-python.readthedocs.io/en/stable/  
 All of the commandline scripts can be called with the `-h` option to display help messages.
 
 ## Requirements
-- Python 3.7 - 3.9
+- Python 3.7 - 3.10
 - CPLEX 12.10 - 22.10
 
 ### Installing CPLEX
 
 [Free license (Trial version)](https://www.ibm.com/analytics/cplex-optimizer): this version is limited to 1000 variables and 1000 constraints, and is therefore not useable on larger models
 
 [Academic license](https://www.ibm.com/academic/technology/data-science): for this, you must sign up using an academic email address.
```

