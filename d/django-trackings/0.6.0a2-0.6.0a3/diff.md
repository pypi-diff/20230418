# Comparing `tmp/django_trackings-0.6.0a2.tar.gz` & `tmp/django_trackings-0.6.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_trackings-0.6.0a2.tar", last modified: Sun Apr 16 23:10:20 2023, max compression
+gzip compressed data, was "django_trackings-0.6.0a3.tar", last modified: Tue Apr 18 17:30:45 2023, max compression
```

## Comparing `django_trackings-0.6.0a2.tar` & `django_trackings-0.6.0a3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-16 23:10:20.000000 django_trackings-0.6.0a2/src/dj_tracker/cache_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/cache_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/cache_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/db_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/field_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-16 23:10:09.000000 django_trackings-0.6.0a2/src/dj_tracker/hash_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/hash_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/pythoncapi_compat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/dj_tracker/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/css/
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/js/query_group.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/dj_tracker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/listing.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/query.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/queries.html
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query.html
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/requests.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templatetags/dj_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-16 23:10:20.000000 django_trackings-0.6.0a2/src/dj_tracker/traceback.c
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/traceback.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/django_trackings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-16 23:10:20.000000 django_trackings-0.6.0a2/src/django_trackings.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-18 17:30:45.000000 django_trackings-0.6.0a3/src/dj_tracker/cache_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/cache_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/cache_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/db_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/field_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-18 17:30:36.000000 django_trackings-0.6.0a3/src/dj_tracker/hash_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/hash_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/pythoncapi_compat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/dj_tracker/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/js/query_group.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/dj_tracker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/queries.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/requests.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templatetags/dj_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-18 17:30:45.000000 django_trackings-0.6.0a3/src/dj_tracker/traceback.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/traceback.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/django_trackings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-18 17:30:45.000000 django_trackings-0.6.0a3/src/django_trackings.egg-info/SOURCES.txt
```

### Comparing `django_trackings-0.6.0a2/LICENSE` & `django_trackings-0.6.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/PKG-INFO` & `django_trackings-0.6.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_trackings
-Version: 0.6.0a2
+Version: 0.6.0a3
 Summary: A Django app that tracks your queries to help optimize them.
 Home-page: https://github.com/tijani-dia/dj-tracker/
 Author: Tidiane Dia
 Author-email: atdia97@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://tijani-dia.github.io/dj-tracker/
 Project-URL: Source, https://github.com/tijani-dia/dj-tracker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django_trackings Version: 0.6.0a2 Summary: A Django
+Metadata-Version: 2.1 Name: django_trackings Version: 0.6.0a3 Summary: A Django
 app that tracks your queries to help optimize them. Home-page: https://
 github.com/tijani-dia/dj-tracker/ Author: Tidiane Dia Author-email:
 atdia97@gmail.com License: BSD-3-Clause Project-URL: Documentation, https://
 tijani-dia.github.io/dj-tracker/ Project-URL: Source, https://github.com/
 tijani-dia/dj-tracker/ Project-URL: Issue tracker, https://github.com/tijani-
 dia/dj-tracker/issues/ Classifier: Development Status :: 3 - Alpha Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
```

### Comparing `django_trackings-0.6.0a2/README.md` & `django_trackings-0.6.0a3/README.md`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/setup.cfg` & `django_trackings-0.6.0a3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_trackings
-version = 0.6.0a2
+version = 0.6.0a3
 description = A Django app that tracks your queries to help optimize them.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tijani-dia/dj-tracker/
 author = Tidiane Dia
 author_email = atdia97@gmail.com
 license = BSD-3-Clause
```

### Comparing `django_trackings-0.6.0a2/setup.py` & `django_trackings-0.6.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/cache_utils.c` & `django_trackings-0.6.0a3/src/dj_tracker/cache_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/cache_utils.pyx` & `django_trackings-0.6.0a3/src/dj_tracker/cache_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/collector.py` & `django_trackings-0.6.0a3/src/dj_tracker/collector.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/constants.py` & `django_trackings-0.6.0a3/src/dj_tracker/constants.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/datastructures.py` & `django_trackings-0.6.0a3/src/dj_tracker/datastructures.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/db_router.py` & `django_trackings-0.6.0a3/src/dj_tracker/db_router.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/field_descriptors.py` & `django_trackings-0.6.0a3/src/dj_tracker/field_descriptors.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/hash_utils.c` & `django_trackings-0.6.0a3/src/dj_tracker/hash_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/hash_utils.pyx` & `django_trackings-0.6.0a3/src/dj_tracker/hash_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/logging.py` & `django_trackings-0.6.0a3/src/dj_tracker/logging.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/migrations/0001_initial.py` & `django_trackings-0.6.0a3/src/dj_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/models.py` & `django_trackings-0.6.0a3/src/dj_tracker/models.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/profile.py` & `django_trackings-0.6.0a3/src/dj_tracker/profile.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/promise.py` & `django_trackings-0.6.0a3/src/dj_tracker/promise.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/pythoncapi_compat.h` & `django_trackings-0.6.0a3/src/dj_tracker/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/css/main.css` & `django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/css/main.css`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/js/query_group.js` & `django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/js/query_group.js`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/base.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/base.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/home.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/home.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/listing.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/listing.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+{% load dj_tracker %}
+
 <form method="GET" class="w-1/5 mt-8 mr-8">
     <div class="listing-form">
         <div>
             <label for="order_by">Order by</label>
             <select id="order_by" name="order_by">
                 {% for option in order_by_options %}
                     <option value="{{ option.name }}" {% if option == active_order_by %} selected{% endif %}>
@@ -16,13 +18,15 @@
                 {% for option in paginate_by_options %}
                     <option value="{{ option }}" {% if option == active_paginate_by %} selected{% endif %}>
                         {{ option }}
                     </option>
                 {% endfor %}
             </select>
         </div>
-        {{ filter.form.as_div }}
+    
+        {{ filter.form|form_as_div }}
     </div>
+
     <div class="w-full py-2 flex justify-center">
         <button type="submit">Apply</button>
     </div>
 </form>
```

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/pagination.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/query.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/queries.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/queries.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_group.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_group.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_groups.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_groups.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/requests.html` & `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/requests.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/test/__init__.py` & `django_trackings-0.6.0a3/src/dj_tracker/test/__init__.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/traceback.c` & `django_trackings-0.6.0a3/src/dj_tracker/traceback.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/traceback.pyx` & `django_trackings-0.6.0a3/src/dj_tracker/traceback.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/tracker.py` & `django_trackings-0.6.0a3/src/dj_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/urls.py` & `django_trackings-0.6.0a3/src/dj_tracker/urls.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a2/src/dj_tracker/views.py` & `django_trackings-0.6.0a3/src/dj_tracker/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import Counter, namedtuple
 from collections.abc import Mapping
 from operator import itemgetter
 
 from django.db.models import Count, Max, Prefetch
+from django.shortcuts import get_object_or_404
 from django.views.generic import TemplateView
 from django.views.generic.detail import DetailView
 from django_filters import BooleanFilter, FilterSet
 from django_filters.views import FilterView
 
 from dj_tracker.cache_utils import lazy_attribute
 from dj_tracker.models import InstanceFieldTracking, Query, QueryGroup, Request
@@ -126,16 +127,16 @@
 class RequestsView(ListView):
     template_name = "dj_tracker/requests.html"
 
     default_order_by = "-date"
     order_by_options = OrderByOptions(
         OrderByOption("Date (latest)", "-date", "-latest_occurrence"),
         OrderByOption("Date (earliest)", "date", "latest_occurrence"),
-        OrderByOption("Occurrence (ascending)", "-occurrence", "-num_trackings"),
-        OrderByOption("Occurrence (descending)", "occurrence", "num_trackings"),
+        OrderByOption("Occurrence (ascending)", "occurrence", "num_trackings"),
+        OrderByOption("Occurrence (descending)", "-occurrence", "-num_trackings"),
         OrderByOption("Path (A -> Z)", "path", "path__path"),
         OrderByOption("Path (Z -> A)", "-path", "-path__path"),
     )
 
     filterset_class = NPlusOneFilter
 
     @lazy_attribute
@@ -160,38 +161,37 @@
         OrderByOption("Number of queries (descending)", "-num_queries", "-num_queries"),
     )
 
     filterset_class = NPlusOneFilter
 
     def setup(self, request, *args, request_id=None, **kwargs):
         super().setup(request, *args, **kwargs)
-        self.request_id = request_id
-
-    def get_queryset(self):
-        qs = super().get_queryset()
-        if self.request_id:
-            qs = qs.filter(trackings__request_id=self.request_id)
-        return qs
+        self.request_obj = (
+            get_object_or_404(Request.objects.select_related("path"), pk=request_id)
+            if request_id
+            else None
+        )
 
     @lazy_attribute
     def base_queryset(cls):
         return (
             QueryGroup.objects.annotate_num_queries()
             .annotate_num_trackings()
             .annotate_latest_occurrence()
         )
 
+    def get_queryset(self):
+        qs = super().get_queryset()
+        if self.request_obj:
+            qs = qs.filter(trackings__request=self.request_obj)
+        return qs
+
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        if self.request_id:
-            context["title"] = Request.objects.select_related("path").get(
-                pk=self.request_id
-            )
-        else:
-            context["title"] = "Query groups"
+        context["title"] = self.request_obj or "Query groups"
         return context
 
 
 class QueryGroupView(DetailView):
     template_name = "dj_tracker/query_group.html"
 
     def get_queryset(self):
```

### Comparing `django_trackings-0.6.0a2/src/django_trackings.egg-info/SOURCES.txt` & `django_trackings-0.6.0a3/src/django_trackings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

