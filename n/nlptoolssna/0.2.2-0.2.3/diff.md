# Comparing `tmp/nlptoolssna-0.2.2.tar.gz` & `tmp/nlptoolssna-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.2.2.tar", last modified: Sat Apr 15 20:24:26 2023, max compression
+gzip compressed data, was "nlptoolssna-0.2.3.tar", last modified: Tue Apr 18 08:39:04 2023, max compression
```

## Comparing `nlptoolssna-0.2.2.tar` & `nlptoolssna-0.2.3.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.800378 nlptoolssna-0.2.2/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-15 20:24:26.801413 nlptoolssna-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.749244 nlptoolssna-0.2.2/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.756028 nlptoolssna-0.2.2/nlptools/
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.758951 nlptoolssna-0.2.2/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.2.2/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.773970 nlptoolssna-0.2.2/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.2.2/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.2.2/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.2.2/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0    10250 2023-04-15 20:21:10.000000 nlptoolssna-0.2.2/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.2.2/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.2.2/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.779829 nlptoolssna-0.2.2/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.2.2/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.2.2/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.795550 nlptoolssna-0.2.2/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-15 20:24:26.000000 nlptoolssna-0.2.2/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-04-15 20:24:26.000000 nlptoolssna-0.2.2/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 20:24:26.000000 nlptoolssna-0.2.2/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-15 20:24:26.000000 nlptoolssna-0.2.2/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.2.2/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       45 2023-04-15 20:24:26.000000 nlptoolssna-0.2.2/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 20:24:26.000000 nlptoolssna-0.2.2/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      403 2023-04-15 20:24:26.803364 nlptoolssna-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1611 2023-04-15 20:22:52.000000 nlptoolssna-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:24:26.799400 nlptoolssna-0.2.2/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.2.2/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.157757 nlptoolssna-0.2.3/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-18 08:39:04.157757 nlptoolssna-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.101660 nlptoolssna-0.2.3/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.108326 nlptoolssna-0.2.3/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.110327 nlptoolssna-0.2.3/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.2.3/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     1304 2023-04-18 08:31:42.000000 nlptoolssna-0.2.3/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.118681 nlptoolssna-0.2.3/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.2.3/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.131176 nlptoolssna-0.2.3/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.2.3/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.2.3/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.2.3/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     9426 2023-04-18 08:38:01.000000 nlptoolssna-0.2.3/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.2.3/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.2.3/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.136423 nlptoolssna-0.2.3/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.2.3/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.2.3/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.151816 nlptoolssna-0.2.3/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       45 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      403 2023-04-18 08:39:04.159738 nlptoolssna-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2023-04-18 08:38:23.000000 nlptoolssna-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.155762 nlptoolssna-0.2.3/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.2.2/CONTRIBUTING.rst` & `nlptoolssna-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/LICENSE` & `nlptoolssna-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/PKG-INFO` & `nlptoolssna-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.2.2/README.rst` & `nlptoolssna-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/docs/Makefile` & `nlptoolssna-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/docs/conf.py` & `nlptoolssna-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/docs/installation.rst` & `nlptoolssna-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/docs/make.bat` & `nlptoolssna-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/nlptools/data/my_data.pickle` & `nlptoolssna-0.2.3/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/nlptools/morph/charsets.py` & `nlptoolssna-0.2.3/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.2.3/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.2.3/nlptools/morph/morph_tagger.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,67 +4,45 @@
 from nlptools.morph.lemmatizeSentence import lemmatize_sentence
 from nlptools.morph.tokenizers_words import simple_word_tokenize
 from nlptools.parse.parser import arStrip
 import os.path
 import requests 
 import json
 import urllib.request
-def load_json_file():
-    # URL of the JSON file on GitHub
-    url = 'https://github.com/eng-aomar/ts/raw/main/500.json'
-
-    # Directory to save the JSON file in
-    package_directory = os.path.dirname(os.path.abspath(__file__))
-
-    # Download the file from the URL
-    filename, headers = urllib.request.urlretrieve(url, package_directory+'/500.json')
-
-    # Load the data from the file into a Python object
-    with open(filename, 'r') as f:
-        my_dict = json.load(f)
-    return my_dict
+from nlptools.DataDownload import downloader
+# def load_json_file():
+#     # URL of the JSON file on GitHub
+#     url = 'https://github.com/eng-aomar/ts/raw/main/500.json'
+
+#     # Directory to save the JSON file in
+#     package_directory = os.path.dirname(os.path.abspath(__file__))
+
+#     # Download the file from the URL
+#     filename, headers = urllib.request.urlretrieve(url, package_directory+'/500.json')
+
+#     # Load the data from the file into a Python object
+#     with open(filename, 'r') as f:
+#         my_dict = json.load(f)
+#    return my_dict
 
 def load_ALMA_dic():
-    """
-    Load the ALMA dictionary from a binary pickle file.
-
-    Args:
-    - file_path: str - The path of the binary pickle file containing the ALMA dictionary.
+   # Open the Pickle file in binary mode
+    filename = 'my_data.pickle'
+    path =downloader._get_appdatadir()
+    file_path = os.path.join(path, filename)
+    
 
-    Returns:
-    - dict: A dictionary containing the ALMA dictionary data.
+    with open(file_path, 'rb') as f:
+       #Load the serialized data from the file
+       ALMA_dic = pickle.load(f)
+       print(ALMA_dic)
+       return ALMA_dic
 
-    Raises:
-    - FileNotFoundError: If the file specified in file_path cannot be found.
-    - pickle.UnpicklingError: If an error occurred while unpickling the data.
-    """
-    # URL of the .pickle file on GitHub
-    url = 'https://raw.githubusercontent.com/eng-aomar/ts/main/500.json'
 
 
-    try:
-        # Download the file from the URL
-        #response = requests.get(url)
-        #data = response.content
-        #Load the data from the file into a Python object
-        #data = pickle.loads(response.content)
-        # with open(file_to_open, 'rb') as f:
-        #     ALMA_dic = pickle.load(f)
-        # #my_dict = pickle.loads(data)
-        # return ALMA_dic
-        response = requests.get(url)
-        data = response.json()
-        return data
-
-    except FileNotFoundError as e:
-        print(f"File not found: {url}")
-        raise e
-    except pickle.UnpicklingError as e:
-        print("Error while unpickling the data.")
-        raise e
 # def load_ALMA_dic(file):
 #     """
 #     Load the ALMA dictionary from a binary pickle file.
 
 #     Args:
 #     - file_path: str - The path of the binary pickle file containing the ALMA dictionary.
 
@@ -236,15 +214,15 @@
         list: A list of lists, where each sublist contains information about a word in the input sentence, including 
               the original word, its lemma, its part of speech (POS) tag, and its lemma frequency.
     """
     
     # Check if the ALMA dictionary has been loaded
     if settings.flag == True:
         settings.flag = False
-    settings.div_dic = load_json_file()
+    settings.div_dic = load_ALMA_dic()
    
     
     # Perform lemmatization on the input sentence
     output_list = lemmatize_sentence(text,lang, task)
     
     # Return the list of lemmatized words
     return output_list
```

### Comparing `nlptoolssna-0.2.2/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.2.3/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/nlptools/parse/parser.py` & `nlptoolssna-0.2.3/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.2/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.2.3/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.2.2/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.2.3/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
+nlptools/DataDownload/__init__.py
+nlptools/DataDownload/downloader.py
 nlptools/data/my_data.pickle
 nlptools/morph/__init__.py
 nlptools/morph/charsets.py
 nlptools/morph/lemmatizeSentence.py
 nlptools/morph/morph_tagger.py
 nlptools/morph/settings.py
 nlptools/morph/tokenizers_words.py
```

### Comparing `nlptoolssna-0.2.2/setup.py` & `nlptoolssna-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     include_package_data=True,
     keywords='nlptools',
     name='nlptoolssna',
     packages=find_packages(include=['nlptools', 'nlptools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/nlptools',
-    version='0.2.2',
+    version='0.2.3',
     zip_safe=False,
 )
```

