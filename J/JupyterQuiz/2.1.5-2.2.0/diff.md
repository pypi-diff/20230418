# Comparing `tmp/JupyterQuiz-2.1.5.tar.gz` & `tmp/JupyterQuiz-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterQuiz-2.1.5.tar", last modified: Sat Mar 11 14:22:14 2023, max compression
+gzip compressed data, was "JupyterQuiz-2.2.0.tar", last modified: Tue Apr 18 16:27:10 2023, max compression
```

## Comparing `JupyterQuiz-2.1.5.tar` & `JupyterQuiz-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1820 2021-07-06 14:35:18.501466 JupyterQuiz-2.1.5/.gitignore
--rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.1.5/CITATION.cff
--rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.1.5/HideQuiz.ipynb
--rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.1.5/LICENSE
--rw-r--r--   0        0        0     8860 2023-03-11 13:44:15.891925 JupyterQuiz-2.1.5/README.md
--rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.1.5/examples/mc-example.gif
--rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.1.5/examples/num-example.gif
--rw-r--r--   0        0        0     6293 2021-06-16 18:37:29.568774 JupyterQuiz-2.1.5/examples/questions.json
--rw-r--r--   0        0        0      661 2023-03-11 14:21:47.341405 JupyterQuiz-2.1.5/jupyterquiz/__init__.py
--rw-r--r--   0        0        0     7273 2023-03-11 14:20:27.514288 JupyterQuiz-2.1.5/jupyterquiz/dynamic.py
--rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.1.5/jupyterquiz/helpers.js
--rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.1.5/jupyterquiz/multiple_choice.js
--rw-r--r--   0        0        0     6127 2022-08-22 19:45:35.869178 JupyterQuiz-2.1.5/jupyterquiz/multiple_choice.py
--rw-r--r--   0        0        0     7570 2022-08-22 19:45:35.870224 JupyterQuiz-2.1.5/jupyterquiz/numeric.js
--rw-r--r--   0        0        0     5907 2022-08-22 19:45:35.871163 JupyterQuiz-2.1.5/jupyterquiz/show_questions.js
--rw-r--r--   0        0        0     2762 2021-07-06 14:33:13.180515 JupyterQuiz-2.1.5/jupyterquiz/styles.css
--rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.1.5/preserve-responses.ipynb
--rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.1.5/previews/github-preview.png
--rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.1.5/previews/github-preview.psd
--rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     1393 2021-07-06 14:33:27.396186 JupyterQuiz-2.1.5/schema/mc_schema.json
--rw-r--r--   0        0        0   166749 2021-06-16 19:44:25.130972 JupyterQuiz-2.1.5/schema/mc_schema.png
--rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.1.5/schema/num_schema.json
--rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.1.5/schema/num_schema.png
--rw-r--r--   0        0        0     8093 2021-06-15 23:07:58.000000 JupyterQuiz-2.1.5/schema/schema.ipynb
--rw-r--r--   0        0        0   209929 2022-09-27 14:12:01.000000 JupyterQuiz-2.1.5/test.ipynb
--rw-r--r--   0        0        0     9174 1970-01-01 00:00:00.000000 JupyterQuiz-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1820 2021-07-06 14:35:18.501466 JupyterQuiz-2.2.0/.gitignore
+-rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.2.0/CITATION.cff
+-rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.2.0/HideQuiz.ipynb
+-rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.2.0/LICENSE
+-rw-r--r--   0        0        0     8860 2023-03-11 13:44:15.891925 JupyterQuiz-2.2.0/README.md
+-rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.2.0/examples/mc-example.gif
+-rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.2.0/examples/num-example.gif
+-rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.2.0/examples/questions.json
+-rw-r--r--   0        0        0      661 2023-04-18 16:18:26.616246 JupyterQuiz-2.2.0/jupyterquiz/__init__.py
+-rw-r--r--   0        0        0     7273 2023-04-18 15:57:35.208735 JupyterQuiz-2.2.0/jupyterquiz/dynamic.py
+-rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.2.0/jupyterquiz/helpers.js
+-rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.js
+-rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.py
+-rw-r--r--   0        0        0     7570 2022-08-22 19:45:35.870224 JupyterQuiz-2.2.0/jupyterquiz/numeric.js
+-rw-r--r--   0        0        0     5944 2023-04-18 16:11:00.030201 JupyterQuiz-2.2.0/jupyterquiz/show_questions.js
+-rw-r--r--   0        0        0     2762 2021-07-06 14:33:13.180515 JupyterQuiz-2.2.0/jupyterquiz/styles.css
+-rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.2.0/preserve-responses.ipynb
+-rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.2.0/previews/github-preview.png
+-rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.2.0/previews/github-preview.psd
+-rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1393 2021-07-06 14:33:27.396186 JupyterQuiz-2.2.0/schema/mc_schema.json
+-rw-r--r--   0        0        0   166749 2021-06-16 19:44:25.130972 JupyterQuiz-2.2.0/schema/mc_schema.png
+-rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.2.0/schema/num_schema.json
+-rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.2.0/schema/num_schema.png
+-rw-r--r--   0        0        0     8093 2021-06-15 23:07:58.000000 JupyterQuiz-2.2.0/schema/schema.ipynb
+-rw-r--r--   0        0        0    54049 2023-04-18 16:14:00.216953 JupyterQuiz-2.2.0/test.ipynb
+-rw-r--r--   0        0        0     9174 1970-01-01 00:00:00.000000 JupyterQuiz-2.2.0/PKG-INFO
```

### Comparing `JupyterQuiz-2.1.5/.gitignore` & `JupyterQuiz-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/HideQuiz.ipynb` & `JupyterQuiz-2.2.0/HideQuiz.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/LICENSE` & `JupyterQuiz-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/README.md` & `JupyterQuiz-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/examples/mc-example.gif` & `JupyterQuiz-2.2.0/examples/mc-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/examples/num-example.gif` & `JupyterQuiz-2.2.0/examples/num-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/examples/questions.json` & `JupyterQuiz-2.2.0/examples/questions.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {'insert': "[(1, OrderedDict([('question', 'Testing parameter to change number of colums for "*

 * *           "answers: Choose all of the following that can be included in Jupyter notebooks?'), "*

 * *           "('type', 'many_choice'), ('answer_cols', 4), ('answers', [OrderedDict([('answer', "*

 * *           "'Text and graphics output from Python'), ('correct', True), ('feedback', "*

 * *           "'Correct.')]), OrderedDict([('answer', 'Typeset mathematics'), ('correct', True), "*

 * *           "('feedback', 'Correct.')]), O […]*

```diff
@@ -27,14 +27,46 @@
                 "feedback": "I hope not."
             }
         ],
         "question": "Choose all of the following that can be included in Jupyter notebooks?",
         "type": "many_choice"
     },
     {
+        "answer_cols": 4,
+        "answers": [
+            {
+                "answer": "Text and graphics output from Python",
+                "correct": true,
+                "feedback": "Correct."
+            },
+            {
+                "answer": "Typeset mathematics",
+                "correct": true,
+                "feedback": "Correct."
+            },
+            {
+                "answer": "Python executable code",
+                "correct": true,
+                "feedback": "Correct."
+            },
+            {
+                "answer": "Formatted text",
+                "correct": true,
+                "feedback": "Correct."
+            },
+            {
+                "answer": "Live snakes via Python",
+                "correct": false,
+                "feedback": "I hope not."
+            }
+        ],
+        "question": "Testing parameter to change number of colums for answers: Choose all of the following that can be included in Jupyter notebooks?",
+        "type": "many_choice"
+    },
+    {
         "answers": [
             {
                 "answer": "Wiki markup",
                 "correct": false,
                 "feedback": "False."
             },
             {
```

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/__init__.py` & `JupyterQuiz-2.2.0/jupyterquiz/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.1.5'
+__version__ = '2.2.0'
 from .dynamic import display_quiz, capture_responses
```

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/dynamic.py` & `JupyterQuiz-2.2.0/jupyterquiz/dynamic.py`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/helpers.js` & `JupyterQuiz-2.2.0/jupyterquiz/helpers.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/multiple_choice.js` & `JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/multiple_choice.py` & `JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/numeric.js` & `JupyterQuiz-2.2.0/jupyterquiz/numeric.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/show_questions.js` & `JupyterQuiz-2.2.0/jupyterquiz/show_questions.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -109,18 +109,19 @@
         aDiv.id = "quizAns" + id + index;
         aDiv.className = 'Answer';
         iDiv.append(aDiv);
 
         //console.log(qa.type);
 
         var num_correct;
-        if (qa.type == "multiple_choice") {
-            num_correct = make_mc(qa, shuffle_answers, outerqDiv, qDiv, aDiv, id);
-        } else if (qa.type == "many_choice") {
+        if ((qa.type == "multiple_choice") || (qa.type == "many_choice")) {
             num_correct = make_mc(qa, shuffle_answers, outerqDiv, qDiv, aDiv, id);
+            if ("answer_cols" in qa) {
+                aDiv.style.gridTemplateColumns = 'auto '.repeat(qa.answer_cols);
+            }
         } else if (qa.type == "numeric") {
             //console.log("numeric");
             make_numeric(qa, outerqDiv, qDiv, aDiv, id);
         }
 
 
         //Make div for feedback
```

### Comparing `JupyterQuiz-2.1.5/jupyterquiz/styles.css` & `JupyterQuiz-2.2.0/jupyterquiz/styles.css`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/preserve-responses.ipynb` & `JupyterQuiz-2.2.0/preserve-responses.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/previews/github-preview.png` & `JupyterQuiz-2.2.0/previews/github-preview.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/previews/github-preview.psd` & `JupyterQuiz-2.2.0/previews/github-preview.psd`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/schema/mc_schema.json` & `JupyterQuiz-2.2.0/schema/mc_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/schema/mc_schema.png` & `JupyterQuiz-2.2.0/schema/mc_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/schema/num_schema.json` & `JupyterQuiz-2.2.0/schema/num_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/schema/num_schema.png` & `JupyterQuiz-2.2.0/schema/num_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/schema/schema.ipynb` & `JupyterQuiz-2.2.0/schema/schema.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.1.5/PKG-INFO` & `JupyterQuiz-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterQuiz
-Version: 2.1.5
+Version: 2.2.0
 Summary: Interactive quizzes for Jupyter and Jupyter Book
 Author-email: "John M. Shea" <jshea@ieee.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: home-page, https://github.com/jmshea/jupyterquiz
 
 # JupyterQuiz
```

