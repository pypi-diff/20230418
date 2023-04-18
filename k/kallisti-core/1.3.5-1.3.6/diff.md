# Comparing `tmp/kallisti-core-1.3.5.tar.gz` & `tmp/kallisti-core-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\f658643\projects\oss-kallisti-core\1\github-jpmc\kallisti-core\dist\tmpvgi9ixcr\kallisti-core-1.3.5.tar", last modified: Wed May  4 06:11:03 2022, max compression
+gzip compressed data, was "kallisti-core-1.3.6.tar", last modified: Tue Apr 18 10:37:13 2023, max compression
```

## Comparing `kallisti-core-1.3.5.tar` & `kallisti-core-1.3.6.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/
--rw-rw-rw-   0        0        0      274 2022-05-04 06:06:15.000000 kallisti-core-1.3.5/.bumpversion.cfg
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/
--rw-rw-rw-   0        0        0      237 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/apps.py
--rw-rw-rw-   0        0        0     2340 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/authentication.py
--rw-rw-rw-   0        0        0     2823 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/lib/
--rw-rw-rw-   0        0        0     6878 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/action.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/lib/authentication/
--rw-rw-rw-   0        0        0     2305 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/authentication/jwt.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/authentication/__init__.py
--rw-rw-rw-   0        0        0     2456 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/credential.py
--rw-rw-rw-   0        0        0     5678 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/expectation.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/lib/observe/
--rw-rw-rw-   0        0        0      254 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/observe/observer.py
--rw-rw-rw-   0        0        0     1020 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/observe/subject.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/observe/__init__.py
--rw-rw-rw-   0        0        0     8431 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/trial_executor.py
--rw-rw-rw-   0        0        0     2051 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/trial_log_recorder.py
--rw-rw-rw-   0        0        0      888 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/trial_scheduler.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/migrations/
--rw-rw-rw-   0        0        0     1524 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      625 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0002_experiment_steps.py
--rw-rw-rw-   0        0        0      462 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0003_trial_parameters.py
--rw-rw-rw-   0        0        0      868 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0004_auto_20190416_1800.py
--rw-rw-rw-   0        0        0      603 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0005_trial_ticket.py
--rw-rw-rw-   0        0        0      425 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0006_trial_initiated_by.py
--rw-rw-rw-   0        0        0      424 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0007_trial_completed_at.py
--rw-rw-rw-   0        0        0      461 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0008_trial_records.py
--rw-rw-rw-   0        0        0     1676 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0009_trialschedule.py
--rw-rw-rw-   0        0        0      840 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0010_auto_20190618_1356.py
--rw-rw-rw-   0        0        0      434 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0011_trialschedule_recurrence_left.py
--rw-rw-rw-   0        0        0      748 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0012_auto_20190709_1827.py
--rw-rw-rw-   0        0        0      662 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0013_notification.py
--rw-rw-rw-   0        0        0      770 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0014_notification_seed.py
--rw-rw-rw-   0        0        0      466 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0015_auto_20190906_1502.py
--rw-rw-rw-   0        0        0      883 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0016_config.py
--rw-rw-rw-   0        0        0      719 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0017_config_seed.py
--rw-rw-rw-   0        0        0      309 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0018_delete_config.py
--rw-rw-rw-   0        0        0      410 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0019_auto_20201230_1554.py
--rw-rw-rw-   0        0        0      433 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/0020_trial_initiated_from.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/models/
--rw-rw-rw-   0        0        0      221 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/base_model.py
--rw-rw-rw-   0        0        0     1487 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/experiment.py
--rw-rw-rw-   0        0        0      445 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/notification.py
--rw-rw-rw-   0        0        0      190 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/singleton_manager.py
--rw-rw-rw-   0        0        0      335 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/singleton_model.py
--rw-rw-rw-   0        0        0     3231 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/step.py
--rw-rw-rw-   0        0        0     5575 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/trial.py
--rw-rw-rw-   0        0        0     3915 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/trial_schedule.py
--rw-rw-rw-   0        0        0       90 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/aws/
--rw-rw-rw-   0        0        0     1769 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/aws/aws_action.py
--rw-rw-rw-   0        0        0       89 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/aws/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/cloud_foundry/
--rw-rw-rw-   0        0        0     2626 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/cloud_foundry/actions.py
--rw-rw-rw-   0        0        0     1659 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/cloud_foundry/cloud_foundry_action.py
--rw-rw-rw-   0        0        0     2077 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/cloud_foundry/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/common/
--rw-rw-rw-   0        0        0     5534 2022-05-04 04:55:00.000000 kallisti-core-1.3.5/kallisticore/modules/common/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/examples/
--rw-rw-rw-   0        0        0      184 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/examples/sample_module1.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/examples/sample_module2/
--rw-rw-rw-   0        0        0      228 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/examples/sample_module2/increment_action.py
--rw-rw-rw-   0        0        0       65 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/examples/sample_module2/multiply_action.py
--rw-rw-rw-   0        0        0       67 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/examples/sample_module2/subtract_action.py
--rw-rw-rw-   0        0        0      236 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/examples/sample_module2/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/kubernetes/
--rw-rw-rw-   0        0        0     5882 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/kubernetes/kubernetes_actions.py
--rw-rw-rw-   0        0        0      977 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/kubernetes/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/modules/prometheus/
--rw-rw-rw-   0        0        0      795 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/prometheus/__init__.py
--rw-rw-rw-   0        0        0       57 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/modules/__init__.py
--rw-rw-rw-   0        0        0      172 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/permissions.py
--rw-rw-rw-   0        0        0     2466 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/renderers.py
--rw-rw-rw-   0        0        0     7071 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/serializers.py
--rw-rw-rw-   0        0        0      691 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/signals.py
--rw-rw-rw-   0        0        0      465 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/tasks.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/templates/
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/templates/kallisticore/
--rw-rw-rw-   0        0        0    17748 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/templates/kallisticore/xsl_template.xml
--rw-rw-rw-   0        0        0     1027 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/urls.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/utils/
--rw-rw-rw-   0        0        0     2670 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/utils/fields.py
--rw-rw-rw-   0        0        0     1976 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/utils/logging.py
--rw-rw-rw-   0        0        0     1148 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/utils/pid_manager.py
--rw-rw-rw-   0        0        0     1329 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/utils/sanitizer.py
--rw-rw-rw-   0        0        0      909 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/utils/singleton.py
--rw-rw-rw-   0        0        0      314 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/utils/threadlocals.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/utils/__init__.py
--rw-rw-rw-   0        0        0       19 2022-05-04 06:06:15.000000 kallisti-core-1.3.5/kallisticore/version.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisticore/views/
--rw-rw-rw-   0        0        0     1261 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/views/experiment.py
--rw-rw-rw-   0        0        0      839 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/views/notification.py
--rw-rw-rw-   0        0        0     1601 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/views/report.py
--rw-rw-rw-   0        0        0     1299 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/views/trial.py
--rw-rw-rw-   0        0        0     1862 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/views/trial_schedule.py
--rw-rw-rw-   0        0        0     1278 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/views/trial_stop.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/views/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/kallisticore/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisti_core.egg-info/
--rw-rw-rw-   0        0        0        1 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisti_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1983 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisti_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisti_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0     6481 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisti_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       19 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/kallisti_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     1668 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/Makefile
--rw-rw-rw-   0        0        0      553 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/manage.py
--rw-rw-rw-   0        0        0      228 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1983 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1314 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/README.md
--rw-rw-rw-   0        0        0       75 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/requirements-dev.txt
--rw-rw-rw-   0        0        0      709 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1751 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/
--rw-rw-rw-   0        0        0      824 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/base.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/lib/
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/lib/authentication/
--rw-rw-rw-   0        0        0     2555 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/authentication/test_jwt.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/authentication/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/lib/observe/
--rw-rw-rw-   0        0        0      778 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/observe/test_observer.py
--rw-rw-rw-   0        0        0     1809 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/observe/test_subject.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/observe/__init__.py
--rw-rw-rw-   0        0        0    10604 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/test_action.py
--rw-rw-rw-   0        0        0     3111 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/test_credential.py
--rw-rw-rw-   0        0        0    11184 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/test_expectation.py
--rw-rw-rw-   0        0        0    41902 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/test_trial_executor.py
--rw-rw-rw-   0        0        0     8169 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/test_trial_log_recorder.py
--rw-rw-rw-   0        0        0     2573 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/test_trial_scheduler.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/models/
--rw-rw-rw-   0        0        0     4387 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/models/test_experiment.py
--rw-rw-rw-   0        0        0      980 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/models/test_notification.py
--rw-rw-rw-   0        0        0     4768 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/models/test_step.py
--rw-rw-rw-   0        0        0    17797 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/models/test_trial.py
--rw-rw-rw-   0        0        0    10086 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/models/test_trial_schedule.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/modules/
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/modules/aws/
--rw-rw-rw-   0        0        0     2282 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/aws/test_aws_action.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/aws/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/
--rw-rw-rw-   0        0        0     5412 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/test_actions.py
--rw-rw-rw-   0        0        0     4205 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/test_cloud_foundry_actions.py
--rw-rw-rw-   0        0        0     2676 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/test_get_user_organization_by_name.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/modules/common/
--rw-rw-rw-   0        0        0    28696 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/common/test_common.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/common/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/modules/kubernetes/
--rw-rw-rw-   0        0        0     9042 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/kubernetes/test_kubernetes_action.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/kubernetes/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/modules/prometheus/
--rw-rw-rw-   0        0        0     2093 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/prometheus/test_prometheus_action.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/prometheus/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/renderers/
--rw-rw-rw-   0        0        0     2165 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/renderers/test_xml_renderer.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/renderers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/serializers/
--rw-rw-rw-   0        0        0     2112 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/serializers/test_experiment_serializer.py
--rw-rw-rw-   0        0        0      680 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/serializers/test_notification_serializer.py
--rw-rw-rw-   0        0        0     5784 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/serializers/test_report_serializer.py
--rw-rw-rw-   0        0        0     2095 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/serializers/test_trial_schedule_serializer.py
--rw-rw-rw-   0        0        0     2250 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/serializers/test_trial_serializer.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/serializers/__init__.py
--rw-rw-rw-   0        0        0     3439 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/test_authentication.py
--rw-rw-rw-   0        0        0     3476 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/test_exceptions.py
--rw-rw-rw-   0        0        0      548 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/test_permissions.py
--rw-rw-rw-   0        0        0     1714 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/test_signals.py
--rw-rw-rw-   0        0        0     1009 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/test_tasks.py
--rw-rw-rw-   0        0        0      191 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/test_urls.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/utils/
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/utils/fixture/
--rw-rw-rw-   0        0        0    14095 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/utils/fixture/trial_result_data.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/utils/fixture/__init__.py
--rw-rw-rw-   0        0        0     7847 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/utils/test_fields.py
--rw-rw-rw-   0        0        0     2768 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/utils/test_logging.py
--rw-rw-rw-   0        0        0     2968 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/utils/test_pid_manager.py
--rw-rw-rw-   0        0        0      941 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/utils/test_sanitizer.py
--rw-rw-rw-   0        0        0     1263 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/utils/test_singleton.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 06:11:03.000000 kallisti-core-1.3.5/tests/kallisticore/views/
--rw-rw-rw-   0        0        0     6293 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/views/test_experiment.py
--rw-rw-rw-   0        0        0     2054 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/views/test_notification.py
--rw-rw-rw-   0        0        0     3932 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/views/test_report.py
--rw-rw-rw-   0        0        0     3745 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/views/test_stop.py
--rw-rw-rw-   0        0        0     7298 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/views/test_trial.py
--rw-rw-rw-   0        0        0     9975 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/views/test_trial_schedule.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:30.000000 kallisti-core-1.3.5/tests/kallisticore/views/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/kallisticore/__init__.py
--rw-rw-rw-   0        0        0      146 2022-04-20 07:37:29.000000 kallisti-core-1.3.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:13.902561 kallisti-core-1.3.6/
+-rw-rw-rw-   0        0        0      274 2023-04-17 11:32:16.000000 kallisti-core-1.3.6/.bumpversion.cfg
+-rw-rw-rw-   0        0        0    11558 2023-04-11 05:58:29.000000 kallisti-core-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0      228 2023-04-11 05:58:30.000000 kallisti-core-1.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1668 2023-04-11 05:58:30.000000 kallisti-core-1.3.6/Makefile
+-rw-rw-rw-   0        0        0     1961 2023-04-18 10:37:13.890665 kallisti-core-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1314 2023-04-11 05:58:30.000000 kallisti-core-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.475846 kallisti-core-1.3.6/kallisti_core.egg-info/
+-rw-rw-rw-   0        0        0     1961 2023-04-18 10:37:06.000000 kallisti-core-1.3.6/kallisti_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6493 2023-04-18 10:37:06.000000 kallisti-core-1.3.6/kallisti_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:37:06.000000 kallisti-core-1.3.6/kallisti_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      740 2023-04-18 10:37:06.000000 kallisti-core-1.3.6/kallisti_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 10:37:06.000000 kallisti-core-1.3.6/kallisti_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.648518 kallisti-core-1.3.6/kallisticore/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/apps.py
+-rw-rw-rw-   0        0        0     2340 2023-04-11 05:58:40.000000 kallisti-core-1.3.6/kallisticore/authentication.py
+-rw-rw-rw-   0        0        0     2823 2023-04-11 05:58:40.000000 kallisti-core-1.3.6/kallisticore/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.526209 kallisti-core-1.3.6/kallisticore/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:37.000000 kallisti-core-1.3.6/kallisticore/lib/__init__.py
+-rw-rw-rw-   0        0        0     6878 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/action.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.511927 kallisti-core-1.3.6/kallisticore/lib/authentication/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/authentication/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/authentication/jwt.py
+-rw-rw-rw-   0        0        0     2456 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/credential.py
+-rw-rw-rw-   0        0        0     5678 2023-04-11 05:58:37.000000 kallisti-core-1.3.6/kallisticore/lib/expectation.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.526141 kallisti-core-1.3.6/kallisticore/lib/observe/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/observe/__init__.py
+-rw-rw-rw-   0        0        0      254 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/observe/observer.py
+-rw-rw-rw-   0        0        0     1020 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/observe/subject.py
+-rw-rw-rw-   0        0        0     8431 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/lib/trial_executor.py
+-rw-rw-rw-   0        0        0     2051 2023-04-11 05:58:37.000000 kallisti-core-1.3.6/kallisticore/lib/trial_log_recorder.py
+-rw-rw-rw-   0        0        0      888 2023-04-11 05:58:37.000000 kallisti-core-1.3.6/kallisticore/lib/trial_scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.534474 kallisti-core-1.3.6/kallisticore/migrations/
+-rw-rw-rw-   0        0        0     1524 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      625 2023-04-11 05:58:34.000000 kallisti-core-1.3.6/kallisticore/migrations/0002_experiment_steps.py
+-rw-rw-rw-   0        0        0      462 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0003_trial_parameters.py
+-rw-rw-rw-   0        0        0      868 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/migrations/0004_auto_20190416_1800.py
+-rw-rw-rw-   0        0        0      603 2023-04-11 05:58:34.000000 kallisti-core-1.3.6/kallisticore/migrations/0005_trial_ticket.py
+-rw-rw-rw-   0        0        0      425 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0006_trial_initiated_by.py
+-rw-rw-rw-   0        0        0      424 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0007_trial_completed_at.py
+-rw-rw-rw-   0        0        0      461 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/migrations/0008_trial_records.py
+-rw-rw-rw-   0        0        0     1676 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0009_trialschedule.py
+-rw-rw-rw-   0        0        0      840 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/migrations/0010_auto_20190618_1356.py
+-rw-rw-rw-   0        0        0      434 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/migrations/0011_trialschedule_recurrence_left.py
+-rw-rw-rw-   0        0        0      748 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0012_auto_20190709_1827.py
+-rw-rw-rw-   0        0        0      662 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0013_notification.py
+-rw-rw-rw-   0        0        0      770 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0014_notification_seed.py
+-rw-rw-rw-   0        0        0      466 2023-04-11 05:58:34.000000 kallisti-core-1.3.6/kallisticore/migrations/0015_auto_20190906_1502.py
+-rw-rw-rw-   0        0        0      883 2023-04-11 05:58:34.000000 kallisti-core-1.3.6/kallisticore/migrations/0016_config.py
+-rw-rw-rw-   0        0        0      719 2023-04-11 05:58:34.000000 kallisti-core-1.3.6/kallisticore/migrations/0017_config_seed.py
+-rw-rw-rw-   0        0        0      309 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/0018_delete_config.py
+-rw-rw-rw-   0        0        0      410 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/migrations/0019_auto_20201230_1554.py
+-rw-rw-rw-   0        0        0      433 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/migrations/0020_trial_initiated_from.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.542247 kallisti-core-1.3.6/kallisticore/models/
+-rw-rw-rw-   0        0        0       90 2023-04-11 05:58:31.000000 kallisti-core-1.3.6/kallisticore/models/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-04-11 05:58:31.000000 kallisti-core-1.3.6/kallisticore/models/base_model.py
+-rw-rw-rw-   0        0        0     1487 2023-04-11 05:58:31.000000 kallisti-core-1.3.6/kallisticore/models/experiment.py
+-rw-rw-rw-   0        0        0      445 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/models/notification.py
+-rw-rw-rw-   0        0        0      190 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/models/singleton_manager.py
+-rw-rw-rw-   0        0        0      335 2023-04-11 05:58:31.000000 kallisti-core-1.3.6/kallisticore/models/singleton_model.py
+-rw-rw-rw-   0        0        0     3231 2023-04-11 05:58:31.000000 kallisti-core-1.3.6/kallisticore/models/step.py
+-rw-rw-rw-   0        0        0     5575 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/models/trial.py
+-rw-rw-rw-   0        0        0     3915 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/models/trial_schedule.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.620409 kallisti-core-1.3.6/kallisticore/modules/
+-rw-rw-rw-   0        0        0       57 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.563621 kallisti-core-1.3.6/kallisticore/modules/aws/
+-rw-rw-rw-   0        0        0       89 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/aws/__init__.py
+-rw-rw-rw-   0        0        0     1769 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/aws/aws_action.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.570138 kallisti-core-1.3.6/kallisticore/modules/cloud_foundry/
+-rw-rw-rw-   0        0        0     2077 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/cloud_foundry/__init__.py
+-rw-rw-rw-   0        0        0     2626 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/cloud_foundry/actions.py
+-rw-rw-rw-   0        0        0     1659 2023-04-11 05:58:39.000000 kallisti-core-1.3.6/kallisticore/modules/cloud_foundry/cloud_foundry_action.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.585874 kallisti-core-1.3.6/kallisticore/modules/common/
+-rw-rw-rw-   0        0        0     5534 2023-04-18 07:44:54.000000 kallisti-core-1.3.6/kallisticore/modules/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.606293 kallisti-core-1.3.6/kallisticore/modules/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:37.000000 kallisti-core-1.3.6/kallisticore/modules/examples/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/examples/sample_module1.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.606218 kallisti-core-1.3.6/kallisticore/modules/examples/sample_module2/
+-rw-rw-rw-   0        0        0      236 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/examples/sample_module2/__init__.py
+-rw-rw-rw-   0        0        0      228 2023-04-11 05:58:38.000000 kallisti-core-1.3.6/kallisticore/modules/examples/sample_module2/increment_action.py
+-rw-rw-rw-   0        0        0       65 2023-04-11 05:58:37.000000 kallisti-core-1.3.6/kallisticore/modules/examples/sample_module2/multiply_action.py
+-rw-rw-rw-   0        0        0       67 2023-04-11 05:58:37.000000 kallisti-core-1.3.6/kallisticore/modules/examples/sample_module2/subtract_action.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.613142 kallisti-core-1.3.6/kallisticore/modules/kubernetes/
+-rw-rw-rw-   0        0        0      977 2023-04-11 05:58:39.000000 kallisti-core-1.3.6/kallisticore/modules/kubernetes/__init__.py
+-rw-rw-rw-   0        0        0     5882 2023-04-11 05:58:39.000000 kallisti-core-1.3.6/kallisticore/modules/kubernetes/kubernetes_actions.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.620334 kallisti-core-1.3.6/kallisticore/modules/prometheus/
+-rw-rw-rw-   0        0        0      795 2023-04-11 05:58:40.000000 kallisti-core-1.3.6/kallisticore/modules/prometheus/__init__.py
+-rw-rw-rw-   0        0        0      172 2023-04-11 05:58:40.000000 kallisti-core-1.3.6/kallisticore/permissions.py
+-rw-rw-rw-   0        0        0     2448 2023-04-17 08:02:53.000000 kallisti-core-1.3.6/kallisticore/renderers.py
+-rw-rw-rw-   0        0        0     7071 2023-04-11 05:58:40.000000 kallisti-core-1.3.6/kallisticore/serializers.py
+-rw-rw-rw-   0        0        0      691 2023-04-11 05:58:30.000000 kallisti-core-1.3.6/kallisticore/signals.py
+-rw-rw-rw-   0        0        0      465 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/tasks.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.628884 kallisti-core-1.3.6/kallisticore/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.633210 kallisti-core-1.3.6/kallisticore/templates/kallisticore/
+-rw-rw-rw-   0        0        0    17748 2023-04-11 05:58:30.000000 kallisti-core-1.3.6/kallisticore/templates/kallisticore/xsl_template.xml
+-rw-rw-rw-   0        0        0     1045 2023-04-17 08:02:53.000000 kallisti-core-1.3.6/kallisticore/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.641373 kallisti-core-1.3.6/kallisticore/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/utils/__init__.py
+-rw-rw-rw-   0        0        0     2670 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/utils/fields.py
+-rw-rw-rw-   0        0        0     1976 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/utils/logging.py
+-rw-rw-rw-   0        0        0     1148 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/utils/pid_manager.py
+-rw-rw-rw-   0        0        0     1329 2023-04-11 05:58:33.000000 kallisti-core-1.3.6/kallisticore/utils/sanitizer.py
+-rw-rw-rw-   0        0        0      909 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/utils/singleton.py
+-rw-rw-rw-   0        0        0      314 2023-04-11 05:58:32.000000 kallisti-core-1.3.6/kallisticore/utils/threadlocals.py
+-rw-rw-rw-   0        0        0       19 2023-04-17 11:32:16.000000 kallisti-core-1.3.6/kallisticore/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.648450 kallisti-core-1.3.6/kallisticore/views/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/views/__init__.py
+-rw-rw-rw-   0        0        0     1261 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/views/experiment.py
+-rw-rw-rw-   0        0        0      839 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/views/notification.py
+-rw-rw-rw-   0        0        0     1601 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/views/report.py
+-rw-rw-rw-   0        0        0     1299 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/views/trial.py
+-rw-rw-rw-   0        0        0     1862 2023-04-11 05:58:36.000000 kallisti-core-1.3.6/kallisticore/views/trial_schedule.py
+-rw-rw-rw-   0        0        0     1278 2023-04-11 05:58:35.000000 kallisti-core-1.3.6/kallisticore/views/trial_stop.py
+-rw-rw-rw-   0        0        0      553 2023-04-11 05:58:29.000000 kallisti-core-1.3.6/manage.py
+-rw-rw-rw-   0        0        0       75 2023-04-11 05:58:29.000000 kallisti-core-1.3.6/requirements-dev.txt
+-rw-rw-rw-   0        0        0      731 2023-04-17 08:02:53.000000 kallisti-core-1.3.6/requirements.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 05:58:29.000000 kallisti-core-1.3.6/runtime.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:37:13.906856 kallisti-core-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1752 2023-04-17 08:02:53.000000 kallisti-core-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.660764 kallisti-core-1.3.6/tests/
+-rw-rw-rw-   0        0        0      146 2023-04-11 05:58:48.000000 kallisti-core-1.3.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.769245 kallisti-core-1.3.6/tests/kallisticore/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.684969 kallisti-core-1.3.6/tests/kallisticore/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.677858 kallisti-core-1.3.6/tests/kallisticore/lib/authentication/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/authentication/__init__.py
+-rw-rw-rw-   0        0        0     2555 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/authentication/test_jwt.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.684902 kallisti-core-1.3.6/tests/kallisticore/lib/observe/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/observe/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/observe/test_observer.py
+-rw-rw-rw-   0        0        0     1809 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/observe/test_subject.py
+-rw-rw-rw-   0        0        0    10604 2023-04-11 05:58:45.000000 kallisti-core-1.3.6/tests/kallisticore/lib/test_action.py
+-rw-rw-rw-   0        0        0     3111 2023-04-11 05:58:45.000000 kallisti-core-1.3.6/tests/kallisticore/lib/test_credential.py
+-rw-rw-rw-   0        0        0    11184 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/test_expectation.py
+-rw-rw-rw-   0        0        0    41902 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/test_trial_executor.py
+-rw-rw-rw-   0        0        0     8169 2023-04-11 05:58:46.000000 kallisti-core-1.3.6/tests/kallisticore/lib/test_trial_log_recorder.py
+-rw-rw-rw-   0        0        0     2573 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/lib/test_trial_scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.692751 kallisti-core-1.3.6/tests/kallisticore/models/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/models/__init__.py
+-rw-rw-rw-   0        0        0     4387 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/models/test_experiment.py
+-rw-rw-rw-   0        0        0      980 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/models/test_notification.py
+-rw-rw-rw-   0        0        0     4768 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/models/test_step.py
+-rw-rw-rw-   0        0        0    17797 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/models/test_trial.py
+-rw-rw-rw-   0        0        0    10086 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/models/test_trial_schedule.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.738905 kallisti-core-1.3.6/tests/kallisticore/modules/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.710332 kallisti-core-1.3.6/tests/kallisticore/modules/aws/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/aws/__init__.py
+-rw-rw-rw-   0        0        0     2282 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/aws/test_aws_action.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.716587 kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/__init__.py
+-rw-rw-rw-   0        0        0     5412 2023-04-11 05:58:43.000000 kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/test_actions.py
+-rw-rw-rw-   0        0        0     4205 2023-04-11 05:58:43.000000 kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/test_cloud_foundry_actions.py
+-rw-rw-rw-   0        0        0     2676 2023-04-11 05:58:43.000000 kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/test_get_user_organization_by_name.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.726244 kallisti-core-1.3.6/tests/kallisticore/modules/common/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/common/__init__.py
+-rw-rw-rw-   0        0        0    28696 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/common/test_common.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.732703 kallisti-core-1.3.6/tests/kallisticore/modules/kubernetes/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/kubernetes/__init__.py
+-rw-rw-rw-   0        0        0     9042 2023-04-11 05:58:42.000000 kallisti-core-1.3.6/tests/kallisticore/modules/kubernetes/test_kubernetes_action.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.738835 kallisti-core-1.3.6/tests/kallisticore/modules/prometheus/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/modules/prometheus/__init__.py
+-rw-rw-rw-   0        0        0     2093 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/modules/prometheus/test_prometheus_action.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.745151 kallisti-core-1.3.6/tests/kallisticore/renderers/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/renderers/__init__.py
+-rw-rw-rw-   0        0        0     2165 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/renderers/test_xml_renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.751224 kallisti-core-1.3.6/tests/kallisticore/serializers/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:43.000000 kallisti-core-1.3.6/tests/kallisticore/serializers/__init__.py
+-rw-rw-rw-   0        0        0     2112 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/serializers/test_experiment_serializer.py
+-rw-rw-rw-   0        0        0      680 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/serializers/test_notification_serializer.py
+-rw-rw-rw-   0        0        0     5784 2023-04-11 05:58:43.000000 kallisti-core-1.3.6/tests/kallisticore/serializers/test_report_serializer.py
+-rw-rw-rw-   0        0        0     2095 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/serializers/test_trial_schedule_serializer.py
+-rw-rw-rw-   0        0        0     2250 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/serializers/test_trial_serializer.py
+-rw-rw-rw-   0        0        0     3439 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/test_authentication.py
+-rw-rw-rw-   0        0        0     3476 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/test_exceptions.py
+-rw-rw-rw-   0        0        0      548 2023-04-11 05:58:47.000000 kallisti-core-1.3.6/tests/kallisticore/test_permissions.py
+-rw-rw-rw-   0        0        0     1714 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/test_signals.py
+-rw-rw-rw-   0        0        0     1009 2023-04-11 05:58:40.000000 kallisti-core-1.3.6/tests/kallisticore/test_tasks.py
+-rw-rw-rw-   0        0        0      191 2023-04-11 05:58:40.000000 kallisti-core-1.3.6/tests/kallisticore/test_urls.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.762864 kallisti-core-1.3.6/tests/kallisticore/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:45.000000 kallisti-core-1.3.6/tests/kallisticore/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.762798 kallisti-core-1.3.6/tests/kallisticore/utils/fixture/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/utils/fixture/__init__.py
+-rw-rw-rw-   0        0        0    14095 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/utils/fixture/trial_result_data.py
+-rw-rw-rw-   0        0        0     7847 2023-04-11 05:58:45.000000 kallisti-core-1.3.6/tests/kallisticore/utils/test_fields.py
+-rw-rw-rw-   0        0        0     2768 2023-04-11 05:58:45.000000 kallisti-core-1.3.6/tests/kallisticore/utils/test_logging.py
+-rw-rw-rw-   0        0        0     2968 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/utils/test_pid_manager.py
+-rw-rw-rw-   0        0        0      941 2023-04-11 05:58:44.000000 kallisti-core-1.3.6/tests/kallisticore/utils/test_sanitizer.py
+-rw-rw-rw-   0        0        0     1263 2023-04-11 05:58:45.000000 kallisti-core-1.3.6/tests/kallisticore/utils/test_singleton.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:37:06.769179 kallisti-core-1.3.6/tests/kallisticore/views/
+-rw-rw-rw-   0        0        0        0 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/views/__init__.py
+-rw-rw-rw-   0        0        0     6443 2023-04-17 08:02:53.000000 kallisti-core-1.3.6/tests/kallisticore/views/test_experiment.py
+-rw-rw-rw-   0        0        0     2054 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/views/test_notification.py
+-rw-rw-rw-   0        0        0     3932 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/views/test_report.py
+-rw-rw-rw-   0        0        0     3745 2023-04-11 05:58:41.000000 kallisti-core-1.3.6/tests/kallisticore/views/test_stop.py
+-rw-rw-rw-   0        0        0     7357 2023-04-17 08:02:53.000000 kallisti-core-1.3.6/tests/kallisticore/views/test_trial.py
+-rw-rw-rw-   0        0        0    10298 2023-04-17 12:29:49.000000 kallisti-core-1.3.6/tests/kallisticore/views/test_trial_schedule.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kallisti-core-1.3.5/kallisticore/authentication.py` & `kallisti-core-1.3.6/kallisticore/authentication.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/exceptions.py` & `kallisti-core-1.3.6/kallisticore/exceptions.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/action.py` & `kallisti-core-1.3.6/kallisticore/lib/action.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/authentication/jwt.py` & `kallisti-core-1.3.6/kallisticore/lib/authentication/jwt.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/credential.py` & `kallisti-core-1.3.6/kallisticore/lib/credential.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/expectation.py` & `kallisti-core-1.3.6/kallisticore/lib/expectation.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/observe/subject.py` & `kallisti-core-1.3.6/kallisticore/lib/observe/subject.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/trial_executor.py` & `kallisti-core-1.3.6/kallisticore/lib/trial_executor.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/trial_log_recorder.py` & `kallisti-core-1.3.6/kallisticore/lib/trial_log_recorder.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/lib/trial_scheduler.py` & `kallisti-core-1.3.6/kallisticore/lib/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0001_initial.py` & `kallisti-core-1.3.6/kallisticore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0002_experiment_steps.py` & `kallisti-core-1.3.6/kallisticore/migrations/0002_experiment_steps.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0004_auto_20190416_1800.py` & `kallisti-core-1.3.6/kallisticore/migrations/0004_auto_20190416_1800.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0005_trial_ticket.py` & `kallisti-core-1.3.6/kallisticore/migrations/0005_trial_ticket.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0009_trialschedule.py` & `kallisti-core-1.3.6/kallisticore/migrations/0009_trialschedule.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0010_auto_20190618_1356.py` & `kallisti-core-1.3.6/kallisticore/migrations/0010_auto_20190618_1356.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0012_auto_20190709_1827.py` & `kallisti-core-1.3.6/kallisticore/migrations/0012_auto_20190709_1827.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0013_notification.py` & `kallisti-core-1.3.6/kallisticore/migrations/0013_notification.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0014_notification_seed.py` & `kallisti-core-1.3.6/kallisticore/migrations/0014_notification_seed.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0016_config.py` & `kallisti-core-1.3.6/kallisticore/migrations/0016_config.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/migrations/0017_config_seed.py` & `kallisti-core-1.3.6/kallisticore/migrations/0017_config_seed.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/models/experiment.py` & `kallisti-core-1.3.6/kallisticore/models/experiment.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/models/step.py` & `kallisti-core-1.3.6/kallisticore/models/step.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/models/trial.py` & `kallisti-core-1.3.6/kallisticore/models/trial.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/models/trial_schedule.py` & `kallisti-core-1.3.6/kallisticore/models/trial_schedule.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/aws/aws_action.py` & `kallisti-core-1.3.6/kallisticore/modules/aws/aws_action.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/cloud_foundry/actions.py` & `kallisti-core-1.3.6/kallisticore/modules/cloud_foundry/actions.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/cloud_foundry/cloud_foundry_action.py` & `kallisti-core-1.3.6/kallisticore/modules/cloud_foundry/cloud_foundry_action.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/cloud_foundry/__init__.py` & `kallisti-core-1.3.6/kallisticore/modules/cloud_foundry/__init__.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/common/__init__.py` & `kallisti-core-1.3.6/kallisticore/modules/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/kubernetes/kubernetes_actions.py` & `kallisti-core-1.3.6/kallisticore/modules/kubernetes/kubernetes_actions.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/kubernetes/__init__.py` & `kallisti-core-1.3.6/kallisticore/modules/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/modules/prometheus/__init__.py` & `kallisti-core-1.3.6/kallisticore/modules/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/renderers.py` & `kallisti-core-1.3.6/kallisticore/renderers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import unicode_literals
 
 from django.conf import settings
 from django.template import loader
-from django.utils import six
-from django.utils.encoding import force_text
-from django.utils.six import StringIO
+import six
+from django.utils.encoding import force_str as force_text
+from six import StringIO
 from django.utils.xmlutils import SimplerXMLGenerator
 from rest_framework.renderers import BaseRenderer
 
 
 class XMLRenderer(BaseRenderer):
     """
     Renderer which serializes to XML.
```

### Comparing `kallisti-core-1.3.5/kallisticore/serializers.py` & `kallisti-core-1.3.6/kallisticore/serializers.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/signals.py` & `kallisti-core-1.3.6/kallisticore/signals.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/templates/kallisticore/xsl_template.xml` & `kallisti-core-1.3.6/kallisticore/templates/kallisticore/xsl_template.xml`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/urls.py` & `kallisti-core-1.3.6/kallisticore/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls import url, include
+from django.urls import re_path, include
 from rest_framework.routers import DefaultRouter
 
 from kallisticore.views.experiment import ExperimentViewSet
 from kallisticore.views.report import ReportAPI
 from kallisticore.views.trial import TrialViewSet
 from kallisticore.views.trial_schedule import TrialScheduleViewSet
 from kallisticore.views.trial_stop import TrialStopAPI
@@ -11,14 +11,14 @@
 router = DefaultRouter()
 router.register(r'experiment', ExperimentViewSet)
 router.register(r'trial', TrialViewSet)
 router.register(r'experiment/(?P<experiment_id>[-\w]+)/schedule',
                 TrialScheduleViewSet, 'trial-schedule')
 
 urlpatterns = [
-    url(r'^', include(router.urls)),
-    url(r'^report', ReportAPI.as_view(), name='report'),
-    url(r'^notification', NotificationViewSet.as_view(
+    re_path(r'^', include(router.urls)),
+    re_path(r'^report', ReportAPI.as_view(), name='report'),
+    re_path(r'^notification', NotificationViewSet.as_view(
         {'get': 'list', 'put': 'update'}), name='notification'),
-    url(r'trial/(?P<trial_id>[-\w]+)/stop', TrialStopAPI.as_view(),
-        name='trial-stop'),
+    re_path(r'trial/(?P<trial_id>[-\w]+)/stop', TrialStopAPI.as_view(),
+            name='trial-stop')
 ]
```

### Comparing `kallisti-core-1.3.5/kallisticore/utils/fields.py` & `kallisti-core-1.3.6/kallisticore/utils/fields.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/utils/logging.py` & `kallisti-core-1.3.6/kallisticore/utils/logging.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/utils/pid_manager.py` & `kallisti-core-1.3.6/kallisticore/utils/pid_manager.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/utils/sanitizer.py` & `kallisti-core-1.3.6/kallisticore/utils/sanitizer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/utils/singleton.py` & `kallisti-core-1.3.6/kallisticore/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/views/experiment.py` & `kallisti-core-1.3.6/kallisticore/views/experiment.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/views/notification.py` & `kallisti-core-1.3.6/kallisticore/views/notification.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/views/report.py` & `kallisti-core-1.3.6/kallisticore/views/report.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/views/trial.py` & `kallisti-core-1.3.6/kallisticore/views/trial.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/views/trial_schedule.py` & `kallisti-core-1.3.6/kallisticore/views/trial_schedule.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisticore/views/trial_stop.py` & `kallisti-core-1.3.6/kallisticore/views/trial_stop.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/kallisti_core.egg-info/PKG-INFO` & `kallisti-core-1.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kallisti-core
-Version: 1.3.5
+Version: 1.3.6
 Summary: Core functionality of Kallisti Chaos Engineering Framework
 Home-page: https://github.com/jpmorganchase/kallisti-core
 Author: The kallisti-core authors
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django :: 2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Kallisti Core
 
 ![Build Status](https://github.com/jpmorganchase/kallisti-core/actions/workflows/build.yml/badge.svg)
@@ -56,9 +55,7 @@
   the relevant issue number if applicable.
 * [Pull Contributor License Agreement (CLA)](https://github.com/jpmorganchase/cla)
   will be required upon PR before we are able to merge.
 
 If you have any questions about the contribution process, please feel free to
 send an email to open_source@jpmorgan.com.
  
-
-
```

### Comparing `kallisti-core-1.3.5/kallisti_core.egg-info/requires.txt` & `kallisti-core-1.3.6/kallisti_core.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 chaostoolkit-cloud-foundry<1.0.0,>=0.7.1
 chaostoolkit-istio<1.0.0,>=0.1.4
 chaostoolkit-kubernetes<1.0.0,>=0.24.0
 chaostoolkit-lib<1.0.0,>=0.22.2
 chaostoolkit-prometheus<1.0.0,>=0.3.0
 chaostoolkit-spring<1.0.0,<=0.2.0
 croniter==0.3.29
-django~=2.2.0
-django-cors-headers==3.1.1
-djangorestframework~=3.11.2
-drf-yasg~=1.20.0
+Django==4.1.7
+django-cors-headers==3.13.0
+djangorestframework==3.14.0
+drf-yasg==1.21.5
 gunicorn==20.0.4
 huey~=2.3.0
 jinja2==2.11.3
 jsonpath-ng==1.4.3
 MarkupSafe==2.0.1
 mysql-connector-python~=8.0.0
 peewee==3.9.3
 pycryptodome~=3.10.0
 python-daemon==2.1.2
 python-jose[pycryptodome]~=3.3.0
 python-logstash==0.4.6
 requests~=2.26.0
 snaptime==0.2.4
 urllib3==1.26.5
+django-utils-six==2.0
 
 [test]
 bump2version==1.0.1
 flake8~=4.0.0
 coverage~=6.0.0
 requests-mock==1.8.0
```

### Comparing `kallisti-core-1.3.5/kallisti_core.egg-info/SOURCES.txt` & `kallisti-core-1.3.6/kallisti_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 manage.py
 requirements-dev.txt
 requirements.txt
+runtime.txt
 setup.py
 kallisti_core.egg-info/PKG-INFO
 kallisti_core.egg-info/SOURCES.txt
 kallisti_core.egg-info/dependency_links.txt
 kallisti_core.egg-info/requires.txt
 kallisti_core.egg-info/top_level.txt
 kallisticore/__init__.py
```

### Comparing `kallisti-core-1.3.5/LICENSE` & `kallisti-core-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/Makefile` & `kallisti-core-1.3.6/Makefile`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/manage.py` & `kallisti-core-1.3.6/manage.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/PKG-INFO` & `kallisti-core-1.3.6/kallisti_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kallisti-core
-Version: 1.3.5
+Version: 1.3.6
 Summary: Core functionality of Kallisti Chaos Engineering Framework
 Home-page: https://github.com/jpmorganchase/kallisti-core
 Author: The kallisti-core authors
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django :: 2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Kallisti Core
 
 ![Build Status](https://github.com/jpmorganchase/kallisti-core/actions/workflows/build.yml/badge.svg)
@@ -56,9 +55,7 @@
   the relevant issue number if applicable.
 * [Pull Contributor License Agreement (CLA)](https://github.com/jpmorganchase/cla)
   will be required upon PR before we are able to merge.
 
 If you have any questions about the contribution process, please feel free to
 send an email to open_source@jpmorgan.com.
  
-
-
```

### Comparing `kallisti-core-1.3.5/README.md` & `kallisti-core-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/requirements.txt` & `kallisti-core-1.3.6/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 chaostoolkit-cloud-foundry>=0.7.1,<1.0.0
 chaostoolkit-istio>=0.1.4,<1.0.0
 chaostoolkit-kubernetes>=0.24.0,<1.0.0
 chaostoolkit-lib>=0.22.2,<1.0.0
 chaostoolkit-prometheus>=0.3.0,<1.0.0
 chaostoolkit-spring<=0.2.0,<1.0.0
 croniter==0.3.29
-django~=2.2.0
-django-cors-headers==3.1.1
-djangorestframework~=3.11.2
-drf-yasg~=1.20.0
+Django==4.1.7
+django-cors-headers==3.13.0
+djangorestframework==3.14.0
+drf-yasg==1.21.5
 gunicorn==20.0.4
 huey~=2.3.0
 jinja2==2.11.3
 jsonpath-ng==1.4.3
 MarkupSafe==2.0.1  # 2.1.0 is incompatible with jinja2 2.11.3
 mysql-connector-python~=8.0.0
 peewee==3.9.3
 pycryptodome~=3.10.0
 python-daemon==2.1.2
 python-jose[pycryptodome]~=3.3.0
 python-logstash==0.4.6
 requests~=2.26.0
 snaptime==0.2.4
 urllib3==1.26.5
+django-utils-six==2.0
```

### Comparing `kallisti-core-1.3.5/setup.py` & `kallisti-core-1.3.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,11 +46,11 @@
     classifiers=(
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Framework :: Django :: 2.0',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.10'
     ),
     include_package_data=True
 )
```

### Comparing `kallisti-core-1.3.5/tests/kallisticore/base.py` & `kallisti-core-1.3.6/tests/kallisticore/base.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/authentication/test_jwt.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/authentication/test_jwt.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/observe/test_observer.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/observe/test_observer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/observe/test_subject.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/observe/test_subject.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/test_action.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/test_action.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/test_credential.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/test_credential.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/test_expectation.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/test_expectation.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/test_trial_executor.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/test_trial_executor.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/test_trial_log_recorder.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/test_trial_log_recorder.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/lib/test_trial_scheduler.py` & `kallisti-core-1.3.6/tests/kallisticore/lib/test_trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/models/test_experiment.py` & `kallisti-core-1.3.6/tests/kallisticore/models/test_experiment.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/models/test_notification.py` & `kallisti-core-1.3.6/tests/kallisticore/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/models/test_step.py` & `kallisti-core-1.3.6/tests/kallisticore/models/test_step.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/models/test_trial.py` & `kallisti-core-1.3.6/tests/kallisticore/models/test_trial.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/models/test_trial_schedule.py` & `kallisti-core-1.3.6/tests/kallisticore/models/test_trial_schedule.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/modules/aws/test_aws_action.py` & `kallisti-core-1.3.6/tests/kallisticore/modules/aws/test_aws_action.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/test_actions.py` & `kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/test_actions.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/test_cloud_foundry_actions.py` & `kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/test_cloud_foundry_actions.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/modules/cloud_foundry/test_get_user_organization_by_name.py` & `kallisti-core-1.3.6/tests/kallisticore/modules/cloud_foundry/test_get_user_organization_by_name.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/modules/common/test_common.py` & `kallisti-core-1.3.6/tests/kallisticore/modules/common/test_common.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/modules/kubernetes/test_kubernetes_action.py` & `kallisti-core-1.3.6/tests/kallisticore/modules/kubernetes/test_kubernetes_action.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/modules/prometheus/test_prometheus_action.py` & `kallisti-core-1.3.6/tests/kallisticore/modules/prometheus/test_prometheus_action.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/renderers/test_xml_renderer.py` & `kallisti-core-1.3.6/tests/kallisticore/renderers/test_xml_renderer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/serializers/test_experiment_serializer.py` & `kallisti-core-1.3.6/tests/kallisticore/serializers/test_experiment_serializer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/serializers/test_notification_serializer.py` & `kallisti-core-1.3.6/tests/kallisticore/serializers/test_notification_serializer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/serializers/test_report_serializer.py` & `kallisti-core-1.3.6/tests/kallisticore/serializers/test_report_serializer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/serializers/test_trial_schedule_serializer.py` & `kallisti-core-1.3.6/tests/kallisticore/serializers/test_trial_schedule_serializer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/serializers/test_trial_serializer.py` & `kallisti-core-1.3.6/tests/kallisticore/serializers/test_trial_serializer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/test_authentication.py` & `kallisti-core-1.3.6/tests/kallisticore/test_authentication.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/test_exceptions.py` & `kallisti-core-1.3.6/tests/kallisticore/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/test_permissions.py` & `kallisti-core-1.3.6/tests/kallisticore/test_permissions.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/test_signals.py` & `kallisti-core-1.3.6/tests/kallisticore/test_signals.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/test_tasks.py` & `kallisti-core-1.3.6/tests/kallisticore/test_tasks.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/utils/fixture/trial_result_data.py` & `kallisti-core-1.3.6/tests/kallisticore/utils/fixture/trial_result_data.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/utils/test_fields.py` & `kallisti-core-1.3.6/tests/kallisticore/utils/test_fields.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/utils/test_logging.py` & `kallisti-core-1.3.6/tests/kallisticore/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/utils/test_pid_manager.py` & `kallisti-core-1.3.6/tests/kallisticore/utils/test_pid_manager.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/utils/test_sanitizer.py` & `kallisti-core-1.3.6/tests/kallisticore/utils/test_sanitizer.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/utils/test_singleton.py` & `kallisti-core-1.3.6/tests/kallisticore/utils/test_singleton.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/views/test_experiment.py` & `kallisti-core-1.3.6/tests/kallisticore/views/test_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.urls import reverse
 from kallisticore.models.experiment import Experiment
 from kallisticore.serializers import ExperimentSerializer
 from rest_framework import status
 from tests.kallisticore.base import KallistiTestSuite
+from uuid import uuid4
 
 
 class TestExperimentListAPI(KallistiTestSuite):
 
     def setUp(self):
         super(TestExperimentListAPI, self).setUp()
         self._token = '123123123123123'
@@ -39,22 +40,23 @@
         self.assertIn(ExperimentSerializer(experiment2).data, response_data)
 
 
 class TestExperimentGetAPI(KallistiTestSuite):
     def setUp(self):
         super(TestExperimentGetAPI, self).setUp()
         self._token = '123123123123123'
+        self._non_existent = uuid4()
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
 
     def tearDown(self):
         self.client.credentials()
         super(TestExperimentGetAPI, self).tearDown()
 
     def test_get_details_with_invalid_id(self):
-        url = reverse('experiment-detail', args=['non-existent'])
+        url = reverse('experiment-detail', args=[self._non_existent])
         response = self.client.get(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
         self.assertEqual(response.data, {'detail': 'Not found.'})
 
     def test_get_details(self):
         experiment = Experiment.create(
@@ -98,22 +100,23 @@
         self.assertEqual(Experiment.objects.count(), 0)
 
 
 class TestExperimentDeleteAPI(KallistiTestSuite):
     def setUp(self):
         super(TestExperimentDeleteAPI, self).setUp()
         self._token = '123123123123123'
+        self._non_existent = uuid4()
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
 
     def tearDown(self):
         self.client.credentials()
         super(TestExperimentDeleteAPI, self).tearDown()
 
     def test_delete_with_invalid_id(self):
-        url = reverse('experiment-detail', args=['non-existent'])
+        url = reverse('experiment-detail', args=[self._non_existent])
         response = self.client.delete(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
         self.assertEqual(response.data, {'detail': 'Not found.'})
 
     def test_delete(self):
         experiment = Experiment.create(
@@ -129,22 +132,23 @@
 class TestExperimentPatchAPI(KallistiTestSuite):
     def setUp(self):
         super(TestExperimentPatchAPI, self).setUp()
         self._data = {'description': 'This experiment would prove go '
                                      'redirection would be resilient to DB '
                                      'failures'}
         self._token = '123123123123123'
+        self._non_existent = uuid4()
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
 
     def tearDown(self):
         self.client.credentials()
         super(TestExperimentPatchAPI, self).tearDown()
 
     def test_patch_with_invalid_id(self):
-        url = reverse('experiment-detail', args=['non-existent'])
+        url = reverse('experiment-detail', args=[self._non_existent])
         response = self.client.patch(url, data=self._data, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
         self.assertEqual(response.data, {'detail': 'Not found.'})
 
     def test_patch(self):
         experiment = Experiment.create(
```

### Comparing `kallisti-core-1.3.5/tests/kallisticore/views/test_notification.py` & `kallisti-core-1.3.6/tests/kallisticore/views/test_notification.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/views/test_report.py` & `kallisti-core-1.3.6/tests/kallisticore/views/test_report.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/views/test_stop.py` & `kallisti-core-1.3.6/tests/kallisticore/views/test_stop.py`

 * *Files identical despite different names*

### Comparing `kallisti-core-1.3.5/tests/kallisticore/views/test_trial.py` & `kallisti-core-1.3.6/tests/kallisticore/views/test_trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from kallisticore import signals
 from kallisticore.authentication import KallistiUser
 from kallisticore.models import Experiment, Trial
 from kallisticore.models.step import Step
 from kallisticore.serializers import TrialSerializer
 from kallisticore.signals import execute_plan_for_trial
 from tests.kallisticore.base import KallistiTestSuite
+from uuid import uuid4
 
 
 class TestTrialListAPI(KallistiTestSuite):
 
     def setUp(self):
         self._token = '123123123123123'
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
@@ -76,15 +77,15 @@
 
 
 class TestTrialGetAPI(KallistiTestSuite):
 
     def setUp(self):
         self._token = '123123123123123'
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
-
+        self.notexists = uuid4()
         self.parameters = {"org": "MY-ORG",
                            "app_name": "hello-world"}
         self.steps = [{"step": "name",
                        "do": "cf.stop_app",
                        "where": {"app_name": "{{app_name}}",
                                  "org_name": "{{org}}"}}]
         self.post_steps = [{"step": "name",
@@ -113,15 +114,15 @@
         response = self.client.get(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         response_data = response.data
         self.assertEqual(TrialSerializer(trial).data, response_data)
 
     def test_get_non_existing_trial(self):
-        url = reverse('trial-detail', args=['notexists'])
+        url = reverse('trial-detail', args=[self.notexists])
         response = self.client.get(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
         self.assertEqual(response.data, {'detail': 'Not found.'})
 
     @mock.patch.object(kallisticore.authentication.DefaultAuthentication,
                        "authenticate",
```

### Comparing `kallisti-core-1.3.5/tests/kallisticore/views/test_trial_schedule.py` & `kallisti-core-1.3.6/tests/kallisticore/views/test_trial_schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.urls import reverse
 from kallisticore.models import Experiment
 from kallisticore.models.trial_schedule import TrialSchedule
 from kallisticore.serializers import TrialScheduleSerializer
 from rest_framework import status
 from tests.kallisticore.base import KallistiTestSuite
+from uuid import uuid4
 
 
 class TestTrialScheduleListAPI(KallistiTestSuite):
 
     def setUp(self):
         self._token = 'test-token'
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
@@ -60,38 +61,40 @@
 
 
 class TestTrialScheduleDetailAPI(KallistiTestSuite):
 
     def setUp(self):
         self._token = '123123123123123'
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
-
+        self._non_existing_pk = uuid4()
+        self._non_existing_experiment_id = uuid4()
         self._experiment = Experiment.create()
         super(TestTrialScheduleDetailAPI, self).setUp()
 
     def tearDown(self):
         self.client.credentials()
         super(TestTrialScheduleDetailAPI, self).tearDown()
 
     def test_detail_with_non_existing_pk(self):
         url = reverse('trial-schedule-detail',
                       kwargs={'experiment_id': self._experiment.id,
-                              'pk': 'non-existing-pk'})
+                              'pk': self._non_existing_pk})
         response = self.client.get(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
     def test_detail_with_non_existing_experiment_id(self):
         trial_schedule = TrialSchedule.create(
             experiment=self._experiment,
             recurrence_pattern='* * * * *'
         )
         url = reverse('trial-schedule-detail',
-                      kwargs={'experiment_id': 'non-existing-experiment-id',
-                              'pk': trial_schedule.id})
+                      kwargs={
+                        'experiment_id': self._non_existing_experiment_id,
+                        'pk': trial_schedule.id})
         response = self.client.get(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
     def test_detail_entry(self):
         trial_schedule = TrialSchedule.create(
             experiment=self._experiment,
@@ -177,14 +180,16 @@
         self.assertEqual(TrialSchedule.objects.count(), 0)
 
 
 class TestTrialScheduleDeleteAPI(KallistiTestSuite):
     def setUp(self):
         super(TestTrialScheduleDeleteAPI, self).setUp()
         self._token = '123123123123123'
+        self._non_existing_id = uuid4()
+        self._non_existing_pk = uuid4()
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
 
     def tearDown(self):
         self.client.credentials()
         super(TestTrialScheduleDeleteAPI, self).tearDown()
 
     def test_delete(self):
@@ -198,37 +203,39 @@
         response = self.client.delete(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
         self.assertEqual(TrialSchedule.objects.count(), 0)
 
     def test_delete_with_invalid_id(self):
         url = reverse('trial-schedule-detail',
-                      kwargs={'experiment_id': 'non-existing-id',
-                              'pk': 'non-existing-pk'})
+                      kwargs={'experiment_id': self._non_existing_id,
+                              'pk': self._non_existing_pk})
         response = self.client.delete(url, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
         self.assertEqual(response.data, {'detail': 'Not found.'})
 
 
 class TestTrialSchedulePatchAPI(KallistiTestSuite):
     def setUp(self):
         super(TestTrialSchedulePatchAPI, self).setUp()
         self._token = '123123123123123'
+        self._non_existing_id = uuid4()
+        self._non_existing_pk = uuid4()
         self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + self._token)
         self._data = {'recurrence_pattern': '5 * * * *'}
 
     def tearDown(self):
         self.client.credentials()
         super(TestTrialSchedulePatchAPI, self).tearDown()
 
     def test_patch_with_invalid_id(self):
         url = reverse('trial-schedule-detail',
-                      kwargs={'experiment_id': 'non-existing-id',
-                              'pk': 'non-existing-pk'})
+                      kwargs={'experiment_id': self._non_existing_id,
+                              'pk': self._non_existing_pk})
         response = self.client.patch(url, data=self._data, format='json')
 
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
         self.assertEqual(response.data, {'detail': 'Not found.'})
 
     def test_patch(self):
         experiment = Experiment.create()
```

