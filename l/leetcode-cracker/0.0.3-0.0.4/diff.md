# Comparing `tmp/leetcode_cracker-0.0.3.tar.gz` & `tmp/leetcode_cracker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetcode_cracker-0.0.3.tar", last modified: Mon Apr 10 10:33:59 2023, max compression
+gzip compressed data, was "leetcode_cracker-0.0.4.tar", last modified: Mon Apr 17 22:55:36 2023, max compression
```

## Comparing `leetcode_cracker-0.0.3.tar` & `leetcode_cracker-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.655075 leetcode_cracker-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-04-10 10:33:59.654078 leetcode_cracker-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2023-04-08 07:25:56.000000 leetcode_cracker-0.0.3/README.md
--rw-rw-rw-   0        0        0      658 2023-04-06 23:36:59.000000 leetcode_cracker-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 10:33:59.655075 leetcode_cracker-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.563600 leetcode_cracker-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.636638 leetcode_cracker-0.0.3/src/leetcode_cracker/
--rw-rw-rw-   0        0        0       21 2023-04-10 10:32:27.000000 leetcode_cracker-0.0.3/src/leetcode_cracker/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-04-10 10:32:09.000000 leetcode_cracker-0.0.3/src/leetcode_cracker/question_392.py
--rw-rw-rw-   0        0        0       37 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.3/src/leetcode_cracker/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.652085 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.905677 leetcode_cracker-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2276 2023-04-17 22:55:36.898683 leetcode_cracker-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1797 2023-04-15 09:14:08.000000 leetcode_cracker-0.0.4/README.md
+-rw-rw-rw-   0        0        0      658 2023-04-06 23:36:59.000000 leetcode_cracker-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:55:36.906675 leetcode_cracker-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.210407 leetcode_cracker-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.814512 leetcode_cracker-0.0.4/src/leetcode_cracker/
+-rw-rw-rw-   0        0        0       21 2023-04-17 22:46:56.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-04-13 09:41:16.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_121.py
+-rw-rw-rw-   0        0        0      923 2023-04-12 00:35:15.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_169.py
+-rw-rw-rw-   0        0        0      780 2023-04-11 01:29:59.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_268.py
+-rw-rw-rw-   0        0        0     1149 2023-04-12 00:18:35.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_283.py
+-rw-rw-rw-   0        0        0     1206 2023-04-11 01:28:11.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/question_392.py
+-rw-rw-rw-   0        0        0       37 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.4/src/leetcode_cracker/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:55:36.894746 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/
+-rw-rw-rw-   0        0        0     2276 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-17 22:55:36.000000 leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/top_level.txt
```

### Comparing `leetcode_cracker-0.0.3/LICENSE` & `leetcode_cracker-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.3/PKG-INFO` & `leetcode_cracker-0.0.4/src/leetcode_cracker.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: leetcode_cracker
-Version: 0.0.3
+Name: leetcode-cracker
+Version: 0.0.4
 Summary: package to assist in solving Leetcode Problems
 Author-email: Albert <albertyqyao@gmail.com>
 Project-URL: Homepage, https://github.com/AlbertY123/leetcode-cracker
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -21,9 +21,22 @@
 - Compare your code with other solutions and learn from different approaches
 
 Leetcode Cracker is designed to help you improve your coding skills and ace your technical interviews. It is easy to install and use.
 
 # How to use the package
 
 1. Import the package: `pip install leetcode-cracker`
-2. Import package locally: `from leetcode_cracker import question_question number`
-3. Call a command: `question_question number.print_solution()`
+2. Import package locally: `from leetcode_cracker import question_392`
+3. Call for question: `question_392.print_question()`
+4. Call for solution: `question_392.print_solution()`
+5. Call for solution stats `question_392.solution_stats()`
+
+# Question Database
+
+# Easy
+
+Question 121 - Best time to buy and sell stock
+Question 169 - Majority Element
+Question 268 - Missing Number
+Question 283 - Moving Zeros
+Question 392 - Is Subsequence
+Question 2469 - Convert the Tempreture
```

### Comparing `leetcode_cracker-0.0.3/pyproject.toml` & `leetcode_cracker-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.3/src/leetcode_cracker/question_392.py` & `leetcode_cracker-0.0.4/src/leetcode_cracker/question_392.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,9 +24,15 @@
                 j += 1
         #If the function has finnished running, return true.
         if i == len(s):
             return True
         else:
             return False
     """)
+def solution_stats():
+    print("""
+        Time: Beats 30.59%
+        Memory: Beats 30.17%
+    """)
+
```

