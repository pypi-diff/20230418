# Comparing `tmp/dbt_feature_flags-0.5.0.tar.gz` & `tmp/dbt_feature_flags-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_feature_flags-0.5.0.tar", max compression
+gzip compressed data, was "dbt_feature_flags-0.5.1.tar", max compression
```

## Comparing `dbt_feature_flags-0.5.0.tar` & `dbt_feature_flags-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10142 2022-11-06 16:29:25.073909 dbt_feature_flags-0.5.0/LICENSE
--rw-r--r--   0        0        0     9611 2022-11-06 16:27:14.455036 dbt_feature_flags-0.5.0/README.md
--rw-r--r--   0        0        0      598 2022-11-06 16:30:32.539379 dbt_feature_flags-0.5.0/dbt_feature_flags/__init__.py
--rw-r--r--   0        0        0     3292 2022-11-06 16:29:55.680821 dbt_feature_flags-0.5.0/dbt_feature_flags/base.py
--rw-r--r--   0        0        0     3922 2023-04-18 06:39:35.939005 dbt_feature_flags-0.5.0/dbt_feature_flags/harness.py
--rw-r--r--   0        0        0     2524 2022-11-06 16:30:04.858005 dbt_feature_flags-0.5.0/dbt_feature_flags/launchdarkly.py
--rw-r--r--   0        0        0     3241 2023-04-18 06:46:15.524831 dbt_feature_flags-0.5.0/dbt_feature_flags/patch.py
--rw-r--r--   0        0        0      609 2023-04-18 06:39:10.390159 dbt_feature_flags-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       70 2022-07-30 05:05:11.823869 dbt_feature_flags-0.5.0/zzz_dbt_feature_flags.pth
--rw-r--r--   0        0        0    10353 1970-01-01 00:00:00.000000 dbt_feature_flags-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2022-11-06 16:29:25.073909 dbt_feature_flags-0.5.1/LICENSE
+-rw-r--r--   0        0        0     9611 2022-11-06 16:27:14.455036 dbt_feature_flags-0.5.1/README.md
+-rw-r--r--   0        0        0      598 2022-11-06 16:30:32.539379 dbt_feature_flags-0.5.1/dbt_feature_flags/__init__.py
+-rw-r--r--   0        0        0     3292 2022-11-06 16:29:55.680821 dbt_feature_flags-0.5.1/dbt_feature_flags/base.py
+-rw-r--r--   0        0        0     3922 2023-04-18 19:13:52.168228 dbt_feature_flags-0.5.1/dbt_feature_flags/harness.py
+-rw-r--r--   0        0        0     2524 2022-11-06 16:30:04.858005 dbt_feature_flags-0.5.1/dbt_feature_flags/launchdarkly.py
+-rw-r--r--   0        0        0     3383 2023-04-18 19:13:41.242843 dbt_feature_flags-0.5.1/dbt_feature_flags/patch.py
+-rw-r--r--   0        0        0      609 2023-04-18 19:14:31.319044 dbt_feature_flags-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2022-07-30 05:05:11.823869 dbt_feature_flags-0.5.1/zzz_dbt_feature_flags.pth
+-rw-r--r--   0        0        0    10353 1970-01-01 00:00:00.000000 dbt_feature_flags-0.5.1/PKG-INFO
```

### Comparing `dbt_feature_flags-0.5.0/LICENSE` & `dbt_feature_flags-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.5.0/README.md` & `dbt_feature_flags-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.5.0/dbt_feature_flags/__init__.py` & `dbt_feature_flags-0.5.1/dbt_feature_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.5.0/dbt_feature_flags/base.py` & `dbt_feature_flags-0.5.1/dbt_feature_flags/base.py`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.5.0/dbt_feature_flags/harness.py` & `dbt_feature_flags-0.5.1/dbt_feature_flags/harness.py`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.5.0/dbt_feature_flags/launchdarkly.py` & `dbt_feature_flags-0.5.1/dbt_feature_flags/launchdarkly.py`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.5.0/dbt_feature_flags/patch.py` & `dbt_feature_flags-0.5.1/dbt_feature_flags/patch.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,18 +75,18 @@
         string: str,
         ctx: t.Dict[str, t.Any],
         node=None,
         capture_macros: bool = False,
         native: bool = False,
     ):
         if client is _MOCK_CLIENT:
-            ctx["feature_flag"] = ctx["var"]
-            ctx["feature_flag_str"] = ctx["var"]
-            ctx["feature_flag_num"] = ctx["var"]
-            ctx["feature_flag_json"] = ctx["var"]
+            ctx["feature_flag"] = ctx.get("var", lambda _, default=False: default)
+            ctx["feature_flag_str"] = ctx.get("var", lambda _, default="": default)
+            ctx["feature_flag_num"] = ctx.get("var", lambda _, default=0: default)
+            ctx["feature_flag_json"] = ctx.get("var", lambda _, default={}: default)
         else:
             ctx["feature_flag"] = client.bool_variation
             ctx["feature_flag_str"] = client.string_variation
             ctx["feature_flag_num"] = client.number_variation
             ctx["feature_flag_json"] = client.json_variation
         return fn(string, ctx, node, capture_macros, native)
```

### Comparing `dbt_feature_flags-0.5.0/pyproject.toml` & `dbt_feature_flags-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-feature-flags"
-version = "0.5.0"
+version = "0.5.1"
 description = "Use feature flags in dbt models"
 authors = ["z3z1ma <butler.alex2010@gmail.com>"]
 include = ["zzz_dbt_feature_flags.pth"]
 readme = "README.md"
 repository = "https://github.com/z3z1ma/dbt-feature-flags"
 homepage = "https://github.com/z3z1ma/dbt-feature-flags"
```

### Comparing `dbt_feature_flags-0.5.0/PKG-INFO` & `dbt_feature_flags-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-feature-flags
-Version: 0.5.0
+Version: 0.5.1
 Summary: Use feature flags in dbt models
 Home-page: https://github.com/z3z1ma/dbt-feature-flags
 Author: z3z1ma
 Author-email: butler.alex2010@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

