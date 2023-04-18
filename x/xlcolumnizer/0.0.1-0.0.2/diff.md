# Comparing `tmp/xlcolumnizer-0.0.1.tar.gz` & `tmp/xlcolumnizer-0.0.2.tar.gz`

## Comparing `xlcolumnizer-0.0.1.tar` & `xlcolumnizer-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.1/updatePackage.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.1/src/xlcolumnizer/__init__.py
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.1/src/xlcolumnizer/_excelColumnizer.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.1/README.md
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.2/updatePackage.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.2/src/xlcolumnizer/__init__.py
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.2/src/xlcolumnizer/_excelColumnizer.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.2/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xlcolumnizer-0.0.2/PKG-INFO
```

### Comparing `xlcolumnizer-0.0.1/updatePackage.txt` & `xlcolumnizer-0.0.2/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `xlcolumnizer-0.0.1/src/xlcolumnizer/_excelColumnizer.py` & `xlcolumnizer-0.0.2/src/xlcolumnizer/_excelColumnizer.py`

 * *Files identical despite different names*

### Comparing `xlcolumnizer-0.0.1/LICENSE.txt` & `xlcolumnizer-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xlcolumnizer-0.0.1/pyproject.toml` & `xlcolumnizer-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xlcolumnizer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A class that helps you recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -21,8 +21,7 @@
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: End Users/Desktop",
     "Development Status :: 5 - Production/Stable"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/generateNscore/xlcolumnizer"
-
```

