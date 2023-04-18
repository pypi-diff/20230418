# Comparing `tmp/huscy.consents-0.7.0a17.tar.gz` & `tmp/huscy.consents-0.7.0a18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.consents-0.7.0a17.tar", last modified: Tue Apr  4 14:02:46 2023, max compression
+gzip compressed data, was "huscy.consents-0.7.0a18.tar", last modified: Tue Apr 18 03:17:43 2023, max compression
```

## Comparing `huscy.consents-0.7.0a17.tar` & `huscy.consents-0.7.0a18.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.693147 huscy.consents-0.7.0a17/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.7.0a17/MANIFEST.in
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1066 2023-04-04 14:02:46.693147 huscy.consents-0.7.0a17/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.7.0a17/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.677146 huscy.consents-0.7.0a17/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.681146 huscy.consents-0.7.0a17/huscy/consents/
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a17/huscy/consents/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a17/huscy/consents/api_urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.7.0a17/huscy/consents/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/forms.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.681146 huscy.consents-0.7.0a17/huscy/consents/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2023-04-04 14:02:46.000000 huscy.consents-0.7.0a17/huscy/consents/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      638 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a17/huscy/consents/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a17/huscy/consents/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6112 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a17/huscy/consents/services.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.677146 huscy.consents-0.7.0a17/huscy/consents/static/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.681146 huscy.consents-0.7.0a17/huscy/consents/static/css/
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/css/fomantic.min.css
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/css/fomantic2.9.0.min.css
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.681146 huscy.consents-0.7.0a17/huscy/consents/static/img/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-03-24 12:56:21.000000 huscy.consents-0.7.0a17/huscy/consents/static/img/logo.svg
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.689146 huscy.consents-0.7.0a17/huscy/consents/static/js/
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/js/fomantic.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/js/fomantic2.9.0.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/js/jquery.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/js/jquery3.6.1.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/js/popper.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/static/js/popper1.16.1.min.js
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.677146 huscy.consents-0.7.0a17/huscy/consents/templates/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.689146 huscy.consents-0.7.0a17/huscy/consents/templates/consents/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      572 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/base.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/create_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4333 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/sign_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3120 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/signed_consent.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/success.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.693147 huscy.consents-0.7.0a17/huscy/consents/templates/consents/text_fragments/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/text_fragments/checkbox.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      111 2023-01-10 14:57:17.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/text_fragments/header.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/text_fragments/paragraph.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.693147 huscy.consents-0.7.0a17/huscy/consents/templates/consents/widgets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/templates/consents/widgets/select_date.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.693147 huscy.consents-0.7.0a17/huscy/consents/templatetags/
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/templatetags/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/templatetags/dict_extras.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a17/huscy/consents/urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a17/huscy/consents/views.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a17/huscy/consents/viewsets.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-04 14:02:46.677146 huscy.consents-0.7.0a17/huscy.consents.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1066 2023-04-04 14:02:46.000000 huscy.consents-0.7.0a17/huscy.consents.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1540 2023-04-04 14:02:46.000000 huscy.consents-0.7.0a17/huscy.consents.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-04 14:02:46.000000 huscy.consents-0.7.0a17/huscy.consents.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      189 2023-04-04 14:02:46.000000 huscy.consents-0.7.0a17/huscy.consents.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-04 14:02:46.000000 huscy.consents-0.7.0a17/huscy.consents.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-04 14:02:46.693147 huscy.consents-0.7.0a17/setup.cfg
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1730 2023-03-10 14:41:58.000000 huscy.consents-0.7.0a17/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.7.0a18/MANIFEST.in
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.7.0a18/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a18/huscy/consents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/api_urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.7.0a18/huscy/consents/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/forms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.602908 huscy.consents-0.7.0a18/huscy/consents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2023-04-18 03:17:42.000000 huscy.consents-0.7.0a18/huscy/consents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      638 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a18/huscy/consents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6112 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a18/huscy/consents/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/static/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/static/consents/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.606909 huscy.consents-0.7.0a18/huscy/consents/static/consents/css/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic.min.css
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic2.9.0.min.css
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.606909 huscy.consents-0.7.0a18/huscy/consents/static/consents/img/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/img/logo.svg
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.614909 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic2.9.0.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery3.6.1.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper1.16.1.min.js
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/templates/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templates/consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/base.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/create_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/sign_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/signed_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/success.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/checkbox.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      111 2023-01-10 14:57:17.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/header.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/paragraph.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templates/consents/widgets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/widgets/select_date.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templatetags/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/templatetags/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/templatetags/dict_extras.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/views.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy.consents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1621 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      189 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/setup.cfg
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1736 2023-04-17 17:43:14.000000 huscy.consents-0.7.0a18/setup.py
```

### Comparing `huscy.consents-0.7.0a17/PKG-INFO` & `huscy.consents-0.7.0a18/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.7.0a17
+Version: 0.7.0a18
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.consents-0.7.0a17/huscy/consents/admin.py` & `huscy.consents-0.7.0a18/huscy/consents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/forms.py` & `huscy.consents-0.7.0a18/huscy/consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/migrations/0001_initial.py` & `huscy.consents-0.7.0a18/huscy/consents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/models.py` & `huscy.consents-0.7.0a18/huscy/consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/serializer.py` & `huscy.consents-0.7.0a18/huscy/consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/services.py` & `huscy.consents-0.7.0a18/huscy/consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/css/fomantic.min.css` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/css/fomantic2.9.0.min.css` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic2.9.0.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/img/logo.svg` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/img/logo.svg`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/js/fomantic.min.js` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/js/fomantic2.9.0.min.js` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic2.9.0.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/js/jquery.min.js` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/js/jquery3.6.1.min.js` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/js/popper.min.js` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/static/js/popper1.16.1.min.js` & `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper1.16.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/templates/consents/base.html` & `huscy.consents-0.7.0a18/huscy/consents/templates/consents/base.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 {% load static %}
 
 <!DOCTYPE html>
 <html>
     <head>
         <title>huscy{% block title %}{% endblock %}</title>
 
-        <script src="{% static 'js/jquery.min.js' %}"></script>
-        <script src="{% static 'js/fomantic.min.js' %}"></script>
+        <script src="{% static 'consents/js/jquery.min.js' %}"></script>
+        <script src="{% static 'consents/js/fomantic.min.js' %}"></script>
 
-        <link rel="stylesheet" type="text/css" href="{% static 'css/fomantic.min.css' %}">
+        <link rel="stylesheet" type="text/css" href="{% static 'consents/css/fomantic.min.css' %}">
 
         <style>
             {% block extra_css %}{% endblock %}
         </style>
     </head>
 
     <body>
```

### Comparing `huscy.consents-0.7.0a17/huscy/consents/templates/consents/create_consent.html` & `huscy.consents-0.7.0a18/huscy/consents/templates/consents/create_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/templates/consents/sign_consent.html` & `huscy.consents-0.7.0a18/huscy/consents/templates/consents/sign_consent.html`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,14 @@
         </div>
 
         <div class="row">
             <div class="six wide column">
                 <button class="ui right floated primary button">Submit</button>
                 <div class="ui right floated button" onClick="document.getElementsByClassName('btn')[0].click()">Reset</div>
 
-                <script src="{% static 'js/popper.min.js' %}"></script>
+                <script src="{% static 'consents/js/popper.min.js' %}"></script>
                 {{ form.media }}
             </div>
         </div>
     </div>
 </form>
 {% endblock %}
```

### Comparing `huscy.consents-0.7.0a17/huscy/consents/templates/consents/signed_consent.html` & `huscy.consents-0.7.0a18/huscy/consents/templates/consents/signed_consent.html`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 {% endblock %}
 
 
 {% block body %}
 <header>
     <div>
-        <img src="{% static 'img/logo.svg' %}">
+        <img src="{% static 'consents/img/logo.svg' %}">
     </div>
 </header>
 
 <main>
     <div class="header">
         <h1>{{ consent.name }}</h1>
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 jsignature_filters %} {% load static %} {% block title %} - signed consent{%
 endblock %} {% block extra_css %} @page { margin: 0; size: A4; } body { margin:
 0; } header { background-color: #eeeeee; } header div { height: 3.2cm; padding:
 5mm 5mm 12mm 5mm; } main { margin: 12mm 15mm; font-family: Arial, Helvetica,
 sans-serif; } main .header { text-align: center; } main .textfragments
 { margin-top: 1.5cm; } main .signature { margin-top: 1cm; } footer { bottom:
 10px; left: 10px; position: fixed; } {% endblock %} {% block body %}
-[{% static 'img/logo.svg' %}]
+[{% static 'consents/img/logo.svg' %}]
 
 ****** {{ consent.name }} ******
 Name         {{ form.cleaned_data.first_name }} {{ form.cleaned_data.last_name
              }}
 Adresse      {{ form.cleaned_data.postal_code }} {{ form.cleaned_data.city }},
              {{ form.cleaned_data.street }}
 Kontaktdaten {{ form.cleaned_data.phone_number }}
```

### Comparing `huscy.consents-0.7.0a17/huscy/consents/views.py` & `huscy.consents-0.7.0a18/huscy/consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy/consents/viewsets.py` & `huscy.consents-0.7.0a18/huscy/consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a17/huscy.consents.egg-info/PKG-INFO` & `huscy.consents-0.7.0a18/huscy.consents.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.7.0a17
+Version: 0.7.0a18
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.consents-0.7.0a17/huscy.consents.egg-info/SOURCES.txt` & `huscy.consents-0.7.0a18/huscy.consents.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 huscy/consents/serializer.py
 huscy/consents/services.py
 huscy/consents/urls.py
 huscy/consents/views.py
 huscy/consents/viewsets.py
 huscy/consents/migrations/0001_initial.py
 huscy/consents/migrations/__init__.py
-huscy/consents/static/css/fomantic.min.css
-huscy/consents/static/css/fomantic2.9.0.min.css
-huscy/consents/static/img/logo.svg
-huscy/consents/static/js/fomantic.min.js
-huscy/consents/static/js/fomantic2.9.0.min.js
-huscy/consents/static/js/jquery.min.js
-huscy/consents/static/js/jquery3.6.1.min.js
-huscy/consents/static/js/popper.min.js
-huscy/consents/static/js/popper1.16.1.min.js
+huscy/consents/static/consents/css/fomantic.min.css
+huscy/consents/static/consents/css/fomantic2.9.0.min.css
+huscy/consents/static/consents/img/logo.svg
+huscy/consents/static/consents/js/fomantic.min.js
+huscy/consents/static/consents/js/fomantic2.9.0.min.js
+huscy/consents/static/consents/js/jquery.min.js
+huscy/consents/static/consents/js/jquery3.6.1.min.js
+huscy/consents/static/consents/js/popper.min.js
+huscy/consents/static/consents/js/popper1.16.1.min.js
 huscy/consents/templates/consents/base.html
 huscy/consents/templates/consents/create_consent.html
 huscy/consents/templates/consents/sign_consent.html
 huscy/consents/templates/consents/signed_consent.html
 huscy/consents/templates/consents/success.html
 huscy/consents/templates/consents/text_fragments/checkbox.html
 huscy/consents/templates/consents/text_fragments/header.html
```

### Comparing `huscy.consents-0.7.0a17/setup.py` & `huscy.consents-0.7.0a18/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
 )
```

