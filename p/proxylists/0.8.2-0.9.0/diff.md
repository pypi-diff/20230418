# Comparing `tmp/proxylists-0.8.2.tar.gz` & `tmp/proxylists-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxylists-0.8.2.tar", last modified: Wed Aug  3 01:39:52 2022, max compression
+gzip compressed data, was "proxylists-0.9.0.tar", last modified: Tue Oct  4 10:53:54 2022, max compression
```

## Comparing `proxylists-0.8.2.tar` & `proxylists-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 01:39:52.896710 proxylists-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1301 2022-08-03 01:39:34.000000 proxylists-0.8.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)       62 2022-08-03 01:39:34.000000 proxylists-0.8.2/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-08-03 01:39:34.000000 proxylists-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    11441 2022-08-03 01:39:34.000000 proxylists-0.8.2/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (116)      153 2022-08-03 01:39:34.000000 proxylists-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      682 2022-08-03 01:39:52.896710 proxylists-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      793 2022-08-03 01:39:34.000000 proxylists-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 01:39:52.892710 proxylists-0.8.2/proxylists/
--rw-r--r--   0 runner    (1001) docker     (116)      441 2022-08-03 01:39:34.000000 proxylists-0.8.2/proxylists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 01:39:52.896710 proxylists-0.8.2/proxylists/proxies/
--rw-r--r--   0 runner    (1001) docker     (116)      194 2022-08-03 01:39:34.000000 proxylists-0.8.2/proxylists/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      997 2022-08-03 01:39:34.000000 proxylists-0.8.2/proxylists/proxies/connections.py
--rw-r--r--   0 runner    (1001) docker     (116)      775 2022-08-03 01:39:34.000000 proxylists-0.8.2/proxylists/proxies/freeproxy.py
--rw-r--r--   0 runner    (1001) docker     (116)      637 2022-08-03 01:39:34.000000 proxylists-0.8.2/proxylists/proxies/hidemy.py
--rw-r--r--   0 runner    (1001) docker     (116)      575 2022-08-03 01:39:34.000000 proxylists-0.8.2/proxylists/proxies/proxydb.py
--rw-r--r--   0 runner    (1001) docker     (116)     1366 2022-08-03 01:39:34.000000 proxylists-0.8.2/proxylists/proxies/server.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 01:39:52.896710 proxylists-0.8.2/proxylists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      682 2022-08-03 01:39:52.000000 proxylists-0.8.2/proxylists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      478 2022-08-03 01:39:52.000000 proxylists-0.8.2/proxylists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-03 01:39:52.000000 proxylists-0.8.2/proxylists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      151 2022-08-03 01:39:52.000000 proxylists-0.8.2/proxylists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-08-03 01:39:52.000000 proxylists-0.8.2/proxylists.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1113 2022-08-03 01:39:34.000000 proxylists-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-08-03 01:39:52.896710 proxylists-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1439 2022-08-03 01:39:34.000000 proxylists-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-04 10:53:54.960547 proxylists-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)     1301 2022-10-04 10:53:38.000000 proxylists-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (116)       62 2022-10-04 10:53:38.000000 proxylists-0.9.0/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-10-04 10:53:38.000000 proxylists-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      153 2022-10-04 10:53:38.000000 proxylists-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      666 2022-10-04 10:53:54.960547 proxylists-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      852 2022-10-04 10:53:38.000000 proxylists-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-04 10:53:54.956547 proxylists-0.9.0/proxylists/
+-rw-r--r--   0 runner    (1001) docker     (116)      428 2022-10-04 10:53:38.000000 proxylists-0.9.0/proxylists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-04 10:53:54.960547 proxylists-0.9.0/proxylists/proxies/
+-rw-r--r--   0 runner    (1001) docker     (116)      194 2022-10-04 10:53:38.000000 proxylists-0.9.0/proxylists/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      994 2022-10-04 10:53:38.000000 proxylists-0.9.0/proxylists/proxies/connections.py
+-rw-r--r--   0 runner    (1001) docker     (116)      775 2022-10-04 10:53:38.000000 proxylists-0.9.0/proxylists/proxies/freeproxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      653 2022-10-04 10:53:38.000000 proxylists-0.9.0/proxylists/proxies/hidemy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      575 2022-10-04 10:53:38.000000 proxylists-0.9.0/proxylists/proxies/proxydb.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1383 2022-10-04 10:53:38.000000 proxylists-0.9.0/proxylists/proxies/server.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-04 10:53:54.960547 proxylists-0.9.0/proxylists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      666 2022-10-04 10:53:54.000000 proxylists-0.9.0/proxylists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      463 2022-10-04 10:53:54.000000 proxylists-0.9.0/proxylists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-04 10:53:54.000000 proxylists-0.9.0/proxylists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      112 2022-10-04 10:53:54.000000 proxylists-0.9.0/proxylists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2022-10-04 10:53:54.000000 proxylists-0.9.0/proxylists.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1113 2022-10-04 10:53:38.000000 proxylists-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-04 10:53:54.960547 proxylists-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1426 2022-10-04 10:53:38.000000 proxylists-0.9.0/setup.py
```

### Comparing `proxylists-0.8.2/CONTRIBUTING.md` & `proxylists-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proxylists-0.8.2/LICENSE` & `proxylists-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxylists-0.8.2/PKG-INFO` & `proxylists-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: proxylists
-Version: 0.8.2
+Version: 0.9.0
 Summary: List of Proxy Servers
 Home-page: https://github.com/phenobarbital/proxylists
 Author: Jesus Lara
 Author-email: jlara@trocglobal.com
+License: BSD
 Project-URL: Source, https://github.com/phenobarbital/proxylists
 Project-URL: Funding, https://paypal.me/phenobarbital
 Project-URL: Say Thanks!, https://saythanks.io/to/phenobarbital
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 License-File: LICENSE
-License-File: LICENSE-APACHE
 
 Get a list of free Proxy Servers
```

### Comparing `proxylists-0.8.2/README.md` & `proxylists-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -37,7 +37,10 @@
 async def get_proxies():
      return await ProxyDB().get_list()
 
 loop = asyncio.get_event_loop()
 proxies = loop.run_until_complete(get_proxies())
 print(proxies)
 ```
+### License ###
+
+Proxylists is licensed under BSD license.
```

### Comparing `proxylists-0.8.2/proxylists/proxies/connections.py` & `proxylists-0.9.0/proxylists/proxies/connections.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def check_host(host: str, port: int = 80, timeout: int = 2) -> bool:
     """
     Check if an Address is reachable and available.
     """
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         s.settimeout(timeout)  # timeout
-        s.connect((address, int(port)))
+        s.connect((host, int(port)))
         return True
     except:
         return False
     finally:
       s.shutdown(socket.SHUT_RDWR)
       s.close()
```

### Comparing `proxylists-0.8.2/proxylists/proxies/freeproxy.py` & `proxylists-0.9.0/proxylists/proxies/freeproxy.py`

 * *Files identical despite different names*

### Comparing `proxylists-0.8.2/proxylists/proxies/hidemy.py` & `proxylists-0.9.0/proxylists/proxies/hidemy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import logging
 from .server import ProxyServer
 
 
+
 class Hidemy(ProxyServer):
     url = "https://hidemy.name/es/proxy-list/?type=s#list"
 
     async def get_proxies(self):
         proxies = []
         try:
             table = self.parser.xpath("//table")[0]
```

### Comparing `proxylists-0.8.2/proxylists/proxies/proxydb.py` & `proxylists-0.9.0/proxylists/proxies/proxydb.py`

 * *Files identical despite different names*

### Comparing `proxylists-0.8.2/proxylists/proxies/server.py` & `proxylists-0.9.0/proxylists/proxies/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             "Connection": "keep-alive",
             "Upgrade-Insecure-Requests": "1",
             "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) "
             "AppleWebKit/537.36 (KHTML, like Gecko) "
             "Chrome/83.0.4103.97 Safari/537.36",
         }
         async with aiohttp.ClientSession() as session:
-            async with session.get(self.url, headers=headers) as response:
+            async with session.get(self.url, headers=headers, timeout=timeout) as response:
                 if response.status == 200:
                     try:
                         content = await response.text()
                     except Exception as e:
                         print(e)
                         b = await response.content.read()
                         content = b.decode("utf-8")
```

### Comparing `proxylists-0.8.2/proxylists.egg-info/PKG-INFO` & `proxylists-0.9.0/proxylists.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: proxylists
-Version: 0.8.2
+Version: 0.9.0
 Summary: List of Proxy Servers
 Home-page: https://github.com/phenobarbital/proxylists
 Author: Jesus Lara
 Author-email: jlara@trocglobal.com
+License: BSD
 Project-URL: Source, https://github.com/phenobarbital/proxylists
 Project-URL: Funding, https://paypal.me/phenobarbital
 Project-URL: Say Thanks!, https://saythanks.io/to/phenobarbital
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 License-File: LICENSE
-License-File: LICENSE-APACHE
 
 Get a list of free Proxy Servers
```

### Comparing `proxylists-0.8.2/pyproject.toml` & `proxylists-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `proxylists-0.8.2/setup.py` & `proxylists-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Get a list of free Proxy Servers
 See:
 https://github.com/phenobarbital/proxylists
 """
 
 from setuptools import setup, find_packages
 
+
 setup(
     name='proxylists',
     version=open("VERSION").read().strip(),
     python_requires=">=3.8.0",
     url='https://github.com/phenobarbital/proxylists',
     description='List of Proxy Servers',
     long_description='Get a list of free Proxy Servers',
@@ -20,27 +21,27 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Programming Language :: Python :: 3.8',
     ],
     author='Jesus Lara',
     author_email='jlara@trocglobal.com',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
+    license='BSD',
+    license_file='LICENSE',
     setup_requires=[
         "wheel==0.37.1",
         "asyncio==3.4.3"
     ],
     install_requires=[
-        "wheel==0.37.1",
         "asyncio==3.4.3",
         "uvloop>=0.16.0",
-        "aiohttp==3.8.1",
+        "aiohttp==3.8.3",
         'requests>=2.25.0',
         'requests[socks]>=2.25.1',
-        'rapidjson>=1.0.0',
-        'python-rapidjson>=1.5',
+        'orjson==3.8.0',
         'lxml==4.9.1'
     ],
     tests_require=[
             'pytest>=5.4.0',
             'coverage'
     ],
     project_urls={  # Optional
```

