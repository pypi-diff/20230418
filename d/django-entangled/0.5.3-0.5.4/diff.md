# Comparing `tmp/django-entangled-0.5.3.tar.gz` & `tmp/django-entangled-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-entangled-0.5.3.tar", last modified: Wed Feb 16 11:43:20 2022, max compression
+gzip compressed data, was "django-entangled-0.5.4.tar", last modified: Tue Apr 18 09:35:26 2023, max compression
```

## Comparing `django-entangled-0.5.3.tar` & `django-entangled-0.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:43:20.644945 django-entangled-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-16 11:43:09.000000 django-entangled-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-02-16 11:43:09.000000 django-entangled-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9700 2022-02-16 11:43:20.644945 django-entangled-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-02-16 11:43:09.000000 django-entangled-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:43:20.644945 django-entangled-0.5.3/django_entangled.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9700 2022-02-16 11:43:20.000000 django-entangled-0.5.3/django_entangled.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-02-16 11:43:20.000000 django-entangled-0.5.3/django_entangled.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 11:43:20.000000 django-entangled-0.5.3/django_entangled.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 11:43:19.000000 django-entangled-0.5.3/django_entangled.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-16 11:43:20.000000 django-entangled-0.5.3/django_entangled.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-16 11:43:20.000000 django-entangled-0.5.3/django_entangled.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:43:20.644945 django-entangled-0.5.3/entangled/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-16 11:43:09.000000 django-entangled-0.5.3/entangled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7313 2022-02-16 11:43:09.000000 django-entangled-0.5.3/entangled/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-02-16 11:43:09.000000 django-entangled-0.5.3/entangled/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-16 11:43:20.644945 django-entangled-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-02-16 11:43:09.000000 django-entangled-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:43:20.644945 django-entangled-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 11:43:09.000000 django-entangled-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-02-16 11:43:09.000000 django-entangled-0.5.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-02-16 11:43:09.000000 django-entangled-0.5.3/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-02-16 11:43:09.000000 django-entangled-0.5.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     8689 2022-02-16 11:43:09.000000 django-entangled-0.5.3/tests/test_entangled.py
--rw-r--r--   0 runner    (1001) docker     (121)     6771 2022-02-16 11:43:09.000000 django-entangled-0.5.3/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (121)     5002 2022-02-16 11:43:09.000000 django-entangled-0.5.3/tests/test_retangled.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:35:26.967570 django-entangled-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-18 09:35:15.000000 django-entangled-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 09:35:15.000000 django-entangled-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-18 09:35:26.967570 django-entangled-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-04-18 09:35:15.000000 django-entangled-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:35:26.967570 django-entangled-0.5.4/django_entangled.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-18 09:35:26.000000 django-entangled-0.5.4/django_entangled.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-18 09:35:26.000000 django-entangled-0.5.4/django_entangled.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:35:26.000000 django-entangled-0.5.4/django_entangled.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:35:26.000000 django-entangled-0.5.4/django_entangled.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 09:35:26.000000 django-entangled-0.5.4/django_entangled.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 09:35:26.000000 django-entangled-0.5.4/django_entangled.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:35:26.967570 django-entangled-0.5.4/entangled/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 09:35:15.000000 django-entangled-0.5.4/entangled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-18 09:35:15.000000 django-entangled-0.5.4/entangled/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-18 09:35:15.000000 django-entangled-0.5.4/entangled/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:35:26.967570 django-entangled-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-18 09:35:15.000000 django-entangled-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:35:26.967570 django-entangled-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:35:15.000000 django-entangled-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-18 09:35:15.000000 django-entangled-0.5.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-18 09:35:15.000000 django-entangled-0.5.4/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-18 09:35:15.000000 django-entangled-0.5.4/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-18 09:35:15.000000 django-entangled-0.5.4/tests/test_entangled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-18 09:35:15.000000 django-entangled-0.5.4/tests/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-18 09:35:15.000000 django-entangled-0.5.4/tests/test_retangled.py
```

### Comparing `django-entangled-0.5.3/LICENSE` & `django-entangled-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-entangled-0.5.3/PKG-INFO` & `django-entangled-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-entangled
-Version: 0.5.3
+Version: 0.5.4
 Summary: Edit JSON field using Django Model Form
 Home-page: https://github.com/jrief/django-entangled
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,JSON
 Platform: OS Independent
@@ -16,17 +16,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-entangled
 
 Edit JSON-Model Fields using a Standard Django Form.
 
@@ -216,10 +219,17 @@
 rather than digging through data.
 
 Foreign keys are stored as `"fieldname": {"model": "appname.modelname", "pk": 1234}` in our JSON field, meaning that
 we have no database constraints. If a target object is deleted, that foreign key points to nowhere. Therefore always
 keep in mind, that we don't have any referential integrity and hence must write our code in a defensive manner.
 
 
-[![Twitter Follow](https://img.shields.io/twitter/follow/jacobrief?style=social)](https://twitter.com/jacobrief)
+## Contributing to the Project
+
+* Please ask question on the [discussion board](https://github.com/jrief/django-entangled/discussions).
+* Ideas for new features shall as well be discussed on that board.
+* The [issue tracker](https://github.com/jrief/django-entangled/issues) shall *exclusively* be used to report bugs.
+* Except for very small fixes (typos etc.), do not open a pull request without an issue.
+* Before writing code, adopt your IDE to respect the project's [.editorconfig](https://github.com/jrief/django-entangled/blob/master/.editorconfig).
 
 
+[![Twitter Follow](https://img.shields.io/twitter/follow/jacobrief?style=social)](https://twitter.com/jacobrief)
```

### Comparing `django-entangled-0.5.3/README.md` & `django-entangled-0.5.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -188,8 +188,17 @@
 rather than digging through data.
 
 Foreign keys are stored as `"fieldname": {"model": "appname.modelname", "pk": 1234}` in our JSON field, meaning that
 we have no database constraints. If a target object is deleted, that foreign key points to nowhere. Therefore always
 keep in mind, that we don't have any referential integrity and hence must write our code in a defensive manner.
 
 
+## Contributing to the Project
+
+* Please ask question on the [discussion board](https://github.com/jrief/django-entangled/discussions).
+* Ideas for new features shall as well be discussed on that board.
+* The [issue tracker](https://github.com/jrief/django-entangled/issues) shall *exclusively* be used to report bugs.
+* Except for very small fixes (typos etc.), do not open a pull request without an issue.
+* Before writing code, adopt your IDE to respect the project's [.editorconfig](https://github.com/jrief/django-entangled/blob/master/.editorconfig).
+
+
 [![Twitter Follow](https://img.shields.io/twitter/follow/jacobrief?style=social)](https://twitter.com/jacobrief)
```

### Comparing `django-entangled-0.5.3/django_entangled.egg-info/PKG-INFO` & `django-entangled-0.5.4/django_entangled.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-entangled
-Version: 0.5.3
+Version: 0.5.4
 Summary: Edit JSON field using Django Model Form
 Home-page: https://github.com/jrief/django-entangled
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,JSON
 Platform: OS Independent
@@ -16,17 +16,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-entangled
 
 Edit JSON-Model Fields using a Standard Django Form.
 
@@ -216,10 +219,17 @@
 rather than digging through data.
 
 Foreign keys are stored as `"fieldname": {"model": "appname.modelname", "pk": 1234}` in our JSON field, meaning that
 we have no database constraints. If a target object is deleted, that foreign key points to nowhere. Therefore always
 keep in mind, that we don't have any referential integrity and hence must write our code in a defensive manner.
 
 
-[![Twitter Follow](https://img.shields.io/twitter/follow/jacobrief?style=social)](https://twitter.com/jacobrief)
+## Contributing to the Project
+
+* Please ask question on the [discussion board](https://github.com/jrief/django-entangled/discussions).
+* Ideas for new features shall as well be discussed on that board.
+* The [issue tracker](https://github.com/jrief/django-entangled/issues) shall *exclusively* be used to report bugs.
+* Except for very small fixes (typos etc.), do not open a pull request without an issue.
+* Before writing code, adopt your IDE to respect the project's [.editorconfig](https://github.com/jrief/django-entangled/blob/master/.editorconfig).
 
 
+[![Twitter Follow](https://img.shields.io/twitter/follow/jacobrief?style=social)](https://twitter.com/jacobrief)
```

### Comparing `django-entangled-0.5.3/entangled/forms.py` & `django-entangled-0.5.4/entangled/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         else:
             untangled_fields, entangled_fields, retangled_fields = [], {}, {}
         if entangled_fields:
             fieldset = set(getattr(attrs['Meta'], 'fields', []))
             fieldset.update(untangled_fields)
             fieldset.update(entangled_fields.keys())
             attrs['Meta'].fields = list(fieldset)
-            attrs['formfield_callback'] = formfield_callback
+            attrs['formfield_callback'] = formfield_callback  # Django up to 4.1
+            attrs['Meta'].formfield_callback = formfield_callback  # Django 4.2 +
         new_class = super().__new__(cls, class_name, bases, attrs)
 
         # perform some model checks
         for modelfield_name in entangled_fields.keys():
             for field_name in entangled_fields[modelfield_name]:
                 assert field_name in new_class.base_fields, \
                     "Field {} listed in `{}.Meta.entangled_fields['{}']` is missing in Form declaration" \
```

### Comparing `django-entangled-0.5.3/entangled/utils.py` & `django-entangled-0.5.4/entangled/utils.py`

 * *Files identical despite different names*

### Comparing `django-entangled-0.5.3/setup.py` & `django-entangled-0.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,20 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
+    'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
 ]
 
 setup(
     name='django-entangled',
     version=__version__,
     description='Edit JSON field using Django Model Form',
     author='Jacob Rief',
```

### Comparing `django-entangled-0.5.3/tests/settings.py` & `django-entangled-0.5.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-entangled-0.5.3/tests/test_entangled.py` & `django-entangled-0.5.4/tests/test_entangled.py`

 * *Files identical despite different names*

### Comparing `django-entangled-0.5.3/tests/test_inheritance.py` & `django-entangled-0.5.4/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `django-entangled-0.5.3/tests/test_retangled.py` & `django-entangled-0.5.4/tests/test_retangled.py`

 * *Files identical despite different names*

