# Comparing `tmp/plexorank-0.0.6.tar.gz` & `tmp/plexorank-0.0.7.tar.gz`

## Comparing `plexorank-0.0.6.tar` & `plexorank-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plexorank-0.0.6/src/plexorank/__init__.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 plexorank-0.0.6/src/plexorank/cipher_tables.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 plexorank-0.0.6/src/plexorank/rank.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 plexorank-0.0.6/src/plexorank/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 plexorank-0.0.6/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 plexorank-0.0.6/LICENSE
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 plexorank-0.0.6/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plexorank-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 plexorank-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/__init__.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/cipher_tables.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/rank.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 plexorank-0.0.7/src/plexorank/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 plexorank-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 plexorank-0.0.7/LICENSE
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 plexorank-0.0.7/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plexorank-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 plexorank-0.0.7/PKG-INFO
```

### Comparing `plexorank-0.0.6/src/plexorank/cipher_tables.py` & `plexorank-0.0.7/src/plexorank/cipher_tables.py`

 * *Files identical despite different names*

### Comparing `plexorank-0.0.6/src/plexorank/rank.py` & `plexorank-0.0.7/src/plexorank/rank.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Functions around generating and modifying elements utilizing a lexicographical ranking system"""
 from math import floor
 
-from plexorank.utils import (
+from built_inspections_http.v2.utils.lexorank.utils import (
     convert_to_base10,
     convert_to_base26,
     decipher_rank,
+    decrement_deciphered_rank,
     find_mean,
     get_greater_length,
     increment_deciphered_rank,
     normalize_rank,
     recipher,
     validate_rank,
 )
 
+LOWER_BOUND = "aaaaaa"
 LOWEST_INITIAL_RANK = "bbbbbb"
 LOWEST_INITIAL_RANK_VALUE = 12356631
 HIGHEST_INITIAL_RANK = "ffffff"
 HIGHEST_INITIAL_RANK_VALUE = 61783155
 INITIAL_CIPHER_LENGTH = 6
 
 # Increment depth describes which "position" you want to increment by 1:
@@ -57,14 +59,20 @@
     new_rank = recipher(mean_base26)
     valid_rank = validate_rank(prev_rank, next_rank, new_rank)
 
     return valid_rank
 
 
 def increment_rank(prev_rank: str) -> str:
-    """Add a rank to the end of the ordered list of ranks by INCREMENT_DEPTH"""
+    """Generate a rank after a supplied rank, incremented by INCREMENT_DEPTH"""
     deciphered = decipher_rank(prev_rank)
     incremented_deciphered = increment_deciphered_rank(deciphered, INCREMENT_DEPTH)
     new_rank = recipher(incremented_deciphered)
     return new_rank
 
 
+def decrement_rank(next_rank: str) -> str:
+    """Generate a rank before a supplied rank, decremented by INCREMENT_DEPTH"""
+    deciphered = decipher_rank(next_rank)
+    decremented_deciphered = decrement_deciphered_rank(deciphered, INCREMENT_DEPTH)
+    new_rank = recipher(decremented_deciphered)
+    return new_rank
```

### Comparing `plexorank-0.0.6/src/plexorank/utils.py` & `plexorank-0.0.7/src/plexorank/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -78,7 +78,34 @@
         if new_deciphered_rank[0] == 26:
             """We've maxed out the potential value of this cipher length. Reset it and tack on an n"""
             new_deciphered_rank = deciphered_rank[:]
             new_deciphered_rank.append(13)
             break
     return new_deciphered_rank
 
+
+def decrement_deciphered_rank(deciphered_rank: list[int], increment_depth: int):
+    """Decrement a list of integers, where 0 is the min with carry-over logic and 25 is the max
+    - increment_depth represents reverse index (which item should we decrement?)
+    - i.e. [1,3,0,7] with increment_depth of 1 should be [1,2,25,7]
+      - The 0 became -1, so that rolled over to 25 and decremented the next digit by 1 (3 -> 2)
+
+    In the event that we are served the upper bound of a rank (i.e. [0,0,0,0]), there's nothing to decrement.
+    As items get moved around, the system will heal itself.
+    """
+    new_deciphered_rank = deciphered_rank[:]
+    index = -increment_depth - 1
+    new_deciphered_rank[index] -= 1
+    while -1 in new_deciphered_rank:
+        new_deciphered_rank[index] = 25
+        new_deciphered_rank[index - 1] -= 1
+        index -= 1
+
+        if new_deciphered_rank[0] == -1:
+            """We can't go any lower. Try to decrease by a single rank, else return [0,0,0,0]"""
+            if deciphered_rank[-1] == 0:
+                return deciphered_rank
+            else:
+                one_down_rank = deciphered_rank[:]
+                one_down_rank[-1] -= 1
+                return one_down_rank
+    return new_deciphered_rank
```

### Comparing `plexorank-0.0.6/LICENSE` & `plexorank-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plexorank-0.0.6/pyproject.toml` & `plexorank-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "plexorank"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Alex Martin", email="raymond.alex.martin@gmail.com"},
 ]
 description = "A lexicographical ranking system for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `plexorank-0.0.6/PKG-INFO` & `plexorank-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plexorank
-Version: 0.0.6
+Version: 0.0.7
 Summary: A lexicographical ranking system for python
 Project-URL: Homepage, https://github.com/subtleco/pylex
 Project-URL: Bug Tracker, https://github.com/subtleco/pylex/issues
 Author-email: Alex Martin <raymond.alex.martin@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

