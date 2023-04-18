# Comparing `tmp/swin-0.0.4.tar.gz` & `tmp/swin-0.0.5.tar.gz`

## Comparing `swin-0.0.4.tar` & `swin-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swin-0.0.4/src/swin/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 swin-0.0.4/src/swin/opts.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 swin-0.0.4/src/swin/package.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swin-0.0.4/src/swin/swin.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 swin-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 swin-0.0.4/LICENSE
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 swin-0.0.4/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 swin-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 swin-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 swin-0.0.5/.github/workflows/lints.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swin-0.0.5/src/swin/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 swin-0.0.5/src/swin/opts.py
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 swin-0.0.5/src/swin/package.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 swin-0.0.5/src/swin/swin.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 swin-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 swin-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 swin-0.0.5/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 swin-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 swin-0.0.5/PKG-INFO
```

### Comparing `swin-0.0.4/src/swin/package.py` & `swin-0.0.5/src/swin/package.py`

 * *Files identical despite different names*

### Comparing `swin-0.0.4/src/swin/swin.py` & `swin-0.0.5/src/swin/swin.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from argparse import ArgumentParser
 from datetime import timedelta
 from prettytable import PrettyTable
 from swin import opts
 from swin.package import PyPIPackage
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 def _print_summary(packages):
     '''
     Prints a summary across packages.
     '''
     print('\nSummary for ', opts.start_date, ' - ', opts.end_date, ':\n', sep='')
     print(packages[0].registry, 'packages by download number:')
@@ -40,18 +40,22 @@
 
 def main():
     '''
     CLI entry
     '''
     parser = ArgumentParser(description='Simple analytics for PyPI packages based on `pypistats`')
     parser.add_argument('--version', action='version', version='%(prog)s '+VERSION)
+    parser.add_argument('--ref', help='reference comparison package')
     parser.add_argument('package', nargs='+', help='PyPI package names for processing')
-    packages = [PyPIPackage(p) for p in parser.parse_args().package]
+    args = parser.parse_args()
+
+    ref = args.ref
+    if ref: ref = PyPIPackage(ref)
+    packages = [PyPIPackage(p, ref=ref) for p in args.package]
 
     for package in packages:
         package.plot_downloads_with_trend()
-# Will add CLI for ref packages later
-#       if package.ref:
-#           package.plot_downloads_share_with_trend()
+        if ref:
+            package.plot_downloads_share_with_trend()
 
     packages.sort(key=lambda package: package.total_downloads, reverse=True)
     _print_summary(packages)
```

### Comparing `swin-0.0.4/.gitignore` & `swin-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `swin-0.0.4/LICENSE` & `swin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swin-0.0.4/pyproject.toml` & `swin-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swin-0.0.4/PKG-INFO` & `swin-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Swin: SoftWare INsights
 Project-URL: Homepage, https://github.com/lunarserge/swin
 Project-URL: Bug Tracker, https://github.com/lunarserge/swin/issues
 Author: Serge Lunev
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,12 +24,22 @@
 
 ## Installation from PyPI
 
 `pip install --upgrade swin`
 
 ## Command-Line Use
 
-`swin [--help] [--version] packages`
+    swin [--help] [--version] [--ref REF] package [package ...]
+
+    positional arguments:
+      package     PyPI package names for processing
+
+    options:
+      -h, --help  show this help message and exit
+      --version   show program's version number and exit
+      --ref REF   reference comparison package
 
 `swin` will create 'charts' folder (or use the existing one) in the current directory and put there one PNG file per input package with daily downloads chart and a trend over time.
 
-`swin` will also print a sorted table with download statistics of the packages specified in the command line.
+`swin` will also print a sorted table with download statistics of the packages specified in the command line.
+
+If `REF` package is specified then `swin` creates additional charts for the share of input packages in comparison with the reference comparison package (e.g. `modin` downloads as percentage of `pandas` downloads over time). These charts include a trendline as well and prefixed with `share-`.
```

