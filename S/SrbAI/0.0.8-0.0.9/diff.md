# Comparing `tmp/SrbAI-0.0.8.tar.gz` & `tmp/SrbAI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SrbAI/SrbAI/dist/.tmp-7bty1fnt/SrbAI-0.0.8.tar", last modified: Sun Apr 16 16:43:09 2023, max compression
+gzip compressed data, was "/home/runner/work/SrbAI/SrbAI/dist/.tmp-0wk43we8/SrbAI-0.0.9.tar", last modified: Sun Apr 16 19:00:19 2023, max compression
```

## Comparing `SrbAI-0.0.8.tar` & `SrbAI-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 16:41:27.000000 SrbAI-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-16 16:43:09.000000 SrbAI-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-16 16:41:27.000000 SrbAI-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 16:41:27.000000 SrbAI-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:43:09.000000 SrbAI-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-16 16:41:27.000000 SrbAI-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/SrbAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/SrbAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/SrbAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/SrbAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/SrbAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/SrbAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/Alati/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/Alati/Transliterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/Alati/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/Glas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/Glas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/text_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/JezickiModeli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/Klasifikatori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/Klasifikatori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/NER/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/NER/NER_classla.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/NER/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:43:09.000000 SrbAI-0.0.8/src/srbai/SintaktickiOperatori/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/SintaktickiOperatori/POS_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/SintaktickiOperatori/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/SintaktickiOperatori/spellcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/SintaktickiOperatori/stemmer_nm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 16:41:27.000000 SrbAI-0.0.8/src/srbai/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 18:58:37.000000 SrbAI-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-16 19:00:19.000000 SrbAI-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-16 18:58:37.000000 SrbAI-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 18:58:37.000000 SrbAI-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 19:00:19.000000 SrbAI-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-16 18:58:37.000000 SrbAI-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/SrbAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/SrbAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/SrbAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/SrbAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/SrbAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/SrbAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/Alati/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/Alati/Transliterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/Alati/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/Glas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/Glas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/JezickiModeli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/Klasifikatori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/Klasifikatori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/NER/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/NER/NER_classla.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/NER/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:00:19.000000 SrbAI-0.0.9/src/srbai/SintaktickiOperatori/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/SintaktickiOperatori/POS_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/SintaktickiOperatori/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/SintaktickiOperatori/spellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/SintaktickiOperatori/stemmer_nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 18:58:37.000000 SrbAI-0.0.9/src/srbai/test.py
```

### Comparing `SrbAI-0.0.8/LICENSE` & `SrbAI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/PKG-INFO` & `SrbAI-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SrbAI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for processing serbian language
 Home-page: https://github.com/Serbian-AI-Society/SrbAI
 Author: Serbian AI Society
 Author-email: nikola.milosevic86@gmail.com
 Project-URL: Bug Tracker, https://github.com/Serbian-AI-Society/SrbAI/issues
 Project-URL: Road Map, https://github.com/Serbian-AI-Society/SrbAI/projects/1
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SrbAI-0.0.8/README.md` & `SrbAI-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/setup.py` & `SrbAI-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SrbAI",
-    version="0.0.8",
+    version="0.0.9",
     author="Serbian AI Society",
     author_email="nikola.milosevic86@gmail.com",
     description="Library for processing serbian language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Serbian-AI-Society/SrbAI",
     project_urls={
@@ -26,10 +26,12 @@
         "nltk",
         "torch>=1.10.2",
         "classla==1.1.0",
         "nlu"
 
     ],
     package_dir={"": "src"},
+    package_data={'': ['src/srbai/Resursi/*']},
+    include_package_data=True,
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
 )
```

### Comparing `SrbAI-0.0.8/src/SrbAI.egg-info/PKG-INFO` & `SrbAI-0.0.9/src/SrbAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SrbAI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for processing serbian language
 Home-page: https://github.com/Serbian-AI-Society/SrbAI
 Author: Serbian AI Society
 Author-email: nikola.milosevic86@gmail.com
 Project-URL: Bug Tracker, https://github.com/Serbian-AI-Society/SrbAI/issues
 Project-URL: Road Map, https://github.com/Serbian-AI-Society/SrbAI/projects/1
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SrbAI-0.0.8/src/SrbAI.egg-info/SOURCES.txt` & `SrbAI-0.0.9/src/SrbAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/Alati/Transliterator.py` & `SrbAI-0.0.9/src/srbai/Alati/Transliterator.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/__main__.py` & `SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/__main__.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/embedding.py` & `SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/embedding.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/globals.py` & `SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/globals.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/io_utils.py` & `SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/io_utils.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/model.py` & `SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/model.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/similarity.py` & `SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/similarity.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/JezickiModeli/FastText/text_preprocessing.py` & `SrbAI-0.0.9/src/srbai/JezickiModeli/FastText/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/SintaktickiOperatori/POS_tagger.py` & `SrbAI-0.0.9/src/srbai/SintaktickiOperatori/POS_tagger.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/SintaktickiOperatori/spellcheck.py` & `SrbAI-0.0.9/src/srbai/SintaktickiOperatori/spellcheck.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.8/src/srbai/SintaktickiOperatori/stemmer_nm.py` & `SrbAI-0.0.9/src/srbai/SintaktickiOperatori/stemmer_nm.py`

 * *Files identical despite different names*

