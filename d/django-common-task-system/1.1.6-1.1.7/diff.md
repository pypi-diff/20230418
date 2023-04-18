# Comparing `tmp/django-common-task-system-1.1.6.tar.gz` & `tmp/django-common-task-system-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.1.6.tar", last modified: Wed Apr 12 09:27:56 2023, max compression
+gzip compressed data, was "django-common-task-system-1.1.7.tar", last modified: Tue Apr 18 02:49:56 2023, max compression
```

## Comparing `django-common-task-system-1.1.6.tar` & `django-common-task-system-1.1.7.tar`

### file list

```diff
@@ -1,82 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.945098 django-common-task-system-1.1.6/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-12 09:27:56.945098 django-common-task-system-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.902086 django-common-task-system-1.1.6/django_common_task_system/
--rw-rw-rw-   0        0        0     2608 2023-04-12 09:03:52.000000 django-common-task-system-1.1.6/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0     6559 2023-04-06 08:09:40.000000 django-common-task-system-1.1.6/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.6/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0      937 2023-03-17 06:16:42.000000 django-common-task-system-1.1.6/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.6/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    12396 2023-03-20 05:05:30.000000 django-common-task-system-1.1.6/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.917091 django-common-task-system-1.1.6/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.6/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.6/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.6/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.6/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0    23088 2023-04-12 05:25:23.000000 django-common-task-system-1.1.6/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     2086 2023-03-22 05:08:57.000000 django-common-task-system-1.1.6/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.889085 django-common-task-system-1.1.6/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.890087 django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.918091 django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.920089 django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.927086 django-common-task-system-1.1.6/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     4826 2023-04-12 09:26:47.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      506 2023-04-11 05:48:06.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     3717 2023-04-11 02:36:41.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.929087 django-common-task-system-1.1.6/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10626 2023-04-07 08:41:18.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    14418 2023-04-11 06:26:02.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1073 2023-04-07 05:56:05.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      800 2023-04-07 05:29:32.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     7503 2023-04-11 06:26:41.000000 django-common-task-system-1.1.6/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.930090 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-04-12 09:15:38.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.932086 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     2970 2023-04-12 09:22:30.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.936087 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      851 2023-04-04 06:16:44.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     2412 2023-04-11 05:50:53.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      834 2023-04-11 05:50:53.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.891086 django-common-task-system-1.1.6/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.940085 django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.6/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      951 2023-04-06 03:57:39.000000 django-common-task-system-1.1.6/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.943089 django-common-task-system-1.1.6/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.6/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.6/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.6/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.6/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.6/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0     6535 2023-04-06 08:05:42.000000 django-common-task-system-1.1.6/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.914087 django-common-task-system-1.1.6/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-12 09:27:56.000000 django-common-task-system-1.1.6/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3411 2023-04-12 09:27:56.000000 django-common-task-system-1.1.6/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:27:56.000000 django-common-task-system-1.1.6/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-12 09:27:56.000000 django-common-task-system-1.1.6/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-12 09:27:56.000000 django-common-task-system-1.1.6/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 09:27:56.945098 django-common-task-system-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-12 09:27:39.000000 django-common-task-system-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.944089 django-common-task-system-1.1.6/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.154166 django-common-task-system-1.1.7/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-18 02:49:56.154166 django-common-task-system-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.111414 django-common-task-system-1.1.7/django_common_task_system/
+-rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.1.7/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0     9800 2023-04-17 08:40:58.000000 django-common-task-system-1.1.7/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.7/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.1.7/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.7/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.1.7/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.121696 django-common-task-system-1.1.7/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0    34023 2023-04-18 02:49:48.000000 django-common-task-system-1.1.7/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.1.7/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.1.7/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.097000 django-common-task-system-1.1.7/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.097000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.122697 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.124696 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.133166 django-common-task-system-1.1.7/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     4987 2023-04-17 08:40:58.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4122 2023-04-13 09:07:07.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.138166 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    17147 2023-04-18 02:49:48.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.139169 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-04-12 09:15:38.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.140166 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     3409 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.143166 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.100000 django-common-task-system-1.1.7/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.100000 django-common-task-system-1.1.7/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.144166 django-common-task-system-1.1.7/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     6709 2023-04-14 09:00:33.000000 django-common-task-system-1.1.7/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.148166 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.7/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.1.7/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.152166 django-common-task-system-1.1.7/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.7/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.7/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.7/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.7/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.7/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    10457 2023-04-18 02:48:30.000000 django-common-task-system-1.1.7/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.116690 django-common-task-system-1.1.7/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4218 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:49:56.154166 django-common-task-system-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-17 01:39:35.000000 django-common-task-system-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.153165 django-common-task-system-1.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.7/tests/__init__.py
```

### Comparing `django-common-task-system-1.1.6/LICENSE` & `django-common-task-system-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/__init__.py` & `django-common-task-system-1.1.7/django_common_task_system/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.apps import apps as django_apps
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.core.management.commands import runserver
+from django.utils.module_loading import import_string
 
 
 class Command(runserver.Command):
 
     def run(self, **options):
         import os
         os.environ['DJANGO_SERVER_ADDRESS'] = "%(protocol)s://%(addr)s:%(port)s" % {
@@ -24,14 +25,17 @@
 
 if not hasattr(settings, 'TASK_SCHEDULE_MODEL'):
     setattr(settings, 'TASK_SCHEDULE_MODEL', 'django_common_task_system.TaskSchedule')
 
 if not hasattr(settings, 'TASK_SCHEDULE_LOG_MODEL'):
     setattr(settings, 'TASK_SCHEDULE_LOG_MODEL', 'django_common_task_system.TaskScheduleLog')
 
+if not hasattr(settings, 'TASK_SCHEDULE_SERIALIZER'):
+    setattr(settings, 'TASK_SCHEDULE_SERIALIZER', 'django_common_task_system.serializers.TaskScheduleSerializer')
+
 
 def get_task_model():
     """
     Return the User model that is active in this project.
     """
     try:
         return django_apps.get_model(settings.TASK_MODEL, require_ready=False)
@@ -74,7 +78,14 @@
             "TASK_SCHEDULE_LOG_MODEL must be of the form 'app_label.model_name'"
         )
     except LookupError:
         raise ImproperlyConfigured(
             "TASK_SCHEDULE_LOG_MODEL refers to model '%s' that has not been installed"
             % settings.SCHEDULE_LOG_MODEL
         )
+
+
+def get_task_schedule_serializer():
+    """
+    Return the User model that is active in this project.
+    """
+    return import_string(settings.TASK_SCHEDULE_SERIALIZER)
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/fields.py` & `django-common-task-system-1.1.7/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/forms.py` & `django-common-task-system-1.1.7/django_common_task_system/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from django import forms
 from django.contrib.admin import widgets
-from .choices import TaskScheduleType, ScheduleTimingType
+from django.utils.module_loading import import_string
+
+from .choices import TaskScheduleType, ScheduleTimingType, TaskScheduleStatus, TaskStatus
 from django_common_objects.widgets import JSONWidget
 from .utils import foreign_key
 from datetime import datetime, time as datetime_time
 from . import models
 
 
 class TaskForm(forms.ModelForm):
@@ -323,7 +325,88 @@
             start_time=cleaned_data.get('schedule_start_time', None)
         )
         return cleaned_data
 
     class Meta:
         model = models.TaskSchedule
         fields = "__all__"
+
+
+class TaskScheduleQueueForm(forms.ModelForm):
+
+    def clean(self):
+        cleaned_data = super(TaskScheduleQueueForm, self).clean()
+        if not self.errors:
+            module = cleaned_data.get('module')
+            config = cleaned_data.get('config')
+            config.setdefault('name', 'SYSTEM_TASK_QUEUE:%s' % cleaned_data['code'])
+            queueCls = import_string(module)
+            validate_config = getattr(queueCls, 'validate_config', None)
+            if validate_config:
+                error = validate_config(config)
+                if error:
+                    self.add_error('config', error)
+            if not self.errors:
+                queue = queueCls(**config)
+                validate = getattr(queue, 'validate', None)
+                if validate:
+                    error = validate()
+                    if error:
+                        self.add_error('config', error)
+        return cleaned_data
+
+    class Meta:
+        model = models.TaskScheduleQueue
+        fields = '__all__'
+
+
+class TaskScheduleProducerForm(forms.ModelForm):
+    name = forms.CharField(max_length=100, label='名称', required=False)
+
+    def __init__(self, *args, **kwargs):
+        super(TaskScheduleProducerForm, self).__init__(*args, **kwargs)
+        if not self.instance.id:
+            self. initial['filters'] = {
+                'status': TaskScheduleStatus.OPENING.value,
+                'task__status': TaskStatus.ENABLE.value,
+            }
+
+    def clean(self):
+        cleaned_data = super(TaskScheduleProducerForm, self).clean()
+        if not self.errors:
+            filters = cleaned_data.get('filters')
+            if not filters:
+                self.add_error('filters', 'filters不能为空')
+            else:
+                try:
+                    models.TaskSchedule.objects.filter(**filters).first()
+                except Exception as e:
+                    self.add_error('filters', 'filters参数错误: %s' % e)
+                else:
+                    name = cleaned_data.get('name')
+                    if not name:
+                        cleaned_data['name'] = "队列(%s)生产者" % cleaned_data.get('queue').name
+        return cleaned_data
+
+    class Meta:
+        model = models.TaskScheduleProducer
+        fields = '__all__'
+
+
+class ConsumerPermissionForm(forms.ModelForm):
+    config = forms.JSONField(required=False, initial={}, label="配置",
+                             widget=forms.HiddenInput())
+    ip_whitelist = forms.CharField(required=False, label="IP白名单", widget=forms.Textarea(
+        attrs={'rows': 10, 'style': 'width: 60%'}))
+
+    def __init__(self, *args, **kwargs):
+        super(ConsumerPermissionForm, self).__init__(*args, **kwargs)
+        if self.instance.id:
+            self.initial['ip_whitelist'] = '\n'.join(self.instance.config.get('ip_whitelist', []) or [])
+
+    def clean(self):
+        cleaned_data = super(ConsumerPermissionForm, self).clean()
+        if not self.errors:
+            ip_whitelist = cleaned_data.pop('ip_whitelist', "")
+            cleaned_data['config'] = {'ip_whitelist': [x.strip() for x in ip_whitelist.split('\n')]}
+        return cleaned_data
+
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.1.7/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.1.7/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/serializers.py` & `django-common-task-system-1.1.7/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,46 +69,30 @@
     pass
 
 
 class SystemScheduleAdmin(base_admin.TaskScheduleAdmin):
 
     task_model = models.SystemTask
     schedule_log_model = models.SystemScheduleLog
-    schedule_put_name = 'system_schedule_queue_put'
+    queues = models.builtins.queues
+    schedule_put_name = 'system_schedule_put'
     list_display = ('id', 'admin_task', 'schedule_type', 'schedule_sub_type', 'next_schedule_time',
                     'status', 'put', 'logs', 'update_time')
     list_filter = ('task__category', )
 
     def has_delete_permission(self, request, obj=None):
         if obj:
             return obj.task.category != models.builtins.tasks.system_default_category
         return True
 
 
 class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
     schedule_retry_name = 'system_schedule_retry'
 
 
-class SystemScheduleQueueAdmin(admin.ModelAdmin):
-    list_display = ('id', 'name', 'code', 'queue_url', 'module', 'update_time')
-
-    fields = (
-        ('code', 'module', 'status'),
-        'name',
-    )
-
-    def queue_url(self, obj):
-        url = reverse('system_schedule_queue_get', args=(obj.code,))
-        return format_html(
-            '<a href="%s" target="_blank">%s</a>' % (url, url)
-        )
-    queue_url.allow_tags = True
-    queue_url.short_description = '队列地址'
-
-
 class SystemProcessAdmin(admin.ModelAdmin):
     list_display = ('process_id', 'process_name', 'log_file', 'status', 'stop_process', 'show_log', 'update_time')
     form = forms.SystemProcessForm
     fields = (
         'system_path',
         'process_name',
         'env',
@@ -133,14 +117,32 @@
         )
     show_log.short_description = '日志'
 
     def has_delete_permission(self, request, obj=None):
         return False
 
 
+class SystemScheduleQueueAdmin(base_admin.TaskScheduleQueueAdmin):
+    form = forms.SystemScheduleQueueForm
+    builtins = models.builtins
+    schedule_get_name = 'system_schedule_get'
+
+
+class SystemScheduleProducerAdmin(base_admin.TaskScheduleProducerAdmin):
+    form = forms.SystemScheduleProducerForm
+    schedule_get_name = 'system_schedule_get'
+    builtins = models.builtins
+
+
+class ConsumerPermissionAdmin(base_admin.ConsumerPermissionAdmin):
+    pass
+
+
 admin.site.register(models.SystemTask, SystemTaskAdmin)
 admin.site.register(models.SystemScheduleCallback, SystemScheduleCallbackAdmin)
 admin.site.register(models.SystemSchedule, SystemScheduleAdmin)
 admin.site.register(models.SystemScheduleLog, SystemScheduleLogAdmin)
 admin.site.register(models.SystemScheduleQueue, SystemScheduleQueueAdmin)
+admin.site.register(models.SystemScheduleProducer, SystemScheduleProducerAdmin)
 admin.site.register(models.SystemProcess, SystemProcessAdmin)
+admin.site.register(models.SystemConsumerPermission, ConsumerPermissionAdmin)
```

#### html2text {}

```diff
@@ -21,36 +21,39 @@
 'admin_status', 'schedules', 'update_time') fields = ( ("parent", 'category',),
 ('queue',), ("name", "status",), "config", 'description', ) filter_horizontal =
 [] list_filter = ('category', 'parent') def has_delete_permission(self,
 request, obj=None): if obj: return obj.category !=
 models.builtins.tasks.system_default_category return True class
 SystemScheduleCallbackAdmin(base_admin.TaskScheduleCallbackAdmin): pass class
 SystemScheduleAdmin(base_admin.TaskScheduleAdmin): task_model =
-models.SystemTask schedule_log_model = models.SystemScheduleLog
-schedule_put_name = 'system_schedule_queue_put' list_display = ('id',
-'admin_task', 'schedule_type', 'schedule_sub_type', 'next_schedule_time',
-'status', 'put', 'logs', 'update_time') list_filter = ('task__category', ) def
-has_delete_permission(self, request, obj=None): if obj: return
-obj.task.category != models.builtins.tasks.system_default_category return True
-class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
-schedule_retry_name = 'system_schedule_retry' class SystemScheduleQueueAdmin
-(admin.ModelAdmin): list_display = ('id', 'name', 'code', 'queue_url',
-'module', 'update_time') fields = ( ('code', 'module', 'status'), 'name', ) def
-queue_url(self, obj): url = reverse('system_schedule_queue_get', args=
-(obj.code,)) return format_html( '%s' % (url, url) ) queue_url.allow_tags =
-True queue_url.short_description = 'éåå°å' class SystemProcessAdmin
+models.SystemTask schedule_log_model = models.SystemScheduleLog queues =
+models.builtins.queues schedule_put_name = 'system_schedule_put' list_display =
+('id', 'admin_task', 'schedule_type', 'schedule_sub_type',
+'next_schedule_time', 'status', 'put', 'logs', 'update_time') list_filter =
+('task__category', ) def has_delete_permission(self, request, obj=None): if
+obj: return obj.task.category != models.builtins.tasks.system_default_category
+return True class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
+schedule_retry_name = 'system_schedule_retry' class SystemProcessAdmin
 (admin.ModelAdmin): list_display = ('process_id', 'process_name', 'log_file',
 'status', 'stop_process', 'show_log', 'update_time') form =
 forms.SystemProcessForm fields = ( 'system_path', 'process_name', 'env',
 'log_file', 'process_id', 'create_time', ) readonly_fields = ('create_time',
 'update_time') def stop_process(self, obj): url = reverse
 ('system_process_stop', args=(obj.process_id,)) return format_html( 'åæ­¢' %
 url ) stop_process.short_description = 'åæ­¢è¿è¡' def show_log(self, obj):
 url = reverse('system_process_log', args=(obj.process_id,)) return format_html
 ( 'æ¥çæ¥å¿' % url ) show_log.short_description = 'æ¥å¿' def
-has_delete_permission(self, request, obj=None): return False
+has_delete_permission(self, request, obj=None): return False class
+SystemScheduleQueueAdmin(base_admin.TaskScheduleQueueAdmin): form =
+forms.SystemScheduleQueueForm builtins = models.builtins schedule_get_name =
+'system_schedule_get' class SystemScheduleProducerAdmin
+(base_admin.TaskScheduleProducerAdmin): form = forms.SystemScheduleProducerForm
+schedule_get_name = 'system_schedule_get' builtins = models.builtins class
+ConsumerPermissionAdmin(base_admin.ConsumerPermissionAdmin): pass
 admin.site.register(models.SystemTask, SystemTaskAdmin) admin.site.register
 (models.SystemScheduleCallback, SystemScheduleCallbackAdmin)
 admin.site.register(models.SystemSchedule, SystemScheduleAdmin)
 admin.site.register(models.SystemScheduleLog, SystemScheduleLogAdmin)
 admin.site.register(models.SystemScheduleQueue, SystemScheduleQueueAdmin)
+admin.site.register(models.SystemScheduleProducer, SystemScheduleProducerAdmin)
 admin.site.register(models.SystemProcess, SystemProcessAdmin)
+admin.site.register(models.SystemConsumerPermission, ConsumerPermissionAdmin)
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from . import models
 from django import forms
 import os
 import time
 from .process import ProcessManager
 from ..system_task_execution.main import start_by_server
+from django_common_task_system.forms import TaskScheduleProducerForm, TaskScheduleQueueForm
 
 
 class SystemTaskForm(forms.ModelForm):
     queue = forms.ModelChoiceField(
         queryset=models.SystemScheduleQueue.objects.all(),
         required=False,
         label='队列',
@@ -86,7 +87,19 @@
             cleaned_data['process_id'] = p.pid
             cleaned_data['status'] = p.is_alive()
         return cleaned_data
 
     class Meta:
         model = models.SystemProcess
         fields = '__all__'
+
+
+class SystemScheduleQueueForm(TaskScheduleQueueForm):
+
+    class Meta(TaskScheduleQueueForm.Meta):
+        model = models.SystemScheduleQueue
+
+
+class SystemScheduleProducerForm(TaskScheduleProducerForm):
+
+    class Meta(TaskScheduleProducerForm.Meta):
+        model = models.SystemScheduleProducer
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             },
         ),
         migrations.CreateModel(
             name='SystemScheduleQueue',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=100, unique=True, verbose_name='队列名称')),
-                ('code', models.CharField(max_length=100, unique=True, validators=[django_common_task_system.system_task.models.code_validator], verbose_name='队列编码')),
+                ('code', models.CharField(max_length=100, unique=True, validators=[django_common_task_system.models.code_validator], verbose_name='队列编码')),
                 ('status', models.BooleanField(default=True, verbose_name='状态')),
                 ('module', models.CharField(choices=[('queue.Queue', '普通队列'), ('queue.LifoQueue', '后进先出队列'), ('queue.PriorityQueue', '优先级队列'), ('_queue.SimpleQueue', '简单队列')], default='queue.Queue', max_length=100, verbose_name='队列类型')),
                 ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
             ],
             options={
                 'verbose_name': '系统队列',
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task/models.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from django.db import models
 from django.conf import settings
-from django.utils.module_loading import import_string
-
+from django_common_task_system.choices import ScheduleQueueModule, TaskScheduleStatus, ConsumerPermissionType
 from django_common_task_system.models import AbstractTask, AbstractTaskSchedule, AbstractTaskScheduleLog, \
-    TaskScheduleLog, AbstractScheduleCallback
-from .choices import ScheduleQueueModule
+    TaskScheduleLog, AbstractScheduleCallback, \
+    AbstractTaskScheduleProducer, AbstractTaskScheduleQueue, AbstractConsumerPermission, \
+    BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, system_initialize_signal
 from django_common_objects.models import CommonCategory
 from django.contrib.auth import get_user_model
+import os
 
 User = get_user_model()
 
 
-def code_validator(value):
-    import re
-    from django.core.validators import ValidationError
-    if re.match(r'[a-zA-Z_-]+', value) is None:
-        raise ValidationError('编码只能包含字母、数字、下划线和中划线')
-
-
 class SystemTask(AbstractTask):
 
     class Meta(AbstractTask.Meta):
         abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
         db_table = 'system_task'
         verbose_name = verbose_name_plural = '系统任务'
 
@@ -29,33 +23,21 @@
         self, force_insert=False, force_update=False, using=None, update_fields=None
     ):
         if self.category_id is None:
             self.category = builtins.tasks.system_default_category
         super().save(force_insert, force_update, using, update_fields)
 
 
-class SystemScheduleQueue(models.Model):
-    id = models.AutoField(primary_key=True, verbose_name='ID')
-    name = models.CharField(max_length=100, verbose_name='队列名称', unique=True)
-    code = models.CharField(max_length=100, verbose_name='队列编码', unique=True, validators=[code_validator])
-    status = models.BooleanField(default=True, verbose_name='状态')
-    module = models.CharField(max_length=100, verbose_name='队列类型',
-                              default=ScheduleQueueModule.QUEUE,
-                              choices=ScheduleQueueModule.choices)
-    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+class SystemScheduleQueue(AbstractTaskScheduleQueue):
 
-    class Meta:
+    class Meta(AbstractTaskScheduleQueue.Meta):
         db_table = 'system_schedule_queue'
         verbose_name = verbose_name_plural = '系统队列'
         abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
 
-    def __str__(self):
-        return "%s(%s)" % (self.name, self.code)
-
 
 class SystemScheduleCallback(AbstractScheduleCallback):
     queue = models.ForeignKey(SystemScheduleQueue, db_constraint=False, related_name='callbacks',
                               on_delete=models.CASCADE, verbose_name='队列')
 
     class Meta(AbstractScheduleCallback.Meta):
         db_table = 'system_schedule_callback'
@@ -72,25 +54,44 @@
     class Meta(AbstractTaskSchedule.Meta):
         db_table = 'system_schedule'
         verbose_name = verbose_name_plural = '系统计划'
         ordering = ('-update_time',)
         abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
 
 
+class SystemScheduleProducer(AbstractTaskScheduleProducer):
+    queue = models.ForeignKey(SystemScheduleQueue, db_constraint=False, related_name='producers',
+                              on_delete=models.CASCADE, verbose_name='队列')
+
+    class Meta(AbstractTaskScheduleProducer.Meta):
+        db_table = 'system_schedule_producer'
+        verbose_name = verbose_name_plural = '计划生产'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
 class SystemScheduleLog(AbstractTaskScheduleLog):
     schedule = models.ForeignKey(SystemSchedule, db_constraint=False, related_name='logs',
                                  on_delete=models.CASCADE, verbose_name='任务计划')
 
     class Meta(AbstractTaskScheduleLog.Meta):
         db_table = 'system_schedule_log'
         verbose_name = verbose_name_plural = '系统日志'
         ordering = ('-schedule_time',)
         abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
 
 
+class SystemConsumerPermission(AbstractConsumerPermission):
+    producer = models.ForeignKey(SystemScheduleProducer, db_constraint=False,
+                                 on_delete=models.CASCADE, verbose_name='生产者')
+
+    class Meta(AbstractConsumerPermission.Meta):
+        db_table = 'system_consumer_permission'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
 class SystemProcess(models.Model):
     id = models.AutoField(primary_key=True, verbose_name='ID')
     process_id = models.PositiveIntegerField(verbose_name='进程ID', unique=True)
     process_name = models.CharField(max_length=100, verbose_name='进程名称')
     env = models.CharField(max_length=500, verbose_name='环境变量', blank=True, null=True)
     status = models.BooleanField(default=True, verbose_name='状态')
     log_file = models.CharField(max_length=200, verbose_name='日志文件')
@@ -101,27 +102,65 @@
         db_table = 'system_process'
         verbose_name = verbose_name_plural = '系统进程'
 
     def __str__(self):
         return "%s(%s)" % (self.process_name, self.process_id)
 
 
-class BuiltinQueues(dict):
+class BuiltinQueues(BaseBuiltinQueues):
+    model = SystemScheduleQueue
 
     def __init__(self):
+        self.opening: SystemScheduleQueue = self.model.objects.get_or_create(
+            code=self.status_params_mapping[TaskScheduleStatus.OPENING.value],
+            defaults={
+                'status': True,
+                'module': ScheduleQueueModule.QUEUE.value,
+                'name': '系统任务队列'
+            }
+        )[0]
+
+        self.test = self.model.objects.get_or_create(
+            code=self.status_params_mapping[TaskScheduleStatus.TEST.value],
+            defaults={
+                'status': True,
+                'module': ScheduleQueueModule.QUEUE.value,
+                'name': '测试任务队列'
+            }
+        )[0]
         super(BuiltinQueues, self).__init__()
-        self.system_task_instance: SystemScheduleQueue = SystemScheduleQueue.objects.get_or_create(
-            code='system', defaults={'name': '系统任务队列'})[0]
-        self.system_test_instance: SystemScheduleQueue = SystemScheduleQueue.objects.get_or_create(
-            code='test', defaults={'name': '测试测试队列'})[0]
-        for q in SystemScheduleQueue.objects.filter(status=True):
-            self[q.code] = import_string(q.module)()
 
-        self.system_task_queue = self[self.system_task_instance.code]
-        self.system_test_queue = self[self.system_test_instance.code]
+
+class BuiltinProducers(BaseBuiltinProducers):
+    model = SystemScheduleProducer
+
+    def __init__(self, queues: BuiltinQueues):
+        self.opening = SystemScheduleProducer.objects.get_or_create(
+            queue=queues.opening,
+            lte_now=True,
+            defaults={
+                'filters': {
+                    'status': TaskScheduleStatus.OPENING.value,
+                },
+                'status': True,
+                'name': '默认'
+            }
+        )[0]
+        self.test = SystemScheduleProducer.objects.get_or_create(
+            queue=queues.test,
+            lte_now=True,
+            defaults={
+                'filters': {
+                    'status': TaskScheduleStatus.TEST.value,
+                },
+                'status': True,
+                'name': '测试'
+            }
+        )[0]
+        super(BuiltinProducers, self).__init__()
 
 
 class BuiltinTasks:
 
     def __init__(self, user, queues: BuiltinQueues):
         self.system_default_category = CommonCategory.objects.get_or_create(
             name='系统任务',
@@ -240,15 +279,15 @@
 
         self.test_sql_produce = SystemTask.objects.get_or_create(
             name='测试SQL生产任务',
             parent=self.sql_produce_parent_task,
             category=self.system_test_category,
             config={
                 'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table,
-                'queue': queues.system_test_instance.code
+                'queue': queues.test.code
             },
             user=user
         )[0]
         self.test_shell_execution = SystemTask.objects.get_or_create(
             name='测试Shell执行任务',
             parent=self.shell_execution_parent_task,
             category=self.system_test_category,
@@ -340,45 +379,70 @@
         }
 
         self.test_sql_execution = SystemSchedule.objects.get_or_create(
             task=tasks.test_sql_execution,
             user=user,
             defaults=defaults
         )[0]
-
         self.test_sql_produce = SystemSchedule.objects.get_or_create(
             task=tasks.test_sql_produce,
             user=user,
             defaults=defaults
         )[0]
         self.test_shell_execution = SystemSchedule.objects.get_or_create(
             task=tasks.test_shell_execution,
             user=user,
             defaults=defaults
         )[0]
 
 
+class BuiltinConsumerPermissions(BaseConsumerPermissions):
+    model = SystemConsumerPermission
+
+    def __init__(self, producers: BuiltinProducers):
+        self.system_consumer_permission = self.model.objects.get_or_create(
+            producer=producers.opening,
+            type=ConsumerPermissionType.IP_WHITE_LIST.value,
+            defaults={
+                'status': True,
+                'config': {
+                    'ip_whitelist': ['127.0.0.1'],
+                }
+            }
+        )[0]
+        super(BuiltinConsumerPermissions, self).__init__()
+
+
 class Builtins:
 
     def __init__(self):
         self._initialized = False
         self._tasks = None
         self._schedules = None
         self._queues = None
+        self._producers = None
+        self._consumer_permissions = None
 
     def initialize(self):
         if not self._initialized:
-            print('初始化内置任务')
-            self._initialized = True
-            user = User.objects.filter(is_superuser=True).order_by('id').first()
-            if not user:
-                raise Exception('未找到超级管理员')
-            self._queues = BuiltinQueues()
-            self._tasks = BuiltinTasks(user, self.queues)
-            self._schedules = BuiltinSchedules(user, self.tasks)
+            if os.environ.get('RUN_MAIN') == 'true':# and os.environ.get('RUN_CLIENT') != 'true':
+                self._initialized = True
+                from django.conf import settings
+                if 'django_common_task_system.system_task' in settings.INSTALLED_APPS:
+                    print('初始化系统内置任务')
+                    user = User.objects.filter(is_superuser=True).order_by('id').first()
+                    if not user:
+                        raise Exception('未找到超级管理员')
+                    self._queues = BuiltinQueues()
+                    self._producers = BuiltinProducers(self._queues)
+                    self._tasks = BuiltinTasks(user, self._queues)
+                    self._schedules = BuiltinSchedules(user, self._tasks)
+                    self._consumer_permissions = BuiltinConsumerPermissions(self._producers)
+                    system_initialize_signal.send(sender='builtin_initialized',
+                                                    app='django_common_task_system.system_task')
 
     @property
     def tasks(self) -> BuiltinTasks:
         self.initialize()
         return self._tasks
 
     @property
@@ -387,9 +451,19 @@
         return self._schedules
 
     @property
     def queues(self) -> BuiltinQueues:
         self.initialize()
         return self._queues
 
+    @property
+    def producers(self) -> BuiltinProducers:
+        self.initialize()
+        return self._producers
+
+    @property
+    def consumer_permissions(self) -> BuiltinConsumerPermissions:
+        self.initialize()
+        return self._consumer_permissions
+
 
 builtins = Builtins()
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task/process.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from multiprocessing import Process
+from multiprocessing import Process, set_start_method
 
 
 class _ProcessManager:
 
     def __init__(self):
         self._processes = {}
 
@@ -11,14 +11,15 @@
         return [x for x in self._processes.values() if x.is_alive()]
 
     @property
     def all_process_ids(self):
         return [k for k, v in self._processes.items() if v.is_alive()]
 
     def create(self, target, *args, **kwargs) -> Process:
+        set_start_method('spawn', True)
         process = Process(target=target, args=args, kwargs=kwargs, daemon=True)
         process.start()
         self._processes[process.pid] = process
         return process
 
     def kill(self, pid):
         if pid in self._processes:
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task/urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.urls import path
 from . import views
 
 
 urlpatterns = [
     path('schedule/produce/<int:pk>/', views.ScheduleProduceView.as_view(), name='system_schedule_produce'),
-    path('schedule/queue/<slug:code>/get/', views.SystemScheduleQueueAPI.get, name='system_schedule_queue_get'),
-    path('schedule/queue/<int:pk>/put/', views.SystemScheduleQueueAPI.put, name='system_schedule_queue_put'),
-    path('schedule/retry/<int:pk>/', views.SystemScheduleQueueAPI.retry, name='system_schedule_retry'),
-    path('schedule/queue/', views.SystemScheduleQueueAPI.status),
+    path('schedule/queue/<slug:code>/get/', views.SystemScheduleQueueAPI.get, name='system_schedule_get'),
+    path('schedule/put/', views.SystemScheduleQueueAPI.put, name='system_schedule_put'),
+    path('schedule/retry/', views.SystemScheduleQueueAPI.retry, name='system_schedule_retry'),
+    path('schedule/queue/status/', views.SystemScheduleQueueAPI.status),
     path('process/logs/<int:process_id>/', views.SystemProcessView.show_logs, name='system_process_log'),
     path('process/stop/<int:process_id>/', views.SystemProcessView.stop_process, name='system_process_stop'),
 ]
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,43 +24,56 @@
         system_task_queue.put(copy.deepcopy(schedule))
         schedule.generate_next_schedule()
     return queryset
 
 
 def request_system_schedule():
 
-    url = urljoin(settings.HOST, reverse('system_schedule_queue_get', args=('system', )))
+    url = urljoin(settings.HOST, reverse('system_schedule_get', args=('opening', )))
     response = requests.get(url)
     if response.status_code == 200:
         result = response.json()
         callback = result.pop('callback')
         if callback:
             callback = TaskScheduleCallback(**callback)
         task = result.pop('task')
         category = task.pop('category')
         tags = task.pop('tags', None)
         user = result.pop('user', None)
+        queue = result.pop('queue', None)
+        parent = task.pop('parent', None)
+        if parent:
+            parent.pop('category')
+            parent.pop('tags')
+            parent = SystemTask(**parent)
         result['next_schedule_time'] = datetime.strptime(result.pop('schedule_time'), '%Y-%m-%d %H:%M:%S')
         schedule = SystemSchedule(
-            task=SystemTask(**task),
+            task=SystemTask(parent=parent, **task),
             callback=callback,
             **result
         )
-        system_task_queue.put(schedule)
+        schedule.queue = queue
+        return schedule
+        # system_task_queue.put(schedule)
 
 
 def get_system_schedule():
-    try:
-        return system_task_queue.get(timeout=2)
-    except Empty:
-        logger.debug('\r[%s]%s' % (time.strftime('%Y-%m-%d %H:%M:%S'), 'waiting for system schedule...'))
-        query_system_schedule()
-        if system_task_queue.empty():
-            request_system_schedule()
-    return get_system_schedule()
+    while True:
+        schedule = request_system_schedule()
+        if schedule:
+            return schedule
+        time.sleep(1)
+    # try:
+    #     return system_task_queue.get(timeout=2)
+    # except Empty:
+    #     logger.debug('\r[%s]%s' % (time.strftime('%Y-%m-%d %H:%M:%S'), 'waiting for system schedule...'))
+    #     query_system_schedule()
+    #     if system_task_queue.empty():
+    #         request_system_schedule()
+    # return get_system_schedule()
 
 
 def get_schedule_executor(schedule):
     try:
         if not schedule.task.parent:
             raise KeyError
         cls = Executors[schedule.task.parent.name]
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self.schedule: SystemSchedule = schedule
 
     def execute(self):
         raise NotImplementedError
 
     def start(self):
         log = SystemScheduleLog(schedule=self.schedule, result={},
-                                status='S',
+                                status='S', queue=self.schedule.queue,
                                 schedule_time=self.schedule.next_schedule_time)
         err = None
         try:
             log.result['result'] = self.execute()
         except Exception as e:
             log.result['error'] = str(e)
             log.status = 'F'    # F: failed
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from django.urls import reverse
 import requests
 from .base import BaseExecutor
 from django.db import connection
 from django_common_task_system.system_task.models import SystemScheduleLog, SystemSchedule, builtins
-from django_common_task_system.models import TaskSchedule, TaskScheduleLog
+from django_common_task_system import get_task_schedule_model, get_schedule_log_model
+from django_common_task_system.models import ScheduleConfig
 from .. import settings
 
 _columns = None
 
+TaskScheduleLog = get_schedule_log_model()
+TaskSchedule = get_task_schedule_model()
+
 
 def get_schedule_table_columns(table):
     global _columns
     if not _columns:
         cmd = '''select GROUP_CONCAT(column_name SEPARATOR ',') from information_schema.`COLUMNS` 
         where column_name <> 'next_schedule_time' 
         and table_name = '%s' GROUP BY table_name''' % table
@@ -19,39 +23,57 @@
             cursor.execute(cmd)
             _columns = cursor.fetchone()[0].split(',')
     return _columns
 
 
 class SystemExceptionExecutor(BaseExecutor):
     name = builtins.tasks.system_exception_handling.name
+    schedule_id = builtins.schedules.system_exception_handling.id
     schedule_model = SystemSchedule
     schedule_log_model = SystemScheduleLog
-    handle_url = 'system_schedule_queue_put'
+    handle_url = 'system_schedule_put'
 
     def execute(self):
         max_retry_times = self.schedule.task.config.get('max_retry_times', 5)
-        columns = get_schedule_table_columns(table=self.schedule_model._meta.db_table)
+        max_fetch_num = self.schedule.task.config.get('max_fetch_num', 1000)
+        # columns = get_schedule_table_columns(table=self.schedule_model._meta.db_table)
+        next_schedule_time = ScheduleConfig(config=self.schedule.config).get_next_time(
+            self.schedule.next_schedule_time)
+        last_schedule_time = self.schedule.next_schedule_time - (next_schedule_time - self.schedule.next_schedule_time)
         command = '''
-            select %s, b.schedule_time as next_schedule_time from %s a join (
-            select schedule_id, schedule_time, count(*) as times, status from %s where create_time > CURDATE() 
-            GROUP BY schedule_id, schedule_time order by schedule_id, schedule_time
-            ) b on a.id = b.schedule_id where times < %s limit 1000
-        ''' % (',a.'.join(columns), self.schedule_model._meta.db_table,
-               self.schedule_log_model._meta.db_table, max_retry_times)
-        schedules = self.schedule_model.objects.raw(command)
-        path = reverse(self.handle_url, args=(self.schedule.id,))
-        url = settings.HOST + path
-        result = {}
-        for schedule in schedules:
-            try:
-                res = requests.get(url)
-                result[schedule.id] = res.status_code
-            except Exception as e:
-                result[schedule.id] = str(e)
-        return result
+            select * from (
+            select queue, schedule_id, schedule_time, count(*) as times, max(create_time) as lastest_time 
+            from %s where create_time > CURDATE() and status != 'S' 
+            GROUP BY queue, schedule_id, schedule_time order by queue, schedule_id, schedule_time
+            ) a where a.times < %s and a.lastest_time > '%s' limit %s
+        ''' % (self.schedule_log_model._meta.db_table, max_retry_times, last_schedule_time, max_fetch_num,)
+        with connection.cursor() as cursor:
+            cursor.execute(command)
+            rows = cursor.fetchall()
+        if rows:
+            path = reverse(self.handle_url)
+            ids, queues, times = [], [], []
+            for q, i, t, *_ in rows:
+                if i == self.schedule_id:
+                    continue
+                ids.append(str(i))
+                queues.append(q)
+                times.append(t.strftime('%Y-%m-%d %H:%M:%S'))
+            if ids:
+                url = settings.HOST + path
+                result = requests.get(url, params={
+                    'i': ','.join(ids),
+                    'q': ','.join(queues),
+                    't': ','.join(times)
+                }).json()
+                if 'error' in result:
+                    raise Exception(result['error'])
+                return result
+        return "no schedule need to retry"
 
 
 class ScheduleExceptionExecutor(SystemExceptionExecutor):
     name = builtins.tasks.task_exception_handling.name
     schedule_model = TaskSchedule
+    schedule_id = builtins.schedules.task_exception_handling.id
     schedule_log_model = TaskScheduleLog
     handle_url = 'task_schedule_put'
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     def execute(self):
         if sys.platform == 'win32':
             raise RuntimeError('Windows系统不支持shell命令执行')
 
         commands = self.schedule.task.config.get('shell', '').split(';')
         filename = '/tmp/shell_executor.sh'
-        with open('filename', 'w') as f:
+        with open(filename, 'w') as f:
             f.write('#!/bin/bash -e \n')
             f.write('; \n'.join(commands))
-        p = subprocess.Popen(['/bin/bash', filename], shell=True, stdout=subprocess.PIPE)
+        p = subprocess.Popen(f'/bin/bash {filename}', shell=True, stdout=subprocess.PIPE)
         out, err = p.communicate()
         if err:
             raise RuntimeError(err)
         return out.decode('utf-8')
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/urls.py` & `django-common-task-system-1.1.7/django_common_task_system/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 router = routers.DefaultRouter()
 router.register(r'schedule-log', views.ScheduleLogViewSet)
 
 
 urlpatterns = [
     path('task/', views.TaskListView.as_view()),
     path('task/<int:pk>/', views.TaskDetailView.as_view()),
-    path('schedule/', views.TaskScheduleListView.as_view()),
-    path('schedule/retry/<int:pk>/', views.TaskScheduleQueueAPI.retry, name='task_schedule_retry'),
-    path('schedule/queue/<int:pk>/put/', views.TaskScheduleQueueAPI.put, name='task_schedule_put'),
-    path('schedule/<int:pk>/', views.TaskScheduleDetailView.as_view()),
-    path('schedule/queue/get/', views.TaskScheduleQueueAPI.get),
-    path('schedule/queue/', views.TaskScheduleQueueAPI.status),
-    path('schedule/queue/<int:pk>/', views.TaskScheduleQueueAPI.get_by_id),
+    path('schedule/list/', views.TaskScheduleListView.as_view()),
+    path('schedule/retry/', views.TaskScheduleQueueAPI.retry, name='task_schedule_retry'),
+    path('schedule/put/', views.TaskScheduleQueueAPI.put, name='task_schedule_put'),
+    path('schedule/detail/<int:pk>/', views.TaskScheduleDetailView.as_view()),
+    path('schedule/queue/<slug:code>/get/', views.TaskScheduleQueueAPI.get, name='task_schedule_get'),
+    path('schedule/queue/detail/<int:pk>/', views.TaskScheduleQueueAPI.get_by_id),
+    path('schedule/queue/status/', views.TaskScheduleQueueAPI.status),
     path('schedule/time-parse/', views.ScheduleTimeParseView.as_view()),
 ] + router.urls
```

### Comparing `django-common-task-system-1.1.6/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.1.7/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.1.7/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.1.7/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.6/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.1.7/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,54 +5,65 @@
 django_common_task_system/__init__.py
 django_common_task_system/admin.py
 django_common_task_system/apps.py
 django_common_task_system/choices.py
 django_common_task_system/fields.py
 django_common_task_system/forms.py
 django_common_task_system/models.py
+django_common_task_system/permissions.py
 django_common_task_system/serializers.py
 django_common_task_system/tests.py
 django_common_task_system/urls.py
 django_common_task_system/views.py
 django_common_task_system.egg-info/PKG-INFO
 django_common_task_system.egg-info/SOURCES.txt
 django_common_task_system.egg-info/dependency_links.txt
 django_common_task_system.egg-info/requires.txt
 django_common_task_system.egg-info/top_level.txt
 django_common_task_system/migrations/0001_initial.py
 django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
 django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+django_common_task_system/migrations/0006_consumerpermission.py
 django_common_task_system/migrations/__init__.py
 django_common_task_system/static/common_task_system/css/calendar.css
 django_common_task_system/static/common_task_system/css/task_schedule_admin.css
 django_common_task_system/static/common_task_system/js/calendar.js
 django_common_task_system/static/common_task_system/js/task_schedule_admin.js
 django_common_task_system/system_task/__init__.py
 django_common_task_system/system_task/admin.py
 django_common_task_system/system_task/apps.py
 django_common_task_system/system_task/choices.py
 django_common_task_system/system_task/forms.py
 django_common_task_system/system_task/models.py
 django_common_task_system/system_task/process.py
+django_common_task_system/system_task/queue.py
+django_common_task_system/system_task/serializers.py
 django_common_task_system/system_task/tests.py
 django_common_task_system/system_task/urls.py
 django_common_task_system/system_task/views.py
 django_common_task_system/system_task/migrations/0001_initial.py
 django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
 django_common_task_system/system_task/migrations/__init__.py
 django_common_task_system/system_task_execution/__init__.py
 django_common_task_system/system_task_execution/main.py
 django_common_task_system/system_task_execution/system_task_execution/__init__.py
 django_common_task_system/system_task_execution/system_task_execution/executor.py
 django_common_task_system/system_task_execution/system_task_execution/settings.py
 django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
 django_common_task_system/system_task_execution/system_task_execution/executors/base.py
 django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
 django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
 django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+django_common_task_system/templates/admin/system_schedule/change_list.html
 django_common_task_system/templates/task_schedule/datetime_range.html
 django_common_task_system/templates/task_schedule/multi_day_select.html
 django_common_task_system/templates/task_schedule/multi_month_day_select.html
 django_common_task_system/templates/task_schedule/nlp_input.html
 django_common_task_system/templates/task_schedule/period.html
 django_common_task_system/templates/task_schedule/period_schedule.html
 django_common_task_system/utils/__init__.py
```

### Comparing `django-common-task-system-1.1.6/setup.py` & `django-common-task-system-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.1.6',
+    version='1.1.7',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

