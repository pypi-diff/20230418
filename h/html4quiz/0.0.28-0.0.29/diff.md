# Comparing `tmp/html4quiz-0.0.28.tar.gz` & `tmp/html4quiz-0.0.29.tar.gz`

## Comparing `html4quiz-0.0.28.tar` & `html4quiz-0.0.29.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.28/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/_common.py
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.28/LICENSE.txt
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 html4quiz-0.0.28/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.28/pyproject.toml
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 html4quiz-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.29/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.29/LICENSE.txt
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 html4quiz-0.0.29/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.29/pyproject.toml
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 html4quiz-0.0.29/PKG-INFO
```

### Comparing `html4quiz-0.0.28/updatePackage.txt` & `html4quiz-0.0.29/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.28/src/html4quiz/_common.py` & `html4quiz-0.0.29/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.28/src/html4quiz/_generateEm.py` & `html4quiz-0.0.29/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.28/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.29/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.28/src/html4quiz/makeChoices.py` & `html4quiz-0.0.29/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.28/LICENSE.txt` & `html4quiz-0.0.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.28/README.md` & `html4quiz-0.0.29/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,23 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.28</li>
+<li>Version 0.0.29</li>
 <ul><li>Added an option to reuse previous work.</li>
-<ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option Treu and re-running the work is all you need to do.</li>
+<ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option <strong>True</strong> and re-running the work is all you need to do.</li>
 <li>The new option, <strong>flag4Previous</strong> can be added as the last argument to the instance as:</li>
-<li>The default value of the option is False.</li></ul>
+<li>If not provided, the default value of the option, False, is assumed.</li></ul>
 
 ```python
 
+flag4Previous = True
 h4q.work('exam1', 'testing', STDs, QGs, flag4Preview, flag4Choice, flag4Shuffling, resources, flag4Previous)
 
 ```
 
 </ul>
 <br>
```

#### html2text {}

```diff
@@ -26,25 +26,27 @@
 ## Where to get it
 pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.28
+    * Version 0.0.29
           o Added an option to reuse previous work.
                 # When an answer of question among many in previous work whose
                   question sheets has been distributed is found incorrect,
-                  simply setting the option Treu and re-running the work is all
+                  simply setting the option True and re-running the work is all
                   you need to do.
                 # The new option, flag4Previous can be added as the last
                   argument to the instance as:
-                # The default value of the option is False.
-          o ```python h4q.work('exam1', 'testing', STDs, QGs, flag4Preview,
-            flag4Choice, flag4Shuffling, resources, flag4Previous) ```
+                # If not provided, the default value of the option, False, is
+                  assumed.
+          o ```python flag4Previous = True h4q.work('exam1', 'testing', STDs,
+            QGs, flag4Preview, flag4Choice, flag4Shuffling, resources,
+            flag4Previous) ```
     *
     * Version 0.0.22
           o Added "res" folder to GitHub for the Javascript scripts of figures
             and additional data saved in JSON format.
           o Added a "getResource()" function to the package to access the data.
           o Some procedures of calling functions were removed to simplify the
             usages of package.
```

### Comparing `html4quiz-0.0.28/pyproject.toml` & `html4quiz-0.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.28"
+version = "0.0.29"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.28/PKG-INFO` & `html4quiz-0.0.29/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.28
+Version: 0.0.29
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -50,22 +50,23 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.28</li>
+<li>Version 0.0.29</li>
 <ul><li>Added an option to reuse previous work.</li>
-<ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option Treu and re-running the work is all you need to do.</li>
+<ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option <strong>True</strong> and re-running the work is all you need to do.</li>
 <li>The new option, <strong>flag4Previous</strong> can be added as the last argument to the instance as:</li>
-<li>The default value of the option is False.</li></ul>
+<li>If not provided, the default value of the option, False, is assumed.</li></ul>
 
 ```python
 
+flag4Previous = True
 h4q.work('exam1', 'testing', STDs, QGs, flag4Preview, flag4Choice, flag4Shuffling, resources, flag4Previous)
 
 ```
 
 </ul>
 <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.28 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.29 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
 github.com/generateNscore/html4quiz/wiki Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
@@ -37,25 +37,27 @@
 ## Where to get it
 pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.28
+    * Version 0.0.29
           o Added an option to reuse previous work.
                 # When an answer of question among many in previous work whose
                   question sheets has been distributed is found incorrect,
-                  simply setting the option Treu and re-running the work is all
+                  simply setting the option True and re-running the work is all
                   you need to do.
                 # The new option, flag4Previous can be added as the last
                   argument to the instance as:
-                # The default value of the option is False.
-          o ```python h4q.work('exam1', 'testing', STDs, QGs, flag4Preview,
-            flag4Choice, flag4Shuffling, resources, flag4Previous) ```
+                # If not provided, the default value of the option, False, is
+                  assumed.
+          o ```python flag4Previous = True h4q.work('exam1', 'testing', STDs,
+            QGs, flag4Preview, flag4Choice, flag4Shuffling, resources,
+            flag4Previous) ```
     *
     * Version 0.0.22
           o Added "res" folder to GitHub for the Javascript scripts of figures
             and additional data saved in JSON format.
           o Added a "getResource()" function to the package to access the data.
           o Some procedures of calling functions were removed to simplify the
             usages of package.
```

