# Comparing `tmp/dapr-ext-fastapi-dev-1.9.0rc1.dev1456.tar.gz` & `tmp/dapr-ext-fastapi-dev-1.9.0rc1.dev1472.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-fastapi-dev-1.9.0rc1.dev1456.tar", last modified: Tue Apr 11 18:06:02 2023, max compression
+gzip compressed data, was "dist/dapr-ext-fastapi-dev-1.9.0rc1.dev1472.tar", last modified: Tue Apr 18 17:05:16 2023, max compression
```

## Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456.tar` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-11 18:05:37.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-11 18:05:37.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-11 18:05:37.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-11 18:05:37.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-11 18:05:37.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 18:05:37.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr_ext_fastapi_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr_ext_fastapi_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr_ext_fastapi_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr_ext_fastapi_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr_ext_fastapi_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr_ext_fastapi_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-11 18:06:02.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-11 18:05:37.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1456/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-18 17:04:51.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-18 17:04:51.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-18 17:04:51.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-18 17:04:51.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-18 17:04:51.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 17:04:51.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr_ext_fastapi_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr_ext_fastapi_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr_ext_fastapi_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr_ext_fastapi_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr_ext_fastapi_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr_ext_fastapi_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-18 17:05:16.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-18 17:04:51.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1472/setup.py
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/LICENSE` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/PKG-INFO` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-fastapi-dev
-Version: 1.9.0rc1.dev1456
+Version: 1.9.0rc1.dev1472
 Summary: The developmental release for Dapr FastAPI extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/__init__.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/actor.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/app.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr/ext/fastapi/version.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr/ext/fastapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/dapr_ext_fastapi_dev.egg-info/PKG-INFO` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/dapr_ext_fastapi_dev.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-fastapi-dev
-Version: 1.9.0rc1.dev1456
+Version: 1.9.0rc1.dev1472
 Summary: The developmental release for Dapr FastAPI extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/setup.cfg` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1456/setup.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1472/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

