# Comparing `tmp/django-custom-modal-admin-0.2.1.tar.gz` & `tmp/django-custom-modal-admin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-custom-modal-admin-0.2.1.tar", last modified: Fri Apr 14 07:58:59 2023, max compression
+gzip compressed data, was "django-custom-modal-admin-0.2.2.tar", last modified: Tue Apr 18 14:06:00 2023, max compression
```

## Comparing `django-custom-modal-admin-0.2.1.tar` & `django-custom-modal-admin-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.721947 django-custom-modal-admin-0.2.1/custom_modal_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.717947 django-custom-modal-admin-0.2.1/custom_modal_admin/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.721947 django-custom-modal-admin-0.2.1/custom_modal_admin/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/static/css/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.721947 django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/custom_modal_admin.js
--rw-r--r--   0 runner    (1001) docker     (123)   253747 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.228304 django-custom-modal-admin-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-18 14:06:00.228304 django-custom-modal-admin-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.220304 django-custom-modal-admin-0.2.2/custom_modal_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.216304 django-custom-modal-admin-0.2.2/custom_modal_admin/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.220304 django-custom-modal-admin-0.2.2/custom_modal_admin/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/static/css/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.224305 django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/custom_modal_admin.js
+-rw-r--r--   0 runner    (1001) docker     (123)   253747 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.224305 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:05:59.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 14:06:00.228304 django-custom-modal-admin-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/setup.py
```

### Comparing `django-custom-modal-admin-0.2.1/CONTRIBUTING.rst` & `django-custom-modal-admin-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/LICENSE.md` & `django-custom-modal-admin-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/PKG-INFO` & `django-custom-modal-admin-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-custom-modal-admin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Your project description goes here
 Home-page: https://github.com/frankhood/django-custom-modal-admin
 Author: FrankHood Business Solutions srl
 Author-email: info@frankhood.it
 License: MIT
 Keywords: django-custom-modal-admin
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-custom-modal-admin-0.2.1/README.rst` & `django-custom-modal-admin-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/custom_modal_admin/static/css/jquery-ui.css` & `django-custom-modal-admin-0.2.2/custom_modal_admin/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/custom_modal_admin.js` & `django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/custom_modal_admin.js`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/jquery-ui.min.js` & `django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/PKG-INFO` & `django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-custom-modal-admin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Your project description goes here
 Home-page: https://github.com/frankhood/django-custom-modal-admin
 Author: FrankHood Business Solutions srl
 Author-email: info@frankhood.it
 License: MIT
 Keywords: django-custom-modal-admin
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/SOURCES.txt` & `django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/requirements_test.txt` & `django-custom-modal-admin-0.2.2/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/setup.cfg` & `django-custom-modal-admin-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.1/setup.py` & `django-custom-modal-admin-0.2.2/setup.py`

 * *Files identical despite different names*

