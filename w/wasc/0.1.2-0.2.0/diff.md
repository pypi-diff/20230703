# Comparing `tmp/wasc-0.1.2.tar.gz` & `tmp/wasc-0.2.0.tar.gz`

## Comparing `wasc-0.1.2.tar` & `wasc-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 wasc-0.1.2/data/agro_alim.csv
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wasc-0.1.2/data/criteria.yml
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wasc-0.1.2/data/example_websites.csv
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/__main__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/abstract_checker.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/checker_factory.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/criterion.py
--rw-r--r--   0        0        0    15835 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/default_checkers.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/report.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/utils.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/cli/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/test_checker.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/test_utils.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/data/crit_example.yml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/data/url_example.csv
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wasc-0.1.2/.gitignore
--rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wasc-0.1.2/README.md
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 wasc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 wasc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 wasc-0.2.0/data/agro_alim.csv
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wasc-0.2.0/data/criteria.yml
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wasc-0.2.0/data/example_websites.csv
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/__main__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/abstract_checker.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/checker_factory.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/criterion.py
+-rw-r--r--   0        0        0    15835 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/default_checkers.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/report.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/utils.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/cli/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/test_checker.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/data/crit_example.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/data/url_example.csv
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wasc-0.2.0/.gitignore
+-rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wasc-0.2.0/README.md
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 wasc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 wasc-0.2.0/PKG-INFO
```

### Comparing `wasc-0.1.2/data/agro_alim.csv` & `wasc-0.2.0/data/agro_alim.csv`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Barilla, https://www.barilla.com/fr-fr
-Bonduelle, https://www.bonduelle.fr/
-Danone, https://www.danone.com/fr.html
-Danone France, https://www.danone.fr/
-Ferrero, https://www.ferrero.fr/
-Fleury Michon, https://www.fleurymichon.fr/
-Groupe Bel, https://www.groupe-bel.com/fr/
-Groupe Panzani, https://www.groupe-panzani.fr/
-Heineken, https://www.heinekenfrance.fr/
-Kronenbourg, https://www.kronenbourg.com/
-Limagrain, https://www.limagrain.com/
-Nestlé, https://www.nestle.fr/
-Orangina Suntory, https://oranginasuntoryfrance.com/
-Pernod Ricard, https://www.pernod-ricard.com/fr
-Rémy Cointreau, https://www.remy-cointreau.com/fr
-Tereos (Béghin Say), https://tereos.com/fr/
-Tipiak, https://groupe.tipiak.fr/fr
-Unilever, https://www.unilever.fr/
+Barilla; https://www.barilla.com/fr-fr
+Bonduelle; https://www.bonduelle.fr/
+Danone; https://www.danone.com/fr.html
+Danone France; https://www.danone.fr/
+Ferrero; https://www.ferrero.fr/
+Fleury Michon; https://www.fleurymichon.fr/
+Groupe Bel; https://www.groupe-bel.com/fr/
+Groupe Panzani; https://www.groupe-panzani.fr/
+Heineken; https://www.heinekenfrance.fr/
+Kronenbourg; https://www.kronenbourg.com/
+Limagrain; https://www.limagrain.com/
+Nestlé; https://www.nestle.fr/
+Orangina Suntory; https://oranginasuntoryfrance.com/
+Pernod Ricard; https://www.pernod-ricard.com/fr
+Rémy Cointreau; https://www.remy-cointreau.com/fr
+Tereos (Béghin Say); https://tereos.com/fr/
+Tipiak; https://groupe.tipiak.fr/fr
+Unilever; https://www.unilever.fr/
```

### Comparing `wasc-0.1.2/src/wasc/abstract_checker.py` & `wasc-0.2.0/src/wasc/abstract_checker.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/src/wasc/checker_factory.py` & `wasc-0.2.0/src/wasc/checker_factory.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/src/wasc/criterion.py` & `wasc-0.2.0/src/wasc/criterion.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/src/wasc/default_checkers.py` & `wasc-0.2.0/src/wasc/default_checkers.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/src/wasc/report.py` & `wasc-0.2.0/src/wasc/report.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/src/wasc/utils.py` & `wasc-0.2.0/src/wasc/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
 #
 # SPDX-License-Identifier: CECILL-2.1
 """
 This module provides some reading functions
 """
-import csv
-
+import pandas as pd
 import yaml
 
 
 def read_criteria_config(filename) :
     """
     Reads the list of criteria.
     Each criterion is associated with a list of checkers
@@ -35,19 +34,19 @@
     Parameters
     ----------
     filename : File
         File containing websites list in CSV format
 
     Returns
     -------
-     : dict
+     : list
         A list of of (websites, url)
     """
-    with open(filename, encoding = "utf-8") as url_file :
-        return [(line[0].strip(), line[1].strip()) for line in csv.reader(url_file)]
+    df = pd.read_csv(filename, sep=";", comment="#", header = None, names=["org", "url"], skipinitialspace=True)
+    return list(zip(df.org, df.url))
 
 def check_and_correct_url(target_url : str, root_url : str) -> str :
     """
     This method check if the target_url is truncated and, if so,
     recompose from the root_url
 
     Parameters
@@ -82,8 +81,19 @@
 
 def find_link(access_tag, root_url):
     while access_tag and access_tag.name != "a" and access_tag.name != "html":
         access_tag = access_tag.parent
     try :
         return check_and_correct_url(access_tag.attrs["href"], root_url)
     except KeyError :
-        pass
+        pass
+
+def dict_to_csv(indict):
+    res = {"Organisation" : []}
+    for org, subdict in indict.items():
+        res["Organisation"].append(org)
+        for checkdict in subdict.values():
+            for key, val in checkdict.items():
+                if key not in res:
+                    res[key] = []
+                res[key].append(val)
+    return res
```

### Comparing `wasc-0.1.2/src/wasc/cli/__init__.py` & `wasc-0.2.0/src/wasc/cli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
 #
 # SPDX-License-Identifier: CECILL-2.1
 import json
 import sys
 
 import click
+import pandas as pd
 from tqdm import tqdm
 
 from wasc.__about__ import __version__
 from wasc.criterion import Criterion
 from wasc.report import Report
-from wasc.utils import read_criteria_config, read_websites
+from wasc.utils import dict_to_csv, read_criteria_config, read_websites
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 DEFAULT_CRIT_DICT = { "Accessibilité" : ["AccessChecker", "AccessLinkChecker"], "Mentions légales" : ["MentionsLegalesChecker"]}
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("websites", type=click.Path(exists=True))
 @click.option("-c", "--criteria", type=click.Path(exists=True),
@@ -43,8 +44,17 @@
     crit_list = [Criterion(crit, checkers) for crit, checkers in crit_dict.items()]
     websites = read_websites(websites)
     click.echo(f"Analysis of {len(websites)} websites...")
     report = {}
     for i in tqdm(range(len(websites))):
         label, url = websites[i]
         report[label] = Report(label, url, crit_list).execute()
-    click.echo(json.dumps(report, sort_keys=True, indent=4, ensure_ascii=False), file=output)
+    if output == sys.stdout:
+        click.echo("Results:")
+    else :
+        click.echo("Save results in " + output.name)
+    if output_format == "json":
+        click.echo(json.dumps(report, sort_keys=True, indent=4, ensure_ascii=False), file=output)
+    elif output_format == "csv":
+        res = dict_to_csv(report)
+        click.echo(pd.DataFrame(res).to_csv(sep=";", index=False), file=output)
+    click.echo("Completed")
```

### Comparing `wasc-0.1.2/tests/test_checker.py` & `wasc-0.2.0/tests/test_checker.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/tests/test_utils.py` & `wasc-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/LICENSE.txt` & `wasc-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wasc-0.1.2/pyproject.toml` & `wasc-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 dependencies = [
   "click",
   "pyyaml",
   "beautifulsoup4",
   "requests",
   "tqdm",
+  "pandas"
 ]
 
 [project.urls]
 Documentation = "https://github.com/gcollet/wasc#readme"
 Issues = "https://github.com/gcollet/wasc/issues"
 Source = "https://github.com/gcollet/wasc"
 
@@ -55,15 +56,15 @@
 [tool.hatch.envs.default.env-vars]
 WASC_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.build.env-vars]
 WACS_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
+test = "pytest -v {args:tests}"
 all_test = "pytest tests/__init__.py"
 test-cov = "coverage run -m pytest {args:tests}"
 lcov = "coverage lcov"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
```

### Comparing `wasc-0.1.2/PKG-INFO` & `wasc-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasc
-Version: 0.1.2
+Version: 0.2.0
 Summary: wasc, for Web Accessibility Simple Checker, helps to evaluate accessibility criteria on a list of websites
 Project-URL: Documentation, https://github.com/gcollet/wasc#readme
 Project-URL: Issues, https://github.com/gcollet/wasc/issues
 Project-URL: Source, https://github.com/gcollet/wasc
 Author-email: Guillaume Collet <bilouweb@free.fr>, Juliette Francis <juliette.francis@etudiant.univ-rennes.fr>
 License-Expression: CECILL-2.1
 License-File: LICENSE.txt
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4
 Requires-Dist: click
+Requires-Dist: pandas
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # wasc
```

