# Comparing `tmp/dapp_runner-0.1.2.tar.gz` & `tmp/dapp_runner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapp_runner-0.1.2.tar", max compression
+gzip compressed data, was "dapp_runner-0.2.0.tar", max compression
```

## Comparing `dapp_runner-0.1.2.tar` & `dapp_runner-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     7652 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/LICENSE
--rw-r--r--   0        0        0    10333 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/README.md
--rw-r--r--   0        0        0       59 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/__init__.py
--rw-r--r--   0        0        0     3694 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/__main__.py
--rw-r--r--   0        0        0     3024 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/_util.py
--rw-r--r--   0        0        0      168 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/descriptor/__init__.py
--rw-r--r--   0        0        0     4687 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/descriptor/base.py
--rw-r--r--   0        0        0     1452 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/descriptor/config.py
--rw-r--r--   0        0        0     8510 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/descriptor/dapp.py
--rw-r--r--   0        0        0      948 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/descriptor/parser.py
--rw-r--r--   0        0        0     2576 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/log.py
--rw-r--r--   0        0        0     5407 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/runner/__init__.py
--rw-r--r--   0        0        0      116 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/runner/error.py
--rw-r--r--   0        0        0      743 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/runner/infile.py
--rw-r--r--   0        0        0      904 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/runner/payload.py
--rw-r--r--   0        0        0    14085 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/runner/runner.py
--rw-r--r--   0        0        0     5044 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/runner/service.py
--rw-r--r--   0        0        0     2295 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/runner/streams.py
--rw-r--r--   0        0        0      458 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/dapp_runner/singleton.py
--rw-r--r--   0        0        0     4893 2023-06-13 06:34:56.587257 dapp_runner-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    11673 1970-01-01 00:00:00.000000 dapp_runner-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/LICENSE
+-rw-r--r--   0        0        0    10333 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/README.md
+-rw-r--r--   0        0        0       59 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/__init__.py
+-rw-r--r--   0        0        0     4410 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/__main__.py
+-rw-r--r--   0        0        0     3024 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/_util.py
+-rw-r--r--   0        0        0       46 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/api/__init__.py
+-rw-r--r--   0        0        0      462 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/api/__main__.py
+-rw-r--r--   0        0        0      208 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/descriptor/__init__.py
+-rw-r--r--   0        0        0     6856 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/descriptor/base.py
+-rw-r--r--   0        0        0     1807 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/descriptor/config.py
+-rw-r--r--   0        0        0    11108 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/descriptor/dapp.py
+-rw-r--r--   0        0        0      136 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/descriptor/error.py
+-rw-r--r--   0        0        0     3472 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/descriptor/manifest.py
+-rw-r--r--   0        0        0      945 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/descriptor/parser.py
+-rw-r--r--   0        0        0     2576 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/log.py
+-rw-r--r--   0        0        0     6427 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/runner/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/runner/error.py
+-rw-r--r--   0        0        0      743 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/runner/infile.py
+-rw-r--r--   0        0        0     2852 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/runner/payload.py
+-rw-r--r--   0        0        0    17637 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/runner/runner.py
+-rw-r--r--   0        0        0     5044 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/runner/service.py
+-rw-r--r--   0        0        0     2295 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/runner/streams.py
+-rw-r--r--   0        0        0      458 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/dapp_runner/singleton.py
+-rw-r--r--   0        0        0     5233 2023-07-03 08:27:23.137318 dapp_runner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11845 1970-01-01 00:00:00.000000 dapp_runner-0.2.0/PKG-INFO
```

### Comparing `dapp_runner-0.1.2/LICENSE` & `dapp_runner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapp_runner-0.1.2/README.md` & `dapp_runner-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dapp_runner-0.1.2/dapp_runner/__main__.py` & `dapp_runner-0.2.0/dapp_runner/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def _get_run_dir(run_id: str) -> Path:
     app_dir = _get_data_dir() / run_id
     app_dir.mkdir(exist_ok=True, parents=True)
     return app_dir
 
 
-@_cli.command()
+@_cli.command(context_settings={"show_default": True})
 @click.option(
     "--data",
     "-d",
     type=Path,
     help="Path to the data file.",
 )
 @click.option(
@@ -81,14 +81,30 @@
     "--config",
     "-c",
     type=Path,
     required=True,
     help="Path to the file containing yagna-specific config.",
 )
 @click.option(
+    "--enable-api",
+    is_flag=True,
+    default=False,
+    help="Configuration override for the `api.enabled` key.",
+)
+@click.option(
+    "--api-host",
+    type=str,
+    help="Configuration override for the `api.host` key.",
+)
+@click.option(
+    "--api-port",
+    type=int,
+    help="Configuration override for the `api.port` key.",
+)
+@click.option(
     "--dev",
     is_flag=True,
     default=False,
     help="Run in a development mode (enable warnings).",
 )
 @click.option(
     "--debug",
@@ -102,14 +118,19 @@
     required=True,
     type=Path,
 )
 @click.option(
     "--silent",
     is_flag=True,
 )
+@click.option(
+    "--skip-manifest-validation",
+    is_flag=True,
+    help="Don't validate and report issues with the manifest, its certificate or signature.",
+)
 def start(
     descriptors: Tuple[Path],
     config: Path,
     **kwargs,
 ) -> None:
     """Start a dApp based on the provided configuration and set of descriptor files."""
     dapp_dict = load_yamls(*descriptors)
@@ -125,15 +146,20 @@
 
     # Provide default values for data, log and state parameters
     for param_name in ["data", "log", "state", "commands"]:
         param_value = kwargs[param_name]
         if not param_value:
             kwargs[param_name] = app_dir / param_name
 
-    start_runner(config_dict, dapp_dict, log_level=log_level, **kwargs)
+    api_config_dict = {
+        k: kwargs.pop(k)
+        for k in set(kwargs.keys()).intersection({"enable_api", "api_host", "api_port"})
+    }
+
+    start_runner(config_dict, api_config_dict, dapp_dict, log_level=log_level, **kwargs)
 
 
 @_cli.command()
 @click.argument(
     "descriptors",
     nargs=-1,
     required=True,
```

### Comparing `dapp_runner-0.1.2/dapp_runner/_util.py` & `dapp_runner-0.2.0/dapp_runner/_util.py`

 * *Files identical despite different names*

### Comparing `dapp_runner-0.1.2/dapp_runner/descriptor/config.py` & `dapp_runner-0.2.0/dapp_runner/descriptor/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,75 @@
 """Class definitions for the Dapp Runner's configuration descriptor."""
 import os
-from dataclasses import dataclass, field
 from typing import Optional
 
-from .base import BaseDescriptor
+from pydantic import BaseModel, Field, validator
 
 
-@dataclass
-class YagnaConfig(BaseDescriptor["YagnaConfig"]):
+class YagnaConfig(BaseModel):
     """Yagna daemon configuration properties.
 
     Properties describing the local requestor daemon configuration that
     the Dapp Runner will use to run services on Golem.
     """
 
-    def __app_key__factory(value: str):  # type: ignore [misc]  # noqa
+    subnet_tag: Optional[str]
+    api_url: Optional[str] = None
+    gsb_url: Optional[str] = None
+    app_key: Optional[str] = None
+
+    class Config:  # noqa: D106
+        extra = "forbid"
+
+    @validator("app_key", always=True)
+    def __app_key__extrapolate(cls, v):
         # TODO this should be applied uniformly across any fields,
         # for now, making an exception for the app key
 
-        if value and value.startswith("$"):
-            return os.environ[value[1:]]
-
-        return value
+        if v and v.startswith("$"):
+            return os.environ[v[1:]]
 
-    subnet_tag: Optional[str]
-    api_url: Optional[str] = None
-    gsb_url: Optional[str] = None
-    app_key: Optional[str] = field(metadata={"factory": __app_key__factory}, default=None)
+        return v
 
 
-@dataclass
-class PaymentConfig:
+class PaymentConfig(BaseModel):
     """Requestor's payment config."""
 
     budget: float
     driver: str
     network: str
 
+    class Config:  # noqa: D106
+        extra = "forbid"
+
 
-@dataclass
-class LimitsConfig:
+class LimitsConfig(BaseModel):
     """Limits of the running app."""
 
     startup_timeout: Optional[int] = None  # seconds
     max_running_time: Optional[int] = None  # seconds
 
+    class Config:  # noqa: D106
+        extra = "forbid"
+
+
+class ApiConfig(BaseModel):
+    """Configuration of the built-in API Server."""
 
-@dataclass
-class Config(BaseDescriptor["Config"]):
+    enabled: bool = False
+    host: str = "127.0.0.1"
+    port: int = 8000
+
+    class Config:  # noqa: D106
+        extra = "forbid"
+
+
+class Config(BaseModel):
     """Root configuration descriptor for the Dapp Runner."""
 
     yagna: YagnaConfig
     payment: PaymentConfig
-    limits: LimitsConfig = field(default_factory=LimitsConfig)
+    limits: LimitsConfig = Field(default_factory=LimitsConfig)
+    api: ApiConfig = Field(default_factory=ApiConfig)
+
+    class Config:  # noqa: D106
+        extra = "forbid"
```

### Comparing `dapp_runner-0.1.2/dapp_runner/descriptor/dapp.py` & `dapp_runner-0.2.0/dapp_runner/descriptor/dapp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """Class definitions for the Dapp Runner's dapp descriptor."""
 import logging
-from dataclasses import dataclass, field, fields
-from typing import Any, Dict, Final, List, Optional, Tuple
+import re
+from typing import Any, Dict, Final, List, Optional, Tuple, Union
 
 import networkx
+from pydantic import Field, PrivateAttr, validator
 
+from yapapi.ctx import Activity
+from yapapi.network import Network
+from yapapi.network import Node as NetworkNode
 from yapapi.payload import vm
 
-from .base import BaseDescriptor, DescriptorError
+from .base import GaomBase
+from .error import DescriptorError
 
 NETWORK_DEFAULT_NAME: Final[str] = "default"
 
 PAYLOAD_RUNTIME_VM: Final[str] = "vm"
 PAYLOAD_RUNTIME_VM_MANIFEST: Final[str] = "vm/manifest"
 
 VM_PAYLOAD_CAPS_KWARG: Final[str] = "capabilities"
@@ -22,160 +27,254 @@
 
 VM_CAPS_VPN: Final[str] = "vpn"
 VM_CAPS_MANIFEST: Final[str] = "manifest-support"
 
 logger = logging.getLogger(__name__)
 
 
-@dataclass
-class PayloadDescriptor:
+class PayloadDescriptor(GaomBase):
     """Yapapi Payload descriptor."""
 
     runtime: str
-    params: Dict[str, Any] = field(default_factory=dict)
+    params: Dict[str, Any] = Field(default_factory=dict)
 
+    class Config:  # noqa: D106
+        extra = "forbid"
 
-@dataclass
-class PortMapping:
+
+class PortMapping(GaomBase):
     """Port mapping for a http proxy."""
 
     remote_port: int
     local_port: Optional[int] = None
+    address: Optional[str] = Field(runtime=True)
+
+    class Config:  # noqa: D106
+        extra = "forbid"
 
 
-@dataclass
-class ProxyDescriptor(BaseDescriptor["ProxyDescriptor"]):
+class ProxyDescriptor(GaomBase):
     """Proxy descriptor."""
 
-    def __ports_factory(value: str) -> PortMapping:  # type: ignore [misc]  # noqa
-        ports = [int(p) for p in value.split(":")]
-        port_mappping = PortMapping(remote_port=ports.pop())
-        if ports:
-            port_mappping.local_port = ports.pop()
-        return port_mappping
+    ports: List[PortMapping]
 
-    ports: List[PortMapping] = field(metadata={"factory": __ports_factory})
+    class Config:  # noqa: D106
+        extra = "forbid"
+
+    @validator("ports", pre=True, each_item=True)
+    def __ports__preprocess(cls, v):
+        if isinstance(v, PortMapping) or isinstance(v, dict):
+            return v
+
+        try:
+            return re.match(
+                r"^(?:(?P<local_port>\d+)\:)?(?P<remote_port>\d+)$", v
+            ).groupdict()  # type: ignore [union-attr]
+        except AttributeError:
+            raise ValueError("Expected format: `remote_port` or `local_port:remote_port`.")
 
 
-@dataclass
 class HttpProxyDescriptor(ProxyDescriptor):
     """HTTP proxy descriptor."""
 
 
-@dataclass
 class SocketProxyDescriptor(ProxyDescriptor):
     """TCP socket proxy descriptor."""
 
 
-@dataclass
-class CommandDescriptor:
+class CommandDescriptor(GaomBase):
     """Exeunit command descriptor."""
 
     cmd: str = EXEUNIT_CMD_RUN
-    params: Dict[str, Any] = field(default_factory=dict)
+    params: Dict[str, Any] = Field(default_factory=dict)
+
+    class Config:  # noqa: D106
+        extra = "forbid"
 
     @classmethod
-    def load(cls, c):
-        """Load a command descriptor from its serialized representation."""
-        if isinstance(c, list):
+    def canonize_input(cls, value: Union[str, List, Dict]):
+        """Convert a single command descriptor to its canonical form.
+
+        Supported formats:
+
+        ```yaml
+        init:
+          - test:
+              args: ["/bin/rm", "/var/log/nginx/access.log", "/var/log/nginx/error.log"]
+              from: "aa"
+              to: "b"
+          - aaa:
+              args: ["/bin/rm", "/var/log/nginx/access.log", "/var/log/nginx/error.log"]
+              from: "aa"
+              to: "b"
+        ```
+
+        ```yaml
+        init: ["/docker-entrypoint.sh"]
+        ```
+
+        ```yaml
+        init:
+          - run:
+              args:
+                - "/docker-entrypoint.sh"
+        ```
+
+        ```yaml
+        init:
+            - ["/docker-entrypoint.sh"]
+            - ["/bin/chmod", "a+x", "/"]
+            - ["/bin/sh", "-c", 'echo "Hello from inside Golem!" > /usr/share/nginx/html/index.html']  # noqa
+        ```
+
+        """
+        if isinstance(value, list):
             # assuming it's a `run`
-            return cls(params={"args": c})
-        elif isinstance(c, dict) and len(c.keys()) == 1:
+            return {"cmd": EXEUNIT_CMD_RUN, "params": {"args": value}}
+        elif isinstance(value, dict) and len(value.keys()) == 1:
             # we don't want to support malformed entries
             # where multiple commands are present in a single dictionary
-            for cmd, params in c.items():
+            for cmd, params in value.items():
                 if cmd == EXEUNIT_CMD_RUN and isinstance(params, list):
                     # support shorthand `run` notation:
                     # - run:
                     #    - ["/golem/run/simulate_observations_ctl.py", "--start"]
                     params = {"args": params}
-                return CommandDescriptor(cmd=cmd, params=params)
+                return {"cmd": cmd, "params": params}
+        elif isinstance(value, dict) and set(value.keys()) == {"cmd", "params"}:
+            return value
         else:
-            raise DescriptorError(f"Cannot parse the command descriptor `{c}`.")
+            raise DescriptorError(f"Cannot parse the command descriptor `{value}`.")
 
 
-class _CommandDescriptorList:
-    """Preprocessor for the exescript commands."""
+class NetworkNodeDescriptor(GaomBase):
+    """GAOM model reflecting yapapi's network `Node`."""
 
-    def _process_command(self, c):
-        self.commands.append(CommandDescriptor.load(c))
+    node_id: str
+    ip: str
 
-    def __init__(self):
-        self.commands = list()
+    class Config:  # noqa: D106
+        extra = "forbid"
 
     @classmethod
-    def load_commands(cls, value) -> List[CommandDescriptor]:
-        """Load the contents of the commands list."""
-        commands_list = cls()
+    def from_network_node(cls, network_node: NetworkNode):
+        """Get a NetworkNodeDescriptor based on a `NetworkNode` object."""
+        return cls(
+            node_id=network_node.node_id,
+            ip=network_node.ip,
+        )
 
-        if len(value) > 0 and isinstance(value[0], str):
-            # support single line definitions, e.g. `init: ["/docker-entrypoint.sh"]`
-            value = [value]
 
-        for c in value:
-            commands_list._process_command(c)
+class ActivityDescriptor(GaomBase):
+    """GAOM model referring to yagna's Activity."""
+
+    id: str
+
+    class Config:  # noqa: D106
+        extra = "forbid"
+
+    @classmethod
+    def from_activity(cls, activity: Activity):
+        """Get an ActivityDescriptor based on an `Activity` object."""
+        return cls(id=activity.id)
+
+
+class AgreementDescriptor(GaomBase):
+    """GAOM model referring to yagna's Agreement."""
+
+    id: str
+    provider_id: str
+    provider_name: str
 
-        return commands_list.commands
+    class Config:  # noqa: D106
+        extra = "forbid"
 
 
-@dataclass
-class ServiceDescriptor(BaseDescriptor["ServiceDescriptor"]):
+class ServiceDescriptor(GaomBase):
     """Yapapi Service descriptor."""
 
     payload: str
-    init: List[CommandDescriptor] = field(
-        metadata={"load": _CommandDescriptorList.load_commands}, default_factory=list
-    )
+    init: List[CommandDescriptor] = Field(default_factory=list)
     network: Optional[str] = None
-    ip: List[str] = field(default_factory=list)
+    ip: List[str] = Field(default_factory=list)
     http_proxy: Optional[HttpProxyDescriptor] = None
     tcp_proxy: Optional[SocketProxyDescriptor] = None
-    depends_on: List[str] = field(default_factory=list)
+    depends_on: List[str] = Field(default_factory=list)
 
+    state: Optional[str] = Field(runtime=True, default=None)
+    network_node: Optional[NetworkNodeDescriptor] = Field(runtime=True, default=None)
+    agreement: Optional[AgreementDescriptor] = Field(runtime=True, default=None)
+    activity: Optional[ActivityDescriptor] = Field(runtime=True, default=None)
+
+    class Config:  # noqa: D106
+        extra = "forbid"
+
+    @validator("init", pre=True)
+    def __init__canonize_commands(cls, v):
+        if len(v) and isinstance(v[0], str):
+            # support single line definitions, e.g. `init: ["/docker-entrypoint.sh"]`
+            v = [v]
+
+        return [CommandDescriptor.canonize_input(v) for v in v]
 
-@dataclass
-class NetworkDescriptor(BaseDescriptor["NetworkDescriptor"]):
+
+class NetworkDescriptor(GaomBase):
     """Yapapi network descriptor."""
 
-    ip: str = field(default="192.168.0.0/24")
+    ip: str = "192.168.0.0/24"
     owner_ip: Optional[str] = None
     mask: Optional[str] = None
     gateway: Optional[str] = None
 
+    class Config:  # noqa: D106
+        extra = "forbid"
 
-@dataclass
-class MetaDescriptor:
+    @classmethod
+    def from_network(cls, network: Network):
+        """Get a NetworkDescriptor based on yapapi's `Network` object."""
+        return cls(
+            ip=network.network_address,
+            owner_ip=network.owner_ip,
+            mask=network.netmask,
+            gateway=network.gateway,
+        )
+
+
+class MetaDescriptor(GaomBase):
     """Meta descriptor for the app.
 
     Silently ignores unknown fields.
     """
 
     name: str = ""
     description: str = ""
     author: str = ""
     version: str = ""
 
-    def __init__(self, **kwargs):
-        for f in fields(self):
-            if f.name in kwargs:
-                setattr(self, f.name, f.type(kwargs.pop(f.name)))
-        if kwargs:
-            logger.debug("Unrecognized `meta` fields: %s", kwargs)
-
 
-@dataclass
-class DappDescriptor(BaseDescriptor["DappDescriptor"]):
+class DappDescriptor(GaomBase):
     """Root dapp descriptor for the Dapp Runner."""
 
     payloads: Dict[str, PayloadDescriptor]
     nodes: Dict[str, ServiceDescriptor]
-    networks: Dict[str, NetworkDescriptor] = field(default_factory=dict)
-    meta: MetaDescriptor = field(default_factory=MetaDescriptor)
+    networks: Dict[str, NetworkDescriptor] = Field(default_factory=dict)
+    meta: MetaDescriptor = Field(default_factory=MetaDescriptor)
+
+    _dependency_graph: networkx.DiGraph = PrivateAttr()
 
-    _dependency_graph: networkx.DiGraph = field(init=False)
+    class Config:  # noqa: D106
+        extra = "forbid"
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.__validate_nodes()
+        self.__implicit_proxy_init()
+        self.__implicit_vpn()
+        self.__implicit_manifest_support()
+        self._resolve_dependencies()
 
     def __validate_nodes(self):
         """Ensure that required payloads and optional networks are defined."""
         for node in self.nodes.values():
             if node.payload not in self.payloads:
                 raise DescriptorError(f"Undefined payload: `{node.payload}`")
             if node.network and node.network not in self.networks:
@@ -208,46 +307,43 @@
         for payload in self.payloads.values():
             if (
                 payload.runtime == PAYLOAD_RUNTIME_VM_MANIFEST
                 and VM_PAYLOAD_CAPS_KWARG not in payload.params
             ):
                 payload.params[VM_PAYLOAD_CAPS_KWARG] = [VM_CAPS_MANIFEST]
 
-    def _resolve_dependencies(self):
-        """Resolve instantiation priorities."""
-
-        # initialize the dependency graph and add a root node
-        self._dependency_graph: networkx.DiGraph = networkx.DiGraph()
-        self._dependency_graph.add_node(DEPENDENCY_ROOT)
-
-        # for now, we only care about the order of services,
-        # later we can enhance the dependency graph to
-        # take all the other entities into consideration
+    def _resolve_depends_on(self):
+        """Resolve dependencies from the `depends_on` clause."""
 
         for name, service in self.nodes.items():
             if service.depends_on:
                 for depends_name in service.depends_on:
                     if depends_name not in self.nodes:
                         raise DescriptorError(
                             f'Unmet `depends_on`: "{depends_name}"' f' in service: "{name}".'
                         )
                     self._dependency_graph.add_edge(name, depends_name)
             else:
                 self._dependency_graph.add_edge(DEPENDENCY_ROOT, name)
 
+    def _resolve_dependencies(self):
+        """Resolve instantiation priorities."""
+
+        # initialize the dependency graph and add a root node
+        self._dependency_graph: networkx.DiGraph = networkx.DiGraph()
+        self._dependency_graph.add_node(DEPENDENCY_ROOT)
+
+        # for now, we only care about the order of services,
+        # later we can enhance the dependency graph to
+        # take all the other entities into consideration
+        self._resolve_depends_on()
+
         if not networkx.is_directed_acyclic_graph(self._dependency_graph):
             raise DescriptorError("Service definition contains a circular `depends_on`.")
 
     def nodes_prioritized(self) -> List[Tuple[str, ServiceDescriptor]]:
         """Get a dict-items-like list of services, ordered by dependencies."""
         return [
             (name, self.nodes[name])
             for name in reversed(list(networkx.topological_sort(self._dependency_graph)))
             if name != DEPENDENCY_ROOT
         ]
-
-    def __post_init__(self):
-        self.__validate_nodes()
-        self.__implicit_proxy_init()
-        self.__implicit_vpn()
-        self.__implicit_manifest_support()
-        self._resolve_dependencies()
```

### Comparing `dapp_runner-0.1.2/dapp_runner/descriptor/parser.py` & `dapp_runner-0.2.0/dapp_runner/descriptor/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import yaml
 
 
 def load_yamls(*yaml_paths: Path) -> Dict[str, Any]:
     """Load the provided YAML files, merging their contents in a deep manner.
 
     The order of the files is relevant, that is: the first YAML is considered the base.
-    All of the remaining files are loaded one by one and deeply merged into the base.
+    All the remaining files are loaded one by one and deeply merged into the base.
 
     Returns a dict representing the result of all YAML files merged into the first one.
     """
 
     def _load_yaml(path: Path) -> Dict[str, Any]:
         with path.open() as f:
             return yaml.load(f, yaml.SafeLoader)
```

### Comparing `dapp_runner-0.1.2/dapp_runner/log.py` & `dapp_runner-0.2.0/dapp_runner/log.py`

 * *Files identical despite different names*

### Comparing `dapp_runner-0.1.2/dapp_runner/runner/__init__.py` & `dapp_runner-0.2.0/dapp_runner/runner/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Optional, TextIO
 
 from colors import cyan, green, magenta
 
 from dapp_runner._util import _print_env_info, cancel_and_await_tasks, json_encoder, utcnow
-from dapp_runner.descriptor import Config, DappDescriptor, DescriptorError
+from dapp_runner.descriptor import Config, DappDescriptor, DescriptorError, manifest
 from dapp_runner.log import enable_logger, log_name_to_level
 
 from .error import RunnerError
 from .infile import feed_from_file
 from .runner import Runner
 from .streams import RunnerStreamer
 
@@ -27,25 +27,39 @@
 def _running_time_elapsed(
     time_started: Optional[datetime],
     max_running_time: Optional[timedelta],
 ) -> bool:
     return bool(time_started and max_running_time and utcnow() > time_started + max_running_time)
 
 
+def _update_api_config(config: Config, api_config_dict: dict):
+    arg_field_map = {"enable_api": "enabled", "api_host": "host", "api_port": "port"}
+
+    for k, v in api_config_dict.items():
+        if v is not None:
+            setattr(config.api, arg_field_map[k], v)
+
+
 async def _run_app(
     config_dict: dict,
+    api_config_dict: dict,
     dapp_dict: dict,
     data_f: TextIO,
     state_f: TextIO,
     commands_f: Optional[TextIO],
     silent=False,
+    skip_manifest_validation=False,
 ):
     """Run the dapp using the Runner."""
-    config = Config.load(config_dict)
-    dapp = DappDescriptor.load(dapp_dict)
+    config = Config(**config_dict)
+    _update_api_config(config, api_config_dict)
+
+    dapp = DappDescriptor(**dapp_dict)
+    if not skip_manifest_validation:
+        manifest.verify_manifests(dapp)
 
     r = Runner(config=config, dapp=dapp)
     _print_env_info(r.golem)
     if dapp.meta.name:
         print(f"Starting app: {green(dapp.meta.name)}\n")
 
     await r.start()
@@ -79,47 +93,57 @@
         startup_timeout,
         max_running_time,
     )
 
     time_started: Optional[datetime] = None
 
     try:
-        while not r.dapp_started and utcnow() < r.commissioning_time + startup_timeout:
+        while (
+            not r.dapp_started
+            and not r.api_shutdown
+            and utcnow() < r.commissioning_time + startup_timeout
+        ):
             await asyncio.sleep(1)
 
-        if not r.dapp_started:
+        if not r.api_shutdown and not r.dapp_started:
             raise Exception(f"Failed to start instances before {startup_timeout} elapsed.")
 
         time_started = utcnow()
         logger.info("Application started.")
 
-        while r.dapp_started and not _running_time_elapsed(time_started, max_running_time):
+        while (
+            r.dapp_started
+            and not r.api_shutdown
+            and not _running_time_elapsed(time_started, max_running_time)
+        ):
             await asyncio.sleep(1)
     finally:
         if _running_time_elapsed(time_started, max_running_time):
             logger.info("Maximum running time: %s elapsed.", max_running_time)
 
         logger.info("Stopping the application...")
         await r.stop()
         await streamer.stop()
 
 
 def start_runner(
     config_dict: dict,
+    api_config_dict: dict,
     dapp_dict: dict,
     data: Path,
     state: Path,
     log: Path,
     dev: bool,
     debug: bool,
     log_level: str,
     commands: Optional[Path] = None,
     stdout: Optional[Path] = None,
     stderr: Optional[Path] = None,
     silent=False,
+    skip_manifest_validation=False,
 ):
     """Launch the runner in an asyncio loop and wait for its shutdown."""
 
     with ExitStack() as stack:
         state_f = stack.enter_context(open(str(state), "w", 1))
         data_f = stack.enter_context(open(str(data), "w", 1))
 
@@ -136,35 +160,46 @@
             file_log_level=log_name_to_level(log_level),
         )
 
         commands_f = stack.enter_context(open(str(commands), "w+", 1)) if commands else None
 
         loop = asyncio.get_event_loop()
         task = loop.create_task(
-            _run_app(config_dict, dapp_dict, data_f, state_f, commands_f, silent)
+            _run_app(
+                config_dict,
+                api_config_dict,
+                dapp_dict,
+                data_f,
+                state_f,
+                commands_f,
+                silent,
+                skip_manifest_validation,
+            )
         )
 
         try:
             loop.run_until_complete(task)
         except KeyboardInterrupt:
-            logger.info("Shutting down ...")
+            logger.info("SIGINT received, shutting down gracefully ...")
             try:
                 loop.run_until_complete(cancel_and_await_tasks(task))
             except KeyboardInterrupt:
-                logger.info("Shutdown interrupted")
+                logger.info(
+                    "Another SIGINT received, graceful shutdown interrupted, exiting immediately."
+                )
             else:
-                logger.info("Shutdown completed")
+                logger.info("Post-SIGINT graceful shutdown completed.")
         except Exception:  # noqa
             sys.stderr.write(traceback.format_exc())
 
 
 def verify_dapp(dapp_dict: dict):
     """Verify the passed app descriptor schema and report any encountered errors."""
     try:
-        dapp = DappDescriptor.load(dapp_dict)
+        dapp = DappDescriptor(**dapp_dict)
         print(dapp)
     except DescriptorError as e:
         print(e)
         return False
 
     return True
```

### Comparing `dapp_runner-0.1.2/dapp_runner/runner/infile.py` & `dapp_runner-0.2.0/dapp_runner/runner/infile.py`

 * *Files identical despite different names*

### Comparing `dapp_runner-0.1.2/dapp_runner/runner/runner.py` & `dapp_runner-0.2.0/dapp_runner/runner/runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 """Main Dapp Runner module."""
 import asyncio
 import logging
-from dataclasses import asdict
 from datetime import datetime
 from typing import Dict, Final, List, Optional
 
+import uvicorn
+
 from yapapi import Golem
+from yapapi.config import ApiConfig
 from yapapi.contrib.service.http_proxy import LocalHttpProxy
 from yapapi.contrib.service.socket_proxy import SocketProxy
 from yapapi.events import CommandExecuted
 from yapapi.network import Network
 from yapapi.payload import Payload
 from yapapi.services import Cluster, Service, ServiceState
 
 from dapp_runner._util import FreePortProvider, cancel_and_await_tasks, utcnow, utcnow_iso_str
 from dapp_runner.descriptor import Config, DappDescriptor
-from dapp_runner.descriptor.dapp import CommandDescriptor, PortMapping, ServiceDescriptor
+from dapp_runner.descriptor.dapp import (
+    ActivityDescriptor,
+    AgreementDescriptor,
+    CommandDescriptor,
+    NetworkDescriptor,
+    NetworkNodeDescriptor,
+    PortMapping,
+    ServiceDescriptor,
+)
 
 from .payload import get_payload
 from .service import DappService, get_service
 
 LOCAL_HTTP_PROXY_DATA_KEY: Final[str] = "local_proxy_address"
+LOCAL_HTTP_PROXY_URI: Final[str] = "http://localhost"
 LOCAL_TCP_PROXY_DATA_KEY: Final[str] = "local_tcp_proxy_address"
+LOCAL_TCP_PROXY_ADDRESS: Final[str] = "localhost"
 DEPENDENCY_WAIT_INTERVAL: Final[float] = 1.0
 
 logger = logging.getLogger(__name__)
 
 
 class Runner:
     """Distributed application runner.
 
     Taking the yagna configuration and distributed application descriptor, the Runner
     uses yapapi to run the desired app on Golem and allows interacting with it.
     """
 
+    _instance: Optional["Runner"] = None
+
     config: Config
     dapp: DappDescriptor
     golem: Golem
     clusters: Dict[str, Cluster]
     commissioning_time: Optional[datetime]
 
     _payloads: Dict[str, Payload]
@@ -50,24 +64,26 @@
     # TODO: Introduce ApplicationState instead of reusing ServiceState
     _desired_app_state: ServiceState
 
     data_queue: asyncio.Queue
     state_queue: asyncio.Queue
     command_queue: asyncio.Queue
 
+    api_server: Optional[uvicorn.Server]
+
     def __init__(self, config: Config, dapp: DappDescriptor):
         self.config = config
         self.dapp = dapp
 
         self.golem = Golem(
             budget=config.payment.budget,
             subnet_tag=config.yagna.subnet_tag,
             payment_driver=config.payment.driver,
             payment_network=config.payment.network,
-            app_key=config.yagna.app_key,
+            api_config=ApiConfig(app_key=config.yagna.app_key),  # type: ignore
         )
 
         self.clusters = {}
         self._payloads = {}
         self._http_proxies = {}
         self._tcp_proxies = {}
         self._networks = {}
@@ -75,18 +91,47 @@
         self.data_queue = asyncio.Queue()
         self.state_queue = asyncio.Queue()
         self.command_queue = asyncio.Queue()
         self._startup_finished = False
         self._desired_app_state = ServiceState.pending
 
         self._report_status_change()
+        Runner._instance = self
+
+        self.api_server = None
+        self.api_shutdown = False
+
+    @classmethod
+    def get_instance(cls):
+        """Get the Runner instance."""
+        return cls._instance
+
+    async def _serve_api(self):
+        assert self.api_server, "Uninitialized API server, call `_start_api` first."
+        try:
+            await self.api_server.serve()
+        finally:
+            # the uvicorn server seems to consume the SIGINT / CancelledError, so
+            # we have to manually mark its shutdown to trigger shutdown of the
+            # whole runner
+            self.api_shutdown = True
+
+    async def _start_api(self):
+        config = uvicorn.Config(
+            "dapp_runner.api:app", host=self.config.api.host, port=self.config.api.port
+        )
+        self.api_server = uvicorn.Server(config)
+        self._tasks.append(asyncio.create_task(self._serve_api()))
 
     async def _create_networks(self):
         for name, desc in self.dapp.networks.items():
-            self._networks[name] = await self.golem.create_network(**asdict(desc))
+            network = await self.golem.create_network(**desc.dict())
+            self._networks[name] = network
+
+            self.dapp.networks[name] = NetworkDescriptor.from_network(network)
 
     async def _load_payloads(self):
         for name, desc in self.dapp.payloads.items():
             self._payloads[name] = await get_payload(desc)
 
     async def _start_local_http_proxy(self, name: str, cluster: Cluster, port_mapping: PortMapping):
         # wait until the service is running before starting the proxy
@@ -94,38 +139,51 @@
             await asyncio.sleep(DEPENDENCY_WAIT_INTERVAL)
 
         port = port_mapping.local_port or FreePortProvider().get_free_port()
         proxy = LocalHttpProxy(cluster, port)
         await proxy.run()
 
         self._http_proxies[name] = proxy
-        self.data_queue.put_nowait({name: {LOCAL_HTTP_PROXY_DATA_KEY: f"http://localhost:{port}"}})
+        proxy_uri = f"{LOCAL_HTTP_PROXY_URI}:{port}"
+        self.data_queue.put_nowait({name: {LOCAL_HTTP_PROXY_DATA_KEY: proxy_uri}})
+
+        # update the GAOM mapping
+        port_mapping.local_port = port
+        port_mapping.address = proxy_uri
 
     async def _start_local_tcp_proxy(self, name: str, service: Service, port_mapping: PortMapping):
         # wait until the service is running before starting the proxy
         while not self._is_cluster_state(name, ServiceState.running):
             await asyncio.sleep(DEPENDENCY_WAIT_INTERVAL)
 
         port = port_mapping.local_port or FreePortProvider().get_free_port()
         proxy = SocketProxy([port])
         await proxy.run_server(service, port_mapping.remote_port)
 
         self._tcp_proxies[name] = proxy
-        self.data_queue.put_nowait({name: {LOCAL_TCP_PROXY_DATA_KEY: f"localhost:{port}"}})
+        proxy_address = f"{LOCAL_TCP_PROXY_ADDRESS}:{port}"
+        self.data_queue.put_nowait({name: {LOCAL_TCP_PROXY_DATA_KEY: proxy_address}})
+
+        # update the GAOM mapping
+        port_mapping.local_port = port
+        port_mapping.address = proxy_address
 
     async def _start_service(self, service_name: str, service_descriptor: ServiceDescriptor):
         # if this service depends on another, wait until the dependency is up
         if service_descriptor.depends_on:
             for depends_name in service_descriptor.depends_on:
                 while depends_name not in self.clusters or not self._is_cluster_state(
                     depends_name, ServiceState.running
                 ):
                     await asyncio.sleep(DEPENDENCY_WAIT_INTERVAL)
 
         logger.debug("Starting service: %s, descriptor: %s", service_name, service_descriptor)
+
+        service_descriptor.interpolate(self.dapp, is_runtime=True)
+
         cluster_class, run_params = await get_service(
             service_name, service_descriptor, self._payloads, self._networks
         )
         cluster = await self.start_cluster(service_name, cluster_class, run_params)
 
         # start the tasks for the local proxies so that
         # it doesn't delay the initialization process
@@ -145,32 +203,35 @@
                     )
 
         # launch queue listeners for all the service instances
         for idx in range(len(cluster.instances)):
             s = cluster.instances[idx]
             self._tasks.extend(
                 [
-                    asyncio.create_task(self._listen_state_queue(s)),
+                    asyncio.create_task(self._listen_state_queue(s, service_descriptor)),
                     asyncio.create_task(self._listen_data_queue(service_name, idx, s)),
                 ]
             )
 
     async def _start_services(self):
         for service_name, service_descriptor in self.dapp.nodes_prioritized():
             await self._start_service(service_name, service_descriptor)
 
         self._startup_finished = True
 
     async def start(self):
         """Start the Golem engine and the dapp."""
 
+        if self.config.api.enabled:
+            await self._start_api()
+
         self.commissioning_time = utcnow()
 
         # explicitly mark that we ultimately want app in "running" state,
-        #  marking app into "starting" sequence.
+        # marking app into "starting" sequence.
         self._desired_app_state = ServiceState.running
 
         await self.golem.start()
 
         await self._create_networks()
         await self._load_payloads()
 
@@ -192,22 +253,28 @@
     def dapp_state(self) -> Dict[str, Dict[int, ServiceState]]:
         """Return the state of the dapp.
 
         State of the dapp is a dictionary containing the state of all the
         Clusters and their Service instances comprising the dapp.
         """
 
-        return {
+        cluster_states = {
             cluster_id: {
                 instance_index: instance.state
                 for instance_index, instance in enumerate(cluster.instances)
             }
             for cluster_id, cluster in self.clusters.items()
         }
 
+        missing_nodes = set(self.dapp.nodes) - set(cluster_states)
+
+        cluster_states.update({node_id: {} for node_id in missing_nodes})
+
+        return cluster_states
+
     @property
     def dapp_started(self) -> bool:
         """Return True if the dapp has been started, False otherwise.
 
         Dapp is considered started if all instances in all commissioned service
         clusters have been started and remain running.
         """
@@ -230,52 +297,87 @@
         return all(
             [
                 self._is_cluster_state(cluster_id, ServiceState.terminated)
                 for cluster_id in self.clusters.keys()
             ]
         )
 
-    async def _listen_state_queue(self, service: DappService):
+    def _update_node_gaom(self, service: DappService, service_descriptor: ServiceDescriptor):
+        # update the state in the GAOM
+        service_descriptor.state = service.state.identifier
+
+        # update the network node if possible
+        if service.network_node and not service_descriptor.network_node:
+            service_descriptor.network_node = NetworkNodeDescriptor.from_network_node(
+                service.network_node
+            )
+
+        # update the activity if possible
+        if service._ctx:  # noqa
+            ctx = service._ctx  # noqa
+            if not service_descriptor.activity:
+                service_descriptor.activity = ActivityDescriptor.from_activity(
+                    ctx._activity
+                )  # noqa
+
+            if not service_descriptor.agreement:
+                service_descriptor.agreement = AgreementDescriptor(
+                    id=ctx._agreement.id,  # noqa
+                    provider_id=ctx.provider_id,
+                    provider_name=ctx.provider_name,
+                )
+
+        # reset the GAOM state on "pending"
+        if service_descriptor.state == "pending":
+            service_descriptor.network_node = None
+            service_descriptor.activity = None
+            service_descriptor.agreement = None
+
+    async def _listen_state_queue(
+        self, service: DappService, service_descriptor: ServiceDescriptor
+    ):
         """On a state change of the instance, update the Runner's state stream."""
         while True:
             await service.state_queue.get()
 
             # on a state change, we're publishing the state of the whole dapp
             self._report_status_change()
+            self._update_node_gaom(service, service_descriptor)
 
     def _report_status_change(self) -> None:
         """Emit message with full state update to state queue."""
 
         nodes_states = self.dapp_state
 
         self.state_queue.put_nowait(
             {
                 "nodes": nodes_states,
-                "app": self._get_app_state_from_nodes(),
+                "app": self._get_app_state_from_nodes(nodes_states),
                 "timestamp": utcnow_iso_str(),
             }
         )
 
-    def _get_app_state_from_nodes(self) -> ServiceState:
+    def _get_app_state_from_nodes(
+        self, dapp_state: Optional[Dict[str, Dict[int, ServiceState]]] = None
+    ) -> ServiceState:
         """Return general application state based on all instances states."""
         # Collect nested node states into simple unique collection of state values
 
-        dapp_state = self.dapp_state
+        dapp_state = dapp_state or self.dapp_state
 
         all_states = set(state for node in dapp_state.values() for state in node.values())
 
-        # If we want dapp to be running handle other states as starting
+        # If we want dapp to be running -> handle other states as starting
         if self._desired_app_state == ServiceState.running:
             # Check node-to-state parity because of node dependency,
             #  states gradually rolls out
 
             if ({self._desired_app_state} == all_states) and (
                 len(dapp_state) == len(self.dapp.nodes)
             ):
-
                 return ServiceState.running
 
             return ServiceState.starting
 
         # If we want dapp to be terminated handle other states as stopping
         if self._desired_app_state == ServiceState.terminated:
             if {self._desired_app_state} == all_states:
@@ -336,15 +438,15 @@
                         "Command for a nonexistent instance (`%s` not in `%s`)",
                         idx,
                         cluster_name,
                     )
                     continue
 
                 logger.debug("Creating runtime command: %s", cmd_def)
-                cmd = CommandDescriptor.load(cmd_def)
+                cmd = CommandDescriptor(**cmd_def)
                 service.command_queue.put_nowait(cmd)
 
     def _is_cluster_state(self, cluster_id: str, state: ServiceState) -> bool:
         """Return True if the state of all instances in the cluster is `state`."""
         return all(s.state == state for s in self.clusters[cluster_id].instances)
 
     async def stop(self):
```

### Comparing `dapp_runner-0.1.2/dapp_runner/runner/service.py` & `dapp_runner-0.2.0/dapp_runner/runner/service.py`

 * *Files identical despite different names*

### Comparing `dapp_runner-0.1.2/dapp_runner/runner/streams.py` & `dapp_runner-0.2.0/dapp_runner/runner/streams.py`

 * *Files identical despite different names*

### Comparing `dapp_runner-0.1.2/pyproject.toml` & `dapp_runner-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapp-runner"
-version = "0.1.2"
+version = "0.2.0"
 description = "Golem dapp-runner - a high-level interface for running decentralized applications using the Golem Network."
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
@@ -33,15 +33,19 @@
 appdirs = "^1.4"
 click = "^7.0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
 dpath = "~2.0.8"
 pyyaml = "^5.0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
 shortuuid = "^1.0"
 ansicolors = "^1.1.8"
 networkx = "^2.8"
-yapapi = "^0.10.1"
+yapapi = "0.11.0"
+pydantic = "^1.10.5"
+fastapi = "^0.93.0"
+uvicorn = {extras = ["standard"], version = "^0.21.0"}
+pyopenssl = "^23.1.1"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "*"  # implicitly required by liccehck
 pip = "*"  # implicitly required by liccehck
 
 autoflake = "^1"
 black = "^21.0b0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
@@ -54,42 +58,42 @@
 pytest-asyncio = "^0.18.3"
 pytest-cov = "^3.0.0"
 liccheck = "^0.7.2"
 pytest-mock = "^3.10.0"
 factory-boy = "^3.2.1"
 isort = "^5.11.4"
 
-[tool.poetry.group.tests_integration]
-optional = true
-
-[tool.poetry.group.tests_integration.dependencies]
-goth = "^0.14.0"
-requests = "^2.28.2"
-
 [tool.poetry.scripts]
 dapp-runner = "dapp_runner.__main__:_cli"
 
 [tool.poe.tasks]
 checks = {sequence = ["checks_codestyle", "checks_typing", "checks_license"], help = "Run all available code checks"}
 checks_codestyle = {sequence = ["_checks_codestyle_flake8", "_checks_codestyle_isort", "_checks_codestyle_black"], help = "Run only code style checks"}
 _checks_codestyle_flake8 = "flake8 dapp_runner tests"
 _checks_codestyle_isort = "isort --check-only --diff ."
 _checks_codestyle_black = "black --check --diff ."
 checks_typing  = {cmd = "mypy --install-types --non-interactive --ignore-missing-imports --check-untyped-defs --warn-unused-ignores --show-error-codes .", help = "Run only code typing checks" }
 checks_license = {sequence = ["_checks_license_export", "_checks_license_verify"], help = "Run only license compatibility checks"}
 _checks_license_export = "poetry export -f requirements.txt -o .requirements.txt"
 _checks_license_verify = "liccheck -r .requirements.txt"
+
 format = {sequence = ["_format_autoflake", "_format_isort", "_format_black"], help = "Run code auto formatting"}
 _format_autoflake = "autoflake ."
 _format_isort = "isort ."
 _format_black = "black ."
+
 tests = {sequence = ["tests_unit"], help = "Run all available tests"}
 tests_unit = {cmd = "pytest --cov --cov-report html --cov-report term -sv tests/unit", help = "Run only unit tests"}
-tests_integration_assets = "python -m goth create-assets tests/goth_tests/assets"
-tests_integration = "pytest -svx tests/goth_tests --disable-pytest-warnings --config-override docker-compose.build-environment.use-prerelease=true --config-path tests/goth_tests/assets/goth-config-testing.yml"
+
+tests_integration_init = ["_tests_integration_env", "_tests_integration_requirements", "_tests_integration_assets"]
+_tests_integration_env = "python -m venv .envs/goth"
+_tests_integration_requirements = ".envs/goth/bin/pip install --extra-index-url https://test.pypi.org/simple/ goth==0.14.1 pytest pytest-asyncio pexpect"
+_tests_integration_assets = ".envs/goth/bin/python -m goth create-assets tests/goth_tests/assets"
+tests_integration = ".envs/goth/bin/python -m pytest -svx tests/goth_tests --disable-pytest-warnings --config-override docker-compose.build-environment.use-prerelease=true --config-path tests/goth_tests/assets/goth-config-testing.yml"
+
 
 [tool.liccheck]
 authorized_licenses = [
   "bsd",
   "new bsd",
   "bsd license",
   "apache 2",
```

### Comparing `dapp_runner-0.1.2/PKG-INFO` & `dapp_runner-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapp-runner
-Version: 0.1.2
+Version: 0.2.0
 Summary: Golem dapp-runner - a high-level interface for running decentralized applications using the Golem Network.
 Home-page: https://github.com/golemfactory/dapp-runner
 License: LGPL-3.0
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,18 +19,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: ansicolors (>=1.1.8,<2.0.0)
 Requires-Dist: appdirs (>=1.4,<2.0)
 Requires-Dist: click (>=7.0,<8.0)
 Requires-Dist: dpath (>=2.0.8,<2.1.0)
+Requires-Dist: fastapi (>=0.93.0,<0.94.0)
 Requires-Dist: networkx (>=2.8,<3.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pyopenssl (>=23.1.1,<24.0.0)
 Requires-Dist: pyyaml (>=5.0,<6.0)
 Requires-Dist: shortuuid (>=1.0,<2.0)
-Requires-Dist: yapapi (>=0.10.1,<0.11.0)
+Requires-Dist: uvicorn[standard] (>=0.21.0,<0.22.0)
+Requires-Dist: yapapi (==0.11.0)
 Project-URL: Repository, https://github.com/golemfactory/dapp-runner
 Description-Content-Type: text/markdown
 
 # Golem dApp Runner
 
 `dapp-runner` is a utility that allows you to run decentralized applications on [Golem](https://www.golem.network/).
 It uses simple application descriptors expressed in `yaml`, similar to those used by
```

