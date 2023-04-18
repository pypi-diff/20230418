# Comparing `tmp/pymathematics-2023.4.17.tar.gz` & `tmp/pymathematics-2023.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.17.tar", last modified: Mon Apr 17 16:55:06 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.18.tar", last modified: Tue Apr 18 13:18:36 2023, max compression
```

## Comparing `pymathematics-2023.4.17.tar` & `pymathematics-2023.4.18.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-17 16:55:06.913364 pymathematics-2023.4.17/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.17/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-17 16:55:06.900365 pymathematics-2023.4.17/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       30 2023-04-16 06:28:23.000000 pymathematics-2023.4.17/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-17 16:55:06.643919 pymathematics-2023.4.17/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    11933 2023-04-17 16:36:03.000000 pymathematics-2023.4.17/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-17 16:36:43.000000 pymathematics-2023.4.17/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-17 16:55:06.830918 pymathematics-2023.4.17/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-17 16:55:06.916367 pymathematics-2023.4.17/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-17 16:36:31.000000 pymathematics-2023.4.17/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-18 13:18:36.387120 pymathematics-2023.4.18/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.18/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-18 13:18:36.377117 pymathematics-2023.4.18/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       28 2023-04-18 13:11:32.000000 pymathematics-2023.4.18/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-18 13:18:35.955893 pymathematics-2023.4.18/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    12206 2023-04-18 13:11:37.000000 pymathematics-2023.4.18/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-18 13:11:26.000000 pymathematics-2023.4.18/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-18 13:18:36.306120 pymathematics-2023.4.18/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-18 13:18:36.391119 pymathematics-2023.4.18/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-18 13:12:28.000000 pymathematics-2023.4.18/setup.py
```

### Comparing `pymathematics-2023.4.17/LICENSE` & `pymathematics-2023.4.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.17/pymathematics/__init__.py` & `pymathematics-2023.4.18/pymathematics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,16 +324,21 @@
 
 def mean_sqrd_error(actual:list,predicted:list) -> int|float:
     if len(actual) != len(predicted):
         raise ValueError("length of actual and predicted data aren't equal!")
     errors = [(actual[i]-predicted[i])**2 for i in range(len(actual))]
     return summation(errors)/len(actual)
 
-def mean_error(actual:list,expected:list) -> list:
-    pass
+def errors(actual:list,predicted:list) -> list:
+    if len(actual) != len(predicted):
+        raise ValueError("length of actual and predicted data aren't equal!")
+    return [actual[x]-predicted[x] for x in range(len(actual))]
+
+def mean_error(actual:list,predicted:list) -> int|float:
+    return mean(errors(actual,predicted))
 
 def power(base:int|float,exponent:int|float) -> int|float:
     return base**exponent
 
 def power_sum(array:list,exponent:int|float) -> list:
     return summation(power_array(array,exponent))
```

### Comparing `pymathematics-2023.4.17/setup.py` & `pymathematics-2023.4.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.17",
+    version = "2023.4.18",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

