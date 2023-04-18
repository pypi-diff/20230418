# Comparing `tmp/odoo_models_connect-0.1.3.tar.gz` & `tmp/odoo_models_connect-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_models_connect-0.1.3.tar", last modified: Mon Apr 17 14:15:11 2023, max compression
+gzip compressed data, was "odoo_models_connect-0.1.4.tar", last modified: Tue Apr 18 19:54:26 2023, max compression
```

## Comparing `odoo_models_connect-0.1.3.tar` & `odoo_models_connect-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-17 14:15:11.011876 odoo_models_connect-0.1.3/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     2829 2023-04-17 14:15:11.010402 odoo_models_connect-0.1.3/PKG-INFO
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     2461 2023-04-11 18:29:59.000000 odoo_models_connect-0.1.3/README.md
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-17 14:15:10.998460 odoo_models_connect-0.1.3/odoo_models_connect/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       72 2023-04-17 14:13:42.000000 odoo_models_connect-0.1.3/odoo_models_connect/__init__.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     5738 2023-04-11 18:31:41.000000 odoo_models_connect-0.1.3/odoo_models_connect/connect_odoo.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)      648 2023-04-12 11:53:38.000000 odoo_models_connect-0.1.3/odoo_models_connect/fields.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     3483 2023-04-17 14:13:28.000000 odoo_models_connect-0.1.3/odoo_models_connect/models.py
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-17 14:15:11.009488 odoo_models_connect-0.1.3/odoo_models_connect.egg-info/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     2829 2023-04-17 14:15:10.000000 odoo_models_connect-0.1.3/odoo_models_connect.egg-info/PKG-INFO
--rw-r--r--   0 lsvtech2022   (501) staff       (20)      360 2023-04-17 14:15:10.000000 odoo_models_connect-0.1.3/odoo_models_connect.egg-info/SOURCES.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)        1 2023-04-17 14:15:10.000000 odoo_models_connect-0.1.3/odoo_models_connect.egg-info/dependency_links.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       21 2023-04-17 14:15:10.000000 odoo_models_connect-0.1.3/odoo_models_connect.egg-info/requires.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       20 2023-04-17 14:15:10.000000 odoo_models_connect-0.1.3/odoo_models_connect.egg-info/top_level.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       38 2023-04-17 14:15:11.012727 odoo_models_connect-0.1.3/setup.cfg
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     1415 2023-04-17 14:15:02.000000 odoo_models_connect-0.1.3/setup.py
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-18 19:54:26.103304 odoo_models_connect-0.1.4/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4531 2023-04-18 19:54:26.102405 odoo_models_connect-0.1.4/PKG-INFO
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4163 2023-04-18 19:47:37.000000 odoo_models_connect-0.1.4/README.md
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-18 19:54:26.093304 odoo_models_connect-0.1.4/odoo_models_connect/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       72 2023-04-17 14:13:42.000000 odoo_models_connect-0.1.4/odoo_models_connect/__init__.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     5738 2023-04-11 18:31:41.000000 odoo_models_connect-0.1.4/odoo_models_connect/connect_odoo.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)      648 2023-04-12 11:53:38.000000 odoo_models_connect-0.1.4/odoo_models_connect/fields.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4080 2023-04-18 19:29:41.000000 odoo_models_connect-0.1.4/odoo_models_connect/models.py
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-18 19:54:26.100506 odoo_models_connect-0.1.4/odoo_models_connect.egg-info/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4531 2023-04-18 19:54:25.000000 odoo_models_connect-0.1.4/odoo_models_connect.egg-info/PKG-INFO
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)      360 2023-04-18 19:54:25.000000 odoo_models_connect-0.1.4/odoo_models_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)        1 2023-04-18 19:54:25.000000 odoo_models_connect-0.1.4/odoo_models_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       21 2023-04-18 19:54:25.000000 odoo_models_connect-0.1.4/odoo_models_connect.egg-info/requires.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       20 2023-04-18 19:54:25.000000 odoo_models_connect-0.1.4/odoo_models_connect.egg-info/top_level.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       38 2023-04-18 19:54:26.103589 odoo_models_connect-0.1.4/setup.cfg
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     1415 2023-04-18 19:48:49.000000 odoo_models_connect-0.1.4/setup.py
```

### Comparing `odoo_models_connect-0.1.3/PKG-INFO` & `odoo_models_connect-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,134 @@
-Metadata-Version: 2.1
-Name: odoo_models_connect
-Version: 0.1.3
-Summary: Library to improve interaction and communication with odoo for integration with other technologies.
-Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
-Author: Deiver Jose Vazquez Moreno
-Author-email: estudiandovazmore@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-
 # odoo-models-connect
 
 Odoo-Models-Connect is an library to improve interaction and communication with [Odoo](https://www.odoo.com/) XML-RPC [External API](https://www.odoo.com/documentation/15.0/webservices/odoo.html) for integration with other technologies.
 
 ## Installing
 
 Install and update using [pip](https://pypi.org/project/odoo-models-connect/):
 
 ```
 $ pip install odoo-models-connect
 ```
 
 ## Example
 
+Initialize the required environment variables
+
+1. Create an .env file
+2. places the environment variables inside the file with these names:
+
+   - DATABASE
+   - USERNAME
+   - PASSWORD
+   - URL
+
+3. import load_env_vars:
+
+   from odoo_models_connect import load_env_vars
+
+4. load environment variables:
+
+   ```
+   load_env_vars('path/to/environment')
+   ```
+
+   ##### NOTE: must end in .env
+
+You can create a high-level interface by declaring models by extending models.OdooModel as follows:
+
+```
+from odoo_models_connect import models, fields, load_env_vars
+
+
+load_env_vars(env_path='path/to/.env')
+
+
+class ResUsers(models.OdooModel):
+    _name = 'res.users'
+
+    name = fields.StringField()
+    login = fields.StringField()
+    password = fields.StringField()
+```
+
+##### NOTE: it is necessary to load the environment variables before doing the inheritance of OdooModel
+
+count of number of records:
+
+```
+>>> ResUsers.search_count()
+4
+```
+
+search and read record by id:
+
+```
+>>> ResUsers.search_by_id(2)
+<ResUsers id=2>
+```
+
+search and read records:
+
+```
+>>> ResUsers.search_read()
+[<ResUsers id=2>, <ResUsers id=6>, <ResUsers id=7>, <ResUsers id=8>]
+```
+
+create a record:
+
+```
+user = ResUsers(
+    name='John',
+    login='John@mail.com',
+    password='john123',
+)
+
+user.create()
+```
+
+update a record:
+
+```
+user = ResUsers(
+    id=8,
+    name='John2',
+    login='John2@mail.com',
+    password='john1234',
+)
+
+user.update()
+```
+
+delete a record:
+
+```
+user = ResUsers(id=10)
+
+user.delete()
+```
+
+### Allowed data types:
+
+- StringField
+- BooleanField
+- BinaryField
+- DateField
+- DateTimeField
+- IntegerField
+- FloatField
+- MonetaryField
+- Many2oneField
+- Many2manyField
+- One2manyField
+
+##
+
+## Other Features
+
 Initialize the odoo connection:
 
 ```
 from odoo_models_connect import ConnectOdoo
 
 odoo = ConnectOdoo('http://localhost:8069', 'db_name')
 ```
@@ -44,17 +147,15 @@
     "password": 'user_password',
     "uid": 7,
 }
 
 odoo.reconnect(session)
 ```
 
-
-## Making queries
-
+### Making queries
 
 To make a simple search of all the elements of a model is used:
 
 ```
 users = odoo.search_read('res.users')
 ```
 
@@ -71,15 +172,16 @@
 ```
 
 You can also bring only the fields that are needed:
 
 ```
 users = odoo.read('res.users', object_ids=[8, 25], fields=['name', 'login'])
 ```
-### NOTE: ids must be of type integer
+
+#### NOTE: ids must be of type integer
 
 You can fetch the id of all the elements of a model stored in a database:
 
 ```
 users_ids = odoo.search_ids('res.users')
 ```
 
@@ -119,8 +221,7 @@
 The delete() method is used to delete an element of a model in a database.
 
 ```
 user_id = 9
 
 odoo.delete('res.users', user_id)
 ```
-
```

### Comparing `odoo_models_connect-0.1.3/odoo_models_connect/connect_odoo.py` & `odoo_models_connect-0.1.4/odoo_models_connect/connect_odoo.py`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.3/odoo_models_connect/fields.py` & `odoo_models_connect-0.1.4/odoo_models_connect/fields.py`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.3/odoo_models_connect/models.py` & `odoo_models_connect-0.1.4/odoo_models_connect/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from dotenv import dotenv_values
 from abc import ABC, abstractmethod
 import os
 from dotenv import load_dotenv
 
 
 def load_env_vars(env_path):
-    """
-    Carga las variables de entorno desde el archivo .env en el directorio actual
-    """
+    if not os.path.exists(env_path):
+        raise FileNotFoundError(".env not found, wrong path")
     load_dotenv(env_path)
 
 
 class OdooModel(object):
     DATABASE = None
     USERNAME = None
     PASSWORD = None
@@ -35,14 +34,22 @@
             for name, value in kwargs.items():
                 setattr(self, name, value)
                 self.FIELDS[name] = value
 
     def __repr__(self):
         return f"<{self.__class__.__name__} id={self.id}>"
 
+    class DoesNotExist(Exception):
+
+        def __init__(self, obj_id):
+            self.id = obj_id
+
+        def __str__(self):
+            return f'Element by id {self.id} does not exist'
+
     @classmethod
     def search_read(cls, query=[], **kwargs):
         records = cls.MODELS.execute_kw(
             cls.DATABASE,
             cls.UUID,
             cls.PASSWORD,
             cls._name,
@@ -50,73 +57,86 @@
             [query],
             {'fields': list(cls.FIELDS.keys())}
         )
         instances = cls._instances_from_list(records)
         return instances
 
     @classmethod
+    def search_count(cls, query=[]):
+        records = cls.search_read(query=query)
+        return len(records)
+
+    @classmethod
+    def search_by_id(cls, obj_id=None):
+        if obj_id is None:
+            raise ValueError("id is required")
+        record = cls.search_read(query=[["id", '=', obj_id]])
+        if len(record) == 0:
+            raise cls.DoesNotExist(obj_id)
+        return record[0]
+
+    @classmethod
     def _instances_from_list(cls, records):
         return [cls._create_instance_from_dict(record) for record in records]
 
     @classmethod
     def _create_instance_from_dict(cls, obj):
         return cls(**obj)
 
     def create(self):
         return self.MODELS.execute_kw(self.DATABASE, self.UUID, self.PASSWORD, self._name, 'create', [self.FIELDS])
 
     def update(self):
-        print(self.FIELDS)
         return self.MODELS.execute_kw(self.DATABASE, self.UUID, self.PASSWORD, self._name, 'write', [[self.id], self.FIELDS])
 
     def delete(self):
         return self.MODELS.execute_kw(self.DATABASE, self.UUID, self.PASSWORD, self._name, 'unlink', [[self.id]])
 
     def __init_subclass__(cls):
         cls._set_config_envs()
         cls._fill_fields()
-        cls.set_attributes_initialized_none()
+        cls._set_attributes_initialized_none()
         super().__init_subclass__()
 
     @classmethod
-    def set_attributes_initialized_none(cls):
-        cls.set_models_attribute()
-        cls.set_uuid_attribute()
+    def _set_attributes_initialized_none(cls):
+        cls._set_models_attribute()
+        cls._set_uuid_attribute()
 
     @classmethod
     def _set_config_envs(cls):
         cls.DATABASE = os.getenv('DATABASE')
         cls.USERNAME = os.getenv('USERNAME')
         cls.PASSWORD = os.getenv('PASSWORD')
         cls.URL = os.getenv('URL')
 
     @classmethod
-    def set_uuid_attribute(cls):
+    def _set_uuid_attribute(cls):
         common = xmlrpc.client.ServerProxy('{}{}'.format(cls.URL, cls.COMMON))
         cls.UUID = common.authenticate(
             cls.DATABASE, cls.USERNAME, cls.PASSWORD, {})
 
     @classmethod
-    def set_models_attribute(cls):
+    def _set_models_attribute(cls):
         cls.MODELS = xmlrpc.client.ServerProxy(
             '{}{}'.format(cls.URL, cls.OBJECTS))
 
     @classmethod
     def _fill_fields(cls):
         cls.FIELDS = {}
-        cls.iterate_dir_class()
+        cls._iterate_dir_class()
 
     @classmethod
-    def iterate_dir_class(cls):
+    def _iterate_dir_class(cls):
         for attr_name in dir(cls):
             attr = cls._is_not_abstract_method_attribute(attr_name)
-            cls.add_field_if_is_odoo_field(attr, attr_name)
+            cls._add_field_if_is_odoo_field(attr, attr_name)
 
     @classmethod
-    def add_field_if_is_odoo_field(cls, attr, attr_name):
+    def _add_field_if_is_odoo_field(cls, attr, attr_name):
         if isinstance(attr, OdooField):
             cls.FIELDS[attr_name] = attr._type
 
     @classmethod
     def _is_not_abstract_method_attribute(cls, attr_name):
         if attr_name != '__abstractmethods__':
             return getattr(cls, attr_name)
```

### Comparing `odoo_models_connect-0.1.3/setup.py` & `odoo_models_connect-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.3'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.1.4'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 # Debe coincidir con el nombre de la carpeta
 PACKAGE_NAME = 'odoo_models_connect'
 AUTHOR = 'Deiver Jose Vazquez Moreno'  # Modificar con vuestros datos
 AUTHOR_EMAIL = 'estudiandovazmore@gmail.com'  # Modificar con vuestros datos
 # Modificar con vuestros datos
 URL = 'https://github.com/DeijoseDevelop/odoo_models_connect'
```

