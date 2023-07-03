# Comparing `tmp/personal_knowledge_library-1.0.4.tar.gz` & `tmp/personal_knowledge_library-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-1.0.4.tar", last modified: Mon Jun 26 07:14:31 2023, max compression
+gzip compressed data, was "personal_knowledge_library-1.0.5.tar", last modified: Mon Jul  3 14:40:01 2023, max compression
```

## Comparing `personal_knowledge_library-1.0.4.tar` & `personal_knowledge_library-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    80585 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/ontomapping/
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/ontomapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/ontomapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80585 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/setup.py
```

### Comparing `personal_knowledge_library-1.0.4/LICENSE` & `personal_knowledge_library-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/PKG-INFO` & `personal_knowledge_library-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.4/README.md` & `personal_knowledge_library-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/__init__.py` & `personal_knowledge_library-1.0.5/knowledge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 # Create the Logger
 logger: Union[logging.Logger, None] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-1.0.4/knowledge/base/__init__.py` & `personal_knowledge_library-1.0.5/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/base/access.py` & `personal_knowledge_library-1.0.5/knowledge/base/access.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/base/entity.py` & `personal_knowledge_library-1.0.5/knowledge/base/entity.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/base/ontology.py` & `personal_knowledge_library-1.0.5/knowledge/base/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/nel/base.py` & `personal_knowledge_library-1.0.5/knowledge/nel/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/nel/engine.py` & `personal_knowledge_library-1.0.5/knowledge/nel/engine.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/ontomapping/__init__.py` & `personal_knowledge_library-1.0.5/knowledge/ontomapping/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 Wacom. All rights reserved.
 import enum
 import json
+import logging
+import os
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, Any, List, Optional
 
 from rdflib import Graph, RDFS, URIRef
 
 from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, DataPropertyType
@@ -482,27 +484,28 @@
 
 
 # Mapping configuration
 mapping_configuration: Optional[MappingConfiguration] = None
 taxonomy_cache: Optional[Dict[str, WikidataClass]] = None
 
 
-def load_configuration():
+def load_configuration(configuration: Path = CONFIGURATION_FILE):
     """
     Loads the configuration.
 
     Raises
     ------
     ValueError
         If the configuration file is not found.
     """
-    global mapping_configuration, taxonomy_cache
-    if CONFIGURATION_FILE.exists():
+    global mapping_configuration
+    if configuration.exists():
         configuration = json.loads(CONFIGURATION_FILE.open('r').read())
         mapping_configuration = build_configuration(configuration)
+
     else:
         raise ValueError(f'Configuration file {CONFIGURATION_FILE} not found.')
 
 
 def get_mapping_configuration() -> MappingConfiguration:
     """
     Returns the mapping configuration.
@@ -510,15 +513,15 @@
     Returns
     -------
     mapping_configuration: MappingConfiguration
         The mapping configuration
     """
     global mapping_configuration
     if mapping_configuration is None:
-        load_configuration()
+        raise ValueError('Please load configuration')
     return mapping_configuration
 
 
 if taxonomy_cache is None:
     if TAXONOMY_FILE.exists():
         try:
             taxonomy = json.loads(TAXONOMY_FILE.open('r').read())
```

### Comparing `personal_knowledge_library-1.0.4/knowledge/ontomapping/manager.py` & `personal_knowledge_library-1.0.5/knowledge/ontomapping/manager.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/public/__init__.py` & `personal_knowledge_library-1.0.5/knowledge/public/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/public/cache.py` & `personal_knowledge_library-1.0.5/knowledge/public/cache.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/public/helper.py` & `personal_knowledge_library-1.0.5/knowledge/public/helper.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/public/relations.py` & `personal_knowledge_library-1.0.5/knowledge/public/relations.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/public/wikidata.py` & `personal_knowledge_library-1.0.5/knowledge/public/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/services/__init__.py` & `personal_knowledge_library-1.0.5/knowledge/services/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/services/base.py` & `personal_knowledge_library-1.0.5/knowledge/services/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/services/graph.py` & `personal_knowledge_library-1.0.5/knowledge/services/graph.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/services/group.py` & `personal_knowledge_library-1.0.5/knowledge/services/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from urllib3 import Retry
 
 from knowledge.base.access import GroupAccessRight
 from knowledge.base.ontology import NAME_TAG
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException
 from knowledge.services.graph import AUTHORIZATION_HEADER_FLAG, CONTENT_TYPE_HEADER_FLAG
 # -------------------------------------- Constant flags ----------------------------------------------------------------
-from knowledge.services.users import User
+from knowledge.services.users import User, FORCE_TAG, LIMIT_TAG, OFFSET_TAG
 
 GROUP_USER_RIGHTS_TAG: str = "groupUserRights"
 JOIN_KEY_PARAM: str = "joinKey"
 USER_TO_ADD_PARAM: str = "userToAddId"
 USER_TO_REMOVE_PARAM: str = "userToRemoveId"
 FORCE_PARAM: str = "force"
 DEFAULT_TIMEOUT: int = 30
@@ -255,76 +255,90 @@
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
             response: Response = session.patch(url, headers=headers, json=payload, verify=self.verify_calls,
                                                timeout=DEFAULT_TIMEOUT)
             if not response.ok:
                 raise WacomServiceException(f'Update of group failed.'
                                             f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def delete_group(self, auth_key: str, group_id: str):
+    def delete_group(self, auth_key: str, group_id: str, force: bool = False):
         """
          Delete a group.
 
          Parameters
          ----------
          auth_key: str
              User key.
          group_id: str
              ID of the group.
+        force: bool (Default = False)
+            If True, the group will be deleted even if it is not empty.
 
          Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
+        params: Dict[str, str] = {
+            FORCE_TAG: str(force).lower()
+        }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
                                    status_forcelist=[500, 502, 503, 504])
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
-            response: Response = session.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
+            response: Response = session.delete(url, headers=headers, params=params,
+                                                verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
             if not response.ok:
                 raise WacomServiceException(f'Deletion of group failed.'
                                             f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def listing_groups(self, auth_key: str, admin: bool = False) -> List[Group]:
+    def listing_groups(self, auth_key: str, admin: bool = False, limit: int = 20, offset: int = 0) -> List[Group]:
         """
         Listing all groups configured for this instance.
 
         Parameters
         ----------
         auth_key: str
             API key for authentication
 
         admin: bool (default:= False)
             Uses admin privilege to show all groups of the tenant.
             Requires user to have the role: TenantAdmin
+        limit: int (default:= 20)
+            Maximum number of groups to return.
+        offset: int (default:= 0)
+            Offset of the first group to return.
 
         Returns
         -------
         user:  List[Groups]
             List of groups.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}'
+        params: Dict[str, int] = {}
         if admin:
             url += '/admin'
+            params[LIMIT_TAG] = limit
+            params[OFFSET_TAG] = offset
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
                                    status_forcelist=[500, 502, 503, 504])
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
-            response: Response = session.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
+            response: Response = session.get(url, headers=headers, params=params,
+                                             verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
             if response.ok:
                 groups: List[Dict[str, Any]] = response.json()
                 return [Group.parse(g) for g in groups]
         raise WacomServiceException(f'Listing of group failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def group(self, auth_key: str, group_id: str) -> GroupInfo:
```

### Comparing `personal_knowledge_library-1.0.4/knowledge/services/ontology.py` & `personal_knowledge_library-1.0.5/knowledge/services/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/services/tenant.py` & `personal_knowledge_library-1.0.5/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/services/users.py` & `personal_knowledge_library-1.0.5/knowledge/services/users.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/utils/rdf.py` & `personal_knowledge_library-1.0.5/knowledge/utils/rdf.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/knowledge/utils/wikipedia.py` & `personal_knowledge_library-1.0.5/knowledge/utils/wikipedia.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.4/setup.py` & `personal_knowledge_library-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
 """)
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
```

