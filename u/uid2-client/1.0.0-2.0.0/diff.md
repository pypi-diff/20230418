# Comparing `tmp/uid2_client-1.0.0.tar.gz` & `tmp/uid2_client-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uid2_client-1.0.0.tar", last modified: Thu Mar  9 17:47:35 2023, max compression
+gzip compressed data, was "uid2_client-2.0.0.tar", last modified: Tue Apr 18 15:18:52 2023, max compression
```

## Comparing `uid2_client-1.0.0.tar` & `uid2_client-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:47:35.443013 uid2_client-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-03-09 17:47:25.000000 uid2_client-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-09 17:47:35.443013 uid2_client-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-09 17:47:25.000000 uid2_client-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-09 17:47:25.000000 uid2_client-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-09 17:47:35.443013 uid2_client-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 17:47:25.000000 uid2_client-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:47:35.439013 uid2_client-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-03-09 17:47:25.000000 uid2_client-1.0.0/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-09 17:47:25.000000 uid2_client-1.0.0/tests/test_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:47:35.443013 uid2_client-1.0.0/uid2_client/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/advertising_token_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/auto_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/identity_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/identity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-09 17:47:25.000000 uid2_client-1.0.0/uid2_client/uid2_base64_url_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:47:35.443013 uid2_client-1.0.0/uid2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-09 17:47:35.000000 uid2_client-1.0.0/uid2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-09 17:47:35.000000 uid2_client-1.0.0/uid2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 17:47:35.000000 uid2_client-1.0.0/uid2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-09 17:47:35.000000 uid2_client-1.0.0/uid2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 17:47:35.000000 uid2_client-1.0.0/uid2_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 17:47:35.000000 uid2_client-1.0.0/uid2_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-18 15:18:44.000000 uid2_client-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-18 15:18:52.002849 uid2_client-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-18 15:18:44.000000 uid2_client-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 15:18:44.000000 uid2_client-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-18 15:18:52.002849 uid2_client-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 15:18:44.000000 uid2_client-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-04-18 15:18:44.000000 uid2_client-2.0.0/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-18 15:18:44.000000 uid2_client-2.0.0/tests/test_key_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-18 15:18:44.000000 uid2_client-2.0.0/tests/test_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/uid2_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/advertising_token_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/auto_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/identity_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/identity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/uid2_base64_url_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/uid2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/zip-safe
```

### Comparing `uid2_client-1.0.0/LICENSE` & `uid2_client-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uid2_client-1.0.0/PKG-INFO` & `uid2_client-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uid2_client
-Version: 1.0.0
+Version: 2.0.0
 Summary: UID2 sdk for the UID2 and EUID apis
 Home-page: https://iabtechlab.com
 Author: UID2 team
 Author-email: Cody Constine <cody.constine@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
```

### Comparing `uid2_client-1.0.0/README.md` & `uid2_client-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `uid2_client-1.0.0/pyproject.toml` & `uid2_client-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,25 @@
     "setuptools >= 40.9.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uid2_client"
-version = "1.0.0"
+version = "2.0.0"
 authors = [
     { name = "Cody Constine", email = "cody.constine@thetradedesk.com" }
 ]
 description = "UID2 sdk for the UID2 and EUID apis"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pycrypto"
+    "pycryptodome"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/IABTechLab/uid2-client-python"
 "Bug Tracker" = "https://github.com/IABTechLab/uid2-client-python/issues"
```

### Comparing `uid2_client-1.0.0/setup.cfg` & `uid2_client-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `uid2_client-1.0.0/tests/test_encryption.py` & `uid2_client-2.0.0/tests/test_encryption.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import base64
 import datetime as dt
 from datetime import timezone
 import unittest
 
 from tests.uid2_token_generator import UID2TokenGenerator, Params
-from uid2_client import decrypt_token, encrypt_data, decrypt_data, encryption_block_size, EncryptionError, Uid2Base64UrlCoder, AdvertisingTokenVersion
+from uid2_client import *
 from uid2_client.identity_scope import IdentityScope
 from uid2_client.identity_type import IdentityType
 from uid2_client.keys import *
 
 _master_secret = bytes([139, 37, 241, 173, 18, 92, 36, 232, 165, 168, 23, 18, 38, 195, 123, 92, 160, 136, 185, 40, 91, 173, 165, 221, 168, 16, 169, 164, 38, 139, 8, 155])
 _site_secret =   bytes([32, 251, 7, 194, 132, 154, 250, 86, 202, 116, 104, 29, 131, 192, 139, 215, 48, 164, 11, 65, 226, 110, 167, 14, 108, 51, 254, 125, 65, 24, 23, 133])
 _master_key_id = 164
 _site_key_id = 165
 _test_site_key_id = 166
 _site_id = 9000
 _site_id2 = 2
 
 _example_id = 'ywsvDNINiZOVSsfkHpLpSJzXzhr6Jx9Z/4Q0+lsEUvM='
 _now = dt.datetime.now(tz=timezone.utc)
-_master_key = EncryptionKey(_master_key_id, -1, _now - dt.timedelta(days=-1), _now, _now + dt.timedelta(days=1), _master_secret)
+_master_key = EncryptionKey(_master_key_id, -1, _now - dt.timedelta(days=-1), _now, _now + dt.timedelta(days=1), _master_secret, keyset_id=9999)
 _site_key = EncryptionKey(_site_key_id, _site_id, _now - dt.timedelta(days=-1), _now, _now + dt.timedelta(days=1), _site_secret)
+_keyset_key = EncryptionKey(_site_key_id, _site_id, _now - dt.timedelta(days=-1), _now, _now + dt.timedelta(days=1), _site_secret, keyset_id=20)
 _test_site_key = EncryptionKey(_test_site_key_id, _site_id, dt.datetime(2020, 1, 1, tzinfo=timezone.utc), dt.datetime(2020, 1, 1, tzinfo=timezone.utc), _now + dt.timedelta(days=1), encryption_block_size * b'9')
 
 class TestEncryptionFunctions(unittest.TestCase):
 
     def test_cross_platform_consistency_check_base64_url_test_cases(self):
         case1 = bytes([ 0xff, 0xE0, 0x88, 0xFF, 0xEE, 0x99, 0x99])
         # the Base64 equivalent is "/+CI/+6ZmQ=="
@@ -79,256 +80,282 @@
         # verify that the dynamically created ad token can be decrypted
         runtime_advertising_token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, master_key, _site_id, site_key, params)
         # best effort check as the token might simply just not require padding
         self.assertEqual(-1, runtime_advertising_token.find('='))
         self.assertEqual(-1, runtime_advertising_token.find('+'))
         self.assertEqual(-1, runtime_advertising_token.find('/'))
 
-        result = decrypt_token(runtime_advertising_token, EncryptionKeysCollection([_master_key, _site_key]))
+        result = decrypt(runtime_advertising_token, EncryptionKeysCollection([_master_key, _site_key]))
         self.assertEqual(_example_id, result.uid2)
 
         # can also decrypt a known token generated from other SDK
-        result = decrypt_token(crossPlatformAdvertisingToken, EncryptionKeysCollection([_master_key, _site_key]))
+        result = decrypt(crossPlatformAdvertisingToken, EncryptionKeysCollection([_master_key, _site_key]))
         self.assertEqual(_example_id, result.uid2)
 
     def test_decrypt_token_v4(self):
         token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
-        result = decrypt_token(token, keys)
+        result = decrypt(token, keys)
 
         self.assertEqual(_example_id, result.uid2)
 
 
     def test_decrypt_token_v4_empty_keys(self):
         token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_no_master_key(self):
         token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_no_site_key(self):
         token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
     def test_decrypt_token_v4_invalid_version(self):
         params = Params(dt.timedelta(hours=1))
         token = UID2TokenGenerator.generate_uid2_token_with_debug_info(_example_id, _master_key, _site_id, _site_key, params, 1)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_expired(self):
         params = Params(dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_custom_now(self):
         expiry = dt.datetime(2021, 3, 22, 9, 1, 2, tzinfo=timezone.utc)
         params = Params(expiry)
         token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys, now=expiry+dt.timedelta(seconds=1))
+            result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
-        result = decrypt_token(token, keys, now=expiry-dt.timedelta(seconds=1))
+        result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
         self.assertEqual(_example_id, result.uid2)
 
 
     def test_decrypt_token_v4_invalid_payload(self):
         params = Params(dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token[:-3], keys)
+            result = decrypt(token[:-3], keys)
 
 
     def test_decrypt_token_v3(self):
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
-        result = decrypt_token(token, keys)
+        result = decrypt(token, keys)
 
         self.assertEqual(_example_id, result.uid2)
 
 
     def test_decrypt_token_v3_empty_keys(self):
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v3_no_master_key(self):
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v3_no_site_key(self):
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
     def test_decrypt_token_v3_invalid_version(self):
         params = Params(dt.timedelta(hours=1))
         token = UID2TokenGenerator.generate_uid2_token_with_debug_info(_example_id, _master_key, _site_id, _site_key, params, 1)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v3_expired(self):
         params = Params(dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v3_custom_now(self):
         expiry = dt.datetime(2021, 3, 22, 9, 1, 2, tzinfo=timezone.utc)
         params = Params(expiry)
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys, now=expiry+dt.timedelta(seconds=1))
+            result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
-        result = decrypt_token(token, keys, now=expiry-dt.timedelta(seconds=1))
+        result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
         self.assertEqual(_example_id, result.uid2)
 
 
     def test_decrypt_token_v3_invalid_payload(self):
         params = Params(dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token[:-3], keys)
+            result = decrypt(token[:-3], keys)
 
 
     def test_decrypt_token_v2(self):
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
-        result = decrypt_token(token, keys)
+        result = decrypt(token, keys)
 
         self.assertEqual(_example_id, result.uid2)
 
 
     def test_decrypt_token_v2_empty_keys(self):
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v2_no_master_key(self):
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v2_no_site_key(self):
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v2_invalid_version(self):
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key, version=1)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v2_expired(self):
         params = Params(dt.datetime.now(tz=timezone.utc) + dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys)
+            result = decrypt(token, keys)
 
 
     def test_decrypt_token_v2_custom_now(self):
         expiry = dt.datetime(2021, 3, 22, 9, 1, 2, tzinfo=timezone.utc)
         params = Params(expiry)
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token, keys, now=expiry+dt.timedelta(seconds=1))
+            result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
-        result = decrypt_token(token, keys, now=expiry-dt.timedelta(seconds=1))
+        result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
         self.assertEqual(_example_id, result.uid2)
 
 
+    def test_smoke_token_v3(self):
+        uid2 = _example_id
+        identity_scope = IdentityScope.UID2
+        now = dt.datetime.now(tz=timezone.utc)
+
+        keys = EncryptionKeysCollection([_master_key, _site_key, _keyset_key], default_keyset_id=20,
+                                        master_keyset_id=9999, caller_site_id=20)
+
+        result = encrypt(uid2, identity_scope, keys, now=now, ad_token_version=AdvertisingTokenVersion.ADVERTISING_TOKEN_V3)
+        final = decrypt(result, keys, now=now)
+
+        self.assertEqual(uid2, final.uid2)
+
+    def test_smoke_token_v4(self):
+        uid2 = _example_id
+        identity_scope = IdentityScope.UID2
+        now = dt.datetime.now(tz=timezone.utc)
+
+        keys = EncryptionKeysCollection([_master_key, _site_key, _keyset_key], default_keyset_id=20,
+                                        master_keyset_id=9999, caller_site_id=20)
+
+        result = encrypt(uid2, identity_scope, keys, now=now)
+        final = decrypt(result, keys, now=now)
+
+        self.assertEqual(uid2, final.uid2)
+
     def test_decrypt_token_v2_invalid_payload(self):
         params = Params(dt.datetime.now(tz=timezone.utc) + dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
-            result = decrypt_token(token[:-3], keys)
+            result = decrypt(token[:-3], keys)
 
 
     def test_encrypt_data_specific_key_and_iv(self):
         data = b'123456'
         iv = 12 * b'0'
         key = _test_site_key
         keys = EncryptionKeysCollection([key])
@@ -582,15 +609,15 @@
                                                       IdentityType.Email.value) #v3 test@example.com
         self.verify_identity_type("EKCoNGWPYng/whjBIwANJHKvvGlGyzARtDIAk95FlJyb",
                                                       IdentityType.Email.value) #v3 EUID test@example.com
 
     def verify_identity_type(self, raw_uid, expected_identity_type):
         token = UID2TokenGenerator.generate_uid2_token_v4(raw_uid, _master_key, _site_id, _site_key)
         keys = EncryptionKeysCollection([_master_key, _site_key])
-        result = decrypt_token(token, keys)
+        result = decrypt(token, keys)
         self.assertEqual(raw_uid, result.uid2)
         self.assertEqual(expected_identity_type, get_token_identity_type(token))
 
 
 def get_token_identity_type(id):
     firstChar = id[0]
     if 'A' == firstChar or 'E' == firstChar: #from UID2-79+Token+ and +ID+format+v3
```

### Comparing `uid2_client-1.0.0/tests/test_keys.py` & `uid2_client-2.0.0/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-1.0.0/uid2_client/auto_refresh.py` & `uid2_client-2.0.0/uid2_client/auto_refresh.py`

 * *Files identical despite different names*

### Comparing `uid2_client-1.0.0/uid2_client/client.py` & `uid2_client-2.0.0/uid2_client/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Internal module for holding the Uid2Client class.
 
 Do not use this module directly, import through uid2_client module instead, e.g.
 
 >>> from uid2_client import Uid2Client
 """
 
-
 import base64
 import datetime as dt
 from datetime import timezone
 import json
 import os
 import urllib.request as request
+import pkg_resources
 
 from .keys import EncryptionKey, EncryptionKeysCollection
 from .encryption import _decrypt_gcm, _encrypt_gcm
 
 
 def _make_dt(timestamp):
     return dt.datetime.fromtimestamp(timestamp, tz=timezone.utc)
@@ -31,15 +31,15 @@
         refresh_keys: get the latest encryption keys for decrypting advertising tokens
 
     Examples:
         Connect to the UID2 service and obtain the latest encryption keys:
         >>> from uid2_client import *
         >>> client = Uid2Client('https://prod.uidapi.com', 'my-authorization-key', 'my-secret-key')
         >>> keys = client.refresh_keys()
-        >>> uid2 = decrypt_token('some-ad-token', keys).uid2
+        >>> uid2 = decrypt('some-ad-token', keys).uid2
     """
 
     def __init__(self, base_url, auth_key, secret_key):
         """Create a new Uid2Client client.
 
         Args:
             base_url (str): base URL for all requests to UID2 services (e.g. 'https://prod.uidapi.com')
@@ -49,59 +49,74 @@
         Note:
             Your authorization key will determine which UID2 services you are allowed to use.
         """
         self._base_url = base_url
         self._auth_key = auth_key
         self._secret_key = base64.b64decode(secret_key)
 
-
     def refresh_keys(self):
         """Get the latest encryption keys for advertising tokens.
 
         This will synchronously connect to the corresponding UID2 service and fetch the latest
         set of encryption keys which can then be used to decrypt advertising tokens using
         the decrypt_token function.
 
         Returns:
             EncryptionKeysCollection containing the keys
         """
         req, nonce = self._make_v2_request(dt.datetime.now(tz=timezone.utc))
-        print(req)
-        resp = self._post('/v2/key/latest', headers=self._auth_headers(), data=req)
-        keys = [EncryptionKey(k['id'], k.get('site_id', -1), _make_dt(k['created']), _make_dt(k['activates']), _make_dt(k['expires']), base64.b64decode(k['secret']))
-            for k in json.loads(self._parse_v2_response(resp.read(), nonce)).get('body')]
-        return EncryptionKeysCollection(keys)
-
+        resp = self._post('/v2/key/sharing', headers=self._auth_headers(), data=req)
+        resp_body = json.loads(self._parse_v2_response(resp.read(), nonce)).get('body')
+        return self._parse_keys_json(resp_body)
+
+    def refresh_json(self, json_str):
+        body = json.loads(json_str)
+        return self._parse_keys_json(body['body'])
+
+
+    def _parse_keys_json(self, resp_body):
+        keys = []
+        for key in resp_body["keys"]:
+            keyset_id = None
+            if "keyset_id" in key:
+                keyset_id = key["keyset_id"]
+            key = EncryptionKey(key['id'],
+                                key.get('site_id', -1),
+                                _make_dt(key['created']),
+                                _make_dt(key['activates']),
+                                _make_dt(key['expires']),
+                                base64.b64decode(key['secret']),
+                                keyset_id)
+            keys.append(key)
+        return EncryptionKeysCollection(keys, resp_body["caller_site_id"], resp_body["master_keyset_id"],
+                                        resp_body.get("default_keyset_id", None), resp_body["token_expiry_seconds"])
 
     def _make_url(self, path):
         return self._base_url + path
 
-
     def _auth_headers(self):
-        return {'Authorization': 'Bearer ' + self._auth_key}
-
+        return {'Authorization': 'Bearer ' + self._auth_key,
+                "X-UID2-Client-Version": "uid2-client-python-" + pkg_resources.get_distribution("uid2_client").version}
 
     def _make_v2_request(self, now):
         payload = int.to_bytes(int(now.timestamp() * 1000), 8, 'big')
         nonce = os.urandom(8)
         payload += nonce
 
         envelope = int.to_bytes(1, 1, 'big')
         envelope += _encrypt_gcm(payload, None, self._secret_key)
 
         return base64.b64encode(envelope), nonce
 
-
     def _parse_v2_response(self, encrypted, nonce):
         payload = _decrypt_gcm(base64.b64decode(encrypted), self._secret_key)
         if nonce != payload[8:16]:
             raise ValueError("nonce mismatch")
         return payload[16:]
 
-
     def _post(self, path, headers, data):
         req = request.Request(self._make_url(path), headers=headers, method='POST', data=data)
         return request.urlopen(req)
 
 
 class Uid2ClientError(Exception):
     """Raised for problems encountered while interacting with UID2 services."""
```

### Comparing `uid2_client-1.0.0/uid2_client/encryption.py` & `uid2_client-2.0.0/uid2_client/encryption.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Internal module for keeping encryption/decryption logic.
 
 Do not use this module directly, import from uid2_client instead, e.g.
->>> from uid2_client import decrypt_token
+>>> from uid2_client import decrypt
 """
 
 
 import base64
 import datetime as dt
 from datetime import timezone
 import os
 from Crypto.Cipher import AES
 from enum import Enum
 
 from uid2_client.advertising_token_version import AdvertisingTokenVersion
 from uid2_client.uid2_base64_url_coder import Uid2Base64UrlCoder
+from uid2_client.identity_type import IdentityType
+from uid2_client.identity_scope import IdentityScope
 
 encryption_block_size = AES.block_size
 """int: block size for encryption routines
 
 This determines the size of initialization vectors (IV), required data padding, etc.
 """
 
@@ -25,15 +27,15 @@
 class _PayloadType(Enum):
     """Enum for types of payload that can be encoded in opaque strings"""
     ENCRYPTED_DATA = 128
     ENCRYPTED_DATA_V3 = 96
 
 base64_url_special_chars = {"-", "_"}
 
-def decrypt_token(token, keys, now=dt.datetime.now(tz=timezone.utc)):
+def decrypt(token, keys, now=dt.datetime.now(tz=timezone.utc)):
     """Decrypt advertising token to extract UID2 details.
 
     Args:
         token (str): advertising token to decrypt
         keys (EncryptionKeysCollection): collection of keys to decrypt the token
         now (datetime): date/time to use as "now" when doing token expiration check
 
@@ -143,14 +145,97 @@
 
     id_bytes = site_payload[36:]
     id_str = base64.b64encode(id_bytes).decode('ascii')
 
     return DecryptedToken(id_str, established, site_id, site_key.site_id)
 
 
+def _encrypt_token(uid2, identity_scope, master_key, site_key, site_id, now, token_expiry, ad_token_version):
+    site_payload = bytearray(128)
+    # Publisher Data
+    site_payload[0:4] = int.to_bytes(site_id, byteorder='big', length=4)  # Site id
+    site_payload[4:12] = int.to_bytes(0, byteorder='big', length=8)  # Publisher ID
+    site_payload[12:16] = int.to_bytes(0, byteorder='big', length=4)  # Client Key ID
+    # User Identity Data
+    site_payload[16:20] = int.to_bytes(0, byteorder='big', length=4)  # Privacy Bits
+    site_payload[20:28] = int.to_bytes(int((now-dt.timedelta(hours=1)).timestamp())*1000, byteorder='big', length=8)  # Established
+    site_payload[28:36] = int.to_bytes(int(now.timestamp())*1000, byteorder='big', length=8)  # last refresh
+    site_payload[36:] = bytes(base64.b64decode(uid2))
+
+    id_payload = _encrypt_gcm(bytes(site_payload), None, site_key.secret)
+
+    # Operator Identity Data
+    master_payload = bytearray(256)
+    master_payload[:8] = int.to_bytes(int(token_expiry.timestamp())*1000, byteorder='big', length=8)  # Expiry
+    master_payload[8:16] = int.to_bytes(int(now.timestamp()), byteorder='big', length=8)  # Token Created
+    master_payload[16:20] = int.to_bytes(0, byteorder='big', length=4)  # Site ID
+    master_payload[20:21] = int.to_bytes(1, byteorder='big', length=1)  # Operator Type
+    master_payload[21:25] = int.to_bytes(0, byteorder='big', length=4)  # Operator Version
+    master_payload[25:29] = int.to_bytes(0, byteorder='big', length=4)  # Operator Key ID
+    master_payload[29:33] = int.to_bytes(site_key.key_id, byteorder='big', length=4) # Site Key ID
+    master_payload[33:] = bytes(id_payload)
+
+    encrypted_master_payload = _encrypt_gcm(bytes(master_payload), None, master_key.secret)
+
+    root_writer = bytearray(len(encrypted_master_payload)+6)
+    first_char = uid2[0]
+    identity_type = IdentityType.Phone if first_char == 'F' or first_char == 'B' else IdentityType.Email
+    root_writer[0:1] = int.to_bytes((int(identity_scope) << 4 | int(identity_type) << 2), byteorder='big', length=1)
+    root_writer[1:2] = int.to_bytes(ad_token_version, byteorder='big', length=1)
+    root_writer[2:6] = int.to_bytes(master_key.key_id, byteorder='big', length=4)
+    root_writer[6:] = bytes(encrypted_master_payload)
+
+    if ad_token_version == AdvertisingTokenVersion.ADVERTISING_TOKEN_V4:
+        return Uid2Base64UrlCoder.encode(root_writer)
+
+    return base64.b64encode(root_writer)
+
+
+
+def encrypt(uid2, indentity_scope, keys, keyset_id=None, **kwargs):
+    """ Encrypt an uid2 into a sharing token
+
+    Args:
+        uid2: the uid2 to be encrypted
+        indentity_scope (IdentityScope): If the key will be uid2 or euid2
+        keys (EncryptionKeysCollection): collection of keys to choose from for encryption
+        keyset_id (int) : An optional keyset id to use for the encryption. Will use default keyset if left blank
+
+    Keyword Args:
+        now (Datetime): the datettime to use for now. Defaults to utc now
+        ad_token_version (AdvertisingTokenVersion): Defaults to v4
+
+    Returns (str): Sharing Token
+
+    """
+    now = kwargs.get("now")
+    if now is None:
+        now = dt.datetime.now(tz=timezone.utc)
+
+    ad_token_version = kwargs.get("ad_token_version")
+    if ad_token_version is None:
+        ad_token_version = AdvertisingTokenVersion.ADVERTISING_TOKEN_V4
+
+    key = keys.get_default_keyset_key(now) if keyset_id is None else keys.get_by_keyset_key(keyset_id, now)
+    master_key = keys.get_by_keyset_key(keys.get_master_keyset_id(), now)
+
+    token_expiry = now + dt.timedelta(days=30) if keys.get_token_expiry_seconds() is None \
+        else now + dt.timedelta(seconds=keys.get_token_expiry_seconds())
+
+    site_id = keys.get_caller_site_id()
+    if site_id is None:
+        print("No Site ID in keys")
+        return
+
+    if key is None:
+        raise EncryptionError("No Keyset Key Found")
+
+    return _encrypt_token(uid2, indentity_scope, master_key, key, site_id, now, token_expiry, ad_token_version)
+
+
 def encrypt_data(data, identity_scope, **kwargs):
     """Encrypt arbitrary binary data.
 
     The data can be decrypted with decrypt_data() function.
 
     Args:
         data (bytes): data to encrypt
@@ -196,15 +281,15 @@
     if key is None:
         site_id = kwargs.get("site_id")
         site_key_site_id = site_id
         advertising_token = kwargs.get("advertising_token")
         if site_id is not None and advertising_token is not None:
             raise ValueError("only one of site_id and advertising_token can be specified")
         if advertising_token is not None:
-            decrypted_token = decrypt_token(advertising_token, keys, now)
+            decrypted_token = decrypt(advertising_token, keys, now)
             site_id = decrypted_token.site_id
             site_key_site_id = decrypted_token.site_key_site_id
 
         key = keys.get_active_site_key(site_key_site_id, now)
         if key is None:
             raise EncryptionError("not authorized for key for the specified site")
     elif not key.is_active(now):
@@ -303,15 +388,15 @@
 
 def _add_pkcs7_padding(data, block_size):
     pad_len = block_size - (len(data) % block_size)
     return data + bytes([pad_len])*pad_len
 
 
 def _encrypt(data, iv, key):
-    cipher = AES.new(key.secret, AES.MODE_CBC, iv=iv)
+    cipher = AES.new(key.secret, AES.MODE_CBC, IV=iv)
     return cipher.encrypt(_add_pkcs7_padding(data, AES.block_size))
 
 
 def _decrypt(encrypted, iv, key):
     cipher = AES.new(key.secret, AES.MODE_CBC, iv=iv)
     data = cipher.decrypt(encrypted)
     # remove pkcs7 padding
```

### Comparing `uid2_client-1.0.0/uid2_client/uid2_base64_url_coder.py` & `uid2_client-2.0.0/uid2_client/uid2_base64_url_coder.py`

 * *Files identical despite different names*

### Comparing `uid2_client-1.0.0/uid2_client.egg-info/PKG-INFO` & `uid2_client-2.0.0/uid2_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uid2-client
-Version: 1.0.0
+Version: 2.0.0
 Summary: UID2 sdk for the UID2 and EUID apis
 Home-page: https://iabtechlab.com
 Author: UID2 team
 Author-email: Cody Constine <cody.constine@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
```

### Comparing `uid2_client-1.0.0/uid2_client.egg-info/SOURCES.txt` & `uid2_client-2.0.0/uid2_client.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tests/test_encryption.py
+tests/test_key_parse.py
 tests/test_keys.py
 uid2_client/__init__.py
 uid2_client/advertising_token_version.py
 uid2_client/auto_refresh.py
 uid2_client/client.py
 uid2_client/encryption.py
 uid2_client/identity_scope.py
```

