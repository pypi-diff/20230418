# Comparing `tmp/kiwitcms-junit.xml-plugin-8.4.tar.gz` & `tmp/kiwitcms-junit.xml-plugin-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kiwitcms-junit.xml-plugin-8.4.tar", last modified: Wed Oct 28 19:56:02 2020, max compression
+gzip compressed data, was "dist/kiwitcms-junit.xml-plugin-9.0.tar", last modified: Wed Jan 13 11:46:34 2021, max compression
```

## Comparing `kiwitcms-junit.xml-plugin-8.4.tar` & `kiwitcms-junit.xml-plugin-9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/
-drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/kiwitcms_junit.xml_plugin.egg-info/
--rw-rw-r--   0 senko     (1002) senko     (1002)     6761 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/kiwitcms_junit.xml_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 senko     (1002) senko     (1002)      352 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/kiwitcms_junit.xml_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)        1 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/kiwitcms_junit.xml_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)       35 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/kiwitcms_junit.xml_plugin.egg-info/requires.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)       18 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/kiwitcms_junit.xml_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/tcms_junit_plugin/
--rw-rw-r--   0 senko     (1002) senko     (1002)     2500 2020-04-03 13:20:38.000000 kiwitcms-junit.xml-plugin-8.4/tcms_junit_plugin/__init__.py
--rw-rw-r--   0 senko     (1002) senko     (1002)    35149 2019-01-29 22:27:54.000000 kiwitcms-junit.xml-plugin-8.4/LICENSE
--rw-rw-r--   0 senko     (1002) senko     (1002)      122 2019-01-29 22:27:54.000000 kiwitcms-junit.xml-plugin-8.4/MANIFEST.in
--rw-rw-r--   0 senko     (1002) senko     (1002)     4590 2020-10-28 19:55:38.000000 kiwitcms-junit.xml-plugin-8.4/README.rst
--rw-rw-r--   0 senko     (1002) senko     (1002)       35 2020-10-28 19:53:52.000000 kiwitcms-junit.xml-plugin-8.4/requirements.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)     1364 2020-10-28 19:54:36.000000 kiwitcms-junit.xml-plugin-8.4/setup.py
--rwxrwxr-x   0 senko     (1002) senko     (1002)      254 2019-01-29 22:33:24.000000 kiwitcms-junit.xml-plugin-8.4/tcms-junit.xml-plugin
--rw-rw-r--   0 senko     (1002) senko     (1002)     6761 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/PKG-INFO
--rw-rw-r--   0 senko     (1002) senko     (1002)       38 2020-10-28 19:56:02.000000 kiwitcms-junit.xml-plugin-8.4/setup.cfg
+drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2021-01-13 11:46:34.000000 kiwitcms-junit.xml-plugin-9.0/
+drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2021-01-13 11:46:34.000000 kiwitcms-junit.xml-plugin-9.0/kiwitcms_junit.xml_plugin.egg-info/
+-rw-rw-r--   0 senko     (1002) senko     (1002)     7005 2021-01-13 11:46:33.000000 kiwitcms-junit.xml-plugin-9.0/kiwitcms_junit.xml_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 senko     (1002) senko     (1002)      352 2021-01-13 11:46:33.000000 kiwitcms-junit.xml-plugin-9.0/kiwitcms_junit.xml_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)        1 2021-01-13 11:46:33.000000 kiwitcms-junit.xml-plugin-9.0/kiwitcms_junit.xml_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)       33 2021-01-13 11:46:33.000000 kiwitcms-junit.xml-plugin-9.0/kiwitcms_junit.xml_plugin.egg-info/requires.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)       18 2021-01-13 11:46:33.000000 kiwitcms-junit.xml-plugin-9.0/kiwitcms_junit.xml_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2021-01-13 11:46:34.000000 kiwitcms-junit.xml-plugin-9.0/tcms_junit_plugin/
+-rw-rw-r--   0 senko     (1002) senko     (1002)     2785 2021-01-11 13:50:32.000000 kiwitcms-junit.xml-plugin-9.0/tcms_junit_plugin/__init__.py
+-rw-rw-r--   0 senko     (1002) senko     (1002)    35149 2019-01-29 22:27:54.000000 kiwitcms-junit.xml-plugin-9.0/LICENSE
+-rw-rw-r--   0 senko     (1002) senko     (1002)      122 2019-01-29 22:27:54.000000 kiwitcms-junit.xml-plugin-9.0/MANIFEST.in
+-rw-rw-r--   0 senko     (1002) senko     (1002)     4762 2021-01-13 11:45:45.000000 kiwitcms-junit.xml-plugin-9.0/README.rst
+-rw-rw-r--   0 senko     (1002) senko     (1002)       33 2021-01-13 11:44:10.000000 kiwitcms-junit.xml-plugin-9.0/requirements.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)     1364 2021-01-13 11:44:24.000000 kiwitcms-junit.xml-plugin-9.0/setup.py
+-rwxrwxr-x   0 senko     (1002) senko     (1002)      254 2019-01-29 22:33:24.000000 kiwitcms-junit.xml-plugin-9.0/tcms-junit.xml-plugin
+-rw-rw-r--   0 senko     (1002) senko     (1002)     7005 2021-01-13 11:46:34.000000 kiwitcms-junit.xml-plugin-9.0/PKG-INFO
+-rw-rw-r--   0 senko     (1002) senko     (1002)       38 2021-01-13 11:46:34.000000 kiwitcms-junit.xml-plugin-9.0/setup.cfg
```

### Comparing `kiwitcms-junit.xml-plugin-8.4/kiwitcms_junit.xml_plugin.egg-info/PKG-INFO` & `kiwitcms-junit.xml-plugin-9.0/kiwitcms_junit.xml_plugin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kiwitcms-junit.xml-plugin
-Version: 8.4
+Version: 9.0
 Summary: junit.xml plugin for Kiwi TCMS test case management system
 Home-page: https://github.com/kiwitcms/junit.xml-plugin
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Description: junit.xml plugin for Kiwi TCMS
         ==============================
@@ -104,14 +104,23 @@
             # define environment variables
             tcms-junit.xml-plugin /path/to/junit.xml
         
         
         Changelog
         ---------
         
+        v9.0 (13 Jan 2021)
+        ~~~~~~~~~~~~~~~~~~
+        
+        - Compatible with Kiwi TCMS v9.0
+        - Update tcms-api to 9.0
+        - Update junitparser to 2.0.0
+        - Adjusted code to handle jUnit v2.0 files
+        
+        
         v8.4 (28 Oct 2020)
         ~~~~~~~~~~~~~~~~~~
         
         - Update tcms-api to 8.6.0
         - Update junitparser to 1.6.0
```

### Comparing `kiwitcms-junit.xml-plugin-8.4/tcms_junit_plugin/__init__.py` & `kiwitcms-junit.xml-plugin-9.0/tcms_junit_plugin/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2021 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPLv3: https://www.gnu.org/licenses/gpl.html
 
 from junitparser import Error, Failure, JUnitXml, Skipped
 from tcms_api.plugin_helpers import Backend
 
 
@@ -25,38 +25,43 @@
         else:
             cases = list(xml)
 
         for xml_case in cases:
             summary = "%s.%s" % (xml_case.classname, xml_case.name)
 
             test_case, _ = self.backend.test_case_get_or_create(summary)
-            test_case_id = test_case['id']
-
-            self.backend.add_test_case_to_plan(test_case_id,
+            self.backend.add_test_case_to_plan(test_case['id'],
                                                self.backend.plan_id)
 
             test_execution_id = self.backend.add_test_case_to_run(
-                test_case_id,
+                test_case['id'],
                 self.backend.run_id)
             comment = 'Result recorded via Kiwi TCMS junit.xml-plugin'
 
-            if xml_case.result is None:
+            if not xml_case.result:
                 status_id = self.backend.get_status_id('PASSED')
 
-            if isinstance(xml_case.result, Failure):
-                status_id = self.backend.get_status_id('FAILED')
-                comment = xml_case.result.tostring()
-
-            if isinstance(xml_case.result, Error):
-                status_id = self.backend.get_status_id('ERROR')
-                comment = xml_case.result.tostring()
-
-            if isinstance(xml_case.result, Skipped):
-                status_id = self.backend.get_status_id('WAIVED')
-                comment = xml_case.result.message
+            # note: since junitpartser v2.0 the result attribute holds
+            # a list of values b/c pytest can produce files which contain
+            # multiple results for the same test case. We take the first!
+            for result in xml_case.result:
+                if isinstance(result, Failure):
+                    status_id = self.backend.get_status_id('FAILED')
+                    comment = result.tostring()
+                    break
+
+                if isinstance(result, Error):
+                    status_id = self.backend.get_status_id('ERROR')
+                    comment = result.tostring()
+                    break
+
+                if isinstance(result, Skipped):
+                    status_id = self.backend.get_status_id('WAIVED')
+                    comment = result.message
+                    break
 
             self.backend.update_test_execution(test_execution_id,
                                                status_id,
                                                comment)
 
             if progress_cb:
                 progress_cb()
```

### Comparing `kiwitcms-junit.xml-plugin-8.4/LICENSE` & `kiwitcms-junit.xml-plugin-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-junit.xml-plugin-8.4/README.rst` & `kiwitcms-junit.xml-plugin-9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,23 @@
     # define environment variables
     tcms-junit.xml-plugin /path/to/junit.xml
 
 
 Changelog
 ---------
 
+v9.0 (13 Jan 2021)
+~~~~~~~~~~~~~~~~~~
+
+- Compatible with Kiwi TCMS v9.0
+- Update tcms-api to 9.0
+- Update junitparser to 2.0.0
+- Adjusted code to handle jUnit v2.0 files
+
+
 v8.4 (28 Oct 2020)
 ~~~~~~~~~~~~~~~~~~
 
 - Update tcms-api to 8.6.0
 - Update junitparser to 1.6.0
```

### Comparing `kiwitcms-junit.xml-plugin-8.4/setup.py` & `kiwitcms-junit.xml-plugin-9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     LONG_DESCRIPTION = readme.read()
 
 
 REQUIREMENTS = open('requirements.txt').readlines()
 
 
 setup(name='kiwitcms-junit.xml-plugin',
-      version='8.4',
+      version='9.0',
       packages=['tcms_junit_plugin'],
       scripts=['tcms-junit.xml-plugin'],
       description='junit.xml plugin for '
                   'Kiwi TCMS test case management system',
       long_description=LONG_DESCRIPTION,
       author='Kiwi TCMS',
       author_email='info@kiwitcms.org',
```

### Comparing `kiwitcms-junit.xml-plugin-8.4/PKG-INFO` & `kiwitcms-junit.xml-plugin-9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kiwitcms-junit.xml-plugin
-Version: 8.4
+Version: 9.0
 Summary: junit.xml plugin for Kiwi TCMS test case management system
 Home-page: https://github.com/kiwitcms/junit.xml-plugin
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Description: junit.xml plugin for Kiwi TCMS
         ==============================
@@ -104,14 +104,23 @@
             # define environment variables
             tcms-junit.xml-plugin /path/to/junit.xml
         
         
         Changelog
         ---------
         
+        v9.0 (13 Jan 2021)
+        ~~~~~~~~~~~~~~~~~~
+        
+        - Compatible with Kiwi TCMS v9.0
+        - Update tcms-api to 9.0
+        - Update junitparser to 2.0.0
+        - Adjusted code to handle jUnit v2.0 files
+        
+        
         v8.4 (28 Oct 2020)
         ~~~~~~~~~~~~~~~~~~
         
         - Update tcms-api to 8.6.0
         - Update junitparser to 1.6.0
```

