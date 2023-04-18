# Comparing `tmp/failSafePackage-0.0.3.tar.gz` & `tmp/failSafePackage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "failSafePackage-0.0.3.tar", last modified: Tue Apr 18 11:07:24 2023, max compression
+gzip compressed data, was "failSafePackage-0.0.4.tar", last modified: Tue Apr 18 13:06:45 2023, max compression
```

## Comparing `failSafePackage-0.0.3.tar` & `failSafePackage-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:07:23.999137 failSafePackage-0.0.3/
--rw-rw-rw-   0        0        0        0 2023-04-18 10:28:08.000000 failSafePackage-0.0.3/Licence.txt
--rw-rw-rw-   0        0        0      188 2023-04-18 11:07:23.998136 failSafePackage-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 11:07:23.954150 failSafePackage-0.0.3/failSafePackage/
--rw-rw-rw-   0        0        0        0 2023-04-18 10:28:45.000000 failSafePackage-0.0.3/failSafePackage/__init__.py
--rw-rw-rw-   0        0        0     1472 2023-04-18 11:00:44.000000 failSafePackage-0.0.3/failSafePackage/fail_safe_validation.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:07:23.992136 failSafePackage-0.0.3/failSafePackage.egg-info/
--rw-rw-rw-   0        0        0      188 2023-04-18 11:07:23.000000 failSafePackage-0.0.3/failSafePackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-04-18 11:07:23.000000 failSafePackage-0.0.3/failSafePackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:07:23.000000 failSafePackage-0.0.3/failSafePackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 11:07:23.000000 failSafePackage-0.0.3/failSafePackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-18 11:07:23.000000 failSafePackage-0.0.3/failSafePackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 11:07:24.001137 failSafePackage-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      315 2023-04-18 11:07:09.000000 failSafePackage-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:06:45.146598 failSafePackage-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-04-18 10:28:08.000000 failSafePackage-0.0.4/Licence.txt
+-rw-rw-rw-   0        0        0      188 2023-04-18 13:06:45.145598 failSafePackage-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 13:06:45.113598 failSafePackage-0.0.4/failSafePackage/
+-rw-rw-rw-   0        0        0        0 2023-04-18 10:28:45.000000 failSafePackage-0.0.4/failSafePackage/__init__.py
+-rw-rw-rw-   0        0        0     1472 2023-04-18 11:00:44.000000 failSafePackage-0.0.4/failSafePackage/fail_safe_validation.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:06:45.140612 failSafePackage-0.0.4/failSafePackage.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-04-18 13:06:44.000000 failSafePackage-0.0.4/failSafePackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-04-18 13:06:44.000000 failSafePackage-0.0.4/failSafePackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:06:44.000000 failSafePackage-0.0.4/failSafePackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 13:06:44.000000 failSafePackage-0.0.4/failSafePackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 13:06:44.000000 failSafePackage-0.0.4/failSafePackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 13:06:45.147599 failSafePackage-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      323 2023-04-18 13:06:36.000000 failSafePackage-0.0.4/setup.py
```

### Comparing `failSafePackage-0.0.3/failSafePackage/fail_safe_validation.py` & `failSafePackage-0.0.4/failSafePackage/fail_safe_validation.py`

 * *Files identical despite different names*

