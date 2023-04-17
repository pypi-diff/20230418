# Comparing `tmp/futurejson-0.2.0.tar.gz` & `tmp/futurejson-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futurejson-0.2.0.tar", last modified: Mon Apr 17 22:07:19 2023, max compression
+gzip compressed data, was "futurejson-0.3.0.tar", last modified: Mon Apr 17 22:12:40 2023, max compression
```

## Comparing `futurejson-0.2.0.tar` & `futurejson-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:07:19.626955 futurejson-0.2.0/
--rw-rw-rw-   0        0        0     1249 2023-04-17 22:07:19.626955 futurejson-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-04-17 21:47:24.000000 futurejson-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 22:07:19.611331 futurejson-0.2.0/futurejson.egg-info/
--rw-rw-rw-   0        0        0     1249 2023-04-17 22:07:19.000000 futurejson-0.2.0/futurejson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-17 22:07:19.000000 futurejson-0.2.0/futurejson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:07:19.000000 futurejson-0.2.0/futurejson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-17 22:07:19.000000 futurejson-0.2.0/futurejson.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:07:19.000000 futurejson-0.2.0/futurejson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 22:07:19.626955 futurejson-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-04-17 22:07:06.000000 futurejson-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:12:40.822054 futurejson-0.3.0/
+-rw-rw-rw-   0        0        0     1249 2023-04-17 22:12:40.822054 futurejson-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-04-17 21:47:24.000000 futurejson-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 22:12:40.806429 futurejson-0.3.0/futurejson.egg-info/
+-rw-rw-rw-   0        0        0     1249 2023-04-17 22:12:40.000000 futurejson-0.3.0/futurejson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-17 22:12:40.000000 futurejson-0.3.0/futurejson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:12:40.000000 futurejson-0.3.0/futurejson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 22:12:40.000000 futurejson-0.3.0/futurejson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:12:40.000000 futurejson-0.3.0/futurejson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:12:40.822054 futurejson-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-17 22:11:58.000000 futurejson-0.3.0/setup.py
```

### Comparing `futurejson-0.2.0/PKG-INFO` & `futurejson-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futurejson
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pure-python FutureJSON implementation
 Home-page: https://github.com/pwaller/pyfiglet
 Author: Andrew
 Author-email: andrew@systemacor.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `futurejson-0.2.0/futurejson.egg-info/PKG-INFO` & `futurejson-0.3.0/futurejson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futurejson
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pure-python FutureJSON implementation
 Home-page: https://github.com/pwaller/pyfiglet
 Author: Andrew
 Author-email: andrew@systemacor.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `futurejson-0.2.0/setup.py` & `futurejson-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='futurejson',
-    version='0.2.0',
+    version='0.3.0',
     author='Andrew',
     author_email='andrew@systemacor.net',
     description='Pure-python FutureJSON implementation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/pwaller/pyfiglet',
     packages=find_packages(),
     install_requires=[
-        'httpx',
-        'psutil',
-        'pycountry',
         'requests',
-        'telegram',
-        'asyncio',
-        'pillow',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

