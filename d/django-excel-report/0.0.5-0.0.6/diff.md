# Comparing `tmp/django_excel_report-0.0.5.tar.gz` & `tmp/django_excel_report-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_excel_report-0.0.5.tar", last modified: Tue Apr 18 12:26:13 2023, max compression
+gzip compressed data, was "django_excel_report-0.0.6.tar", last modified: Tue Apr 18 13:08:51 2023, max compression
```

## Comparing `django_excel_report-0.0.5.tar` & `django_excel_report-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 12:26:13.537238 django_excel_report-0.0.5/
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     3409 2023-04-17 11:26:32.000000 django_excel_report-0.0.5/LICENSE
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1840 2023-04-18 12:26:13.537238 django_excel_report-0.0.5/PKG-INFO
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1100 2023-04-17 13:59:12.000000 django_excel_report-0.0.5/README.md
-drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 12:26:13.537238 django_excel_report-0.0.5/django_excel_report/
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)      160 2023-04-17 09:44:59.000000 django_excel_report-0.0.5/django_excel_report/__init__.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       39 2023-04-13 14:47:05.000000 django_excel_report-0.0.5/django_excel_report/error.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1426 2023-04-17 13:59:12.000000 django_excel_report-0.0.5/django_excel_report/report.py
-drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 12:26:13.537238 django_excel_report-0.0.5/django_excel_report/writer/
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       63 2023-04-17 08:21:06.000000 django_excel_report-0.0.5/django_excel_report/writer/__init__.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1527 2023-04-18 12:24:36.000000 django_excel_report-0.0.5/django_excel_report/writer/accessors.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     4132 2023-04-17 13:59:12.000000 django_excel_report-0.0.5/django_excel_report/writer/acessors_builder.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1192 2023-04-13 17:43:59.000000 django_excel_report-0.0.5/django_excel_report/writer/get_queryset_builder.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1209 2023-04-17 08:21:06.000000 django_excel_report-0.0.5/django_excel_report/writer/report_meta.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     2416 2023-04-17 13:59:12.000000 django_excel_report-0.0.5/django_excel_report/writer/writer.py
-drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 12:26:13.537238 django_excel_report-0.0.5/django_excel_report.egg-info/
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1840 2023-04-18 12:26:13.000000 django_excel_report-0.0.5/django_excel_report.egg-info/PKG-INFO
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)      728 2023-04-18 12:26:13.000000 django_excel_report-0.0.5/django_excel_report.egg-info/SOURCES.txt
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)        1 2023-04-18 12:26:13.000000 django_excel_report-0.0.5/django_excel_report.egg-info/dependency_links.txt
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)        1 2023-04-18 12:25:41.000000 django_excel_report-0.0.5/django_excel_report.egg-info/not-zip-safe
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       18 2023-04-18 12:26:13.000000 django_excel_report-0.0.5/django_excel_report.egg-info/requires.txt
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       20 2023-04-18 12:26:13.000000 django_excel_report-0.0.5/django_excel_report.egg-info/top_level.txt
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       38 2023-04-18 12:26:13.537238 django_excel_report-0.0.5/setup.cfg
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1161 2023-04-18 12:26:05.000000 django_excel_report-0.0.5/setup.py
-drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 12:26:13.537238 django_excel_report-0.0.5/tests/
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1997 2023-04-17 08:21:06.000000 django_excel_report-0.0.5/tests/test_base_report_attributes.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1279 2023-04-17 08:21:06.000000 django_excel_report-0.0.5/tests/test_related_processors.py
--rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)      872 2023-04-17 08:21:06.000000 django_excel_report-0.0.5/tests/test_report_get_row.py
+drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 13:08:51.089928 django_excel_report-0.0.6/
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     3409 2023-04-17 11:26:32.000000 django_excel_report-0.0.6/LICENSE
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1840 2023-04-18 13:08:51.089928 django_excel_report-0.0.6/PKG-INFO
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1100 2023-04-17 13:59:12.000000 django_excel_report-0.0.6/README.md
+drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 13:08:51.085928 django_excel_report-0.0.6/django_excel_report/
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)      160 2023-04-17 09:44:59.000000 django_excel_report-0.0.6/django_excel_report/__init__.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       39 2023-04-13 14:47:05.000000 django_excel_report-0.0.6/django_excel_report/error.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1426 2023-04-17 13:59:12.000000 django_excel_report-0.0.6/django_excel_report/report.py
+drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 13:08:51.085928 django_excel_report-0.0.6/django_excel_report/writer/
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       63 2023-04-17 08:21:06.000000 django_excel_report-0.0.6/django_excel_report/writer/__init__.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1708 2023-04-18 12:59:34.000000 django_excel_report-0.0.6/django_excel_report/writer/accessors.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     4132 2023-04-17 13:59:12.000000 django_excel_report-0.0.6/django_excel_report/writer/acessors_builder.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1192 2023-04-13 17:43:59.000000 django_excel_report-0.0.6/django_excel_report/writer/get_queryset_builder.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1209 2023-04-17 08:21:06.000000 django_excel_report-0.0.6/django_excel_report/writer/report_meta.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     2416 2023-04-17 13:59:12.000000 django_excel_report-0.0.6/django_excel_report/writer/writer.py
+drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 13:08:51.085928 django_excel_report-0.0.6/django_excel_report.egg-info/
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1840 2023-04-18 13:08:51.000000 django_excel_report-0.0.6/django_excel_report.egg-info/PKG-INFO
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)      758 2023-04-18 13:08:51.000000 django_excel_report-0.0.6/django_excel_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)        1 2023-04-18 13:08:51.000000 django_excel_report-0.0.6/django_excel_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)        1 2023-04-18 13:08:23.000000 django_excel_report-0.0.6/django_excel_report.egg-info/not-zip-safe
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       18 2023-04-18 13:08:51.000000 django_excel_report-0.0.6/django_excel_report.egg-info/requires.txt
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       20 2023-04-18 13:08:51.000000 django_excel_report-0.0.6/django_excel_report.egg-info/top_level.txt
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)       38 2023-04-18 13:08:51.089928 django_excel_report-0.0.6/setup.cfg
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1161 2023-04-18 13:08:39.000000 django_excel_report-0.0.6/setup.py
+drwxrwxr-x   0 borisalekseev  (1000) borisalekseev  (1000)        0 2023-04-18 13:08:51.089928 django_excel_report-0.0.6/tests/
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1997 2023-04-17 08:21:06.000000 django_excel_report-0.0.6/tests/test_base_report_attributes.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1486 2023-04-18 13:02:47.000000 django_excel_report-0.0.6/tests/test_get_values_list.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)     1279 2023-04-17 08:21:06.000000 django_excel_report-0.0.6/tests/test_related_processors.py
+-rw-rw-r--   0 borisalekseev  (1000) borisalekseev  (1000)      872 2023-04-17 08:21:06.000000 django_excel_report-0.0.6/tests/test_report_get_row.py
```

### Comparing `django_excel_report-0.0.5/LICENSE` & `django_excel_report-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/PKG-INFO` & `django_excel_report-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_excel_report
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simplify excel reports from django apps
 Author: Boris Alekseev
 Author-email: i.borisalekseev@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Project-URL: Source, https://github.com/dichem/django-excel-report
```

### Comparing `django_excel_report-0.0.5/README.md` & `django_excel_report-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/django_excel_report/report.py` & `django_excel_report-0.0.6/django_excel_report/report.py`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/django_excel_report/writer/accessors.py` & `django_excel_report-0.0.6/django_excel_report/writer/accessors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Iterator, Iterable
+from typing import Callable, Iterator, Generator
 
 from django.db.models import Model
 
 
 def get_field(field: str) -> Callable:
     def func(self, obj: Model, from_iterator=False):
         if from_iterator:
@@ -22,29 +22,31 @@
     def func(self, obj: Model, from_iterator=False) -> Callable:
         # if fk is null, get_field anyway returns empty string
         return other_func(self, getattr(obj, field, ""), from_iterator)
     return func
 
 
 def get_values_list(func):
-    def wrapper(self, obj=None, result=None):
+    def wrapper(self, obj=None, result=None, recursive_call=False):
         values_list = []
         if obj:
             result = func(self, obj)
 
-        if not isinstance(result, Iterable):
-            values_list.append(str(result))
+        if not isinstance(result, (list, Generator)):
+            if result is not None:
+                values_list.append(str(result))
 
         else:
             for entity in result:
-                if not isinstance(entity, Iterable):
+                if not isinstance(entity, (list, Generator)) and entity is not None:
                     values_list.append(str(entity))
                 else:
-                    values_list.extend(wrapper(self, result=entity))
-
+                    values_list.extend(wrapper(self, result=entity, recursive_call=True))
+        if recursive_call:
+            return values_list
         return values_list or [""]
 
     return wrapper
 
 
 class Accessors:
     FIELD = get_field
```

### Comparing `django_excel_report-0.0.5/django_excel_report/writer/acessors_builder.py` & `django_excel_report-0.0.6/django_excel_report/writer/acessors_builder.py`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/django_excel_report/writer/get_queryset_builder.py` & `django_excel_report-0.0.6/django_excel_report/writer/get_queryset_builder.py`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/django_excel_report/writer/report_meta.py` & `django_excel_report-0.0.6/django_excel_report/writer/report_meta.py`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/django_excel_report/writer/writer.py` & `django_excel_report-0.0.6/django_excel_report/writer/writer.py`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/django_excel_report.egg-info/PKG-INFO` & `django_excel_report-0.0.6/django_excel_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-excel-report
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simplify excel reports from django apps
 Author: Boris Alekseev
 Author-email: i.borisalekseev@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Project-URL: Source, https://github.com/dichem/django-excel-report
```

### Comparing `django_excel_report-0.0.5/django_excel_report.egg-info/SOURCES.txt` & `django_excel_report-0.0.6/django_excel_report.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 django_excel_report/writer/__init__.py
 django_excel_report/writer/accessors.py
 django_excel_report/writer/acessors_builder.py
 django_excel_report/writer/get_queryset_builder.py
 django_excel_report/writer/report_meta.py
 django_excel_report/writer/writer.py
 tests/test_base_report_attributes.py
+tests/test_get_values_list.py
 tests/test_related_processors.py
 tests/test_report_get_row.py
```

### Comparing `django_excel_report-0.0.5/setup.py` & `django_excel_report-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
```

### Comparing `django_excel_report-0.0.5/tests/test_base_report_attributes.py` & `django_excel_report-0.0.6/tests/test_base_report_attributes.py`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/tests/test_related_processors.py` & `django_excel_report-0.0.6/tests/test_related_processors.py`

 * *Files identical despite different names*

### Comparing `django_excel_report-0.0.5/tests/test_report_get_row.py` & `django_excel_report-0.0.6/tests/test_report_get_row.py`

 * *Files identical despite different names*

