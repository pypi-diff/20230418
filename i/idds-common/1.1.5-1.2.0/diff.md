# Comparing `tmp/idds-common-1.1.5.tar.gz` & `tmp/idds-common-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-common-1.1.5.tar", last modified: Sat Mar  4 21:39:56 2023, max compression
+gzip compressed data, was "idds-common-1.2.0.tar", last modified: Tue Apr 18 09:36:51 2023, max compression
```

## Comparing `idds-common-1.1.5.tar` & `idds-common-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.017593 idds-common-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-04 21:39:47.000000 idds-common-1.1.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-04 21:39:56.017593 idds-common-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-04 21:39:47.000000 idds-common-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.013593 idds-common-1.1.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.013593 idds-common-1.1.5/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.013593 idds-common-1.1.5/lib/idds/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20052 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/dict_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.013593 idds-common-1.1.5/lib/idds/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/plugin/plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-03-04 21:39:47.000000 idds-common-1.1.5/lib/idds/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-04 21:39:54.000000 idds-common-1.1.5/lib/idds/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.017593 idds-common-1.1.5/lib/idds_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-04 21:39:55.000000 idds-common-1.1.5/lib/idds_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-04 21:39:55.000000 idds-common-1.1.5/lib/idds_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 21:39:55.000000 idds-common-1.1.5/lib/idds_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-04 21:39:55.000000 idds-common-1.1.5/lib/idds_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-04 21:39:55.000000 idds-common-1.1.5/lib/idds_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 21:39:56.017593 idds-common-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-03-04 21:39:47.000000 idds-common-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.013593 idds-common-1.1.5/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.017593 idds-common-1.1.5/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-04 21:39:54.000000 idds-common-1.1.5/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 09:36:40.000000 idds-common-1.2.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 09:36:51.574952 idds-common-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 09:36:40.000000 idds-common-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/lib/idds/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/dict_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/lib/idds/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/plugin/plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-18 09:36:40.000000 idds-common-1.2.0/lib/idds/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 09:36:49.000000 idds-common-1.2.0/lib/idds/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/lib/idds_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 09:36:51.000000 idds-common-1.2.0/lib/idds_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 09:36:51.000000 idds-common-1.2.0/lib/idds_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:36:51.000000 idds-common-1.2.0/lib/idds_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 09:36:51.000000 idds-common-1.2.0/lib/idds_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 09:36:51.000000 idds-common-1.2.0/lib/idds_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 09:36:51.578952 idds-common-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-18 09:36:40.000000 idds-common-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:51.574952 idds-common-1.2.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-18 09:36:49.000000 idds-common-1.2.0/tools/env/environment.yml
```

### Comparing `idds-common-1.1.5/LICENSE.rst` & `idds-common-1.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/PKG-INFO` & `idds-common-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.1.5
+Version: 1.2.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.1.5/lib/idds/common/authentication.py` & `idds-common-1.2.0/lib/idds/common/authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -380,14 +380,16 @@
 # "/DC=ch/DC=cern/OU=Organic Units/OU=Users/CN=wguan/CN=667815/CN=Wen Guan/CN=1883443395"
 def get_user_name_from_dn1(dn):
     try:
         up = re.compile('/(DC|O|OU|C|L)=[^\/]+')        # noqa W605
         username = up.sub('', dn)
         up2 = re.compile('/CN=[0-9]+')
         username = up2.sub('', username)
+        up2 = re.compile('/CN=[0-9]+')
+        username = up2.sub('', username)
         up3 = re.compile(' [0-9]+')
         username = up3.sub('', username)
         up4 = re.compile('_[0-9]+')
         username = up4.sub('', username)
         username = username.replace('/CN=proxy', '')
         username = username.replace('/CN=limited proxy', '')
         username = username.replace('limited proxy', '')
@@ -417,23 +419,28 @@
 # 'CN=203633261,CN=Wen Guan,CN=667815,CN=wguan,OU=Users,OU=Organic Units,DC=cern,DC=ch'
 def get_user_name_from_dn2(dn):
     try:
         up = re.compile(',(DC|O|OU|C|L)=[^\,]+')        # noqa W605
         username = up.sub('', dn)
         up2 = re.compile(',CN=[0-9]+')
         username = up2.sub('', username)
+        up2 = re.compile('CN=[0-9]+,')
+        username = up2.sub(',', username)
         up3 = re.compile(' [0-9]+')
         username = up3.sub('', username)
         up4 = re.compile('_[0-9]+')
         username = up4.sub('', username)
         username = username.replace(',CN=proxy', '')
         username = username.replace(',CN=limited proxy', '')
         username = username.replace('limited proxy', '')
+        username = re.sub(',CN=Robot:[^/]+,', ',', username)
         username = re.sub(',CN=Robot:[^/]+', '', username)
+        username = re.sub(',CN=Robot[^/]+,', ',', username)
         username = re.sub(',CN=Robot[^/]+', '', username)
+        username = re.sub(',CN=nickname:[^/]+,', ',', username)
         username = re.sub(',CN=nickname:[^/]+', '', username)
         pat = re.compile('.*,CN=([^\,]+),CN=([^\,]+)')         # noqa W605
         mat = pat.match(username)
         if mat:
             username = mat.group(1)
         else:
             username = username.replace(',CN=', '')
```

### Comparing `idds-common-1.1.5/lib/idds/common/cache.py` & `idds-common-1.2.0/lib/idds/common/cache.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/lib/idds/common/config.py` & `idds-common-1.2.0/lib/idds/common/config.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/lib/idds/common/constants.py` & `idds-common-1.2.0/lib/idds/common/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2022
+# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 """
 Constants.
 """
 
 from enum import Enum
 
@@ -28,14 +28,16 @@
     Transformer = 'transformer'
     Transporter = 'transporter'
     Carrier = 'carrier'
     Conductor = 'conductor'
     Consumer = 'consumer'
     EventBus = 'eventbus'
     Cache = 'cache'
+    Archiver = 'archiver'
+    Coordinator = 'coordinator'
 
 
 class HTTP_STATUS_CODE:
     OK = 200
     Created = 201
     Accepted = 202
 
@@ -284,21 +286,28 @@
     Failed = 3
     FinalFailed = 4
     Lost = 5
     Deleted = 6
     Mapped = 7
     FakeAvailable = 8
     Missing = 9
+    Cancelled = 10
 
 
 class ContentLocking(IDDSEnum):
     Idle = 0
     Locking = 1
 
 
+class ContentFetchStatus(IDDSEnum):
+    New = 0
+    Fetching = 1
+    Fetched = 2
+
+
 class GranularityType(IDDSEnum):
     File = 0
     Event = 1
 
 
 class ProcessingStatus(IDDSEnum):
     New = 0
@@ -334,14 +343,20 @@
 
 
 class ProcessingLocking(IDDSEnum):
     Idle = 0
     Locking = 1
 
 
+class HealthStatus(IDDSEnum):
+    Default = 0
+    InActive = 1
+    Active = 2
+
+
 class MessageType(IDDSEnum):
     StageInFile = 0
     StageInCollection = 1
     StageInWork = 2
     ActiveLearningFile = 3
     ActiveLearningCollection = 4
     ActiveLearningWork = 5
@@ -465,14 +480,20 @@
     Transporter = 2
     Carrier = 3
     Conductor = 4
     Rest = 5
     Other = 6
 
 
+class ReturnCode(IDDSEnum):
+    Ok = 0
+    Failed = 255
+    Locked = 1
+
+
 def get_work_status_from_transform_processing_status(status):
     if status in [ProcessingStatus.New, TransformStatus.New]:
         return WorkStatus.New
     elif status in [ProcessingStatus.Submitting, ProcessingStatus.Submitted, TransformStatus.Transforming]:
         return WorkStatus.Transforming
     elif status in [ProcessingStatus.Running]:
         return WorkStatus.Transforming
```

### Comparing `idds-common-1.1.5/lib/idds/common/dict_class.py` & `idds-common-1.2.0/lib/idds/common/dict_class.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/lib/idds/common/exceptions.py` & `idds-common-1.2.0/lib/idds/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/lib/idds/common/plugin/plugin_base.py` & `idds-common-1.2.0/lib/idds/common/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/lib/idds/common/plugin/plugin_utils.py` & `idds-common-1.2.0/lib/idds/common/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/lib/idds/common/status_utils.py` & `idds-common-1.2.0/lib/idds/common/status_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.1.5/lib/idds/common/utils.py` & `idds-common-1.2.0/lib/idds/common/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2021
+# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 
+import errno
 import datetime
 import logging
 import json
 import os
 import re
 import requests
 import subprocess
@@ -519,7 +520,64 @@
             did = did[:-1]
         return scope, did
 
 
 def truncate_string(string, length=800):
     string = (string[:length] + '...') if string and len(string) > length else string
     return string
+
+
+def merge_dict(dict1, dict2):
+    keys = list(dict1.keys())
+    for key in list(dict2.keys()):
+        if key not in keys:
+            keys.append(key)
+    for key in keys:
+        if key in dict2:
+            if key not in dict1 or dict1[key] is None:
+                dict1[key] = dict2[key]
+            else:
+                if dict2[key] is None:
+                    continue
+                elif isinstance(dict1[key], type(dict2[key])):
+                    raise Exception("type of %s is different from %s, cannot merge" % (type(dict1[key]), type(dict2[key])))
+                elif dict1[key] == dict2[key]:
+                    continue
+                elif type(dict1[key]) in (list, tuple, str):
+                    dict1[key] = dict1[key] + dict2[key]
+                elif type(dict1[key]) in (int, float, complex):
+                    dict1[key] = dict1[key] + dict2[key]
+                elif type(dict1[key]) in (bool, bool):
+                    dict1[key] = True
+                elif type(dict1[key]) in (dict, dict):
+                    dict1[key] = merge_dict(dict1[key], dict2[key])
+    return dict1
+
+
+def pid_exists(pid):
+    """
+    Check whether pid exists in the current process table.
+    UNIX only.
+    """
+    if pid < 0:
+        return False
+    if pid == 0:
+        # According to "man 2 kill" PID 0 refers to every process
+        # in the process group of the calling process.
+        # On certain systems 0 is a valid PID but we have no way
+        # to know that in a portable fashion.
+        raise ValueError('invalid PID 0')
+    try:
+        os.kill(pid, 0)
+    except OSError as err:
+        if err.errno == errno.ESRCH:
+            # ESRCH == No such process
+            return False
+        elif err.errno == errno.EPERM:
+            # EPERM clearly means there's a process to deny access to
+            return True
+        else:
+            # According to "man 2 kill" possible error values are
+            # (EINVAL, EPERM, ESRCH)
+            raise
+    else:
+        return True
```

### Comparing `idds-common-1.1.5/lib/idds_common.egg-info/PKG-INFO` & `idds-common-1.2.0/lib/idds_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.1.5
+Version: 1.2.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.1.5/lib/idds_common.egg-info/SOURCES.txt` & `idds-common-1.2.0/lib/idds_common.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 lib/idds/__init__.py
 lib/idds/common/__init__.py
 lib/idds/common/authentication.py
 lib/idds/common/cache.py
 lib/idds/common/config.py
 lib/idds/common/constants.py
 lib/idds/common/dict_class.py
+lib/idds/common/event.py
 lib/idds/common/exceptions.py
 lib/idds/common/status_utils.py
 lib/idds/common/utils.py
 lib/idds/common/version.py
 lib/idds/common/plugin/__init__.py
 lib/idds/common/plugin/plugin_base.py
 lib/idds/common/plugin/plugin_utils.py
```

### Comparing `idds-common-1.1.5/setup.py` & `idds-common-1.2.0/setup.py`

 * *Files identical despite different names*

