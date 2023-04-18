# Comparing `tmp/plexorank-0.0.7.tar.gz` & `tmp/plexorank-0.0.8.tar.gz`

## Comparing `plexorank-0.0.7.tar` & `plexorank-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/__init__.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/cipher_tables.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/rank.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 plexorank-0.0.7/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 plexorank-0.0.7/LICENSE
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 plexorank-0.0.7/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plexorank-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 plexorank-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plexorank-0.0.8/src/plexorank/__init__.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 plexorank-0.0.8/src/plexorank/cipher_tables.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 plexorank-0.0.8/src/plexorank/rank.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 plexorank-0.0.8/src/plexorank/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 plexorank-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 plexorank-0.0.8/LICENSE
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 plexorank-0.0.8/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plexorank-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 plexorank-0.0.8/PKG-INFO
```

### Comparing `plexorank-0.0.7/src/plexorank/cipher_tables.py` & `plexorank-0.0.8/src/plexorank/cipher_tables.py`

 * *Files identical despite different names*

### Comparing `plexorank-0.0.7/src/plexorank/rank.py` & `plexorank-0.0.8/src/plexorank/rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Functions around generating and modifying elements utilizing a lexicographical ranking system"""
 from math import floor
 
-from built_inspections_http.v2.utils.lexorank.utils import (
+from plexorank.utils import (
     convert_to_base10,
     convert_to_base26,
     decipher_rank,
     decrement_deciphered_rank,
     find_mean,
     get_greater_length,
     increment_deciphered_rank,
```

### Comparing `plexorank-0.0.7/src/plexorank/utils.py` & `plexorank-0.0.8/src/plexorank/utils.py`

 * *Files identical despite different names*

### Comparing `plexorank-0.0.7/LICENSE` & `plexorank-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `plexorank-0.0.7/pyproject.toml` & `plexorank-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "plexorank"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Alex Martin", email="raymond.alex.martin@gmail.com"},
 ]
 description = "A lexicographical ranking system for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `plexorank-0.0.7/PKG-INFO` & `plexorank-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plexorank
-Version: 0.0.7
+Version: 0.0.8
 Summary: A lexicographical ranking system for python
 Project-URL: Homepage, https://github.com/subtleco/pylex
 Project-URL: Bug Tracker, https://github.com/subtleco/pylex/issues
 Author-email: Alex Martin <raymond.alex.martin@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

