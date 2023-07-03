# Comparing `tmp/configcat-client-7.0.1.tar.gz` & `tmp/configcat-client-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configcat-client-7.0.1.tar", last modified: Mon Mar 20 10:30:31 2023, max compression
+gzip compressed data, was "configcat-client-8.0.0.tar", last modified: Mon Jul  3 11:08:40 2023, max compression
```

## Comparing `configcat-client-7.0.1.tar` & `configcat-client-8.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:30:31.092011 configcat-client-7.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-20 10:30:14.000000 configcat-client-7.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-20 10:30:14.000000 configcat-client-7.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-20 10:30:14.000000 configcat-client-7.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-20 10:30:31.092011 configcat-client-7.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-03-20 10:30:14.000000 configcat-client-7.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:30:31.092011 configcat-client-7.0.1/configcat_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-20 10:30:31.000000 configcat-client-7.0.1/configcat_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-20 10:30:31.000000 configcat-client-7.0.1/configcat_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:30:31.000000 configcat-client-7.0.1/configcat_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-20 10:30:31.000000 configcat-client-7.0.1/configcat_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-20 10:30:31.000000 configcat-client-7.0.1/configcat_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:30:31.092011 configcat-client-7.0.1/configcatclient/
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/configcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/configcatclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/configcatoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/configentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/configfetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/configservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/datagovernance.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/evaluationdetails.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/localdictionarydatasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/localfiledatasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/overridedatasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/pollingmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/refreshresult.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/rolloutevaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-20 10:30:14.000000 configcat-client-7.0.1/configcatclient/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-20 10:30:14.000000 configcat-client-7.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-20 10:30:31.092011 configcat-client-7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-20 10:30:14.000000 configcat-client-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:08:40.717530 configcat-client-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 11:08:29.000000 configcat-client-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 11:08:29.000000 configcat-client-8.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 11:08:29.000000 configcat-client-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-03 11:08:40.717530 configcat-client-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-03 11:08:29.000000 configcat-client-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:08:40.713530 configcat-client-8.0.0/configcat_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-03 11:08:40.000000 configcat-client-8.0.0/configcat_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-03 11:08:40.000000 configcat-client-8.0.0/configcat_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:08:40.000000 configcat-client-8.0.0/configcat_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 11:08:40.000000 configcat-client-8.0.0/configcat_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 11:08:40.000000 configcat-client-8.0.0/configcat_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:08:40.717530 configcat-client-8.0.0/configcatclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/configcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/configcatclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/configcatoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/configentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/configfetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/configservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/datagovernance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/evaluationdetails.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/localdictionarydatasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/localfiledatasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/overridedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/pollingmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/refreshresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/rolloutevaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 11:08:29.000000 configcat-client-8.0.0/configcatclient/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 11:08:29.000000 configcat-client-8.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 11:08:40.717530 configcat-client-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-03 11:08:29.000000 configcat-client-8.0.0/setup.py
```

### Comparing `configcat-client-7.0.1/LICENSE` & `configcat-client-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/LICENSE.txt` & `configcat-client-8.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/PKG-INFO` & `configcat-client-8.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: configcat-client
-Version: 7.0.1
+Version: 8.0.0
 Summary: ConfigCat SDK for Python. https://configcat.com
 Home-page: https://github.com/configcat/python-sdk
 Author: ConfigCat
 Author-email: developer@configcat.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 License-File: LICENSE.txt
 
 Feature Flags created by developers for developers with <3. ConfigCat lets you manage feature flags across frontend, backend, mobile, and desktop apps without (re)deploying code. % rollouts, user targeting, segmentation. Feature toggle SDKs for all main languages. Alternative to LaunchDarkly. Host yourself, or use the hosted management app at https://configcat.com.
```

### Comparing `configcat-client-7.0.1/README.md` & `configcat-client-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/configcat_client.egg-info/PKG-INFO` & `configcat-client-8.0.0/configcat_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: configcat-client
-Version: 7.0.1
+Version: 8.0.0
 Summary: ConfigCat SDK for Python. https://configcat.com
 Home-page: https://github.com/configcat/python-sdk
 Author: ConfigCat
 Author-email: developer@configcat.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 License-File: LICENSE.txt
 
 Feature Flags created by developers for developers with <3. ConfigCat lets you manage feature flags across frontend, backend, mobile, and desktop apps without (re)deploying code. % rollouts, user targeting, segmentation. Feature toggle SDKs for all main languages. Alternative to LaunchDarkly. Host yourself, or use the hosted management app at https://configcat.com.
```

### Comparing `configcat-client-7.0.1/configcat_client.egg-info/SOURCES.txt` & `configcat-client-8.0.0/configcat_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/configcatclient/configcatclient.py` & `configcat-client-8.0.0/configcatclient/configcatclient.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from threading import Lock
 
 from . import utils
 from .configservice import ConfigService
-from .constants import ROLLOUT_RULES, VARIATION_ID, VALUE, ROLLOUT_PERCENTAGE_ITEMS, CONFIG_FILE_NAME
+from .constants import ROLLOUT_RULES, VARIATION_ID, VALUE, ROLLOUT_PERCENTAGE_ITEMS
 from .evaluationdetails import EvaluationDetails
 from .interfaces import ConfigCatClientException
 from .logger import Logger
 from .configfetcher import ConfigFetcher
 from .configcache import NullConfigCache
 from .configcatoptions import ConfigCatOptions, Hooks
 from .overridedatasource import OverrideBehaviour
 from .refreshresult import RefreshResult
 from .rolloutevaluator import RolloutEvaluator
-import hashlib
 from collections import namedtuple
 import copy
 from .utils import method_is_called_from, get_date_time
 
 KeyValue = namedtuple('KeyValue', 'key value')
 
 
@@ -33,16 +32,18 @@
         :param options: Configuration `ConfigCatOptions` for `ConfigCatClient`.
         :return: the `ConfigCatClient` instance.
         """
         with cls._lock:
             client = cls._instances.get(sdk_key)
             if client is not None:
                 if options is not None:
-                    client.log.warning('Client for sdk_key `%s` is already created and will be reused; '
-                                       'options passed are being ignored.' % sdk_key)
+                    client.log.warning('There is an existing client instance for the specified SDK Key. '
+                                       'No new client instance will be created and the specified options are ignored. '
+                                       'Returning the existing client instance. SDK Key: \'%s\'.',
+                                       sdk_key, event_id=3000)
                 return client
 
             if options is None:
                 options = ConfigCatOptions()
 
             client = ConfigCatClient(sdk_key=sdk_key,
                                      options=options)
@@ -63,16 +64,16 @@
                  sdk_key,
                  options=ConfigCatOptions()):
 
         self._hooks = options.hooks if options.hooks is not None else Hooks()
         self.log = Logger('configcat', self._hooks)
 
         if not method_is_called_from(ConfigCatClient.get):
-            self.log.warning('ConfigCatClient.__init__() is deprecated. '
-                             'Create the ConfigCat Client as a Singleton object with `ConfigCatClient.get()` instead')
+            raise ConfigCatClientException('ConfigCatClient.__init__() is private. Create the ConfigCat Client as a '
+                                           'Singleton object with `ConfigCatClient.get()` instead.')
 
         if sdk_key is None:
             raise ConfigCatClientException('SDK Key is required.')
 
         self._sdk_key = sdk_key
         self._default_user = options.default_user
         self._rollout_evaluator = RolloutEvaluator(self.log)
@@ -109,18 +110,20 @@
         :param key: the identifier of the feature flag or setting.
         :param default_value: in case of any failure, this value will be returned.
         :param user: the user object to identify the caller.
         :return: the value.
         """
         settings, fetch_time = self.__get_settings()
         if settings is None:
-            message = 'Evaluating get_value(\'{}\') failed. Cache is empty. ' \
-                      'Returning default_value in your get_value call: [{}].'.format(key, str(default_value))
-            self.log.error(message)
-            self._hooks.invoke_on_flag_evaluated(EvaluationDetails.from_error(key, default_value, message))
+            message = 'Config JSON is not present when evaluating setting \'%s\'. ' \
+                      'Returning the `%s` parameter that you specified in your application: \'%s\'.'
+            message_args = (key, 'default_value', str(default_value))
+            self.log.error(message, *message_args, event_id=1000)
+            self._hooks.invoke_on_flag_evaluated(
+                EvaluationDetails.from_error(key, default_value, Logger.format(message, message_args)))
             return default_value
 
         details = self.__evaluate(key=key,
                                   user=user,
                                   default_value=default_value,
                                   default_variation_id=None,
                                   settings=settings,
@@ -135,18 +138,19 @@
         :param key: the identifier of the feature flag or setting.
         :param default_value: in case of any failure, this value will be returned.
         :param user: the user object to identify the caller.
         :return: the evaluation details.
         """
         settings, fetch_time = self.__get_settings()
         if settings is None:
-            message = 'Evaluating get_value_details(\'{}\') failed. Cache is empty. ' \
-                      'Returning default_value in your get_value_details call: [{}].'.format(key, str(default_value))
-            self.log.error(message)
-            details = EvaluationDetails.from_error(key, default_value, message)
+            message = 'Config JSON is not present when evaluating setting \'%s\'. ' \
+                      'Returning the `%s` parameter that you specified in your application: \'%s\'.'
+            message_args = (key, 'default_value', str(default_value))
+            self.log.error(message, *message_args, event_id=1000)
+            details = EvaluationDetails.from_error(key, default_value, Logger.format(message, message_args))
             self._hooks.invoke_on_flag_evaluated(details)
             return details
 
         details = self.__evaluate(key=key,
                                   user=user,
                                   default_value=default_value,
                                   default_variation_id=None,
@@ -159,77 +163,29 @@
         """
         Gets all setting keys.
 
         :return: list of keys.
         """
         settings, _ = self.__get_settings()
         if settings is None:
+            self.log.error('Config JSON is not present. Returning %s.', 'empty list', event_id=1000)
             return []
 
         return list(settings)
 
-    def get_variation_id(self, key, default_variation_id, user=None):
-        """
-        Gets the Variation ID (analytics) of a feature flag or setting based on it's key.
-
-        :param key: the identifier of the feature flag or setting.
-        :param default_variation_id: in case of any failure, this value will be returned.
-        :param user: the user object to identify the caller.
-        :return: the variation ID.
-        """
-        self.log.warning('get_variation_id is deprecated and will be removed in a future major version. '
-                         'Please use [get_value_details] instead.')
-
-        settings, fetch_time = self.__get_settings()
-        if settings is None:
-            message = 'Evaluating get_variation_id(\'{}\') failed. Cache is empty. ' \
-                      'Returning default_variation_id in your get_variation_id call: ' \
-                      '[{}].'.format(key, str(default_variation_id))
-            self.log.error(message)
-            self._hooks.invoke_on_flag_evaluated(EvaluationDetails.from_error(key, None, message, default_variation_id))
-            return default_variation_id
-
-        details = self.__evaluate(key=key,
-                                  user=user,
-                                  default_value=None,
-                                  default_variation_id=default_variation_id,
-                                  settings=settings,
-                                  fetch_time=fetch_time)
-        return details.variation_id
-
-    def get_all_variation_ids(self, user=None):
-        """
-        Gets the Variation IDs (analytics) of all feature flags or settings.
-
-        :param user: the user object to identify the caller.
-        :return: list of variation IDs
-        """
-        self.log.warning('get_all_variation_ids is deprecated and will be removed in a future major version. '
-                         'Please use [get_all_value_details] instead.')
-
-        keys = self.get_all_keys()
-        variation_ids = []
-        for key in keys:
-            variation_id = self.get_variation_id(key, None, user)
-            if variation_id is not None:
-                variation_ids.append(variation_id)
-
-        return variation_ids
-
     def get_key_and_value(self, variation_id):
         """
         Gets the key of a setting, and it's value identified by the given Variation ID (analytics)
 
         :param variation_id: variation ID
         :return: key and value
         """
         settings, _ = self.__get_settings()
         if settings is None:
-            self.log.warning('Evaluating get_key_and_value(\'%s\') failed. Cache is empty. '
-                             'Returning None.' % variation_id)
+            self.log.error('Config JSON is not present. Returning %s.', 'None', event_id=1000)
             return None
 
         for key, value in list(settings.items()):
             if variation_id == value.get(VARIATION_ID):
                 return KeyValue(key, value[VALUE])
 
             rollout_rules = value.get(ROLLOUT_RULES, [])
@@ -238,27 +194,31 @@
                     return KeyValue(key, rollout_rule[VALUE])
 
             rollout_percentage_items = value.get(ROLLOUT_PERCENTAGE_ITEMS, [])
             for rollout_percentage_item in rollout_percentage_items:
                 if variation_id == rollout_percentage_item.get(VARIATION_ID):
                     return KeyValue(key, rollout_percentage_item[VALUE])
 
-        self.log.error('Could not find the setting for the given variation_id: ' + variation_id)
+        self.log.error('Could not find the setting for the specified variation ID: \'%s\'.', variation_id, event_id=2011)
         return None
 
     def get_all_values(self, user=None):
         """
         Evaluates and returns the values of all feature flags and settings.
 
         :param user: the user object to identify the caller.
         :return: dictionary of values
         """
-        keys = self.get_all_keys()
+        settings, _ = self.__get_settings()
+        if settings is None:
+            self.log.error('Config JSON is not present. Returning %s.', 'empty dictionary', event_id=1000)
+            return {}
+
         all_values = {}
-        for key in keys:
+        for key in list(settings):
             value = self.get_value(key, None, user)
             if value is not None:
                 all_values[key] = value
 
         return all_values
 
     def get_all_value_details(self, user=None):
@@ -266,20 +226,19 @@
         Gets the values along with evaluation details of all feature flags and settings.
 
         :param user: the user object to identify the caller.
         :return: list of all evaluation details
         """
         settings, fetch_time = self.__get_settings()
         if settings is None:
-            message = 'Evaluating get_all_value_details() failed. Cache is empty. Returning empty list.'
-            self.log.error(message)
+            self.log.error('Config JSON is not present. Returning %s.', 'empty list', event_id=1000)
             return []
 
         details_result = []
-        for key, value in list(settings.items()):
+        for key in list(settings):
             details = self.__evaluate(key=key,
                                       user=user,
                                       default_value=None,
                                       default_variation_id=None,
                                       settings=settings,
                                       fetch_time=fetch_time)
             details_result.append(details)
@@ -314,26 +273,25 @@
 
     def set_online(self):
         """
         Configures the SDK to allow HTTP requests.
         """
         if self._config_service:
             self._config_service.set_online()
-
-        self.log.debug('Switched to ONLINE mode.')
+        else:
+            self.log.warning('Client is configured to use the `%s` override behavior, thus `%s()` has no effect.',
+                             'LocalOnly', 'set_online', event_id=3202)
 
     def set_offline(self):
         """
         Configures the SDK to not initiate HTTP requests and work only from its cache.
         """
         if self._config_service:
             self._config_service.set_offline()
 
-        self.log.debug('Switched to OFFLINE mode.')
-
     def is_offline(self):
         """
         True when the SDK is configured not to initiate HTTP requests, otherwise False.
         """
         if self._config_service:
             return self._config_service.is_offline()
 
@@ -386,17 +344,14 @@
                     local_settings = {}
                 result = copy.deepcopy(remote_settings)
                 result.update(local_settings)
                 return result, fetch_time
 
         return self._config_service.get_settings()
 
-    def __get_cache_key(self):
-        return hashlib.sha1(('python_' + CONFIG_FILE_NAME + '_' + self._sdk_key).encode('utf-8')).hexdigest()
-
     def __evaluate(self, key, user, default_value, default_variation_id, settings, fetch_time):
         user = user if user is not None else self._default_user
         value, variation_id, rule, percentage_rule, error = self._rollout_evaluator.evaluate(
             key=key,
             user=user,
             default_value=default_value,
             default_variation_id=default_variation_id,
```

### Comparing `configcat-client-7.0.1/configcatclient/configcatoptions.py` & `configcat-client-8.0.0/configcatclient/configcatoptions.py`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/configcatclient/configfetcher.py` & `configcat-client-8.0.0/configcatclient/configfetcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from platform import python_version
 from requests import HTTPError
 from requests import Timeout
 
 from .configentry import ConfigEntry
 from .constants import CONFIG_FILE_NAME, PREFERENCES, BASE_URL, REDIRECT
 from .datagovernance import DataGovernance
+from .logger import Logger
 from .utils import get_utc_now_seconds_since_epoch
 from .version import CONFIGCATCLIENT_VERSION
 
 if sys.version_info < (2, 7, 9):
     requests.packages.urllib3.disable_warnings()
 
 BASE_URL_GLOBAL = 'https://cdn-global.configcat.com'
@@ -132,22 +133,23 @@
         if redirect == int(RedirectMode.NoRedirect):
             # Return the response
             return fetch_response
 
         # Try to download again with the new url
 
         if redirect == int(RedirectMode.ShouldRedirect):
-            self.log.warning('Your data_governance parameter at ConfigCatClient initialization is not in sync '
-                             'with your preferences on the ConfigCat Dashboard: '
-                             'https://app.configcat.com/organization/data-governance. '
-                             'Only Organization Admins can access this preference.')
+            self.log.warning('The `dataGovernance` parameter specified at the client initialization is not in sync '
+                             'with the preferences on the ConfigCat Dashboard. '
+                             'Read more: https://configcat.com/docs/advanced/data-governance/',
+                             event_id=3002)
 
         # To prevent loops we check if we retried at least 3 times with the new base_url
         if retries >= 2:
-            self.log.error('Redirect loop during config.json fetch. Please contact support@configcat.com.')
+            self.log.error('Redirection loop encountered while trying to fetch config JSON. '
+                           'Please contact us at https://configcat.com/support/', event_id=1104)
             return fetch_response
 
         # Retry the config download with the new base_url
         return self.get_configuration(etag, retries + 1)
 
     def _fetch(self, etag):
         uri = self._base_url + '/' + BASE_PATH + self._sdk_key + BASE_EXTENSION
@@ -163,30 +165,34 @@
             response.raise_for_status()
 
             if response.status_code in [200, 201, 202, 203, 204]:
                 response_etag = response.headers.get('Etag')
                 if response_etag is None:
                     response_etag = ''
                 config = response.json()
-                return FetchResponse.success(ConfigEntry(config, response_etag, get_utc_now_seconds_since_epoch()))
+                return FetchResponse.success(
+                    ConfigEntry(config, response_etag, response.text, get_utc_now_seconds_since_epoch()))
             elif response.status_code == 304:
                 return FetchResponse.not_modified()
             elif response.status_code in [404, 403]:
-                error = 'Double-check your SDK Key at https://app.configcat.com/sdkkey. ' \
-                        'Received unexpected response: %s' % str(response)
-                self.log.error(error)
-                return FetchResponse.failure(error, False)
+                error = 'Your SDK Key seems to be wrong. ' \
+                        'You can find the valid SDK Key at https://app.configcat.com/sdkkey. ' \
+                        'Received unexpected response: %s'
+                error_args = (str(response), )
+                self.log.error(error, *error_args, event_id=1100)
+                return FetchResponse.failure(Logger.format(error, error_args), False)
             else:
                 raise (requests.HTTPError(response))
         except HTTPError as e:
-            error = 'Unexpected HTTP response was received: %s' % str(e.response)
-            self.log.error(error)
-            return FetchResponse.failure(error, True)
+            error = 'Unexpected HTTP response was received while trying to fetch config JSON: %s'
+            error_args = (str(e.response), )
+            self.log.error(error, *error_args, event_id=1101)
+            return FetchResponse.failure(Logger.format(error, error_args), True)
         except Timeout:
-            error = 'Request timed out. Timeout values: [connect: {}s, read: {}s]'.format(
-                self.get_connect_timeout(), self.get_read_timeout())
-            self.log.error(error)
-            return FetchResponse.failure(error, True)
+            error = 'Request timed out while trying to fetch config JSON. Timeout values: [connect: %gs, read: %gs]'
+            error_args = (self.get_connect_timeout(), self.get_read_timeout())
+            self.log.error(error, *error_args, event_id=1102)
+            return FetchResponse.failure(Logger.format(error, error_args), True)
         except Exception as e:
-            error = 'Exception occurred during fetching: ' + str(e)
-            self.log.error(error)
-            return FetchResponse.failure(error, True)
+            error = 'Unexpected error occurred while trying to fetch config JSON.'
+            self.log.exception(error, event_id=1103)
+            return FetchResponse.failure(Logger.format(error, (), e), True)
```

### Comparing `configcat-client-7.0.1/configcatclient/configservice.py` & `configcat-client-8.0.0/configcatclient/configservice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import hashlib
-import json
 from threading import Thread, Event, Lock
 
 from . import utils
 from .configentry import ConfigEntry
-from .constants import CONFIG_FILE_NAME, FEATURE_FLAGS
+from .constants import CONFIG_FILE_NAME, FEATURE_FLAGS, SERIALIZATION_FORMAT_VERSION
 from .pollingmode import AutoPollingMode, LazyLoadingMode
 from .refreshresult import RefreshResult
 
 
 class ConfigService(object):
     def __init__(self, sdk_key, polling_mode, hooks, config_fetcher, log, config_cache, is_offline):
-        self._sdk_key = sdk_key
         self._cached_entry = ConfigEntry.empty
         self._cached_entry_string = ''
         self._polling_mode = polling_mode
         self.log = log
         self._config_cache = config_cache
         self._hooks = hooks
-        self._cache_key = hashlib.sha1(('python_' + CONFIG_FILE_NAME + '_' + self._sdk_key).encode('utf-8')).hexdigest()
+        self._cache_key = ConfigService._get_cache_key(sdk_key)
         self._config_fetcher = config_fetcher
         self._is_offline = is_offline
         self._response_future = None
         self._initialized = Event()
         self._lock = Lock()
         self._ongoing_fetch = False
         self._fetch_finished = Event()
@@ -33,27 +31,33 @@
         else:
             self._set_initialized()
 
     def get_settings(self):
         if isinstance(self._polling_mode, LazyLoadingMode):
             entry, _ = self._fetch_if_older(
                 utils.get_utc_now_seconds_since_epoch() - self._polling_mode.cache_refresh_interval_seconds)
-            return entry.config.get(FEATURE_FLAGS), entry.fetch_time
+            return (entry.config.get(FEATURE_FLAGS, {}), entry.fetch_time) \
+                if not entry.is_empty() \
+                else (None, utils.distant_past)
         elif isinstance(self._polling_mode, AutoPollingMode) and not self._initialized.is_set():
             elapsed_time = (utils.get_utc_now() - self._start_time).total_seconds()
             if elapsed_time < self._polling_mode.max_init_wait_time_seconds:
                 self._initialized.wait(self._polling_mode.max_init_wait_time_seconds - elapsed_time)
 
                 # Max wait time expired without result, notify subscribers with the cached config.
                 if not self._initialized.is_set():
                     self._set_initialized()
-                    return self._cached_entry.config.get(FEATURE_FLAGS), self._cached_entry.fetch_time
+                    return (self._cached_entry.config.get(FEATURE_FLAGS, {}), self._cached_entry.fetch_time) \
+                        if not self._cached_entry.is_empty() \
+                        else (None, utils.distant_past)
 
         entry, _ = self._fetch_if_older(utils.distant_past, prefer_cache=True)
-        return entry.config.get(FEATURE_FLAGS), entry.fetch_time
+        return (entry.config.get(FEATURE_FLAGS, {}), entry.fetch_time) \
+            if not entry.is_empty() \
+            else (None, utils.distant_past)
 
     def refresh(self):
         """
         :return: RefreshResult object
         """
         _, error = self._fetch_if_older(utils.distant_future)
         return RefreshResult(is_success=error is None, error=error)
@@ -63,24 +67,28 @@
             if not self._is_offline:
                 return
 
             self._is_offline = False
             if isinstance(self._polling_mode, AutoPollingMode):
                 self._start_poll()
 
+            self.log.info('Switched to %s mode.', 'ONLINE', event_id=5200)
+
     def set_offline(self):
         with self._lock:
             if self._is_offline:
                 return
 
             self._is_offline = True
             if isinstance(self._polling_mode, AutoPollingMode):
                 self._stopped.set()
                 self._thread.join()
 
+            self.log.info('Switched to %s mode.', 'OFFLINE', event_id=5200)
+
     def is_offline(self):
         return self._is_offline  # atomic operation in python (lock is not needed)
 
     def close(self):
         if isinstance(self._polling_mode, AutoPollingMode):
             self._stopped.set()
 
@@ -106,16 +114,16 @@
             # The initialized check ensures that we subscribe for the ongoing fetch during the
             # max init wait time window in case of auto poll.
             if prefer_cache and self._initialized.is_set():
                 return self._cached_entry, None
 
             # If we are in offline mode we are not allowed to initiate fetch.
             if self._is_offline:
-                offline_warning = 'The SDK is in offline mode, it can not initiate HTTP calls.'
-                self.log.warning(offline_warning)
+                offline_warning = 'Client is in offline mode, it cannot initiate HTTP calls.'
+                self.log.warning(offline_warning, event_id=3200)
                 return self._cached_entry, offline_warning
 
         # No fetch is running, initiate a new one.
         # Ensure only one fetch request is running at a time.
         # If there's an ongoing fetch running, we will wait for the ongoing fetch.
         if self._ongoing_fetch:
             self._fetch_finished.wait()
@@ -158,24 +166,29 @@
                 break
 
     def _set_initialized(self):
         if not self._initialized.is_set():
             self._initialized.set()
             self._hooks.invoke_on_client_ready()
 
+    @staticmethod
+    def _get_cache_key(sdk_key):
+        return hashlib.sha1(
+            (sdk_key + '_' + CONFIG_FILE_NAME + '.json' + '_' + SERIALIZATION_FORMAT_VERSION).encode('utf-8')).hexdigest()
+
     def _read_cache(self):
         try:
             json_string = self._config_cache.get(self._cache_key)
             if not json_string or json_string == self._cached_entry_string:
                 return ConfigEntry.empty
 
             self._cached_entry_string = json_string
-            return ConfigEntry.create_from_json(json.loads(json_string))
-        except Exception as e:
-            self.log.error('An error occurred during the cache read. ' + str(e))
+            return ConfigEntry.create_from_string(json_string)
+        except Exception:
+            self.log.exception('Error occurred while reading the cache.', event_id=2200)
             return ConfigEntry.empty
 
     def _write_cache(self, config_entry):
         try:
-            self._config_cache.set(self._cache_key, json.dumps(config_entry.to_json()))
-        except Exception as e:
-            self.log.error('An error occurred during the cache write. ' + str(e))
+            self._config_cache.set(self._cache_key, config_entry.serialize())
+        except Exception:
+            self.log.exception('Error occurred while writing the cache.', event_id=2201)
```

### Comparing `configcat-client-7.0.1/configcatclient/evaluationdetails.py` & `configcat-client-8.0.0/configcatclient/evaluationdetails.py`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/configcatclient/localdictionarydatasource.py` & `configcat-client-8.0.0/configcatclient/localdictionarydatasource.py`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/configcatclient/localfiledatasource.py` & `configcat-client-8.0.0/configcatclient/localfiledatasource.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 
 
 class LocalFileDataSource(OverrideDataSource):
     def __init__(self, file_path, override_behaviour, log):
         OverrideDataSource.__init__(self, override_behaviour=override_behaviour)
         self.log = log
         if not os.path.exists(file_path):
-            self.log.error('The file \'%s\' does not exists.' % file_path)
+            self.log.error('Cannot find the local config file \'%s\'. '
+                           'This is a path that your application provided to the ConfigCat SDK '
+                           'by passing it to the constructor of the `LocalFileFlagOverrides` class. '
+                           'Read more: https://configcat.com/docs/sdk-reference/python/#json-file',
+                           file_path, event_id=1300)
 
         self._file_path = file_path
         self._settings = None
         self._cached_file_stamp = 0
 
     def get_overrides(self):
         self._reload_file_content()
@@ -38,11 +42,11 @@
                     if 'flags' in data:
                         self._settings = {}
                         source = data['flags']
                         for key, value in source.items():
                             self._settings[key] = {VALUE: value}
                     else:
                         self._settings = data[FEATURE_FLAGS]
-        except OSError as e:
-            self.log.error('Could not read the content of the file %s. %s' % (self._file_path, e))
-        except ValueError as e:
-            self.log.error('Could not decode json from file %s. %s' % (self._file_path, e))
+        except OSError:
+            self.log.exception('Failed to read the local config file \'%s\'.', self._file_path, event_id=1302)
+        except ValueError:
+            self.log.exception('Failed to decode JSON from the local config file \'%s\'.', self._file_path, event_id=2302)
```

### Comparing `configcat-client-7.0.1/configcatclient/overridedatasource.py` & `configcat-client-8.0.0/configcatclient/overridedatasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class FlagOverrides(object):
     __metaclass__ = ABCMeta
 
     @abstractmethod
     def create_data_source(self, log):
         """
-        :returns the created OverrideDataSource
+        :return: the created OverrideDataSource
         """
 
 
 class OverrideDataSource(object):
     __metaclass__ = ABCMeta
 
     def __init__(self, override_behaviour):
@@ -36,9 +36,9 @@
 
     def get_behaviour(self):
         return self._override_behaviour
 
     @abstractmethod
     def get_overrides(self):
         """
-        :returns the override dictionary
+        :return: the override dictionary
         """
```

### Comparing `configcat-client-7.0.1/configcatclient/pollingmode.py` & `configcat-client-8.0.0/configcatclient/pollingmode.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,26 @@
     Describes a polling mode.
     """
     __metaclass__ = ABCMeta
 
     @abstractmethod
     def identifier(self):
         """
-        :returns the identifier of polling mode. Used for analytical purposes in HTTP User-Agent headers.
+        :return: the identifier of polling mode. Used for analytical purposes in HTTP User-Agent headers.
         """
 
     @staticmethod
     def auto_poll(poll_interval_seconds=60, max_init_wait_time_seconds=5):
         """
         Creates a configured auto polling configuration.
 
-        :param poll_interval_seconds: sets at least how often this policy should fetch the latest configuration and refresh the cache.
-        :param max_init_wait_time_seconds: sets the maximum waiting time between initialization and the first config acquisition in seconds.
+        :param poll_interval_seconds:
+            sets at least how often this policy should fetch the latest configuration and refresh the cache.
+        :param max_init_wait_time_seconds:
+            sets the maximum waiting time between initialization and the first config acquisition in seconds.
         """
 
         if poll_interval_seconds < 1:
             poll_interval_seconds = 1
 
         if max_init_wait_time_seconds < 0:
             max_init_wait_time_seconds = 0
@@ -32,15 +34,16 @@
                                max_init_wait_time_seconds=max_init_wait_time_seconds)
 
     @staticmethod
     def lazy_load(cache_refresh_interval_seconds=60):
         """
         Creates a configured lazy loading polling configuration.
 
-        :param cache_refresh_interval_seconds: sets how long the cache will store its value before fetching the latest from the network again.
+        :param cache_refresh_interval_seconds:
+            sets how long the cache will store its value before fetching the latest from the network again.
         """
 
         if cache_refresh_interval_seconds < 1:
             cache_refresh_interval_seconds = 1
 
         return LazyLoadingMode(cache_refresh_interval_seconds=cache_refresh_interval_seconds)
```

### Comparing `configcat-client-7.0.1/configcatclient/rolloutevaluator.py` & `configcat-client-8.0.0/configcatclient/rolloutevaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import hashlib
 import semver
 
+from .logger import Logger
+
 from .constants import ROLLOUT_RULES, ROLLOUT_PERCENTAGE_ITEMS, VALUE, VARIATION_ID, COMPARISON_ATTRIBUTE, \
     COMPARISON_VALUE, COMPARATOR, PERCENTAGE
 from .user import User
 
 
 class RolloutEvaluator(object):
     SEMANTIC_VERSION_COMPARATORS = ['<', '<=', '>', '>=']
@@ -28,60 +30,65 @@
         'IS ONE OF (Sensitive)',
         'IS NOT ONE OF (Sensitive)'
     ]
 
     def __init__(self, log):
         self.log = log
 
-    def evaluate(self, key, user, default_value, default_variation_id, settings):
+    def evaluate(self, key, user, default_value, default_variation_id, settings):  # noqa: C901
         """
         returns value, variation_id, matched_evaluation_rule, matched_evaluation_percentage_rule, error
         """
         setting_descriptor = settings.get(key)
 
         if setting_descriptor is None:
-            error = 'Evaluating get_value(\'{}\') failed. Value not found for key \'{}\' ' \
-                    'Returning default_value: [{}]. ' \
-                    'Here are the available keys: {}'.format(key, key, str(default_value),
-                                                             ', '.join(list(settings)))
-
-            self.log.error(error)
-            return default_value, default_variation_id, None, None, error
+            error = 'Failed to evaluate setting \'%s\' (the key was not found in config JSON). ' \
+                    'Returning the `%s` parameter that you specified in your application: \'%s\'. ' \
+                    'Available keys: [%s].'
+            error_args = (key, 'default_value', str(default_value), ', '.join("'{}'".format(s) for s in list(settings)))
+            self.log.error(error, *error_args, event_id=1001)
+            return default_value, default_variation_id, None, None, Logger.format(error, error_args)
 
         rollout_rules = setting_descriptor.get(ROLLOUT_RULES, [])
         rollout_percentage_items = setting_descriptor.get(ROLLOUT_PERCENTAGE_ITEMS, [])
 
-        if user is not None and type(user) is not User:
-            self.log.warning('Evaluating get_value(\'%s\'). User Object is not an instance of User type.' % key)
+        user_has_invalid_type = user is not None and type(user) is not User
+        if user_has_invalid_type:
+            self.log.warning('Cannot evaluate targeting rules and %% options for setting \'%s\' '
+                             '(User Object is not an instance of User type).',
+                             key, event_id=4001)
             user = None
 
         if user is None:
-            if len(rollout_rules) > 0 or len(rollout_percentage_items) > 0:
-                self.log.warning('Evaluating get_value(\'%s\'). UserObject missing! '
-                                 'You should pass a UserObject to get_value(), '
+            if not user_has_invalid_type and (len(rollout_rules) > 0 or len(rollout_percentage_items) > 0):
+                self.log.warning('Cannot evaluate targeting rules and %% options for setting \'%s\' '
+                                 '(User Object is missing). '
+                                 'You should pass a User Object to the evaluation methods like `get_value()` '
                                  'in order to make targeting work properly. '
-                                 'Read more: https://configcat.com/docs/advanced/user-object/' %
-                                 key)
+                                 'Read more: https://configcat.com/docs/advanced/user-object/',
+                                 key, event_id=3001)
             return_value = setting_descriptor.get(VALUE, default_value)
             return_variation_id = setting_descriptor.get(VARIATION_ID, default_variation_id)
-            self.log.info('Returning [%s]' % str(return_value))
+            self.log.info('%s', 'Returning [%s]' % str(return_value), event_id=5000)
             return return_value, return_variation_id, None, None, None
 
         log_entries = ['Evaluating get_value(\'%s\').' % key, 'User object:\n%s' % str(user)]
 
         try:
             # Evaluate targeting rules
             for rollout_rule in rollout_rules:
                 comparison_attribute = rollout_rule.get(COMPARISON_ATTRIBUTE)
                 comparison_value = rollout_rule.get(COMPARISON_VALUE)
                 comparator = rollout_rule.get(COMPARATOR)
 
                 user_value = user.get_attribute(comparison_attribute)
                 if user_value is None or not user_value:
-                    log_entries.append(self._format_no_match_rule(comparison_attribute, user_value, comparator, comparison_value))
+                    log_entries.append(
+                        self._format_no_match_rule(comparison_attribute, user_value, comparator, comparison_value)
+                    )
                     continue
 
                 value = rollout_rule.get(VALUE)
                 variation_id = rollout_rule.get(VARIATION_ID, default_variation_id)
 
                 # IS ONE OF
                 if comparator == 0:
@@ -109,31 +116,32 @@
                         return value, variation_id, rollout_rule, None, None
 
                 # IS ONE OF, IS NOT ONE OF (Semantic version)
                 elif 4 <= comparator <= 5:
                     try:
                         match = False
                         for x in filter(None, [x.strip() for x in str(comparison_value).split(',')]):
-                            match = semver.match(str(user_value).strip(), '==' + x) or match
+                            match = semver.VersionInfo.parse(str(user_value).strip()).match('==' + x) or match
                         if (match and comparator == 4) or (not match and comparator == 5):
                             log_entries.append(self._format_match_rule(comparison_attribute, user_value, comparator,
                                                                        comparison_value, value))
                             return value, variation_id, rollout_rule, None, None
                     except ValueError as e:
                         message = self._format_validation_error_rule(comparison_attribute, user_value, comparator,
                                                                      comparison_value, str(e))
                         self.log.warning(message)
                         log_entries.append(message)
                         continue
 
                 # LESS THAN, LESS THAN OR EQUALS TO, GREATER THAN, GREATER THAN OR EQUALS TO (Semantic version)
                 elif 6 <= comparator <= 9:
                     try:
-                        if semver.match(str(user_value).strip(),
-                                        self.SEMANTIC_VERSION_COMPARATORS[comparator - 6] + str(comparison_value).strip()):
+                        if semver.VersionInfo.parse(str(user_value).strip()).match(
+                            self.SEMANTIC_VERSION_COMPARATORS[comparator - 6] + str(comparison_value).strip()
+                        ):
                             log_entries.append(self._format_match_rule(comparison_attribute, user_value, comparator,
                                                                        comparison_value, value))
                             return value, variation_id, rollout_rule, None, None
                     except ValueError as e:
                         message = self._format_validation_error_rule(comparison_attribute, user_value, comparator,
                                                                      comparison_value, str(e))
                         self.log.warning(message)
@@ -157,21 +165,25 @@
                         message = self._format_validation_error_rule(comparison_attribute, user_value, comparator,
                                                                      comparison_value, str(e))
                         self.log.warning(message)
                         log_entries.append(message)
                         continue
                 # IS ONE OF (Sensitive)
                 elif comparator == 16:
-                    if str(hashlib.sha1(user_value.encode('utf8')).hexdigest()) in [x.strip() for x in str(comparison_value).split(',')]:
+                    if str(hashlib.sha1(user_value.encode('utf8')).hexdigest()) in [  # NOSONAR python:S4790
+                        x.strip() for x in str(comparison_value).split(',')
+                    ]:
                         log_entries.append(self._format_match_rule(comparison_attribute, user_value, comparator,
                                                                    comparison_value, value))
                         return value, variation_id, rollout_rule, None, None
                 # IS NOT ONE OF (Sensitive)
                 elif comparator == 17:
-                    if str(hashlib.sha1(user_value.encode('utf8')).hexdigest()) not in [x.strip() for x in str(comparison_value).split(',')]:
+                    if str(hashlib.sha1(user_value.encode('utf8')).hexdigest()) not in [  # NOSONAR python:S4790
+                        x.strip() for x in str(comparison_value).split(',')
+                    ]:
                         log_entries.append(self._format_match_rule(comparison_attribute, user_value, comparator,
                                                                    comparison_value, value))
                         return value, variation_id, rollout_rule, None, None
 
                 log_entries.append(self._format_no_match_rule(comparison_attribute, user_value, comparator, comparison_value))
 
             # Evaluate variations
@@ -190,15 +202,15 @@
                         return percentage_value, variation_id, None, rollout_percentage_item, None
 
             return_value = setting_descriptor.get(VALUE, default_value)
             return_variation_id = setting_descriptor.get(VARIATION_ID, default_variation_id)
             log_entries.append('Returning %s' % return_value)
             return return_value, return_variation_id, None, None, None
         finally:
-            self.log.info('\n'.join(log_entries))
+            self.log.info('%s', '\n'.join(log_entries), event_id=5000)
 
     def _format_match_rule(self, comparison_attribute, user_value, comparator, comparison_value, value):
         return 'Evaluating rule: [%s:%s] [%s] [%s] => match, returning: %s' \
                % (comparison_attribute, user_value, self.COMPARATOR_TEXTS[comparator], comparison_value, value)
 
     def _format_no_match_rule(self, comparison_attribute, user_value, comparator, comparison_value):
         return 'Evaluating rule: [%s:%s] [%s] [%s] => no match' \
```

### Comparing `configcat-client-7.0.1/configcatclient/user.py` & `configcat-client-8.0.0/configcatclient/user.py`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/configcatclient/utils.py` & `configcat-client-8.0.0/configcatclient/utils.py`

 * *Files identical despite different names*

### Comparing `configcat-client-7.0.1/setup.py` & `configcat-client-8.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def parse_requirements(filename):
     lines = (line.strip() for line in open(filename))
     return [line for line in lines if line]
 
 
-configcatclient_version = '7.0.1'
+configcatclient_version = '8.0.0'
 
 requirements = parse_requirements('requirements.txt')
 
 setup(
     name='configcat-client',
     version=configcatclient_version,
     packages=['configcatclient'],
@@ -26,22 +26,20 @@
                      'Host yourself, or use the hosted management app at https://configcat.com.',
     install_requires=requirements,
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
     ],
 )
```

