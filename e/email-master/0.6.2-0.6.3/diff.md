# Comparing `tmp/email-master-0.6.2.tar.gz` & `tmp/email-master-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/email-master/email-master/dist/tmp8x0tbwos/email-master-0.6.2.tar", last modified: Fri Sep 16 17:09:41 2022, max compression
+gzip compressed data, was "/home/runner/work/email-master/email-master/dist/.tmp-_4vdnwfw/email-master-0.6.3.tar", last modified: Tue Apr 18 21:23:39 2023, max compression
```

## Comparing `email-master-0.6.2.tar` & `email-master-0.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 17:09:41.000000 email-master-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-09-16 17:09:21.000000 email-master-0.6.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-16 17:09:41.000000 email-master-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master/
--rw-r--r--   0 runner    (1001) docker     (121)    22462 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master/msg/
--rw-r--r--   0 runner    (1001) docker     (121)     7659 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/msg/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/msg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master/eml/
--rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/eml/message.py
--rw-r--r--   0 runner    (1001) docker     (121)    20883 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/eml/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/eml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/attachments.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)    16918 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master/pgp/
--rw-r--r--   0 runner    (1001) docker     (121)    18084 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/pgp/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8648 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/pgp/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/pgp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14806 2022-09-16 17:09:21.000000 email-master-0.6.2/email_master/rfc3156.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 17:09:21.000000 email-master-0.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-09-16 17:09:41.000000 email-master-0.6.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-09-16 17:09:41.000000 email-master-0.6.2/email_master.egg-info/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:23:39.000000 email-master-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 21:23:39.000000 email-master-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 21:23:24.000000 email-master-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22462 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master/eml/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/eml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/eml/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20883 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/eml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master/msg/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/msg/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master/pgp/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/pgp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/pgp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/pgp/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14806 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/rfc3156.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-18 21:23:24.000000 email-master-0.6.3/email_master/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 21:23:39.000000 email-master-0.6.3/email_master.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:23:39.000000 email-master-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 21:23:24.000000 email-master-0.6.3/setup.py
```

### Comparing `email-master-0.6.2/setup.py` & `email-master-0.6.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 with open('./README.rst') as f:
     long_description = f.read()
 
 setup(
     name='email-master',
     packages=['email_master', 'email_master.eml', 'email_master.msg', 'email_master.pgp'],
-    version='0.6.2',
+    version='0.6.3',
     description='Master Email Parsing Package',
     author='Swimlane',
     author_email="info@swimlane.com",
     long_description=long_description,
     install_requires=[
         "pendulum==2.1.2",
         "compressed-rtf==1.0.5",
         "extract_msg==0.23.2",
-        "PGPy==0.5.4",
-        "cryptography==37.0"
+        "PGPy==0.6.0"
     ],
     keywords=['utilities', 'email', 'parsing', 'eml', 'msg'],
     classifiers=[],
 )
```

### Comparing `email-master-0.6.2/email_master/compat.py` & `email-master-0.6.3/email_master/compat.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/msg/parser.py` & `email-master-0.6.3/email_master/msg/parser.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/eml/message.py` & `email-master-0.6.3/email_master/eml/message.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/eml/parser.py` & `email-master-0.6.3/email_master/eml/parser.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/parser.py` & `email-master-0.6.3/email_master/parser.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/attachments.py` & `email-master-0.6.3/email_master/attachments.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/messages.py` & `email-master-0.6.3/email_master/messages.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/util.py` & `email-master-0.6.3/email_master/util.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/pgp/config.py` & `email-master-0.6.3/email_master/pgp/config.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/pgp/wrapper.py` & `email-master-0.6.3/email_master/pgp/wrapper.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master/rfc3156.py` & `email-master-0.6.3/email_master/rfc3156.py`

 * *Files identical despite different names*

### Comparing `email-master-0.6.2/email_master.egg-info/SOURCES.txt` & `email-master-0.6.3/email_master.egg-info/SOURCES.txt`

 * *Files identical despite different names*

