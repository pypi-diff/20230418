# Comparing `tmp/archytas-0.2.1.tar.gz` & `tmp/archytas-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-0.2.1.tar", max compression
+gzip compressed data, was "archytas-0.2.2.tar", max compression
```

## Comparing `archytas-0.2.1.tar` & `archytas-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    32472 2023-04-18 18:59:36.329688 archytas-0.2.1/LICENSE
--rw-r--r--   0        0        0     2577 2023-04-18 18:59:36.329688 archytas-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/agent.py
--rw-r--r--   0        0        0      513 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/auth.py
--rw-r--r--   0        0        0     6701 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/demo_tools.py
--rw-r--r--   0        0        0     3229 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/prompt.py
--rw-r--r--   0        0        0     5548 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/react.py
--rw-r--r--   0        0        0     1005 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/repl.py
--rw-r--r--   0        0        0    17317 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/tool_utils.py
--rw-r--r--   0        0        0     1561 2023-04-18 18:59:36.329688 archytas-0.2.1/archytas/tools.py
--rw-r--r--   0        0        0      758 2023-04-18 18:59:36.333688 archytas-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 archytas-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-04-18 20:18:52.896203 archytas-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2577 2023-04-18 20:18:52.896203 archytas-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/agent.py
+-rw-r--r--   0        0        0      513 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/auth.py
+-rw-r--r--   0        0        0     6701 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/demo_tools.py
+-rw-r--r--   0        0        0     3229 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/prompt.py
+-rw-r--r--   0        0        0     5548 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/react.py
+-rw-r--r--   0        0        0     1005 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/repl.py
+-rw-r--r--   0        0        0    17317 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/tool_utils.py
+-rw-r--r--   0        0        0     1521 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/tools.py
+-rw-r--r--   0        0        0      758 2023-04-18 20:18:52.900203 archytas-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 archytas-0.2.2/PKG-INFO
```

### Comparing `archytas-0.2.1/LICENSE` & `archytas-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/README.md` & `archytas-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/agent.py` & `archytas-0.2.2/archytas/agent.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/auth.py` & `archytas-0.2.2/archytas/auth.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/demo_tools.py` & `archytas-0.2.2/archytas/demo_tools.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/prompt.py` & `archytas-0.2.2/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/react.py` & `archytas-0.2.2/archytas/react.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/repl.py` & `archytas-0.2.2/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/tool_utils.py` & `archytas-0.2.2/archytas/tool_utils.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.1/archytas/tools.py` & `archytas-0.2.2/archytas/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from archytas.tool_utils import tool, toolset
 
 
-from easyrepl import readl
 @tool()
 def ask_user(query:str) -> str:
     """
     Ask the user a question and get their response. 
     
     You should ask the user a question if you do not have enough information to complete the task, and there is no suitable tool to help you.
     
     Args:
         query (str): The question to ask the user
 
     Returns:
         str: The user's response
     """
-    return readl(prompt=f'{query} ')
+    return input(query)
 
 
 
 from datetime import datetime
 import pytz
 @tool(name='datetime')
 def datetime_tool(format:str='%Y-%m-%d %H:%M:%S %Z', timezone:str='UTC') -> str:
```

### Comparing `archytas-0.2.1/pyproject.toml` & `archytas-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "0.2.1"
+version = "0.2.2"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-0.2.1/PKG-INFO` & `archytas-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

