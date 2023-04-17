# Comparing `tmp/arabica-1.4.5.tar.gz` & `tmp/arabica-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.4.5.tar", last modified: Mon Apr 17 20:41:54 2023, max compression
+gzip compressed data, was "arabica-1.4.6.tar", last modified: Mon Apr 17 22:10:11 2023, max compression
```

## Comparing `arabica-1.4.5.tar` & `arabica-1.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:41:54.800879 arabica-1.4.5/
--rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.5/LICENSE
--rw-rw-rw-   0        0        0     7537 2023-04-17 20:41:54.800879 arabica-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     6767 2023-04-17 20:39:21.000000 arabica-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 20:41:54.739123 arabica-1.4.5/arabica/
--rw-rw-rw-   0        0        0      105 2023-04-17 20:38:04.000000 arabica-1.4.5/arabica/__init__.py
--rw-rw-rw-   0        0        0    11740 2023-04-16 21:14:18.000000 arabica-1.4.5/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.5/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.5/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.5/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.5/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.5/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.5/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.5/arabica/sentiment.py
--rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.5/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:41:54.800879 arabica-1.4.5/arabica.egg-info/
--rw-rw-rw-   0        0        0     7537 2023-04-17 20:41:54.000000 arabica-1.4.5/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-17 20:41:54.000000 arabica-1.4.5/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:41:54.000000 arabica-1.4.5/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-04-17 20:41:54.000000 arabica-1.4.5/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 20:41:54.000000 arabica-1.4.5/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-04-17 20:38:04.000000 arabica-1.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 20:41:54.818619 arabica-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-04-17 20:39:21.000000 arabica-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:10:11.499354 arabica-1.4.6/
+-rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0     7537 2023-04-17 22:10:11.499354 arabica-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 22:10:11.440319 arabica-1.4.6/arabica/
+-rw-rw-rw-   0        0        0      105 2023-04-17 22:07:56.000000 arabica-1.4.6/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11740 2023-04-17 21:41:36.000000 arabica-1.4.6/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.6/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.6/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.6/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.6/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.6/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.6/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.6/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.6/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:10:11.497356 arabica-1.4.6/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7537 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-04-17 22:07:56.000000 arabica-1.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:10:11.510482 arabica-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-17 22:07:56.000000 arabica-1.4.6/setup.py
```

### Comparing `arabica-1.4.5/PKG-INFO` & `arabica-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.5/README.md` & `arabica-1.4.6/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,8 @@
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
 * **Meta-data description:** TBA
 
 ---
 
-Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
+Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.4.5/arabica/arabica_freq.py` & `arabica-1.4.6/arabica/arabica_freq.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,22 +45,22 @@
     data=data.set_index(data['time'])
     data.replace("", float("NaN"), inplace=True)
     data.dropna(subset = ["text"], inplace=True)
 
     if skip is not None:
         data['text'] = data.text.str.replace('|'.join(skip), '.', regex=True).str.strip()
 
+    if stopwords is not None:
+        data['text'] = data.text.map(lambda x: remove_stopwords(x,stopwords=[stopwords]))
+
     if lower_case is True:
         data['text'] = np.vectorize(lower_casing)(data['text'])
 
     data['text'] = np.vectorize(preprocess)(data['text'])
 
-    if stopwords is not None:
-        data['text'] = data.text.map(lambda x: remove_stopwords(x,stopwords=[stopwords]))
-
     if numbers is True:
         data['text'] = np.vectorize(remove_numbers)(data['text'])
 
     periods = []
     unigrams_freq = []
     bigrams_freq = []
     trigrams_freq = []
```

### Comparing `arabica-1.4.5/arabica/cappuccino.py` & `arabica-1.4.6/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.5/arabica/clean_ngram.py` & `arabica-1.4.6/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.5/arabica/coffee_break.py` & `arabica-1.4.6/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.5/arabica/group.py` & `arabica-1.4.6/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.5/arabica/preprocess.py` & `arabica-1.4.6/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.5/arabica.egg-info/PKG-INFO` & `arabica-1.4.6/arabica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.5/pyproject.toml` & `arabica-1.4.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.4.5"
+version = "1.4.6"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.4.5/setup.py` & `arabica-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.4.5",
+        version="1.4.6",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

