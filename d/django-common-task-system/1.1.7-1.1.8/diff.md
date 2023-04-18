# Comparing `tmp/django-common-task-system-1.1.7.tar.gz` & `tmp/django-common-task-system-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.1.7.tar", last modified: Tue Apr 18 02:49:56 2023, max compression
+gzip compressed data, was "django-common-task-system-1.1.8.tar", last modified: Tue Apr 18 06:28:24 2023, max compression
```

## Comparing `django-common-task-system-1.1.7.tar` & `django-common-task-system-1.1.8.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.154166 django-common-task-system-1.1.7/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.7/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-18 02:49:56.154166 django-common-task-system-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.111414 django-common-task-system-1.1.7/django_common_task_system/
--rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.1.7/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0     9800 2023-04-17 08:40:58.000000 django-common-task-system-1.1.7/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.7/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.1.7/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.7/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.1.7/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.121696 django-common-task-system-1.1.7/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.7/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0    34023 2023-04-18 02:49:48.000000 django-common-task-system-1.1.7/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.1.7/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.1.7/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.097000 django-common-task-system-1.1.7/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.097000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.122697 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.124696 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.133166 django-common-task-system-1.1.7/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     4987 2023-04-17 08:40:58.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     4122 2023-04-13 09:07:07.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.138166 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    17147 2023-04-18 02:49:48.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.1.7/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.139169 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-04-12 09:15:38.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.140166 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.143166 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.100000 django-common-task-system-1.1.7/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.100000 django-common-task-system-1.1.7/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.144166 django-common-task-system-1.1.7/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     6709 2023-04-14 09:00:33.000000 django-common-task-system-1.1.7/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.148166 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.7/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.1.7/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.152166 django-common-task-system-1.1.7/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.7/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.7/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.7/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.7/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.7/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    10457 2023-04-18 02:48:30.000000 django-common-task-system-1.1.7/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.116690 django-common-task-system-1.1.7/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4218 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-18 02:49:56.000000 django-common-task-system-1.1.7/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 02:49:56.154166 django-common-task-system-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-17 01:39:35.000000 django-common-task-system-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:49:56.153165 django-common-task-system-1.1.7/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.129534 django-common-task-system-1.1.8/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-18 06:28:24.129534 django-common-task-system-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.086859 django-common-task-system-1.1.8/django_common_task_system/
+-rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.1.8/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0     9800 2023-04-17 08:40:58.000000 django-common-task-system-1.1.8/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.8/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.1.8/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.8/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.1.8/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.098240 django-common-task-system-1.1.8/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.8/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.1.8/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    34023 2023-04-18 02:49:48.000000 django-common-task-system-1.1.8/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.1.8/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.1.8/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.070854 django-common-task-system-1.1.8/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.070854 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.099247 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.101249 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.108444 django-common-task-system-1.1.8/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     4987 2023-04-17 08:40:58.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4122 2023-04-13 09:07:07.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.113959 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    17147 2023-04-18 02:49:48.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.1.8/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.114958 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-04-12 09:15:38.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.116958 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     3409 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.120527 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.072862 django-common-task-system-1.1.8/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.072862 django-common-task-system-1.1.8/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.121534 django-common-task-system-1.1.8/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     6709 2023-04-14 09:00:33.000000 django-common-task-system-1.1.8/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.124535 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.8/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.1.8/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.128534 django-common-task-system-1.1.8/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.8/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.8/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.8/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.8/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.8/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    10457 2023-04-18 02:48:30.000000 django-common-task-system-1.1.8/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.093549 django-common-task-system-1.1.8/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4253 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-18 06:28:24.000000 django-common-task-system-1.1.8/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:28:24.129534 django-common-task-system-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-18 06:24:58.000000 django-common-task-system-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:28:24.128534 django-common-task-system-1.1.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.8/tests/__init__.py
```

### Comparing `django-common-task-system-1.1.7/LICENSE` & `django-common-task-system-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/__init__.py` & `django-common-task-system-1.1.8/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/admin.py` & `django-common-task-system-1.1.8/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/choices.py` & `django-common-task-system-1.1.8/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/fields.py` & `django-common-task-system-1.1.8/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/forms.py` & `django-common-task-system-1.1.8/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.1.8/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.1.8/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.1.8/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.1.8/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/models.py` & `django-common-task-system-1.1.8/django_common_task_system/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/permissions.py` & `django-common-task-system-1.1.8/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/serializers.py` & `django-common-task-system-1.1.8/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.1.8/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/models.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/process.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task/views.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.1.8/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.1.8/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.1.8/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/urls.py` & `django-common-task-system-1.1.8/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.1.8/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.1.8/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.1.8/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system/views.py` & `django-common-task-system-1.1.8/django_common_task_system/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.7/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.1.8/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 django_common_task_system/__init__.py
 django_common_task_system/admin.py
 django_common_task_system/apps.py
 django_common_task_system/choices.py
 django_common_task_system/fields.py
 django_common_task_system/forms.py
+django_common_task_system/mixin.py
 django_common_task_system/models.py
 django_common_task_system/permissions.py
 django_common_task_system/serializers.py
 django_common_task_system/tests.py
 django_common_task_system/urls.py
 django_common_task_system/views.py
 django_common_task_system.egg-info/PKG-INFO
```

### Comparing `django-common-task-system-1.1.7/setup.py` & `django-common-task-system-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.1.7',
+    version='1.1.8',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

