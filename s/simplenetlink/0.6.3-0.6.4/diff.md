# Comparing `tmp/simplenetlink-0.6.3-py3-none-any.whl.zip` & `tmp/simplenetlink-0.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10366 bytes, number of entries: 6
--rw-r--r--  2.0 unx    19657 b- defN 23-Jul-02 22:01 simplenetlink/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-02 22:02 simplenetlink-0.6.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     6444 b- defN 23-Jul-02 22:02 simplenetlink-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 22:02 simplenetlink-0.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-02 22:02 simplenetlink-0.6.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      500 b- defN 23-Jul-02 22:02 simplenetlink-0.6.3.dist-info/RECORD
-6 files, 38064 bytes uncompressed, 9460 bytes compressed:  75.1%
+Zip file size: 10445 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    20405 b- defN 23-Jul-03 07:29 simplenetlink/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-03 07:30 simplenetlink-0.6.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6444 b- defN 23-Jul-03 07:30 simplenetlink-0.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 07:30 simplenetlink-0.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-03 07:30 simplenetlink-0.6.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      500 b- defN 23-Jul-03 07:30 simplenetlink-0.6.4.dist-info/RECORD
+6 files, 38812 bytes uncompressed, 9539 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: simplenetlink/__init__.py
 Comment: 
 
-Filename: simplenetlink-0.6.3.dist-info/LICENSE
+Filename: simplenetlink-0.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: simplenetlink-0.6.3.dist-info/METADATA
+Filename: simplenetlink-0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: simplenetlink-0.6.3.dist-info/WHEEL
+Filename: simplenetlink-0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: simplenetlink-0.6.3.dist-info/top_level.txt
+Filename: simplenetlink-0.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: simplenetlink-0.6.3.dist-info/RECORD
+Filename: simplenetlink-0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplenetlink/__init__.py

```diff
@@ -10,22 +10,21 @@
         self._log = logging.getLogger("SimpleNetlink")
         self._current_namespace = namespace
         self._previous_namespace_instance = None
         self._previous_namespace = None
         self._log.level = logging.DEBUG
         self._supported_virtual_interface_types = ["ipvlan", "tagged"]
 
-
     def reset(self):
         self._current_namespace = None
         self._previous_namespace_instance = None
         self._previous_namespace = None
         if self.ipr:
             self.ipr.close()
-        self.ipr= IPRoute()
+        self.ipr = IPRoute()
 
     def get_interface_index(self, ifname):
         res = self.ipr.link_lookup(ifname=ifname)
         if len(res) == 1:
             return res[0]
         else:
             if len(res) == 0:
@@ -79,17 +78,31 @@
         self._previous_namespace_instance = tmp_i
         self._previous_namespace = tmp
         self._log.debug(f"restored previous namespace {self._current_namespace}")
         return True
 
     def delete_namespace(self, namespace):
         if namespace in self.get_namespaces():
-            ns = NetNS(namespace)
-            ns.close()
-            ns.remove()
+            self.set_current_namespace(namespace)
+            for (
+                interface_name,
+                interface_cfg,
+            ) in self.get_network_interfaces_info().items():
+                for ipv4 in interface_cfg.get("ipv4", []):
+                    self.interface_delete_ipv4(interface_name, ipv4["prefix"])
+                for ipv6 in interface_cfg.get("ipv6", []):
+                    self.interface_delete_ipv4(interface_name, ipv6["prefix"])
+            self.ipr.close()
+            self.ipr.remove()
+            self.restore_previous_namespace()
+
+            # ns = NetNS(namespace)
+
+            # ns.close()
+            # ns.remove()
 
             self._log.debug(f"removed namespace {namespace}")
             if namespace == self._current_namespace:
                 self.set_current_namespace(None)
             time.sleep(
                 0.1
             )  # give kernel some time, this workarounds various 'already existing' problams
@@ -126,15 +139,15 @@
             self._log.debug(
                 f"found interface {interface_name} in namespace {namespace} with index {idx}"
             )
         else:
             self._log.debug(f"cannot find interface {interface_name} in any namespace")
         return (namespace, idx)
 
-    def __create_tagged(self, interface_name,options={}, **kwargs):
+    def __create_tagged(self, interface_name, options={}, **kwargs):
         if kwargs.get("parent_interface"):
             (base_namespace, base_idx) = self.find_interface_in_all_namespaces(
                 kwargs.get("parent_interface")
             )
             self._log.debug(
                 f"found parent_interface {kwargs.get('parent_interface')} in namespace {base_namespace}"
             )
@@ -151,15 +164,15 @@
 
             self.ipr.link(
                 "add",
                 ifname=interface_name,
                 kind="vlan",
                 link=base_idx,
                 vlan_id=int(kwargs.get("vlan_id")),
-                **options
+                **options,
             )
             idx = self.get_interface_index(interface_name)
             namespace = kwargs.get("namespace")
             if namespace:
                 if kwargs.get("namespace") not in self.get_namespaces():
                     self.create_namespace(namespace)
                 self.ipr.link("set", index=idx, net_ns_fd=namespace)
@@ -190,16 +203,15 @@
                 "add",
                 ifname=interface_name,
                 kind="ipvlan",
                 link=base_idx,
                 ipvlan_mode=ipvlan_modes[
                     "l2"
                 ],  # l2 mode so arp can be handled from namespace
-                **options
-                
+                **options,
             )
             idx = self.get_interface_index(interface_name)
             namespace = kwargs.get("namespace")
             if namespace:
                 self.set_current_namespace(namespace)
                 self.set_current_namespace(base_namespace)
                 self.ipr.link("set", index=idx, net_ns_fd=kwargs.get("namespace"))
@@ -211,17 +223,17 @@
             return (namespace, idx)
         else:
             raise ValueError(
                 f"parent_interface not specified for ipvlan interface {interface_name}"
             )
 
     def create_interface(self, interface_name, **kwargs):
-        options={}
+        options = {}
         if kwargs.get("mtu"):
-            options["mtu"]=kwargs.get("mtu")
+            options["mtu"] = kwargs.get("mtu")
 
         f = getattr(self, f"_SimpleNetlink__create_{kwargs.get('type')}")
         if f:
             (namespace, idx) = f(interface_name, options, **kwargs)
             if kwargs.get("link_state", "").lower() == "down":
                 self.ipr.link("set", index=idx, state="down")
             else:
@@ -229,60 +241,56 @@
                     f"enabling interface {interface_name} in namespace {namespace}"
                 )
                 self.ipr.link("set", index=idx, state="up")
             return (namespace, idx)
         else:
             raise ValueError(f"type {kwargs.get('type')} not implemented")
 
-    def _resolve_interface_type_by_index(self,idx):
-        info={}
-        for attr in self.ipr.link("get", index=idx)[0]['attrs']:
+    def _resolve_interface_type_by_index(self, idx):
+        info = {}
+        for attr in self.ipr.link("get", index=idx)[0]["attrs"]:
             if attr[0] == "IFLA_LINKINFO":
                 for inner_attr in attr[1]["attrs"]:
                     if inner_attr[0] == "IFLA_INFO_KIND":
-                        info['type']=inner_attr[1]
-                        if info['type']=="vlan":
-                            info['type']="tagged"
-                    if info['type'] == 'tagged' and inner_attr[0] == "IFLA_INFO_DATA":
-                        for ii in inner_attr[1]['attrs']:
+                        info["type"] = inner_attr[1]
+                        if info["type"] == "vlan":
+                            info["type"] = "tagged"
+                    if info["type"] == "tagged" and inner_attr[0] == "IFLA_INFO_DATA":
+                        for ii in inner_attr[1]["attrs"]:
                             if ii[0] == "IFLA_VLAN_ID":
-                                info['vlan_id']=ii[1]
+                                info["vlan_id"] = ii[1]
                 break
         return info
 
     def get_interface_mtu(self):
-        for attr in self.ipr.link("get", index=idx)[0]['attrs']:
+        for attr in self.ipr.link("get", index=idx)[0]["attrs"]:
             if attr[0] == "IFLA_MTU":
                 return attr[1]
 
     def get_interface_ip(self, interface, **kwargs):
         namespace, idx = self.find_interface_in_all_namespaces(interface)
         self.set_current_namespace(namespace)
-        retval={
-            'ipv4':[],
-            'ipv6':[]
-        }
+        retval = {"ipv4": [], "ipv6": []}
 
         for entry in self.ipr.get_addr(index=idx):
-
-            for attr in entry['attrs']:
+            for attr in entry["attrs"]:
                 if attr[0] == "IFA_ADDRESS":
                     if entry["family"] == 2:
-                        retval['ipv4'].append(f"{attr[1]}/{entry['prefixlen']}")
+                        retval["ipv4"].append(f"{attr[1]}/{entry['prefixlen']}")
                     if entry["family"] == 10:
-                        retval['ipv6'].append(f"{attr[1]}/{entry['prefixlen']}")
+                        retval["ipv6"].append(f"{attr[1]}/{entry['prefixlen']}")
                 break
 
         return retval
 
-    def get_interface_ipv4(self,interface):
-        return self.get_interface_ip(interface)['ipv4']
+    def get_interface_ipv4(self, interface):
+        return self.get_interface_ip(interface)["ipv4"]
 
-    def get_interface_ipv6(self,interface):
-        return self.get_interface_ip(interface)['ipv6']
+    def get_interface_ipv6(self, interface):
+        return self.get_interface_ip(interface)["ipv6"]
 
     def ensure_interface_exists(self, interface, **kwargs):
         self.reset()
         namespace, idx = self.find_interface_in_all_namespaces(interface)
         self.set_current_namespace(namespace)
 
         if idx:
@@ -298,61 +306,61 @@
                     self.set_current_namespace(kwargs.get("namespace"))
                     self.interface_up(interface)
                 else:
                     self.set_current_namespace(namespace)
                     self.ipr.link("set", index=idx, net_ns_pid=1)
                     self.set_current_namespace(None)
                     self.interface_up(interface)
-            
-            interface_info=self._resolve_interface_type_by_index(idx)
-            if kwargs.get('type'):
 
-                if interface_info.get('type') != kwargs.get('type'):
+            interface_info = self._resolve_interface_type_by_index(idx)
+            if kwargs.get("type"):
+                if interface_info.get("type") != kwargs.get("type"):
                     self.delete_interface()
-                    raise ValueError("Cannot change interface type. please delete the interface and recreate with new configuration")
-            
+                    raise ValueError(
+                        "Cannot change interface type. please delete the interface and recreate with new configuration"
+                    )
+
             if kwargs.get("mtu"):
                 self.ipr.link("set", index=idx, mtu=kwargs.get("mtu"))
-            
-            
-            if kwargs.get("link_state") in ["up","down"]:
+
+            if kwargs.get("link_state") in ["up", "down"]:
                 if kwargs.get("link_state") == "up":
                     self.interface_up(interface)
                 else:
                     self.interface_down(interface)
             elif kwargs.get("link_state") == None:
                 pass
             else:
-                raise ValueError(f"{kwargs['link_state']} is not a valid link state. Valid link_state values up,down")
+                raise ValueError(
+                    f"{kwargs['link_state']} is not a valid link state. Valid link_state values up,down"
+                )
 
         else:
             if kwargs.get("type") in self._supported_virtual_interface_types:
                 self._log.debug(
                     f'interface type of {interface} is virtual interface of type {kwargs.get("type")} which does not exist -> creating'
                 )
                 namespace, idx = self.create_interface(interface, **kwargs)
             else:
                 raise ValueError(
                     f"either physical interface just doesn't exist (typo?) or virtual type {kwargs.get('type')} is not supported"
                 )
-        
-        v4_diff_list=self.get_interface_ipv4(interface)
+
+        v4_diff_list = self.get_interface_ipv4(interface)
 
         for ipv4_config_item in kwargs.get("ipv4", []):
             self.interface_add_ipv4(interface, ipv4_config_item)
             if ipv4_config_item in v4_diff_list:
                 v4_diff_list.remove(ipv4_config_item)
         if v4_diff_list:
             self._log.debug(
-                    f'interface {interface} has dangling ipv4 addresses {v4_diff_list}'
-                )
+                f"interface {interface} has dangling ipv4 addresses {v4_diff_list}"
+            )
             for ip in v4_diff_list:
-                self.interface_delete_ipv4(interface,ip)
-        
-
+                self.interface_delete_ipv4(interface, ip)
 
         return (namespace, idx)
 
     def interface_add_ipv4(self, interface_name, prefix):
         idx = self.get_interface_index(interface_name)
         if not idx:
             raise ValueError(
@@ -396,57 +404,53 @@
             else:
                 raise (e)
         self._log.debug(
             f"setting ipv4_address {prefix} on {interface_name} in namespace {self._current_namespace}"
         )
         return True
 
-    def interface_up(self,interface_name):
+    def interface_up(self, interface_name):
         idx = self.get_interface_index(interface_name)
         if not idx:
             raise ValueError(
                 f"interface {interface_name} not found in namespace {self._current_namespace}"
             )
         self.ipr.link("set", index=idx, state="up")
 
-    def interface_down(self,interface_name):
+    def interface_down(self, interface_name):
         idx = self.get_interface_index(interface_name)
         if not idx:
             raise ValueError(
                 f"interface {interface_name} not found in namespace {self._current_namespace}"
             )
         self.ipr.link("set", index=idx, state="down")
 
     def get_routes(self):
-        retval = {
-            'static':{},
-            'dynamic':{},
-            'local':{}
-        }
+        retval = {"static": {}, "dynamic": {}, "local": {}}
         for route in self.ipr.route("show", type=1):
-            if route.get_attr('RTA_GATEWAY'):
-                dest = route.get_attr('RTA_DST')
+            if route.get_attr("RTA_GATEWAY"):
+                dest = route.get_attr("RTA_DST")
                 if dest:
-                    dest=f"{dest}/{route.get('dst_len')}"
+                    dest = f"{dest}/{route.get('dst_len')}"
                 else:
-                    dest='default'
-                if dest not in retval['static']:
-                    retval['static'][dest]=[]
-                retval['static'][dest].append(route.get_attr('RTA_GATEWAY'))
-            elif route.get_attr('RTA_PREFSRC'):
+                    dest = "default"
+                if dest not in retval["static"]:
+                    retval["static"][dest] = []
+                retval["static"][dest].append(route.get_attr("RTA_GATEWAY"))
+            elif route.get_attr("RTA_PREFSRC"):
                 dest = f"{route.get_attr('RTA_DST')}/{route.get('dst_len')}"
-                if dest not in retval['local']:
-                    retval['local'][dest]=[]
-                retval['local'][dest].append(f"{route.get_attr('RTA_PREFSRC')}")
+                if dest not in retval["local"]:
+                    retval["local"][dest] = []
+                retval["local"][dest].append(f"{route.get_attr('RTA_PREFSRC')}")
             else:
-                raise ValueError(f'Never come here, if so something is really wrong. {route}')
+                raise ValueError(
+                    f"Never come here, if so something is really wrong. {route}"
+                )
         return retval
 
-
-
     def add_route(self, prefix, nexthop):
         try:
             self.ipr.route("add", gateway=nexthop, dst=prefix)
             self._log.debug(
                 f"added route {prefix} via {nexthop} in namespace {self._current_namespace}"
             )
         except netlink.exceptions.NetlinkError as e:
@@ -477,23 +481,25 @@
             for addr in self.ipr.get_addr(
                 family=socket.AF_INET, label=link.get_attr("IFLA_IFNAME")
             ):
                 ipv4.append(
                     {
                         "prefix_length": addr["prefixlen"],
                         "address": addr.get_attr("IFA_ADDRESS"),
+                        "prefix": f'{addr.get_attr("IFA_ADDRESS")}/{addr["prefixlen"]}',
                     }
                 )
             for addr in self.ipr.get_addr(
                 family=socket.AF_INET6, label=link.get_attr("IFLA_IFNAME")
             ):
                 ipv6.append(
                     {
                         "prefix_length": addr["prefixlen"],
                         "address": addr.get_attr("IFA_ADDRESS"),
+                        "prefix": f'{addr.get_attr("IFA_ADDRESS")}/{addr["prefixlen"]}',
                     }
                 )
             results[link.get_attr("IFLA_IFNAME")] = {
                 "link_state": link["state"].lower(),
                 "oper_state": link.get_attr("IFLA_OPERSTATE").lower(),
                 "mac_address": link.get_attr("IFLA_ADDRESS", "None").lower(),
                 "mtu": link.get_attr("IFLA_MTU"),
```

## Comparing `simplenetlink-0.6.3.dist-info/LICENSE` & `simplenetlink-0.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simplenetlink-0.6.3.dist-info/METADATA` & `simplenetlink-0.6.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplenetlink
-Version: 0.6.3
+Version: 0.6.4
 Summary: Abstraction layer for for simplified usage of pyroute2
 Home-page: https://github.com/jinjamator/simplenetlink
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

