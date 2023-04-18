# Comparing `tmp/EmoTFIDF-1.1.0.tar.gz` & `tmp/EmoTFIDF-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmoTFIDF-1.1.0.tar", last modified: Mon Apr 17 21:01:59 2023, max compression
+gzip compressed data, was "EmoTFIDF-1.1.1.tar", last modified: Tue Apr 18 10:48:50 2023, max compression
```

## Comparing `EmoTFIDF-1.1.0.tar` & `EmoTFIDF-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-17 21:01:59.100029 EmoTFIDF-1.1.0/
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-17 21:01:59.099578 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2353 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/requires.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/top_level.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.0/LICENSE
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2353 2023-04-17 21:01:59.099823 EmoTFIDF-1.1.0/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1843 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.0/README.md
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4764 2023-04-17 17:02:30.000000 EmoTFIDF-1.1.0/emotfidf.py
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-17 21:01:59.100084 EmoTFIDF-1.1.0/setup.cfg
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-17 21:01:51.000000 EmoTFIDF-1.1.0/setup.py
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 10:48:50.323196 EmoTFIDF-1.1.1/
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 10:48:50.322777 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/requires.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.1/LICENSE
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 10:48:50.322995 EmoTFIDF-1.1.1/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.1/README.md
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4764 2023-04-17 17:02:30.000000 EmoTFIDF-1.1.1/emotfidf.py
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-18 10:48:50.323244 EmoTFIDF-1.1.1/setup.cfg
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-18 10:48:37.000000 EmoTFIDF-1.1.1/setup.py
```

### Comparing `EmoTFIDF-1.1.0/EmoTFIDF.egg-info/PKG-INFO` & `EmoTFIDF-1.1.1/EmoTFIDF.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,7 +81,11 @@
 
 
 Added a set_lexicon_path option if you would like to use your own lexicon
 Remember to keep the same structure as the original emotions lexicon which located [here](https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json)
 ```
 emTFIDF.set_lexicon_path("other_lexicon.json")
 ```
+
+##Update 1.1.1
+
+Updated the lexical db with some help from ChatGPT
```

### Comparing `EmoTFIDF-1.1.0/LICENSE` & `EmoTFIDF-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.0/PKG-INFO` & `EmoTFIDF-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,7 +81,11 @@
 
 
 Added a set_lexicon_path option if you would like to use your own lexicon
 Remember to keep the same structure as the original emotions lexicon which located [here](https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json)
 ```
 emTFIDF.set_lexicon_path("other_lexicon.json")
 ```
+
+##Update 1.1.1
+
+Updated the lexical db with some help from ChatGPT
```

### Comparing `EmoTFIDF-1.1.0/README.md` & `EmoTFIDF-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,8 +66,12 @@
 Thanks to [artofchores](https://www.reddit.com/user/artofchores/), from Reddit for his feedback.
 
 
 Added a set_lexicon_path option if you would like to use your own lexicon
 Remember to keep the same structure as the original emotions lexicon which located [here](https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json)
 ```
 emTFIDF.set_lexicon_path("other_lexicon.json")
-```
+```
+
+##Update 1.1.1
+
+Updated the lexical db with some help from ChatGPT
```

### Comparing `EmoTFIDF-1.1.0/emotfidf.py` & `EmoTFIDF-1.1.1/emotfidf.py`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.0/setup.py` & `EmoTFIDF-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         nltk.download('wordnet')
         nltk.download('punkt')
         nltk.download('stopwords')
 
 
 setuptools.setup(
     name="EmoTFIDF",
-    version="1.1.0",
+    version="1.1.1",
     author="mmsa12",
     author_email="mmsa12@gmail.com",
     description="A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion"
                 "2- Integrating TFIDF to add a context"
                 "Note that lexicon license is for research purposes only.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

