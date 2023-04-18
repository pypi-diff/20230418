# Comparing `tmp/excelcolumnizer-0.0.3.tar.gz` & `tmp/excelcolumnizer-0.0.4.tar.gz`

## Comparing `excelcolumnizer-0.0.3.tar` & `excelcolumnizer-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.3/updatePackage.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.3/src/excelcolumnizer/__init__.py
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.3/src/excelcolumnizer/_excelColumnizer.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.3/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/updatePackage.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/src/excelcolumnizer/__init__.py
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/src/excelcolumnizer/_excelColumnizer.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/PKG-INFO
```

### Comparing `excelcolumnizer-0.0.3/updatePackage.txt` & `excelcolumnizer-0.0.4/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.3/src/excelcolumnizer/_excelColumnizer.py` & `excelcolumnizer-0.0.4/src/excelcolumnizer/_excelColumnizer.py`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.3/LICENSE.txt` & `excelcolumnizer-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.3/README.md` & `excelcolumnizer-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 ## What is it?
 
 A package that helps you recover columns of Excel data converted from PDF files.
 
 ## Where to get it
 
-<pre lang=sh>pip install xlcolumnizer</pre>
+<pre lang=sh>pip install excelcolumnizer</pre>
 
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.3</li>
+<li>Version 0.0.4</li>
 
 ```python
 
 import excelcolumnizer as xl
 
 xlpath='<full name of your excel file including extension>'
 xl.sheet(xlpath)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # excelcolumnizer ## What is it? A package that helps you recover columns of
 Excel data converted from PDF files. ## Where to get it
-pip install xlcolumnizer
+pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.3
+    * Version 0.0.4
     * ```python import excelcolumnizer as xl xlpath='' xl.sheet(xlpath) ```
           o A GUI with tksheet will be opened with the contents of excel file.
           o Here is a recommending set of actions to try:
                1. Remove unwanted rows (F7)
                2. Remove unwanted columns (F7) or combine columns (F5)
                3. Click a cell to insert (F1) or delete the cell (F3)
           o
```

### Comparing `excelcolumnizer-0.0.3/pyproject.toml` & `excelcolumnizer-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excelcolumnizer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A small packages that helps you recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `excelcolumnizer-0.0.3/PKG-INFO` & `excelcolumnizer-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excelcolumnizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -21,24 +21,24 @@
 
 ## What is it?
 
 A package that helps you recover columns of Excel data converted from PDF files.
 
 ## Where to get it
 
-<pre lang=sh>pip install xlcolumnizer</pre>
+<pre lang=sh>pip install excelcolumnizer</pre>
 
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.3</li>
+<li>Version 0.0.4</li>
 
 ```python
 
 import excelcolumnizer as xl
 
 xlpath='<full name of your excel file including extension>'
 xl.sheet(xlpath)
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.3 Summary: A small
+Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.4 Summary: A small
 packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier: Topic
 :: Office/Business :: Financial :: Accounting Classifier: Topic :: Office/
 Business :: Financial :: Point-Of-Sale Classifier: Topic :: Office/Business ::
 Financial :: Spreadsheet Requires-Python: >=3.7 Description-Content-Type: text/
 markdown # excelcolumnizer ## What is it? A package that helps you recover
 columns of Excel data converted from PDF files. ## Where to get it
-pip install xlcolumnizer
+pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.3
+    * Version 0.0.4
     * ```python import excelcolumnizer as xl xlpath='' xl.sheet(xlpath) ```
           o A GUI with tksheet will be opened with the contents of excel file.
           o Here is a recommending set of actions to try:
                1. Remove unwanted rows (F7)
                2. Remove unwanted columns (F7) or combine columns (F5)
                3. Click a cell to insert (F1) or delete the cell (F3)
           o
```

