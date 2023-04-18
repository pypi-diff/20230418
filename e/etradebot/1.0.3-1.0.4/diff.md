# Comparing `tmp/etradebot-1.0.3.tar.gz` & `tmp/etradebot-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etradebot-1.0.3.tar", last modified: Tue Apr 18 19:23:03 2023, max compression
+gzip compressed data, was "etradebot-1.0.4.tar", last modified: Tue Apr 18 19:36:27 2023, max compression
```

## Comparing `etradebot-1.0.3.tar` & `etradebot-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:03.298000 etradebot-1.0.3/
--rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4944 2023-04-18 19:23:03.293000 etradebot-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4398 2023-04-16 01:46:23.000000 etradebot-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:02.680000 etradebot-1.0.3/authentication/
--rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.3/authentication/__init__.py
--rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.3/authentication/authentication.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:02.687000 etradebot-1.0.3/etrade/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.3/etrade/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.3/etrade/etrade.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:02.711000 etradebot-1.0.3/etradebot.egg-info/
--rw-rw-rw-   0        0        0     4944 2023-04-18 19:23:02.000000 etradebot-1.0.3/etradebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-04-18 19:23:02.000000 etradebot-1.0.3/etradebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       46 2023-04-18 19:23:02.000000 etradebot-1.0.3/etradebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      267 2023-04-18 19:23:02.000000 etradebot-1.0.3/etradebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2023-04-18 19:23:02.000000 etradebot-1.0.3/etradebot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:02.717000 etradebot-1.0.3/execute/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.3/execute/__init__.py
--rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.3/execute/execute.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:02.734000 etradebot-1.0.3/model/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.3/model/__init__.py
--rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.3/model/investor_views.py
--rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.3/model/model.py
--rw-rw-rw-   0        0        0       42 2023-04-18 19:23:03.296000 etradebot-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1375 2023-04-18 19:19:05.000000 etradebot-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:02.750000 etradebot-1.0.3/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.3/strategies/__init__.py
--rw-rw-rw-   0        0        0     3038 2023-04-18 19:12:36.000000 etradebot-1.0.3/strategies/cape_strategy.py
--rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.3/strategies/example_strategy.py
--rw-rw-rw-   0        0        0     1397 2023-04-18 19:13:26.000000 etradebot-1.0.3/strategies/strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:03.252000 etradebot-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.3/tests/mock_responses.py
--rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.3/tests/test_authentication.py
--rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.3/tests/test_etrade.py
--rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.3/tests/test_execute.py
--rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.3/tests/test_model.py
--rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.3/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:23:03.287000 etradebot-1.0.3/utils/
--rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.3/utils/__init__.py
--rw-rw-rw-   0        0        0     1126 2023-04-17 04:03:16.000000 etradebot-1.0.3/utils/credentials.py
--rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.3/utils/fake_data.py
--rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.3/utils/logging_config.py
--rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.3/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:27.034000 etradebot-1.0.4/
+-rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4944 2023-04-18 19:36:26.656000 etradebot-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4398 2023-04-16 01:46:23.000000 etradebot-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.086000 etradebot-1.0.4/authentication/
+-rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.4/authentication/__init__.py
+-rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.4/authentication/authentication.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.100000 etradebot-1.0.4/etrade/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/etrade/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.4/etrade/etrade.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.559000 etradebot-1.0.4/etradebot.egg-info/
+-rw-rw-rw-   0        0        0     4944 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       46 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       59 2023-04-18 19:36:25.000000 etradebot-1.0.4/etradebot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.568000 etradebot-1.0.4/execute/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/execute/__init__.py
+-rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.4/execute/execute.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.580000 etradebot-1.0.4/model/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/model/__init__.py
+-rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.4/model/investor_views.py
+-rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.4/model/model.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 19:36:27.032000 etradebot-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-04-18 19:34:10.000000 etradebot-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.602000 etradebot-1.0.4/strategies/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.4/strategies/__init__.py
+-rw-rw-rw-   0        0        0     3038 2023-04-18 19:12:36.000000 etradebot-1.0.4/strategies/cape_strategy.py
+-rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.4/strategies/example_strategy.py
+-rw-rw-rw-   0        0        0     1397 2023-04-18 19:13:26.000000 etradebot-1.0.4/strategies/strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.631000 etradebot-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.4/tests/mock_responses.py
+-rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.4/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.4/tests/test_etrade.py
+-rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.4/tests/test_execute.py
+-rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.4/tests/test_model.py
+-rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:36:26.653000 etradebot-1.0.4/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.4/utils/__init__.py
+-rw-rw-rw-   0        0        0     1126 2023-04-17 04:03:16.000000 etradebot-1.0.4/utils/credentials.py
+-rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.4/utils/fake_data.py
+-rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.4/utils/logging_config.py
+-rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.4/utils/portfolio.py
```

### Comparing `etradebot-1.0.3/LICENSE` & `etradebot-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/PKG-INFO` & `etradebot-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etradebot
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python-based trading bot for the E-Trade platform
 Home-page: https://github.com/nathanramoscfa/etradebot
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `etradebot-1.0.3/README.md` & `etradebot-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/authentication/authentication.py` & `etradebot-1.0.4/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/etrade/etrade.py` & `etradebot-1.0.4/etrade/etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/etradebot.egg-info/PKG-INFO` & `etradebot-1.0.4/etradebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etradebot
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python-based trading bot for the E-Trade platform
 Home-page: https://github.com/nathanramoscfa/etradebot
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `etradebot-1.0.3/etradebot.egg-info/SOURCES.txt` & `etradebot-1.0.4/etradebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/execute/execute.py` & `etradebot-1.0.4/execute/execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/model/investor_views.py` & `etradebot-1.0.4/model/investor_views.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/model/model.py` & `etradebot-1.0.4/model/model.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/setup.py` & `etradebot-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='etradebot',
-    version='1.0.3',
+    version='1.0.4',
     url='https://github.com/nathanramoscfa/etradebot',
     license='MIT',
     author='Nathan Ramos, CFA®',
     author_email='info@nrcapitalmanagement.com',
     description='A Python-based trading bot for the E-Trade platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `etradebot-1.0.3/strategies/cape_strategy.py` & `etradebot-1.0.4/strategies/cape_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/strategies/example_strategy.py` & `etradebot-1.0.4/strategies/example_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/strategies/strategy.py` & `etradebot-1.0.4/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/tests/mock_responses.py` & `etradebot-1.0.4/tests/mock_responses.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/tests/test_authentication.py` & `etradebot-1.0.4/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/tests/test_etrade.py` & `etradebot-1.0.4/tests/test_etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/tests/test_execute.py` & `etradebot-1.0.4/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/tests/test_model.py` & `etradebot-1.0.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/utils/credentials.py` & `etradebot-1.0.4/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/utils/fake_data.py` & `etradebot-1.0.4/utils/fake_data.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/utils/logging_config.py` & `etradebot-1.0.4/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.3/utils/portfolio.py` & `etradebot-1.0.4/utils/portfolio.py`

 * *Files identical despite different names*

