# Comparing `tmp/algokit_utils-1.0.2b7-py3-none-any.whl.zip` & `tmp/algokit_utils-1.0.3b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 30665 bytes, number of entries: 14
+Zip file size: 30653 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     3476 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     3513 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7508 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    65563 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    65541 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7424 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    19350 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1931 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx      934 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     3824 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.2b7.dist-info/LICENSE
--rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.2b7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.2b7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1174 b- defN 16-Jan-01 00:00 algokit_utils-1.0.2b7.dist-info/RECORD
-14 files, 117734 bytes uncompressed, 28711 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1174 b- defN 16-Jan-01 00:00 algokit_utils-1.0.3b1.dist-info/RECORD
+14 files, 117712 bytes uncompressed, 28699 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.0.2b7.dist-info/LICENSE
+Filename: algokit_utils-1.0.3b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.0.2b7.dist-info/METADATA
+Filename: algokit_utils-1.0.3b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.0.2b7.dist-info/WHEEL
+Filename: algokit_utils-1.0.3b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.0.2b7.dist-info/RECORD
+Filename: algokit_utils-1.0.3b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/application_client.py

```diff
@@ -1457,25 +1457,25 @@
         **app_spec_note.__dict__,
         deleted=False,
     )
     return app_metadata
 
 
 def _convert_call_parameters(args: CommonCallParameters | CommonCallParametersDict | None) -> CreateCallParameters:
-    _args = dataclasses.asdict(args) if isinstance(args, CommonCallParameters) else (args or {})
+    _args = args.__dict__ if isinstance(args, CommonCallParameters) else (args or {})
     return CreateCallParameters(**_args)
 
 
 def _convert_deploy_args(
     _args: ABICallArgs | ABICallArgsDict | None,
     note: au_deploy.AppDeployMetaData,
     signer: TransactionSigner | None,
     sender: str | None,
 ) -> tuple[ABIMethod | bool | None, ABIArgsDict, CreateCallParameters]:
-    args = dataclasses.asdict(_args) if isinstance(_args, ABICallArgs) else (_args or {})
+    args = _args.__dict__ if isinstance(_args, ABICallArgs) else (_args or {})
 
     # return most derived type, unused parameters are ignored
     parameters = CreateCallParameters(
         note=note.encode(),
         signer=signer,
         sender=sender,
         suggested_params=args.get("suggested_params"),
```

## Comparing `algokit_utils-1.0.2b7.dist-info/LICENSE` & `algokit_utils-1.0.3b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.0.2b7.dist-info/METADATA` & `algokit_utils-1.0.3b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.0.2b7
+Version: 1.0.3b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.0.2b7.dist-info/RECORD` & `algokit_utils-1.0.3b1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_utils/__init__.py,sha256=dpVhBwD1h0gaVNSSbt2RreJanO3h10fPxHuj4opksU8,3476
 algokit_utils/_transfer.py,sha256=9ghNJC3AE5yK0a55RTZu4suI14xeEIt6RlBSihWht-A,3513
 algokit_utils/account.py,sha256=_kkMxUybfQXfmyGD9nNRz5vH1YQy_GaKgrGPxhcdDOQ,7508
-algokit_utils/application_client.py,sha256=ApX6r4AV8Mbgtykj4Ja0Ybdp-wiLQGckrchiOg-21DM,65563
+algokit_utils/application_client.py,sha256=AcxLoKae14bH_dmMxUGR3BsEdAvGts_2aXcS7QDhr4c,65541
 algokit_utils/application_specification.py,sha256=paQh-8AOVL83AcBJQCKF-fRrgMPVI1x1z-105YSX_cg,7424
 algokit_utils/deploy.py,sha256=dfOFs-PkYrpUqSuLKhxf52S5gVKmjj9rWBkPiv2vEE8,19350
 algokit_utils/logic_error.py,sha256=P28a0EsbifwCv-KZ1gke7dNadA4R-FuD1zEjQbb3mDc,1931
 algokit_utils/models.py,sha256=fbLh5DoQQFM0GFktg3jE5qVpgac1EPborBQYr8UzQOk,934
 algokit_utils/network_clients.py,sha256=uB-V7eQerNDG7oJg0EiiPNbzOBYfIjM-40WSna7aPN4,3824
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.0.2b7.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.0.2b7.dist-info/METADATA,sha256=N-U_i93UnaCrXbGG-SRk4lMLZ5nBTKY5796s8ALtJUg,1873
-algokit_utils-1.0.2b7.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.0.2b7.dist-info/RECORD,,
+algokit_utils-1.0.3b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.0.3b1.dist-info/METADATA,sha256=gQ15qKZg54AFb6ZGqMWZpkgHudoZ7MIxTBBNyRswdCk,1873
+algokit_utils-1.0.3b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.0.3b1.dist-info/RECORD,,
```

