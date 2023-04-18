# Comparing `tmp/django_trackings-0.6.0a3.tar.gz` & `tmp/django_trackings-0.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_trackings-0.6.0a3.tar", last modified: Tue Apr 18 17:30:45 2023, max compression
+gzip compressed data, was "django_trackings-0.6.1a0.tar", last modified: Tue Apr 18 17:37:59 2023, max compression
```

## Comparing `django_trackings-0.6.0a3.tar` & `django_trackings-0.6.1a0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-18 17:30:45.000000 django_trackings-0.6.0a3/src/dj_tracker/cache_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/cache_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/cache_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/db_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/field_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-18 17:30:36.000000 django_trackings-0.6.0a3/src/dj_tracker/hash_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/hash_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/pythoncapi_compat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/dj_tracker/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/css/
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.658357 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/js/query_group.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.654357 django_trackings-0.6.0a3/src/dj_tracker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/listing.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/query.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/queries.html
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query.html
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/requests.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/templatetags/dj_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/dj_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-18 17:30:45.000000 django_trackings-0.6.0a3/src/dj_tracker/traceback.c
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/traceback.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-04-18 17:30:28.000000 django_trackings-0.6.0a3/src/dj_tracker/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:30:45.662357 django_trackings-0.6.0a3/src/django_trackings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-18 17:30:45.000000 django_trackings-0.6.0a3/src/django_trackings.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-18 17:37:59.351720 django_trackings-0.6.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-18 17:37:58.000000 django_trackings-0.6.1a0/src/dj_tracker/cache_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/cache_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/cache_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/db_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/field_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-18 17:37:50.000000 django_trackings-0.6.1a0/src/dj_tracker/hash_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/hash_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/pythoncapi_compat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/dj_tracker/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/js/query_group.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/dj_tracker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/queries.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/requests.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templatetags/dj_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-18 17:37:58.000000 django_trackings-0.6.1a0/src/dj_tracker/traceback.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/traceback.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/django_trackings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-18 17:37:59.000000 django_trackings-0.6.1a0/src/django_trackings.egg-info/SOURCES.txt
```

### Comparing `django_trackings-0.6.0a3/LICENSE` & `django_trackings-0.6.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/PKG-INFO` & `django_trackings-0.6.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_trackings
-Version: 0.6.0a3
+Version: 0.6.1a0
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
-Metadata-Version: 2.1 Name: django_trackings Version: 0.6.0a3 Summary: A Django
+Metadata-Version: 2.1 Name: django_trackings Version: 0.6.1a0 Summary: A Django
 app that tracks your queries to help optimize them. Home-page: https://
 github.com/tijani-dia/dj-tracker/ Author: Tidiane Dia Author-email:
 atdia97@gmail.com License: BSD-3-Clause Project-URL: Documentation, https://
 tijani-dia.github.io/dj-tracker/ Project-URL: Source, https://github.com/
 tijani-dia/dj-tracker/ Project-URL: Issue tracker, https://github.com/tijani-
 dia/dj-tracker/issues/ Classifier: Development Status :: 3 - Alpha Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
```

### Comparing `django_trackings-0.6.0a3/README.md` & `django_trackings-0.6.1a0/README.md`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/setup.cfg` & `django_trackings-0.6.1a0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_trackings
-version = 0.6.0a3
+version = 0.6.1a0
 description = A Django app that tracks your queries to help optimize them.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tijani-dia/dj-tracker/
 author = Tidiane Dia
 author_email = atdia97@gmail.com
 license = BSD-3-Clause
```

### Comparing `django_trackings-0.6.0a3/setup.py` & `django_trackings-0.6.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/cache_utils.c` & `django_trackings-0.6.1a0/src/dj_tracker/cache_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/cache_utils.pyx` & `django_trackings-0.6.1a0/src/dj_tracker/cache_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/collector.py` & `django_trackings-0.6.1a0/src/dj_tracker/collector.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/constants.py` & `django_trackings-0.6.1a0/src/dj_tracker/constants.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/datastructures.py` & `django_trackings-0.6.1a0/src/dj_tracker/datastructures.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,14 @@
             "query_string": request.META.get("QUERY_STRING", ""),
         }
         self.started_at = now()
         self.finished = False
         self.queries = HashableCounter()
         self.num_queries = self.num_queries_saved = 0
         Collector.add_request(self)
-        weakref_finalize(request, self.request_finished)
 
     def add_query(self, query_id):
         self.queries[query_id] += 1
         self.num_queries_saved += 1
         if self.ready:
             Collector.request_ready(self)
```

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/db_router.py` & `django_trackings-0.6.1a0/src/dj_tracker/db_router.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/field_descriptors.py` & `django_trackings-0.6.1a0/src/dj_tracker/field_descriptors.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/hash_utils.c` & `django_trackings-0.6.1a0/src/dj_tracker/hash_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/hash_utils.pyx` & `django_trackings-0.6.1a0/src/dj_tracker/hash_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/logging.py` & `django_trackings-0.6.1a0/src/dj_tracker/logging.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/migrations/0001_initial.py` & `django_trackings-0.6.1a0/src/dj_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/models.py` & `django_trackings-0.6.1a0/src/dj_tracker/models.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/profile.py` & `django_trackings-0.6.1a0/src/dj_tracker/profile.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/promise.py` & `django_trackings-0.6.1a0/src/dj_tracker/promise.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/pythoncapi_compat.h` & `django_trackings-0.6.1a0/src/dj_tracker/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/css/main.css` & `django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/css/main.css`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/static/dj_tracker/js/query_group.js` & `django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/js/query_group.js`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/base.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/base.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/home.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/home.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/listing.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/listing.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/pagination.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/includes/query.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/queries.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/queries.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_group.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_group.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/query_groups.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_groups.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templates/dj_tracker/requests.html` & `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/requests.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/templatetags/dj_tracker.py` & `django_trackings-0.6.1a0/src/dj_tracker/templatetags/dj_tracker.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/test/__init__.py` & `django_trackings-0.6.1a0/src/dj_tracker/test/__init__.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/traceback.c` & `django_trackings-0.6.1a0/src/dj_tracker/traceback.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/traceback.pyx` & `django_trackings-0.6.1a0/src/dj_tracker/traceback.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/tracker.py` & `django_trackings-0.6.1a0/src/dj_tracker/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,17 @@
 
     def patch_send(send):
         @wraps(send)
         def wrapper(sender, **named):
             try:
                 return send(sender, **named)
             finally:
+                if tracker := get_request().__dict__.get("_tracker"):
+                    tracker.request_finished()
+
                 set_request(DUMMY_REQUEST)
 
         return wrapper
 
     @cached_property
     def get_tracker(request):
         return RequestTracker(request)
```

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/urls.py` & `django_trackings-0.6.1a0/src/dj_tracker/urls.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/dj_tracker/views.py` & `django_trackings-0.6.1a0/src/dj_tracker/views.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a3/src/django_trackings.egg-info/SOURCES.txt` & `django_trackings-0.6.1a0/src/django_trackings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

