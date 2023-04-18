# Comparing `tmp/sesg-0.0.5.tar.gz` & `tmp/sesg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesg-0.0.5.tar", max compression
+gzip compressed data, was "sesg-0.0.6.tar", max compression
```

## Comparing `sesg-0.0.5.tar` & `sesg-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.5/LICENSE
--rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.5/README.md
--rw-r--r--   0        0        0     2779 2023-04-18 12:05:47.964047 sesg-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.5/src/sesg/__init__.py
--rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.5/src/sesg/graph.py
--rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.5/src/sesg/metrics.py
--rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.5/src/sesg/scopus/__init__.py
--rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.5/src/sesg/scopus/api.py
--rw-r--r--   0        0        0     6080 2023-04-18 12:05:40.816197 sesg-0.0.5/src/sesg/scopus/client.py
--rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.5/src/sesg/scopus_client.py
--rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.5/src/sesg/search_string.py
--rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.5/src/sesg/snowballing.py
--rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.5/src/sesg/topic_extraction.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.6/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.6/README.md
+-rw-r--r--   0        0        0     2801 2023-04-18 16:48:51.447223 sesg-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.6/src/sesg/__init__.py
+-rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.6/src/sesg/graph.py
+-rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.6/src/sesg/metrics.py
+-rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.6/src/sesg/scopus/__init__.py
+-rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.6/src/sesg/scopus/api.py
+-rw-r--r--   0        0        0     6080 2023-04-18 12:05:40.816197 sesg-0.0.6/src/sesg/scopus/client.py
+-rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.6/src/sesg/scopus_client.py
+-rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.6/src/sesg/search_string.py
+-rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.6/src/sesg/snowballing.py
+-rw-r--r--   0        0        0     6042 2023-04-18 16:47:52.299822 sesg-0.0.6/src/sesg/topic_extraction.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 sesg-0.0.6/PKG-INFO
```

### Comparing `sesg-0.0.5/LICENSE` & `sesg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/pyproject.toml` & `sesg-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sesg"
-version = "0.0.5"
+version = "0.0.6"
 description = "SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string."
 authors = ["Demetrius Panovitch <demetrius.mp789@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
   {include = "sesg", from = "src"}
 ]
@@ -29,14 +29,15 @@
 httpx = "^0.24.0"
 graphviz = "^0.20.1"
 scikit-learn = "^1.2.2"
 levenshtein = "^0.20.9"
 torch = "^2.0.0"
 nltk = "^3.8.1"
 numpy = "1.23.5"
+umap-learn = "^0.5.3"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.261"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `sesg-0.0.5/src/sesg/graph.py` & `sesg-0.0.6/src/sesg/graph.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/src/sesg/metrics.py` & `sesg-0.0.6/src/sesg/metrics.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/src/sesg/scopus/api.py` & `sesg-0.0.6/src/sesg/scopus/api.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/src/sesg/scopus/client.py` & `sesg-0.0.6/src/sesg/scopus/client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/src/sesg/scopus_client.py` & `sesg-0.0.6/src/sesg/scopus_client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/src/sesg/search_string.py` & `sesg-0.0.6/src/sesg/search_string.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/src/sesg/snowballing.py` & `sesg-0.0.6/src/sesg/snowballing.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.5/src/sesg/topic_extraction.py` & `sesg-0.0.6/src/sesg/topic_extraction.py`

 * *Files 12% similar despite different names*

```diff
@@ -114,41 +114,58 @@
 
     return topics
 
 
 def extract_topics_with_bertopic(
     *,
     docs: List[str],
+    top_n_words: int,
+    min_topic_size: int,
+    umap_n_neighbors: int,
 ) -> List[List[str]]:
     """Extracts topics from a list of documents using BERTopic.
 
     Args:
         docs (List[str]): List of documents.
+        top_n_words (int): Number of words per topic to extract. Setting this too high can negatively impact topic embeddings as topics are typically best represented by at most 10 words.
+        min_topic_size (int): Minimum size of the topic. Increasing this value will lead to a lower number of clusters/topics.
+        umap_n_neighbors (int): Number of neighboring sample points used when making the manifold approximation. Increasing this value typically results in a more global view of the embedding structure whilst smaller values result in a more local view. Increasing this value often results in larger clusters being created.
 
     Returns:
         List of topics, where a topic is a list of words.
 
     Examples:
         >>> extract_topics_with_bertopic(  # doctest: +SKIP
         ...     docs=["detecting code smells with machine learning", "code smells detection tools", "error detection in Java software with machine learning"],
         ... )
         [["word1 topic1", "word2 topic1"], ["word1 topic2", "word2 topic2"]]
     """  # noqa: E501
     from bertopic import BERTopic
+    from umap.umap_ import UMAP
 
     vectorizer_model = CountVectorizer(
         stop_words="english",
         ngram_range=(1, 3),
     )
 
+    umap_model = UMAP(
+        n_neighbors=umap_n_neighbors,
+        n_components=5,
+        min_dist=0.0,
+        metric="cosine",
+        low_memory=False,
+    )
+
     topic_model = BERTopic(
         language="english",
         verbose=True,
-        min_topic_size=2,
+        top_n_words=top_n_words,
+        min_topic_size=min_topic_size,
         vectorizer_model=vectorizer_model,
+        umap_model=umap_model,
     )
 
     topic_model.fit_transform(docs)
 
     # topic_model.get_topics() will return a Mapping where
     # the key is the index of the topic,
     # and the value is a list of tuples
```

### Comparing `sesg-0.0.5/PKG-INFO` & `sesg-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesg
-Version: 0.0.5
+Version: 0.0.6
 Summary: SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string.
 License: GPL-3.0-only
 Author: Demetrius Panovitch
 Author-email: demetrius.mp789@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -19,14 +19,15 @@
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: levenshtein (>=0.20.9,<0.21.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: thefuzz[speedup] (>=0.19.0,<0.20.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
 Project-URL: Documentation, https://sesg-package.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/demetrius-mp/sesg-package/issues
 Project-URL: Source Code, https://github.com/demetrius-mp/sesg-package
 Description-Content-Type: text/markdown
 
 # sesg-package
```

