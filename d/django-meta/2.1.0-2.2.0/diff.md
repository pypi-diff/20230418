# Comparing `tmp/django-meta-2.1.0.tar.gz` & `tmp/django-meta-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-meta-2.1.0.tar", last modified: Thu Jul 28 21:12:42 2022, max compression
+gzip compressed data, was "django-meta-2.2.0.tar", last modified: Tue Apr 18 21:11:41 2023, max compression
```

## Comparing `django-meta-2.1.0.tar` & `django-meta-2.2.0.tar`

### file list

```diff
@@ -1,68 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-07-28 21:12:05.000000 django-meta-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-07-28 21:12:05.000000 django-meta-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-07-28 21:12:05.000000 django-meta-2.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-28 21:12:05.000000 django-meta-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-07-28 21:12:05.000000 django-meta-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8057 2022-07-28 21:12:42.291601 django-meta-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-07-28 21:12:05.000000 django-meta-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/django_meta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8057 2022-07-28 21:12:42.000000 django-meta-2.1.0/django_meta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-28 21:12:42.000000 django-meta-2.1.0/django_meta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 21:12:42.000000 django-meta-2.1.0/django_meta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 21:12:30.000000 django-meta-2.1.0/django_meta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-28 21:12:42.000000 django-meta-2.1.0/django_meta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-28 21:12:42.000000 django-meta-2.1.0/django_meta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.287601 django-meta-2.1.0/meta/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     6343 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/templates/meta/
--rw-r--r--   0 runner    (1001) docker     (121)     4571 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/templates/meta/meta.html
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/templates/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/templates/meta_mixin/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/templates/meta_mixin/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7009 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/templatetags/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/templatetags/meta_extra.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10604 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:12:42.291601 django-meta-2.1.0/meta_mixin/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-28 21:12:05.000000 django-meta-2.1.0/meta_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-07-28 21:12:05.000000 django-meta-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-07-28 21:12:42.291601 django-meta-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-28 21:12:05.000000 django-meta-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-18 21:11:06.000000 django-meta-2.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-18 21:11:06.000000 django-meta-2.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-18 21:11:06.000000 django-meta-2.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-18 21:11:06.000000 django-meta-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 21:11:06.000000 django-meta-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-18 21:11:41.059384 django-meta-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-18 21:11:06.000000 django-meta-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/django_meta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-18 21:11:41.000000 django-meta-2.2.0/django_meta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-18 21:11:41.000000 django-meta-2.2.0/django_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:11:41.000000 django-meta-2.2.0/django_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:11:27.000000 django-meta-2.2.0/django_meta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 21:11:41.000000 django-meta-2.2.0/django_meta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 21:11:41.000000 django-meta-2.2.0/django_meta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.055384 django-meta-2.2.0/meta/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/templates/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/templates/meta/meta.html
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/templates/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/templates/meta_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/templates/meta_mixin/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/templatetags/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/templatetags/meta_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/meta_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-18 21:11:06.000000 django-meta-2.2.0/meta_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-18 21:11:06.000000 django-meta-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 21:11:41.059384 django-meta-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:11:06.000000 django-meta-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:41.059384 django-meta-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-18 21:11:06.000000 django-meta-2.2.0/tests/test_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-18 21:11:06.000000 django-meta-2.2.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-04-18 21:11:06.000000 django-meta-2.2.0/tests/test_metadata_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-04-18 21:11:06.000000 django-meta-2.2.0/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-04-18 21:11:06.000000 django-meta-2.2.0/tests/test_templatetags.py
```

### Comparing `django-meta-2.1.0/AUTHORS.rst` & `django-meta-2.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/CONTRIBUTING.rst` & `django-meta-2.2.0/CONTRIBUTING.rst`

 * *Files 5% similar despite different names*

```diff
@@ -161,11 +161,11 @@
 #. Update changelog via towncrier: ``towncrier --yes``
 #. Commit changelog with ``git commit --amend`` to merge with bumpversion commit
 #. Create tag ``git tag <version>``
 #. Push tag to github
 #. Publish the release from the tags page
 #. If pipeline succeeds, push ``master``
 #. Merge ``master`` back on ``develop``
-#. Bump developement version via task: ``inv tag-dev -l (major|minor|patch)``
+#. Bump development version via task: ``inv tag-dev -l (major|minor|patch)``
 #. Push ``develop``
 
 .. _towncrier: https://pypi.org/project/towncrier/#news-fragments
```

### Comparing `django-meta-2.1.0/HISTORY.rst` & `django-meta-2.2.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+2.2.0 (2023-04-18)
+==================
+
+Features
+--------
+
+- Move to ruff (#138)
+- Add support for Django 4.2 (#144)
+
+
 2.1.0 (2022-07-28)
 ==================
 
 Bugfixes
 --------
 
 - Changes imports from ugettext_lazy to gettext_lazy to fix deprecation warning (#130)
```

### Comparing `django-meta-2.1.0/LICENSE` & `django-meta-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/PKG-INFO` & `django-meta-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: django-meta
-Version: 2.1.0
+Version: 2.2.0
 Summary: Pluggable app for handling webpage meta tags and OpenGraph properties
 Home-page: https://github.com/nephila/django-meta
 Author: Monwara LLC
 Author-email: branko@monwara.com
 Maintainer: Nephila
 Maintainer-email: info@nephila.digital
 License: BSD
 Project-URL: Documentation, https://django-meta.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ===========
 django-meta
@@ -52,22 +51,22 @@
 Supported versions
 ******************
 
 ******
 Django
 ******
 
-2.2 to 4.0 (newer versions might work but are not tested yet)
+3.2 to 4.2 (newer versions might work but are not tested yet)
 
 
 ******
 Python
 ******
 
-Python 3.7 to 3.10
+Python 3.9 to 3.11
 
 *************
 Basic concept
 *************
 
 ``django-meta`` provides a **view-method** and **model-method** interface to provide and handle meta informations
 
@@ -138,14 +137,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+2.2.0 (2023-04-18)
+==================
+
+Features
+--------
+
+- Move to ruff (#138)
+- Add support for Django 4.2 (#144)
+
+
 2.1.0 (2022-07-28)
 ==================
 
 Bugfixes
 --------
 
 - Changes imports from ugettext_lazy to gettext_lazy to fix deprecation warning (#130)
```

### Comparing `django-meta-2.1.0/README.rst` & `django-meta-2.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 Supported versions
 ******************
 
 ******
 Django
 ******
 
-2.2 to 4.0 (newer versions might work but are not tested yet)
+3.2 to 4.2 (newer versions might work but are not tested yet)
 
 
 ******
 Python
 ******
 
-Python 3.7 to 3.10
+Python 3.9 to 3.11
 
 *************
 Basic concept
 *************
 
 ``django-meta`` provides a **view-method** and **model-method** interface to provide and handle meta informations
```

### Comparing `django-meta-2.1.0/django_meta.egg-info/PKG-INFO` & `django-meta-2.2.0/django_meta.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: django-meta
-Version: 2.1.0
+Version: 2.2.0
 Summary: Pluggable app for handling webpage meta tags and OpenGraph properties
 Home-page: https://github.com/nephila/django-meta
 Author: Monwara LLC
 Author-email: branko@monwara.com
 Maintainer: Nephila
 Maintainer-email: info@nephila.digital
 License: BSD
 Project-URL: Documentation, https://django-meta.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ===========
 django-meta
@@ -52,22 +51,22 @@
 Supported versions
 ******************
 
 ******
 Django
 ******
 
-2.2 to 4.0 (newer versions might work but are not tested yet)
+3.2 to 4.2 (newer versions might work but are not tested yet)
 
 
 ******
 Python
 ******
 
-Python 3.7 to 3.10
+Python 3.9 to 3.11
 
 *************
 Basic concept
 *************
 
 ``django-meta`` provides a **view-method** and **model-method** interface to provide and handle meta informations
 
@@ -138,14 +137,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+2.2.0 (2023-04-18)
+==================
+
+Features
+--------
+
+- Move to ruff (#138)
+- Add support for Django 4.2 (#144)
+
+
 2.1.0 (2022-07-28)
 ==================
 
 Bugfixes
 --------
 
 - Changes imports from ugettext_lazy to gettext_lazy to fix deprecation warning (#130)
```

### Comparing `django-meta-2.1.0/django_meta.egg-info/SOURCES.txt` & `django-meta-2.2.0/django_meta.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -31,8 +31,13 @@
 meta/locale/tr/LC_MESSAGES/django.po
 meta/templates/meta.html
 meta/templates/meta/meta.html
 meta/templates/meta_mixin/meta.html
 meta/templatetags/__init__.py
 meta/templatetags/meta.py
 meta/templatetags/meta_extra.py
-meta_mixin/__init__.py
+meta_mixin/__init__.py
+tests/test_asgi.py
+tests/test_meta.py
+tests/test_metadata_mixin.py
+tests/test_mixin.py
+tests/test_templatetags.py
```

### Comparing `django-meta-2.1.0/meta/locale/ar/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/de/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/en/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/es/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/it/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/lt/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/nl/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/pt_BR/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/ru/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/locale/tr/LC_MESSAGES/django.po` & `django-meta-2.2.0/meta/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/models.py` & `django-meta-2.2.0/meta/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     def get_request(self):
         """
         Retrieve request from current instance
         """
         warnings.warn(
             "use meta.utils.get_request function, ModelMeta.get_request will be removed in version 3.0",
             PendingDeprecationWarning,
+            stacklevel=2,
         )
         return get_request()
 
     def get_author(self):
         """
         Retrieve the author object. This is meant to be overridden in the model
         to return the actual author instance (e.g.: the user object).
```

### Comparing `django-meta-2.1.0/meta/settings.py` & `django-meta-2.2.0/meta/settings.py`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/templates/meta/meta.html` & `django-meta-2.2.0/meta/templates/meta/meta.html`

 * *Files identical despite different names*

### Comparing `django-meta-2.1.0/meta/templatetags/meta.py` & `django-meta-2.2.0/meta/templatetags/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,33 +192,33 @@
 
 
 @register.simple_tag
 def googleplus_prop(name, value):
     """
     Legacy Google+ property
     """
-    warnings.warn("googleplus_prop will be removed in version 3.0", PendingDeprecationWarning)
+    warnings.warn("googleplus_prop will be removed in version 3.0", PendingDeprecationWarning, stacklevel=2)
     return schemaorg_prop(name, value)
 
 
 @register.simple_tag
 def googleplus_html_scope(value):
     """
     Legacy Google+ scope
     """
-    warnings.warn("googleplus_html_scope will be removed in version 3.0", PendingDeprecationWarning)
+    warnings.warn("googleplus_html_scope will be removed in version 3.0", PendingDeprecationWarning, stacklevel=2)
     return schemaorg_html_scope(value)
 
 
 @register.simple_tag
 def googleplus_scope(value):
     """
     Legacy Google+ scope
     """
-    warnings.warn("googleplus_scope will be removed in version 3.0", PendingDeprecationWarning)
+    warnings.warn("googleplus_scope will be removed in version 3.0", PendingDeprecationWarning, stacklevel=2)
     return schemaorg_html_scope(value)
 
 
 @register.simple_tag(takes_context=True)
 def meta_namespaces(context):
     """
     Include OG namespaces. To be used in the <head> tag.
@@ -259,9 +259,9 @@
 
 
 @register.simple_tag(takes_context=True)
 def meta_namespaces_gplus(context):
     """
     Legacy Google+ attributes.
     """
-    warnings.warn("meta_namespaces_gplus will be removed in version 3.0", PendingDeprecationWarning)
+    warnings.warn("meta_namespaces_gplus will be removed in version 3.0", PendingDeprecationWarning, stacklevel=2)
     return meta_namespaces_schemaorg(context)
```

### Comparing `django-meta-2.1.0/meta/views.py` & `django-meta-2.2.0/meta/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,24 +235,26 @@
         return self.twitter_site
 
     def get_meta_twitter_creator(self, context=None):
         return self.twitter_creator
 
     @property
     def twitter_card(self):
-        warnings.warn("twitter_card attribute will be removed in version 3.0", PendingDeprecationWarning)
+        warnings.warn("twitter_card attribute will be removed in version 3.0", PendingDeprecationWarning, stacklevel=2)
         return self.twitter_type
 
     @twitter_card.setter
     def twitter_card(self, value):
-        warnings.warn("twitter_card attribute will be removed in version 3.0", PendingDeprecationWarning)
+        warnings.warn("twitter_card attribute will be removed in version 3.0", PendingDeprecationWarning, stacklevel=2)
         self.twitter_type = value
 
     def get_meta_twitter_card(self, context=None):
-        warnings.warn("get_meta_twitter_card attribute will be removed in version 3.0", PendingDeprecationWarning)
+        warnings.warn(
+            "get_meta_twitter_card attribute will be removed in version 3.0", PendingDeprecationWarning, stacklevel=2
+        )
         return self.twitter_type
 
     def get_meta_twitter_type(self, context=None):
         return self.twitter_type
 
     def get_meta_facebook_app_id(self, context=None):
         return self.facebook_app_id
```

### Comparing `django-meta-2.1.0/setup.cfg` & `django-meta-2.2.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-[bumpversion]
-current_version = 2.1.0
-parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.?)(?P<release>[a-z]*)(?P<relver>\d*)
-serialize = 
-	{major}.{minor}.{patch}.{release}{relver}
-	{major}.{minor}.{patch}
-commit = True
-tag = True
-sign_tags = True
-tag_name = {new_version}
-message = Release {new_version}
-
-[bumpversion:part:release]
-optional_value = gamma
-values = 
-	dev
-	a
-	b
-	rc
-	gamma
-
-[bumpversion:file:meta/__init__.py]
-
 [metadata]
 name = django-meta
 version = attr: meta.__version__
 url = https://github.com/nephila/django-meta
 project_urls = 
 	Documentation = https://django-meta.readthedocs.io/
 author = Monwara LLC
@@ -35,48 +12,42 @@
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
-	Framework :: Django :: 2.2
-	Framework :: Django :: 3.0
-	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
-install_requires = 
-	six
 setup_requires = 
 	setuptools
 packages = meta
 python_requires = >=3.7
 test_suite = cms_helper.run
 zip_safe = False
 
 [options.package_data]
 * = *.txt, *.rst
 meta = *.html *.png *.gif *js *jpg *jpeg *svg *py *mo *po
 
 [options.extras_require]
 docs = 
-	django<4.0
-
-[upload]
-repository = https://upload.pypi.org/legacy/
+	django<5.0
 
 [sdist]
 formats = zip
 
 [bdist_wheel]
 universal = 1
```

