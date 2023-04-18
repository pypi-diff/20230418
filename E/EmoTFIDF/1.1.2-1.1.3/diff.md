# Comparing `tmp/EmoTFIDF-1.1.2.tar.gz` & `tmp/EmoTFIDF-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmoTFIDF-1.1.2.tar", last modified: Tue Apr 18 11:52:48 2023, max compression
+gzip compressed data, was "EmoTFIDF-1.1.3.tar", last modified: Tue Apr 18 17:10:45 2023, max compression
```

## Comparing `EmoTFIDF-1.1.2.tar` & `EmoTFIDF-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 11:52:48.413936 EmoTFIDF-1.1.2/
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 11:52:48.413566 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/requires.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-18 11:52:48.000000 EmoTFIDF-1.1.2/EmoTFIDF.egg-info/top_level.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.2/LICENSE
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 11:52:48.413761 EmoTFIDF-1.1.2/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.2/README.md
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4801 2023-04-18 11:51:14.000000 EmoTFIDF-1.1.2/emotfidf.py
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-18 11:52:48.413987 EmoTFIDF-1.1.2/setup.cfg
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-18 11:52:35.000000 EmoTFIDF-1.1.2/setup.py
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 17:10:45.610976 EmoTFIDF-1.1.3/
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-18 17:10:45.610564 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/requires.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-18 17:10:45.000000 EmoTFIDF-1.1.3/EmoTFIDF.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.3/LICENSE
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-18 17:10:45.610794 EmoTFIDF-1.1.3/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.3/README.md
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4804 2023-04-18 12:02:05.000000 EmoTFIDF-1.1.3/emotfidf.py
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-18 17:10:45.611027 EmoTFIDF-1.1.3/setup.cfg
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-18 17:10:18.000000 EmoTFIDF-1.1.3/setup.py
```

### Comparing `EmoTFIDF-1.1.2/EmoTFIDF.egg-info/PKG-INFO` & `EmoTFIDF-1.1.3/EmoTFIDF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.2/LICENSE` & `EmoTFIDF-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.2/PKG-INFO` & `EmoTFIDF-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.2/README.md` & `EmoTFIDF-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.2/emotfidf.py` & `EmoTFIDF-1.1.3/emotfidf.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,14 @@
         em_frequencies = Counter()
         for word in self.em_list:
             em_frequencies[word] += 1
         for e in self.em_dict.keys():
             if e in self.ifidf_for_words:
                 tfidf_weight = self.ifidf_for_words[e]
                 for a in self.em_dict[e]:
-                    new_fre = round(em_frequencies[a] / tfidf_weight, 2)
+                    new_fre = round(em_frequencies[a] / tfidf_weight*2 , 2)
                     em_frequencies[a] = new_fre
         sum_values = sum(em_frequencies.values())
         for key in em_frequencies.keys():
             em_percent.update({key: round(float(em_frequencies[key]) / float(sum_values), 3)})
         self.em_tfidf = em_percent
         self.em_tfidf = em_percent
```

### Comparing `EmoTFIDF-1.1.2/setup.py` & `EmoTFIDF-1.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         nltk.download('wordnet')
         nltk.download('punkt')
         nltk.download('stopwords')
 
 
 setuptools.setup(
     name="EmoTFIDF",
-    version="1.1.2",
+    version="1.1.3",
     author="mmsa12",
     author_email="mmsa12@gmail.com",
     description="A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion"
                 "2- Integrating TFIDF to add a context"
                 "Note that lexicon license is for research purposes only.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

