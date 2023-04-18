# Comparing `tmp/django-model-observer-1.0.0.tar.gz` & `tmp/django-model-observer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-model-observer-1.0.0.tar", last modified: Wed Jun 22 07:21:55 2022, max compression
+gzip compressed data, was "django-model-observer-1.1.0.tar", last modified: Tue Apr 18 07:38:01 2023, max compression
```

## Comparing `django-model-observer-1.0.0.tar` & `django-model-observer-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-22 07:21:55.952787 django-model-observer-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     3459 2022-06-22 07:21:34.000000 django-model-observer-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      230 2022-06-22 07:21:34.000000 django-model-observer-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      950 2022-06-22 07:21:55.952787 django-model-observer-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      598 2022-06-22 07:21:34.000000 django-model-observer-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-22 07:21:55.952787 django-model-observer-1.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1436 2022-06-22 07:21:34.000000 django-model-observer-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-22 07:21:55.949787 django-model-observer-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-22 07:21:55.950786 django-model-observer-1.0.0/src/django_model_observer/
--rw-r--r--   0 root         (0) root         (0)      195 2022-06-22 07:21:34.000000 django-model-observer-1.0.0/src/django_model_observer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11399 2022-06-22 07:21:34.000000 django-model-observer-1.0.0/src/django_model_observer/observer.py
--rw-r--r--   0 root         (0) root         (0)      950 2022-06-22 07:21:34.000000 django-model-observer-1.0.0/src/django_model_observer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-22 07:21:55.951786 django-model-observer-1.0.0/src/django_model_observer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      950 2022-06-22 07:21:55.000000 django-model-observer-1.0.0/src/django_model_observer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      406 2022-06-22 07:21:55.000000 django-model-observer-1.0.0/src/django_model_observer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       43 2022-06-22 07:21:55.000000 django-model-observer-1.0.0/src/django_model_observer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-06-22 07:21:55.000000 django-model-observer-1.0.0/src/django_model_observer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-06-22 07:21:55.000000 django-model-observer-1.0.0/src/django_model_observer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      450 2022-06-22 07:21:54.000000 django-model-observer-1.0.0/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:38:01.647594 django-model-observer-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3459 2022-06-22 07:21:34.000000 django-model-observer-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      230 2022-06-22 07:21:34.000000 django-model-observer-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-18 07:38:01.646594 django-model-observer-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      598 2022-06-22 07:21:34.000000 django-model-observer-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 07:38:01.647594 django-model-observer-1.1.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1612 2023-04-18 07:37:48.000000 django-model-observer-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:38:01.639594 django-model-observer-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:38:01.644594 django-model-observer-1.1.0/src/django_model_observer/
+-rw-r--r--   0 root         (0) root         (0)      195 2022-06-22 07:21:34.000000 django-model-observer-1.1.0/src/django_model_observer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11399 2022-06-22 07:21:34.000000 django-model-observer-1.1.0/src/django_model_observer/observer.py
+-rw-r--r--   0 root         (0) root         (0)      950 2022-06-22 07:21:34.000000 django-model-observer-1.1.0/src/django_model_observer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:38:01.646594 django-model-observer-1.1.0/src/django_model_observer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-18 07:38:01.000000 django-model-observer-1.1.0/src/django_model_observer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      406 2023-04-18 07:38:01.000000 django-model-observer-1.1.0/src/django_model_observer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-18 07:38:01.000000 django-model-observer-1.1.0/src/django_model_observer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-18 07:38:01.000000 django-model-observer-1.1.0/src/django_model_observer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-18 07:38:01.000000 django-model-observer-1.1.0/src/django_model_observer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-18 07:38:01.000000 django-model-observer-1.1.0/version.conf
```

### Comparing `django-model-observer-1.0.0/LICENSE` & `django-model-observer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-model-observer-1.0.0/PKG-INFO` & `django-model-observer-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: django-model-observer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Наблюдатель за моделями Django
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/django-model-observer/
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
```

### Comparing `django-model-observer-1.0.0/README.md` & `django-model-observer-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-model-observer-1.0.0/setup.py` & `django-model-observer-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,28 +21,32 @@
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     package_dir={'': 'src'},
     packages=find_packages('src'),
     include_package_data=True,
     dependency_links=(
         'http://pypi.bars-open.ru/simple/m3-builder',
     ),
     setup_requires=(
         'm3-builder>=1.2,<2',
     ),
     install_requires=(
         'six>=1.11,<2',
-        'Django>=2.2,<4.1',
+        'Django>=2.2,<4.3',
     ),
     set_build_info=Path(__file__).parent,
 )
```

### Comparing `django-model-observer-1.0.0/src/django_model_observer/observer.py` & `django-model-observer-1.1.0/src/django_model_observer/observer.py`

 * *Files identical despite different names*

### Comparing `django-model-observer-1.0.0/src/django_model_observer/utils.py` & `django-model-observer-1.1.0/src/django_model_observer/utils.py`

 * *Files identical despite different names*

### Comparing `django-model-observer-1.0.0/src/django_model_observer.egg-info/PKG-INFO` & `django-model-observer-1.1.0/src/django_model_observer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: django-model-observer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Наблюдатель за моделями Django
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/django-model-observer/
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
```

