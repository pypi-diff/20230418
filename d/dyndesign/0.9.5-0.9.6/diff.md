# Comparing `tmp/dyndesign-0.9.5.tar.gz` & `tmp/dyndesign-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyndesign-0.9.5.tar", max compression
+gzip compressed data, was "dyndesign-0.9.6.tar", max compression
```

## Comparing `dyndesign-0.9.5.tar` & `dyndesign-0.9.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    12777 2022-12-29 08:45:04.154594 dyndesign-0.9.5/README.rst
--rw-r--r--   0        0        0      172 2022-12-29 08:45:04.154594 dyndesign-0.9.5/dyndesign/__init__.py
--rw-r--r--   0        0        0     6038 2022-12-29 08:45:04.154594 dyndesign-0.9.5/dyndesign/classmerger.py
--rw-r--r--   0        0        0      643 2022-12-29 08:45:04.154594 dyndesign-0.9.5/dyndesign/dynloader.py
--rw-r--r--   0        0        0     5948 2022-12-29 08:45:04.154594 dyndesign-0.9.5/dyndesign/dynmethod.py
--rw-r--r--   0        0        0     1512 2022-12-29 08:45:04.154594 dyndesign-0.9.5/dyndesign/singletonmeta.py
--rw-r--r--   0        0        0     1160 2022-12-29 08:45:04.154594 dyndesign-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    13878 1970-01-01 00:00:00.000000 dyndesign-0.9.5/setup.py
--rw-r--r--   0        0        0    14139 1970-01-01 00:00:00.000000 dyndesign-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    12892 2023-04-18 10:57:56.029367 dyndesign-0.9.6/README.rst
+-rw-r--r--   0        0        0      172 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/__init__.py
+-rw-r--r--   0        0        0     7465 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/classmerger.py
+-rw-r--r--   0        0        0      643 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/dynloader.py
+-rw-r--r--   0        0        0     5948 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/dynmethod.py
+-rw-r--r--   0        0        0     1512 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/singletonmeta.py
+-rw-r--r--   0        0        0     1160 2023-04-18 10:57:56.029367 dyndesign-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    14254 1970-01-01 00:00:00.000000 dyndesign-0.9.6/PKG-INFO
```

### Comparing `dyndesign-0.9.5/README.rst` & `dyndesign-0.9.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     # Method `m2` of class `Base`
 
 
 When a merged class is instantiated with arguments, the constructor of each
 merging class is invoked, since constructors are excluded from being overloaded.
 Also, arguments passed to each constructor are adaptively filtered based on the
 constructor signature so that each constructor takes just the arguments it
-requires, and no exception is raised for the exceeding arguments passed:
+requires, and no exception is raised for exceeding or missing arguments passed:
 
 .. code:: python
 
     class A:
         def __init__(self):
             print("No argument passed to class `A`")
 
@@ -137,14 +137,19 @@
     MergedClass("Alpha", "Beta", kw1="kwarg #1", kw2="kwarg #2")
 
     # No argument passed to class `A`
     # Argument a='Alpha' passed to class `B`
     # Argument a='Alpha', b='Beta' and kw1='kwarg #1' passed to class `C`
     # Argument kw2='kwarg #2' passed to class `D`
 
+    MergedClass()
+
+    # No argument passed to class `A`
+    # Argument kw2='kwarg #2' passed to class `D`
+
 
 It is also possible to extend the same behavior of the constructor ``__init__``
 (i.e., all the methods from all the merged classes are invoked rather than being
 overloaded by the same name method from the rightmost class) to other methods. A
 list of method names whose instances have to be all invoked can be specified in
 the ``invoke_all`` argument of ``mergeclasses``. Adaptive filtering of the
 arguments of the method instances is performed as well.
```

### Comparing `dyndesign-0.9.5/dyndesign/classmerger.py` & `dyndesign-0.9.6/dyndesign/classmerger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Merge a base class with one or more extension classes."""
 
 from functools import wraps
 from typing import Any, Callable, Dict, List, Tuple, Type, Union
 from collections import deque
+import re
 import inspect
 
 from dyndesign.dynloader import importclass
 
 __all__ = ["mergeclasses"]
 
 
@@ -55,14 +56,26 @@
             callable(args[0]) and
             next((True for s in inspect.stack() if s.function == DECORATED_STACK_FUNCTION_NAME), False)
         )
     except IndexError:
         return False
 
 
+def __is_missing_arguments_exception(e: Exception, method_instance: Callable) -> bool:
+    """Detect whether an exception is caused by missing positional arguments when invoking a method or not.
+
+    :param e: exception to check.
+    :param method_instance: method invoked.
+    :return: True if the exception is caused by missing positional arguments, False otherwise.
+    """
+    exception_message = e.args[0]
+    matching_regex = fr'({re.escape(method_instance.__name__)}|{re.escape(method_instance.__qualname__)})\(\) missing'
+    return re.match(matching_regex, exception_message) is not None
+
+
 def __decorator_builder(
     func: Callable,
     decorator_instance: Callable,
     is_last_decorator: bool = False
 ) -> Callable:
     """Build a single decorator wrapper around a method using an instance of decorator.
 
@@ -95,20 +108,26 @@
             __decorator_builder(func, decorator_instance),
             decorator_instances=decorator_instances
         )
     else:
         return __decorator_builder(func, decorator_instance, is_last_decorator=True)
 
 
-def __merge_not_overloaded(classes: List[Type], method: str) -> Union[Callable, None]:
+def __merge_not_overloaded(
+    classes: List[Type],
+    method: str,
+    strict_merged_args: bool
+) -> Union[Callable, None]:
     """Build a merged method by calling all the same-name method instances from the merged classes. If the method is
     used as a decorator (via `decoratewith`), then all the decorator instances are merged and called in pipeline.
 
     :param classes: merged classes.
     :param method: name of the method to be merged.
+    :param strict_merged_args: whether a `TypeError` exception is raised or not in case one or more positional
+                               arguments are missing.
     :return: merged method if two or more method instances are found, None otherwise.
     """
     all_method_instances = [getattr(cur_class, method) for cur_class in classes if method in dir(cur_class)]
     if len(all_method_instances) < 2:
         return None
 
     def call_all_method_instances(obj, *args, **kwargs):
@@ -117,42 +136,52 @@
         if __is_method_used_as_decorator(*args):
             decorated_method = __merged_decorator_builder(args[0], method_instances)
             returned_value = decorated_method(obj, *args, **kwargs)
         else:
             for method_instance in method_instances:
                 if not inspect.ismethoddescriptor(method_instance):
                     filtered_args, filtered_kwargs = __adapt_arguments(method_instance, *args, **kwargs)
-                    returned_value = method_instance(obj, *filtered_args, **filtered_kwargs)
+                    try:
+                        returned_value = method_instance(obj, *filtered_args, **filtered_kwargs)
+                    except TypeError as e:
+                        if strict_merged_args or not __is_missing_arguments_exception(e, method_instance):
+                            raise e
         return returned_value
 
     return call_all_method_instances
 
 
 def __preprocess_classes(all_classes: Any) -> List[Type]:
     """Dynamically import classes if passed as strings."""
     return [importclass(class_id) if type(class_id) == str else class_id for class_id in all_classes]
 
 
 def mergeclasses(
     base_class: Any,
     *extension_classes: Any,
-    invoke_all: Union[List[str], None] = None
+    invoke_all: Union[List[str], None] = None,
+    strict_merged_args = False
 ) -> Type:
     """Merge (i.e., extend) a base class with one or more extension classes. If more than one extension classes are
     provided, then the classes are extended in sequence following the order of `extension_classes`.
 
     :param base_class: base class.
     :param extension_classes: extension classes.
     :param invoke_all: list of methods (in addition to `__init__`) whose instances are invoked (if present) from all
                        the merged classes, rather than being overloaded by the instance from the rightmost class.
+    :param strict_merged_args: controls whether a `TypeError` exception is raised or not in case one or more positional
+                               arguments are missing in the `invoke_all` methods. It is set to True if an exception is
+                               raised, or False if the methods are silently skipped.
     :return: merged class.
     """
     all_classes = __preprocess_classes((base_class,) + extension_classes)
     invoke_all = ["__init__"] + (invoke_all or [])
     methods_not_oveloaded = {
-        method: merged for method in invoke_all if (merged := __merge_not_overloaded(all_classes, method))
+        method: merged for method in invoke_all if (
+            merged := __merge_not_overloaded(all_classes, method, strict_merged_args)
+        )
     }
     return type(
         all_classes[0].__name__,
         tuple(all_classes[::-1]),
         methods_not_oveloaded
     )
```

### Comparing `dyndesign-0.9.5/dyndesign/dynloader.py` & `dyndesign-0.9.6/dyndesign/dynloader.py`

 * *Files identical despite different names*

### Comparing `dyndesign-0.9.5/dyndesign/dynmethod.py` & `dyndesign-0.9.6/dyndesign/dynmethod.py`

 * *Files identical despite different names*

### Comparing `dyndesign-0.9.5/dyndesign/singletonmeta.py` & `dyndesign-0.9.6/dyndesign/singletonmeta.py`

 * *Files identical despite different names*

### Comparing `dyndesign-0.9.5/pyproject.toml` & `dyndesign-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dyndesign"
-version = "0.9.5"
+version = "0.9.6"
 description = "Toolset for Dynamic Design Patterns in Python."
 authors = ["Patrizio Gelosi <patrizio.gelosi@amarulasolutions.com>"]
 maintainers = ["Patrizio Gelosi <patrizio.gelosi@amarulasolutions.com>"]
 repository = "https://github.com/amarula/dyndesign"
 license = "MIT"
 readme = "README.rst"
 keywords = ["design", "pattern", "dynamic", "decorator", "inheritance"]
```

### Comparing `dyndesign-0.9.5/setup.py` & `dyndesign-0.9.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,460 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dyndesign
+Version: 0.9.6
+Summary: Toolset for Dynamic Design Patterns in Python.
+Home-page: https://github.com/amarula/dyndesign
+License: MIT
+Keywords: design,pattern,dynamic,decorator,inheritance
+Author: Patrizio Gelosi
+Author-email: patrizio.gelosi@amarulasolutions.com
+Maintainer: Patrizio Gelosi
+Maintainer-email: patrizio.gelosi@amarulasolutions.com
+Requires-Python: >=3.8,<4.0
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Repository, https://github.com/amarula/dyndesign
+Description-Content-Type: text/x-rst
 
-packages = \
-['dyndesign']
+DynDesign
+=========
 
-package_data = \
-{'': ['*']}
+|Build Status| |PyPi Version Status| |Python Version Status| |License|
 
-setup_kwargs = {
-    'name': 'dyndesign',
-    'version': '0.9.5',
-    'description': 'Toolset for Dynamic Design Patterns in Python.',
-    'long_description': 'DynDesign\n=========\n\n|Build Status| |PyPi Version Status| |Python Version Status| |License|\n\nA set of tools for Dynamic Design Patterns in Python.\n\n\nInstall\n-------\n\nDyndesign is on the Python Package Index (PyPI):\n\n::\n\n    pip install dyndesign\n\n\nOverview\n--------\n\nMerge two or more classes:\n\n.. code:: python\n\n    from dyndesign import mergeclasses\n\n    MergedClass = mergeclasses(Base, Ext1, Ext2, ...)\n\nDecorate a method with one or more instance methods loaded at runtime:\n\n.. code:: python\n\n    from dyndesign import decoratewith\n\n    @decoratewith("decorator_1", "component.decorator_2", ...)\n    def decorated_method(self, ...):\n        ...\n\nSafely invoke functions or methods from a ``safezone`` context manager:\n\n.. code:: python\n\n    from dyndesign import safezone\n\n    with safezone():\n        ...\n        function_possibly_non_existent()\n        ...\n\nCreate and destroy Singleton classes:\n\n.. code:: python\n\n    from dyndesign import SingletonMeta\n\n    class Singleton(metaclass=SingletonMeta):\n        ...\n\n    singleton_instance = Singleton(...)\n    same_singleton_instance = Singleton()\n    Singleton().destroy_singleton()\n    new_singleton_instance = Singleton(...)\n\nImport classes dynamically using the path:\n\n.. code:: python\n\n    from dyndesign import importclass\n\n    ImportedClass = importclass("directory.module.class_name")\n\n\nMerging Classes\n---------------\n\nDyndesign provides API ``mergeclasses`` to merge two or more classes as if they\nwere dictionaries, so that the merged class has the attributes and methods of\nthe base class and of the extension classes. If two or more classes have the\nsame attributes/methods, the attributes/methods from the rightmost classes (in\nthe order in which the classes are passed to ``mergeclasses``) overload the\nones from the leftmost classes, similarly to what happens when merging\ndictionaries.\n\n.. code:: python\n\n    from dyndesign import mergeclasses\n\n    class Base:\n        def __init__(self, init_value):\n            self.param = init_value\n\n        def m1(self):\n            print(f"Method `m1` of class `Base`, and {self.param=}")\n\n        def m2(self):\n            print(f"Method `m2` of class `Base`")\n\n    class Ext:\n        def m1(self):\n            print(f"Method `m1` of class `Ext`, and {self.param=}")\n\n    MergedClass = mergeclasses(Base, Ext)\n    merged_instance = MergedClass("INITIAL VALUE")\n    merged_instance.m1()\n    merged_instance.m2()\n\n    # Method `m1` of class `Ext`, and self.param=\'INITIAL VALUE\'\n    # Method `m2` of class `Base`\n\n\nWhen a merged class is instantiated with arguments, the constructor of each\nmerging class is invoked, since constructors are excluded from being overloaded.\nAlso, arguments passed to each constructor are adaptively filtered based on the\nconstructor signature so that each constructor takes just the arguments it\nrequires, and no exception is raised for the exceeding arguments passed:\n\n.. code:: python\n\n    class A:\n        def __init__(self):\n            print("No argument passed to class `A`")\n\n    class B:\n        def __init__(self, a):\n            print(f"Argument {a=} passed to class `B`")\n\n    class C:\n        def __init__(self, a, b, kw1=None):\n            print(f"Argument {a=}, {b=} and {kw1=} passed to class `C`")\n\n    class D:\n        def __init__(self, kw2=None):\n            print(f"Argument {kw2=} passed to class `D`")\n\n    MergedClass = mergeclasses(A, B, C, D)\n    MergedClass("Alpha", "Beta", kw1="kwarg #1", kw2="kwarg #2")\n\n    # No argument passed to class `A`\n    # Argument a=\'Alpha\' passed to class `B`\n    # Argument a=\'Alpha\', b=\'Beta\' and kw1=\'kwarg #1\' passed to class `C`\n    # Argument kw2=\'kwarg #2\' passed to class `D`\n\n\nIt is also possible to extend the same behavior of the constructor ``__init__``\n(i.e., all the methods from all the merged classes are invoked rather than being\noverloaded by the same name method from the rightmost class) to other methods. A\nlist of method names whose instances have to be all invoked can be specified in\nthe ``invoke_all`` argument of ``mergeclasses``. Adaptive filtering of the\narguments of the method instances is performed as well.\n\n.. code:: python\n\n    class E:\n        def method(self):\n            print("No argument passed to `method` of class `E`")\n\n    class F:\n        def method(self, a):\n            print(f"Argument {a=} passed to `method` of class `F`")\n\n    MergedClass = mergeclasses(E, F, invoke_all=["method"])\n    MergedClass().method("Alpha")\n\n    # No argument passed to `method` of class `E`\n    # Argument a=\'Alpha\' passed to `method` of class `F`\n\n\nDynamic Decorators\n------------------\n\nMeta decorator ``decoratewith`` decorates a class method with one or more\npipelined instance decorators (regardless whether they statically exist or not).\nThe syntax of the dynamic decorators aims to get rid of the boilerplate for\nwrapping and returning the decorator code, leaving just the wrapper\'s code. For\nexample, dynamic decorators can be used to decorate a method from a base class\nwith a method from an extension class:\n\n.. code:: python\n\n    from dyndesign import decoratewith\n\n    class Base:\n        @decoratewith("decorator")\n        def m(self):\n            print(f"Method `m` of class `Base`")\n\n    class Ext:\n        def decorator(self, func):\n            print("Beginning of method decoration from Ext.")\n            func(self)\n            print("End of method decoration from Ext.")\n\n    merged = mergeclasses(Base, Ext)()\n    merged.m()\n\n    # Beginning of method decoration from Ext.\n    # Method `m` of class `Base`\n    # End of method decoration from Ext.\n\nIf a decorator name is passed in the ``invoke_all`` argument of\n``mergeclasses``, then multiple decorator instances with the same name from\ndifferent extension classes may be used in pipeline:\n\n.. code:: python\n\n    class Ext2:\n        def decorator(self, func):\n            print("Beginning of method decoration from Ext2.")\n            func(self)\n            print("End of method decoration from Ext2.")\n\n    merged = mergeclasses(Base, Ext, Ext2, invoke_all=["decorator"])()\n    merged.m()\n\n    # Beginning of method decoration from Ext.\n    # Beginning of method decoration from Ext2.\n    # Method `m` of class `Base`\n    # End of method decoration from Ext2.\n    # End of method decoration from Ext.\n\n\nArguments of ``decoratewith`` are loaded at runtime as properties of the\nvariable \'self\': a dynamic decorator can be, for example, a method of a\ncomponent class. In case of dynamic decoration from a sub-instance of \'self\',\nthe instance object of the decorated method is passed to the decorator as the\nargument ``decorated_self``. If a dynamic decorator is not found at runtime\n(e.g., because it is a method of an optional class that has not been merged),\nthen the code execution proceeds normally, as shown below with the decorator\n``non_existent_decorator``:\n\n.. code:: python\n\n    class Base:\n        def __init__(self):\n            self.comp = Component()\n\n        @decoratewith("comp.decorator1", "comp.decorator2", "non_existent_decorator")\n        def m(self):\n            print("Method `m` of class `Base`")\n\n    class Component:\n        def __init__(self):\n            self.value = "Initial"\n\n        def decorator1(self, func, decorated_self):\n            print(f"Beginning of method decoration #1 ({self.value=})")\n            self.value = "Processed"\n            func(decorated_self)\n            print("End of method decoration #1")\n\n        def decorator2(self, func, decorated_self):\n            print(f"Beginning of method decoration #2 ({self.value=})")\n            func(decorated_self)\n            print("End of method decoration #2")\n\n    base = Base()\n    base.m()\n\n    # Beginning of method decoration #1 (self.value=\'Initial\')\n    # Beginning of method decoration #2 (self.value=\'Processed\')\n    # Method `m` of class `Base`\n    # End of method decoration #2\n    # End of method decoration #1\n\n\nSafezone Context Manager\n------------------------\n\nAny function or method that may or may not exist at runtime (e.g., methods of\nmerged classes) can be invoked from Context Manager ``safezone`` in order to\nsuppress the possible exceptions raised if the function or method is not found\nat runtime. Optionally, a fallback function/method can be also passed. If no\nfunction name(s) is passed as argument of ``safezone``, then each function in\nthe safe zone\'s code is protected; if any function name(s) is passed, the\nprotection is restricted to the functions having that/those name(s). For\nexample, ``safezone`` can be used to safely call functions that may or may not\nexist at runtime:\n\n.. code:: python\n\n    from dyndesign import safezone\n    \n    def fallback():\n        print("Fallback function")\n\n    def function_a():\n        print("Function `a`")\n\n    with safezone(fallback=fallback):\n        function_a()\n        non_existent_function()\n\n    # Function `a`\n    # Fallback function\n\n\nA further example shows that ``safezone`` can be used to safely invoke methods\nof classes that may or may not be merged with other classes:\n\n.. code:: python\n\n    class Base:\n        def fallback(self):\n            print("Fallback method")\n\n        def m(self, class_desc):\n            print(f"Method `m` of {class_desc}")\n            with safezone("optional_method", fallback=self.fallback):\n                self.optional_method()\n\n    class ExtOptional:\n        def optional_method(self):\n            print("Optional method from class `ExtOptional`")\n\n    merged = mergeclasses(Base, ExtOptional)()\n    merged.m("merged class")\n    base = Base()\n    base.m("class `Base` standalone")\n\n    # Method `m` of merged class\n    # Optional method from class `ExtOptional`\n    # Method `m` of class `Base` standalone\n    # Fallback method\n\n\nInvoking methods safely\n-----------------------\n\nAs alternative to ``safezone`` context manager, ``safeinvoke`` can be used to\nsafely invoke methods that may or may not exist at runtime. To this end, method\n``m`` of class ``Base`` of the example above can be replaced as follows:\n\n.. code:: python\n\n    from dyndesign import safeinvoke\n\n    ...\n\n        def m(self, class_desc):\n            print(f"Method `m` of {class_desc}")\n            safeinvoke("optional_method", self, fallback=self.fallback)\n\n\nSingleton classes\n-----------------\n\nSingleton classes can be swiftly created and destroyed with\n``destroy_singleton``:\n\n.. code:: python\n\n    from dyndesign import SingletonMeta\n\n    class Singleton(metaclass=SingletonMeta):\n        def __init__(self, instance_id = None):\n            if instance_id:\n                self.instance_id = instance_id\n            print(f"Created a {instance_id} instance of `Singleton`")\n\n        def where_points(self, object_name):\n            print(f"Object `{object_name}` points to the {self.instance_id} instance")\n\n    s_A = Singleton("first")\n    s_A.where_points("s_A")\n    s_B = Singleton()\n    s_B.where_points("s_B")\n    Singleton().destroy_singleton()\n    s_C = Singleton("second")\n    s_C.where_points("s_C")\n\n    # Created a first instance of `Singleton`\n    # Object `s_A` points to the first instance\n    # Object `s_B` points to the first instance\n    # Created a second instance of `Singleton`\n    # Object `s_C` points to the second instance\n\nThe class method ``destroy`` of SingletonMeta can be invoked to destroy all the\nSingleton classes at once. As a further alternative to the instance call\n``destroy_singleton``, the names of the Singleton classes to destroy can be\npassed to the class method ``destroy``:\n\n.. code:: python\n\n    Singleton().destroy_singleton() # Destroy only `Singleton`\n    SingletonMeta.destroy() # Destroy all the singleton classes\n    SingletonMeta.destroy(\'Singleton1\', \'Singleton2\', \'Singleton3\') # Destroy selectively\n\n\nImporting classes dynamically\n-----------------------------\n\nClasses can be imported dynamically using the package/class names or the path in\ndot-notation as shown below:\n\n.. code:: python\n\n    from dyndesign import importclass\n\n    ClassA = importclass(\'package_A\', \'ClassA\')\n    ClassB = importclass(\'directory_B.package_B.ClassB\')\n\n\nRunning tests\n--------------\n\nTo run the tests using your default python:\n\n::\n\n    pip install -U pytest\n    python3 -m pytest test\n\n\n.. |Build Status| image:: https://github.com/amarula/dyndesign/actions/workflows/python-app.yml/badge.svg\n    :target: https://github.com/amarula/dyndesign/actions\n.. |Python Version Status| image:: https://img.shields.io/badge/python-3.8_3.9_3.10_3.11-blue.svg\n    :target: https://github.com/amarula/dyndesign/actions\n.. |PyPi Version Status| image:: https://badge.fury.io/py/dyndesign.svg\n    :target: https://badge.fury.io/py/dyndesign\n.. |License| image:: https://img.shields.io/badge/License-MIT-yellow.svg\n    :target: https://opensource.org/licenses/MIT\n',
-    'author': 'Patrizio Gelosi',
-    'author_email': 'patrizio.gelosi@amarulasolutions.com',
-    'maintainer': 'Patrizio Gelosi',
-    'maintainer_email': 'patrizio.gelosi@amarulasolutions.com',
-    'url': 'https://github.com/amarula/dyndesign',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+A set of tools for Dynamic Design Patterns in Python.
 
 
-setup(**setup_kwargs)
+Install
+-------
+
+Dyndesign is on the Python Package Index (PyPI):
+
+::
+
+    pip install dyndesign
+
+
+Overview
+--------
+
+Merge two or more classes:
+
+.. code:: python
+
+    from dyndesign import mergeclasses
+
+    MergedClass = mergeclasses(Base, Ext1, Ext2, ...)
+
+Decorate a method with one or more instance methods loaded at runtime:
+
+.. code:: python
+
+    from dyndesign import decoratewith
+
+    @decoratewith("decorator_1", "component.decorator_2", ...)
+    def decorated_method(self, ...):
+        ...
+
+Safely invoke functions or methods from a ``safezone`` context manager:
+
+.. code:: python
+
+    from dyndesign import safezone
+
+    with safezone():
+        ...
+        function_possibly_non_existent()
+        ...
+
+Create and destroy Singleton classes:
+
+.. code:: python
+
+    from dyndesign import SingletonMeta
+
+    class Singleton(metaclass=SingletonMeta):
+        ...
+
+    singleton_instance = Singleton(...)
+    same_singleton_instance = Singleton()
+    Singleton().destroy_singleton()
+    new_singleton_instance = Singleton(...)
+
+Import classes dynamically using the path:
+
+.. code:: python
+
+    from dyndesign import importclass
+
+    ImportedClass = importclass("directory.module.class_name")
+
+
+Merging Classes
+---------------
+
+Dyndesign provides API ``mergeclasses`` to merge two or more classes as if they
+were dictionaries, so that the merged class has the attributes and methods of
+the base class and of the extension classes. If two or more classes have the
+same attributes/methods, the attributes/methods from the rightmost classes (in
+the order in which the classes are passed to ``mergeclasses``) overload the
+ones from the leftmost classes, similarly to what happens when merging
+dictionaries.
+
+.. code:: python
+
+    from dyndesign import mergeclasses
+
+    class Base:
+        def __init__(self, init_value):
+            self.param = init_value
+
+        def m1(self):
+            print(f"Method `m1` of class `Base`, and {self.param=}")
+
+        def m2(self):
+            print(f"Method `m2` of class `Base`")
+
+    class Ext:
+        def m1(self):
+            print(f"Method `m1` of class `Ext`, and {self.param=}")
+
+    MergedClass = mergeclasses(Base, Ext)
+    merged_instance = MergedClass("INITIAL VALUE")
+    merged_instance.m1()
+    merged_instance.m2()
+
+    # Method `m1` of class `Ext`, and self.param='INITIAL VALUE'
+    # Method `m2` of class `Base`
+
+
+When a merged class is instantiated with arguments, the constructor of each
+merging class is invoked, since constructors are excluded from being overloaded.
+Also, arguments passed to each constructor are adaptively filtered based on the
+constructor signature so that each constructor takes just the arguments it
+requires, and no exception is raised for exceeding or missing arguments passed:
+
+.. code:: python
+
+    class A:
+        def __init__(self):
+            print("No argument passed to class `A`")
+
+    class B:
+        def __init__(self, a):
+            print(f"Argument {a=} passed to class `B`")
+
+    class C:
+        def __init__(self, a, b, kw1=None):
+            print(f"Argument {a=}, {b=} and {kw1=} passed to class `C`")
+
+    class D:
+        def __init__(self, kw2=None):
+            print(f"Argument {kw2=} passed to class `D`")
+
+    MergedClass = mergeclasses(A, B, C, D)
+    MergedClass("Alpha", "Beta", kw1="kwarg #1", kw2="kwarg #2")
+
+    # No argument passed to class `A`
+    # Argument a='Alpha' passed to class `B`
+    # Argument a='Alpha', b='Beta' and kw1='kwarg #1' passed to class `C`
+    # Argument kw2='kwarg #2' passed to class `D`
+
+    MergedClass()
+
+    # No argument passed to class `A`
+    # Argument kw2='kwarg #2' passed to class `D`
+
+
+It is also possible to extend the same behavior of the constructor ``__init__``
+(i.e., all the methods from all the merged classes are invoked rather than being
+overloaded by the same name method from the rightmost class) to other methods. A
+list of method names whose instances have to be all invoked can be specified in
+the ``invoke_all`` argument of ``mergeclasses``. Adaptive filtering of the
+arguments of the method instances is performed as well.
+
+.. code:: python
+
+    class E:
+        def method(self):
+            print("No argument passed to `method` of class `E`")
+
+    class F:
+        def method(self, a):
+            print(f"Argument {a=} passed to `method` of class `F`")
+
+    MergedClass = mergeclasses(E, F, invoke_all=["method"])
+    MergedClass().method("Alpha")
+
+    # No argument passed to `method` of class `E`
+    # Argument a='Alpha' passed to `method` of class `F`
+
+
+Dynamic Decorators
+------------------
+
+Meta decorator ``decoratewith`` decorates a class method with one or more
+pipelined instance decorators (regardless whether they statically exist or not).
+The syntax of the dynamic decorators aims to get rid of the boilerplate for
+wrapping and returning the decorator code, leaving just the wrapper's code. For
+example, dynamic decorators can be used to decorate a method from a base class
+with a method from an extension class:
+
+.. code:: python
+
+    from dyndesign import decoratewith
+
+    class Base:
+        @decoratewith("decorator")
+        def m(self):
+            print(f"Method `m` of class `Base`")
+
+    class Ext:
+        def decorator(self, func):
+            print("Beginning of method decoration from Ext.")
+            func(self)
+            print("End of method decoration from Ext.")
+
+    merged = mergeclasses(Base, Ext)()
+    merged.m()
+
+    # Beginning of method decoration from Ext.
+    # Method `m` of class `Base`
+    # End of method decoration from Ext.
+
+If a decorator name is passed in the ``invoke_all`` argument of
+``mergeclasses``, then multiple decorator instances with the same name from
+different extension classes may be used in pipeline:
+
+.. code:: python
+
+    class Ext2:
+        def decorator(self, func):
+            print("Beginning of method decoration from Ext2.")
+            func(self)
+            print("End of method decoration from Ext2.")
+
+    merged = mergeclasses(Base, Ext, Ext2, invoke_all=["decorator"])()
+    merged.m()
+
+    # Beginning of method decoration from Ext.
+    # Beginning of method decoration from Ext2.
+    # Method `m` of class `Base`
+    # End of method decoration from Ext2.
+    # End of method decoration from Ext.
+
+
+Arguments of ``decoratewith`` are loaded at runtime as properties of the
+variable 'self': a dynamic decorator can be, for example, a method of a
+component class. In case of dynamic decoration from a sub-instance of 'self',
+the instance object of the decorated method is passed to the decorator as the
+argument ``decorated_self``. If a dynamic decorator is not found at runtime
+(e.g., because it is a method of an optional class that has not been merged),
+then the code execution proceeds normally, as shown below with the decorator
+``non_existent_decorator``:
+
+.. code:: python
+
+    class Base:
+        def __init__(self):
+            self.comp = Component()
+
+        @decoratewith("comp.decorator1", "comp.decorator2", "non_existent_decorator")
+        def m(self):
+            print("Method `m` of class `Base`")
+
+    class Component:
+        def __init__(self):
+            self.value = "Initial"
+
+        def decorator1(self, func, decorated_self):
+            print(f"Beginning of method decoration #1 ({self.value=})")
+            self.value = "Processed"
+            func(decorated_self)
+            print("End of method decoration #1")
+
+        def decorator2(self, func, decorated_self):
+            print(f"Beginning of method decoration #2 ({self.value=})")
+            func(decorated_self)
+            print("End of method decoration #2")
+
+    base = Base()
+    base.m()
+
+    # Beginning of method decoration #1 (self.value='Initial')
+    # Beginning of method decoration #2 (self.value='Processed')
+    # Method `m` of class `Base`
+    # End of method decoration #2
+    # End of method decoration #1
+
+
+Safezone Context Manager
+------------------------
+
+Any function or method that may or may not exist at runtime (e.g., methods of
+merged classes) can be invoked from Context Manager ``safezone`` in order to
+suppress the possible exceptions raised if the function or method is not found
+at runtime. Optionally, a fallback function/method can be also passed. If no
+function name(s) is passed as argument of ``safezone``, then each function in
+the safe zone's code is protected; if any function name(s) is passed, the
+protection is restricted to the functions having that/those name(s). For
+example, ``safezone`` can be used to safely call functions that may or may not
+exist at runtime:
+
+.. code:: python
+
+    from dyndesign import safezone
+    
+    def fallback():
+        print("Fallback function")
+
+    def function_a():
+        print("Function `a`")
+
+    with safezone(fallback=fallback):
+        function_a()
+        non_existent_function()
+
+    # Function `a`
+    # Fallback function
+
+
+A further example shows that ``safezone`` can be used to safely invoke methods
+of classes that may or may not be merged with other classes:
+
+.. code:: python
+
+    class Base:
+        def fallback(self):
+            print("Fallback method")
+
+        def m(self, class_desc):
+            print(f"Method `m` of {class_desc}")
+            with safezone("optional_method", fallback=self.fallback):
+                self.optional_method()
+
+    class ExtOptional:
+        def optional_method(self):
+            print("Optional method from class `ExtOptional`")
+
+    merged = mergeclasses(Base, ExtOptional)()
+    merged.m("merged class")
+    base = Base()
+    base.m("class `Base` standalone")
+
+    # Method `m` of merged class
+    # Optional method from class `ExtOptional`
+    # Method `m` of class `Base` standalone
+    # Fallback method
+
+
+Invoking methods safely
+-----------------------
+
+As alternative to ``safezone`` context manager, ``safeinvoke`` can be used to
+safely invoke methods that may or may not exist at runtime. To this end, method
+``m`` of class ``Base`` of the example above can be replaced as follows:
+
+.. code:: python
+
+    from dyndesign import safeinvoke
+
+    ...
+
+        def m(self, class_desc):
+            print(f"Method `m` of {class_desc}")
+            safeinvoke("optional_method", self, fallback=self.fallback)
+
+
+Singleton classes
+-----------------
+
+Singleton classes can be swiftly created and destroyed with
+``destroy_singleton``:
+
+.. code:: python
+
+    from dyndesign import SingletonMeta
+
+    class Singleton(metaclass=SingletonMeta):
+        def __init__(self, instance_id = None):
+            if instance_id:
+                self.instance_id = instance_id
+            print(f"Created a {instance_id} instance of `Singleton`")
+
+        def where_points(self, object_name):
+            print(f"Object `{object_name}` points to the {self.instance_id} instance")
+
+    s_A = Singleton("first")
+    s_A.where_points("s_A")
+    s_B = Singleton()
+    s_B.where_points("s_B")
+    Singleton().destroy_singleton()
+    s_C = Singleton("second")
+    s_C.where_points("s_C")
+
+    # Created a first instance of `Singleton`
+    # Object `s_A` points to the first instance
+    # Object `s_B` points to the first instance
+    # Created a second instance of `Singleton`
+    # Object `s_C` points to the second instance
+
+The class method ``destroy`` of SingletonMeta can be invoked to destroy all the
+Singleton classes at once. As a further alternative to the instance call
+``destroy_singleton``, the names of the Singleton classes to destroy can be
+passed to the class method ``destroy``:
+
+.. code:: python
+
+    Singleton().destroy_singleton() # Destroy only `Singleton`
+    SingletonMeta.destroy() # Destroy all the singleton classes
+    SingletonMeta.destroy('Singleton1', 'Singleton2', 'Singleton3') # Destroy selectively
+
+
+Importing classes dynamically
+-----------------------------
+
+Classes can be imported dynamically using the package/class names or the path in
+dot-notation as shown below:
+
+.. code:: python
+
+    from dyndesign import importclass
+
+    ClassA = importclass('package_A', 'ClassA')
+    ClassB = importclass('directory_B.package_B.ClassB')
+
+
+Running tests
+--------------
+
+To run the tests using your default python:
+
+::
+
+    pip install -U pytest
+    python3 -m pytest test
+
+
+.. |Build Status| image:: https://github.com/amarula/dyndesign/actions/workflows/python-app.yml/badge.svg
+    :target: https://github.com/amarula/dyndesign/actions
+.. |Python Version Status| image:: https://img.shields.io/badge/python-3.8_3.9_3.10_3.11-blue.svg
+    :target: https://github.com/amarula/dyndesign/actions
+.. |PyPi Version Status| image:: https://badge.fury.io/py/dyndesign.svg
+    :target: https://badge.fury.io/py/dyndesign
+.. |License| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+    :target: https://opensource.org/licenses/MIT
+
```

