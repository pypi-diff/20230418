# Comparing `tmp/nso-oc-2.44.0.tar.gz` & `tmp/nso-oc-2.45.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.44.0.tar", last modified: Fri Apr 14 13:48:34 2023, max compression
+gzip compressed data, was "nso-oc-2.45.0.tar", last modified: Tue Apr 18 19:01:22 2023, max compression
```

## Comparing `nso-oc-2.44.0.tar` & `nso-oc-2.45.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.706246 nso-oc-2.44.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-14 13:48:08.000000 nso-oc-2.44.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 13:48:08.000000 nso-oc-2.44.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 13:48:34.706246 nso-oc-2.44.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 13:48:08.000000 nso-oc-2.44.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.702246 nso-oc-2.44.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 13:48:34.000000 nso-oc-2.44.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.702246 nso-oc-2.44.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.706246 nso-oc-2.44.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    49391 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29451 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:48:34.706246 nso-oc-2.44.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-14 13:48:08.000000 nso-oc-2.44.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 13:48:08.000000 nso-oc-2.44.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 13:48:34.706246 nso-oc-2.44.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 13:48:08.000000 nso-oc-2.44.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:01:22.753960 nso-oc-2.45.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-18 19:00:55.000000 nso-oc-2.45.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 19:00:55.000000 nso-oc-2.45.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-18 19:01:22.753960 nso-oc-2.45.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-18 19:00:55.000000 nso-oc-2.45.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:01:22.749960 nso-oc-2.45.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-18 19:01:22.000000 nso-oc-2.45.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-18 19:01:22.000000 nso-oc-2.45.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:01:22.000000 nso-oc-2.45.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 19:01:22.000000 nso-oc-2.45.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 19:01:22.000000 nso-oc-2.45.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 19:01:22.000000 nso-oc-2.45.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:01:22.749960 nso-oc-2.45.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:01:22.753960 nso-oc-2.45.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29451 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:01:22.753960 nso-oc-2.45.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-18 19:00:55.000000 nso-oc-2.45.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 19:00:55.000000 nso-oc-2.45.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 19:01:22.753960 nso-oc-2.45.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-18 19:00:55.000000 nso-oc-2.45.0/setup.py
```

### Comparing `nso-oc-2.44.0/LICENSE` & `nso-oc-2.45.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/PKG-INFO` & `nso-oc-2.45.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.44.0
+Version: 2.45.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.44.0/README.md` & `nso-oc-2.45.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.45.0/nso_oc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.44.0
+Version: 2.45.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.44.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.45.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/README.md` & `nso-oc-2.45.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/common.py` & `nso-oc-2.45.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/main.py` & `nso-oc-2.45.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/common_xe.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         for prot_index, prot_item in enumerate(redistribute[protocol]):
             proto_config = append_new_to_table_connections(protocol, table_connections, dst_prot)
             if len(redistribute_leftover.get(protocol, [])) > prot_index:
                 prot_item_leftover = redistribute_leftover[protocol][prot_index]
             else:
                 prot_item_leftover = None
 
-            process_protocol(proto_config, prot_item, prot_item_leftover, dst_process_num)
+            process_protocol(proto_config, prot_item, prot_item_leftover, dst_process_num, dst_prot)
 
             if prot_item_leftover and len(prot_item_leftover) == 0:
                 redistribute_leftover[protocol][prot_index] = None
         
         for leftover_prot in redistribute_leftover.get(protocol, []):
             if leftover_prot:
                 updated_prot_list.append(leftover_prot)
@@ -94,15 +94,15 @@
             redistribute_leftover[protocol] = updated_prot_list
         else:
             if redistribute_leftover != {}:
                 del redistribute_leftover[protocol]
     else:
         proto_config = append_new_to_table_connections(protocol, table_connections, dst_prot)
         temp_redistribute_leftover = redistribute_leftover.get(protocol) if redistribute_leftover else None
-        process_protocol(proto_config, redistribute[protocol], temp_redistribute_leftover, dst_process_num)
+        process_protocol(proto_config, redistribute[protocol], temp_redistribute_leftover, dst_process_num, dst_prot)
 
         if (redistribute_leftover and redistribute_leftover[protocol] != None 
             and len(redistribute_leftover[protocol]) == 0):
             del redistribute_leftover[protocol]
 
 def append_new_to_table_connections(protocol, table_connections, dst_prot):
     proto_config = {
@@ -112,15 +112,18 @@
     }
     proto_config_parent = copy.deepcopy(proto_config)
     proto_config_parent["openconfig-network-instance:config"] = proto_config
     table_connections.append(proto_config_parent)
 
     return proto_config
 
-def process_protocol(proto_config, redistribute_protocol, redistribute_protocol_leftover, dst_process_num):
+def process_protocol(proto_config, redistribute_protocol, redistribute_protocol_leftover, dst_process_num, dst_prot):
+    if dst_prot == "OSPF" and not "subnets" in redistribute_protocol:
+        raise ValueError("Required subnets keyword is non-existent.")
+
     process_src_protocol(proto_config, redistribute_protocol, redistribute_protocol_leftover, "id")
     process_src_protocol(proto_config, redistribute_protocol, redistribute_protocol_leftover, "as-no")
     if dst_process_num != None:
         proto_config["openconfig-network-instance-ext:dst-protocol-process-number"] = dst_process_num
     if "route-map" in redistribute_protocol:
         proto_config["openconfig-network-instance:import-policy"] = redistribute_protocol["route-map"]
```

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             {
                 "openconfig-network-instance:name": "default",
                 "openconfig-network-instance:config": {
                     "openconfig-network-instance:name": "default",
                     "openconfig-network-instance:type": "DEFAULT_INSTANCE",
                     "openconfig-network-instance:enabled": "true"
                 },
-                "openconfig-network-instance:mpls": {"openconfig-network-instance:global": {}},
                 "openconfig-network-instance:protocols": {"openconfig-network-instance:protocol": []},
                 "openconfig-network-instance:interfaces": {"openconfig-network-instance:interface": []},
                 "openconfig-network-instance:vlans": {}
             }
         ]
     }
 }
@@ -92,17 +91,14 @@
             del config_leftover["tailf-ned-cisco-ios:vrf"]["definition"]
         if len(config_leftover["tailf-ned-cisco-ios:vrf"]) == 0:
             del config_leftover["tailf-ned-cisco-ios:vrf"]
     interfaces_by_vrf = get_interfaces_by_vrf(config_before)
     route_forwarding_list_by_vrf = get_route_forwarding_list_by_vrf(config_before)
     configure_network_instances(config_before, config_leftover, interfaces_by_vrf, route_forwarding_list_by_vrf)
 
-    if config_before.get("tailf-ned-cisco-ios:mpls", {}):
-        configure_mpls_default_network_instance(config_before, config_leftover)
-
     if type(config_before.get("tailf-ned-cisco-ios:ip", {}).get("multicast-routing", {}).get("distributed", '')) is list:
         configure_pim_network_instance(config_before, config_leftover)
         configure_igmp_network_instance(config_before, config_leftover)
         configure_cgmp_network_instance(config_before, config_leftover)
 
     cleanup_null_ospf_leftovers(config_leftover)
     cleanup_null_static_route_leftovers(config_leftover)
@@ -181,15 +177,16 @@
 
     for net_inst in openconfig_network_instances["openconfig-network-instance:network-instances"][
         "openconfig-network-instance:network-instance"]:
         configure_network_interfaces(net_inst, interfaces_by_vrf)
 
         if len(interfaces_by_vrf.get(net_inst["openconfig-network-instance:name"], [])) > 0:
             vrf_interfaces = interfaces_by_vrf.get(net_inst["openconfig-network-instance:name"])
-            xe_ospfv2.configure_xe_ospf(net_inst, vrf_interfaces, config_before, config_leftover)
+            xe_ospfv2.configure_xe_ospf(net_inst, vrf_interfaces, config_before, config_leftover, 
+                                        network_instances_notes)
         if len(route_forwarding_list_by_vrf.get(net_inst["openconfig-network-instance:name"], [])) > 0:
             vrf_forwarding_list = route_forwarding_list_by_vrf.get(net_inst["openconfig-network-instance:name"])
             xe_static_route.configure_xe_static_routes(net_inst, vrf_forwarding_list, config_leftover,
                                                        network_instances_notes)
         
         xe_ospfv2.configure_xe_ospf_redistribution(net_inst, config_before, config_leftover, router_ospf_by_vrf)
         xe_bgp.configure_xe_bgp(net_inst, config_before, config_leftover, network_instances_notes)
@@ -311,119 +308,14 @@
         index = 0
         for oc_name in openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"]:
             for oc_instance, oc_instance_name in oc_name.items():
                 if oc_instance_name == instance_name:
                     openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][index]["openconfig-network-instance:protocols"]["openconfig-network-instance:protocol"].append(network_instance)
             index += 1
 
-def configure_mpls_default_network_instance(config_before, config_leftover):
-
-    """
-    Translates NSO XE NED to MDD OpenConfig Network Instance for MPLS and interface MPLS configuration (default network instance)
-    """
-
-    ttl_propagate = {
-        "openconfig-network-instance:config": {
-            "openconfig-network-instance:ttl-propagation": None
-        }
-    }
-    signaling_protocols = {
-        "openconfig-network-instance:signaling-protocols": {
-            "openconfig-network-instance:ldp": {
-                "openconfig-network-instance:global": {
-                    "openconfig-network-instance:config": {
-                        "openconfig-network-instance:lsr-id": ""
-                    },
-                    "openconfig-network-instance:graceful-restart": {
-                        "openconfig-network-instance:config": {
-                            "openconfig-network-instance:enabled": False
-                        }
-                    }
-                },
-                "openconfig-network-instance:interface-attributes": {
-                    "openconfig-network-instance:config": {
-                        "openconfig-network-instance:hello-holdtime": None,
-                        "openconfig-network-instance:hello-interval": None
-                    }
-                }
-            }
-        }
-    }
-    mpls_interface_attributes = {
-        "openconfig-network-instance:interface-attributes": {
-            "openconfig-network-instance:interface": []
-        }
-    }
-    mpls_interface = {
-        "openconfig-network-instance:interface-id": "",
-        "openconfig-network-instance:config": {
-            "openconfig-network-instance:mpls-enabled": False,
-            "openconfig-network-instance:interface-id": "",
-            "openconfig-network-instance:mpls-mtu": 1500,
-            "openconfig-network-instance:mpls-bgp-forwarding": False
-        },
-        "openconfig-network-instance:interface-ref": {
-            "openconfig-network-instance:config": {
-                "openconfig-network-instance:interface": "",
-                "openconfig-network-instance:subinterface": ""
-            }
-        }
-    }
-
-    propagate_ttl = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("mpls-ip-conf", {}).get("ip", {}).get("propagate-ttl-conf", {}).get("propagate-ttl", {})
-    if propagate_ttl is True:
-        ttl_propagate["openconfig-network-instance:config"]["openconfig-network-instance:ttl-propagation"] = True
-    elif propagate_ttl is False:
-        ttl_propagate["openconfig-network-instance:config"]["openconfig-network-instance:ttl-propagation"] = False
-    openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][0]["openconfig-network-instance:mpls"]["openconfig-network-instance:global"].update(ttl_propagate)
-    if "mpls-ip-conf" in config_leftover.get("tailf-ned-cisco-ios:mpls", {}):
-        del config_leftover["tailf-ned-cisco-ios:mpls"]["mpls-ip-conf"]
-
-    if config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}):
-        if config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("graceful-restart-enable", {}).get("graceful-restart", ''):
-            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:global"]["openconfig-network-instance:graceful-restart"]["openconfig-network-instance:config"]["openconfig-network-instance:enabled"] = True
-        ldp_rid = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("router-id", {}).get("interface", '')
-        if ldp_rid:
-            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:global"]["openconfig-network-instance:config"]["openconfig-network-instance:lsr-id"] = ldp_rid
-        ldp_disc_holdtime = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("discovery", {}).get("hello", {}).get("holdtime", '')
-        ldp_disc_interval = config_before.get("tailf-ned-cisco-ios:mpls", {}).get("ldp", {}).get("discovery", {}).get("hello", {}).get("interval", '')
-        if ldp_disc_holdtime:
-            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:interface-attributes"]["openconfig-network-instance:config"]["openconfig-network-instance:hello-holdtime"] = ldp_disc_holdtime
-        if ldp_disc_interval:
-            signaling_protocols["openconfig-network-instance:signaling-protocols"]["openconfig-network-instance:ldp"]["openconfig-network-instance:interface-attributes"]["openconfig-network-instance:config"]["openconfig-network-instance:hello-interval"] = ldp_disc_interval
-        openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][0]["openconfig-network-instance:mpls"].update(signaling_protocols)
-        del config_leftover["tailf-ned-cisco-ios:mpls"]["ldp"]
-
-    for interface_type in config_before.get("tailf-ned-cisco-ios:interface", {}):
-        for nso_index, value in enumerate(config_before["tailf-ned-cisco-ios:interface"][interface_type]):
-            tmp_mpls_interface = copy.deepcopy(mpls_interface)
-            if value.get("mpls", {}):
-                int_num = str(value['name']).split(".")[0]
-                subint_num = 0
-                if "." in str(value['name']):
-                    subint_num = value['name'].split(".")[1]
-
-                tmp_mpls_interface["openconfig-network-instance:interface-id"] = int_num
-                tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:interface-id"] = int_num
-                tmp_mpls_interface["openconfig-network-instance:interface-ref"]["openconfig-network-instance:config"]["openconfig-network-instance:interface"] = interface_type + int_num
-                tmp_mpls_interface["openconfig-network-instance:interface-ref"]["openconfig-network-instance:config"]["openconfig-network-instance:subinterface"] = subint_num
-
-                for mpls_key, mpls_value in value.get("mpls", {}).items():
-                    if "ip" in mpls_key:
-                        tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:mpls-enabled"] = True
-                    if "mtu" in mpls_key:
-                        tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:mpls-mtu"] = mpls_value
-                    if "bgp" in mpls_key and "forwarding" in mpls_value:
-                        tmp_mpls_interface["openconfig-network-instance:config"]["openconfig-network-instance:mpls-bgp-forwarding"] = True
-
-                mpls_interface_attributes["openconfig-network-instance:interface-attributes"]["openconfig-network-instance:interface"].append(tmp_mpls_interface)
-                del config_leftover["tailf-ned-cisco-ios:interface"][interface_type][nso_index]["mpls"]
-
-    openconfig_network_instances["openconfig-network-instance:network-instances"]["openconfig-network-instance:network-instance"][0]["openconfig-network-instance:mpls"]["openconfig-network-instance:global"].update(mpls_interface_attributes)
-    del config_leftover["tailf-ned-cisco-ios:mpls"]
 
 def configure_igmp_network_instance(config_before, config_leftover):
     """
     Translates NSO XE NED to MDD OpenConfig Network Instance for IP multicast and interface IGMP configuration
     """
 
     igmp_protocol_by_networkinstance = {}
@@ -648,27 +540,33 @@
 
 
 def cleanup_null_ospf_leftovers(config_leftover):
     ospf_leftover = config_leftover.get("tailf-ned-cisco-ios:router", {}).get("ospf", [])
     updated_ospf_list = []
 
     for ospf_index in range(len(ospf_leftover)):
+        cleanup_network_statements(ospf_leftover[ospf_index])
         cleanup_neighbors(ospf_leftover[ospf_index])
         cleanup_traffic_area(ospf_leftover[ospf_index])
         cleanup_virtual_link(ospf_leftover[ospf_index])
 
         if len(ospf_leftover[ospf_index]) > 0:
             updated_ospf_list.append(ospf_leftover[ospf_index])
 
     if len(updated_ospf_list) > 0:
         config_leftover.get("tailf-ned-cisco-ios:router", {})["ospf"] = updated_ospf_list
     elif "ospf" in config_leftover.get("tailf-ned-cisco-ios:router", {}):
         del config_leftover["tailf-ned-cisco-ios:router"]["ospf"]
 
 
+def cleanup_network_statements(ospf_leftover):
+    if "network" in ospf_leftover:
+        del ospf_leftover["network"]
+
+
 def cleanup_neighbors(ospf_leftover):
     if "neighbor" in ospf_leftover:
         del ospf_leftover["neighbor"]
 
 
 def cleanup_virtual_link(ospf_leftover):
     if len(ospf_leftover.get("area", [])) < 1:
```

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     from xe import common_xe
 
 ospf_network_types = {
     "broadcast": "BROADCAST_NETWORK",
     "point-to-point": "POINT_TO_POINT_NETWORK",
     "non-broadcast": "NON_BROADCAST_NETWORK"
 }
+xe_ospf_notes = []
 
-
-def configure_xe_ospf(net_inst, vrf_interfaces, config_before, config_leftover):
+def configure_xe_ospf(net_inst, vrf_interfaces, config_before, config_leftover, network_instances_notes):
     """
     Translates NSO XE NED to MDD OpenConfig Network Instances
     """
     instance_type = net_inst["openconfig-network-instance:config"]["openconfig-network-instance:type"]
     net_protocols = net_inst["openconfig-network-instance:protocols"]["openconfig-network-instance:protocol"]
     ospf_list = config_before.get("tailf-ned-cisco-ios:router", {}).get("ospf")
 
@@ -31,14 +31,16 @@
         return
 
     for ospf_index, ospf in enumerate(ospf_list):
         if ((instance_type == "L3VRF" and "vrf" in ospf)
                 or (instance_type == "DEFAULT_INSTANCE" and not "vrf" in ospf)):
             process_ospf(net_protocols, vrf_interfaces, config_leftover, ospf_index, ospf)
 
+    network_instances_notes += xe_ospf_notes
+
 
 def configure_xe_ospf_redistribution(net_inst, config_before, config_leftover, router_ospf_by_vrf):
     ospf_before = config_before.get("tailf-ned-cisco-ios:router", {"ospf": []}).get("ospf")
 
     if ospf_before == None or len(ospf_before) == 0:
         return
         
@@ -61,55 +63,93 @@
             del router_ospf_leftover["redistribute"]
         if "vrf" in router_ospf_leftover:
             del router_ospf_leftover["vrf"]
         if len(router_ospf_leftover) == 1 and "id" in router_ospf_leftover:
             del router_ospf_leftover["id"]
 
 
-def get_interfaces_by_area(network_statements, vrf_interfaces):
+def get_interfaces_by_area(ospf_id, network_statements, vrf_interfaces):
     """
     Assigns OSPF enabled interfaces by area, based on OSPF network statements.
     Network statement wildcard masks are treated like ACLs to determine which interface will be attached
     to an OSPF area.
     Source: https://www.cisco.com/c/en/us/td/docs/ios-xml/ios/iproute_ospf/command/iro-cr-book/ospf-i1.html#wp2261032279
 
     TODO: Consider creating network statement sort algorithm
     As there can be multiple network statements, some may be more specific than others and they can point to different
     OSPF areas. The more specific statements should be prioritized over the less specific ones.
     """
     processed_interfaces = set()
     interfaces_by_area = {}
     sorted_network_statements = sorted(network_statements, key=cmp_to_key(sort_by_mask))
+    unmatched_statements = set()
+    matched_statements_with_intf = set()
+    # This is for tracking only, because the same statement can appear again for unmatched statements.
+    matched_statements = set()
+
+    if len(sorted_network_statements) > 0:
+        xe_ospf_notes.append("\n\nNo direct translation for network statements from XE to OC. \
+Below are the leftover network statements.")
+        xe_ospf_notes.append(f"OSPF ID: {ospf_id}")
 
     for net_stmt in sorted_network_statements:
         # Use get method for net_stmt, since it contains input values that we did not generate and cannot guarantee.
         stmt_mask = net_stmt.get("mask", "")
         area_id = net_stmt.get("area", "0")
         merged_statement_ip = binary_merge(net_stmt.get("ip", ""), net_stmt.get("mask", ""))
 
         for vrf_intf in vrf_interfaces:
             full_intf_name = vrf_intf["type"] + vrf_intf["name"]
+            intf_addr = vrf_intf["ip"]["address"]["primary"]["address"]
+            merged_vrf_intf_ip = binary_merge(intf_addr, stmt_mask)
 
-            if (full_intf_name in processed_interfaces):
-                continue
+            if merged_statement_ip == merged_vrf_intf_ip:
+                matched_stmt = {
+                    "interface": full_intf_name,
+                    "interface_ip": intf_addr
+                }
+                matched_stmt.update(net_stmt)
+                matched_statements.add(net_stmt_to_str(net_stmt))
+                matched_statements_with_intf.add(net_stmt_to_str(matched_stmt))
 
-            merged_vrf_intf_ip = binary_merge(vrf_intf["ip"]["address"]["primary"]["address"], stmt_mask)
+                if (full_intf_name in processed_interfaces):
+                    continue
 
-            if merged_statement_ip == merged_vrf_intf_ip:
                 # If there's a match, then this interface is OSPF enabled
                 processed_interfaces.add(full_intf_name)
 
                 if not area_id in interfaces_by_area:
                     interfaces_by_area[area_id] = []
 
                 interfaces_by_area[area_id].append(vrf_intf)
+            else:
+                unmatched_statements.add(net_stmt_to_str(net_stmt))
+
+    if len(unmatched_statements) > 0 or len(matched_statements_with_intf) > 0:
+        unmatched_statements -= matched_statements
+        xe_ospf_notes.append("Matched statements:")
+        for matched_statement in matched_statements_with_intf: xe_ospf_notes.append(matched_statement)
+        xe_ospf_notes.append("Non-matching statements:")
+        for unmatched_statement in unmatched_statements: xe_ospf_notes.append(unmatched_statement)
+        xe_ospf_notes.append("\n")
 
     return interfaces_by_area
 
 
+def net_stmt_to_str(net_stmt):
+    net_stmt_str = ""
+    
+    if "interface" in net_stmt:
+        net_stmt_str += f"\tInterface: {net_stmt['interface']}, Interface IP: {net_stmt['interface_ip']}\n"
+    
+    net_stmt_str += f"\tMask: {net_stmt.get('mask', '')}, IP: {net_stmt.get('ip', '')}, Area: {net_stmt.get('area', '')}"
+
+    return net_stmt_str
+
+
 def sort_by_mask(stmt1, stmt2):
     """
     A comparator to sort by mask, ordered from most specific (mask of 0.0.0.0) to least specific (mask of 255.255.255.255).
     """
     mask1 = stmt1.get("mask", None)
     mask2 = stmt2.get("mask", None)
 
@@ -365,15 +405,15 @@
 
     ospfv2_global["openconfig-network-instance:config"].update(oc_default_info_originate)
 
 
 def check_areas(ospf_leftover, net_protocols, vrf_interfaces, config_leftover, prot_index, ospf):
     intf_config_leftover = config_leftover.get("tailf-ned-cisco-ios:interface", {})
     ospfv2_area = get_ospfv2_area(net_protocols, prot_index)
-    interfaces_by_area = get_interfaces_by_area(ospf.get("network", []), vrf_interfaces)
+    interfaces_by_area = get_interfaces_by_area(ospf.get("id"), ospf.get("network", []), vrf_interfaces)
     area_list = populate_area_list(ospf)
     is_area_0_present = check_for_area_0(area_list)
     for area in area_list:
         leftover_area = list(filter(lambda temp_area: temp_area["id"] == area["id"], ospf_leftover.get("area", [])))
         set_ospfv2_areas(ospfv2_area, area, leftover_area, ospf, ospf_leftover)
 
         if is_area_0_present and int(area["id"]) != 0:
```

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.45.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.45.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.45.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.45.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.45.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.45.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.44.0/setup.py` & `nso-oc-2.45.0/setup.py`

 * *Files identical despite different names*

