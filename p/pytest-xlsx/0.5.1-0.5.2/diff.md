# Comparing `tmp/pytest_xlsx-0.5.1-py3-none-any.whl.zip` & `tmp/pytest_xlsx-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 15408 bytes, number of entries: 14
+Zip file size: 15451 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pytest_xlsx/__init__.py
--rw-r--r--  2.0 unx     2728 b- defN 16-Jan-01 00:00 pytest_xlsx/_plugin.py
--rw-r--r--  2.0 unx     7947 b- defN 16-Jan-01 00:00 pytest_xlsx/file.py
--rw-r--r--  2.0 unx     7074 b- defN 16-Jan-01 00:00 pytest_xlsx/funcs.py
+-rw-r--r--  2.0 unx     2727 b- defN 16-Jan-01 00:00 pytest_xlsx/_plugin.py
+-rw-r--r--  2.0 unx     7962 b- defN 16-Jan-01 00:00 pytest_xlsx/file.py
+-rw-r--r--  2.0 unx     7104 b- defN 16-Jan-01 00:00 pytest_xlsx/funcs.py
 -rw-r--r--  2.0 unx      673 b- defN 16-Jan-01 00:00 pytest_xlsx/hooks.py
--rw-r--r--  2.0 unx      219 b- defN 16-Jan-01 00:00 pytest_xlsx/models.py
--rw-r--r--  2.0 unx     2783 b- defN 16-Jan-01 00:00 pytest_xlsx/plugin.py
+-rw-r--r--  2.0 unx      218 b- defN 16-Jan-01 00:00 pytest_xlsx/models.py
+-rw-r--r--  2.0 unx     2782 b- defN 16-Jan-01 00:00 pytest_xlsx/plugin.py
 -rw-r--r--  2.0 unx      328 b- defN 16-Jan-01 00:00 pytest_xlsx/runner.py
--rw-r--r--  2.0 unx      551 b- defN 16-Jan-01 00:00 pytest_xlsx/settings.py
-?rw-------  2.0 unx       36 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.1.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.1.dist-info/WHEEL
-?rw-------  2.0 unx     1253 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx    11341 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.1.dist-info/licenses/LICENSE.md
-?rw-------  2.0 unx     1118 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.1.dist-info/RECORD
-14 files, 36138 bytes uncompressed, 13554 bytes compressed:  62.5%
+-rw-r--r--  2.0 unx      559 b- defN 16-Jan-01 00:00 pytest_xlsx/settings.py
+?rw-------  2.0 unx       36 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.2.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.2.dist-info/WHEEL
+?rw-------  2.0 unx     1297 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx    11341 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.2.dist-info/licenses/LICENSE.md
+?rw-------  2.0 unx     1118 b- defN 16-Jan-01 00:00 pytest_xlsx-0.5.2.dist-info/RECORD
+14 files, 36232 bytes uncompressed, 13597 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: pytest_xlsx/runner.py
 Comment: 
 
 Filename: pytest_xlsx/settings.py
 Comment: 
 
-Filename: pytest_xlsx-0.5.1.dist-info/entry_points.txt
+Filename: pytest_xlsx-0.5.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_xlsx-0.5.1.dist-info/WHEEL
+Filename: pytest_xlsx-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_xlsx-0.5.1.dist-info/METADATA
+Filename: pytest_xlsx-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: pytest_xlsx-0.5.1.dist-info/licenses/LICENSE.md
+Filename: pytest_xlsx-0.5.2.dist-info/licenses/LICENSE.md
 Comment: 
 
-Filename: pytest_xlsx-0.5.1.dist-info/RECORD
+Filename: pytest_xlsx-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_xlsx/_plugin.py

```diff
@@ -54,15 +54,14 @@
 class AllureXlsxPlugin(XlsxPlugin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta_column_name = self.config.getini("xlsx_meta_column_name")
 
     @pytest.hookimpl(tryfirst=True)
     def pytest_xlsx_run_step(self, item: XlsxItem, request: FixtureRequest):
-
         if self.meta_column_name not in item.current_step:
             return
 
         keys = list(item.current_step)
         arg_column_index = keys.index(self.meta_column_name) + 1
         if len(keys) <= arg_column_index:
             return None
```

## pytest_xlsx/file.py

```diff
@@ -26,15 +26,14 @@
     def collect(self):
         for sheet in funcs.iter_xlsx_sheet(self.path):
             logger.debug(f"{self.path.absolute()} -> {sheet.title=}")
             yield XlsxSheet.from_parent(self, name=sheet.title, obj=sheet)
 
 
 class XlsxSheet(pytest.Class):
-
     xlsx_data: models.Suite
 
     @classmethod
     def from_parent(cls, parent, *, name, obj=None, **kw):
         _ = super().from_parent(parent, name=name, **kw)
         _.obj = models.Suite(**dict(funcs.SheetHandler(obj).to_dict()))
 
@@ -114,21 +113,21 @@
     ):
         logger.debug(f"parametrize = {parametrize_marks}")
         arg_names = [i[0].split(",") for i in parametrize_marks]
         arg_vals = [funcs.LoadData(parent.path, i[1]).data for i in parametrize_marks]
 
         keys = [key.strip() for key in get_value_by_sequence(*arg_names)]
 
-        case_str = case.json()
+        case_str = case.model_dump_json()
 
         for vals in itertools.product(*arg_vals):
             values = list(get_value_by_sequence(*vals))
 
             data_str = Template(case_str).safe_substitute(dict(zip(keys, values)))
-            new_case = models.Case.parse_obj(json.loads(data_str))
+            new_case = models.Case.model_validate(json.loads(data_str))
             new_case.meta["name"][0][0] += str(values)
             new_case.meta["mark"] = list(
                 filter(lambda i: i[0] != "parametrize", new_case.meta["mark"])
             )
             yield from _case_to_xlsx_item(0, new_case, parent)
 
     def _call_obj(self, request: pytest.FixtureRequest):
```

## pytest_xlsx/funcs.py

```diff
@@ -88,15 +88,14 @@
             "meta": {},
             "steps": [],
         }
 
         self.headers_map = self._get_headers_map()
 
         if debug is False:
-
             self.contents = list(self._get_contents())
             self.make_case_list(self.contents)
 
     def _get_headers_map(self) -> dict[Optional[str], list[int]]:
         logger.debug("加载表头")
         for row_index, row_content in enumerate(
             self.ws.iter_rows(values_only=True, max_row=1),
@@ -176,15 +175,14 @@
         return content_type
 
     def make_case_list(self, contents):
         for content in contents:
             self._parse_content(content)
 
     def to_dict(self):
-
         return OrderedDict({"name": self.ws.title, "case_list": self.case_list})
 
 
 class LoadData:
     """
     尝试多种方式加载数据：
         - json加载
@@ -218,19 +216,18 @@
         return self._data
 
     def try_json(self):
         return json.loads(self.row_data)
 
     def try_str(self):
         if "," in self.row_data:
-
             return self.row_data.replace(" ", "").split(",")
 
     def try_file(self):
-
+        # todo 支持绝对路径
         path = self.path.parent / self.row_data
         if not path.exists():
             return
 
         data = None
         match path.suffix:
             case ".json":
```

## pytest_xlsx/models.py

```diff
@@ -6,10 +6,9 @@
 class Case(BaseModel):
     id: int
     meta: dict[str, list[list[str]]]
     steps: List[dict]
 
 
 class Suite(BaseModel):
-
     name: str
     case_list: List[Case]
```

## pytest_xlsx/plugin.py

```diff
@@ -89,11 +89,10 @@
     if report.fspath.endswith(".xlsx"):
         from py.xml import html
 
         cells[1] = html.td(report.nodeid, class_="col-name")
 
 
 def pytest_collect_file(parent, file_path: Path):
-
     if file_path.suffix == ".xlsx" and file_path.name.startswith("test"):
         logger.debug(f"XlsxFile: {file_path.absolute()}")
         return XlsxFile.from_parent(parent, path=file_path)
```

## pytest_xlsx/settings.py

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings
 
 
 class Settings(BaseSettings):
     meta_column_name: str = "meta_flag"
 
 
 class ProxySettings:
@@ -17,12 +17,11 @@
     def __setattr__(self, key, value):
         if key == "_obj":
             self.__dict__[key] = value
         else:
             setattr(self._obj, key, value)
 
     def reload_settings(self, d):
-
         self._obj = Settings(**d)
 
 
 settings: Settings = ProxySettings()
```

## Comparing `pytest_xlsx-0.5.1.dist-info/METADATA` & `pytest_xlsx-0.5.2.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pytest-xlsx
-Version: 0.5.1
+Version: 0.5.2
 Summary: pytest plugin for generating test cases by xlsx(excel)
 License: Apache-2.0
 Author: dongfangtianyu
 Requires-Python: >=3.10
 Requires-Dist: allure-pytest>=2.12.0
 Requires-Dist: openpyxl>=3.0.10
-Requires-Dist: pydantic>=1.9.1
+Requires-Dist: pydantic-settings>=2.0.0
+Requires-Dist: pydantic<3,>=2.0
 Requires-Dist: pytest-html>=3.2.0
 Requires-Dist: pytest-result-log>=1.0.0
-Requires-Dist: pytest>=7.2.0
+Requires-Dist: pytest<8,>=7.4.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: tabulate[widechars]>=0.9.0
 Requires-Dist: wcwidth>=0.2.5
 Project-URL: Homepage, https://github.com/dongfangtianyu/pytest-xlsx
 Description-Content-Type: text/markdown
 
 # pytest-xlsx
```

## Comparing `pytest_xlsx-0.5.1.dist-info/licenses/LICENSE.md` & `pytest_xlsx-0.5.2.dist-info/licenses/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pytest_xlsx-0.5.1.dist-info/RECORD` & `pytest_xlsx-0.5.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pytest_xlsx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pytest_xlsx/_plugin.py,sha256=QwtWUw4S_9qSXzCqgzbugK4a6cj7fdCMGoVCEB6M1z4,2728
-pytest_xlsx/file.py,sha256=_1sEllk41whThW8HrwRytLZpJphUngRd75yksLA1-is,7947
-pytest_xlsx/funcs.py,sha256=wBLoSuAouAdVWYR7BYn1GtBTiTmP3Y8Qp8BHLoGNJXA,7074
+pytest_xlsx/_plugin.py,sha256=xOUzNvBl4vF8qJtl05-PbhUkS_f9oP1hAjIklnkwHWE,2727
+pytest_xlsx/file.py,sha256=KGiwWotVtjQelhc2VL1yQv54jMsisrZdAfSNxsbn4n8,7962
+pytest_xlsx/funcs.py,sha256=6A_d8ErhFS_sYHVshnIT3VcI97FKzM9gxAlkV_Zric4,7104
 pytest_xlsx/hooks.py,sha256=5QGE9qwv-bFYEy847MAYs1Jyyz3b5AVUXpM8DQM7PQ0,673
-pytest_xlsx/models.py,sha256=P51YV6Bt1fLEKPryL2mnT4B9kNgl0N7g03b9hOqUA-c,219
-pytest_xlsx/plugin.py,sha256=aacrOiaTpP7u6ZdkGYxtq08fs36zHpzaJ7zeGRE-Koc,2783
+pytest_xlsx/models.py,sha256=XxfNvbZYjdlZFDQyUYzl7SaOMBzAoRz2sSW_kMfAh9U,218
+pytest_xlsx/plugin.py,sha256=Q_RLOhwrFrCKid-iYcDsIiinB-vN4DhQYjBz-HFhRt8,2782
 pytest_xlsx/runner.py,sha256=pT2bZjmma2k3fzoAUlEZgG0fSQnVf9YP3uTAuNBbYfw,328
-pytest_xlsx/settings.py,sha256=sc4kjGcWMGJrJT0jXDMcNtAlWRDimoN6Dr-a6ncCY4U,551
-pytest_xlsx-0.5.1.dist-info/entry_points.txt,sha256=PkBf7zbtxAqd-aOE4jOqyj1Rh2m9Geb6Ehs1Nys9xVg,36
-pytest_xlsx-0.5.1.dist-info/WHEEL,sha256=JtIceljpZF_3FlF7JEESqvYUELdenaIGNR7wSL2mRl0,87
-pytest_xlsx-0.5.1.dist-info/METADATA,sha256=l8xn-LuVw4VoYf8ZzOKRuM8KTfGh23fvY0STNyMUQIk,1253
-pytest_xlsx-0.5.1.dist-info/licenses/LICENSE.md,sha256=6qhOc97sqEXSxt28gu1PqN796LEMcgvHvdkh9drcpXc,11341
-pytest_xlsx-0.5.1.dist-info/RECORD,,
+pytest_xlsx/settings.py,sha256=05a0kHyMI9qUoIVk70caY9wCbi6poP1bvQw-w-F1M4M,559
+pytest_xlsx-0.5.2.dist-info/entry_points.txt,sha256=PkBf7zbtxAqd-aOE4jOqyj1Rh2m9Geb6Ehs1Nys9xVg,36
+pytest_xlsx-0.5.2.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
+pytest_xlsx-0.5.2.dist-info/METADATA,sha256=7TkjIhCN-cZFruDa4AdrCW6U-XOLFMs6Kw8_DEJpY98,1297
+pytest_xlsx-0.5.2.dist-info/licenses/LICENSE.md,sha256=6qhOc97sqEXSxt28gu1PqN796LEMcgvHvdkh9drcpXc,11341
+pytest_xlsx-0.5.2.dist-info/RECORD,,
```

