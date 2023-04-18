# Comparing `tmp/NamasteiG-0.2.4.tar.gz` & `tmp/NamasteiG-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NamasteiG-0.2.4.tar", last modified: Sat Apr 15 13:30:36 2023, max compression
+gzip compressed data, was "NamasteiG-0.2.5.tar", last modified: Tue Apr 18 03:00:11 2023, max compression
```

## Comparing `NamasteiG-0.2.4.tar` & `NamasteiG-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.050384 NamasteiG-0.2.4/
--rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      838 2023-04-15 13:30:36.050384 NamasteiG-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.4/README.md
--rw-rw-rw-   0        0        0      593 2023-04-15 13:26:28.000000 NamasteiG-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 13:30:36.050384 NamasteiG-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.034396 NamasteiG-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.041264 NamasteiG-0.2.4/src/NamasteiG/
--rw-rw-rw-   0        0        0    19992 2023-04-15 13:26:10.000000 NamasteiG-0.2.4/src/NamasteiG/__init__.py
--rw-rw-rw-   0        0        0      499 2022-12-14 18:59:48.000000 NamasteiG-0.2.4/src/NamasteiG/example.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.041264 NamasteiG-0.2.4/src/NamasteiG.egg-info/
--rw-rw-rw-   0        0        0      838 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/
+-rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      838 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.5/README.md
+-rw-rw-rw-   0        0        0      593 2023-04-18 02:58:50.000000 NamasteiG-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.372567 NamasteiG-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.372567 NamasteiG-0.2.5/src/NamasteiG/
+-rw-rw-rw-   0        0        0    19940 2023-04-18 02:58:38.000000 NamasteiG-0.2.5/src/NamasteiG/__init__.py
+-rw-rw-rw-   0        0        0      499 2022-12-14 18:59:48.000000 NamasteiG-0.2.5/src/NamasteiG/example.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/src/NamasteiG.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/top_level.txt
```

### Comparing `NamasteiG-0.2.4/LICENSE` & `NamasteiG-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.4/PKG-INFO` & `NamasteiG-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.4
+Version: 0.2.5
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NamasteiG-0.2.4/pyproject.toml` & `NamasteiG-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NamasteiG"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Abhinav Bhardwaj", email="abhinav.bhardwaj.56614@gmail.com" },
 ]
 description = "Most PowerFull Instagram Library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NamasteiG-0.2.4/src/NamasteiG/__init__.py` & `NamasteiG-0.2.5/src/NamasteiG/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import uuid
 import string
 import requests
-import sys
 import random
 import secrets
 import time
 from urllib.parse   import urlencode
 import base64
 from Cryptodome.Cipher import AES, PKCS1_v1_5
 from Cryptodome.PublicKey import RSA
@@ -48,16 +47,16 @@
         self.user = User
         self.passw=Password
         self.PigeonSession = f'UFS-{str(uuid.uuid4())}-0'
         self.IgDeviceId = uuid.uuid4()
         self.IgFamilyDeviceId = uuid.uuid4()
         self.AndroidID = f'android-{secrets.token_hex(8)}'
         rnd=str(random.randint(150, 999))
-        self.UserAgent = "Instagram 276.1.0.26.103 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"][random.randint(0, 11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 460846236)"
-        self.Blockversion = '0620e51c315c4db6af09d9ba44f8802cb1253abbf7902647f6e1e0e327c8d93f'
+        self.UserAgent = "Instagram 278.0.0.21.117 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"][random.randint(0, 11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 464315254)"
+        self.Blockversion = '329007815be126bc02ffebcd41f0e4f8d889d871c12ca57fe5cbc3ece5196505'
 
     def generate_jazoest(self,symbols):
         amount = sum(ord(s) for s in symbols)
         return f'2{amount}'
 
     def GetMid(self):
         data = urlencode({
@@ -205,29 +204,31 @@
                 'Xclaim': self.xclaim,
                 'BearerToken': self.sessionid,
                 'igid':self.igid,
             }
 
         else:
             print(response.text)
-            sys.exit()
 
-            # value = {
-            #     "Response": self.response,
-            #     "Mid": self.mid,
-            #     'PigeonSession': self.PigeonSession,
-            #     "IgDeviceId": self.IgDeviceId,
-            #     "IgFamilyDeviceId": self.IgFamilyDeviceId,
-            #     "AndroidID": self.AndroidID,
-            #     'UserAgent': self.UserAgent,
-            #     'BlockVersion': self.Blockversion
-            # }
+
+            value = {
+                "Response": self.response,
+                "Mid": self.mid,
+                'PigeonSession': self.PigeonSession,
+                "IgDeviceId": self.IgDeviceId,
+                "IgFamilyDeviceId": self.IgFamilyDeviceId,
+                "AndroidID": self.AndroidID,
+                'UserAgent': self.UserAgent,
+                'BlockVersion': self.Blockversion
+            }
 
         return value
     def head(self):
+
+
         headers = {
             'Host': 'i.instagram.com',
             'X-Ig-App-Locale': 'en_US',
             'X-Ig-Device-Locale': 'en_US',
             'X-Ig-Mapped-Locale': 'en_US',
             'X-Pigeon-Session-Id': str(self.PigeonSession),
             'X-Pigeon-Rawclienttime': str(round(time.time(), 3)),
@@ -413,15 +414,15 @@
             )
             return response.text
 
         except Exception as E:
             print(E)
 
 
-
+#
 # if __name__ == '__main__':
 #     ig=Instagram('','')
-#     ig.Login()
-#     print(ig.Follow_UserID('4567890'))
+#     ig.Login(1)
+#     print(ig.Scrape_Followers(''))
```

### Comparing `NamasteiG-0.2.4/src/NamasteiG.egg-info/PKG-INFO` & `NamasteiG-0.2.5/src/NamasteiG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.4
+Version: 0.2.5
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

