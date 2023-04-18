# Comparing `tmp/sui_brownie-0.31.0-py3-none-any.whl.zip` & `tmp/sui_brownie-0.31.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27329 bytes, number of entries: 16
+Zip file size: 27336 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-01 10:43 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    86164 b- defN 23-Apr-11 09:37 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    86180 b- defN 23-Apr-18 07:14 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-11 02:45 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/RECORD
-16 files, 151972 bytes uncompressed, 25187 bytes compressed:  83.4%
+-rw-r--r--  2.0 unx      983 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/RECORD
+16 files, 151988 bytes uncompressed, 25194 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-0.31.0.dist-info/METADATA
+Filename: sui_brownie-0.31.1.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-0.31.0.dist-info/WHEEL
+Filename: sui_brownie-0.31.1.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-0.31.0.dist-info/top_level.txt
+Filename: sui_brownie-0.31.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-0.31.0.dist-info/RECORD
+Filename: sui_brownie-0.31.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -1893,15 +1893,15 @@
             self.account.account_address,
             package_id,
             abi["module_name"],
             abi["func_name"],
             type_arguments,
             arguments,
             gas_object,
-            gas_budget,
+            str(gas_budget),
             None
         )
         return result
 
     def simulate(
             self,
             package_id,
@@ -1937,15 +1937,15 @@
             package_id,
             abi,
             type_arguments,
             arguments,
             gas_price=gas_price,
             gas_budget=gas_budget
         )
-        tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
+        tx_bytes = base64.b64encode(msg.value.value.kind.encode).decode("ascii")
         return self.client.sui_devInspectTransactionBlock(
             self.account.account_address,
             tx_bytes,
             None,
             None
         )
```

## Comparing `sui_brownie-0.31.0.dist-info/METADATA` & `sui_brownie-0.31.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 0.31.0
+Version: 0.31.1
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `sui_brownie-0.31.0.dist-info/RECORD` & `sui_brownie-0.31.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=iHrr4e51D6pRPxvu5GcClo1bo5ia0QeP99KDU7bcEh8,86164
+sui_brownie/sui_brownie.py,sha256=W7QyQeSfhtIGpG6PJxyIVBBJq1RPGp4VfscqhAS4oTk,86180
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-0.31.0.dist-info/METADATA,sha256=fOdHX9q7z3rJt0g1XT78D03ZJbOA4Nxd7rWnFqwdHRk,983
-sui_brownie-0.31.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-0.31.0.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-0.31.0.dist-info/RECORD,,
+sui_brownie-0.31.1.dist-info/METADATA,sha256=Wkgs6mfdT7fzhH8qktX72BJUbgZ-q1yWkIlT4y0i8zw,983
+sui_brownie-0.31.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-0.31.1.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-0.31.1.dist-info/RECORD,,
```

