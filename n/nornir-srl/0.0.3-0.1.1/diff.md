# Comparing `tmp/nornir_srl-0.0.3.tar.gz` & `tmp/nornir_srl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_srl-0.0.3.tar", max compression
+gzip compressed data, was "nornir_srl-0.1.1.tar", max compression
```

## Comparing `nornir_srl-0.0.3.tar` & `nornir_srl-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    12129 2023-04-25 19:19:50.485815 nornir_srl-0.0.3/README.md
--rw-r--r--   0        0        0       22 2022-11-20 12:27:33.451929 nornir_srl-0.0.3/nornir_srl/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 18:28:42.918760 nornir_srl-0.0.3/nornir_srl/connections/__init__.py
--rw-r--r--   0        0        0     3781 2023-04-25 18:20:26.447734 nornir_srl-0.0.3/nornir_srl/connections/helpers.py
--rw-r--r--   0        0        0    19453 2023-04-25 19:12:50.201512 nornir_srl-0.0.3/nornir_srl/connections/srlinux.py
--rw-r--r--   0        0        0     9599 2023-04-25 18:56:11.575576 nornir_srl-0.0.3/nornir_srl/fsc.py
--rw-r--r--   0        0        0        0 2022-10-30 22:33:33.108689 nornir_srl-0.0.3/nornir_srl/tasks/__init__.py
--rw-r--r--   0        0        0      373 2022-11-25 22:31:43.343296 nornir_srl-0.0.3/nornir_srl/tasks/helpers.py
--rw-r--r--   0        0        0     8844 2023-01-03 20:18:09.232105 nornir_srl-0.0.3/nornir_srl/tasks/srl_config.py
--rw-r--r--   0        0        0      846 2023-04-25 19:22:17.657001 nornir_srl-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    13559 2023-04-25 19:23:33.933824 nornir_srl-0.0.3/setup.py
--rw-r--r--   0        0        0    13139 2023-04-25 19:23:33.934759 nornir_srl-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    12132 2023-04-26 13:29:14.866549 nornir_srl-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2022-11-20 12:27:33.451929 nornir_srl-0.1.1/nornir_srl/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 18:28:42.918760 nornir_srl-0.1.1/nornir_srl/connections/__init__.py
+-rw-r--r--   0        0        0     3854 2023-04-27 15:04:05.839013 nornir_srl-0.1.1/nornir_srl/connections/helpers.py
+-rw-r--r--   0        0        0    22336 2023-04-28 14:58:03.317817 nornir_srl-0.1.1/nornir_srl/connections/srlinux.py
+-rw-r--r--   0        0        0     9593 2023-04-28 15:22:20.913311 nornir_srl-0.1.1/nornir_srl/fsc.py
+-rw-r--r--   0        0        0        0 2022-10-30 22:33:33.108689 nornir_srl-0.1.1/nornir_srl/tasks/__init__.py
+-rw-r--r--   0        0        0      373 2022-11-25 22:31:43.343296 nornir_srl-0.1.1/nornir_srl/tasks/helpers.py
+-rw-r--r--   0        0        0     8844 2023-01-03 20:18:09.232105 nornir_srl-0.1.1/nornir_srl/tasks/srl_config.py
+-rw-r--r--   0        0        0      846 2023-04-28 15:33:39.158264 nornir_srl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13562 2023-04-28 15:33:46.522847 nornir_srl-0.1.1/setup.py
+-rw-r--r--   0        0        0    13142 2023-04-28 15:33:46.523670 nornir_srl-0.1.1/PKG-INFO
```

### Comparing `nornir_srl-0.0.3/README.md` & `nornir_srl-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 python3 -m venv .venv
 source .venv/bin/activate
 ```
 Following command will install the the `nornir_srl` module and all its dependencies, including Nornir core.
 
 ```
 pip install wheel
-pip install nornir_srl
+pip install -U nornir-srl
 ```
 Create the Nornir confguration file, for example:
 
 ```yaml
 # nornir_config.yaml
 inventory:
     #    plugin: SimpleInventory
```

### Comparing `nornir_srl-0.0.3/nornir_srl/connections/helpers.py` & `nornir_srl-0.1.1/nornir_srl/connections/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Tuple, Optional
 import json
 import difflib
-import fnmatch
+import re
 
 def normalize_gnmi_resp(resp: Dict) -> List[Dict[str, Any]]:
     """
     remove gnmi notification and update envelopes from payload
     to make it comparable to intent struct
 
     Args:
@@ -69,21 +69,24 @@
 def filter_fields(d: Dict, *fields: str) -> Dict:
     return  { 
             k:v for k,v in d.items()
                 if k in [ f.replace('_', '-') for f in fields ]
         }
     
 def strip_modules(d: Dict) -> Dict:
+    p = re.compile(r"srl_nokia-[^:]+:")
+
     if isinstance(d, list):
         return [strip_modules(x) for x in d]
     elif isinstance(d, dict):
         return {strip_modules(k): strip_modules(v) for k, v in d.items()}
     elif isinstance(d, str):
         if d.startswith("srl_nokia-") and ":" in d:
-            return d[(d.index(":") + 1):]
+#            return d[(d.index(":") + 1):]
+            return re.sub(p, '', d)
         return d
     else:
         return d
 
 
 #def strip_modules(d: Dict) -> Dict:
 #    stripped = {}
```

### Comparing `nornir_srl-0.0.3/nornir_srl/connections/srlinux.py` & `nornir_srl-0.1.1/nornir_srl/connections/srlinux.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         ]                
         result = {}
         for spec in path_specs:
             resp = self.get(paths = [spec.get("path") ], datatype=spec["datatype"])
             for path in resp[0]:
                 result.update({k:v for k,v in resp[0][path].items() if k in spec["fields"] } )
         if result.get('software-version'):
-                result['software-version'] = result['software-version'].split('-')[0]
+                result['software-version'] = result['software-version'].split('-')[0].lstrip('v')
 
         return {'sys_info': [result] }
 
     def get_sum_subitf(self, interface:Optional[str] = '*' ) -> Dict[str, Any]:
         path_spec = {
                 "path": f"/interface[name={interface}]/subinterface",
                 "jmespath": 'interface[].{Itf:name, subitfs: subinterface[].{Subitf:name,\
@@ -128,60 +128,111 @@
                 "key": "index",
             }
         resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
         res = jmespath.search(path_spec["jmespath"], resp[0])
         return {'subinterface': res }
     
     def get_bgp_rib(self, route_fam:str, route_type:Optional[str] = '2', network_instance:Optional[str] = '*') -> Dict[str, Any]:
+        BGP_RIB_MOD = 'bgp-rib'
+        mod_version = [ m for m in self.capabilities.get("supported_models", []) if BGP_RIB_MOD in m.get("name")][0].get("version") 
+        BGP_EVPN_VERSION_MAP = {
+            1: ("20"),
+        }
+        BGP_IP_VERSION_MAP = {
+            1: ("2021-", "2022-"),
+            2: ("2023-", "20"),
+        }
         ROUTE_FAMILY = {
             "evpn": "evpn",
             "ipv4": "ipv4-unicast",
             "ipv6": "ipv6-unicast",
         }
         ROUTE_TYPE = {
             "1": "ethernet-ad-routes",
             "2": "mac-ip-routes",
             "3": "imet-routes",
             "4": "ethernet-segment-routes",
             "5": "ip-prefix-routes",
         }
+        def augment_routes(d, attribs): # augment routes with attributes
+            if isinstance(d, list):
+                return [augment_routes(x, attribs) for x in d]
+            elif isinstance(d, dict):
+                if "attr-id" in d:
+                    d.update(attribs.get(d["attr-id"], {}))
+                    d['_r_state'] = ('u' if d['used-route'] else '') + ('*' if d['valid-route'] else '') + ('>' if d['best-route'] else '')
+                    if d.get('vni', 0) == 0:
+                        d['vni'] = '-'
+                    return d
+                else:
+                    return {k: augment_routes(v,attribs) for k, v in d.items()}
+            else:
+                return d
+
+        evpn_path_version = [ k for k,v  in sorted(BGP_EVPN_VERSION_MAP.items(), key=lambda item: item[0]) if len ( [ ver for ver in v if mod_version.startswith(ver)]) > 0 ] [0]
+        ip_path_version = [ k for k,v  in sorted(BGP_IP_VERSION_MAP.items(), key=lambda item: item[0]) if len ( [ ver for ver in v if mod_version.startswith(ver)]) > 0 ] [0]
+
         if route_fam not in ROUTE_FAMILY:
             raise ValueError(f"Invalid route family {route_fam}")
         if route_type and route_type not in ROUTE_TYPE:
             raise ValueError(f"Invalid route type {route_type}")
         
         PATH_BGP_PATH_ATTRIBS = f"/network-instance[name={network_instance}]/bgp-rib/attr-sets/attr-set"
-        RIB_EVPN_PATH = (
+        RIB_EVPN_PATH_VERSIONS = {
+            1: { 
+                'RIB_EVPN_PATH':
+                    (
                         f"/network-instance[name={network_instance}]/bgp-rib/"
                         f"{ROUTE_FAMILY[route_fam]}/rib-in-out/rib-in-post/"
                         f"{ROUTE_TYPE[route_type]}"
-                )
-        RIB_EVPN_JMESPATH_COMMON = '"network-instance"[].{ni:name, Rib:"bgp-rib"."' + ROUTE_FAMILY[route_fam] + \
-                            '"."rib-in-out"."rib-in-post"."' + ROUTE_TYPE[route_type] + '"[]'
-        RIB_EVPN_JMESPATH_ATTRS = {
-            "1": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, Tag:"ethernet-tag-id",vni:vni, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-            "2": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "MAC":"mac-address", "IP":"ip-address",vni:vni,"next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-            "3": '.{RD:"route-distinguisher", peer:neighbor, Tag:"ethernet-tag-id", "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-            "4": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-            "5": '.{RD:"route-distinguisher", peer:neighbor, lpref:"local-pref", "IP-Pfx":"ip-prefix",vni:vni, med:med, "next-hop":"next-hop", GW:"gateway-ip",origin:origin, "0_st":"_r_state"}}',
-        }         
-        PATH_SPECS = {
-            "evpn": {
-                "path": RIB_EVPN_PATH,
-                "jmespath": RIB_EVPN_JMESPATH_COMMON + RIB_EVPN_JMESPATH_ATTRS[route_type],
-                "datatype": "state",
+                    ),
+                'RIB_EVPN_JMESPATH_COMMON': '"network-instance"[].{ni:name, Rib:"bgp-rib"."' + ROUTE_FAMILY[route_fam] + \
+                            '"."rib-in-out"."rib-in-post"."' + ROUTE_TYPE[route_type] + '"[]',
+                'RIB_EVPN_JMESPATH_ATTRS': {
+                    "1": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, Tag:"ethernet-tag-id",vni:vni, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
+                    "2": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "MAC":"mac-address", "IP":"ip-address",vni:vni,"next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
+                    "3": '.{RD:"route-distinguisher", peer:neighbor, Tag:"ethernet-tag-id", "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
+                    "4": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
+                    "5": '.{RD:"route-distinguisher", peer:neighbor, lpref:"local-pref", "IP-Pfx":"ip-prefix",vni:vni, med:med, "next-hop":"next-hop", GW:"gateway-ip",origin:origin, "0_st":"_r_state"}}',
+                },       
             },
-            "ipv4": {
-                "path": (
+        }
+        RIB_IP_PATH_VERSIONS = {
+            1: {
+                'RIB_IP_PATH': 
+                    (
                         f"/network-instance[name={network_instance}]/bgp-rib/"
                         f"{ROUTE_FAMILY[route_fam]}/local-rib/routes"
-                ),
-                "jmespath": '"network-instance"[].{ni:name, Rib:"bgp-rib"."' + ROUTE_FAMILY[route_fam] +
+                    ),
+                'RIB_IP_JMESPATH': '"network-instance"[].{ni:name, Rib:"bgp-rib"."' + ROUTE_FAMILY[route_fam] +
                         '"."local-rib"."routes"[]' +
                         '.{neighbor:neighbor, "0_st":"_r_state", "Pfx":prefix, "lpref":"local-pref", med:med, "next-hop":"next-hop","as-path":"as-path".segment[0].member}}',
+
+            },
+            2: {
+                'RIB_IP_PATH':    
+                    (
+                        f"/network-instance[name={network_instance}]/bgp-rib/afi-safi[afi-safi-name={ROUTE_FAMILY[route_fam]}]/"
+                        f"{ROUTE_FAMILY[route_fam]}/local-rib/routes"
+                    ),  
+                'RIB_IP_JMESPATH': '"network-instance"[].{ni:name, Rib:"bgp-rib"."afi-safi"[]."' + ROUTE_FAMILY[route_fam] +
+                        '"."local-rib"."routes"[]' +
+                        '.{neighbor:neighbor, "0_st":"_r_state", "Pfx":prefix, "lpref":"local-pref", med:med, "next-hop":"next-hop","as-path":"as-path".segment[0].member}}',
+            },
+        }
+
+        PATH_SPECS = {
+            "evpn": {
+                "path": RIB_EVPN_PATH_VERSIONS[evpn_path_version]["RIB_EVPN_PATH"],
+                "jmespath": RIB_EVPN_PATH_VERSIONS[evpn_path_version]["RIB_EVPN_JMESPATH_COMMON"] + RIB_EVPN_PATH_VERSIONS[evpn_path_version]['RIB_EVPN_JMESPATH_ATTRS'][route_type],
+                "datatype": "state",
+            },
+            "ipv4": {
+                "path": RIB_IP_PATH_VERSIONS[ip_path_version]['RIB_IP_PATH'],
+                "jmespath": RIB_IP_PATH_VERSIONS[ip_path_version]['RIB_IP_JMESPATH'],
                 "datatype": "state",
             },
             
         }
         attribs = dict()
         resp = self.get(paths = [ PATH_BGP_PATH_ATTRIBS ], datatype="state")
         for ni in resp[0].get("network-instance", []):
@@ -190,58 +241,64 @@
             for path in ni.get("bgp-rib", {}).get("attr-sets", {}).get("attr-set", []):
                 path_copy = copy.deepcopy(path)
                 attribs[ni["name"]].update( { path_copy.pop("index"): path_copy } )
 
         path_spec = PATH_SPECS[route_fam]
         resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
         for ni in resp[0].get("network-instance", []):
-            if route_fam == "evpn":
-                for route in ni.get("bgp-rib",{}).get("evpn", {}).get('rib-in-out', {}).get('rib-in-post', {}).get(ROUTE_TYPE[route_type], []):
-                    route.update(attribs[ni["name"]][route["attr-id"]])
-                    route['_r_state'] = ('u' if route['used-route'] else '') + ('*' if route['valid-route'] else '') + ('>' if route['best-route'] else '')
-                    if route.get('vni', 0) == 0:
-                        route['vni'] = '-'
-            elif route_fam == "ipv4":
-                for route in ni['bgp-rib'][ROUTE_FAMILY[route_fam]]['local-rib']['routes']:
-                    route.update(attribs[ni["name"]][route["attr-id"]])
-                    route['_r_state'] = ('u' if route['used-route'] else '') + ('*' if route['valid-route'] else '') + ('>' if route['best-route'] else '')
-            elif route_fam == "ipv6":
-                pass
+            ni = augment_routes(ni, attribs[ni["name"]])
 
         res = jmespath.search(path_spec["jmespath"], resp[0])
         if res:
             for ni in res:
                 for route in ni.get('Rib', []):
                     route['as-path'] = str(route['as-path']) + ' i' if route.get('as-path') else 'i'
         else:
             res = []
         return {'bgp_rib': res }
 
     def get_sum_bgp(self, network_instance:Optional[str] = '*' ) -> Dict[str, Any]:
+        BGP_MOD = 'urn:srl_nokia/bgp:srl_nokia-bgp'
+        mod_version = [ m for m in self.capabilities.get("supported_models", []) if BGP_MOD == m.get("name")][0].get("version") 
+        BGP_VERSION_MAP = {
+            1: ("2021-", "2022-"),
+            2: ("2023-3", "20")
+        }
+        our_version = [ k for k,v  in sorted(BGP_VERSION_MAP.items(), key=lambda item: item[0]) if len ( [ ver for ver in v if mod_version.startswith(ver)]) > 0 ] [0]
         def augment_resp(resp):
             for ni in resp[0]["network-instance"]:
                 if ni.get('protocols') and ni['protocols'].get('bgp'):
                     for peer in ni['protocols']['bgp']['neighbor']:
-                        if peer.get('evpn'):
-                            peer["_evpn"] = str(peer["evpn"]["received-routes"]) + "/" + \
-                            str(peer["evpn"]["active-routes"]) + "/" + \
-                            str(peer["evpn"]["sent-routes"]) if peer["evpn"]["admin-state"] == "enable" else "disabled"
+                        peer_data = dict()
+                        if our_version == 1:
+                            peer_data['evpn'] = peer.get('evpn')
+                            peer_data['ipv4-unicast'] = peer.get('ipv4-unicast')
+                        elif our_version == 2:
+                            for afi in peer.get('afi-safi', []):
+                                if afi['afi-safi-name'] == 'evpn':
+                                    peer_data['evpn'] = afi
+                                elif afi['afi-safi-name'] == 'ipv4-unicast':
+                                    peer_data['ipv4-unicast'] = afi
+                        if peer_data.get('evpn'):
+                            peer["_evpn"] = str(peer_data["evpn"]["received-routes"]) + "/" + \
+                            str(peer_data["evpn"]["active-routes"]) + "/" + \
+                            str(peer_data["evpn"]["sent-routes"]) if peer_data["evpn"]["admin-state"] == "enable" else "disabled"
                         else:
-                            peer["_evpn"] = "disabled"
-                        if peer.get('ipv4-unicast'):
-                            if peer["ipv4-unicast"]["admin-state"] == "enable":
-                                peer["_ipv4"] = str(peer["ipv4-unicast"]["received-routes"]) + "/" + \
-                                    str(peer["ipv4-unicast"]["active-routes"]) + "/" + \
-                                    str(peer["ipv4-unicast"]["sent-routes"])
-                                if peer["ipv4-unicast"].get("oper-state")== "down":
+                            peer["_evpn"] = "-"
+                        if peer_data.get('ipv4-unicast'):
+                            if peer_data["ipv4-unicast"]["admin-state"] == "enable":
+                                peer["_ipv4"] = str(peer_data["ipv4-unicast"]["received-routes"]) + "/" + \
+                                    str(peer_data["ipv4-unicast"]["active-routes"]) + "/" + \
+                                    str(peer_data["ipv4-unicast"]["sent-routes"])
+                                if peer_data["ipv4-unicast"].get("oper-state")== "down":
                                     peer["_ipv4"] = "down"
                             else:
                                 peer["_ipv4"] = "disabled"
                         else:
-                            peer["_ipv4"] = "disabled"
+                            peer["_ipv4"] = "-"
 
         path_spec = {
                 "path": f"/network-instance[name={network_instance}]/protocols/bgp/neighbor",
                 "jmespath": '"network-instance"[].{NetwInst:name, Neighbors: protocols.bgp.neighbor[].{"1_peer":"peer-address",\
                     peer_as:"peer-as", state:"session-state",local_as:"local-as"[]."as-number",\
                     "group":"peer-group", "export_policy":"export-policy", "import_policy":"import-policy",\
                     "AFI/SAFI\\nIPv4-UC\\nRx/Act/Tx":"_ipv4", "AFI/SAFI\\nEVPN\\nRx/Act/Tx":"_evpn"}}',
@@ -332,15 +389,15 @@
         res = jmespath.search(path_spec["jmespath"], resp[0])
         return {'ipv4_rib': res }    
     
     def get_nwi_itf(self, nw_instance:Optional[str] = '*') -> Dict[str, Any]:
         path_spec = {
                 "path": f"/network-instance[name={nw_instance}]",
                 "jmespath": '"network-instance"[].{name:name,oper:"oper-state",type:type,itfs: interface[].{Subitf:name,\
-                      "if-oper":"oper-state", "if-dwn-reason":"oper-down-reason","mac-learning":"oper-mac-learning"}}',
+                      "if-oper":"oper-state", "if-dwn-reason":"oper-down-reason"}}',
                 "datatype": "state",
             }
         resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
         res = jmespath.search(path_spec["jmespath"], resp[0])
         return {'nwi_itfs': res }
 
     def get(
```

### Comparing `nornir_srl-0.0.3/nornir_srl/fsc.py` & `nornir_srl-0.1.1/nornir_srl/fsc.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,14 @@
         'disable': '[info]',
         'routed': '[cyan]',
         'bridged': '[blue]',
         'established': '[ok]',
         'active': '[cyan]',
     }
 
-    
-
     console = Console(theme=table_theme)
     if kwargs.get("box_type") and kwargs["box_type"] != None:
         box_type = str(kwargs["box_type"]).upper()
         try:
             box_type = getattr(importlib.import_module("rich.box"), box_type)
         except AttributeError:
             print(f"Unknown box type {box_type}. Check 'python -m rich.box' for valid box types.")
```

### Comparing `nornir_srl-0.0.3/nornir_srl/tasks/srl_config.py` & `nornir_srl-0.1.1/nornir_srl/tasks/srl_config.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.0.3/pyproject.toml` & `nornir_srl-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_srl"
-version = "0.0.3"
+version = "0.1.1"
 description = "Nornir connection plugin for SRLinux"
 authors = ["Walter De Smedt <walter.de.smedt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/wdesmedt/nornir_srl"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nornir_srl-0.0.3/setup.py` & `nornir_srl-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 entry_points = \
 {'console_scripts': ['fcli = nornir_srl.fsc:cli'],
  'nornir.plugins.connections': ['srlinux = '
                                 'nornir_srl.connections.srlinux:SrLinux']}
 
 setup_kwargs = {
     'name': 'nornir-srl',
-    'version': '0.0.3',
+    'version': '0.1.1',
     'description': 'Nornir connection plugin for SRLinux',
-    'long_description': '# nornir_srl\nThis module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations.\n\nThe current functionality is focused on a read-only _network-wide CLI_ to perform show commands across an entire set or subset for SRLinux nodes, as defined in the Nornir inventory and through command-line filter options. It shows output in a tabular format for easy reading.\nFollowing versions will focus on configuration management and command execution on the nodes.\n\n# Prerequisites\n\nThis module requires [Nornir Core](https://github.com/nornir-automation/nornir) that includes the Nornir core components for which this module is an add-on.\nNornir needs a [configuration file](https://nornir.readthedocs.io/en/latest/configuration/index.html) to tell it at a minimum where to find the inventory and what inventory plugin is used. Also runner configuration parameters, like #threads/workers for parallel execution are defined here but sane defaults are used.\n\nSince this module is using gNMI as the management inteface, at a minimum, a CA certificate is required that was used to create per-device certs and keys. If you use [Containerlab](https://containerlab.dev/) this root cert is auto-generated for SRLinux nodes and available in the lab subfolder created by the containerlab cli. This file needs to be referenced via the inventory (per-device or per-group). See below for details.\n\n# Installation\n\nCreate a Python virtual-env using your favorite workflow, For example:\n```\nmkdir nornir-srl && cd nornir-srl\npython3 -m venv .venv\nsource .venv/bin/activate\n```\nFollowing command will install the the `nornir_srl` module and all its dependencies, including Nornir core.\n\n```\npip install wheel\npip install nornir_srl\n```\nCreate the Nornir confguration file, for example:\n\n```yaml\n# nornir_config.yaml\ninventory:\n    #    plugin: SimpleInventory\n    plugin: YAMLInventory\n    options:\n        host_file: "./inventory/hosts.yaml"\n        group_file: "./inventory/groups.yaml"\n        defaults_file: "./inventory/defaults.yaml"\nrunner:\n    plugin: threaded\n    options:\n        num_workers: 20\n```\nCreate the inventory files as referenced in the above configuration file, for example:\n```yaml\n## hosts.yaml\nclab-4l2s-l1:\n    hostname: clab-4l2s-l1\n    groups: [srl, fabric, leafs]\nclab-4l2s-l2:\n    hostname: clab-4l2s-l2\n    groups: [srl, fabric, leafs]\nclab-4l2s-s1:\n    hostname: clab-4l2s-s1\n    groups: [srl, fabric, spines]\n```\n\n```yaml\n## groups.yaml\nglobal:\n    data:\n        domain: clab\nsrl:\n    connection_options:\n        srlinux:\n            port: 57400\n            username: admin\n            password: admin\n            extras:\n                path_cert: "./root-ca.pem"\nspines:\n    groups: [ global ]\n    data:\n        role: spine\n        type: ixr-d3\nleafs:\n    groups: [ global ]\n    data:\n        role: leaf\n        type: ixr-d2\n```\nThe root certificate is specified once for all devices in group `srl` via the `connection_options.srlinux.extras.path_cert` parameter.\n\n# Use\n\nCurrently, only the network-wide cli functionality is supported via the `fcli` command\n```\n$ fcli --help\nUsage: fcli [OPTIONS] REPORT\n\nOptions:\n  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]\n  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf\n  -f, --field-filter TEXT    filter fields, e.g. -f state=up -f\n                             admin_state=enable\n  -b, --box-type TEXT        box type of printed table, e.g. -b\n                             minimal_double_head. \'python -m rich.box\' for\n                             options\n  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn\n                             -o route_type=2 for \'bgp-rib report\n  --help                     Show this message and exit.\n  ```\n  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:\n```\n$ fcli test\nReport test not found. Available reports: [\'bgp-peers\', \'subinterface\', \'ipv4-rib\', \'mac-table\', \'sys-info\', \'nwi-itfs\', \'lldp-nbrs\']\n```\n\nThe nornir configuration file (`-c` option) is mandatory for nornir to find the inventory files.\nOptionally, you can specify filters to control the output. There are 2 types of filters:\n\n- inventory filters, specified with the `-i` option, filter on the inventory, e.g. `-i hostname=clab-4l2s-l1`  or `-i role=leaf` based on inventory data\n- field filters, specified with the `-f` option. This filters based on the fields shown in the report and a value substring, e.g. `-f state=esta`. Multiple field filters can be specified by repeated `-f` options\n- report-specific options are options specific to a report, if applicable. Currently, the only report that needs extra arguments is \'bgp-rib\', i.e. `route_fam=evpn|ipv4|ipv6` and `route_type=1|2|3|4|5`. The latter relates to EVPN route-trypes and is optional. Defaults to \'2\' (mac-ip-routes). \n\nExamples:\n```\n$ fcli bgp-peers -i role=spine\n                                        BGP Peers                                         \n                               Inventory:{\'role\': \'spine\'}                                \n               ╷          ╷                 ╷         ╷          ╷         ╷              \n  Node         │ NetwInst │ 1_Peer          │ 2_Group │ local_as │ peer_as │ state        \n ══════════════╪══════════╪═════════════════╪═════════╪══════════╪═════════╪═════════════ \n  clab-4l2s-s1 │ default  │ 192.168.0.1     │ leafs   │ [65100]  │ 65001   │ established  \n               │          │ 192.168.0.3     │ leafs   │ [65100]  │ 65002   │ established  \n               │          │ 192.168.0.5     │ leafs   │ [65100]  │ 65003   │ established  \n               │          │ 192.168.0.7     │ leafs   │ [65100]  │ 65004   │ established  \n               │          │ 192.168.0.225   │ dcgw    │ [65100]  │ 65200   │ active       \n               │          │ 192.168.0.227   │ dcgw    │ [65100]  │ 65201   │ active       \n               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect      \n               │          │ 192.168.255.201 │ overlay │ [100]    │ 100     │ connect      \n ──────────────┼──────────┼─────────────────┼─────────┼──────────┼─────────┼───────────── \n  clab-4l2s-s2 │ default  │ 192.168.0.229   │ dcgw    │ [65100]  │ 65200   │ active       \n               │          │ 192.168.0.231   │ dcgw    │ [65100]  │ 65201   │ active       \n               │          │ 192.168.1.1     │ leafs   │ [65100]  │ 65001   │ established  \n               │          │ 192.168.1.3     │ leafs   │ [65100]  │ 65002   │ established  \n               │          │ 192.168.1.5     │ leafs   │ [65100]  │ 65003   │ established  \n               │          │ 192.168.1.7     │ leafs   │ [65100]  │ 65004   │ established  \n               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect     \n```\n\n```\nfcli bgp-rib -r route_fam=evpn -r route_type=2 -f 0_st=\'u*>\'\n                                                                                      BGP RIB                                                                                      \n                                                                              Fields:{\'0_st\': \'u*>\'}                                                                               \n                                                              Report options:{\'route_fam\': \'evpn\', \'route_type\': \'2\'}                                                              \n               ╷         ╷      ╷                               ╷              ╷                   ╷                   ╷         ╷               ╷        ╷                 ╷      \n  Node         │ ni      │ 0_st │ ESI                           │ IP           │ MAC               │ RD                │ as-path │ next-hop      │ origin │ peer            │ vni  \n ══════════════╪═════════╪══════╪═══════════════════════════════╪══════════════╪═══════════════════╪═══════════════════╪═════════╪═══════════════╪════════╪═════════════════╪═════ \n  clab-4l2s-l1 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 0.0.0.0      │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 10.200.1.10  │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.2   │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n ──────────────┼─────────┼──────┼───────────────────────────────┼──────────────┼───────────────────┼───────────────────┼─────────┼───────────────┼────────┼─────────────────┼───── \n  clab-4l2s-l2 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.1   │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n```\n\n\n  \n',
+    'long_description': '# nornir_srl\nThis module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations.\n\nThe current functionality is focused on a read-only _network-wide CLI_ to perform show commands across an entire set or subset for SRLinux nodes, as defined in the Nornir inventory and through command-line filter options. It shows output in a tabular format for easy reading.\nFollowing versions will focus on configuration management and command execution on the nodes.\n\n# Prerequisites\n\nThis module requires [Nornir Core](https://github.com/nornir-automation/nornir) that includes the Nornir core components for which this module is an add-on.\nNornir needs a [configuration file](https://nornir.readthedocs.io/en/latest/configuration/index.html) to tell it at a minimum where to find the inventory and what inventory plugin is used. Also runner configuration parameters, like #threads/workers for parallel execution are defined here but sane defaults are used.\n\nSince this module is using gNMI as the management inteface, at a minimum, a CA certificate is required that was used to create per-device certs and keys. If you use [Containerlab](https://containerlab.dev/) this root cert is auto-generated for SRLinux nodes and available in the lab subfolder created by the containerlab cli. This file needs to be referenced via the inventory (per-device or per-group). See below for details.\n\n# Installation\n\nCreate a Python virtual-env using your favorite workflow, For example:\n```\nmkdir nornir-srl && cd nornir-srl\npython3 -m venv .venv\nsource .venv/bin/activate\n```\nFollowing command will install the the `nornir_srl` module and all its dependencies, including Nornir core.\n\n```\npip install wheel\npip install -U nornir-srl\n```\nCreate the Nornir confguration file, for example:\n\n```yaml\n# nornir_config.yaml\ninventory:\n    #    plugin: SimpleInventory\n    plugin: YAMLInventory\n    options:\n        host_file: "./inventory/hosts.yaml"\n        group_file: "./inventory/groups.yaml"\n        defaults_file: "./inventory/defaults.yaml"\nrunner:\n    plugin: threaded\n    options:\n        num_workers: 20\n```\nCreate the inventory files as referenced in the above configuration file, for example:\n```yaml\n## hosts.yaml\nclab-4l2s-l1:\n    hostname: clab-4l2s-l1\n    groups: [srl, fabric, leafs]\nclab-4l2s-l2:\n    hostname: clab-4l2s-l2\n    groups: [srl, fabric, leafs]\nclab-4l2s-s1:\n    hostname: clab-4l2s-s1\n    groups: [srl, fabric, spines]\n```\n\n```yaml\n## groups.yaml\nglobal:\n    data:\n        domain: clab\nsrl:\n    connection_options:\n        srlinux:\n            port: 57400\n            username: admin\n            password: admin\n            extras:\n                path_cert: "./root-ca.pem"\nspines:\n    groups: [ global ]\n    data:\n        role: spine\n        type: ixr-d3\nleafs:\n    groups: [ global ]\n    data:\n        role: leaf\n        type: ixr-d2\n```\nThe root certificate is specified once for all devices in group `srl` via the `connection_options.srlinux.extras.path_cert` parameter.\n\n# Use\n\nCurrently, only the network-wide cli functionality is supported via the `fcli` command\n```\n$ fcli --help\nUsage: fcli [OPTIONS] REPORT\n\nOptions:\n  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]\n  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf\n  -f, --field-filter TEXT    filter fields, e.g. -f state=up -f\n                             admin_state=enable\n  -b, --box-type TEXT        box type of printed table, e.g. -b\n                             minimal_double_head. \'python -m rich.box\' for\n                             options\n  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn\n                             -o route_type=2 for \'bgp-rib report\n  --help                     Show this message and exit.\n  ```\n  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:\n```\n$ fcli test\nReport test not found. Available reports: [\'bgp-peers\', \'subinterface\', \'ipv4-rib\', \'mac-table\', \'sys-info\', \'nwi-itfs\', \'lldp-nbrs\']\n```\n\nThe nornir configuration file (`-c` option) is mandatory for nornir to find the inventory files.\nOptionally, you can specify filters to control the output. There are 2 types of filters:\n\n- inventory filters, specified with the `-i` option, filter on the inventory, e.g. `-i hostname=clab-4l2s-l1`  or `-i role=leaf` based on inventory data\n- field filters, specified with the `-f` option. This filters based on the fields shown in the report and a value substring, e.g. `-f state=esta`. Multiple field filters can be specified by repeated `-f` options\n- report-specific options are options specific to a report, if applicable. Currently, the only report that needs extra arguments is \'bgp-rib\', i.e. `route_fam=evpn|ipv4|ipv6` and `route_type=1|2|3|4|5`. The latter relates to EVPN route-trypes and is optional. Defaults to \'2\' (mac-ip-routes). \n\nExamples:\n```\n$ fcli bgp-peers -i role=spine\n                                        BGP Peers                                         \n                               Inventory:{\'role\': \'spine\'}                                \n               ╷          ╷                 ╷         ╷          ╷         ╷              \n  Node         │ NetwInst │ 1_Peer          │ 2_Group │ local_as │ peer_as │ state        \n ══════════════╪══════════╪═════════════════╪═════════╪══════════╪═════════╪═════════════ \n  clab-4l2s-s1 │ default  │ 192.168.0.1     │ leafs   │ [65100]  │ 65001   │ established  \n               │          │ 192.168.0.3     │ leafs   │ [65100]  │ 65002   │ established  \n               │          │ 192.168.0.5     │ leafs   │ [65100]  │ 65003   │ established  \n               │          │ 192.168.0.7     │ leafs   │ [65100]  │ 65004   │ established  \n               │          │ 192.168.0.225   │ dcgw    │ [65100]  │ 65200   │ active       \n               │          │ 192.168.0.227   │ dcgw    │ [65100]  │ 65201   │ active       \n               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect      \n               │          │ 192.168.255.201 │ overlay │ [100]    │ 100     │ connect      \n ──────────────┼──────────┼─────────────────┼─────────┼──────────┼─────────┼───────────── \n  clab-4l2s-s2 │ default  │ 192.168.0.229   │ dcgw    │ [65100]  │ 65200   │ active       \n               │          │ 192.168.0.231   │ dcgw    │ [65100]  │ 65201   │ active       \n               │          │ 192.168.1.1     │ leafs   │ [65100]  │ 65001   │ established  \n               │          │ 192.168.1.3     │ leafs   │ [65100]  │ 65002   │ established  \n               │          │ 192.168.1.5     │ leafs   │ [65100]  │ 65003   │ established  \n               │          │ 192.168.1.7     │ leafs   │ [65100]  │ 65004   │ established  \n               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect     \n```\n\n```\nfcli bgp-rib -r route_fam=evpn -r route_type=2 -f 0_st=\'u*>\'\n                                                                                      BGP RIB                                                                                      \n                                                                              Fields:{\'0_st\': \'u*>\'}                                                                               \n                                                              Report options:{\'route_fam\': \'evpn\', \'route_type\': \'2\'}                                                              \n               ╷         ╷      ╷                               ╷              ╷                   ╷                   ╷         ╷               ╷        ╷                 ╷      \n  Node         │ ni      │ 0_st │ ESI                           │ IP           │ MAC               │ RD                │ as-path │ next-hop      │ origin │ peer            │ vni  \n ══════════════╪═════════╪══════╪═══════════════════════════════╪══════════════╪═══════════════════╪═══════════════════╪═════════╪═══════════════╪════════╪═════════════════╪═════ \n  clab-4l2s-l1 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 0.0.0.0      │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 10.200.1.10  │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.2   │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n ──────────────┼─────────┼──────┼───────────────────────────────┼──────────────┼───────────────────┼───────────────────┼─────────┼───────────────┼────────┼─────────────────┼───── \n  clab-4l2s-l2 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.1   │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n```\n\n\n  \n',
     'author': 'Walter De Smedt',
     'author_email': 'walter.de.smedt@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/wdesmedt/nornir_srl',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `nornir_srl-0.0.3/PKG-INFO` & `nornir_srl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-srl
-Version: 0.0.3
+Version: 0.1.1
 Summary: Nornir connection plugin for SRLinux
 Home-page: https://github.com/wdesmedt/nornir_srl
 Author: Walter De Smedt
 Author-email: walter.de.smedt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -45,15 +45,15 @@
 python3 -m venv .venv
 source .venv/bin/activate
 ```
 Following command will install the the `nornir_srl` module and all its dependencies, including Nornir core.
 
 ```
 pip install wheel
-pip install nornir_srl
+pip install -U nornir-srl
 ```
 Create the Nornir confguration file, for example:
 
 ```yaml
 # nornir_config.yaml
 inventory:
     #    plugin: SimpleInventory
```

