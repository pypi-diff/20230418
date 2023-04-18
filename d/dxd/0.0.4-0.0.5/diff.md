# Comparing `tmp/dxd-0.0.4.tar.gz` & `tmp/dxd-0.0.5.tar.gz`

## Comparing `dxd-0.0.4.tar` & `dxd-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/__about__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/__init__.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/column.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/engine.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/expr.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/kvstore.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/pattern.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/postgres_engine.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/sqlite_engine.py
--rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/table.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 dxd-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dxd-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 dxd-0.0.4/tests/test_tinyorm.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 dxd-0.0.4/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dxd-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 dxd-0.0.4/README.md
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 dxd-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dxd-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/__about__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/__init__.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/column.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/engine.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/expr.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/kvstore.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/pattern.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/postgres_engine.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/sqlite_engine.py
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 dxd-0.0.5/dxd/table.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 dxd-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dxd-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 dxd-0.0.5/tests/test_tinyorm.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 dxd-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dxd-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 dxd-0.0.5/README.md
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 dxd-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dxd-0.0.5/PKG-INFO
```

### Comparing `dxd-0.0.4/dxd/column.py` & `dxd-0.0.5/dxd/column.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/dxd/engine.py` & `dxd-0.0.5/dxd/engine.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/dxd/expr.py` & `dxd-0.0.5/dxd/expr.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/dxd/kvstore.py` & `dxd-0.0.5/dxd/kvstore.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/dxd/pattern.py` & `dxd-0.0.5/dxd/pattern.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/dxd/postgres_engine.py` & `dxd-0.0.5/dxd/postgres_engine.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/dxd/sqlite_engine.py` & `dxd-0.0.5/dxd/sqlite_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from enum import Enum
 import logging
 from sqlite3 import PrepareProtocol as P, Connection
 import datetime
 import textwrap
 from typing import Any, NewType, Type
 import uuid
-from miniscutil import as_optional, register_adapter
-from miniscutil.type_util import as_newtype
+from miniscutil import as_optional, register_adapter, as_newtype
 from .engine import Engine
 
 logger = logging.getLogger("dxd.sqlite3")
 
 
 def ident(x):
     return x
```

### Comparing `dxd-0.0.4/dxd/table.py` & `dxd-0.0.5/dxd/table.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/tests/conftest.py` & `dxd-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/tests/test_tinyorm.py` & `dxd-0.0.5/tests/test_tinyorm.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/.gitignore` & `dxd-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/LICENSE.txt` & `dxd-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/README.md` & `dxd-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/pyproject.toml` & `dxd-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dxd-0.0.4/PKG-INFO` & `dxd-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxd
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: Documentation, https://github.com/EdAyers/sss/dxd#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/dxd/issues
 Project-URL: Source, https://github.com/EdAyers/sss/dxd
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

