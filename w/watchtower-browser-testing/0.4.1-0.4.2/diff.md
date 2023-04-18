# Comparing `tmp/watchtower_browser_testing-0.4.1.tar.gz` & `tmp/watchtower_browser_testing-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.4.1.tar", last modified: Tue Apr 18 07:11:40 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.2.tar", last modified: Tue Apr 18 07:26:00 2023, max compression
```

## Comparing `watchtower_browser_testing-0.4.1.tar` & `watchtower_browser_testing-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/
--rw-rw-rw-   0        0        0      310 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6149 2023-04-18 07:11:24.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    16875 2023-04-17 17:56:52.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-18 07:11:33.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/
+-rw-rw-rw-   0        0        0      310 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.068505 watchtower_browser_testing-0.4.2/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6193 2023-04-18 07:25:52.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    16875 2023-04-17 17:56:52.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-18 07:25:52.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:26:00.074687 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-18 07:25:59.000000 watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.4.1/setup.py` & `watchtower_browser_testing-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.1/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.4.2/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.1/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.2/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.1/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.4.2/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     margin-right: 0.5rem;
 }
 
 .message_check {
     vertical-align: text-bottom;
     margin-right: 0.5rem;
 }
+
+.scenario {
+    margin-bottom: 2rem;
+}
 </style>
 </head>
 <body>
     <div class="container">
         <div class="{{ content.type }}" id="container_{{ content.id }}" >
             {% if test_results %}
             {% if test_results.n_errors %}
```

### Comparing `watchtower_browser_testing-0.4.1/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.2/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.1/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.2/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.2/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

