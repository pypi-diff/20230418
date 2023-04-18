# Comparing `tmp/arrendatools_plantillas-2.0.0.tar.gz` & `tmp/arrendatools_plantillas-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools_plantillas-2.0.0.tar", last modified: Mon Apr 17 17:22:28 2023, max compression
+gzip compressed data, was "arrendatools_plantillas-2.1.0.tar", last modified: Tue Apr 18 17:48:28 2023, max compression
```

## Comparing `arrendatools_plantillas-2.0.0.tar` & `arrendatools_plantillas-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:22:28.655507 arrendatools_plantillas-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-17 17:22:28.655507 arrendatools_plantillas-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1201 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:22:28.655507 arrendatools_plantillas-2.0.0/arrendatools_plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:22:28.655507 arrendatools_plantillas-2.0.0/arrendatools_plantillas/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas/filters/formato_fecha.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas/filters/numero_a_palabras.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:22:28.655507 arrendatools_plantillas-2.0.0/arrendatools_plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-17 17:22:28.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      489 2023-04-17 17:22:28.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 17:22:28.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-17 17:22:28.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-17 17:22:28.000000 arrendatools_plantillas-2.0.0/arrendatools_plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-17 17:22:28.659507 arrendatools_plantillas-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-17 17:22:26.000000 arrendatools_plantillas-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:48:28.315572 arrendatools_plantillas-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-04-18 17:48:28.315572 arrendatools_plantillas-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:48:28.315572 arrendatools_plantillas-2.1.0/arrendatools_plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:48:28.315572 arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/fecha.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/formato_fecha.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/formato_numeros.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/numero_a_palabras.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:48:28.315572 arrendatools_plantillas-2.1.0/arrendatools_plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-04-18 17:48:28.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      581 2023-04-18 17:48:28.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 17:48:28.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-18 17:48:28.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-18 17:48:28.000000 arrendatools_plantillas-2.1.0/arrendatools_plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-18 17:48:28.315572 arrendatools_plantillas-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-04-18 17:48:25.000000 arrendatools_plantillas-2.1.0/setup.py
```

### Comparing `arrendatools_plantillas-2.0.0/LICENSE` & `arrendatools_plantillas-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-2.0.0/README.md` & `arrendatools_plantillas-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-2.0.0/arrendatools_plantillas/filters/formato_fecha.py` & `arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/formato_fecha.py`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-2.0.0/arrendatools_plantillas/filters/numero_a_palabras.py` & `arrendatools_plantillas-2.1.0/arrendatools_plantillas/filters/numero_a_palabras.py`

 * *Files identical despite different names*

