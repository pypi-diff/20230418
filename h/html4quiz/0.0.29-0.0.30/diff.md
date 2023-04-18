# Comparing `tmp/html4quiz-0.0.29.tar.gz` & `tmp/html4quiz-0.0.30.tar.gz`

## Comparing `html4quiz-0.0.29.tar` & `html4quiz-0.0.30.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.29/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/_common.py
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.29/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.29/LICENSE.txt
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 html4quiz-0.0.29/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.29/pyproject.toml
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 html4quiz-0.0.29/PKG-INFO
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.30/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.30/LICENSE.txt
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 html4quiz-0.0.30/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.30/pyproject.toml
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 html4quiz-0.0.30/PKG-INFO
```

### Comparing `html4quiz-0.0.29/updatePackage.txt` & `html4quiz-0.0.30/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.29/src/html4quiz/_common.py` & `html4quiz-0.0.30/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.29/src/html4quiz/_generateEm.py` & `html4quiz-0.0.30/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.29/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.30/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.29/src/html4quiz/makeChoices.py` & `html4quiz-0.0.30/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.29/LICENSE.txt` & `html4quiz-0.0.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.29/README.md` & `html4quiz-0.0.30/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 ## What is it?
 
 html4quiz is a package that helps you generate question sheets with as many HTML files as you want and grade answers from text files submitted by students.
 
 ## Features
 <ul>
-<li>Everything is on your local PC, grows with your creativity, and you own them all.</li>
+<li>Unlike the many quiz generators available online, everything is on your local PC, grows with your creativity, and you own everything.</li>
 <li>Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
+<li>Except for the math equations, each HTML file is complete in itself.</li>
 <li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
-<li>Grading answers from text files submitted by students can be done with a few keystrokes.</li>
+<li>Saving answers to a file can be repeated as many times as desired.</li>
+<li>Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
 <li>A question begins with a short answer in a number or word.</li>
-<li>Questions with numeric answers can be converted to multiple choice questions simply by flipping the flag.</li>
+<li>Questions with numeric answers can be converted to multiple choice questions simply by flipping the option flag.</li>
 <li>Questions can start with multiple choice.</li>
 <li>Mathematical equations in LaTeX format can be included in both question texts and choices.</li>
 <li>Figures can be included in both question text and choices.</li>
 <li>Question text, mathematical equations, and figures are all randomly selected for each question sheet in a controlled manner.</li>
 <li>Randomness is acquired by executing the answer string, which is a short Python script, that is part of question.</li>
 <li>To increase your creativity, user-defined functions can be easily added for the answer string.</li>
 </ul>
@@ -31,14 +33,22 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
+<li>Version 0.0.30</li>
+<ul><li>In addition to using a user-defined function for answers, a new way to use resources saved in <a href="https://github.com/generateNscore/html4quiz/tree/main/res">html4quiz/res</a> is added.</li>
+<li>For details, please look at <a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004.py">Ex004.py</a></li>
+<li><a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004/Ex004/index.html">Previews</a></li>
+</ul>
+<br>
+
+
 <li>Version 0.0.29</li>
 <ul><li>Added an option to reuse previous work.</li>
 <ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option <strong>True</strong> and re-running the work is all you need to do.</li>
 <li>The new option, <strong>flag4Previous</strong> can be added as the last argument to the instance as:</li>
 <li>If not provided, the default value of the option, False, is assumed.</li></ul>
 
 ```python
@@ -62,21 +72,14 @@
 <li>So is the name of repository in GitHub.</li></ul>
 <br>
 <li>Version 0.0.20</li>
 
 <ul><li>Finallized a way to upload/download Javascript scripts saved in JSON files for figures.<a href="https://github.com/generateNscore/html4quiz/wiki#h-download-json-file-of-javascript-code-for-figure-contents">H. Download Json file of Javascript code for figure contents</a></li></ul>
 <br>
 
-<li>Version 0.0.16</li>
-
-<ul><li>In addition to typical short-answer questions that can be answered on the screen, a new kind questions for which students are required to "play" with mouse to complete a required task to answer is added.</li>
-<li>Example: <a href="https://generateNscore.github.io/html4quiz/Examples/Nk001/Nk001.py">Nk001.py</a></li>
-</ul>
-<br>
-
 <li>Version 0.0.11</li>
 
 <ul><li>A way to stay in short-answer question is added as:</li>
   
 ```python
   
 answer = [{'choices':None, 'ans': ans}]
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 # html4quiz ## What is it? html4quiz is a package that helps you generate
 question sheets with as many HTML files as you want and grade answers from text
 files submitted by students. ## Features
-    * Everything is on your local PC, grows with your creativity, and you own
-      them all.
+    * Unlike the many quiz generators available online, everything is on your
+      local PC, grows with your creativity, and you own everything.
     * Question sheets in HTML files, each named with a corresponding
       identification number, are distributed to students over the network.
+    * Except for the math equations, each HTML file is complete in itself.
     * Students use their mobile devices to read, answer questions, save answers
       to a text file for submission within the same HTML page, and submit the
       text file as directed over the network.
-    * Grading answers from text files submitted by students can be done with a
-      few keystrokes.
+    * Saving answers to a file can be repeated as many times as desired.
+    * Grade answers in text files submitted by all students can be achieved
+      with a few keystrokes.
     * A question begins with a short answer in a number or word.
     * Questions with numeric answers can be converted to multiple choice
-      questions simply by flipping the flag.
+      questions simply by flipping the option flag.
     * Questions can start with multiple choice.
     * Mathematical equations in LaTeX format can be included in both question
       texts and choices.
     * Figures can be included in both question text and choices.
     * Question text, mathematical equations, and figures are all randomly
       selected for each question sheet in a controlled manner.
     * Randomness is acquired by executing the answer string, which is a short
@@ -26,14 +28,20 @@
 ## Where to get it
 pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
+    * Version 0.0.30
+          o In addition to using a user-defined function for answers, a new way
+            to use resources saved in html4quiz/res is added.
+          o For details, please look at Ex004.py
+          o Previews
+    *
     * Version 0.0.29
           o Added an option to reuse previous work.
                 # When an answer of question among many in previous work whose
                   question sheets has been distributed is found incorrect,
                   simply setting the option True and re-running the work is all
                   you need to do.
                 # The new option, flag4Previous can be added as the last
@@ -56,21 +64,14 @@
           o So is the name of repository in GitHub.
     *
     * Version 0.0.20
           o Finallized a way to upload/download Javascript scripts saved in
             JSON files for figures.H._Download_Json_file_of_Javascript_code_for
             figure_contents
     *
-    * Version 0.0.16
-          o In addition to typical short-answer questions that can be answered
-            on the screen, a new kind questions for which students are required
-            to "play" with mouse to complete a required task to answer is
-            added.
-          o Example: Nk001.py
-    *
     * Version 0.0.11
           o A way to stay in short-answer question is added as:
           o ```python answer = [{'choices':None, 'ans': ans}] ```
                 # This answering form is different from the one of
           o ```python answer = [{'choices':None, 'ans':vA+vB, 'fn':
             'variation0_int'}] ```
           o This is about Specifying_method_of_convering_short-answer_to_a_set
```

### Comparing `html4quiz-0.0.29/pyproject.toml` & `html4quiz-0.0.30/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.29"
+version = "0.0.30"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.29/PKG-INFO` & `html4quiz-0.0.30/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.29
+Version: 0.0.30
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -21,20 +21,22 @@
 
 ## What is it?
 
 html4quiz is a package that helps you generate question sheets with as many HTML files as you want and grade answers from text files submitted by students.
 
 ## Features
 <ul>
-<li>Everything is on your local PC, grows with your creativity, and you own them all.</li>
+<li>Unlike the many quiz generators available online, everything is on your local PC, grows with your creativity, and you own everything.</li>
 <li>Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
+<li>Except for the math equations, each HTML file is complete in itself.</li>
 <li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
-<li>Grading answers from text files submitted by students can be done with a few keystrokes.</li>
+<li>Saving answers to a file can be repeated as many times as desired.</li>
+<li>Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
 <li>A question begins with a short answer in a number or word.</li>
-<li>Questions with numeric answers can be converted to multiple choice questions simply by flipping the flag.</li>
+<li>Questions with numeric answers can be converted to multiple choice questions simply by flipping the option flag.</li>
 <li>Questions can start with multiple choice.</li>
 <li>Mathematical equations in LaTeX format can be included in both question texts and choices.</li>
 <li>Figures can be included in both question text and choices.</li>
 <li>Question text, mathematical equations, and figures are all randomly selected for each question sheet in a controlled manner.</li>
 <li>Randomness is acquired by executing the answer string, which is a short Python script, that is part of question.</li>
 <li>To increase your creativity, user-defined functions can be easily added for the answer string.</li>
 </ul>
@@ -50,14 +52,22 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
+<li>Version 0.0.30</li>
+<ul><li>In addition to using a user-defined function for answers, a new way to use resources saved in <a href="https://github.com/generateNscore/html4quiz/tree/main/res">html4quiz/res</a> is added.</li>
+<li>For details, please look at <a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004.py">Ex004.py</a></li>
+<li><a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004/Ex004/index.html">Previews</a></li>
+</ul>
+<br>
+
+
 <li>Version 0.0.29</li>
 <ul><li>Added an option to reuse previous work.</li>
 <ul><li>When an answer of question among many in previous work whose question sheets has been distributed is found incorrect, simply setting the option <strong>True</strong> and re-running the work is all you need to do.</li>
 <li>The new option, <strong>flag4Previous</strong> can be added as the last argument to the instance as:</li>
 <li>If not provided, the default value of the option, False, is assumed.</li></ul>
 
 ```python
@@ -81,21 +91,14 @@
 <li>So is the name of repository in GitHub.</li></ul>
 <br>
 <li>Version 0.0.20</li>
 
 <ul><li>Finallized a way to upload/download Javascript scripts saved in JSON files for figures.<a href="https://github.com/generateNscore/html4quiz/wiki#h-download-json-file-of-javascript-code-for-figure-contents">H. Download Json file of Javascript code for figure contents</a></li></ul>
 <br>
 
-<li>Version 0.0.16</li>
-
-<ul><li>In addition to typical short-answer questions that can be answered on the screen, a new kind questions for which students are required to "play" with mouse to complete a required task to answer is added.</li>
-<li>Example: <a href="https://generateNscore.github.io/html4quiz/Examples/Nk001/Nk001.py">Nk001.py</a></li>
-</ul>
-<br>
-
 <li>Version 0.0.11</li>
 
 <ul><li>A way to stay in short-answer question is added as:</li>
   
 ```python
   
 answer = [{'choices':None, 'ans': ans}]
```

#### html2text {}

```diff
@@ -1,33 +1,35 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.29 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.30 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
 github.com/generateNscore/html4quiz/wiki Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
 :: End Users/Desktop Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Topic :: Education :: Testing Requires-Python: >=3.7
 Description-Content-Type: text/markdown # html4quiz ## What is it? html4quiz is
 a package that helps you generate question sheets with as many HTML files as
 you want and grade answers from text files submitted by students. ## Features
-    * Everything is on your local PC, grows with your creativity, and you own
-      them all.
+    * Unlike the many quiz generators available online, everything is on your
+      local PC, grows with your creativity, and you own everything.
     * Question sheets in HTML files, each named with a corresponding
       identification number, are distributed to students over the network.
+    * Except for the math equations, each HTML file is complete in itself.
     * Students use their mobile devices to read, answer questions, save answers
       to a text file for submission within the same HTML page, and submit the
       text file as directed over the network.
-    * Grading answers from text files submitted by students can be done with a
-      few keystrokes.
+    * Saving answers to a file can be repeated as many times as desired.
+    * Grade answers in text files submitted by all students can be achieved
+      with a few keystrokes.
     * A question begins with a short answer in a number or word.
     * Questions with numeric answers can be converted to multiple choice
-      questions simply by flipping the flag.
+      questions simply by flipping the option flag.
     * Questions can start with multiple choice.
     * Mathematical equations in LaTeX format can be included in both question
       texts and choices.
     * Figures can be included in both question text and choices.
     * Question text, mathematical equations, and figures are all randomly
       selected for each question sheet in a controlled manner.
     * Randomness is acquired by executing the answer string, which is a short
@@ -37,14 +39,20 @@
 ## Where to get it
 pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
+    * Version 0.0.30
+          o In addition to using a user-defined function for answers, a new way
+            to use resources saved in html4quiz/res is added.
+          o For details, please look at Ex004.py
+          o Previews
+    *
     * Version 0.0.29
           o Added an option to reuse previous work.
                 # When an answer of question among many in previous work whose
                   question sheets has been distributed is found incorrect,
                   simply setting the option True and re-running the work is all
                   you need to do.
                 # The new option, flag4Previous can be added as the last
@@ -67,21 +75,14 @@
           o So is the name of repository in GitHub.
     *
     * Version 0.0.20
           o Finallized a way to upload/download Javascript scripts saved in
             JSON files for figures.H._Download_Json_file_of_Javascript_code_for
             figure_contents
     *
-    * Version 0.0.16
-          o In addition to typical short-answer questions that can be answered
-            on the screen, a new kind questions for which students are required
-            to "play" with mouse to complete a required task to answer is
-            added.
-          o Example: Nk001.py
-    *
     * Version 0.0.11
           o A way to stay in short-answer question is added as:
           o ```python answer = [{'choices':None, 'ans': ans}] ```
                 # This answering form is different from the one of
           o ```python answer = [{'choices':None, 'ans':vA+vB, 'fn':
             'variation0_int'}] ```
           o This is about Specifying_method_of_convering_short-answer_to_a_set
```

