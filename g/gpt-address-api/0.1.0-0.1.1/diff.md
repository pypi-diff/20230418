# Comparing `tmp/gpt_address_api-0.1.0.tar.gz` & `tmp/gpt_address_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_address_api-0.1.0.tar", last modified: Sat Apr 15 08:39:24 2023, max compression
+gzip compressed data, was "gpt_address_api-0.1.1.tar", last modified: Tue Apr 18 20:45:20 2023, max compression
```

## Comparing `gpt_address_api-0.1.0.tar` & `gpt_address_api-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:24.382592 gpt_address_api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-15 08:39:16.000000 gpt_address_api-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-15 08:39:24.382592 gpt_address_api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-15 08:39:16.000000 gpt_address_api-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:39:24.382592 gpt_address_api-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-15 08:39:16.000000 gpt_address_api-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:24.378592 gpt_address_api-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:24.378592 gpt_address_api-0.1.0/src/gpt_address_api/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 08:39:16.000000 gpt_address_api-0.1.0/src/gpt_address_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-15 08:39:16.000000 gpt_address_api-0.1.0/src/gpt_address_api/gpt_address_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:24.382592 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-15 08:39:24.000000 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-15 08:39:24.000000 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:39:24.000000 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-15 08:39:24.000000 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:39:24.000000 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 08:39:24.000000 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 08:39:24.000000 gpt_address_api-0.1.0/src/gpt_address_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:20.357427 gpt_address_api-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-18 20:45:10.000000 gpt_address_api-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-18 20:45:20.357427 gpt_address_api-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-18 20:45:10.000000 gpt_address_api-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:45:20.357427 gpt_address_api-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-18 20:45:10.000000 gpt_address_api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:20.357427 gpt_address_api-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:20.357427 gpt_address_api-0.1.1/src/gpt_address_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 20:45:10.000000 gpt_address_api-0.1.1/src/gpt_address_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-18 20:45:10.000000 gpt_address_api-0.1.1/src/gpt_address_api/gpt_address_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:20.357427 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-18 20:45:20.000000 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-18 20:45:20.000000 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:45:20.000000 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 20:45:20.000000 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:45:20.000000 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 20:45:20.000000 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 20:45:20.000000 gpt_address_api-0.1.1/src/gpt_address_api.egg-info/top_level.txt
```

### Comparing `gpt_address_api-0.1.0/LICENSE` & `gpt_address_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_address_api-0.1.0/PKG-INFO` & `gpt_address_api-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_address_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: Decentralized GPT API for everyone !
 Home-page: https://github.com/Naruno/GPT-Address-API
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # GPT Address API (GPTAAPI) for Naruno
         GPTAAPI is a decentralized API for OpenAI GPT. It allows you to use GPT without exposing your API key to the public. It is based on the [Naruno](https://naruno.org/) blockchain and uses the [Naruno API](https://naruno.org/api/) to communicate with the blockchain. GPTAAPI is written in Python and uses the [OpenAI GPT-3 API](https://openai.com/blog/openai-api/) to communicate with GPT.
@@ -48,15 +48,15 @@
         my_gptaapi_server.add_user("client_address")
         
         my_gptaapi_server.run()
         ```
         
         also you can use in command line:
         ```console	
-        gptaapi --password MyNarunoPass --encrypt_key "mystrongencrypt_key" --trusted_users ["client_address"] --api_key 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 run
+        gptaapi --password MyNarunoPass --encrypt_key "mystrongencrypt_key" --trusted_users ["client_address"] --api_key my_open_ai_api_key run
         ```
         
         ### Client
         To use gptaapi, you can call the gptaapi.ask function with your blockchain address, message and encryption key as the parameter:
         
         ```python
         from gpt_address_api import gptaapi
```

### Comparing `gpt_address_api-0.1.0/README.md` & `gpt_address_api-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 my_gptaapi_server.add_user("client_address")
 
 my_gptaapi_server.run()
 ```
 
 also you can use in command line:
 ```console	
-gptaapi --password MyNarunoPass --encrypt_key "mystrongencrypt_key" --trusted_users ["client_address"] --api_key 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 run
+gptaapi --password MyNarunoPass --encrypt_key "mystrongencrypt_key" --trusted_users ["client_address"] --api_key my_open_ai_api_key run
 ```
 
 ### Client
 To use gptaapi, you can call the gptaapi.ask function with your blockchain address, message and encryption key as the parameter:
 
 ```python
 from gpt_address_api import gptaapi
```

### Comparing `gpt_address_api-0.1.0/setup.py` & `gpt_address_api-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='gpt_address_api',
-version='0.1.0',
+version='0.1.1',
 description="""Decentralized GPT API for everyone !""",
 long_description_content_type="text/markdown",
 include_package_data=True,
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 url='https://github.com/Naruno/GPT-Address-API',
 author="Naruno Developers",
 author_email='onur.atakan.ulusoy@naruno.org',
```

### Comparing `gpt_address_api-0.1.0/src/gpt_address_api/gpt_address_api.py` & `gpt_address_api-0.1.1/src/gpt_address_api/gpt_address_api.py`

 * *Files identical despite different names*

### Comparing `gpt_address_api-0.1.0/src/gpt_address_api.egg-info/PKG-INFO` & `gpt_address_api-0.1.1/src/gpt_address_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-address-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: Decentralized GPT API for everyone !
 Home-page: https://github.com/Naruno/GPT-Address-API
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # GPT Address API (GPTAAPI) for Naruno
         GPTAAPI is a decentralized API for OpenAI GPT. It allows you to use GPT without exposing your API key to the public. It is based on the [Naruno](https://naruno.org/) blockchain and uses the [Naruno API](https://naruno.org/api/) to communicate with the blockchain. GPTAAPI is written in Python and uses the [OpenAI GPT-3 API](https://openai.com/blog/openai-api/) to communicate with GPT.
@@ -48,15 +48,15 @@
         my_gptaapi_server.add_user("client_address")
         
         my_gptaapi_server.run()
         ```
         
         also you can use in command line:
         ```console	
-        gptaapi --password MyNarunoPass --encrypt_key "mystrongencrypt_key" --trusted_users ["client_address"] --api_key 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 run
+        gptaapi --password MyNarunoPass --encrypt_key "mystrongencrypt_key" --trusted_users ["client_address"] --api_key my_open_ai_api_key run
         ```
         
         ### Client
         To use gptaapi, you can call the gptaapi.ask function with your blockchain address, message and encryption key as the parameter:
         
         ```python
         from gpt_address_api import gptaapi
```

