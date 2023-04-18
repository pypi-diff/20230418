# Comparing `tmp/EmoTFIDF-1.1.1.tar.gz` & `tmp/EmoTFIDF-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmoTFIDF-1.1.1.tar", last modified: Tue Apr 18 10:48:50 2023, max compression
+gzip compressed data, was "EmoTFIDF-1.1.2.tar", last modified: Tue Apr 18 11:52:48 2023, max compression
```

## Comparing `EmoTFIDF-1.1.1.tar` & `EmoTFIDF-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 10:48:50.323196 EmoTFIDF-1.1.1/
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 10:48:50.322777 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/requires.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-18 10:48:50.000000 EmoTFIDF-1.1.1/EmoTFIDF.egg-info/top_level.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.1/LICENSE
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 10:48:50.322995 EmoTFIDF-1.1.1/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.1/README.md
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4764 2023-04-17 17:02:30.000000 EmoTFIDF-1.1.1/emotfidf.py
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-18 10:48:50.323244 EmoTFIDF-1.1.1/setup.cfg
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-18 10:48:37.000000 EmoTFIDF-1.1.1/setup.py
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 11:52:48.413936 EmoTFIDF-1.1.2/
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 11:52:48.413566 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/requires.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.2/LICENSE
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 11:52:48.413761 EmoTFIDF-1.1.2/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.2/README.md
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4801 2023-04-18 11:51:14.000000 EmoTFIDF-1.1.2/emotfidf.py
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-18 11:52:48.413987 EmoTFIDF-1.1.2/setup.cfg
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-18 11:52:35.000000 EmoTFIDF-1.1.2/setup.py
```

### Comparing `EmoTFIDF-1.1.1/EmoTFIDF.egg-info/PKG-INFO` & `EmoTFIDF-1.1.2/EmoTFIDF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.1/LICENSE` & `EmoTFIDF-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.1/PKG-INFO` & `EmoTFIDF-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.1/README.md` & `EmoTFIDF-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.1/emotfidf.py` & `EmoTFIDF-1.1.2/emotfidf.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # get emotions
     em_list = []
     em_dict = dict()
     em_frequencies = Counter()
     lexicon_keys = self.lexicon.keys()
     for word in self.words:
         if word in lexicon_keys:
-            emotions_found = self.lexicon[word]
+            emotions_found = list(set([s for s in self.lexicon[word] if s.strip()]))
             if emotions_found is not None:
                 if 'negative' in emotions_found:
                     emotions_found.remove('negative')
                 elif 'positive' in emotions_found:
                     emotions_found.remove('positive')
                 em_list.extend(emotions_found)
                 em_dict.update({word: self.lexicon[word]})
```

### Comparing `EmoTFIDF-1.1.1/setup.py` & `EmoTFIDF-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         nltk.download('wordnet')
         nltk.download('punkt')
         nltk.download('stopwords')
 
 
 setuptools.setup(
     name="EmoTFIDF",
-    version="1.1.1",
+    version="1.1.2",
     author="mmsa12",
     author_email="mmsa12@gmail.com",
     description="A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion"
                 "2- Integrating TFIDF to add a context"
                 "Note that lexicon license is for research purposes only.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

