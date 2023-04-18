# Comparing `tmp/polymers-0.3.0-cp39-none-win_amd64.whl.zip` & `tmp/polymers-0.3.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1141122 bytes, number of entries: 6
--rw-r--r--  4.6 unx     4213 b- defN 23-Apr-06 21:38 polymers-0.3.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-06 21:38 polymers-0.3.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     1569 b- defN 23-Apr-06 21:38 polymers-0.3.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      115 b- defN 23-Apr-06 21:38 polymers/__init__.py
--rwxr-xr-x  4.6 unx  4718592 b- defN 23-Apr-06 21:38 polymers/polymers.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      484 b- defN 23-Apr-06 21:38 polymers-0.3.0.dist-info/RECORD
-6 files, 4725069 bytes uncompressed, 1140252 bytes compressed:  75.9%
+Zip file size: 1172636 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     4213 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1569 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      115 b- defN 23-Apr-18 19:35 polymers/__init__.py
+-rwxr-xr-x  4.6 unx  4857344 b- defN 23-Apr-18 19:35 polymers/polymers.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      484 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/RECORD
+6 files, 4863821 bytes uncompressed, 1171766 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: polymers-0.3.0.dist-info/METADATA
+Filename: polymers-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: polymers-0.3.0.dist-info/WHEEL
+Filename: polymers-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: polymers-0.3.0.dist-info/license_files/LICENSE
+Filename: polymers-0.3.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: polymers/__init__.py
 Comment: 
 
 Filename: polymers/polymers.cp39-win_amd64.pyd
 Comment: 
 
-Filename: polymers-0.3.0.dist-info/RECORD
+Filename: polymers-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `polymers-0.3.0.dist-info/METADATA` & `polymers-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymers
-Version: 0.3.0
+Version: 0.3.1
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: cffi
@@ -14,17 +14,17 @@
 Summary: Polymers Modeling Library
 Keywords: julia,polymers,python,rust
 Author: Michael R. Buche
 Author-email: mrbuche@sandia.gov
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://sandialabs.github.io/Polymers
 Project-URL: Repository, https://github.com/sandialabs/polymers
 Project-URL: Documentation, https://polymers.readthedocs.io
+Project-URL: Homepage, https://sandialabs.github.io/Polymers
 
 # Polymers Modeling Library
 
 [![website](https://img.shields.io/badge/GitHub-website-6e5494?logo=github)](https://sandialabs.github.io/Polymers)
 [![examples](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/binder.svg)](https://mybinder.org/v2/gh/sandialabs/Polymers/main)
 
 The library is implemented entirely in Rust, including the Python API. The Julia API calls the Rust library.
```

## Comparing `polymers-0.3.0.dist-info/license_files/LICENSE` & `polymers-0.3.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

