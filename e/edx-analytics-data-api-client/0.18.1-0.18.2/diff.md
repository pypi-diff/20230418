# Comparing `tmp/edx-analytics-data-api-client-0.18.1.tar.gz` & `tmp/edx-analytics-data-api-client-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-analytics-data-api-client-0.18.1.tar", last modified: Mon Jul 25 18:03:41 2022, max compression
+gzip compressed data, was "edx-analytics-data-api-client-0.18.2.tar", last modified: Tue Apr 18 19:29:47 2023, max compression
```

## Comparing `edx-analytics-data-api-client-0.18.1.tar` & `edx-analytics-data-api-client-0.18.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 18:03:41.671831 edx-analytics-data-api-client-0.18.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/NOTICE.TXT
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-07-25 18:03:41.671831 edx-analytics-data-api-client-0.18.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 18:03:41.667831 edx-analytics-data-api-client-0.18.1/analyticsclient/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6686 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 18:03:41.671831 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/activity_types.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/data_formats.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/demographics.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/education_levels.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/enrollment_modes.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/genders.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/constants/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     4930 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/course.py
--rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/course_summaries.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/course_totals.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/programs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/analyticsclient/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 18:03:41.671831 edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-07-25 18:03:40.000000 edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-07-25 18:03:41.000000 edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 18:03:40.000000 edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-25 18:03:40.000000 edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-25 18:03:40.000000 edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 18:03:41.671831 edx-analytics-data-api-client-0.18.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-25 18:03:41.671831 edx-analytics-data-api-client-0.18.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-07-25 18:03:26.000000 edx-analytics-data-api-client-0.18.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:29:47.037385 edx-analytics-data-api-client-0.18.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/NOTICE.TXT
+-rw-r--r--   0 runner    (1001) docker     (122)     2372 2023-04-18 19:29:47.037385 edx-analytics-data-api-client-0.18.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:29:47.033385 edx-analytics-data-api-client-0.18.2/analyticsclient/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6686 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:29:47.033385 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/activity_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/demographics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/education_levels.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/enrollment_modes.py
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/genders.py
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/constants/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/course.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2927 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/course_summaries.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/course_totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/programs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/analyticsclient/status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:29:47.033385 edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2372 2023-04-18 19:29:46.000000 edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-04-18 19:29:47.000000 edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 19:29:46.000000 edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-18 19:29:46.000000 edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-18 19:29:46.000000 edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 19:29:47.037385 edx-analytics-data-api-client-0.18.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 19:29:47.037385 edx-analytics-data-api-client-0.18.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-04-18 19:29:43.000000 edx-analytics-data-api-client-0.18.2/setup.py
```

### Comparing `edx-analytics-data-api-client-0.18.1/LICENSE.TXT` & `edx-analytics-data-api-client-0.18.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/NOTICE.TXT` & `edx-analytics-data-api-client-0.18.2/NOTICE.TXT`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/PKG-INFO` & `edx-analytics-data-api-client-0.18.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: edx-analytics-data-api-client
-Version: 0.18.1
+Version: 0.18.2
 Summary: Client used to access edX analytics data warehouse
-Home-page: https://github.com/edx/edx-analytics-data-api-client
+Home-page: https://github.com/openedx/edx-analytics-data-api-client
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache License 2.0
 Description: edX Analytics API Client |build-status| |coverage-status|
         =========================================================
         
         The edX Analytics API Client (henceforth, client) allows users to retrieve data from the edX data warehouse. Currently,
@@ -23,18 +23,18 @@
         
         Contributions are very welcome, but for legal reasons, you must submit a signed
         `individual contributor's agreement`_ before we can accept your contribution. See our
         `CONTRIBUTING`_ file for more information -- it also contains guidelines for how to maintain
         high code quality, which will make your contribution more likely to be accepted.
         
         .. _individual contributor's agreement: http://code.edx.org/individual-contributor-agreement.pdf
-        .. _CONTRIBUTING: https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst
+        .. _CONTRIBUTING: https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst
         
-        .. |build-status| image:: https://github.com/edx/edx-analytics-data-api-client/workflows/Python%20CI/badge.svg?branch=master
-           :target: https://github.com/edx/edx-analytics-data-api-client/actions?query=workflow%3A%22Python+CI%22
+        .. |build-status| image:: https://github.com/openedx/edx-analytics-data-api-client/workflows/Python%20CI/badge.svg?branch=master
+           :target: https://github.com/openedx/edx-analytics-data-api-client/actions?query=workflow%3A%22Python+CI%22
         .. |coverage-status| image:: https://coveralls.io/repos/edx/edx-analytics-data-api-client/badge.png
            :target: https://coveralls.io/r/edx/edx-analytics-data-api-client
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `edx-analytics-data-api-client-0.18.1/README.rst` & `edx-analytics-data-api-client-0.18.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 
 Contributions are very welcome, but for legal reasons, you must submit a signed
 `individual contributor's agreement`_ before we can accept your contribution. See our
 `CONTRIBUTING`_ file for more information -- it also contains guidelines for how to maintain
 high code quality, which will make your contribution more likely to be accepted.
 
 .. _individual contributor's agreement: http://code.edx.org/individual-contributor-agreement.pdf
-.. _CONTRIBUTING: https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst
+.. _CONTRIBUTING: https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst
 
-.. |build-status| image:: https://github.com/edx/edx-analytics-data-api-client/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/edx-analytics-data-api-client/actions?query=workflow%3A%22Python+CI%22
+.. |build-status| image:: https://github.com/openedx/edx-analytics-data-api-client/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/edx-analytics-data-api-client/actions?query=workflow%3A%22Python+CI%22
 .. |coverage-status| image:: https://coveralls.io/repos/edx/edx-analytics-data-api-client/badge.png
    :target: https://coveralls.io/r/edx/edx-analytics-data-api-client
```

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/base.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/base.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/client.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/client.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/course.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/course.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/course_summaries.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/course_summaries.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/course_totals.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/course_totals.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/module.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/module.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/programs.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/programs.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/analyticsclient/status.py` & `edx-analytics-data-api-client-0.18.2/analyticsclient/status.py`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/PKG-INFO` & `edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: edx-analytics-data-api-client
-Version: 0.18.1
+Version: 0.18.2
 Summary: Client used to access edX analytics data warehouse
-Home-page: https://github.com/edx/edx-analytics-data-api-client
+Home-page: https://github.com/openedx/edx-analytics-data-api-client
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache License 2.0
 Description: edX Analytics API Client |build-status| |coverage-status|
         =========================================================
         
         The edX Analytics API Client (henceforth, client) allows users to retrieve data from the edX data warehouse. Currently,
@@ -23,18 +23,18 @@
         
         Contributions are very welcome, but for legal reasons, you must submit a signed
         `individual contributor's agreement`_ before we can accept your contribution. See our
         `CONTRIBUTING`_ file for more information -- it also contains guidelines for how to maintain
         high code quality, which will make your contribution more likely to be accepted.
         
         .. _individual contributor's agreement: http://code.edx.org/individual-contributor-agreement.pdf
-        .. _CONTRIBUTING: https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst
+        .. _CONTRIBUTING: https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst
         
-        .. |build-status| image:: https://github.com/edx/edx-analytics-data-api-client/workflows/Python%20CI/badge.svg?branch=master
-           :target: https://github.com/edx/edx-analytics-data-api-client/actions?query=workflow%3A%22Python+CI%22
+        .. |build-status| image:: https://github.com/openedx/edx-analytics-data-api-client/workflows/Python%20CI/badge.svg?branch=master
+           :target: https://github.com/openedx/edx-analytics-data-api-client/actions?query=workflow%3A%22Python+CI%22
         .. |coverage-status| image:: https://coveralls.io/repos/edx/edx-analytics-data-api-client/badge.png
            :target: https://coveralls.io/r/edx/edx-analytics-data-api-client
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `edx-analytics-data-api-client-0.18.1/edx_analytics_data_api_client.egg-info/SOURCES.txt` & `edx-analytics-data-api-client-0.18.2/edx_analytics_data_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-analytics-data-api-client-0.18.1/setup.py` & `edx-analytics-data-api-client-0.18.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 VERSION = get_version("analyticsclient", "__init__.py")
 
 
 setup(
     name='edx-analytics-data-api-client',
     version=VERSION,
     packages=['analyticsclient', 'analyticsclient.constants'],
-    url='https://github.com/edx/edx-analytics-data-api-client',
+    url='https://github.com/openedx/edx-analytics-data-api-client',
     description='Client used to access edX analytics data warehouse',
     long_description=LONG_DESCRIPTION,
     license='Apache License 2.0',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
```

