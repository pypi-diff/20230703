# Comparing `tmp/pulp-glue-0.19.2.tar.gz` & `tmp/pulp-glue-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-0.19.2.tar", last modified: Mon May 22 12:50:47 2023, max compression
+gzip compressed data, was "pulp-glue-0.20.0.tar", last modified: Mon Jul  3 12:15:26 2023, max compression
```

## Comparing `pulp-glue-0.19.2.tar` & `pulp-glue-0.20.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.081300 pulp-glue-0.19.2/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 12:50:47.081300 pulp-glue-0.19.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.069300 pulp-glue-0.19.2/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.073300 pulp-glue-0.19.2/pulp_glue/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/ansible/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/ansible/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.077300 pulp-glue-0.19.2/pulp_glue/certguard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/certguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/certguard/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/certguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.077300 pulp-glue-0.19.2/pulp_glue/common/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35601 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/common/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/common/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)    22792 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/common/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.077300 pulp-glue-0.19.2/pulp_glue/container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/container/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/container/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.077300 pulp-glue-0.19.2/pulp_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.077300 pulp-glue-0.19.2/pulp_glue/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/file/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.077300 pulp-glue-0.19.2/pulp_glue/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/python/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.081300 pulp-glue-0.19.2/pulp_glue/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/rpm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pulp_glue/rpm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:50:47.073300 pulp-glue-0.19.2/pulp_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 12:50:47.000000 pulp-glue-0.19.2/pulp_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-22 12:50:47.000000 pulp-glue-0.19.2/pulp_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:50:47.000000 pulp-glue-0.19.2/pulp_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 12:50:47.000000 pulp-glue-0.19.2/pulp_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 12:50:47.000000 pulp-glue-0.19.2/pulp_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:50:47.081300 pulp-glue-0.19.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-22 12:50:35.000000 pulp-glue-0.19.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.861583 pulp-glue-0.20.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.861583 pulp-glue-0.20.0/pulp_glue/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/ansible/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/ansible/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.861583 pulp-glue-0.20.0/pulp_glue/certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/certguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/certguard/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/certguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/pulp_glue/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38240 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/common/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/common/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/pulp_glue/container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/container/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/container/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/pulp_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/pulp_glue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/file/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/pulp_glue/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/python/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/pulp_glue/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/rpm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pulp_glue/rpm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:15:26.861583 pulp-glue-0.20.0/pulp_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-03 12:15:26.000000 pulp-glue-0.20.0/pulp_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 12:15:26.000000 pulp-glue-0.20.0/pulp_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:15:26.000000 pulp-glue-0.20.0/pulp_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 12:15:26.000000 pulp-glue-0.20.0/pulp_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 12:15:26.000000 pulp-glue-0.20.0/pulp_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:15:26.865583 pulp-glue-0.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-03 12:15:14.000000 pulp-glue-0.20.0/setup.py
```

### Comparing `pulp-glue-0.19.2/PKG-INFO` & `pulp-glue-0.20.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.19.2
+Version: 0.20.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.19.2/pulp_glue/ansible/context.py` & `pulp-glue-0.20.0/pulp_glue/ansible/context.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,115 +4,127 @@
     EntityDefinition,
     PluginRequirement,
     PulpContentContext,
     PulpDistributionContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
-    registered_repository_contexts,
 )
 from pulp_glue.common.i18n import get_translation
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
 class PulpAnsibleCollectionVersionContext(PulpContentContext):
+    PLUGIN = "ansible"
+    RESOURCE_TYPE = "collection_version"
     ENTITY = _("ansible collection version")
     ENTITIES = _("ansible collection versions")
     HREF = "ansible_collection_version_href"
     ID_PREFIX = "content_ansible_collection_versions"
     UPLOAD_ID: ClassVar[str] = "upload_collection"
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.7.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.7.0")]
 
     def upload(self, file: IO[bytes], **kwargs: Any) -> Any:  # type:ignore
         return self.call("upload", body={"file": file})
 
 
 class PulpAnsibleRoleContext(PulpContentContext):
+    PLUGIN = "ansible"
+    RESOURCE_TYPE = "role"
     ENTITY = _("ansible role")
     ENTITIES = _("ansible roles")
     HREF = "ansible_role_href"
     ID_PREFIX = "content_ansible_roles"
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.7.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.7.0")]
 
 
 class PulpAnsibleCollectionVersionSignatureContext(PulpContentContext):
+    PLUGIN = "ansible"
+    RESOURCE_TYPE = "collection_version_signature"
     ENTITY = _("ansible collection version signature")
     ENTITIES = _("ansible collection version signatures")
     HREF = _("ansible_collection_version_signature_href")
     ID_PREFIX = "content_ansible_collection_signatures"
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.12.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.12.0")]
 
     def create(
         self,
         body: EntityDefinition,
         parameters: Optional[Mapping[str, Any]] = None,
         non_blocking: bool = False,
     ) -> Any:
         self.pulp_ctx.needs_plugin(
-            PluginRequirement("ansible", min="0.13.0", feature=_("collection version creation"))
+            PluginRequirement(
+                "ansible", specifier=">=0.13.0", feature=_("collection version creation")
+            )
         )
         return super().create(body=body, parameters=parameters, non_blocking=non_blocking)
 
 
 class PulpAnsibleDistributionContext(PulpDistributionContext):
+    PLUGIN = "ansible"
+    RESOURCE_TYPE = "ansible"
     ENTITY = _("ansible distribution")
     ENTITIES = _("ansible distributions")
     HREF = "ansible_ansible_distribution_href"
     ID_PREFIX = "distributions_ansible_ansible"
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.7.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.7.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
         return body
 
 
 class PulpAnsibleRoleRemoteContext(PulpRemoteContext):
+    PLUGIN = "ansible"
+    RESOURCE_TYPE = "role"
     ENTITY = _("role remote")
     ENTITIES = _("role remotes")
     HREF = "ansible_role_remote_href"
     ID_PREFIX = "remotes_ansible_role"
     HREF_PATTERN = r"remotes/(?P<plugin>ansible)/(?P<resource_type>role)/"
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.7.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.7.0")]
 
 
 class PulpAnsibleCollectionRemoteContext(PulpRemoteContext):
+    PLUGIN = "ansible"
+    RESOURCE_TYPE = "collection"
     ENTITY = _("collection remote")
     ENTITIES = _("collection remotes")
     HREF = "ansible_collection_remote_href"
     ID_PREFIX = "remotes_ansible_collection"
     HREF_PATTERN = r"remotes/(?P<plugin>ansible)/(?P<resource_type>collection)/"
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.7.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.7.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if "requirements" in body.keys():
             body["requirements_file"] = body.pop("requirements")
         return body
 
 
 class PulpAnsibleRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "ansible_ansible_repository_version_href"
     ID_PREFIX = "repositories_ansible_ansible_versions"
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.7.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.7.0")]
 
 
 class PulpAnsibleRepositoryContext(PulpRepositoryContext):
+    PLUGIN = "ansible"
+    RESOURCE_TYPE = "ansible"
     HREF = "ansible_ansible_repository_href"
     ID_PREFIX = "repositories_ansible_ansible"
     ENTITY = _("ansible repository")
     ENTITIES = _("ansible repositories")
     VERSION_CONTEXT = PulpAnsibleRepositoryVersionContext
     CAPABILITIES = {
         "sync": [PluginRequirement("ansible")],
         "pulpexport": [PluginRequirement("ansible")],
     }
     NULLABLES = PulpRepositoryContext.NULLABLES | {"gpgkey"}
-    NEEDS_PLUGINS = [PluginRequirement("ansible", min="0.7.0")]
-
-
-registered_repository_contexts["ansible:ansible"] = PulpAnsibleRepositoryContext
+    NEEDS_PLUGINS = [PluginRequirement("ansible", specifier=">=0.7.0")]
```

### Comparing `pulp-glue-0.19.2/pulp_glue/certguard/context.py` & `pulp-glue-0.20.0/pulp_glue/certguard/context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from pulp_glue.common.context import PluginRequirement
+from pulp_glue.common.context import PluginRequirement, PulpContentGuardContext
 from pulp_glue.common.i18n import get_translation
-from pulp_glue.core.context import PulpContentGuardContext
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
 class PulpX509CertGuardContext(PulpContentGuardContext):
+    PLUGIN = "certguard"
+    RESOURCE_TYPE = "x509"
     ENTITY = _("x509 certguard")
     ENTITIES = _("x509 certguards")
     HREF = "certguard_x509_cert_guard_href"
     ID_PREFIX = "contentguards_certguard_x509"
-    NEEDS_PLUGINS = [PluginRequirement("certguard", min="1.4.0")]
+    NEEDS_PLUGINS = [PluginRequirement("certguard", specifier=">=1.4.0")]
 
 
 class PulpRHSMCertGuardContext(PulpContentGuardContext):
+    PLUGIN = "certguard"
+    RESOURCE_TYPE = "rhsm"
     ENTITY = _("RHSM certguard")
     ENTITIES = _("RHSM certguards")
     HREF = "certguard_r_h_s_m_cert_guard_href"
     ID_PREFIX = "contentguards_certguard_rhsm"
-    NEEDS_PLUGINS = [PluginRequirement("certguard", min="1.4.0")]
+    NEEDS_PLUGINS = [PluginRequirement("certguard", specifier=">=1.4.0")]
```

### Comparing `pulp-glue-0.19.2/pulp_glue/common/context.py` & `pulp-glue-0.20.0/pulp_glue/common/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 import datetime
 import os
 import re
 import sys
 import time
-from typing import (
-    IO,
-    Any,
-    ClassVar,
-    Dict,
-    List,
-    Mapping,
-    NamedTuple,
-    Optional,
-    Set,
-    Type,
-    Union,
-    cast,
-)
+from typing import IO, Any, ClassVar, Dict, List, Mapping, Optional, Set, Type, Union, cast
 
-from packaging.version import parse as parse_version
+from packaging.specifiers import SpecifierSet
 from requests import HTTPError
 
 from pulp_glue.common.i18n import get_translation
 from pulp_glue.common.openapi import OpenAPI, OpenAPIError
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 DEFAULT_LIMIT = 25
-BATCH_SIZE = 25
+BATCH_SIZE = 1000
 DATETIME_FORMATS = [
     "%Y-%m-%dT%H:%M:%S.%fZ",  # Pulp format
     "%Y-%m-%d",  # intl. format
     "%Y-%m-%d %H:%M:%S",  # ... with time
     "%Y-%m-%dT%H:%M:%S",  # ... with time and T as a separator
     "%y/%m/%d",  # US format
     "%y/%m/%d %h:%M:%S %p",  # ... with time
@@ -50,20 +37,47 @@
 class PreprocessedEntityDefinition(Dict[str, Any]):
     pass
 
 
 EntityDefinition = Union[Dict[str, Any], PreprocessedEntityDefinition]
 
 
-class PluginRequirement(NamedTuple):
-    name: str
-    min: Optional[str] = None
-    max: Optional[str] = None
-    feature: Optional[str] = None
-    inverted: bool = False
+class PluginRequirement:
+    def __init__(
+        self,
+        name: str,
+        min: Optional[str] = None,
+        max: Optional[str] = None,
+        feature: Optional[str] = None,
+        inverted: bool = False,
+        specifier: Optional[Union[str, SpecifierSet]] = None,
+    ):
+        self.name = name
+        self.feature = feature
+        self.inverted = inverted
+        if min is None and max is None:
+            specifier = specifier or ""
+        else:
+            assert specifier is None
+            specifier = ""
+            separator = ""
+            if min:
+                specifier += f">={min}"
+                separator = ","
+            if max:
+                specifier += f"{separator}<{max}"
+        if isinstance(specifier, SpecifierSet):
+            self.specifier = specifier
+        else:
+            self.specifier = SpecifierSet(specifier, prereleases=True)
+
+    def __contains__(self, version: Optional[str]) -> bool:
+        if version is None:
+            return self.inverted
+        return (version in self.specifier) != self.inverted
 
 
 class PulpException(Exception):
     pass
 
 
 class PulpNoWait(Exception):
@@ -109,53 +123,55 @@
         timeout: int,
         domain: str = "default",
         format: Optional[str] = None,  # Deprecated
     ) -> None:
         self._api: Optional[OpenAPI] = None
         self._api_root: str = api_root
         self._api_kwargs = api_kwargs
-        self._needed_plugins: List[PluginRequirement] = [PluginRequirement("core", min="3.11.0")]
+        self._needed_plugins: List[PluginRequirement] = [
+            PluginRequirement("core", specifier=">=3.11.0")
+        ]
         self.isatty: bool = sys.stdout.isatty()
         self.pulp_domain: str = domain
 
         self.background_tasks: bool = background_tasks
         self.timeout: int = timeout
         self.start_time: Optional[datetime.datetime] = None
 
     def _patch_api_spec(self) -> None:
         # A place for last minute fixes to the api_spec.
         # WARNING: Operations are already indexed at this point.
         api_spec = self.api.api_spec
-        if self.has_plugin(PluginRequirement("core", max="3.20.0")):
+        if self.has_plugin(PluginRequirement("core", specifier="<3.20.0")):
             for method, path in self.api.operations.values():
                 operation = api_spec["paths"][path][method]
                 if method == "get" and "parameters" in operation:
                     for parameter in operation["parameters"]:
                         if (
                             parameter["name"] == "ordering"
                             and parameter["in"] == "query"
                             and "schema" in parameter
                             and parameter["schema"]["type"] == "string"
                         ):
                             parameter["schema"] = {"type": "array", "items": {"type": "string"}}
                             parameter["explode"] = False
                             parameter["style"] = "form"
-        if self.has_plugin(PluginRequirement("core", max="3.22.0")):
+        if self.has_plugin(PluginRequirement("core", specifier="<3.22.0")):
             for method, path in self.api.operations.values():
                 operation = api_spec["paths"][path][method]
                 if method == "get" and "parameters" in operation:
                     for parameter in operation["parameters"]:
                         if (
                             parameter["name"] in ["fields", "exclude_fields"]
                             and parameter["in"] == "query"
                             and "schema" in parameter
                             and parameter["schema"]["type"] == "string"
                         ):
                             parameter["schema"] = {"type": "array", "items": {"type": "string"}}
-        if self.has_plugin(PluginRequirement("core", max="99.99.0")):
+        if self.has_plugin(PluginRequirement("core", specifier="<99.99.0")):
             # https://github.com/pulp/pulpcore/issues/3634
             for operation_id, (method, path) in self.api.operations.items():
                 if (
                     operation_id == "repository_versions_list"
                     or (
                         operation_id.startswith("repositories_")
                         and operation_id.endswith("_versions_list")
@@ -167,21 +183,21 @@
                         if (
                             parameter["name"] == "content__in"
                             and parameter["in"] == "query"
                             and "schema" in parameter
                             and parameter["schema"]["type"] == "string"
                         ):
                             parameter["schema"] = {"type": "array", "items": {"type": "string"}}
-        if self.has_plugin(PluginRequirement("file", min="1.10.0", max="1.11.0")):
+        if self.has_plugin(PluginRequirement("file", specifier=">=1.10.0,<1.11.0")):
             operation = api_spec["paths"]["{file_file_alternate_content_source_href}refresh/"][
                 "post"
             ]
             operation.pop("requestBody")
         if self.has_plugin(
-            PluginRequirement("python", max="99.99.0.dev")
+            PluginRequirement("python", specifier="<99.99.0.dev")
         ):  # TODO Add version bounds
             python_remote_serializer = api_spec["components"]["schemas"]["python.PythonRemote"]
             patched_python_remote_serializer = api_spec["components"]["schemas"][
                 "Patchedpython.PythonRemote"
             ]
             for prop in ("includes", "excludes"):
                 python_remote_serializer["properties"][prop]["type"] = "array"
@@ -383,56 +399,38 @@
                 )
             )
 
     def has_plugin(
         self,
         plugin_requirement: PluginRequirement,
     ) -> bool:
-        if not self.component_versions:
-            # Prior to 3.9 we do not have this information.
-            # Assume we have no plugin installed.
-            return not plugin_requirement.inverted
         version: Optional[str] = self.component_versions.get(plugin_requirement.name)
-        if version is None:
-            return plugin_requirement.inverted
-        if plugin_requirement.min is not None:
-            if parse_version(version) < parse_version(plugin_requirement.min):
-                return plugin_requirement.inverted
-        if plugin_requirement.max is not None:
-            if parse_version(version) >= parse_version(plugin_requirement.max):
-                return plugin_requirement.inverted
-        return not plugin_requirement.inverted
+        return version in plugin_requirement
 
     def needs_plugin(
         self,
         plugin_requirement: PluginRequirement,
     ) -> None:
         if self._api is not None:
             if not self.has_plugin(plugin_requirement):
-                specifier = plugin_requirement.name
-                separator = ""
-                if plugin_requirement.min is not None:
-                    specifier += f">={plugin_requirement.min}"
-                    separator = ","
-                if plugin_requirement.max is not None:
-                    specifier += f"{separator}<{plugin_requirement.max}"
+                component = f"{plugin_requirement.name}{plugin_requirement.specifier}"
                 feature = plugin_requirement.feature or _("this command")
                 if plugin_requirement.inverted:
                     msg = _(
-                        "The server provides the pulp component '{specifier}',"
+                        "The server provides the pulp component '{component}',"
                         " which prevents the use of {feature}."
                         " See 'pulp status' for installed components."
                     )
                 else:
                     msg = _(
-                        "The server does not provide the pulp component '{specifier}',"
+                        "The server does not provide the pulp component '{component}',"
                         " which is needed to use {feature}."
                         " See 'pulp status' for installed components."
                     )
-                raise PulpException(msg.format(specifier=specifier, feature=feature))
+                raise PulpException(msg.format(component=component, feature=feature))
         else:
             # Schedule for later checking
             self._needed_plugins.append(plugin_requirement)
 
 
 class PulpEntityContext:
     """
@@ -450,15 +448,15 @@
     NULLABLES: ClassVar[Set[str]] = set()
     # List of necessary plugin to operate such an entity in the server
     NEEDS_PLUGINS: ClassVar[List[PluginRequirement]] = []
     # Subclasses can specify version dependent capabilities here
     # e.g. `CAPABILITIES = {
     #           "feature1": [
     #               PluginRequirement("file"),
-    #               PluginRequirement("core", min="3.7.0")
+    #               PluginRequirement("core", specifier=">=3.7.0")
     #           ]
     #       }
     CAPABILITIES: ClassVar[Dict[str, List[PluginRequirement]]] = {}
     HREF_PATTERN: str
 
     # Hidden values for the lazy entity lookup
     _entity: Optional[EntityDefinition]
@@ -772,35 +770,54 @@
         "max_retries",
         "total_timeout",
         "connect_timeout",
         "sock_connect_timeout",
         "sock_read_timeout",
         "rate_limit",
     }
+    TYPE_REGISTRY: Dict[str, Type["PulpRemoteContext"]] = {}
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if hasattr(cls, "PLUGIN") and hasattr(cls, "RESOURCE_TYPE"):
+            cls.TYPE_REGISTRY[f"{cls.PLUGIN}:{cls.RESOURCE_TYPE}"] = cls
 
 
 class PulpPublicationContext(PulpEntityContext):
     ENTITY = _("publication")
     ENTITIES = _("publications")
     ID_PREFIX = "publications"
     HREF_PATTERN = r"publications/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
+    TYPE_REGISTRY: Dict[str, Type["PulpPublicationContext"]] = {}
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if hasattr(cls, "PLUGIN") and hasattr(cls, "RESOURCE_TYPE"):
+            cls.TYPE_REGISTRY[f"{cls.PLUGIN}:{cls.RESOURCE_TYPE}"] = cls
 
     def list(self, limit: int, offset: int, parameters: Dict[str, Any]) -> List[Any]:
         if parameters.get("repository") is not None:
             self.pulp_ctx.needs_plugin(
-                PluginRequirement("core", min="3.20.0", feature=_("repository filter"))
+                PluginRequirement("core", specifier=">=3.20.0", feature=_("repository filter"))
             )
         return super().list(limit, offset, parameters)
 
 
 class PulpDistributionContext(PulpEntityContext):
     ENTITY = _("distribution")
     ENTITIES = _("distributions")
     ID_PREFIX = "distributions"
     HREF_PATTERN = r"distributions/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
+    NULLABLES = {"content_guard", "publication", "remote", "repository", "repository_version"}
+    TYPE_REGISTRY: Dict[str, Type["PulpDistributionContext"]] = {}
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if hasattr(cls, "PLUGIN") and hasattr(cls, "RESOURCE_TYPE"):
+            cls.TYPE_REGISTRY[f"{cls.PLUGIN}:{cls.RESOURCE_TYPE}"] = cls
 
 
 class PulpRepositoryVersionContext(PulpEntityContext):
     ENTITY = _("repository version")
     ENTITIES = _("repository versions")
     ID_PREFIX = "repository_versions"
     repository_ctx: "PulpRepositoryContext"
@@ -823,23 +840,29 @@
 class PulpRepositoryContext(PulpEntityContext):
     ENTITY = _("repository")
     ENTITIES = _("repositories")
     HREF_PATTERN = r"repositories/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
     ID_PREFIX = "repositories"
     VERSION_CONTEXT: ClassVar[Type[PulpRepositoryVersionContext]] = PulpRepositoryVersionContext
     NULLABLES = {"description", "retain_repo_versions"}
+    TYPE_REGISTRY: Dict[str, Type["PulpRepositoryContext"]] = {}
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if hasattr(cls, "PLUGIN") and hasattr(cls, "RESOURCE_TYPE"):
+            cls.TYPE_REGISTRY[f"{cls.PLUGIN}:{cls.RESOURCE_TYPE}"] = cls
 
     def get_version_context(self) -> PulpRepositoryVersionContext:
         return self.VERSION_CONTEXT(self.pulp_ctx, self)
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if "retain_repo_versions" in body:
-            self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.13.0"))
-        if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.13.0", max="3.15.0")):
+            self.pulp_ctx.needs_plugin(PluginRequirement("core", specifier=">=3.13.0"))
+        if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.13.0,<3.15.0")):
             # "retain_repo_versions" has been named "retained_versions" until pulpcore 3.15
             # https://github.com/pulp/pulpcore/pull/1472
             if "retain_repo_versions" in body:
                 body["retained_versions"] = body.pop("retain_repo_versions")
         return body
 
     def sync(self, href: Optional[str] = None, body: Optional[EntityDefinition] = None) -> Any:
@@ -862,29 +885,35 @@
         return self.call("modify", parameters={self.HREF: href or self.pulp_href}, body=body)
 
 
 class PulpContentContext(PulpEntityContext):
     ENTITY = _("content")
     ENTITIES = _("content")
     ID_PREFIX = "content"
+    TYPE_REGISTRY: Dict[str, Type["PulpContentContext"]] = {}
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if hasattr(cls, "PLUGIN") and hasattr(cls, "RESOURCE_TYPE"):
+            cls.TYPE_REGISTRY[f"{cls.PLUGIN}:{cls.RESOURCE_TYPE}"] = cls
 
     def upload(
         self,
         file: IO[bytes],
         chunk_size: int,
         repository: Optional[PulpRepositoryContext],
         **kwargs: Any,
     ) -> Any:
         """Create a content unit by uploading a file"""
         self.needs_capability("upload")
         size = os.path.getsize(file.name)
         body: Dict[str, Any] = {**kwargs}
         if chunk_size > size:
             body["file"] = file
-        elif self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.20.0")):
+        elif self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.20.0")):
             from pulp_glue.core.context import PulpUploadContext
 
             upload_href = PulpUploadContext(self.pulp_ctx).upload_file(file, chunk_size)
             body["upload"] = upload_href
         else:
             from pulp_glue.core.context import PulpArtifactContext
 
@@ -896,22 +925,44 @@
 
 
 class PulpACSContext(PulpEntityContext):
     ENTITY = _("ACS")
     ENTITIES = _("ACSes")
     HREF_PATTERN = r"acs/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
     ID_PREFIX = "acs"
+    TYPE_REGISTRY: Dict[str, Type["PulpACSContext"]] = {}
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if hasattr(cls, "PLUGIN") and hasattr(cls, "RESOURCE_TYPE"):
+            cls.TYPE_REGISTRY[f"{cls.PLUGIN}:{cls.RESOURCE_TYPE}"] = cls
 
     def refresh(self, href: Optional[str] = None) -> Any:
         return self.call("refresh", parameters={self.HREF: href or self.pulp_href})
 
 
+class PulpContentGuardContext(PulpEntityContext):
+    ENTITY = "content guard"
+    ENTITIES = "content guards"
+    ID_PREFIX = "contentguards"
+    HREF_PATTERN = r"contentguards/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
+    NULLABLES = {"description"}
+    TYPE_REGISTRY: Dict[str, Type["PulpContentGuardContext"]] = {}
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if hasattr(cls, "PLUGIN") and hasattr(cls, "RESOURCE_TYPE"):
+            cls.TYPE_REGISTRY[f"{cls.PLUGIN}:{cls.RESOURCE_TYPE}"] = cls
+
+
 EntityFieldDefinition = Union[None, str, PulpEntityContext]
 
 
 ##############################################################################
 # Registries for Contexts of different sorts
 # A command can use these to identify e.g. all repository types known to the CLI
 # Note that it will only be fully populated, once all plugins are loaded.
+# This is deprecated. Please specify PLUGIN and RESOURCE_TYPE on the context instead.
 
-
-registered_repository_contexts: Dict[str, Type[PulpRepositoryContext]] = {}
+registered_repository_contexts: Dict[
+    str, Type[PulpRepositoryContext]
+] = PulpRepositoryContext.TYPE_REGISTRY
```

### Comparing `pulp-glue-0.19.2/pulp_glue/common/i18n.py` & `pulp-glue-0.20.0/pulp_glue/common/i18n.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.2/pulp_glue/common/openapi.py` & `pulp-glue-0.20.0/pulp_glue/common/openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # copyright (c) 2020, Matthias Dellweg
 # GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import base64
 import datetime
 import json
 import os
+from contextlib import suppress
 from io import BufferedReader
 from typing import IO, Any, Callable, Dict, List, Optional, Tuple, Union
 from urllib.parse import urljoin
 
 import requests
 import urllib3
 
@@ -202,14 +203,17 @@
                 param = params.pop(name)
                 param_spec = param_specs.pop(name)
                 param_schema = param_spec.get("schema")
                 if param_schema:
                     param = self.validate_schema(param_schema, name, param)
 
                 if isinstance(param, List):
+                    if not param:
+                        # Don't propagate an empty list here
+                        continue
                     # Check if we need to implode the list
                     style = (
                         param_spec.get("style") or "form"
                         if param_in in ("query", "cookie")
                         else "simple"
                     )
                     explode: bool = param_spec.get("explode", style == "form")
@@ -238,15 +242,58 @@
             schema_name = schema_ref[21:]
             schema = self.api_spec["components"]["schemas"][schema_name]
 
         if value is None and schema.get("nullable", False):
             return None
 
         schema_type = schema.get("type", "string")
-        if schema_type == "object":
+        allOf = schema.get("allOf")
+        anyOf = schema.get("anyOf")
+        oneOf = schema.get("oneOf")
+        not_schema = schema.get("not")
+        if allOf:
+            old_value = value
+            value = self.validate_schema(allOf[0], name, value)
+            for sub_schema in allOf[1:]:
+                # TODO check if it is possible to combine non object types.
+                value.update(self.validate_schema(sub_schema, name, old_value))
+        elif anyOf:
+            for sub_schema in anyOf:
+                with suppress(OpenAPIValidationError):
+                    value = self.validate_schema(sub_schema, name, value)
+                    break
+            else:
+                raise OpenAPIValidationError(
+                    _("No schema in anyOf validated for {name}.").format(name=name)
+                )
+        elif oneOf:
+            old_value = value
+            found_valid = False
+            for sub_schema in anyOf:
+                with suppress(OpenAPIValidationError):
+                    value = self.validate_schema(sub_schema, name, old_value)
+                    if found_valid:
+                        raise OpenAPIValidationError(
+                            _("Multiple schemas in oneOf validated for {name}.").format(name=name)
+                        )
+                    found_valid = True
+            if not found_valid:
+                raise OpenAPIValidationError(
+                    _("No schema in anyOf validated for {name}.").format(name=name)
+                )
+        elif not_schema:
+            try:
+                self.validate_schema(not_schema, name, value)
+            except OpenAPIValidationError:
+                pass
+            else:
+                raise OpenAPIValidationError(
+                    _("Forbidden schema for {name} validated.").format(name=name)
+                )
+        elif schema_type == "object":
             value = self.validate_object(schema, name, value)
         elif schema_type == "array":
             value = self.validate_array(schema, name, value)
         elif schema_type == "string":
             value = self.validate_string(schema, name, value)
         elif schema_type == "integer":
             value = self.validate_integer(schema, name, value)
@@ -297,14 +344,20 @@
     def validate_array(self, schema: Any, name: str, value: Any) -> List[Any]:
         if not isinstance(value, List):
             raise OpenAPIValidationError(_("'{name}' is expected to be a list.").format(name=name))
         item_schema = schema["items"]
         return [self.validate_schema(item_schema, name, item) for item in value]
 
     def validate_string(self, schema: Any, name: str, value: Any) -> Union[str, UploadType]:
+        enum = schema.get("enum")
+        if enum:
+            if value not in enum:
+                raise OpenAPIValidationError(
+                    _("'{name}' is not one of the valid choices.").format(name=name)
+                )
         schema_format = schema.get("format")
         if schema_format == "date":
             if not isinstance(value, datetime.date):
                 raise OpenAPIValidationError(
                     _("'{name}' is expected to be a date.").format(name=name)
                 )
             return value.strftime(ISO_DATE_FORMAT)
```

### Comparing `pulp-glue-0.19.2/pulp_glue/container/context.py` & `pulp-glue-0.20.0/pulp_glue/container/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,103 +5,111 @@
     PluginRequirement,
     PulpContentContext,
     PulpDistributionContext,
     PulpEntityContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
-    registered_repository_contexts,
 )
 from pulp_glue.common.i18n import get_translation
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
 class PulpContainerBlobContext(PulpContentContext):
+    PLUGIN = "container"
+    RESOURCE_TYPE = "blob"
     ENTITY = _("container blob")
     ENTITIES = _("container blobs")
     HREF = "container_blob_href"
     ID_PREFIX = "content_container_blobs"
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
 
 
 class PulpContainerManifestContext(PulpContentContext):
+    PLUGIN = "container"
+    RESOURCE_TYPE = "manifest"
     ENTITY = _("container manifest")
     ENTITIES = _("container manifests")
     HREF = "container_manifest_href"
     ID_PREFIX = "content_container_manifests"
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
 
 
 class PulpContainerTagContext(PulpContentContext):
+    PLUGIN = "container"
+    RESOURCE_TYPE = "tag"
     ENTITY = _("container tag")
     ENTITIES = _("container tags")
     HREF = "container_tag_href"
     ID_PREFIX = "content_container_tags"
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
 
     def find(self, **kwargs: Any) -> Any:
         if "digest" in kwargs and isinstance(kwargs["digest"], str):
             kwargs["digest"] = [kwargs["digest"]]
         return super().find(**kwargs)
 
 
 class PulpContainerNamespaceContext(PulpEntityContext):
     ENTITY = _("container namespace")
     ENTITIES = _("container namespaces")
     HREF = "container_container_namespace_href"
     ID_PREFIX = "pulp_container_namespaces"
     HREF_PATTERN = r"(?P<plugin>pulp_container)/(?P<resource_type>namespaces)/"
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
-    CAPABILITIES = {"roles": [PluginRequirement("container", min="2.11.0")]}
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("container", specifier=">=2.11.0")]}
 
 
 class PulpContainerDistributionContext(PulpDistributionContext):
+    PLUGIN = "container"
+    RESOURCE_TYPE = "container"
     ENTITY = _("container distribution")
     ENTITIES = _("container distributions")
     HREF = "container_container_distribution_href"
     ID_PREFIX = "distributions_container_container"
-    NULLABLES = {"repository_version", "repository"}
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
-    CAPABILITIES = {"roles": [PluginRequirement("container", min="2.11.0")]}
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("container", specifier=">=2.11.0")]}
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
         return body
 
 
 class PulpContainerRemoteContext(PulpRemoteContext):
+    PLUGIN = "container"
+    RESOURCE_TYPE = "container"
     ENTITY = _("container remote")
     ENTITIES = _("container remotes")
     HREF = "container_container_remote_href"
     ID_PREFIX = "remotes_container_container"
     NULLABLES = PulpRemoteContext.NULLABLES | {"include_tags", "exclude_tags"}
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
-    CAPABILITIES = {"roles": [PluginRequirement("container", min="2.11.0")]}
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("container", specifier=">=2.11.0")]}
 
 
 class PulpContainerRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "container_container_repository_version_href"
     ID_PREFIX = "repositories_container_container_versions"
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
 
 
 class PulpContainerPushRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "container_container_push_repository_version_href"
     ID_PREFIX = "repositories_container_container_push_versions"
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
 
 
 class PulpContainerBaseRepositoryContext(PulpRepositoryContext):
-    NEEDS_PLUGINS = [PluginRequirement("container", min="2.3.0")]
+    NEEDS_PLUGINS = [PluginRequirement("container", specifier=">=2.3.0")]
 
     def tag(self, tag: str, digest: str) -> Any:
         self.needs_capability("tag")
         return self.call(
             "tag",
             parameters={self.HREF: self.pulp_href},
             body={"tag": tag, "digest": digest},
@@ -113,25 +121,27 @@
             "untag",
             parameters={self.HREF: self.pulp_href},
             body={"tag": tag},
         )
 
 
 class PulpContainerRepositoryContext(PulpContainerBaseRepositoryContext):
+    PLUGIN = "container"
+    RESOURCE_TYPE = "container"
     HREF = "container_container_repository_href"
     ID_PREFIX = "repositories_container_container"
     ENTITY = _("container repository")
     ENTITIES = _("container repositories")
     VERSION_CONTEXT = PulpContainerRepositoryVersionContext
     HREF_PATTERN = r"repositories/(?P<plugin>container)/(?P<resource_type>container)/"
     CAPABILITIES = {
         "sync": [PluginRequirement("container")],
-        "pulpexport": [PluginRequirement("container", min="2.8.0")],
-        "tag": [PluginRequirement("container", min="2.3.0")],
-        "roles": [PluginRequirement("container", min="2.11.0")],
+        "pulpexport": [PluginRequirement("container", specifier=">=2.8.0")],
+        "tag": [PluginRequirement("container", specifier=">=2.3.0")],
+        "roles": [PluginRequirement("container", specifier=">=2.11.0")],
     }
 
     def modify(
         self,
         href: Optional[str] = None,
         add_content: Optional[List[str]] = None,
         remove_content: Optional[List[str]] = None,
@@ -165,27 +175,25 @@
             "digests": digests,
             "media_types": media_types,
         }
         return self.call("copy_manifests", parameters={self.HREF: self.pulp_href}, body=body)
 
 
 class PulpContainerPushRepositoryContext(PulpContainerBaseRepositoryContext):
+    PLUGIN = "container"
+    RESOURCE_TYPE = "push"
     HREF = "container_container_push_repository_href"
     ID_PREFIX = "repositories_container_container_push"
     ENTITY = _("push container repository")
     ENTITIES = _("push container repositories")
     VERSION_CONTEXT = PulpContainerPushRepositoryVersionContext
     HREF_PATTERN = r"repositories/(?P<plugin>container)/(?P<resource_type>container-push)/"
     CAPABILITIES = {
-        "tag": [PluginRequirement("container", min="2.3.0")],
-        "roles": [PluginRequirement("container", min="2.11.0")],
-        "remove": [PluginRequirement("container", min="2.4.0")],
+        "tag": [PluginRequirement("container", specifier=">=2.3.0")],
+        "roles": [PluginRequirement("container", specifier=">=2.11.0")],
+        "remove": [PluginRequirement("container", specifier=">=2.4.0")],
     }
 
     def remove_image(self, digest: str) -> Any:
         self.needs_capability("remove")
         body = {"digest": digest}
         return self.call("remove_image", parameters={self.HREF: self.pulp_href}, body=body)
-
-
-registered_repository_contexts["container:container"] = PulpContainerRepositoryContext
-registered_repository_contexts["container:push"] = PulpContainerPushRepositoryContext
```

### Comparing `pulp-glue-0.19.2/pulp_glue/core/context.py` & `pulp-glue-0.20.0/pulp_glue/core/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import sys
 from typing import IO, Any, ClassVar, Dict, List, Optional
 
 from pulp_glue.common.context import (
     EntityDefinition,
     PluginRequirement,
+    PulpContentGuardContext,
     PulpContext,
     PulpEntityContext,
     PulpException,
 )
 from pulp_glue.common.i18n import get_translation
 
 translation = get_translation(__name__)
@@ -20,20 +21,20 @@
 class PulpAccessPolicyContext(PulpEntityContext):
     ENTITY = _("access policy")
     ENTITIES = _("access policies")
     HREF = "access_policy_href"
     ID_PREFIX = "access_policies"
 
     def reset(self) -> Any:
-        self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.17.0"))
+        self.pulp_ctx.needs_plugin(PluginRequirement("core", specifier=">=3.17.0"))
         return self.call("reset", parameters={self.HREF: self.pulp_href})
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
-        if not self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.17.0")):
+        if not self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.17.0")):
             if "creation_hooks" in body:
                 body["permissions_assignment"] = body.pop("creation_hooks")
         return body
 
 
 class PulpArtifactContext(PulpEntityContext):
     ENTITY = _("artifact")
@@ -84,15 +85,15 @@
 
 
 class PulpDomainContext(PulpEntityContext):
     ENTITY = _("Pulp domain")
     ENTITIES = _("Pulp domains")
     HREF = "domain_href"
     ID_PREFIX = "domains"
-    NEEDS_PLUGINS = [PluginRequirement("core", "3.23.0.dev")]
+    NEEDS_PLUGINS = [PluginRequirement("core", specifier=">=3.23.0")]
 
 
 class PulpExporterContext(PulpEntityContext):
     ENTITY = _("Pulp exporter")
     ENTITIES = _("Pulp exporters")
     HREF = "pulp_exporter_href"
     ID_PREFIX = "exporters_core_pulp"
@@ -112,27 +113,27 @@
 
 class PulpGroupContext(PulpEntityContext):
     ENTITY = _("user group")
     ENTITIES = _("user groups")
     # Handled by a workaround
     # HREF = "group_href"
     ID_PREFIX = "groups"
-    CAPABILITIES = {"roles": [PluginRequirement("core", min="3.17.0")]}
+    CAPABILITIES = {"roles": [PluginRequirement("core", specifier=">=3.17.0")]}
 
     @property
     def HREF(self) -> str:  # type:ignore
-        if not self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.17.0")):
+        if not self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.17.0")):
             return "auth_group_href"
         return "group_href"
 
 
 class PulpGroupPermissionContext(PulpEntityContext):
     ENTITY = _("group permission")
     ENTITIES = _("group permissions")
-    NEEDS_PLUGINS = [PluginRequirement("core", max="3.20.0", feature=_("group permissions"))]
+    NEEDS_PLUGINS = [PluginRequirement("core", specifier="<3.20.0", feature=_("group permissions"))]
     group_ctx: PulpGroupContext
 
     def __init__(self, pulp_ctx: PulpContext, group_ctx: PulpGroupContext) -> None:
         super().__init__(pulp_ctx)
         self.group_ctx = group_ctx
 
     def call(
@@ -156,15 +157,15 @@
             validate_body=validate_body,
         )
 
     def find(self, **kwargs: Any) -> Any:
         """Workaroud for the missing ability to filter"""
         # # TODO fix upstream and adjust to guard for the proper version
         # # https://pulp.plan.io/issues/8241
-        # if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.99.dev")):
+        # if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.99.dev")):
         #     # Workaround not needed anymore
         #     return super().find(**kwargs)
         search_result = self.list(limit=sys.maxsize, offset=0, parameters={})
         for key, value in kwargs.items():
             search_result = [res for res in search_result if res[key] == value]
         if len(search_result) != 1:
             raise PulpException(
@@ -184,40 +185,40 @@
     ENTITIES = _("group model permissions")
     # Handled by a workaround
     # HREF = "groups_model_permission_href"
     ID_PREFIX = "groups_model_permissions"
 
     @property
     def HREF(self) -> str:  # type:ignore
-        if not self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.17.0")):
+        if not self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.17.0")):
             return "auth_groups_model_permission_href"
         return "groups_model_permission_href"
 
 
 class PulpGroupObjectPermissionContext(PulpGroupPermissionContext):
     ENTITY = _("group object permission")
     ENTITIES = _("group object permissions")
     # Handled by a workaround
     # HREF = "groups_object_permission_href"
     ID_PREFIX = "groups_object_permissions"
 
     @property
     def HREF(self) -> str:  # type:ignore
-        if not self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.17.0")):
+        if not self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.17.0")):
             return "auth_groups_object_permission_href"
         return "groups_object_permission_href"
 
 
 class PulpGroupRoleContext(PulpEntityContext):
     ENTITY = _("group role")
     ENTITIES = _("group roles")
     HREF = "groups_group_role_href"
     ID_PREFIX = "groups_roles"
     NULLABLES = {"content_object"}
-    NEEDS_PLUGINS = [PluginRequirement("core", min="3.17.0", feature=_("group roles"))]
+    NEEDS_PLUGINS = [PluginRequirement("core", specifier=">=3.17.0", feature=_("group roles"))]
     group_ctx: PulpGroupContext
 
     def __init__(self, pulp_ctx: PulpContext, group_ctx: PulpGroupContext) -> None:
         super().__init__(pulp_ctx)
         self.group_ctx = group_ctx
 
     @property
@@ -231,83 +232,79 @@
     # Handled by a workaround
     # HREF = "groups_user_href"
     ID_PREFIX = "groups_users"
     group_ctx: PulpGroupContext
 
     @property
     def HREF(self) -> str:  # type:ignore
-        if not self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.17.0")):
+        if not self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.17.0")):
             return "auth_groups_user_href"
         return "groups_user_href"
 
     def __init__(self, pulp_ctx: PulpContext, group_ctx: PulpGroupContext) -> None:
         super().__init__(pulp_ctx)
         self.group_ctx = group_ctx
 
     @property
     def scope(self) -> Dict[str, Any]:
         return {self.group_ctx.HREF: self.group_ctx.pulp_href}
 
 
-class PulpContentGuardContext(PulpEntityContext):
-    ENTITY = "content guard"
-    ENTITIES = "content guards"
-    ID_PREFIX = "contentguards"
-    HREF_PATTERN = r"contentguards/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
-    NULLABLES = {"description"}
-
-
 class PulpContentRedirectContentGuardContext(PulpContentGuardContext):
+    PLUGIN = "core"
+    RESOURCE_TYPE = "content_redirect"
     ENTITY = "content redirect content guard"
     ENTITIES = "content redirect content guards"
     HREF = "content_redirect_content_guard_href"
     ID_PREFIX = "contentguards_core_content_redirect"
-    NEEDS_PLUGINS = [PluginRequirement("core", min="3.18.0")]
+    NEEDS_PLUGINS = [PluginRequirement("core", specifier=">=3.18.0")]
 
 
 class PulpImporterContext(PulpEntityContext):
     ENTITY = _("Pulp importer")
     ENTITIES = _("Pulp importers")
     HREF = "pulp_importer_href"
     ID_PREFIX = "importers_core_pulp"
 
 
 class PulpOrphanContext(PulpEntityContext):
     def cleanup(self, body: Optional[Dict[str, Any]] = None) -> Any:
         if body is not None:
             body = self.preprocess_entity(body)
             if "orphan_protection_time" in body:
-                self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.15.0"))
+                self.pulp_ctx.needs_plugin(PluginRequirement("core", specifier=">=3.15.0"))
         else:
             body = {}
-        if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.14.0")):
+        if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.14.0")):
             result = self.pulp_ctx.call("orphans_cleanup_cleanup", body=body)
         else:
             if body:
-                self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.14.0"))
+                self.pulp_ctx.needs_plugin(PluginRequirement("core", specifier=">=3.14.0"))
             result = self.pulp_ctx.call("orphans_delete")
         return result
 
 
 class PulpRbacContentGuardContext(PulpContentGuardContext):
+    PLUGIN = "core"
+    RESOURCE_TYPE = "rbac"
     ENTITY = "RBAC content guard"
     ENTITIES = "RBAC content guards"
     HREF = "r_b_a_c_content_guard_href"
     ID_PREFIX = "contentguards_core_rbac"
     DOWNLOAD_ROLE: ClassVar[str] = "core.rbaccontentguard_downloader"
-    CAPABILITIES = {"roles": [PluginRequirement("core", min="3.17.0")]}
-    NEEDS_PLUGINS = [PluginRequirement("core", min="3.15.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("core", specifier=">=3.17.0")]}
+    NEEDS_PLUGINS = [PluginRequirement("core", specifier=">=3.15.0")]
 
     def assign(
         self,
         href: Optional[str] = None,
         users: Optional[List[str]] = None,
         groups: Optional[List[str]] = None,
     ) -> Any:
-        if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.17.0")):
+        if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.17.0")):
             body: EntityDefinition = {"users": users, "groups": groups}
             body["role"] = self.DOWNLOAD_ROLE
             return self.call("add_role", parameters={self.HREF: href or self.pulp_href}, body=body)
         else:
             body = {"usernames": users, "groupnames": groups}
             return self.call(
                 "assign_permission", parameters={self.HREF: href or self.pulp_href}, body=body
@@ -315,15 +312,15 @@
 
     def remove(
         self,
         href: Optional[str] = None,
         users: Optional[List[str]] = None,
         groups: Optional[List[str]] = None,
     ) -> Any:
-        if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.17.0")):
+        if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.17.0")):
             body: EntityDefinition = {"users": users, "groups": groups}
             body["role"] = self.DOWNLOAD_ROLE
             return self.call(
                 "remove_role", parameters={self.HREF: href or self.pulp_href}, body=body
             )
         else:
             body = {"usernames": users, "groupnames": groups}
@@ -334,15 +331,15 @@
 
 class PulpRoleContext(PulpEntityContext):
     ENTITY = _("role")
     ENTITIES = _("roles")
     HREF = "role_href"
     ID_PREFIX = "roles"
     NULLABLES = {"description"}
-    NEEDS_PLUGINS = [PluginRequirement("core", min="3.17.0")]
+    NEEDS_PLUGINS = [PluginRequirement("core", specifier=">=3.17.0")]
 
 
 class PulpSigningServiceContext(PulpEntityContext):
     ENTITY = _("signing service")
     ENTITIES = _("signing services")
     HREF = "signing_service_href"
     ID_PREFIX = "signing_services"
@@ -350,47 +347,47 @@
 
 
 class PulpTaskContext(PulpEntityContext):
     ENTITY = _("task")
     ENTITIES = _("tasks")
     HREF = "task_href"
     ID_PREFIX = "tasks"
-    CAPABILITIES = {"roles": [PluginRequirement("core", min="3.17.0")]}
+    CAPABILITIES = {"roles": [PluginRequirement("core", specifier=">=3.17.0")]}
 
     resource_context: Optional[PulpEntityContext] = None
 
     def list(self, limit: int, offset: int, parameters: Dict[str, Any]) -> List[Any]:
         if (
             parameters.get("logging_cid") is not None
             or parameters.get("logging_cid__contains") is not None
         ):
-            self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.14.0"))
-        if not self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.22.0")):
+            self.pulp_ctx.needs_plugin(PluginRequirement("core", specifier=">=3.14.0"))
+        if not self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.22.0")):
             parameters = parameters.copy()
             reserved_resources = parameters.pop("reserved_resources", None)
             exclusive_resources = parameters.pop("exclusive_resources", None)
             shared_resources = parameters.pop("shared_resources", None)
             if (
                 parameters.pop("reserved_resources__in", None)
                 or parameters.pop("exclusive_resources__in", None)
                 or parameters.pop("shared_resources__in", None)
             ):
-                self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.22.0"))
+                self.pulp_ctx.needs_plugin(PluginRequirement("core", specifier=">=3.22.0"))
             reserved_resources_record = []
             if reserved_resources:
                 reserved_resources_record.append(reserved_resources)
             if exclusive_resources:
                 reserved_resources_record.append(exclusive_resources)
             if shared_resources:
                 reserved_resources_record.append("shared:" + shared_resources)
             if len(reserved_resources_record) > 1:
                 self.pulp_ctx.needs_plugin(
                     PluginRequirement(
                         "core",
-                        min="3.22.0",
+                        specifier=">=3.22.0",
                         feature=_("specify multiple reserved resources"),
                     ),
                 )
             parameters["reserved_resources_record"] = reserved_resources_record
 
         return super().list(limit=limit, offset=offset, parameters=parameters)
 
@@ -406,40 +403,40 @@
             task = self.pulp_ctx.wait_for_task(task, expect_cancel=True)
             self.pulp_ctx.echo(_("Done."), err=True)
         return task
 
     @property
     def scope(self) -> Dict[str, Any]:
         if self.resource_context:
-            if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.22.0")):
+            if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.22.0")):
                 return {"reserved_resources": self.resource_context.pulp_href}
             else:
                 return {"reserved_resources_record": [self.resource_context.pulp_href]}
         else:
             return {}
 
     def purge(
         self,
         finished_before: Optional[datetime.datetime],
         states: Optional[List[str]],
     ) -> Any:
-        self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.17.0"))
+        self.pulp_ctx.needs_plugin(PluginRequirement("core", specifier=">=3.17.0"))
         body: Dict[str, Any] = {}
         if finished_before:
             body["finished_before"] = finished_before
         if states:
             body["states"] = states
         return self.call(
             "purge",
             body=body,
         )
 
     def summary(self) -> Dict[str, int]:
         task_states = ["waiting", "skipped", "running", "completed", "failed", "canceled"]
-        if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.14.0")):
+        if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.14.0")):
             task_states.append("canceling")
         result = {}
         for state in task_states:
             payload = {"limit": 1, "state": state}
             result[state] = self.call("list", parameters=payload)["count"]
         return result
```

### Comparing `pulp-glue-0.19.2/pulp_glue/file/context.py` & `pulp-glue-0.20.0/pulp_glue/file/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,38 +6,41 @@
     PulpACSContext,
     PulpContentContext,
     PulpDistributionContext,
     PulpPublicationContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
-    registered_repository_contexts,
 )
 from pulp_glue.common.i18n import get_translation
 from pulp_glue.core.context import PulpArtifactContext
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
 class PulpFileACSContext(PulpACSContext):
+    PLUGIN = "file"
+    RESOURCE_TYPE = "file"
     ENTITY = _("file ACS")
     ENTITIES = _("file ACSes")
     HREF = "file_file_alternate_content_source_href"
     ID_PREFIX = "acs_file_file"
-    NEEDS_PLUGINS = [PluginRequirement("file", min="1.9.0")]
-    CAPABILITIES = {"roles": [PluginRequirement("file", min="1.11.0")]}
+    NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.9.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("file", specifier=">=1.11.0")]}
 
 
 class PulpFileContentContext(PulpContentContext):
+    PLUGIN = "file"
+    RESOURCE_TYPE = "file"
     ENTITY = _("file content")
     ENTITIES = _("file content")
     HREF = "file_file_content_href"
     ID_PREFIX = "content_file_files"
-    NEEDS_PLUGINS = [PluginRequirement("file", min="1.6.0")]
+    NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.6.0")]
     CAPABILITIES = {"upload": []}
 
     def create(
         self,
         body: EntityDefinition,
         parameters: Optional[Mapping[str, Any]] = None,
         non_blocking: bool = False,
@@ -47,80 +50,84 @@
             body["artifact"] = PulpArtifactContext(
                 self.pulp_ctx, entity={"sha256": body.pop("sha256")}
             )
         return super().create(body=body, parameters=parameters, non_blocking=non_blocking)
 
 
 class PulpFileDistributionContext(PulpDistributionContext):
+    PLUGIN = "file"
+    RESOURCE_TYPE = "file"
     ENTITY = _("file distribution")
     ENTITIES = _("file distributions")
     HREF = "file_file_distribution_href"
     ID_PREFIX = "distributions_file_file"
-    NULLABLES = {"publication", "repository"}
-    CAPABILITIES = {"roles": [PluginRequirement("file", min="1.11.0")]}
-    NEEDS_PLUGINS = [PluginRequirement("file", min="1.6.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("file", specifier=">=1.11.0")]}
+    NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.6.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
-        if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.16.0")):
+        if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.16.0")):
             if "repository" in body and "publication" not in body:
                 body["publication"] = None
             if "repository" not in body and "publication" in body:
                 body["repository"] = None
         return body
 
 
 class PulpFilePublicationContext(PulpPublicationContext):
+    PLUGIN = "file"
+    RESOURCE_TYPE = "file"
     ENTITY = _("file publication")
     ENTITIES = _("file publications")
     HREF = "file_file_publication_href"
     ID_PREFIX = "publications_file_file"
-    CAPABILITIES = {"roles": [PluginRequirement("file", min="1.11.0")]}
+    CAPABILITIES = {"roles": [PluginRequirement("file", specifier=">=1.11.0")]}
     NULLABLES = {"manifest"}
-    NEEDS_PLUGINS = [PluginRequirement("file", min="1.6.0")]
+    NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.6.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
         return body
 
 
 class PulpFileRemoteContext(PulpRemoteContext):
+    PLUGIN = "file"
+    RESOURCE_TYPE = "file"
     ENTITY = _("file remote")
     ENTITIES = _("file remotes")
     HREF = "file_file_remote_href"
     ID_PREFIX = "remotes_file_file"
-    CAPABILITIES = {"roles": [PluginRequirement("file", min="1.11.0")]}
-    NEEDS_PLUGINS = [PluginRequirement("file", min="1.6.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("file", specifier=">=1.11.0")]}
+    NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.6.0")]
 
 
 class PulpFileRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "file_file_repository_version_href"
     ID_PREFIX = "repositories_file_file_versions"
-    NEEDS_PLUGINS = [PluginRequirement("file", min="1.6.0")]
+    NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.6.0")]
 
 
 class PulpFileRepositoryContext(PulpRepositoryContext):
+    PLUGIN = "file"
+    RESOURCE_TYPE = "file"
     HREF = "file_file_repository_href"
     ENTITY = _("file repository")
     ENTITIES = _("file repositories")
     ID_PREFIX = "repositories_file_file"
     VERSION_CONTEXT = PulpFileRepositoryVersionContext
     CAPABILITIES = {
         "sync": [PluginRequirement("file")],
         "pulpexport": [PluginRequirement("file")],
-        "roles": [PluginRequirement("file", min="1.11.0")],
+        "roles": [PluginRequirement("file", specifier=">=1.11.0")],
     }
     NULLABLES = PulpRepositoryContext.NULLABLES.union({"manifest"})
-    NEEDS_PLUGINS = [PluginRequirement("file", min="1.6.0")]
+    NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.6.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if "autopublish" in body:
-            self.pulp_ctx.needs_plugin(PluginRequirement("file", min="1.7.0"))
+            self.pulp_ctx.needs_plugin(PluginRequirement("file", specifier=">=1.7.0"))
         return body
-
-
-registered_repository_contexts["file:file"] = PulpFileRepositoryContext
```

### Comparing `pulp-glue-0.19.2/pulp_glue/python/context.py` & `pulp-glue-0.20.0/pulp_glue/python/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,99 +3,104 @@
     PluginRequirement,
     PulpContentContext,
     PulpDistributionContext,
     PulpPublicationContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
-    registered_repository_contexts,
 )
 from pulp_glue.common.i18n import get_translation
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
 class PulpPythonContentContext(PulpContentContext):
+    PLUGIN = "python"
+    RESOURCE_TYPE = "package"
     ENTITY = _("python package")
     ENTITIES = _("python packages")
     HREF = "python_python_package_content_href"
     ID_PREFIX = "content_python_packages"
-    NEEDS_PLUGINS = [PluginRequirement("python", min="3.1.0")]
+    NEEDS_PLUGINS = [PluginRequirement("python", specifier=">=3.1.0")]
     CAPABILITIES = {"upload": []}
 
 
 class PulpPythonDistributionContext(PulpDistributionContext):
+    PLUGIN = "python"
+    RESOURCE_TYPE = "python"
     ENTITY = _("python distribution")
     ENTITIES = _("python distributions")
     HREF = "python_python_distribution_href"
     ID_PREFIX = "distributions_python_pypi"
-    NULLABLES = {"publication", "repository"}
-    NEEDS_PLUGINS = [PluginRequirement("python", min="3.1.0")]
+    NEEDS_PLUGINS = [PluginRequirement("python", specifier=">=3.1.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if "allow_uploads" in body:
-            self.pulp_ctx.needs_plugin(PluginRequirement("python", min="3.4.0"))
+            self.pulp_ctx.needs_plugin(PluginRequirement("python", specifier=">=3.4.0"))
         if "remote" in body:
-            self.pulp_ctx.needs_plugin(PluginRequirement("python", min="3.6.0"))
-        if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.16.0")):
+            self.pulp_ctx.needs_plugin(PluginRequirement("python", specifier=">=3.6.0"))
+        if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.16.0")):
             if "repository" in body and "publication" not in body:
                 body["publication"] = None
             if "repository" not in body and "publication" in body:
                 body["repository"] = None
         return body
 
 
 class PulpPythonPublicationContext(PulpPublicationContext):
+    PLUGIN = "python"
+    RESOURCE_TYPE = "python"
     ENTITY = _("python publication")
     ENTITIES = _("python publications")
     HREF = "python_python_publication_href"
     ID_PREFIX = "publications_python_pypi"
-    NEEDS_PLUGINS = [PluginRequirement("python", min="3.1.0")]
+    NEEDS_PLUGINS = [PluginRequirement("python", specifier=">=3.1.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
         return body
 
 
 class PulpPythonRemoteContext(PulpRemoteContext):
+    PLUGIN = "python"
+    RESOURCE_TYPE = "python"
     ENTITY = _("python remote")
     ENTITIES = _("python remotes")
     HREF = "python_python_remote_href"
     ID_PREFIX = "remotes_python_python"
-    NEEDS_PLUGINS = [PluginRequirement("python", min="3.1.0")]
+    NEEDS_PLUGINS = [PluginRequirement("python", specifier=">=3.1.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if "keep_latest_packages" in body or "package_types" in body or "exclude_platforms" in body:
-            self.pulp_ctx.needs_plugin(PluginRequirement("python", min="3.2.0"))
+            self.pulp_ctx.needs_plugin(PluginRequirement("python", specifier=">=3.2.0"))
         return body
 
 
 class PulpPythonRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "python_python_repository_version_href"
     ID_PREFIX = "repositories_python_python_versions"
-    NEEDS_PLUGINS = [PluginRequirement("python", min="3.1.0")]
+    NEEDS_PLUGINS = [PluginRequirement("python", specifier=">=3.1.0")]
 
 
 class PulpPythonRepositoryContext(PulpRepositoryContext):
+    PLUGIN = "python"
+    RESOURCE_TYPE = "python"
     HREF = "python_python_repository_href"
     ENTITY = _("python repository")
     ENTITIES = _("python repositories")
     ID_PREFIX = "repositories_python_python"
     VERSION_CONTEXT = PulpPythonRepositoryVersionContext
     CAPABILITIES = {"sync": [PluginRequirement("python")]}
-    NEEDS_PLUGINS = [PluginRequirement("python", min="3.1.0")]
+    NEEDS_PLUGINS = [PluginRequirement("python", specifier=">=3.1.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if "autopublish" in body:
-            self.pulp_ctx.needs_plugin(PluginRequirement("python", min="3.3.0"))
+            self.pulp_ctx.needs_plugin(PluginRequirement("python", specifier=">=3.3.0"))
         return body
-
-
-registered_repository_contexts["python:python"] = PulpPythonRepositoryContext
```

### Comparing `pulp-glue-0.19.2/pulp_glue.egg-info/PKG-INFO` & `pulp-glue-0.20.0/pulp_glue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.19.2
+Version: 0.20.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.19.2/pulp_glue.egg-info/SOURCES.txt` & `pulp-glue-0.20.0/pulp_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.2/setup.py` & `pulp-glue-0.20.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,21 @@
     name="pulp-glue",
     description="Version agnostic glue library to talk to pulpcore's REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pulp Team",
     author_email="pulp-list@redhat.com",
     url="https://github.com/pulp/pulp-cli",
-    version="0.19.2",
+    version="0.20.0",
     packages=plugin_packages,
     package_data={"": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=[
-        "packaging",
-        "setuptools",
-        "requests~=2.24",
+        "packaging>=20.0,<24",
+        "requests>=2.24.0,<2.32",
     ],
     license="GPLv2+",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Other Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
```

