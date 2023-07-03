# Comparing `tmp/guarddog-1.1.4.tar.gz` & `tmp/guarddog-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.1.4.tar", max compression
+gzip compressed data, was "guarddog-1.2.tar", max compression
```

## Comparing `guarddog-1.1.4.tar` & `guarddog-1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-03-30 10:53:40.280762 guarddog-1.1.4/LICENSE
--rw-r--r--   0        0        0      314 2023-03-30 10:53:40.280762 guarddog-1.1.4/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      154 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9622 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0      609 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0      696 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0      793 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     1176 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0     4153 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      976 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      723 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1803 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11057 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2023-03-30 10:53:40.284762 guarddog-1.1.4/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3479 2023-03-30 10:53:40.288763 guarddog-1.1.4/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      438 2023-03-30 10:53:40.288763 guarddog-1.1.4/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2023-03-30 10:53:40.288763 guarddog-1.1.4/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2023-03-30 10:53:40.288763 guarddog-1.1.4/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2023-03-30 10:53:40.288763 guarddog-1.1.4/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5620 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0      889 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      682 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4599 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     1367 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2269 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1786 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0      716 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0      835 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0      926 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    11289 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/cli.py
--rw-r--r--   0        0        0      315 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6185 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2699 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5487 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11176 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2023-03-30 10:53:40.292763 guarddog-1.1.4/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2023-03-30 10:53:40.292763 guarddog-1.1.4/pypi.rst
--rw-r--r--   0        0        0     1721 2023-03-30 10:53:54.617719 guarddog-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 guarddog-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-03 07:15:42.313327 guarddog-1.2/LICENSE
+-rw-r--r--   0        0        0      314 2023-07-03 07:15:42.313327 guarddog-1.2/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      154 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9679 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0      696 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     1176 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0     4153 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      976 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1803 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11057 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      438 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5620 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0      889 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      682 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4599 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     1806 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2269 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1786 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0      716 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0      835 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0      926 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    11907 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6185 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2699 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5487 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11176 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2023-07-03 07:15:42.321327 guarddog-1.2/pypi.rst
+-rw-r--r--   0        0        0     1302 2023-07-03 07:15:54.413624 guarddog-1.2/pyproject.toml
+-rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 guarddog-1.2/PKG-INFO
```

### Comparing `guarddog-1.1.4/LICENSE` & `guarddog-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/analyzer.py` & `guarddog-1.2/guarddog/analyzer/analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import os
 import subprocess
+from collections import defaultdict
 from pathlib import Path
-from typing import Optional, Iterable, List
+from typing import Iterable, List, Optional
 
 from guarddog.analyzer.metadata import get_metadata_detectors
 from guarddog.ecosystems import ECOSYSTEM
 
 
 def get_rules(file_extension, path):
     return set(rule.replace(file_extension, "") for rule in os.listdir(path) if rule.endswith(file_extension))
@@ -173,15 +174,15 @@
             log.debug("No source code rules to run")
             return {"results": {}, "errors": {}, "issues": 0}
 
         try:
             log.debug(f"Running source code rules against {path}")
             response = self._invoke_semgrep(target=path, rules=rules_path)
             rule_results = self._format_semgrep_response(response, targetpath=targetpath)
-            issues += len(rule_results)
+            issues += sum(len(res) for res in rule_results.values())
 
             results = results | rule_results
         except Exception as e:
             errors["rules-all"] = f"failed to run rule: {str(e)}"
 
         return {"results": results, "errors": errors, "issues": issues}
 
@@ -225,43 +226,44 @@
                 Paths in formatted resonse will be rooted from targetpath.
 
         Returns:
             dict: formatted response in the form...
 
             {
                 ...
-                <rule-name>: {
-                    <path-to-code:line-num>: <dangerous-code>
+                <rule-name>: [
+                    {
+                        <path-to-code:line-num>: <dangerous-code>
+                        ...
+                    },
                     ...
-                },
+                ],
                 ...
             }
         """
 
-        results = {}
+        results = defaultdict(list)
 
         for result in response["results"]:
             rule_name = rule or result["check_id"].split(".")[-1]
             code_snippet = result["extra"]["lines"]
             line = result["start"]["line"]
 
             file_path = os.path.abspath(result["path"])
             if targetpath:
                 file_path = os.path.relpath(file_path, targetpath)
 
             location = file_path + ":" + str(line)
             code = self.trim_code_snippet(code_snippet)
 
-            if rule_name not in result:
-                results[rule_name] = []
-                results[rule_name].append({
-                    'location': location,
-                    'code': code,
-                    'message': result["extra"]["message"]
-                })
+            results[rule_name].append({
+                'location': location,
+                'code': code,
+                'message': result["extra"]["message"]
+            })
 
         return results
 
     # Makes sure the matching code to be displayed isn't too long
     def trim_code_snippet(self, code):
         THRESHOLD = 250
         if len(code) > THRESHOLD:
```

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/detector.py` & `guarddog-1.2/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.2/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.2/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.2/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.2/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.2/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.2/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/potentially_compromised_email_domain.py` & `guarddog-1.2/guarddog/analyzer/metadata/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.2/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.2/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.2/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.2/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.2/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.2/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.2/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
         top_packages_information = None
 
         if top_packages_filename in os.listdir(resources_dir):
             update_time = datetime.fromtimestamp(os.path.getmtime(top_packages_path))
 
             if datetime.now() - update_time <= timedelta(days=30):
-                top_packages_file = open(top_packages_path, "r")
-                top_packages_information = json.load(top_packages_file)["rows"]
+                with open(top_packages_path, "r") as top_packages_file:
+                    top_packages_information = json.load(top_packages_file)["rows"]
 
         if top_packages_information is None:
             response = requests.get(popular_packages_url).json()
             with open(top_packages_path, "w+") as f:
                 json.dump(response, f, ensure_ascii=False, indent=4)
 
             top_packages_information = response["rows"]
```

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.2/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.2/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.2/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.2/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.2/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/download-executable.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/download-executable.yml`

 * *Files 7% similar despite different names*

```diff
@@ -6,35 +6,45 @@
     metadata:
       description: Identify when a package downloads and makes executable a remote binary
     mode: taint
     pattern-sinks:
       - patterns:
           - pattern-either:
               - pattern: |
-                  $FILE = open("$LOC", ...)
+                  $FILE = open($LOC, ...)
                   ...
                   $FILE.write($REQUEST)
                   ...
                   $CHANGE_PERMISSIONS
               - pattern: |
-                  with open("$LOC", ...) as $FILE:
+                  with open($LOC, ...) as $FILE:
                     ...
                     $FILE.write($REQUEST)
                   ...
                   $CHANGE_PERMISSIONS
+              - pattern: |
+                  open($LOC, ...).write($REQUEST)
+                  ...
+                  $CHANGE_PERMISSIONS
           - metavariable-pattern:
               metavariable: $CHANGE_PERMISSIONS
               pattern-either:
                 - pattern: os.chmod("$LOC", 777)
+                - pattern: os.chmod($LOC, 777)
                 - pattern: os.chmod("$LOC", <...stat.S_IEXEC...>)
+                - pattern: os.chmod($LOC, <...stat.S_IEXEC...>)
                 - pattern: chmod("$LOC", 777)
+                - pattern: chmod($LOC, 777)
                 - pattern: chmod("$LOC", <...stat.S_IEXEC...>)
+                - pattern: chmod($LOC, <...stat.S_IEXEC...>)
+                - pattern: os.system(f"...{$LOC}...")
     pattern-sources:
       - pattern: (...).send(...)
       - pattern: send(...)
       - pattern: (...).request(...)
       - pattern: request(...)
       - pattern: (...).urlopen(...)
       - pattern: urlopen(...)
       - pattern: (...).getresponse(...)
       - pattern: getresponse(...)
-    severity: WARNING
+      - pattern: requests.$FUNC(...)
+    severity: WARNING
```

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-install-script.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/npm-install-script.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/shady-links.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/shady-links.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.2/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/cli.py` & `guarddog-1.2/guarddog/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,35 +161,47 @@
     """
 
     rule_param = _get_rule_pram(rules, exclude_rules)
     scanner = cast(Optional[PackageScanner], get_scanner(ecosystem, False))
     if scanner is None:
         sys.stderr.write(f"Command scan is not supported for ecosystem {ecosystem}")
         exit(1)
-    results = {}
+    results = []
     if is_local_target(identifier):
         log.debug(f"Considering that '{identifier}' is a local target, scanning filesystem")
-        results = scanner.scan_local(identifier, rule_param)
+        if os.path.isdir(identifier):
+            log.debug(f"Considering that '{identifier}' as a local directory")
+            for package in os.listdir(identifier):
+                results.append({'package': package} | scanner.scan_local(f"{identifier}/{package}", rule_param))
+        else:
+            results.append({'package': identifier} | scanner.scan_local(identifier, rule_param))
     else:
         log.debug(f"Considering that '{identifier}' is a remote target")
         try:
-            results = scanner.scan_remote(identifier, version, rule_param)
+            results.append({'package': identifier} | scanner.scan_remote(identifier, version, rule_param))
         except Exception as e:
             sys.stderr.write("\n")
             sys.stderr.write(str(e))
             sys.exit()
 
     if output_format == "json":
         import json as js
-        print(js.dumps(results))
+        if len(results) == 1:
+            # return only a json like {}
+            print(js.dumps(results[0]))
+        else:
+            # Return a list of result like [{},{}]
+            print(js.dumps(results))
     else:
-        print_scan_results(results, identifier)
+        for result in results:
+            print_scan_results(result, result['package'])
 
     if exit_non_zero_on_finding:
-        exit_with_status_code(results)
+        for result in results:
+            exit_with_status_code(result)
 
 
 def _list_rules(ecosystem):
     table = PrettyTable()
     table.align = "l"
     table.field_names = ["Rule type", "Rule name", "Description"]
```

### Comparing `guarddog-1.1.4/guarddog/reporters/sarif.py` & `guarddog-1.2/guarddog/reporters/sarif.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/scanners/__init__.py` & `guarddog-1.2/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.2/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.2/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.2/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.2/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/scanners/scanner.py` & `guarddog-1.2/guarddog/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/utils/archives.py` & `guarddog-1.2/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/guarddog/utils/package_info.py` & `guarddog-1.2/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.1.4/pyproject.toml` & `guarddog-1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,45 @@
 [tool.poetry]
 name = "guarddog"
 description = "GuardDog is a CLI tool to Identify malicious PyPI packages"
 authors = ["Ellen Wang", "Christophe Tafani-Dereeper"]
 license = "Apache-2.0"
 readme = "pypi.rst"
 repository = "https://github.com/DataDog/guarddog"
-version = "v1.1.4"
+version = "v1.2"
 
 [tool.poetry.scripts]
 guarddog = "guarddog.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
-docker = "==6.0.1"
 # NOTE: Before https://github.com/returntocorp/semgrep/issues/6631 is addressed, we can't seem to upgrade past 0.112.1
 semgrep = "==0.112.1"
-requests = "==2.28.2"
-tqdm = "==4.65.0"
-python-dotenv = "==1.0.0"
-python-dateutil = "==2.8.2"
-attrs = "==21.4.0"
-boltons = "==21.0.0"
-bracex = "==2.3.post1"
-charset-normalizer = "==2.1.1"
-click = "==8.1.3"
-click-option-group = "==0.5.5"
-colorama = "==0.4.6"
-defusedxml = "==0.7.1"
-face = "==20.1.1"
-glom = "==22.1.0"
-idna = "==3.4"
-jsonschema = "==4.17.3"
-pyparsing = "==3.0.9"
-python-lsp-jsonrpc = "==1.0.0"
-six = "==1.16.0"
-typing-extensions = "==4.5.0"
-ujson = "==5.7.0"
-urllib3 = "==1.26.15"
-wcmatch = "==8.4.1"
-websocket-client = "==1.5.1"
-mypy-extensions = "==1.0.0"
-pathspec = "==0.11.1"
-platformdirs = "==3.2.0"
-tomli = "==2.0.1"
-pathos = ">=0.2.9,<0.4.0"
-pytest = "^7.1.2"
-flake8 = ">=5.0.4,<7.0.0"
+requests = "^2.29.0"
+python-dateutil = "^2.8.2"
+click = "^8.1.3"
+click-option-group = "^0.5.5"
+colorama = "^0.4.6"  # used by click
+urllib3 = "^1.26.15"
 python-whois = "^0.8.0"
 termcolor = "^2.1.0"
-setuptools = ">=65.6.3,<68.0.0"
 tarsafe = "^0.0.5"
 semantic-version = "^2.10.0"
 pyyaml = "^6.0"
-pygit2 = "^1.11.1"
+# 1.12+ requires new version of libgit2 which is not avaiable in Alpine
+pygit2 = ">=1.11,<1.13"
 configparser = "^5.3.0"
 prettytable="^3.6.0"
 
 [tool.poetry.dev-dependencies]
+mypy = "^1.4.1"
+coverage = "^7.2.7"
+flake8 = ">=5.0.4,<7.0.0"
+pytest = "^7.4.0"
+setuptools = ">=65.6.3,<69.0.0"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning"
 ]
 testpaths = [
     "tests/analyzer/metadata",
```

### Comparing `guarddog-1.1.4/PKG-INFO` & `guarddog-1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,34 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.1.4
+Version: 1.2
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (==21.4.0)
-Requires-Dist: boltons (==21.0.0)
-Requires-Dist: bracex (==2.3.post1)
-Requires-Dist: charset-normalizer (==2.1.1)
-Requires-Dist: click (==8.1.3)
-Requires-Dist: click-option-group (==0.5.5)
-Requires-Dist: colorama (==0.4.6)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click-option-group (>=0.5.5,<0.6.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
-Requires-Dist: defusedxml (==0.7.1)
-Requires-Dist: docker (==6.0.1)
-Requires-Dist: face (==20.1.1)
-Requires-Dist: flake8 (>=5.0.4,<7.0.0)
-Requires-Dist: glom (==22.1.0)
-Requires-Dist: idna (==3.4)
-Requires-Dist: jsonschema (==4.17.3)
-Requires-Dist: mypy-extensions (==1.0.0)
-Requires-Dist: pathos (>=0.2.9,<0.4.0)
-Requires-Dist: pathspec (==0.11.1)
-Requires-Dist: platformdirs (==3.2.0)
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
-Requires-Dist: pygit2 (>=1.11.1,<2.0.0)
-Requires-Dist: pyparsing (==3.0.9)
-Requires-Dist: pytest (>=7.1.2,<8.0.0)
-Requires-Dist: python-dateutil (==2.8.2)
-Requires-Dist: python-dotenv (==1.0.0)
-Requires-Dist: python-lsp-jsonrpc (==1.0.0)
+Requires-Dist: pygit2 (>=1.11,<1.13)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-whois (>=0.8.0,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (==2.28.2)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: semgrep (==0.112.1)
-Requires-Dist: setuptools (>=65.6.3,<68.0.0)
-Requires-Dist: six (==1.16.0)
 Requires-Dist: tarsafe (>=0.0.5,<0.0.6)
 Requires-Dist: termcolor (>=2.1.0,<3.0.0)
-Requires-Dist: tomli (==2.0.1)
-Requires-Dist: tqdm (==4.65.0)
-Requires-Dist: typing-extensions (==4.5.0)
-Requires-Dist: ujson (==5.7.0)
-Requires-Dist: urllib3 (==1.26.15)
-Requires-Dist: wcmatch (==8.4.1)
-Requires-Dist: websocket-client (==1.5.1)
+Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Project-URL: Repository, https://github.com/DataDog/guarddog
 Description-Content-Type: text/x-rst
 
 # GuardDog
 
 See https://github.com/datadog/guarddog
```

