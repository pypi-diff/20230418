# Comparing `tmp/django-listable-0.7.0.tar.gz` & `tmp/django-listable-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-listable-0.7.0.tar", last modified: Fri Feb 24 17:36:36 2023, max compression
+gzip compressed data, was "django-listable-0.8.0.tar", last modified: Tue Apr 18 13:35:56 2023, max compression
```

## Comparing `django-listable-0.7.0.tar` & `django-listable-0.8.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.294904 django-listable-0.7.0/
--rw-r--r--   0 randlet   (1000) randlet   (1000)      161 2022-05-16 05:54:23.000000 django-listable-0.7.0/AUTHORS.rst
--rw-r--r--   0 randlet   (1000) randlet   (1000)     3279 2022-05-16 05:54:23.000000 django-listable-0.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 randlet   (1000) randlet   (1000)     2181 2023-02-24 17:30:50.000000 django-listable-0.7.0/HISTORY.rst
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1478 2022-05-16 05:54:23.000000 django-listable-0.7.0/LICENSE
--rw-r--r--   0 randlet   (1000) randlet   (1000)      176 2022-05-16 05:54:23.000000 django-listable-0.7.0/MANIFEST.in
--rw-rw-r--   0 randlet   (1000) randlet   (1000)    19555 2023-02-24 17:36:36.294904 django-listable-0.7.0/PKG-INFO
--rw-r--r--   0 randlet   (1000) randlet   (1000)    16631 2022-05-16 05:54:23.000000 django-listable-0.7.0/README.rst
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.286904 django-listable-0.7.0/django_listable.egg-info/
--rw-r--r--   0 randlet   (1000) randlet   (1000)    19555 2023-02-24 17:36:36.000000 django-listable-0.7.0/django_listable.egg-info/PKG-INFO
--rw-r--r--   0 randlet   (1000) randlet   (1000)     2404 2023-02-24 17:36:36.000000 django-listable-0.7.0/django_listable.egg-info/SOURCES.txt
--rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2023-02-24 17:36:36.000000 django-listable-0.7.0/django_listable.egg-info/dependency_links.txt
--rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2022-05-16 05:54:23.000000 django-listable-0.7.0/django_listable.egg-info/not-zip-safe
--rw-r--r--   0 randlet   (1000) randlet   (1000)        9 2023-02-24 17:36:36.000000 django-listable-0.7.0/django_listable.egg-info/top_level.txt
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.286904 django-listable-0.7.0/listable/
--rw-rw-r--   0 randlet   (1000) randlet   (1000)       22 2023-02-24 17:30:50.000000 django-listable-0.7.0/listable/__init__.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)       24 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/models.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)      993 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/settings.py
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.286904 django-listable-0.7.0/listable/static/
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.286904 django-listable-0.7.0/listable/static/listable/
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.290904 django-listable-0.7.0/listable/static/listable/css/
--rw-r--r--   0 randlet   (1000) randlet   (1000)    15809 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/bootstrap-datepicker.min.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1148 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/bootstrap.multiselect.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     8133 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/daterangepicker.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1765 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/demo_page.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)    10732 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/demo_table.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     8446 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/demo_table_jui.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)    29063 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/font-awesome.min.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1115 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/jquery.dataTables.bootstrap.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     4520 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/jquery.dataTables.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     4541 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/jquery.dataTables_themeroller.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)      499 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/css/listable.css
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.290904 django-listable-0.7.0/listable/static/listable/fonts/
--rw-r--r--   0 randlet   (1000) randlet   (1000)   391622 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/fonts/fontawesome-webfont.svg
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.290904 django-listable-0.7.0/listable/static/listable/img/
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1361 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/back_disabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/back_enabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1375 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/back_enabled_hover.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1363 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/forward_disabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1380 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/forward_enabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/forward_enabled_hover.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1118 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/sort_asc.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1050 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/sort_asc_disabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1136 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/sort_both.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1127 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/sort_desc.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1045 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/img/sort_desc_disabled.png
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.294904 django-listable-0.7.0/listable/static/listable/js/
--rw-r--r--   0 randlet   (1000) randlet   (1000)    34174 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/bootstrap-datepicker.min.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    63315 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/bootstrap.multiselect.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    68583 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/daterangepicker.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)     6316 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.bootstrap.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    34181 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.columnFilter.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)   373929 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    70879 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.min.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1628 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.searchPlugins.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)     4782 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.sort.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    93434 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/jquery.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    11927 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/listable.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)   134906 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/moment.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    46645 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/static/listable/js/moment.min.js
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.286904 django-listable-0.7.0/listable/templates/
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.294904 django-listable-0.7.0/listable/templates/listable/
--rw-r--r--   0 randlet   (1000) randlet   (1000)      712 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/templates/listable/_table.html
--rw-r--r--   0 randlet   (1000) randlet   (1000)      662 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/templates/listable/base.html
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.294904 django-listable-0.7.0/listable/templatetags/
--rw-r--r--   0 randlet   (1000) randlet   (1000)        0 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/templatetags/__init__.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)     8762 2022-10-03 20:43:12.000000 django-listable-0.7.0/listable/templatetags/listable.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)     2105 2022-05-16 05:54:23.000000 django-listable-0.7.0/listable/utils.py
--rw-rw-r--   0 randlet   (1000) randlet   (1000)    20183 2023-02-24 17:30:50.000000 django-listable-0.7.0/listable/views.py
--rw-rw-r--   0 randlet   (1000) randlet   (1000)       68 2023-02-24 17:36:36.294904 django-listable-0.7.0/setup.cfg
--rw-rw-r--   0 randlet   (1000) randlet   (1000)     1608 2023-02-24 17:30:50.000000 django-listable-0.7.0/setup.py
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-02-24 17:36:36.294904 django-listable-0.7.0/tests/
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1129 2022-05-16 05:54:23.000000 django-listable-0.7.0/tests/test_tags.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)      543 2022-05-16 05:54:23.000000 django-listable-0.7.0/tests/test_utils.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)    13431 2022-05-16 05:54:23.000000 django-listable-0.7.0/tests/test_views.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)      136 2022-05-16 05:54:23.000000 django-listable-0.7.0/tests/tests.py
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      161 2022-05-16 05:54:23.000000 django-listable-0.8.0/AUTHORS.rst
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     3279 2022-05-16 05:54:23.000000 django-listable-0.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)     2410 2023-04-18 13:33:01.000000 django-listable-0.8.0/HISTORY.rst
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1478 2022-05-16 05:54:23.000000 django-listable-0.8.0/LICENSE
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      176 2022-05-16 05:54:23.000000 django-listable-0.8.0/MANIFEST.in
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    20049 2023-04-18 13:35:56.299035 django-listable-0.8.0/PKG-INFO
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    16896 2023-04-18 13:33:01.000000 django-listable-0.8.0/README.rst
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/django_listable.egg-info/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    20049 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/PKG-INFO
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     2404 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/SOURCES.txt
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/dependency_links.txt
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2022-05-16 05:54:23.000000 django-listable-0.8.0/django_listable.egg-info/not-zip-safe
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        9 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/top_level.txt
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)       22 2023-04-18 13:33:01.000000 django-listable-0.8.0/listable/__init__.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)       24 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/models.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      993 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/settings.py
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.287036 django-listable-0.8.0/listable/static/
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.287036 django-listable-0.8.0/listable/static/listable/
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/static/listable/css/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    15809 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/bootstrap-datepicker.min.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1148 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/bootstrap.multiselect.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     8133 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/daterangepicker.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1765 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/demo_page.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    10732 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/demo_table.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     8446 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/demo_table_jui.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    29063 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/font-awesome.min.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1115 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.bootstrap.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     4520 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     4541 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/jquery.dataTables_themeroller.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      499 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/listable.css
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/static/listable/fonts/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)   391622 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/fonts/fontawesome-webfont.svg
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/static/listable/img/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1361 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/back_disabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/back_enabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1375 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/back_enabled_hover.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1363 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/forward_disabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1380 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/forward_enabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/forward_enabled_hover.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1118 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_asc.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1050 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_asc_disabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1136 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_both.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1127 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_desc.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1045 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_desc_disabled.png
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/listable/static/listable/js/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    34174 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/bootstrap-datepicker.min.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    63315 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/bootstrap.multiselect.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    68583 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/daterangepicker.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     6316 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.bootstrap.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    34181 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.columnFilter.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)   373929 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    70879 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.min.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1628 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.searchPlugins.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     4782 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.sort.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    93434 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    11927 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/listable.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)   134906 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/moment.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    46645 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/moment.min.js
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.287036 django-listable-0.8.0/listable/templates/
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/listable/templates/listable/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      712 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/templates/listable/_table.html
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      662 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/templates/listable/base.html
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/listable/templatetags/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        0 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/templatetags/__init__.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     8762 2022-10-03 20:43:12.000000 django-listable-0.8.0/listable/templatetags/listable.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     2105 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/utils.py
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    20434 2023-04-18 13:33:01.000000 django-listable-0.8.0/listable/views.py
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)       68 2023-04-18 13:35:56.299035 django-listable-0.8.0/setup.cfg
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)     1608 2023-04-18 13:33:01.000000 django-listable-0.8.0/setup.py
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/tests/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1129 2022-05-16 05:54:23.000000 django-listable-0.8.0/tests/test_tags.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      543 2022-05-16 05:54:23.000000 django-listable-0.8.0/tests/test_utils.py
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    16228 2023-04-18 13:33:01.000000 django-listable-0.8.0/tests/test_views.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      136 2022-05-16 05:54:23.000000 django-listable-0.8.0/tests/tests.py
```

### Comparing `django-listable-0.7.0/CONTRIBUTING.rst` & `django-listable-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/HISTORY.rst` & `django-listable-0.8.0/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 .. :changelog:
 
 =======
 History
 =======
 
+0.8.0 (2023-04-18)
+------------------
+
+* Added a loose_text_search setting to views.  Set ``loose_text_search = True``
+  on your view to enable partial matching in your text searches. For example
+  "Fo Ba" will match "Foo Bar".
+
 0.7.0 (2023-02-24)
 ------------------
 
 * Listable for Django 3.2
 
 0.6.0 (2021-10-07)
 ------------------
```

### Comparing `django-listable-0.7.0/LICENSE` & `django-listable-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/PKG-INFO` & `django-listable-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-listable
-Version: 0.7.0
+Version: 0.8.0
 Summary: A reusable Django app to make integrations with the DataTables javascript library easy.
 Home-page: https://github.com/randlet/django-listable
 Author: Randle Taylor
 Author-email: randle.taylor@gmail.com
 License: BSD
 Keywords: django-listable
 Classifier: Development Status :: 4 - Beta
@@ -255,14 +255,21 @@
         "last_name": "last_name__exact",
         "genericname": "genericname__icontains",
         "department__name": False,
     }
 
 if a field is not declared in search_field's it a filter using `icontains` is assumed.
 
+ *loose_text_search*
+
+If set to True, will split search terms. E.g. "Sm ti" will return an object with field value of "Small Ticket".
+This is very similar to how Django's admin backend does its searches. Be default, the value is False for backward
+compatibility.
+
+
 *order_fields (optional)*
 
 Order fields allows you to define how a column should be ordered (similar to
 Django's ordering or order_by).  For example::
 
 
     order_fields = {
@@ -624,14 +631,21 @@
 
 
 
 =======
 History
 =======
 
+0.8.0 (2023-04-18)
+------------------
+
+* Added a loose_text_search setting to views.  Set ``loose_text_search = True``
+  on your view to enable partial matching in your text searches. For example
+  "Fo Ba" will match "Foo Bar".
+
 0.7.0 (2023-02-24)
 ------------------
 
 * Listable for Django 3.2
 
 0.6.0 (2021-10-07)
 ------------------
```

### Comparing `django-listable-0.7.0/README.rst` & `django-listable-0.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,21 @@
         "last_name": "last_name__exact",
         "genericname": "genericname__icontains",
         "department__name": False,
     }
 
 if a field is not declared in search_field's it a filter using `icontains` is assumed.
 
+ *loose_text_search*
+
+If set to True, will split search terms. E.g. "Sm ti" will return an object with field value of "Small Ticket".
+This is very similar to how Django's admin backend does its searches. Be default, the value is False for backward
+compatibility.
+
+
 *order_fields (optional)*
 
 Order fields allows you to define how a column should be ordered (similar to
 Django's ordering or order_by).  For example::
 
 
     order_fields = {
```

### Comparing `django-listable-0.7.0/django_listable.egg-info/PKG-INFO` & `django-listable-0.8.0/django_listable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-listable
-Version: 0.7.0
+Version: 0.8.0
 Summary: A reusable Django app to make integrations with the DataTables javascript library easy.
 Home-page: https://github.com/randlet/django-listable
 Author: Randle Taylor
 Author-email: randle.taylor@gmail.com
 License: BSD
 Keywords: django-listable
 Classifier: Development Status :: 4 - Beta
@@ -255,14 +255,21 @@
         "last_name": "last_name__exact",
         "genericname": "genericname__icontains",
         "department__name": False,
     }
 
 if a field is not declared in search_field's it a filter using `icontains` is assumed.
 
+ *loose_text_search*
+
+If set to True, will split search terms. E.g. "Sm ti" will return an object with field value of "Small Ticket".
+This is very similar to how Django's admin backend does its searches. Be default, the value is False for backward
+compatibility.
+
+
 *order_fields (optional)*
 
 Order fields allows you to define how a column should be ordered (similar to
 Django's ordering or order_by).  For example::
 
 
     order_fields = {
@@ -624,14 +631,21 @@
 
 
 
 =======
 History
 =======
 
+0.8.0 (2023-04-18)
+------------------
+
+* Added a loose_text_search setting to views.  Set ``loose_text_search = True``
+  on your view to enable partial matching in your text searches. For example
+  "Fo Ba" will match "Foo Bar".
+
 0.7.0 (2023-02-24)
 ------------------
 
 * Listable for Django 3.2
 
 0.6.0 (2021-10-07)
 ------------------
```

### Comparing `django-listable-0.7.0/django_listable.egg-info/SOURCES.txt` & `django-listable-0.8.0/django_listable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/settings.py` & `django-listable-0.8.0/listable/settings.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/bootstrap-datepicker.min.css` & `django-listable-0.8.0/listable/static/listable/css/bootstrap-datepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/bootstrap.multiselect.css` & `django-listable-0.8.0/listable/static/listable/css/bootstrap.multiselect.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/daterangepicker.css` & `django-listable-0.8.0/listable/static/listable/css/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/demo_page.css` & `django-listable-0.8.0/listable/static/listable/css/demo_page.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/demo_table.css` & `django-listable-0.8.0/listable/static/listable/css/demo_table.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/demo_table_jui.css` & `django-listable-0.8.0/listable/static/listable/css/demo_table_jui.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/font-awesome.min.css` & `django-listable-0.8.0/listable/static/listable/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/jquery.dataTables.bootstrap.css` & `django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/jquery.dataTables.css` & `django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/css/jquery.dataTables_themeroller.css` & `django-listable-0.8.0/listable/static/listable/css/jquery.dataTables_themeroller.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/fonts/fontawesome-webfont.svg` & `django-listable-0.8.0/listable/static/listable/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/back_disabled.png` & `django-listable-0.8.0/listable/static/listable/img/back_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/back_enabled.png` & `django-listable-0.8.0/listable/static/listable/img/back_enabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/back_enabled_hover.png` & `django-listable-0.8.0/listable/static/listable/img/back_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/forward_disabled.png` & `django-listable-0.8.0/listable/static/listable/img/forward_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/forward_enabled.png` & `django-listable-0.8.0/listable/static/listable/img/forward_enabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/forward_enabled_hover.png` & `django-listable-0.8.0/listable/static/listable/img/forward_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/sort_asc.png` & `django-listable-0.8.0/listable/static/listable/img/sort_asc.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/sort_asc_disabled.png` & `django-listable-0.8.0/listable/static/listable/img/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/sort_both.png` & `django-listable-0.8.0/listable/static/listable/img/sort_both.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/sort_desc.png` & `django-listable-0.8.0/listable/static/listable/img/sort_desc.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/img/sort_desc_disabled.png` & `django-listable-0.8.0/listable/static/listable/img/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/bootstrap-datepicker.min.js` & `django-listable-0.8.0/listable/static/listable/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/bootstrap.multiselect.js` & `django-listable-0.8.0/listable/static/listable/js/bootstrap.multiselect.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/daterangepicker.js` & `django-listable-0.8.0/listable/static/listable/js/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.bootstrap.js` & `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.columnFilter.js` & `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.columnFilter.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.js` & `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.min.js` & `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.searchPlugins.js` & `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.searchPlugins.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/jquery.dataTables.sort.js` & `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.sort.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/jquery.js` & `django-listable-0.8.0/listable/static/listable/js/jquery.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/listable.js` & `django-listable-0.8.0/listable/static/listable/js/listable.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/moment.js` & `django-listable-0.8.0/listable/static/listable/js/moment.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/static/listable/js/moment.min.js` & `django-listable-0.8.0/listable/static/listable/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/templates/listable/_table.html` & `django-listable-0.8.0/listable/templates/listable/_table.html`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/templates/listable/base.html` & `django-listable-0.8.0/listable/templates/listable/base.html`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/templatetags/listable.py` & `django-listable-0.8.0/listable/templatetags/listable.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/utils.py` & `django-listable-0.8.0/listable/utils.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/listable/views.py` & `django-listable-0.8.0/listable/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from django.db.models import Q
 import django.db.models.fields
 from django.http import Http404, HttpResponse
 from django.template.loader import get_template
 from django.urls import resolve
 from django.utils import formats, timezone
+from django.utils.text import smart_split
 from django.utils.translation import ugettext as _
 from django.views.generic import ListView
 import six
 
 from . import settings as li_settings
 from . import utils
 
@@ -60,14 +61,15 @@
 
 class BaseListableView(ListView):
 
     fields = ()
     widgets = {}
     order_fields = {}
     search_fields = {}
+    loose_text_search = False
     headers = {}
 
     multi_separator = ', '
 
     paginate_by = li_settings.LISTABLE_PAGINATE_BY
     filter_delay = li_settings.LISTABLE_FILTER_DELAY
 
@@ -367,14 +369,16 @@
                             filtering = '{0}__icontains'.format(filtering)
 
                         elif widget in [DATE, DATE_RANGE]:
                             filtering = '{0}__range'.format(filtering)
 
                         if has_none:
                             qs = qs.filter(Q(**{"{0}__isnull".format(field): True}) | Q(**{filtering: search_term})).distinct()
+                        elif widget == TEXT and self.loose_text_search:
+                            qs = qs.filter(*[Q(**{filtering: term}) for term in smart_split(search_term)])
                         else:
                             qs = qs.filter(**{filtering: search_term}).distinct()
 
                 else:
 
                     if self.get_extra() and 'select' in self.get_extra() and field in self.get_extra()['select']:
                         raise ValueError('Multiple filters on field not configurable with extra.')
```

### Comparing `django-listable-0.7.0/setup.py` & `django-listable-0.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = '0.7.0'
+version = '0.8.0'
 
 if sys.argv[-1] == 'publish':
     os.system('python setup.py sdist upload')
     print("You probably want to also tag the version now:")
     print("  git tag -a %s -m 'version %s'" % (version, version))
     print("  git push --tags")
     sys.exit()
```

### Comparing `django-listable-0.7.0/tests/test_tags.py` & `django-listable-0.8.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/tests/test_utils.py` & `django-listable-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.7.0/tests/test_views.py` & `django-listable-0.8.0/tests/test_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import codecs
 import datetime
 import json
 import sys
 
+from unittest import mock
+
 from django.db.models import Q
 from django.test import Client, TestCase
 from django.urls import reverse
 from django.utils import timezone
 from listable import settings as lisettings
 
 from staff.models import INACTIVE, Staff
@@ -112,14 +114,43 @@
         payload = json.loads(response.content.decode('utf-8'))
         data = payload.pop("aaData")
         num_records = Staff.objects.filter(department__name=search_term).count()
 
         self.assertTrue(len(data) > 0)
         self.assertEqual(payload["iTotalDisplayRecords"], num_records)
 
+    def test_filter_plain_loose(self):
+        """Test filtering based on a plain text input with loose_text_searc = True"""
+
+        client = Client()
+        search_term = "Vol ta"  # should match Volup tas department
+        url = reverse("staff-list")+"?sEcho=1&iColumns=8&sColumns=&iDisplayStart=0&iDisplayLength=10&mDataProp_0=0&mDataProp_1=1&mDataProp_2=2&mDataProp_3=3&mDataProp_4=4&mDataProp_5=5&mDataProp_6=6&mDataProp_7=7&sSearch=&bRegex=false&sSearch_0=&bRegex_0=false&bSearchable_0=true&sSearch_1=&bRegex_1=false&bSearchable_1=true&sSearch_2=&bRegex_2=false&bSearchable_2=true&sSearch_3={search_term}&bRegex_3=false&bSearchable_3=true&sSearch_4=&bRegex_4=false&bSearchable_4=true&sSearch_5=&bRegex_5=false&bSearchable_5=true&sSearch_6=&bRegex_6=false&bSearchable_6=true&sSearch_7=&bRegex_7=false&bSearchable_7=true&iSortingCols=0&bSortable_0=true&bSortable_1=true&bSortable_2=true&bSortable_3=true&bSortable_4=true&bSortable_5=true&bSortable_6=true&bSortable_7=true&sRangeSeparator=~&_=1414439607643".format(search_term=search_term)
+
+        with mock.patch("staff.views.StaffList.loose_text_search", True):
+            response = client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+
+        num_records = Staff.objects.filter(department__name="Volup tas").count()
+        payload = json.loads(response.content.decode('utf-8'))
+        data = payload.pop("aaData")
+        assert len(data) == num_records
+
+    def test_filter_plain_loose_disabled(self):
+        """Test filtering based on a plain text input with loose_text_search = True"""
+
+        client = Client()
+        search_term = "Vol ta"  # should not match Volup tas department
+        url = reverse("staff-list")+"?sEcho=1&iColumns=8&sColumns=&iDisplayStart=0&iDisplayLength=10&mDataProp_0=0&mDataProp_1=1&mDataProp_2=2&mDataProp_3=3&mDataProp_4=4&mDataProp_5=5&mDataProp_6=6&mDataProp_7=7&sSearch=&bRegex=false&sSearch_0=&bRegex_0=false&bSearchable_0=true&sSearch_1=&bRegex_1=false&bSearchable_1=true&sSearch_2=&bRegex_2=false&bSearchable_2=true&sSearch_3={search_term}&bRegex_3=false&bSearchable_3=true&sSearch_4=&bRegex_4=false&bSearchable_4=true&sSearch_5=&bRegex_5=false&bSearchable_5=true&sSearch_6=&bRegex_6=false&bSearchable_6=true&sSearch_7=&bRegex_7=false&bSearchable_7=true&iSortingCols=0&bSortable_0=true&bSortable_1=true&bSortable_2=true&bSortable_3=true&bSortable_4=true&bSortable_5=true&bSortable_6=true&bSortable_7=true&sRangeSeparator=~&_=1414439607643".format(search_term=search_term)
+
+        with mock.patch("staff.views.StaffList.loose_text_search", False):
+            response = client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+
+        payload = json.loads(response.content.decode('utf-8'))
+        data = payload.pop("aaData")
+        assert len(data) == 0
+
     def test_filter_iterable(self):
         """Test filtering based on a plain text input"""
 
         client = Client()
         search_term = "Abbott"
         url = reverse("staff-list")+"?sEcho=19&iColumns=8&sColumns=&iDisplayStart=0&iDisplayLength=10&mDataProp_0=0&mDataProp_1=1&mDataProp_2=2&mDataProp_3=3&mDataProp_4=4&mDataProp_5=5&mDataProp_6=6&mDataProp_7=7&sSearch=&bRegex=false&sSearch_0=&bRegex_0=false&bSearchable_0=true&sSearch_1={search_term}&bRegex_1=false&bSearchable_1=true&sSearch_2=&bRegex_2=false&bSearchable_2=true&sSearch_3=&bRegex_3=false&bSearchable_3=true&sSearch_4=&bRegex_4=false&bSearchable_4=true&sSearch_5=&bRegex_5=false&bSearchable_5=true&sSearch_6=&bRegex_6=false&bSearchable_6=true&sSearch_7=&bRegex_7=false&bSearchable_7=true&iSortingCols=0&bSortable_0=true&bSortable_1=true&bSortable_2=true&bSortable_3=true&bSortable_4=true&bSortable_5=true&bSortable_6=true&bSortable_7=true&sRangeSeparator=~&_=1414439607645".format(search_term=search_term)
```

