# Comparing `tmp/basaran-0.15.3.tar.gz` & `tmp/basaran-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.15.3.tar", last modified: Fri Apr 14 20:11:30 2023, max compression
+gzip compressed data, was "basaran-0.16.0.tar", last modified: Tue Apr 18 16:20:26 2023, max compression
```

## Comparing `basaran-0.15.3.tar` & `basaran-0.16.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:11:30.221544 basaran-0.15.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-14 20:08:53.000000 basaran-0.15.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 20:08:53.000000 basaran-0.15.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 20:11:30.221544 basaran-0.15.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-14 20:08:53.000000 basaran-0.15.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:11:30.213544 basaran-0.15.3/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:11:30.217544 basaran-0.15.3/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:11:30.217544 basaran-0.15.3/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 20:08:53.000000 basaran-0.15.3/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:11:30.217544 basaran-0.15.3/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 20:11:30.000000 basaran-0.15.3/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 20:11:30.000000 basaran-0.15.3/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:11:30.000000 basaran-0.15.3/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 20:11:30.000000 basaran-0.15.3/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 20:11:30.000000 basaran-0.15.3/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:11:30.221544 basaran-0.15.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 20:08:53.000000 basaran-0.15.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:11:30.221544 basaran-0.15.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 20:08:53.000000 basaran-0.15.3/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-14 20:08:53.000000 basaran-0.15.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-14 20:08:53.000000 basaran-0.15.3/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:20:26.124930 basaran-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 16:17:55.000000 basaran-0.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 16:17:55.000000 basaran-0.16.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-18 16:20:26.124930 basaran-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-18 16:17:55.000000 basaran-0.16.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:20:26.120931 basaran-0.16.0/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:20:26.124930 basaran-0.16.0/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:20:26.124930 basaran-0.16.0/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-18 16:17:55.000000 basaran-0.16.0/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:20:26.124930 basaran-0.16.0/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-18 16:20:26.000000 basaran-0.16.0/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-18 16:20:26.000000 basaran-0.16.0/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:20:26.000000 basaran-0.16.0/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 16:20:26.000000 basaran-0.16.0/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 16:20:26.000000 basaran-0.16.0/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:20:26.124930 basaran-0.16.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-18 16:17:55.000000 basaran-0.16.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:20:26.124930 basaran-0.16.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-18 16:17:55.000000 basaran-0.16.0/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-18 16:17:55.000000 basaran-0.16.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-18 16:17:55.000000 basaran-0.16.0/tests/test_tokenizer.py
```

### Comparing `basaran-0.15.3/LICENSE` & `basaran-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/PKG-INFO` & `basaran-0.16.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.15.3
+Version: 0.16.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.15.3/README.md` & `basaran-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran/__init__.py` & `basaran-0.16.0/basaran/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # https://docs.pylonsproject.org/projects/waitress/en/stable/arguments.html
 SERVER_THREADS = int(os.getenv("SERVER_THREADS", "32"))
 SERVER_IDENTITY = os.getenv("SERVER_IDENTITY", "basaran")
 SERVER_CONNECTION_LIMIT = int(os.getenv("SERVER_CONNECTION_LIMIT", "512"))
 SERVER_CHANNEL_TIMEOUT = int(os.getenv("SERVER_CHANNEL_TIMEOUT", "300"))
 SERVER_MODEL_NAME = os.getenv("SERVER_MODEL_NAME", "") or MODEL
 SERVER_NO_PLAYGROUND = is_true(os.getenv("SERVER_NO_PLAYGROUND", ""))
+SERVER_CORS_ORIGINS = os.getenv("SERVER_CORS_ORIGINS", "*")
 
 # Completion-related arguments:
 COMPLETION_MAX_PROMPT = int(os.getenv("COMPLETION_MAX_PROMPT", "4096"))
 COMPLETION_MAX_TOKENS = int(os.getenv("COMPLETION_MAX_TOKENS", "4096"))
 COMPLETION_MAX_N = int(os.getenv("COMPLETION_MAX_N", "5"))
 COMPLETION_MAX_LOGPROBS = int(os.getenv("COMPLETION_MAX_LOGPROBS", "5"))
 COMPLETION_MAX_INTERVAL = int(os.getenv("COMPLETION_MAX_INTERVAL", "50"))
```

### Comparing `basaran-0.15.3/basaran/__main__.py` & `basaran-0.16.0/basaran/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import json
 import secrets
 import time
 
 import waitress
 from flask import Flask, Response, abort, jsonify, render_template, request
+from flask_cors import CORS
 
 from . import is_true
 from .choice import reduce_choice
 from .model import load_model
 
 # Configurations from environment variables.
 from . import MODEL
@@ -24,14 +25,15 @@
 from . import MODEL_HALF_PRECISION
 from . import SERVER_THREADS
 from . import SERVER_IDENTITY
 from . import SERVER_CONNECTION_LIMIT
 from . import SERVER_CHANNEL_TIMEOUT
 from . import SERVER_MODEL_NAME
 from . import SERVER_NO_PLAYGROUND
+from . import SERVER_CORS_ORIGINS
 from . import COMPLETION_MAX_PROMPT
 from . import COMPLETION_MAX_TOKENS
 from . import COMPLETION_MAX_N
 from . import COMPLETION_MAX_LOGPROBS
 from . import COMPLETION_MAX_INTERVAL
 
 # Load the language model to be served.
@@ -48,14 +50,17 @@
 # Create and configure application.
 app = Flask(__name__)
 app.json.ensure_ascii = False
 app.json.sort_keys = False
 app.json.compact = True
 app.url_map.strict_slashes = False
 
+# Configure cross-origin resource sharing (CORS).
+CORS(app, origins=SERVER_CORS_ORIGINS.split(","))
+
 
 def parse_options(schema):
     """Parse options specified in query parameters and request body."""
     options = {}
     payload = request.get_json(silent=True)
     for key, dtype in schema.items():
         # Allow casting from int to float.
```

### Comparing `basaran-0.15.3/basaran/choice.py` & `basaran-0.16.0/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran/model.py` & `basaran-0.16.0/basaran/model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran/static/playground.css` & `basaran-0.16.0/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran/static/playground.js` & `basaran-0.16.0/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran/static/presets.json` & `basaran-0.16.0/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran/templates/playground.html` & `basaran-0.16.0/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran/tokenizer.py` & `basaran-0.16.0/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/basaran.egg-info/PKG-INFO` & `basaran-0.16.0/basaran.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.15.3
+Version: 0.16.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.15.3/setup.py` & `basaran-0.16.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.15.3"
+VERSION = "0.16.0"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
     "Hugging Face Transformers-based text generation models.",
     author="Hyperonym",
     author_email="prompt@hyperonym.org",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.8.0",
-    install_requires=["flask", "jinja2", "torch", "transformers", "waitress"],
+    install_requires=[
+        "flask-cors",
+        "flask",
+        "jinja2",
+        "torch",
+        "transformers",
+        "waitress",
+    ],
     keywords=["api", "huggingface", "nlp", "openai", "transformer"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

### Comparing `basaran-0.15.3/tests/test_choice.py` & `basaran-0.16.0/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/tests/test_model.py` & `basaran-0.16.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.3/tests/test_tokenizer.py` & `basaran-0.16.0/tests/test_tokenizer.py`

 * *Files identical despite different names*

