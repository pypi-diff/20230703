# Comparing `tmp/drf_keycloak_auth-0.1.0.tar.gz` & `tmp/drf_keycloak_auth-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_keycloak_auth-0.1.0.tar", last modified: Fri Jan 13 01:12:51 2023, max compression
+gzip compressed data, was "drf_keycloak_auth-0.2.0.tar", last modified: Mon Jul  3 02:22:52 2023, max compression
```

## Comparing `drf_keycloak_auth-0.1.0.tar` & `drf_keycloak_auth-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 01:12:51.751260 drf_keycloak_auth-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5295 2023-01-13 01:12:51.751260 drf_keycloak_auth-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4636 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 01:12:51.749260 drf_keycloak_auth-0.1.0/drf_keycloak_auth/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    11859 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2512 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/keycloak.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1751 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 01:12:51.751260 drf_keycloak_auth-0.1.0/drf_keycloak_auth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5295 2023-01-13 01:12:51.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-01-13 01:12:51.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 01:12:51.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-01-13 01:12:51.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-13 01:12:51.000000 drf_keycloak_auth-0.1.0/drf_keycloak_auth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-13 01:12:51.751260 drf_keycloak_auth-0.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1150 2023-01-13 01:12:46.000000 drf_keycloak_auth-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:22:52.452438 drf_keycloak_auth-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5347 2023-07-03 02:22:52.452438 drf_keycloak_auth-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4729 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:22:52.450438 drf_keycloak_auth-0.2.0/drf_keycloak_auth/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    10919 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/keycloak.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:22:52.451438 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5347 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:22:52.452438 drf_keycloak_auth-0.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1142 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/setup.py
```

### Comparing `drf_keycloak_auth-0.1.0/LICENSE` & `drf_keycloak_auth-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.1.0/PKG-INFO` & `drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: drf_keycloak_auth
-Version: 0.1.0
+Name: drf-keycloak-auth
+Version: 0.2.0
 Summary: A convenience libary for authenticating users from Keycloak access tokens
 Home-page: https://gitlab.com/ecocommons-australia/lib/drf-keycloak-auth
-Author: EcoCommons Australia, Gary Burgmann
-Author-email: ecocommons@griffith.edu.au, garyburgmann@gmail.com
+Author: EcoCommons Australia
+Author-email: ecocommons@griffith.edu.au
 License: MIT
 Keywords: drf,django,rest_framework,djangorestframework,authentication,python3,keycloak
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DRF Keycloak Auth
 
 ## Requirements
 
@@ -143,28 +143,28 @@
 KEYCLOAK_MULTI_OIDC_JSON=
 {
 "hostname1": { OIDC adaptor },
 "hostname2": { OIDC adaptor },
 }
 ```
 
-KeycloakMultiAuthentication should instead be configured as the authentication class.
+KeycloakMultiAuthentication should be configured as the authentication class. 
 
 ```
 REST_FRAMEWORK = {
   ...
   'DEFAULT_AUTHENTICATION_CLASSES': [
     ...
     'rest_framework.authentication.SessionAuthentication',
     'drf_keycloak_auth.authentication.KeycloakMultiAuthentication',
   ]
 }
 ```
 ___
 NOTE: This will ignore `DEFAULTS` parameters for hostname, realm and client credentials.  All other parameters are still shared accross tenancies.
-
+NOTE2: `KeycloakAuthentication` can still be present as a fallback for simpler cases like local dev.
 ___
 
 
 ## Contributing
 
 * Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
```

### Comparing `drf_keycloak_auth-0.1.0/README.md` & `drf_keycloak_auth-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -127,28 +127,28 @@
 KEYCLOAK_MULTI_OIDC_JSON=
 {
 "hostname1": { OIDC adaptor },
 "hostname2": { OIDC adaptor },
 }
 ```
 
-KeycloakMultiAuthentication should instead be configured as the authentication class.
+KeycloakMultiAuthentication should be configured as the authentication class. 
 
 ```
 REST_FRAMEWORK = {
   ...
   'DEFAULT_AUTHENTICATION_CLASSES': [
     ...
     'rest_framework.authentication.SessionAuthentication',
     'drf_keycloak_auth.authentication.KeycloakMultiAuthentication',
   ]
 }
 ```
 ___
 NOTE: This will ignore `DEFAULTS` parameters for hostname, realm and client credentials.  All other parameters are still shared accross tenancies.
-
+NOTE2: `KeycloakAuthentication` can still be present as a fallback for simpler cases like local dev.
 ___
 
 
 ## Contributing
 
 * Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
```

### Comparing `drf_keycloak_auth-0.1.0/drf_keycloak_auth/authentication.py` & `drf_keycloak_auth-0.2.0/drf_keycloak_auth/authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     exceptions,
 )
 from rest_framework.exceptions import AuthenticationFailed
 from keycloak import KeycloakOpenID
 from .keycloak import (
     get_keycloak_openid,
     get_resource_roles,
-    add_role_prefix
+    add_roles_prefix
 )
 from .settings import api_settings
 from . import __title__
 
 
 log = logging.getLogger(__title__)
 User = get_user_model()
@@ -64,17 +64,20 @@
                     f'{decoded_token}'
                 )
                 user = AnonymousUser()
             else:
                 user = self._handle_local_user(decoded_token)
 
             log.debug(
-                'KeycloakAuthentication.authenticate_credentials: '
-                f'{user} | {decoded_token}'
+                'KeycloakAuthentication.authenticate_credentials:\n'
+                '################# decoded_token ###############\n'
+                f'{user} | {decoded_token}\n'
+                '################ /decoded_token ###############'
             )
+
             return (user, decoded_token)
         except Exception as e:
             log.error(
                 'KeycloakAuthentication.authenticate_credentials | '
                 f'Exception: {e}'
             )
             raise AuthenticationFailed() from e
@@ -98,15 +101,17 @@
         if (
             keycloak_username_field
             and
             isinstance(keycloak_username_field, str)
         ):
             django_fields['username'] = \
                 decoded_token.get(keycloak_username_field, '')
+
         django_fields['email'] = decoded_token.get('email', '')
+
         # django stores first_name and last_name as empty strings
         # by default, not None
         django_fields['first_name'] = \
             decoded_token.get('given_name', '')
         django_fields['last_name'] = \
             decoded_token.get('family_name', '')
 
@@ -214,15 +219,15 @@
             if (
                 valid_user
                 and api_settings.KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF
                 and type(api_settings.KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF)
                 in [list, tuple, set]
             ):
                 is_staff_roles = set(
-                    add_role_prefix(
+                    add_roles_prefix(
                         api_settings.KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF
                     )
                 )
                 log.debug(
                     f'KeycloakAuthentication._user_toggle_is_staff | {user} | '
                     f'is_staff_roles: {is_staff_roles}'
                 )
@@ -236,14 +241,15 @@
                     f'KeycloakAuthentication._user_toggle_is_staff | {user} | '
                     f'is_staff: {is_staff}'
                 )
                 # don't write unnecessarily, check different first
                 if is_staff != user.is_staff:
                     user.is_staff = is_staff
                     user.save()
+
         except Exception as e:
             log.warning(
                 'KeycloakAuthentication._user_toggle_is_staff | '
                 f'Exception: {e}'
             )
 
 
@@ -263,71 +269,47 @@
             for key, oidc in oidc_dict.items():
                 if key in str(hostname):
                     log.info(f"get_host_oidc: Found OIDC adapter for '{hostname}'")
                     return get_keycloak_openid(oidc)
             return None
 
         # Resolve OIDC adapter by hostname
-        if isinstance(api_settings.KEYCLOAK_MULTI_OIDC_JSON, dict):
-            try:
-                self.keycloak_openid = get_host_oidc(
-                    request.get_host(),
-                    api_settings.KEYCLOAK_MULTI_OIDC_JSON)
-
-                if self.keycloak_openid is None:
-                    raise OIDCConfigException(f"Could not determine OIDC adapter for "
-                                        f"'{str(request.get_host())}'. Trying all")
-
-                credentials = super().authenticate(request)
-                if credentials:
-                    # Append realm_name
-                    credentials[1].update(
-                        {'realm_name': self.keycloak_openid.realm_name}
-                    )
-                    return credentials
+        if not isinstance(api_settings.KEYCLOAK_MULTI_OIDC_JSON, dict):
+            raise OIDCConfigException(f"OIDC config not available")
 
-            except OIDCConfigException as e:
-                log.warning(
-                    'KeycloakMultiAuthentication.authenticate | '
-                    f'OIDCConfigException: {e})'
+        try:
+            self.keycloak_openid = get_host_oidc(
+                request.get_host(),
+                api_settings.KEYCLOAK_MULTI_OIDC_JSON)
+
+            if self.keycloak_openid is None:
+                raise OIDCConfigException(f"Could not determine OIDC adapter for "
+                                          f"'{str(request.get_host())}'. Trying all")
+
+            credentials = super().authenticate(request)
+            if credentials:
+                # Append realm_name
+                credentials[1].update(
+                    {'realm_name': self.keycloak_openid.realm_name}
                 )
+                return credentials
 
-            except AuthenticationFailed as e:
-                log.info(
-                    'KeycloakMultiAuthentication.authenticate | '
-                    f'AuthenticationFailed: {e})'
-                )
+        except OIDCConfigException as e:
+            log.warning(
+                'KeycloakMultiAuthentication.authenticate | '
+                f'OIDCConfigException: {e})'
+            )
 
-            except Exception as e:
-                log.error(
-                    'KeycloakMultiAuthentication.authenticate | '
-                    f'Exception: {e})'
-                )
+        except AuthenticationFailed as e:
+            log.info(
+                'KeycloakMultiAuthentication.authenticate | '
+                f'AuthenticationFailed: {e})'
+            )
 
-        # Legacy
-        else:
-            log.info("(Deprecated) Using legacy OIDC authentication")
-            for oidc in api_settings.KEYCLOAK_MULTI_OIDC_JSON:
-                try:
-                    self.keycloak_openid = get_keycloak_openid(oidc)
-
-                    credentials = super().authenticate(request)
-                    if credentials:
-                        # Append realm_name
-                        credentials[1].update(
-                            {'realm_name': self.keycloak_openid.realm_name}
-                        )
-                        break
-
-                except AuthenticationFailed as e:
-                    log.info(
-                        'KeycloakMultiAuthentication.authenticate | '
-                        f'AuthenticationFailed: {e})'
-                    )
+        except Exception as e:
+            log.error(
+                'KeycloakMultiAuthentication.authenticate | '
+                f'Exception: {e})'
+            )
 
-                except Exception as e:
-                    log.error(
-                        'KeycloakMultiAuthentication.authenticate | '
-                        f'Exception: {e} ({self.keycloak_openid.realm_name})'
-                    )
 
         return credentials
```

### Comparing `drf_keycloak_auth-0.1.0/drf_keycloak_auth/keycloak.py` & `drf_keycloak_auth-0.2.0/drf_keycloak_auth/keycloak.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ module for app specific keycloak connection """
 from typing import Dict, List
+import traceback
 import logging
 
 from keycloak import KeycloakOpenID
 
 from .settings import api_settings
 from . import __title__
 
@@ -14,15 +15,14 @@
 def get_keycloak_openid(oidc: dict = None) -> KeycloakOpenID:
     try:
         if oidc:
             log.info(
                 'get_keycloak_openid: '
                 f'OIDC realm={oidc["realm"]}'
             )
-
             return KeycloakOpenID(
                 server_url=oidc["auth-server-url"],
                 realm_name=oidc["realm"],
                 client_id=oidc["resource"],
                 client_secret_key=oidc["credentials"]["secret"]
             )
 
@@ -44,32 +44,34 @@
     """
     resource_access_roles = []
     try:
         if client_id is None:
             client_id = api_settings.KEYCLOAK_CLIENT_ID
 
         log.debug(f'{__name__} - get_resource_roles - client_id: {client_id}')
+
         resource_access_roles = (
-            decoded_token['resource_access']
-            [client_id]
-            ['roles']
+            decoded_token
+            .get('resource_access', {})
+            .get(client_id, {})
+            .get('roles', [])
         )
-        roles = add_role_prefix(resource_access_roles)
+        roles = add_roles_prefix(resource_access_roles)
         log.debug(f'{__name__} - get_resource_roles - roles: {roles}')
 
         return roles
+
     except Exception as e:
-        log.warning(f'{__name__} - get_resource_roles - Exception: {e}')
+        log.warning(f'{__name__} - get_resource_roles - Exception: ({str(type(e).__name__ )}) {e}\n'
+                    f'{traceback.format_exc()}')
         return []
 
 
-def add_role_prefix(roles: List[str]) -> List[str]:
-    """
-    add role prefix configured by KEYCLOAK_ROLE_SET_PREFIX to a list of roles
-    """
+def add_roles_prefix(roles: List[str]) -> List[str]:
+    """ add role prefix configured by KEYCLOAK_ROLE_SET_PREFIX to a list of roles """
     log.debug(f'{__name__} - get_resource_roles - roles: {roles}')
     prefixed_roles = [prefix_role(x) for x in roles]
     log.debug(
         f'{__name__} - get_resource_roles - prefixed_roles: {prefixed_roles}'
     )
     return prefixed_roles
```

### Comparing `drf_keycloak_auth-0.1.0/drf_keycloak_auth/permissions.py` & `drf_keycloak_auth-0.2.0/drf_keycloak_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.1.0/drf_keycloak_auth/settings.py` & `drf_keycloak_auth-0.2.0/drf_keycloak_auth/settings.py`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.1.0/drf_keycloak_auth.egg-info/PKG-INFO` & `drf_keycloak_auth-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: drf-keycloak-auth
-Version: 0.1.0
+Name: drf_keycloak_auth
+Version: 0.2.0
 Summary: A convenience libary for authenticating users from Keycloak access tokens
 Home-page: https://gitlab.com/ecocommons-australia/lib/drf-keycloak-auth
-Author: EcoCommons Australia, Gary Burgmann
-Author-email: ecocommons@griffith.edu.au, garyburgmann@gmail.com
+Author: EcoCommons Australia
+Author-email: ecocommons@griffith.edu.au
 License: MIT
 Keywords: drf,django,rest_framework,djangorestframework,authentication,python3,keycloak
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DRF Keycloak Auth
 
 ## Requirements
 
@@ -143,28 +143,28 @@
 KEYCLOAK_MULTI_OIDC_JSON=
 {
 "hostname1": { OIDC adaptor },
 "hostname2": { OIDC adaptor },
 }
 ```
 
-KeycloakMultiAuthentication should instead be configured as the authentication class.
+KeycloakMultiAuthentication should be configured as the authentication class. 
 
 ```
 REST_FRAMEWORK = {
   ...
   'DEFAULT_AUTHENTICATION_CLASSES': [
     ...
     'rest_framework.authentication.SessionAuthentication',
     'drf_keycloak_auth.authentication.KeycloakMultiAuthentication',
   ]
 }
 ```
 ___
 NOTE: This will ignore `DEFAULTS` parameters for hostname, realm and client credentials.  All other parameters are still shared accross tenancies.
-
+NOTE2: `KeycloakAuthentication` can still be present as a fallback for simpler cases like local dev.
 ___
 
 
 ## Contributing
 
 * Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
```

### Comparing `drf_keycloak_auth-0.1.0/setup.py` & `drf_keycloak_auth-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     license=meta.__license__,
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.4',
+    python_requires='>=3',
     install_requires=[
         'djangorestframework>=3.9,<4',
-        'python-keycloak>=0.22.0,<1',
-        'django>=2',
+        'python-keycloak>=3.3',
+        'django>=3',
         'urllib3<1.27,>=1.21.1',
         'pytz'
     ],
     keywords=[
         'drf',
         'django',
         'rest_framework',
```

