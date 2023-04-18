# Comparing `tmp/hugging_py_face-0.1.0.tar.gz` & `tmp/hugging_py_face-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hugging_py_face-0.1.0.tar", last modified: Tue Apr 18 10:56:29 2023, max compression
+gzip compressed data, was "dist\hugging_py_face-0.1.1.tar", last modified: Tue Apr 18 17:55:57 2023, max compression
```

## Comparing `hugging_py_face-0.1.0.tar` & `hugging_py_face-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/
--rw-rw-rw-   0        0        0     5915 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4550 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face/
--rw-rw-rw-   0        0        0      422 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/__about__.py
--rw-rw-rw-   0        0        0      112 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/__init__.py
--rw-rw-rw-   0        0        0     3877 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/audio_processing.py
--rw-rw-rw-   0        0        0     2844 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/computer_vision.py
--rw-rw-rw-   0        0        0      320 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/config_parser.py
--rw-rw-rw-   0        0        0     1479 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/multimedia_processing.py
--rw-rw-rw-   0        0        0    17241 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/nlp.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/
--rw-rw-rw-   0        0        0     5915 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      940 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/
+-rw-rw-rw-   0        0        0     6177 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4692 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face/
+-rw-rw-rw-   0        0        0      466 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/__about__.py
+-rw-rw-rw-   0        0        0      112 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/__init__.py
+-rw-rw-rw-   0        0        0     3877 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/audio_processing.py
+-rw-rw-rw-   0        0        0     2844 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face/config/
+-rw-rw-rw-   0        0        0      719 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/config/config.yaml
+-rw-rw-rw-   0        0        0      320 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/config_parser.py
+-rw-rw-rw-   0        0        0     1479 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/multimedia_processing.py
+-rw-rw-rw-   0        0        0    17264 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/nlp.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/
+-rw-rw-rw-   0        0        0     6177 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/setup.py
```

### Comparing `hugging_py_face-0.1.0/PKG-INFO` & `hugging_py_face-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: hugging_py_face
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
-License: UNKNOWN
+License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
+        Copyright Â© 2023 Minura Punchihewa
+        
         Hugging-Py-Face is a powerful Python package that provides seamless integration with the Hugging Face Inference API, allowing you to easily perform inference on your machine learning models hosted on the Hugging Face Model Hub. 
         
         One of the key benefits of using the Hugging Face Inference API is that it provides a scalable and efficient way to perform inference on your models, by allowing you to easily deploy and serve your models in the cloud. Additionally, the Inference API provides a simple and standardized API that can be used across different programming languages, making it easy to integrate your models with other services and tools.
         
         With Hugging-Py-Face, you can take advantage of these benefits while also enjoying the simplicity and flexibility of using Python.
         
         It allows you to easily customize your API requests, adjust request parameters, handle authentication and access tokens, and interact with a wide range of machine learning models hosted on the Hugging Face Model Hub.
@@ -106,12 +108,16 @@
         ```
         
         Additionally, both of the above tasks can also be performed on a pandas DataFrame. For example:
         ```
         ap.audio_classification_in_df(df, 'audio')
         # where df is a pandas DataFrame and 'audio' is the column name containing the audio file paths or URLs
         ```
+        
+        # License
+        This code is licensed under the GNU GENERAL PUBLIC LICENSE. See LICENSE.txt for details.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hugging_py_face-0.1.0/README.md` & `hugging_py_face-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Hugging-Py-Face
+Copyright © 2023 Minura Punchihewa
+
 Hugging-Py-Face is a powerful Python package that provides seamless integration with the Hugging Face Inference API, allowing you to easily perform inference on your machine learning models hosted on the Hugging Face Model Hub. 
 
 One of the key benefits of using the Hugging Face Inference API is that it provides a scalable and efficient way to perform inference on your models, by allowing you to easily deploy and serve your models in the cloud. Additionally, the Inference API provides a simple and standardized API that can be used across different programming languages, making it easy to integrate your models with other services and tools.
 
 With Hugging-Py-Face, you can take advantage of these benefits while also enjoying the simplicity and flexibility of using Python.
 
 It allows you to easily customize your API requests, adjust request parameters, handle authentication and access tokens, and interact with a wide range of machine learning models hosted on the Hugging Face Model Hub.
@@ -96,8 +98,11 @@
 ap.audio_classification(["dogs.wav", "cats.wav"])
 ```
 
 Additionally, both of the above tasks can also be performed on a pandas DataFrame. For example:
 ```
 ap.audio_classification_in_df(df, 'audio')
 # where df is a pandas DataFrame and 'audio' is the column name containing the audio file paths or URLs
-```
+```
+
+# License
+This code is licensed under the GNU GENERAL PUBLIC LICENSE. See LICENSE.txt for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hugging_py_face-0.1.0/hugging_py_face/audio_processing.py` & `hugging_py_face-0.1.1/hugging_py_face/audio_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.1.0/hugging_py_face/computer_vision.py` & `hugging_py_face-0.1.1/hugging_py_face/computer_vision.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.1.0/hugging_py_face/multimedia_processing.py` & `hugging_py_face-0.1.1/hugging_py_face/multimedia_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.1.0/hugging_py_face/nlp.py` & `hugging_py_face-0.1.1/hugging_py_face/nlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         :param df: a pandas DataFrame containing the strings to be summarized.
         :param column: the column containing the strings to be summarized.
         :param parameters: a dict of parameters. For more information, see the `detailed parameters for the summarization task <https://huggingface.co/docs/api-inference/detailed_parameters#summarization-task>`_.
         :param options: a dict of options. For more information, see the `detailed parameters for the summarization task <https://huggingface.co/docs/api-inference/detailed_parameters#summarization-task>`_.
         :param model: the model to use for the summarization task. If not provided, the recommended model from Hugging Face will be used.
         :return: a pandas DataFrame with the summarizations for the strings. The summarizations will be added as a new column called 'predictions' to the original DataFrame.
         """
-        predictions = self._query_in_df(df, column, options=options, model=model, task='summarization')
+        predictions = self._query_in_df(df, column, parameters=parameters, options=options, model=model, task='summarization')
         df['predictions'] = [prediction['summary_text'] for prediction in predictions]
         return df
 
     def question_answering(self, question: Text, context: Text, model: Optional[Text] = None) -> Dict:
         """
         Answer a question using the provided context.
```

### Comparing `hugging_py_face-0.1.0/hugging_py_face.egg-info/PKG-INFO` & `hugging_py_face-0.1.1/hugging_py_face.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: hugging-py-face
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
-License: UNKNOWN
+License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
+        Copyright Â© 2023 Minura Punchihewa
+        
         Hugging-Py-Face is a powerful Python package that provides seamless integration with the Hugging Face Inference API, allowing you to easily perform inference on your machine learning models hosted on the Hugging Face Model Hub. 
         
         One of the key benefits of using the Hugging Face Inference API is that it provides a scalable and efficient way to perform inference on your models, by allowing you to easily deploy and serve your models in the cloud. Additionally, the Inference API provides a simple and standardized API that can be used across different programming languages, making it easy to integrate your models with other services and tools.
         
         With Hugging-Py-Face, you can take advantage of these benefits while also enjoying the simplicity and flexibility of using Python.
         
         It allows you to easily customize your API requests, adjust request parameters, handle authentication and access tokens, and interact with a wide range of machine learning models hosted on the Hugging Face Model Hub.
@@ -106,12 +108,16 @@
         ```
         
         Additionally, both of the above tasks can also be performed on a pandas DataFrame. For example:
         ```
         ap.audio_classification_in_df(df, 'audio')
         # where df is a pandas DataFrame and 'audio' is the column name containing the audio file paths or URLs
         ```
+        
+        # License
+        This code is licensed under the GNU GENERAL PUBLIC LICENSE. See LICENSE.txt for details.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hugging_py_face-0.1.0/setup.py` & `hugging_py_face-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,12 +24,15 @@
     description=about['__description__'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=(
         "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ),
-    include_package_data=True,
+    package_data={
+        'hugging_py_face': ['config/*.yml', 'config/*.yaml']
+    },
     python_requires=">=3.7"
 )
```

