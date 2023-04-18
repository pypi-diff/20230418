# Comparing `tmp/django_rq_scheduler-2023.5.0b4.tar.gz` & `tmp/django_rq_scheduler-2023.5.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rq_scheduler-2023.5.0b4.tar", max compression
+gzip compressed data, was "django_rq_scheduler-2023.5.0b5.tar", max compression
```

## Comparing `django_rq_scheduler-2023.5.0b4.tar` & `django_rq_scheduler-2023.5.0b5.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0     1107 2023-04-17 16:42:06.746785 django_rq_scheduler-2023.5.0b4/LICENSE
--rw-r--r--   0        0        0     1704 2023-04-17 16:42:06.746785 django_rq_scheduler-2023.5.0b4/README.md
--rw-r--r--   0        0        0     1741 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/pyproject.toml
--rw-r--r--   0        0        0      134 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/__init__.py
--rw-r--r--   0        0        0      147 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     5661 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/admin/job.py
--rw-r--r--   0        0        0     1641 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0      355 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/apps.py
--rw-r--r--   0        0        0     1207 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1189 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/delete_failed_executions.py
--rw-r--r--   0        0        0     1908 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     3417 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3602 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     2962 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1374 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     7162 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0     1051 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1362 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      661 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     7643 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      187 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/queue.py
--rw-r--r--   0        0        0    15140 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/scheduled_job.py
--rw-r--r--   0        0        0      366 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/py.typed
--rw-r--r--   0        0        0     4858 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/queues.py
--rw-r--r--   0        0        0     7780 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/rq_classes.py
--rw-r--r--   0        0        0      932 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/settings.py
--rw-r--r--   0        0        0      163 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1559 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     1282 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/delete_job.html
--rw-r--r--   0        0        0     7124 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     2697 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs-list.partial.html
--rw-r--r--   0        0        0     6285 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0     1055 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     4120 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3032 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1875 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      535 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/jobs.py
--rw-r--r--   0        0        0      668 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5887 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     2349 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_job_decorator.py
--rw-r--r--   0        0        0     4304 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    27529 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     2211 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    14933 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_views.py
--rw-r--r--   0        0        0     1577 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3311 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     2572 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tools.py
--rw-r--r--   0        0        0     1736 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/urls.py
--rw-r--r--   0        0        0    16009 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/views.py
--rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-04-18 20:24:54.707516 django_rq_scheduler-2023.5.0b5/LICENSE
+-rw-r--r--   0        0        0     1558 2023-04-18 20:24:54.707516 django_rq_scheduler-2023.5.0b5/README.md
+-rw-r--r--   0        0        0     1741 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     5661 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/admin/job.py
+-rw-r--r--   0        0        0     1641 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0      281 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/apps.py
+-rw-r--r--   0        0        0     1207 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1189 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1908 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     3417 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3602 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     3090 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     7162 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      728 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1362 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      661 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     7643 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0      935 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3102 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/queue.py
+-rw-r--r--   0        0        0    15140 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/scheduled_job.py
+-rw-r--r--   0        0        0      366 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/py.typed
+-rw-r--r--   0        0        0     4858 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/queues.py
+-rw-r--r--   0        0        0     7780 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/rq_classes.py
+-rw-r--r--   0        0        0      932 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/settings.py
+-rw-r--r--   0        0        0      163 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1559 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     1282 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/delete_job.html
+-rw-r--r--   0        0        0     7124 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     2697 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs-list.partial.html
+-rw-r--r--   0        0        0     6297 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0     1055 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     4120 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3032 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1875 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0     1396 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0      668 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5887 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     2349 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_decorator.py
+-rw-r--r--   0        0        0     4816 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    27529 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     2211 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    14933 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0     1577 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3311 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     2572 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tools.py
+-rw-r--r--   0        0        0     1736 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/urls.py
+-rw-r--r--   0        0        0    16009 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/views.py
+-rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b5/PKG-INFO
```

### Comparing `django_rq_scheduler-2023.5.0b4/LICENSE` & `django_rq_scheduler-2023.5.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/README.md` & `django_rq_scheduler-2023.5.0b5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -3,21 +3,17 @@
 [![Django CI](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml/badge.svg)](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml)
 ![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/cunla/b756396efb895f0e34558c980f1ca0c7/raw/django-rq-scheduler-4.json)
 [![badge](https://img.shields.io/pypi/dm/django-rq-scheduler)](https://pypi.org/project/django-rq-scheduler/)
 [![Open Source Helpers](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler/badges/users.svg)](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler)
 
 Documentation can be found in https://django-rq-scheduler.readthedocs.io/en/latest/
 
->  **Warning**: In v2023.3.0, django-rq-scheduler was refactored significantly to support
-> calculation of parameters in runtime.
-> You can now add a callable param to your scheduled job, and it will be
-> calculated when the job is performed.
-> 
-> 1. It is highly recommended you save your existing database before upgrading!
-> 2. Once you upgraded, recreate your jobs.
+> **Note**: Starting v2023.5.0, django-rq-scheduler does not require django-rq.
+> All required views were migrated. Make sure to read the installation notes in the documentation.
+> Particularly how to set up your `urls.py`.
 
 > **Note** Starting v2023.1, requirement for rq_scheduler was removed and instead
 > one of the django-rq workers should run with `--with-scheduler` parameter
 > as mentioned [here](https://github.com/rq/django-rq#support-for-scheduled-jobs).
 
 
 # Sponsor
```

### Comparing `django_rq_scheduler-2023.5.0b4/pyproject.toml` & `django_rq_scheduler-2023.5.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-rq-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "2023.5.0b4"
+version = "2023.5.0b5"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
     "Daniel Moran <daniel.maruani@gmail.com>",
 ]
 maintainers = [
```

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/admin/job.py` & `django_rq_scheduler-2023.5.0b5/scheduler/admin/job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/admin/redis_models.py` & `django_rq_scheduler-2023.5.0b5/scheduler/admin/redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/decorators.py` & `django_rq_scheduler-2023.5.0b5/scheduler/decorators.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/delete_failed_executions.py` & `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/delete_failed_executions.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/export.py` & `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/export.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/import.py` & `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqstats.py` & `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqstats.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqworker.py` & `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqworker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import logging
 import os
 import sys
 
 import click
 from django.core.management.base import BaseCommand
 from django.db import connections
 from redis.exceptions import ConnectionError
 from rq import use_connection
 from rq.logutils import setup_loghandlers
 
 from scheduler.tools import create_worker
 
-LOG_LEVELS = {
-    0: "CRITICAL",
-    1: "WARNING",
-    2: "INFO",
-    3: "DEBUG",
+VERBOSITY_TO_LOG_LEVEL = {
+    0: logging.CRITICAL,
+    1: logging.WARNING,
+    2: logging.INFO,
+    3: logging.DEBUG,
 }
 
 
 def reset_db_connections():
     for c in connections.all():
         c.close()
 
@@ -46,36 +47,38 @@
         parser.add_argument('--max-jobs', action='store', default=None, dest='max_jobs', type=int,
                             help='Maximum number of jobs to execute before terminating worker')
         parser.add_argument(
             'queues', nargs='*', type=str,
             help='The queues to work on, separated by space, all queues should be using the same redis')
 
     def handle(self, **options):
-        queues = options.get('queues', 'default')
+        queues = options.get('queues', [])
+        if not queues:
+            queues = ['default', ]
         click.echo(f'Starting worker for queues {queues}')
         pidfile = options.get('pidfile')
         if pidfile:
             with open(os.path.expanduser(pidfile), "w") as fp:
                 fp.write(str(os.getpid()))
 
         # Verbosity is defined by default in BaseCommand for all commands
         verbosity = options.get('verbosity', 1)
-        level = LOG_LEVELS.get(verbosity, 'INFO')
-        setup_loghandlers(level)
+        log_level = VERBOSITY_TO_LOG_LEVEL.get(verbosity, logging.INFO)
+        setup_loghandlers(log_level)
 
         try:
             # Instantiate a worker
             w = create_worker(*queues, name=options['name'], default_worker_ttl=options['worker_ttl'], )
 
             # Call use_connection to push the redis connection into LocalStack
             # without this, jobs using RQ's get_current_job() will fail
             use_connection(w.connection)
 
             # Close any opened DB connection before any fork
             reset_db_connections()
 
             w.work(burst=options.get('burst', False),
-                   logging_level=verbosity,
+                   logging_level=log_level,
                    max_jobs=options['max_jobs'], )
         except ConnectionError as e:
             click.echo(str(e), err=True)
             sys.exit(1)
```

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/run_job.py` & `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/run_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0003_auto_20220329_2107.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0006_auto_20230118_1640.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 # Generated by Django 4.1.5 on 2023-01-18 16:40
 
 from django.db import migrations
 
 
 def forwards_func(apps, schema_editor):
-    cronjob_model = apps.get_model(app_label='scheduler', model_name='CronJob')
-    scheduler_job = cronjob_model.objects.create(
-        cron_string='* * * * *',
-        name='Job scheduling jobs',
-        callable='scheduler.apps.reschedule_all_jobs',
-        enabled=True,
-        queue='default',
-    )
-    scheduler_job.save()
+    pass
 
 
 def reverse_func(apps, schema_editor):
     # forwards_func() creates two Country instances,
     # so reverse_func() should delete them.
     cronjob_model = apps.get_model(app_label='scheduler', model_name='CronJob')
     db_alias = schema_editor.connection.alias
```

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0007_add_result_ttl.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0010_queue.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0010_queue.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/models/args.py` & `django_rq_scheduler-2023.5.0b5/scheduler/models/args.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/models/scheduled_job.py` & `django_rq_scheduler-2023.5.0b5/scheduler/models/scheduled_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/queues.py` & `django_rq_scheduler-2023.5.0b5/scheduler/queues.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/rq_classes.py` & `django_rq_scheduler-2023.5.0b5/scheduler/rq_classes.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/settings.py` & `django_rq_scheduler-2023.5.0b5/scheduler/settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/confirm_action.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/delete_job.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/delete_job.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/job_detail.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs-list.partial.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs.html`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                                         {{ job.id }}
                                     </a>
                                 </th>
                                 <td>
                                     {{ job.created_at|date:"Y-m-d, H:i:s" }}
                                 </td>
                                 <td>
-                                    {{ job.scheduled_at|date:"Y-m-d, H:i:s" }}
+                                    {{ job|job_scheduled_time:queue|date:"Y-m-d, H:i:s" }}
                                 </td>
                                 <td>
                                     {{ job.enqueued_at|date:"Y-m-d, H:i:s" }}
                                 </td>
                                 <td>
                                     {{ job.ended_at|date:"Y-m-d, H:i:s" }}
                                 </td>
```

#### html2text {}

```diff
@@ -11,15 +11,16 @@
     * {% endif %}
     * Empty_Queue
 {% csrf_token %}
 {% if job_status == 'Failed' %}
 Requeue
 {% endif %}
   Go
-�ID     Created              Scheduled              Enqueued              Ended              Status         Callable           Worker
-  {      {                    {                      {                     {                  {              {                  {
-�{      {                    {                      {                     {                  {              {                  {
-  job.id job.created_at|date: job.scheduled_at|date: job.enqueued_at|date: job.ended_at|date: job.get_status job|show_func_name job.worker_name|default:
-  }}     "Y-m-d, H:i:s" }}    "Y-m-d, H:i:s" }}      "Y-m-d, H:i:s" }}     "Y-m-d, H:i:s" }}  }}             }}                 '-' }}
+�ID     Created              Scheduled               Enqueued              Ended              Status         Callable           Worker
+  {      {                    {                       {                     {                  {              {                  {
+  {      {                    {                       {                     {                  {              {                  {
+�job.id job.created_at|date: job|job_scheduled_time: job.enqueued_at|date: job.ended_at|date: job.get_status job|show_func_name job.worker_name|default:
+  }}     "Y-m-d, H:i:s" }}    queue|date:"Y-m-d, H:i: "Y-m-d, H:i:s" }}     "Y-m-d, H:i:s" }}  }}             }}                 '-' }}
+                              s" }}
 {% for p in page_range %} {% if p == page %} {{ p }} {% elif forloop.last %} {
 {_p_}} {% else %} {{_p_}} {% endif %} {% endfor %} {{ num_jobs }} jobs
 {% endblock %}
```

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/queue_workers.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/stats.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/stats.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,21 @@
                         </th>
                         <th>
                             <a href="{% url 'queue_failed_jobs' queue.name %}">
                                 {{ queue.failed_jobs }}
                             </a>
                         </th>
                         <th>
-                            <a href="{% url 'queue_failed_jobs' queue.name %}">
-                                {{ queue.canceled_jobs }}
+                            <a href="{% url 'queue_scheduled_jobs' queue.name %}">
+                                {{ queue.scheduled_jobs }}
                             </a>
                         </th>
                         <th>
-                            <a href="{% url 'queue_scheduled_jobs' queue.name %}">
-                                {{ queue.scheduled_jobs }}
+                            <a href="{% url 'queue_failed_jobs' queue.name %}">
+                                {{ queue.canceled_jobs }}
                             </a>
                         </th>
                         <th><a href="{% url 'queue_workers' queue.name %}">
                             {{ queue.workers }}
                         </a>
                         </th>
                         <td>{{ queue.connection_kwargs.host }}</td>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% extends "admin/base_site.html" %} {% block title %}Queues {{ block.super }}
 {% endblock %} {% block extrastyle %} {{ block.super }}
  {% endblock %} {% block content_title %}
 ****** RQ Queues ******
 {% endblock %} {% block breadcrumbs %}
 Home › Queues
 {% endblock %} {% block content %}
-Name       Queued     Oldest Queued Job          Active Jobs        Deferred Jobs       Finished Jobs       Failed Jobs       Scheduled Jobs      Canceled Jobs        Workers       Host                         Port                         DB                         Scheduler PID
+Name       Queued     Oldest Queued Job          Active Jobs        Deferred Jobs       Finished Jobs       Failed Jobs       Scheduled Jobs       Canceled Jobs       Workers       Host                         Port                         DB                         Scheduler PID
            Jobs
-{          {          {                          {                  {                   {                   {                 {                   {                    {             {                            {                            {                          {
-{          {          {                          {                  {                   {                   {                 {                   {                    {             {                            {                            {                          {
-queue.name queue.jobs queue.oldest_job_timestamp queue.started_jobs queue.deferred_jobs queue.finished_jobs queue.failed_jobs queue.canceled_jobs queue.scheduled_jobs queue.workers queue.connection_kwargs.host queue.connection_kwargs.port queue.connection_kwargs.db queue.scheduler_pid|default_if_none:
-}}         }}         }}                         }}                 }}                  }}                  }}                }}                  }}                   }}            }}                           }}                           }}                         "Inactive" }}
+{          {          {                          {                  {                   {                   {                 {                    {                   {             {                            {                            {                          {
+{          {          {                          {                  {                   {                   {                 {                    {                   {             {                            {                            {                          {
+queue.name queue.jobs queue.oldest_job_timestamp queue.started_jobs queue.deferred_jobs queue.finished_jobs queue.failed_jobs queue.scheduled_jobs queue.canceled_jobs queue.workers queue.connection_kwargs.host queue.connection_kwargs.port queue.connection_kwargs.db queue.scheduler_pid|default_if_none:
+}}         }}         }}                         }}                 }}                  }}                  }}                }}                   }}                  }}            }}                           }}                           }}                         "Inactive" }}
 
 View_as_JSON
 {% endblock %}
```

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/worker_details.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers.html` & `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/templatetags/scheduler_tags.py` & `django_rq_scheduler-2023.5.0b5/scheduler/templatetags/scheduler_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django import template
 
-from scheduler.rq_classes import JobExecution
+from scheduler.rq_classes import JobExecution, DjangoQueue
 from scheduler.tools import get_scheduled_job
 
 register = template.Library()
 
 
 @register.filter
 def show_func_name(rq_job: JobExecution) -> str:
@@ -45,7 +45,15 @@
     if ended_at:
         runtime = job.ended_at - job.started_at
         return f'{int(runtime.microseconds / 1000)}ms'
     elif job.started_at:
         return "Still running"
     else:
         return "-"
+
+
+@register.filter
+def job_scheduled_time(job: JobExecution, queue: DjangoQueue):
+    try:
+        return queue.scheduled_job_registry.get_scheduled_time(job.id)
+    except Exception:
+        return None
```

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/jobs.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/jobs.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_internals.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_job_arg_models.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_arg_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_job_decorator.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_decorator.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_mgmt_cmds.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_mgmt_cmds.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,32 @@
 from scheduler.tests.jobs import failing_job, test_job
 from scheduler.tests.testtools import job_factory
 from . import test_settings  # noqa
 
 
 class RqworkerTestCase(TestCase):
 
+    def test_rqworker__no_queues_params(self):
+        queue = get_queue('default')
+
+        # enqueue some jobs that will fail
+        jobs = []
+        job_ids = []
+        for _ in range(0, 3):
+            job = queue.enqueue(failing_job)
+            jobs.append(job)
+            job_ids.append(job.id)
+
+        # Create a worker to execute these jobs
+        call_command('rqworker', burst=True)
+
+        # check if all jobs are really failed
+        for job in jobs:
+            self.assertTrue(job.is_failed)
+
     def test_rqworker__run_jobs(self):
         queue = get_queue('default')
 
         # enqueue some jobs that will fail
         jobs = []
         job_ids = []
         for _ in range(0, 3):
@@ -100,15 +118,15 @@
         jobs.append(job_factory(ScheduledJob, enabled=True))
         jobs.append(job_factory(RepeatableJob, enabled=True))
 
         # act
         call_command('export', filename=self.tmpfile.name)
         # assert
         result = json.load(self.tmpfile)
-        self.assertEqual(len(jobs) + 1, len(result))
+        self.assertEqual(len(jobs), len(result))
         self.assertEqual(result[0], jobs[0].to_dict())
         self.assertEqual(result[1], jobs[1].to_dict())
 
 
 class ImportTest(TestCase):
     def setUp(self) -> None:
         self.tmpfile = tempfile.NamedTemporaryFile(mode='w')
```

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_models.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_redis_models.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_settings.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_views.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_worker.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tests/testtools.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tests/testtools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/tools.py` & `django_rq_scheduler-2023.5.0b5/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/urls.py` & `django_rq_scheduler-2023.5.0b5/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/scheduler/views.py` & `django_rq_scheduler-2023.5.0b5/scheduler/views.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b4/PKG-INFO` & `django_rq_scheduler-2023.5.0b5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq-scheduler
-Version: 2023.5.0b4
+Version: 2023.5.0b5
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-rq-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
 Author-email: daniel.maruani@gmail.com
 Maintainer: Daniel Moran
@@ -44,21 +44,17 @@
 [![Django CI](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml/badge.svg)](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml)
 ![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/cunla/b756396efb895f0e34558c980f1ca0c7/raw/django-rq-scheduler-4.json)
 [![badge](https://img.shields.io/pypi/dm/django-rq-scheduler)](https://pypi.org/project/django-rq-scheduler/)
 [![Open Source Helpers](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler/badges/users.svg)](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler)
 
 Documentation can be found in https://django-rq-scheduler.readthedocs.io/en/latest/
 
->  **Warning**: In v2023.3.0, django-rq-scheduler was refactored significantly to support
-> calculation of parameters in runtime.
-> You can now add a callable param to your scheduled job, and it will be
-> calculated when the job is performed.
-> 
-> 1. It is highly recommended you save your existing database before upgrading!
-> 2. Once you upgraded, recreate your jobs.
+> **Note**: Starting v2023.5.0, django-rq-scheduler does not require django-rq.
+> All required views were migrated. Make sure to read the installation notes in the documentation.
+> Particularly how to set up your `urls.py`.
 
 > **Note** Starting v2023.1, requirement for rq_scheduler was removed and instead
 > one of the django-rq workers should run with `--with-scheduler` parameter
 > as mentioned [here](https://github.com/rq/django-rq#support-for-scheduled-jobs).
 
 
 # Sponsor
```

