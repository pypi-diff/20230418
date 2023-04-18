# Comparing `tmp/fast_depends-1.1.0.tar.gz` & `tmp/fast_depends-1.1.1.tar.gz`

## Comparing `fast_depends-1.1.0.tar` & `fast_depends-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/__init__.py
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/construct.py
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/injector.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/model.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/provider.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/types.py
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/usage.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/library/model.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.0/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.0/README.md
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 fast_depends-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 fast_depends-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/__init__.py
+-rw-r--r--   0        0        0     7989 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/construct.py
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/injector.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/model.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/provider.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/types.py
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/usage.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fast_depends-1.1.1/fast_depends/library/model.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.1.1/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.1/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.1/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.1/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.1/README.md
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 fast_depends-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 fast_depends-1.1.1/PKG-INFO
```

### Comparing `fast_depends-1.1.0/CONTRIBUTING.md` & `fast_depends-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/.github/workflows/documentation.yml` & `fast_depends-1.1.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/.github/workflows/publish_coverage.yml` & `fast_depends-1.1.1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/.github/workflows/publish_pypi.yml` & `fast_depends-1.1.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/.github/workflows/tests.yml` & `fast_depends-1.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/fast_depends/construct.py` & `fast_depends-1.1.1/fast_depends/construct.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,25 @@
             param_name,
         )
     else:
         field_info = FieldInfo(default=default)
 
     alias = field_info.alias or param_name
 
+    if custom and custom.required is True:
+        required = True
+    else:
+        required = field_info.default in (Required, Undefined, inspect._empty)
+
     field = create_response_field(
         name=param_name,
         type_=annotation,
-        default=field_info.default if depends is None else None,
+        default=None if any((depends, custom)) else field_info.default,
         alias=alias,
-        required=field_info.default in (Required, Undefined, inspect._empty),
+        required=required,
         field_info=field_info,
     )
 
     return custom, depends, field
 
 
 def get_typed_signature(call: AnyCallable) -> inspect.Signature:
```

### Comparing `fast_depends-1.1.0/fast_depends/injector.py` & `fast_depends-1.1.1/fast_depends/injector.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/fast_depends/model.py` & `fast_depends-1.1.1/fast_depends/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/fast_depends/usage.py` & `fast_depends-1.1.1/fast_depends/usage.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/fast_depends/utils.py` & `fast_depends-1.1.1/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/LICENSE` & `fast_depends-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/README.md` & `fast_depends-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/pyproject.toml` & `fast_depends-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.0/PKG-INFO` & `fast_depends-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.1.0
+Version: 1.1.1
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

