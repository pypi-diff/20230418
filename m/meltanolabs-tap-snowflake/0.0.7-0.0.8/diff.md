# Comparing `tmp/meltanolabs_tap_snowflake-0.0.7.tar.gz` & `tmp/meltanolabs_tap_snowflake-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_tap_snowflake-0.0.7.tar", max compression
+gzip compressed data, was "meltanolabs_tap_snowflake-0.0.8.tar", max compression
```

## Comparing `meltanolabs_tap_snowflake-0.0.7.tar` & `meltanolabs_tap_snowflake-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1047 2022-12-02 15:14:13.880468 meltanolabs_tap_snowflake-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       28 2022-12-02 15:14:03.252464 meltanolabs_tap_snowflake-0.0.7/tap_snowflake/__init__.py
--rw-r--r--   0        0        0     8595 2022-12-02 15:14:03.252464 meltanolabs_tap_snowflake-0.0.7/tap_snowflake/client.py
--rw-r--r--   0        0        0     1745 2022-12-02 15:14:03.252464 meltanolabs_tap_snowflake-0.0.7/tap_snowflake/tap.py
--rw-r--r--   0        0        0       36 2022-12-02 15:14:03.252464 meltanolabs_tap_snowflake-0.0.7/tap_snowflake/tests/__init__.py
--rw-r--r--   0        0        0      678 2022-12-02 15:14:03.252464 meltanolabs_tap_snowflake-0.0.7/tap_snowflake/tests/test_core.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 meltanolabs_tap_snowflake-0.0.7/setup.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 meltanolabs_tap_snowflake-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1047 2022-12-05 08:39:50.096731 meltanolabs_tap_snowflake-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       28 2022-12-05 08:39:36.116955 meltanolabs_tap_snowflake-0.0.8/tap_snowflake/__init__.py
+-rw-r--r--   0        0        0     8595 2022-12-05 08:39:36.116955 meltanolabs_tap_snowflake-0.0.8/tap_snowflake/client.py
+-rw-r--r--   0        0        0     1745 2022-12-05 08:39:36.116955 meltanolabs_tap_snowflake-0.0.8/tap_snowflake/tap.py
+-rw-r--r--   0        0        0       36 2022-12-05 08:39:36.116955 meltanolabs_tap_snowflake-0.0.8/tap_snowflake/tests/__init__.py
+-rw-r--r--   0        0        0      678 2022-12-05 08:39:36.116955 meltanolabs_tap_snowflake-0.0.8/tap_snowflake/tests/test_core.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 meltanolabs_tap_snowflake-0.0.8/setup.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 meltanolabs_tap_snowflake-0.0.8/PKG-INFO
```

### Comparing `meltanolabs_tap_snowflake-0.0.7/pyproject.toml` & `meltanolabs_tap_snowflake-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-tap-snowflake"
-version = "v0.0.7"
+version = "v0.0.8"
 description = "`tap-snowflake` is a Singer tap for Snowflake, built with the Meltano SDK for Singer Taps."
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
 license = "Apache 2.0"
```

### Comparing `meltanolabs_tap_snowflake-0.0.7/tap_snowflake/client.py` & `meltanolabs_tap_snowflake-0.0.8/tap_snowflake/client.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_snowflake-0.0.7/tap_snowflake/tap.py` & `meltanolabs_tap_snowflake-0.0.8/tap_snowflake/tap.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_snowflake-0.0.7/tap_snowflake/tests/test_core.py` & `meltanolabs_tap_snowflake-0.0.8/tap_snowflake/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_snowflake-0.0.7/setup.py` & `meltanolabs_tap_snowflake-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'snowflake-sqlalchemy>=1.4.3,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['tap-snowflake = tap_snowflake.tap:TapSnowflake.cli']}
 
 setup_kwargs = {
     'name': 'meltanolabs-tap-snowflake',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': '`tap-snowflake` is a Singer tap for Snowflake, built with the Meltano SDK for Singer Taps.',
     'long_description': 'None',
     'author': 'Ken Payne',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `meltanolabs_tap_snowflake-0.0.7/PKG-INFO` & `meltanolabs_tap_snowflake-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-tap-snowflake
-Version: 0.0.7
+Version: 0.0.8
 Summary: `tap-snowflake` is a Singer tap for Snowflake, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

