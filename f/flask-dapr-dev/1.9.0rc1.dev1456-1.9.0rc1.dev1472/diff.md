# Comparing `tmp/flask-dapr-dev-1.9.0rc1.dev1456.tar.gz` & `tmp/flask-dapr-dev-1.9.0rc1.dev1472.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-dapr-dev-1.9.0rc1.dev1456.tar", last modified: Tue Apr 11 18:05:53 2023, max compression
+gzip compressed data, was "dist/flask-dapr-dev-1.9.0rc1.dev1472.tar", last modified: Tue Apr 18 17:05:08 2023, max compression
```

## Comparing `flask-dapr-dev-1.9.0rc1.dev1456.tar` & `flask-dapr-dev-1.9.0rc1.dev1472.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-11 18:05:37.000000 flask-dapr-dev-1.9.0rc1.dev1456/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-11 18:05:37.000000 flask-dapr-dev-1.9.0rc1.dev1456/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-11 18:05:37.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-11 18:05:37.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-11 18:05:37.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 18:05:37.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-11 18:05:53.000000 flask-dapr-dev-1.9.0rc1.dev1456/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-11 18:05:37.000000 flask-dapr-dev-1.9.0rc1.dev1456/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-18 17:04:51.000000 flask-dapr-dev-1.9.0rc1.dev1472/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-18 17:04:51.000000 flask-dapr-dev-1.9.0rc1.dev1472/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-18 17:04:51.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-18 17:04:51.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-18 17:04:51.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 17:04:51.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-18 17:05:08.000000 flask-dapr-dev-1.9.0rc1.dev1472/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-18 17:04:51.000000 flask-dapr-dev-1.9.0rc1.dev1472/setup.py
```

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/LICENSE` & `flask-dapr-dev-1.9.0rc1.dev1472/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/PKG-INFO` & `flask-dapr-dev-1.9.0rc1.dev1472/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask-dapr-dev
-Version: 1.9.0rc1.dev1456
+Version: 1.9.0rc1.dev1472
 Summary: The developmental release for Dapr Python SDK Flask.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/README.rst` & `flask-dapr-dev-1.9.0rc1.dev1472/README.rst`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/__init__.py` & `flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/__init__.py`

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

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/actor.py` & `flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/actor.py`

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

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/app.py` & `flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/app.py`

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

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr/version.py` & `flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr/version.py`

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

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/flask_dapr_dev.egg-info/PKG-INFO` & `flask-dapr-dev-1.9.0rc1.dev1472/flask_dapr_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask-dapr-dev
-Version: 1.9.0rc1.dev1456
+Version: 1.9.0rc1.dev1472
 Summary: The developmental release for Dapr Python SDK Flask.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/setup.cfg` & `flask-dapr-dev-1.9.0rc1.dev1472/setup.cfg`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1456/setup.py` & `flask-dapr-dev-1.9.0rc1.dev1472/setup.py`

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

