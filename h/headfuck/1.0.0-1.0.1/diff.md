# Comparing `tmp/headfuck-1.0.0.tar.gz` & `tmp/headfuck-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "headfuck-1.0.1.tar", max compression
```

## Comparing `headfuck-1.0.0.tar` & `headfuck-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 headfuck-1.0.0/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headfuck-1.0.0/src/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 headfuck-1.0.0/src/file.bf
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 headfuck-1.0.0/src/interpreter.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 headfuck-1.0.0/.gitignore
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 headfuck-1.0.0/LICENSE
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 headfuck-1.0.0/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 headfuck-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 headfuck-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-17 22:22:36.300042 headfuck-1.0.1/LICENSE
+-rw-r--r--   0        0        0      804 2023-04-17 22:22:24.899784 headfuck-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 22:03:23.039464 headfuck-1.0.1/headfuck/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-17 22:38:15.468576 headfuck-1.0.1/headfuck/file.bf
+-rw-r--r--   0        0        0      383 2023-04-17 22:43:04.265948 headfuck-1.0.1/headfuck/hff.py
+-rw-r--r--   0        0        0     3391 2023-04-17 22:27:17.839894 headfuck-1.0.1/headfuck/interpreter.py
+-rw-r--r--   0        0        0      612 2023-04-17 22:39:43.834195 headfuck-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 headfuck-1.0.1/PKG-INFO
```

### Comparing `headfuck-1.0.0/src/interpreter.py` & `headfuck-1.0.1/headfuck/interpreter.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,13 +84,13 @@
     for i in range(index-1,-1,-1):
         if code[i]==']': loop_counter+=1
         elif code[i]=='[':
             if loop_counter==0:
                 return i
             else: loop_counter-=1
     raise SyntaxError(f'Unmatched ] at index {index}')
-
-while True:
-    code = input()
-    result = interpret(code)
-    print(result)
-    quit()
+if __name__ == "__main__":
+    while True:
+        code = input()
+        result = interpret(code)
+        print(result)
+        quit()
```

### Comparing `headfuck-1.0.0/LICENSE` & `headfuck-1.0.1/LICENSE`

 * *Files identical despite different names*

