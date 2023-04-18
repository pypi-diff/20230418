# Comparing `tmp/air_drf_relation-0.5.5.tar.gz` & `tmp/air_drf_relation-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air_drf_relation-0.5.5.tar", last modified: Sat Feb 11 11:38:29 2023, max compression
+gzip compressed data, was "air_drf_relation-0.5.6.tar", last modified: Tue Apr 18 16:00:51 2023, max compression
```

## Comparing `air_drf_relation-0.5.5.tar` & `air_drf_relation-0.5.6.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.549384 air_drf_relation-0.5.5/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1074 2021-06-27 18:03:44.000000 air_drf_relation-0.5.5/LICENSE
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       87 2021-06-27 19:16:11.000000 air_drf_relation-0.5.5/MANIFEST.in
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-02-11 11:38:29.549542 air_drf_relation-0.5.5/PKG-INFO
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     6483 2022-05-26 10:52:59.000000 air_drf_relation-0.5.5/README.md
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.535695 air_drf_relation-0.5.5/air_drf_relation/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      346 2022-05-26 10:45:07.000000 air_drf_relation-0.5.5/air_drf_relation/__init__.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.539868 air_drf_relation-0.5.5/air_drf_relation/__pycache__/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      492 2022-05-26 10:48:51.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1452 2022-05-04 08:27:13.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/context_builder.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-04 08:28:39.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/decorators.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3466 2022-03-03 07:13:47.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2441 2022-05-26 11:22:49.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/fields.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1236 2022-05-04 08:27:13.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/filters.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1671 2023-02-08 22:30:26.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/model_fields.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5012 2023-02-11 11:33:06.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3021 2023-02-08 21:41:02.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)    11023 2023-02-11 11:33:06.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/serializers.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      332 2022-05-26 10:48:51.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1180 2022-05-26 11:22:35.000000 air_drf_relation-0.5.5/air_drf_relation/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      832 2022-05-04 08:26:21.000000 air_drf_relation-0.5.5/air_drf_relation/context_builder.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      696 2022-05-04 07:31:58.000000 air_drf_relation-0.5.5/air_drf_relation/decorators.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     4316 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/air_drf_relation/extra_kwargs.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1855 2022-05-26 11:22:46.000000 air_drf_relation-0.5.5/air_drf_relation/fields.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      690 2022-05-04 07:35:13.000000 air_drf_relation-0.5.5/air_drf_relation/filters.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1151 2023-02-08 22:30:19.000000 air_drf_relation-0.5.5/air_drf_relation/model_fields.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5763 2023-02-11 11:19:46.000000 air_drf_relation-0.5.5/air_drf_relation/preload_objects_manager.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3103 2023-02-08 21:41:00.000000 air_drf_relation-0.5.5/air_drf_relation/queryset_optimization.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)    10941 2023-02-11 11:32:45.000000 air_drf_relation-0.5.5/air_drf_relation/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      240 2022-05-26 10:47:07.000000 air_drf_relation-0.5.5/air_drf_relation/settings.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      651 2022-05-26 11:22:17.000000 air_drf_relation-0.5.5/air_drf_relation/utils.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.536665 air_drf_relation-0.5.5/air_drf_relation.egg-info/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-02-11 11:38:29.000000 air_drf_relation-0.5.5/air_drf_relation.egg-info/PKG-INFO
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2343 2023-02-11 11:38:29.000000 air_drf_relation-0.5.5/air_drf_relation.egg-info/SOURCES.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-02-11 11:38:29.000000 air_drf_relation-0.5.5/air_drf_relation.egg-info/dependency_links.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-02-08 22:24:16.000000 air_drf_relation-0.5.5/air_drf_relation.egg-info/not-zip-safe
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       41 2023-02-11 11:38:29.000000 air_drf_relation-0.5.5/air_drf_relation.egg-info/requires.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       50 2023-02-11 11:38:29.000000 air_drf_relation-0.5.5/air_drf_relation.egg-info/top_level.txt
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.541144 air_drf_relation-0.5.5/device/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      144 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.541647 air_drf_relation-0.5.5/device/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      698 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      371 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/migrations/0002_alter_device_code.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      251 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      888 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2505 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/device/views.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.544010 air_drf_relation-0.5.5/film/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.5/film/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2023-02-08 21:16:41.000000 air_drf_relation-0.5.5/film/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2023-02-08 21:16:41.000000 air_drf_relation-0.5.5/film/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.544644 air_drf_relation-0.5.5/film/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1093 2023-02-08 22:30:35.000000 air_drf_relation-0.5.5/film/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.5/film/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      586 2023-02-11 10:43:36.000000 air_drf_relation-0.5.5/film/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      877 2023-02-08 22:29:38.000000 air_drf_relation-0.5.5/film/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2081 2023-02-08 23:03:58.000000 air_drf_relation-0.5.5/film/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2023-02-08 23:17:50.000000 air_drf_relation-0.5.5/film/urls.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      217 2023-02-08 23:17:39.000000 air_drf_relation-0.5.5/film/views.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       73 2023-02-11 11:38:29.550446 air_drf_relation-0.5.5/setup.cfg
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      886 2023-02-11 11:36:15.000000 air_drf_relation-0.5.5/setup.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.546184 air_drf_relation-0.5.5/table/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.5/table/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.5/table/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      142 2022-05-13 12:51:44.000000 air_drf_relation-0.5.5/table/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.547322 air_drf_relation-0.5.5/table/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-13 12:54:15.000000 air_drf_relation-0.5.5/table/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      417 2022-05-13 12:58:02.000000 air_drf_relation-0.5.5/table/migrations/0002_table_name.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1820 2022-05-13 15:42:11.000000 air_drf_relation-0.5.5/table/migrations/0003_auto_20220513_1542.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      545 2022-05-13 15:43:10.000000 air_drf_relation-0.5.5/table/migrations/0004_material_company.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.5/table/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      916 2022-05-13 15:43:05.000000 air_drf_relation-0.5.5/table/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1342 2023-02-11 11:37:09.000000 air_drf_relation-0.5.5/table/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5277 2023-02-11 11:37:29.000000 air_drf_relation-0.5.5/table/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.5/table/views.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.548470 air_drf_relation-0.5.5/task/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-02-11 11:38:29.549280 air_drf_relation-0.5.5/task/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      558 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      387 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/migrations/0002_alter_task_image.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      598 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/migrations/0003_tag.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      512 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/migrations/0004_tag_task.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      391 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      462 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1346 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/urls.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      935 2022-03-03 07:12:43.000000 air_drf_relation-0.5.5/task/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.264019 air_drf_relation-0.5.6/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1074 2021-06-27 18:03:44.000000 air_drf_relation-0.5.6/LICENSE
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       87 2021-06-27 19:16:11.000000 air_drf_relation-0.5.6/MANIFEST.in
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-04-18 16:00:51.264165 air_drf_relation-0.5.6/PKG-INFO
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     6483 2022-05-26 10:52:59.000000 air_drf_relation-0.5.6/README.md
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.250992 air_drf_relation-0.5.6/air_drf_relation/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      346 2022-05-26 10:45:07.000000 air_drf_relation-0.5.6/air_drf_relation/__init__.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.255461 air_drf_relation-0.5.6/air_drf_relation/__pycache__/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      492 2022-05-26 10:48:51.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1452 2022-05-04 08:27:13.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/context_builder.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-04 08:28:39.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/decorators.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3466 2022-03-03 07:13:47.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2441 2022-05-26 11:22:49.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/fields.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1236 2022-05-04 08:27:13.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/filters.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1662 2023-04-18 14:12:35.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/model_fields.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5012 2023-02-11 11:33:06.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3021 2023-02-08 21:41:02.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)    11176 2023-04-18 15:58:49.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/serializers.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      332 2022-05-26 10:48:51.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1157 2023-04-18 15:58:32.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      832 2022-05-04 08:26:21.000000 air_drf_relation-0.5.6/air_drf_relation/context_builder.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      696 2022-05-04 07:31:58.000000 air_drf_relation-0.5.6/air_drf_relation/decorators.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     4316 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/air_drf_relation/extra_kwargs.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1855 2022-05-26 11:22:46.000000 air_drf_relation-0.5.6/air_drf_relation/fields.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      690 2022-05-04 07:35:13.000000 air_drf_relation-0.5.6/air_drf_relation/filters.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1137 2023-04-18 14:12:13.000000 air_drf_relation-0.5.6/air_drf_relation/model_fields.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5763 2023-02-11 11:19:46.000000 air_drf_relation-0.5.6/air_drf_relation/preload_objects_manager.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3103 2023-02-08 21:41:00.000000 air_drf_relation-0.5.6/air_drf_relation/queryset_optimization.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)    11007 2023-04-18 15:58:48.000000 air_drf_relation-0.5.6/air_drf_relation/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      240 2022-05-26 10:47:07.000000 air_drf_relation-0.5.6/air_drf_relation/settings.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      786 2023-04-18 15:58:31.000000 air_drf_relation-0.5.6/air_drf_relation/utils.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.252097 air_drf_relation-0.5.6/air_drf_relation.egg-info/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/PKG-INFO
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2343 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/SOURCES.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/dependency_links.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-02-08 22:24:16.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/not-zip-safe
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       41 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/requires.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       50 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/top_level.txt
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.256624 air_drf_relation-0.5.6/device/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      144 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.257058 air_drf_relation-0.5.6/device/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      698 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      371 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/migrations/0002_alter_device_code.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      251 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      888 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2505 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.258708 air_drf_relation-0.5.6/film/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.259171 air_drf_relation-0.5.6/film/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1093 2023-02-08 22:30:35.000000 air_drf_relation-0.5.6/film/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      586 2023-02-11 10:43:36.000000 air_drf_relation-0.5.6/film/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      877 2023-02-08 22:29:38.000000 air_drf_relation-0.5.6/film/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1845 2023-04-18 14:12:56.000000 air_drf_relation-0.5.6/film/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2023-02-08 23:17:50.000000 air_drf_relation-0.5.6/film/urls.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      217 2023-02-08 23:17:39.000000 air_drf_relation-0.5.6/film/views.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       73 2023-04-18 16:00:51.264977 air_drf_relation-0.5.6/setup.cfg
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      886 2023-04-18 16:00:49.000000 air_drf_relation-0.5.6/setup.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.260650 air_drf_relation-0.5.6/table/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      142 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.261823 air_drf_relation-0.5.6/table/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-13 12:54:15.000000 air_drf_relation-0.5.6/table/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      417 2022-05-13 12:58:02.000000 air_drf_relation-0.5.6/table/migrations/0002_table_name.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1820 2022-05-13 15:42:11.000000 air_drf_relation-0.5.6/table/migrations/0003_auto_20220513_1542.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      545 2022-05-13 15:43:10.000000 air_drf_relation-0.5.6/table/migrations/0004_material_company.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      916 2022-05-13 15:43:05.000000 air_drf_relation-0.5.6/table/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1342 2023-02-11 11:37:09.000000 air_drf_relation-0.5.6/table/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5277 2023-04-18 14:13:22.000000 air_drf_relation-0.5.6/table/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.263100 air_drf_relation-0.5.6/task/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.263920 air_drf_relation-0.5.6/task/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      558 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      387 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0002_alter_task_image.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      598 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0003_tag.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      512 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0004_tag_task.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      391 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      462 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1346 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/urls.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      935 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/views.py
```

### Comparing `air_drf_relation-0.5.5/LICENSE` & `air_drf_relation-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/PKG-INFO` & `air_drf_relation-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air_drf_relation
-Version: 0.5.5
+Version: 0.5.6
 Summary: Improved interaction with DRF relations.
 Home-page: https://github.com/bubaley/air-drf-relation
 Author: bubaley
 Author-email: bubaley.fu@gmail.com
 License: MIT
 Description: **AIR-DRF-RELATION**
```

### Comparing `air_drf_relation-0.5.5/README.md` & `air_drf_relation-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/context_builder.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/context_builder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/decorators.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/decorators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/fields.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/fields.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/filters.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/filters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/model_fields.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/model_fields.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb  8 22:30:19 2023 UTC, .py size: 1151 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7b22 e463 7f04 0000  a.......{".c....
+00000000: 610d 0d0a 0000 0000 3da5 3e64 7104 0000  a.......=.>dq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 5a07 4700  m.Z...d.d.l.Z.G.
 00000060: 6405 6406 8400 6406 6503 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6404 5300 2907 e900 0000 0029 01da 0966  d.S.)......)...f
@@ -42,64 +42,63 @@
 00000290: 0029 0572 0b00 0000 da04 6e61 6d65 da04  .).r......name..
 000002a0: 7061 7468 720c 0000 0072 0d00 0000 720e  pathr....r....r.
 000002b0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
 000002c0: 0000 0d00 0000 7306 0000 0000 0112 010a  ......s.........
 000002d0: 017a 1d41 6972 4461 7461 636c 6173 7346  .z.AirDataclassF
 000002e0: 6965 6c64 2e64 6563 6f6e 7374 7275 6374  ield.deconstruct
 000002f0: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
-00000300: 0004 0000 0043 0000 0073 3400 0000 7c01  .....C...s4...|.
+00000300: 0004 0000 0043 0000 0073 3000 0000 7c01  .....C...s0...|.
 00000310: 6400 7500 720c 7c01 5300 7400 a001 7c01  d.u.r.|.S.t...|.
-00000320: a101 7d04 7c04 7c00 a002 a100 6b02 7226  ..}.|.|.....k.r&
-00000330: 7c04 5300 7403 7c00 6a04 7c04 6401 8d02  |.S.t.|.j.|.d...
-00000340: 5300 a902 4e29 0272 0800 0000 da04 6461  S...N).r......da
-00000350: 7461 2905 da04 6a73 6f6e da05 6c6f 6164  ta)...json..load
-00000360: 73da 0c5f 6765 745f 6465 6661 756c 7472  s.._get_defaultr
-00000370: 0200 0000 7208 0000 0029 0572 0b00 0000  ....r....).r....
-00000380: da05 7661 6c75 65da 0a65 7870 7265 7373  ..value..express
-00000390: 696f 6eda 0a63 6f6e 6e65 6374 696f 6eda  ion..connection.
-000003a0: 036f 626a 7210 0000 0072 1000 0000 7211  .objr....r....r.
-000003b0: 0000 00da 0d66 726f 6d5f 6462 5f76 616c  .....from_db_val
-000003c0: 7565 1200 0000 730c 0000 0000 0108 0104  ue....s.........
-000003d0: 010a 010c 0104 017a 1f41 6972 4461 7461  .......z.AirData
-000003e0: 636c 6173 7346 6965 6c64 2e66 726f 6d5f  classField.from_
-000003f0: 6462 5f76 616c 7565 6302 0000 0000 0000  db_valuec.......
-00000400: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00000410: 0073 3400 0000 7400 7c01 7c00 6a01 8302  .s4...t.|.|.j...
-00000420: 7210 7c01 5300 7c01 6400 7500 721c 7c01  r.|.S.|.d.u.r.|.
-00000430: 5300 7402 a003 7c01 a101 7d02 7404 7c00  S.t...|...}.t.|.
-00000440: 6a01 7c02 6401 8d02 5300 7215 0000 0029  j.|.d...S.r....)
-00000450: 05da 0a69 7369 6e73 7461 6e63 6572 0800  ...isinstancer..
-00000460: 0000 7217 0000 0072 1800 0000 7202 0000  ..r....r....r...
-00000470: 0029 0372 0b00 0000 721a 0000 0072 1d00  .).r....r....r..
-00000480: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000490: 00da 0974 6f5f 7079 7468 6f6e 1a00 0000  ...to_python....
-000004a0: 730c 0000 0000 010c 0104 0108 0104 010a  s...............
-000004b0: 017a 1b41 6972 4461 7461 636c 6173 7346  .z.AirDataclassF
-000004c0: 6965 6c64 2e74 6f5f 7079 7468 6f6e 6302  ield.to_pythonc.
-000004d0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000004e0: 0000 0043 0000 0073 2400 0000 7400 7c01  ...C...s$...t.|.
-000004f0: 8301 7316 7401 a002 7c00 a003 a100 a101  ..s.t...|.......
-00000500: 5300 7401 a002 7404 7c01 8301 a101 5300  S.t...t.|.....S.
-00000510: 7207 0000 0029 0572 0500 0000 7217 0000  r....).r....r...
-00000520: 00da 0564 756d 7073 7219 0000 0072 0400  ...dumpsr....r..
-00000530: 0000 2902 720b 0000 0072 1a00 0000 7210  ..).r....r....r.
-00000540: 0000 0072 1000 0000 7211 0000 00da 0e67  ...r....r......g
-00000550: 6574 5f70 7265 705f 7661 6c75 6522 0000  et_prep_value"..
-00000560: 0073 0600 0000 0001 0801 0e01 7a20 4169  .s..........z Ai
-00000570: 7244 6174 6163 6c61 7373 4669 656c 642e  rDataclassField.
-00000580: 6765 745f 7072 6570 5f76 616c 7565 2909  get_prep_value).
-00000590: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000005a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000005b0: 6d65 5f5f 720a 0000 0072 1200 0000 721e  me__r....r....r.
-000005c0: 0000 0072 2000 0000 7222 0000 00da 0d5f  ...r ...r"....._
-000005d0: 5f63 6c61 7373 6365 6c6c 5f5f 7210 0000  _classcell__r...
-000005e0: 0072 1000 0000 720e 0000 0072 1100 0000  .r....r....r....
-000005f0: 7206 0000 0007 0000 0073 0a00 0000 0802  r........s......
-00000600: 0c04 0c05 0808 0808 7206 0000 0029 0a5a  ........r....).Z
-00000610: 0664 6163 6974 6572 0200 0000 da09 646a  .daciter......dj
-00000620: 616e 676f 2e64 6272 0300 0000 da0b 6461  ango.dbr......da
-00000630: 7461 636c 6173 7365 7372 0400 0000 7205  taclassesr....r.
-00000640: 0000 0072 1700 0000 da09 4a53 4f4e 4669  ...r......JSONFi
-00000650: 656c 6472 0600 0000 7210 0000 0072 1000  eldr....r....r..
-00000660: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
-00000670: 6f64 756c 653e 0100 0000 7308 0000 000c  odule>....s.....
-00000680: 010c 0110 0108 03                        .......
+00000320: a101 7d04 7c04 6400 7500 7222 6400 5300  ..}.|.d.u.r"d.S.
+00000330: 7402 7c00 6a03 7c04 6401 8d02 5300 a902  t.|.j.|.d...S...
+00000340: 4e29 0272 0800 0000 da04 6461 7461 2904  N).r......data).
+00000350: da04 6a73 6f6e da05 6c6f 6164 7372 0200  ..json..loadsr..
+00000360: 0000 7208 0000 0029 0572 0b00 0000 da05  ..r....).r......
+00000370: 7661 6c75 65da 0a65 7870 7265 7373 696f  value..expressio
+00000380: 6eda 0a63 6f6e 6e65 6374 696f 6eda 036f  n..connection..o
+00000390: 626a 7210 0000 0072 1000 0000 7211 0000  bjr....r....r...
+000003a0: 00da 0d66 726f 6d5f 6462 5f76 616c 7565  ...from_db_value
+000003b0: 1200 0000 730c 0000 0000 0108 0104 010a  ....s...........
+000003c0: 0108 0104 017a 1f41 6972 4461 7461 636c  .....z.AirDatacl
+000003d0: 6173 7346 6965 6c64 2e66 726f 6d5f 6462  assField.from_db
+000003e0: 5f76 616c 7565 6302 0000 0000 0000 0000  _valuec.........
+000003f0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00000400: 3400 0000 7400 7c01 7c00 6a01 8302 7210  4...t.|.|.j...r.
+00000410: 7c01 5300 7c01 6400 7500 721c 7c01 5300  |.S.|.d.u.r.|.S.
+00000420: 7402 a003 7c01 a101 7d02 7404 7c00 6a01  t...|...}.t.|.j.
+00000430: 7c02 6401 8d02 5300 7215 0000 0029 05da  |.d...S.r....)..
+00000440: 0a69 7369 6e73 7461 6e63 6572 0800 0000  .isinstancer....
+00000450: 7217 0000 0072 1800 0000 7202 0000 0029  r....r....r....)
+00000460: 0372 0b00 0000 7219 0000 0072 1c00 0000  .r....r....r....
+00000470: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00000480: 0974 6f5f 7079 7468 6f6e 1a00 0000 730c  .to_python....s.
+00000490: 0000 0000 010c 0104 0108 0104 010a 017a  ...............z
+000004a0: 1b41 6972 4461 7461 636c 6173 7346 6965  .AirDataclassFie
+000004b0: 6c64 2e74 6f5f 7079 7468 6f6e 6302 0000  ld.to_pythonc...
+000004c0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000004d0: 0043 0000 0073 2400 0000 7400 7c01 8301  .C...s$...t.|...
+000004e0: 7316 7401 a002 7c00 a003 a100 a101 5300  s.t...|.......S.
+000004f0: 7401 a002 7404 7c01 8301 a101 5300 7207  t...t.|.....S.r.
+00000500: 0000 0029 0572 0500 0000 7217 0000 00da  ...).r....r.....
+00000510: 0564 756d 7073 da0c 5f67 6574 5f64 6566  .dumps.._get_def
+00000520: 6175 6c74 7204 0000 0029 0272 0b00 0000  aultr....).r....
+00000530: 7219 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00000540: 1100 0000 da0e 6765 745f 7072 6570 5f76  ......get_prep_v
+00000550: 616c 7565 2200 0000 7306 0000 0000 0108  alue"...s.......
+00000560: 010e 017a 2041 6972 4461 7461 636c 6173  ...z AirDataclas
+00000570: 7346 6965 6c64 2e67 6574 5f70 7265 705f  sField.get_prep_
+00000580: 7661 6c75 6529 09da 085f 5f6e 616d 655f  value)...__name_
+00000590: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000005a0: 5f71 7561 6c6e 616d 655f 5f72 0a00 0000  _qualname__r....
+000005b0: 7212 0000 0072 1d00 0000 721f 0000 0072  r....r....r....r
+000005c0: 2200 0000 da0d 5f5f 636c 6173 7363 656c  ".....__classcel
+000005d0: 6c5f 5f72 1000 0000 7210 0000 0072 0e00  l__r....r....r..
+000005e0: 0000 7211 0000 0072 0600 0000 0700 0000  ..r....r........
+000005f0: 730a 0000 0008 020c 040c 0508 0808 0872  s..............r
+00000600: 0600 0000 290a 5a06 6461 6369 7465 7202  ....).Z.daciter.
+00000610: 0000 00da 0964 6a61 6e67 6f2e 6462 7203  .....django.dbr.
+00000620: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
+00000630: 7204 0000 0072 0500 0000 7217 0000 00da  r....r....r.....
+00000640: 094a 534f 4e46 6965 6c64 7206 0000 0072  .JSONFieldr....r
+00000650: 1000 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+00000660: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000670: 0073 0800 0000 0c01 0c01 1001 0803       .s............
```

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/serializers.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/serializers.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Feb 11 11:32:45 2023 UTC, .py size: 10941 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,689 +1,699 @@
-00000000: 610d 0d0a 0000 0000 dd7c e763 bd2a 0000  a........|.c.*..
+00000000: 610d 0d0a 0000 0000 38be 3e64 ff2a 0000  a.......8.>d.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
+00000020: 0005 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6407 6c0e 6d0f 5a0f 0100 6400 6408 6c10  d.l.m.Z...d.d.l.
 00000090: 6d11 5a11 0100 6400 6409 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
 000000a0: 0100 6400 640a 6c14 6d15 5a15 0100 6400  ..d.d.l.m.Z...d.
 000000b0: 640b 6c16 6d17 5a17 0100 6400 640c 6c18  d.l.m.Z...d.d.l.
 000000c0: 6d19 5a19 0100 6400 640d 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
-000000d0: 0100 6400 640e 6c1c 6d1d 5a1d 0100 6501  ..d.d.l.m.Z...e.
-000000e0: 640f 6513 6410 8d02 5a1e 4700 6411 6412  d.e.d...Z.G.d.d.
-000000f0: 8400 6412 650d 6a1f 8303 5a20 4700 6413  ..d.e.j...Z G.d.
-00000100: 6414 8400 6414 650d 6a21 6520 8304 5a22  d...d.e.j!e ..Z"
-00000110: 4700 6415 6416 8400 6416 650d 6a23 8303  G.d.d...d.e.j#..
-00000120: 5a24 4700 6417 6418 8400 6418 6520 8303  Z$G.d.d...d.e ..
-00000130: 5a25 4700 6419 641a 8400 641a 6525 8303  Z%G.d.d...d.e%..
-00000140: 5a26 4700 641b 641c 8400 641c 6511 8303  Z&G.d.d...d.e...
-00000150: 5a27 641d 5300 291e e900 0000 0029 03da  Z'd.S.)......)..
-00000160: 0754 7970 6556 6172 da04 4469 6374 da03  .TypeVar..Dict..
-00000170: 416e 7929 01da 0455 5549 4429 01da 0565  Any)...UUID)...e
-00000180: 6d70 7479 2901 da16 5072 696d 6172 794b  mpty)...PrimaryK
-00000190: 6579 5265 6c61 7465 6446 6965 6c64 2901  eyRelatedField).
-000001a0: da0a 6d6f 6465 6c5f 6d65 7461 2901 da0b  ..model_meta)...
-000001b0: 7365 7269 616c 697a 6572 7329 01da 0a46  serializers)...F
-000001c0: 6f72 6569 676e 4b65 7929 01da 1344 6174  oreignKey)...Dat
-000001d0: 6163 6c61 7373 5365 7269 616c 697a 6572  aclassSerializer
-000001e0: 2901 da09 4461 7461 636c 6173 7329 01da  )...Dataclass)..
-000001f0: 1b73 6574 5f65 6d70 7479 5f72 6571 7565  .set_empty_reque
-00000200: 7374 5f69 6e5f 6b77 6172 6773 2901 da12  st_in_kwargs)...
-00000210: 4578 7472 614b 7761 7267 7346 6163 746f  ExtraKwargsFacto
-00000220: 7279 2901 da0f 4169 7252 656c 6174 6564  ry)...AirRelated
-00000230: 4669 656c 6429 01da 1550 7265 6c6f 6164  Field)...Preload
-00000240: 4f62 6a65 6374 734d 616e 6167 6572 2901  ObjectsManager).
-00000250: da11 6f70 7469 6d69 7a65 5f71 7565 7279  ..optimize_query
-00000260: 7365 74da 0154 2901 da05 626f 756e 6463  set..T)...boundc
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0400 0000 0000 0000 734a 0000 0065 005a  ........sJ...e.Z
-00000290: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
-000002a0: 0364 0364 0484 005a 0464 0564 0684 005a  .d.d...Z.d.d...Z
-000002b0: 0564 0c87 0066 0164 0864 0984 095a 0665  .d...f.d.d...Z.e
-000002c0: 0787 0066 0164 0a64 0b84 0883 015a 0887  ...f.d.d.....Z..
-000002d0: 0004 005a 0953 0029 0dda 0d41 6972 5365  ...Z.S.)...AirSe
-000002e0: 7269 616c 697a 6572 6301 0000 0000 0000  rializerc.......
-000002f0: 0000 0000 0003 0000 0004 0000 000f 0000  ................
-00000300: 0073 2a00 0000 6400 7c00 5f00 7c02 a001  .s*...d.|._.|...
-00000310: 6401 6400 a102 7c00 5f02 7403 8300 6a04  d.d...|._.t...j.
-00000320: 7c01 6900 7c02 a401 8e01 0100 6400 5300  |.i.|.......d.S.
-00000330: a902 4eda 0f70 7265 6c6f 6164 5f6f 626a  ..N..preload_obj
-00000340: 6563 7473 2905 da18 5f70 7265 6c6f 6164  ects)..._preload
-00000350: 5f6f 626a 6563 7473 5f6d 616e 6167 6572  _objects_manager
-00000360: da03 706f 7072 1600 0000 da05 7375 7065  ..popr......supe
-00000370: 72da 085f 5f69 6e69 745f 5fa9 03da 0473  r..__init__....s
-00000380: 656c 66da 0461 7267 73da 066b 7761 7267  elf..args..kwarg
-00000390: 73a9 01da 095f 5f63 6c61 7373 5f5f a900  s....__class__..
-000003a0: fa55 2f55 7365 7273 2f6b 6972 696c 6c63  .U/Users/kirillc
-000003b0: 656c 6973 6576 2f70 726f 6a65 6374 732f  elisev/projects/
-000003c0: 7079 7468 6f6e 2f61 6972 2d64 7266 2d72  python/air-drf-r
-000003d0: 656c 6174 696f 6e2f 6169 725f 6472 665f  elation/air_drf_
-000003e0: 7265 6c61 7469 6f6e 2f73 6572 6961 6c69  relation/seriali
-000003f0: 7a65 7273 2e70 7972 1a00 0000 1500 0000  zers.pyr........
-00000400: 7306 0000 0000 0106 010e 017a 1641 6972  s..........z.Air
-00000410: 5365 7269 616c 697a 6572 2e5f 5f69 6e69  Serializer.__ini
-00000420: 745f 5f63 0300 0000 0000 0000 0000 0000  t__c............
-00000430: 0300 0000 0200 0000 4300 0000 730c 0000  ........C...s...
-00000440: 0074 0064 0183 0182 0164 0053 0029 024e  .t.d.....d.S.).N
-00000450: 7a1f 6075 7064 6174 6528 2960 206d 7573  z.`update()` mus
-00000460: 7420 6265 2069 6d70 6c65 6d65 6e74 6564  t be implemented
-00000470: 2ea9 01da 134e 6f74 496d 706c 656d 656e  .....NotImplemen
-00000480: 7465 6445 7272 6f72 a903 721c 0000 00da  tedError..r.....
-00000490: 0869 6e73 7461 6e63 65da 0e76 616c 6964  .instance..valid
-000004a0: 6174 6564 5f64 6174 6172 2100 0000 7221  ated_datar!...r!
-000004b0: 0000 0072 2200 0000 da06 7570 6461 7465  ...r".....update
-000004c0: 1a00 0000 7302 0000 0000 017a 1441 6972  ....s......z.Air
-000004d0: 5365 7269 616c 697a 6572 2e75 7064 6174  Serializer.updat
-000004e0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-000004f0: 0000 0200 0000 4300 0000 730c 0000 0074  ......C...s....t
-00000500: 0064 0183 0182 0164 0053 0029 024e 7a1f  .d.....d.S.).Nz.
-00000510: 6063 7265 6174 6528 2960 206d 7573 7420  `create()` must 
-00000520: 6265 2069 6d70 6c65 6d65 6e74 6564 2e72  be implemented.r
-00000530: 2300 0000 a902 721c 0000 0072 2700 0000  #.....r....r'...
-00000540: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-00000550: 0663 7265 6174 651d 0000 0073 0200 0000  .create....s....
-00000560: 0001 7a14 4169 7253 6572 6961 6c69 7a65  ..z.AirSerialize
-00000570: 722e 6372 6561 7465 4663 0200 0000 0000  r.createFc......
-00000580: 0000 0000 0000 0200 0000 0300 0000 0300  ................
-00000590: 0000 732e 0000 007c 006a 0064 0175 0172  ..s....|.j.d.u.r
-000005a0: 1a74 01a0 027c 00a1 01a0 03a1 007c 005f  .t...|.......|._
-000005b0: 0474 0574 067c 0083 02a0 077c 01a1 0101  .t.t.|.....|....
-000005c0: 0064 0053 0029 024e 4629 0872 1600 0000  .d.S.).NF).r....
-000005d0: 7210 0000 00da 1b67 6574 5f70 7265 6c6f  r......get_prelo
-000005e0: 6164 5f6f 626a 6563 7473 5f6d 616e 6167  ad_objects_manag
-000005f0: 6572 da04 696e 6974 7217 0000 0072 1900  er..initr....r..
-00000600: 0000 7214 0000 00da 0869 735f 7661 6c69  ..r......is_vali
-00000610: 64a9 0272 1c00 0000 da0f 7261 6973 655f  d..r......raise_
-00000620: 6578 6365 7074 696f 6e72 1f00 0000 7221  exceptionr....r!
-00000630: 0000 0072 2200 0000 722d 0000 0020 0000  ...r"...r-... ..
-00000640: 0073 0600 0000 0001 0a01 1001 7a16 4169  .s..........z.Ai
-00000650: 7253 6572 6961 6c69 7a65 722e 6973 5f76  rSerializer.is_v
-00000660: 616c 6964 6301 0000 0000 0000 0000 0000  alidc...........
-00000670: 0006 0000 0004 0000 000f 0000 0073 9e00  .............s..
-00000680: 0000 4700 6401 6402 8400 6402 8302 7d03  ..G.d.d...d...}.
-00000690: 7400 7c00 6402 6400 8303 7d04 7c04 7330  t.|.d.d...}.|.s0
-000006a0: 7c03 8300 7d04 7401 7c00 6402 7c04 8303  |...}.t.|.d.|...
-000006b0: 0100 7402 7c04 6403 8302 7346 7401 7c04  ..t.|.d...sFt.|.
-000006c0: 6403 7403 8303 0100 7404 7405 7c00 8302  d.t.....t.t.|...
-000006d0: 6a06 7c01 6900 7c02 a401 8e01 7d05 7402  j.|.i.|.....}.t.
-000006e0: 7c05 6404 8302 729a 7c05 6a07 6400 7500  |.d...r.|.j.d.u.
-000006f0: 729a 7c05 6a08 729a 7402 7c05 6a08 6405  r.|.j.r.t.|.j.d.
-00000700: 8302 729a 7c05 6a08 6a09 729a 7409 7c05  ..r.|.j.j.r.t.|.
-00000710: 6a0a 7c05 6a08 8302 7c05 5f0a 7c05 5300  j.|.j...|._.|.S.
-00000720: 2906 4e63 0000 0000 0000 0000 0000 0000  ).Nc............
-00000730: 0000 0000 0100 0000 4000 0000 730c 0000  ........@...s...
-00000740: 0065 005a 0164 005a 0264 0153 0029 027a  .e.Z.d.Z.d.S.).z
-00000750: 2541 6972 5365 7269 616c 697a 6572 2e6d  %AirSerializer.m
-00000760: 616e 795f 696e 6974 2e3c 6c6f 6361 6c73  any_init.<locals
-00000770: 3e2e 4d65 7461 4e29 03da 085f 5f6e 616d  >.MetaN)...__nam
-00000780: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000790: 0c5f 5f71 7561 6c6e 616d 655f 5f72 2100  .__qualname__r!.
-000007a0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-000007b0: 00da 044d 6574 6127 0000 0073 0200 0000  ...Meta'...s....
-000007c0: 0801 7233 0000 00da 156c 6973 745f 7365  ..r3.....list_se
-000007d0: 7269 616c 697a 6572 5f63 6c61 7373 da06  rializer_class..
-000007e0: 7061 7265 6e74 7211 0000 0029 0bda 0767  parentr....)...g
-000007f0: 6574 6174 7472 da07 7365 7461 7474 72da  etattr..setattr.
-00000800: 0768 6173 6174 7472 da11 4169 724c 6973  .hasattr..AirLis
-00000810: 7453 6572 6961 6c69 7a65 7272 1900 0000  tSerializerr....
-00000820: 7214 0000 00da 096d 616e 795f 696e 6974  r......many_init
-00000830: 7235 0000 00da 0563 6869 6c64 7211 0000  r5.....childr...
-00000840: 0072 2600 0000 2906 da03 636c 7372 1d00  .r&...)...clsr..
-00000850: 0000 721e 0000 0072 3300 0000 da04 6d65  ..r....r3.....me
-00000860: 7461 da0a 7365 7269 616c 697a 6572 721f  ta..serializerr.
-00000870: 0000 0072 2100 0000 7222 0000 0072 3a00  ...r!...r"...r:.
-00000880: 0000 2500 0000 7320 0000 0000 020e 020c  ..%...s ........
-00000890: 0104 0106 010c 010a 010c 0116 0314 0106  ................
-000008a0: 010a ff02 0106 ff02 0210 017a 1741 6972  ...........z.Air
-000008b0: 5365 7269 616c 697a 6572 2e6d 616e 795f  Serializer.many_
-000008c0: 696e 6974 2901 4629 0a72 3000 0000 7231  init).F).r0...r1
-000008d0: 0000 0072 3200 0000 721a 0000 0072 2800  ...r2...r....r(.
-000008e0: 0000 722a 0000 0072 2d00 0000 da0b 636c  ..r*...r-.....cl
-000008f0: 6173 736d 6574 686f 6472 3a00 0000 da0d  assmethodr:.....
-00000900: 5f5f 636c 6173 7363 656c 6c5f 5f72 2100  __classcell__r!.
-00000910: 0000 7221 0000 0072 1f00 0000 7222 0000  ..r!...r....r"..
-00000920: 0072 1400 0000 1400 0000 730c 0000 0008  .r........s.....
-00000930: 010c 0508 0308 030e 0502 0172 1400 0000  ...........r....
-00000940: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000950: 0004 0000 0000 0000 0073 ac00 0000 6500  .........s....e.
-00000960: 5a01 6400 5a02 4700 6401 6402 8400 6402  Z.d.Z.G.d.d...d.
-00000970: 8302 5a03 8700 6601 6403 6404 8408 5a04  ..Z...f.d.d...Z.
-00000980: 8700 6601 6405 6406 8408 5a05 6407 6408  ..f.d.d...Z.d.d.
-00000990: 8400 5a06 6409 640a 8400 5a07 6422 8700  ..Z.d.d...Z.d"..
-000009a0: 6601 640c 640d 8409 5a08 640e 640f 8400  f.d.d...Z.d.d...
-000009b0: 5a09 6410 6411 8400 5a0a 6412 6413 8400  Z.d.d...Z.d.d...
-000009c0: 5a0b 6414 6415 8400 5a0c 6416 6417 8400  Z.d.d...Z.d.d...
-000009d0: 5a0d 6418 6419 8400 5a0e 641a 641b 8400  Z.d.d...Z.d.d...
-000009e0: 5a0f 641c 641d 8400 5a10 8700 6601 641e  Z.d.d...Z...f.d.
-000009f0: 641f 8408 5a11 8700 6601 6420 6421 8408  d...Z...f.d d!..
-00000a00: 5a12 8700 0400 5a13 5300 2923 da12 4169  Z.....Z.S.)#..Ai
-00000a10: 724d 6f64 656c 5365 7269 616c 697a 6572  rModelSerializer
-00000a20: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000a30: 0001 0000 0040 0000 0073 2400 0000 6500  .....@...s$...e.
-00000a40: 5a01 6400 5a02 6401 5a03 6402 5a04 6402  Z.d.Z.d.Z.d.Z.d.
-00000a50: 5a05 6402 5a06 6900 5a07 6403 5a08 6401  Z.d.Z.i.Z.d.Z.d.
-00000a60: 5300 2904 7a17 4169 724d 6f64 656c 5365  S.).z.AirModelSe
-00000a70: 7269 616c 697a 6572 2e4d 6574 614e 7221  rializer.MetaNr!
-00000a80: 0000 0054 2909 7230 0000 0072 3100 0000  ...T).r0...r1...
-00000a90: 7232 0000 00da 056d 6f64 656c da06 6669  r2.....model..fi
-00000aa0: 656c 6473 da10 7265 6164 5f6f 6e6c 795f  elds..read_only_
-00000ab0: 6669 656c 6473 5a11 7772 6974 655f 6f6e  fieldsZ.write_on
-00000ac0: 6c79 5f66 6965 6c64 73da 0c65 7874 7261  ly_fields..extra
-00000ad0: 5f6b 7761 7267 7372 1100 0000 7221 0000  _kwargsr....r!..
-00000ae0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00000af0: 7233 0000 003a 0000 0073 0c00 0000 0801  r3...:...s......
-00000b00: 0401 0401 0401 0401 0401 7233 0000 0063  ..........r3...c
-00000b10: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000b20: 0400 0000 0f00 0000 73cc 0000 007c 02a0  ........s....|..
-00000b30: 0064 0164 00a1 027c 005f 017c 02a0 0064  .d.d...|._.|...d
-00000b40: 0264 00a1 027c 005f 0264 037c 005f 0364  .d...|._.d.|._.d
-00000b50: 047c 0276 0072 3a7c 02a0 0064 0464 03a1  .|.v.r:|...d.d..
-00000b60: 027c 005f 036e 1c74 047c 006a 0564 0483  .|._.n.t.|.j.d..
-00000b70: 0272 5674 067c 006a 0564 0464 0383 037c  .rVt.|.j.d.d...|
-00000b80: 005f 037c 02a0 0064 0569 00a1 027c 005f  ._.|...d.i...|._
-00000b90: 0764 067c 0276 0172 7674 087c 0264 078d  .d.|.v.rvt.|.d..
-00000ba0: 0101 007c 006a 0173 887c 006a 097c 0264  ...|.j.s.|.j.|.d
-00000bb0: 078d 0101 007c 006a 0273 987c 00a0 0a7c  .....|.j.s.|...|
-00000bc0: 02a1 0101 007c 00a0 0ba1 007c 005f 0c7c  .....|.....|._.|
-00000bd0: 00a0 0da1 0001 0074 0e74 0f7c 0083 026a  .......t.t.|...j
-00000be0: 107c 0169 007c 02a4 018e 0101 007c 00a0  .|.i.|.......|..
-00000bf0: 11a1 0001 0064 0053 0029 084e da06 6163  .....d.S.).N..ac
-00000c00: 7469 6f6e da04 7573 6572 5472 1100 0000  tion..userTr....
-00000c10: 7245 0000 00da 0763 6f6e 7465 7874 a901  rE.....context..
-00000c20: 721e 0000 0029 1272 1800 0000 7246 0000  r....).r....rF..
-00000c30: 0072 4700 0000 7211 0000 0072 3800 0000  .rG...r....r8...
-00000c40: 7233 0000 0072 3600 0000 da15 5f69 6e69  r3...r6....._ini
-00000c50: 7469 616c 5f65 7874 7261 5f6b 7761 7267  tial_extra_kwarg
-00000c60: 7372 0d00 0000 da15 5f73 6574 5f61 6374  sr......_set_act
-00000c70: 696f 6e5f 6672 6f6d 5f76 6965 77da 165f  ion_from_view.._
-00000c80: 7365 745f 7573 6572 5f66 726f 6d5f 7265  set_user_from_re
-00000c90: 7175 6573 74da 115f 6765 745f 6578 7472  quest.._get_extr
-00000ca0: 615f 6b77 6172 6773 7245 0000 00da 1e5f  a_kwargsrE....._
-00000cb0: 7570 6461 7465 5f65 7874 7261 5f6b 7761  update_extra_kwa
-00000cc0: 7267 735f 696e 5f66 6965 6c64 7372 1900  rgs_in_fieldsr..
-00000cd0: 0000 7241 0000 0072 1a00 0000 da0e 5f75  ..rA...r......_u
-00000ce0: 7064 6174 655f 6669 656c 6473 721b 0000  pdate_fieldsr...
-00000cf0: 0072 1f00 0000 7221 0000 0072 2200 0000  .r....r!...r"...
-00000d00: 721a 0000 0042 0000 0073 2400 0000 0001  r....B...s$.....
-00000d10: 0e01 0e01 0601 0801 1001 0c01 1001 0e01  ................
-00000d20: 0801 0a02 0601 0c01 0601 0a01 0a01 0801  ................
-00000d30: 1601 7a1b 4169 724d 6f64 656c 5365 7269  ..z.AirModelSeri
-00000d40: 616c 697a 6572 2e5f 5f69 6e69 745f 5f63  alizer.__init__c
-00000d50: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-00000d60: 0400 0000 0300 0000 7324 0000 0074 0074  ........s$...t.t
-00000d70: 017c 0083 027d 037c 0173 187c 03a0 027c  .|...}.|.s.|...|
-00000d80: 02a1 0153 007c 03a0 037c 017c 02a1 0253  ...S.|...|.|...S
-00000d90: 00a9 014e 2904 7219 0000 0072 4100 0000  ...N).r....rA...
-00000da0: 722a 0000 0072 2800 0000 2904 721c 0000  r*...r(...).r...
-00000db0: 0072 2600 0000 7227 0000 005a 0b73 7570  .r&...r'...Z.sup
-00000dc0: 6572 5f63 6c61 7373 721f 0000 0072 2100  er_classr....r!.
-00000dd0: 0000 7222 0000 00da 1075 7064 6174 655f  ..r".....update_
-00000de0: 6f72 5f63 7265 6174 6557 0000 0073 0400  or_createW...s..
-00000df0: 0000 0001 0a01 7a23 4169 724d 6f64 656c  ......z#AirModel
-00000e00: 5365 7269 616c 697a 6572 2e75 7064 6174  Serializer.updat
-00000e10: 655f 6f72 5f63 7265 6174 6563 0200 0000  e_or_createc....
-00000e20: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000e30: 4300 0000 730c 0000 007c 00a0 0064 007c  C...s....|...d.|
-00000e40: 01a1 0253 0072 5000 0000 a901 7251 0000  ...S.rP.....rQ..
-00000e50: 0072 2900 0000 7221 0000 0072 2100 0000  .r)...r!...r!...
-00000e60: 7222 0000 0072 2a00 0000 5b00 0000 7302  r"...r*...[...s.
-00000e70: 0000 0000 017a 1941 6972 4d6f 6465 6c53  .....z.AirModelS
-00000e80: 6572 6961 6c69 7a65 722e 6372 6561 7465  erializer.create
-00000e90: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000ea0: 0004 0000 0043 0000 0073 0c00 0000 7c00  .....C...s....|.
-00000eb0: a000 7c01 7c02 a102 5300 7250 0000 0072  ..|.|...S.rP...r
-00000ec0: 5200 0000 7225 0000 0072 2100 0000 7221  R...r%...r!...r!
-00000ed0: 0000 0072 2200 0000 7228 0000 005e 0000  ...r"...r(...^..
-00000ee0: 0073 0200 0000 0001 7a19 4169 724d 6f64  .s......z.AirMod
-00000ef0: 656c 5365 7269 616c 697a 6572 2e75 7064  elSerializer.upd
-00000f00: 6174 6546 6302 0000 0000 0000 0000 0000  ateFc...........
-00000f10: 0002 0000 0003 0000 0003 0000 0073 1e00  .............s..
-00000f20: 0000 7c00 a000 a100 0100 7401 7402 7c00  ..|.......t.t.|.
-00000f30: 8302 6a03 7c01 6401 8d01 0100 6400 5300  ..j.|.d.....d.S.
-00000f40: 2902 4ea9 0172 2f00 0000 2904 da1a 5f66  ).N..r/...)..._f
-00000f50: 696c 7465 725f 7175 6572 7973 6574 5f62  ilter_queryset_b
-00000f60: 795f 6669 656c 6473 7219 0000 0072 4100  y_fieldsr....rA.
-00000f70: 0000 722d 0000 0072 2e00 0000 721f 0000  ..r-...r....r...
-00000f80: 0072 2100 0000 7222 0000 0072 2d00 0000  .r!...r"...r-...
-00000f90: 6100 0000 7304 0000 0000 0108 017a 1b41  a...s........z.A
-00000fa0: 6972 4d6f 6465 6c53 6572 6961 6c69 7a65  irModelSerialize
-00000fb0: 722e 6973 5f76 616c 6964 6301 0000 0000  r.is_validc.....
-00000fc0: 0000 0000 0000 0008 0000 0004 0000 0043  ...............C
-00000fd0: 0000 0073 bc00 0000 7400 7c00 6a01 6401  ...s....t.|.j.d.
-00000fe0: 8302 7310 6400 5300 7402 a003 7c00 6a01  ..s.d.S.t...|.j.
-00000ff0: 6a04 a101 7d01 6402 6403 8400 7c00 6a05  j...}.d.d...|.j.
-00001000: a006 a100 4400 8301 7d02 7c02 4400 5d0c  ....D...}.|.D.].
-00001010: 7d03 7c00 6a05 7c03 3d00 7136 7c00 6a05  }.|.j.|.=.q6|.j.
-00001020: a006 a100 4400 5d68 5c02 7d04 7d05 7407  ....D.]h\.}.}.t.
-00001030: 7c05 7408 8302 7362 714e 7c00 7c05 5f09  |.t...sbqN|.|._.
-00001040: 7c01 6a0a 7c04 1900 6a0b 7d06 7c05 6a0c  |.j.|...j.}.|.j.
-00001050: 7d07 7c06 6a0d 7388 6404 7c05 5f0e 714e  }.|.j.s.d.|._.qN
-00001060: 7c06 6a0f 724e 7c07 a010 6405 a101 6400  |.j.rN|...d...d.
-00001070: 7500 72a2 6406 7c05 5f11 7c07 a010 6407  u.r.d.|._.|...d.
-00001080: a101 6400 7500 724e 6404 7c05 5f12 714e  ..d.u.rNd.|._.qN
-00001090: 6400 5300 2908 4e72 4200 0000 6301 0000  d.S.).NrB...c...
-000010a0: 0000 0000 0000 0000 0003 0000 0006 0000  ................
-000010b0: 0053 0000 0073 2a00 0000 6700 7c00 5d22  .S...s*...g.|.]"
-000010c0: 5c02 7d01 7d02 7400 7c02 6400 8302 7204  \.}.}.t.|.d...r.
-000010d0: 7401 7c02 6400 6401 8303 7204 7c01 9102  t.|.d.d...r.|...
-000010e0: 7104 5300 2902 da06 6869 6464 656e 5429  q.S.)...hiddenT)
-000010f0: 0272 3800 0000 7236 0000 0029 03da 022e  .r8...r6...)....
-00001100: 30da 0a66 6965 6c64 5f6e 616d 65da 0566  0..field_name..f
-00001110: 6965 6c64 7221 0000 0072 2100 0000 7222  ieldr!...r!...r"
-00001120: 0000 00da 0a3c 6c69 7374 636f 6d70 3e69  .....<listcomp>i
-00001130: 0000 0073 0400 0000 0c01 16ff 7a35 4169  ...s........z5Ai
-00001140: 724d 6f64 656c 5365 7269 616c 697a 6572  rModelSerializer
-00001150: 2e5f 7570 6461 7465 5f66 6965 6c64 732e  ._update_fields.
-00001160: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00001170: 6d70 3e54 da08 7265 7175 6972 6564 46da  mp>T..requiredF.
-00001180: 0a61 6c6c 6f77 5f6e 756c 6c29 1372 3800  .allow_null).r8.
-00001190: 0000 7233 0000 0072 0800 0000 da0e 6765  ..r3...r......ge
-000011a0: 745f 6669 656c 645f 696e 666f 7242 0000  t_field_inforB..
-000011b0: 0072 4300 0000 da05 6974 656d 73da 0a69  .rC.....items..i
-000011c0: 7369 6e73 7461 6e63 6572 0f00 0000 7235  sinstancer....r5
-000011d0: 0000 00da 0972 656c 6174 696f 6e73 da0b  .....relations..
-000011e0: 6d6f 6465 6c5f 6669 656c 64da 075f 6b77  model_field.._kw
-000011f0: 6172 6773 da08 6564 6974 6162 6c65 da09  args..editable..
-00001200: 7265 6164 5f6f 6e6c 79da 046e 756c 6cda  read_only..null.
-00001210: 0367 6574 725a 0000 0072 5b00 0000 2908  .getrZ...r[...).
-00001220: 721c 0000 00da 0469 6e66 6fda 0d68 6964  r......info..hid
-00001230: 6465 6e5f 6669 656c 6473 da02 656c 7257  den_fields..elrW
-00001240: 0000 0072 5800 0000 7260 0000 00da 0c66  ...rX...r`.....f
-00001250: 6965 6c64 5f6b 7761 7267 7372 2100 0000  ield_kwargsr!...
-00001260: 7221 0000 0072 2200 0000 724f 0000 0065  r!...r"...rO...e
-00001270: 0000 0073 2800 0000 0001 0c01 0401 0e01  ...s(...........
-00001280: 1402 0801 0a01 1201 0a01 0201 0601 0c01  ................
-00001290: 0601 0601 0601 0201 0601 0e01 0601 0e01  ................
-000012a0: 7a21 4169 724d 6f64 656c 5365 7269 616c  z!AirModelSerial
-000012b0: 697a 6572 2e5f 7570 6461 7465 5f66 6965  izer._update_fie
-000012c0: 6c64 7363 0100 0000 0000 0000 0000 0000  ldsc............
-000012d0: 0500 0000 0500 0000 4300 0000 7390 0000  ........C...s...
-000012e0: 007c 00a0 00a1 007d 017c 01a0 01a1 0044  .|.....}.|.....D
-000012f0: 005d 7a5c 027d 027d 037c 006a 02a0 037c  .]z\.}.}.|.j...|
-00001300: 02a1 0173 2671 1064 007d 0474 047c 0374  ...s&q.d.}.t.|.t
-00001310: 0583 0272 467c 036a 0672 4001 0064 0053  ...rF|.j.r@..d.S
-00001320: 007c 036a 077d 047c 0473 5664 017c 036a  .|.j.}.|.sVd.|.j
-00001330: 089b 009d 027d 0474 097c 006a 0a7c 0483  .....}.t.|.j.|..
-00001340: 0272 1074 0b74 0c7c 006a 0a7c 0483 0283  .r.t.t.|.j.|....
-00001350: 0172 1074 0c7c 006a 0a7c 0483 027c 007c  .r.t.|.j.|...|.|
-00001360: 036a 0d64 028d 027c 035f 0d71 1064 0053  .j.d...|._.q.d.S
-00001370: 0029 034e 5a09 7175 6572 7973 6574 5f29  .).NZ.queryset_)
-00001380: 0272 1c00 0000 da08 7175 6572 7973 6574  .r......queryset
-00001390: 290e da13 5f67 6574 5f72 656c 6174 6564  )..._get_related
-000013a0: 5f66 6965 6c64 7372 5d00 0000 da0c 696e  _fieldsr].....in
-000013b0: 6974 6961 6c5f 6461 7461 7265 0000 0072  itial_datare...r
-000013c0: 5e00 0000 720f 0000 00da 1a71 7565 7279  ^...r......query
-000013d0: 7365 745f 6675 6e63 7469 6f6e 5f64 6973  set_function_dis
-000013e0: 6162 6c65 645a 1671 7565 7279 7365 745f  abledZ.queryset_
-000013f0: 6675 6e63 7469 6f6e 5f6e 616d 6572 5700  function_namerW.
-00001400: 0000 7238 0000 0072 2000 0000 da08 6361  ..r8...r .....ca
-00001410: 6c6c 6162 6c65 7236 0000 0072 6a00 0000  llabler6...rj...
-00001420: 2905 721c 0000 00da 0e72 656c 6174 6564  ).r......related
-00001430: 5f66 6965 6c64 7372 5700 0000 7258 0000  _fieldsrW...rX..
-00001440: 00da 0d66 756e 6374 696f 6e5f 6e61 6d65  ...function_name
-00001450: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00001460: 5400 0000 7c00 0000 731a 0000 0000 0108  T...|...s.......
-00001470: 0110 010c 0102 0104 010a 0106 0106 0106  ................
-00001480: 0104 010c 011c 017a 2d41 6972 4d6f 6465  .......z-AirMode
-00001490: 6c53 6572 6961 6c69 7a65 722e 5f66 696c  lSerializer._fil
-000014a0: 7465 725f 7175 6572 7973 6574 5f62 795f  ter_queryset_by_
-000014b0: 6669 656c 6473 6301 0000 0000 0000 0000  fieldsc.........
-000014c0: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
-000014d0: 3600 0000 7400 8300 7d01 7c00 6a01 a002  6...t...}.|.j...
-000014e0: a100 4400 5d20 5c02 7d02 7d03 7403 7c03  ..D.] \.}.}.t.|.
-000014f0: 8301 7404 7405 6602 7600 7210 7c03 7c01  ..t.t.f.v.r.|.|.
-00001500: 7c02 3c00 7110 7c01 5300 7250 0000 0029  |.<.q.|.S.rP...)
-00001510: 06da 0464 6963 7472 4300 0000 725d 0000  ...dictrC...r]..
-00001520: 00da 0474 7970 6572 0f00 0000 7207 0000  ...typer....r...
-00001530: 0029 0472 1c00 0000 726f 0000 0072 5700  .).r....ro...rW.
-00001540: 0000 7258 0000 0072 2100 0000 7221 0000  ..rX...r!...r!..
-00001550: 0072 2200 0000 726b 0000 008b 0000 0073  .r"...rk.......s
-00001560: 0a00 0000 0001 0601 1201 1001 0a01 7a26  ..............z&
-00001570: 4169 724d 6f64 656c 5365 7269 616c 697a  AirModelSerializ
-00001580: 6572 2e5f 6765 745f 7265 6c61 7465 645f  er._get_related_
-00001590: 6669 656c 6473 6301 0000 0000 0000 0000  fieldsc.........
-000015a0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-000015b0: 2e00 0000 6401 7c00 6a00 6901 7d01 7401  ....d.|.j.i.}.t.
-000015c0: 7c00 6a02 7c01 7c00 6a03 6402 8d03 a004  |.j.|.|.j.d.....
-000015d0: a100 6a05 7d02 7c00 a006 a100 0100 7c02  ..j.}.|.......|.
-000015e0: 5300 2903 4e72 4500 0000 2903 723d 0000  S.).NrE...).r=..
-000015f0: 00da 0464 6174 6172 4600 0000 2907 724a  ...datarF...).rJ
-00001600: 0000 0072 0e00 0000 7233 0000 0072 4600  ...r....r3...rF.
-00001610: 0000 722c 0000 0072 4500 0000 da23 5f64  ..r,...rE....#_d
-00001620: 656c 6574 655f 6375 7374 6f6d 5f65 7874  elete_custom_ext
-00001630: 7261 5f6b 7761 7267 735f 696e 5f6d 6574  ra_kwargs_in_met
-00001640: 6129 0372 1c00 0000 7273 0000 0072 4500  a).r....rs...rE.
-00001650: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00001660: 0072 4d00 0000 9200 0000 7308 0000 0000  .rM.......s.....
-00001670: 010a 0118 0108 017a 2441 6972 4d6f 6465  .......z$AirMode
-00001680: 6c53 6572 6961 6c69 7a65 722e 5f67 6574  lSerializer._get
-00001690: 5f65 7874 7261 5f6b 7761 7267 7363 0100  _extra_kwargsc..
-000016a0: 0000 0000 0000 0000 0000 0300 0000 0900  ................
-000016b0: 0000 4300 0000 7368 0000 007c 006a 00a0  ..C...sh...|.j..
-000016c0: 01a1 0044 005d 585c 027d 017d 027a 387c  ...D.]X\.}.}.z8|
-000016d0: 006a 026a 027c 0119 006a 03a0 047c 02a1  .j.j.|...j...|..
-000016e0: 0101 0069 007c 006a 026a 027c 0119 006a  ...i.|.j.j.|...j
-000016f0: 05a5 017c 02a5 017c 006a 026a 027c 0119  ...|...|.j.j.|..
-00001700: 005f 0557 0071 0a04 0074 0679 6001 0001  ._.W.q...t.y`...
-00001710: 0001 0059 0071 0a59 0071 0a30 0071 0a64  ...Y.q.Y.q.0.q.d
-00001720: 0053 0072 5000 0000 2907 7245 0000 0072  .S.rP...).rE...r
-00001730: 5d00 0000 7243 0000 00da 085f 5f64 6963  ]...rC.....__dic
-00001740: 745f 5f72 2800 0000 7261 0000 00da 084b  t__r(...ra.....K
-00001750: 6579 4572 726f 7229 0372 1c00 0000 da03  eyError).r......
-00001760: 6b65 79da 0576 616c 7565 7221 0000 0072  key..valuer!...r
-00001770: 2100 0000 7222 0000 0072 4e00 0000 9800  !...r"...rN.....
-00001780: 0000 730c 0000 0000 0112 0102 0114 0124  ..s............$
-00001790: 010c 017a 3141 6972 4d6f 6465 6c53 6572  ...z1AirModelSer
-000017a0: 6961 6c69 7a65 722e 5f75 7064 6174 655f  ializer._update_
-000017b0: 6578 7472 615f 6b77 6172 6773 5f69 6e5f  extra_kwargs_in_
-000017c0: 6669 656c 6473 6301 0000 0000 0000 0000  fieldsc.........
-000017d0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-000017e0: 4200 0000 7400 7c00 6a01 6401 8302 7310  B...t.|.j.d...s.
-000017f0: 6400 5300 7c00 6a01 6a02 a003 a100 4400  d.S.|.j.j.....D.
-00001800: 5d20 5c02 7d01 7d02 7c02 a004 6402 6400  ] \.}.}.|...d.d.
-00001810: a102 0100 7c02 a004 6403 6400 a102 0100  ....|...d.d.....
-00001820: 711c 6400 5300 2904 4e72 4500 0000 da07  q.d.S.).NrE.....
-00001830: 706b 5f6f 6e6c 7972 5500 0000 2905 7238  pk_onlyrU...).r8
-00001840: 0000 0072 3300 0000 7245 0000 0072 5d00  ...r3...rE...r].
-00001850: 0000 7218 0000 0029 0372 1c00 0000 7257  ..r....).r....rW
-00001860: 0000 0072 5800 0000 7221 0000 0072 2100  ...rX...r!...r!.
-00001870: 0000 7222 0000 0072 7400 0000 a000 0000  ..r"...rt.......
-00001880: 730a 0000 0000 010c 0104 0114 010c 017a  s..............z
-00001890: 3641 6972 4d6f 6465 6c53 6572 6961 6c69  6AirModelSeriali
-000018a0: 7a65 722e 5f64 656c 6574 655f 6375 7374  zer._delete_cust
-000018b0: 6f6d 5f65 7874 7261 5f6b 7761 7267 735f  om_extra_kwargs_
-000018c0: 696e 5f6d 6574 6163 0200 0000 0000 0000  in_metac........
-000018d0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-000018e0: 732e 0000 007c 01a0 0064 0164 00a1 027d  s....|...d.d...}
-000018f0: 027c 0273 1464 0053 007c 02a0 0064 02a1  .|.s.d.S.|...d..
-00001900: 017d 037c 0372 2a7c 036a 017c 005f 0164  .}.|.r*|.j.|._.d
-00001910: 0053 0029 034e 7248 0000 00da 0476 6965  .S.).NrH.....vie
-00001920: 7729 0272 6500 0000 7246 0000 0029 0472  w).re...rF...).r
-00001930: 1c00 0000 721e 0000 0072 4800 0000 727a  ....r....rH...rz
-00001940: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00001950: 0000 724b 0000 00a7 0000 0073 0c00 0000  ..rK.......s....
-00001960: 0001 0c01 0401 0401 0a01 0401 7a28 4169  ............z(Ai
-00001970: 724d 6f64 656c 5365 7269 616c 697a 6572  rModelSerializer
-00001980: 2e5f 7365 745f 6163 7469 6f6e 5f66 726f  ._set_action_fro
-00001990: 6d5f 7669 6577 6302 0000 0000 0000 0000  m_viewc.........
-000019a0: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
-000019b0: 4600 0000 7c01 a000 6401 6400 a102 7d02  F...|...d.d...}.
-000019c0: 7c02 7314 6400 5300 7c02 a000 6402 a101  |.s.d.S.|...d...
-000019d0: 7d03 7c03 7242 7401 7c03 6403 8302 7242  }.|.rBt.|.d...rB
-000019e0: 7402 7c03 6403 8302 7d04 7c04 6a03 7242  t.|.d...}.|.j.rB
-000019f0: 7c04 7c00 5f04 6400 5300 2904 4e72 4800  |.|._.d.S.).NrH.
-00001a00: 0000 da07 7265 7175 6573 7472 4700 0000  ....requestrG...
-00001a10: 2905 7265 0000 0072 3800 0000 7236 0000  ).re...r8...r6..
-00001a20: 00da 1069 735f 6175 7468 656e 7469 6361  ...is_authentica
-00001a30: 7465 6472 4700 0000 2905 721c 0000 0072  tedrG...).r....r
-00001a40: 1e00 0000 7248 0000 0072 7b00 0000 7247  ....rH...r{...rG
-00001a50: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00001a60: 0000 724c 0000 00af 0000 0073 1000 0000  ..rL.......s....
-00001a70: 0001 0c01 0401 0401 0a01 0e01 0a01 0601  ................
-00001a80: 7a29 4169 724d 6f64 656c 5365 7269 616c  z)AirModelSerial
-00001a90: 697a 6572 2e5f 7365 745f 7573 6572 5f66  izer._set_user_f
-00001aa0: 726f 6d5f 7265 7175 6573 7463 0100 0000  rom_requestc....
-00001ab0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00001ac0: 0f00 0000 7348 0000 007c 02a0 0064 0164  ....sH...|...d.d
-00001ad0: 02a1 0272 2e64 037c 0276 0172 1e74 017c  ...r.d.|.v.r.t.|
-00001ae0: 0264 048d 0101 007c 006a 027c 0169 007c  .d.....|.j.|.i.|
-00001af0: 02a4 018e 0153 0074 0383 006a 047c 0067  .....S.t...j.|.g
-00001b00: 017c 01a2 0152 0069 007c 02a4 018e 0153  .|...R.i.|.....S
-00001b10: 0029 054e da04 6d61 6e79 4672 4800 0000  .).N..manyFrH...
-00001b20: 7249 0000 0029 0572 1800 0000 720d 0000  rI...).r....r...
-00001b30: 0072 3a00 0000 7219 0000 00da 075f 5f6e  .r:...r......__n
-00001b40: 6577 5f5f 2903 723c 0000 0072 1d00 0000  ew__).r<...r....
-00001b50: 721e 0000 0072 1f00 0000 7221 0000 0072  r....r....r!...r
-00001b60: 2200 0000 727e 0000 00b9 0000 0073 0a00  "...r~.......s..
-00001b70: 0000 0001 0c01 0801 0a01 1001 7a1a 4169  ............z.Ai
-00001b80: 724d 6f64 656c 5365 7269 616c 697a 6572  rModelSerializer
-00001b90: 2e5f 5f6e 6577 5f5f 6302 0000 0000 0000  .__new__c.......
-00001ba0: 0000 0000 0004 0000 0004 0000 0003 0000  ................
-00001bb0: 0073 5c00 0000 7400 7c00 6401 8302 6400  .s\...t.|.d...d.
-00001bc0: 7500 721e 7c00 6a01 721e 7401 7c01 7c00  u.r.|.j.r.t.|.|.
-00001bd0: 8302 7d01 7402 7403 7c00 8302 a004 7c01  ..}.t.t.|.....|.
-00001be0: a101 7d02 7c02 4400 5d24 7d03 7405 7c02  ..}.|.D.]$}.t.|.
-00001bf0: 7c03 1900 8301 7406 6b02 7232 7407 7c02  |.....t.k.r2t.|.
-00001c00: 7c03 1900 8301 7c02 7c03 3c00 7132 7c02  |.....|.|.<.q2|.
-00001c10: 5300 2902 4e72 3500 0000 2908 7236 0000  S.).Nr5...).r6..
-00001c20: 0072 1100 0000 7219 0000 0072 4100 0000  .r....r....rA...
-00001c30: da11 746f 5f72 6570 7265 7365 6e74 6174  ..to_representat
-00001c40: 696f 6e72 7200 0000 7205 0000 00da 0373  ionrr...r......s
-00001c50: 7472 2904 721c 0000 0072 2600 0000 7273  tr).r....r&...rs
-00001c60: 0000 0072 6800 0000 721f 0000 0072 2100  ...rh...r....r!.
-00001c70: 0000 7222 0000 0072 7f00 0000 c000 0000  ..r"...r........
-00001c80: 730e 0000 0000 0114 010a 0110 0108 0110  s...............
-00001c90: 0112 017a 2441 6972 4d6f 6465 6c53 6572  ...z$AirModelSer
-00001ca0: 6961 6c69 7a65 722e 746f 5f72 6570 7265  ializer.to_repre
-00001cb0: 7365 6e74 6174 696f 6e29 0146 2914 7230  sentation).F).r0
-00001cc0: 0000 0072 3100 0000 7232 0000 0072 3300  ...r1...r2...r3.
-00001cd0: 0000 721a 0000 0072 5100 0000 722a 0000  ..r....rQ...r*..
-00001ce0: 0072 2800 0000 722d 0000 0072 4f00 0000  .r(...r-...rO...
-00001cf0: 7254 0000 0072 6b00 0000 724d 0000 0072  rT...rk...rM...r
-00001d00: 4e00 0000 7274 0000 0072 4b00 0000 724c  N...rt...rK...rL
-00001d10: 0000 0072 7e00 0000 727f 0000 0072 4000  ...r~...r....r@.
-00001d20: 0000 7221 0000 0072 2100 0000 721f 0000  ..r!...r!...r...
-00001d30: 0072 2200 0000 7241 0000 0039 0000 0073  .r"...rA...9...s
-00001d40: 2000 0000 0801 0e08 0c15 0c04 0803 0803   ...............
-00001d50: 0e04 0817 080f 0807 0806 0808 0807 0808  ................
-00001d60: 080a 0c07 7241 0000 0063 0000 0000 0000  ....rA...c......
-00001d70: 0000 0000 0000 0000 0000 0400 0000 0000  ................
-00001d80: 0000 7336 0000 0065 005a 0164 005a 0287  ..s6...e.Z.d.Z..
-00001d90: 0066 0164 0164 0284 085a 0364 0887 0066  .f.d.d...Z.d...f
-00001da0: 0164 0464 0584 095a 0487 0066 0164 0664  .d.d...Z...f.d.d
-00001db0: 0784 085a 0587 0004 005a 0653 0029 0972  ...Z.....Z.S.).r
-00001dc0: 3900 0000 6301 0000 0000 0000 0000 0000  9...c...........
-00001dd0: 0003 0000 0004 0000 000f 0000 0073 2e00  .............s..
-00001de0: 0000 7c02 a000 6401 6400 a102 7c00 5f01  ..|...d.d...|._.
-00001df0: 7402 7403 7c00 8302 6a04 7c01 6900 7c02  t.t.|...j.|.i.|.
-00001e00: a401 8e01 0100 6400 7c00 5f05 6400 5300  ......d.|._.d.S.
-00001e10: 7215 0000 0029 0672 1800 0000 7216 0000  r....).r....r...
-00001e20: 0072 1900 0000 7239 0000 0072 1a00 0000  .r....r9...r....
-00001e30: 7217 0000 0029 0372 1c00 0000 721d 0000  r....).r....r...
-00001e40: 00da 0b6c 6973 745f 6b77 6172 6773 721f  ...list_kwargsr.
-00001e50: 0000 0072 2100 0000 7222 0000 0072 1a00  ...r!...r"...r..
-00001e60: 0000 cb00 0000 7306 0000 0000 010e 0116  ......s.........
-00001e70: 017a 1a41 6972 4c69 7374 5365 7269 616c  .z.AirListSerial
-00001e80: 697a 6572 2e5f 5f69 6e69 745f 5f46 6302  izer.__init__Fc.
-00001e90: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001ea0: 0000 0003 0000 0073 4200 0000 7c00 6a00  .......sB...|.j.
-00001eb0: 6401 7501 722c 7401 7c00 6a02 6402 6400  d.u.r,t.|.j.d.d.
-00001ec0: 8303 6401 7501 722c 7403 a004 7c00 a101  ..d.u.r,t...|...
-00001ed0: a005 a100 7c00 5f06 7407 7408 7c00 8302  ....|._.t.t.|...
-00001ee0: 6a09 7c01 6403 8d01 0100 6400 5300 2904  j.|.d.....d.S.).
-00001ef0: 4e46 7216 0000 0072 5300 0000 290a 7216  NFr....rS...).r.
-00001f00: 0000 0072 3600 0000 723b 0000 0072 1000  ...r6...r;...r..
-00001f10: 0000 722b 0000 0072 2c00 0000 7217 0000  ..r+...r,...r...
-00001f20: 0072 1900 0000 7239 0000 0072 2d00 0000  .r....r9...r-...
-00001f30: 722e 0000 0072 1f00 0000 7221 0000 0072  r....r....r!...r
-00001f40: 2200 0000 722d 0000 00d0 0000 0073 0600  "...r-.......s..
-00001f50: 0000 0001 1c01 1001 7a1a 4169 724c 6973  ........z.AirLis
-00001f60: 7453 6572 6961 6c69 7a65 722e 6973 5f76  tSerializer.is_v
-00001f70: 616c 6964 6303 0000 0000 0000 0000 0000  alidc...........
-00001f80: 0003 0000 0004 0000 0003 0000 0073 1600  .............s..
-00001f90: 0000 7400 7401 7c00 8302 a002 7c01 7c02  ..t.t.|.....|.|.
-00001fa0: a102 0100 6400 5300 7250 0000 0029 0372  ....d.S.rP...).r
-00001fb0: 1900 0000 7239 0000 0072 2800 0000 7225  ....r9...r(...r%
-00001fc0: 0000 0072 1f00 0000 7221 0000 0072 2200  ...r....r!...r".
-00001fd0: 0000 7228 0000 00d5 0000 0073 0200 0000  ..r(.......s....
-00001fe0: 0001 7a18 4169 724c 6973 7453 6572 6961  ..z.AirListSeria
-00001ff0: 6c69 7a65 722e 7570 6461 7465 2901 4629  lizer.update).F)
-00002000: 0772 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
-00002010: 721a 0000 0072 2d00 0000 7228 0000 0072  r....r-...r(...r
-00002020: 4000 0000 7221 0000 0072 2100 0000 721f  @...r!...r!...r.
-00002030: 0000 0072 2200 0000 7239 0000 00ca 0000  ...r"...r9......
-00002040: 0073 0600 0000 0801 0c05 0e05 7239 0000  .s..........r9..
-00002050: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002060: 0000 0300 0000 0000 0000 732c 0000 0065  ..........s,...e
-00002070: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
-00002080: 085a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
-00002090: 005a 0587 0004 005a 0653 0029 07da 1241  .Z.....Z.S.)...A
-000020a0: 6972 456d 7074 7953 6572 6961 6c69 7a65  irEmptySerialize
-000020b0: 7263 0100 0000 0000 0000 0000 0000 0300  rc..............
-000020c0: 0000 0400 0000 0f00 0000 731a 0000 0074  ..........s....t
-000020d0: 0074 017c 0083 026a 027c 0169 007c 02a4  .t.|...j.|.i.|..
-000020e0: 018e 0101 0064 0053 0072 5000 0000 2903  .....d.S.rP...).
-000020f0: 7219 0000 0072 8200 0000 721a 0000 0072  r....r....r....r
-00002100: 1b00 0000 721f 0000 0072 2100 0000 7222  ....r....r!...r"
-00002110: 0000 0072 1a00 0000 db00 0000 7302 0000  ...r........s...
-00002120: 0000 017a 1b41 6972 456d 7074 7953 6572  ...z.AirEmptySer
-00002130: 6961 6c69 7a65 722e 5f5f 696e 6974 5f5f  ializer.__init__
-00002140: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00002150: 0001 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
-00002160: 8300 8201 6400 5300 7250 0000 00a9 01da  ....d.S.rP......
-00002170: 0e4e 6f74 496d 706c 656d 656e 7465 6472  .NotImplementedr
-00002180: 2500 0000 7221 0000 0072 2100 0000 7222  %...r!...r!...r"
-00002190: 0000 0072 2800 0000 de00 0000 7302 0000  ...r(.......s...
-000021a0: 0000 017a 1941 6972 456d 7074 7953 6572  ...z.AirEmptySer
-000021b0: 6961 6c69 7a65 722e 7570 6461 7465 6302  ializer.updatec.
-000021c0: 0000 0000 0000 0000 0000 0002 0000 0001  ................
-000021d0: 0000 0043 0000 0073 0a00 0000 7400 8300  ...C...s....t...
-000021e0: 8201 6400 5300 7250 0000 0072 8300 0000  ..d.S.rP...r....
-000021f0: 7229 0000 0072 2100 0000 7221 0000 0072  r)...r!...r!...r
-00002200: 2200 0000 722a 0000 00e1 0000 0073 0200  "...r*.......s..
-00002210: 0000 0001 7a19 4169 7245 6d70 7479 5365  ....z.AirEmptySe
-00002220: 7269 616c 697a 6572 2e63 7265 6174 6529  rializer.create)
-00002230: 0772 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
-00002240: 721a 0000 0072 2800 0000 722a 0000 0072  r....r(...r*...r
-00002250: 4000 0000 7221 0000 0072 2100 0000 721f  @...r!...r!...r.
-00002260: 0000 0072 2200 0000 7282 0000 00d9 0000  ...r"...r.......
-00002270: 0073 0600 0000 0802 0c03 0803 7282 0000  .s..........r...
-00002280: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002290: 0000 0300 0000 0000 0000 731c 0000 0065  ..........s....e
-000022a0: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
-000022b0: 085a 0387 0004 005a 0453 0029 03da 1441  .Z.....Z.S.)...A
-000022c0: 6972 4479 6e61 6d69 6353 6572 6961 6c69  irDynamicSeriali
-000022d0: 7a65 7263 0100 0000 0000 0000 0000 0000  zerc............
-000022e0: 0600 0000 0400 0000 0f00 0000 7374 0000  ............st..
-000022f0: 007c 02a0 0064 01a1 017d 0374 017c 0383  .|...d...}.t.|..
-00002300: 0174 026b 0273 1e74 0364 0283 0182 017c  .t.k.s.t.d.....|
-00002310: 03a0 04a1 0044 005d 325c 027d 047d 057c  .....D.]2\.}.}.|
-00002320: 057c 006a 056a 057c 043c 007c 047c 006a  .|.j.j.|.<.|.|.j
-00002330: 056a 057c 0419 005f 067c 0467 017c 006a  .j.|..._.|.g.|.j
-00002340: 056a 057c 0419 005f 0771 2674 0874 097c  .j.|..._.q&t.t.|
-00002350: 0083 026a 0a7c 0169 007c 02a4 018e 0101  ...j.|.i.|......
-00002360: 0064 0053 0029 034e da06 7661 6c75 6573  .d.S.).N..values
-00002370: 7a16 7661 6c75 6573 2073 686f 756c 6420  z.values should 
-00002380: 6265 2064 6963 742e 290b 7218 0000 0072  be dict.).r....r
-00002390: 7200 0000 7271 0000 00da 0954 7970 6545  r...rq.....TypeE
-000023a0: 7272 6f72 725d 0000 0072 4300 0000 7257  rrorr]...rC...rW
-000023b0: 0000 00da 0c73 6f75 7263 655f 6174 7472  .....source_attr
-000023c0: 7372 1900 0000 7285 0000 0072 1a00 0000  sr....r....r....
-000023d0: 2906 721c 0000 0072 1d00 0000 721e 0000  ).r....r....r...
-000023e0: 0072 8600 0000 7277 0000 0072 7800 0000  .r....rw...rx...
-000023f0: 721f 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
-00002400: 1a00 0000 e600 0000 7310 0000 0000 010a  ........s.......
-00002410: 010c 0108 0110 010c 010e 0112 017a 1d41  .............z.A
-00002420: 6972 4479 6e61 6d69 6353 6572 6961 6c69  irDynamicSeriali
-00002430: 7a65 722e 5f5f 696e 6974 5f5f 2905 7230  zer.__init__).r0
-00002440: 0000 0072 3100 0000 7232 0000 0072 1a00  ...r1...r2...r..
-00002450: 0000 7240 0000 0072 2100 0000 7221 0000  ..r@...r!...r!..
-00002460: 0072 1f00 0000 7222 0000 0072 8500 0000  .r....r"...r....
-00002470: e500 0000 7302 0000 0008 0172 8500 0000  ....s......r....
-00002480: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002490: 0004 0000 0000 0000 0073 4800 0000 6500  .........sH...e.
-000024a0: 5a01 6400 5a02 6503 6504 6505 6602 1900  Z.d.Z.e.e.e.f...
-000024b0: 6506 6401 9c02 8700 6601 6402 6403 840c  e.d.....f.d.d...
-000024c0: 5a07 6508 6601 8700 6601 6404 6405 8409  Z.e.f...f.d.d...
-000024d0: 5a09 8700 6601 6406 6407 8408 5a0a 8700  Z...f.d.d...Z...
-000024e0: 0400 5a0b 5300 2908 da16 4169 7244 6174  ..Z.S.)...AirDat
-000024f0: 6163 6c61 7373 5365 7269 616c 697a 6572  aclassSerializer
-00002500: 2902 7273 0000 00da 0672 6574 7572 6e63  ).rs.....returnc
-00002510: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00002520: 0500 0000 0300 0000 7368 0000 0074 0074  ........sh...t.t
-00002530: 017c 0083 02a0 027c 01a1 017d 027c 006a  .|.....|...}.|.j
-00002540: 036a 047d 037c 026a 05a0 06a1 0044 005d  .j.}.|.j.....D.]
-00002550: 407d 0474 077c 027c 0483 0274 086b 0272  @}.t.|.|...t.k.r
-00002560: 227c 006a 0972 4a74 077c 006a 097c 0464  "|.j.rJt.|.j.|.d
-00002570: 0083 037d 056e 0c74 077c 037c 0464 0083  ...}.n.t.|.|.d..
-00002580: 037d 0574 0a7c 027c 047c 0583 0301 0071  .}.t.|.|.|.....q
-00002590: 227c 0253 0072 5000 0000 290b 7219 0000  "|.S.rP...).r...
-000025a0: 0072 8900 0000 da11 746f 5f69 6e74 6572  .r......to_inter
-000025b0: 6e61 6c5f 7661 6c75 6572 3300 0000 da09  nal_valuer3.....
-000025c0: 6461 7461 636c 6173 7372 7500 0000 da04  dataclassru.....
-000025d0: 6b65 7973 7236 0000 0072 0600 0000 7226  keysr6...r....r&
-000025e0: 0000 0072 3700 0000 2906 721c 0000 0072  ...r7...).r....r
-000025f0: 7300 0000 7226 0000 0072 8c00 0000 7277  s...r&...r....rw
-00002600: 0000 0072 7800 0000 721f 0000 0072 2100  ...rx...r....r!.
-00002610: 0000 7222 0000 0072 8b00 0000 f200 0000  ..r"...r........
-00002620: 7312 0000 0000 0110 0108 010e 010e 0106  s...............
-00002630: 0110 020c 010e 017a 2841 6972 4461 7461  .......z(AirData
-00002640: 636c 6173 7353 6572 6961 6c69 7a65 722e  classSerializer.
-00002650: 746f 5f69 6e74 6572 6e61 6c5f 7661 6c75  to_internal_valu
-00002660: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00002670: 0000 0400 0000 0300 0000 7338 0000 007c  ..........s8...|
-00002680: 006a 0072 2874 017c 006a 0064 0164 0083  .j.r(t.|.j.d.d..
-00002690: 0372 2874 017c 006a 006a 027c 006a 0364  .r(t.|.j.j.|.j.d
-000026a0: 0083 037c 005f 0274 0474 057c 0083 02a0  ...|._.t.t.|....
-000026b0: 067c 01a1 0153 0029 024e 7226 0000 0029  .|...S.).Nr&...)
-000026c0: 0772 3500 0000 7236 0000 0072 2600 0000  .r5...r6...r&...
-000026d0: da06 736f 7572 6365 7219 0000 0072 8900  ..sourcer....r..
-000026e0: 0000 da0e 7275 6e5f 7661 6c69 6461 7469  ....run_validati
-000026f0: 6f6e 2902 721c 0000 0072 7300 0000 721f  on).r....rs...r.
-00002700: 0000 0072 2100 0000 7222 0000 0072 8f00  ...r!...r"...r..
-00002710: 0000 fe00 0000 7306 0000 0000 0114 0114  ......s.........
-00002720: 017a 2541 6972 4461 7461 636c 6173 7353  .z%AirDataclassS
-00002730: 6572 6961 6c69 7a65 722e 7275 6e5f 7661  erializer.run_va
-00002740: 6c69 6461 7469 6f6e 6302 0000 0000 0000  lidationc.......
-00002750: 0000 0000 0003 0000 0004 0000 0003 0000  ................
-00002760: 0073 4200 0000 7c01 6400 7501 7232 7400  .sB...|.d.u.r2t.
-00002770: 7c01 7401 8302 7232 7c00 6a02 4400 5d18  |.t...r2|.j.D.].
-00002780: 7d02 7c02 6a03 7c01 7601 7218 6400 7c01  }.|.j.|.v.r.d.|.
-00002790: 7c02 6a03 3c00 7118 7404 7405 7c00 8302  |.j.<.q.t.t.|...
-000027a0: a006 7c01 a101 5300 7250 0000 0029 0772  ..|...S.rP...).r
-000027b0: 5e00 0000 7271 0000 00da 105f 7772 6974  ^...rq....._writ
-000027c0: 6162 6c65 5f66 6965 6c64 7372 5700 0000  able_fieldsrW...
-000027d0: 7219 0000 0072 8900 0000 727f 0000 0029  r....r....r....)
-000027e0: 0372 1c00 0000 7226 0000 0072 6800 0000  .r....r&...rh...
-000027f0: 721f 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
-00002800: 7f00 0000 0301 0000 730c 0000 0000 0108  ........s.......
-00002810: 010a 010a 010a 010c 017a 2841 6972 4461  .........z(AirDa
-00002820: 7461 636c 6173 7353 6572 6961 6c69 7a65  taclassSerialize
-00002830: 722e 746f 5f72 6570 7265 7365 6e74 6174  r.to_representat
-00002840: 696f 6e29 0c72 3000 0000 7231 0000 0072  ion).r0...r1...r
-00002850: 3200 0000 7203 0000 0072 8000 0000 7204  2...r....r....r.
-00002860: 0000 0072 1200 0000 728b 0000 0072 0600  ...r....r....r..
-00002870: 0000 728f 0000 0072 7f00 0000 7240 0000  ..r....r....r@..
-00002880: 0072 2100 0000 7221 0000 0072 1f00 0000  .r!...r!...r....
-00002890: 7222 0000 0072 8900 0000 f100 0000 7306  r"...r........s.
-000028a0: 0000 0008 011c 0c10 0572 8900 0000 4e29  .........r....N)
-000028b0: 28da 0674 7970 696e 6772 0200 0000 7203  (..typingr....r.
-000028c0: 0000 0072 0400 0000 da04 7575 6964 7205  ...r......uuidr.
-000028d0: 0000 00da 1572 6573 745f 6672 616d 6577  .....rest_framew
-000028e0: 6f72 6b2e 6669 656c 6473 7206 0000 00da  ork.fieldsr.....
-000028f0: 1872 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
-00002900: 7265 6c61 7469 6f6e 7372 0700 0000 5a14  relationsr....Z.
-00002910: 7265 7374 5f66 7261 6d65 776f 726b 2e75  rest_framework.u
-00002920: 7469 6c73 7208 0000 00da 0e72 6573 745f  tilsr......rest_
-00002930: 6672 616d 6577 6f72 6b72 0900 0000 da10  frameworkr......
-00002940: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
-00002950: 720a 0000 005a 2672 6573 745f 6672 616d  r....Z&rest_fram
-00002960: 6577 6f72 6b5f 6461 7461 636c 6173 7365  ework_dataclasse
-00002970: 732e 7365 7269 616c 697a 6572 7372 0b00  s.serializersr..
-00002980: 0000 5a20 7265 7374 5f66 7261 6d65 776f  ..Z rest_framewo
-00002990: 726b 5f64 6174 6163 6c61 7373 6573 2e74  rk_dataclasses.t
-000029a0: 7970 6573 720c 0000 005a 2061 6972 5f64  ypesr....Z air_d
-000029b0: 7266 5f72 656c 6174 696f 6e2e 636f 6e74  rf_relation.cont
-000029c0: 6578 745f 6275 696c 6465 7272 0d00 0000  ext_builderr....
-000029d0: 5a1d 6169 725f 6472 665f 7265 6c61 7469  Z.air_drf_relati
-000029e0: 6f6e 2e65 7874 7261 5f6b 7761 7267 7372  on.extra_kwargsr
-000029f0: 0e00 0000 5a17 6169 725f 6472 665f 7265  ....Z.air_drf_re
-00002a00: 6c61 7469 6f6e 2e66 6965 6c64 7372 0f00  lation.fieldsr..
-00002a10: 0000 da28 6169 725f 6472 665f 7265 6c61  ...(air_drf_rela
-00002a20: 7469 6f6e 2e70 7265 6c6f 6164 5f6f 626a  tion.preload_obj
-00002a30: 6563 7473 5f6d 616e 6167 6572 7210 0000  ects_managerr...
-00002a40: 00da 2661 6972 5f64 7266 5f72 656c 6174  ..&air_drf_relat
-00002a50: 696f 6e2e 7175 6572 7973 6574 5f6f 7074  ion.queryset_opt
-00002a60: 696d 697a 6174 696f 6e72 1100 0000 7212  imizationr....r.
-00002a70: 0000 00da 0a53 6572 6961 6c69 7a65 7272  .....Serializerr
-00002a80: 1400 0000 da0f 4d6f 6465 6c53 6572 6961  ......ModelSeria
-00002a90: 6c69 7a65 7272 4100 0000 da0e 4c69 7374  lizerrA.....List
-00002aa0: 5365 7269 616c 697a 6572 7239 0000 0072  Serializerr9...r
-00002ab0: 8200 0000 7285 0000 0072 8900 0000 7221  ....r....r....r!
-00002ac0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00002ad0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002ae0: 732a 0000 0014 010c 010c 010c 010c 010c  s*..............
-00002af0: 010c 010c 010c 020c 010c 010c 010c 010c  ................
-00002b00: 020c 0312 2514 7f00 1212 0f10 0c10 0c    ....%..........
+000000d0: 0100 6400 640e 6c1c 6d1d 5a1d 0100 6400  ..d.d.l.m.Z...d.
+000000e0: 640f 6c1e 6d1f 5a1f 0100 6501 6410 6513  d.l.m.Z...e.d.e.
+000000f0: 6411 8d02 5a20 4700 6412 6413 8400 6413  d...Z G.d.d...d.
+00000100: 650d 6a21 8303 5a22 4700 6414 6415 8400  e.j!..Z"G.d.d...
+00000110: 6415 650d 6a23 6522 8304 5a24 4700 6416  d.e.j#e"..Z$G.d.
+00000120: 6417 8400 6417 650d 6a25 8303 5a26 4700  d...d.e.j%..Z&G.
+00000130: 6418 6419 8400 6419 6522 8303 5a27 4700  d.d...d.e"..Z'G.
+00000140: 641a 641b 8400 641b 6527 8303 5a28 4700  d.d...d.e'..Z(G.
+00000150: 641c 641d 8400 641d 6511 8303 5a29 641e  d.d...d.e...Z)d.
+00000160: 5300 291f e900 0000 0029 03da 0754 7970  S.)......)...Typ
+00000170: 6556 6172 da04 4469 6374 da03 416e 7929  eVar..Dict..Any)
+00000180: 01da 0455 5549 4429 01da 0565 6d70 7479  ...UUID)...empty
+00000190: 2901 da16 5072 696d 6172 794b 6579 5265  )...PrimaryKeyRe
+000001a0: 6c61 7465 6446 6965 6c64 2901 da0a 6d6f  latedField)...mo
+000001b0: 6465 6c5f 6d65 7461 2901 da0b 7365 7269  del_meta)...seri
+000001c0: 616c 697a 6572 7329 01da 0a46 6f72 6569  alizers)...Forei
+000001d0: 676e 4b65 7929 01da 1344 6174 6163 6c61  gnKey)...Datacla
+000001e0: 7373 5365 7269 616c 697a 6572 2901 da09  ssSerializer)...
+000001f0: 4461 7461 636c 6173 7329 01da 1b73 6574  Dataclass)...set
+00000200: 5f65 6d70 7479 5f72 6571 7565 7374 5f69  _empty_request_i
+00000210: 6e5f 6b77 6172 6773 2901 da12 4578 7472  n_kwargs)...Extr
+00000220: 614b 7761 7267 7346 6163 746f 7279 2901  aKwargsFactory).
+00000230: da0f 4169 7252 656c 6174 6564 4669 656c  ..AirRelatedFiel
+00000240: 6429 01da 1550 7265 6c6f 6164 4f62 6a65  d)...PreloadObje
+00000250: 6374 734d 616e 6167 6572 2901 da11 6f70  ctsManager)...op
+00000260: 7469 6d69 7a65 5f71 7565 7279 7365 7429  timize_queryset)
+00000270: 01da 0f73 7472 696e 6769 6679 5f75 7569  ...stringify_uui
+00000280: 6473 da01 5429 01da 0562 6f75 6e64 6300  ds..T)...boundc.
+00000290: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+000002a0: 0000 0000 0000 0073 5600 0000 6500 5a01  .......sV...e.Z.
+000002b0: 6400 5a02 8700 6601 6401 6402 8408 5a03  d.Z...f.d.d...Z.
+000002c0: 6403 6404 8400 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
+000002d0: 640e 8700 6601 6408 6409 8409 5a06 8700  d...f.d.d...Z...
+000002e0: 6601 640a 640b 8408 5a07 6508 8700 6601  f.d.d...Z.e...f.
+000002f0: 640c 640d 8408 8301 5a09 8700 0400 5a0a  d.d.....Z.....Z.
+00000300: 5300 290f da0d 4169 7253 6572 6961 6c69  S.)...AirSeriali
+00000310: 7a65 7263 0100 0000 0000 0000 0000 0000  zerc............
+00000320: 0300 0000 0400 0000 0f00 0000 732a 0000  ............s*..
+00000330: 0064 007c 005f 007c 02a0 0164 0164 00a1  .d.|._.|...d.d..
+00000340: 027c 005f 0274 0383 006a 047c 0169 007c  .|._.t...j.|.i.|
+00000350: 02a4 018e 0101 0064 0053 00a9 024e da0f  .......d.S...N..
+00000360: 7072 656c 6f61 645f 6f62 6a65 6374 7329  preload_objects)
+00000370: 05da 185f 7072 656c 6f61 645f 6f62 6a65  ..._preload_obje
+00000380: 6374 735f 6d61 6e61 6765 72da 0370 6f70  cts_manager..pop
+00000390: 7217 0000 00da 0573 7570 6572 da08 5f5f  r......super..__
+000003a0: 696e 6974 5f5f a903 da04 7365 6c66 da04  init__....self..
+000003b0: 6172 6773 da06 6b77 6172 6773 a901 da09  args..kwargs....
+000003c0: 5f5f 636c 6173 735f 5fa9 00fa 552f 5573  __class__...U/Us
+000003d0: 6572 732f 6b69 7269 6c6c 6365 6c69 7365  ers/kirillcelise
+000003e0: 762f 7072 6f6a 6563 7473 2f70 7974 686f  v/projects/pytho
+000003f0: 6e2f 6169 722d 6472 662d 7265 6c61 7469  n/air-drf-relati
+00000400: 6f6e 2f61 6972 5f64 7266 5f72 656c 6174  on/air_drf_relat
+00000410: 696f 6e2f 7365 7269 616c 697a 6572 732e  ion/serializers.
+00000420: 7079 721b 0000 0016 0000 0073 0600 0000  pyr........s....
+00000430: 0001 0601 0e01 7a16 4169 7253 6572 6961  ......z.AirSeria
+00000440: 6c69 7a65 722e 5f5f 696e 6974 5f5f 6303  lizer.__init__c.
+00000450: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+00000460: 0000 0043 0000 0073 0c00 0000 7400 6401  ...C...s....t.d.
+00000470: 8301 8201 6400 5300 2902 4e7a 1f60 7570  ....d.S.).Nz.`up
+00000480: 6461 7465 2829 6020 6d75 7374 2062 6520  date()` must be 
+00000490: 696d 706c 656d 656e 7465 642e a901 da13  implemented.....
+000004a0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+000004b0: 726f 72a9 0372 1d00 0000 da08 696e 7374  ror..r......inst
+000004c0: 616e 6365 da0e 7661 6c69 6461 7465 645f  ance..validated_
+000004d0: 6461 7461 7222 0000 0072 2200 0000 7223  datar"...r"...r#
+000004e0: 0000 00da 0675 7064 6174 651b 0000 0073  .....update....s
+000004f0: 0200 0000 0001 7a14 4169 7253 6572 6961  ......z.AirSeria
+00000500: 6c69 7a65 722e 7570 6461 7465 6302 0000  lizer.updatec...
+00000510: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000520: 0043 0000 0073 0c00 0000 7400 6401 8301  .C...s....t.d...
+00000530: 8201 6400 5300 2902 4e7a 1f60 6372 6561  ..d.S.).Nz.`crea
+00000540: 7465 2829 6020 6d75 7374 2062 6520 696d  te()` must be im
+00000550: 706c 656d 656e 7465 642e 7224 0000 00a9  plemented.r$....
+00000560: 0272 1d00 0000 7228 0000 0072 2200 0000  .r....r(...r"...
+00000570: 7222 0000 0072 2300 0000 da06 6372 6561  r"...r#.....crea
+00000580: 7465 1e00 0000 7302 0000 0000 017a 1441  te....s......z.A
+00000590: 6972 5365 7269 616c 697a 6572 2e63 7265  irSerializer.cre
+000005a0: 6174 6546 6302 0000 0000 0000 0000 0000  ateFc...........
+000005b0: 0002 0000 0003 0000 0003 0000 0073 2e00  .............s..
+000005c0: 0000 7c00 6a00 6401 7501 721a 7401 a002  ..|.j.d.u.r.t...
+000005d0: 7c00 a101 a003 a100 7c00 5f04 7405 7406  |.......|._.t.t.
+000005e0: 7c00 8302 a007 7c01 a101 0100 6400 5300  |.....|.....d.S.
+000005f0: 2902 4e46 2908 7217 0000 0072 1000 0000  ).NF).r....r....
+00000600: da1b 6765 745f 7072 656c 6f61 645f 6f62  ..get_preload_ob
+00000610: 6a65 6374 735f 6d61 6e61 6765 72da 0469  jects_manager..i
+00000620: 6e69 7472 1800 0000 721a 0000 0072 1500  nitr....r....r..
+00000630: 0000 da08 6973 5f76 616c 6964 a902 721d  ....is_valid..r.
+00000640: 0000 00da 0f72 6169 7365 5f65 7863 6570  .....raise_excep
+00000650: 7469 6f6e 7220 0000 0072 2200 0000 7223  tionr ...r"...r#
+00000660: 0000 0072 2e00 0000 2100 0000 7306 0000  ...r....!...s...
+00000670: 0000 010a 0110 017a 1641 6972 5365 7269  .......z.AirSeri
+00000680: 616c 697a 6572 2e69 735f 7661 6c69 6463  alizer.is_validc
+00000690: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+000006a0: 0300 0000 0300 0000 7314 0000 0074 0083  ........s....t..
+000006b0: 00a0 017c 01a1 017d 0274 027c 0283 0153  ...|...}.t.|...S
+000006c0: 00a9 014e 2903 721a 0000 00da 1174 6f5f  ...N).r......to_
+000006d0: 7265 7072 6573 656e 7461 7469 6f6e 7212  representationr.
+000006e0: 0000 0029 0372 1d00 0000 7227 0000 00da  ...).r....r'....
+000006f0: 0464 6174 6172 2000 0000 7222 0000 0072  .datar ...r"...r
+00000700: 2300 0000 7232 0000 0026 0000 0073 0400  #...r2...&...s..
+00000710: 0000 0001 0c01 7a1f 4169 7253 6572 6961  ......z.AirSeria
+00000720: 6c69 7a65 722e 746f 5f72 6570 7265 7365  lizer.to_represe
+00000730: 6e74 6174 696f 6e63 0100 0000 0000 0000  ntationc........
+00000740: 0000 0000 0600 0000 0400 0000 0f00 0000  ................
+00000750: 739e 0000 0047 0064 0164 0284 0064 0283  s....G.d.d...d..
+00000760: 027d 0374 007c 0064 0264 0083 037d 047c  .}.t.|.d.d...}.|
+00000770: 0473 307c 0383 007d 0474 017c 0064 027c  .s0|...}.t.|.d.|
+00000780: 0483 0301 0074 027c 0464 0383 0273 4674  .....t.|.d...sFt
+00000790: 017c 0464 0374 0383 0301 0074 0474 057c  .|.d.t.....t.t.|
+000007a0: 0083 026a 067c 0169 007c 02a4 018e 017d  ...j.|.i.|.....}
+000007b0: 0574 027c 0564 0483 0272 9a7c 056a 0764  .t.|.d...r.|.j.d
+000007c0: 0075 0072 9a7c 056a 0872 9a74 027c 056a  .u.r.|.j.r.t.|.j
+000007d0: 0864 0583 0272 9a7c 056a 086a 0972 9a74  .d...r.|.j.j.r.t
+000007e0: 097c 056a 0a7c 056a 0883 027c 055f 0a7c  .|.j.|.j...|._.|
+000007f0: 0553 0029 064e 6300 0000 0000 0000 0000  .S.).Nc.........
+00000800: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+00000810: 0c00 0000 6500 5a01 6400 5a02 6401 5300  ....e.Z.d.Z.d.S.
+00000820: 2902 7a25 4169 7253 6572 6961 6c69 7a65  ).z%AirSerialize
+00000830: 722e 6d61 6e79 5f69 6e69 742e 3c6c 6f63  r.many_init.<loc
+00000840: 616c 733e 2e4d 6574 614e 2903 da08 5f5f  als>.MetaN)...__
+00000850: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000860: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000870: 7222 0000 0072 2200 0000 7222 0000 0072  r"...r"...r"...r
+00000880: 2300 0000 da04 4d65 7461 2c00 0000 7302  #.....Meta,...s.
+00000890: 0000 0008 0172 3700 0000 da15 6c69 7374  .....r7.....list
+000008a0: 5f73 6572 6961 6c69 7a65 725f 636c 6173  _serializer_clas
+000008b0: 73da 0670 6172 656e 7472 1100 0000 290b  s..parentr....).
+000008c0: da07 6765 7461 7474 72da 0773 6574 6174  ..getattr..setat
+000008d0: 7472 da07 6861 7361 7474 72da 1141 6972  tr..hasattr..Air
+000008e0: 4c69 7374 5365 7269 616c 697a 6572 721a  ListSerializerr.
+000008f0: 0000 0072 1500 0000 da09 6d61 6e79 5f69  ...r......many_i
+00000900: 6e69 7472 3900 0000 da05 6368 696c 6472  nitr9.....childr
+00000910: 1100 0000 7227 0000 0029 06da 0363 6c73  ....r'...)...cls
+00000920: 721e 0000 0072 1f00 0000 7237 0000 00da  r....r....r7....
+00000930: 046d 6574 61da 0a73 6572 6961 6c69 7a65  .meta..serialize
+00000940: 7272 2000 0000 7222 0000 0072 2300 0000  rr ...r"...r#...
+00000950: 723e 0000 002a 0000 0073 2000 0000 0002  r>...*...s .....
+00000960: 0e03 0c01 0401 0601 0c01 0a01 0c01 1602  ................
+00000970: 1401 0601 0aff 0201 06ff 0202 1001 7a17  ..............z.
+00000980: 4169 7253 6572 6961 6c69 7a65 722e 6d61  AirSerializer.ma
+00000990: 6e79 5f69 6e69 7429 0146 290b 7234 0000  ny_init).F).r4..
+000009a0: 0072 3500 0000 7236 0000 0072 1b00 0000  .r5...r6...r....
+000009b0: 7229 0000 0072 2b00 0000 722e 0000 0072  r)...r+...r....r
+000009c0: 3200 0000 da0b 636c 6173 736d 6574 686f  2.....classmetho
+000009d0: 6472 3e00 0000 da0d 5f5f 636c 6173 7363  dr>.....__classc
+000009e0: 656c 6c5f 5f72 2200 0000 7222 0000 0072  ell__r"...r"...r
+000009f0: 2000 0000 7223 0000 0072 1500 0000 1500   ...r#...r......
+00000a00: 0000 730e 0000 0008 010c 0508 0308 030e  ..s.............
+00000a10: 050c 0402 0172 1500 0000 6300 0000 0000  .....r....c.....
+00000a20: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00000a30: 0000 0073 ac00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000a40: 4700 6401 6402 8400 6402 8302 5a03 8700  G.d.d...d...Z...
+00000a50: 6601 6403 6404 8408 5a04 8700 6601 6405  f.d.d...Z...f.d.
+00000a60: 6406 8408 5a05 6407 6408 8400 5a06 6409  d...Z.d.d...Z.d.
+00000a70: 640a 8400 5a07 6422 8700 6601 640c 640d  d...Z.d"..f.d.d.
+00000a80: 8409 5a08 640e 640f 8400 5a09 6410 6411  ..Z.d.d...Z.d.d.
+00000a90: 8400 5a0a 6412 6413 8400 5a0b 6414 6415  ..Z.d.d...Z.d.d.
+00000aa0: 8400 5a0c 6416 6417 8400 5a0d 6418 6419  ..Z.d.d...Z.d.d.
+00000ab0: 8400 5a0e 641a 641b 8400 5a0f 641c 641d  ..Z.d.d...Z.d.d.
+00000ac0: 8400 5a10 8700 6601 641e 641f 8408 5a11  ..Z...f.d.d...Z.
+00000ad0: 8700 6601 6420 6421 8408 5a12 8700 0400  ..f.d d!..Z.....
+00000ae0: 5a13 5300 2923 da12 4169 724d 6f64 656c  Z.S.)#..AirModel
+00000af0: 5365 7269 616c 697a 6572 6300 0000 0000  Serializerc.....
+00000b00: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00000b10: 0000 0073 2400 0000 6500 5a01 6400 5a02  ...s$...e.Z.d.Z.
+00000b20: 6401 5a03 6402 5a04 6402 5a05 6402 5a06  d.Z.d.Z.d.Z.d.Z.
+00000b30: 6900 5a07 6403 5a08 6401 5300 2904 7a17  i.Z.d.Z.d.S.).z.
+00000b40: 4169 724d 6f64 656c 5365 7269 616c 697a  AirModelSerializ
+00000b50: 6572 2e4d 6574 614e 7222 0000 0054 2909  er.MetaNr"...T).
+00000b60: 7234 0000 0072 3500 0000 7236 0000 00da  r4...r5...r6....
+00000b70: 056d 6f64 656c da06 6669 656c 6473 da10  .model..fields..
+00000b80: 7265 6164 5f6f 6e6c 795f 6669 656c 6473  read_only_fields
+00000b90: 5a11 7772 6974 655f 6f6e 6c79 5f66 6965  Z.write_only_fie
+00000ba0: 6c64 73da 0c65 7874 7261 5f6b 7761 7267  lds..extra_kwarg
+00000bb0: 7372 1100 0000 7222 0000 0072 2200 0000  sr....r"...r"...
+00000bc0: 7222 0000 0072 2300 0000 7237 0000 003f  r"...r#...r7...?
+00000bd0: 0000 0073 0c00 0000 0801 0401 0401 0401  ...s............
+00000be0: 0401 0401 7237 0000 0063 0100 0000 0000  ....r7...c......
+00000bf0: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
+00000c00: 0000 73cc 0000 007c 02a0 0064 0164 00a1  ..s....|...d.d..
+00000c10: 027c 005f 017c 02a0 0064 0264 00a1 027c  .|._.|...d.d...|
+00000c20: 005f 0264 037c 005f 0364 047c 0276 0072  ._.d.|._.d.|.v.r
+00000c30: 3a7c 02a0 0064 0464 03a1 027c 005f 036e  :|...d.d...|._.n
+00000c40: 1c74 047c 006a 0564 0483 0272 5674 067c  .t.|.j.d...rVt.|
+00000c50: 006a 0564 0464 0383 037c 005f 037c 02a0  .j.d.d...|._.|..
+00000c60: 0064 0569 00a1 027c 005f 0764 067c 0276  .d.i...|._.d.|.v
+00000c70: 0172 7674 087c 0264 078d 0101 007c 006a  .rvt.|.d.....|.j
+00000c80: 0173 887c 006a 097c 0264 078d 0101 007c  .s.|.j.|.d.....|
+00000c90: 006a 0273 987c 00a0 0a7c 02a1 0101 007c  .j.s.|...|.....|
+00000ca0: 00a0 0ba1 007c 005f 0c7c 00a0 0da1 0001  .....|._.|......
+00000cb0: 0074 0e74 0f7c 0083 026a 107c 0169 007c  .t.t.|...j.|.i.|
+00000cc0: 02a4 018e 0101 007c 00a0 11a1 0001 0064  .......|.......d
+00000cd0: 0053 0029 084e da06 6163 7469 6f6e da04  .S.).N..action..
+00000ce0: 7573 6572 5472 1100 0000 7249 0000 00da  userTr....rI....
+00000cf0: 0763 6f6e 7465 7874 a901 721f 0000 0029  .context..r....)
+00000d00: 1272 1900 0000 724a 0000 0072 4b00 0000  .r....rJ...rK...
+00000d10: 7211 0000 0072 3c00 0000 7237 0000 0072  r....r<...r7...r
+00000d20: 3a00 0000 da15 5f69 6e69 7469 616c 5f65  :....._initial_e
+00000d30: 7874 7261 5f6b 7761 7267 7372 0d00 0000  xtra_kwargsr....
+00000d40: da15 5f73 6574 5f61 6374 696f 6e5f 6672  .._set_action_fr
+00000d50: 6f6d 5f76 6965 77da 165f 7365 745f 7573  om_view.._set_us
+00000d60: 6572 5f66 726f 6d5f 7265 7175 6573 74da  er_from_request.
+00000d70: 115f 6765 745f 6578 7472 615f 6b77 6172  ._get_extra_kwar
+00000d80: 6773 7249 0000 00da 1e5f 7570 6461 7465  gsrI....._update
+00000d90: 5f65 7874 7261 5f6b 7761 7267 735f 696e  _extra_kwargs_in
+00000da0: 5f66 6965 6c64 7372 1a00 0000 7245 0000  _fieldsr....rE..
+00000db0: 0072 1b00 0000 da0e 5f75 7064 6174 655f  .r......_update_
+00000dc0: 6669 656c 6473 721c 0000 0072 2000 0000  fieldsr....r ...
+00000dd0: 7222 0000 0072 2300 0000 721b 0000 0047  r"...r#...r....G
+00000de0: 0000 0073 2400 0000 0001 0e01 0e01 0601  ...s$...........
+00000df0: 0801 1001 0c01 1001 0e01 0801 0a02 0601  ................
+00000e00: 0c01 0601 0a01 0a01 0801 1601 7a1b 4169  ............z.Ai
+00000e10: 724d 6f64 656c 5365 7269 616c 697a 6572  rModelSerializer
+00000e20: 2e5f 5f69 6e69 745f 5f63 0300 0000 0000  .__init__c......
+00000e30: 0000 0000 0000 0400 0000 0400 0000 0300  ................
+00000e40: 0000 7324 0000 0074 0074 017c 0083 027d  ..s$...t.t.|...}
+00000e50: 037c 0173 187c 03a0 027c 02a1 0153 007c  .|.s.|...|...S.|
+00000e60: 03a0 037c 017c 02a1 0253 0072 3100 0000  ...|.|...S.r1...
+00000e70: 2904 721a 0000 0072 4500 0000 722b 0000  ).r....rE...r+..
+00000e80: 0072 2900 0000 2904 721d 0000 0072 2700  .r)...).r....r'.
+00000e90: 0000 7228 0000 005a 0b73 7570 6572 5f63  ..r(...Z.super_c
+00000ea0: 6c61 7373 7220 0000 0072 2200 0000 7223  lassr ...r"...r#
+00000eb0: 0000 00da 1075 7064 6174 655f 6f72 5f63  .....update_or_c
+00000ec0: 7265 6174 655c 0000 0073 0400 0000 0001  reate\...s......
+00000ed0: 0a01 7a23 4169 724d 6f64 656c 5365 7269  ..z#AirModelSeri
+00000ee0: 616c 697a 6572 2e75 7064 6174 655f 6f72  alizer.update_or
+00000ef0: 5f63 7265 6174 6563 0200 0000 0000 0000  _createc........
+00000f00: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000f10: 730c 0000 007c 00a0 0064 007c 01a1 0253  s....|...d.|...S
+00000f20: 0072 3100 0000 a901 7254 0000 0072 2a00  .r1.....rT...r*.
+00000f30: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
+00000f40: 0072 2b00 0000 6000 0000 7302 0000 0000  .r+...`...s.....
+00000f50: 017a 1941 6972 4d6f 6465 6c53 6572 6961  .z.AirModelSeria
+00000f60: 6c69 7a65 722e 6372 6561 7465 6303 0000  lizer.createc...
+00000f70: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00000f80: 0043 0000 0073 0c00 0000 7c00 a000 7c01  .C...s....|...|.
+00000f90: 7c02 a102 5300 7231 0000 0072 5500 0000  |...S.r1...rU...
+00000fa0: 7226 0000 0072 2200 0000 7222 0000 0072  r&...r"...r"...r
+00000fb0: 2300 0000 7229 0000 0063 0000 0073 0200  #...r)...c...s..
+00000fc0: 0000 0001 7a19 4169 724d 6f64 656c 5365  ....z.AirModelSe
+00000fd0: 7269 616c 697a 6572 2e75 7064 6174 6546  rializer.updateF
+00000fe0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000ff0: 0003 0000 0003 0000 0073 1a00 0000 7c00  .........s....|.
+00001000: a000 a100 0100 7401 7402 7c00 8302 6a03  ......t.t.|...j.
+00001010: 7c01 6401 8d01 5300 2902 4ea9 0172 3000  |.d...S.).N..r0.
+00001020: 0000 2904 da1a 5f66 696c 7465 725f 7175  ..)..._filter_qu
+00001030: 6572 7973 6574 5f62 795f 6669 656c 6473  eryset_by_fields
+00001040: 721a 0000 0072 4500 0000 722e 0000 0072  r....rE...r....r
+00001050: 2f00 0000 7220 0000 0072 2200 0000 7223  /...r ...r"...r#
+00001060: 0000 0072 2e00 0000 6600 0000 7304 0000  ...r....f...s...
+00001070: 0000 0108 017a 1b41 6972 4d6f 6465 6c53  .....z.AirModelS
+00001080: 6572 6961 6c69 7a65 722e 6973 5f76 616c  erializer.is_val
+00001090: 6964 6301 0000 0000 0000 0000 0000 0008  idc.............
+000010a0: 0000 0004 0000 0043 0000 0073 bc00 0000  .......C...s....
+000010b0: 7400 7c00 6a01 6401 8302 7310 6400 5300  t.|.j.d...s.d.S.
+000010c0: 7402 a003 7c00 6a01 6a04 a101 7d01 6402  t...|.j.j...}.d.
+000010d0: 6403 8400 7c00 6a05 a006 a100 4400 8301  d...|.j.....D...
+000010e0: 7d02 7c02 4400 5d0c 7d03 7c00 6a05 7c03  }.|.D.].}.|.j.|.
+000010f0: 3d00 7136 7c00 6a05 a006 a100 4400 5d68  =.q6|.j.....D.]h
+00001100: 5c02 7d04 7d05 7407 7c05 7408 8302 7362  \.}.}.t.|.t...sb
+00001110: 714e 7c00 7c05 5f09 7c01 6a0a 7c04 1900  qN|.|._.|.j.|...
+00001120: 6a0b 7d06 7c05 6a0c 7d07 7c06 6a0d 7388  j.}.|.j.}.|.j.s.
+00001130: 6404 7c05 5f0e 714e 7c06 6a0f 724e 7c07  d.|._.qN|.j.rN|.
+00001140: a010 6405 a101 6400 7500 72a2 6406 7c05  ..d...d.u.r.d.|.
+00001150: 5f11 7c07 a010 6407 a101 6400 7500 724e  _.|...d...d.u.rN
+00001160: 6404 7c05 5f12 714e 6400 5300 2908 4e72  d.|._.qNd.S.).Nr
+00001170: 4600 0000 6301 0000 0000 0000 0000 0000  F...c...........
+00001180: 0003 0000 0006 0000 0053 0000 0073 2a00  .........S...s*.
+00001190: 0000 6700 7c00 5d22 5c02 7d01 7d02 7400  ..g.|.]"\.}.}.t.
+000011a0: 7c02 6400 8302 7204 7401 7c02 6400 6401  |.d...r.t.|.d.d.
+000011b0: 8303 7204 7c01 9102 7104 5300 2902 da06  ..r.|...q.S.)...
+000011c0: 6869 6464 656e 5429 0272 3c00 0000 723a  hiddenT).r<...r:
+000011d0: 0000 0029 03da 022e 30da 0a66 6965 6c64  ...)....0..field
+000011e0: 5f6e 616d 65da 0566 6965 6c64 7222 0000  _name..fieldr"..
+000011f0: 0072 2200 0000 7223 0000 00da 0a3c 6c69  .r"...r#.....<li
+00001200: 7374 636f 6d70 3e6e 0000 0073 0400 0000  stcomp>n...s....
+00001210: 0c01 16ff 7a35 4169 724d 6f64 656c 5365  ....z5AirModelSe
+00001220: 7269 616c 697a 6572 2e5f 7570 6461 7465  rializer._update
+00001230: 5f66 6965 6c64 732e 3c6c 6f63 616c 733e  _fields.<locals>
+00001240: 2e3c 6c69 7374 636f 6d70 3e54 da08 7265  .<listcomp>T..re
+00001250: 7175 6972 6564 46da 0a61 6c6c 6f77 5f6e  quiredF..allow_n
+00001260: 756c 6c29 1372 3c00 0000 7237 0000 0072  ull).r<...r7...r
+00001270: 0800 0000 da0e 6765 745f 6669 656c 645f  ......get_field_
+00001280: 696e 666f 7246 0000 0072 4700 0000 da05  inforF...rG.....
+00001290: 6974 656d 73da 0a69 7369 6e73 7461 6e63  items..isinstanc
+000012a0: 6572 0f00 0000 7239 0000 00da 0972 656c  er....r9.....rel
+000012b0: 6174 696f 6e73 da0b 6d6f 6465 6c5f 6669  ations..model_fi
+000012c0: 656c 64da 075f 6b77 6172 6773 da08 6564  eld.._kwargs..ed
+000012d0: 6974 6162 6c65 da09 7265 6164 5f6f 6e6c  itable..read_onl
+000012e0: 79da 046e 756c 6cda 0367 6574 725d 0000  y..null..getr]..
+000012f0: 0072 5e00 0000 2908 721d 0000 00da 0469  .r^...).r......i
+00001300: 6e66 6fda 0d68 6964 6465 6e5f 6669 656c  nfo..hidden_fiel
+00001310: 6473 da02 656c 725a 0000 0072 5b00 0000  ds..elrZ...r[...
+00001320: 7263 0000 00da 0c66 6965 6c64 5f6b 7761  rc.....field_kwa
+00001330: 7267 7372 2200 0000 7222 0000 0072 2300  rgsr"...r"...r#.
+00001340: 0000 7253 0000 006a 0000 0073 2800 0000  ..rS...j...s(...
+00001350: 0001 0c01 0401 0e01 1402 0801 0a01 1201  ................
+00001360: 0a01 0201 0601 0c01 0601 0601 0601 0201  ................
+00001370: 0601 0e01 0601 0e01 7a21 4169 724d 6f64  ........z!AirMod
+00001380: 656c 5365 7269 616c 697a 6572 2e5f 7570  elSerializer._up
+00001390: 6461 7465 5f66 6965 6c64 7363 0100 0000  date_fieldsc....
+000013a0: 0000 0000 0000 0000 0500 0000 0500 0000  ................
+000013b0: 4300 0000 7390 0000 007c 00a0 00a1 007d  C...s....|.....}
+000013c0: 017c 01a0 01a1 0044 005d 7a5c 027d 027d  .|.....D.]z\.}.}
+000013d0: 037c 006a 02a0 037c 02a1 0173 2671 1064  .|.j...|...s&q.d
+000013e0: 007d 0474 047c 0374 0583 0272 467c 036a  .}.t.|.t...rF|.j
+000013f0: 0672 4001 0064 0053 007c 036a 077d 047c  .r@..d.S.|.j.}.|
+00001400: 0473 5664 017c 036a 089b 009d 027d 0474  .sVd.|.j.....}.t
+00001410: 097c 006a 0a7c 0483 0272 1074 0b74 0c7c  .|.j.|...r.t.t.|
+00001420: 006a 0a7c 0483 0283 0172 1074 0c7c 006a  .j.|.....r.t.|.j
+00001430: 0a7c 0483 027c 007c 036a 0d64 028d 027c  .|...|.|.j.d...|
+00001440: 035f 0d71 1064 0053 0029 034e 5a09 7175  ._.q.d.S.).NZ.qu
+00001450: 6572 7973 6574 5f29 0272 1d00 0000 da08  eryset_).r......
+00001460: 7175 6572 7973 6574 290e da13 5f67 6574  queryset)..._get
+00001470: 5f72 656c 6174 6564 5f66 6965 6c64 7372  _related_fieldsr
+00001480: 6000 0000 da0c 696e 6974 6961 6c5f 6461  `.....initial_da
+00001490: 7461 7268 0000 0072 6100 0000 720f 0000  tarh...ra...r...
+000014a0: 00da 1a71 7565 7279 7365 745f 6675 6e63  ...queryset_func
+000014b0: 7469 6f6e 5f64 6973 6162 6c65 645a 1671  tion_disabledZ.q
+000014c0: 7565 7279 7365 745f 6675 6e63 7469 6f6e  ueryset_function
+000014d0: 5f6e 616d 6572 5a00 0000 723c 0000 0072  _namerZ...r<...r
+000014e0: 2100 0000 da08 6361 6c6c 6162 6c65 723a  !.....callabler:
+000014f0: 0000 0072 6d00 0000 2905 721d 0000 00da  ...rm...).r.....
+00001500: 0e72 656c 6174 6564 5f66 6965 6c64 7372  .related_fieldsr
+00001510: 5a00 0000 725b 0000 00da 0d66 756e 6374  Z...r[.....funct
+00001520: 696f 6e5f 6e61 6d65 7222 0000 0072 2200  ion_namer"...r".
+00001530: 0000 7223 0000 0072 5700 0000 8100 0000  ..r#...rW.......
+00001540: 731a 0000 0000 0108 0110 010c 0102 0104  s...............
+00001550: 010a 0106 0106 0106 0104 010c 011c 017a  ...............z
+00001560: 2d41 6972 4d6f 6465 6c53 6572 6961 6c69  -AirModelSeriali
+00001570: 7a65 722e 5f66 696c 7465 725f 7175 6572  zer._filter_quer
+00001580: 7973 6574 5f62 795f 6669 656c 6473 6301  yset_by_fieldsc.
+00001590: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+000015a0: 0000 0043 0000 0073 3600 0000 7400 8300  ...C...s6...t...
+000015b0: 7d01 7c00 6a01 a002 a100 4400 5d20 5c02  }.|.j.....D.] \.
+000015c0: 7d02 7d03 7403 7c03 8301 7404 7405 6602  }.}.t.|...t.t.f.
+000015d0: 7600 7210 7c03 7c01 7c02 3c00 7110 7c01  v.r.|.|.|.<.q.|.
+000015e0: 5300 7231 0000 0029 06da 0464 6963 7472  S.r1...)...dictr
+000015f0: 4700 0000 7260 0000 00da 0474 7970 6572  G...r`.....typer
+00001600: 0f00 0000 7207 0000 0029 0472 1d00 0000  ....r....).r....
+00001610: 7272 0000 0072 5a00 0000 725b 0000 0072  rr...rZ...r[...r
+00001620: 2200 0000 7222 0000 0072 2300 0000 726e  "...r"...r#...rn
+00001630: 0000 0090 0000 0073 0a00 0000 0001 0601  .......s........
+00001640: 1201 1001 0a01 7a26 4169 724d 6f64 656c  ......z&AirModel
+00001650: 5365 7269 616c 697a 6572 2e5f 6765 745f  Serializer._get_
+00001660: 7265 6c61 7465 645f 6669 656c 6473 6301  related_fieldsc.
+00001670: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00001680: 0000 0043 0000 0073 2e00 0000 6401 7c00  ...C...s....d.|.
+00001690: 6a00 6901 7d01 7401 7c00 6a02 7c01 7c00  j.i.}.t.|.j.|.|.
+000016a0: 6a03 6402 8d03 a004 a100 6a05 7d02 7c00  j.d.......j.}.|.
+000016b0: a006 a100 0100 7c02 5300 2903 4e72 4900  ......|.S.).NrI.
+000016c0: 0000 2903 7241 0000 0072 3300 0000 724a  ..).rA...r3...rJ
+000016d0: 0000 0029 0772 4e00 0000 720e 0000 0072  ...).rN...r....r
+000016e0: 3700 0000 724a 0000 0072 2d00 0000 7249  7...rJ...r-...rI
+000016f0: 0000 00da 235f 6465 6c65 7465 5f63 7573  ....#_delete_cus
+00001700: 746f 6d5f 6578 7472 615f 6b77 6172 6773  tom_extra_kwargs
+00001710: 5f69 6e5f 6d65 7461 2903 721d 0000 0072  _in_meta).r....r
+00001720: 3300 0000 7249 0000 0072 2200 0000 7222  3...rI...r"...r"
+00001730: 0000 0072 2300 0000 7251 0000 0097 0000  ...r#...rQ......
+00001740: 0073 0800 0000 0001 0a01 1801 0801 7a24  .s............z$
+00001750: 4169 724d 6f64 656c 5365 7269 616c 697a  AirModelSerializ
+00001760: 6572 2e5f 6765 745f 6578 7472 615f 6b77  er._get_extra_kw
+00001770: 6172 6773 6301 0000 0000 0000 0000 0000  argsc...........
+00001780: 0003 0000 0009 0000 0043 0000 0073 6800  .........C...sh.
+00001790: 0000 7c00 6a00 a001 a100 4400 5d58 5c02  ..|.j.....D.]X\.
+000017a0: 7d01 7d02 7a38 7c00 6a02 6a02 7c01 1900  }.}.z8|.j.j.|...
+000017b0: 6a03 a004 7c02 a101 0100 6900 7c00 6a02  j...|.....i.|.j.
+000017c0: 6a02 7c01 1900 6a05 a501 7c02 a501 7c00  j.|...j...|...|.
+000017d0: 6a02 6a02 7c01 1900 5f05 5700 710a 0400  j.j.|..._.W.q...
+000017e0: 7406 7960 0100 0100 0100 5900 710a 5900  t.y`......Y.q.Y.
+000017f0: 710a 3000 710a 6400 5300 7231 0000 0029  q.0.q.d.S.r1...)
+00001800: 0772 4900 0000 7260 0000 0072 4700 0000  .rI...r`...rG...
+00001810: da08 5f5f 6469 6374 5f5f 7229 0000 0072  ..__dict__r)...r
+00001820: 6400 0000 da08 4b65 7945 7272 6f72 2903  d.....KeyError).
+00001830: 721d 0000 00da 036b 6579 da05 7661 6c75  r......key..valu
+00001840: 6572 2200 0000 7222 0000 0072 2300 0000  er"...r"...r#...
+00001850: 7252 0000 009d 0000 0073 0c00 0000 0001  rR.......s......
+00001860: 1201 0201 1401 2401 0c01 7a31 4169 724d  ......$...z1AirM
+00001870: 6f64 656c 5365 7269 616c 697a 6572 2e5f  odelSerializer._
+00001880: 7570 6461 7465 5f65 7874 7261 5f6b 7761  update_extra_kwa
+00001890: 7267 735f 696e 5f66 6965 6c64 7363 0100  rgs_in_fieldsc..
+000018a0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+000018b0: 0000 4300 0000 7342 0000 0074 007c 006a  ..C...sB...t.|.j
+000018c0: 0164 0183 0273 1064 0053 007c 006a 016a  .d...s.d.S.|.j.j
+000018d0: 02a0 03a1 0044 005d 205c 027d 017d 027c  .....D.] \.}.}.|
+000018e0: 02a0 0464 0264 00a1 0201 007c 02a0 0464  ...d.d.....|...d
+000018f0: 0364 00a1 0201 0071 1c64 0053 0029 044e  .d.....q.d.S.).N
+00001900: 7249 0000 00da 0770 6b5f 6f6e 6c79 7258  rI.....pk_onlyrX
+00001910: 0000 0029 0572 3c00 0000 7237 0000 0072  ...).r<...r7...r
+00001920: 4900 0000 7260 0000 0072 1900 0000 2903  I...r`...r....).
+00001930: 721d 0000 0072 5a00 0000 725b 0000 0072  r....rZ...r[...r
+00001940: 2200 0000 7222 0000 0072 2300 0000 7276  "...r"...r#...rv
+00001950: 0000 00a5 0000 0073 0a00 0000 0001 0c01  .......s........
+00001960: 0401 1401 0c01 7a36 4169 724d 6f64 656c  ......z6AirModel
+00001970: 5365 7269 616c 697a 6572 2e5f 6465 6c65  Serializer._dele
+00001980: 7465 5f63 7573 746f 6d5f 6578 7472 615f  te_custom_extra_
+00001990: 6b77 6172 6773 5f69 6e5f 6d65 7461 6302  kwargs_in_metac.
+000019a0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+000019b0: 0000 0043 0000 0073 2e00 0000 7c01 a000  ...C...s....|...
+000019c0: 6401 6400 a102 7d02 7c02 7314 6400 5300  d.d...}.|.s.d.S.
+000019d0: 7c02 a000 6402 a101 7d03 7c03 722a 7c03  |...d...}.|.r*|.
+000019e0: 6a01 7c00 5f01 6400 5300 2903 4e72 4c00  j.|._.d.S.).NrL.
+000019f0: 0000 da04 7669 6577 2902 7268 0000 0072  ....view).rh...r
+00001a00: 4a00 0000 2904 721d 0000 0072 1f00 0000  J...).r....r....
+00001a10: 724c 0000 0072 7c00 0000 7222 0000 0072  rL...r|...r"...r
+00001a20: 2200 0000 7223 0000 0072 4f00 0000 ac00  "...r#...rO.....
+00001a30: 0000 730c 0000 0000 010c 0104 0104 010a  ..s.............
+00001a40: 0104 017a 2841 6972 4d6f 6465 6c53 6572  ...z(AirModelSer
+00001a50: 6961 6c69 7a65 722e 5f73 6574 5f61 6374  ializer._set_act
+00001a60: 696f 6e5f 6672 6f6d 5f76 6965 7763 0200  ion_from_viewc..
+00001a70: 0000 0000 0000 0000 0000 0500 0000 0400  ................
+00001a80: 0000 4300 0000 7346 0000 007c 01a0 0064  ..C...sF...|...d
+00001a90: 0164 00a1 027d 027c 0273 1464 0053 007c  .d...}.|.s.d.S.|
+00001aa0: 02a0 0064 02a1 017d 037c 0372 4274 017c  ...d...}.|.rBt.|
+00001ab0: 0364 0383 0272 4274 027c 0364 0383 027d  .d...rBt.|.d...}
+00001ac0: 047c 046a 0372 427c 047c 005f 0464 0053  .|.j.rB|.|._.d.S
+00001ad0: 0029 044e 724c 0000 00da 0772 6571 7565  .).NrL.....reque
+00001ae0: 7374 724b 0000 0029 0572 6800 0000 723c  strK...).rh...r<
+00001af0: 0000 0072 3a00 0000 da10 6973 5f61 7574  ...r:.....is_aut
+00001b00: 6865 6e74 6963 6174 6564 724b 0000 0029  henticatedrK...)
+00001b10: 0572 1d00 0000 721f 0000 0072 4c00 0000  .r....r....rL...
+00001b20: 727d 0000 0072 4b00 0000 7222 0000 0072  r}...rK...r"...r
+00001b30: 2200 0000 7223 0000 0072 5000 0000 b400  "...r#...rP.....
+00001b40: 0000 7310 0000 0000 010c 0104 0104 010a  ..s.............
+00001b50: 010e 010a 0106 017a 2941 6972 4d6f 6465  .......z)AirMode
+00001b60: 6c53 6572 6961 6c69 7a65 722e 5f73 6574  lSerializer._set
+00001b70: 5f75 7365 725f 6672 6f6d 5f72 6571 7565  _user_from_reque
+00001b80: 7374 6301 0000 0000 0000 0000 0000 0003  stc.............
+00001b90: 0000 0004 0000 000f 0000 0073 4800 0000  ...........sH...
+00001ba0: 7c02 a000 6401 6402 a102 722e 6403 7c02  |...d.d...r.d.|.
+00001bb0: 7601 721e 7401 7c02 6404 8d01 0100 7c00  v.r.t.|.d.....|.
+00001bc0: 6a02 7c01 6900 7c02 a401 8e01 5300 7403  j.|.i.|.....S.t.
+00001bd0: 8300 6a04 7c00 6701 7c01 a201 5200 6900  ..j.|.g.|...R.i.
+00001be0: 7c02 a401 8e01 5300 2905 4eda 046d 616e  |.....S.).N..man
+00001bf0: 7946 724c 0000 0072 4d00 0000 2905 7219  yFrL...rM...).r.
+00001c00: 0000 0072 0d00 0000 723e 0000 0072 1a00  ...r....r>...r..
+00001c10: 0000 da07 5f5f 6e65 775f 5f29 0372 4000  ....__new__).r@.
+00001c20: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00001c30: 0072 2200 0000 7223 0000 0072 8000 0000  .r"...r#...r....
+00001c40: be00 0000 730a 0000 0000 010c 0108 010a  ....s...........
+00001c50: 0110 017a 1a41 6972 4d6f 6465 6c53 6572  ...z.AirModelSer
+00001c60: 6961 6c69 7a65 722e 5f5f 6e65 775f 5f63  ializer.__new__c
+00001c70: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001c80: 0300 0000 0300 0000 732e 0000 0074 007c  ........s....t.|
+00001c90: 0064 0183 0264 0075 0072 1e7c 006a 0172  .d...d.u.r.|.j.r
+00001ca0: 1e74 017c 017c 0083 027d 0174 0274 037c  .t.|.|...}.t.t.|
+00001cb0: 0083 02a0 047c 01a1 0153 0029 024e 7239  .....|...S.).Nr9
+00001cc0: 0000 0029 0572 3a00 0000 7211 0000 0072  ...).r:...r....r
+00001cd0: 1a00 0000 7245 0000 0072 3200 0000 2902  ....rE...r2...).
+00001ce0: 721d 0000 0072 2700 0000 7220 0000 0072  r....r'...r ...r
+00001cf0: 2200 0000 7223 0000 0072 3200 0000 c500  "...r#...r2.....
+00001d00: 0000 7306 0000 0000 0114 010a 017a 2441  ..s..........z$A
+00001d10: 6972 4d6f 6465 6c53 6572 6961 6c69 7a65  irModelSerialize
+00001d20: 722e 746f 5f72 6570 7265 7365 6e74 6174  r.to_representat
+00001d30: 696f 6e29 0146 2914 7234 0000 0072 3500  ion).F).r4...r5.
+00001d40: 0000 7236 0000 0072 3700 0000 721b 0000  ..r6...r7...r...
+00001d50: 0072 5400 0000 722b 0000 0072 2900 0000  .rT...r+...r)...
+00001d60: 722e 0000 0072 5300 0000 7257 0000 0072  r....rS...rW...r
+00001d70: 6e00 0000 7251 0000 0072 5200 0000 7276  n...rQ...rR...rv
+00001d80: 0000 0072 4f00 0000 7250 0000 0072 8000  ...rO...rP...r..
+00001d90: 0000 7232 0000 0072 4400 0000 7222 0000  ..r2...rD...r"..
+00001da0: 0072 2200 0000 7220 0000 0072 2300 0000  .r"...r ...r#...
+00001db0: 7245 0000 003e 0000 0073 2000 0000 0801  rE...>...s .....
+00001dc0: 0e08 0c15 0c04 0803 0803 0e04 0817 080f  ................
+00001dd0: 0807 0806 0808 0807 0808 080a 0c07 7245  ..............rE
+00001de0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001df0: 0000 0000 0400 0000 0000 0000 7336 0000  ............s6..
+00001e00: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+00001e10: 0284 085a 0364 0887 0066 0164 0464 0584  ...Z.d...f.d.d..
+00001e20: 095a 0487 0066 0164 0664 0784 085a 0587  .Z...f.d.d...Z..
+00001e30: 0004 005a 0653 0029 0972 3d00 0000 6301  ...Z.S.).r=...c.
+00001e40: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001e50: 0000 000f 0000 0073 2e00 0000 7c02 a000  .......s....|...
+00001e60: 6401 6400 a102 7c00 5f01 7402 7403 7c00  d.d...|._.t.t.|.
+00001e70: 8302 6a04 7c01 6900 7c02 a401 8e01 0100  ..j.|.i.|.......
+00001e80: 6400 7c00 5f05 6400 5300 7216 0000 0029  d.|._.d.S.r....)
+00001e90: 0672 1900 0000 7217 0000 0072 1a00 0000  .r....r....r....
+00001ea0: 723d 0000 0072 1b00 0000 7218 0000 0029  r=...r....r....)
+00001eb0: 0372 1d00 0000 721e 0000 00da 0b6c 6973  .r....r......lis
+00001ec0: 745f 6b77 6172 6773 7220 0000 0072 2200  t_kwargsr ...r".
+00001ed0: 0000 7223 0000 0072 1b00 0000 cc00 0000  ..r#...r........
+00001ee0: 7306 0000 0000 010e 0116 017a 1a41 6972  s..........z.Air
+00001ef0: 4c69 7374 5365 7269 616c 697a 6572 2e5f  ListSerializer._
+00001f00: 5f69 6e69 745f 5f46 6302 0000 0000 0000  _init__Fc.......
+00001f10: 0000 0000 0002 0000 0004 0000 0003 0000  ................
+00001f20: 0073 4200 0000 7c00 6a00 6401 7501 722c  .sB...|.j.d.u.r,
+00001f30: 7401 7c00 6a02 6402 6400 8303 6401 7501  t.|.j.d.d...d.u.
+00001f40: 722c 7403 a004 7c00 a101 a005 a100 7c00  r,t...|.......|.
+00001f50: 5f06 7407 7408 7c00 8302 6a09 7c01 6403  _.t.t.|...j.|.d.
+00001f60: 8d01 0100 6400 5300 2904 4e46 7217 0000  ....d.S.).NFr...
+00001f70: 0072 5600 0000 290a 7217 0000 0072 3a00  .rV...).r....r:.
+00001f80: 0000 723f 0000 0072 1000 0000 722c 0000  ..r?...r....r,..
+00001f90: 0072 2d00 0000 7218 0000 0072 1a00 0000  .r-...r....r....
+00001fa0: 723d 0000 0072 2e00 0000 722f 0000 0072  r=...r....r/...r
+00001fb0: 2000 0000 7222 0000 0072 2300 0000 722e   ...r"...r#...r.
+00001fc0: 0000 00d1 0000 0073 0600 0000 0001 1c01  .......s........
+00001fd0: 1001 7a1a 4169 724c 6973 7453 6572 6961  ..z.AirListSeria
+00001fe0: 6c69 7a65 722e 6973 5f76 616c 6964 6303  lizer.is_validc.
+00001ff0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00002000: 0000 0003 0000 0073 1600 0000 7400 7401  .......s....t.t.
+00002010: 7c00 8302 a002 7c01 7c02 a102 0100 6400  |.....|.|.....d.
+00002020: 5300 7231 0000 0029 0372 1a00 0000 723d  S.r1...).r....r=
+00002030: 0000 0072 2900 0000 7226 0000 0072 2000  ...r)...r&...r .
+00002040: 0000 7222 0000 0072 2300 0000 7229 0000  ..r"...r#...r)..
+00002050: 00d6 0000 0073 0200 0000 0001 7a18 4169  .....s......z.Ai
+00002060: 724c 6973 7453 6572 6961 6c69 7a65 722e  rListSerializer.
+00002070: 7570 6461 7465 2901 4629 0772 3400 0000  update).F).r4...
+00002080: 7235 0000 0072 3600 0000 721b 0000 0072  r5...r6...r....r
+00002090: 2e00 0000 7229 0000 0072 4400 0000 7222  ....r)...rD...r"
+000020a0: 0000 0072 2200 0000 7220 0000 0072 2300  ...r"...r ...r#.
+000020b0: 0000 723d 0000 00cb 0000 0073 0600 0000  ..r=.......s....
+000020c0: 0801 0c05 0e05 723d 0000 0063 0000 0000  ......r=...c....
+000020d0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000020e0: 0000 0000 732c 0000 0065 005a 0164 005a  ....s,...e.Z.d.Z
+000020f0: 0287 0066 0164 0164 0284 085a 0364 0364  ...f.d.d...Z.d.d
+00002100: 0484 005a 0464 0564 0684 005a 0587 0004  ...Z.d.d...Z....
+00002110: 005a 0653 0029 07da 1241 6972 456d 7074  .Z.S.)...AirEmpt
+00002120: 7953 6572 6961 6c69 7a65 7263 0100 0000  ySerializerc....
+00002130: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00002140: 0f00 0000 731a 0000 0074 0074 017c 0083  ....s....t.t.|..
+00002150: 026a 027c 0169 007c 02a4 018e 0101 0064  .j.|.i.|.......d
+00002160: 0053 0072 3100 0000 2903 721a 0000 0072  .S.r1...).r....r
+00002170: 8200 0000 721b 0000 0072 1c00 0000 7220  ....r....r....r 
+00002180: 0000 0072 2200 0000 7223 0000 0072 1b00  ...r"...r#...r..
+00002190: 0000 dc00 0000 7302 0000 0000 017a 1b41  ......s......z.A
+000021a0: 6972 456d 7074 7953 6572 6961 6c69 7a65  irEmptySerialize
+000021b0: 722e 5f5f 696e 6974 5f5f 6303 0000 0000  r.__init__c.....
+000021c0: 0000 0000 0000 0003 0000 0001 0000 0043  ...............C
+000021d0: 0000 0073 0a00 0000 7400 8300 8201 6400  ...s....t.....d.
+000021e0: 5300 7231 0000 00a9 01da 0e4e 6f74 496d  S.r1.......NotIm
+000021f0: 706c 656d 656e 7465 6472 2600 0000 7222  plementedr&...r"
+00002200: 0000 0072 2200 0000 7223 0000 0072 2900  ...r"...r#...r).
+00002210: 0000 df00 0000 7302 0000 0000 017a 1941  ......s......z.A
+00002220: 6972 456d 7074 7953 6572 6961 6c69 7a65  irEmptySerialize
+00002230: 722e 7570 6461 7465 6302 0000 0000 0000  r.updatec.......
+00002240: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
+00002250: 0073 0a00 0000 7400 8300 8201 6400 5300  .s....t.....d.S.
+00002260: 7231 0000 0072 8300 0000 722a 0000 0072  r1...r....r*...r
+00002270: 2200 0000 7222 0000 0072 2300 0000 722b  "...r"...r#...r+
+00002280: 0000 00e2 0000 0073 0200 0000 0001 7a19  .......s......z.
+00002290: 4169 7245 6d70 7479 5365 7269 616c 697a  AirEmptySerializ
+000022a0: 6572 2e63 7265 6174 6529 0772 3400 0000  er.create).r4...
+000022b0: 7235 0000 0072 3600 0000 721b 0000 0072  r5...r6...r....r
+000022c0: 2900 0000 722b 0000 0072 4400 0000 7222  )...r+...rD...r"
+000022d0: 0000 0072 2200 0000 7220 0000 0072 2300  ...r"...r ...r#.
+000022e0: 0000 7282 0000 00da 0000 0073 0600 0000  ..r........s....
+000022f0: 0802 0c03 0803 7282 0000 0063 0000 0000  ......r....c....
+00002300: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00002310: 0000 0000 731c 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00002320: 0287 0066 0164 0164 0284 085a 0387 0004  ...f.d.d...Z....
+00002330: 005a 0453 0029 03da 1441 6972 4479 6e61  .Z.S.)...AirDyna
+00002340: 6d69 6353 6572 6961 6c69 7a65 7263 0100  micSerializerc..
+00002350: 0000 0000 0000 0000 0000 0600 0000 0400  ................
+00002360: 0000 0f00 0000 7374 0000 007c 02a0 0064  ......st...|...d
+00002370: 01a1 017d 0374 017c 0383 0174 026b 0273  ...}.t.|...t.k.s
+00002380: 1e74 0364 0283 0182 017c 03a0 04a1 0044  .t.d.....|.....D
+00002390: 005d 325c 027d 047d 057c 057c 006a 056a  .]2\.}.}.|.|.j.j
+000023a0: 057c 043c 007c 047c 006a 056a 057c 0419  .|.<.|.|.j.j.|..
+000023b0: 005f 067c 0467 017c 006a 056a 057c 0419  ._.|.g.|.j.j.|..
+000023c0: 005f 0771 2674 0874 097c 0083 026a 0a7c  ._.q&t.t.|...j.|
+000023d0: 0169 007c 02a4 018e 0101 0064 0053 0029  .i.|.......d.S.)
+000023e0: 034e da06 7661 6c75 6573 7a16 7661 6c75  .N..valuesz.valu
+000023f0: 6573 2073 686f 756c 6420 6265 2064 6963  es should be dic
+00002400: 742e 290b 7219 0000 0072 7500 0000 7274  t.).r....ru...rt
+00002410: 0000 00da 0954 7970 6545 7272 6f72 7260  .....TypeErrorr`
+00002420: 0000 0072 4700 0000 725a 0000 00da 0c73  ...rG...rZ.....s
+00002430: 6f75 7263 655f 6174 7472 7372 1a00 0000  ource_attrsr....
+00002440: 7285 0000 0072 1b00 0000 2906 721d 0000  r....r....).r...
+00002450: 0072 1e00 0000 721f 0000 0072 8600 0000  .r....r....r....
+00002460: 7279 0000 0072 7a00 0000 7220 0000 0072  ry...rz...r ...r
+00002470: 2200 0000 7223 0000 0072 1b00 0000 e700  "...r#...r......
+00002480: 0000 7310 0000 0000 010a 010c 0108 0110  ..s.............
+00002490: 010c 010e 0112 017a 1d41 6972 4479 6e61  .......z.AirDyna
+000024a0: 6d69 6353 6572 6961 6c69 7a65 722e 5f5f  micSerializer.__
+000024b0: 696e 6974 5f5f 2905 7234 0000 0072 3500  init__).r4...r5.
+000024c0: 0000 7236 0000 0072 1b00 0000 7244 0000  ..r6...r....rD..
+000024d0: 0072 2200 0000 7222 0000 0072 2000 0000  .r"...r"...r ...
+000024e0: 7223 0000 0072 8500 0000 e600 0000 7302  r#...r........s.
+000024f0: 0000 0008 0172 8500 0000 6300 0000 0000  .....r....c.....
+00002500: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00002510: 0000 0073 4800 0000 6500 5a01 6400 5a02  ...sH...e.Z.d.Z.
+00002520: 6503 6504 6505 6602 1900 6506 6401 9c02  e.e.e.f...e.d...
+00002530: 8700 6601 6402 6403 840c 5a07 6508 6601  ..f.d.d...Z.e.f.
+00002540: 8700 6601 6404 6405 8409 5a09 8700 6601  ..f.d.d...Z...f.
+00002550: 6406 6407 8408 5a0a 8700 0400 5a0b 5300  d.d...Z.....Z.S.
+00002560: 2908 da16 4169 7244 6174 6163 6c61 7373  )...AirDataclass
+00002570: 5365 7269 616c 697a 6572 2902 7233 0000  Serializer).r3..
+00002580: 00da 0672 6574 7572 6e63 0200 0000 0000  ...returnc......
+00002590: 0000 0000 0000 0600 0000 0500 0000 0300  ................
+000025a0: 0000 7368 0000 0074 0074 017c 0083 02a0  ..sh...t.t.|....
+000025b0: 027c 01a1 017d 027c 006a 036a 047d 037c  .|...}.|.j.j.}.|
+000025c0: 026a 05a0 06a1 0044 005d 407d 0474 077c  .j.....D.]@}.t.|
+000025d0: 027c 0483 0274 086b 0272 227c 006a 0972  .|...t.k.r"|.j.r
+000025e0: 4a74 077c 006a 097c 0464 0083 037d 056e  Jt.|.j.|.d...}.n
+000025f0: 0c74 077c 037c 0464 0083 037d 0574 0a7c  .t.|.|.d...}.t.|
+00002600: 027c 047c 0583 0301 0071 227c 0253 0072  .|.|.....q"|.S.r
+00002610: 3100 0000 290b 721a 0000 0072 8900 0000  1...).r....r....
+00002620: da11 746f 5f69 6e74 6572 6e61 6c5f 7661  ..to_internal_va
+00002630: 6c75 6572 3700 0000 da09 6461 7461 636c  luer7.....datacl
+00002640: 6173 7372 7700 0000 da04 6b65 7973 723a  assrw.....keysr:
+00002650: 0000 0072 0600 0000 7227 0000 0072 3b00  ...r....r'...r;.
+00002660: 0000 2906 721d 0000 0072 3300 0000 7227  ..).r....r3...r'
+00002670: 0000 0072 8c00 0000 7279 0000 0072 7a00  ...r....ry...rz.
+00002680: 0000 7220 0000 0072 2200 0000 7223 0000  ..r ...r"...r#..
+00002690: 0072 8b00 0000 f300 0000 7312 0000 0000  .r........s.....
+000026a0: 0110 0108 010e 010e 0106 0110 020c 010e  ................
+000026b0: 017a 2841 6972 4461 7461 636c 6173 7353  .z(AirDataclassS
+000026c0: 6572 6961 6c69 7a65 722e 746f 5f69 6e74  erializer.to_int
+000026d0: 6572 6e61 6c5f 7661 6c75 6563 0200 0000  ernal_valuec....
+000026e0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000026f0: 0300 0000 7338 0000 007c 006a 0072 2874  ....s8...|.j.r(t
+00002700: 017c 006a 0064 0164 0083 0372 2874 017c  .|.j.d.d...r(t.|
+00002710: 006a 006a 027c 006a 0364 0083 037c 005f  .j.j.|.j.d...|._
+00002720: 0274 0474 057c 0083 02a0 067c 01a1 0153  .t.t.|.....|...S
+00002730: 0029 024e 7227 0000 0029 0772 3900 0000  .).Nr'...).r9...
+00002740: 723a 0000 0072 2700 0000 da06 736f 7572  r:...r'.....sour
+00002750: 6365 721a 0000 0072 8900 0000 da0e 7275  cer....r......ru
+00002760: 6e5f 7661 6c69 6461 7469 6f6e 2902 721d  n_validation).r.
+00002770: 0000 0072 3300 0000 7220 0000 0072 2200  ...r3...r ...r".
+00002780: 0000 7223 0000 0072 8f00 0000 ff00 0000  ..r#...r........
+00002790: 7306 0000 0000 0114 0114 017a 2541 6972  s..........z%Air
+000027a0: 4461 7461 636c 6173 7353 6572 6961 6c69  DataclassSeriali
+000027b0: 7a65 722e 7275 6e5f 7661 6c69 6461 7469  zer.run_validati
+000027c0: 6f6e 6302 0000 0000 0000 0000 0000 0003  onc.............
+000027d0: 0000 0004 0000 0003 0000 0073 4200 0000  ...........sB...
+000027e0: 7c01 6400 7501 7232 7400 7c01 7401 8302  |.d.u.r2t.|.t...
+000027f0: 7232 7c00 6a02 4400 5d18 7d02 7c02 6a03  r2|.j.D.].}.|.j.
+00002800: 7c01 7601 7218 6400 7c01 7c02 6a03 3c00  |.v.r.d.|.|.j.<.
+00002810: 7118 7404 7405 7c00 8302 a006 7c01 a101  q.t.t.|.....|...
+00002820: 5300 7231 0000 0029 0772 6100 0000 7274  S.r1...).ra...rt
+00002830: 0000 00da 105f 7772 6974 6162 6c65 5f66  ....._writable_f
+00002840: 6965 6c64 7372 5a00 0000 721a 0000 0072  ieldsrZ...r....r
+00002850: 8900 0000 7232 0000 0029 0372 1d00 0000  ....r2...).r....
+00002860: 7227 0000 0072 6b00 0000 7220 0000 0072  r'...rk...r ...r
+00002870: 2200 0000 7223 0000 0072 3200 0000 0401  "...r#...r2.....
+00002880: 0000 730c 0000 0000 0108 010a 010a 010a  ..s.............
+00002890: 010c 017a 2841 6972 4461 7461 636c 6173  ...z(AirDataclas
+000028a0: 7353 6572 6961 6c69 7a65 722e 746f 5f72  sSerializer.to_r
+000028b0: 6570 7265 7365 6e74 6174 696f 6e29 0c72  epresentation).r
+000028c0: 3400 0000 7235 0000 0072 3600 0000 7203  4...r5...r6...r.
+000028d0: 0000 00da 0373 7472 7204 0000 0072 1300  .....strr....r..
+000028e0: 0000 728b 0000 0072 0600 0000 728f 0000  ..r....r....r...
+000028f0: 0072 3200 0000 7244 0000 0072 2200 0000  .r2...rD...r"...
+00002900: 7222 0000 0072 2000 0000 7223 0000 0072  r"...r ...r#...r
+00002910: 8900 0000 f200 0000 7306 0000 0008 011c  ........s.......
+00002920: 0c10 0572 8900 0000 4e29 2ada 0674 7970  ...r....N)*..typ
+00002930: 696e 6772 0200 0000 7203 0000 0072 0400  ingr....r....r..
+00002940: 0000 da04 7575 6964 7205 0000 00da 1572  ....uuidr......r
+00002950: 6573 745f 6672 616d 6577 6f72 6b2e 6669  est_framework.fi
+00002960: 656c 6473 7206 0000 00da 1872 6573 745f  eldsr......rest_
+00002970: 6672 616d 6577 6f72 6b2e 7265 6c61 7469  framework.relati
+00002980: 6f6e 7372 0700 0000 5a14 7265 7374 5f66  onsr....Z.rest_f
+00002990: 7261 6d65 776f 726b 2e75 7469 6c73 7208  ramework.utilsr.
+000029a0: 0000 00da 0e72 6573 745f 6672 616d 6577  .....rest_framew
+000029b0: 6f72 6b72 0900 0000 da10 646a 616e 676f  orkr......django
+000029c0: 2e64 622e 6d6f 6465 6c73 720a 0000 005a  .db.modelsr....Z
+000029d0: 2672 6573 745f 6672 616d 6577 6f72 6b5f  &rest_framework_
+000029e0: 6461 7461 636c 6173 7365 732e 7365 7269  dataclasses.seri
+000029f0: 616c 697a 6572 7372 0b00 0000 5a20 7265  alizersr....Z re
+00002a00: 7374 5f66 7261 6d65 776f 726b 5f64 6174  st_framework_dat
+00002a10: 6163 6c61 7373 6573 2e74 7970 6573 720c  aclasses.typesr.
+00002a20: 0000 005a 2061 6972 5f64 7266 5f72 656c  ...Z air_drf_rel
+00002a30: 6174 696f 6e2e 636f 6e74 6578 745f 6275  ation.context_bu
+00002a40: 696c 6465 7272 0d00 0000 5a1d 6169 725f  ilderr....Z.air_
+00002a50: 6472 665f 7265 6c61 7469 6f6e 2e65 7874  drf_relation.ext
+00002a60: 7261 5f6b 7761 7267 7372 0e00 0000 5a17  ra_kwargsr....Z.
+00002a70: 6169 725f 6472 665f 7265 6c61 7469 6f6e  air_drf_relation
+00002a80: 2e66 6965 6c64 7372 0f00 0000 da28 6169  .fieldsr.....(ai
+00002a90: 725f 6472 665f 7265 6c61 7469 6f6e 2e70  r_drf_relation.p
+00002aa0: 7265 6c6f 6164 5f6f 626a 6563 7473 5f6d  reload_objects_m
+00002ab0: 616e 6167 6572 7210 0000 00da 2661 6972  anagerr.....&air
+00002ac0: 5f64 7266 5f72 656c 6174 696f 6e2e 7175  _drf_relation.qu
+00002ad0: 6572 7973 6574 5f6f 7074 696d 697a 6174  eryset_optimizat
+00002ae0: 696f 6e72 1100 0000 5a16 6169 725f 6472  ionr....Z.air_dr
+00002af0: 665f 7265 6c61 7469 6f6e 2e75 7469 6c73  f_relation.utils
+00002b00: 7212 0000 0072 1300 0000 da0a 5365 7269  r....r......Seri
+00002b10: 616c 697a 6572 7215 0000 00da 0f4d 6f64  alizerr......Mod
+00002b20: 656c 5365 7269 616c 697a 6572 7245 0000  elSerializerrE..
+00002b30: 00da 0e4c 6973 7453 6572 6961 6c69 7a65  ...ListSerialize
+00002b40: 7272 3d00 0000 7282 0000 0072 8500 0000  rr=...r....r....
+00002b50: 7289 0000 0072 2200 0000 7222 0000 0072  r....r"...r"...r
+00002b60: 2200 0000 7223 0000 00da 083c 6d6f 6475  "...r#.....<modu
+00002b70: 6c65 3e01 0000 0073 2c00 0000 1401 0c01  le>....s,.......
+00002b80: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+00002b90: 0c01 0c01 0c01 0c01 0c02 0c03 1229 147f  .............)..
+00002ba0: 000e 120f 100c 100c                      ........
```

### Comparing `air_drf_relation-0.5.5/air_drf_relation/__pycache__/utils.cpython-39.pyc` & `air_drf_relation-0.5.6/air_drf_relation/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 26 11:22:17 2022 UTC, .py size: 651 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-00000000: 610d 0d0a 0000 0000 e962 8f62 8b02 0000  a........b.b....
+00000000: 610d 0d0a 0000 0000 27be 3e64 1203 0000  a.......'.>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
-00000030: 6401 6c00 5a00 6402 6403 8400 5a01 6502  d.l.Z.d.d...Z.e.
-00000040: 6503 6404 9c02 6405 6406 8404 5a04 6503  e.d...d.d...Z.e.
-00000050: 6407 9c01 6408 6409 8404 5a05 6506 6507  d...d.d...Z.e.e.
-00000060: 640a 9c02 640b 640c 8404 5a08 6401 5300  d...d.d...Z.d.S.
-00000070: 290d e900 0000 004e 6302 0000 0000 0000  )......Nc.......
-00000080: 0000 0000 0002 0000 0003 0000 0003 0000  ................
-00000090: 0073 3c00 0000 7400 7c00 8301 7401 7402  .s<...t.|...t.t.
-000000a0: 6602 7600 7222 8700 6601 6401 6402 8408  f.v.r"..f.d.d...
-000000b0: 7c00 4400 8301 5300 7400 7c00 8301 7403  |.D...S.t.|...t.
-000000c0: 6b02 7238 7c00 a004 8800 a101 5300 7c00  k.r8|.......S.|.
-000000d0: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-000000e0: 0000 0200 0000 0500 0000 1300 0000 7326  ..............s&
-000000f0: 0000 0067 007c 005d 1e7d 0174 007c 0183  ...g.|.].}.t.|..
-00000100: 0174 016b 0272 1e7c 01a0 0288 00a1 016e  .t.k.r.|.......n
-00000110: 027c 0191 0271 0453 00a9 0029 03da 0474  .|...q.S...)...t
-00000120: 7970 65da 0464 6963 74da 0367 6574 2902  ype..dict..get).
-00000130: da02 2e30 da01 76a9 01da 0770 6b5f 6e61  ...0..v....pk_na
-00000140: 6d65 7202 0000 00fa 4f2f 5573 6572 732f  mer.....O/Users/
-00000150: 6b69 7269 6c6c 6365 6c69 7365 762f 7072  kirillcelisev/pr
-00000160: 6f6a 6563 7473 2f70 7974 686f 6e2f 6169  ojects/python/ai
-00000170: 722d 6472 662d 7265 6c61 7469 6f6e 2f61  r-drf-relation/a
-00000180: 6972 5f64 7266 5f72 656c 6174 696f 6e2f  ir_drf_relation/
-00000190: 7574 696c 732e 7079 da0a 3c6c 6973 7463  utils.py..<listc
-000001a0: 6f6d 703e 0600 0000 f300 0000 007a 2467  omp>.........z$g
-000001b0: 6574 5f70 6b5f 6672 6f6d 5f64 6174 612e  et_pk_from_data.
-000001c0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000001d0: 6d70 3e29 0572 0300 0000 da04 6c69 7374  mp>).r......list
-000001e0: da05 7475 706c 6572 0400 0000 7205 0000  ..tupler....r...
-000001f0: 0029 02da 0464 6174 6172 0900 0000 7202  .)...datar....r.
-00000200: 0000 0072 0800 0000 720a 0000 00da 1067  ...r....r......g
-00000210: 6574 5f70 6b5f 6672 6f6d 5f64 6174 6104  et_pk_from_data.
-00000220: 0000 0073 0600 0000 0001 1001 1201 7210  ...s..........r.
-00000230: 0000 0029 02da 0676 616c 7565 73da 0672  ...)...values..r
-00000240: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-00000250: 0000 0400 0000 0400 0000 4300 0000 731a  ..........C...s.
-00000260: 0000 0069 007d 027c 0044 005d 0c7d 037c  ...i.}.|.D.].}.|
-00000270: 017c 027c 033c 0071 087c 0253 00a9 014e  .|.|.<.q.|.S...N
-00000280: 7202 0000 0029 0472 1100 0000 5a0a 7661  r....).r....Z.va
-00000290: 6c75 655f 6461 7461 da06 7265 7375 6c74  lue_data..result
-000002a0: da02 656c 7202 0000 0072 0200 0000 720a  ..elr....r....r.
-000002b0: 0000 00da 1563 7265 6174 655f 6469 6374  .....create_dict
-000002c0: 5f66 726f 6d5f 6c69 7374 0a00 0000 7308  _from_list....s.
-000002d0: 0000 0000 0104 0108 010a 0172 1600 0000  ...........r....
-000002e0: 2901 7211 0000 0063 0200 0000 0000 0000  ).r....c........
-000002f0: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
-00000300: 7322 0000 007c 01a0 00a1 0044 005d 145c  s"...|.....D.].\
-00000310: 027d 027d 0374 017c 007c 027c 0383 0301  .}.}.t.|.|.|....
-00000320: 0071 087c 0053 0072 1300 0000 2902 da05  .q.|.S.r....)...
-00000330: 6974 656d 73da 0773 6574 6174 7472 2904  items..setattr).
-00000340: da08 696e 7374 616e 6365 7211 0000 00da  ..instancer.....
-00000350: 036b 6579 da05 7661 6c75 6572 0200 0000  .key..valuer....
-00000360: 7202 0000 0072 0a00 0000 da13 7365 745f  r....r......set_
-00000370: 7661 6c75 6573 5f74 6f5f 636c 6173 7311  values_to_class.
-00000380: 0000 0073 0600 0000 0001 1001 0e01 721c  ...s..........r.
-00000390: 0000 0029 0272 1b00 0000 7212 0000 0063  ...).r....r....c
-000003a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000003b0: 0800 0000 4300 0000 732a 0000 007a 1074  ....C...s*...z.t
-000003c0: 00a0 017c 00a1 0101 0057 0064 0153 0004  ...|.....W.d.S..
-000003d0: 0074 0279 2401 0001 0001 0059 0064 0253  .t.y$......Y.d.S
-000003e0: 0030 0064 0053 0029 034e 5446 2903 da04  .0.d.S.).NTF)...
-000003f0: 7575 6964 da04 5555 4944 da0a 5661 6c75  uuid..UUID..Valu
-00000400: 6545 7272 6f72 2901 721b 0000 0072 0200  eError).r....r..
-00000410: 0000 7202 0000 0072 0a00 0000 da07 6973  ..r....r......is
-00000420: 5f75 7569 6417 0000 0073 0a00 0000 0001  _uuid....s......
-00000430: 0201 0a01 0601 0c01 7220 0000 0029 0972  ........r ...).r
-00000440: 1d00 0000 7210 0000 0072 0d00 0000 7204  ....r....r....r.
-00000450: 0000 0072 1600 0000 721c 0000 00da 0373  ...r....r......s
-00000460: 7472 da04 626f 6f6c 7220 0000 0072 0200  tr..boolr ...r..
-00000470: 0000 7202 0000 0072 0200 0000 720a 0000  ..r....r....r...
-00000480: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000490: 0800 0000 0803 0806 1007 0e06            ............
+00000020: 0003 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 6d03 5a03 0100 6403 6404 8400 5a04 6505  m.Z...d.d...Z.e.
+00000050: 6506 6405 9c02 6406 6407 8404 5a07 6408  e.d...d.d...Z.d.
+00000060: 6409 8400 5a08 6401 5300 290a e900 0000  d...Z.d.S.).....
+00000070: 004e 2902 da07 4d61 7070 696e 67da 0853  .N)...Mapping..S
+00000080: 6571 7565 6e63 6563 0200 0000 0000 0000  equencec........
+00000090: 0000 0000 0200 0000 0300 0000 0300 0000  ................
+000000a0: 733c 0000 0074 007c 0083 0174 0174 0266  s<...t.|...t.t.f
+000000b0: 0276 0072 2287 0066 0164 0164 0284 087c  .v.r"..f.d.d...|
+000000c0: 0044 0083 0153 0074 007c 0083 0174 036b  .D...S.t.|...t.k
+000000d0: 0272 387c 00a0 0488 00a1 0153 007c 0053  .r8|.......S.|.S
+000000e0: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
+000000f0: 0002 0000 0005 0000 0013 0000 0073 2600  .............s&.
+00000100: 0000 6700 7c00 5d1e 7d01 7400 7c01 8301  ..g.|.].}.t.|...
+00000110: 7401 6b02 721e 7c01 a002 8800 a101 6e02  t.k.r.|.......n.
+00000120: 7c01 9102 7104 5300 a900 2903 da04 7479  |...q.S...)...ty
+00000130: 7065 da04 6469 6374 da03 6765 7429 02da  pe..dict..get)..
+00000140: 022e 30da 0176 a901 da07 706b 5f6e 616d  ..0..v....pk_nam
+00000150: 6572 0400 0000 fa4f 2f55 7365 7273 2f6b  er.....O/Users/k
+00000160: 6972 696c 6c63 656c 6973 6576 2f70 726f  irillcelisev/pro
+00000170: 6a65 6374 732f 7079 7468 6f6e 2f61 6972  jects/python/air
+00000180: 2d64 7266 2d72 656c 6174 696f 6e2f 6169  -drf-relation/ai
+00000190: 725f 6472 665f 7265 6c61 7469 6f6e 2f75  r_drf_relation/u
+000001a0: 7469 6c73 2e70 79da 0a3c 6c69 7374 636f  tils.py..<listco
+000001b0: 6d70 3e07 0000 00f3 0000 0000 7a24 6765  mp>.........z$ge
+000001c0: 745f 706b 5f66 726f 6d5f 6461 7461 2e3c  t_pk_from_data.<
+000001d0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000001e0: 703e 2905 7205 0000 00da 046c 6973 74da  p>).r......list.
+000001f0: 0574 7570 6c65 7206 0000 0072 0700 0000  .tupler....r....
+00000200: 2902 da04 6461 7461 720b 0000 0072 0400  )...datar....r..
+00000210: 0000 720a 0000 0072 0c00 0000 da10 6765  ..r....r......ge
+00000220: 745f 706b 5f66 726f 6d5f 6461 7461 0500  t_pk_from_data..
+00000230: 0000 7306 0000 0000 0110 0112 0172 1200  ..s..........r..
+00000240: 0000 2902 da06 7661 6c75 6573 da06 7265  ..)...values..re
+00000250: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
+00000260: 0004 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
+00000270: 0000 6900 7d02 7c00 4400 5d0c 7d03 7c01  ..i.}.|.D.].}.|.
+00000280: 7c02 7c03 3c00 7108 7c02 5300 a901 4e72  |.|.<.q.|.S...Nr
+00000290: 0400 0000 2904 7213 0000 005a 0a76 616c  ....).r....Z.val
+000002a0: 7565 5f64 6174 61da 0672 6573 756c 74da  ue_data..result.
+000002b0: 0265 6c72 0400 0000 7204 0000 0072 0c00  .elr....r....r..
+000002c0: 0000 da15 6372 6561 7465 5f64 6963 745f  ....create_dict_
+000002d0: 6672 6f6d 5f6c 6973 740b 0000 0073 0800  from_list....s..
+000002e0: 0000 0001 0401 0801 0a01 7218 0000 0063  ..........r....c
+000002f0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00000300: 0400 0000 4300 0000 7376 0000 0074 007c  ....C...sv...t.|
+00000310: 0074 0183 0272 2a7c 00a0 02a1 0044 005d  .t...r*|.....D.]
+00000320: 147d 0174 037c 007c 0119 0083 017c 007c  .}.t.|.|.....|.|
+00000330: 013c 0071 126e 4874 007c 0074 0483 0272  .<.q.nHt.|.t...r
+00000340: 5e74 007c 0074 0583 0273 5e74 067c 0083  ^t.|.t...s^t.|..
+00000350: 0144 005d 145c 027d 027d 0374 037c 0383  .D.].\.}.}.t.|..
+00000360: 017c 007c 023c 0071 466e 1474 007c 0074  .|.|.<.qFn.t.|.t
+00000370: 076a 0883 0272 7274 057c 0083 0153 007c  .j...rrt.|...S.|
+00000380: 0053 0072 1500 0000 2909 da0a 6973 696e  .S.r....)...isin
+00000390: 7374 616e 6365 7206 0000 00da 046b 6579  stancer......key
+000003a0: 73da 0f73 7472 696e 6769 6679 5f75 7569  s..stringify_uui
+000003b0: 6473 720f 0000 00da 0373 7472 da09 656e  dsr......str..en
+000003c0: 756d 6572 6174 65da 0475 7569 64da 0455  umerate..uuid..U
+000003d0: 5549 4429 04da 0576 616c 7565 da01 6bda  UID)...value..k.
+000003e0: 0169 7209 0000 0072 0400 0000 7204 0000  .ir....r....r...
+000003f0: 0072 0c00 0000 721b 0000 0012 0000 0073  .r....r........s
+00000400: 1200 0000 0001 0a01 0c01 1401 1401 1001  ................
+00000410: 1001 0c01 0801 721b 0000 0029 0972 1e00  ......r....).r..
+00000420: 0000 da0f 636f 6c6c 6563 7469 6f6e 732e  ....collections.
+00000430: 6162 6372 0200 0000 7203 0000 0072 1200  abcr....r....r..
+00000440: 0000 720f 0000 0072 0600 0000 7218 0000  ..r....r....r...
+00000450: 0072 1b00 0000 7204 0000 0072 0400 0000  .r....r....r....
+00000460: 7204 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+00000470: 756c 653e 0100 0000 7308 0000 0008 0110  ule>....s.......
+00000480: 0308 0610 07                             .....
```

### Comparing `air_drf_relation-0.5.5/air_drf_relation/context_builder.py` & `air_drf_relation-0.5.6/air_drf_relation/context_builder.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/decorators.py` & `air_drf_relation-0.5.6/air_drf_relation/decorators.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/extra_kwargs.py` & `air_drf_relation-0.5.6/air_drf_relation/extra_kwargs.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/fields.py` & `air_drf_relation-0.5.6/air_drf_relation/fields.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/filters.py` & `air_drf_relation-0.5.6/air_drf_relation/filters.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/model_fields.py` & `air_drf_relation-0.5.6/air_drf_relation/model_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         kwargs['data_class'] = self.data_class
         return name, path, args, kwargs
 
     def from_db_value(self, value, expression, connection):
         if value is None:
             return value
         obj = json.loads(value)
-        if obj == self._get_default():
-            return obj
+        if obj is None:
+            return None
         return from_dict(data_class=self.data_class, data=obj)
 
     def to_python(self, value):
         if isinstance(value, self.data_class):
             return value
         if value is None:
             return value
```

### Comparing `air_drf_relation-0.5.5/air_drf_relation/preload_objects_manager.py` & `air_drf_relation-0.5.6/air_drf_relation/preload_objects_manager.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/queryset_optimization.py` & `air_drf_relation-0.5.6/air_drf_relation/queryset_optimization.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/air_drf_relation/serializers.py` & `air_drf_relation-0.5.6/air_drf_relation/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from rest_framework_dataclasses.types import Dataclass
 
 from air_drf_relation.context_builder import set_empty_request_in_kwargs
 from air_drf_relation.extra_kwargs import ExtraKwargsFactory
 from air_drf_relation.fields import AirRelatedField
 from air_drf_relation.preload_objects_manager import PreloadObjectsManager
 from air_drf_relation.queryset_optimization import optimize_queryset
+from air_drf_relation.utils import stringify_uuids
 
 T = TypeVar('T', bound=Dataclass)
 
 
 class AirSerializer(serializers.Serializer):
     def __init__(self, *args, **kwargs):
         self._preload_objects_manager = None
@@ -30,27 +31,31 @@
         raise NotImplementedError('`create()` must be implemented.')
 
     def is_valid(self, raise_exception=False):
         if self.preload_objects is not False:
             self._preload_objects_manager = PreloadObjectsManager.get_preload_objects_manager(self).init()
         super(AirSerializer, self).is_valid(raise_exception)
 
+    def to_representation(self, instance):
+        data = super().to_representation(instance)
+        return stringify_uuids(data)
+
     @classmethod
     def many_init(cls, *args, **kwargs):
         class Meta:
             pass
+
         meta = getattr(cls, 'Meta', None)
         if not meta:
             meta = Meta()
             setattr(cls, 'Meta', meta)
         if not hasattr(meta, 'list_serializer_class'):
             setattr(meta, 'list_serializer_class', AirListSerializer)
         serializer = super(AirSerializer, cls).many_init(*args, **kwargs)
 
-
         if hasattr(serializer, 'parent') and serializer.parent is None:
             if serializer.child and \
                     hasattr(serializer.child, 'optimize_queryset') and serializer.child.optimize_queryset:
                 serializer.instance = optimize_queryset(serializer.instance, serializer.child)
         return serializer
 
 
@@ -92,15 +97,15 @@
         return self.update_or_create(None, validated_data)
 
     def update(self, instance, validated_data):
         return self.update_or_create(instance, validated_data)
 
     def is_valid(self, raise_exception=False):
         self._filter_queryset_by_fields()
-        super(AirModelSerializer, self).is_valid(raise_exception=raise_exception)
+        return super(AirModelSerializer, self).is_valid(raise_exception=raise_exception)
 
     def _update_fields(self):
         if not hasattr(self.Meta, 'model'):
             return
         info = model_meta.get_field_info(self.Meta.model)
         hidden_fields = [field_name for field_name, field in self.fields.items() if
                          hasattr(field, 'hidden') and getattr(field, 'hidden', True)]
@@ -188,19 +193,15 @@
                 set_empty_request_in_kwargs(kwargs=kwargs)
             return cls.many_init(*args, **kwargs)
         return super().__new__(cls, *args, **kwargs)
 
     def to_representation(self, instance):
         if getattr(self, 'parent') is None and self.optimize_queryset:
             instance = optimize_queryset(instance, self)
-        data = super(AirModelSerializer, self).to_representation(instance)
-        for el in data:
-            if type(data[el]) == UUID:
-                data[el] = str(data[el])
-        return data
+        return super(AirModelSerializer, self).to_representation(instance)
 
 
 class AirListSerializer(serializers.ListSerializer):
     def __init__(self, *args, **list_kwargs):
         self.preload_objects = list_kwargs.pop('preload_objects', None)
         super(AirListSerializer, self).__init__(*args, **list_kwargs)
         self._preload_objects_manager = None
```

### Comparing `air_drf_relation-0.5.5/air_drf_relation.egg-info/PKG-INFO` & `air_drf_relation-0.5.6/air_drf_relation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air-drf-relation
-Version: 0.5.5
+Version: 0.5.6
 Summary: Improved interaction with DRF relations.
 Home-page: https://github.com/bubaley/air-drf-relation
 Author: bubaley
 Author-email: bubaley.fu@gmail.com
 License: MIT
 Description: **AIR-DRF-RELATION**
```

### Comparing `air_drf_relation-0.5.5/air_drf_relation.egg-info/SOURCES.txt` & `air_drf_relation-0.5.6/air_drf_relation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/device/migrations/0001_initial.py` & `air_drf_relation-0.5.6/device/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/device/serializers.py` & `air_drf_relation-0.5.6/device/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/device/tests.py` & `air_drf_relation-0.5.6/device/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/film/migrations/0001_initial.py` & `air_drf_relation-0.5.6/film/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/film/models.py` & `air_drf_relation-0.5.6/film/models.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/film/serializers.py` & `air_drf_relation-0.5.6/film/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/film/tests.py` & `air_drf_relation-0.5.6/film/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,19 @@
         FilmInformation(description='123', budget=123, rating='123')
         self.film = Film.objects.create(name='demo', release_date=datetime.utcnow().date())
         self.film.actors.set(Actor.objects.all())
 
     def test_to_representation(self):
         result = FilmSerializer(self.film).data
         self.assertEqual(result['information'], None)
-        self.film.information = FilmInformation(1, '1', '1')
+        information = FilmInformation(1, '1', '1')
+        self.film.information = information
+        self.film.save()
+        self.film.information = None
         self.film.save()
-        # self.film.information = {'budget': 1}
-        # self.film.save()
-        # self.film.refresh_from_db()
-        information = FilmSerializer(self.film).data['information']
-        # keys = ['rating', 'description']
-        # values = [getattr(information, v) for v in keys]
-        # self.assertEqual(values, [None], None)
 
     def test_validation(self):
         data = {'name': 'demo', 'release_date': '2021-01-01', 'actors': [], 'information': {}}
         # serializer = FilmSerializer(data=data)
         # self.assertRaises(ValidationError, serializer.is_valid, True)
         data['information'] = {'budget': 1, 'rating': 1, 'description': '1', 'active': False}
         serializer = FilmSerializer(data=data)
```

### Comparing `air_drf_relation-0.5.5/setup.py` & `air_drf_relation-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='air_drf_relation',
-      version='0.5.5',
+      version='0.5.6',
       description='Improved interaction with DRF relations.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       keywords='django rest relation nested pk primary object',
       url='https://github.com/bubaley/air-drf-relation',
       author='bubaley',
       author_email='bubaley.fu@gmail.com',
```

### Comparing `air_drf_relation-0.5.5/table/migrations/0001_initial.py` & `air_drf_relation-0.5.6/table/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/table/migrations/0003_auto_20220513_1542.py` & `air_drf_relation-0.5.6/table/migrations/0003_auto_20220513_1542.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/table/migrations/0004_material_company.py` & `air_drf_relation-0.5.6/table/migrations/0004_material_company.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/table/models.py` & `air_drf_relation-0.5.6/table/models.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/table/serializers.py` & `air_drf_relation-0.5.6/table/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/table/tests.py` & `air_drf_relation-0.5.6/table/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                  'legs': [{'color': get_id(self._colors_count), 'name': '1', 'code': 1} for _ in range(5)]} for v in
                 range(self._table_count)]
         serializer = TableWithLegsSerializer(data=data, many=True)
         serializer.is_valid(raise_exception=True)
         self.assertEqual(len(connection.queries), 2)
 
     @queries_count
-    def test_toogle_preload_objects(self):
+    def test_toggle_preload_objects(self):
         data = [{'name': v, 'material': get_id(self._materials_count), 'color': get_id(self._colors_count),
                  'legs': [{'color': get_id(self._colors_count), 'name': '1', 'code': 1} for _ in range(5)]} for v in
                 range(300)]
         PreloadObjectsManager.disable_search_for_preloaded_objects()
         serializer = TableWithLegsSerializer(data=data, many=True)
         serializer.is_valid(raise_exception=True)
         self.assertGreater(len(connection.queries), 2000)
```

### Comparing `air_drf_relation-0.5.5/task/migrations/0001_initial.py` & `air_drf_relation-0.5.6/task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/task/migrations/0003_tag.py` & `air_drf_relation-0.5.6/task/migrations/0003_tag.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/task/migrations/0004_tag_task.py` & `air_drf_relation-0.5.6/task/migrations/0004_tag_task.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/task/tests.py` & `air_drf_relation-0.5.6/task/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.5/task/views.py` & `air_drf_relation-0.5.6/task/views.py`

 * *Files identical despite different names*

