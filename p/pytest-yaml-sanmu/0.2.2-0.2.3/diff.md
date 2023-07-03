# Comparing `tmp/pytest_yaml_sanmu-0.2.2-py3-none-any.whl.zip` & `tmp/pytest_yaml_sanmu-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8192 bytes, number of entries: 11
+Zip file size: 8194 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pytest_yaml/__init__.py
 -rw-r--r--  2.0 unx     1810 b- defN 16-Jan-01 00:00 pytest_yaml/_plugin.py
--rw-r--r--  2.0 unx     7039 b- defN 16-Jan-01 00:00 pytest_yaml/file.py
+-rw-r--r--  2.0 unx     7045 b- defN 16-Jan-01 00:00 pytest_yaml/file.py
 -rw-r--r--  2.0 unx      661 b- defN 16-Jan-01 00:00 pytest_yaml/hooks.py
--rw-r--r--  2.0 unx      868 b- defN 16-Jan-01 00:00 pytest_yaml/models.py
+-rw-r--r--  2.0 unx      874 b- defN 16-Jan-01 00:00 pytest_yaml/models.py
 -rw-r--r--  2.0 unx     1425 b- defN 16-Jan-01 00:00 pytest_yaml/plugin.py
 -rw-r--r--  2.0 unx     2350 b- defN 16-Jan-01 00:00 pytest_yaml/templates.py
-?rw-------  2.0 unx       36 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/WHEEL
-?rw-------  2.0 unx     1859 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/METADATA
-?rw-------  2.0 unx      885 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/RECORD
-11 files, 17020 bytes uncompressed, 6692 bytes compressed:  60.7%
+?rw-------  2.0 unx       36 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.3.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.3.dist-info/WHEEL
+?rw-------  2.0 unx     1859 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.3.dist-info/METADATA
+?rw-------  2.0 unx      885 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.3.dist-info/RECORD
+11 files, 17032 bytes uncompressed, 6694 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pytest_yaml/plugin.py
 Comment: 
 
 Filename: pytest_yaml/templates.py
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.2.dist-info/entry_points.txt
+Filename: pytest_yaml_sanmu-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.2.dist-info/WHEEL
+Filename: pytest_yaml_sanmu-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.2.dist-info/METADATA
+Filename: pytest_yaml_sanmu-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.2.dist-info/RECORD
+Filename: pytest_yaml_sanmu-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_yaml/file.py

```diff
@@ -113,15 +113,15 @@
             arg_names.extend(str_or_list(i["parametrize"]["keys"]))
 
         arg_vals = []
         for i in parametrize_marks:
             vals = i["parametrize"]["vals"]
             arg_vals.append(vals)
 
-        template_case: Case = case.copy()
+        template_case: Case = case.model_copy()
         template_case.mark = [m for m in case.mark if not is_parametrize(m)]
         case_str = template_case.to_yaml()
         # logger.warning(f"{case_str=}")
 
         for vals in itertools.product(*arg_vals):
             vals = list(get_value_by_sequence(*vals))
             case_yaml = Template(case_str).safe_substitute(dict(zip(arg_names, vals)))
```

## pytest_yaml/models.py

```diff
@@ -23,13 +23,13 @@
         :return:
         """
         # print(case_dict)
 
         return cls(**case_dict)
 
     def to_yaml(self):
-        return yaml.dump(self.dict(), allow_unicode=True, sort_keys=False)
+        return yaml.dump(self.model_dump(), allow_unicode=True, sort_keys=False)
 
     @classmethod
     def from_yaml(cls, yaml_str):
         data = yaml.safe_load(yaml_str)
         return cls(**data)
```

## Comparing `pytest_yaml_sanmu-0.2.2.dist-info/METADATA` & `pytest_yaml_sanmu-0.2.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-sanmu
-Version: 0.2.2
+Version: 0.2.3
 Summary: pytest plugin for generating test cases by yaml
 License: Apache-2.0
 Author-email: dongfangtianyu <7629022+dongfangtianyu@users.noreply.github.com>
 Requires-Python: >=3.10
 Requires-Dist: allure-pytest>=2.13.0
-Requires-Dist: pydantic>=1.10.4
-Requires-Dist: pytest>=7.2.0
+Requires-Dist: pydantic<3,>=2.0
+Requires-Dist: pytest>=7.4.0
 Requires-Dist: pyyaml>=6.0
 Project-URL: Homepage, https://github.com/dongfangtianyu/pytest-yaml-sanmul
 Description-Content-Type: text/markdown
 
 # pytest-yml
 
 pytest plugin for generating test cases by yaml
```

## Comparing `pytest_yaml_sanmu-0.2.2.dist-info/RECORD` & `pytest_yaml_sanmu-0.2.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pytest_yaml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytest_yaml/_plugin.py,sha256=QSTtELd_duC7uw0cKt8pfM67jonbzIlUMgYrdCD1_dE,1810
-pytest_yaml/file.py,sha256=YCm2hjOrcLhRUpnx7gIoiFJ-IPQM8ufMO2avf02m3EA,7039
+pytest_yaml/file.py,sha256=z9_r20We010Fifw4x8XevEGBEW4fybtMa12Kn3BPgPw,7045
 pytest_yaml/hooks.py,sha256=cclZKDIxTpWoRFZHqXzukmSwPjpmx8aH1iSWhs0Io8o,661
-pytest_yaml/models.py,sha256=2hBsq9K2XUYVjmJcykv8CvezdeXiMbLcGNIYl7OGanM,868
+pytest_yaml/models.py,sha256=ZeBqFcCSx6y7sZn6dSR5-PT0Z3icZx95v_vjA7Hil78,874
 pytest_yaml/plugin.py,sha256=Z69brEVc5wZVvFYMUfqd1iAUt_RmaBtHN8C1kLYzmwM,1425
 pytest_yaml/templates.py,sha256=eMxiigvnqC2p88S4cbzqodddXWKLgdmdTdvrJE2YUrs,2350
-pytest_yaml_sanmu-0.2.2.dist-info/entry_points.txt,sha256=pEQ-BthnhQfWoRegIMd3s8W8oR9tMHZz_soP_RAGXTs,36
-pytest_yaml_sanmu-0.2.2.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
-pytest_yaml_sanmu-0.2.2.dist-info/METADATA,sha256=O5UdjneUix99VIQHVHn7-VRIVA0nTqPGkte-ZQ_uMd0,1859
-pytest_yaml_sanmu-0.2.2.dist-info/RECORD,,
+pytest_yaml_sanmu-0.2.3.dist-info/entry_points.txt,sha256=pEQ-BthnhQfWoRegIMd3s8W8oR9tMHZz_soP_RAGXTs,36
+pytest_yaml_sanmu-0.2.3.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
+pytest_yaml_sanmu-0.2.3.dist-info/METADATA,sha256=5Z4HD0qLZQruUDUW8CdUUvwIGPLCL2PQxAh_9ComBBw,1859
+pytest_yaml_sanmu-0.2.3.dist-info/RECORD,,
```

