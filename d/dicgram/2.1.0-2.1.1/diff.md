# Comparing `tmp/dicgram-2.1.0.tar.gz` & `tmp/dicgram-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dicgram-2.1.0.tar", last modified: Wed Mar 29 01:28:32 2023, max compression
+gzip compressed data, was "dist/dicgram-2.1.1.tar", last modified: Tue Apr 18 18:30:26 2023, max compression
```

## Comparing `dicgram-2.1.0.tar` & `dicgram-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:28:32.000000 dicgram-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-29 01:28:24.000000 dicgram-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-03-29 01:28:32.000000 dicgram-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-03-29 01:28:24.000000 dicgram-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:28:32.000000 dicgram-2.1.0/dicgram/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-29 01:28:24.000000 dicgram-2.1.0/dicgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-03-29 01:28:24.000000 dicgram-2.1.0/dicgram/cliente.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-03-29 01:28:24.000000 dicgram-2.1.0/dicgram/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-29 01:28:24.000000 dicgram-2.1.0/dicgram/mensagem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-29 01:28:24.000000 dicgram-2.1.0/dicgram/metodos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:28:32.000000 dicgram-2.1.0/dicgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-03-29 01:28:32.000000 dicgram-2.1.0/dicgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-29 01:28:32.000000 dicgram-2.1.0/dicgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 01:28:32.000000 dicgram-2.1.0/dicgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-29 01:28:32.000000 dicgram-2.1.0/dicgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-29 01:28:32.000000 dicgram-2.1.0/dicgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 01:28:32.000000 dicgram-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-29 01:28:24.000000 dicgram-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:28:32.000000 dicgram-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-29 01:28:24.000000 dicgram-2.1.0/tests/testes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:26.000000 dicgram-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 18:30:15.000000 dicgram-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-18 18:30:26.000000 dicgram-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-18 18:30:15.000000 dicgram-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:26.000000 dicgram-2.1.1/dicgram/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 18:30:15.000000 dicgram-2.1.1/dicgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-04-18 18:30:15.000000 dicgram-2.1.1/dicgram/cliente.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-18 18:30:15.000000 dicgram-2.1.1/dicgram/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-18 18:30:15.000000 dicgram-2.1.1/dicgram/mensagem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-18 18:30:15.000000 dicgram-2.1.1/dicgram/metodos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:26.000000 dicgram-2.1.1/dicgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-18 18:30:26.000000 dicgram-2.1.1/dicgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-18 18:30:26.000000 dicgram-2.1.1/dicgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:30:26.000000 dicgram-2.1.1/dicgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 18:30:26.000000 dicgram-2.1.1/dicgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 18:30:26.000000 dicgram-2.1.1/dicgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:30:26.000000 dicgram-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-18 18:30:15.000000 dicgram-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:26.000000 dicgram-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-18 18:30:15.000000 dicgram-2.1.1/tests/testes.py
```

### Comparing `dicgram-2.1.0/LICENSE` & `dicgram-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicgram-2.1.0/PKG-INFO` & `dicgram-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicgram
-Version: 2.1.0
+Version: 2.1.1
 Summary: Framework para criar bots do Telegram
 Home-page: https://github.com/marcellobatiista/dicgram
 Author: Marcelo Batista
 Author-email: batista.marcelo34@gmail.com
 License: MIT
 Keywords: telegram chat messenger api client library python
 Requires-Python: >=3.7
```

### Comparing `dicgram-2.1.0/README.md` & `dicgram-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dicgram-2.1.0/dicgram/cliente.py` & `dicgram-2.1.1/dicgram/cliente.py`

 * *Files identical despite different names*

### Comparing `dicgram-2.1.0/dicgram/decorators.py` & `dicgram-2.1.1/dicgram/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,24 +52,34 @@
 
         :param args: argumentos da função decorada
         :param kwargs: argumentos nomeados da função decorada
         :return: None
         """
 
         self = args[0]
+
+        # Verifica a url do webhook tem o endpoint
+        endpoints = '/'.join(self._webhook_url.split('/')[3:])
+        if not endpoints:
+            self._webhook_url = f'{self._webhook_url}/webhook'
+            endpoints = '/webhook'
+        else:
+            endpoints = f'/{endpoints}'
+
+        # Define o webhook
         self._set_webhook(self._webhook_url)
 
         import logging
         from flask import Flask, request, jsonify
 
         app = Flask(__name__)
         log = logging.getLogger('werkzeug')
         log.setLevel(logging.ERROR)
 
-        @app.route('/' + self._webhook_url.split('/')[-1], methods=['POST'])
+        @app.route('/' + endpoints, methods=['POST'])
         def webhook():
             """
             Webhook
 
             :return: Json com status
             """
```

### Comparing `dicgram-2.1.0/dicgram/mensagem.py` & `dicgram-2.1.1/dicgram/mensagem.py`

 * *Files identical despite different names*

### Comparing `dicgram-2.1.0/dicgram/metodos.py` & `dicgram-2.1.1/dicgram/metodos.py`

 * *Files identical despite different names*

### Comparing `dicgram-2.1.0/dicgram.egg-info/PKG-INFO` & `dicgram-2.1.1/dicgram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicgram
-Version: 2.1.0
+Version: 2.1.1
 Summary: Framework para criar bots do Telegram
 Home-page: https://github.com/marcellobatiista/dicgram
 Author: Marcelo Batista
 Author-email: batista.marcelo34@gmail.com
 License: MIT
 Keywords: telegram chat messenger api client library python
 Requires-Python: >=3.7
```

### Comparing `dicgram-2.1.0/setup.py` & `dicgram-2.1.1/setup.py`

 * *Files identical despite different names*

