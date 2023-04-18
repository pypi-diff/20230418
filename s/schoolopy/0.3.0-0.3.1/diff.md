# Comparing `tmp/schoolopy-0.3.0.tar.gz` & `tmp/schoolopy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolopy-0.3.0.tar", last modified: Tue Sep 27 00:47:44 2022, max compression
+gzip compressed data, was "schoolopy-0.3.1.tar", last modified: Tue Apr 18 15:43:00 2023, max compression
```

## Comparing `schoolopy-0.3.0.tar` & `schoolopy-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 erik       (501) staff       (20)        0 2022-09-27 00:47:44.117778 schoolopy-0.3.0/
--rw-rw-r--   0 erik       (501) staff       (20)     1068 2021-12-12 22:47:42.000000 schoolopy-0.3.0/LICENSE
--rw-rw-r--   0 erik       (501) staff       (20)     3398 2022-09-27 00:47:44.117941 schoolopy-0.3.0/PKG-INFO
--rw-rw-r--   0 erik       (501) staff       (20)     3159 2021-12-31 15:59:30.000000 schoolopy-0.3.0/README.rst
-drwxrwxr-x   0 erik       (501) staff       (20)        0 2022-09-27 00:47:44.112083 schoolopy-0.3.0/schoolopy/
--rw-rw-r--   0 erik       (501) staff       (20)      101 2021-12-12 22:47:42.000000 schoolopy-0.3.0/schoolopy/__init__.py
--rw-rw-r--   0 erik       (501) staff       (20)     4940 2021-12-12 22:47:42.000000 schoolopy-0.3.0/schoolopy/authentication.py
--rw-rw-r--   0 erik       (501) staff       (20)      369 2021-12-12 22:47:42.000000 schoolopy-0.3.0/schoolopy/errors.py
--rw-rw-r--   0 erik       (501) staff       (20)    89621 2022-07-09 18:59:51.000000 schoolopy-0.3.0/schoolopy/main.py
--rw-rw-r--   0 erik       (501) staff       (20)     1439 2022-07-09 18:59:51.000000 schoolopy-0.3.0/schoolopy/models.py
-drwxrwxr-x   0 erik       (501) staff       (20)        0 2022-09-27 00:47:44.117429 schoolopy-0.3.0/schoolopy.egg-info/
--rw-rw-r--   0 erik       (501) staff       (20)     3398 2022-09-27 00:47:44.000000 schoolopy-0.3.0/schoolopy.egg-info/PKG-INFO
--rw-rw-r--   0 erik       (501) staff       (20)      341 2022-09-27 00:47:44.000000 schoolopy-0.3.0/schoolopy.egg-info/SOURCES.txt
--rw-rw-r--   0 erik       (501) staff       (20)        1 2022-09-27 00:47:44.000000 schoolopy-0.3.0/schoolopy.egg-info/dependency_links.txt
--rw-rw-r--   0 erik       (501) staff       (20)        1 2021-12-31 15:53:59.000000 schoolopy-0.3.0/schoolopy.egg-info/not-zip-safe
--rw-rw-r--   0 erik       (501) staff       (20)       36 2022-09-27 00:47:44.000000 schoolopy-0.3.0/schoolopy.egg-info/requires.txt
--rw-rw-r--   0 erik       (501) staff       (20)       10 2022-09-27 00:47:44.000000 schoolopy-0.3.0/schoolopy.egg-info/top_level.txt
--rw-rw-r--   0 erik       (501) staff       (20)       80 2022-09-27 00:47:44.118522 schoolopy-0.3.0/setup.cfg
--rw-rw-r--   0 erik       (501) staff       (20)      544 2022-07-09 19:00:02.000000 schoolopy-0.3.0/setup.py
+drwxrwxr-x   0 erik       (501) staff       (20)        0 2023-04-18 15:43:00.249733 schoolopy-0.3.1/
+-rw-rw-r--   0 erik       (501) staff       (20)     1068 2023-04-18 15:42:41.000000 schoolopy-0.3.1/LICENSE
+-rw-rw-r--   0 erik       (501) staff       (20)     3398 2023-04-18 15:43:00.249929 schoolopy-0.3.1/PKG-INFO
+-rw-rw-r--   0 erik       (501) staff       (20)     3159 2023-04-18 15:42:41.000000 schoolopy-0.3.1/README.rst
+drwxrwxr-x   0 erik       (501) staff       (20)        0 2023-04-18 15:43:00.242767 schoolopy-0.3.1/schoolopy/
+-rw-rw-r--   0 erik       (501) staff       (20)      101 2023-04-18 15:42:41.000000 schoolopy-0.3.1/schoolopy/__init__.py
+-rw-rw-r--   0 erik       (501) staff       (20)     4940 2023-04-18 15:42:41.000000 schoolopy-0.3.1/schoolopy/authentication.py
+-rw-rw-r--   0 erik       (501) staff       (20)      369 2023-04-18 15:42:41.000000 schoolopy-0.3.1/schoolopy/errors.py
+-rw-rw-r--   0 erik       (501) staff       (20)    89413 2023-04-18 15:42:41.000000 schoolopy-0.3.1/schoolopy/main.py
+-rw-rw-r--   0 erik       (501) staff       (20)     1439 2023-04-18 15:42:41.000000 schoolopy-0.3.1/schoolopy/models.py
+drwxrwxr-x   0 erik       (501) staff       (20)        0 2023-04-18 15:43:00.249341 schoolopy-0.3.1/schoolopy.egg-info/
+-rw-rw-r--   0 erik       (501) staff       (20)     3398 2023-04-18 15:43:00.000000 schoolopy-0.3.1/schoolopy.egg-info/PKG-INFO
+-rw-rw-r--   0 erik       (501) staff       (20)      341 2023-04-18 15:43:00.000000 schoolopy-0.3.1/schoolopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik       (501) staff       (20)        1 2023-04-18 15:43:00.000000 schoolopy-0.3.1/schoolopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik       (501) staff       (20)        1 2023-04-18 15:43:00.000000 schoolopy-0.3.1/schoolopy.egg-info/not-zip-safe
+-rw-rw-r--   0 erik       (501) staff       (20)       36 2023-04-18 15:43:00.000000 schoolopy-0.3.1/schoolopy.egg-info/requires.txt
+-rw-rw-r--   0 erik       (501) staff       (20)       10 2023-04-18 15:43:00.000000 schoolopy-0.3.1/schoolopy.egg-info/top_level.txt
+-rw-rw-r--   0 erik       (501) staff       (20)       80 2023-04-18 15:43:00.263730 schoolopy-0.3.1/setup.cfg
+-rw-rw-r--   0 erik       (501) staff       (20)      544 2023-04-18 15:42:50.000000 schoolopy-0.3.1/setup.py
```

### Comparing `schoolopy-0.3.0/LICENSE` & `schoolopy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schoolopy-0.3.0/PKG-INFO` & `schoolopy-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolopy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper for Schoology's API.
 Home-page: https://github.com/ErikBoesen/schoolopy
 Author: Erik Boesen
 Author-email: me@erikboesen.com
 License: MIT
 License-File: LICENSE
```

### Comparing `schoolopy-0.3.0/README.rst` & `schoolopy-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `schoolopy-0.3.0/schoolopy/authentication.py` & `schoolopy-0.3.1/schoolopy/authentication.py`

 * *Files identical despite different names*

### Comparing `schoolopy-0.3.0/schoolopy/main.py` & `schoolopy-0.3.1/schoolopy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,26 +293,23 @@
         """
         Get data on all sections of a given course.
 
         :return: List of Section objects.
         """
         return [Section(raw) for raw in self._get('courses/%s/sections' % course_id)['section']]
 
-    def get_sections(self, course_id=None):
+    def get_sections(self, user_id=None):
         """
         Get data on all sections in which a user is enrolled.
-        If course_id is passed, the call will be passed through to get_course_sections,
-        which performs the original purpose of this method.
 
         :return: List of Section objects.
         """
-        # For backwards-compatibility
-        if course_id is not None:
-            return self.get_course_sections(course_id)
-        return [Section(raw) for raw in self._get('sections')['section']]
+        if user_id is not None:
+            return self.get_user_sections(user_id)
+        return self.get_user_sections(self.get_me()['uid'])
 
     def get_section(self, section_id):
         """
         Get data on a section.
 
         :param section_id: ID of section on which to get data.
         :return: Section object.
```

### Comparing `schoolopy-0.3.0/schoolopy/models.py` & `schoolopy-0.3.1/schoolopy/models.py`

 * *Files identical despite different names*

### Comparing `schoolopy-0.3.0/schoolopy.egg-info/PKG-INFO` & `schoolopy-0.3.1/schoolopy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolopy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper for Schoology's API.
 Home-page: https://github.com/ErikBoesen/schoolopy
 Author: Erik Boesen
 Author-email: me@erikboesen.com
 License: MIT
 License-File: LICENSE
```

### Comparing `schoolopy-0.3.0/setup.py` & `schoolopy-0.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.rst', 'r') as fh:
       long_description = fh.read()
 
 setup(name='schoolopy',
-      version='0.3.0',
+      version='0.3.1',
       description='A Python wrapper for Schoology\'s API.',
       long_description=long_description,
       url='https://github.com/ErikBoesen/schoolopy',
       author='Erik Boesen',
       author_email='me@erikboesen.com',
       license='MIT',
       packages=['schoolopy'],
```

