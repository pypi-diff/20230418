# Comparing `tmp/skip-pydjamodb-0.0.9.1.tar.gz` & `tmp/skip-pydjamodb-0.0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-pydjamodb-0.0.9.1.tar", last modified: Thu Jan 12 17:04:22 2023, max compression
+gzip compressed data, was "skip-pydjamodb-0.0.9.2.tar", last modified: Mon Jan 16 23:53:27 2023, max compression
```

## Comparing `skip-pydjamodb-0.0.9.1.tar` & `skip-pydjamodb-0.0.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:04:22.289690 skip-pydjamodb-0.0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-12 17:04:22.289690 skip-pydjamodb-0.0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:04:22.289690 skip-pydjamodb-0.0.9.1/pydjamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/pydjamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/pydjamodb/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/pydjamodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/pydjamodb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/pydjamodb/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/pydjamodb/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 17:04:22.289690 skip-pydjamodb-0.0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-01-12 17:04:12.000000 skip-pydjamodb-0.0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:04:22.289690 skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-12 17:04:22.000000 skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-12 17:04:22.000000 skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 17:04:22.000000 skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 17:04:22.000000 skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-12 17:04:22.000000 skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-12 17:04:22.000000 skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/pydjamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 23:53:26.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/top_level.txt
```

### Comparing `skip-pydjamodb-0.0.9.1/LICENSE` & `skip-pydjamodb-0.0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.1/PKG-INFO` & `skip-pydjamodb-0.0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-pydjamodb
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: Django interface to PyDjamoDB.
 Home-page: https://github.com/skip-pay/pydjamodb
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,DynamoDB,PyDjamoDB
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip-pydjamodb-0.0.9.1/README.md` & `skip-pydjamodb-0.0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.1/pydjamodb/attributes.py` & `skip-pydjamodb-0.0.9.2/pydjamodb/attributes.py`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.1/pydjamodb/connection.py` & `skip-pydjamodb-0.0.9.2/pydjamodb/connection.py`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.1/pydjamodb/models.py` & `skip-pydjamodb-0.0.9.2/pydjamodb/models.py`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.1/pydjamodb/queryset.py` & `skip-pydjamodb-0.0.9.2/pydjamodb/queryset.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,17 +175,17 @@
         elif operator == 'gte':
             return field >= value
         elif operator == 'between':
             return field.between(*value)
         elif operator == 'in':
             return field.is_in(value)
         elif operator == 'exists' and value:
-            return field.exists(value)
+            return field.exists()
         elif operator == 'exists' and not value:
-            return field.does_not_exist(value)
+            return field.does_not_exist()
         elif operator == 'startswith':
             return field.startswith(value)
         elif operator == 'contains':
             return field.contains(value)
         else:
             raise InvalidOperator('Invalid operator "{}"'.format(operator))
```

### Comparing `skip-pydjamodb-0.0.9.1/pydjamodb/test_runner.py` & `skip-pydjamodb-0.0.9.2/pydjamodb/test_runner.py`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.1/setup.py` & `skip-pydjamodb-0.0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='skip-pydjamodb',
-    version='0.0.9.1',
+    version='0.0.9.2',
     description="Django interface to PyDjamoDB.",
     keywords='django, DynamoDB, PyDjamoDB',
     author='Lubos Matl',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/pydjamodb',
     license='MIT',
     package_dir={'pydjamodb': 'pydjamodb'},
```

### Comparing `skip-pydjamodb-0.0.9.1/skip_pydjamodb.egg-info/PKG-INFO` & `skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-pydjamodb
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: Django interface to PyDjamoDB.
 Home-page: https://github.com/skip-pay/pydjamodb
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,DynamoDB,PyDjamoDB
 Classifier: Development Status :: 3 - Alpha
```

