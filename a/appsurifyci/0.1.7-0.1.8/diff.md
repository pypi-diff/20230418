# Comparing `tmp/appsurifyci-0.1.7.tar.gz` & `tmp/appsurifyci-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appsurifyci-0.1.7.tar", last modified: Tue Apr 11 19:28:00 2023, max compression
+gzip compressed data, was "appsurifyci-0.1.8.tar", last modified: Tue Apr 18 19:14:40 2023, max compression
```

## Comparing `appsurifyci-0.1.7.tar` & `appsurifyci-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 19:28:00.019140 appsurifyci-0.1.7/
--rw-rw-rw-   0        0        0     2021 2022-11-03 08:45:50.000000 appsurifyci-0.1.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2021-03-19 06:30:43.000000 appsurifyci-0.1.7/LICENCE.txt
--rw-rw-rw-   0        0        0       32 2021-03-19 06:30:43.000000 appsurifyci-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6077 2023-04-11 19:28:00.019140 appsurifyci-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3468 2022-05-18 03:22:21.000000 appsurifyci-0.1.7/README.md
--rw-rw-rw-   0        0        0        8 2021-03-19 06:30:43.000000 appsurifyci-0.1.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 19:27:59.989488 appsurifyci-0.1.7/appsurifyci/
--rw-rw-rw-   0        0        0    38805 2023-04-11 19:25:12.000000 appsurifyci-0.1.7/appsurifyci/GitToAppsurify.py
--rw-rw-rw-   0        0        0    37851 2022-10-28 20:12:12.000000 appsurifyci-0.1.7/appsurifyci/GitToAppsurifyDev.py
--rw-rw-rw-   0        0        0   124785 2023-03-15 20:06:23.000000 appsurifyci-0.1.7/appsurifyci/RunTestsWithAppsurify3.py
--rw-rw-rw-   0        0        0   103616 2022-11-16 08:17:51.000000 appsurifyci-0.1.7/appsurifyci/RunTestsWithAppsurifyDev.py
--rw-rw-rw-   0        0        0        0 2021-03-19 06:30:43.000000 appsurifyci-0.1.7/appsurifyci/__init__.py
--rw-rw-rw-   0        0        0     6159 2023-03-15 20:06:40.000000 appsurifyci-0.1.7/appsurifyci/appsurifytests.txt
--rw-rw-rw-   0        0        0      286 2023-03-15 19:43:54.000000 appsurifyci-0.1.7/appsurifyci/testpython.py
--rw-rw-rw-   0        0        0      396 2022-08-12 01:27:20.000000 appsurifyci-0.1.7/appsurifyci/trxcpnvert.py
-drwxrwxrwx   0        0        0        0 2023-04-11 19:28:00.017108 appsurifyci-0.1.7/appsurifyci.egg-info/
--rw-rw-rw-   0        0        0     6077 2023-04-11 19:27:59.000000 appsurifyci-0.1.7/appsurifyci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-04-11 19:27:59.000000 appsurifyci-0.1.7/appsurifyci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 19:27:59.000000 appsurifyci-0.1.7/appsurifyci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-04-11 19:27:59.000000 appsurifyci-0.1.7/appsurifyci.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 19:27:59.000000 appsurifyci-0.1.7/appsurifyci.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 19:27:59.000000 appsurifyci-0.1.7/appsurifyci.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 19:28:00.019140 appsurifyci-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-04-11 19:18:26.000000 appsurifyci-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:14:40.092770 appsurifyci-0.1.8/
+-rw-rw-rw-   0        0        0     2021 2022-11-03 08:45:50.000000 appsurifyci-0.1.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2021-03-19 06:30:43.000000 appsurifyci-0.1.8/LICENCE.txt
+-rw-rw-rw-   0        0        0       32 2021-03-19 06:30:43.000000 appsurifyci-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6077 2023-04-18 19:14:40.092770 appsurifyci-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3468 2022-05-18 03:22:21.000000 appsurifyci-0.1.8/README.md
+-rw-rw-rw-   0        0        0        8 2021-03-19 06:30:43.000000 appsurifyci-0.1.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 19:14:40.071665 appsurifyci-0.1.8/appsurifyci/
+-rw-rw-rw-   0        0        0    38839 2023-04-18 19:13:55.000000 appsurifyci-0.1.8/appsurifyci/GitToAppsurify.py
+-rw-rw-rw-   0        0        0    37851 2022-10-28 20:12:12.000000 appsurifyci-0.1.8/appsurifyci/GitToAppsurifyDev.py
+-rw-rw-rw-   0        0        0   124785 2023-03-15 20:06:23.000000 appsurifyci-0.1.8/appsurifyci/RunTestsWithAppsurify3.py
+-rw-rw-rw-   0        0        0   103616 2022-11-16 08:17:51.000000 appsurifyci-0.1.8/appsurifyci/RunTestsWithAppsurifyDev.py
+-rw-rw-rw-   0        0        0        0 2021-03-19 06:30:43.000000 appsurifyci-0.1.8/appsurifyci/__init__.py
+-rw-rw-rw-   0        0        0     6159 2023-03-15 20:06:40.000000 appsurifyci-0.1.8/appsurifyci/appsurifytests.txt
+-rw-rw-rw-   0        0        0      286 2023-03-15 19:43:54.000000 appsurifyci-0.1.8/appsurifyci/testpython.py
+-rw-rw-rw-   0        0        0      396 2022-08-12 01:27:20.000000 appsurifyci-0.1.8/appsurifyci/trxcpnvert.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:14:40.091349 appsurifyci-0.1.8/appsurifyci.egg-info/
+-rw-rw-rw-   0        0        0     6077 2023-04-18 19:14:39.000000 appsurifyci-0.1.8/appsurifyci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-04-18 19:14:39.000000 appsurifyci-0.1.8/appsurifyci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 19:14:39.000000 appsurifyci-0.1.8/appsurifyci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-04-18 19:14:39.000000 appsurifyci-0.1.8/appsurifyci.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 19:14:39.000000 appsurifyci-0.1.8/appsurifyci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 19:14:39.000000 appsurifyci-0.1.8/appsurifyci.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 19:14:40.092770 appsurifyci-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-04-18 19:14:32.000000 appsurifyci-0.1.8/setup.py
```

### Comparing `appsurifyci-0.1.7/CHANGELOG.txt` & `appsurifyci-0.1.8/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/LICENCE.txt` & `appsurifyci-0.1.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/PKG-INFO` & `appsurifyci-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appsurifyci
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package used to run tests using Appsurify
 Home-page: https://appsurify.com
 Author: James Farrier
 Author-email: jamesfarrier@appsurify.com
 License: MIT
 Keywords: appsurify
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `appsurifyci-0.1.7/README.md` & `appsurifyci-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/appsurifyci/GitToAppsurify.py` & `appsurifyci-0.1.8/appsurifyci/GitToAppsurify.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,16 +653,16 @@
     person_date = "{}T{}{}".format(person_date[0], person_date[1], person_date[2])
     return {"name": person_name, "email": person_email, "date": person_date}
 
 
 def execute(commandLine):
     process = subprocess.Popen(commandLine, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
-    out = process.stdout.read().strip().decode("UTF-8")
-    error = process.stderr.read().strip().decode("UTF-8")
+    out = process.stdout.read().strip().decode("UTF-8", errors='ignore')
+    error = process.stderr.read().strip().decode("UTF-8", errors='ignore')
 
     if error:
         process.kill()
         if DEBUG:
             logging.debug("Execution '{}'".format(repr(commandLine)))
             logging.debug("with error '{}'".format(error))
         raise Exception(error)
```

### Comparing `appsurifyci-0.1.7/appsurifyci/GitToAppsurifyDev.py` & `appsurifyci-0.1.8/appsurifyci/GitToAppsurifyDev.py`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/appsurifyci/RunTestsWithAppsurify3.py` & `appsurifyci-0.1.8/appsurifyci/RunTestsWithAppsurify3.py`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/appsurifyci/RunTestsWithAppsurifyDev.py` & `appsurifyci-0.1.8/appsurifyci/RunTestsWithAppsurifyDev.py`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/appsurifyci/appsurifytests.txt` & `appsurifyci-0.1.8/appsurifyci/appsurifytests.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/appsurifyci.egg-info/PKG-INFO` & `appsurifyci-0.1.8/appsurifyci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appsurifyci
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package used to run tests using Appsurify
 Home-page: https://appsurify.com
 Author: James Farrier
 Author-email: jamesfarrier@appsurify.com
 License: MIT
 Keywords: appsurify
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `appsurifyci-0.1.7/appsurifyci.egg-info/SOURCES.txt` & `appsurifyci-0.1.8/appsurifyci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.7/setup.py` & `appsurifyci-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='appsurifyci',
-  version='0.1.7',
+  version='0.1.8',
   description='Package used to run tests using Appsurify',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://appsurify.com',  
   author='James Farrier',
   author_email='jamesfarrier@appsurify.com',
   license='MIT',
```

