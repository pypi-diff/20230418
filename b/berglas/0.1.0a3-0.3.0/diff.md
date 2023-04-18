# Comparing `tmp/berglas-0.1.0a3.tar.gz` & `tmp/berglas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/berglas-0.1.0a3.tar", last modified: Tue Aug  6 21:17:46 2019, max compression
+gzip compressed data, was "berglas-0.3.0.tar", last modified: Tue Apr 18 21:02:58 2023, max compression
```

## Comparing `berglas-0.1.0a3.tar` & `berglas-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 amaru      (501) admin       (80)        0 2019-08-06 21:17:46.000000 berglas-0.1.0a3/
--rw-r--r--   0 amaru      (501) admin       (80)     4995 2019-08-06 21:17:46.000000 berglas-0.1.0a3/PKG-INFO
--rw-r--r--   0 amaru      (501) admin       (80)     3184 2019-07-26 22:14:33.000000 berglas-0.1.0a3/README.rst
-drwxr-xr-x   0 amaru      (501) admin       (80)        0 2019-08-06 21:17:46.000000 berglas-0.1.0a3/berglas/
--rw-r--r--   0 amaru      (501) admin       (80)       89 2019-08-06 21:17:33.000000 berglas-0.1.0a3/berglas/__init__.py
--rw-r--r--   0 amaru      (501) admin       (80)     1255 2019-07-26 22:14:33.000000 berglas-0.1.0a3/berglas/auto.py
--rw-r--r--   0 amaru      (501) admin       (80)      271 2019-07-26 18:27:09.000000 berglas-0.1.0a3/berglas/constants.py
--rw-r--r--   0 amaru      (501) admin       (80)       41 2019-07-26 01:34:27.000000 berglas-0.1.0a3/berglas/exceptions.py
--rw-r--r--   0 amaru      (501) admin       (80)     4444 2019-08-06 21:14:07.000000 berglas-0.1.0a3/berglas/resolver.py
--rw-r--r--   0 amaru      (501) admin       (80)     4616 2019-07-26 23:04:36.000000 berglas-0.1.0a3/berglas/runtime.py
-drwxr-xr-x   0 amaru      (501) admin       (80)        0 2019-08-06 21:17:46.000000 berglas-0.1.0a3/berglas.egg-info/
--rw-r--r--   0 amaru      (501) admin       (80)     4995 2019-08-06 21:17:46.000000 berglas-0.1.0a3/berglas.egg-info/PKG-INFO
--rw-r--r--   0 amaru      (501) admin       (80)      301 2019-08-06 21:17:46.000000 berglas-0.1.0a3/berglas.egg-info/SOURCES.txt
--rw-r--r--   0 amaru      (501) admin       (80)        1 2019-08-06 21:17:46.000000 berglas-0.1.0a3/berglas.egg-info/dependency_links.txt
--rw-r--r--   0 amaru      (501) admin       (80)      181 2019-08-06 21:17:46.000000 berglas-0.1.0a3/berglas.egg-info/requires.txt
--rw-r--r--   0 amaru      (501) admin       (80)        8 2019-08-06 21:17:46.000000 berglas-0.1.0a3/berglas.egg-info/top_level.txt
--rw-r--r--   0 amaru      (501) admin       (80)      297 2019-08-06 21:17:46.000000 berglas-0.1.0a3/setup.cfg
--rw-r--r--   0 amaru      (501) admin       (80)     2568 2019-07-26 22:14:33.000000 berglas-0.1.0a3/setup.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-18 21:02:58.533967 berglas-0.3.0/
+-rw-r--r--   0 maru       (501) staff       (20)    11345 2023-04-11 20:34:42.000000 berglas-0.3.0/LICENSE
+-rw-r--r--   0 maru       (501) staff       (20)     4406 2023-04-18 21:02:58.534024 berglas-0.3.0/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)     3476 2023-04-18 20:55:34.000000 berglas-0.3.0/README.rst
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-18 21:02:58.533240 berglas-0.3.0/berglas/
+-rw-r--r--   0 maru       (501) staff       (20)       87 2023-04-18 21:02:57.000000 berglas-0.3.0/berglas/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     1255 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/auto.py
+-rw-r--r--   0 maru       (501) staff       (20)      271 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/constants.py
+-rw-r--r--   0 maru       (501) staff       (20)       41 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)     4610 2023-04-18 20:43:05.000000 berglas-0.3.0/berglas/resolver.py
+-rw-r--r--   0 maru       (501) staff       (20)     4616 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/runtime.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-18 21:02:58.533868 berglas-0.3.0/berglas.egg-info/
+-rw-r--r--   0 maru       (501) staff       (20)     4406 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)      324 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/SOURCES.txt
+-rw-r--r--   0 maru       (501) staff       (20)        1 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/dependency_links.txt
+-rw-r--r--   0 maru       (501) staff       (20)      190 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/requires.txt
+-rw-r--r--   0 maru       (501) staff       (20)        8 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/top_level.txt
+-rw-r--r--   0 maru       (501) staff       (20)      211 2023-04-11 20:34:42.000000 berglas-0.3.0/pyproject.toml
+-rw-r--r--   0 maru       (501) staff       (20)      256 2023-04-18 21:02:58.534263 berglas-0.3.0/setup.cfg
+-rw-r--r--   0 maru       (501) staff       (20)     2626 2023-04-18 20:43:05.000000 berglas-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `berglas-0.1.0a3/PKG-INFO` & `berglas-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,150 @@
 Metadata-Version: 2.1
 Name: berglas
-Version: 0.1.0a3
+Version: 0.3.0
 Summary: Berglas Python Library
 Home-page: https://github.com/maroux/berglas-python
 Author: Aniruddha Maru
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
-Description: Berglas Library for Python
-        ==========================
-        
-        .. image:: https://travis-ci.org/maroux/berglas-python.svg?branch=master
-            :target: https://travis-ci.org/maroux/berglas-python
-        
-        .. image:: https://coveralls.io/repos/github/maroux/berglas-python/badge.svg?branch=master
-            :target: https://coveralls.io/github/maroux/berglas-python?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/berglas.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/berglas
-        
-        .. image:: https://img.shields.io/pypi/pyversions/berglas.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/berglas
-        
-        .. image:: https://img.shields.io/pypi/implementation/berglas.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/berglas
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/ambv/black
-        
-        This library automatically parses berglas references when imported.
-        
-        Only Python 3.6+ is supported currently.
-        
-        You can find the latest, most up to date, documentation on `Github`_.
-        
-        Quick Start
-        -----------
-        
-        Install library:
-        
-        .. code:: sh
-        
-            pip install berglas
-        
-        Import the module:
-        
-        .. code:: python
-        
-            import berglas.auto  # noqa
-        
-        When imported, the `berglas` module will:
-        
-        1. Detect the runtime environment and call the appropriate API to get the list
-        of environment variables that were set on the resource at deploy time
-        
-        1. Download and decrypt any secrets that match the `Berglas environment
-        variable reference syntax`_
-        
-        1. Replace the value for the environment variable with the decrypted secret
-        
-        You can also opt out of auto-parsing and call the library yourself instead:
-        
-        .. code:: python
-        
-            import os
-        
-            from berglas import resolver
-        
-            if __name__ == '__main__':
-                client = resolver.Client()
-                client.replace("MY_SECRET")
-                print(os.environ["MY_SECRET"])
-        
-                // alternatively, use resolve method to simply get the value without updating environment:
-                my_secret = client.resolve(os.environ["MY_SECRET"])
-                print(my_secret)
-        
-        Release Notes
-        -------------
-        
-        v0.1
-        ~~~~
-        
-        - First version
-        
-        Development
-        -----------
-        
-        Getting Started
-        ~~~~~~~~~~~~~~~
-        Assuming that you have Python, ``pyenv`` and ``pyenv-virtualenv`` installed, set up your
-        environment and install the required dependencies like this instead of
-        the ``pip install berglas`` defined above:
-        
-        .. code:: sh
-        
-            $ git clone https://github.com/maroux/berglas-python.git
-            $ cd python
-            $ pyenv virtualenv 3.7.2 berglas-3.7
-            ...
-            $ pyenv shell berglas-3.7
-            $ pip install -r requirements/dev-3.7.txt
-        
-        Running Tests
-        ~~~~~~~~~~~~~
-        You can run tests in using ``make test``. By default,
-        it will run all of the unit and functional tests, but you can also specify your own
-        ``py.test`` options.
-        
-        .. code:: sh
-        
-            $ py.test
-        
-        
-        Getting Help
-        ------------
-        
-        We use GitHub issues for tracking bugs and feature requests.
-        
-        * If it turns out that you may have found a bug, please `open an issue <https://github.com/maroux/berglas-python/issues/new>`__
-        
-        .. _Github: github.com/maroux/berglas-python
-        .. _Berglas environment variable reference syntax: https://github.com/GoogleCloudPlatform/berglas/blob/master/doc/reference-syntax.md
-        
 Keywords: secrets gcs gcp
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Provides-Extra: dev
-Provides-Extra: publish
 Provides-Extra: test
+Provides-Extra: publish
+License-File: LICENSE
+
+Berglas Library for Python
+==========================
+
+.. image:: https://travis-ci.org/maroux/berglas-python.svg?branch=master
+    :target: https://travis-ci.org/maroux/berglas-python
+
+.. image:: https://coveralls.io/repos/github/maroux/berglas-python/badge.svg?branch=master
+    :target: https://coveralls.io/github/maroux/berglas-python?branch=master
+
+.. image:: https://img.shields.io/pypi/v/berglas.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/berglas
+
+.. image:: https://img.shields.io/pypi/pyversions/berglas.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/berglas
+
+.. image:: https://img.shields.io/pypi/implementation/berglas.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/berglas
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+
+This library automatically parses berglas references when imported.
+
+Only Python 3.6+ is supported currently.
+
+You can find the latest, most up to date, documentation on `Github`_.
+
+Quick Start
+-----------
+
+Install library:
+
+.. code:: sh
+
+    pip install berglas
+
+Import the module:
+
+.. code:: python
+
+    import berglas.auto  # noqa
+
+When imported, the `berglas` module will:
+
+1. Detect the runtime environment and call the appropriate API to get the list
+of environment variables that were set on the resource at deploy time
+
+1. Download and decrypt any secrets that match the `Berglas environment
+variable reference syntax`_
+
+1. Replace the value for the environment variable with the decrypted secret
+
+You can also opt out of auto-parsing and call the library yourself instead:
+
+.. code:: python
+
+    import os
+
+    from berglas import resolver
+
+    if __name__ == '__main__':
+        client = resolver.Client()
+        client.replace("MY_SECRET")
+        print(os.environ["MY_SECRET"])
+
+        // alternatively, use resolve method to simply get the value without updating environment:
+        my_secret = client.resolve(os.environ["MY_SECRET"])
+        print(my_secret)
+
+Release Notes
+-------------
+
+v0.1
+~~~~
+
+- First version
+
+Development
+-----------
+
+Getting Started
+~~~~~~~~~~~~~~~
+Assuming that you have Python, ``pyenv`` and ``pyenv-virtualenv`` installed, set up your
+environment and install the required dependencies like this instead of
+the ``pip install berglas`` defined above:
+
+.. code:: sh
+
+    $ git clone https://github.com/maroux/berglas-python.git
+    $ cd python
+    $ pyenv virtualenv 3.9.14 berglas-3.9
+    ...
+    $ pyenv shell berglas-3.9
+    $ pip install setuptools==58
+    $ pip install -r requirements/dev-3.9.txt
+
+Updating Requirements Files
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Update the `install_requires` variable in `setup.py` and then from the pyenv virtualenv shell run:
+.. code:: sh
+
+    $ python -m pip install pip==18.0 pip-tools==3.2.0 --upgrade
+    $ make pip_compile
+
+Running Tests
+~~~~~~~~~~~~~
+You can run tests in using ``make test``. By default,
+it will run all of the unit and functional tests, but you can also specify your own
+``py.test`` options.
+
+.. code:: sh
+
+    $ py.test
+
+
+Getting Help
+------------
+
+We use GitHub issues for tracking bugs and feature requests.
+
+* If it turns out that you may have found a bug, please `open an issue <https://github.com/maroux/berglas-python/issues/new>`__
+
+.. _Github: github.com/maroux/berglas-python
+.. _Berglas environment variable reference syntax: https://github.com/GoogleCloudPlatform/berglas/blob/master/doc/reference-syntax.md
```

### Comparing `berglas-0.1.0a3/README.rst` & `berglas-0.3.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -84,18 +84,27 @@
 environment and install the required dependencies like this instead of
 the ``pip install berglas`` defined above:
 
 .. code:: sh
 
     $ git clone https://github.com/maroux/berglas-python.git
     $ cd python
-    $ pyenv virtualenv 3.7.2 berglas-3.7
+    $ pyenv virtualenv 3.9.14 berglas-3.9
     ...
-    $ pyenv shell berglas-3.7
-    $ pip install -r requirements/dev-3.7.txt
+    $ pyenv shell berglas-3.9
+    $ pip install setuptools==58
+    $ pip install -r requirements/dev-3.9.txt
+
+Updating Requirements Files
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Update the `install_requires` variable in `setup.py` and then from the pyenv virtualenv shell run:
+.. code:: sh
+
+    $ python -m pip install pip==18.0 pip-tools==3.2.0 --upgrade
+    $ make pip_compile
 
 Running Tests
 ~~~~~~~~~~~~~
 You can run tests in using ``make test``. By default,
 it will run all of the unit and functional tests, but you can also specify your own
 ``py.test`` options.
```

### Comparing `berglas-0.1.0a3/berglas/auto.py` & `berglas-0.3.0/berglas/auto.py`

 * *Files identical despite different names*

### Comparing `berglas-0.1.0a3/berglas/resolver.py` & `berglas-0.3.0/berglas/resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,20 @@
 
         try:
             ciphertext = base64.decodebytes(parts[1])
         except binascii.Error:
             raise AutoException("invalid ciphertext: failed to parse ciphertext")
 
         try:
-            response = self.kms_client.decrypt(key, enc_dek, path.encode("UTF8"))
+            request = kms.DecryptRequest(
+                name=key,
+                ciphertext=enc_dek,
+                additional_authenticated_data=path.encode("UTF8")
+            )
+            response = self.kms_client.decrypt(request=request)
             dek = response.plaintext
         except (GoogleAPICallError, RetryError, ValueError):
             raise AutoException("failed to decrypt dek")
 
         return _decrypt_gcm(dek, ciphertext)
 
     def resolve(self, value: str) -> bytes:
```

### Comparing `berglas-0.1.0a3/berglas/runtime.py` & `berglas-0.3.0/berglas/runtime.py`

 * *Files identical despite different names*

### Comparing `berglas-0.1.0a3/berglas.egg-info/PKG-INFO` & `berglas-0.3.0/berglas.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,150 @@
 Metadata-Version: 2.1
 Name: berglas
-Version: 0.1.0a3
+Version: 0.3.0
 Summary: Berglas Python Library
 Home-page: https://github.com/maroux/berglas-python
 Author: Aniruddha Maru
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
-Description: Berglas Library for Python
-        ==========================
-        
-        .. image:: https://travis-ci.org/maroux/berglas-python.svg?branch=master
-            :target: https://travis-ci.org/maroux/berglas-python
-        
-        .. image:: https://coveralls.io/repos/github/maroux/berglas-python/badge.svg?branch=master
-            :target: https://coveralls.io/github/maroux/berglas-python?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/berglas.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/berglas
-        
-        .. image:: https://img.shields.io/pypi/pyversions/berglas.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/berglas
-        
-        .. image:: https://img.shields.io/pypi/implementation/berglas.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/berglas
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/ambv/black
-        
-        This library automatically parses berglas references when imported.
-        
-        Only Python 3.6+ is supported currently.
-        
-        You can find the latest, most up to date, documentation on `Github`_.
-        
-        Quick Start
-        -----------
-        
-        Install library:
-        
-        .. code:: sh
-        
-            pip install berglas
-        
-        Import the module:
-        
-        .. code:: python
-        
-            import berglas.auto  # noqa
-        
-        When imported, the `berglas` module will:
-        
-        1. Detect the runtime environment and call the appropriate API to get the list
-        of environment variables that were set on the resource at deploy time
-        
-        1. Download and decrypt any secrets that match the `Berglas environment
-        variable reference syntax`_
-        
-        1. Replace the value for the environment variable with the decrypted secret
-        
-        You can also opt out of auto-parsing and call the library yourself instead:
-        
-        .. code:: python
-        
-            import os
-        
-            from berglas import resolver
-        
-            if __name__ == '__main__':
-                client = resolver.Client()
-                client.replace("MY_SECRET")
-                print(os.environ["MY_SECRET"])
-        
-                // alternatively, use resolve method to simply get the value without updating environment:
-                my_secret = client.resolve(os.environ["MY_SECRET"])
-                print(my_secret)
-        
-        Release Notes
-        -------------
-        
-        v0.1
-        ~~~~
-        
-        - First version
-        
-        Development
-        -----------
-        
-        Getting Started
-        ~~~~~~~~~~~~~~~
-        Assuming that you have Python, ``pyenv`` and ``pyenv-virtualenv`` installed, set up your
-        environment and install the required dependencies like this instead of
-        the ``pip install berglas`` defined above:
-        
-        .. code:: sh
-        
-            $ git clone https://github.com/maroux/berglas-python.git
-            $ cd python
-            $ pyenv virtualenv 3.7.2 berglas-3.7
-            ...
-            $ pyenv shell berglas-3.7
-            $ pip install -r requirements/dev-3.7.txt
-        
-        Running Tests
-        ~~~~~~~~~~~~~
-        You can run tests in using ``make test``. By default,
-        it will run all of the unit and functional tests, but you can also specify your own
-        ``py.test`` options.
-        
-        .. code:: sh
-        
-            $ py.test
-        
-        
-        Getting Help
-        ------------
-        
-        We use GitHub issues for tracking bugs and feature requests.
-        
-        * If it turns out that you may have found a bug, please `open an issue <https://github.com/maroux/berglas-python/issues/new>`__
-        
-        .. _Github: github.com/maroux/berglas-python
-        .. _Berglas environment variable reference syntax: https://github.com/GoogleCloudPlatform/berglas/blob/master/doc/reference-syntax.md
-        
 Keywords: secrets gcs gcp
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Provides-Extra: dev
-Provides-Extra: publish
 Provides-Extra: test
+Provides-Extra: publish
+License-File: LICENSE
+
+Berglas Library for Python
+==========================
+
+.. image:: https://travis-ci.org/maroux/berglas-python.svg?branch=master
+    :target: https://travis-ci.org/maroux/berglas-python
+
+.. image:: https://coveralls.io/repos/github/maroux/berglas-python/badge.svg?branch=master
+    :target: https://coveralls.io/github/maroux/berglas-python?branch=master
+
+.. image:: https://img.shields.io/pypi/v/berglas.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/berglas
+
+.. image:: https://img.shields.io/pypi/pyversions/berglas.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/berglas
+
+.. image:: https://img.shields.io/pypi/implementation/berglas.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/berglas
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+
+This library automatically parses berglas references when imported.
+
+Only Python 3.6+ is supported currently.
+
+You can find the latest, most up to date, documentation on `Github`_.
+
+Quick Start
+-----------
+
+Install library:
+
+.. code:: sh
+
+    pip install berglas
+
+Import the module:
+
+.. code:: python
+
+    import berglas.auto  # noqa
+
+When imported, the `berglas` module will:
+
+1. Detect the runtime environment and call the appropriate API to get the list
+of environment variables that were set on the resource at deploy time
+
+1. Download and decrypt any secrets that match the `Berglas environment
+variable reference syntax`_
+
+1. Replace the value for the environment variable with the decrypted secret
+
+You can also opt out of auto-parsing and call the library yourself instead:
+
+.. code:: python
+
+    import os
+
+    from berglas import resolver
+
+    if __name__ == '__main__':
+        client = resolver.Client()
+        client.replace("MY_SECRET")
+        print(os.environ["MY_SECRET"])
+
+        // alternatively, use resolve method to simply get the value without updating environment:
+        my_secret = client.resolve(os.environ["MY_SECRET"])
+        print(my_secret)
+
+Release Notes
+-------------
+
+v0.1
+~~~~
+
+- First version
+
+Development
+-----------
+
+Getting Started
+~~~~~~~~~~~~~~~
+Assuming that you have Python, ``pyenv`` and ``pyenv-virtualenv`` installed, set up your
+environment and install the required dependencies like this instead of
+the ``pip install berglas`` defined above:
+
+.. code:: sh
+
+    $ git clone https://github.com/maroux/berglas-python.git
+    $ cd python
+    $ pyenv virtualenv 3.9.14 berglas-3.9
+    ...
+    $ pyenv shell berglas-3.9
+    $ pip install setuptools==58
+    $ pip install -r requirements/dev-3.9.txt
+
+Updating Requirements Files
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Update the `install_requires` variable in `setup.py` and then from the pyenv virtualenv shell run:
+.. code:: sh
+
+    $ python -m pip install pip==18.0 pip-tools==3.2.0 --upgrade
+    $ make pip_compile
+
+Running Tests
+~~~~~~~~~~~~~
+You can run tests in using ``make test``. By default,
+it will run all of the unit and functional tests, but you can also specify your own
+``py.test`` options.
+
+.. code:: sh
+
+    $ py.test
+
+
+Getting Help
+------------
+
+We use GitHub issues for tracking bugs and feature requests.
+
+* If it turns out that you may have found a bug, please `open an issue <https://github.com/maroux/berglas-python/issues/new>`__
+
+.. _Github: github.com/maroux/berglas-python
+.. _Berglas environment variable reference syntax: https://github.com/GoogleCloudPlatform/berglas/blob/master/doc/reference-syntax.md
```

### Comparing `berglas-0.1.0a3/setup.py` & `berglas-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,26 +40,27 @@
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
     ],
     python_requires=">=3.6",
     keywords="secrets gcs gcp",
     # https://mypy.readthedocs.io/en/latest/installed_packages.html
     package_data={"berglas": ["py.typed"]},
     packages=find_packages(exclude=["tests", "tests.*"]),
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=["pycryptodome", "google-api-python-client", "google-cloud-storage", "google-cloud-kms"],
+    install_requires=["pycryptodome", "google-api-python-client>=2", "google-cloud-storage>=2", "google-cloud-kms>=2"],
     tests_require=tests_require,
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={"dev": ["flake8"], "test": tests_require, "publish": ["twine", "wheel"]},
     include_package_data=True,
```

