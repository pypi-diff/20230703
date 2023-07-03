# Comparing `tmp/langchain_wenxin-0.6.0.tar.gz` & `tmp/langchain_wenxin-0.7.0.tar.gz`

## Comparing `langchain_wenxin-0.6.0.tar` & `langchain_wenxin-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/chat_models.py
--rw-r--r--   0        0        0    17115 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/chat_models/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/chat_models/test_wenxin.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/llms/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/llms/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/tools/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/tools/test_callbacks.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/README.md
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/chat_models.py
+-rw-r--r--   0        0        0    17115 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/chat_models/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/chat_models/test_wenxin.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/llms/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/llms/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/tools/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/tools/test_callbacks.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/README.md
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/PKG-INFO
```

### Comparing `langchain_wenxin-0.6.0/src/langchain_wenxin/chat_models.py` & `langchain_wenxin-0.7.0/src/langchain_wenxin/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.6.0/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.7.0/src/langchain_wenxin/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.6.0/src/langchain_wenxin/retrievers.py` & `langchain_wenxin-0.7.0/src/langchain_wenxin/retrievers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import requests
 from langchain.docstore.document import Document
 from langchain.schema import BaseRetriever
 
 
 @dataclass
 class BaizhongSearchParams:
-    # 查询库索引,与项目ID一致
+    # 查询库索引，与项目 ID 一致
     project_id: int
-    # 返回query相关内容数量
+    # 返回 query 相关内容数量
     size: int
-    # faiss检索返回数量
+    # faiss 检索返回数量
     db_top: Optional[int] = None
     # 精排排序结果条数
     rank_top: Optional[int] = None
     # 参与精排的最大条数
     rank_size: Optional[int] = None
     # 过滤精排分数低于该值的结果
     doc_score: Optional[float] = None
@@ -101,26 +101,28 @@
 
     async def aget_relevant_documents(self, query: str) -> List[Document]:
         raise NotImplementedError
 
 
 def find_outliers(data: List[float], max_size: int):
     """计算离群值，data 必须是一个倒序排列的数组"""
+    if len(data) <= max_size:
+        return data
     # 计算相邻元素的差值
     diff = [data[i] - data[i+1] for i in range(len(data) - 1)]
     # 计算平均差值
     avg_diff = np.mean(diff)
     # 离群值列表
     outliers = []
     # 从数组的开始处检查每个元素
     for i in range(len(data) - 1):
         # 如果元素与其后续元素的差值大于平均差值
         if (data[i] - data[i+1]) > avg_diff:
             outliers.append(data[i])
-            # 如果找到3个离群值则退出循环
+            # 如果找到 3 个离群值则退出循环
             if len(outliers) == max_size:
                 break
     # 如果没有找到离群值，返回数组中的最大值作为一个离群值
     if not outliers:
         outliers.append(data[0])
 
     return outliers
```

### Comparing `langchain_wenxin-0.6.0/tests/integration_tests/chat_models/test_wenxin.py` & `langchain_wenxin-0.7.0/tests/integration_tests/chat_models/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.6.0/tests/integration_tests/llms/test_wenxin.py` & `langchain_wenxin-0.7.0/tests/integration_tests/llms/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.6.0/tests/tools/test_callbacks.py` & `langchain_wenxin-0.7.0/tests/tools/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.6.0/.gitignore` & `langchain_wenxin-0.7.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.DS_Store
```

### Comparing `langchain_wenxin-0.6.0/LICENSE.txt` & `langchain_wenxin-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.6.0/README.md` & `langchain_wenxin-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.6.0/pyproject.toml` & `langchain_wenxin-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "langchain-wenxin"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Tao Yang", email = "swulling@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `langchain_wenxin-0.6.0/PKG-INFO` & `langchain_wenxin-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.6.0
+Version: 0.7.0
 Project-URL: Documentation, https://github.com/unknown/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/unknown/langchain-wenxin/issues
 Project-URL: Source, https://github.com/unknown/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: langchain>=0.0.175
 Requires-Dist: numpy
 Requires-Dist: requests
 Requires-Dist: sseclient-py
 Description-Content-Type: text/markdown
```

