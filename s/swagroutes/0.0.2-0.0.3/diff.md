# Comparing `tmp/swagroutes-0.0.2.tar.gz` & `tmp/swagroutes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagroutes-0.0.2.tar", last modified: Tue Apr 18 18:54:06 2023, max compression
+gzip compressed data, was "swagroutes-0.0.3.tar", last modified: Tue Apr 18 19:15:07 2023, max compression
```

## Comparing `swagroutes-0.0.2.tar` & `swagroutes-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:54:06.861450 swagroutes-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 18:53:54.000000 swagroutes-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 18:54:06.861450 swagroutes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 18:53:54.000000 swagroutes-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:54:06.861450 swagroutes-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-18 18:53:54.000000 swagroutes-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:54:06.861450 swagroutes-0.0.2/swagroutes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 18:53:54.000000 swagroutes-0.0.2/swagroutes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-18 18:53:54.000000 swagroutes-0.0.2/swagroutes/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-18 18:53:54.000000 swagroutes-0.0.2/swagroutes/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:54:06.861450 swagroutes-0.0.2/swagroutes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 18:54:06.000000 swagroutes-0.0.2/swagroutes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-18 18:54:06.000000 swagroutes-0.0.2/swagroutes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:54:06.000000 swagroutes-0.0.2/swagroutes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 18:54:06.000000 swagroutes-0.0.2/swagroutes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 18:54:06.000000 swagroutes-0.0.2/swagroutes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 18:54:06.000000 swagroutes-0.0.2/swagroutes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:54:06.861450 swagroutes-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:53:54.000000 swagroutes-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-18 18:53:54.000000 swagroutes-0.0.2/tests/test_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:15:07.006977 swagroutes-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 19:14:55.000000 swagroutes-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 19:15:07.006977 swagroutes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 19:14:55.000000 swagroutes-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 19:15:07.010977 swagroutes-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-18 19:14:55.000000 swagroutes-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:15:07.006977 swagroutes-0.0.3/swagroutes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 19:14:55.000000 swagroutes-0.0.3/swagroutes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 19:14:55.000000 swagroutes-0.0.3/swagroutes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-18 19:14:55.000000 swagroutes-0.0.3/swagroutes/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-18 19:14:55.000000 swagroutes-0.0.3/swagroutes/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:15:07.006977 swagroutes-0.0.3/swagroutes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 19:15:06.000000 swagroutes-0.0.3/swagroutes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-18 19:15:07.000000 swagroutes-0.0.3/swagroutes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:15:06.000000 swagroutes-0.0.3/swagroutes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 19:15:06.000000 swagroutes-0.0.3/swagroutes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 19:15:06.000000 swagroutes-0.0.3/swagroutes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 19:15:06.000000 swagroutes-0.0.3/swagroutes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:15:07.006977 swagroutes-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 19:14:55.000000 swagroutes-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-18 19:14:55.000000 swagroutes-0.0.3/tests/test_extractor.py
```

### Comparing `swagroutes-0.0.2/LICENSE` & `swagroutes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.2/PKG-INFO` & `swagroutes-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagroutes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to fetch the details of assets hosted on AWS.
 Home-page: https://github.com/amalmurali47/swagroutes
 Author: Amal Murali
 Author-email: amalmurali47@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swagroutes-0.0.2/README.md` & `swagroutes-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.2/setup.py` & `swagroutes-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.2/swagroutes/cli.py` & `swagroutes-0.0.3/swagroutes/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,12 +24,7 @@
 
     if args.output:
         with open(args.output, 'w') as outfile:
             outfile.write('\n'.join(all_routes))
     else:
         for route in all_routes:
             print(route)
-
-
-if __name__ == "__main__":
-    main()
-
```

### Comparing `swagroutes-0.0.2/swagroutes/extractor.py` & `swagroutes-0.0.3/swagroutes/extractor.py`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.2/swagroutes.egg-info/PKG-INFO` & `swagroutes-0.0.3/swagroutes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagroutes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to fetch the details of assets hosted on AWS.
 Home-page: https://github.com/amalmurali47/swagroutes
 Author: Amal Murali
 Author-email: amalmurali47@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swagroutes-0.0.2/tests/test_extractor.py` & `swagroutes-0.0.3/tests/test_extractor.py`

 * *Files identical despite different names*

