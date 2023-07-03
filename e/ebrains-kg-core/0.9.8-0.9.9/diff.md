# Comparing `tmp/ebrains_kg_core-0.9.8.tar.gz` & `tmp/ebrains_kg_core-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/HumanBrainProject/kg-core-python/kg-core-python/dist/tmpufatgpxw/ebrains_kg_core-0.9.8.tar", last modified: Thu Aug 25 14:29:47 2022, max compression
+gzip compressed data, was "/builds/HumanBrainProject/kg-core-python/kg-core-python/dist/tmp6xmv198q/ebrains_kg_core-0.9.9.tar", last modified: Mon Aug 29 13:00:33 2022, max compression
```

## Comparing `ebrains_kg_core-0.9.8.tar` & `ebrains_kg_core-0.9.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/
--rw-rw-r--   0 root         (0) root         (0)    11364 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      297 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8236 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/ebrains_kg_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)      297 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/ebrains_kg_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      354 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/ebrains_kg_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/ebrains_kg_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/ebrains_kg_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/ebrains_kg_core.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/kg_core/
--rw-rw-r--   0 root         (0) root         (0)     8853 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/kg_core/__communication.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/kg_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    32033 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/kg_core/kg.py
--rw-rw-r--   0 root         (0) root         (0)     5784 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/kg_core/oauth.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/kg_core/py.typed
--rw-rw-r--   0 root         (0) root         (0)     2386 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/kg_core/request.py
--rw-rw-r--   0 root         (0) root         (0)    13129 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/kg_core/response.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-25 14:29:47.000000 ebrains_kg_core-0.9.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2390 2022-08-25 14:29:25.000000 ebrains_kg_core-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/
+-rw-rw-r--   0 root         (0) root         (0)    11364 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      297 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8236 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/ebrains_kg_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      297 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/ebrains_kg_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      354 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/ebrains_kg_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/ebrains_kg_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/ebrains_kg_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/ebrains_kg_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/kg_core/
+-rw-rw-r--   0 root         (0) root         (0)     8853 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/kg_core/__communication.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/kg_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    33409 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/kg_core/kg.py
+-rw-rw-r--   0 root         (0) root         (0)     5784 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/kg_core/oauth.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/kg_core/py.typed
+-rw-rw-r--   0 root         (0) root         (0)     2386 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/kg_core/request.py
+-rw-rw-r--   0 root         (0) root         (0)    13173 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/kg_core/response.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-29 13:00:33.000000 ebrains_kg_core-0.9.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2390 2022-08-29 13:00:07.000000 ebrains_kg_core-0.9.9/setup.py
```

### Comparing `ebrains_kg_core-0.9.8/LICENSE` & `ebrains_kg_core-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ebrains_kg_core-0.9.8/README.md` & `ebrains_kg_core-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ebrains_kg_core-0.9.8/kg_core/__communication.py` & `ebrains_kg_core-0.9.9/kg_core/__communication.py`

 * *Files identical despite different names*

### Comparing `ebrains_kg_core-0.9.8/kg_core/kg.py` & `ebrains_kg_core-0.9.9/kg_core/kg.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,466 +57,522 @@
 
 class Admin(RequestsWithTokenHandler):
     def __init__(self, config: KGConfig):
         super(Admin, self).__init__(config)
 
     def assign_type_to_space(self, space: str, target_type: str) -> Optional[Error]:
         """Assign a type to a space"""
-        result = self._put(path=f"spaces/{space}/types", payload=None, params={ 
+        params = { 
             "type": target_type
-        })
+        }
+        result = self._put(path=f"spaces/{space}/types", payload=None, params=params)
         return translate_error(result)
 
     def calculate_instance_invitation_scope(self, instance_id: UUID) -> Optional[Error]:
         """Update invitation scope for this instance"""
-        result = self._put(path=f"instances/{instance_id}/invitationScope", payload=None, params={})
+        params = {}
+        result = self._put(path=f"instances/{instance_id}/invitationScope", payload=None, params=params)
         return translate_error(result)
 
     def create_space_definition(self, space: str, autorelease: bool = False, client_space: bool = False, defer_cache: bool = False) -> Optional[Error]:
         """Explicitly specify a space"""
-        result = self._put(path=f"spaces/{space}/specification", payload=None, params={ 
+        params = { 
             "autorelease": autorelease,
             "clientSpace": client_space,
             "deferCache": defer_cache
-        })
+        }
+        result = self._put(path=f"spaces/{space}/specification", payload=None, params=params)
         return translate_error(result)
 
     def create_type_definition(self, payload: dict, target_type: str, is_global: Optional[bool] = None) -> Optional[Error]:
         """Specify a type"""
-        result = self._put(path="types/specification", payload=payload, params={ 
+        params = { 
             "global": is_global,
             "type": target_type
-        })
+        }
+        result = self._put(path="types/specification", payload=payload, params=params)
         return translate_error(result)
 
     def define_property(self, payload: dict, property_name: str, is_global: Optional[bool] = None) -> Optional[Error]:
         """Upload a property specification either globally or for the requesting client"""
-        result = self._put(path="properties", payload=payload, params={ 
+        params = { 
             "global": is_global,
             "property": property_name
-        })
+        }
+        result = self._put(path="properties", payload=payload, params=params)
         return translate_error(result)
 
     def define_property_for_type(self, payload: dict, property_name: str, target_type: str, is_global: Optional[bool] = None) -> Optional[Error]:
         """Define a property specification either globally for the requesting client"""
-        result = self._put(path="propertiesForType", payload=payload, params={ 
+        params = { 
             "global": is_global,
             "property": property_name,
             "type": target_type
-        })
+        }
+        result = self._put(path="propertiesForType", payload=payload, params=params)
         return translate_error(result)
 
     def deprecate_property(self, property_name: str, is_global: Optional[bool] = None) -> Optional[Error]:
         """Upload a property specification either globally or for the requesting client"""
-        result = self._delete(path="properties", params={ 
+        params = { 
             "global": is_global,
             "property": property_name
-        })
+        }
+        result = self._delete(path="properties", params=params)
         return translate_error(result)
 
     def deprecate_property_for_type(self, property_name: str, target_type: str, is_global: Optional[bool] = None) -> Optional[Error]:
         """Deprecate a property specification for a specific type either globally or for the requesting client"""
-        result = self._delete(path="propertiesForType", params={ 
+        params = { 
             "global": is_global,
             "property": property_name,
             "type": target_type
-        })
+        }
+        result = self._delete(path="propertiesForType", params=params)
         return translate_error(result)
 
     def get_all_role_definitions(self) -> Optional[Error]:
-        result = self._get(path="setup/permissions", params={})
+        params = {}
+        result = self._get(path="setup/permissions", params=params)
         return translate_error(result)
 
     def get_claim_for_role(self, role: str, space: Optional[str] = None) -> Optional[Error]:
-        result = self._get(path=f"setup/permissions/{role}", params={ 
+        params = { 
             "space": space
-        })
+        }
+        result = self._get(path=f"setup/permissions/{role}", params=params)
         return translate_error(result)
 
     def list_instances_with_invitations(self) -> Result[ListOfUUID]:
         """List instances with invitations"""
-        result = self._get(path="instancesWithInvitations", params={})
+        params = {}
+        result = self._get(path="instancesWithInvitations", params=params)
         return Result[ListOfUUID](response=result, constructor=ListOfUUID)
 
     def register_terms_of_use(self, payload: dict) -> Optional[Error]:
-        result = self._put(path="setup/termsOfUse", payload=payload, params={})
+        params = {}
+        result = self._put(path="setup/termsOfUse", payload=payload, params=params)
         return translate_error(result)
 
     def remove_space_definition(self, space: str) -> Optional[Error]:
         """Remove a space definition"""
-        result = self._delete(path=f"spaces/{space}/specification", params={})
+        params = {}
+        result = self._delete(path=f"spaces/{space}/specification", params=params)
         return translate_error(result)
 
     def remove_type_definition(self, is_global: Optional[bool] = None, target_type: Optional[str] = None) -> Optional[Error]:
         """Remove a type definition"""
-        result = self._delete(path="types/specification", params={ 
+        params = { 
             "type": target_type,
             "global": is_global
-        })
+        }
+        result = self._delete(path="types/specification", params=params)
         return translate_error(result)
 
     def remove_type_from_space(self, space: str, target_type: str) -> Optional[Error]:
         """Remove a type in space definition"""
-        result = self._delete(path=f"spaces/{space}/types", params={ 
+        params = { 
             "type": target_type
-        })
+        }
+        result = self._delete(path=f"spaces/{space}/types", params=params)
         return translate_error(result)
 
     def rerun_events(self, space: str) -> Optional[Error]:
         """Trigger a rerun of the events of this space"""
-        result = self._put(path=f"spaces/{space}/eventHistory", payload=None, params={})
+        params = {}
+        result = self._put(path=f"spaces/{space}/eventHistory", payload=None, params=params)
         return translate_error(result)
 
     def trigger_inference(self, space: str, identifier: Optional[str] = None, is_async: bool = False) -> Optional[Error]:
         """Triggers the inference of all documents of the given space"""
-        result = self._post(path=f"spaces/{space}/inference", payload=None, params={ 
+        params = { 
             "identifier": identifier,
             "async": is_async
-        })
+        }
+        result = self._post(path=f"spaces/{space}/inference", payload=None, params=params)
         return translate_error(result)
 
     def update_claim_for_role(self, payload: dict, remove: bool, role: str, space: Optional[str] = None) -> Optional[Error]:
-        result = self._patch(path=f"setup/permissions/{role}", payload=payload, params={ 
+        params = { 
             "space": space,
             "remove": remove
-        })
+        }
+        result = self._patch(path=f"setup/permissions/{role}", payload=payload, params=params)
         return translate_error(result)
 
 
 class Instances(RequestsWithTokenHandler):
     def __init__(self, config: KGConfig):
         super(Instances, self).__init__(config)
 
     def contribute_to_full_replacement(self, payload: dict, instance_id: UUID, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> Result[Instance]:
         """Replace contribution to an existing instance"""
-        result = self._put(path=f"instances/{instance_id}", payload=payload, params={ 
+        params = { 
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._put(path=f"instances/{instance_id}", payload=payload, params=params)
         return Result[Instance](response=result, constructor=Instance)
 
     def contribute_to_partial_replacement(self, payload: dict, instance_id: UUID, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> Result[Instance]:
         """Partially update contribution to an existing instance"""
-        result = self._patch(path=f"instances/{instance_id}", payload=payload, params={ 
+        params = { 
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._patch(path=f"instances/{instance_id}", payload=payload, params=params)
         return Result[Instance](response=result, constructor=Instance)
 
     def create_new(self, payload: dict, space: str, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> Result[Instance]:
         """Create new instance with a system generated id"""
-        result = self._post(path="instances", payload=payload, params={ 
+        params = { 
             "space": space,
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._post(path="instances", payload=payload, params=params)
         return Result[Instance](response=result, constructor=Instance)
 
     def create_new_with_id(self, payload: dict, instance_id: UUID, space: str, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> Result[Instance]:
         """Create new instance with a client defined id"""
-        result = self._post(path=f"instances/{instance_id}", payload=payload, params={ 
+        params = { 
             "space": space,
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._post(path=f"instances/{instance_id}", payload=payload, params=params)
         return Result[Instance](response=result, constructor=Instance)
 
     def delete(self, instance_id: UUID) -> Optional[Error]:
         """Delete an instance"""
-        result = self._delete(path=f"instances/{instance_id}", params={})
+        params = {}
+        result = self._delete(path=f"instances/{instance_id}", params=params)
         return translate_error(result)
 
     def get_by_id(self, instance_id: UUID, stage: Stage = Stage.RELEASED, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> Result[Instance]:
         """Get the instance"""
-        result = self._get(path=f"instances/{instance_id}", params={ 
+        params = { 
             "stage": stage,
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._get(path=f"instances/{instance_id}", params=params)
         return Result[Instance](response=result, constructor=Instance)
 
     def get_by_identifiers(self, payload: dict, stage: Stage = Stage.RELEASED, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> ResultsById[Instance]:
         """Read instances by the given list of (external) identifiers"""
-        result = self._post(path="instancesByIdentifiers", payload=payload, params={ 
+        params = { 
             "stage": stage,
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._post(path="instancesByIdentifiers", payload=payload, params=params)
         return ResultsById[Instance](response=result, constructor=Instance)
 
     def get_by_ids(self, payload: dict, stage: Stage = Stage.RELEASED, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> ResultsById[Instance]:
         """Bulk operation of /instances/{id} to read instances by their UUIDs"""
-        result = self._post(path="instancesByIds", payload=payload, params={ 
+        params = { 
             "stage": stage,
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._post(path="instancesByIds", payload=payload, params=params)
         return ResultsById[Instance](response=result, constructor=Instance)
 
     def get_incoming_links(self, instance_id: UUID, property_name: str, target_type: str, stage: Stage = Stage.RELEASED, pagination: Pagination = Pagination()) -> ResultPage[Instance]:
         """Get incoming links for a specific instance (paginated)"""
-        result = self._get(path=f"instances/{instance_id}/incomingLinks", params={ 
+        params = { 
             "stage": stage,
             "property": property_name,
             "type": target_type,
             "from": pagination.start,
             "size": pagination.size,
             "returnTotalResults": pagination.return_total_results
-        })
+        }
+        result = self._get(path=f"instances/{instance_id}/incomingLinks", params=params)
         return ResultPage[Instance](response=result, constructor=Instance)
 
     def get_release_status(self, instance_id: UUID, release_tree_scope: ReleaseTreeScope) -> Result[ReleaseStatus]:
         """Get the release status for an instance"""
-        result = self._get(path=f"instances/{instance_id}/release/status", params={ 
+        params = { 
             "releaseTreeScope": release_tree_scope
-        })
+        }
+        result = self._get(path=f"instances/{instance_id}/release/status", params=params)
         return Result[ReleaseStatus](response=result, constructor=ReleaseStatus)
 
     def get_release_status_by_ids(self, payload: dict, release_tree_scope: ReleaseTreeScope) -> ResultsById[ReleaseStatus]:
         """Get the release status for multiple instances"""
-        result = self._post(path="instancesByIds/release/status", payload=payload, params={ 
+        params = { 
             "releaseTreeScope": release_tree_scope
-        })
+        }
+        result = self._post(path="instancesByIds/release/status", payload=payload, params=params)
         return ResultsById[ReleaseStatus](response=result, constructor=ReleaseStatus)
 
     def get_scope(self, instance_id: UUID, apply_restrictions: bool = False, return_permissions: bool = False, stage: Stage = Stage.RELEASED) -> Result[Scope]:
         """Get the scope for the instance by its KG-internal ID"""
-        result = self._get(path=f"instances/{instance_id}/scope", params={ 
+        params = { 
             "stage": stage,
             "returnPermissions": return_permissions,
             "applyRestrictions": apply_restrictions
-        })
+        }
+        result = self._get(path=f"instances/{instance_id}/scope", params=params)
         return Result[Scope](response=result, constructor=Scope)
 
     def invite_user_for(self, instance_id: UUID, user_id: UUID) -> Optional[Error]:
         """Create or update an invitation for the given user to review the given instance"""
-        result = self._put(path=f"instances/{instance_id}/invitedUsers/{user_id}", payload=None, params={})
+        params = {}
+        result = self._put(path=f"instances/{instance_id}/invitedUsers/{user_id}", payload=None, params=params)
         return translate_error(result)
 
     def list(self, target_type: str, filter_property: Optional[str] = None, filter_value: Optional[str] = None, search_by_label: Optional[str] = None, space: Optional[str] = None, stage: Stage = Stage.RELEASED, response_configuration: ResponseConfiguration = ResponseConfiguration(), pagination: Pagination = Pagination()) -> ResultPage[Instance]:
         """Returns a list of instances according to their types"""
-        result = self._get(path="instances", params={ 
+        params = { 
             "stage": stage,
             "type": target_type,
             "space": space,
             "searchByLabel": search_by_label,
             "filterProperty": filter_property,
             "filterValue": filter_value,
             "returnPayload": response_configuration.return_payload,
             "returnPermissions": response_configuration.return_permissions,
             "returnAlternatives": response_configuration.return_alternatives,
             "returnEmbedded": response_configuration.return_embedded,
             "from": pagination.start,
             "size": pagination.size,
             "returnTotalResults": pagination.return_total_results
-        })
+        }
+        result = self._get(path="instances", params=params)
         return ResultPage[Instance](response=result, constructor=Instance)
 
     def list_invitations(self, instance_id: UUID) -> Result[ListOfReducedUserInformation]:
         """List invitations for review for the given instance"""
-        result = self._get(path=f"instances/{instance_id}/invitedUsers", params={})
+        params = {}
+        result = self._get(path=f"instances/{instance_id}/invitedUsers", params=params)
         return Result[ListOfReducedUserInformation](response=result, constructor=ListOfReducedUserInformation)
 
     def move(self, instance_id: UUID, space: str, extended_response_configuration: ExtendedResponseConfiguration = ExtendedResponseConfiguration()) -> Result[Instance]:
         """Move an instance to another space"""
-        result = self._put(path=f"instances/{instance_id}/spaces/{space}", payload=None, params={ 
+        params = { 
             "returnIncomingLinks": extended_response_configuration.return_incoming_links,
             "incomingLinksPageSize": extended_response_configuration.incoming_links_page_size,
             "returnPayload": extended_response_configuration.return_payload,
             "returnPermissions": extended_response_configuration.return_permissions,
             "returnAlternatives": extended_response_configuration.return_alternatives,
             "returnEmbedded": extended_response_configuration.return_embedded
-        })
+        }
+        result = self._put(path=f"instances/{instance_id}/spaces/{space}", payload=None, params=params)
         return Result[Instance](response=result, constructor=Instance)
 
     def release(self, instance_id: UUID, revision: Optional[str] = None) -> Optional[Error]:
         """Release or re-release an instance"""
-        result = self._put(path=f"instances/{instance_id}/release", payload=None, params={ 
+        params = { 
             "revision": revision
-        })
+        }
+        result = self._put(path=f"instances/{instance_id}/release", payload=None, params=params)
         return translate_error(result)
 
     def revoke_user_invitation(self, instance_id: UUID, user_id: UUID) -> Optional[Error]:
         """Revoke an invitation for the given user to review the given instance"""
-        result = self._delete(path=f"instances/{instance_id}/invitedUsers/{user_id}", params={})
+        params = {}
+        result = self._delete(path=f"instances/{instance_id}/invitedUsers/{user_id}", params=params)
         return translate_error(result)
 
     def unrelease(self, instance_id: UUID) -> Optional[Error]:
         """Unrelease an instance"""
-        result = self._delete(path=f"instances/{instance_id}/release", params={})
+        params = {}
+        result = self._delete(path=f"instances/{instance_id}/release", params=params)
         return translate_error(result)
 
 
 class Jsonld(RequestsWithTokenHandler):
     def __init__(self, config: KGConfig):
         super(Jsonld, self).__init__(config)
 
     def normalize_payload(self, payload: dict) -> Optional[Error]:
         """Normalizes the passed payload according to the EBRAINS KG conventions"""
-        result = self._post(path="jsonld/normalizedPayload", payload=payload, params={})
+        params = {}
+        result = self._post(path="jsonld/normalizedPayload", payload=payload, params=params)
         return translate_error(result)
 
 
 class Queries(RequestsWithTokenHandler):
     def __init__(self, config: KGConfig):
         super(Queries, self).__init__(config)
 
-    def execute_query_by_id(self, query_id: UUID, all_request_params: Dict[str, Any] = {}, instance_id: Optional[UUID] = None, restrict_to_spaces: Optional[List[str]] = None, stage: Stage = Stage.RELEASED, pagination: Pagination = Pagination()) -> ResultPage[JsonLdDocument]:
+    def execute_query_by_id(self, query_id: UUID, additional_request_params: Dict[str, Any] = {}, instance_id: Optional[UUID] = None, restrict_to_spaces: Optional[List[str]] = None, stage: Stage = Stage.RELEASED, pagination: Pagination = Pagination()) -> ResultPage[JsonLdDocument]:
         """Execute a stored query to receive the instances"""
-        result = self._get(path=f"queries/{query_id}/instances", params={ 
+        params = { 
             "from": pagination.start,
             "size": pagination.size,
             "returnTotalResults": pagination.return_total_results,
             "stage": stage,
             "instanceId": instance_id,
-            "restrictToSpaces": restrict_to_spaces,
-            "allRequestParams": all_request_params
-        })
+            "restrictToSpaces": restrict_to_spaces
+        }
+        for k, v in additional_request_params:
+            if k not in params:
+                params[k] = v
+        result = self._get(path=f"queries/{query_id}/instances", params=params)
         return ResultPage[JsonLdDocument](response=result, constructor=JsonLdDocument)
 
     def get_query_specification(self, query_id: UUID) -> Result[Instance]:
         """Get the query specification with the given query id in a specific space"""
-        result = self._get(path=f"queries/{query_id}", params={})
+        params = {}
+        result = self._get(path=f"queries/{query_id}", params=params)
         return Result[Instance](response=result, constructor=Instance)
 
     def list_per_root_type(self, search: Optional[str] = None, target_type: Optional[str] = None, pagination: Pagination = Pagination()) -> ResultPage[Instance]:
         """List the queries and filter them by root type and/or text in the label, name or description"""
-        result = self._get(path="queries", params={ 
+        params = { 
             "from": pagination.start,
             "size": pagination.size,
             "returnTotalResults": pagination.return_total_results,
             "type": target_type,
             "search": search
-        })
+        }
+        result = self._get(path="queries", params=params)
         return ResultPage[Instance](response=result, constructor=Instance)
 
     def remove_query(self, query_id: UUID) -> Optional[Error]:
         """Remove a query specification"""
-        result = self._delete(path=f"queries/{query_id}", params={})
+        params = {}
+        result = self._delete(path=f"queries/{query_id}", params=params)
         return translate_error(result)
 
     def save_query(self, payload: dict, query_id: UUID, space: Optional[str] = None) -> Result[Instance]:
         """Create or save a query specification"""
-        result = self._put(path=f"queries/{query_id}", payload=payload, params={ 
+        params = { 
             "space": space
-        })
+        }
+        result = self._put(path=f"queries/{query_id}", payload=payload, params=params)
         return Result[Instance](response=result, constructor=Instance)
 
-    def test_query(self, payload: dict, all_request_params: Dict[str, Any] = {}, instance_id: Optional[UUID] = None, restrict_to_spaces: Optional[List[str]] = None, stage: Stage = Stage.RELEASED, pagination: Pagination = Pagination()) -> ResultPage[JsonLdDocument]:
+    def test_query(self, payload: dict, additional_request_params: Dict[str, Any] = {}, instance_id: Optional[UUID] = None, restrict_to_spaces: Optional[List[str]] = None, stage: Stage = Stage.RELEASED, pagination: Pagination = Pagination()) -> ResultPage[JsonLdDocument]:
         """Execute the query in the payload in test mode (e.g. for execution before saving with the KG QueryBuilder)"""
-        result = self._post(path="queries", payload=payload, params={ 
+        params = { 
             "from": pagination.start,
             "size": pagination.size,
             "returnTotalResults": pagination.return_total_results,
             "stage": stage,
             "instanceId": instance_id,
-            "restrictToSpaces": restrict_to_spaces,
-            "allRequestParams": all_request_params
-        })
+            "restrictToSpaces": restrict_to_spaces
+        }
+        for k, v in additional_request_params:
+            if k not in params:
+                params[k] = v
+        result = self._post(path="queries", payload=payload, params=params)
         return ResultPage[JsonLdDocument](response=result, constructor=JsonLdDocument)
 
 
 class Spaces(RequestsWithTokenHandler):
     def __init__(self, config: KGConfig):
         super(Spaces, self).__init__(config)
 
     def get(self, space: str, permissions: bool = False) -> Result[SpaceInformation]:
-        result = self._get(path=f"spaces/{space}", params={ 
+        params = { 
             "permissions": permissions
-        })
+        }
+        result = self._get(path=f"spaces/{space}", params=params)
         return Result[SpaceInformation](response=result, constructor=SpaceInformation)
 
     def list(self, permissions: bool = False, pagination: Pagination = Pagination()) -> ResultPage[SpaceInformation]:
-        result = self._get(path="spaces", params={ 
+        params = { 
             "from": pagination.start,
             "size": pagination.size,
             "returnTotalResults": pagination.return_total_results,
             "permissions": permissions
-        })
+        }
+        result = self._get(path="spaces", params=params)
         return ResultPage[SpaceInformation](response=result, constructor=SpaceInformation)
 
 
 class Types(RequestsWithTokenHandler):
     def __init__(self, config: KGConfig):
         super(Types, self).__init__(config)
 
     def get_by_name(self, payload: dict, space: Optional[str] = None, stage: Stage = Stage.RELEASED, with_incoming_links: bool = False, with_properties: bool = False) -> ResultsById[TypeInformation]:
         """Returns the types according to the list of names - either with property information or without"""
-        result = self._post(path="typesByName", payload=payload, params={ 
+        params = { 
             "stage": stage,
             "withProperties": with_properties,
             "withIncomingLinks": with_incoming_links,
             "space": space
-        })
+        }
+        result = self._post(path="typesByName", payload=payload, params=params)
         return ResultsById[TypeInformation](response=result, constructor=TypeInformation)
 
     def list(self, space: Optional[str] = None, stage: Stage = Stage.RELEASED, with_incoming_links: bool = False, with_properties: bool = False, pagination: Pagination = Pagination()) -> ResultPage[TypeInformation]:
         """Returns the types available - either with property information or without"""
-        result = self._get(path="types", params={ 
+        params = { 
             "stage": stage,
             "space": space,
             "withProperties": with_properties,
             "withIncomingLinks": with_incoming_links,
             "from": pagination.start,
             "size": pagination.size,
             "returnTotalResults": pagination.return_total_results
-        })
+        }
+        result = self._get(path="types", params=params)
         return ResultPage[TypeInformation](response=result, constructor=TypeInformation)
 
 
 class Users(RequestsWithTokenHandler):
     def __init__(self, config: KGConfig):
         super(Users, self).__init__(config)
 
     def accept_terms_of_use(self, version: str) -> Optional[Error]:
         """Accept the terms of use in the given version"""
-        result = self._post(path=f"users/termsOfUse/{version}/accept", payload=None, params={})
+        params = {}
+        result = self._post(path=f"users/termsOfUse/{version}/accept", payload=None, params=params)
         return translate_error(result)
 
     def get_open_id_config_url(self) -> Result[JsonLdDocument]:
         """Get the endpoint of the openid configuration"""
-        result = self._get(path="users/authorization/config", params={})
+        params = {}
+        result = self._get(path="users/authorization/config", params=params)
         return Result[JsonLdDocument](response=result, constructor=JsonLdDocument)
 
     def get_terms_of_use(self) -> Optional[TermsOfUse]:
         """Get the current terms of use"""
-        result = self._get(path="users/termsOfUse", params={})
+        params = {}
+        result = self._get(path="users/termsOfUse", params=params)
         return None if not result.content else TermsOfUse(**result.content)
 
     def my_info(self) -> Result[User]:
         """Retrieve user information from the passed token (including detailed information such as e-mail address)"""
-        result = self._get(path="users/me", params={})
+        params = {}
+        result = self._get(path="users/me", params=params)
         return Result[User](response=result, constructor=User)
 
 
 class ClientBuilder(object):
 
     def __init__(self, host_name: str, enable_profiling: bool):
         self._host_name = host_name
```

### Comparing `ebrains_kg_core-0.9.8/kg_core/oauth.py` & `ebrains_kg_core-0.9.9/kg_core/oauth.py`

 * *Files identical despite different names*

### Comparing `ebrains_kg_core-0.9.8/kg_core/request.py` & `ebrains_kg_core-0.9.9/kg_core/request.py`

 * *Files identical despite different names*

### Comparing `ebrains_kg_core-0.9.8/kg_core/response.py` & `ebrains_kg_core-0.9.9/kg_core/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,18 +191,18 @@
         }
 
 
 ResponseType = TypeVar("ResponseType")
 
 
 def translate_error(response: KGRequestWithResponseContext) -> Optional[Error]:
-    return Error(**response.content["error"]) if response.content and "error" in response.content and response.content[
-        "error"] \
-        else Error(code=response.status_code, message=http.client.responses[
-        response.status_code]) if response.status_code and response.status_code >= 400 else None
+    if response.content and "error" in response.content and response.content["error"] and type(response.content["error"]) != str:
+        return Error(**response.content["error"])
+    else:
+        return Error(code=response.status_code, message=http.client.responses[response.status_code]) if response.status_code and response.status_code >= 400 else None
 
 
 class _AbstractResult(ABC):
 
     def __init__(self, response: KGRequestWithResponseContext):
         self.message: Optional[str] = response.content[
             "message"] if response.content and "message" in response.content else None
```

### Comparing `ebrains_kg_core-0.9.8/setup.py` & `ebrains_kg_core-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 from setuptools import setup
 
 long_description = "This is a client library to access the EBRAINS KG core API via python."
 
 setup(
     name='ebrains_kg_core',
-    version='0.9.8',
+    version='0.9.9',
     packages=['kg_core'],
     package_data = {
         'kg_core': ['py.typed'],
     },
     install_requires=['requests', 'pydantic'],
     author='EBRAINS',
     scripts=[],
```

