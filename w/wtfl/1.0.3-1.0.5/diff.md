# Comparing `tmp/wtfl-1.0.3.tar.gz` & `tmp/wtfl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtfl-1.0.3.tar", max compression
+gzip compressed data, was "wtfl-1.0.5.tar", max compression
```

## Comparing `wtfl-1.0.3.tar` & `wtfl-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-04-18 11:26:56.748016 wtfl-1.0.3/LICENSE
--rw-r--r--   0        0        0     8723 2023-04-18 11:26:56.748016 wtfl-1.0.3/README.md
--rw-r--r--   0        0        0      578 2023-04-18 11:26:56.748016 wtfl-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/__init__.py
--rw-r--r--   0        0        0     4607 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/grammar.py
--rw-r--r--   0        0        0     2720 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/internal_types.py
--rw-r--r--   0        0        0     4519 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/parser.py
--rw-r--r--   0        0        0     5233 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/reader.py
--rw-r--r--   0        0        0     1798 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/writer.py
--rw-r--r--   0        0        0     9562 1970-01-01 00:00:00.000000 wtfl-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-18 11:53:10.252805 wtfl-1.0.5/LICENSE
+-rw-r--r--   0        0        0     8724 2023-04-18 11:53:10.252805 wtfl-1.0.5/README.md
+-rw-r--r--   0        0        0      578 2023-04-18 11:53:10.252805 wtfl-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/__init__.py
+-rw-r--r--   0        0        0     4606 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/grammar.py
+-rw-r--r--   0        0        0     2720 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/internal_types.py
+-rw-r--r--   0        0        0     4519 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/parser.py
+-rw-r--r--   0        0        0     6099 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/reader.py
+-rw-r--r--   0        0        0     1798 2023-04-18 11:53:10.252805 wtfl-1.0.5/wtfl/writer.py
+-rw-r--r--   0        0        0     9563 1970-01-01 00:00:00.000000 wtfl-1.0.5/PKG-INFO
```

### Comparing `wtfl-1.0.3/LICENSE` & `wtfl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.3/README.md` & `wtfl-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 ...The key is 35 now
 ```
 
 ## Types
 
 ### Numbers
 
-There are decimal integer literals, such as `102`, `-4` `0`, and, as expected, some other:
+There are decimal integer literals, such as `102`, `-4`, `0`, and, as expected, some other:
 
 - Binary (2) with `0b` prefix: `0b10010`
 - Octal (8) with `0o` prefix: `0o755`
 - Decimal (10) with `0d` prefix: `0d102`
 - Duodecimal (12) with `0z` prefix: `0z9a1`
 - Vigesimal (20) with `0v` prefix: `0vjija`
 - Roman numerals with `0r` prefix: `0rXIMI`
```

### Comparing `wtfl-1.0.3/pyproject.toml` & `wtfl-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wtfl"
-version = "1.0.3"
+version = "1.0.5"
 description = "Well-Designed Text-based Friendly Language"
 authors = ["Dmitry Gritsenko <k01419q45@ya.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/wtfl"
 homepage = "https://github.com/evtn/wtfl"
 keywords = ["markup", "config"]
```

### Comparing `wtfl-1.0.3/wtfl/grammar.py` & `wtfl-1.0.5/wtfl/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 g.IS[2] = Literal("is") | "are" | "'s" | "'re" | "do" | "does" | "be"
 g.ISNT[2] = Literal("isn't") | "aren't" | "'sn't" | "'ren't"
 
 g.OF[2] = "of"
 g.THAT[2] = Literal("that") | "this" | "these" | "those"
 g.THERE[2] = "there"
 g.HAVE[2] = Literal("have") | "has" | "'ve"
-g.HAVENT[2] = Literal("haven't") | "hasn't" | "'ve'n't"
+g.HAVENT[2] = Literal("haven't") | "hasn't" | "'ven't"
 
 g.CAN[2] = "can"
 g.CANT[2] = Literal("cannot") | "can't"
 g.BOOL[2] = RegExp(r"(true|false)(n't)?")
 g.RETURN[2] = "return"
 g.SKIP[2] = "skip"
 g.STAY[2] = "stay"
```

### Comparing `wtfl-1.0.3/wtfl/internal_types.py` & `wtfl-1.0.5/wtfl/internal_types.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.3/wtfl/parser.py` & `wtfl-1.0.5/wtfl/parser.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.3/wtfl/reader.py` & `wtfl-1.0.5/wtfl/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,20 @@
     def create_path(self, path: KeyChain):
         store = self.keys
 
         for key in path:
             if key in store:
                 new_store: StateValue = store[key]
                 if not isinstance(new_store, Store):
-                    raise ValueError("what?", path, key, new_store)
+                    raise ValueError(
+                        "Unknown resolving error occured, report this to the developer",
+                        path,
+                        key,
+                        new_store,
+                    )
             else:
                 new_store = Store()
                 store[key] = new_store
 
             store = new_store
 
         return store
@@ -112,17 +117,44 @@
 
         last_key = path[-1]
 
         assert not isinstance(value, Object)
 
         store[last_key] = value
 
+    def resolve_path(self, path: KeyChain) -> Store | None:
+        store = self.keys
+
+        for key in path:
+            if key in store:
+                new_store: StateValue = store[key]
+                if not isinstance(new_store, Store):
+                    return None
+            else:
+                return None
+
+            store = new_store
+
+        return store
+
     def add_constraint(self, constraint: Constraint):
         key = constraint.key
 
+        path = list(constraint.key)
+
+        store = self.resolve_path(path)
+
+        if store:
+            for value in store.keys.values():
+                try:
+                    constraint.check(value)
+                except:
+                    warn("Too late, it's already done")
+                    break
+
         if key not in self.constraints:
             self.constraints[key] = []
 
         self.constraints[key].append(constraint)
 
     def check_constraint(self, op: Assign):
         path = tuple(op.key)
```

### Comparing `wtfl-1.0.3/wtfl/writer.py` & `wtfl-1.0.5/wtfl/writer.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.3/PKG-INFO` & `wtfl-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtfl
-Version: 1.0.3
+Version: 1.0.5
 Summary: Well-Designed Text-based Friendly Language
 Home-page: https://github.com/evtn/wtfl
 License: MIT
 Keywords: markup,config
 Author: Dmitry Gritsenko
 Author-email: k01419q45@ya.ru
 Requires-Python: >=3.7,<4.0
@@ -210,15 +210,15 @@
 ...The key is 35 now
 ```
 
 ## Types
 
 ### Numbers
 
-There are decimal integer literals, such as `102`, `-4` `0`, and, as expected, some other:
+There are decimal integer literals, such as `102`, `-4`, `0`, and, as expected, some other:
 
 - Binary (2) with `0b` prefix: `0b10010`
 - Octal (8) with `0o` prefix: `0o755`
 - Decimal (10) with `0d` prefix: `0d102`
 - Duodecimal (12) with `0z` prefix: `0z9a1`
 - Vigesimal (20) with `0v` prefix: `0vjija`
 - Roman numerals with `0r` prefix: `0rXIMI`
```

