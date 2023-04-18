# Comparing `tmp/ipa-core-0.1.1.tar.gz` & `tmp/ipa-core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipa-core-0.1.1.tar", last modified: Wed Dec 21 10:24:18 2022, max compression
+gzip compressed data, was "ipa-core-0.1.2.tar", last modified: Tue Apr 18 14:55:20 2023, max compression
```

## Comparing `ipa-core-0.1.1.tar` & `ipa-core-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-21 10:24:03.000000 ipa-core-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2022-12-21 10:24:18.906382 ipa-core-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2022-12-21 10:24:03.000000 ipa-core-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-21 10:24:03.000000 ipa-core-0.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/ipa/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/ipa/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/ipa/data/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/data/sentence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/data/word.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/ipa/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/ipa/preprocessing/sentence_splitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/sentence_splitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/sentence_splitters/base_sentence_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/sentence_splitters/spacy_sentence_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/ipa/preprocessing/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/tokenizers/base_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/tokenizers/spacy_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/tokenizers/stanza_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/preprocessing/tokenizers/whitespace_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2022-12-21 10:24:03.000000 ipa-core-0.1.1/ipa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 10:24:18.906382 ipa-core-0.1.1/ipa_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2022-12-21 10:24:18.000000 ipa-core-0.1.1/ipa_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-21 10:24:18.000000 ipa-core-0.1.1/ipa_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 10:24:18.000000 ipa-core-0.1.1/ipa_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-21 10:24:18.000000 ipa-core-0.1.1/ipa_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-21 10:24:18.000000 ipa-core-0.1.1/ipa_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2022-12-21 10:24:03.000000 ipa-core-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-21 10:24:03.000000 ipa-core-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-21 10:24:18.910382 ipa-core-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2022-12-21 10:24:03.000000 ipa-core-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 14:55:09.000000 ipa-core-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-18 14:55:20.978759 ipa-core-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-18 14:55:09.000000 ipa-core-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 14:55:09.000000 ipa-core-0.1.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/ipa/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/ipa/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/ipa/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/data/sentence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/data/word.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/ipa/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/ipa/preprocessing/sentence_splitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/sentence_splitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/sentence_splitters/base_sentence_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/sentence_splitters/spacy_sentence_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/ipa/preprocessing/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/tokenizers/base_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/tokenizers/stanza_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/preprocessing/tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-18 14:55:09.000000 ipa-core-0.1.2/ipa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:20.978759 ipa-core-0.1.2/ipa_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-18 14:55:20.000000 ipa-core-0.1.2/ipa_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-18 14:55:20.000000 ipa-core-0.1.2/ipa_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:55:20.000000 ipa-core-0.1.2/ipa_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 14:55:20.000000 ipa-core-0.1.2/ipa_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 14:55:20.000000 ipa-core-0.1.2/ipa_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 14:55:09.000000 ipa-core-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 14:55:09.000000 ipa-core-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 14:55:20.978759 ipa-core-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-18 14:55:09.000000 ipa-core-0.1.2/setup.py
```

### Comparing `ipa-core-0.1.1/PKG-INFO` & `ipa-core-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipa-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: NLP Preprocessing Pipeline Wrappers
 Home-page: https://github.com/Riccorl/ipa
 Author: Riccardo Orlando
 Author-email: orlandoricc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch stanza spacy trankit preprocessing tokenization pos tagging lemmatization
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipa-core-0.1.1/README.md` & `ipa-core-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/common/logging.py` & `ipa-core-0.1.2/ipa/common/logging.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/common/utils.py` & `ipa-core-0.1.2/ipa/common/utils.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/data/sentence.py` & `ipa-core-0.1.2/ipa/data/sentence.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/data/word.py` & `ipa-core-0.1.2/ipa/data/word.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/preprocessing/sentence_splitters/base_sentence_splitter.py` & `ipa-core-0.1.2/ipa/preprocessing/sentence_splitters/base_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/preprocessing/sentence_splitters/spacy_sentence_splitter.py` & `ipa-core-0.1.2/ipa/preprocessing/sentence_splitters/spacy_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/preprocessing/tokenizers/__init__.py` & `ipa-core-0.1.2/ipa/preprocessing/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/preprocessing/tokenizers/base_tokenizer.py` & `ipa-core-0.1.2/ipa/preprocessing/tokenizers/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/preprocessing/tokenizers/spacy_tokenizer.py` & `ipa-core-0.1.2/ipa/preprocessing/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/preprocessing/tokenizers/stanza_tokenizer.py` & `ipa-core-0.1.2/ipa/preprocessing/tokenizers/stanza_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa/preprocessing/tokenizers/whitespace_tokenizer.py` & `ipa-core-0.1.2/ipa/preprocessing/tokenizers/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/ipa_core.egg-info/PKG-INFO` & `ipa-core-0.1.2/ipa_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipa-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: NLP Preprocessing Pipeline Wrappers
 Home-page: https://github.com/Riccorl/ipa
 Author: Riccardo Orlando
 Author-email: orlandoricc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch stanza spacy trankit preprocessing tokenization pos tagging lemmatization
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipa-core-0.1.1/ipa_core.egg-info/SOURCES.txt` & `ipa-core-0.1.2/ipa_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipa-core-0.1.1/setup.py` & `ipa-core-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipa-core",  # Replace with your own project name
-    version="0.1.1",
+    version="0.1.2",
     author="Riccardo Orlando",
     author_email="orlandoricc@gmail.com",
     description="NLP Preprocessing Pipeline Wrappers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Riccorl/ipa",
     keywords="NLP deep learning transformer pytorch stanza spacy trankit preprocessing"
```

