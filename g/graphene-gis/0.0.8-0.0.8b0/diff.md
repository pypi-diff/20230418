# Comparing `tmp/graphene-gis-0.0.8.tar.gz` & `tmp/graphene-gis-0.0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graphene-gis-0.0.8.tar", last modified: Tue Apr 18 20:51:23 2023, max compression
+gzip compressed data, was "dist/graphene-gis-0.0.8b0.tar", last modified: Mon Feb 28 07:30:21 2022, max compression
```

## Comparing `graphene-gis-0.0.8.tar` & `graphene-gis-0.0.8b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/
--rw-r--r--   0 frost     (1000) frost     (1000)     1060 2022-02-28 07:21:01.000000 graphene-gis-0.0.8/LICENSE.md
--rw-r--r--   0 frost     (1000) frost     (1000)     6234 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)     5695 2023-04-18 20:51:03.000000 graphene-gis-0.0.8/README.md
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/graphene_gis/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2020-06-20 23:25:40.000000 graphene-gis-0.0.8/graphene_gis/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1124 2022-02-11 20:52:54.000000 graphene-gis-0.0.8/graphene_gis/converter.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1539 2022-02-28 07:21:04.000000 graphene-gis-0.0.8/graphene_gis/scalars.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/graphene_gis.egg-info/
--rw-r--r--   0 frost     (1000) frost     (1000)     6234 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/graphene_gis.egg-info/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)      318 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/graphene_gis.egg-info/SOURCES.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/graphene_gis.egg-info/dependency_links.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        1 2021-01-04 06:59:21.000000 graphene-gis-0.0.8/graphene_gis.egg-info/not-zip-safe
--rw-r--r--   0 frost     (1000) frost     (1000)      194 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/graphene_gis.egg-info/requires.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       13 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/graphene_gis.egg-info/top_level.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-04-18 20:51:23.000000 graphene-gis-0.0.8/setup.cfg
--rw-r--r--   0 frost     (1000) frost     (1000)     1226 2023-04-18 20:51:03.000000 graphene-gis-0.0.8/setup.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/
+-rw-r--r--   0 frost     (1000) frost     (1000)     1060 2022-02-28 07:21:01.000000 graphene-gis-0.0.8b0/LICENSE.md
+-rw-r--r--   0 frost     (1000) frost     (1000)     6150 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)     5590 2022-02-28 07:23:30.000000 graphene-gis-0.0.8b0/README.md
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/graphene_gis/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2020-06-20 23:25:40.000000 graphene-gis-0.0.8b0/graphene_gis/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1124 2022-02-11 20:52:54.000000 graphene-gis-0.0.8b0/graphene_gis/converter.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1539 2022-02-28 07:21:04.000000 graphene-gis-0.0.8b0/graphene_gis/scalars.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/graphene_gis.egg-info/
+-rw-r--r--   0 frost     (1000) frost     (1000)     6150 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/graphene_gis.egg-info/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)      318 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/graphene_gis.egg-info/SOURCES.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        1 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/graphene_gis.egg-info/dependency_links.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        1 2021-01-04 06:59:21.000000 graphene-gis-0.0.8b0/graphene_gis.egg-info/not-zip-safe
+-rw-r--r--   0 frost     (1000) frost     (1000)      219 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/graphene_gis.egg-info/requires.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       13 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/graphene_gis.egg-info/top_level.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       38 2022-02-28 07:30:21.000000 graphene-gis-0.0.8b0/setup.cfg
+-rw-r--r--   0 frost     (1000) frost     (1000)     1264 2022-02-28 07:23:57.000000 graphene-gis-0.0.8b0/setup.py
```

### Comparing `graphene-gis-0.0.8/LICENSE.md` & `graphene-gis-0.0.8b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `graphene-gis-0.0.8/PKG-INFO` & `graphene-gis-0.0.8b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: graphene-gis
-Version: 0.0.8
+Version: 0.0.8b0
 Summary: GIS support for graphene-django
 Home-page: https://github.com/EverWinter23/graphene-gis
 Author: Rishabh Mehta
 Author-email: eternal.blizzard23@gmail.com
+License: UNKNOWN
 Keywords: api graphql graphene geos gis
 Platform: any
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE.md
 
 ### graphene-gis
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/EverWinter23/graphene-gis/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/EverWinter23/graphene-gis/tree/master)
+[![CircleCI](https://circleci.com/gh/EverWinter23/graphene-gis.svg?style=shield)](https://circleci.com/gh/EverWinter23/graphene-gis)
 
 ### INSTALLATION
 
 `django==2.2` is supported. Install the `graphene-gis` with pip:
 
 ```bash
 $ pip install graphene-gis
@@ -228,14 +229,15 @@
 $ twine upload dist/*
 ```
 
 ### UPDATE
 
 - [x] Targeting graphene-v3 update by March'22 -> [MR](https://github.com/EverWinter23/graphene-gis/pull/16)
 - Install the pre-release using:
-- [ ] Django 4.2 LTS support by May'23
 
   `pip install graphene-gis==0.0.8b0`
 
 ### LICENSE [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This code falls under the MIT license which permits the reuse of the proprietary software provided that all copies of the licensed software include a copy of the MIT License terms and the copyright notice. Go crazy!
+
+
```

### Comparing `graphene-gis-0.0.8/README.md` & `graphene-gis-0.0.8b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### graphene-gis
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/EverWinter23/graphene-gis/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/EverWinter23/graphene-gis/tree/master)
+[![CircleCI](https://circleci.com/gh/EverWinter23/graphene-gis.svg?style=shield)](https://circleci.com/gh/EverWinter23/graphene-gis)
 
 ### INSTALLATION
 
 `django==2.2` is supported. Install the `graphene-gis` with pip:
 
 ```bash
 $ pip install graphene-gis
@@ -211,14 +211,13 @@
 $ twine upload dist/*
 ```
 
 ### UPDATE
 
 - [x] Targeting graphene-v3 update by March'22 -> [MR](https://github.com/EverWinter23/graphene-gis/pull/16)
 - Install the pre-release using:
-- [ ] Django 4.2 LTS support by May'23
 
   `pip install graphene-gis==0.0.8b0`
 
 ### LICENSE [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This code falls under the MIT license which permits the reuse of the proprietary software provided that all copies of the licensed software include a copy of the MIT License terms and the copyright notice. Go crazy!
```

### Comparing `graphene-gis-0.0.8/graphene_gis/converter.py` & `graphene-gis-0.0.8b0/graphene_gis/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-gis-0.0.8/graphene_gis/scalars.py` & `graphene-gis-0.0.8b0/graphene_gis/scalars.py`

 * *Files identical despite different names*

### Comparing `graphene-gis-0.0.8/graphene_gis.egg-info/PKG-INFO` & `graphene-gis-0.0.8b0/graphene_gis.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: graphene-gis
-Version: 0.0.8
+Version: 0.0.8b0
 Summary: GIS support for graphene-django
 Home-page: https://github.com/EverWinter23/graphene-gis
 Author: Rishabh Mehta
 Author-email: eternal.blizzard23@gmail.com
+License: UNKNOWN
 Keywords: api graphql graphene geos gis
 Platform: any
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE.md
 
 ### graphene-gis
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/EverWinter23/graphene-gis/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/EverWinter23/graphene-gis/tree/master)
+[![CircleCI](https://circleci.com/gh/EverWinter23/graphene-gis.svg?style=shield)](https://circleci.com/gh/EverWinter23/graphene-gis)
 
 ### INSTALLATION
 
 `django==2.2` is supported. Install the `graphene-gis` with pip:
 
 ```bash
 $ pip install graphene-gis
@@ -228,14 +229,15 @@
 $ twine upload dist/*
 ```
 
 ### UPDATE
 
 - [x] Targeting graphene-v3 update by March'22 -> [MR](https://github.com/EverWinter23/graphene-gis/pull/16)
 - Install the pre-release using:
-- [ ] Django 4.2 LTS support by May'23
 
   `pip install graphene-gis==0.0.8b0`
 
 ### LICENSE [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This code falls under the MIT license which permits the reuse of the proprietary software provided that all copies of the licensed software include a copy of the MIT License terms and the copyright notice. Go crazy!
+
+
```

### Comparing `graphene-gis-0.0.8/setup.py` & `graphene-gis-0.0.8b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,38 +12,39 @@
 ] + tests_require
 
 with open("README.md", "r") as desc:
     long_description = desc.read()
 
 setup(
     name="graphene-gis",
-    version="0.0.8",
+    version="0.0.8b0",
     description="GIS support for graphene-django",
     long_description_content_type='text/markdown',
     url="https://github.com/EverWinter23/graphene-gis",
     long_description=long_description,
     keywords="api graphql graphene geos gis",
     packages=find_packages(exclude=["tests"]),
     author="Rishabh Mehta",
     author_email="eternal.blizzard23@gmail.com",
     install_requires=[
         "graphene>=3.0.0,<4",
-        "graphene-django>=3.0.0,<4",
+        "graphene-django>=3.0.0b7,<4",
+        "graphql-core>=3.1.2,<4",
     ],
 
     setup_requires=["pytest-runner"],
     tests_require=tests_require,
 
     extras_require={
         "test": tests_require,
         "dev": dev_requires,
     },
 
     classifiers=(
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ),
 
     include_package_data=True,
     zip_safe=False,
     platforms="any",
```

