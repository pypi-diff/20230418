# Comparing `tmp/address_name_system-0.2.2.tar.gz` & `tmp/address_name_system-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "address_name_system-0.2.2.tar", last modified: Tue Apr  4 14:55:56 2023, max compression
+gzip compressed data, was "address_name_system-0.2.3.tar", last modified: Tue Apr 18 20:50:19 2023, max compression
```

## Comparing `address_name_system-0.2.2.tar` & `address_name_system-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:55:56.165842 address_name_system-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-04 14:55:47.000000 address_name_system-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-04 14:55:56.165842 address_name_system-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-04 14:55:47.000000 address_name_system-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:55:56.165842 address_name_system-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-04 14:55:47.000000 address_name_system-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:55:56.161842 address_name_system-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:55:56.165842 address_name_system-0.2.2/src/address_name_system/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 14:55:47.000000 address_name_system-0.2.2/src/address_name_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-04 14:55:47.000000 address_name_system-0.2.2/src/address_name_system/address_name_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:55:56.165842 address_name_system-0.2.2/src/address_name_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-04 14:55:56.000000 address_name_system-0.2.2/src/address_name_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-04 14:55:56.000000 address_name_system-0.2.2/src/address_name_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:55:56.000000 address_name_system-0.2.2/src/address_name_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-04 14:55:56.000000 address_name_system-0.2.2/src/address_name_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:55:56.000000 address_name_system-0.2.2/src/address_name_system.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 14:55:56.000000 address_name_system-0.2.2/src/address_name_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 14:55:56.000000 address_name_system-0.2.2/src/address_name_system.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:50:19.137426 address_name_system-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-18 20:50:08.000000 address_name_system-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-18 20:50:19.137426 address_name_system-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-18 20:50:08.000000 address_name_system-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:50:19.137426 address_name_system-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 20:50:08.000000 address_name_system-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:50:19.133426 address_name_system-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:50:19.133426 address_name_system-0.2.3/src/address_name_system/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 20:50:08.000000 address_name_system-0.2.3/src/address_name_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-18 20:50:08.000000 address_name_system-0.2.3/src/address_name_system/address_name_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:50:19.133426 address_name_system-0.2.3/src/address_name_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-18 20:50:18.000000 address_name_system-0.2.3/src/address_name_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-18 20:50:19.000000 address_name_system-0.2.3/src/address_name_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:50:18.000000 address_name_system-0.2.3/src/address_name_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 20:50:18.000000 address_name_system-0.2.3/src/address_name_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:50:18.000000 address_name_system-0.2.3/src/address_name_system.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 20:50:18.000000 address_name_system-0.2.3/src/address_name_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 20:50:18.000000 address_name_system-0.2.3/src/address_name_system.egg-info/top_level.txt
```

### Comparing `address_name_system-0.2.2/LICENSE` & `address_name_system-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `address_name_system-0.2.2/PKG-INFO` & `address_name_system-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: address_name_system
-Version: 0.2.2
+Version: 0.2.3
 Summary: Mapping Addresses to Dynamic IPs, Simplified
 Home-page: https://github.com/Naruno/Address-Name-System
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # Address Name System (ANS) for Naruno
         ANS is a decentralized system that maps blockchain addresses to dynamic IPs, making it easy to access servers with changing IP addresses. With ANS, you can access your server by using your unique blockchain address instead of constantly searching for its changing IP address.
```

### Comparing `address_name_system-0.2.2/README.md` & `address_name_system-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `address_name_system-0.2.2/setup.py` & `address_name_system-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='address_name_system',
-version='0.2.2',
+version='0.2.3',
 description="""Mapping Addresses to Dynamic IPs, Simplified""",
 long_description_content_type="text/markdown",
 include_package_data=True,
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 url='https://github.com/Naruno/Address-Name-System',
 author="Naruno Developers",
 author_email='onur.atakan.ulusoy@naruno.org',
@@ -16,8 +16,8 @@
 install_requires=[
     "fire==0.5.0"
 ],
 entry_points = {
     'console_scripts': ['ans=address_name_system.address_name_system:main'],
 },
 python_requires=">= 3",
-zip_safe=False)
+zip_safe=False)
```

### Comparing `address_name_system-0.2.2/src/address_name_system/address_name_system.py` & `address_name_system-0.2.3/src/address_name_system/address_name_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,21 +99,23 @@
     def set_encrypt_key(self, encrypt_key):
         self.encrypt_key = encrypt_key
     
     def add_user(self, user):
         self.trusted_users.append(user)
 
     def run(self):
+        if self.encrypt_key == None:
+            raise Exception("Encryption Key not provided")
         while True:
             data = self.integration.get()
             if data != []:
                 for each in data:
                     if each["fromUser"] in self.trusted_users:
                         self.integration.send("myip", self.self_ip, each["fromUser"])
             time.sleep(5)
 
     def close(self):
         self.integration.close()
 
 def main():
     ans.command_line = True
-    fire.Fire(ans)
+    fire.Fire(ans)
```

### Comparing `address_name_system-0.2.2/src/address_name_system.egg-info/PKG-INFO` & `address_name_system-0.2.3/src/address_name_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: address-name-system
-Version: 0.2.2
+Version: 0.2.3
 Summary: Mapping Addresses to Dynamic IPs, Simplified
 Home-page: https://github.com/Naruno/Address-Name-System
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # Address Name System (ANS) for Naruno
         ANS is a decentralized system that maps blockchain addresses to dynamic IPs, making it easy to access servers with changing IP addresses. With ANS, you can access your server by using your unique blockchain address instead of constantly searching for its changing IP address.
```

