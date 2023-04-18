# Comparing `tmp/samshee-0.1.3.tar.gz` & `tmp/samshee-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samshee-0.1.3.tar", last modified: Tue Apr 11 09:40:14 2023, max compression
+gzip compressed data, was "samshee-0.1.4.tar", last modified: Tue Apr 18 06:24:38 2023, max compression
```

## Comparing `samshee-0.1.3.tar` & `samshee-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.3/LICENSE
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 09:40:14.245348 samshee-0.1.3/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.3/README.md
--rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-04-11 09:40:08.000000 samshee-0.1.3/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-04-11 09:40:14.245348 samshee-0.1.3/setup.cfg
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/src/
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/src/samshee/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.3/src/samshee/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.3/src/samshee/samplesheetv2.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.3/src/samshee/sectionedsheet.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    26109 2023-04-11 09:39:21.000000 samshee-0.1.3/src/samshee/validation.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/src/samshee.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/top_level.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/tests/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.3/tests/test_validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.4/LICENSE
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-18 06:24:38.406971 samshee-0.1.4/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.4/README.md
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-04-18 06:24:04.000000 samshee-0.1.4/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-04-18 06:24:38.406971 samshee-0.1.4/setup.cfg
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.403638 samshee-0.1.4/src/
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/src/samshee/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.4/src/samshee/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.4/src/samshee/samplesheetv2.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.4/src/samshee/sectionedsheet.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    26101 2023-04-18 06:23:27.000000 samshee-0.1.4/src/samshee/validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/src/samshee.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/top_level.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/tests/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.4/tests/test_validation.py
```

### Comparing `samshee-0.1.3/LICENSE` & `samshee-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `samshee-0.1.3/PKG-INFO` & `samshee-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.3
+Version: 0.1.4
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.3/README.md` & `samshee-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `samshee-0.1.3/pyproject.toml` & `samshee-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samshee"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Jakob Simeth", email="jakob.simeth@ukr.de" }
 ]
 description="A schema-agnostic parser and writer for illumina sample sheets v2."
 readme = "README.md"
 license={file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `samshee-0.1.3/src/samshee/samplesheetv2.py` & `samshee-0.1.4/src/samshee/samplesheetv2.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.3/src/samshee/sectionedsheet.py` & `samshee-0.1.4/src/samshee/sectionedsheet.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.3/src/samshee/validation.py` & `samshee-0.1.4/src/samshee/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 },
                 "OverrideCycles": {
                     "type": "string",
                     "pattern": r"^([NYIU][0-9]+;?){1,}$",
                 },
                 "SoftwareVersion": {
                     "type": "string",
-                    "pattern": r"^[0-9]+\.[0-9]+\.[0-9]+.*",
+                    "pattern": r"^[0-9]+\.[0-9]+.*",
                 },
             },
             "BCLConvert_Data": {
                 "type": "object",
                 "required": ["Sample_ID"],
                 "properties": {
                     "Sample_ID": {
```

### Comparing `samshee-0.1.3/src/samshee.egg-info/PKG-INFO` & `samshee-0.1.4/src/samshee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.3
+Version: 0.1.4
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.3/tests/test_validation.py` & `samshee-0.1.4/tests/test_validation.py`

 * *Files identical despite different names*

