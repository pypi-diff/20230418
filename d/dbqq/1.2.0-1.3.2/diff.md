# Comparing `tmp/dbqq-1.2.0.tar.gz` & `tmp/dbqq-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbqq-1.2.0.tar", last modified: Sat Apr 15 12:13:03 2023, max compression
+gzip compressed data, was "dbqq-1.3.2.tar", last modified: Tue Apr 18 09:58:53 2023, max compression
```

## Comparing `dbqq-1.2.0.tar` & `dbqq-1.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.127417 dbqq-1.2.0/
--rw-rw-rw-   0        0        0    13111 2023-04-15 12:13:03.126417 dbqq-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    12588 2023-04-15 12:06:19.000000 dbqq-1.2.0/README.md
--rw-rw-rw-   0        0        0     1083 2023-04-15 12:06:19.000000 dbqq-1.2.0/license.md
--rw-rw-rw-   0        0        0     1123 2023-04-15 12:12:48.000000 dbqq-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 12:13:03.128406 dbqq-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.003666 dbqq-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.031683 dbqq-1.2.0/src/dbqq/
--rw-rw-rw-   0        0        0      134 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.062403 dbqq-1.2.0/src/dbqq/cli/
--rw-rw-rw-   0        0        0      967 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/cli/clean_connections.py
--rw-rw-rw-   0        0        0      713 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/cli/initialize_connections.py
--rw-rw-rw-   0        0        0     1422 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/cli/run_query.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.082407 dbqq-1.2.0/src/dbqq/connectors/
--rw-rw-rw-   0        0        0     1017 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/connectors/__init__.py
--rw-rw-rw-   0        0        0     5604 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/connectors/_base.py
--rw-rw-rw-   0        0        0     1778 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/connectors/_polar_connector.py
--rw-rw-rw-   0        0        0     5476 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/connectors/databricks.py
--rw-rw-rw-   0        0        0     2888 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/connectors/mssql.py
--rw-rw-rw-   0        0        0     4725 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/connectors/oracle.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.085407 dbqq-1.2.0/src/dbqq/enums/
--rw-rw-rw-   0        0        0       46 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.092414 dbqq-1.2.0/src/dbqq/enums/parsed/
--rw-rw-rw-   0        0        0       40 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/enums/parsed/__init__.py
--rw-rw-rw-   0        0        0      755 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/enums/parsed/sql.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.098410 dbqq-1.2.0/src/dbqq/security/
--rw-rw-rw-   0        0        0      112 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.111413 dbqq-1.2.0/src/dbqq/security/cli/
--rw-rw-rw-   0        0        0       54 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/cli/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/cli/decrypt_yaml.py
--rw-rw-rw-   0        0        0     1036 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/cli/encrypt_yaml.py
--rw-rw-rw-   0        0        0     1708 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/cli/write_keys.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.122415 dbqq-1.2.0/src/dbqq/security/functions/
--rw-rw-rw-   0        0        0      119 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/functions/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/functions/_functions.py
--rw-rw-rw-   0        0        0     4166 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/functions/_yaml.py
--rw-rw-rw-   0        0        0     2330 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/security/helpers.py
--rw-rw-rw-   0        0        0     5311 2023-04-15 12:06:19.000000 dbqq-1.2.0/src/dbqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:13:03.051400 dbqq-1.2.0/src/dbqq.egg-info/
--rw-rw-rw-   0        0        0    13111 2023-04-15 12:13:02.000000 dbqq-1.2.0/src/dbqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-04-15 12:13:02.000000 dbqq-1.2.0/src/dbqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 12:13:02.000000 dbqq-1.2.0/src/dbqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-04-15 12:13:02.000000 dbqq-1.2.0/src/dbqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      141 2023-04-15 12:13:02.000000 dbqq-1.2.0/src/dbqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 12:13:02.000000 dbqq-1.2.0/src/dbqq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.651556 dbqq-1.3.2/
+-rw-rw-rw-   0        0        0    14132 2023-04-18 09:58:53.648543 dbqq-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13402 2023-04-18 08:39:10.000000 dbqq-1.3.2/README.md
+-rw-rw-rw-   0        0        0     1083 2023-04-18 08:39:10.000000 dbqq-1.3.2/license.md
+-rw-rw-rw-   0        0        0     1289 2023-04-18 09:57:42.000000 dbqq-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:58:53.652558 dbqq-1.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.519047 dbqq-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.546056 dbqq-1.3.2/src/dbqq/
+-rw-rw-rw-   0        0        0      134 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.578095 dbqq-1.3.2/src/dbqq/cli/
+-rw-rw-rw-   0        0        0      967 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/cli/clean_connections.py
+-rw-rw-rw-   0        0        0      713 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/cli/initialize_connections.py
+-rw-rw-rw-   0        0        0     1422 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/cli/run_query.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.599545 dbqq-1.3.2/src/dbqq/connectors/
+-rw-rw-rw-   0        0        0     1017 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7038 2023-04-18 08:39:55.000000 dbqq-1.3.2/src/dbqq/connectors/_base.py
+-rw-rw-rw-   0        0        0     1778 2023-04-18 08:40:16.000000 dbqq-1.3.2/src/dbqq/connectors/_polar_connector.py
+-rw-rw-rw-   0        0        0     5634 2023-04-18 09:58:15.000000 dbqq-1.3.2/src/dbqq/connectors/databricks.py
+-rw-rw-rw-   0        0        0     2906 2023-04-18 09:58:15.000000 dbqq-1.3.2/src/dbqq/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4747 2023-04-18 09:58:15.000000 dbqq-1.3.2/src/dbqq/connectors/oracle.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.601545 dbqq-1.3.2/src/dbqq/enums/
+-rw-rw-rw-   0        0        0       46 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.610534 dbqq-1.3.2/src/dbqq/enums/parsed/
+-rw-rw-rw-   0        0        0       40 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/enums/parsed/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/enums/parsed/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.617548 dbqq-1.3.2/src/dbqq/security/
+-rw-rw-rw-   0        0        0      112 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.633540 dbqq-1.3.2/src/dbqq/security/cli/
+-rw-rw-rw-   0        0        0       54 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/decrypt_yaml.py
+-rw-rw-rw-   0        0        0     1036 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/encrypt_yaml.py
+-rw-rw-rw-   0        0        0     1708 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/write_keys.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.645549 dbqq-1.3.2/src/dbqq/security/functions/
+-rw-rw-rw-   0        0        0      119 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/functions/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/functions/_functions.py
+-rw-rw-rw-   0        0        0     4166 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/functions/_yaml.py
+-rw-rw-rw-   0        0        0     2330 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/helpers.py
+-rw-rw-rw-   0        0        0     5311 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.567082 dbqq-1.3.2/src/dbqq.egg-info/
+-rw-rw-rw-   0        0        0    14132 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      339 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/top_level.txt
```

### Comparing `dbqq-1.2.0/PKG-INFO` & `dbqq-1.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: dbqq
-Version: 1.2.0
-Author-email: Chris Mamon <chrisam1993@live.com>
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: license.md
-
 # Database Quick Query
 
 - [Database Quick Query](#database-quick-query)
   - [Environment Variables](#environment-variables)
   - [Initialization](#initialization)
   - [Connection Configuration](#connection-configuration)
   - [Encrypting Configs](#encrypting-configs)
@@ -26,14 +12,15 @@
     - [Getting Basic Table Metadata](#getting-basic-table-metadata)
     - [Running Queries from a File](#running-queries-from-a-file)
       - [Extracting queries and connections from a file](#extracting-queries-and-connections-from-a-file)
         - [Basic Connection No Cache](#basic-connection-no-cache)
         - [Connection With Cache](#connection-with-cache)
         - [Connection With Cache and Date Lower Bound](#connection-with-cache-and-date-lower-bound)
     - [Parsing Files](#parsing-files)
+    - [Jinja Templates](#jinja-templates)
   - [Common Table Expressions](#common-table-expressions)
     - [Rollback](#rollback)
   - [Databricks Development](#databricks-development)
   - [CLI Tools](#cli-tools)
     - [dbqq-clean-connections](#dbqq-clean-connections)
     - [dbqq-run-sql](#dbqq-run-sql)
 
@@ -365,14 +352,64 @@
 from dbqq import utils
 
 enum = utils.parse_file("<path to file>")
 ```
 
 enums for parsed sql can be found in connectors.enums.parsed.sql
 
+### Jinja Templates
+
+We can parse jinja templates, let's say we have a template called `test_query.sql.j2`
+
+```jinja
+select
+{% for item in  columns %}
+{% if loop.last %}
+    {{ item }}
+{% else %}
+    {{ item }},
+{% endif %}
+{% endfor %}
+from
+  some.table
+```
+
+We can create a `RenderedTemplateLoader` from it using the following
+
+```python
+import dbqq.connectors as dbc
+
+conn = dbc.<source>.<conn>()
+
+rendered_template_loader = conn.render_template(
+    "test_query.sql.j2",
+    columns=[
+      "col1",
+      "col2",
+      "col3",
+      "col4"
+    ],
+)
+
+# will return a object that shows the renderedquery
+
+"""
+select
+  col1,
+  col2,
+  col3,
+  col4
+from
+  some.table
+"""
+
+table = rendered_template_loader.execute()
+
+```
+
 ## Common Table Expressions
 
 We can construct a common table expression with the following method
 
 ```python
 from dbqq import utils
 from triple_quote_clean import TripleQuoteCleaner
```

### Comparing `dbqq-1.2.0/README.md` & `dbqq-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: dbqq
+Version: 1.3.2
+Summary: quickly connect to and query databases
+Author-email: Chris Mamon <chrisam1993@live.com>
+Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
+Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: license.md
+
 # Database Quick Query
 
 - [Database Quick Query](#database-quick-query)
   - [Environment Variables](#environment-variables)
   - [Initialization](#initialization)
   - [Connection Configuration](#connection-configuration)
   - [Encrypting Configs](#encrypting-configs)
@@ -12,14 +29,15 @@
     - [Getting Basic Table Metadata](#getting-basic-table-metadata)
     - [Running Queries from a File](#running-queries-from-a-file)
       - [Extracting queries and connections from a file](#extracting-queries-and-connections-from-a-file)
         - [Basic Connection No Cache](#basic-connection-no-cache)
         - [Connection With Cache](#connection-with-cache)
         - [Connection With Cache and Date Lower Bound](#connection-with-cache-and-date-lower-bound)
     - [Parsing Files](#parsing-files)
+    - [Jinja Templates](#jinja-templates)
   - [Common Table Expressions](#common-table-expressions)
     - [Rollback](#rollback)
   - [Databricks Development](#databricks-development)
   - [CLI Tools](#cli-tools)
     - [dbqq-clean-connections](#dbqq-clean-connections)
     - [dbqq-run-sql](#dbqq-run-sql)
 
@@ -351,14 +369,64 @@
 from dbqq import utils
 
 enum = utils.parse_file("<path to file>")
 ```
 
 enums for parsed sql can be found in connectors.enums.parsed.sql
 
+### Jinja Templates
+
+We can parse jinja templates, let's say we have a template called `test_query.sql.j2`
+
+```jinja
+select
+{% for item in  columns %}
+{% if loop.last %}
+    {{ item }}
+{% else %}
+    {{ item }},
+{% endif %}
+{% endfor %}
+from
+  some.table
+```
+
+We can create a `RenderedTemplateLoader` from it using the following
+
+```python
+import dbqq.connectors as dbc
+
+conn = dbc.<source>.<conn>()
+
+rendered_template_loader = conn.render_template(
+    "test_query.sql.j2",
+    columns=[
+      "col1",
+      "col2",
+      "col3",
+      "col4"
+    ],
+)
+
+# will return a object that shows the renderedquery
+
+"""
+select
+  col1,
+  col2,
+  col3,
+  col4
+from
+  some.table
+"""
+
+table = rendered_template_loader.execute()
+
+```
+
 ## Common Table Expressions
 
 We can construct a common table expression with the following method
 
 ```python
 from dbqq import utils
 from triple_quote_clean import TripleQuoteCleaner
```

### Comparing `dbqq-1.2.0/license.md` & `dbqq-1.3.2/license.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/pyproject.toml` & `dbqq-1.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires      = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbqq"
-version = "1.2.0"
+description = "quickly connect to and query databases"
+version = "1.3.2"
 readme = "README.md"
 dependencies = [
-  "tabulate==0.9.0",
-  "rsa==4.9",
-  "pyaml==21.10.1",
-  "polars==0.16.14",
-  "databricks-sql-connector==2.4.0",
-  "pyarrow==11.0.0",
-  "connectorx==0.3.1",
+  "tabulate",
+  "rsa",
+  "pyaml",
+  "polars",
+  "databricks-sql-connector",
+  "pyarrow",
+  "connectorx",
   "triple-quote-clean"
 ]
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
@@ -25,14 +26,18 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 authors = [
     {name = "Chris Mamon", email="chrisam1993@live.com"}
 ]
 
+[project.urls]
+"Homepage" = "https://github.com/Chr1sC0de/database-quick-query"
+"Bug Tracker" = "https://github.com/Chr1sC0de/database-quick-query/issues"
+
 [project.scripts]
 dbqq-write-keys = "dbqq.security.cli.write_keys:run"
 dbqq-encrypt-yaml = "dbqq.security.cli.encrypt_yaml:run"
 dbqq-decrypt-yaml = "dbqq.security.cli.decrypt_yaml:run"
 dbqq-run-sql = "dbqq.cli.run_query:run"
 dbqq-clean-connections = "dbqq.cli.clean_connections:run"
-dbqq-initialize-connections = "dbqq.cli.initialize_connections:run"
+dbqq-initialize-connections = "dbqq.cli.initialize_connections:run"
```

### Comparing `dbqq-1.2.0/src/dbqq/cli/clean_connections.py` & `dbqq-1.3.2/src/dbqq/cli/clean_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/cli/initialize_connections.py` & `dbqq-1.3.2/src/dbqq/cli/initialize_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/cli/run_query.py` & `dbqq-1.3.2/src/dbqq/cli/run_query.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/connectors/__init__.py` & `dbqq-1.3.2/src/dbqq/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/connectors/_base.py` & `dbqq-1.3.2/src/dbqq/connectors/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 import re
+import jinja2.nativetypes
 import yaml
 import polars as pl
 import pathlib as pt
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from uuid import uuid1
 
 
 class Base(ABC):
     to_cache: bool = False
+    description_query: str = None
+
+    class RenderedTemplateLoader:
+        def __init__(self, query: str, connection: "Base"):
+            self.query = query
+            self.connection = connection
+
+        def execute(self, *args, **kwargs) -> pl.LazyFrame:
+            return self(*args, **kwargs)
+
+        def __call__(self, *args, **kwargs) -> pl.LazyFrame:
+            return self.connection(self.query, *args, **kwargs)
+
+        def __repr__(self):
+            output = f"<{self.__class__.__name__} object at {hex(id(self))}>\n"
+            output += f"with {repr(self.connection)}\n"
+            output += self.query
+            return output
 
     @dataclass
     class QueryInfo:
         query: str
         time_taken: timedelta
 
     @dataclass
@@ -27,20 +46,39 @@
         ...
 
     class meta:
         QUERY = "query"
         TIMETAKEN = "time_taken"
         PARQUETFILE = "parquet_file"
 
-    def from_file(self, filepath: pt.Path, *args, **kwargs):
+    def from_file(self, filepath: pt.Path, *args, **kwargs) -> pl.LazyFrame:
         with open(filepath, "r") as f:
             query = f.read().replace(";", "")
-            query = re.sub("--!.+\n", "")
+            query = re.sub("--!.+\n", "", query)
         return self(query, *args, **kwargs)
 
+    def render_template(
+        self, filepath: pt.Path, *args, **kwargs
+    ) -> "Base.RenderedTemplateLoader":
+        with open(filepath, "r") as f:
+            query = f.read().replace(";", "")
+            query = re.sub("--!.+\n", "", query)
+
+        environment = jinja2.nativetypes.NativeEnvironment(
+            trim_blocks=True, lstrip_blocks=True, autoescape=True
+        )
+
+        query = environment.from_string(query).render(*args, **kwargs)
+        return Base.RenderedTemplateLoader(query, self)
+
+    def execute(
+        self, *args, scan_parquet_kwargs=None, **run_query_kwargs
+    ) -> pl.LazyFrame:
+        return self(*args, scan_parquet_kwargs=None, **run_query_kwargs)
+
     def __call__(
         self, query: str, *args, scan_parquet_kwargs=None, **run_query_kwargs
     ) -> pl.LazyFrame:
         self.query_info = self.QueryInfo(None, None)
 
         if self.to_cache:
             cached_df = self._load_from_cache(
```

### Comparing `dbqq-1.2.0/src/dbqq/connectors/_polar_connector.py` & `dbqq-1.3.2/src/dbqq/connectors/_polar_connector.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/connectors/databricks.py` & `dbqq-1.3.2/src/dbqq/connectors/databricks.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,16 +41,14 @@
         for t in GENERIC_TYPE_MAP.keys():
             if t in type:
                 return t
         return "UNIDENTIFIED"
 
 
 class _DatabricksBase(Base):
-    connections = []
-
     def __new__(cls, *args, **kwargs):
         if "DATABRICKS_RUNTIME_VERSION" in os.environ.keys():
             conn = super().__new__(Cluster, *args, **kwargs)
             conn.__init__()
             return conn
 
         return super().__new__(cls, *args, **kwargs)
@@ -79,14 +77,19 @@
         self.cursor.close()
 
     def describe_columns(self, table_name: str) -> pl.LazyFrame:
         query = f"describe {table_name}"
 
         description: pl.LazyFrame = self(query)
 
+        self.description_query = (
+            query
+            + "\n-- the result of this query is post-processed with polars"
+        )
+
         description = (
             description.filter(pl.col("col_name").str.contains("^\#").is_not())
             .unique()
             .rename({c: c.upper() for c in description.columns})
             .with_columns(pl.lit(None).alias("DATA_LENGTH"))
             .with_columns(
                 pl.col("DATA_TYPE")
@@ -110,14 +113,15 @@
             .select(
                 [
                     "COL_NAME",
                     "DATA_TYPE",
                     "DATA_LENGTH",
                     "DATA_PRECISION",
                     "DATA_SCALE",
+                    "GENERIC_TYPE",
                 ]
             )
         )
         description = description.select(
             [pl.col(c) for c in description.columns if c != "COMMENT"]
         )
```

### Comparing `dbqq-1.2.0/src/dbqq/connectors/mssql.py` & `dbqq-1.3.2/src/dbqq/connectors/mssql.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,14 @@
         for t in GENERIC_TYPE_MAP.keys():
             if t in type:
                 return t
         return "UNIDENTIFIED"
 
 
 class _MSSQLBase(PolarsConnector):
-    connections = []
-
     def __init__(self, username, password, hostname, port, database):
         self.connection = "mssql://%s:%s@%s:%s/%s" % (
             username,
             urllib.parse.quote_plus(password),
             hostname,
             port,
             database,
@@ -75,14 +73,16 @@
             from sys.tables t
             join sys.columns c on t.object_id = c.object_id
             where t.name = '{table_name.split(".")[-1]}'
         """
             >> tqc
         )
 
+        self.description_query = query
+
         description = self(query, **kwargs)
 
         description = description.rename(
             {c: c.upper() for c in description.columns}
         )
 
         description = description.with_columns(
```

### Comparing `dbqq-1.2.0/src/dbqq/connectors/oracle.py` & `dbqq-1.3.2/src/dbqq/connectors/oracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,27 @@
     else:
         for t in GENERIC_TYPE_MAP.keys():
             if t in type:
                 return t
         return "UNIDENTIFIED"
 
 
-# class _OracleBase(Base):
 class _OracleBase(PolarsConnector):
-    connections = []
-
     def __init__(self, username, password, hostname, port, database):
         self.connection = "oracle://%s:%s@%s:%s/%s" % (
             username,
             password,
             hostname,
             port,
             database,
         )
 
-    def describe_columns(self, table_name, owner=None, **kwargs):
+    def describe_columns(
+        self, table_name, owner=None, **kwargs
+    ) -> pl.LazyFrame:
         table_name = table_name.upper()
 
         if owner is not None:
             owner = owner.upper()
 
         if "." in table_name:
             owner, table_name = table_name.split(".")
@@ -124,14 +123,16 @@
                     order by col.owner, col.table_name, col.column_id
                 )
                 and lower(table_name) = '{table_name.lower()}'
             """
                 >> tqc
             )
 
+        self.description_query = query
+
         description = self(query, **kwargs)
 
         description = description.with_columns(
             pl.col("DATA_TYPE")
             .apply(generic_type_mapper)
             .alias("GENERIC_TYPE")
         )
```

### Comparing `dbqq-1.2.0/src/dbqq/security/cli/decrypt_yaml.py` & `dbqq-1.3.2/src/dbqq/security/cli/decrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/security/cli/encrypt_yaml.py` & `dbqq-1.3.2/src/dbqq/security/cli/encrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/security/cli/write_keys.py` & `dbqq-1.3.2/src/dbqq/security/cli/write_keys.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/security/functions/_functions.py` & `dbqq-1.3.2/src/dbqq/security/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/security/functions/_yaml.py` & `dbqq-1.3.2/src/dbqq/security/functions/_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/security/helpers.py` & `dbqq-1.3.2/src/dbqq/security/helpers.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq/utils.py` & `dbqq-1.3.2/src/dbqq/utils.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.2.0/src/dbqq.egg-info/PKG-INFO` & `dbqq-1.3.2/src/dbqq.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: dbqq
-Version: 1.2.0
+Version: 1.3.2
+Summary: quickly connect to and query databases
 Author-email: Chris Mamon <chrisam1993@live.com>
+Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
+Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,14 +29,15 @@
     - [Getting Basic Table Metadata](#getting-basic-table-metadata)
     - [Running Queries from a File](#running-queries-from-a-file)
       - [Extracting queries and connections from a file](#extracting-queries-and-connections-from-a-file)
         - [Basic Connection No Cache](#basic-connection-no-cache)
         - [Connection With Cache](#connection-with-cache)
         - [Connection With Cache and Date Lower Bound](#connection-with-cache-and-date-lower-bound)
     - [Parsing Files](#parsing-files)
+    - [Jinja Templates](#jinja-templates)
   - [Common Table Expressions](#common-table-expressions)
     - [Rollback](#rollback)
   - [Databricks Development](#databricks-development)
   - [CLI Tools](#cli-tools)
     - [dbqq-clean-connections](#dbqq-clean-connections)
     - [dbqq-run-sql](#dbqq-run-sql)
 
@@ -365,14 +369,64 @@
 from dbqq import utils
 
 enum = utils.parse_file("<path to file>")
 ```
 
 enums for parsed sql can be found in connectors.enums.parsed.sql
 
+### Jinja Templates
+
+We can parse jinja templates, let's say we have a template called `test_query.sql.j2`
+
+```jinja
+select
+{% for item in  columns %}
+{% if loop.last %}
+    {{ item }}
+{% else %}
+    {{ item }},
+{% endif %}
+{% endfor %}
+from
+  some.table
+```
+
+We can create a `RenderedTemplateLoader` from it using the following
+
+```python
+import dbqq.connectors as dbc
+
+conn = dbc.<source>.<conn>()
+
+rendered_template_loader = conn.render_template(
+    "test_query.sql.j2",
+    columns=[
+      "col1",
+      "col2",
+      "col3",
+      "col4"
+    ],
+)
+
+# will return a object that shows the renderedquery
+
+"""
+select
+  col1,
+  col2,
+  col3,
+  col4
+from
+  some.table
+"""
+
+table = rendered_template_loader.execute()
+
+```
+
 ## Common Table Expressions
 
 We can construct a common table expression with the following method
 
 ```python
 from dbqq import utils
 from triple_quote_clean import TripleQuoteCleaner
```

### Comparing `dbqq-1.2.0/src/dbqq.egg-info/SOURCES.txt` & `dbqq-1.3.2/src/dbqq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

