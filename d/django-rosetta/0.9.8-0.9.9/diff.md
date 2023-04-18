# Comparing `tmp/django-rosetta-0.9.8.tar.gz` & `tmp/django-rosetta-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rosetta-0.9.8.tar", last modified: Wed Dec  8 08:49:00 2021, max compression
+gzip compressed data, was "django-rosetta-0.9.9.tar", last modified: Tue Apr 18 13:37:56 2023, max compression
```

## Comparing `django-rosetta-0.9.8.tar` & `django-rosetta-0.9.9.tar`

### file list

```diff
@@ -1,177 +1,183 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/
--rw-r--r--   0 marco     (1000) marco     (1000)     1080 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)      505 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/MANIFEST.in
--rw-rw-r--   0 marco     (1000) marco     (1000)     2577 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     1449 2021-04-12 11:22:37.000000 django-rosetta-0.9.8/README.rst
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/django_rosetta.egg-info/
--rw-rw-r--   0 marco     (1000) marco     (1000)     2577 2021-12-08 08:49:00.000000 django-rosetta-0.9.8/django_rosetta.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     3595 2021-12-08 08:49:00.000000 django-rosetta-0.9.8/django_rosetta.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2021-12-08 08:49:00.000000 django-rosetta-0.9.8/django_rosetta.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2021-03-19 14:34:32.000000 django-rosetta-0.9.8/django_rosetta.egg-info/not-zip-safe
--rw-rw-r--   0 marco     (1000) marco     (1000)       41 2021-12-08 08:49:00.000000 django-rosetta-0.9.8/django_rosetta.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        8 2021-12-08 08:49:00.000000 django-rosetta-0.9.8/django_rosetta.egg-info/top_level.txt
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/docs/
--rw-r--r--   0 marco     (1000) marco     (1000)     7437 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/docs/Makefile
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/docs/_static/
--rw-r--r--   0 marco     (1000) marco     (1000)    82082 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/docs/_static/rosetta-1.png
--rw-r--r--   0 marco     (1000) marco     (1000)    81407 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/docs/_static/rosetta-2.1.png
--rw-rw-r--   0 marco     (1000) marco     (1000)    11507 2021-12-08 08:17:44.000000 django-rosetta-0.9.8/docs/changes.rst
--rw-r--r--   0 marco     (1000) marco     (1000)     9551 2021-01-11 09:57:45.000000 django-rosetta-0.9.8/docs/conf.py
--rw-r--r--   0 marco     (1000) marco     (1000)      729 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/docs/index.rst
--rw-r--r--   0 marco     (1000) marco     (1000)     1160 2021-01-11 10:05:19.000000 django-rosetta-0.9.8/docs/installation.rst
--rw-rw-r--   0 marco     (1000) marco     (1000)     7016 2021-06-17 07:48:38.000000 django-rosetta-0.9.8/docs/settings.rst
--rw-r--r--   0 marco     (1000) marco     (1000)     2239 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/docs/usage.rst
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/
--rw-rw-r--   0 marco     (1000) marco     (1000)      313 2021-12-08 08:17:55.000000 django-rosetta-0.9.8/rosetta/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2502 2020-06-07 14:43:25.000000 django-rosetta-0.9.8/rosetta/access.py
--rw-r--r--   0 marco     (1000) marco     (1000)      320 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/apps.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/conf/
--rw-rw-r--   0 marco     (1000) marco     (1000)     4382 2021-06-17 07:48:38.000000 django-rosetta-0.9.8/rosetta/conf/__init__.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/ar/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 marco     (1000) marco     (1000)     4315 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 marco     (1000) marco     (1000)     6406 2021-05-13 11:47:18.000000 django-rosetta-0.9.8/rosetta/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/cs/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/cs/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     3243 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     5632 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/de/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/de/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     2698 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     5497 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/es/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/es/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     4186 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     6737 2020-03-22 17:29:13.000000 django-rosetta-0.9.8/rosetta/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/fa/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/fa/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     4535 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     6515 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/fr/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/fr/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     3399 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     5763 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/hu/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/hu/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     2133 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     5084 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/it/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/it/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     3055 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     5578 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/ky/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/rosetta/locale/ky/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     4235 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/ky/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     6244 2020-06-07 13:15:46.000000 django-rosetta-0.9.8/rosetta/locale/ky/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/nl/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/locale/nl/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     2292 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     5273 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/pl/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/locale/pl/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     4052 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     6170 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/ru/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/locale/ru/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     2091 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     5459 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/tr/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 marco     (1000) marco     (1000)     4148 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 marco     (1000) marco     (1000)     6388 2021-03-04 12:31:27.000000 django-rosetta-0.9.8/rosetta/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/uk/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/locale/uk/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     4680 2021-08-19 06:50:03.000000 django-rosetta-0.9.8/rosetta/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)     6887 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/locale/xx/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/locale/xx/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)      473 2021-12-08 08:46:16.000000 django-rosetta-0.9.8/rosetta/locale/xx/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)      835 2021-12-08 08:46:18.000000 django-rosetta-0.9.8/rosetta/locale/xx/LC_MESSAGES/django.po
--rw-r--r--   0 marco     (1000) marco     (1000)     5995 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/poutil.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      221 2021-01-11 09:56:09.000000 django-rosetta-0.9.8/rosetta/signals.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/static/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/static/admin/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/static/admin/img/
--rw-r--r--   0 marco     (1000) marco     (1000)      667 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/static/admin/img/icon_searchbox_rosetta.png
--rw-rw-r--   0 marco     (1000) marco     (1000)     4395 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/rosetta/storage.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/templates/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/templates/rosetta/
--rw-rw-r--   0 marco     (1000) marco     (1000)      734 2021-01-11 09:50:45.000000 django-rosetta-0.9.8/rosetta/templates/rosetta/admin_index.html
--rw-rw-r--   0 marco     (1000) marco     (1000)     1498 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/rosetta/templates/rosetta/base.html
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/templates/rosetta/css/
--rw-rw-r--   0 marco     (1000) marco     (1000)     2052 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/rosetta/templates/rosetta/css/rosetta.css
--rw-r--r--   0 marco     (1000) marco     (1000)     3817 2020-06-07 15:03:22.000000 django-rosetta-0.9.8/rosetta/templates/rosetta/file-list.html
--rw-rw-r--   0 marco     (1000) marco     (1000)     9975 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/rosetta/templates/rosetta/form.html
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/templates/rosetta/js/
--rw-rw-r--   0 marco     (1000) marco     (1000)     6334 2021-06-17 07:48:38.000000 django-rosetta-0.9.8/rosetta/templates/rosetta/js/rosetta.js
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/templatetags/
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/templatetags/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1725 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/rosetta/templatetags/rosetta.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/tests/
--rw-r--r--   0 marco     (1000) marco     (1000)       29 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)      914 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue186.template
--rw-r--r--   0 marco     (1000) marco     (1000)     1217 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue24gh.template
--rw-r--r--   0 marco     (1000) marco     (1000)      731 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue34gh.template
--rw-r--r--   0 marco     (1000) marco     (1000)    21234 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue38gh.template
--rw-r--r--   0 marco     (1000) marco     (1000)      756 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue39gh.template
--rw-r--r--   0 marco     (1000) marco     (1000)      842 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue60.template
--rw-r--r--   0 marco     (1000) marco     (1000)      759 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue67.template
--rw-r--r--   0 marco     (1000) marco     (1000)      659 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.issue79.template
--rw-r--r--   0 marco     (1000) marco     (1000)      824 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.template
--rw-r--r--   0 marco     (1000) marco     (1000)     2155 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/django.po.test44.template
--rw-r--r--   0 marco     (1000) marco     (1000)      658 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/pr44.po.template
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/tests/test_app/
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/test_app/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)      142 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/test_app/apps.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/tests/test_app/locale/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/rosetta/tests/test_app/locale/xx/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/rosetta/tests/test_app/locale/xx/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)      555 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.mo
--rw-r--r--   0 marco     (1000) marco     (1000)      995 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.po
--rw-rw-r--   0 marco     (1000) marco     (1000)    44468 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/rosetta/tests/tests.py
--rw-r--r--   0 marco     (1000) marco     (1000)      182 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/urls.py
--rw-r--r--   0 marco     (1000) marco     (1000)       29 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/rosetta/tests/views.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     4624 2021-03-04 14:03:44.000000 django-rosetta-0.9.8/rosetta/translate_utils.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1205 2021-11-09 16:12:32.000000 django-rosetta-0.9.8/rosetta/urls.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    29017 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/rosetta/views.py
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)     2269 2021-12-08 08:37:28.000000 django-rosetta-0.9.8/setup.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/testproject/
--rw-r--r--   0 marco     (1000) marco     (1000)      121 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/.coveragerc
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)      106 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/coverage.sh
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/testproject/fixtures/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/testproject/fixtures/vcr_cassettes/
--rw-rw-r--   0 marco     (1000) marco     (1000)      912 2021-03-04 13:55:52.000000 django-rosetta-0.9.8/testproject/fixtures/vcr_cassettes/test_47_azure_ajax_translation.yaml
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/testproject/locale/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/testproject/locale/bs-Cyrl-BA/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/testproject/locale/bs-Cyrl-BA/LC_MESSAGES/
--rw-rw-r--   0 marco     (1000) marco     (1000)      889 2021-03-04 12:27:57.000000 django-rosetta-0.9.8/testproject/locale/bs-Cyrl-BA/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/testproject/locale/fr/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/testproject/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 marco     (1000) marco     (1000)      633 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/testproject/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 marco     (1000) marco     (1000)     1367 2021-08-19 06:43:58.000000 django-rosetta-0.9.8/testproject/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/testproject/locale/fr_FR.utf8/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.312722 django-rosetta-0.9.8/testproject/locale/fr_FR.utf8/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     1083 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/locale/fr_FR.utf8/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/testproject/locale/xx/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/testproject/locale/xx/LC_MESSAGES/
--rw-rw-r--   0 marco     (1000) marco     (1000)     2130 2021-03-04 12:27:57.000000 django-rosetta-0.9.8/testproject/locale/xx/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/testproject/locale/yy/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/testproject/locale/yy/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)     1067 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/locale/yy/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.304722 django-rosetta-0.9.8/testproject/locale/yy-Anot/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/testproject/locale/yy-Anot/LC_MESSAGES/
--rw-r--r--   0 marco     (1000) marco     (1000)      889 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/locale/yy-Anot/LC_MESSAGES/django.po
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.308722 django-rosetta-0.9.8/testproject/locale/zh_Hans/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/testproject/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 marco     (1000) marco     (1000)      455 2021-03-04 14:43:33.000000 django-rosetta-0.9.8/testproject/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-r--   0 marco     (1000) marco     (1000)      889 2021-03-04 14:52:45.000000 django-rosetta-0.9.8/testproject/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 marco     (1000) marco     (1000)      378 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/manage.py
--rw-r--r--   0 marco     (1000) marco     (1000)   147456 2021-06-17 07:41:49.000000 django-rosetta-0.9.8/testproject/rosetta.db
--rw-rw-r--   0 marco     (1000) marco     (1000)     4172 2021-06-17 07:48:38.000000 django-rosetta-0.9.8/testproject/settings.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-12-08 08:49:00.316722 django-rosetta-0.9.8/testproject/templates/
--rw-r--r--   0 marco     (1000) marco     (1000)      179 2019-06-20 07:32:02.000000 django-rosetta-0.9.8/testproject/templates/test.html
--rw-rw-r--   0 marco     (1000) marco     (1000)      319 2021-11-09 16:12:32.000000 django-rosetta-0.9.8/testproject/urls.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2396 2021-12-08 08:22:16.000000 django-rosetta-0.9.8/tox.ini
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.681684 django-rosetta-0.9.9/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1080 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)      505 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/MANIFEST.in
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2627 2023-04-18 13:37:56.681684 django-rosetta-0.9.9/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1519 2022-05-18 08:56:26.000000 django-rosetta-0.9.9/README.rst
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.665684 django-rosetta-0.9.9/django_rosetta.egg-info/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2627 2023-04-18 13:37:56.000000 django-rosetta-0.9.9/django_rosetta.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3773 2023-04-18 13:37:56.000000 django-rosetta-0.9.9/django_rosetta.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2023-04-18 13:37:56.000000 django-rosetta-0.9.9/django_rosetta.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2021-03-19 14:34:32.000000 django-rosetta-0.9.9/django_rosetta.egg-info/not-zip-safe
+-rw-rw-r--   0 marco     (1000) marco     (1000)       41 2023-04-18 13:37:56.000000 django-rosetta-0.9.9/django_rosetta.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        8 2023-04-18 13:37:56.000000 django-rosetta-0.9.9/django_rosetta.egg-info/top_level.txt
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.665684 django-rosetta-0.9.9/docs/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7437 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/docs/Makefile
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.665684 django-rosetta-0.9.9/docs/_static/
+-rw-r--r--   0 marco     (1000) marco     (1000)    82082 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/docs/_static/rosetta-1.png
+-rw-r--r--   0 marco     (1000) marco     (1000)    81407 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/docs/_static/rosetta-2.1.png
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12134 2023-04-18 13:33:46.000000 django-rosetta-0.9.9/docs/changes.rst
+-rw-rw-r--   0 marco     (1000) marco     (1000)     9520 2023-04-18 13:35:41.000000 django-rosetta-0.9.9/docs/conf.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      729 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/docs/index.rst
+-rw-r--r--   0 marco     (1000) marco     (1000)     1160 2021-01-11 10:05:19.000000 django-rosetta-0.9.9/docs/installation.rst
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7254 2023-04-18 13:25:10.000000 django-rosetta-0.9.9/docs/settings.rst
+-rw-r--r--   0 marco     (1000) marco     (1000)     2239 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/docs/usage.rst
+-rw-rw-r--   0 marco     (1000) marco     (1000)      766 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/pyproject.toml
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      313 2022-01-06 15:56:08.000000 django-rosetta-0.9.9/rosetta/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2658 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/access.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      320 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/apps.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/conf/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4542 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/conf/__init__.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/locale/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/ar/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4315 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)     6406 2021-05-13 11:47:18.000000 django-rosetta-0.9.9/rosetta/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/cs/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     3243 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     5632 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/de/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/de/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2698 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     5497 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/es/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/es/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4186 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     6737 2020-03-22 17:29:13.000000 django-rosetta-0.9.9/rosetta/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/fa/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4535 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)     6514 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/fr/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     3399 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     5763 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/hu/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2133 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     5084 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/it/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/it/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     3055 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     5578 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/ky/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/ky/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4235 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)     6242 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/nl/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2292 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     5273 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/pl/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4052 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)     6169 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/ru/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.669684 django-rosetta-0.9.9/rosetta/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2091 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     5459 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.657684 django-rosetta-0.9.9/rosetta/locale/tr/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4148 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)     6388 2021-03-04 12:31:27.000000 django-rosetta-0.9.9/rosetta/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/locale/uk/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4680 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)     6887 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/locale/xx/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/locale/xx/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)      416 2023-04-18 13:22:01.000000 django-rosetta-0.9.9/rosetta/locale/xx/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)      831 2023-04-18 13:22:22.000000 django-rosetta-0.9.9/rosetta/locale/xx/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/locale/zh_hans/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/locale/zh_hans/LC_MESSAGES/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2673 2022-05-18 08:44:34.000000 django-rosetta-0.9.9/rosetta/locale/zh_hans/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5791 2022-01-06 16:17:48.000000 django-rosetta-0.9.9/rosetta/locale/zh_hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 marco     (1000) marco     (1000)     6661 2023-04-18 13:25:10.000000 django-rosetta-0.9.9/rosetta/poutil.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      221 2021-01-11 09:56:09.000000 django-rosetta-0.9.9/rosetta/signals.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/static/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/static/admin/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/static/admin/img/
+-rw-r--r--   0 marco     (1000) marco     (1000)      667 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/static/admin/img/icon_searchbox_rosetta.png
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4396 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/storage.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/templates/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/templates/rosetta/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      734 2021-01-11 09:50:45.000000 django-rosetta-0.9.9/rosetta/templates/rosetta/admin_index.html
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1511 2023-04-18 13:08:20.000000 django-rosetta-0.9.9/rosetta/templates/rosetta/base.html
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/templates/rosetta/css/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2052 2021-08-19 06:43:58.000000 django-rosetta-0.9.9/rosetta/templates/rosetta/css/rosetta.css
+-rw-r--r--   0 marco     (1000) marco     (1000)     3817 2020-06-07 15:03:22.000000 django-rosetta-0.9.9/rosetta/templates/rosetta/file-list.html
+-rw-rw-r--   0 marco     (1000) marco     (1000)     9975 2023-04-18 12:55:45.000000 django-rosetta-0.9.9/rosetta/templates/rosetta/form.html
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/templates/rosetta/js/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4818 2023-04-18 13:08:20.000000 django-rosetta-0.9.9/rosetta/templates/rosetta/js/rosetta.js
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.673684 django-rosetta-0.9.9/rosetta/templatetags/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/templatetags/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1727 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/templatetags/rosetta.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/rosetta/tests/
+-rw-r--r--   0 marco     (1000) marco     (1000)       29 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/tests/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      913 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue186.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1216 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue24gh.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)      730 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue34gh.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)    21230 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue38gh.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)      755 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue39gh.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)      837 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue60.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)      756 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue67.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)      655 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.issue79.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)      819 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/django.po.template
+-rw-r--r--   0 marco     (1000) marco     (1000)     2155 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/tests/django.po.test44.template
+-rw-rw-r--   0 marco     (1000) marco     (1000)      655 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/pr44.po.template
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/rosetta/tests/test_app/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/tests/test_app/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      142 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/test_app/apps.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/tests/test_app/locale/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/rosetta/tests/test_app/locale/xx/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/rosetta/tests/test_app/locale/xx/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)      555 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.mo
+-rw-r--r--   0 marco     (1000) marco     (1000)      995 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.po
+-rw-rw-r--   0 marco     (1000) marco     (1000)    44588 2023-04-18 13:25:10.000000 django-rosetta-0.9.9/rosetta/tests/tests.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      185 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/tests/urls.py
+-rw-r--r--   0 marco     (1000) marco     (1000)       29 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/rosetta/tests/views.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5519 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/translate_utils.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1208 2023-04-18 13:25:10.000000 django-rosetta-0.9.9/rosetta/urls.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    28775 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/rosetta/views.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2023-04-18 13:37:56.681684 django-rosetta-0.9.9/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2269 2021-12-08 08:37:28.000000 django-rosetta-0.9.9/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/
+-rw-r--r--   0 marco     (1000) marco     (1000)      121 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/testproject/.coveragerc
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/testproject/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      106 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/testproject/coverage.sh
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/fixtures/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/fixtures/vcr_cassettes/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      886 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/testproject/fixtures/vcr_cassettes/test_47_2_deeps_ajax_translation.yaml
+-rw-rw-r--   0 marco     (1000) marco     (1000)      912 2021-03-04 13:55:52.000000 django-rosetta-0.9.9/testproject/fixtures/vcr_cassettes/test_47_azure_ajax_translation.yaml
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/bs-Cyrl-BA/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/locale/bs-Cyrl-BA/LC_MESSAGES/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      889 2021-03-04 12:27:57.000000 django-rosetta-0.9.9/testproject/locale/bs-Cyrl-BA/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/fr/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      633 2021-08-19 06:43:58.000000 django-rosetta-0.9.9/testproject/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1367 2021-08-19 06:43:58.000000 django-rosetta-0.9.9/testproject/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/fr_FR.utf8/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/locale/fr_FR.utf8/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1083 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/testproject/locale/fr_FR.utf8/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/xx/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/locale/xx/LC_MESSAGES/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2130 2021-03-04 12:27:57.000000 django-rosetta-0.9.9/testproject/locale/xx/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/yy/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/locale/yy/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1067 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/testproject/locale/yy/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/yy-Anot/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/locale/yy-Anot/LC_MESSAGES/
+-rw-r--r--   0 marco     (1000) marco     (1000)      889 2019-06-20 07:32:02.000000 django-rosetta-0.9.9/testproject/locale/yy-Anot/LC_MESSAGES/django.po
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.661684 django-rosetta-0.9.9/testproject/locale/zh_Hans/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.677684 django-rosetta-0.9.9/testproject/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      455 2021-03-04 14:43:33.000000 django-rosetta-0.9.9/testproject/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-r--   0 marco     (1000) marco     (1000)      889 2021-03-04 14:52:45.000000 django-rosetta-0.9.9/testproject/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 marco     (1000) marco     (1000)      381 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/testproject/manage.py
+-rw-r--r--   0 marco     (1000) marco     (1000)   147456 2023-04-18 12:33:17.000000 django-rosetta-0.9.9/testproject/rosetta.db
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4166 2023-04-18 13:06:22.000000 django-rosetta-0.9.9/testproject/settings.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 13:37:56.681684 django-rosetta-0.9.9/testproject/templates/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      180 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/testproject/templates/test.html
+-rw-rw-r--   0 marco     (1000) marco     (1000)      320 2023-01-17 14:44:21.000000 django-rosetta-0.9.9/testproject/urls.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2168 2023-01-17 14:45:44.000000 django-rosetta-0.9.9/tox.ini
```

### Comparing `django-rosetta-0.9.8/LICENSE` & `django-rosetta-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/PKG-INFO` & `django-rosetta-0.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-rosetta
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Django application that eases the translation of Django projects
 Home-page: https://github.com/mbi/django-rosetta
 Author: Marco Bonetti
 Author-email: mbonetti@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Localization
@@ -41,15 +40,15 @@
   :target: https://github.com/mbi/django-rosetta/blob/develop/LICENSE
 
 
 Rosetta is a `Django <http://www.djangoproject.com/>`_ application that facilitates the translation process of your Django projects.
 
 Because it doesn't export any models, Rosetta doesn't create any tables in your project's database. Rosetta can be installed and uninstalled by simply adding and removing a single entry in your project's `INSTALLED_APPS` and a single line in your main ``urls.py`` file.
 
-Note: as of version 0.9.0, django-rosetta requires Django 1.11 or later, as of version 0.9.6, django-rosetta requires Django 2.2 or later
+Note: as of version 0.9.0, django-rosetta requires Django 1.11 or later, as of version 0.9.6, django-rosetta requires Django 2.2 or later, and as of version 0.9.9 django-rosetta supports Django 3.2 or later.
 
 ********
 Features
 ********
 
 * Reads and writes your project's `gettext` catalogs (po and mo files)
 * Installed and uninstalled in under a minute
@@ -59,9 +58,7 @@
 
 
 *************
 Documentation
 *************
 
 Please refer to the `online documentation <http://django-rosetta.readthedocs.org/>`_ to install Rosetta and get started.
-
-
```

### Comparing `django-rosetta-0.9.8/README.rst` & `django-rosetta-0.9.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   :target: https://github.com/mbi/django-rosetta/blob/develop/LICENSE
 
 
 Rosetta is a `Django <http://www.djangoproject.com/>`_ application that facilitates the translation process of your Django projects.
 
 Because it doesn't export any models, Rosetta doesn't create any tables in your project's database. Rosetta can be installed and uninstalled by simply adding and removing a single entry in your project's `INSTALLED_APPS` and a single line in your main ``urls.py`` file.
 
-Note: as of version 0.9.0, django-rosetta requires Django 1.11 or later, as of version 0.9.6, django-rosetta requires Django 2.2 or later
+Note: as of version 0.9.0, django-rosetta requires Django 1.11 or later, as of version 0.9.6, django-rosetta requires Django 2.2 or later, and as of version 0.9.9 django-rosetta supports Django 3.2 or later.
 
 ********
 Features
 ********
 
 * Reads and writes your project's `gettext` catalogs (po and mo files)
 * Installed and uninstalled in under a minute
```

### Comparing `django-rosetta-0.9.8/django_rosetta.egg-info/PKG-INFO` & `django-rosetta-0.9.9/django_rosetta.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-rosetta
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Django application that eases the translation of Django projects
 Home-page: https://github.com/mbi/django-rosetta
 Author: Marco Bonetti
 Author-email: mbonetti@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Localization
@@ -41,15 +40,15 @@
   :target: https://github.com/mbi/django-rosetta/blob/develop/LICENSE
 
 
 Rosetta is a `Django <http://www.djangoproject.com/>`_ application that facilitates the translation process of your Django projects.
 
 Because it doesn't export any models, Rosetta doesn't create any tables in your project's database. Rosetta can be installed and uninstalled by simply adding and removing a single entry in your project's `INSTALLED_APPS` and a single line in your main ``urls.py`` file.
 
-Note: as of version 0.9.0, django-rosetta requires Django 1.11 or later, as of version 0.9.6, django-rosetta requires Django 2.2 or later
+Note: as of version 0.9.0, django-rosetta requires Django 1.11 or later, as of version 0.9.6, django-rosetta requires Django 2.2 or later, and as of version 0.9.9 django-rosetta supports Django 3.2 or later.
 
 ********
 Features
 ********
 
 * Reads and writes your project's `gettext` catalogs (po and mo files)
 * Installed and uninstalled in under a minute
@@ -59,9 +58,7 @@
 
 
 *************
 Documentation
 *************
 
 Please refer to the `online documentation <http://django-rosetta.readthedocs.org/>`_ to install Rosetta and get started.
-
-
```

### Comparing `django-rosetta-0.9.8/django_rosetta.egg-info/SOURCES.txt` & `django-rosetta-0.9.9/django_rosetta.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tox.ini
 django_rosetta.egg-info/PKG-INFO
 django_rosetta.egg-info/SOURCES.txt
 django_rosetta.egg-info/dependency_links.txt
 django_rosetta.egg-info/not-zip-safe
 django_rosetta.egg-info/requires.txt
@@ -54,14 +55,16 @@
 rosetta/locale/ru/LC_MESSAGES/django.po
 rosetta/locale/tr/LC_MESSAGES/django.mo
 rosetta/locale/tr/LC_MESSAGES/django.po
 rosetta/locale/uk/LC_MESSAGES/django.mo
 rosetta/locale/uk/LC_MESSAGES/django.po
 rosetta/locale/xx/LC_MESSAGES/django.mo
 rosetta/locale/xx/LC_MESSAGES/django.po
+rosetta/locale/zh_hans/LC_MESSAGES/django.mo
+rosetta/locale/zh_hans/LC_MESSAGES/django.po
 rosetta/static/admin/img/icon_searchbox_rosetta.png
 rosetta/templates/rosetta/admin_index.html
 rosetta/templates/rosetta/base.html
 rosetta/templates/rosetta/file-list.html
 rosetta/templates/rosetta/form.html
 rosetta/templates/rosetta/css/rosetta.css
 rosetta/templates/rosetta/js/rosetta.js
@@ -89,14 +92,15 @@
 testproject/.coveragerc
 testproject/__init__.py
 testproject/coverage.sh
 testproject/manage.py
 testproject/rosetta.db
 testproject/settings.py
 testproject/urls.py
+testproject/fixtures/vcr_cassettes/test_47_2_deeps_ajax_translation.yaml
 testproject/fixtures/vcr_cassettes/test_47_azure_ajax_translation.yaml
 testproject/locale/bs-Cyrl-BA/LC_MESSAGES/django.po
 testproject/locale/fr/LC_MESSAGES/django.mo
 testproject/locale/fr/LC_MESSAGES/django.po
 testproject/locale/fr_FR.utf8/LC_MESSAGES/django.po
 testproject/locale/xx/LC_MESSAGES/django.po
 testproject/locale/yy-Anot/LC_MESSAGES/django.po
```

### Comparing `django-rosetta-0.9.8/docs/Makefile` & `django-rosetta-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/docs/_static/rosetta-1.png` & `django-rosetta-0.9.9/docs/_static/rosetta-1.png`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/docs/_static/rosetta-2.1.png` & `django-rosetta-0.9.9/docs/_static/rosetta-2.1.png`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/docs/changes.rst` & `django-rosetta-0.9.9/docs/changes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Version History
 ===============
 
+Version 0.9.9
+-------------
+* Use packaged jQuery instead of the CDN version. (#274, thanks @stephanema1)
+* Test test_47_azure_ajax_translation: avoid DNS lookup for better isolation. Should fix #233
+* Adds Chinese (Simplified) translation. (#266 thanks @chenluyong)
+* Test against Django 4.1 and 4.2
+* Limit supported versions to Django 3.2 and later, using Python 3.8, 3.9 and 3.10
+* Proxy Deepl translations suggestions through the back-end to avoid CORS issues. (#271 thanks @rafaelromon, @biermeester and @matthiask)
+* Format code with pre-commit
+* Replace case sensitivity check with setting (#273 thanks @patroqueeet)
+
+
 Version 0.9.8
 -------------
 * Test against Django 4.0
 
 
 Version 0.9.7
 -------------
```

### Comparing `django-rosetta-0.9.8/docs/conf.py` & `django-rosetta-0.9.9/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Django Rosetta documentation build configuration file, created by
 # sphinx-quickstart on Thu Apr  2 15:19:37 2015.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
@@ -21,15 +20,15 @@
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 
 
 def get_version():
-    sys.path.insert(0, os.path.abspath('..'))
+    sys.path.insert(0, os.path.abspath(".."))
     from rosetta import get_version as get_version_
 
     return get_version_()
 
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
@@ -42,31 +41,31 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = []
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Django Rosetta'
-copyright = u'2008 – 2021 Marco Bonetti and contributors'
-author = u'Marco Bonetti'
+project = "Django Rosetta"
+copyright = "2008 – 2023 Marco Bonetti and contributors"
+author = "Marco Bonetti"
 
 
 version = get_version()
 # The full version, including alpha/beta/rc tags.
 release = get_version()
 
 # The language for content autogenerated by Sphinx. Refer to documentation
@@ -80,15 +79,15 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
@@ -98,15 +97,15 @@
 # add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
@@ -143,15 +142,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 # html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
@@ -206,15 +205,15 @@
 # html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
 # html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'DjangoRosettadoc'
+htmlhelp_basename = "DjangoRosettadoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
@@ -227,18 +226,18 @@
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     (
         master_doc,
-        'DjangoRosetta.tex',
-        u'Django Rosetta Documentation',
-        u'Marco Bonetti',
-        'manual',
+        "DjangoRosetta.tex",
+        "Django Rosetta Documentation",
+        "Marco Bonetti",
+        "manual",
     )
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
@@ -259,34 +258,34 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, 'djangorosetta', u'Django Rosetta Documentation', [author], 1)]
+man_pages = [(master_doc, "djangorosetta", "Django Rosetta Documentation", [author], 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
-        'DjangoRosetta',
-        u'Django Rosetta Documentation',
+        "DjangoRosetta",
+        "Django Rosetta Documentation",
         author,
-        'DjangoRosetta',
-        'One line description of project.',
-        'Miscellaneous',
+        "DjangoRosetta",
+        "One line description of project.",
+        "Miscellaneous",
     )
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
```

### Comparing `django-rosetta-0.9.8/docs/index.rst` & `django-rosetta-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/docs/installation.rst` & `django-rosetta-0.9.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/docs/settings.rst` & `django-rosetta-0.9.9/docs/settings.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 * ``ROSETTA_EXCLUDED_PATHS``: Exclude paths defined in this list from being searched (usually ends with "locale"). Defaults to ``()``
 * ``ROSETTA_AUTO_COMPILE``: Determines whether the MO file is automatically compiled when the PO file is saved. Defaults to ``True``.
 * ``ROSETTA_ENABLE_REFLANG``: Enables a selector for picking a reference language other than English. Defaults to ``False``.
 * ``ROSETTA_SHOW_AT_ADMIN_PANEL``: Adds a handy link to Rosetta at the bottom of the Django admin apps index. Defaults to ``False``.
 * ``ROSETTA_LOGIN_URL``: Use this if you want to override the login URL for rosetta. Defaults to ``settings.LOGIN_URL``.
 * ``ROSETTA_LANGUAGES``: List of languages that Rosetta will offer to translate. This is useful when you wish to translate a language that is not yet defined in ``settings.LANGUAGES``. Defaults to ``settings.LANGUAGES``.
 * ``ROSETTA_SHOW_OCCURRENCES``: Determines whether occurrences (where the original text appears) should be shown next to the translations for context. Defaults to ``True``.
+* ``ROSETTA_CASE_SENSITIVE_FILESYSTEM``: Overrides auto-detection of case sensitive OS. Defaults to ``None`` which enables auto-detection. Useful when running case sensitive OS (e.g. Ubuntu) in docker on case insensitive OS (e.g. MacOS).
 
 
 
 
 Storages
 --------
```

### Comparing `django-rosetta-0.9.8/docs/usage.rst` & `django-rosetta-0.9.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/access.py` & `django-rosetta-0.9.9/rosetta/access.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,53 +11,65 @@
 
 
 def get_access_control_function():
     """
     Return a predicate for determining if a user can
     access the Rosetta views
     """
-    access_function = getattr(settings, 'ROSETTA_ACCESS_CONTROL_FUNCTION', None)
+    access_function = getattr(settings, "ROSETTA_ACCESS_CONTROL_FUNCTION", None)
     if access_function is None:
         return is_superuser_staff_or_in_translators_group
     elif isinstance(access_function, str):
         # Dynamically load a permissions function
-        perm_module, perm_func = access_function.rsplit('.', 1)
+        perm_module, perm_func = access_function.rsplit(".", 1)
         perm_module = importlib.import_module(perm_module)
         return getattr(perm_module, perm_func)
     elif callable(access_function):
         return access_function
     else:
         raise TypeError(access_function)
 
 
 # Default access control test
 def is_superuser_staff_or_in_translators_group(user):
-    if not getattr(settings, 'ROSETTA_REQUIRES_AUTH', True):
+    if not getattr(settings, "ROSETTA_REQUIRES_AUTH", True):
         return True
     try:
         if not user.is_authenticated:
             return False
         elif user.is_superuser and user.is_staff:
             return True
         else:
-            return user.groups.filter(name='translators').exists()
+            return user.groups.filter(name="translators").exists()
     except AttributeError:
-        if not hasattr(user, 'is_authenticated') or not hasattr(user, 'is_superuser') or not hasattr(user, 'groups'):
-            raise ImproperlyConfigured('If you are using custom User Models you must implement a custom authentication method for Rosetta. See ROSETTA_ACCESS_CONTROL_FUNCTION here: https://django-rosetta.readthedocs.org/en/latest/settings.html')
+        if (
+            not hasattr(user, "is_authenticated")
+            or not hasattr(user, "is_superuser")
+            or not hasattr(user, "groups")
+        ):
+            raise ImproperlyConfigured(
+                "If you are using custom User Models you must implement a custom authentication method for Rosetta. See ROSETTA_ACCESS_CONTROL_FUNCTION here: https://django-rosetta.readthedocs.org/en/latest/settings.html"
+            )
         raise
 
 
 def can_translate_language(user, langid):
     try:
         if not rosetta_settings.ROSETTA_LANGUAGE_GROUPS:
             return can_translate(user)
         elif not user.is_authenticated:
             return False
         elif user.is_superuser and user.is_staff:
             return True
         else:
-            return user.groups.filter(name='translators-%s' % langid).exists()
+            return user.groups.filter(name="translators-%s" % langid).exists()
 
     except AttributeError:
-        if not hasattr(user, 'is_authenticated') or not hasattr(user, 'is_superuser') or not hasattr(user, 'groups'):
-            raise ImproperlyConfigured('If you are using custom User Models you must implement a custom authentication method for Rosetta. See ROSETTA_ACCESS_CONTROL_FUNCTION here: https://django-rosetta.readthedocs.org/en/latest/settings.html')
+        if (
+            not hasattr(user, "is_authenticated")
+            or not hasattr(user, "is_superuser")
+            or not hasattr(user, "groups")
+        ):
+            raise ImproperlyConfigured(
+                "If you are using custom User Models you must implement a custom authentication method for Rosetta. See ROSETTA_ACCESS_CONTROL_FUNCTION here: https://django-rosetta.readthedocs.org/en/latest/settings.html"
+            )
         raise
```

### Comparing `django-rosetta-0.9.8/rosetta/conf/__init__.py` & `django-rosetta-0.9.9/rosetta/conf/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,104 +2,116 @@
 For a description of each rosetta setting see: docs/settings.rst.
 """
 
 from django.conf import settings as dj_settings
 from django.core.signals import setting_changed
 
 
-__all__ = ['settings']
+__all__ = ["settings"]
 
 
 class RosettaSettings(object):
     """
     Class that holds rosetta settings.
 
     The settings object is an instance of this class and is reloaded when
     the ``setting_changed`` signal is dispatched.
     """
 
     SETTINGS = {
-        'ROSETTA_MESSAGES_PER_PAGE': ('MESSAGES_PER_PAGE', 10),
-        'ROSETTA_ENABLE_TRANSLATION_SUGGESTIONS': (
-            'ENABLE_TRANSLATION_SUGGESTIONS',
+        "ROSETTA_MESSAGES_PER_PAGE": ("MESSAGES_PER_PAGE", 10),
+        "ROSETTA_ENABLE_TRANSLATION_SUGGESTIONS": (
+            "ENABLE_TRANSLATION_SUGGESTIONS",
             False,
         ),
-        'YANDEX_TRANSLATE_KEY': ('YANDEX_TRANSLATE_KEY', None),
-        'AZURE_CLIENT_SECRET': ('AZURE_CLIENT_SECRET', None),
-        'GOOGLE_APPLICATION_CREDENTIALS_PATH': (
-            'GOOGLE_APPLICATION_CREDENTIALS_PATH',
+        "YANDEX_TRANSLATE_KEY": ("YANDEX_TRANSLATE_KEY", None),
+        "AZURE_CLIENT_SECRET": ("AZURE_CLIENT_SECRET", None),
+        "GOOGLE_APPLICATION_CREDENTIALS_PATH": (
+            "GOOGLE_APPLICATION_CREDENTIALS_PATH",
             None,
         ),
-        'GOOGLE_PROJECT_ID': ('GOOGLE_PROJECT_ID', None),
-        'DEEPL_AUTH_KEY': ('DEEPL_AUTH_KEY', None),
-        'ROSETTA_MAIN_LANGUAGE': ('MAIN_LANGUAGE', None),
-        'ROSETTA_MESSAGES_SOURCE_LANGUAGE_CODE': ('MESSAGES_SOURCE_LANGUAGE_CODE', 'en'),
-        'ROSETTA_MESSAGES_SOURCE_LANGUAGE_NAME': (
-            'MESSAGES_SOURCE_LANGUAGE_NAME',
-            'English',
-        ),
-        'ROSETTA_ACCESS_CONTROL_FUNCTION': ('ACCESS_CONTROL_FUNCTION', None),
-        'ROSETTA_WSGI_AUTO_RELOAD': ('WSGI_AUTO_RELOAD', False),
-        'ROSETTA_UWSGI_AUTO_RELOAD': ('UWSGI_AUTO_RELOAD', False),
-        'ROSETTA_EXCLUDED_APPLICATIONS': ('EXCLUDED_APPLICATIONS', ()),
-        'ROSETTA_POFILE_WRAP_WIDTH': ('POFILE_WRAP_WIDTH', 78),
-        'ROSETTA_STORAGE_CLASS': ('STORAGE_CLASS', 'rosetta.storage.CacheRosettaStorage'),
-        'ROSETTA_ENABLE_REFLANG': ('ENABLE_REFLANG', False),
-        'ROSETTA_POFILENAMES': ('POFILENAMES', ('django.po', 'djangojs.po')),
-        'ROSETTA_CACHE_NAME': (
-            'ROSETTA_CACHE_NAME',
-            'rosetta' if 'rosetta' in dj_settings.CACHES else 'default',
-        ),
-        'ROSETTA_REQUIRES_AUTH': ('ROSETTA_REQUIRES_AUTH', True),
-        'ROSETTA_EXCLUDED_PATHS': ('ROSETTA_EXCLUDED_PATHS', ()),
-        'ROSETTA_LANGUAGE_GROUPS': ('ROSETTA_LANGUAGE_GROUPS', False),
-        'ROSETTA_AUTO_COMPILE': ('AUTO_COMPILE', True),
-        'ROSETTA_SHOW_AT_ADMIN_PANEL': ('SHOW_AT_ADMIN_PANEL', False),
-        'ROSETTA_LOGIN_URL': ('LOGIN_URL', dj_settings.LOGIN_URL),
-        'ROSETTA_LANGUAGES': ('ROSETTA_LANGUAGES', dj_settings.LANGUAGES),
-        'ROSETTA_SHOW_OCCURRENCES': ('SHOW_OCCURRENCES', True),
+        "GOOGLE_PROJECT_ID": ("GOOGLE_PROJECT_ID", None),
+        "DEEPL_AUTH_KEY": ("DEEPL_AUTH_KEY", None),
+        "ROSETTA_MAIN_LANGUAGE": ("MAIN_LANGUAGE", None),
+        "ROSETTA_MESSAGES_SOURCE_LANGUAGE_CODE": (
+            "MESSAGES_SOURCE_LANGUAGE_CODE",
+            "en",
+        ),
+        "ROSETTA_MESSAGES_SOURCE_LANGUAGE_NAME": (
+            "MESSAGES_SOURCE_LANGUAGE_NAME",
+            "English",
+        ),
+        "ROSETTA_ACCESS_CONTROL_FUNCTION": ("ACCESS_CONTROL_FUNCTION", None),
+        "ROSETTA_WSGI_AUTO_RELOAD": ("WSGI_AUTO_RELOAD", False),
+        "ROSETTA_UWSGI_AUTO_RELOAD": ("UWSGI_AUTO_RELOAD", False),
+        "ROSETTA_EXCLUDED_APPLICATIONS": ("EXCLUDED_APPLICATIONS", ()),
+        "ROSETTA_POFILE_WRAP_WIDTH": ("POFILE_WRAP_WIDTH", 78),
+        "ROSETTA_STORAGE_CLASS": (
+            "STORAGE_CLASS",
+            "rosetta.storage.CacheRosettaStorage",
+        ),
+        "ROSETTA_ENABLE_REFLANG": ("ENABLE_REFLANG", False),
+        "ROSETTA_POFILENAMES": ("POFILENAMES", ("django.po", "djangojs.po")),
+        "ROSETTA_CACHE_NAME": (
+            "ROSETTA_CACHE_NAME",
+            "rosetta" if "rosetta" in dj_settings.CACHES else "default",
+        ),
+        "ROSETTA_REQUIRES_AUTH": ("ROSETTA_REQUIRES_AUTH", True),
+        "ROSETTA_EXCLUDED_PATHS": ("ROSETTA_EXCLUDED_PATHS", ()),
+        "ROSETTA_LANGUAGE_GROUPS": ("ROSETTA_LANGUAGE_GROUPS", False),
+        "ROSETTA_AUTO_COMPILE": ("AUTO_COMPILE", True),
+        "ROSETTA_SHOW_AT_ADMIN_PANEL": ("SHOW_AT_ADMIN_PANEL", False),
+        "ROSETTA_LOGIN_URL": ("LOGIN_URL", dj_settings.LOGIN_URL),
+        "ROSETTA_LANGUAGES": ("ROSETTA_LANGUAGES", dj_settings.LANGUAGES),
+        "ROSETTA_SHOW_OCCURRENCES": ("SHOW_OCCURRENCES", True),
         # Deepl API language codes are different then those of django, so if this is not set according to your desired languages,
         # We use the first 2 letters of django language code.
         # In which case it would work fine for most of the languages,
         # But for 'en' if you want "EN-GB" for example, please set it in this dictionary.
         # you can find the supported languages list of DeepL API here: https://www.deepl.com/docs-api/translating-text/request/
         # ex: DEEPL_LANGUAGES = {"fr": "FR", "en": "EN-GB", "zh_Hans": "ZH"}
-        'DEEPL_LANGUAGES': ('DEEPL_LANGUAGES', {}),
+        "DEEPL_LANGUAGES": ("DEEPL_LANGUAGES", {}),
     }
 
     def __init__(self):
         # make sure we don't assign self._settings directly here, to avoid
         # recursion in __setattr__, we delegate to the parent instead
-        super(RosettaSettings, self).__setattr__('_settings', {})
+        super(RosettaSettings, self).__setattr__("_settings", {})
         self.load()
 
     def load(self):
         for user_setting, (rosetta_setting, default) in self.SETTINGS.items():
-            self._settings[rosetta_setting] = getattr(dj_settings, user_setting, default)
+            self._settings[rosetta_setting] = getattr(
+                dj_settings, user_setting, default
+            )
 
     def reload(self):
         self.__init__()
 
     def __getattr__(self, attr):
         if attr not in self._settings:
-            raise AttributeError("'RosettaSettings' object has not attribute '%s'" % attr)
+            raise AttributeError(
+                "'RosettaSettings' object has not attribute '%s'" % attr
+            )
         return self._settings[attr]
 
     def __setattr__(self, attr, value):
         if attr not in self._settings:
-            raise AttributeError("'RosettaSettings' object has not attribute '%s'" % attr)
+            raise AttributeError(
+                "'RosettaSettings' object has not attribute '%s'" % attr
+            )
         self._settings[attr] = value
 
 
 # This is our global settings object
 settings = RosettaSettings()
 
 
 # Signal handler to reload settings when needed
 def reload_settings(*args, **kwargs):
-    val = kwargs.get('setting')
+    val = kwargs.get("setting")
     if val in settings.SETTINGS:
         settings.reload()
 
 
 # Connect the setting_changed signal to our handler
 setting_changed.connect(reload_settings)
```

### Comparing `django-rosetta-0.9.8/rosetta/locale/ar/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/ar/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/cs/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/cs/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/de/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/de/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/es/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/es/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/fa/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/fa/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/fa/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -197,8 +197,7 @@
 msgstr "در حال نمایش:"
 
 #: templates/rosetta/pofile.html:148
 #, python-format
 msgid "%(hits)s/%(message_number)s message"
 msgid_plural "%(hits)s/%(message_number)s messages"
 msgstr[0] "%(hits)s از %(message_number)s پیام"
-
```

### Comparing `django-rosetta-0.9.8/rosetta/locale/fr/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/fr/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/hu/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/hu/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/it/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/it/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/ky/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/ky/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/ky/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/ky/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Soyuzbek Orozbek uulu <soyuzbek196.kg@gmail.com>, 2020.
-# 
+#
 # Translators:
 # Soyuzbek Orozbek uulu <soyuzbek196.kg@gmail.com>, 2020
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-05-26 21:56+0100\n"
 "PO-Revision-Date: 2020-05-26 15:58+0000\n"
 "Last-Translator: Soyuzbek Orozbek uulu <soyuzbek196.kg@gmail.com>, 2020\n"
```

### Comparing `django-rosetta-0.9.8/rosetta/locale/nl/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/nl/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/pl/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/pl/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/pl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2014-02-28 13:36+0100\n"
 "PO-Revision-Date: 2014-12-10 17:26+0124\n"
 "Last-Translator: Anonymous User <arrviasto@gmail.com>\n"
```

### Comparing `django-rosetta-0.9.8/rosetta/locale/ru/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/ru/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/tr/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/tr/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/uk/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/uk/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/locale/xx/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/locale/xx/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -27,11 +27,7 @@
 #: templates/base.html:43
 msgid "String 3 with comment"
 msgstr ""
 
 msgctxt "Context hint"
 msgid "String 4"
 msgstr ""
-
-
-
-
```

### Comparing `django-rosetta-0.9.8/rosetta/poutil.py` & `django-rosetta-0.9.9/rosetta/poutil.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def timestamp_with_timezone(dt=None):
     """
     Return a timestamp with a timezone for the configured locale.  If all else
     fails, consider localtime to be UTC.
     """
     dt = dt or datetime.now()
     if timezone is None:
-        return dt.strftime('%Y-%m-%d %H:%M%z')
+        return dt.strftime("%Y-%m-%d %H:%M%z")
     if not dt.tzinfo:
         tz = timezone.get_current_timezone()
         if not tz:
             tz = timezone.utc
         dt = dt.replace(tzinfo=timezone.get_current_timezone())
     return dt.strftime("%Y-%m-%d %H:%M%z")
 
@@ -37,89 +37,125 @@
 
     """
 
     paths = []
 
     # project/locale
     if settings.SETTINGS_MODULE:
-        parts = settings.SETTINGS_MODULE.split('.')
+        parts = settings.SETTINGS_MODULE.split(".")
     else:
         # if settings.SETTINGS_MODULE is None, we are probably in "test" mode
         # and override_settings() was used
         # see: https://code.djangoproject.com/ticket/25911
-        parts = os.environ.get(ENVIRONMENT_VARIABLE).split('.')
+        parts = os.environ.get(ENVIRONMENT_VARIABLE).split(".")
     project = __import__(parts[0], {}, {}, [])
-    abs_project_path = os.path.normpath(os.path.abspath(os.path.dirname(project.__file__)))
+    abs_project_path = os.path.normpath(
+        os.path.abspath(os.path.dirname(project.__file__))
+    )
     if project_apps:
-        if os.path.exists(os.path.abspath(os.path.join(os.path.dirname(project.__file__), 'locale'))):
-            paths.append(os.path.abspath(os.path.join(os.path.dirname(project.__file__), 'locale')))
-        if os.path.exists(os.path.abspath(os.path.join(os.path.dirname(project.__file__), '..', 'locale'))):
-            paths.append(os.path.abspath(os.path.join(os.path.dirname(project.__file__), '..', 'locale')))
-
-    case_sensitive_file_system = True
-    tmphandle, tmppath = tempfile.mkstemp()
-    if os.path.exists(tmppath.upper()):
-        # Case insensitive file system.
-        case_sensitive_file_system = False
+        if os.path.exists(
+            os.path.abspath(os.path.join(os.path.dirname(project.__file__), "locale"))
+        ):
+            paths.append(
+                os.path.abspath(
+                    os.path.join(os.path.dirname(project.__file__), "locale")
+                )
+            )
+        if os.path.exists(
+            os.path.abspath(
+                os.path.join(os.path.dirname(project.__file__), "..", "locale")
+            )
+        ):
+            paths.append(
+                os.path.abspath(
+                    os.path.join(os.path.dirname(project.__file__), "..", "locale")
+                )
+            )
+
+    # is OS case sensitive? settings preferred over auto detection
+    case_sensitive_file_system = getattr(
+        settings, "ROSETTA_CASE_SENSITIVE_FILESYSTEM", None
+    )
+
+    # in case of no settings, attempt auto detection
+    if case_sensitive_file_system is None:
+        case_sensitive_file_system = True
+        tmphandle, tmppath = tempfile.mkstemp()
+        if os.path.exists(tmppath.upper()):
+            # Case insensitive file system.
+            case_sensitive_file_system = False
 
     # django/locale
     if django_apps:
-        django_paths = cache.get('rosetta_django_paths')
+        django_paths = cache.get("rosetta_django_paths")
         if django_paths is None:
             django_paths = []
-            for root, dirnames, filename in os.walk(os.path.abspath(os.path.dirname(django.__file__))):
-                if 'locale' in dirnames:
-                    django_paths.append(os.path.join(root, 'locale'))
+            for root, dirnames, filename in os.walk(
+                os.path.abspath(os.path.dirname(django.__file__))
+            ):
+                if "locale" in dirnames:
+                    django_paths.append(os.path.join(root, "locale"))
                     continue
-            cache.set('rosetta_django_paths', django_paths, 60 * 60)
+            cache.set("rosetta_django_paths", django_paths, 60 * 60)
         paths = paths + django_paths
     # settings
     for localepath in settings.LOCALE_PATHS:
         if os.path.isdir(localepath):
             paths.append(localepath)
 
     # project/app/locale
     for app_ in apps.get_app_configs():
-        if rosetta_settings.EXCLUDED_APPLICATIONS and app_.name in rosetta_settings.EXCLUDED_APPLICATIONS:
+        if (
+            rosetta_settings.EXCLUDED_APPLICATIONS
+            and app_.name in rosetta_settings.EXCLUDED_APPLICATIONS
+        ):
             continue
 
         app_path = app_.path
         # django apps
-        if 'contrib' in app_path and 'django' in app_path and not django_apps:
+        if "contrib" in app_path and "django" in app_path and not django_apps:
             continue
 
         # third party external
         if not third_party_apps and abs_project_path not in app_path:
             continue
 
         # local apps
         if not project_apps and abs_project_path in app_path:
             continue
 
-        if os.path.exists(os.path.abspath(os.path.join(app_path, 'locale'))):
-            paths.append(os.path.abspath(os.path.join(app_path, 'locale')))
-        if os.path.exists(os.path.abspath(os.path.join(app_path, '..', 'locale'))):
-            paths.append(os.path.abspath(os.path.join(app_path, '..', 'locale')))
+        if os.path.exists(os.path.abspath(os.path.join(app_path, "locale"))):
+            paths.append(os.path.abspath(os.path.join(app_path, "locale")))
+        if os.path.exists(os.path.abspath(os.path.join(app_path, "..", "locale"))):
+            paths.append(os.path.abspath(os.path.join(app_path, "..", "locale")))
 
     ret = set()
     langs = [lang]
-    if u'-' in lang:
-        _l, _c = map(lambda x: x.lower(), lang.split(u'-', 1))
-        langs += [u'%s_%s' % (_l, _c), u'%s_%s' % (_l, _c.upper()), u'%s_%s' % (_l, _c.capitalize())]
-    elif u'_' in lang:
-        _l, _c = map(lambda x: x.lower(), lang.split(u'_', 1))
-        langs += [u'%s-%s' % (_l, _c), u'%s-%s' % (_l, _c.upper()), u'%s_%s' % (_l, _c.capitalize())]
+    if "-" in lang:
+        _l, _c = map(lambda x: x.lower(), lang.split("-", 1))
+        langs += [
+            "%s_%s" % (_l, _c),
+            "%s_%s" % (_l, _c.upper()),
+            "%s_%s" % (_l, _c.capitalize()),
+        ]
+    elif "_" in lang:
+        _l, _c = map(lambda x: x.lower(), lang.split("_", 1))
+        langs += [
+            "%s-%s" % (_l, _c),
+            "%s-%s" % (_l, _c.upper()),
+            "%s_%s" % (_l, _c.capitalize()),
+        ]
 
     paths = map(os.path.normpath, paths)
     paths = list(set(paths))
     for path in paths:
         # Exclude paths
         if path not in rosetta_settings.ROSETTA_EXCLUDED_PATHS:
             for lang_ in langs:
-                dirname = os.path.join(path, lang_, 'LC_MESSAGES')
+                dirname = os.path.join(path, lang_, "LC_MESSAGES")
                 for fn in rosetta_settings.POFILENAMES:
                     filename = os.path.join(dirname, fn)
                     abs_path = os.path.abspath(filename)
                     # On case insensitive filesystems (looking at you, MacOS)
                     # compare the lowercase absolute path of the po file
                     # to all lowercased paths already collected.
                     # This is not an issue on sane filesystems
@@ -155,12 +191,12 @@
 
     r = list(set(r))
     r.sort()
     prev = 10000
     for e in r[:]:
         if prev + 1 < e:
             try:
-                r.insert(r.index(e), '...')
+                r.insert(r.index(e), "...")
             except ValueError:
                 pass
         prev = e
     return r
```

### Comparing `django-rosetta-0.9.8/rosetta/static/admin/img/icon_searchbox_rosetta.png` & `django-rosetta-0.9.9/rosetta/static/admin/img/icon_searchbox_rosetta.png`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/storage.py` & `django-rosetta-0.9.9/rosetta/storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from django.conf import settings
 from django.core.cache import caches
 from django.core.exceptions import ImproperlyConfigured
 
 from .conf import settings as rosetta_settings
 
+
 cache = caches[rosetta_settings.ROSETTA_CACHE_NAME]
 
 
 class BaseRosettaStorage(object):
     def __init__(self, request):
         self.request = request
 
@@ -43,16 +44,16 @@
 
 
 class SessionRosettaStorage(BaseRosettaStorage):
     def __init__(self, request):
         super(SessionRosettaStorage, self).__init__(request)
 
         if (
-            'signed_cookies' in settings.SESSION_ENGINE
-            and 'pickle' not in settings.SESSION_SERIALIZER.lower()
+            "signed_cookies" in settings.SESSION_ENGINE
+            and "pickle" not in settings.SESSION_SERIALIZER.lower()
         ):
             raise ImproperlyConfigured(
                 "Sorry, but django-rosetta doesn't support the `signed_cookies` SESSION_ENGINE, because rosetta specific session files cannot be serialized."
             )
 
     def get(self, key, default=None):
         if key in self.request.session:
@@ -71,45 +72,45 @@
 
 class CacheRosettaStorage(BaseRosettaStorage):
     # unlike the session storage backend, cache is shared among all users
     # so we need to per-user key prefix, which we store in the session
     def __init__(self, request):
         super(CacheRosettaStorage, self).__init__(request)
 
-        if 'rosetta_cache_storage_key_prefix' in self.request.session:
-            self._key_prefix = self.request.session['rosetta_cache_storage_key_prefix']
+        if "rosetta_cache_storage_key_prefix" in self.request.session:
+            self._key_prefix = self.request.session["rosetta_cache_storage_key_prefix"]
         else:
             self._key_prefix = hashlib.new(
-                'sha1', str(time.time()).encode('utf8')
+                "sha1", str(time.time()).encode("utf8")
             ).hexdigest()
-            self.request.session['rosetta_cache_storage_key_prefix'] = self._key_prefix
+            self.request.session["rosetta_cache_storage_key_prefix"] = self._key_prefix
 
-        if self.request.session['rosetta_cache_storage_key_prefix'] != self._key_prefix:
+        if self.request.session["rosetta_cache_storage_key_prefix"] != self._key_prefix:
             raise ImproperlyConfigured(
                 "You can't use the CacheRosettaStorage because your Django Session storage doesn't seem to be working. The CacheRosettaStorage relies on the Django Session storage to avoid conflicts."
             )
 
         # Make sure we're not using DummyCache
         if (
-            'dummycache'
-            in settings.CACHES[rosetta_settings.ROSETTA_CACHE_NAME]['BACKEND'].lower()
+            "dummycache"
+            in settings.CACHES[rosetta_settings.ROSETTA_CACHE_NAME]["BACKEND"].lower()
         ):
             raise ImproperlyConfigured(
                 "You can't use the CacheRosettaStorage if your cache isn't correctly set up (you are using the DummyCache cache backend)."
             )
 
         # Make sure the cache actually works
         try:
-            self.set('rosetta_cache_test', 'rosetta')
-            if not self.get('rosetta_cache_test') == 'rosetta':
+            self.set("rosetta_cache_test", "rosetta")
+            if not self.get("rosetta_cache_test") == "rosetta":
                 raise ImproperlyConfigured(
                     "You can't use the CacheRosettaStorage if your cache isn't correctly set up, please double check your Django DATABASES setting and that the cache server is responding."
                 )
         finally:
-            self.delete('rosetta_cache_test')
+            self.delete("rosetta_cache_test")
 
     def get(self, key, default=None):
         # print ('get', self._key_prefix + key)
         return cache.get(self._key_prefix + key, default)
 
     def set(self, key, val):
         # print ('set', self._key_prefix + key)
@@ -123,10 +124,10 @@
         # print ('del', self._key_prefix + key)
         cache.delete(self._key_prefix + key)
 
 
 def get_storage(request):
     from rosetta.conf import settings
 
-    storage_module, storage_class = settings.STORAGE_CLASS.rsplit('.', 1)
+    storage_module, storage_class = settings.STORAGE_CLASS.rsplit(".", 1)
     storage_module = importlib.import_module(storage_module)
     return getattr(storage_module, storage_class)(request)
```

### Comparing `django-rosetta-0.9.8/rosetta/templates/rosetta/admin_index.html` & `django-rosetta-0.9.9/rosetta/templates/rosetta/admin_index.html`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/templates/rosetta/base.html` & `django-rosetta-0.9.9/rosetta/templates/rosetta/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="{% static "admin/css/base.css" %}" type="text/css"/>
     <link rel="stylesheet" href="{% static "admin/css/forms.css" %}" type="text/css"/>
     <link rel="stylesheet" href="{% static "admin/css/changelists.css" %}" type="text/css"/>
     <style type="text/css" media="screen">
         {% include 'rosetta/css/rosetta.css' %}
     </style>
     {% block extra_styles %}{% endblock %}
-    <script src="//code.jquery.com/jquery-1.12.4.min.js"></script>
+    <script src="{% static "admin/js/vendor/jquery/jquery.min.js" %}"></script>
     <script type="text/javascript">
         {% include 'rosetta/js/rosetta.js' %}
     </script>
 </head>
 <body>
     <div id="container">
         <div id="header">
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {% load static %}
 
 ss/base.css" %}" type="text/css"/>
 ss/forms.css" %}" type="text/css"/>
 ss/changelists.css" %}" type="text/css"/>
  {% block extra_styles %}{% endblock %}
+s/vendor/jquery/jquery.min.js" %}">
 {% block header %}
 ****** Rosetta ******
 {% endblock %}
 {% block breadcumbs %}{% endblock %}
 {% block main %}{% endblock %}
 Rosetta {{version}}
```

### Comparing `django-rosetta-0.9.8/rosetta/templates/rosetta/css/rosetta.css` & `django-rosetta-0.9.9/rosetta/templates/rosetta/css/rosetta.css`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/templates/rosetta/file-list.html` & `django-rosetta-0.9.9/rosetta/templates/rosetta/file-list.html`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/templates/rosetta/form.html` & `django-rosetta-0.9.9/rosetta/templates/rosetta/form.html`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/templates/rosetta/js/rosetta.js` & `django-rosetta-0.9.9/rosetta/templates/rosetta/js/rosetta.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -6,60 +6,20 @@
 
     $('.location a').show().toggle(function() {
         $('.hide', $(this).parent()).show();
     }, function() {
         $('.hide', $(this).parent()).hide();
     });
 
-
     {
         %
         if rosetta_settings.ENABLE_TRANSLATION_SUGGESTIONS %
     } {
         %
-        if rosetta_settings.DEEPL_AUTH_KEY %
-    }
-
-    $('a.suggest').click(function(e) {
-        e.preventDefault();
-        var a = $(this);
-        var str = a.html();
-        var orig = $('.original .message', a.parents('tr')).html();
-        var trans = $('textarea', a.parent());
-        var apiUrl = "https://api-free.deepl.com/v2/translate"; {
-            %
-            if deepl_language_code %
-        }
-        var destLangRoot = '{{ deepl_language_code }}'; {
-            %
-            else %
-        }
-        var destLangRoot = '{{ rosetta_i18n_lang_code_normalized }}'.substring(0, 2); {
-            % endif %
-        }
-        var sourceLang = '{{ rosetta_settings.MESSAGES_SOURCE_LANGUAGE_CODE }}'.substring(0, 2);
-        let authKey = '{{ rosetta_settings.DEEPL_AUTH_KEY }}:fx';
-
-        a.attr('class', 'suggesting').html('...');
-        fetch(apiUrl, {
-                method: 'POST',
-                headers: {
-                    "Content-Type": "application/x-www-form-urlencoded"
-                },
-                body: `auth_key=${authKey}&text=${orig}&source_lang=${sourceLang}&target_lang=${destLangRoot}`
-            }).then(response => {
-                if (response.ok) {
-                    return response.json();
-                }
-            }).then(data => {
-                trans.val(data.translations[0].text.replace(/<br>/g, '\n').replace(/<\/?code>/g, '').replace(/&lt;/g, '<').replace(/&gt;/g, '>'));
-            })
-            .catch(error => console.log(error));
-    }); {
-        % elif rosetta_settings.AZURE_CLIENT_SECRET or rosetta_settings.GOOGLE_APPLICATION_CREDENTIALS_PATH %
+        if rosetta_settings.DEEPL_AUTH_KEY or rosetta_settings.AZURE_CLIENT_SECRET or rosetta_settings.GOOGLE_APPLICATION_CREDENTIALS_PATH %
     }
     $('a.suggest').click(function(e) {
         e.preventDefault();
         var a = $(this);
         var str = a.html();
         var orig = $('.original .message', a.parents('tr')).html();
         var trans = $('textarea', a.parent());
@@ -68,15 +28,15 @@
 
         orig = unescape(orig).replace(/<br\s?\/?>/g, '\n').replace(/<code>/, '').replace(/<\/code>/g, '').replace(/&gt;/g, '>').replace(/&lt;/g, '<');
         a.attr('class', 'suggesting').html('...');
 
         $.getJSON("{% url 'rosetta.translate_text' %}", {
                 from: sourceLang,
                 to: destLang,
-                text: orig
+                text: orig,
             },
             function(data) {
                 if (data.success) {
                     trans.val(unescape(data.translation).replace(/&#39;/g, '\'').replace(/&quot;/g, '"').replace(/%\s+(\([^\)]+\))\s*s/g, ' %$1s '));
                     a.hide();
                 } else {
                     a.text(data.error);
@@ -140,15 +100,15 @@
 
     $('.translation textarea')
 
         .blur(function() {
             if ($(this).val()) {
                 $('.alert', $(this).parents('tr')).remove();
                 var RX = /%(?:\([^\s\)]*\))?[sdf]|\{[\w\d_]+?\}/g,
-                    origs = $(this).parents('tr').find('.original>.message').html().match(RX),
+                    origs = $(this).parents('tr').find('.original span').html().match(RX),
                     trads = $(this).val().match(RX),
                     error = $('<span class="alert">Unmatched variables</span>');
 
                 if (origs && trads) {
                     for (var i = trads.length; i--;) {
                         var key = trads[i];
                         if (-1 == $.inArray(key, origs)) {
```

### Comparing `django-rosetta-0.9.8/rosetta/templatetags/rosetta.py` & `django-rosetta-0.9.9/rosetta/templatetags/rosetta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import re
 
 from django import template
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
+
 from rosetta.access import can_translate
 
+
 register = template.Library()
-rx = re.compile(r'(%(\([^\s\)]*\))?[sd]|\{[\w\d_]+?\})')
+rx = re.compile(r"(%(\([^\s\)]*\))?[sd]|\{[\w\d_]+?\})")
 
 can_translate = register.filter(can_translate)
 
 
 def format_message(message):
     return mark_safe(
-        rx.sub('<code>\\1</code>', escape(message).replace(r'\n', '<br />\n'))
+        rx.sub("<code>\\1</code>", escape(message).replace(r"\n", "<br />\n"))
     )
 
 
 format_message = register.filter(format_message)
 
 
 def lines_count(message):
-    return 1 + sum([len(line) / 50 for line in message.split('\n')])
+    return 1 + sum([len(line) / 50 for line in message.split("\n")])
 
 
 lines_count = register.filter(lines_count)
 
 
 def mult(a, b):
     return int(a) * int(b)
@@ -55,31 +57,31 @@
 
 
 def do_incr(parser, token):
     args = token.split_contents()
     if len(args) < 2:
         raise SyntaxError("'incr' tag requires at least one argument")
     name = args[1]
-    if not hasattr(parser, '_namedIncrNodes'):
+    if not hasattr(parser, "_namedIncrNodes"):
         parser._namedIncrNodes = {}
     if name not in parser._namedIncrNodes:
         parser._namedIncrNodes[name] = IncrNode(0)
     return parser._namedIncrNodes[name]
 
 
-do_incr = register.tag('increment', do_incr)
+do_incr = register.tag("increment", do_incr)
 
 
 class IncrNode(template.Node):
     def __init__(self, init_val=0):
         self.val = init_val
 
     def render(self, context):
         self.val += 1
         return str(self.val)
 
 
 def is_fuzzy(message):
-    return message and hasattr(message, 'flags') and 'fuzzy' in message.flags
+    return message and hasattr(message, "flags") and "fuzzy" in message.flags
 
 
 is_fuzzy = register.filter(is_fuzzy)
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue186.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue186.template`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue24gh.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue24gh.template`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue34gh.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue34gh.template`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue38gh.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue38gh.template`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
@@ -362,10 +362,7 @@
 msgstr ""
 
 msgid "xeXu5ur6xtXV69d2-7u7Fz5eD6TpYXyNVcFd28vjsZ7fnYIrzTTMEn__E_5ykGYGm-aY_7JXpx9_fXD9K-75dlH1vTvOv2w2HsZPL9zu7MdvupP-qNh5xo8PjfCLkR1kO4QUmB8CZHeW2BcGw2nYTjt7I7NcBLDuNM9PpbvPQt3le1Pex String 49"
 msgstr ""
 
 msgid "xeXu5ur6xtXV69d2-7u7Fz5eD6TpYXyNVcFd28vjsZ7fnYIrzTTMEn__E_5ykGYGm-aY_7JXpx9_fXD9K-75dlH1vTvOv2w2HsZPL9zu7MdvupP-qNh5xo8PjfCLkR1kO4QUmB8CZHeW2BcGw2nYTjt7I7NcBLDuNM9PpbvPQt3le1Pex String 50"
 msgstr ""
-
-
-
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue39gh.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue39gh.template`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue60.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue60.template`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
@@ -27,11 +27,7 @@
 #: templates/base.html:43
 msgid "String 3 with comment"
 msgstr ""
 
 msgctxt "Context hint"
 msgid "String 4"
 msgstr ""
-
-
-
-
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue67.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue67.template`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
@@ -20,9 +20,7 @@
 
 
 msgid "String 1"
 msgstr ""
 
 msgid "String 2"
 msgstr ""
-
-
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.issue79.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.issue79.template`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
@@ -18,10 +18,7 @@
 
 
 msgid "String 1"
 msgstr ""
 
 #~ msgid "String 2"
 #~ msgstr ""
-
-
-
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.template`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Rosetta\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2009-10-21 12:21+0200\n"
 "PO-Revision-Date: 2008-09-22 11:02\n"
 "Last-Translator: Admin Admin <admin@admin.com>\n"
@@ -27,11 +27,7 @@
 #: templates/base.html:43
 msgid "String 3 with comment"
 msgstr ""
 
 msgctxt "Context hint"
 msgid "String 4"
 msgstr ""
-
-
-
-
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/django.po.test44.template` & `django-rosetta-0.9.9/rosetta/tests/django.po.test44.template`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/tests/pr44.po.template` & `django-rosetta-0.9.9/testproject/locale/fr_FR.utf8/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: Rosetta\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2009-10-21 12:21+0200\n"
-"PO-Revision-Date: 2008-09-22 11:02\n"
-"Last-Translator: Admin Admin <admin@admin.com>\n"
-"Language-Team: French <LL@li.org>\n"
+"POT-Creation-Date: 2015-09-14 02:28-0500\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Translated-Using: django-rosetta 0.4.RC2\n"
-
-
-msgid "String 1"
-msgstr ""
-
-#~ msgid "String 2"
-#~ msgstr ""
-
-
+"Language: \n"
+"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
+"X-Translated-Using: django-rosetta 0.7.5\n"
+
+#: templates/test.html:3
+msgid "Some text to translate"
+msgstr "oiwue oqwiue§o§"
 
+#: templates/test.html:5
+#, python-format
+msgid ""
+"\n"
+"one bottle of beer on the wall\n"
+msgid_plural ""
+"\n"
+"%(num_bottles)s bottles of beer on the wall\n"
+msgstr[0] ""
+"\n"
+"%(num_bottles)s bottles of beer on the wall\n"
+msgstr[1] ""
+"\n"
+"%(num_bottles)s bottles of beer on the wall\n"
+msgstr[0] ""
+msgstr[1] ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-rosetta-0.9.8/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/rosetta/tests/test_app/locale/xx/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/rosetta/tests/tests.py` & `django-rosetta-0.9.9/rosetta/tests/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,664 +1,673 @@
 import filecmp
 import hashlib
 import os
 import shutil
+from unittest import mock
 from urllib.parse import urlencode
 
-import vcr
 from django import VERSION
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.dispatch import receiver
 from django.http import Http404
 from django.test import RequestFactory, TestCase, override_settings
 from django.test.client import Client
 from django.urls import resolve, reverse
 from django.utils.encoding import force_bytes
+
+import vcr
 from rosetta import views
+from rosetta.poutil import find_pos
 from rosetta.signals import entry_changed, post_save
 from rosetta.storage import get_storage
 
 
 class RosettaTestCase(TestCase):
     def __init__(self, *args, **kwargs):
         super(RosettaTestCase, self).__init__(*args, **kwargs)
         self.curdir = os.path.dirname(__file__)
         self.dest_file = os.path.normpath(
-            os.path.join(self.curdir, '../locale/xx/LC_MESSAGES/django.po')
+            os.path.join(self.curdir, "../locale/xx/LC_MESSAGES/django.po")
         )
 
     def setUp(self):
         from django.contrib.auth.models import User
 
         user = User.objects.create_superuser(
-            'test_admin', 'test@test.com', 'test_password'
+            "test_admin", "test@test.com", "test_password"
         )
         user2 = User.objects.create_superuser(
-            'test_admin2', 'test@test2.com', 'test_password'
+            "test_admin2", "test@test2.com", "test_password"
         )
         user3 = User.objects.create_superuser(
-            'test_admin3', 'test@test2.com', 'test_password'
+            "test_admin3", "test@test2.com", "test_password"
         )
 
         user3.is_staff = False
         user3.save()
 
         self.user = user
         self.client2 = Client()
 
-        self.client.login(username=user.username, password='test_password')
-        self.client2.login(username=user2.username, password='test_password')
+        self.client.login(username=user.username, password="test_password")
+        self.client2.login(username=user2.username, password="test_password")
 
-        shutil.copy(self.dest_file, self.dest_file + '.orig')
+        shutil.copy(self.dest_file, self.dest_file + ".orig")
 
     def tearDown(self):
-        shutil.move(self.dest_file + '.orig', self.dest_file)
+        shutil.move(self.dest_file + ".orig", self.dest_file)
 
     def copy_po_file_from_template(self, template_path):
         """Utility method to handle swapping a template po file in place for
         testing.
         """
         src_path = os.path.normpath(os.path.join(self.curdir, template_path))
         shutil.copy(src_path, self.dest_file)
 
     @property
     def xx_form_url(self):
-        kwargs = {'po_filter': 'third-party', 'lang_id': 'xx', 'idx': 0}
-        return reverse('rosetta-form', kwargs=kwargs)
+        kwargs = {"po_filter": "third-party", "lang_id": "xx", "idx": 0}
+        return reverse("rosetta-form", kwargs=kwargs)
 
     @property
     def all_file_list_url(self):
-        return reverse('rosetta-file-list', kwargs={'po_filter': 'all'})
+        return reverse("rosetta-file-list", kwargs={"po_filter": "all"})
 
     @property
     def project_file_list_url(self):
-        return reverse('rosetta-file-list', kwargs={'po_filter': 'project'})
+        return reverse("rosetta-file-list", kwargs={"po_filter": "project"})
 
     @property
     def third_party_file_list_url(self):
-        return reverse('rosetta-file-list', kwargs={'po_filter': 'third-party'})
+        return reverse("rosetta-file-list", kwargs={"po_filter": "third-party"})
 
     def test_1_ListLoading(self):
         r = self.client.get(self.third_party_file_list_url)
         self.assertTrue(
-            os.path.normpath('rosetta/locale/xx/LC_MESSAGES/django.po')
+            os.path.normpath("rosetta/locale/xx/LC_MESSAGES/django.po")
             in r.content.decode()
         )
 
-    @override_settings(ROSETTA_LANGUAGES=(('xx', 'dummy language'),))
+    @override_settings(ROSETTA_LANGUAGES=(("xx", "dummy language"),))
     def test_2_PickFile(self):
         r = self.client.get(self.xx_form_url)
-        self.assertTrue('dummy language' in r.content.decode())
+        self.assertTrue("dummy language" in r.content.decode())
 
     def test_3_DownloadZIP(self):
-        kwargs = {'po_filter': 'third-party', 'lang_id': 'xx', 'idx': 0}
-        url = reverse('rosetta-download-file', kwargs=kwargs)
+        kwargs = {"po_filter": "third-party", "lang_id": "xx", "idx": 0}
+        url = reverse("rosetta-download-file", kwargs=kwargs)
         r = self.client.get(url)
-        self.assertTrue('application/x-zip' in r['content-type'])
+        self.assertTrue("application/x-zip" in r["content-type"])
 
-    @override_settings(ROSETTA_LANGUAGES=(('xx', 'dummy language'),))
+    @override_settings(ROSETTA_LANGUAGES=(("xx", "dummy language"),))
     def test_4_DoChanges(self):
-        self.copy_po_file_from_template('./django.po.template')
-        untranslated_url = self.xx_form_url + '?msg_filter=untranslated'
-        translated_url = self.xx_form_url + '?msg_filter=translated'
+        self.copy_po_file_from_template("./django.po.template")
+        untranslated_url = self.xx_form_url + "?msg_filter=untranslated"
+        translated_url = self.xx_form_url + "?msg_filter=translated"
 
         # Load the template file
         r = self.client.get(untranslated_url)
 
         # make sure both strings are untranslated
-        self.assertTrue('dummy language' in r.content.decode())
-        self.assertTrue('String 1' in r.content.decode())
-        self.assertTrue('String 2' in r.content.decode())
-        self.assertTrue('m_e48f149a8b2e8baa81b816c0edf93890' in r.content.decode())
+        self.assertTrue("dummy language" in r.content.decode())
+        self.assertTrue("String 1" in r.content.decode())
+        self.assertTrue("String 2" in r.content.decode())
+        self.assertTrue("m_e48f149a8b2e8baa81b816c0edf93890" in r.content.decode())
 
         # post a translation
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
         r = self.client.post(untranslated_url, data, follow=True)
 
         # reload all untranslated strings
         r = self.client.get(untranslated_url)
 
         # the translated string no longer is up for translation
-        self.assertTrue('String 1' in r.content.decode())
-        self.assertTrue('String 2' not in r.content.decode())
+        self.assertTrue("String 1" in r.content.decode())
+        self.assertTrue("String 2" not in r.content.decode())
 
         # display only translated strings
         r = self.client.get(translated_url)
 
         # The translation was persisted
-        self.assertTrue('String 1' not in r.content.decode())
-        self.assertTrue('String 2' in r.content.decode())
-        self.assertTrue('Hello, world' in r.content.decode())
+        self.assertTrue("String 1" not in r.content.decode())
+        self.assertTrue("String 2" in r.content.decode())
+        self.assertTrue("Hello, world" in r.content.decode())
 
-    @override_settings(ROSETTA_LANGUAGES=(('xx', 'dummy language'),))
+    @override_settings(ROSETTA_LANGUAGES=(("xx", "dummy language"),))
     def test_5_TestIssue67(self):
         # issue 67: http://code.google.com/p/django-rosetta/issues/detail?id=67
-        self.copy_po_file_from_template('./django.po.issue67.template')
+        self.copy_po_file_from_template("./django.po.issue67.template")
 
         # Make sure the plurals string is valid
-        with open(self.dest_file, 'r') as f_:
+        with open(self.dest_file, "r") as f_:
             content = f_.read()
-        self.assertTrue('Hello, world' not in content)
-        self.assertTrue('|| n%100>=20) ? 1 : 2)' in content)
+        self.assertTrue("Hello, world" not in content)
+        self.assertTrue("|| n%100>=20) ? 1 : 2)" in content)
         del content
 
-        r = self.client.get(self.xx_form_url + '?msg_filter=untranslated')
+        r = self.client.get(self.xx_form_url + "?msg_filter=untranslated")
 
         # make sure all strings are untranslated
-        self.assertTrue('dummy language' in r.content.decode())
-        self.assertTrue('String 1' in r.content.decode())
-        self.assertTrue('String 2' in r.content.decode())
-        self.assertTrue('m_e48f149a8b2e8baa81b816c0edf93890' in r.content.decode())
+        self.assertTrue("dummy language" in r.content.decode())
+        self.assertTrue("String 1" in r.content.decode())
+        self.assertTrue("String 2" in r.content.decode())
+        self.assertTrue("m_e48f149a8b2e8baa81b816c0edf93890" in r.content.decode())
 
         # post a translation
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
-        self.client.post(self.xx_form_url + '?msg_filter=untranslated', data)
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
+        self.client.post(self.xx_form_url + "?msg_filter=untranslated", data)
 
         # Make sure the plurals string is still valid
-        with open(self.dest_file, 'r') as f_:
+        with open(self.dest_file, "r") as f_:
             content = f_.read()
-        self.assertTrue('Hello, world' in str(content))
-        self.assertTrue('|| n%100>=20) ? 1 : 2)' in str(content))
-        self.assertTrue('or n%100>=20) ? 1 : 2)' not in str(content))
+        self.assertTrue("Hello, world" in str(content))
+        self.assertTrue("|| n%100>=20) ? 1 : 2)" in str(content))
+        self.assertTrue("or n%100>=20) ? 1 : 2)" not in str(content))
         del content
 
-    @override_settings(ROSETTA_LANGUAGES=(('xx', 'dummy language'),))
+    @override_settings(ROSETTA_LANGUAGES=(("xx", "dummy language"),))
     def test_6_ExcludedApps(self):
-        with self.settings(ROSETTA_EXCLUDED_APPLICATIONS=('rosetta',)):
+        with self.settings(ROSETTA_EXCLUDED_APPLICATIONS=("rosetta",)):
             r = self.client.get(self.third_party_file_list_url)
-            self.assertNotContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+            self.assertNotContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
 
         with self.settings(ROSETTA_EXCLUDED_APPLICATIONS=()):
             r = self.client.get(self.third_party_file_list_url)
-            self.assertContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+            self.assertContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
 
     def test_7_selfInApplist(self):
         r = self.client.get(self.third_party_file_list_url)
-        self.assertContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+        self.assertContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
 
         r = self.client.get(self.project_file_list_url)
-        self.assertNotContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+        self.assertNotContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
 
-    @override_settings(ROSETTA_LANGUAGES=(('xx', 'dummy language'),))
+    @override_settings(ROSETTA_LANGUAGES=(("xx", "dummy language"),))
     def test_8_hideObsoletes(self):
         r = self.client.get(self.xx_form_url)
 
         # not in listing
         for p in range(1, 5):
-            r = self.client.get(self.xx_form_url + '?page=%d' % p)
-            self.assertTrue('dummy language' in r.content.decode())
-            self.assertTrue('Les deux' not in r.content.decode())
-
-        r = self.client.get(self.xx_form_url + '?query=Les%20Deux')
-        self.assertContains(r, 'dummy language')
-        self.assertNotContains(r, 'Les deux')
+            r = self.client.get(self.xx_form_url + "?page=%d" % p)
+            self.assertTrue("dummy language" in r.content.decode())
+            self.assertTrue("Les deux" not in r.content.decode())
+
+        r = self.client.get(self.xx_form_url + "?query=Les%20Deux")
+        self.assertContains(r, "dummy language")
+        self.assertNotContains(r, "Les deux")
 
     def test_9_concurrency(self):
-        self.copy_po_file_from_template('./django.po.template')
-        translated_url = self.xx_form_url + '?msg_filter=translated'
-        untranslated_url = self.xx_form_url + '?msg_filter=untranslated'
+        self.copy_po_file_from_template("./django.po.template")
+        translated_url = self.xx_form_url + "?msg_filter=translated"
+        untranslated_url = self.xx_form_url + "?msg_filter=untranslated"
 
         # Load the template file
         r = self.client.get(untranslated_url)
         r2 = self.client2.get(untranslated_url)
 
-        self.assertContains(r, 'String 1')
-        self.assertContains(r2, 'String 1')
-        self.assertContains(r, 'm_08e4e11e2243d764fc45a5a4fba5d0f2')
+        self.assertContains(r, "String 1")
+        self.assertContains(r2, "String 1")
+        self.assertContains(r, "m_08e4e11e2243d764fc45a5a4fba5d0f2")
 
-        data = {'m_08e4e11e2243d764fc45a5a4fba5d0f2': 'Hello, world'}
+        data = {"m_08e4e11e2243d764fc45a5a4fba5d0f2": "Hello, world"}
         r = self.client.post(untranslated_url, data, follow=True)
 
         # Client 2 reloads, forces a reload of the catalog; untranslated
         # string1 is now translated
         r2 = self.client2.get(untranslated_url, follow=True)
-        self.assertNotContains(r, 'String 1')
-        self.assertContains(r, 'String 2')
-        self.assertNotContains(r2, 'String 1')
-        self.assertContains(r2, 'String 2')
+        self.assertNotContains(r, "String 1")
+        self.assertContains(r, "String 2")
+        self.assertNotContains(r2, "String 1")
+        self.assertContains(r2, "String 2")
 
         r = self.client.get(untranslated_url)
         r2 = self.client2.get(untranslated_url)
 
-        self.assertContains(r2, 'String 2')
-        self.assertContains(r2, 'm_e48f149a8b2e8baa81b816c0edf93890')
-        self.assertContains(r, 'String 2')
-        self.assertContains(r, 'm_e48f149a8b2e8baa81b816c0edf93890')
+        self.assertContains(r2, "String 2")
+        self.assertContains(r2, "m_e48f149a8b2e8baa81b816c0edf93890")
+        self.assertContains(r, "String 2")
+        self.assertContains(r, "m_e48f149a8b2e8baa81b816c0edf93890")
 
         # client 2 posts!
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world, from client two!'}
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world, from client two!"}
         r2 = self.client2.post(untranslated_url, data, follow=True)
 
-        self.assertNotContains(r2, 'save-conflict')
+        self.assertNotContains(r2, "save-conflict")
 
         # uh-oh here comes client 1
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world, from client one!'}
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world, from client one!"}
         r = self.client.post(untranslated_url, data, follow=True)
         # An error message is displayed
-        self.assertContains(r, 'save-conflict')
+        self.assertContains(r, "save-conflict")
 
         # client 2 won
-        with open(self.dest_file, 'r') as po_file:
+        with open(self.dest_file, "r") as po_file:
             pofile_content = po_file.read()
-        self.assertTrue('Hello, world, from client two!' in pofile_content)
+        self.assertTrue("Hello, world, from client two!" in pofile_content)
 
         # Both clients show all strings, error messages are gone
         r = self.client.get(translated_url)
-        self.assertNotContains(r, 'save-conflict')
+        self.assertNotContains(r, "save-conflict")
         r2 = self.client2.get(translated_url)
-        self.assertNotContains(r2, 'save-conflict')
+        self.assertNotContains(r2, "save-conflict")
         r = self.client.get(self.xx_form_url)
-        self.assertNotContains(r, 'save-conflict')
+        self.assertNotContains(r, "save-conflict")
         r2 = self.client2.get(self.xx_form_url)
-        self.assertNotContains(r2, 'save-conflict')
+        self.assertNotContains(r2, "save-conflict")
 
         # Both have client's two version
-        self.assertContains(r, 'Hello, world, from client two!')
-        self.assertContains(r2, 'Hello, world, from client two!')
+        self.assertContains(r, "Hello, world, from client two!")
+        self.assertContains(r2, "Hello, world, from client two!")
 
     def test_10_issue_79_num_entries(self):
-        self.copy_po_file_from_template('./django.po.issue79.template')
+        self.copy_po_file_from_template("./django.po.issue79.template")
         r = self.client.get(self.third_party_file_list_url)
         self.assertContains(r, '<td class="ch-messages r">1</td>')
         self.assertContains(r, '<td class="ch-progress r">0%</td>')
         self.assertContains(r, '<td class="ch-obsolete r">1</td>')
 
     def test_11_issue_80_tab_indexes(self):
         r = self.client.get(self.xx_form_url)
         self.assertTrue('tabindex="3"' in r.content.decode())
 
     def test_12_issue_82_staff_user(self):
         self.client3 = Client()
-        self.client3.login(username='test_admin3', password='test_password')
+        self.client3.login(username="test_admin3", password="test_password")
 
         # When auth is required, we get an empty response (and a redirect) with
         # this user.
         with self.settings(ROSETTA_REQUIRES_AUTH=True):
             r = self.client3.get(self.xx_form_url)
             self.assertFalse(r.content.decode())
             self.assertEqual(r.status_code, 302)
 
         # When it's not required, we sail through.
         with self.settings(ROSETTA_REQUIRES_AUTH=False):
             r = self.client3.get(self.xx_form_url)
             self.assertTrue(r.content.decode())
             self.assertEqual(r.status_code, 200)
 
-    @override_settings(ROSETTA_LANGUAGES=(('fr', 'French'), ('xx', 'Dummy Language')))
+    @override_settings(ROSETTA_LANGUAGES=(("fr", "French"), ("xx", "Dummy Language")))
     def test_13_catalog_filters(self):
         r = self.client.get(self.third_party_file_list_url)
         self.assertTrue(
-            os.path.normpath('rosetta/locale/xx/LC_MESSAGES/django.po')
+            os.path.normpath("rosetta/locale/xx/LC_MESSAGES/django.po")
             in r.content.decode()
         )
 
-        url = reverse('rosetta-file-list', kwargs={'po_filter': 'django'})
+        url = reverse("rosetta-file-list", kwargs={"po_filter": "django"})
         r = self.client.get(url)
         self.assertTrue(
-            os.path.normpath('rosetta/locale/xx/LC_MESSAGES/django.po')
+            os.path.normpath("rosetta/locale/xx/LC_MESSAGES/django.po")
             not in r.content.decode()
         )
 
         r = self.client.get(self.all_file_list_url)
         self.assertTrue(
-            os.path.normpath('rosetta/locale/xx/LC_MESSAGES/django.po')
+            os.path.normpath("rosetta/locale/xx/LC_MESSAGES/django.po")
             in r.content.decode()
         )
 
         r = self.client.get(self.project_file_list_url)
         self.assertTrue(
-            os.path.normpath('rosetta/locale/xx/LC_MESSAGES/django.po')
+            os.path.normpath("rosetta/locale/xx/LC_MESSAGES/django.po")
             not in r.content.decode()
         )
 
     def test_14_issue_99_context_and_comments(self):
         r = self.client.get(self.xx_form_url)
-        self.assertTrue('This is a text of the base template' in r.content.decode())
-        self.assertTrue('Context hint' in r.content.decode())
+        self.assertTrue("This is a text of the base template" in r.content.decode())
+        self.assertTrue("Context hint" in r.content.decode())
 
     def test_15_issue_87_entry_changed_signal(self):
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
         r = self.client.get(self.xx_form_url)
 
         @receiver(entry_changed)
         def test_receiver(sender, **kwargs):
-            self.test_old_msgstr = kwargs.get('old_msgstr')
+            self.test_old_msgstr = kwargs.get("old_msgstr")
             self.test_new_msgstr = sender.msgstr
             self.test_msg_id = sender.msgid
 
-        self.assertTrue('m_e48f149a8b2e8baa81b816c0edf93890' in r.content.decode())
+        self.assertTrue("m_e48f149a8b2e8baa81b816c0edf93890" in r.content.decode())
 
         # post a translation
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
         self.client.post(self.xx_form_url, data)
 
-        self.assertTrue(self.test_old_msgstr == '')
-        self.assertTrue(self.test_new_msgstr == 'Hello, world')
-        self.assertTrue(self.test_msg_id == 'String 2')
+        self.assertTrue(self.test_old_msgstr == "")
+        self.assertTrue(self.test_new_msgstr == "Hello, world")
+        self.assertTrue(self.test_msg_id == "String 2")
 
         del (self.test_old_msgstr, self.test_new_msgstr, self.test_msg_id)
 
     def test_16_issue_101_post_save_signal(self):
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
         r = self.client.get(self.xx_form_url)
 
         @receiver(post_save)
         def test_receiver(sender, **kwargs):
-            self.test_sig_lang = kwargs.get('language_code')
+            self.test_sig_lang = kwargs.get("language_code")
 
-        self.assertTrue('m_e48f149a8b2e8baa81b816c0edf93890' in r.content.decode())
+        self.assertTrue("m_e48f149a8b2e8baa81b816c0edf93890" in r.content.decode())
 
         # post a translation
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
         self.client.post(self.xx_form_url, data)
 
-        self.assertTrue(self.test_sig_lang == 'xx')
+        self.assertTrue(self.test_sig_lang == "xx")
         del self.test_sig_lang
 
     def test_17_issue_103_post_save_signal_has_request(self):
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
         r = self.client.get(self.xx_form_url)
 
         @receiver(post_save)
         def test_receiver(sender, **kwargs):
-            self.test_16_has_request = 'request' in kwargs
+            self.test_16_has_request = "request" in kwargs
 
-        self.assertTrue('m_e48f149a8b2e8baa81b816c0edf93890' in r.content.decode())
+        self.assertTrue("m_e48f149a8b2e8baa81b816c0edf93890" in r.content.decode())
 
         # post a translation
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
         r = self.client.post(self.xx_form_url, data)
 
         self.assertTrue(self.test_16_has_request)
         del self.test_16_has_request
 
     def test_18_Test_Issue_gh24(self):
-        self.copy_po_file_from_template('./django.po.issue24gh.template')
+        self.copy_po_file_from_template("./django.po.issue24gh.template")
         r = self.client.get(self.xx_form_url)
 
-        self.assertTrue('m_bb9d8fe6159187b9ea494c1b313d23d4' in r.content.decode())
+        self.assertTrue("m_bb9d8fe6159187b9ea494c1b313d23d4" in r.content.decode())
 
         # Post a translation, it should have properly wrapped lines
         data = {
-            'm_bb9d8fe6159187b9ea494c1b313d23d4': 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean '
-            'commodo ligula eget dolor. Aenean massa. Cum sociis natoque '
-            'penatibus et magnis dis parturient montes, nascetur ridiculus '
-            'mus. Donec quam felis, ultricies nec, pellentesque eu, pretium '
-            'quis, sem. Nulla consequat massa quis enim. Donec pede justo, '
-            'fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, '
-            'rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum '
-            'felis eu pede mollis pretium.'
+            "m_bb9d8fe6159187b9ea494c1b313d23d4": (
+                "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean "
+                "commodo ligula eget dolor. Aenean massa. Cum sociis natoque "
+                "penatibus et magnis dis parturient montes, nascetur ridiculus "
+                "mus. Donec quam felis, ultricies nec, pellentesque eu, pretium "
+                "quis, sem. Nulla consequat massa quis enim. Donec pede justo, "
+                "fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, "
+                "rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum "
+                "felis eu pede mollis pretium."
+            )
         }
         r = self.client.post(self.xx_form_url, data)
-        with open(self.dest_file, 'r') as po_file:
+        with open(self.dest_file, "r") as po_file:
             pofile_content = po_file.read()
 
         self.assertTrue('"pede mollis pretium."' in pofile_content)
 
         # Again, with unwrapped lines
-        self.copy_po_file_from_template('./django.po.issue24gh.template')
+        self.copy_po_file_from_template("./django.po.issue24gh.template")
         with self.settings(ROSETTA_POFILE_WRAP_WIDTH=0):
             r = self.client.get(self.xx_form_url)
-            self.assertTrue('m_bb9d8fe6159187b9ea494c1b313d23d4' in r.content.decode())
+            self.assertTrue("m_bb9d8fe6159187b9ea494c1b313d23d4" in r.content.decode())
             r = self.client.post(self.xx_form_url, data)
-            with open(self.dest_file, 'r') as po_file:
+            with open(self.dest_file, "r") as po_file:
                 pofile_content = po_file.read()
             self.assertTrue('felis eu pede mollis pretium."' in pofile_content)
 
     def test_19_Test_Issue_gh34(self):
-        self.copy_po_file_from_template('./django.po.issue34gh.template')
+        self.copy_po_file_from_template("./django.po.issue34gh.template")
         r = self.client.get(self.xx_form_url)
-        self.assertTrue('m_ff7060c1a9aae9c42af4d54ac8551f67_1' in r.content.decode())
-        self.assertTrue('m_ff7060c1a9aae9c42af4d54ac8551f67_0' in r.content.decode())
-        self.assertTrue('m_09f7e02f1290be211da707a266f153b3' in r.content.decode())
+        self.assertTrue("m_ff7060c1a9aae9c42af4d54ac8551f67_1" in r.content.decode())
+        self.assertTrue("m_ff7060c1a9aae9c42af4d54ac8551f67_0" in r.content.decode())
+        self.assertTrue("m_09f7e02f1290be211da707a266f153b3" in r.content.decode())
 
         # post a translation, it should have properly wrapped lines
         data = {
-            'm_ff7060c1a9aae9c42af4d54ac8551f67_0': 'Foo %s',
-            'm_ff7060c1a9aae9c42af4d54ac8551f67_1': 'Bar %s',
-            'm_09f7e02f1290be211da707a266f153b3': 'Salut',
+            "m_ff7060c1a9aae9c42af4d54ac8551f67_0": "Foo %s",
+            "m_ff7060c1a9aae9c42af4d54ac8551f67_1": "Bar %s",
+            "m_09f7e02f1290be211da707a266f153b3": "Salut",
         }
         r = self.client.post(self.xx_form_url, data)
-        with open(self.dest_file, 'r') as po_file:
+        with open(self.dest_file, "r") as po_file:
             pofile_content = po_file.read()
         self.assertTrue('msgstr "Salut\\n"' in pofile_content)
         self.assertTrue('msgstr[0] ""\n"\\n"\n"Foo %s\\n"' in pofile_content)
         self.assertTrue('msgstr[1] ""\n"\\n"\n"Bar %s\\n"' in pofile_content)
 
     @override_settings(
-        SESSION_ENGINE='django.contrib.sessions.backends.signed_cookies',
-        ROSETTA_STORAGE_CLASS='rosetta.storage.CacheRosettaStorage',
+        SESSION_ENGINE="django.contrib.sessions.backends.signed_cookies",
+        ROSETTA_STORAGE_CLASS="rosetta.storage.CacheRosettaStorage",
     )
     def test_20_Test_Issue_gh38(self):
         # (Have to log in again, since our session engine changed)
-        self.client.login(username='test_admin', password='test_password')
+        self.client.login(username="test_admin", password="test_password")
         self.assertTrue(
-            'django.contrib.sessions.middleware.SessionMiddleware' in settings.MIDDLEWARE
+            "django.contrib.sessions.middleware.SessionMiddleware"
+            in settings.MIDDLEWARE
         )
 
         # Only one backend to test: cache backend
-        self.copy_po_file_from_template('./django.po.issue38gh.template')
+        self.copy_po_file_from_template("./django.po.issue38gh.template")
 
         r = self.client.get(self.xx_form_url)
-        self.assertFalse(len(str(self.client.cookies.get('sessionid'))) > 4096)
-        self.assertTrue('m_9efd113f7919952523f06e0d88da9c54' in r.content.decode())
+        self.assertFalse(len(str(self.client.cookies.get("sessionid"))) > 4096)
+        self.assertTrue("m_9efd113f7919952523f06e0d88da9c54" in r.content.decode())
 
-        data = {'m_9efd113f7919952523f06e0d88da9c54': 'Testing cookie length'}
+        data = {"m_9efd113f7919952523f06e0d88da9c54": "Testing cookie length"}
         r = self.client.post(self.xx_form_url, data)
-        with open(self.dest_file, 'r') as po_file:
+        with open(self.dest_file, "r") as po_file:
             pofile_content = po_file.read()
-        self.assertTrue('Testing cookie length' in pofile_content)
+        self.assertTrue("Testing cookie length" in pofile_content)
 
-        r = self.client.get(self.xx_form_url + '?filter=translated')
-        self.assertTrue('Testing cookie length' in r.content.decode())
-        self.assertTrue('m_9f6c442c6d579707440ba9dada0fb373' in r.content.decode())
+        r = self.client.get(self.xx_form_url + "?filter=translated")
+        self.assertTrue("Testing cookie length" in r.content.decode())
+        self.assertTrue("m_9f6c442c6d579707440ba9dada0fb373" in r.content.decode())
 
-    @override_settings(ROSETTA_STORAGE_CLASS='rosetta.storage.CacheRosettaStorage')
+    @override_settings(ROSETTA_STORAGE_CLASS="rosetta.storage.CacheRosettaStorage")
     def test_21_concurrency_of_cache_backend(self):
-        self.copy_po_file_from_template('./django.po.issue38gh.template')
+        self.copy_po_file_from_template("./django.po.issue38gh.template")
 
         # Force caching into play by making .po file read-only
         os.chmod(self.dest_file, 292)  # 0444
 
         self.client.get(self.xx_form_url)
         self.client2.get(self.xx_form_url)
         self.assertNotEqual(
-            self.client.session.get('rosetta_cache_storage_key_prefix'),
-            self.client2.session.get('rosetta_cache_storage_key_prefix'),
+            self.client.session.get("rosetta_cache_storage_key_prefix"),
+            self.client2.session.get("rosetta_cache_storage_key_prefix"),
         )
 
         # Clean up (restore perms)
         os.chmod(self.dest_file, 420)  # 0644
 
     def test_22_Test_Issue_gh39(self):
-        self.copy_po_file_from_template('./django.po.issue39gh.template')
+        self.copy_po_file_from_template("./django.po.issue39gh.template")
 
         r = self.client.get(self.xx_form_url)
         # We have distinct hashes, even though the msgid and msgstr are identical
-        self.assertTrue('m_4765f7de94996d3de5975fa797c3451f' in r.content.decode())
-        self.assertTrue('m_08e4e11e2243d764fc45a5a4fba5d0f2' in r.content.decode())
+        self.assertTrue("m_4765f7de94996d3de5975fa797c3451f" in r.content.decode())
+        self.assertTrue("m_08e4e11e2243d764fc45a5a4fba5d0f2" in r.content.decode())
 
-    @override_settings(ROSETTA_LANGUAGES=(('xx', 'dummy language'),))
+    @override_settings(ROSETTA_LANGUAGES=(("xx", "dummy language"),))
     def test_23_save_header_data(self):
         from django.contrib.auth.models import User
 
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
 
         unicode_user = User.objects.create_user(
-            'test_unicode', 'save_header_data@test.com', 'test_unicode'
+            "test_unicode", "save_header_data@test.com", "test_unicode"
         )
         unicode_user.first_name = "aéaéaé aàaàaàa"
         unicode_user.last_name = "aâââ üüüü"
         unicode_user.is_superuser, unicode_user.is_staff = True, True
         unicode_user.save()
 
-        self.client.login(username='test_unicode', password='test_unicode')
+        self.client.login(username="test_unicode", password="test_unicode")
 
         # Load the template file
-        r = self.client.get(self.xx_form_url + '?filter=untranslated')
+        r = self.client.get(self.xx_form_url + "?filter=untranslated")
 
         # make sure both strings are untranslated
-        self.assertTrue('dummy language' in r.content.decode())
-        self.assertTrue('String 1' in r.content.decode())
-        self.assertTrue('String 2' in r.content.decode())
-        self.assertTrue('m_e48f149a8b2e8baa81b816c0edf93890' in r.content.decode())
+        self.assertTrue("dummy language" in r.content.decode())
+        self.assertTrue("String 1" in r.content.decode())
+        self.assertTrue("String 2" in r.content.decode())
+        self.assertTrue("m_e48f149a8b2e8baa81b816c0edf93890" in r.content.decode())
 
         # post a translation
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
-        r = self.client.post(self.xx_form_url + '?filter=untranslated', data)
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
+        r = self.client.post(self.xx_form_url + "?filter=untranslated", data)
         # read the result
-        with open(self.dest_file, 'r') as f_:
+        with open(self.dest_file, "r") as f_:
             content = f_.read()
 
         # make sure unicode data was properly converted to ascii
-        self.assertTrue('Hello, world' in content)
-        self.assertTrue('save_header_data@test.com' in content)
-        self.assertTrue('aéaéaé aàaàaàa aâââ üüüü' in content)
+        self.assertTrue("Hello, world" in content)
+        self.assertTrue("save_header_data@test.com" in content)
+        self.assertTrue("aéaéaé aàaàaàa aâââ üüüü" in content)
 
     def test_24_percent_translation(self):
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
 
         # Load the template file
         r = self.client.get(self.xx_form_url)
 
-        self.assertTrue('Progress: 0%' in r.content.decode())
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
+        self.assertTrue("Progress: 0%" in r.content.decode())
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
         r = self.client.post(self.xx_form_url, data, follow=True)
-        self.assertTrue('Progress: 25%' in r.content.decode())
+        self.assertTrue("Progress: 25%" in r.content.decode())
 
     def test_25_replace_access_control(self):
         # Test default access control allows access
         response = self.client.get(self.project_file_list_url)
         self.assertEqual(200, response.status_code)
 
         # Now replace access control with a function reference,
         # and check we get redirected
-        with self.settings(ROSETTA_ACCESS_CONTROL_FUNCTION='rosetta.tests.no_access'):
+        with self.settings(ROSETTA_ACCESS_CONTROL_FUNCTION="rosetta.tests.no_access"):
             response = self.client.get(self.project_file_list_url)
             self.assertEqual(302, response.status_code)
 
         # Now replace access control with a function itself,
         # and check we get redirected
         with self.settings(ROSETTA_ACCESS_CONTROL_FUNCTION=lambda user: False):
             response = self.client.get(self.project_file_list_url)
             self.assertEqual(302, response.status_code)
 
     def test_26_urlconf_accept_dots_and_underscores(self):
-        resolver_match = resolve('/rosetta/files/all/fr_FR.utf8/0/')
-        self.assertEqual(resolver_match.url_name, 'rosetta-form')
-        self.assertEqual(resolver_match.kwargs['lang_id'], 'fr_FR.utf8')
+        resolver_match = resolve("/rosetta/files/all/fr_FR.utf8/0/")
+        self.assertEqual(resolver_match.url_name, "rosetta-form")
+        self.assertEqual(resolver_match.kwargs["lang_id"], "fr_FR.utf8")
 
     def test_27_extended_urlconf_language_code_loads_file(self):
         url = reverse(
-            'rosetta-form', kwargs={'po_filter': 'all', 'lang_id': 'fr_FR.utf8', 'idx': 0}
+            "rosetta-form",
+            kwargs={"po_filter": "all", "lang_id": "fr_FR.utf8", "idx": 0},
         )
         r = self.client.get(url)
-        self.assertTrue('French (France), UTF8' in r.content.decode())
-        self.assertTrue('m_03a603523bd75b00414a413657acdeb2' in r.content.decode())
+        self.assertTrue("French (France), UTF8" in r.content.decode())
+        self.assertTrue("m_03a603523bd75b00414a413657acdeb2" in r.content.decode())
 
     def test_28_issue_gh87(self):
         """Make sure that rosetta_i18n_catalog_filter is passed into the context."""
         r = self.client.get(self.third_party_file_list_url)
         self.assertContains(
             r, '<li class="active"><a href="/rosetta/files/third-party/">'
         )
 
     @override_settings(
-        SESSION_ENGINE='django.contrib.sessions.backends.signed_cookies',
-        ROSETTA_STORAGE_CLASS='rosetta.storage.SessionRosettaStorage',
+        SESSION_ENGINE="django.contrib.sessions.backends.signed_cookies",
+        ROSETTA_STORAGE_CLASS="rosetta.storage.SessionRosettaStorage",
     )
     def test_29_unsupported_p3_django_16_storage(self):
         if VERSION[0:2] < (2, 0):
             self.assertTrue(
-                'django.contrib.sessions.middleware.SessionMiddleware'
+                "django.contrib.sessions.middleware.SessionMiddleware"
                 in settings.MIDDLEWARE
             )
 
             # Force caching to be used by making the pofile read-only
             os.chmod(self.dest_file, 292)  # 0444
 
             # (Have to log in again, since our session engine changed)
-            self.client.login(username='test_admin', password='test_password')
+            self.client.login(username="test_admin", password="test_password")
 
             with self.assertRaises(ImproperlyConfigured):
                 self.client.get(self.xx_form_url)
 
             # Cleanup
             os.chmod(self.dest_file, 420)  # 0644
 
     @override_settings(
-        ROSETTA_POFILENAMES=('pr44.po',), ROSETTA_LANGUAGES=(('xx', 'dummy language'),)
+        ROSETTA_POFILENAMES=("pr44.po",), ROSETTA_LANGUAGES=(("xx", "dummy language"),)
     )
     def test_30_pofile_names(self):
         os.unlink(self.dest_file)
         destfile = os.path.normpath(
-            os.path.join(self.curdir, '../locale/xx/LC_MESSAGES/pr44.po')
+            os.path.join(self.curdir, "../locale/xx/LC_MESSAGES/pr44.po")
         )
         shutil.copy(
-            os.path.normpath(os.path.join(self.curdir, './pr44.po.template')), destfile
+            os.path.normpath(os.path.join(self.curdir, "./pr44.po.template")), destfile
         )
 
         r = self.client.get(self.third_party_file_list_url)
-        self.assertTrue('xx/LC_MESSAGES/pr44.po' in r.content.decode())
+        self.assertTrue("xx/LC_MESSAGES/pr44.po" in r.content.decode())
 
         r = self.client.get(self.xx_form_url)
-        self.assertTrue('dummy language' in r.content.decode())
+        self.assertTrue("dummy language" in r.content.decode())
 
         # (Clean up)
         os.unlink(destfile)
 
     def test_31_pr_102__exclude_paths(self):
         r = self.client.get(self.third_party_file_list_url)
-        self.assertContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
-        exclude_path = os.path.normpath(os.path.join(self.curdir, '../locale'))
+        self.assertContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
+        exclude_path = os.path.normpath(os.path.join(self.curdir, "../locale"))
         with self.settings(ROSETTA_EXCLUDED_PATHS=exclude_path):
             r = self.client.get(self.third_party_file_list_url)
-            self.assertNotContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+            self.assertNotContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
 
     def test_32_pr_103__language_groups(self):
-        from django.contrib.auth.models import User, Group
+        from django.contrib.auth.models import Group, User
 
         # Default behavior: non-admins need to be in a translators group; they
         # see all catalogs
-        translators = Group.objects.create(name='translators')
-        translators_xx = Group.objects.create(name='translators-xx')
+        translators = Group.objects.create(name="translators")
+        translators_xx = Group.objects.create(name="translators-xx")
 
-        user4 = User.objects.create_user('test_admin4', 'test@test3.com', 'test_password')
+        user4 = User.objects.create_user(
+            "test_admin4", "test@test3.com", "test_password"
+        )
         user4.groups.add(translators)
         user4.is_superuser = False
         user4.is_staff = True
         user4.save()
 
         with self.settings(ROSETTA_LANGUAGE_GROUPS=False):
-            self.client.login(username='test_admin4', password='test_password')
+            self.client.login(username="test_admin4", password="test_password")
             r = self.client.get(self.third_party_file_list_url)
-            self.assertContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+            self.assertContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
 
         with self.settings(ROSETTA_LANGUAGE_GROUPS=True):
             r = self.client.get(self.third_party_file_list_url)
-            self.assertNotContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+            self.assertNotContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
             # Now add them to the custom group
             user4.groups.add(translators_xx)
             r = self.client.get(self.third_party_file_list_url)
-            self.assertContains(r, 'rosetta/locale/xx/LC_MESSAGES/django.po')
+            self.assertContains(r, "rosetta/locale/xx/LC_MESSAGES/django.po")
 
     @override_settings(
-        ROSETTA_ENABLE_REFLANG=True, ROSETTA_LANGUAGES=(('xx', 'dummy language'),)
+        ROSETTA_ENABLE_REFLANG=True, ROSETTA_LANGUAGES=(("xx", "dummy language"),)
     )
     def test_33_reflang(self):
-        self.copy_po_file_from_template('./django.po.issue60.template')
+        self.copy_po_file_from_template("./django.po.issue60.template")
         r = self.client.get(self.xx_form_url)
 
         # Verify that there's an option to select a reflang
         self.assertTrue(
             '<option value="?ref_lang=xx">dummy language</option>' in r.content.decode()
         )
 
-        r = self.client.get(self.xx_form_url + '?ref_lang=xx')
+        r = self.client.get(self.xx_form_url + "?ref_lang=xx")
         # The translated string in the test PO file ends up in the "Reference" column
         self.assertTrue(
             '<span class="message">translated-string1</span>' in r.content.decode()
         )
 
     def test_show_occurrences(self):
         r = self.client.get(self.xx_form_url)
@@ -669,102 +678,105 @@
             # Verify that occurrences not in view
             self.assertFalse('<td class="location">' in r.content.decode())
 
     def test_34_issue_113_app_configs(self):
         r = self.client.get(self.all_file_list_url)
         self.assertTrue('rosetta/files/all/xx/1/">Test_App' in r.content.decode())
 
-    @override_settings(ROSETTA_STORAGE_CLASS='rosetta.storage.CacheRosettaStorage')
+    @override_settings(ROSETTA_STORAGE_CLASS="rosetta.storage.CacheRosettaStorage")
     def test_35_issue_135_display_exception_messages(self):
         # Note: the old version of this test looked for a 'Permission denied'
         # message reflected in the response. That behavior has now changed so
         # that changes that can't be persisted through the filesystem .po file
         # are saved to the cached version of the .po file.
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
 
-        r = self.client.get(self.xx_form_url + '?msg_filter=untranslated')
-        self.assertContains(r, 'm_e48f149a8b2e8baa81b816c0edf93890')
+        r = self.client.get(self.xx_form_url + "?msg_filter=untranslated")
+        self.assertContains(r, "m_e48f149a8b2e8baa81b816c0edf93890")
 
         # make the pofile read-only
         os.chmod(self.dest_file, 292)  # 0444
 
         # post a translation
-        data = {'m_e48f149a8b2e8baa81b816c0edf93890': 'Hello, world'}
+        data = {"m_e48f149a8b2e8baa81b816c0edf93890": "Hello, world"}
         self.client.post(self.xx_form_url, data, follow=True)
 
         # Confirm that the filesystem file hasn't changed
-        tmpl_path = os.path.normpath(os.path.join(self.curdir, 'django.po.template'))
+        tmpl_path = os.path.normpath(os.path.join(self.curdir, "django.po.template"))
         self.assertTrue(filecmp.cmp(tmpl_path, self.dest_file))
 
         # Confirm that the cached version has been updated
-        cache_key = 'po-file-%s' % self.dest_file
+        cache_key = "po-file-%s" % self.dest_file
         request = RequestFactory().get(self.xx_form_url)
         request.user = self.user
         request.session = self.client.session
         storage = get_storage(request)
 
         po_file = storage.get(cache_key)
-        entry = po_file.find('String 2')
-        self.assertEqual(entry.msgstr, 'Hello, world')
+        entry = po_file.find("String 2")
+        self.assertEqual(entry.msgstr, "Hello, world")
 
         # cleanup
         os.chmod(self.dest_file, 420)  # 0644
 
     def test_36_issue_142_complex_locales(self):
         r = self.client.get(self.all_file_list_url)
-        self.assertContains(r, 'locale/bs-Cyrl-BA/LC_MESSAGES/django.po')
+        self.assertContains(r, "locale/bs-Cyrl-BA/LC_MESSAGES/django.po")
 
-    @override_settings(ROSETTA_LANGUAGES=(('yy-Anot', u'Yet Another dummy language'),))
+    @override_settings(ROSETTA_LANGUAGES=(("yy-Anot", "Yet Another dummy language"),))
     def test_37_issue_133_complex_locales(self):
         r = self.client.get(self.all_file_list_url)
-        self.assertContains(r, 'locale/yy-Anot/LC_MESSAGES/django.po')
+        self.assertContains(r, "locale/yy-Anot/LC_MESSAGES/django.po")
 
     def test_38_issue_161_more_weird_locales(self):
         r = self.client.get(self.all_file_list_url)
-        self.assertTrue(r, 'locale/zh_Hans/LC_MESSAGES/django.po')
+        self.assertTrue(r, "locale/zh_Hans/LC_MESSAGES/django.po")
 
     def test_39_invalid_get_page(self):
-        url = self.xx_form_url + '?filter=untranslated'
+        url = self.xx_form_url + "?filter=untranslated"
 
         r = self.client.get(url)  # Page not specified
-        self.assertEqual(r.context['page'], 1)
+        self.assertEqual(r.context["page"], 1)
 
-        r = self.client.get(url + '&page=')  # No number given
-        self.assertEqual(r.context['page'], 1)
+        r = self.client.get(url + "&page=")  # No number given
+        self.assertEqual(r.context["page"], 1)
 
-        r = self.client.get(url + '&page=9999')  # Too-high number given
-        self.assertEqual(r.context['page'], 1)
+        r = self.client.get(url + "&page=9999")  # Too-high number given
+        self.assertEqual(r.context["page"], 1)
 
-        r = self.client.get(url + '&page=x')  # Non-number given
-        self.assertEqual(r.context['page'], 1)
+        r = self.client.get(url + "&page=x")  # Non-number given
+        self.assertEqual(r.context["page"], 1)
 
     def test_40_issue_155_auto_compile(self):
         def file_hash(file_string):
             with open(file_string, encoding="latin-1") as file:
-                file_content = file.read().encode('utf-8')
+                file_content = file.read().encode("utf-8")
             return hashlib.md5(file_content).hexdigest()
 
         def message_hashes():
             r = self.client.get(self.xx_form_url)
-            return {m.msgid: 'm_' + m.md5hash for m in r.context['rosetta_messages']}
+            return {m.msgid: "m_" + m.md5hash for m in r.context["rosetta_messages"]}
 
         po_file = self.dest_file
-        mo_file = self.dest_file[:-3] + '.mo'
+        mo_file = self.dest_file[:-3] + ".mo"
 
         # MO file will be compiled by default.
         # Get PO and MO files into an initial reference state (MO will be
         # created or updated)
         msg_hashes = message_hashes()
-        data = {msg_hashes['String 1']: 'Translation 1'}
+        data = {msg_hashes["String 1"]: "Translation 1"}
         self.client.post(self.xx_form_url, data)
-        po_file_hash_before, mo_file_hash_before = file_hash(po_file), file_hash(mo_file)
+        po_file_hash_before, mo_file_hash_before = (
+            file_hash(po_file),
+            file_hash(mo_file),
+        )
 
         # Make a change to the translations
         msg_hashes = message_hashes()
-        data = {msg_hashes['String 1']: 'Translation 2'}
+        data = {msg_hashes["String 1"]: "Translation 2"}
         self.client.post(self.xx_form_url, data)
 
         # Get the new hashes of the PO and MO file contents
         po_file_hash_after, mo_file_hash_after = file_hash(po_file), file_hash(mo_file)
 
         # Both the PO and MO should have changed
         self.assertNotEqual(po_file_hash_before, po_file_hash_after)
@@ -774,15 +786,15 @@
         with self.settings(ROSETTA_AUTO_COMPILE=False):
             # Make a change to the translations
             po_file_hash_before, mo_file_hash_before = (
                 po_file_hash_after,
                 mo_file_hash_after,
             )
             msg_hashes = message_hashes()
-            data = {msg_hashes['String 1']: "Translation 3"}
+            data = {msg_hashes["String 1"]: "Translation 3"}
             self.client.post(self.xx_form_url, data)
             po_file_hash_after, mo_file_hash_after = (
                 file_hash(po_file),
                 file_hash(mo_file),
             )
 
             # Only the PO should have changed, the MO should be unchanged
@@ -791,15 +803,15 @@
 
             # Verify that translating another string also leaves the MO unchanged
             po_file_hash_before, mo_file_hash_before = (
                 po_file_hash_after,
                 mo_file_hash_after,
             )
             msg_hashes = message_hashes()
-            data = {msg_hashes['String 2']: "Translation 4"}
+            data = {msg_hashes["String 2"]: "Translation 4"}
             self.client.post(self.xx_form_url, data)
             po_file_hash_after, mo_file_hash_after = (
                 file_hash(po_file),
                 file_hash(mo_file),
             )
 
             self.assertNotEqual(po_file_hash_before, po_file_hash_after)
@@ -807,27 +819,27 @@
 
         with self.settings(ROSETTA_AUTO_COMPILE=True):
             po_file_hash_before, mo_file_hash_before = (
                 po_file_hash_after,
                 mo_file_hash_after,
             )
             msg_hashes = message_hashes()
-            data = {msg_hashes['String 2']: "Translation 5"}
+            data = {msg_hashes["String 2"]: "Translation 5"}
             self.client.post(self.xx_form_url, data)
             po_file_hash_after, mo_file_hash_after = (
                 file_hash(po_file),
                 file_hash(mo_file),
             )
 
             self.assertNotEqual(po_file_hash_before, po_file_hash_after)
             self.assertNotEqual(mo_file_hash_before, mo_file_hash_after)
 
     def test_41_pr_176_embed_in_admin(self):
-        resp = self.client.get(reverse('admin:index'))
-        self.assertContains(resp, 'app-rosetta module')
+        resp = self.client.get(reverse("admin:index"))
+        self.assertContains(resp, "app-rosetta module")
 
     def _setup_view(self, view, request, *args, **kwargs):
         """Mimic as_view() returned callable, but returns view instance.
 
         args and kwargs are the same you would pass to ``reverse()``
         (From http://tech.novapost.fr/django-unit-test-your-views-en.html.)
         """
@@ -836,20 +848,20 @@
         view.kwargs = kwargs
         return view
 
     def test_42_view_property_po_file_is_writable(self):
         """Confirm that we're accurately determining the filesystem write-perms
         on our .po file.
         """
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
 
         # By default, we're writable
         request = RequestFactory().get(self.xx_form_url)
         request.user = self.user
-        kwargs = {'po_filter': 'third-party', 'lang_id': 'xx', 'idx': 0}
+        kwargs = {"po_filter": "third-party", "lang_id": "xx", "idx": 0}
         view = self._setup_view(
             view=views.TranslationFormView(), request=request, **kwargs
         )
         self.assertTrue(view.po_file_is_writable)
 
         # Now try again with the file not writable. (Regenerate the view, since
         # this po_file_is_writable is cached for the life of the request.)
@@ -863,207 +875,206 @@
         # Cleanup
         os.chmod(self.dest_file, 420)  # 0644
 
     def test_43_view_property_po_file_path(self):
         """Confirm our class-based views properly parse/validate the path of the
         .po file in question derived from the url kwargs.
         """
-        self.copy_po_file_from_template('./django.po.template')
+        self.copy_po_file_from_template("./django.po.template")
 
         # By default, when all goes well, we get our existing .po file path
         request = RequestFactory().get(self.xx_form_url)
         request.user = self.user
-        kwargs = {'po_filter': 'third-party', 'lang_id': 'xx', 'idx': 0}
+        kwargs = {"po_filter": "third-party", "lang_id": "xx", "idx": 0}
         view = self._setup_view(
             view=views.TranslationFormView(), request=request, **kwargs
         )
         self.assertEqual(view.po_file_path, self.dest_file)
 
         # But if the language isn't an option, we get a 404
         with self.settings(
-            ROSETTA_LANGUAGES=[lang for lang, __ in settings.LANGUAGES if lang != 'xx']
+            ROSETTA_LANGUAGES=[lang for lang, __ in settings.LANGUAGES if lang != "xx"]
         ):
             view = self._setup_view(
                 view=views.TranslationFormView(), request=request, **kwargs
             )
             with self.assertRaises(Http404):
                 view.po_file_path
 
         # And if the index doesn't correspond with a file, we get a 404
-        new_kwargs = {'po_filter': 'third-party', 'lang_id': 'xx', 'idx': 9}
+        new_kwargs = {"po_filter": "third-party", "lang_id": "xx", "idx": 9}
         view = self._setup_view(
             view=views.TranslationFormView(),
             # Recycle request, even though url kwargs conflict with ones below.
             request=request,
-            **new_kwargs
+            **new_kwargs,
         )
         with self.assertRaises(Http404):
             view.po_file_path
 
     def test_44_message_search_function(self):
         """Confirm that search of the .po file works across the various message
         fields.
         """
-        self.copy_po_file_from_template('./django.po.test44.template')
-        url = self.xx_form_url + '?query=%s'
+        self.copy_po_file_from_template("./django.po.test44.template")
+        url = self.xx_form_url + "?query=%s"
 
         # Here's the message entry we're considering:
         # #. Translators: consectetur adipisicing
         # #: templates/eiusmod/tempor.html:43
         # msgid "Lorem ipsum"
         # msgstr "dolor sit amet"
         # It is buried at the end of the file, so without searching for it, it
         # shouldn't be on the page
-        r = self.client.get(url % '')
-        self.assertNotContains(r, 'Lorem')
+        r = self.client.get(url % "")
+        self.assertNotContains(r, "Lorem")
 
         # Search msgid
-        r = self.client.get(url % 'ipsum')
-        self.assertContains(r, 'Lorem')
+        r = self.client.get(url % "ipsum")
+        self.assertContains(r, "Lorem")
 
         # Search msgstr
-        r = self.client.get(url % 'dolor')
-        self.assertContains(r, 'Lorem')
+        r = self.client.get(url % "dolor")
+        self.assertContains(r, "Lorem")
 
         # Search occurences
-        r = self.client.get(url % 'tempor')
-        self.assertContains(r, 'Lorem')
+        r = self.client.get(url % "tempor")
+        self.assertContains(r, "Lorem")
 
         # Search comments
-        r = self.client.get(url % 'adipisicing')
-        self.assertContains(r, 'Lorem')
+        r = self.client.get(url % "adipisicing")
+        self.assertContains(r, "Lorem")
 
         # Search context
-        r = self.client.get(url % 'pellentesque')
-        self.assertContains(r, 'Lorem')
+        r = self.client.get(url % "pellentesque")
+        self.assertContains(r, "Lorem")
 
     def test_45_issue186_plural_msg_search(self):
         """Confirm that search of the .po file works for plurals."""
-        self.copy_po_file_from_template('./django.po.issue186.template')
-        url = self.xx_form_url + '?query=%s'
+        self.copy_po_file_from_template("./django.po.issue186.template")
+        url = self.xx_form_url + "?query=%s"
 
         # Here's the message entry we're considering:
         # msgstr "%d Child"
         # msgid_plural "%d Childrenen"
         # msgstr[0] "%d Tchilt"
         # msgstr[1] "%d Tchildren"
 
         # First, confirm that we don't ALWAYS see this particular message on the
         # page.
-        r = self.client.get(url % 'kids')
-        self.assertNotContains(r, 'Child')
+        r = self.client.get(url % "kids")
+        self.assertNotContains(r, "Child")
 
         # Search msgid_plural
-        r = self.client.get(url % 'childrenen')
-        self.assertContains(r, 'Child')
+        r = self.client.get(url % "childrenen")
+        self.assertContains(r, "Child")
 
         # Search msgstr[0]
-        r = self.client.get(url % 'tchilt')
-        self.assertContains(r, 'Child')
+        r = self.client.get(url % "tchilt")
+        self.assertContains(r, "Child")
 
         # Search msgstr[1]
-        r = self.client.get(url % 'tchildren')
-        self.assertContains(r, 'Child')
+        r = self.client.get(url % "tchildren")
+        self.assertContains(r, "Child")
 
     def test_46_search_string_with_unicode_symbols(self):
         """Confirm that search works with unicode symbols"""
-        url = self.xx_form_url + '?' + urlencode({'query': force_bytes(u'Лорем')})
+        url = self.xx_form_url + "?" + urlencode({"query": force_bytes("Лорем")})
 
         # It shouldn't raise
         r = self.client.get(url)
         self.assertEqual(r.status_code, 200)
 
     @vcr.use_cassette(
-        'fixtures/vcr_cassettes/test_47_azure_ajax_translation.yaml',
-        match_on=['method', 'scheme', 'host', 'port', 'path', 'query', 'raw_body'],
-        record_mode='new_episodes',
+        "fixtures/vcr_cassettes/test_47_azure_ajax_translation.yaml",
+        match_on=["method", "scheme", "host", "port", "path", "query", "raw_body"],
+        record_mode="once",
     )
     @override_settings(DEEPL_AUTH_KEY=None, AZURE_CLIENT_SECRET="FAKE")
     def test_47_azure_ajax_translation(self):
         r = self.client.get(
-            reverse('rosetta.translate_text') + '?from=en&to=fr&text=hello%20world'
+            reverse("rosetta.translate_text") + "?from=en&to=fr&text=hello%20world"
+        )
+        self.assertContains(r, '"Salut tout le monde"')
+
+    @vcr.use_cassette(
+        "fixtures/vcr_cassettes/test_47_2_deeps_ajax_translation.yaml",
+        match_on=["method", "scheme", "host", "port", "path", "query", "raw_body"],
+        record_mode="once",
+    )
+    @override_settings(DEEPL_AUTH_KEY="FAKE", AZURE_CLIENT_SECRET=None)
+    def test_47_2_deeps_ajax_translation(self):
+        r = self.client.get(
+            reverse("rosetta.translate_text") + "?from=en&to=fr&text=hello%20world"
         )
         self.assertContains(r, '"Salut tout le monde"')
 
     @override_settings(ROSETTA_REQUIRES_AUTH=True)
     def test_48_requires_auth_not_respected_issue_203(self):
         self.client.logout()
         r = self.client.get(self.all_file_list_url)
         self.assertRedirects(
             r,
-            '{}?next=/rosetta/files/all/'.format(settings.LOGIN_URL),
+            "{}?next=/rosetta/files/all/".format(settings.LOGIN_URL),
             fetch_redirect_response=False,
         )
         self.assertEqual(302, r.status_code)
 
     @override_settings(ROSETTA_REQUIRES_AUTH=False)
     def test_49_requires_auth_not_respected_issue_203(self):
         r = self.client.get(self.all_file_list_url)
         self.assertEqual(200, r.status_code)
 
-    @override_settings(ROSETTA_REQUIRES_AUTH=True, ROSETTA_LOGIN_URL='/custom-url/')
+    @override_settings(ROSETTA_REQUIRES_AUTH=True, ROSETTA_LOGIN_URL="/custom-url/")
     def test_50_custom_login_url(self):
         self.client.logout()
         r = self.client.get(self.all_file_list_url)
         self.assertRedirects(
-            r, '/custom-url/?next=/rosetta/files/all/', fetch_redirect_response=False
+            r, "/custom-url/?next=/rosetta/files/all/", fetch_redirect_response=False
         )
         self.assertEqual(302, r.status_code)
 
     def test_51_rosetta_languages(self):
-        self.assertTrue('xx' in dict(settings.LANGUAGES))
-        self.assertFalse('yy' in dict(settings.LANGUAGES))
+        self.assertTrue("xx" in dict(settings.LANGUAGES))
+        self.assertFalse("yy" in dict(settings.LANGUAGES))
 
-        with self.settings(ROSETTA_LANGUAGES=(('xx', 'foo language'),)):
+        with self.settings(ROSETTA_LANGUAGES=(("xx", "foo language"),)):
             r = self.client.get(self.project_file_list_url)
-            self.assertTrue('foo language' in r.content.decode())
-            self.assertFalse('bar language' in r.content.decode())
+            self.assertTrue("foo language" in r.content.decode())
+            self.assertFalse("bar language" in r.content.decode())
 
         with self.settings(
-            ROSETTA_LANGUAGES=(('xx', 'foo language'), ('yy', 'bar language'))
+            ROSETTA_LANGUAGES=(("xx", "foo language"), ("yy", "bar language"))
         ):
             r = self.client.get(self.project_file_list_url)
-            self.assertTrue('foo language' in r.content.decode())
-            self.assertTrue('bar language' in r.content.decode())
-
-    def test_52_deepl_languages_handled_correctly(self):
-        """
-        If DEEPL_LANGUAGES set in settings, we use that one, if not, we use django's language code.
-        """
-        if settings.DEEPL_AUTH_KEY:
-            with self.settings(DEEPL_LANGUAGES={"fr_FR.utf8": "FR"}):
-                r = self.client.get(
-                    reverse(
-                        "rosetta-form",
-                        kwargs={
-                            "po_filter": "project",
-                            "lang_id": "fr_FR.utf8",
-                            "idx": "0",
-                        },
-                    )
-                )
-                self.assertContains(r, "var destLangRoot = 'FR'")
-            with self.settings(DEEPL_LANGUAGES=None):
-                r = self.client.get(
-                    reverse(
-                        "rosetta-form",
-                        kwargs={
-                            "po_filter": "project",
-                            "lang_id": "fr_FR.utf8",
-                            "idx": "0",
-                        },
-                    )
-                )
-                self.assertContains(r, "var destLangRoot = 'fr-FR.utf8'.substring(0, 2)")
+            self.assertTrue("foo language" in r.content.decode())
+            self.assertTrue("bar language" in r.content.decode())
 
     def test_198_embed_in_admin_access_control(self):
-        resp = self.client.get(reverse('admin:index'))
-        self.assertContains(resp, 'rosetta-content-main')
+        resp = self.client.get(reverse("admin:index"))
+        self.assertContains(resp, "rosetta-content-main")
 
         with self.settings(ROSETTA_ACCESS_CONTROL_FUNCTION=lambda user: False):
-            resp = self.client.get(reverse('admin:index'))
-            self.assertNotContains(resp, 'rosetta-content-main')
+            resp = self.client.get(reverse("admin:index"))
+            self.assertNotContains(resp, "rosetta-content-main")
+
+    @mock.patch("rosetta.poutil.os.path.exists")
+    def test_273_override_case_sensitivity(self, path_mock):
+        path_mock.exists.return_value = False
+        # no setting
+        find_pos("en")
+        path_mock.assert_called_with(mock.ANY)
+
+        path_mock.reset_mock()
+        with override_settings(ROSETTA_CASE_SENSITIVE_FILESYSTEM=False):
+            find_pos("en")
+            path_mock.isfile.assert_not_called()
+
+        path_mock.reset_mock()
+        with override_settings(ROSETTA_CASE_SENSITIVE_FILESYSTEM=True):
+            find_pos("en")
+            path_mock.isfile.assert_not_called()
 
 
 # Stubbed access control function
 def no_access(user):
     return False
```

### Comparing `django-rosetta-0.9.8/rosetta/translate_utils.py` & `django-rosetta-0.9.9/rosetta/translate_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,87 @@
 import json
 import uuid
 
-from django.conf import settings
-
 import requests
 
+from django.conf import settings
+
 
 class TranslationException(Exception):
     pass
 
 
 def translate(text, from_language, to_language):
-    AZURE_CLIENT_SECRET = getattr(settings, 'AZURE_CLIENT_SECRET', None)
+    AZURE_CLIENT_SECRET = getattr(settings, "AZURE_CLIENT_SECRET", None)
     GOOGLE_APPLICATION_CREDENTIALS_PATH = getattr(
-        settings, 'GOOGLE_APPLICATION_CREDENTIALS_PATH', None
+        settings, "GOOGLE_APPLICATION_CREDENTIALS_PATH", None
     )
-    GOOGLE_PROJECT_ID = getattr(settings, 'GOOGLE_PROJECT_ID', None)
+    GOOGLE_PROJECT_ID = getattr(settings, "GOOGLE_PROJECT_ID", None)
+    DEEPL_AUTH_KEY = getattr(settings, "DEEPL_AUTH_KEY", None)
 
-    if AZURE_CLIENT_SECRET:
+    if DEEPL_AUTH_KEY:
+        deepl_language_code = None
+        DEEPL_LANGUAGES = getattr(settings, "DEEPL_LANGUAGES", None)
+        if type(DEEPL_LANGUAGES) is dict:
+            deepl_language_code = DEEPL_LANGUAGES.get(to_language, None)
+
+        if deepl_language_code is None:
+            deepl_language_code = to_language[:2].upper()
+
+        return translate_by_deepl(
+            text,
+            deepl_language_code.upper(),
+            DEEPL_AUTH_KEY,
+        )
+
+    elif AZURE_CLIENT_SECRET:
         return translate_by_azure(text, from_language, to_language, AZURE_CLIENT_SECRET)
     elif GOOGLE_APPLICATION_CREDENTIALS_PATH and GOOGLE_PROJECT_ID:
         return translate_by_google(
             text,
             from_language,
             to_language,
             GOOGLE_APPLICATION_CREDENTIALS_PATH,
             GOOGLE_PROJECT_ID,
         )
     else:
-        raise TranslationException('No translation API service is configured.')
+        raise TranslationException("No translation API service is configured.")
+
+
+def translate_by_deepl(text, to_language, auth_key):
+    r = requests.post(
+        "https://api-free.deepl.com/v2/translate",
+        headers={"Authorization": f"DeepL-Auth-Key {auth_key}"},
+        data={
+            "target_lang": to_language.upper(),
+            "text": text,
+        },
+    )
+    return r.json().get("translations")[0].get("text")
 
 
 def translate_by_azure(text, from_language, to_language, subscription_key):
     """
     This method does the heavy lifting of connecting to the translator API and fetching a response
     :param text: The source text to be translated
     :param from_language: The language of the source text
     :param to_language: The target language to translate the text into
     :param subscription_key: An API key that grants you access to the Azure translation service
     :return: Returns the response from the AZURE service as a python object. For more information about the
     response, please visit
     https://docs.microsoft.com/en-us/azure/cognitive-services/translator/reference/v3-0-translate?tabs=curl
     """
 
-    AZURE_TRANSLATOR_HOST = 'https://api.cognitive.microsofttranslator.com'
-    AZURE_TRANSLATOR_PATH = '/translate?api-version=3.0'
+    AZURE_TRANSLATOR_HOST = "https://api.cognitive.microsofttranslator.com"
+    AZURE_TRANSLATOR_PATH = "/translate?api-version=3.0"
 
     headers = {
-        'Ocp-Apim-Subscription-Key': subscription_key,
-        'Content-type': 'application/json',
-        'X-ClientTraceId': str(uuid.uuid4()),
+        "Ocp-Apim-Subscription-Key": subscription_key,
+        "Content-type": "application/json",
+        "X-ClientTraceId": str(uuid.uuid4()),
     }
 
     url_parameters = {"from": from_language, "to": to_language}
 
     request_data = [{"text": text}]
 
     api_hostname = AZURE_TRANSLATOR_HOST + AZURE_TRANSLATOR_PATH
@@ -108,22 +136,22 @@
     text, input_language, output_language, creadentials_path, project_id
 ):
     from google.cloud import translate as google_translate
 
     client = google_translate.TranslationServiceClient.from_service_account_json(
         creadentials_path
     )
-    parent = "projects/{}/locations/{}".format(project_id, 'global')
+    parent = "projects/{}/locations/{}".format(project_id, "global")
     try:
         api_response = client.translate_text(
             request=dict(
                 parent=parent,
                 contents=[text],
-                mime_type='text/plain',
+                mime_type="text/plain",
                 source_language_code=input_language,
-                target_language_code=output_language.split('.', 1)[0],
+                target_language_code=output_language.split(".", 1)[0],
             )
         )
     except Exception as e:
-        raise TranslationException('Google API error: {}'.format(e))
+        raise TranslationException("Google API error: {}".format(e))
     else:
         return str(api_response.translations[0].translated_text)
```

### Comparing `django-rosetta-0.9.8/rosetta/views.py` & `django-rosetta-0.9.9/rosetta/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,54 +2,54 @@
 import os
 import os.path
 import re
 import zipfile
 from io import BytesIO
 from urllib.parse import urlencode
 
+from polib import pofile
+
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth.decorators import user_passes_test
 from django.core.paginator import Paginator
-from django.http import (Http404, HttpResponse, HttpResponseRedirect,
-                         JsonResponse)
+from django.http import Http404, HttpResponse, HttpResponseRedirect, JsonResponse
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.encoding import force_bytes
 from django.utils.functional import Promise, cached_property
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.cache import never_cache
 from django.views.generic import TemplateView, View
-from polib import pofile
 
 from . import get_version as get_rosetta_version
 from .access import can_translate, can_translate_language
 from .conf import settings as rosetta_settings
 from .poutil import find_pos, pagination_range, timestamp_with_timezone
 from .signals import entry_changed, post_save
 from .storage import get_storage
 from .translate_utils import TranslationException, translate
 
 
 def get_app_name(path):
-    return path.split('/locale')[0].split('/')[-1]
+    return path.split("/locale")[0].split("/")[-1]
 
 
 class LoginURL(Promise):
     """
     Tests friendly login URL, url is resolved at runtime.
     """
 
     def __str__(self):
         return rosetta_settings.LOGIN_URL
 
 
-@method_decorator(never_cache, 'dispatch')
+@method_decorator(never_cache, "dispatch")
 @method_decorator(
-    user_passes_test(lambda user: can_translate(user), LoginURL()), 'dispatch'
+    user_passes_test(lambda user: can_translate(user), LoginURL()), "dispatch"
 )
 class RosettaBaseMixin(object):
     """A mixin class for Rosetta's class-based views. It provides:
     * security (see class decorators)
     * a property for the 'po_filter' url argument
     """
 
@@ -60,16 +60,16 @@
     def po_filter(self):
         """Return the filter applied to all of the .po files under consideration
         to determine which file is currently being translated. Options are:
         'all', 'django', 'third-party', 'project'.
 
         If the filter isn't in this list, throw a 404.
         """
-        po_filter = self.kwargs.get('po_filter')
-        if po_filter not in {'all', 'django', 'third-party', 'project'}:
+        po_filter = self.kwargs.get("po_filter")
+        if po_filter not in {"all", "django", "third-party", "project"}:
             raise Http404
         return po_filter
 
 
 class RosettaFileLevelMixin(RosettaBaseMixin):
     """Mixin for dealing with views that work specifically with a single
     .po file. In addition to what the super class brings, it adds the following
@@ -93,35 +93,35 @@
         validating that:
         1. the language is in rosetta_settings.ROSETTA_LANGUAGES, and
         2. the current user is permitted to translate that language
 
         (If either of the above fail, throw a 404.)
         """
         # (Formerly known as "rosetta_i18n_lang_code")
-        lang_id = self.kwargs['lang_id']
+        lang_id = self.kwargs["lang_id"]
         if lang_id not in {lang[0] for lang in rosetta_settings.ROSETTA_LANGUAGES}:
             raise Http404
         if not can_translate_language(self.request.user, lang_id):
             raise Http404
         return lang_id
 
     @cached_property
     def po_file_path(self):
         """Based on the url kwargs, infer and return the path to the .po file to
         be shown/updated.
 
         Throw a 404 if a file isn't found.
         """
         # This was formerly referred to as 'rosetta_i18n_fn'
-        idx = self.kwargs['idx']
+        idx = self.kwargs["idx"]
         idx = int(idx)  # idx matched url re expression; calling int() is safe
 
-        third_party_apps = self.po_filter in ('all', 'third-party')
-        django_apps = self.po_filter in ('all', 'django')
-        project_apps = self.po_filter in ('all', 'project')
+        third_party_apps = self.po_filter in ("all", "third-party")
+        django_apps = self.po_filter in ("all", "django")
+        project_apps = self.po_filter in ("all", "project")
 
         po_paths = find_pos(
             self.language_id,
             project_apps=project_apps,
             django_apps=django_apps,
             third_party_apps=third_party_apps,
         )
@@ -149,40 +149,40 @@
             )
             for entry in po_file:
                 # Entry is an object representing a single entry in the catalog.
                 # We iterate through the *entire catalog*, pasting a hashed
                 # value of the meat of each entry on its side in an attribute
                 # called "md5hash".
                 str_to_hash = (
-                    str(entry.msgid) + str(entry.msgstr) + str(entry.msgctxt or '')
-                ).encode('utf8')
+                    str(entry.msgid) + str(entry.msgstr) + str(entry.msgctxt or "")
+                ).encode("utf8")
                 entry.md5hash = hashlib.md5(str_to_hash).hexdigest()
         else:
             storage = get_storage(self.request)
             po_file = storage.get(self.po_file_cache_key, None)
             if not po_file:
                 po_file = pofile(self.po_file_path)
                 for entry in po_file:
                     # Entry is an object representing a single entry in the
                     # catalog. We iterate through the entire catalog, pasting
                     # a hashed value of the meat of each entry on its side in
                     # an attribute called "md5hash".
                     str_to_hash = (
-                        str(entry.msgid) + str(entry.msgstr) + str(entry.msgctxt or '')
-                    ).encode('utf8')
-                    entry.md5hash = hashlib.new('md5', str_to_hash).hexdigest()
+                        str(entry.msgid) + str(entry.msgstr) + str(entry.msgctxt or "")
+                    ).encode("utf8")
+                    entry.md5hash = hashlib.new("md5", str_to_hash).hexdigest()
                 storage.set(self.po_file_cache_key, po_file)
         return po_file
 
     @cached_property
     def po_file_cache_key(self):
         """Return the cache key used to save/access the .po file (when actually
         persisted in cache).
         """
-        return 'po-file-%s' % self.po_file_path
+        return "po-file-%s" % self.po_file_path
 
     @cached_property
     def po_file_is_writable(self):
         """Return True if we're able (in terms of file system permissions) to
         write out changes to the .po file we're translating.
         """
         # (This was formerly called 'rosetta_i18n_write'.)
@@ -190,23 +190,23 @@
 
 
 class TranslationFileListView(RosettaBaseMixin, TemplateView):
     """Lists the languages, the gettext catalog files that can be translated,
     and their translation progress for a filtered list of apps/projects.
     """
 
-    http_method_names = ['get']
-    template_name = 'rosetta/file-list.html'
+    http_method_names = ["get"]
+    template_name = "rosetta/file-list.html"
 
     def get_context_data(self, **kwargs):
         context = super(TranslationFileListView, self).get_context_data(**kwargs)
 
-        third_party_apps = self.po_filter in ('all', 'third-party')
-        django_apps = self.po_filter in ('all', 'django')
-        project_apps = self.po_filter in ('all', 'project')
+        third_party_apps = self.po_filter in ("all", "third-party")
+        django_apps = self.po_filter in ("all", "django")
+        project_apps = self.po_filter in ("all", "project")
 
         languages = []
         has_pos = False
         for language in rosetta_settings.ROSETTA_LANGUAGES:
             if not can_translate_language(self.request.user, language[0]):
                 continue
 
@@ -220,18 +220,18 @@
                 (get_app_name(lang), os.path.realpath(lang), pofile(lang))
                 for lang in po_paths
             ]
             po_files.sort(key=lambda app: app[0])
             languages.append((language[0], _(language[1]), po_files))
             has_pos = has_pos or bool(po_paths)
 
-        context['version'] = get_rosetta_version()
-        context['languages'] = languages
-        context['has_pos'] = has_pos
-        context['po_filter'] = self.po_filter
+        context["version"] = get_rosetta_version()
+        context["languages"] = languages
+        context["has_pos"] = has_pos
+        context["po_filter"] = self.po_filter
         return context
 
 
 class TranslationFormView(RosettaFileLevelMixin, TemplateView):
     """Show a form with a page's worth of messages to be translated; handle its
     submission by updating cached pofile and, if possible, writing out changes
     to existing .po file.
@@ -246,26 +246,26 @@
     * query: a search string, where only matches are shown. Fields that are
       searched include: source, translated text, "occurence" file path, or
       context hints.
     """
 
     # Note: due to the unorthodox nature of the form itself, we're not using
     # Django's generic FormView as our base class.
-    http_method_names = ['get', 'post']
-    template_name = 'rosetta/form.html'
+    http_method_names = ["get", "post"]
+    template_name = "rosetta/form.html"
 
     def fix_nls(self, in_, out_):
         """Fixes submitted translations by filtering carriage returns and pairing
         newlines at the begging and end of the translated string with the original
         """
         if 0 == len(in_) or 0 == len(out_):
             return out_
 
         if "\r" in out_ and "\r" not in in_:
-            out_ = out_.replace("\r", '')
+            out_ = out_.replace("\r", "")
 
         if "\n" == in_[0] and "\n" != out_[0]:
             out_ = "\n" + out_
         elif "\n" != in_[0] and "\n" == out_[0]:
             out_ = out_.lstrip()
         if 0 == len(out_):
             pass
@@ -288,16 +288,16 @@
         file is updated (so it can be downloaded). Then the user is redirected
         to the next page of messages (if there is one; otherwise they're
         redirected back to the current page).
         """
         # The message text inputs are captured as hashes of their initial
         # contents, preceded by "m_". Messages with plurals end with their
         # variation number.
-        single_text_input_regex = re.compile(r'^m_([0-9a-f]+)$')
-        plural_text_input_regex = re.compile(r'^m_([0-9a-f]+)_([0-9]+)$')
+        single_text_input_regex = re.compile(r"^m_([0-9a-f]+)$")
+        plural_text_input_regex = re.compile(r"^m_([0-9a-f]+)_([0-9]+)$")
         file_change = False
         for field_name, new_msgstr in request.POST.items():
             md5hash = None
 
             if plural_text_input_regex.match(field_name):
                 md5hash, plural_id = plural_text_input_regex.match(field_name).groups()
                 md5hash = str(md5hash)
@@ -311,33 +311,33 @@
                     plural_id = int(plural_id)
 
             elif single_text_input_regex.match(field_name):
                 md5hash = str(single_text_input_regex.match(field_name).groups()[0])
                 plural_id = None
 
             if md5hash is not None:  # Empty string should be processed!
-                entry = self.po_file.find(md5hash, 'md5hash')
+                entry = self.po_file.find(md5hash, "md5hash")
                 # If someone did a makemessage, some entries might
                 # have been removed, so we need to check.
                 if entry:
                     old_msgstr = entry.msgstr
                     if plural_id is not None:  # 0 is ok!
                         entry.msgstr_plural[plural_id] = self.fix_nls(
                             entry.msgid_plural, new_msgstr
                         )
                     else:
                         entry.msgstr = self.fix_nls(entry.msgid, new_msgstr)
 
-                    is_fuzzy = bool(self.request.POST.get('f_%s' % md5hash, False))
-                    old_fuzzy = 'fuzzy' in entry.flags
+                    is_fuzzy = bool(self.request.POST.get("f_%s" % md5hash, False))
+                    old_fuzzy = "fuzzy" in entry.flags
 
                     if old_fuzzy and not is_fuzzy:
-                        entry.flags.remove('fuzzy')
+                        entry.flags.remove("fuzzy")
                     elif not old_fuzzy and is_fuzzy:
-                        entry.flags.append('fuzzy')
+                        entry.flags.append("fuzzy")
 
                     file_change = True
 
                     if old_msgstr != new_msgstr or old_fuzzy != is_fuzzy:
                         entry_changed.send(
                             sender=entry,
                             user=request.user,
@@ -354,47 +354,47 @@
                             "be saved: this usually happens when the catalog file "
                             "changes on disk after you last loaded it."
                         ),
                     )
 
         if file_change and self.po_file_is_writable:
             try:
-                self.po_file.metadata['Last-Translator'] = "{} {} <{}>".format(
-                    getattr(self.request.user, 'first_name', 'Anonymous'),
-                    getattr(self.request.user, 'last_name', 'User'),
-                    getattr(self.request.user, 'email', 'anonymous@user.tld'),
+                self.po_file.metadata["Last-Translator"] = "{} {} <{}>".format(
+                    getattr(self.request.user, "first_name", "Anonymous"),
+                    getattr(self.request.user, "last_name", "User"),
+                    getattr(self.request.user, "email", "anonymous@user.tld"),
                 )
-                self.po_file.metadata['X-Translated-Using'] = u"django-rosetta %s" % (
+                self.po_file.metadata["X-Translated-Using"] = "django-rosetta %s" % (
                     get_rosetta_version()
                 )
-                self.po_file.metadata['PO-Revision-Date'] = timestamp_with_timezone()
+                self.po_file.metadata["PO-Revision-Date"] = timestamp_with_timezone()
             except UnicodeDecodeError:
                 pass
 
             try:
                 self.po_file.save()
                 po_filepath, ext = os.path.splitext(self.po_file_path)
 
                 if rosetta_settings.AUTO_COMPILE:
-                    self.po_file.save_as_mofile(po_filepath + '.mo')
+                    self.po_file.save_as_mofile(po_filepath + ".mo")
 
                 post_save.send(
                     sender=None, language_code=self.language_id, request=self.request
                 )
                 # Try auto-reloading via the WSGI daemon mode reload mechanism
                 should_try_wsgi_reload = (
                     rosetta_settings.WSGI_AUTO_RELOAD
-                    and 'mod_wsgi.process_group' in self.request.environ
-                    and self.request.environ.get('mod_wsgi.process_group', None)
-                    and 'SCRIPT_FILENAME' in self.request.environ
-                    and int(self.request.environ.get('mod_wsgi.script_reloading', 0))
+                    and "mod_wsgi.process_group" in self.request.environ
+                    and self.request.environ.get("mod_wsgi.process_group", None)
+                    and "SCRIPT_FILENAME" in self.request.environ
+                    and int(self.request.environ.get("mod_wsgi.script_reloading", 0))
                 )
                 if should_try_wsgi_reload:
                     try:
-                        os.utime(self.request.environ.get('SCRIPT_FILENAME'), None)
+                        os.utime(self.request.environ.get("SCRIPT_FILENAME"), None)
                     except OSError:
                         pass
                 # Try auto-reloading via uwsgi daemon reload mechanism
                 if rosetta_settings.UWSGI_AUTO_RELOAD:
                     try:
                         import uwsgi
 
@@ -409,33 +409,33 @@
             storage = get_storage(self.request)
             storage.set(self.po_file_cache_key, self.po_file)
 
         # Reconstitute url to redirect to. Start with determining whether the
         # page number can be incremented.
         paginator = Paginator(self.get_entries(), rosetta_settings.MESSAGES_PER_PAGE)
         try:
-            page = int(self._request_request('page', 1))
+            page = int(self._request_request("page", 1))
         except ValueError:
             page = 1  # fall back to page 1
         else:
             if not (0 < page <= paginator.num_pages):
                 page = 1
         if page < paginator.num_pages:
             page += 1
         query_string_args = {
-            'msg_filter': self.msg_filter,
-            'query': self.query,
-            'ref_lang': self.ref_lang,
-            'page': page,
+            "msg_filter": self.msg_filter,
+            "query": self.query,
+            "ref_lang": self.ref_lang,
+            "page": page,
         }
         # Winnow down the query string args to non-blank ones
         query_string_args = {k: v for k, v in query_string_args.items() if v}
         return HttpResponseRedirect(
             "{url}?{qs}".format(
-                url=reverse('rosetta-form', kwargs=self.kwargs),
+                url=reverse("rosetta-form", kwargs=self.kwargs),
                 qs=urlencode_safe(query_string_args),
             )
         )
 
     def get_context_data(self, **kwargs):
         context = super(TranslationFormView, self).get_context_data(**kwargs)
         entries = self.get_entries()
@@ -454,19 +454,19 @@
                         o.ref_txt = o.msgid
             else:
                 for o in paginator.object_list:
                     o.ref_txt = o.msgid
             # XXX: having "MSGID" at the end of the dropdown is really odd, no?
             # Why not instead do this?
             # LANGUAGES = [('', '----')] + list(settings.LANGUAGES)
-            LANGUAGES.append(('msgid', 'MSGID'))
+            LANGUAGES.append(("msgid", "MSGID"))
 
         # Determine page number & how pagination links should be displayed
         try:
-            page = int(self._request_request('page', 1))
+            page = int(self._request_request("page", 1))
         except ValueError:
             page = 1  # fall back to page 1
         else:
             if not (0 < page <= paginator.num_pages):
                 page = 1
         needs_pagination = paginator.num_pages > 1
         if needs_pagination:
@@ -485,103 +485,100 @@
             # Translate from id to language name
             for language in rosetta_settings.ROSETTA_LANGUAGES:
                 if language[0] == main_language_id:
                     main_language = _(language[1])
                     break
         if main_language:
             main_lang_po_path = self.po_file_path.replace(
-                '/%s/' % self.language_id, '/%s/' % main_language_id
+                "/%s/" % self.language_id, "/%s/" % main_language_id
             )
             # XXX: brittle; what if this path doesn't exist? Isn't a .po file?
             main_lang_po = pofile(main_lang_po_path)
 
             for message in rosetta_messages:
                 message.main_lang = main_lang_po.find(message.msgid).msgstr
 
         # Collect some constants for the template
         rosetta_i18n_lang_name = str(
             dict(rosetta_settings.ROSETTA_LANGUAGES).get(self.language_id)
         )
         # "bidi" as in "bi-directional"
-        rosetta_i18n_lang_bidi = self.language_id.split('-')[0] in settings.LANGUAGES_BIDI
+        rosetta_i18n_lang_bidi = (
+            self.language_id.split("-")[0] in settings.LANGUAGES_BIDI
+        )
         query_string_args = {}
         if self.msg_filter:
-            query_string_args['msg_filter'] = self.msg_filter
+            query_string_args["msg_filter"] = self.msg_filter
         if self.query:
-            query_string_args['query'] = self.query
+            query_string_args["query"] = self.query
         if self.ref_lang:
-            query_string_args['ref_lang'] = self.ref_lang
+            query_string_args["ref_lang"] = self.ref_lang
         # Base for pagination links; the page num itself is added in template
         pagination_query_string_base = urlencode_safe(query_string_args)
         # Base for msg filter links; it doesn't make sense to persist page
         # numbers in these links. We just pass in ref_lang, if it's set.
         filter_query_string_base = urlencode_safe(
-            {k: v for k, v in query_string_args.items() if k == 'ref_lang'}
+            {k: v for k, v in query_string_args.items() if k == "ref_lang"}
         )
 
-        deepl_language_code = None
-        if rosetta_settings.DEEPL_LANGUAGES:
-            deepl_language_code = rosetta_settings.DEEPL_LANGUAGES.get(
-                self.language_id, None
-            )
-
         context.update(
             {
-                'version': get_rosetta_version(),
-                'LANGUAGES': LANGUAGES,
-                'rosetta_settings': rosetta_settings,
-                'rosetta_i18n_lang_name': rosetta_i18n_lang_name,
-                'rosetta_i18n_lang_code': self.language_id,
-                'rosetta_i18n_lang_code_normalized': self.language_id.replace('_', '-'),
-                'rosetta_i18n_lang_bidi': rosetta_i18n_lang_bidi,
-                'rosetta_i18n_filter': self.msg_filter,
-                'rosetta_i18n_write': self.po_file_is_writable,
-                'rosetta_messages': rosetta_messages,
-                'page_range': needs_pagination and page_range,
-                'needs_pagination': needs_pagination,
-                'main_language': main_language,
-                'rosetta_i18n_app': get_app_name(self.po_file_path),
-                'page': page,
-                'query': self.query,
-                'pagination_query_string_base': pagination_query_string_base,
-                'filter_query_string_base': filter_query_string_base,
-                'paginator': paginator,
-                'rosetta_i18n_pofile': self.po_file,
-                'ref_lang': self.ref_lang,
-                'deepl_language_code': deepl_language_code,
+                "version": get_rosetta_version(),
+                "LANGUAGES": LANGUAGES,
+                "rosetta_settings": rosetta_settings,
+                "rosetta_i18n_lang_name": rosetta_i18n_lang_name,
+                "rosetta_i18n_lang_code": self.language_id,
+                "rosetta_i18n_lang_code_normalized": self.language_id.replace("_", "-"),
+                "rosetta_i18n_lang_bidi": rosetta_i18n_lang_bidi,
+                "rosetta_i18n_filter": self.msg_filter,
+                "rosetta_i18n_write": self.po_file_is_writable,
+                "rosetta_messages": rosetta_messages,
+                "page_range": needs_pagination and page_range,
+                "needs_pagination": needs_pagination,
+                "main_language": main_language,
+                "rosetta_i18n_app": get_app_name(self.po_file_path),
+                "page": page,
+                "query": self.query,
+                "pagination_query_string_base": pagination_query_string_base,
+                "filter_query_string_base": filter_query_string_base,
+                "paginator": paginator,
+                "rosetta_i18n_pofile": self.po_file,
+                "ref_lang": self.ref_lang,
             }
         )
 
         return context
 
     @cached_property
     def ref_lang(self):
         """Return the language id for the "reference language" (the language to
         be translated *from*, if not English).
 
         Throw a 404 if it's not in rosetta_settings.ROSETTA_LANGUAGES.
         """
-        ref_lang = self._request_request('ref_lang', 'msgid')
-        if ref_lang != 'msgid':
+        ref_lang = self._request_request("ref_lang", "msgid")
+        if ref_lang != "msgid":
             allowed_languages = {lang[0] for lang in rosetta_settings.ROSETTA_LANGUAGES}
             if ref_lang not in allowed_languages:
                 raise Http404
         return ref_lang
 
     @cached_property
     def ref_lang_po_file(self):
         """Return a parsed .po file object for the "reference language", if one
         exists, otherwise None.
         """
         ref_pofile = None
-        if rosetta_settings.ENABLE_REFLANG and self.ref_lang != 'msgid':
-            replacement = '{separator}locale{separator}{ref_lang}'.format(
+        if rosetta_settings.ENABLE_REFLANG and self.ref_lang != "msgid":
+            replacement = "{separator}locale{separator}{ref_lang}".format(
                 separator=os.sep, ref_lang=self.ref_lang
             )
-            pattern = r'\{separator}locale\{separator}[a-z]{{2}}'.format(separator=os.sep)
+            pattern = r"\{separator}locale\{separator}[a-z]{{2}}".format(
+                separator=os.sep
+            )
             ref_fn = re.sub(pattern, replacement, self.po_file_path)
             try:
                 ref_pofile = pofile(ref_fn)
             except IOError:
                 # there's a syntax error in the PO file and polib can't
                 # open it. Let's just do nothing and thus display msgids.
                 # XXX: :-/
@@ -594,26 +591,26 @@
         or a default.
 
         If a query is also specified in the request, then return None.
         """
         if self.query:
             msg_filter = None
         else:
-            msg_filter = self._request_request('msg_filter', 'all')
-            available_msg_filters = {'untranslated', 'translated', 'fuzzy', 'all'}
+            msg_filter = self._request_request("msg_filter", "all")
+            available_msg_filters = {"untranslated", "translated", "fuzzy", "all"}
             if msg_filter not in available_msg_filters:
-                msg_filter = 'all'
+                msg_filter = "all"
         return msg_filter
 
     @cached_property
     def query(self):
         """Strip and return the query (for searching the catalog) from the
         request, or None.
         """
-        return self._request_request('query', '').strip() or None
+        return self._request_request("query", "").strip() or None
 
     def get_entries(self):
         """Return a list of the entries (messages) that would be part of the
         current "view"; that is, all of the ones from this .po file matching the
         current query or msg_filter.
         """
         if self.query:
@@ -622,87 +619,87 @@
 
             def concat_entry(e):
                 return (
                     str(e.msgstr)
                     + str(e.msgid)
                     + str(e.msgctxt)
                     + str(e.comment)
-                    + u''.join([o[0] for o in e.occurrences])
+                    + "".join([o[0] for o in e.occurrences])
                     + str(e.msgid_plural)
-                    + u''.join(e.msgstr_plural.values())
+                    + "".join(e.msgstr_plural.values())
                 )
 
             entries = [
                 e_
                 for e_ in self.po_file
                 if not e_.obsolete and rx.search(concat_entry(e_))
             ]
         else:
             # Scenario #2: filtered list of messages
-            if self.msg_filter == 'untranslated':
+            if self.msg_filter == "untranslated":
                 entries = self.po_file.untranslated_entries()
-            elif self.msg_filter == 'translated':
+            elif self.msg_filter == "translated":
                 entries = self.po_file.translated_entries()
-            elif self.msg_filter == 'fuzzy':
+            elif self.msg_filter == "fuzzy":
                 entries = [e_ for e_ in self.po_file.fuzzy_entries() if not e_.obsolete]
             else:
                 # ("all")
                 entries = [e_ for e_ in self.po_file if not e_.obsolete]
         return entries
 
 
 class TranslationFileDownload(RosettaFileLevelMixin, View):
     """Download a zip file for a specific catalog including both the raw (.po)
     and compiled (.mo) files, either as they exist on disk, or, if what's on
     disk is unwritable (permissions-wise), return what's in the cache.
     """
 
-    http_method_names = [u'get']
+    http_method_names = ["get"]
 
     def get(self, request, *args, **kwargs):
         try:
-            if len(self.po_file_path.split('/')) >= 5:
-                offered_fn = '_'.join(self.po_file_path.split('/')[-5:])
+            if len(self.po_file_path.split("/")) >= 5:
+                offered_fn = "_".join(self.po_file_path.split("/")[-5:])
             else:
-                offered_fn = self.po_file_path.split('/')[-1]
-            po_fn = str(self.po_file_path.split('/')[-1])
-            mo_fn = str(po_fn.replace('.po', '.mo'))  # not so smart, huh
+                offered_fn = self.po_file_path.split("/")[-1]
+            po_fn = str(self.po_file_path.split("/")[-1])
+            mo_fn = str(po_fn.replace(".po", ".mo"))  # not so smart, huh
             zipdata = BytesIO()
             with zipfile.ZipFile(zipdata, mode="w") as zipf:
                 zipf.writestr(po_fn, str(self.po_file).encode("utf8"))
                 zipf.writestr(mo_fn, self.po_file.to_binary())
             zipdata.seek(0)
 
             response = HttpResponse(zipdata.read())
-            filename = 'filename=%s.%s.zip' % (offered_fn, self.language_id)
-            response['Content-Disposition'] = 'attachment; %s' % filename
-            response['Content-Type'] = 'application/x-zip'
+            filename = "filename=%s.%s.zip" % (offered_fn, self.language_id)
+            response["Content-Disposition"] = "attachment; %s" % filename
+            response["Content-Type"] = "application/x-zip"
             return response
         except Exception:
             # XXX: should add a message!
             return HttpResponseRedirect(
-                reverse('rosetta-file-list', kwargs={'po_filter': 'project'})
+                reverse("rosetta-file-list", kwargs={"po_filter": "project"})
             )
 
 
 @user_passes_test(lambda user: can_translate(user), LoginURL())
 def translate_text(request):
 
-    language_from = request.GET.get('from', None)
-    language_to = request.GET.get('to', None)
-    text = request.GET.get('text', None)
+    language_from = request.GET.get("from", None)
+    language_to = request.GET.get("to", None)
+    text = request.GET.get("text", None)
 
     if language_from == language_to:
-        data = {'success': True, 'translation': text}
+        data = {"success": True, "translation": text}
     else:
         try:
             translated_text = translate(text, language_from, language_to)
 
-            data = {'success': True, 'translation': translated_text}
+            data = {"success": True, "translation": translated_text}
         except TranslationException as e:
-            data = {'success': False, 'error': str(e)}
+            data = {"success": False, "error": str(e)}
 
     return JsonResponse(data)
 
 
 def urlencode_safe(query):
     return urlencode({k: force_bytes(v) for k, v in query.items()})
```

### Comparing `django-rosetta-0.9.8/setup.py` & `django-rosetta-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/fixtures/vcr_cassettes/test_47_azure_ajax_translation.yaml` & `django-rosetta-0.9.9/testproject/fixtures/vcr_cassettes/test_47_azure_ajax_translation.yaml`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/locale/bs-Cyrl-BA/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/testproject/locale/bs-Cyrl-BA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/locale/fr/LC_MESSAGES/django.mo` & `django-rosetta-0.9.9/testproject/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/locale/fr/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/testproject/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/locale/fr_FR.utf8/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/testproject/locale/yy-Anot/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -8,34 +8,27 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-14 02:28-0500\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: \n"
 "Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
-"X-Translated-Using: django-rosetta 0.7.5\n"
 
 #: templates/test.html:3
 msgid "Some text to translate"
-msgstr "oiwue oqwiue§o§"
+msgstr ""
 
 #: templates/test.html:5
 #, python-format
 msgid ""
 "\n"
 "one bottle of beer on the wall\n"
 msgid_plural ""
 "\n"
 "%(num_bottles)s bottles of beer on the wall\n"
 msgstr[0] ""
-"\n"
-"%(num_bottles)s bottles of beer on the wall\n"
-msgstr[1] ""
-"\n"
-"%(num_bottles)s bottles of beer on the wall\n"
-msgstr[0] ""
 msgstr[1] ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-rosetta-0.9.8/testproject/locale/xx/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/testproject/locale/xx/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/locale/yy/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/testproject/locale/yy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/locale/yy-Anot/LC_MESSAGES/django.po` & `django-rosetta-0.9.9/testproject/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rosetta-0.9.8/testproject/rosetta.db` & `django-rosetta-0.9.9/testproject/rosetta.db`

 * *Files 2% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -65,18 +65,20 @@
 CREATE TABLE IF NOT EXISTS "auth_group" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(150) NOT NULL UNIQUE);
 CREATE TABLE IF NOT EXISTS "django_session" ("session_key" varchar(40) NOT NULL PRIMARY KEY, "session_data" text NOT NULL, "expire_date" datetime NOT NULL);
 INSERT INTO django_session VALUES('kdagkp40wwn5v0smlcnne29imvscc5xc','OTVjYTg1NGFkYzBmYzQ4NTFkOGJkZjg5MjU3ODc5YjBkYTdhMmI3MDp7Il9hdXRoX3VzZXJfaWQiOiIxIiwiX2F1dGhfdXNlcl9iYWNrZW5kIjoiZGphbmdvLmNvbnRyaWIuYXV0aC5iYWNrZW5kcy5Nb2RlbEJhY2tlbmQiLCJfYXV0aF91c2VyX2hhc2giOiJmNzNmZTkyODNkNzdiMTI1NzQyYTU3ZGRmNzljNmI5NzdjOGVhZDc0In0=','2020-06-21 08:22:37.060754');
 INSERT INTO django_session VALUES('b2ijzfa9l79wt54dc360p6tdab9j6h5c','.eJxVjMsOwiAUBf-FtSFcKMW6dO83ELgPqZqSlHZl_HfbpAvdnpk5bxXTupS4Np7jSOqiQJ1-t5zwydMO6JGme9VYp2Ues94VfdCmb5X4dT3cv4OSWtlqQeNZhMRh9o5sz2BhYDTCIXDG0AdAgnNnyYHxgF48skEZNqkzSX2-E_046w:1kyuD3:p59_-ELKGG57cqg4P2Ff2RBjGtzGrI02EUIXhXI2L5U','2021-01-25 04:14:01.193482');
 INSERT INTO django_session VALUES('8lq3nfsqix52vq748hpfpa9ez8xmxgd4','.eJxVjMsOwiAUBf-FtSFcKMW6dO83ELgPqZqSlHZl_HfbpAvdnpk5bxXTupS4Np7jSOqiQJ1-t5zwydMO6JGme9VYp2Ues94VfdCmb5X4dT3cv4OSWtlqQeNZhMRh9o5sz2BhYDTCIXDG0AdAgnNnyYHxgF48skEZNqkzSX2-E_046w:1lHnkL:Kvalg-afjVlYSOHubP9U9XXoVoOUsioZoIutOTHUG5Y','2021-03-18 07:10:29.316342');
 INSERT INTO django_session VALUES('4bb2g7xz0j51h41aldjdh3a7a0ogo5zd','.eJxVjMEOwiAQBf-FsyFAYaEevfcbCLCLVA0kpT0Z_9026UGvM_Pem_mwrcVvnRY_I7syyS6_LIb0pHoIfIR6bzy1ui5z5EfCT9v51JBet7P9Oyihl32tM7ikYIgQk7XG4KCdtCSFUwJxDAFU1srEjAKkGBClIJOdFkDjzjX7fAHMpzcN:1lh9os:Nf5KO7uipQVmRC8XZMZCQTdLXBC9MJUyJLDieXOl8PQ','2021-05-27 06:47:58.811663');
 INSERT INTO django_session VALUES('42gp35hdwlumc811qutbxgscm8uymrxd','.eJxVjMEOwiAQBf-FsyFAYaEevfcbCLCLVA0kpT0Z_9026UGvM_Pem_mwrcVvnRY_I7syyS6_LIb0pHoIfIR6bzy1ui5z5EfCT9v51JBet7P9Oyihl32tM7ikYIgQk7XG4KCdtCSFUwJxDAFU1srEjAKkGBClIJOdFkDjzjX7fAHMpzcN:1ltmer:qzd7GI4cRkIQHCYa95IcmE3y3_Xt6zbt3MsZIcBq81A','2021-07-01 02:41:49.682751');
+INSERT INTO django_session VALUES('xgho7zzjoa3d4cpacfmdq6o1yb7dscw4','.eJxVjE0OgyAYRO_CuiEgAtpl956BfD9YbBtIRFdN764mLuxmFvPezFcEWJcU1hrnMLG4Cy1u1w6B3jEfgF-Qn0VSycs8oTwUedIqh8Lx8zjdv4MENe1rh1Fxb0Z04LklBqPYYtR7WG01dEQWmdBTz94ZHBU23jB2ZBoFrRW_DRkIOQc:1pHnJZ:FF7Hl0XST-9hmtgoL0rN4Cmfq-ZCMvXh6H6fa57F3ZI','2023-01-31 08:51:53.979295');
+INSERT INTO django_session VALUES('cqy69s8zft2gkm6hpvp3j1bgxezbb3yu','.eJxVjEEOwiAQRe_C2hBoGSgu3XuGZpgZpGpoUtqV8e7apAvd_vfef6kRt7WMW5NlnFidlVWn3y0hPaTugO9Yb7Omua7LlPSu6IM2fZ1ZnpfD_Tso2Mq3NoaQkeMAhC6RhQA-mexFqAeMyboc_cDS2U6IwAILxYwumAA9sVPvDwfoOLs:1pokWL:rX0dEtAJUTQcWLoJZ0_MqDAP4HCzWS6nZfEH2ezbubQ','2023-05-02 07:33:17.615258');
 CREATE TABLE IF NOT EXISTS "django_site" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(50) NOT NULL, "domain" varchar(100) NOT NULL UNIQUE);
 INSERT INTO django_site VALUES(1,'example.com','example.com');
 CREATE TABLE IF NOT EXISTS "auth_user" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "password" varchar(128) NOT NULL, "last_login" datetime NULL, "is_superuser" bool NOT NULL, "username" varchar(150) NOT NULL UNIQUE, "last_name" varchar(150) NOT NULL, "email" varchar(254) NOT NULL, "is_staff" bool NOT NULL, "is_active" bool NOT NULL, "date_joined" datetime NOT NULL, "first_name" varchar(150) NOT NULL);
-INSERT INTO auth_user VALUES(1,'pbkdf2_sha256$260000$kJQrJWreRryyYlGERgMlON$Gv5UPPNTKDb2uAHWseThpBFgoq4nwRzqHvAtHjRBgBA=','2021-06-17 02:41:49.677510',1,'admin','','admin@admin.com',1,1,'2020-06-07 08:22:31.781154','');
+INSERT INTO auth_user VALUES(1,'pbkdf2_sha256$600000$HzcpoJsNfFGuGxT2awmUUp$T54iYUWI33MQRnR/hzTUL9CGNXYbEw7luLmwW8jrfhg=','2023-04-18 07:33:17.608625',1,'admin','','admin@admin.com',1,1,'2020-06-07 08:22:31.781154','');
 DELETE FROM sqlite_sequence;
 INSERT INTO sqlite_sequence VALUES('django_migrations',20);
 INSERT INTO sqlite_sequence VALUES('django_admin_log',0);
 INSERT INTO sqlite_sequence VALUES('django_content_type',7);
 INSERT INTO sqlite_sequence VALUES('auth_permission',28);
 INSERT INTO sqlite_sequence VALUES('auth_group',0);
 INSERT INTO sqlite_sequence VALUES('django_site',1);
```

### Comparing `django-rosetta-0.9.8/testproject/settings.py` & `django-rosetta-0.9.9/testproject/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import sys
 
 import django
 
+
 SITE_ID = 1
 
 PROJECT_PATH = os.path.abspath(os.path.dirname(__file__))
 
 PYTHON_VERSION = "%s.%s" % sys.version_info[:2]
 
 DATABASES = {
@@ -64,21 +65,21 @@
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
 )
 
 # Note: languages are overridden in the test runner
 LANGUAGES = (
-    ("en", u"English"),
-    ("bs-Cyrl-BA", u"Bosnian (Cyrillic) (Bosnia and Herzegovina)"),
-    ("ja", u"日本語"),
-    ("xx", u"XXXXX"),
-    ("fr", u"French"),
-    ("zh_Hans", u"Chinese (Simplified)"),
-    ("fr_FR.utf8", u"French (France), UTF8"),
+    ("en", "English"),
+    ("bs-Cyrl-BA", "Bosnian (Cyrillic) (Bosnia and Herzegovina)"),
+    ("ja", "日本語"),
+    ("xx", "XXXXX"),
+    ("fr", "French"),
+    ("zh_Hans", "Chinese (Simplified)"),
+    ("fr_FR.utf8", "French (France), UTF8"),
 )
 
 
 SILENCED_SYSTEM_CHECKS = ["translation.E002"]
 
 
 LOCALE_PATHS = [os.path.join(PROJECT_PATH, "locale")]
```

### Comparing `django-rosetta-0.9.8/tox.ini` & `django-rosetta-0.9.9/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 [tox]
 envlist =
         flake8,
-        py{36,37,38,39}-django{22,30,31,32},
-        py{38,39}-django40,
-        py310-django{32,40},
+        py{38,39,310}-django{32,40,41,42},
         gettext,
         docs
 
 
 [gh-actions]
 python =
-  3.10: py310-django32, py310-django40
-  3.9: py39-django22, py39-django30, py39-django31, py39-django32, py39-django40
-  3.8: py38-django22, py38-django30, py38-django31, py38-django32, py38-django40
-  3.7: py37-django22, py37-django30, py37-django31, py37-django32, flake8
-  3.6: py36-django22, py36-django30, py36-django31, py36-django32, gettext, docs
+  3.10: py310-django32, py310-django40, py310-django41, py310-django42
+  3.9: py39-django32, py39-django40, py39-django41, py39-django42
+  3.8: py38-django32, py38-django40, py38-django41, py38-django42
 
 
 skipsdist = True
 
 minversion = 3.8.0
 requires = virtualenv>=20.3.0
 
 [testenv]
 changedir = testproject
 commands =
-        python -Wd manage.py test rosetta
+        python -Wd manage.py test rosetta {posargs}
 
 setenv =
         PYTHONDONTWRITEBYTECODE=1
 
 deps =
-        django22: Django>=2.2.17,<=2.2.99
-        django30: Django>=3.0,<=3.0.99
-        django31: Django>=3.1,<=3.1.99
         django32: Django>=3.2,<=3.2.99
         django40: Django>=4.0,<4.1
+        django41: Django>=4.1a,<4.2
+        django42: Django>=4.2a,<4.3
 
-        django{22,30,31}: python-memcached
-        django{32,40}: pymemcache
+        pymemcache
         requests
         polib>=1.1.0
         goslate
         vcrpy
         coverage
 
 [testenv:gettext]
@@ -62,14 +56,16 @@
       msgfmt -c -o it/LC_MESSAGES/django.mo it/LC_MESSAGES/django.po
       msgfmt -c -o ky/LC_MESSAGES/django.mo ky/LC_MESSAGES/django.po
       msgfmt -c -o nl/LC_MESSAGES/django.mo nl/LC_MESSAGES/django.po
       msgfmt -c -o pl/LC_MESSAGES/django.mo pl/LC_MESSAGES/django.po
       msgfmt -c -o ru/LC_MESSAGES/django.mo ru/LC_MESSAGES/django.po
       msgfmt -c -o tr/LC_MESSAGES/django.mo tr/LC_MESSAGES/django.po
       msgfmt -c -o uk/LC_MESSAGES/django.mo uk/LC_MESSAGES/django.po
+      msgfmt -c -o zh_hans/LC_MESSAGES/django.mo zh_hans/LC_MESSAGES/django.po
+
 
 [testenv:docs]
 deps = sphinx
 changedir = docs
 commands=
         sphinx-build -W -b html . _build/html
```

