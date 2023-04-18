# Comparing `tmp/secenv-1.1.1.tar.gz` & `tmp/secenv-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secenv-1.1.1.tar", last modified: Thu Apr 13 12:52:20 2023, max compression
+gzip compressed data, was "secenv-1.2.0.tar", last modified: Tue Apr 18 08:40:17 2023, max compression
```

## Comparing `secenv-1.1.1.tar` & `secenv-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:52:20.148365 secenv-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-04-13 12:51:44.000000 secenv-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    50212 2023-04-13 12:52:20.148365 secenv-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8953 2023-04-13 12:51:44.000000 secenv-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1161 2023-04-13 12:51:45.000000 secenv-1.1.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:52:20.144364 secenv-1.1.1/secenv/
--rw-rw-rw-   0 root         (0) root         (0)     8556 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3750 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:52:20.148365 secenv-1.1.1/secenv/contexts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/contexts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/contexts/aws_assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:52:20.148365 secenv-1.1.1/secenv/stores/
--rw-rw-rw-   0 root         (0) root         (0)     4303 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3421 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/aws.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/azure.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/bitwarden.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/env.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/pass.py
--rw-rw-rw-   0 root         (0) root         (0)     2799 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/scaleway.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/stores/vault.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-04-13 12:51:44.000000 secenv-1.1.1/secenv/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:52:20.144364 secenv-1.1.1/secenv.egg-info/
--rw-r--r--   0 root         (0) root         (0)    50212 2023-04-13 12:52:20.000000 secenv-1.1.1/secenv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-13 12:52:20.000000 secenv-1.1.1/secenv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:52:20.000000 secenv-1.1.1/secenv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-13 12:52:20.000000 secenv-1.1.1/secenv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-13 12:52:20.000000 secenv-1.1.1/secenv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 12:52:20.000000 secenv-1.1.1/secenv.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:52:20.148365 secenv-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-13 12:51:44.000000 secenv-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:52:20.148365 secenv-1.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-04-13 12:51:44.000000 secenv-1.1.1/tests/test_config_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-04-13 12:51:44.000000 secenv-1.1.1/tests/test_context_output.py
--rw-rw-rw-   0 root         (0) root         (0)     5754 2023-04-13 12:51:44.000000 secenv-1.1.1/tests/test_fill_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-04-13 12:51:44.000000 secenv-1.1.1/tests/test_gen_context.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-04-13 12:51:44.000000 secenv-1.1.1/tests/test_list_contexts.py
--rw-rw-rw-   0 root         (0) root         (0)    10980 2023-04-13 12:51:44.000000 secenv-1.1.1/tests/test_stores.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-13 12:51:44.000000 secenv-1.1.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:40:17.400108 secenv-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-04-18 08:39:43.000000 secenv-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-04-18 08:40:17.400108 secenv-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8953 2023-04-18 08:39:43.000000 secenv-1.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-04-18 08:39:44.000000 secenv-1.2.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:40:17.396108 secenv-1.2.0/secenv/
+-rw-rw-rw-   0 root         (0) root         (0)    11962 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3750 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:40:17.396108 secenv-1.2.0/secenv/contexts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/contexts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/contexts/aws_assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:40:17.400108 secenv-1.2.0/secenv/stores/
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/aws.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/azure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/bitwarden.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/pass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/scaleway.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/stores/vault.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-04-18 08:39:43.000000 secenv-1.2.0/secenv/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:40:17.396108 secenv-1.2.0/secenv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-04-18 08:40:17.000000 secenv-1.2.0/secenv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-18 08:40:17.000000 secenv-1.2.0/secenv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:40:17.000000 secenv-1.2.0/secenv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-18 08:40:17.000000 secenv-1.2.0/secenv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-18 08:40:17.000000 secenv-1.2.0/secenv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-18 08:40:17.000000 secenv-1.2.0/secenv.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 08:40:17.400108 secenv-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-18 08:39:43.000000 secenv-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:40:17.400108 secenv-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5623 2023-04-18 08:39:43.000000 secenv-1.2.0/tests/test_config_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-04-18 08:39:43.000000 secenv-1.2.0/tests/test_context_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     5754 2023-04-18 08:39:43.000000 secenv-1.2.0/tests/test_fill_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-04-18 08:39:43.000000 secenv-1.2.0/tests/test_gen_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-04-18 08:39:43.000000 secenv-1.2.0/tests/test_list_contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)    10980 2023-04-18 08:39:43.000000 secenv-1.2.0/tests/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-18 08:39:43.000000 secenv-1.2.0/tests/test_utils.py
```

### Comparing `secenv-1.1.1/LICENSE` & `secenv-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/PKG-INFO` & `secenv-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.1.1
+Version: 1.2.0
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.1.1/README.md` & `secenv-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/pyproject.toml` & `secenv-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "secenv"
-version = "1.1.1"
+version = "1.2.0"
 description = "An utility tool to list, read and fill secrets from multiple stores."
 readme = "README.md"
 authors = [{ name = "Keltio Labs", email = "labs@keltio.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `secenv-1.1.1/secenv/__init__.py` & `secenv-1.2.0/secenv/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import argparse
 import importlib
 import pathlib
 import sys
-from typing import Dict
+from typing import Dict, List
 
 import pkg_resources
 import yaml
 
 from . import context
 from .stores import StoreInterface, fill_secret, read_secret
 
@@ -19,20 +19,25 @@
 
 
 def load_config():
     """
     Load the configuration file and converts it from YAML to a Python object.
     """
     global config, no_config_available
-    if pathlib.Path(".secenv.yaml").exists():
-        config = yaml.load(open(".secenv.yaml", "r"), Loader=yaml.Loader)
-    elif pathlib.Path(".secenv.yml").exists():
-        config = yaml.load(open(".secenv.yml", "r"), Loader=yaml.Loader)
-    else:
-        print("Config error: .secenv.yaml not found")
+    try:
+        if pathlib.Path(".secenv.yaml").exists():
+            config = yaml.load(open(".secenv.yaml", "r"), Loader=yaml.Loader)
+        elif pathlib.Path(".secenv.yml").exists():
+            config = yaml.load(open(".secenv.yml", "r"), Loader=yaml.Loader)
+        else:
+            print("Config error: .secenv.yaml not found")
+            return
+
+    except yaml.parser.ParserError as e:
+        print("Config error: config is not a valid YAML file:", e)
         return
 
     if config:
         no_config_available = False
     else:
         print("Config error: file is empty")
 
@@ -53,14 +58,18 @@
     subparsers_group = parser.add_subparsers()
     subparsers = {}
 
     subparsers["version"] = subparsers_group.add_parser(
         "version", help="get secenv version"
     )
 
+    subparsers["validate"] = subparsers_group.add_parser(
+        "validate", help="validate secenv config"
+    )
+
     subparsers["secrets"] = subparsers_group.add_parser(
         "secrets", help="fill secrets in the stores"
     )
 
     subparsers["contexts"] = subparsers_group.add_parser(
         "contexts", help="list available contexts"
     )
@@ -226,14 +235,88 @@
     """
     if "contexts" in config:
         return "\n".join(config["contexts"])
     else:
         return ""
 
 
+def validate_config() -> List[str]:
+    """
+    Validate a configuration file.
+
+    Returns:
+        List[str]: List of found errors
+    """
+
+    load_config()
+
+    logs = []
+
+    if "stores" not in config:
+        config["stores"] = {}
+    for name, obj in config["stores"].items():
+        if "type" in obj and "extends" in obj:
+            logs.append(f"Store '{name}' contains both 'type' and 'extends' keys")
+
+        if "type" not in obj and "extends" not in obj:
+            logs.append(f"Store '{name}' contains neither 'type' nor 'extends' keys")
+
+        if "extends" in obj and obj["extends"] not in config["stores"]:
+            logs.append(
+                f"Store '{name}' extends an inexistent store '{obj['extends']}'"
+            )
+
+    if "secrets" not in config:
+        config["secrets"] = []
+    for idx, obj in enumerate(config["secrets"]):
+        if "store" not in obj:
+            logs.append(f"Secret {idx} doesn't contain the 'store' key")
+        if "secret" not in obj:
+            logs.append(f"Secret {idx} doesn't contain the 'secret' key")
+        if "store" in obj and obj["store"] not in config["stores"]:
+            logs.append(f"Secret {idx} references an inexistent store '{obj['store']}'")
+        if "generate" in obj and "type" not in obj["generate"]:
+            logs.append(f"Secret {idx} generation doesn't have a type")
+
+    if "contexts" not in config:
+        config["contexts"] = {}
+    for name, obj in config["contexts"].items():
+        for extended in obj.get("extends", []):
+            if extended not in config["contexts"]:
+                logs.append(
+                    f"Context '{name}' extends an inexistent context '{extended}'"
+                )
+
+        for var_name, var_obj in obj.get("vars", {}).items():
+            if type(var_obj) is str:
+                continue
+            if "store" not in var_obj:
+                logs.append(
+                    f"Secret '{name}/{var_name}' doesn't contain the 'store' key"
+                )
+            if "store" in var_obj and var_obj["store"] not in config["stores"]:
+                logs.append(
+                    f"Secret '{name}/{var_name}' references an inexistent store '{var_obj['store']}'"
+                )
+            if "secret" not in var_obj:
+                logs.append(
+                    f"Secret '{name}/{var_name}' doesn't contain the 'secret' key"
+                )
+            if "key" in var_obj and type(var_obj["key"]) is not str:
+                logs.append(
+                    f"Secret '{name}/{var_name}' defines 'key' with wrong type '{type(var_obj['key'])}' (expects 'str')"
+                )
+            if "sensitive" in var_obj and type(var_obj["sensitive"]) is not bool:
+                logs.append(
+                    f"Secret '{name}/{var_name}' defines 'sensitive' with wrong type '{type(var_obj['sensitive'])}' (expects 'bool')"
+                )
+
+    return logs
+
+
 def main():
     if len(sys.argv) == 2 and "version" == sys.argv[1]:
         print(f"secenv version {VERSION}")
         sys.exit(0)
 
     load_config()
     stores = {} if no_config_available else find_stores()
@@ -261,14 +344,22 @@
             if "contexts" not in config or context_name not in config["contexts"]:
                 print(f"Config error: context '{context_name}' not found")
                 sys.exit(1)
             ctx = gen_context(context_name, stores)
             print(context.format_output(ctx, args["format"]))
             return
 
+    elif "validate" in sys.argv[1]:
+        errors = validate_config()
+        if not errors:
+            print("Configuration valid!")
+        else:
+            print("\n".join(errors))
+        return
+
     else:
         # retrieving a specific secret
         # TODO: replace sys.argv[1] with something more beautiful
         # like from 'args' directly
         store = stores[sys.argv[1]]
         result = read_secret(store, args)
         print(result)
```

### Comparing `secenv-1.1.1/secenv/context.py` & `secenv-1.2.0/secenv/context.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/contexts/aws_assume_role.py` & `secenv-1.2.0/secenv/contexts/aws_assume_role.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/__init__.py` & `secenv-1.2.0/secenv/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/aws.py` & `secenv-1.2.0/secenv/stores/aws.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/azure.py` & `secenv-1.2.0/secenv/stores/azure.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/bitwarden.py` & `secenv-1.2.0/secenv/stores/bitwarden.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/env.py` & `secenv-1.2.0/secenv/stores/env.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/gcp.py` & `secenv-1.2.0/secenv/stores/gcp.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/pass.py` & `secenv-1.2.0/secenv/stores/pass.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/scaleway.py` & `secenv-1.2.0/secenv/stores/scaleway.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/stores/vault.py` & `secenv-1.2.0/secenv/stores/vault.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv/utils.py` & `secenv-1.2.0/secenv/utils.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/secenv.egg-info/PKG-INFO` & `secenv-1.2.0/secenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.1.1
+Version: 1.2.0
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.1.1/secenv.egg-info/SOURCES.txt` & `secenv-1.2.0/secenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/tests/test_context_output.py` & `secenv-1.2.0/tests/test_context_output.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/tests/test_fill_secrets.py` & `secenv-1.2.0/tests/test_fill_secrets.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/tests/test_gen_context.py` & `secenv-1.2.0/tests/test_gen_context.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/tests/test_stores.py` & `secenv-1.2.0/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `secenv-1.1.1/tests/test_utils.py` & `secenv-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

