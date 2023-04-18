# Comparing `tmp/helloworldplayerlili-0.0.1.tar.gz` & `tmp/helloworldplayerlili-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helloworldplayerlili-0.0.1.tar", last modified: Tue Apr 18 14:58:09 2023, max compression
+gzip compressed data, was "helloworldplayerlili-0.0.2.tar", last modified: Tue Apr 18 15:07:12 2023, max compression
```

## Comparing `helloworldplayerlili-0.0.1.tar` & `helloworldplayerlili-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 14:58:09.748475 helloworldplayerlili-0.0.1/
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)    35148 2023-04-18 12:58:47.000000 helloworldplayerlili-0.0.1/LICENSE
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      731 2023-04-18 14:58:09.748475 helloworldplayerlili-0.0.1/PKG-INFO
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      604 2023-04-18 14:57:47.000000 helloworldplayerlili-0.0.1/README.md
-drwxrwxr-x   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 14:58:09.748475 helloworldplayerlili-0.0.1/helloworldplayerlili/
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)       42 2023-04-18 12:52:36.000000 helloworldplayerlili-0.0.1/helloworldplayerlili/__init__.py
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 12:41:54.000000 helloworldplayerlili-0.0.1/helloworldplayerlili/lala.py
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      507 2023-04-18 12:52:22.000000 helloworldplayerlili-0.0.1/helloworldplayerlili/player.py
-drwxrwxr-x   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 14:58:09.748475 helloworldplayerlili-0.0.1/helloworldplayerlili.egg-info/
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      731 2023-04-18 14:58:09.000000 helloworldplayerlili-0.0.1/helloworldplayerlili.egg-info/PKG-INFO
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      295 2023-04-18 14:58:09.000000 helloworldplayerlili-0.0.1/helloworldplayerlili.egg-info/SOURCES.txt
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        1 2023-04-18 14:58:09.000000 helloworldplayerlili-0.0.1/helloworldplayerlili.egg-info/dependency_links.txt
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)       21 2023-04-18 14:58:09.000000 helloworldplayerlili-0.0.1/helloworldplayerlili.egg-info/top_level.txt
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)       38 2023-04-18 14:58:09.748475 helloworldplayerlili-0.0.1/setup.cfg
--rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      331 2023-04-18 14:57:41.000000 helloworldplayerlili-0.0.1/setup.py
+drwxrwxr-x   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 15:07:12.441287 helloworldplayerlili-0.0.2/
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)    35148 2023-04-18 12:58:47.000000 helloworldplayerlili-0.0.2/LICENSE
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      733 2023-04-18 15:07:12.441287 helloworldplayerlili-0.0.2/PKG-INFO
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      606 2023-04-18 14:59:24.000000 helloworldplayerlili-0.0.2/README.md
+drwxrwxr-x   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 15:07:12.437287 helloworldplayerlili-0.0.2/helloworldplayerlili/
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)       42 2023-04-18 12:52:36.000000 helloworldplayerlili-0.0.2/helloworldplayerlili/__init__.py
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 12:41:54.000000 helloworldplayerlili-0.0.2/helloworldplayerlili/lala.py
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      507 2023-04-18 12:52:22.000000 helloworldplayerlili-0.0.2/helloworldplayerlili/player.py
+drwxrwxr-x   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        0 2023-04-18 15:07:12.441287 helloworldplayerlili-0.0.2/helloworldplayerlili.egg-info/
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      733 2023-04-18 15:07:12.000000 helloworldplayerlili-0.0.2/helloworldplayerlili.egg-info/PKG-INFO
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      295 2023-04-18 15:07:12.000000 helloworldplayerlili-0.0.2/helloworldplayerlili.egg-info/SOURCES.txt
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)        1 2023-04-18 15:07:12.000000 helloworldplayerlili-0.0.2/helloworldplayerlili.egg-info/dependency_links.txt
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)       21 2023-04-18 15:07:12.000000 helloworldplayerlili-0.0.2/helloworldplayerlili.egg-info/top_level.txt
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)       38 2023-04-18 15:07:12.441287 helloworldplayerlili-0.0.2/setup.cfg
+-rw-rw-r--   0 liliana.loaiza (146958256) liliana.loaiza (146958256)      331 2023-04-18 14:59:48.000000 helloworldplayerlili-0.0.2/setup.py
```

### Comparing `helloworldplayerlili-0.0.1/LICENSE` & `helloworldplayerlili-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `helloworldplayerlili-0.0.1/PKG-INFO` & `helloworldplayerlili-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helloworldplayerlili
-Version: 0.0.1
+Version: 0.0.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Test Player
 This is a test player
 
 
@@ -28,12 +28,12 @@
 
 ## Package release
 ```
 # sdist = source distribution | bdist = build distribution
 > python3 setup.py sdist bdist_wheel
 
 # Check dist for invalid markup
-twine check dist/*
+> twine check dist/*
 
 # Upload dist
 > twine upload dist/*
 ```
```

### Comparing `helloworldplayerlili-0.0.1/README.md` & `helloworldplayerlili-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
 ## Package release
 ```
 # sdist = source distribution | bdist = build distribution
 > python3 setup.py sdist bdist_wheel
 
 # Check dist for invalid markup
-twine check dist/*
+> twine check dist/*
 
 # Upload dist
 > twine upload dist/*
 ```
```

### Comparing `helloworldplayerlili-0.0.1/helloworldplayerlili.egg-info/PKG-INFO` & `helloworldplayerlili-0.0.2/helloworldplayerlili.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helloworldplayerlili
-Version: 0.0.1
+Version: 0.0.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Test Player
 This is a test player
 
 
@@ -28,12 +28,12 @@
 
 ## Package release
 ```
 # sdist = source distribution | bdist = build distribution
 > python3 setup.py sdist bdist_wheel
 
 # Check dist for invalid markup
-twine check dist/*
+> twine check dist/*
 
 # Upload dist
 > twine upload dist/*
 ```
```

