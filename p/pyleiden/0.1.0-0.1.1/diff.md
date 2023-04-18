# Comparing `tmp/pyleiden-0.1.0.tar.gz` & `tmp/pyleiden-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleiden-0.1.0.tar", last modified: Tue Apr 18 02:12:28 2023, max compression
+gzip compressed data, was "pyleiden-0.1.1.tar", last modified: Tue Apr 18 02:16:15 2023, max compression
```

## Comparing `pyleiden-0.1.0.tar` & `pyleiden-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    32422 2023-03-30 22:21:28.913564 pyleiden-0.1.0/LICENSE
--rw-r--r--   0        0        0     7771 2023-04-18 02:10:30.853915 pyleiden-0.1.0/pyleiden/README.md
--rw-r--r--   0        0        0      123 2023-04-17 21:18:48.774050 pyleiden-0.1.0/pyleiden/__init__.py
--rw-r--r--   0        0        0     4354 2023-04-18 01:32:26.595206 pyleiden-0.1.0/pyleiden/pyleiden.py
--rw-r--r--   0        0        0      504 2023-04-17 23:44:07.548761 pyleiden-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 pyleiden-0.1.0/setup.py
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 pyleiden-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-03-30 22:21:28.913564 pyleiden-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7771 2023-04-18 02:10:30.853915 pyleiden-0.1.1/README.md
+-rw-r--r--   0        0        0      123 2023-04-18 02:15:29.883216 pyleiden-0.1.1/pyleiden/__init__.py
+-rw-r--r--   0        0        0     4354 2023-04-18 01:32:26.595206 pyleiden-0.1.1/pyleiden/pyleiden.py
+-rw-r--r--   0        0        0      525 2023-04-18 02:13:57.823782 pyleiden-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 pyleiden-0.1.1/setup.py
+-rw-r--r--   0        0        0     8170 1970-01-01 00:00:00.000000 pyleiden-0.1.1/PKG-INFO
```

### Comparing `pyleiden-0.1.0/LICENSE` & `pyleiden-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyleiden-0.1.0/pyleiden/README.md` & `pyleiden-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyleiden-0.1.0/pyleiden/pyleiden.py` & `pyleiden-0.1.1/pyleiden/pyleiden.py`

 * *Files identical despite different names*

### Comparing `pyleiden-0.1.0/setup.py` & `pyleiden-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = \
 ['igraph >=0.10.3']
 
 entry_points = \
 {'console_scripts': ['pyleiden = pyleiden.pyleiden:main']}
 
 setup(name='pyleiden',
-      version='0.1.0',
+      version='0.1.1',
       description='pyLeiden: a CLI tool for clustering with the Leiden algorithm',
       author=None,
       author_email='Antonio Camargo <antoniop.camargo@gmail.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

