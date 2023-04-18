# Comparing `tmp/elevenlabs-0.2.0.tar.gz` & `tmp/elevenlabs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.0.tar", last modified: Tue Apr 18 16:27:04 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.1.tar", last modified: Tue Apr 18 17:02:49 2023, max compression
```

## Comparing `elevenlabs-0.2.0.tar` & `elevenlabs-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.566462 elevenlabs-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 16:27:04.566462 elevenlabs-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.562462 elevenlabs-0.2.0/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.562462 elevenlabs-0.2.0/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.562462 elevenlabs-0.2.0/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:27:04.566462 elevenlabs-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.743512 elevenlabs-0.2.1/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.743512 elevenlabs-0.2.1/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/setup.py
```

### Comparing `elevenlabs-0.2.0/PKG-INFO` & `elevenlabs-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.0
+Version: 0.2.1
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.0/README.md` & `elevenlabs-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 <img src="LOGO.png"></img>
+[![PyPI - Python Version](https://img.shields.io/pypi/v/elevenlabs?style=flat&colorA=black&colorB=black)](https://pypi.org/project/elevenlabs/)
+[![Downloads](https://static.pepy.tech/personalized-badge/elevenlabs?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads)](https://pepy.tech/project/elevenlabs)
+[![Twitter](https://img.shields.io/twitter/url/https/twitter.com?style=social&label=elevenlabsio)](https://twitter.com/elevenlabsio)
+
 
 The official Python API for [Elevenlabs](https://elevenlabs.io/) text-to-speech software. Eleven brings the most compelling, rich and lifelike voices to creators and developers in just a few lines of code.
 
 
 ## ⚙️ Install
 
 ```bash
 pip install elevenlabs
 ```
-[![PyPI - Python Version](https://img.shields.io/pypi/v/elevenlabs?style=flat&colorA=black&colorB=black)](https://pypi.org/project/elevenlabs/)
-[![Downloads](https://static.pepy.tech/personalized-badge/elevenlabs?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads)](https://pepy.tech/project/elevenlabs)
 
 ## 🗣️ Usage
-
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/flavioschneider/49468d728a816c6538fd2f56b3b50b96/elevenlabs-python.ipynb)
 ```py
 from elevenlabs import generate, play
 
 text = """ Hi! I'm the world's most advanced text-to-speech system, made by elevenlabs. """
 audio = generate(text)
 play(audio)
 ```
 
-
 <details> <summary> Play </summary>
 
 <i> Don't forget to unmute the player! </i>
 
 [voice.webm](https://user-images.githubusercontent.com/12028621/232730309-e47bc907-78ec-4acf-a73a-0d77ba25fd6b.webm)
 
 </details>
```

### Comparing `elevenlabs-0.2.0/elevenlabs/__init__.py` & `elevenlabs-0.2.1/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.0/elevenlabs/api/base.py` & `elevenlabs-0.2.1/elevenlabs/api/base.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.0/elevenlabs/api/history.py` & `elevenlabs-0.2.1/elevenlabs/api/history.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.0/elevenlabs/api/tts.py` & `elevenlabs-0.2.1/elevenlabs/api/tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.0/elevenlabs/api/voice.py` & `elevenlabs-0.2.1/elevenlabs/api/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.0/elevenlabs/utils.py` & `elevenlabs-0.2.1/elevenlabs/utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.0/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.1/elevenlabs.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.0
+Version: 0.2.1
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.0/setup.py` & `elevenlabs-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.0",
+    version="0.2.1",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
     install_requires=[
-        "torch>=1.6",
+        "pydantic>=1.10",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
```

