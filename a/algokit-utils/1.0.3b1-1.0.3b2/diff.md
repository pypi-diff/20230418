# Comparing `tmp/algokit_utils-1.0.3b1-py3-none-any.whl.zip` & `tmp/algokit_utils-1.0.3b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 30653 bytes, number of entries: 14
+Zip file size: 30666 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     3476 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     3513 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7508 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    65541 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    65567 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7424 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
--rw-r--r--  2.0 unx    19350 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx    19351 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1931 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx      934 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     3824 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1174 b- defN 16-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/RECORD
-14 files, 117712 bytes uncompressed, 28699 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1174 b- defN 16-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/RECORD
+14 files, 117739 bytes uncompressed, 28712 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.0.3b1.dist-info/LICENSE
+Filename: algokit_utils-1.0.3b2.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.0.3b1.dist-info/METADATA
+Filename: algokit_utils-1.0.3b2.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.0.3b1.dist-info/WHEEL
+Filename: algokit_utils-1.0.3b2.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.0.3b1.dist-info/RECORD
+Filename: algokit_utils-1.0.3b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/application_client.py

```diff
@@ -80,15 +80,15 @@
 
     def __init__(self, program: str, client: AlgodClient):
         """
         Fully compile the program source to binary and generate a
         source map for matching pc to line number
         """
         self.teal = program
-        result: dict = client.compile(self.teal, source_map=True)
+        result: dict = client.compile(au_deploy.strip_comments(self.teal), source_map=True)
         self.raw_binary = base64.b64decode(result["result"])
         self.binary_hash: str = result["hash"]
         self.source_map = SourceMap(result["sourcemap"])
 
 
 def num_extra_program_pages(approval: bytes, clear: bytes) -> int:
     """Calculate minimum number of extra_pages required for provided approval and clear programs"""
```

## algokit_utils/deploy.py

```diff
@@ -283,21 +283,21 @@
 ) -> None:
     if allow_update is not None:
         template_values[_UPDATABLE] = int(allow_update)
     if allow_delete is not None:
         template_values[_DELETABLE] = int(allow_delete)
 
 
-def _strip_comments(program: str) -> str:
-    lines = [x.split("//", maxsplit=1)[0] for x in program.splitlines()]
+def strip_comments(program: str) -> str:
+    lines = [line.split("//", maxsplit=1)[0] for line in program.splitlines()]
     return "\n".join(lines)
 
 
 def check_template_variables(approval_program: str, template_values: TemplateValueDict) -> None:
-    approval_program = _strip_comments(approval_program)
+    approval_program = strip_comments(approval_program)
     if UPDATABLE_TEMPLATE_NAME in approval_program and _UPDATABLE not in template_values:
         raise DeploymentFailedError(
             "allow_update must be specified if deploy time configuration of update is being used"
         )
     if DELETABLE_TEMPLATE_NAME in approval_program and _DELETABLE not in template_values:
         raise DeploymentFailedError(
             "allow_delete must be specified if deploy time configuration of delete is being used"
@@ -339,21 +339,21 @@
 
         program_lines, matches = _replace_template_variable(program_lines, template_variable_name, value)
 
     return "\n".join(program_lines)
 
 
 def has_template_vars(app_spec: ApplicationSpecification) -> bool:
-    return "TMPL_" in _strip_comments(app_spec.approval_program) or "TMPL_" in _strip_comments(app_spec.clear_program)
+    return "TMPL_" in strip_comments(app_spec.approval_program) or "TMPL_" in strip_comments(app_spec.clear_program)
 
 
 def get_deploy_control(
     app_spec: ApplicationSpecification, template_var: str, on_complete: transaction.OnComplete
 ) -> bool | None:
-    if template_var not in _strip_comments(app_spec.approval_program):
+    if template_var not in strip_comments(app_spec.approval_program):
         return None
     return get_call_config(app_spec.bare_call_config, on_complete) != CallConfig.NEVER or any(
         h for h in app_spec.hints.values() if get_call_config(h.call_config, on_complete) != CallConfig.NEVER
     )
 
 
 def get_call_config(method_config: MethodConfigDict, on_complete: transaction.OnComplete) -> CallConfig:
```

## Comparing `algokit_utils-1.0.3b1.dist-info/LICENSE` & `algokit_utils-1.0.3b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.0.3b1.dist-info/METADATA` & `algokit_utils-1.0.3b2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.0.3b1
+Version: 1.0.3b2
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.0.3b1.dist-info/RECORD` & `algokit_utils-1.0.3b2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_utils/__init__.py,sha256=dpVhBwD1h0gaVNSSbt2RreJanO3h10fPxHuj4opksU8,3476
 algokit_utils/_transfer.py,sha256=9ghNJC3AE5yK0a55RTZu4suI14xeEIt6RlBSihWht-A,3513
 algokit_utils/account.py,sha256=_kkMxUybfQXfmyGD9nNRz5vH1YQy_GaKgrGPxhcdDOQ,7508
-algokit_utils/application_client.py,sha256=AcxLoKae14bH_dmMxUGR3BsEdAvGts_2aXcS7QDhr4c,65541
+algokit_utils/application_client.py,sha256=jq2izmBWdLIgqFWe_Yl7uFdJs5mEbwjsjC97YKt12NI,65567
 algokit_utils/application_specification.py,sha256=paQh-8AOVL83AcBJQCKF-fRrgMPVI1x1z-105YSX_cg,7424
-algokit_utils/deploy.py,sha256=dfOFs-PkYrpUqSuLKhxf52S5gVKmjj9rWBkPiv2vEE8,19350
+algokit_utils/deploy.py,sha256=kpWb4oLurEM1P0BgRaQ_HXUq3aZOcT5t_5GJapNgzak,19351
 algokit_utils/logic_error.py,sha256=P28a0EsbifwCv-KZ1gke7dNadA4R-FuD1zEjQbb3mDc,1931
 algokit_utils/models.py,sha256=fbLh5DoQQFM0GFktg3jE5qVpgac1EPborBQYr8UzQOk,934
 algokit_utils/network_clients.py,sha256=uB-V7eQerNDG7oJg0EiiPNbzOBYfIjM-40WSna7aPN4,3824
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.0.3b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.0.3b1.dist-info/METADATA,sha256=gQ15qKZg54AFb6ZGqMWZpkgHudoZ7MIxTBBNyRswdCk,1873
-algokit_utils-1.0.3b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.0.3b1.dist-info/RECORD,,
+algokit_utils-1.0.3b2.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.0.3b2.dist-info/METADATA,sha256=hLBL3tFB55Dfvaa909K4_p883Yq8BfDJSRxsQKyr3lU,1873
+algokit_utils-1.0.3b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.0.3b2.dist-info/RECORD,,
```

