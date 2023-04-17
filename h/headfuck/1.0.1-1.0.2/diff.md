# Comparing `tmp/headfuck-1.0.1.tar.gz` & `tmp/headfuck-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headfuck-1.0.1.tar", max compression
+gzip compressed data, was "headfuck-1.0.2.tar", max compression
```

## Comparing `headfuck-1.0.1.tar` & `headfuck-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-04-17 22:22:36.300042 headfuck-1.0.1/LICENSE
--rw-r--r--   0        0        0      804 2023-04-17 22:22:24.899784 headfuck-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-17 22:03:23.039464 headfuck-1.0.1/headfuck/__init__.py
--rw-r--r--   0        0        0       19 2023-04-17 22:38:15.468576 headfuck-1.0.1/headfuck/file.bf
--rw-r--r--   0        0        0      383 2023-04-17 22:43:04.265948 headfuck-1.0.1/headfuck/hff.py
--rw-r--r--   0        0        0     3391 2023-04-17 22:27:17.839894 headfuck-1.0.1/headfuck/interpreter.py
--rw-r--r--   0        0        0      612 2023-04-17 22:39:43.834195 headfuck-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 headfuck-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-17 22:22:36.300042 headfuck-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1094 2023-04-17 22:46:53.278302 headfuck-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 22:03:23.039464 headfuck-1.0.2/headfuck/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-17 22:38:15.468576 headfuck-1.0.2/headfuck/file.bf
+-rw-r--r--   0        0        0      369 2023-04-17 22:43:35.306725 headfuck-1.0.2/headfuck/hff.py
+-rw-r--r--   0        0        0     3405 2023-04-17 22:46:11.747278 headfuck-1.0.2/headfuck/interpreter.py
+-rw-r--r--   0        0        0      590 2023-04-17 22:55:17.950576 headfuck-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 headfuck-1.0.2/PKG-INFO
```

### Comparing `headfuck-1.0.1/LICENSE` & `headfuck-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `headfuck-1.0.1/headfuck/interpreter.py` & `headfuck-1.0.2/headfuck/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,11 +86,11 @@
         elif code[i]=='[':
             if loop_counter==0:
                 return i
             else: loop_counter-=1
     raise SyntaxError(f'Unmatched ] at index {index}')
 if __name__ == "__main__":
     while True:
-        code = input()
+        code = input("Enter code: ")
         result = interpret(code)
         print(result)
         quit()
```

### Comparing `headfuck-1.0.1/pyproject.toml` & `headfuck-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.poetry]
 name = "headfuck"
-version = "1.0.1"
+version = "1.0.2"
 description = "An esoteric programming language similar to Brainfuck"
 authors = ["JJPMaster <joshuaponce2008@gmail.com>"]
-license = "Unlicense"
 readme = "README.md"
 packages = [{include = "headfuck"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: Public Domain",
   "Operating System :: OS Independent"
 ]
```

