# Comparing `tmp/bw2parameters-0.7.tar.gz` & `tmp/bw2parameters-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw2parameters-0.7.tar", last modified: Sat Dec 25 10:57:05 2021, max compression
+gzip compressed data, was "bw2parameters-1.1.0.tar", last modified: Tue Apr 18 08:53:14 2023, max compression
```

## Comparing `bw2parameters-0.7.tar` & `bw2parameters-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-12-25 10:57:05.412076 bw2parameters-0.7/
--rw-r--r--   0 cmutel     (501) staff       (20)      101 2021-12-23 10:01:33.000000 bw2parameters-0.7/.hgignore
--rw-r--r--   0 cmutel     (501) staff       (20)     1351 2021-12-25 10:43:09.000000 bw2parameters-0.7/CHANGES.md
--rw-r--r--   0 cmutel     (501) staff       (20)     3220 2021-12-23 10:01:33.000000 bw2parameters-0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 cmutel     (501) staff       (20)     1498 2021-12-23 10:01:33.000000 bw2parameters-0.7/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)       43 2021-12-25 10:56:59.000000 bw2parameters-0.7/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     3384 2021-12-25 10:57:05.410980 bw2parameters-0.7/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      903 2021-12-25 10:50:39.000000 bw2parameters-0.7/README.md
--rw-r--r--   0 cmutel     (501) staff       (20)     1145 2021-12-23 10:01:33.000000 bw2parameters-0.7/appveyor.yml
--rw-r--r--   0 cmutel     (501) staff       (20)      625 2021-12-23 10:01:33.000000 bw2parameters-0.7/bitbucket-pipelines.yml
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-12-25 10:57:05.389590 bw2parameters-0.7/bw2parameters/
--rw-r--r--   0 cmutel     (501) staff       (20)      187 2021-12-25 10:44:31.000000 bw2parameters-0.7/bw2parameters/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)      686 2021-12-25 10:44:46.000000 bw2parameters-0.7/bw2parameters/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3379 2021-12-25 10:44:46.000000 bw2parameters-0.7/bw2parameters/mangling.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9267 2021-12-25 10:44:47.000000 bw2parameters-0.7/bw2parameters/parameter_set.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1326 2021-12-25 10:44:46.000000 bw2parameters-0.7/bw2parameters/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-12-25 10:57:05.398568 bw2parameters-0.7/bw2parameters.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     3384 2021-12-25 10:57:05.000000 bw2parameters-0.7/bw2parameters.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      590 2021-12-25 10:57:05.000000 bw2parameters-0.7/bw2parameters.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2021-12-25 10:57:05.000000 bw2parameters-0.7/bw2parameters.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2021-12-25 10:57:05.000000 bw2parameters-0.7/bw2parameters.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       14 2021-12-25 10:57:05.000000 bw2parameters-0.7/bw2parameters.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-12-25 10:57:05.404812 bw2parameters-0.7/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     6822 2021-12-23 10:01:33.000000 bw2parameters-0.7/docs/Makefile
--rw-r--r--   0 cmutel     (501) staff       (20)     7981 2021-12-23 10:01:33.000000 bw2parameters-0.7/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3297 2021-12-25 10:51:42.000000 bw2parameters-0.7/docs/index.rst
--rw-r--r--   0 cmutel     (501) staff       (20)     6731 2021-12-23 10:01:33.000000 bw2parameters-0.7/docs/make.bat
--rw-r--r--   0 cmutel     (501) staff       (20)       35 2021-12-23 10:01:33.000000 bw2parameters-0.7/pytest.ini
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2021-12-23 10:01:33.000000 bw2parameters-0.7/requirements.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2021-12-25 10:57:05.412244 bw2parameters-0.7/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     1088 2021-12-25 10:56:28.000000 bw2parameters-0.7/setup.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-12-25 10:57:05.407941 bw2parameters-0.7/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)     1478 2021-12-23 10:01:33.000000 bw2parameters-0.7/tests/test_mangling.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2847 2021-12-23 10:01:33.000000 bw2parameters-0.7/tests/test_monte_carlo.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7321 2021-12-23 10:01:33.000000 bw2parameters-0.7/tests/test_parameter_set.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-18 08:53:14.651582 bw2parameters-1.1.0/
+-rw-r--r--   0 chrismutel   (501) staff       (20)       48 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/.gitignore
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1817 2023-04-18 08:40:31.000000 bw2parameters-1.1.0/CHANGES.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3220 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2817 2023-04-17 11:56:17.000000 bw2parameters-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1498 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       43 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2060 2023-04-18 08:53:14.651684 bw2parameters-1.1.0/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      903 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-18 08:53:14.647338 bw2parameters-1.1.0/bw2parameters/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-17 12:01:36.000000 bw2parameters-1.1.0/bw2parameters/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      637 2023-04-17 12:02:37.000000 bw2parameters-1.1.0/bw2parameters/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      686 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/bw2parameters/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9270 2023-04-17 11:54:59.000000 bw2parameters-1.1.0/bw2parameters/interpreter.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3379 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/bw2parameters/mangling.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11565 2023-04-17 11:54:59.000000 bw2parameters-1.1.0/bw2parameters/parameter_set.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2909 2023-04-17 11:54:59.000000 bw2parameters-1.1.0/bw2parameters/pint.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1149 2023-04-17 12:06:31.000000 bw2parameters-1.1.0/bw2parameters/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-18 08:53:14.648212 bw2parameters-1.1.0/bw2parameters.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2060 2023-04-18 08:53:14.000000 bw2parameters-1.1.0/bw2parameters.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1005 2023-04-18 08:53:14.000000 bw2parameters-1.1.0/bw2parameters.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-18 08:53:14.000000 bw2parameters-1.1.0/bw2parameters.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-18 08:53:14.000000 bw2parameters-1.1.0/bw2parameters.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      140 2023-04-18 08:53:14.000000 bw2parameters-1.1.0/bw2parameters.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       24 2023-04-18 08:53:14.000000 bw2parameters-1.1.0/bw2parameters.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-18 08:53:14.648695 bw2parameters-1.1.0/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6822 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/docs/Makefile
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7981 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4066 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/docs/index.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6731 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/docs/make.bat
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-17 11:56:17.000000 bw2parameters-1.1.0/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)       35 2023-02-26 08:38:31.000000 bw2parameters-1.1.0/pytest.ini
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1767 2023-04-18 08:53:14.652045 bw2parameters-1.1.0/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-18 08:53:14.651353 bw2parameters-1.1.0/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2663 2023-04-17 11:55:03.000000 bw2parameters-1.1.0/tests/test_interpreter.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1506 2023-04-17 11:55:03.000000 bw2parameters-1.1.0/tests/test_mangling.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2705 2023-04-17 11:55:03.000000 bw2parameters-1.1.0/tests/test_monte_carlo.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7317 2023-04-17 11:55:03.000000 bw2parameters-1.1.0/tests/test_parameter_set.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6524 2023-04-17 11:55:03.000000 bw2parameters-1.1.0/tests/test_pint_interpreter.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      880 2023-04-17 11:55:03.000000 bw2parameters-1.1.0/tests/test_pint_parameter_set.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1172 2023-04-17 11:48:34.000000 bw2parameters-1.1.0/tests/test_pint_wrapper.py
```

### Comparing `bw2parameters-0.7/CODE_OF_CONDUCT.md` & `bw2parameters-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bw2parameters-0.7/LICENSE` & `bw2parameters-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw2parameters-0.7/README.md` & `bw2parameters-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bw2parameters-0.7/bw2parameters/errors.py` & `bw2parameters-1.1.0/bw2parameters/errors.py`

 * *Files identical despite different names*

### Comparing `bw2parameters-0.7/bw2parameters/mangling.py` & `bw2parameters-1.1.0/bw2parameters/mangling.py`

 * *Files identical despite different names*

### Comparing `bw2parameters-0.7/bw2parameters/parameter_set.py` & `bw2parameters-1.1.0/bw2parameters/parameter_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # -*- coding: utf-8 -*-
 from numbers import Number
 from pprint import pformat
 
 import numpy as np
-from asteval import Interpreter
 from stats_arrays import uncertainty_choices
 
 from .errors import *
-from .utils import EXISTING_SYMBOLS, get_symbols, isidentifier, isstr
+from .interpreter import Interpreter, PintInterpreter
+from .pint import PintWrapper
+from .utils import isidentifier
 
 MC_ERROR_TEXT = """Formula returned array of wrong shape:
 Name: {}
 Formula: {}
 Expected shape: {}
 Returned shape: {}"""
 
 
 class ParameterSet(object):
-    def __init__(self, params, global_params=None):
+    def __init__(self, params, global_params=None, interpreter=None):
         self.params = params
         self.global_params = global_params or {}
+        self.interpreter = interpreter or Interpreter()
         self.basic_validation()
+        self.all_param_names = set(self.params).union(set(self.global_params))
         self.references = self.get_references()
         for name, references in self.references.items():
             if name in references:
                 raise SelfReference(
-                    u"Formula for parameter {} references itself".format(name)
+                    "Formula for parameter {} references itself".format(name)
                 )
 
         self.order = self.get_order()
 
     def get_order(self):
         """Get a list of parameter name in an order that they can be safely evaluated"""
         order = []
-        seen = set()
+        seen = set(self.interpreter.symtable.keys())
         refs = self.references.copy()
 
         while refs:
             last_iteration = set(refs.keys())
             for k, v in refs.items():
                 if not v.difference(seen):
                     seen.add(k)
@@ -52,124 +55,127 @@
                     (k, v)
                     for k, v in refs.items()
                     if not {x.lower() for x in v}.difference(seen_lower_case)
                 ]
                 if wrong_case:
                     raise CapitalizationError(
                         (
-                            u"Possible errors in upper/lower case letters for some parameters.\n"
-                            u"Unmatched references:\n{}\nMatched references:\n{}"
+                            "Possible errors in upper/lower case letters for some parameters.\n"
+                            "Unmatched references:\n{}\nMatched references:\n{}"
                         ).format(
-                            pformat(refs, indent=2), pformat(sorted(seen), indent=2)
+                            pformat(refs, indent=2),
+                            pformat(sorted(seen), indent=2),
                         )
                     )
                 raise ParameterError(
                     (
-                        u"Undefined or circular references for the following:"
-                        u"\n{}\nExisting references:\n{}"
-                    ).format(pformat(refs, indent=2), pformat(sorted(order), indent=2))
+                        "Undefined or circular references for the following:"
+                        "\n{}\nExisting references:\n{}"
+                    ).format(
+                        pformat(refs, indent=2),
+                        pformat(sorted(order), indent=2),
+                    )
                 )
 
         return order
 
     def get_references(self):
         """Create dictionary of parameter references"""
         refs = {
-            key: get_symbols(value["formula"]) if value.get("formula") else set()
+            key: self.interpreter.get_unknown_symbols(value.get("formula"))
             for key, value in self.params.items()
         }
         refs.update({key: set() for key in self.global_params})
         return refs
 
     def basic_validation(self):
         """Basic validation needed to build ``references`` and ``order``"""
         if not isinstance(self.params, dict):
-            raise ValueError(u"Parameters are not a dictionary")
+            raise ValueError("Parameters are not a dictionary")
         if not isinstance(self.global_params, dict):
-            raise ValueError(u"Global parameters are not a dictionary")
+            raise ValueError("Global parameters are not a dictionary")
         for key, value in self.params.items():
             if not isinstance(value, dict):
-                raise ValueError(u"Parameter value {} is not a dictionary".format(key))
+                raise ValueError("Parameter value {} is not a dictionary".format(key))
             elif not (
-                isinstance(value.get("amount"), (Number, np.ndarray))
-                or isstr(value.get("formula"))
+                self.interpreter.is_numeric(value.get("amount"))
+                or isinstance(value.get("formula"), str)
             ):
                 raise ValueError(
                     (
-                        u"Parameter {} must have either ``amount`` "
-                        u"or ``formula`` field"
+                        "Parameter {} must have either ``amount`` "
+                        "or ``formula`` field"
                     ).format(key)
                 )
             elif not isidentifier(key):
                 raise ValueError(
-                    u"Parameter label {} not a valid Python name".format(key)
+                    "Parameter label {} not a valid Python name".format(key)
                 )
-            elif key in EXISTING_SYMBOLS:
+            elif key in self.interpreter.BUILTIN_SYMBOLS:
                 raise DuplicateName(
-                    u"Parameter name {} is a built-in symbol".format(key)
+                    "Parameter name {} is a built-in symbol".format(key)
                 )
         for key, value in self.global_params.items():
-            if not isinstance(value, (Number, np.ndarray)):
+            if not self.interpreter.is_numeric(value):
                 raise ValueError(
-                    (
-                        u"Global parameter {} does not have a " u"numeric value: {}"
-                    ).format(key, value)
+                    ("Global parameter {} does not have a " "numeric value: {}").format(
+                        key, value
+                    )
                 )
             elif not isidentifier(key):
                 raise ValueError(
-                    (u"Global parameter label {} not a valid " u"Python name").format(
-                        key
-                    )
+                    "Global parameter label {} not a valid " "Python name".format(key)
                 )
 
     def evaluate(self):
         """Evaluate each formula. Returns dictionary of parameter names and values."""
-        interpreter = Interpreter()
+        interpreter = self.interpreter
         result = {}
         for key in self.order:
             if key in self.global_params:
-                interpreter.symtable[key] = result[key] = self.global_params[key]
+                value = self.global_params[key]
             elif self.params[key].get("formula"):
                 value = interpreter(self.params[key]["formula"])
-                interpreter.symtable[key] = result[key] = value
             elif "amount" in self.params[key]:
-                interpreter.symtable[key] = result[key] = self.params[key]["amount"]
+                value = self.params[key]["amount"]
             else:
                 raise ValueError(
-                    u"No suitable formula or static amount found " u"in {}".format(key)
+                    "No suitable formula or static amount found " "in {}".format(key)
                 )
+            result[key] = value
+            self.interpreter.add_symbols({key: value})
         return result
 
     def evaluate_and_set_amount_field(self):
         """Evaluate each formula. Updates the ``amount`` field of each parameter."""
         result = self.evaluate()
         for key, value in self.params.items():
-            value[u"amount"] = result[key]
+            value["amount"] = result[key]
         return result
 
     def evaluate_monte_carlo(self, iterations=1000):
         """Evaluate each formula using Monte Carlo and variable uncertainty data, if present.
 
         Formulas **must** return a one-dimensional array, or ``BroadcastingError`` is raised.
 
         Returns dictionary of ``{parameter name: numpy array}``."""
-        interpreter = Interpreter()
+        interpreter = self.interpreter
         result = {}
 
         def get_rng_sample(obj):
             if isinstance(obj, np.ndarray):
                 # Already a Monte Carlo sample
                 return obj
             if "uncertainty_type" not in obj:
                 if "uncertainty type" not in obj:
                     obj = obj.copy()
                     obj["uncertainty_type"] = 0
-                    obj["loc"] = obj["amount"]
                 else:
                     obj["uncertainty_type"] = obj["uncertainty type"]
+                obj["loc"] = obj.get("loc") or obj["amount"]
             kls = uncertainty_choices[obj["uncertainty_type"]]
             return kls.bounded_random_variables(kls.from_dicts(obj), iterations).ravel()
 
         def fix_shape(array):
             if array is None:
                 return np.zeros((iterations,))
             elif isinstance(array, Number):
@@ -211,24 +217,80 @@
 
         self.evaluate_and_set_amount_field()
 
         # Evaluate formulas in exchanges
         interpreter = self.get_interpreter()
         for obj in ds:
             if "formula" in obj and "amount" not in obj:
-                obj[u"amount"] = interpreter(obj["formula"])
+                obj["amount"] = interpreter(obj["formula"])
 
         # Changes in-place, but return anyway
         return ds
 
     def get_interpreter(self, evaluate_first=True):
-        """Get an instance of ``asteval.Interpreter`` that is prepopulated with global and local symbol names and values."""
+        """Get an instance of ``asteval.Interpreter`` that is prepopulated with global and local \
+        symbol names and values."""
         if evaluate_first:
             self.evaluate_and_set_amount_field()
 
-        interpreter = Interpreter()
+        interpreter = self.interpreter
         for key, value in self.global_params.items():
             interpreter.symtable[key] = value
         for key, value in self.params.items():
             interpreter.symtable[key] = value["amount"]
 
         return interpreter
+
+
+class PintParameterSet(ParameterSet):
+    def __init__(self, params, global_params=None, interpreter=None):
+        super().__init__(
+            params=params,
+            global_params=global_params,
+            interpreter=interpreter or PintInterpreter(),
+        )
+
+    def get_references(self):
+        """Create dictionary of parameter references"""
+        refs = {
+            key: self.interpreter.get_unknown_symbols(
+                value.get("formula"),
+                no_pint_units=self.all_param_names,  # ensures that parameter names are not accidentally parsed as units
+            )
+            for key, value in self.params.items()
+        }
+        refs.update({key: set() for key in self.global_params})
+        return refs
+
+    def evaluate(self):
+        """Evaluate each formula. Returns dictionary of parameter names and values."""
+        result = {}
+        for key in self.order:
+            if key in self.global_params:
+                value = self.global_params[key]
+            elif self.params[key].get("formula"):
+                value = self.interpreter(self.params[key]["formula"])
+            elif "amount" in self.params[key]:
+                value = self.params[key]["amount"]
+                value = PintWrapper.to_quantity(
+                    value, self.params[key].get("unit")
+                )  # add unit if given
+            else:
+                raise ValueError(
+                    "No suitable formula or static amount found " "in {}".format(key)
+                )
+            result[key] = value
+            self.interpreter.add_symbols({key: value})
+        return result
+
+    def evaluate_and_set_amount_field(self):
+        """
+        Evaluate each formula. Updates the ``amount`` field of each parameter. Also updates the ``unit`` field
+        if no unit is given.
+        """
+        result = self.evaluate()
+        for key, value in self.params.items():
+            self.interpreter.set_amount_and_unit(
+                obj=value,
+                quantity=result[key],
+            )
+        return result
```

### Comparing `bw2parameters-0.7/bw2parameters/utils.py` & `bw2parameters-1.1.0/bw2parameters/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,18 @@
+from typing import Union
 import ast
-
-import asteval
-
-try:
-    # Python 2
-    string_type = basestring
-except NameError:
-    # Python 3
-    string_type = str
-
-
-def _get_existing_symbols():
-    interpreter = asteval.Interpreter()
-    return set(interpreter.symtable)
-
-
-EXISTING_SYMBOLS = _get_existing_symbols()
-
-
-def get_symbols(expression):
-    interpreter = asteval.Interpreter()
-    nf = asteval.NameFinder()
-    nf.generic_visit(interpreter.parse(expression))
-    return set(nf.names).difference(EXISTING_SYMBOLS)
+import importlib.metadata
 
 
 def isidentifier(ident):
     """Determines, if string is valid Python identifier.
 
     Stolen from http://stackoverflow.com/questions/12700893/how-to-check-if-a-string-is-a-valid-python-identifier-including-keyword-check"""
 
-    if not isinstance(ident, string_type):
+    if not isinstance(ident, str):
         raise TypeError("expected str, but got {!r}".format(type(ident)))
 
     # Resulting AST of simple identifier is <Module [<Expr <Name "foo">>]>
     try:
         root = ast.parse(ident)
     except SyntaxError:
         return False
@@ -46,9 +24,20 @@
         or not isinstance(root.body[0].value, ast.Name)
         or root.body[0].value.id != ident
     ):
         return False
     return True
 
 
-def isstr(s):
-    return isinstance(s, string_type)
+def get_version_tuple() -> tuple:
+    def as_integer(x: str) -> Union[int, str]:
+        try:
+            return int(x)
+        except ValueError:
+            return x
+
+    return tuple(
+        as_integer(v)
+        for v in importlib.metadata.version("bw2parameters")
+        .strip()
+        .split(".")
+    )
```

### Comparing `bw2parameters-0.7/docs/Makefile` & `bw2parameters-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bw2parameters-0.7/docs/conf.py` & `bw2parameters-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw2parameters-0.7/docs/index.rst` & `bw2parameters-1.1.0/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -65,8 +65,28 @@
 Note the following:
 
 * Variables and formulas must be defined with unique names.
 * Variable and formula names can't contradict the existing built-in functions. Available functions are documented in the `asteval documentation <http://newville.github.io/asteval/basics.html#built-in-functions>`__.
 * Formulas should not include the equals sign; instead of ``{'formula': 'a = b + c', 'name': 'a'}`` do ``{'formula': 'b + c', 'name': 'a'}``.
 * Formulas can only reference defined variables.
 
+**New as of version 0.8:**
+
+You can evaluate formulas with units in them. In order for this to work, you need to install the optional dependency `pint <https://github.com/hgrecco/pint>`__. To do so, type ``pip install bw2parameters[pint]`` into your terminal. Example usage:
+
+.. code-block:: python
+
+    In [12]: from bw2parameters import PintParameterSet
+    In [13]: ps = PintParameterSet({
+   ...:         'A': {'formula': '1 m'},
+   ...:         'B': {'formula': 'A + 200 mm'},
+   ...:         'C': {'formula': 'B * kg/m'},
+   ...:         'D': {'formula': 'A * B * C'},
+   ...:     })
+    In [14]: ps.evaluate()
+    Out[4]:
+    {'A': 1 <Unit('meter')>,
+    'B': 1.2 <Unit('meter')>,
+    'C': 1.2 <Unit('kilogram')>,
+    'D': 1.44 <Unit('kilogram * meter ** 2')>}
+
 Brightway2-parameters is Python 2.7 & 3.3+ compatible, has 100% test coverage, and is 2-clause BSD licensed and free. Source code `on Github <https://github.com/brightway-lca/brightway2-parameters>`__.
```

### Comparing `bw2parameters-0.7/docs/make.bat` & `bw2parameters-1.1.0/docs/make.bat`

 * *Files identical despite different names*

