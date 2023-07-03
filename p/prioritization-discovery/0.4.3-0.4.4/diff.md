# Comparing `tmp/prioritization_discovery-0.4.3.tar.gz` & `tmp/prioritization_discovery-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prioritization_discovery-0.4.3.tar", max compression
+gzip compressed data, was "prioritization_discovery-0.4.4.tar", max compression
```

## Comparing `prioritization_discovery-0.4.3.tar` & `prioritization_discovery-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11349 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/LICENSE
--rw-r--r--   0        0        0     2040 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/README.md
--rw-r--r--   0        0        0      702 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       43 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/__init__.py
--rw-r--r--   0        0        0      883 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/config.py
--rw-r--r--   0        0        0     4984 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/discovery.py
--rw-r--r--   0        0        0    12584 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/rules.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 prioritization_discovery-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-03 19:10:16.674701 prioritization_discovery-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2018 2023-07-03 19:10:16.674701 prioritization_discovery-0.4.4/README.md
+-rw-r--r--   0        0        0      702 2023-07-03 19:10:16.674701 prioritization_discovery-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-03 19:10:16.674701 prioritization_discovery-0.4.4/src/prioritization_discovery/__init__.py
+-rw-r--r--   0        0        0      883 2023-07-03 19:10:16.674701 prioritization_discovery-0.4.4/src/prioritization_discovery/config.py
+-rw-r--r--   0        0        0     4984 2023-07-03 19:10:16.674701 prioritization_discovery-0.4.4/src/prioritization_discovery/discovery.py
+-rw-r--r--   0        0        0    12175 2023-07-03 19:10:16.674701 prioritization_discovery-0.4.4/src/prioritization_discovery/rules.py
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 prioritization_discovery-0.4.4/PKG-INFO
```

### Comparing `prioritization_discovery-0.4.3/LICENSE` & `prioritization_discovery-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.3/README.md` & `prioritization_discovery-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Prioritization Discovery
 
-![case-attribute-discovery](https://github.com/AutomatedProcessImprovement/prioritization-discovery/actions/workflows/build.yaml/badge.svg)
+![ci](https://github.com/AutomatedProcessImprovement/prioritization-discovery/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/prioritization-discovery)
 
 Python algorithm to discover, from an event log, the case priority levels and the rules that classify a process case in its corresponding
 level. For example, the cases of a process can belong to three priority levels (low, medium, high), where the activity instances of cases
 with high priority are executed before than activity instances of cases with low priority (when both of them are enabled at the same time).
 
 ### Example of use
```

### Comparing `prioritization_discovery-0.4.3/pyproject.toml` & `prioritization_discovery-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prioritization-discovery"
-version = "0.4.3"
+version = "0.4.4"
 description = "Python algorithm to discover, from an event log, prioritization rules that lead to one activity instance to be executed before another."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "prioritization_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `prioritization_discovery-0.4.3/src/prioritization_discovery/config.py` & `prioritization_discovery-0.4.4/src/prioritization_discovery/config.py`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.3/src/prioritization_discovery/discovery.py` & `prioritization_discovery-0.4.4/src/prioritization_discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.3/src/prioritization_discovery/rules.py` & `prioritization_discovery-0.4.4/src/prioritization_discovery/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,16 +103,16 @@
         if tree_.feature[current_node] != _tree.TREE_UNDEFINED:
             # Decision node: add rule and keep search through each child
             name = feature_name[current_node]
             threshold = tree_.threshold[current_node]
             # Add ID and rule for left and right children
             missing_nodes += [tree_.children_left[current_node], tree_.children_right[current_node]]
             current_rules += [
-                current_rule + [{"attribute": name, "condition": "<=", "value": threshold}],
-                current_rule + [{"attribute": name, "condition": ">", "value": threshold}],
+                current_rule + [{'attribute': name, 'comparison': '<=', 'value': threshold}],
+                current_rule + [{'attribute': name, 'comparison': '>', 'value': threshold}]
             ]
         else:
             # Leaf node
             current_impurity = tree_.impurity[current_node]
             current_sample_sizes = tree_.value[current_node][0]  # Number of positive samples
             # If it is the best leaf node, save it
             if current_sample_sizes[0] < current_sample_sizes[1] and (  # Less samples with negative outcome
@@ -127,50 +127,34 @@
 
 
 def _summarize_rules(rules: list) -> list:
     filtered_rules = []
     # Merge rules by same feature
     attributes = {rule["attribute"] for rule in rules}
     for attribute in attributes:
-        operators = {rule["condition"] for rule in rules if rule["attribute"] == attribute}
+        operators = {rule['comparison'] for rule in rules if rule['attribute'] == attribute}
         if len(operators) > 1:
             # Add interval rule
-            filtered_rules += [
-                {
-                    "attribute": attribute,
-                    "condition": "in",
-                    "value": "({},{}]".format(
-                        max(
-                            [
-                                rule["value"]
-                                for rule in rules
-                                if rule["attribute"] == attribute and rule["condition"] == ">"
-                            ]
-                        ),
-                        min(
-                            [
-                                rule["value"]
-                                for rule in rules
-                                if rule["attribute"] == attribute and rule["condition"] == "<="
-                            ]
-                        ),
-                    ),
-                }
-            ]
+            filtered_rules += [{
+                'attribute': attribute,
+                'comparison': 'in',
+                'value': "({},{}]".format(
+                    max([rule['value'] for rule in rules if rule['attribute'] == attribute and rule['comparison'] == ">"]),
+                    min([rule['value'] for rule in rules if rule['attribute'] == attribute and rule['comparison'] == "<="])
+                )
+            }]
         else:
             # Add single rule
             operator = operators.pop()
-            values = [rule["value"] for rule in rules if rule["attribute"] == attribute]
-            filtered_rules += [
-                {
-                    "attribute": attribute,
-                    "condition": operator,
-                    "value": str(min(values)) if operator == "<=" else str(max(values)),
-                }
-            ]
+            values = [rule['value'] for rule in rules if rule['attribute'] == attribute]
+            filtered_rules += [{
+                'attribute': attribute,
+                'comparison': operator,
+                'value': str(min(values)) if operator == "<=" else str(max(values))
+            }]
     # Return rules
     return filtered_rules
 
 
 def _predict(rules: list, data: pd.DataFrame) -> list:
     predictions = []
     # Predict each observation
@@ -185,18 +169,18 @@
 
 
 def _fulfill_ruleset(rules: list, observation: pd.Series):
     fulfills = True
     for rule in rules:
         values = [float(value) for value in re.findall(r"[\d.]+", rule["value"])]
         if (
-            (rule["condition"] == "<=" and observation[rule["attribute"]] > values[0])
-            or (rule["condition"] == ">" and observation[rule["attribute"]] <= values[0])
-            or (rule["condition"] == "in" and observation[rule["attribute"]] <= values[0])
-            or (rule["condition"] == "in" and observation[rule["attribute"]] > values[1])
+                (rule['comparison'] == "<=" and observation[rule['attribute']] > values[0]) or
+                (rule['comparison'] == ">" and observation[rule['attribute']] <= values[0]) or
+                (rule['comparison'] == "in" and observation[rule['attribute']] <= values[0]) or
+                (rule['comparison'] == "in" and observation[rule['attribute']] > values[1])
         ):
             fulfills = False
     return fulfills
 
 
 def _reverse_one_hot_encoding(model: list, dummy_columns: dict, data: pd.DataFrame) -> list:
     # Deep copy of the list
@@ -222,46 +206,48 @@
     diff_than_attributes = {  # Empty list for each attribute to store the assigned values
         attribute: [] for attribute in dummy_columns
     }
     equal_to_attributes = []  # Attributes with a rule '='
     rules_to_remove = []  # Indices of the rules to remove because of redundancy
     # Parse each rule in the ruleset
     for rule in ruleset:
-        if rule["attribute"] in dummy_map:
-            (orig_name, orig_value) = dummy_map[rule["attribute"]]
-            rule["attribute"] = orig_name
-            rule["value"] = orig_value
-            if rule["condition"] == ">":
-                rule["condition"] = "="
+        if rule['attribute'] in dummy_map:
+            (orig_name, orig_value) = dummy_map[rule['attribute']]
+            rule['attribute'] = orig_name
+            rule['value'] = orig_value
+            if rule['comparison'] == ">":
+                rule['comparison'] = "="
                 equal_to_attributes += [orig_name]
             else:
-                rule["condition"] = "!="
+                rule['comparison'] = "!="
                 diff_than_attributes[orig_name] += [orig_value]
     # Remove rules with '!=' if there's also a rule with '='
     for attribute in set(equal_to_attributes):
-        rules_to_remove += [  # Get the index of the rules of this attribute with "!=" condition
-            index for index, rule in enumerate(ruleset) if rule["attribute"] == attribute and rule["condition"] == "!="
+        rules_to_remove += [  # Get the index of the rules of this attribute with "!=" comparison
+            index
+            for index, rule in enumerate(ruleset)
+            if rule['attribute'] == attribute and rule['comparison'] == "!="
         ]
     # Check if any categorical rule with N possible values got N-1 times '!=' (meaning it's '=' to the missing value).
     for attribute in diff_than_attributes:
         if (
             attribute not in equal_to_attributes
             and len(diff_than_attributes[attribute]) > 0
             and len(diff_than_attributes[attribute]) == len(dummy_columns[attribute]) - 1
         ):
             # Attribute has N possible values, and N-1 rules saying 'different from', simplify it
             new_rule = {
-                "attribute": attribute,
-                "condition": "=",
-                "value": [  # Get the missing value in all "!=" rules for this attribute
-                    value for value in dummy_columns[attribute] if value not in diff_than_attributes[attribute]
-                ][
-                    0
-                ],  # Get the first element (there should be only one)
+                'attribute': attribute,
+                'comparison': "=",
+                'value': [  # Get the missing value in all "!=" rules for this attribute
+                    value
+                    for value in dummy_columns[attribute]
+                    if value not in diff_than_attributes[attribute]
+                ][0]  # Get the first element (there should be only one)
             }
-            # Get the index of the rules of this attribute with "!=" condition
-            rules_to_remove += [index for index, rule in enumerate(ruleset) if rule["attribute"] == attribute]
+            # Get the index of the rules of this attribute with "!=" comparison
+            rules_to_remove += [index for index, rule in enumerate(ruleset) if rule['attribute'] == attribute]
             # Add new rule to ruleset
             ruleset += [new_rule]
     # Remove redundant rules
     for i in sorted(rules_to_remove, reverse=True):
         del ruleset[i]
```

### Comparing `prioritization_discovery-0.4.3/PKG-INFO` & `prioritization_discovery-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prioritization-discovery
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python algorithm to discover, from an event log, prioritization rules that lead to one activity instance to be executed before another.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,15 +12,15 @@
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandasql (>=0.7.3,<0.8.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prioritization Discovery
 
-![case-attribute-discovery](https://github.com/AutomatedProcessImprovement/prioritization-discovery/actions/workflows/build.yaml/badge.svg)
+![ci](https://github.com/AutomatedProcessImprovement/prioritization-discovery/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/prioritization-discovery)
 
 Python algorithm to discover, from an event log, the case priority levels and the rules that classify a process case in its corresponding
 level. For example, the cases of a process can belong to three priority levels (low, medium, high), where the activity instances of cases
 with high priority are executed before than activity instances of cases with low priority (when both of them are enabled at the same time).
 
 ### Example of use
```

