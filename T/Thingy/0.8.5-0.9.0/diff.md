# Comparing `tmp/Thingy-0.8.5.tar.gz` & `tmp/Thingy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Thingy-0.8.5.tar", last modified: Mon Jul  2 07:44:09 2018, max compression
+gzip compressed data, was "Thingy-0.9.0.tar", last modified: Tue Jun 28 19:49:05 2022, max compression
```

## Comparing `Thingy-0.8.5.tar` & `Thingy-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2018-07-02 07:44:09.000000 Thingy-0.8.5/
-drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2018-07-02 07:44:09.000000 Thingy-0.8.5/Thingy.egg-info/
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)       12 2018-07-02 07:44:08.000000 Thingy-0.8.5/Thingy.egg-info/requires.txt
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2017-02-10 18:23:44.000000 Thingy-0.8.5/Thingy.egg-info/not-zip-safe
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     3408 2018-07-02 07:44:08.000000 Thingy-0.8.5/Thingy.egg-info/PKG-INFO
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)        7 2018-07-02 07:44:08.000000 Thingy-0.8.5/Thingy.egg-info/top_level.txt
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)      217 2018-07-02 07:44:08.000000 Thingy-0.8.5/Thingy.egg-info/SOURCES.txt
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2018-07-02 07:44:08.000000 Thingy-0.8.5/Thingy.egg-info/dependency_links.txt
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)      783 2018-07-02 07:43:17.000000 Thingy-0.8.5/setup.py
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     2162 2018-07-02 07:43:05.000000 Thingy-0.8.5/README.rst
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     3408 2018-07-02 07:44:09.000000 Thingy-0.8.5/PKG-INFO
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)      178 2018-07-02 07:44:09.000000 Thingy-0.8.5/setup.cfg
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     5885 2018-07-02 07:43:05.000000 Thingy-0.8.5/thingy.py
+drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2022-06-28 19:49:05.958262 Thingy-0.9.0/
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     1105 2022-03-05 00:12:41.000000 Thingy-0.9.0/LICENSE
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     2940 2022-06-28 19:49:05.958262 Thingy-0.9.0/PKG-INFO
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     2469 2022-03-05 00:12:41.000000 Thingy-0.9.0/README.rst
+drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2022-06-28 19:49:05.958262 Thingy-0.9.0/Thingy.egg-info/
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     2940 2022-06-28 19:49:05.000000 Thingy-0.9.0/Thingy.egg-info/PKG-INFO
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)      196 2022-06-28 19:49:05.000000 Thingy-0.9.0/Thingy.egg-info/SOURCES.txt
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2022-06-28 19:49:05.000000 Thingy-0.9.0/Thingy.egg-info/dependency_links.txt
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2022-06-28 19:49:05.000000 Thingy-0.9.0/Thingy.egg-info/not-zip-safe
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)        7 2022-06-28 19:49:05.000000 Thingy-0.9.0/Thingy.egg-info/top_level.txt
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)      199 2022-06-28 19:49:05.959262 Thingy-0.9.0/setup.cfg
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)      741 2022-06-28 19:48:17.000000 Thingy-0.9.0/setup.py
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     5825 2022-06-28 19:40:40.000000 Thingy-0.9.0/thingy.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Thingy-0.8.5/Thingy.egg-info/PKG-INFO` & `Thingy-0.9.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,109 @@
-Metadata-Version: 1.1
-Name: Thingy
-Version: 0.8.5
-Summary: Dictionary as an object, that can have different views
-Home-page: https://github.com/numberly/thingy
-Author: Guillaume Gelin
-Author-email: ramnes@1000mercis.com
-License: MIT
-Description-Content-Type: UNKNOWN
-Description: ======
-        Thingy
-        ======
-        
-        .. image:: https://img.shields.io/pypi/v/thingy.svg
-           :target: https://pypi.python.org/pypi/Thingy
-        .. image:: https://img.shields.io/github/license/numberly/thingy.svg
-           :target: https://github.com/numberly/thingy/blob/master/LICENSE
-        .. image:: https://img.shields.io/travis/numberly/thingy.svg
-           :target: https://travis-ci.org/numberly/thingy
-        .. image:: https://img.shields.io/coveralls/numberly/thingy.svg
-           :target: https://coveralls.io/github/numberly/thingy
-        .. image:: https://readthedocs.org/projects/python-thingy/badge
-           :target: https://python-thingy.readthedocs.io
-        
-        |
-        
-        Dictionaries as objects, that can have different dictionary views!
-        
-        
-        Install
-        =======
-        
-        .. code-block:: sh
-        
-           $ pip install thingy
-        
-        
-        Examples
-        ========
-        
-        Dictionaries as objects...
-        --------------------------
-        
-        .. code-block:: python
-        
-           >>> class MyThingy(Thingy)
-           ...     @property
-           ...     def foobaz(self):
-           ...         return self.foo + self.baz
-        
-           >>> thingy = MyThingy({"foo": "bar", "baz": "qux"})
-           >>> thingy.foo
-           "bar"
-           >>> thingy.foobaz
-           "barqux"
-        
-           >>> thingy.foo = "BARRRR"
-           >>> thingy.view()
-           {"foo": "BARRRR", "baz": "qux"}
-        
-        
-        ...that can have different dictionary views!
-        --------------------------------------------
-        
-        .. code-block:: python
-        
-           >>> MyThingy.add_view(name="fooz", include=["foo", "foobaz"])
-           >>> MyThingy.add_view(name="no_foo", defaults=True, exclude="foo")
-        
-           >>> thingy = MyThingy({"foo": "bar", "baz": "qux"})
-           >>> thingy.view("fooz")
-           {"foo": "bar", "foobaz": "barqux"}
-           >>> thingy.view("no_foo")
-           {"baz": "qux"}
-        
-        
-        Why Thingy?
-        ===========
-        
-        Because it's much more enjoyable to write ``foo.bar`` than ``foo["bar"]``.
-        
-        Thingy is mainly meant to be used inside other libraries to provide abstractions
-        over dictionaries, which can be useful for writing ORMs or similar utilities.
-        
-        Thingy's views system is also particularly useful as-is when you intensively
-        manipulate dictionaries and often restrict those dictionaries to a few redundant
-        items.
-        
-        
-        Tests
-        =====
-        
-        To run Thingy tests:
-        
-        * install developers requirements with ``pip install -r requirements.txt``;
-        * run ``pytest``.
-        
-        
-        License
-        =======
-        
-        MIT
-        
-Platform: any
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+======
+Thingy
+======
+
+.. image:: https://img.shields.io/pypi/v/thingy.svg
+   :target: https://pypi.python.org/pypi/Thingy
+.. image:: https://img.shields.io/github/license/Refty/thingy.svg
+   :target: https://github.com/Refty/thingy/blob/master/LICENSE
+.. image:: https://img.shields.io/travis/Refty/thingy.svg
+   :target: https://travis-ci.org/Refty/thingy
+.. image:: https://img.shields.io/coveralls/Refty/thingy.svg
+   :target: https://coveralls.io/github/Refty/thingy
+.. image:: https://readthedocs.org/projects/python-thingy/badge
+   :target: https://python-thingy.readthedocs.io
+
+|
+
+Dictionaries as objects, that can have different dictionary views!
+
+
+Install
+=======
+
+.. code-block:: sh
+
+   $ pip install thingy
+
+
+Examples
+========
+
+Dictionaries as objects...
+--------------------------
+
+.. code-block:: python
+
+   >>> class MyThingy(Thingy)
+   ...     @property
+   ...     def foobaz(self):
+   ...         return self.foo + self.baz
+
+   >>> thingy = MyThingy({"foo": "bar", "baz": "qux"})
+   >>> thingy.foo
+   "bar"
+   >>> thingy.foobaz
+   "barqux"
+
+   >>> thingy.foo = "BARRRR"
+   >>> thingy.view()
+   {"foo": "BARRRR", "baz": "qux"}
+
+
+...that can have different dictionary views!
+--------------------------------------------
+
+.. code-block:: python
+
+   >>> MyThingy.add_view(name="fooz", include=["foo", "foobaz"])
+   >>> MyThingy.add_view(name="no_foo", defaults=True, exclude="foo")
+
+   >>> thingy = MyThingy({"foo": "bar", "baz": "qux"})
+   >>> thingy.view("fooz")
+   {"foo": "bar", "foobaz": "barqux"}
+   >>> thingy.view("no_foo")
+   {"baz": "qux"}
+
+
+Why Thingy?
+===========
+
+Because it's much more enjoyable to write ``foo.bar`` than ``foo["bar"]``.
+
+Thingy is mainly meant to be used inside other libraries to provide abstractions
+over dictionaries, which can be useful for writing ORMs or similar utilities.
+
+Thingy's views system is also particularly useful as-is when you intensively
+manipulate dictionaries and often restrict those dictionaries to a few redundant
+items.
+
+
+Tests
+=====
+
+To run Thingy tests:
+
+* install developers requirements with ``pip install -r requirements.txt``;
+* run ``pytest``.
+
+
+Sponsors
+========
+
+.. image:: https://raw.githubusercontent.com/Refty/thingy/master/img/numberly.png
+    :alt: Numberly
+    :align: center
+    :target: https://numberly.com/
+
+|
+
+.. image:: https://raw.githubusercontent.com/Refty/thingy/master/img/refty.png
+    :alt: Refty
+    :align: center
+    :target: https://refty.co/
+
+
+License
+=======
+
+MIT
```

### Comparing `Thingy-0.8.5/setup.py` & `Thingy-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 def get_description():
     with open("README.rst") as file:
         return file.read()
 
 
 setup(
     name="Thingy",
-    version="0.8.5",
-    url="https://github.com/numberly/thingy",
+    version="0.9.0",
+    url="https://github.com/Refty/thingy",
     license="MIT",
     author="Guillaume Gelin",
-    author_email="ramnes@1000mercis.com",
+    author_email="guillaume@refty.co",
     description="Dictionary as an object, that can have different views",
     long_description=get_description(),
     py_modules=["thingy"],
     include_package_data=True,
     zip_safe=False,
     platforms="any",
-    install_requires=["six>=1.10.0"],
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Topic :: Software Development :: Libraries :: Python Modules"
-    ]
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
 )
```

### Comparing `Thingy-0.8.5/thingy.py` & `Thingy-0.9.0/thingy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 import re
 from collections import OrderedDict
 
-import six
-
 
 class classproperty(property):
-
     def __init__(self, function):
         property.__init__(self, function)
         self.function_name = function.__name__
 
     def __get__(self, instance, cls):
         if instance:
             try:
                 return instance.__dict__[self.function_name]
             except KeyError:
-                raise AttributeError("'{}' object has no attribute '{}' "
-                                     "(but its class has!)"
-                                     .format(cls.__name__, self.function_name))
+                raise AttributeError(
+                    "'{}' object has no attribute '{}' (but its class has!)".format(
+                        cls.__name__, self.function_name
+                    )
+                )
         return self.fget(cls)
 
 
 class View(object):
     """Transform an :class:`object` into a dict
 
     :param bool defaults: Include attributes of object
     :param list include: A list of properties to include
     :param list exclude: A list of attributes to exclude
     :param bool ordered: Use an :class:`OrderedDict` instead
     """
 
-    def __init__(self, defaults=False, include=None, exclude=None,
-                 ordered=False):
+    def __init__(self, defaults=False, include=None, exclude=None, ordered=False):
         self.defaults = defaults
-        if isinstance(include, six.string_types):
+        if isinstance(include, str):
             include = [include]
         self.include = include or []
-        if isinstance(exclude, six.string_types):
+        if isinstance(exclude, str):
             exclude = [exclude]
         self.exclude = exclude or []
         self.ordered = ordered
 
     def __call__(self, thingy):
         if self.ordered:
             d = OrderedDict()
@@ -61,15 +59,14 @@
         return d
 
 
 registry = []
 
 
 class ThingyMetaClass(type):
-
     def __new__(cls, name, bases, attrs):
         attrs.setdefault("_views", {})
         klass = type.__new__(cls, name, bases, attrs)
         if "defaults" not in klass._views:
             klass.add_view("defaults", defaults=True)
         registry.append(klass)
         return klass
@@ -79,17 +76,17 @@
     for cls in type(instance).mro():
         try:
             return cls.__dict__[attr]
         except KeyError:
             pass
 
 
-@six.add_metaclass(ThingyMetaClass)
-class Thingy(object):
+class Thingy(object, metaclass=ThingyMetaClass):
     """Allows you to use object notation instead of dict notation"""
+
     _view_cls = View
     _silent = True
 
     def __init__(self, *args, **kwargs):
         self._update(*args, **kwargs)
 
     def __setattr__(self, attr, value):
@@ -128,15 +125,14 @@
         return self._views[name](self)
 
 
 names_regex = re.compile("([A-Z]+(?![a-z])|[A-Z][a-z]+)")
 
 
 class NamesMixin(object):
-
     @classmethod
     def get_names(cls):
         names = names_regex.findall(cls.__name__)
         return [name.lower() for name in names]
 
     @classproperty
     def names(cls):
```

