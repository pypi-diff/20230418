# Comparing `tmp/nopea-0.0.8.tar.gz` & `tmp/nopea-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nopea-0.0.8.tar", last modified: Sun May 24 21:48:15 2020, max compression
+gzip compressed data, was "dist/nopea-0.0.9.tar", last modified: Sun May 31 09:04:38 2020, max compression
```

## Comparing `nopea-0.0.8.tar` & `nopea-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-24 21:48:15.490173 nopea-0.0.8/
--rw-rw-r--   0 christian  (1000) christian  (1000)       37 2020-05-02 15:45:49.000000 nopea-0.0.8/MANIFEST.in
--rw-rw-r--   0 christian  (1000) christian  (1000)     4368 2020-05-24 21:48:15.486173 nopea-0.0.8/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)     3191 2020-05-24 21:48:11.000000 nopea-0.0.8/README.md
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-24 21:48:15.486173 nopea-0.0.8/nopea/
--rw-rw-r--   0 christian  (1000) christian  (1000)       56 2020-05-02 15:45:49.000000 nopea-0.0.8/nopea/__init__.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-24 21:48:15.486173 nopea-0.0.8/nopea/adaptors/
--rw-rw-r--   0 christian  (1000) christian  (1000)        0 2020-05-02 15:45:49.000000 nopea-0.0.8/nopea/adaptors/__init__.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     9629 2020-05-24 21:15:04.000000 nopea-0.0.8/nopea/adaptors/mysql.py
--rw-rw-r--   0 christian  (1000) christian  (1000)    10097 2020-05-24 21:42:57.000000 nopea-0.0.8/nopea/adaptors/postgres.py
--rw-rw-r--   0 christian  (1000) christian  (1000)    10499 2020-05-24 21:15:04.000000 nopea-0.0.8/nopea/adaptors/sqlite.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     3856 2020-05-24 21:32:25.000000 nopea-0.0.8/nopea/dbobject.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      235 2020-05-02 15:45:49.000000 nopea-0.0.8/nopea/exceptions.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     4375 2020-05-24 21:15:04.000000 nopea-0.0.8/nopea/fields.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     2709 2020-05-23 21:35:27.000000 nopea-0.0.8/nopea/managers.py
--rw-rw-r--   0 christian  (1000) christian  (1000)    10495 2020-05-24 21:48:11.000000 nopea-0.0.8/nopea/migrations.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     6723 2020-05-24 21:15:04.000000 nopea-0.0.8/nopea/queryset.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-24 21:48:15.486173 nopea-0.0.8/nopea.egg-info/
--rw-rw-r--   0 christian  (1000) christian  (1000)     4368 2020-05-24 21:48:15.000000 nopea-0.0.8/nopea.egg-info/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)      502 2020-05-24 21:48:15.000000 nopea-0.0.8/nopea.egg-info/SOURCES.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        1 2020-05-24 21:48:15.000000 nopea-0.0.8/nopea.egg-info/dependency_links.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)       24 2020-05-24 21:48:15.000000 nopea-0.0.8/nopea.egg-info/requires.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        6 2020-05-24 21:48:15.000000 nopea-0.0.8/nopea.egg-info/top_level.txt
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-24 21:48:15.486173 nopea-0.0.8/scaffold/
--rw-rw-r--   0 christian  (1000) christian  (1000)        0 2020-05-02 15:45:49.000000 nopea-0.0.8/scaffold/__init__.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      784 2020-05-02 15:45:49.000000 nopea-0.0.8/scaffold/app.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      187 2020-05-02 15:45:49.000000 nopea-0.0.8/scaffold/migrations.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      378 2020-05-02 15:45:49.000000 nopea-0.0.8/scaffold/models.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      179 2020-05-02 15:45:49.000000 nopea-0.0.8/scaffold/shell.py
--rw-rw-r--   0 christian  (1000) christian  (1000)       38 2020-05-24 21:48:15.490173 nopea-0.0.8/setup.cfg
--rw-rw-r--   0 christian  (1000) christian  (1000)      615 2020-05-24 21:48:11.000000 nopea-0.0.8/setup.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-31 09:04:38.545693 nopea-0.0.9/
+-rw-rw-r--   0 christian  (1000) christian  (1000)       37 2020-05-02 15:45:49.000000 nopea-0.0.9/MANIFEST.in
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4368 2020-05-31 09:04:38.545693 nopea-0.0.9/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3191 2020-05-31 09:03:59.000000 nopea-0.0.9/README.md
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-31 09:04:38.545693 nopea-0.0.9/nopea/
+-rw-rw-r--   0 christian  (1000) christian  (1000)       56 2020-05-02 15:45:49.000000 nopea-0.0.9/nopea/__init__.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-31 09:04:38.545693 nopea-0.0.9/nopea/adaptors/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        0 2020-05-02 15:45:49.000000 nopea-0.0.9/nopea/adaptors/__init__.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     9629 2020-05-24 21:15:04.000000 nopea-0.0.9/nopea/adaptors/mysql.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    10097 2020-05-26 18:44:33.000000 nopea-0.0.9/nopea/adaptors/postgres.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    10499 2020-05-24 21:15:04.000000 nopea-0.0.9/nopea/adaptors/sqlite.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3951 2020-05-26 18:52:52.000000 nopea-0.0.9/nopea/dbobject.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      235 2020-05-02 15:45:49.000000 nopea-0.0.9/nopea/exceptions.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4536 2020-05-26 18:47:48.000000 nopea-0.0.9/nopea/fields.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2709 2020-05-23 21:35:27.000000 nopea-0.0.9/nopea/managers.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    10495 2020-05-24 21:48:11.000000 nopea-0.0.9/nopea/migrations.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     6723 2020-05-26 18:44:05.000000 nopea-0.0.9/nopea/queryset.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-31 09:04:38.545693 nopea-0.0.9/nopea.egg-info/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4368 2020-05-31 09:04:38.000000 nopea-0.0.9/nopea.egg-info/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      502 2020-05-31 09:04:38.000000 nopea-0.0.9/nopea.egg-info/SOURCES.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        1 2020-05-31 09:04:38.000000 nopea-0.0.9/nopea.egg-info/dependency_links.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)       24 2020-05-31 09:04:38.000000 nopea-0.0.9/nopea.egg-info/requires.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        6 2020-05-31 09:04:38.000000 nopea-0.0.9/nopea.egg-info/top_level.txt
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2020-05-31 09:04:38.545693 nopea-0.0.9/scaffold/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        0 2020-05-02 15:45:49.000000 nopea-0.0.9/scaffold/__init__.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      784 2020-05-02 15:45:49.000000 nopea-0.0.9/scaffold/app.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      187 2020-05-02 15:45:49.000000 nopea-0.0.9/scaffold/migrations.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      378 2020-05-02 15:45:49.000000 nopea-0.0.9/scaffold/models.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      179 2020-05-02 15:45:49.000000 nopea-0.0.9/scaffold/shell.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)       38 2020-05-31 09:04:38.545693 nopea-0.0.9/setup.cfg
+-rw-rw-r--   0 christian  (1000) christian  (1000)      615 2020-05-31 09:04:11.000000 nopea-0.0.9/setup.py
```

### Comparing `nopea-0.0.8/PKG-INFO` & `nopea-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nopea
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides an ORM for MySQL, PostgreSQL and SQLite.
 Home-page: UNKNOWN
 Author: Christian Kokoska
 Author-email: info@softcreate.de
 License: GPLv3
 Description: # Nopea
-        (Version 0.0.8)
+        (Version 0.0.9)
         
         ---
         ## Purpose
         Provides an ORM for MySQL, PostgreSQL and SQLite.
         
         ## Usage
```

### Comparing `nopea-0.0.8/README.md` & `nopea-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Nopea
-(Version 0.0.8)
+(Version 0.0.9)
 
 ---
 ## Purpose
 Provides an ORM for MySQL, PostgreSQL and SQLite.
 
 ## Usage
```

### Comparing `nopea-0.0.8/nopea/adaptors/mysql.py` & `nopea-0.0.9/nopea/adaptors/mysql.py`

 * *Files identical despite different names*

### Comparing `nopea-0.0.8/nopea/adaptors/postgres.py` & `nopea-0.0.9/nopea/adaptors/postgres.py`

 * *Files identical despite different names*

### Comparing `nopea-0.0.8/nopea/adaptors/sqlite.py` & `nopea-0.0.9/nopea/adaptors/sqlite.py`

 * *Files identical despite different names*

### Comparing `nopea-0.0.8/nopea/dbobject.py` & `nopea-0.0.9/nopea/dbobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-from nopea.fields import DbField, ForeignKey, PkField
+from nopea.fields import DbField, ForeignKey, PkField, ReverseLazy
 from nopea.managers import Manager
 from nopea.queryset import QuerySet
 
 
 class MetaType(type):
 
     def __init__(cls, name, bases, attrs):
@@ -62,14 +62,16 @@
 
     def get_settings(self):
         settings = {}
         for fieldname in self.fieldnames:
             value = getattr(self, fieldname)
             if isinstance(value, DbObject):
                 value = value.id
+            if isinstance(value, ReverseLazy):
+                value = value().id
             settings[fieldname] = value
         return settings
 
     @classmethod
     def create_table(cls, tablename=None):
         create_table_query = cls.adaptor.get_create_table_query(cls(), tablename)
         return cls.adaptor.execute_query(create_table_query[0], create_table_query[1])
```

### Comparing `nopea-0.0.8/nopea/fields.py` & `nopea-0.0.9/nopea/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
     def __init__(self):
         self.value = Unresolved()
 
     def make_value(self, value):
         self.value = value
 
+    def get_value(self):
+        return self.value
+
     def get_drop_column_query(self, base=None):
         # Must be a function for sqlite
         return self.adaptor.get_drop_column_query(self, base)
 
 
 class PkField(DbField):
 
@@ -128,14 +131,19 @@
                 self.value = reference_obj[0]
         else:
             self.value = ReverseLazy(value, self.reference_class)
 
     def __get__(self, instance, owner):
         return self
 
+    def get_value(self):
+        if self.lazy:
+            return self.value().id
+        return self.value
+
     @property
     def partial_create_table_query(self):
         return self.adaptor.get_foreignkey_field_create_query_base()
 
     @property
     def partial_create_table_query_extension(self):
         return self.adaptor.get_foreignkey_field_create_query_extension(self.reference_class)
```

### Comparing `nopea-0.0.8/nopea/managers.py` & `nopea-0.0.9/nopea/managers.py`

 * *Files identical despite different names*

### Comparing `nopea-0.0.8/nopea/migrations.py` & `nopea-0.0.9/nopea/migrations.py`

 * *Files identical despite different names*

### Comparing `nopea-0.0.8/nopea/queryset.py` & `nopea-0.0.9/nopea/queryset.py`

 * *Files identical despite different names*

### Comparing `nopea-0.0.8/nopea.egg-info/PKG-INFO` & `nopea-0.0.9/nopea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nopea
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides an ORM for MySQL, PostgreSQL and SQLite.
 Home-page: UNKNOWN
 Author: Christian Kokoska
 Author-email: info@softcreate.de
 License: GPLv3
 Description: # Nopea
-        (Version 0.0.8)
+        (Version 0.0.9)
         
         ---
         ## Purpose
         Provides an ORM for MySQL, PostgreSQL and SQLite.
         
         ## Usage
```

### Comparing `nopea-0.0.8/scaffold/app.py` & `nopea-0.0.9/scaffold/app.py`

 * *Files identical despite different names*

### Comparing `nopea-0.0.8/setup.py` & `nopea-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 setupargs = {
     'name': 'nopea',
     'description': 'Provides an ORM for MySQL, PostgreSQL and SQLite.',
 
     'license': 'GPLv3',
-    'version': '0.0.8',
+    'version': '0.0.9',
 
     'packages': ['nopea', 'nopea.adaptors'],
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
 
     'author': 'Christian Kokoska',
     'author_email': 'info@softcreate.de',
```

