# Comparing `tmp/airflow-provider-sqream-blue-0.0.7.tar.gz` & `tmp/airflow-provider-sqream-blue-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow-provider-sqream-blue-0.0.7.tar", last modified: Tue Apr 18 15:43:52 2023, max compression
+gzip compressed data, was "airflow-provider-sqream-blue-0.0.8.tar", last modified: Tue Apr 18 16:03:39 2023, max compression
```

## Comparing `airflow-provider-sqream-blue-0.0.7.tar` & `airflow-provider-sqream-blue-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/sqream_blue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/sqream_blue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/sqream_blue/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/sqream_blue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/sqream_blue.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `airflow-provider-sqream-blue-0.0.7/LICENSE` & `airflow-provider-sqream-blue-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.7/PKG-INFO` & `airflow-provider-sqream-blue-0.0.8/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-Metadata-Version: 2.1
-Name: airflow-provider-sqream-blue
-Version: 0.0.7
-Summary: About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.
-Home-page: https://github.com/SQream/apache-airflow-providers-sqream-blue
-Author: SQream
-Author-email: info@sqream.com
-License: Apache License 2.0
-Platform: UNKNOWN
-Classifier: Framework :: Apache Airflow
-Classifier: Framework :: Apache Airflow :: Provider
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 apache-airflow-providers-sqream-blue
 =====================================
 Apache Airflow is a popular open source orchestration tool. It allows users to write complex workflows composed of multiple kinds of actions and services using DAGs, and to schedule, debug and monitor workflow runs.
 
 Different kind of actions are represented with specialized Python classes, called “Operators”. Each SaaS database vendor can build one or more customized Operators for performing different DB operations (e.g. execute arbitrary SQL statements, schedule DB job runs etc.).
 
 This package is an Operator for executing SQL statments on SQream Blue using Python connector.
 
 
 Requirements
 -------------
 
-* Python 3.7+
+* Python 3.9+
 
 
 Installing the Airflow-provider-sqream-blue
 -------------------------------------------
 The Airflow provider sqream-blue is available via `PyPi <https://pypi.org/project/airflow-provider-sqream-blue/>`_.
 
 Install the connector with ``pip3``:
@@ -123,9 +108,7 @@
 
 
 The execution of the Dag File -
 
 .. image:: images/execution_dag.png
    :width: 600
  
-
-
```

### Comparing `airflow-provider-sqream-blue-0.0.7/README.rst` & `airflow-provider-sqream-blue-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: airflow-provider-sqream-blue
+Version: 0.0.8
+Summary: About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.
+Home-page: https://github.com/SQream/apache-airflow-providers-sqream-blue
+Author: SQream
+Author-email: info@sqream.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Apache Airflow
+Classifier: Framework :: Apache Airflow :: Provider
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 apache-airflow-providers-sqream-blue
 =====================================
 Apache Airflow is a popular open source orchestration tool. It allows users to write complex workflows composed of multiple kinds of actions and services using DAGs, and to schedule, debug and monitor workflow runs.
 
 Different kind of actions are represented with specialized Python classes, called “Operators”. Each SaaS database vendor can build one or more customized Operators for performing different DB operations (e.g. execute arbitrary SQL statements, schedule DB job runs etc.).
 
 This package is an Operator for executing SQL statments on SQream Blue using Python connector.
 
 
 Requirements
 -------------
 
-* Python 3.7+
+* Python 3.9+
 
 
 Installing the Airflow-provider-sqream-blue
 -------------------------------------------
 The Airflow provider sqream-blue is available via `PyPi <https://pypi.org/project/airflow-provider-sqream-blue/>`_.
 
 Install the connector with ``pip3``:
@@ -108,7 +126,9 @@
 
 
 The execution of the Dag File -
 
 .. image:: images/execution_dag.png
    :width: 600
  
+
+
```

### Comparing `airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/PKG-INFO` & `airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sqream-blue
-Version: 0.0.7
+Version: 0.0.8
 Summary: About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.
 Home-page: https://github.com/SQream/apache-airflow-providers-sqream-blue
 Author: SQream
 Author-email: info@sqream.com
 License: Apache License 2.0
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
-Requires-Python: ~=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 apache-airflow-providers-sqream-blue
 =====================================
 Apache Airflow is a popular open source orchestration tool. It allows users to write complex workflows composed of multiple kinds of actions and services using DAGs, and to schedule, debug and monitor workflow runs.
 
@@ -21,15 +24,15 @@
 
 This package is an Operator for executing SQL statments on SQream Blue using Python connector.
 
 
 Requirements
 -------------
 
-* Python 3.7+
+* Python 3.9+
 
 
 Installing the Airflow-provider-sqream-blue
 -------------------------------------------
 The Airflow provider sqream-blue is available via `PyPi <https://pypi.org/project/airflow-provider-sqream-blue/>`_.
 
 Install the connector with ``pip3``:
```

### Comparing `airflow-provider-sqream-blue-0.0.7/setup.py` & `airflow-provider-sqream-blue-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 """Perform the package sqream_blue-provider setup."""
 setup(
     name='airflow-provider-sqream-blue',
-    version="0.0.7",
+    version="0.0.8",
     description='About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
+    classifiers=[
+        "Programming Language :: Python :: 3.9",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+        "Framework :: Apache Airflow",
+        "Framework :: Apache Airflow :: Provider",
+    ],
+    python_requires='>=3.9',
     entry_points={
         "apache_airflow_provider": [
             "provider_info=sqream_blue.__init__:get_provider_info"
         ]
     },
     license='Apache License 2.0',
     packages=['sqream_blue', 'sqream_blue.hooks','sqream_blue.operators'],
-    install_requires=['apache-airflow>=2.0', 'apache-airflow-providers-common-sql==1.3.2', 'pysqream-blue==1.0.23'],
+    install_requires=['pysqream-blue>=1.0.26', 'apache-airflow>=2.0', 'apache-airflow-providers-common-sql==1.3.2'],
     setup_requires=['setuptools', 'wheel'],
     author='SQream',
     author_email='info@sqream.com',
     url='https://github.com/SQream/apache-airflow-providers-sqream-blue',
-    classifiers=[
-        "Framework :: Apache Airflow",
-        "Framework :: Apache Airflow :: Provider",
-    ],
-    python_requires='~=3.7',
 )
```

### Comparing `airflow-provider-sqream-blue-0.0.7/sqream_blue/__init__.py` & `airflow-provider-sqream-blue-0.0.8/sqream_blue/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/sqream_blue.py` & `airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/sqream_blue.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     provider manager from that version.
     """
 
     def dec(func):
         @wraps(func)
         def inner():
             field_behaviors = func()
-            conn_attrs = {"host", "login", "password", "port", "database"}
+            conn_attrs = {"host", "access_token", "port", "extra"}
 
             def _ensure_prefix(field):
                 if field not in conn_attrs and not field.startswith("extra__"):
                     return f"extra__{conn_type}__{field}"
                 else:
                     return field
 
@@ -47,36 +47,37 @@
     def get_connection_form_widgets() -> dict[str, Any]:
         """Returns connection widgets to add to connection form"""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
 
         return {
-            "database": StringField(lazy_gettext("Database"), widget=BS3TextFieldWidget())
+            "database": StringField(lazy_gettext("Database"), widget=BS3TextFieldWidget()),
+            "access_token": StringField(lazy_gettext("Access token"), widget=BS3TextFieldWidget())
         }
 
     @staticmethod
     @_ensure_prefixes(conn_type="sqream_blue")
     def get_ui_field_behaviour() -> dict[str, Any]:
         """Returns custom field behaviour"""
-
-        return {
-            "hidden_fields": ["port", "schema", "extra"],
-            "relabeling": {},
-            "placeholders": {
+        fileds = {
                 "host": "enter host domain to connect to SQream",
-                "login": "enter username to connect to SQream",
-                "password": "enter password to connect to SQream",
+                "Access token": "enter access token to connect to SQream",
                 "database": "enter db name to connect to SQream",
-            },
+            }
+        return {
+            "hidden_fields": ["port", "schema", "extra", "login", "password"],
+            "relabeling": {},
+            "placeholders": fileds,
         }
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.database = kwargs.pop("database", None)
+        self.access_token = kwargs.pop("access_token", None)
         self.query_ids: list[str] = []
 
     def _get_field(self, extra_dict, field_name):
         backcompat_prefix = "extra__sqream_blue__"
         backcompat_key = f"{backcompat_prefix}{field_name}"
         if field_name.startswith("extra__"):
             raise ValueError(
@@ -99,18 +100,18 @@
         """
         One method to fetch connection params as a dict
         used in get_uri() and get_connection()
         """
         conn = self.get_connection(self.sqream_blue_conn_id)  # type: ignore[attr-defined]
         extra_dict = conn.extra_dejson
         database = self._get_field(extra_dict, "database") or "master"
+        access_token = self._get_field(extra_dict, "access_token")
         conn_config = {
             "host": conn.host,
-            "username": conn.login,
-            "password": conn.password,
+            "access_token": self.access_token or access_token,
             "database": self.database or database
         }
         return conn_config
 
     def get_conn(self):
         """Returns a sqream_blue.connection object"""
         conn_config = self._get_conn_params()
```

### Comparing `airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/sqream_blue.py` & `airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/sqream_blue.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,22 @@
     ui_color = "#ededed"
 
     def __init__(
             self,
             *,
             sqream_blue_conn_id: str = "sqream_blue_default",
             database: str | None = None,
+            access_token: str | None = None,
             **kwargs,
     ) -> None:
-        if any([database]):
+        if any([database]) and any([access_token]):
             hook_params = kwargs.pop("hook_params", {})
             kwargs["hook_params"] = {
                 "database": database,
+                "access_token": access_token,
                 **hook_params,
             }
         super().__init__(conn_id=sqream_blue_conn_id, **kwargs)
 
     def _process_output(self, results: list[Any], descriptions: list[Sequence[Sequence] | None]) -> list[Any]:
         validated_descriptions: list[Sequence[Sequence]] = []
         for idx, description in enumerate(descriptions):
```

