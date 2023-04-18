# Comparing `tmp/django-knocker-0.5.0.tar.gz` & `tmp/django-knocker-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-knocker-0.5.0.tar", last modified: Sun Feb 19 22:36:56 2023, max compression
+gzip compressed data, was "django-knocker-0.5.1.tar", last modified: Tue Apr 18 21:01:23 2023, max compression
```

## Comparing `django-knocker-0.5.0.tar` & `django-knocker-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:36:56.296051 django-knocker-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-19 22:36:16.000000 django-knocker-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-02-19 22:36:16.000000 django-knocker-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-19 22:36:16.000000 django-knocker-0.5.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-19 22:36:16.000000 django-knocker-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-19 22:36:16.000000 django-knocker-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-02-19 22:36:56.296051 django-knocker-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-02-19 22:36:16.000000 django-knocker-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:36:56.292051 django-knocker-0.5.0/django_knocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-02-19 22:36:56.000000 django-knocker-0.5.0/django_knocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-19 22:36:56.000000 django-knocker-0.5.0/django_knocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 22:36:56.000000 django-knocker-0.5.0/django_knocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 22:36:41.000000 django-knocker-0.5.0/django_knocker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-19 22:36:56.000000 django-knocker-0.5.0/django_knocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-19 22:36:56.000000 django-knocker-0.5.0/django_knocker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:36:56.292051 django-knocker-0.5.0/knocker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-19 22:36:16.000000 django-knocker-0.5.0/knocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-19 22:36:16.000000 django-knocker-0.5.0/knocker/consumers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-02-19 22:36:16.000000 django-knocker-0.5.0/knocker/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:36:16.000000 django-knocker-0.5.0/knocker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-19 22:36:16.000000 django-knocker-0.5.0/knocker/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-19 22:36:16.000000 django-knocker-0.5.0/knocker/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:36:56.284051 django-knocker-0.5.0/knocker/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:36:56.292051 django-knocker-0.5.0/knocker/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-19 22:36:16.000000 django-knocker-0.5.0/knocker/static/js/knocker.js
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-19 22:36:16.000000 django-knocker-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-19 22:36:56.296051 django-knocker-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 22:36:16.000000 django-knocker-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:36:56.296051 django-knocker-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-19 22:36:16.000000 django-knocker-0.5.0/tests/test_consumers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-02-19 22:36:16.000000 django-knocker-0.5.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:01:23.258565 django-knocker-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-18 21:00:43.000000 django-knocker-0.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-18 21:00:43.000000 django-knocker-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-18 21:00:43.000000 django-knocker-0.5.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-18 21:00:43.000000 django-knocker-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 21:00:43.000000 django-knocker-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-18 21:01:23.258565 django-knocker-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-18 21:00:43.000000 django-knocker-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:01:23.258565 django-knocker-0.5.1/django_knocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-18 21:01:23.000000 django-knocker-0.5.1/django_knocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-18 21:01:23.000000 django-knocker-0.5.1/django_knocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:01:23.000000 django-knocker-0.5.1/django_knocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:01:08.000000 django-knocker-0.5.1/django_knocker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 21:01:23.000000 django-knocker-0.5.1/django_knocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 21:01:23.000000 django-knocker-0.5.1/django_knocker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:01:23.258565 django-knocker-0.5.1/knocker/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 21:00:43.000000 django-knocker-0.5.1/knocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-18 21:00:43.000000 django-knocker-0.5.1/knocker/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-18 21:00:43.000000 django-knocker-0.5.1/knocker/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:00:43.000000 django-knocker-0.5.1/knocker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-18 21:00:43.000000 django-knocker-0.5.1/knocker/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-18 21:00:43.000000 django-knocker-0.5.1/knocker/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:01:23.258565 django-knocker-0.5.1/knocker/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:01:23.258565 django-knocker-0.5.1/knocker/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-18 21:00:43.000000 django-knocker-0.5.1/knocker/static/js/knocker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 21:00:43.000000 django-knocker-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-18 21:01:23.258565 django-knocker-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:00:43.000000 django-knocker-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:01:23.258565 django-knocker-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-18 21:00:43.000000 django-knocker-0.5.1/tests/test_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-18 21:00:43.000000 django-knocker-0.5.1/tests/test_models.py
```

### Comparing `django-knocker-0.5.0/CONTRIBUTING.rst` & `django-knocker-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/HISTORY.rst` & `django-knocker-0.5.1/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 ***************
 History
 ***************
 
 .. towncrier release notes start
 
+0.5.1 (2023-04-18)
+==================
+
+Features
+--------
+
+- Add support for django 4.2 (#22)
+
+
 0.5.0 (2023-02-19)
 ==================
 
 Features
 --------
 
 - Upgrade to Channels 4.0 (#19)
```

### Comparing `django-knocker-0.5.0/LICENSE` & `django-knocker-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/PKG-INFO` & `django-knocker-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-knocker
-Version: 0.5.0
+Version: 0.5.1
 Summary: Channels-based desktop notification system
 Home-page: https://github.com/nephila/django-knocker
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: BSD
 Project-URL: Documentation, https://django-knocker.readthedocs.io/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -112,14 +113,23 @@
 
 ***************
 History
 ***************
 
 .. towncrier release notes start
 
+0.5.1 (2023-04-18)
+==================
+
+Features
+--------
+
+- Add support for django 4.2 (#22)
+
+
 0.5.0 (2023-02-19)
 ==================
 
 Features
 --------
 
 - Upgrade to Channels 4.0 (#19)
```

### Comparing `django-knocker-0.5.0/README.rst` & `django-knocker-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/django_knocker.egg-info/PKG-INFO` & `django-knocker-0.5.1/django_knocker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-knocker
-Version: 0.5.0
+Version: 0.5.1
 Summary: Channels-based desktop notification system
 Home-page: https://github.com/nephila/django-knocker
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: BSD
 Project-URL: Documentation, https://django-knocker.readthedocs.io/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -112,14 +113,23 @@
 
 ***************
 History
 ***************
 
 .. towncrier release notes start
 
+0.5.1 (2023-04-18)
+==================
+
+Features
+--------
+
+- Add support for django 4.2 (#22)
+
+
 0.5.0 (2023-02-19)
 ==================
 
 Features
 --------
 
 - Upgrade to Channels 4.0 (#19)
```

### Comparing `django-knocker-0.5.0/django_knocker.egg-info/SOURCES.txt` & `django-knocker-0.5.1/django_knocker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/knocker/consumers.py` & `django-knocker-0.5.1/knocker/consumers.py`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/knocker/mixins.py` & `django-knocker-0.5.1/knocker/mixins.py`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/knocker/signals.py` & `django-knocker-0.5.1/knocker/signals.py`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/knocker/static/js/knocker.js` & `django-knocker-0.5.1/knocker/static/js/knocker.js`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/setup.cfg` & `django-knocker-0.5.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
@@ -36,17 +37,14 @@
 test_suite = cms_helper.run
 zip_safe = False
 
 [options.package_data]
 * = *.txt, *.rst
 knocker = *.html *.png *.gif *js *jpg *jpeg *svg *py *mo *po
 
-[upload]
-repository = https://upload.pypi.org/legacy/
-
 [sdist]
 formats = zip
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
```

### Comparing `django-knocker-0.5.0/tests/test_consumers.py` & `django-knocker-0.5.1/tests/test_consumers.py`

 * *Files identical despite different names*

### Comparing `django-knocker-0.5.0/tests/test_models.py` & `django-knocker-0.5.1/tests/test_models.py`

 * *Files identical despite different names*

