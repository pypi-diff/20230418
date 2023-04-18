# Comparing `tmp/html4quiz-0.0.27.tar.gz` & `tmp/html4quiz-0.0.28.tar.gz`

## Comparing `html4quiz-0.0.27.tar` & `html4quiz-0.0.28.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.27/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/_common.py
--rw-r--r--   0        0        0    28066 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.27/LICENSE.txt
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 html4quiz-0.0.27/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.27/pyproject.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 html4quiz-0.0.27/PKG-INFO
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.28/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.28/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.28/LICENSE.txt
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 html4quiz-0.0.28/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.28/pyproject.toml
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 html4quiz-0.0.28/PKG-INFO
```

### Comparing `html4quiz-0.0.27/updatePackage.txt` & `html4quiz-0.0.28/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.27/src/html4quiz/_common.py` & `html4quiz-0.0.28/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.27/src/html4quiz/_generateEm.py` & `html4quiz-0.0.28/src/html4quiz/_generateEm.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
   answers[parseInt(myRadio.name.slice(1))]=parseInt(myRadio.value)+1;
   addAnswers2Textarea();
 }
 
 function setCheckedRadio(q) {
   var radios = document.getElementsByName('Q'+q.toString());
   //for (let j=0; j<radios.length; j++) {radios[j].removeAttribute("checked");}
-  if (radios.length > 0 && answers[q] != null && Number.isInteger(answers[q]) ) {radios[answers[q]-1].setAttribute("checked", true);}
+  if (radios.length > 0 && answers[q] != null) {radios[answers[q]-1].setAttribute("checked", true);}
 }
 
 function destroyClickedElement(event) {
     document.body.removeChild(event.target);
 }
 </script>
 '''
```

### Comparing `html4quiz-0.0.27/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.28/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.27/src/html4quiz/makeChoices.py` & `html4quiz-0.0.28/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.27/LICENSE.txt` & `html4quiz-0.0.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.27/README.md` & `html4quiz-0.0.28/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,28 +31,29 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.27</li>
-<ul><li>Deleted a incomplete feature.</li>
-<ul><li>It is postponed.</li></ul>
-</ul>
-<br>
-<li>Version 0.0.26</li>
-<ul><li>A bug in Javascript script in radiobuttons.</li>
-<ul><li>Fixed.</li></ul>
-</ul>
-<br>
-<li>Version 0.0.25</li>
-<ul><li>Testing for README.md link to GitHub.</li>
+<li>Version 0.0.28</li>
+<ul><li>Added an option to reuse previous work.</li>
+<ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option Treu and re-running the work is all you need to do.</li>
+<li>The new option, <strong>flag4Previous</strong> can be added as the last argument to the instance as:</li>
+<li>The default value of the option is False.</li></ul>
+
+```python
+
+h4q.work('exam1', 'testing', STDs, QGs, flag4Preview, flag4Choice, flag4Shuffling, resources, flag4Previous)
+
+```
+
 </ul>
 <br>
+
 <li>Version 0.0.22</li>
 <ul><li>Added "res" folder to GitHub for the Javascript scripts of figures and additional data saved in JSON format.</li>
 <li>Added a "getResource()" function to the package to access the data.</li>
 <li>Some procedures of calling functions were removed to simplify the usages of package.</li>
 </ul>
 <br>
 <li>Version 0.0.21</li>
```

#### html2text {}

```diff
@@ -26,24 +26,25 @@
 ## Where to get it
 pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.27
-          o Deleted a incomplete feature.
-                # It is postponed.
-    *
-    * Version 0.0.26
-          o A bug in Javascript script in radiobuttons.
-                # Fixed.
-    *
-    * Version 0.0.25
-          o Testing for README.md link to GitHub.
+    * Version 0.0.28
+          o Added an option to reuse previous work.
+                # When an answer of question among many in previous work whose
+                  question sheets has been distributed is found incorrect,
+                  simply setting the option Treu and re-running the work is all
+                  you need to do.
+                # The new option, flag4Previous can be added as the last
+                  argument to the instance as:
+                # The default value of the option is False.
+          o ```python h4q.work('exam1', 'testing', STDs, QGs, flag4Preview,
+            flag4Choice, flag4Shuffling, resources, flag4Previous) ```
     *
     * Version 0.0.22
           o Added "res" folder to GitHub for the Javascript scripts of figures
             and additional data saved in JSON format.
           o Added a "getResource()" function to the package to access the data.
           o Some procedures of calling functions were removed to simplify the
             usages of package.
```

### Comparing `html4quiz-0.0.27/pyproject.toml` & `html4quiz-0.0.28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.27"
+version = "0.0.28"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.27/PKG-INFO` & `html4quiz-0.0.28/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.27
+Version: 0.0.28
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -50,28 +50,29 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.27</li>
-<ul><li>Deleted a incomplete feature.</li>
-<ul><li>It is postponed.</li></ul>
-</ul>
-<br>
-<li>Version 0.0.26</li>
-<ul><li>A bug in Javascript script in radiobuttons.</li>
-<ul><li>Fixed.</li></ul>
-</ul>
-<br>
-<li>Version 0.0.25</li>
-<ul><li>Testing for README.md link to GitHub.</li>
+<li>Version 0.0.28</li>
+<ul><li>Added an option to reuse previous work.</li>
+<ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option Treu and re-running the work is all you need to do.</li>
+<li>The new option, <strong>flag4Previous</strong> can be added as the last argument to the instance as:</li>
+<li>The default value of the option is False.</li></ul>
+
+```python
+
+h4q.work('exam1', 'testing', STDs, QGs, flag4Preview, flag4Choice, flag4Shuffling, resources, flag4Previous)
+
+```
+
 </ul>
 <br>
+
 <li>Version 0.0.22</li>
 <ul><li>Added "res" folder to GitHub for the Javascript scripts of figures and additional data saved in JSON format.</li>
 <li>Added a "getResource()" function to the package to access the data.</li>
 <li>Some procedures of calling functions were removed to simplify the usages of package.</li>
 </ul>
 <br>
 <li>Version 0.0.21</li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.27 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.28 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
 github.com/generateNscore/html4quiz/wiki Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
@@ -37,24 +37,25 @@
 ## Where to get it
 pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.27
-          o Deleted a incomplete feature.
-                # It is postponed.
-    *
-    * Version 0.0.26
-          o A bug in Javascript script in radiobuttons.
-                # Fixed.
-    *
-    * Version 0.0.25
-          o Testing for README.md link to GitHub.
+    * Version 0.0.28
+          o Added an option to reuse previous work.
+                # When an answer of question among many in previous work whose
+                  question sheets has been distributed is found incorrect,
+                  simply setting the option Treu and re-running the work is all
+                  you need to do.
+                # The new option, flag4Previous can be added as the last
+                  argument to the instance as:
+                # The default value of the option is False.
+          o ```python h4q.work('exam1', 'testing', STDs, QGs, flag4Preview,
+            flag4Choice, flag4Shuffling, resources, flag4Previous) ```
     *
     * Version 0.0.22
           o Added "res" folder to GitHub for the Javascript scripts of figures
             and additional data saved in JSON format.
           o Added a "getResource()" function to the package to access the data.
           o Some procedures of calling functions were removed to simplify the
             usages of package.
```

