# Comparing `tmp/mauth-client-1.4.0.tar.gz` & `tmp/mauth_client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mauth-client-1.4.0.tar", max compression
+gzip compressed data, was "mauth_client-1.5.0.tar", max compression
```

## Comparing `mauth-client-1.4.0.tar` & `mauth_client-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1062 2022-10-05 19:57:20.102645 mauth-client-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0     6084 2022-10-05 19:57:20.102645 mauth-client-1.4.0/README.md
--rw-r--r--   0        0        0      243 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/__init__.py
--rw-r--r--   0        0        0     9672 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/authenticator.py
--rw-r--r--   0        0        0      434 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/config.py
--rw-r--r--   0        0        0      479 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/consts.py
--rw-r--r--   0        0        0      633 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/exceptions.py
--rw-r--r--   0        0        0     2046 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/key_holder.py
--rw-r--r--   0        0        0       54 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/lambda_authenticator/__init__.py
--rw-r--r--   0        0        0      761 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/lambda_authenticator/lambda_authenticator.py
--rw-r--r--   0        0        0      679 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/lambda_helper.py
--rw-r--r--   0        0        0       76 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/middlewares/__init__.py
--rw-r--r--   0        0        0     4082 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/middlewares/asgi.py
--rw-r--r--   0        0        0     2114 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/middlewares/wsgi.py
--rw-r--r--   0        0        0       26 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/requests_mauth/__init__.py
--rw-r--r--   0        0        0     1304 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/requests_mauth/client.py
--rw-r--r--   0        0        0     2795 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/rsa_signer.py
--rw-r--r--   0        0        0     2324 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/rsa_verifier.py
--rw-r--r--   0        0        0     6196 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/signable.py
--rw-r--r--   0        0        0     1731 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/signed.py
--rw-r--r--   0        0        0     2849 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/signer.py
--rw-r--r--   0        0        0      790 2022-10-05 19:57:20.106646 mauth-client-1.4.0/mauth_client/utils.py
--rw-r--r--   0        0        0     1370 2022-10-05 19:57:20.106646 mauth-client-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7247 2022-10-05 19:58:11.808471 mauth-client-1.4.0/setup.py
--rw-r--r--   0        0        0     7343 2022-10-05 19:58:11.809125 mauth-client-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-18 17:30:43.630772 mauth_client-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     6084 2023-04-18 17:30:43.630772 mauth_client-1.5.0/README.md
+-rw-r--r--   0        0        0      243 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/__init__.py
+-rw-r--r--   0        0        0     9672 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/authenticator.py
+-rw-r--r--   0        0        0      434 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/config.py
+-rw-r--r--   0        0        0      479 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/consts.py
+-rw-r--r--   0        0        0      633 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/exceptions.py
+-rw-r--r--   0        0        0     2046 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/key_holder.py
+-rw-r--r--   0        0        0       54 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/lambda_authenticator/__init__.py
+-rw-r--r--   0        0        0      761 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/lambda_authenticator/lambda_authenticator.py
+-rw-r--r--   0        0        0      679 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/lambda_helper.py
+-rw-r--r--   0        0        0       76 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/middlewares/__init__.py
+-rw-r--r--   0        0        0     4082 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/middlewares/asgi.py
+-rw-r--r--   0        0        0     2114 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/middlewares/wsgi.py
+-rw-r--r--   0        0        0       26 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/requests_mauth/__init__.py
+-rw-r--r--   0        0        0     1304 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/requests_mauth/client.py
+-rw-r--r--   0        0        0     2795 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/rsa_signer.py
+-rw-r--r--   0        0        0     2324 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/rsa_verifier.py
+-rw-r--r--   0        0        0     6196 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/signable.py
+-rw-r--r--   0        0        0     1731 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/signed.py
+-rw-r--r--   0        0        0     2849 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/signer.py
+-rw-r--r--   0        0        0      820 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/utils.py
+-rw-r--r--   0        0        0     1421 2023-04-18 17:30:43.634772 mauth_client-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 mauth_client-1.5.0/PKG-INFO
```

### Comparing `mauth-client-1.4.0/LICENSE.txt` & `mauth_client-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/README.md` & `mauth_client-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/authenticator.py` & `mauth_client-1.5.0/mauth_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/exceptions.py` & `mauth_client-1.5.0/mauth_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/key_holder.py` & `mauth_client-1.5.0/mauth_client/key_holder.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/lambda_authenticator/lambda_authenticator.py` & `mauth_client-1.5.0/mauth_client/lambda_authenticator/lambda_authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/lambda_helper.py` & `mauth_client-1.5.0/mauth_client/lambda_helper.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/middlewares/asgi.py` & `mauth_client-1.5.0/mauth_client/middlewares/asgi.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/middlewares/wsgi.py` & `mauth_client-1.5.0/mauth_client/middlewares/wsgi.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/requests_mauth/client.py` & `mauth_client-1.5.0/mauth_client/requests_mauth/client.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/rsa_signer.py` & `mauth_client-1.5.0/mauth_client/rsa_signer.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/rsa_verifier.py` & `mauth_client-1.5.0/mauth_client/rsa_verifier.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/signable.py` & `mauth_client-1.5.0/mauth_client/signable.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/signed.py` & `mauth_client-1.5.0/mauth_client/signed.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/signer.py` & `mauth_client-1.5.0/mauth_client/signer.py`

 * *Files identical despite different names*

### Comparing `mauth-client-1.4.0/mauth_client/utils.py` & `mauth_client-1.5.0/mauth_client/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import base64
-import cchardet
+import charset_normalizer
 from hashlib import sha512
 
 
 def make_bytes(val):
     """
     :param str val: The supplied value (string-like)
     """
@@ -21,14 +21,14 @@
 
 def base64_encode(signature):
     return base64.b64encode(signature).decode("US-ASCII").replace("\n", "")
 
 
 def decode(byte_string: bytes) -> str:
     """
-    Attempt to decode a byte string with utf and fallback to cchardet.
+    Attempt to decode a byte string with utf and fallback to charset_normalizer.
     """
     try:
         return byte_string.decode("utf-8")
     except UnicodeDecodeError:
-        encoding = cchardet.detect(byte_string)["encoding"]
+        encoding = charset_normalizer.detect(byte_string)["encoding"]
         return byte_string.decode(encoding)
```

### Comparing `mauth-client-1.4.0/pyproject.toml` & `mauth_client-1.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mauth-client"
-version = "1.4.0"
+version = "1.5.0"
 description = "MAuth Client for Python"
 repository = "https://github.com/mdsol/mauth-client-python"
 authors = ["Medidata Solutions <support@mdsol.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -13,39 +13,40 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.13"
+python = "^3.7"
 requests = "^2.23"
-cachetools = "^4.1"
+cachetools = "^5.3"
 rsa = "^4.0"
-importlib-metadata = {version = "^3.6", python = "<3.8"}
+importlib-metadata = {version = ">=3.6", python = "<3.8"}
 asgiref = "^3.5.2"
-cchardet = "^2.1.7"
+charset-normalizer = "^3.1.0"
 
 [tool.poetry.dev-dependencies]
 boto3 = "^1.24"
 flask = "^2"
 python-dateutil = "^2.8"
 requests-mock = "^1.7"
-pytest = "^6"
-pytest-cov = "^2.8"
+pytest = "^7"
+pytest-cov = "^4"
 pytest-freezegun = "^0.4"
 pytest-randomly = "^3.11"
-pytest-subtests = "^0.3"
+pytest-subtests = "^0.10"
 flake8 = "^3.7"
-tox = "^3.22.0"
+tox = "^3.28"
 fastapi = "^0.80.0"
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `mauth-client-1.4.0/setup.py` & `mauth_client-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,218 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mauth-client
+Version: 1.5.0
+Summary: MAuth Client for Python
+Home-page: https://github.com/mdsol/mauth-client-python
+License: MIT
+Author: Medidata Solutions
+Author-email: support@mdsol.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: asgiref (>=3.5.2,<4.0.0)
+Requires-Dist: cachetools (>=5.3,<6.0)
+Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
+Requires-Dist: importlib-metadata (>=3.6) ; python_version < "3.8"
+Requires-Dist: requests (>=2.23,<3.0)
+Requires-Dist: rsa (>=4.0,<5.0)
+Project-URL: Repository, https://github.com/mdsol/mauth-client-python
+Description-Content-Type: text/markdown
+
+# MAuth Client Python
+[![Build
+Status](https://travis-ci.com/mdsol/mauth-client-python.svg?token=YCqgqZjJBpwz6GCprYaV&branch=develop)](https://travis-ci.com/mdsol/mauth-client-python)
+
+MAuth Client Python is an authentication library to manage the information needed to both sign and authenticate requests and responses for Medidata's MAuth authentication system.
+
+
+## Pre-requisites
+
+To use MAuth Authenticator you will need:
+
+* An MAuth app ID
+* An MAuth private key (with the public key registered with Medidata's MAuth server)
+
+
+## Installation
+
+To resolve packages using pip, add the following to ~/.pip/pip.conf:
+```
+[global]
+index-url = https://<username>:<password>@mdsol.jfrog.io/mdsol/api/pypi/pypi-packages/simple/
+```
+
+Install using pip:
+```
+$ pip install mauth-client
+```
+
+Or directly from GitHub:
+```
+$ pip install git+https://github.com/mdsol/mauth-client-python.git
+```
+
+This will also install the dependencies.
+
+To resolve using a requirements file, the index URL can be specified in the first line of the file:
+```
+--index-url https://<username>:<password>@mdsol.jfrog.io/mdsol/api/pypi/pypi-packages/simple/
+mauth-client==<latest version>
+```
+
+## Usage
+
+### Signing Outgoing Requests
+
+```python
+import requests
+from mauth_client.requests_mauth import MAuth
+
+# MAuth configuration
+APP_UUID = "<MAUTH_APP_UUID>"
+private_key = open("private.key", "r").read()
+mauth = MAuth(APP_UUID, private_key)
+
+# Call an MAuth protected resource, in this case an iMedidata API
+# listing the studies for a particular user
+user_uuid = "10ac3b0e-9fe2-11df-a531-12313900d531"
+url = "https://innovate.imedidata.com/api/v2/users/{}/studies.json".format(user_uuid)
+
+# Make the requests call, passing the auth client
+result = requests.get(url, auth=mauth)
+
+# Print results
+if result.status_code == 200:
+    print([r["uuid"] for r in result.json()["studies"]])
+print(result.text)
+```
+
+The `mauth_sign_versions` option can be set as an environment variable to specify protocol versions to sign outgoing requests:
+
+| Key                   | Value                                                                                |
+| --------------------- | ------------------------------------------------------------------------------------ |
+| `MAUTH_SIGN_VERSIONS` | **(optional)** Comma-separated protocol versions to sign requests. Defaults to `v1`. |
+
+This option can also be passed to the constructor:
+
+```python
+mauth_sign_versions = "v1,v2"
+mauth = MAuth(APP_UUID, private_key, mauth_sign_versions)
+```
+
+
+### Authenticating Incoming Requests
+
+MAuth Client Python supports AWS Lambda functions and Flask applications to authenticate MAuth signed requests.
+
+The following variables are **required** to be configured in the environment variables:
+
+| Key            | Value                                                         |
+| -------------- | ------------------------------------------------------------- |
+| `APP_UUID`     | APP_UUID for the AWS Lambda function                          |
+| `PRIVATE_KEY`  | Encrypted private key for the APP_UUID                        |
+| `MAUTH_URL`    | MAuth service URL (e.g. https://mauth-innovate.imedidata.com) |
+
+
+The following variables can optionally be set in the environment variables:
+
+| Key                    | Value                                                                                     |
+| ---------------------- | ----------------------------------------------------------------------------------------- |
+| `MAUTH_API_VERSION`    | **(optional)** MAuth API version. Only `v1` exists as of this writing. Defaults to `v1`.  |
+| `MAUTH_MODE`           | **(optional)** Method to authenticate requests. `local` or `remote`. Defaults to `local`. |
+| `V2_ONLY_AUTHENTICATE` | **(optional)** Authenticate requests with only V2. Defaults to `False`.                   |
+
+
+#### AWS Lambda functions
+
+```python
+from mauth_client.lambda_authenticator import LambdaAuthenticator
+
+authenticator = LambdaAuthenticator(method, url, headers, body)
+authentic, status_code, message = authenticator.is_authentic()
+app_uuid = authenticator.get_app_uuid()
+```
+
+#### WSGI Applications
+
+To apply to a WSGI application you should use the `MAuthWSGIMiddleware`. You
+can make certain paths exempt from authentication by passing the `exempt`
+option with a set of paths to exempt.
+
+Here is an example for Flask. Note that requesting app's UUID and the
+protocol version will be added to the request environment for successfully
+authenticated requests.
+
+```python
+from flask import Flask, request, jsonify
+from mauth_client.consts import ENV_APP_UUID, ENV_PROTOCOL_VERSION
+from mauth_client.middlewares import MAuthWSGIMiddleware
+
+app = Flask("MyApp")
+app.wsgi_app = MAuthWSGIMiddleware(app.wsgi_app, exempt={"/app_status"})
+
+@app.get("/")
+def root():
+    return jsonify({
+        "msg": "authenticated",
+        "app_uuid": request.environ[ENV_APP_UUID],
+        "protocol_version": request.environ[ENV_PROTOCOL_VERSION],
+    })
+
+@app.get("/app_status")
+    return "this route is exempt from authentication"
+```
+
+#### ASGI Applications
+
+To apply to an ASGI application you should use the `MAuthASGIMiddleware`. You
+can make certain paths exempt from authentication by passing the `exempt`
+option with a set of paths to exempt.
+
+Here is an example for FastAPI. Note that requesting app's UUID and the
+protocol version will be added to the ASGI `scope` for successfully
+authenticated requests.
+
+```python
+from fastapi import FastAPI, Request
+from mauth_client.consts import ENV_APP_UUID, ENV_PROTOCOL_VERSION
+from mauth_client.middlewares import MAuthASGIMiddleware
+
+app = FastAPI()
+app.add_middleware(MAuthASGIMiddleware, exempt={"/app_status"})
+
+@app.get("/")
+async def root(request: Request):
+    return {
+        "msg": "authenticated",
+        "app_uuid": request.scope[ENV_APP_UUID],
+        "protocol_version": request.scope[ENV_PROTOCOL_VERSION],
+    }
+
+@app.get("/app_status")
+async def app_status():
+    return {
+        "msg": "this route is exempt from authentication",
+    }
+```
 
-packages = \
-['mauth_client',
- 'mauth_client.lambda_authenticator',
- 'mauth_client.middlewares',
- 'mauth_client.requests_mauth']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['asgiref>=3.5.2,<4.0.0',
- 'cachetools>=4.1,<5.0',
- 'cchardet>=2.1.7,<3.0.0',
- 'requests>=2.23,<3.0',
- 'rsa>=4.0,<5.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=3.6,<4.0']}
-
-setup_kwargs = {
-    'name': 'mauth-client',
-    'version': '1.4.0',
-    'description': 'MAuth Client for Python',
-    'long_description': '# MAuth Client Python\n[![Build\nStatus](https://travis-ci.com/mdsol/mauth-client-python.svg?token=YCqgqZjJBpwz6GCprYaV&branch=develop)](https://travis-ci.com/mdsol/mauth-client-python)\n\nMAuth Client Python is an authentication library to manage the information needed to both sign and authenticate requests and responses for Medidata\'s MAuth authentication system.\n\n\n## Pre-requisites\n\nTo use MAuth Authenticator you will need:\n\n* An MAuth app ID\n* An MAuth private key (with the public key registered with Medidata\'s MAuth server)\n\n\n## Installation\n\nTo resolve packages using pip, add the following to ~/.pip/pip.conf:\n```\n[global]\nindex-url = https://<username>:<password>@mdsol.jfrog.io/mdsol/api/pypi/pypi-packages/simple/\n```\n\nInstall using pip:\n```\n$ pip install mauth-client\n```\n\nOr directly from GitHub:\n```\n$ pip install git+https://github.com/mdsol/mauth-client-python.git\n```\n\nThis will also install the dependencies.\n\nTo resolve using a requirements file, the index URL can be specified in the first line of the file:\n```\n--index-url https://<username>:<password>@mdsol.jfrog.io/mdsol/api/pypi/pypi-packages/simple/\nmauth-client==<latest version>\n```\n\n## Usage\n\n### Signing Outgoing Requests\n\n```python\nimport requests\nfrom mauth_client.requests_mauth import MAuth\n\n# MAuth configuration\nAPP_UUID = "<MAUTH_APP_UUID>"\nprivate_key = open("private.key", "r").read()\nmauth = MAuth(APP_UUID, private_key)\n\n# Call an MAuth protected resource, in this case an iMedidata API\n# listing the studies for a particular user\nuser_uuid = "10ac3b0e-9fe2-11df-a531-12313900d531"\nurl = "https://innovate.imedidata.com/api/v2/users/{}/studies.json".format(user_uuid)\n\n# Make the requests call, passing the auth client\nresult = requests.get(url, auth=mauth)\n\n# Print results\nif result.status_code == 200:\n    print([r["uuid"] for r in result.json()["studies"]])\nprint(result.text)\n```\n\nThe `mauth_sign_versions` option can be set as an environment variable to specify protocol versions to sign outgoing requests:\n\n| Key                   | Value                                                                                |\n| --------------------- | ------------------------------------------------------------------------------------ |\n| `MAUTH_SIGN_VERSIONS` | **(optional)** Comma-separated protocol versions to sign requests. Defaults to `v1`. |\n\nThis option can also be passed to the constructor:\n\n```python\nmauth_sign_versions = "v1,v2"\nmauth = MAuth(APP_UUID, private_key, mauth_sign_versions)\n```\n\n\n### Authenticating Incoming Requests\n\nMAuth Client Python supports AWS Lambda functions and Flask applications to authenticate MAuth signed requests.\n\nThe following variables are **required** to be configured in the environment variables:\n\n| Key            | Value                                                         |\n| -------------- | ------------------------------------------------------------- |\n| `APP_UUID`     | APP_UUID for the AWS Lambda function                          |\n| `PRIVATE_KEY`  | Encrypted private key for the APP_UUID                        |\n| `MAUTH_URL`    | MAuth service URL (e.g. https://mauth-innovate.imedidata.com) |\n\n\nThe following variables can optionally be set in the environment variables:\n\n| Key                    | Value                                                                                     |\n| ---------------------- | ----------------------------------------------------------------------------------------- |\n| `MAUTH_API_VERSION`    | **(optional)** MAuth API version. Only `v1` exists as of this writing. Defaults to `v1`.  |\n| `MAUTH_MODE`           | **(optional)** Method to authenticate requests. `local` or `remote`. Defaults to `local`. |\n| `V2_ONLY_AUTHENTICATE` | **(optional)** Authenticate requests with only V2. Defaults to `False`.                   |\n\n\n#### AWS Lambda functions\n\n```python\nfrom mauth_client.lambda_authenticator import LambdaAuthenticator\n\nauthenticator = LambdaAuthenticator(method, url, headers, body)\nauthentic, status_code, message = authenticator.is_authentic()\napp_uuid = authenticator.get_app_uuid()\n```\n\n#### WSGI Applications\n\nTo apply to a WSGI application you should use the `MAuthWSGIMiddleware`. You\ncan make certain paths exempt from authentication by passing the `exempt`\noption with a set of paths to exempt.\n\nHere is an example for Flask. Note that requesting app\'s UUID and the\nprotocol version will be added to the request environment for successfully\nauthenticated requests.\n\n```python\nfrom flask import Flask, request, jsonify\nfrom mauth_client.consts import ENV_APP_UUID, ENV_PROTOCOL_VERSION\nfrom mauth_client.middlewares import MAuthWSGIMiddleware\n\napp = Flask("MyApp")\napp.wsgi_app = MAuthWSGIMiddleware(app.wsgi_app, exempt={"/app_status"})\n\n@app.get("/")\ndef root():\n    return jsonify({\n        "msg": "authenticated",\n        "app_uuid": request.environ[ENV_APP_UUID],\n        "protocol_version": request.environ[ENV_PROTOCOL_VERSION],\n    })\n\n@app.get("/app_status")\n    return "this route is exempt from authentication"\n```\n\n#### ASGI Applications\n\nTo apply to an ASGI application you should use the `MAuthASGIMiddleware`. You\ncan make certain paths exempt from authentication by passing the `exempt`\noption with a set of paths to exempt.\n\nHere is an example for FastAPI. Note that requesting app\'s UUID and the\nprotocol version will be added to the ASGI `scope` for successfully\nauthenticated requests.\n\n```python\nfrom fastapi import FastAPI, Request\nfrom mauth_client.consts import ENV_APP_UUID, ENV_PROTOCOL_VERSION\nfrom mauth_client.middlewares import MAuthASGIMiddleware\n\napp = FastAPI()\napp.add_middleware(MAuthASGIMiddleware, exempt={"/app_status"})\n\n@app.get("/")\nasync def root(request: Request):\n    return {\n        "msg": "authenticated",\n        "app_uuid": request.scope[ENV_APP_UUID],\n        "protocol_version": request.scope[ENV_PROTOCOL_VERSION],\n    }\n\n@app.get("/app_status")\nasync def app_status():\n    return {\n        "msg": "this route is exempt from authentication",\n    }\n```\n\n## Contributing\n\nSee [CONTRIBUTING](CONTRIBUTING.md)\n',
-    'author': 'Medidata Solutions',
-    'author_email': 'support@mdsol.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mdsol/mauth-client-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.13,<4.0.0',
-}
+## Contributing
 
+See [CONTRIBUTING](CONTRIBUTING.md)
 
-setup(**setup_kwargs)
```

