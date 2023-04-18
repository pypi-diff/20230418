# Comparing `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.4b0.tar.gz` & `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.5.tar.gz`

## Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0.tar` & `rozklad_ontu_parser_makisukurisu-0.0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/requirements.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/run_lint.bat
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/run_lint.sh
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/example.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/base.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/dataclasses.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/enums.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/parser.py
--rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/sender.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/LICENSE
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/readme.md
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/run_lint.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/run_lint.sh
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/example.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/base.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/dataclasses.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/enums.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/parser.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/sender.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/LICENSE
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/readme.md
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.5/PKG-INFO
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/ISSUE_TEMPLATE/feature_request.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/pylint.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/python-publish.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/example.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/example.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/base.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/base.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/dataclasses.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/dataclasses.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/enums.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/enums.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/parser.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/parser.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/sender.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/ontu_parser/classes/sender.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module for sending operations"""
 import time
 from datetime import datetime
 import requests
 from selenium import webdriver
 from selenium.webdriver import FirefoxOptions
-from selenium.webdriver.common.proxy import Proxy, ProxyType
 
 from .base import BaseClass
 from .enums import RequestsEnum
 
 class TTLValue(BaseClass):
     """Describes value with some time to live (like authorization token)"""
     _ttl: int = 3600  # Time To Live (in seconds)
@@ -116,30 +115,21 @@
                 if cookie['name'] == 'PHPSESSID':
                     phpsesid = cookie['value']
         return (notbot, pow_result, phpsesid)
 
     def get_notbot(self):
         """Gets notbot by making webdriver request (emulates JS)"""
         options = self._browser_kwargs.pop('options', None)
-        desired_capabilities = self._browser_kwargs.pop('desired_capabilities', None)
         if not options:
             options = FirefoxOptions()
             options.add_argument("--headless")
-        if not desired_capabilities:
-            print("Using local proxy at port 8888 (if available)")
-            proxy = Proxy()
-            proxy.proxy_type = ProxyType.MANUAL
-            proxy.http_proxy = "127.0.0.1:8888"
-            proxy.ssl_proxy = "127.0.0.1:8888"
-            desired_capabilities = webdriver.DesiredCapabilities.FIREFOX
-            proxy.add_to_capabilities(desired_capabilities)
 
         driver = webdriver.Firefox(
             options=options,
-            desired_capabilities=desired_capabilities,
+            # desired_capabilities=desired_capabilities,
             **self._browser_kwargs
         )
         i = 0
         while True:
             print("Making request to get cookies")
             notbot, pow_result, phpsesid = self.__make_request(
                 driver=driver
@@ -184,15 +174,15 @@
             )
 
         try:
             response: requests.Response = session.request(
                 method=method,
                 url=self.link,
                 cookies=self.cookies.value,
-                data=data
+                data=data,
             )
         except Exception as exception:
             raise ValueError(
                 f'could not get response from {self.link}, got exception: {exception}',
                 self.link,
                 exception
             ) from exception
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/LICENSE` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/pyproject.toml` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rozklad_ontu_parser_MakisuKurisu"
-version = "0.0.3.4b"
+version = "0.0.3.5"
 authors = [
   {  name="Pavlo Pohorieltsev", email="667strets@gmail.com"  },
 ]
 description = "Package for parsing data from rozklad.ontu.edu.ua"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/readme.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/readme.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/PKG-INFO` & `rozklad_ontu_parser_makisukurisu-0.0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozklad_ontu_parser_MakisuKurisu
-Version: 0.0.3.4b0
+Version: 0.0.3.5
 Summary: Package for parsing data from rozklad.ontu.edu.ua
 Project-URL: Homepage, https://github.com/makisukurisu/rozklad-ontu-parser
 Project-URL: Bug Tracker, https://github.com/makisukurisu/rozklad-ontu-parser/issues
 Author-email: Pavlo Pohorieltsev <667strets@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

