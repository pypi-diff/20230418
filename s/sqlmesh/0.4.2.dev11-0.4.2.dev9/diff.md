# Comparing `tmp/sqlmesh-0.4.2.dev11.tar.gz` & `tmp/sqlmesh-0.4.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.4.2.dev11.tar", last modified: Tue Apr 18 05:42:03 2023, max compression
+gzip compressed data, was "sqlmesh-0.4.2.dev9.tar", last modified: Tue Apr 18 04:12:59 2023, max compression
```

## Comparing `sqlmesh-0.4.2.dev11.tar` & `sqlmesh-0.4.2.dev9.tar`

### file list

```diff
@@ -1,692 +1,692 @@
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.705602 sqlmesh-0.4.2.dev11/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.627584 sqlmesh-0.4.2.dev11/.circleci/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1872 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/.circleci/config.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)     4414 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/.circleci/continue_config.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       66 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/.dockerignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     2152 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     1900 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/.pre-commit-config.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      234 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/.readthedocs.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      135 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev11/Dockerfile.api
--rw-r--r--   0 izeigerman   (501) staff       (20)      383 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/Dockerfile.app
--rw-r--r--   0 izeigerman   (501) staff       (20)    11346 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/LICENSE
--rw-r--r--   0 izeigerman   (501) staff       (20)     1855 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/Makefile
--rw-r--r--   0 izeigerman   (501) staff       (20)     2012 2023-04-18 05:42:03.705689 sqlmesh-0.4.2.dev11/PKG-INFO
--rw-r--r--   0 izeigerman   (501) staff       (20)     1250 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/README.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1008 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docker-compose.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.628708 sqlmesh-0.4.2.dev11/docs/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.614017 sqlmesh-0.4.2.dev11/docs/_readthedocs/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.628847 sqlmesh-0.4.2.dev11/docs/_readthedocs/html/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/docs/_readthedocs/html/.keep
--rw-r--r--   0 izeigerman   (501) staff       (20)     9981 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docs/comparisons.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.629965 sqlmesh-0.4.2.dev11/docs/concepts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.630195 sqlmesh-0.4.2.dev11/docs/concepts/architecture/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1334 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/architecture/serialization.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1113 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     6693 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/docs/concepts/audits.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/environments.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5914 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/glossary.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       13 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/hooks.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     3027 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/macros.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.630781 sqlmesh-0.4.2.dev11/docs/concepts/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     9934 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/models/model_kinds.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7454 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/models/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/models/python_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     4938 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/models/seed_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5356 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/models/sql_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     6631 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/overview.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.630901 sqlmesh-0.4.2.dev11/docs/concepts/plans/
--rw-r--r--   0 izeigerman   (501) staff       (20)    43124 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 izeigerman   (501) staff       (20)     8981 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/plans.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       37 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/concepts/team_development.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5699 2023-02-27 20:36:43.000000 sqlmesh-0.4.2.dev11/docs/concepts/tests.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      607 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev11/docs/development.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.631507 sqlmesh-0.4.2.dev11/docs/guides/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docs/guides/connections.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    10756 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docs/guides/models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     2136 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docs/guides/projects.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.632145 sqlmesh-0.4.2.dev11/docs/guides/scheduling/
--rw-r--r--   0 izeigerman   (501) staff       (20)   740917 2023-02-24 17:54:11.000000 sqlmesh-0.4.2.dev11/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   379880 2023-02-24 17:54:11.000000 sqlmesh-0.4.2.dev11/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 izeigerman   (501) staff       (20)     5648 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/guides/scheduling.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1854 2023-02-27 20:36:43.000000 sqlmesh-0.4.2.dev11/docs/guides/testing.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5510 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/docs/index.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      290 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev11/docs/installation.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.632961 sqlmesh-0.4.2.dev11/docs/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2905 2023-04-03 17:47:07.000000 sqlmesh-0.4.2.dev11/docs/integrations/airflow.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7309 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docs/integrations/dbt.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    20383 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docs/integrations/engines.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      926 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/integrations/github.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      217 2023-03-25 06:07:32.000000 sqlmesh-0.4.2.dev11/docs/integrations/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      665 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev11/docs/prerequisites.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    10774 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/docs/quick_start.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.633540 sqlmesh-0.4.2.dev11/docs/reference/
--rw-r--r--   0 izeigerman   (501) staff       (20)     5816 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/reference/cli.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    13240 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/reference/configuration.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     4091 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/reference/notebook.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1127 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/reference/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       14 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/reference/python.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       16 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/docs/release_notes.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      122 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/docs/requirements.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)     3249 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/docs/sqlmesh.png
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.633656 sqlmesh-0.4.2.dev11/examples/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.634356 sqlmesh-0.4.2.dev11/examples/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1713 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev11/examples/airflow/Dockerfile.template
--rw-r--r--   0 izeigerman   (501) staff       (20)     2164 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev11/examples/airflow/Makefile
--rw-r--r--   0 izeigerman   (501) staff       (20)      942 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev11/examples/airflow/README.md
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.4.2.dev11/examples/airflow/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.634500 sqlmesh-0.4.2.dev11/examples/airflow/dags/
--rw-r--r--   0 izeigerman   (501) staff       (20)      263 2023-03-09 17:15:39.000000 sqlmesh-0.4.2.dev11/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3515 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev11/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev11/examples/airflow/requirements.txt
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.634795 sqlmesh-0.4.2.dev11/examples/airflow/spark_conf/
--rw-r--r--   0 izeigerman   (501) staff       (20)      872 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev11/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 izeigerman   (501) staff       (20)      151 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev11/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.635152 sqlmesh-0.4.2.dev11/examples/sushi/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.635462 sqlmesh-0.4.2.dev11/examples/sushi/audits/
--rw-r--r--   0 izeigerman   (501) staff       (20)      105 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/audits/items.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      119 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/audits/order_items.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      829 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi/config.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.635638 sqlmesh-0.4.2.dev11/examples/sushi/data/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi/data/.keep
--rw-r--r--   0 izeigerman   (501) staff       (20)      551 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/helper.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.635937 sqlmesh-0.4.2.dev11/examples/sushi/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/hooks/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.636252 sqlmesh-0.4.2.dev11/examples/sushi/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/macros/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      702 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/macros/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.637636 sqlmesh-0.4.2.dev11/examples/sushi/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)      913 2023-03-13 20:04:07.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      204 2023-03-03 17:17:44.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     1914 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/items.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1892 2023-03-13 20:04:07.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/order_items.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1646 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/orders.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      346 2023-03-25 04:59:10.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      465 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      123 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-04-18 05:41:42.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      197 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.637763 sqlmesh-0.4.2.dev11/examples/sushi/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-03-24 20:49:46.000000 sqlmesh-0.4.2.dev11/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.637892 sqlmesh-0.4.2.dev11/examples/sushi/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1459 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev11/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.638675 sqlmesh-0.4.2.dev11/examples/sushi_dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)       15 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/.user.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.638984 sqlmesh-0.4.2.dev11/examples/sushi_dbt/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-14 18:30:53.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      507 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.639264 sqlmesh-0.4.2.dev11/examples/sushi_dbt/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-03-03 23:53:25.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-02-28 16:05:24.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.640173 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1125 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      182 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      309 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      752 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      186 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.615733 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.640296 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.640417 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.640652 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.640777 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.640883 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.641013 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.641118 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      783 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.641763 sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)       97 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.641913 sqlmesh-0.4.2.dev11/examples/sushi_dbt/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.642042 sqlmesh-0.4.2.dev11/examples/sushi_dbt/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev11/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.642301 sqlmesh-0.4.2.dev11/examples/wursthall/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.616549 sqlmesh-0.4.2.dev11/examples/wursthall/audits/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.642450 sqlmesh-0.4.2.dev11/examples/wursthall/audits/db/
--rw-r--r--   0 izeigerman   (501) staff       (20)      141 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev11/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       66 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/config.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.642767 sqlmesh-0.4.2.dev11/examples/wursthall/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/macros/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      618 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.642932 sqlmesh-0.4.2.dev11/examples/wursthall/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.643502 sqlmesh-0.4.2.dev11/examples/wursthall/models/db/
--rw-r--r--   0 izeigerman   (501) staff       (20)      428 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      256 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     3145 2023-02-16 23:39:50.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      537 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.644100 sqlmesh-0.4.2.dev11/examples/wursthall/models/src/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1667 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      120 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     3419 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      892 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.616966 sqlmesh-0.4.2.dev11/examples/wursthall/seeds/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.644225 sqlmesh-0.4.2.dev11/examples/wursthall/seeds/src/
--rw-r--r--   0 izeigerman   (501) staff       (20)     7416 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev11/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.644527 sqlmesh-0.4.2.dev11/examples/wursthall/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-02-20 22:54:27.000000 sqlmesh-0.4.2.dev11/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      955 2023-02-20 22:54:27.000000 sqlmesh-0.4.2.dev11/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)     2094 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/mkdocs.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.644660 sqlmesh-0.4.2.dev11/pdoc/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)     1153 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev11/pdoc/cli.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.644786 sqlmesh-0.4.2.dev11/pdoc/templates/
--rw-r--r--   0 izeigerman   (501) staff       (20)      131 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.644932 sqlmesh-0.4.2.dev11/posts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.646504 sqlmesh-0.4.2.dev11/posts/virtual_environments/
--rw-r--r--   0 izeigerman   (501) staff       (20)   318753 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/posts/virtual_environments/change_categorization.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   274526 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/posts/virtual_environments/isolated_rigid_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   163619 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/posts/virtual_environments/partial_breaking.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   298971 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/posts/virtual_environments/stateful_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   366545 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/posts/virtual_environments/virtual_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)  1344487 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/posts/virtual_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 izeigerman   (501) staff       (20)    18666 2023-04-17 20:22:17.000000 sqlmesh-0.4.2.dev11/posts/virtual_environments.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      734 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/pytest.ini
--rw-r--r--   0 izeigerman   (501) staff       (20)     1344 2023-04-18 05:42:03.706228 sqlmesh-0.4.2.dev11/setup.cfg
--rw-r--r--   0 izeigerman   (501) staff       (20)     3056 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/setup.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.647801 sqlmesh-0.4.2.dev11/sqlmesh/
--rw-r--r--   0 izeigerman   (501) staff       (20)        3 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/.airflowignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     3676 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      175 2023-04-18 05:42:03.000000 sqlmesh-0.4.2.dev11/sqlmesh/_version.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.649005 sqlmesh-0.4.2.dev11/sqlmesh/cli/
--rw-r--r--   0 izeigerman   (501) staff       (20)      821 2023-04-18 04:08:49.000000 sqlmesh-0.4.2.dev11/sqlmesh/cli/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4314 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/cli/example_project.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8938 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/cli/main.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1391 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev11/sqlmesh/cli/options.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.651455 sqlmesh-0.4.2.dev11/sqlmesh/core/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      586 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/_typing.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.651837 sqlmesh-0.4.2.dev11/sqlmesh/core/audit/
--rw-r--r--   0 izeigerman   (501) staff       (20)      449 2023-01-27 03:51:22.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1071 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8136 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.652925 sqlmesh-0.4.2.dev11/sqlmesh/core/config/
--rw-r--r--   0 izeigerman   (501) staff       (20)      638 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1001 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      940 2023-02-08 20:28:46.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18770 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/connection.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3355 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1655 2023-02-08 20:28:46.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5389 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/root.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8432 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    29242 2023-04-18 04:18:48.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/console.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      731 2023-03-16 20:42:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/constants.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    34133 2023-04-18 02:26:32.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8612 2023-03-10 17:30:08.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/context_diff.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    17626 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/dialect.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.654703 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2390 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      762 2023-01-18 00:01:51.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    28278 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4238 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10243 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      393 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1930 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1971 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1398 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7713 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1181 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2658 2023-03-01 00:12:50.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3678 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1815 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/environment.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      742 2023-02-09 01:00:20.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/hooks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9362 2023-03-08 20:46:19.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18920 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.655655 sqlmesh-0.4.2.dev11/sqlmesh/core/model/
--rw-r--r--   0 izeigerman   (501) staff       (20)      546 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1498 2023-04-17 22:52:49.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/cache.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1300 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2417 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/decorator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    47553 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7382 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/kind.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12622 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/meta.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2017 2023-03-15 19:25:00.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/model/seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2314 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.656003 sqlmesh-0.4.2.dev11/sqlmesh/core/plan/
--rw-r--r--   0 izeigerman   (501) staff       (20)      191 2022-12-27 15:59:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    24670 2023-04-18 04:18:48.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/plan/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8075 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12174 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/renderer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15386 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    19427 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.656472 sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/
--rw-r--r--   0 izeigerman   (501) staff       (20)      527 2023-02-13 20:33:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    31370 2023-04-18 04:39:17.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18706 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.657037 sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/
--rw-r--r--   0 izeigerman   (501) staff       (20)      692 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13080 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12222 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    19996 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12062 2023-04-18 02:26:32.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/test.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1412 2022-12-24 00:00:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/core/user.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.659139 sqlmesh-0.4.2.dev11/sqlmesh/dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)       79 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15639 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    11330 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/builtin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1969 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/column.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9663 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3229 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12410 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/package.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3530 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/profile.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/project.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1049 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3145 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/source.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    11118 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/target.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-02 18:36:40.000000 sqlmesh-0.4.2.dev11/sqlmesh/dbt/util.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.659399 sqlmesh-0.4.2.dev11/sqlmesh/engines/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/engines/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4437 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/engines/commands.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.659690 sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3414 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.660102 sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      148 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2571 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.660229 sqlmesh-0.4.2.dev11/sqlmesh/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.660737 sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2210 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1726 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1829 2023-01-18 20:54:37.000000 sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13153 2023-03-15 19:24:58.000000 sqlmesh-0.4.2.dev11/sqlmesh/magics.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.660993 sqlmesh-0.4.2.dev11/sqlmesh/migrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/migrations/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1749 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/py.typed
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.661108 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.662247 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-04 00:12:26.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4020 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3830 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18799 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.662570 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-16 21:08:59.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2132 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      868 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8508 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.663578 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1341 2023-01-18 20:54:37.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6307 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2549 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      877 2023-01-31 17:31:24.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1211 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1340 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5222 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10922 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4400 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1292 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4139 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5006 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.665514 sqlmesh-0.4.2.dev11/sqlmesh/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4326 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/concurrency.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7530 2023-02-14 22:10:01.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      410 2022-12-30 16:25:50.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/conversions.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4329 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/dag.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7549 2023-04-18 02:34:51.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/date.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1244 2023-02-04 22:32:08.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/errors.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15925 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/jinja.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15093 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/pandas.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1609 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/pydantic.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1534 2023-01-25 18:09:57.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/rich.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6166 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1301 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev11/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.648473 sqlmesh-0.4.2.dev11/sqlmesh.egg-info/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2012 2023-04-18 05:42:03.000000 sqlmesh-0.4.2.dev11/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 izeigerman   (501) staff       (20)    20173 2023-04-18 05:42:03.000000 sqlmesh-0.4.2.dev11/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)        1 2023-04-18 05:42:03.000000 sqlmesh-0.4.2.dev11/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)      142 2023-04-18 05:42:03.000000 sqlmesh-0.4.2.dev11/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)      787 2023-04-18 05:42:03.000000 sqlmesh-0.4.2.dev11/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-04-18 05:42:03.000000 sqlmesh-0.4.2.dev11/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)    21020 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/sqlmesh.svg
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.665940 sqlmesh-0.4.2.dev11/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      285 2023-02-07 17:58:48.000000 sqlmesh-0.4.2.dev11/tests/common_fixtures.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3773 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/conftest.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.668689 sqlmesh-0.4.2.dev11/tests/core/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/core/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.669766 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    27289 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1298 2023-02-07 16:29:13.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1281 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2613 2023-02-14 20:17:36.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7155 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3245 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7073 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/tests/core/test_audit.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6611 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/tests/core/test_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      850 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/core/test_connection_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10703 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/core/test_context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2749 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev11/tests/core/test_dialect.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      464 2022-12-28 17:42:44.000000 sqlmesh-0.4.2.dev11/tests/core/test_environment.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    25987 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/core/test_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5760 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/tests/core/test_macros.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    24586 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/core/test_model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15859 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/tests/core/test_plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3886 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/tests/core/test_plan_evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4557 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/core/test_scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    29395 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/tests/core/test_schema_diff.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      857 2023-01-06 17:16:27.000000 sqlmesh-0.4.2.dev11/tests/core/test_seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    25050 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/core/test_snapshot.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9922 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    21886 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/core/test_state_sync.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.670517 sqlmesh-0.4.2.dev11/tests/dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-16 16:43:18.000000 sqlmesh-0.4.2.dev11/tests/dbt/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      630 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/dbt/conftest.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2564 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/tests/dbt/test_adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12387 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/dbt/test_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    16511 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/tests/dbt/test_transformation.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.670690 sqlmesh-0.4.2.dev11/tests/engines/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/engines/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.671062 sqlmesh-0.4.2.dev11/tests/engines/spark/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/engines/spark/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      357 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/engines/spark/conftest.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1503 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.622212 sqlmesh-0.4.2.dev11/tests/fixtures/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.619707 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.671941 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.672104 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.619842 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1055 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.672238 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 izeigerman   (501) staff       (20)    10264 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.672533 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.673408 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      334 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      863 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      196 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.621442 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.673543 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.673680 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.674448 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.674929 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1155 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      108 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      193 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.675088 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.675231 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.675373 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      540 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)     1249 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.675791 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)       42 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.675941 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.676363 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.676515 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.676793 sqlmesh-0.4.2.dev11/tests/fixtures/migrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)     9823 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/fixtures/migrations/environments.json
--rw-r--r--   0 izeigerman   (501) staff       (20)    25229 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev11/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.676958 sqlmesh-0.4.2.dev11/tests/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/integrations/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.677183 sqlmesh-0.4.2.dev11/tests/integrations/github/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/integrations/github/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.677340 sqlmesh-0.4.2.dev11/tests/integrations/github/fixtures/
--rw-r--r--   0 izeigerman   (501) staff       (20)      816 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 izeigerman   (501) staff       (20)      477 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.677494 sqlmesh-0.4.2.dev11/tests/schedulers/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/schedulers/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.678275 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1414 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.678616 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/operators/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4280 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9673 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1226 2023-03-13 21:05:48.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6043 2023-03-02 21:54:32.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5785 2023-03-02 21:54:32.000000 sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.680407 sqlmesh-0.4.2.dev11/tests/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/utils/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3580 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/tests/utils/test_concurrency.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6430 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev11/tests/utils/test_connection_pool.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1381 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev11/tests/utils/test_dag.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1818 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/utils/test_date.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      551 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/utils/test_filesystem.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5516 2023-03-07 20:10:54.000000 sqlmesh-0.4.2.dev11/tests/utils/test_jinja.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5790 2023-03-03 23:53:25.000000 sqlmesh-0.4.2.dev11/tests/utils/test_metaprogramming.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2501 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev11/tests/utils/test_pandas.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      518 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev11/tests/utils/test_pydantic.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2911 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/tests/utils/test_transactional_file.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1194 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev11/tests/utils/test_yaml.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.680649 sqlmesh-0.4.2.dev11/tests/web/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev11/tests/web/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15137 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/tests/web/test_main.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.680775 sqlmesh-0.4.2.dev11/web/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev11/web/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.682860 sqlmesh-0.4.2.dev11/web/client/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1104 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/.eslintrc.js
--rw-r--r--   0 izeigerman   (501) staff       (20)       94 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)      129 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/.prettierignore
--rw-r--r--   0 izeigerman   (501) staff       (20)      403 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev11/web/client/.prettierrc.js
--rw-r--r--   0 izeigerman   (501) staff       (20)     1076 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/web/client/index.html
--rw-r--r--   0 izeigerman   (501) staff       (20)    36926 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/openapi.json
--rw-r--r--   0 izeigerman   (501) staff       (20)      330 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/orval.config.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)   408504 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/package-lock.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     2395 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/package.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     1642 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/playwright.config.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)       82 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev11/web/client/postcss.config.js
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.622965 sqlmesh-0.4.2.dev11/web/client/public/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.683013 sqlmesh-0.4.2.dev11/web/client/public/favicons/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2473 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.683424 sqlmesh-0.4.2.dev11/web/client/src/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.683859 sqlmesh-0.4.2.dev11/web/client/src/api/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1220 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/api/channels.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     4473 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/web/client/src/api/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3247 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/api/instance.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.623204 sqlmesh-0.4.2.dev11/web/client/src/assets/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.623314 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.685444 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74500 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74524 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74368 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    73964 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    68940 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    67284 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74116 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    73916 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.690122 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    55004 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56384 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57104 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    62320 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56652 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    61688 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57680 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    53148 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57060 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56836 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    61460 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    52820 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    59176 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    63876 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    60768 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    81732 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    60992 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    64792 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.690857 sqlmesh-0.4.2.dev11/web/client/src/context/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4198 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/web/client/src/context/context.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3385 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/context/editor.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      923 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/context/fileTree.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2661 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/context/plan.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1562 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/context/theme.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.691164 sqlmesh-0.4.2.dev11/web/client/src/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)      308 2023-03-02 00:19:27.000000 sqlmesh-0.4.2.dev11/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      817 2023-02-27 20:28:04.000000 sqlmesh-0.4.2.dev11/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     9237 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/web/client/src/index.css
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.623552 sqlmesh-0.4.2.dev11/web/client/src/library/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.624760 sqlmesh-0.4.2.dev11/web/client/src/library/components/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.691322 sqlmesh-0.4.2.dev11/web/client/src/library/components/banner/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1295 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.691462 sqlmesh-0.4.2.dev11/web/client/src/library/components/button/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4517 2023-03-25 06:07:32.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.691594 sqlmesh-0.4.2.dev11/web/client/src/library/components/button/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)     3516 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.691733 sqlmesh-0.4.2.dev11/web/client/src/library/components/divider/
--rw-r--r--   0 izeigerman   (501) staff       (20)      856 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.691878 sqlmesh-0.4.2.dev11/web/client/src/library/components/divider/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      632 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.693499 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1388 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 izeigerman   (501) staff       (20)     4897 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8064 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     2718 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     9819 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8190 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3527 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.693825 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 izeigerman   (501) staff       (20)     5880 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3987 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1538 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.694527 sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/
--rw-r--r--   0 izeigerman   (501) staff       (20)    10852 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6045 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     2997 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      562 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.694875 sqlmesh-0.4.2.dev11/web/client/src/library/components/graph/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2961 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3146 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.695375 sqlmesh-0.4.2.dev11/web/client/src/library/components/ide/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4342 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6011 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    22356 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.695750 sqlmesh-0.4.2.dev11/web/client/src/library/components/input/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2087 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.696370 sqlmesh-0.4.2.dev11/web/client/src/library/components/logo/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2292 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     4637 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8042 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.696829 sqlmesh-0.4.2.dev11/web/client/src/library/components/modal/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1560 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1447 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.699427 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/
--rw-r--r--   0 izeigerman   (501) staff       (20)     7538 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6775 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1312 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    10448 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1178 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    15001 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     9926 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    10478 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3444 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2155 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2634 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.699619 sqlmesh-0.4.2.dev11/web/client/src/library/components/progress/
--rw-r--r--   0 izeigerman   (501) staff       (20)      713 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.700291 sqlmesh-0.4.2.dev11/web/client/src/library/components/root/
--rw-r--r--   0 izeigerman   (501) staff       (20)      526 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1921 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      443 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.700636 sqlmesh-0.4.2.dev11/web/client/src/library/components/splitPane/
--rw-r--r--   0 izeigerman   (501) staff       (20)      788 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.700807 sqlmesh-0.4.2.dev11/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 izeigerman   (501) staff       (20)    11713 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.700983 sqlmesh-0.4.2.dev11/web/client/src/library/components/toggle/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1453 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1197 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/main.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.701846 sqlmesh-0.4.2.dev11/web/client/src/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1647 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev11/web/client/src/models/artifact.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/models/directory.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     4190 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev11/web/client/src/models/environment.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1760 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/src/models/file.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      173 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev11/web/client/src/models/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      766 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev11/web/client/src/models/initial.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      200 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev11/web/client/src/routes.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.702089 sqlmesh-0.4.2.dev11/web/client/src/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)       35 2023-01-20 18:11:03.000000 sqlmesh-0.4.2.dev11/web/client/src/tests/setup.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev11/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.702360 sqlmesh-0.4.2.dev11/web/client/src/types/
--rw-r--r--   0 izeigerman   (501) staff       (20)      467 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/types/enum.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      137 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/types/index.d.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.702619 sqlmesh-0.4.2.dev11/web/client/src/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4102 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/client/src/utils/index.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5245 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/utils/index.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.702750 sqlmesh-0.4.2.dev11/web/client/src/workers/
--rw-r--r--   0 izeigerman   (501) staff       (20)      113 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/workers/index.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.703000 sqlmesh-0.4.2.dev11/web/client/src/workers/sqlglot/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1105 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1578 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5842 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/tailwind.config.js
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.703138 sqlmesh-0.4.2.dev11/web/client/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      170 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/tests/initial.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1141 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/client/tsconfig.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     1297 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev11/web/client/vite.config.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.704108 sqlmesh-0.4.2.dev11/web/server/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev11/web/server/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.704243 sqlmesh-0.4.2.dev11/web/server/api/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev11/web/server/api/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 05:42:03.705482 sqlmesh-0.4.2.dev11/web/server/api/endpoints/
--rw-r--r--   0 izeigerman   (501) staff       (20)      784 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4864 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/commands.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      819 2023-02-27 20:28:04.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1858 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/directories.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      708 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/environments.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      637 2023-02-15 19:33:57.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/events.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5528 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/files.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1834 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/lineage.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      969 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/models.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3806 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/server/api/endpoints/plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3381 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/server/console.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1374 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/server/main.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5724 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/server/models.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      260 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev11/web/server/openapi.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2401 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev11/web/server/settings.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2114 2023-02-04 22:32:08.000000 sqlmesh-0.4.2.dev11/web/server/sse.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2419 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev11/web/server/utils.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.396966 sqlmesh-0.4.2.dev9/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.321769 sqlmesh-0.4.2.dev9/.circleci/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1872 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/.circleci/config.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4414 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/.circleci/continue_config.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)       66 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/.dockerignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2152 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/.gitignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1900 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/.pre-commit-config.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      234 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/.readthedocs.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      135 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/Dockerfile.api
+-rw-r--r--   0 izeigerman   (501) staff       (20)      383 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/Dockerfile.app
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11346 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/LICENSE
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1855 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/Makefile
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2011 2023-04-18 04:12:59.397046 sqlmesh-0.4.2.dev9/PKG-INFO
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1250 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/README.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1008 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docker-compose.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.323791 sqlmesh-0.4.2.dev9/docs/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.309533 sqlmesh-0.4.2.dev9/docs/_readthedocs/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.323910 sqlmesh-0.4.2.dev9/docs/_readthedocs/html/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/docs/_readthedocs/html/.keep
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9981 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/comparisons.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325008 sqlmesh-0.4.2.dev9/docs/concepts/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325258 sqlmesh-0.4.2.dev9/docs/concepts/architecture/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1334 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1113 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6693 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/docs/concepts/audits.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/environments.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5914 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/glossary.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)       13 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/hooks.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3027 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/macros.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325839 sqlmesh-0.4.2.dev9/docs/concepts/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9934 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7454 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/overview.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/python_models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4938 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/seed_models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5356 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/sql_models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6631 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/overview.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325957 sqlmesh-0.4.2.dev9/docs/concepts/plans/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    43124 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8981 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/plans.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)       37 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/team_development.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5699 2023-02-27 20:36:43.000000 sqlmesh-0.4.2.dev9/docs/concepts/tests.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      607 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/docs/development.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.326561 sqlmesh-0.4.2.dev9/docs/guides/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/guides/connections.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10756 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/guides/models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2136 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/guides/projects.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.327152 sqlmesh-0.4.2.dev9/docs/guides/scheduling/
+-rw-r--r--   0 izeigerman   (501) staff       (20)   740917 2023-02-24 17:54:11.000000 sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   379880 2023-02-24 17:54:11.000000 sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5648 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/guides/scheduling.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1854 2023-02-27 20:36:43.000000 sqlmesh-0.4.2.dev9/docs/guides/testing.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5510 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/docs/index.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      290 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/docs/installation.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.327958 sqlmesh-0.4.2.dev9/docs/integrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2905 2023-04-03 17:47:07.000000 sqlmesh-0.4.2.dev9/docs/integrations/airflow.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7309 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/integrations/dbt.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    20383 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/integrations/engines.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      926 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/integrations/github.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      217 2023-03-25 06:07:32.000000 sqlmesh-0.4.2.dev9/docs/integrations/overview.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      665 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/docs/prerequisites.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10774 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/quick_start.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.328548 sqlmesh-0.4.2.dev9/docs/reference/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5816 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/cli.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13240 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/configuration.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4091 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/notebook.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1127 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/overview.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)       14 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/python.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)       16 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/release_notes.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      122 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/docs/requirements.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3249 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/docs/sqlmesh.png
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.328672 sqlmesh-0.4.2.dev9/examples/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.329367 sqlmesh-0.4.2.dev9/examples/airflow/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1713 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev9/examples/airflow/Dockerfile.template
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2164 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/examples/airflow/Makefile
+-rw-r--r--   0 izeigerman   (501) staff       (20)      942 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/README.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.4.2.dev9/examples/airflow/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.329499 sqlmesh-0.4.2.dev9/examples/airflow/dags/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      263 2023-03-09 17:15:39.000000 sqlmesh-0.4.2.dev9/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3515 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev9/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/requirements.txt
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.329801 sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      872 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      151 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330329 sqlmesh-0.4.2.dev9/examples/sushi/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330590 sqlmesh-0.4.2.dev9/examples/sushi/audits/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      105 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/audits/items.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      119 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      829 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi/config.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330726 sqlmesh-0.4.2.dev9/examples/sushi/data/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi/data/.keep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      551 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/helper.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330960 sqlmesh-0.4.2.dev9/examples/sushi/hooks/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.331220 sqlmesh-0.4.2.dev9/examples/sushi/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/macros/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      702 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/macros/macros.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.332573 sqlmesh-0.4.2.dev9/examples/sushi/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      913 2023-03-13 20:04:07.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      204 2023-03-03 17:17:44.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/customers.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1914 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/items.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1892 2023-03-13 20:04:07.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/order_items.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1646 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/orders.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      346 2023-03-25 04:59:10.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      465 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      123 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-04-18 04:08:52.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      197 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.332693 sqlmesh-0.4.2.dev9/examples/sushi/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-03-24 20:49:46.000000 sqlmesh-0.4.2.dev9/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.332824 sqlmesh-0.4.2.dev9/examples/sushi/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1459 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.333510 sqlmesh-0.4.2.dev9/examples/sushi_dbt/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       15 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.333661 sqlmesh-0.4.2.dev9/examples/sushi_dbt/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-14 18:30:53.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      507 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.333933 sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-03-03 23:53:25.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-02-28 16:05:24.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.334936 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1125 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      182 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      309 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      752 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      186 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.311399 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335093 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335247 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335528 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335676 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335776 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335878 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335976 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      783 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.336619 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)       97 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.336748 sqlmesh-0.4.2.dev9/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.336878 sqlmesh-0.4.2.dev9/examples/sushi_dbt/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337132 sqlmesh-0.4.2.dev9/examples/wursthall/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.312325 sqlmesh-0.4.2.dev9/examples/wursthall/audits/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337304 sqlmesh-0.4.2.dev9/examples/wursthall/audits/db/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      141 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev9/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       66 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/config.yaml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337654 sqlmesh-0.4.2.dev9/examples/wursthall/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      618 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337833 sqlmesh-0.4.2.dev9/examples/wursthall/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.338355 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      428 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      256 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3145 2023-02-16 23:39:50.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      537 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339022 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1667 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      120 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3419 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      892 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.312821 sqlmesh-0.4.2.dev9/examples/wursthall/seeds/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339172 sqlmesh-0.4.2.dev9/examples/wursthall/seeds/src/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7416 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339435 sqlmesh-0.4.2.dev9/examples/wursthall/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-02-20 22:54:27.000000 sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      955 2023-02-20 22:54:27.000000 sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2094 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/mkdocs.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339581 sqlmesh-0.4.2.dev9/pdoc/
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)     1153 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/pdoc/cli.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339727 sqlmesh-0.4.2.dev9/pdoc/templates/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      131 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339882 sqlmesh-0.4.2.dev9/posts/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.341317 sqlmesh-0.4.2.dev9/posts/virtual_environments/
+-rw-r--r--   0 izeigerman   (501) staff       (20)   318753 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/change_categorization.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   274526 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/isolated_rigid_envs.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   163619 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/partial_breaking.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   298971 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/stateful_envs.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   366545 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)  1344487 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18666 2023-04-17 20:22:17.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      734 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/pytest.ini
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1344 2023-04-18 04:12:59.397589 sqlmesh-0.4.2.dev9/setup.cfg
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3056 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/setup.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.342715 sqlmesh-0.4.2.dev9/sqlmesh/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        3 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/.airflowignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3676 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      173 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh/_version.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.344096 sqlmesh-0.4.2.dev9/sqlmesh/cli/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      821 2023-04-18 04:08:49.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4314 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/example_project.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8938 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/main.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1391 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/options.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.346536 sqlmesh-0.4.2.dev9/sqlmesh/core/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      586 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/_typing.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.346969 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      449 2023-01-27 03:51:22.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1071 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8136 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.348250 sqlmesh-0.4.2.dev9/sqlmesh/core/config/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      638 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1001 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      940 2023-02-08 20:28:46.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18770 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/connection.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3355 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/loader.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1655 2023-02-08 20:28:46.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/model.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5389 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/root.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8432 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    29182 2023-04-18 02:47:18.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/console.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      731 2023-03-16 20:42:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/constants.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    34133 2023-04-18 02:26:32.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/context.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8612 2023-03-10 17:30:08.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/context_diff.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    17626 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/dialect.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.349928 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2390 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      762 2023-01-18 00:01:51.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    28278 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4238 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10243 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      393 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1930 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1971 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1398 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7713 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1181 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2658 2023-03-01 00:12:50.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3678 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1815 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/environment.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      742 2023-02-09 01:00:20.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/hooks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9362 2023-03-08 20:46:19.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/loader.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18920 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/macros.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.350896 sqlmesh-0.4.2.dev9/sqlmesh/core/model/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      546 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1498 2023-04-17 22:52:49.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/cache.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1300 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2417 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    47553 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/definition.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7382 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/kind.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12622 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/meta.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2017 2023-03-15 19:25:00.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/seed.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2314 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.351261 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      191 2022-12-27 15:59:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    24483 2023-04-18 04:09:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8075 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12174 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/renderer.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15386 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/scheduler.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    19427 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.351751 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      527 2023-02-13 20:33:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    31251 2023-04-18 04:05:15.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18706 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.352240 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      692 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13080 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12222 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    19996 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12062 2023-04-18 02:26:32.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/test.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1412 2022-12-24 00:00:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/user.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354033 sqlmesh-0.4.2.dev9/sqlmesh/dbt/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       79 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15639 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11330 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1969 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/column.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9663 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3229 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/loader.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/model.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12410 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/package.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3530 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/profile.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/project.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1049 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/seed.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3145 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/source.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11118 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/target.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-02 18:36:40.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/util.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354255 sqlmesh-0.4.2.dev9/sqlmesh/engines/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4437 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/commands.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354501 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3414 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354848 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      148 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2571 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354969 sqlmesh-0.4.2.dev9/sqlmesh/integrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.355424 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2210 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1726 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1829 2023-01-18 20:54:37.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13153 2023-03-15 19:24:58.000000 sqlmesh-0.4.2.dev9/sqlmesh/magics.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.355782 sqlmesh-0.4.2.dev9/sqlmesh/migrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1749 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/py.typed
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.355930 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.357195 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-04 00:12:26.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4020 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3830 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18799 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.357548 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-16 21:08:59.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2132 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      868 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8508 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.358623 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1341 2023-01-18 20:54:37.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6307 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2549 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      877 2023-01-31 17:31:24.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1211 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1340 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5222 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10922 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4400 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1292 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4139 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5006 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.360288 sqlmesh-0.4.2.dev9/sqlmesh/utils/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4326 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7530 2023-02-14 22:10:01.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      410 2022-12-30 16:25:50.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/conversions.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4329 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/dag.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7549 2023-04-18 02:34:51.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/date.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1244 2023-02-04 22:32:08.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/errors.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15925 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/jinja.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15093 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/pandas.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1609 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1534 2023-01-25 18:09:57.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/rich.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6166 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1301 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.343576 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2011 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 izeigerman   (501) staff       (20)    20173 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)        1 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)      142 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)      787 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)    21020 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/sqlmesh.svg
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.360610 sqlmesh-0.4.2.dev9/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      285 2023-02-07 17:58:48.000000 sqlmesh-0.4.2.dev9/tests/common_fixtures.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3773 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/conftest.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.363636 sqlmesh-0.4.2.dev9/tests/core/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/core/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.364777 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    27289 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1298 2023-02-07 16:29:13.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1281 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2613 2023-02-14 20:17:36.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7155 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3245 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7073 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/tests/core/test_audit.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6611 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      850 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_connection_config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10703 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_context.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2749 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/tests/core/test_dialect.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      464 2022-12-28 17:42:44.000000 sqlmesh-0.4.2.dev9/tests/core/test_environment.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    25987 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_integration.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5760 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_macros.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    24586 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_model.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15859 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/test_plan.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3886 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4557 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_scheduler.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    29395 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/test_schema_diff.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      857 2023-01-06 17:16:27.000000 sqlmesh-0.4.2.dev9/tests/core/test_seed.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    25050 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_snapshot.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9922 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    21886 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_state_sync.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.365473 sqlmesh-0.4.2.dev9/tests/dbt/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-16 16:43:18.000000 sqlmesh-0.4.2.dev9/tests/dbt/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      630 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/dbt/conftest.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2564 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/dbt/test_adapter.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12387 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/dbt/test_config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    16511 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/tests/dbt/test_transformation.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.365718 sqlmesh-0.4.2.dev9/tests/engines/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.366142 sqlmesh-0.4.2.dev9/tests/engines/spark/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/spark/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      357 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/spark/conftest.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1503 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.316475 sqlmesh-0.4.2.dev9/tests/fixtures/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.315288 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.366966 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.367114 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.315423 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1055 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.367276 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10264 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.367604 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368374 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      334 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      863 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      196 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.315742 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368533 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368677 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368944 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369396 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1155 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      108 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      193 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369542 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369680 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369800 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      540 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1249 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370097 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       42 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370233 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370688 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370840 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371107 sqlmesh-0.4.2.dev9/tests/fixtures/migrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9823 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)    25229 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371463 sqlmesh-0.4.2.dev9/tests/integrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/integrations/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371734 sqlmesh-0.4.2.dev9/tests/integrations/github/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/integrations/github/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371873 sqlmesh-0.4.2.dev9/tests/integrations/github/fixtures/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      816 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)      477 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371992 sqlmesh-0.4.2.dev9/tests/schedulers/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/schedulers/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.372877 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1414 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.373292 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4280 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9673 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1226 2023-03-13 21:05:48.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6043 2023-03-02 21:54:32.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5785 2023-03-02 21:54:32.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.374814 sqlmesh-0.4.2.dev9/tests/utils/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3580 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/utils/test_concurrency.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6430 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev9/tests/utils/test_connection_pool.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1381 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/utils/test_dag.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1818 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/test_date.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      551 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/test_filesystem.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5516 2023-03-07 20:10:54.000000 sqlmesh-0.4.2.dev9/tests/utils/test_jinja.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5790 2023-03-03 23:53:25.000000 sqlmesh-0.4.2.dev9/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2501 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev9/tests/utils/test_pandas.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      518 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/test_pydantic.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2911 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/utils/test_transactional_file.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1194 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev9/tests/utils/test_yaml.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.375038 sqlmesh-0.4.2.dev9/tests/web/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/tests/web/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15137 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/tests/web/test_main.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.375155 sqlmesh-0.4.2.dev9/web/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/web/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.377130 sqlmesh-0.4.2.dev9/web/client/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1104 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/.eslintrc.js
+-rw-r--r--   0 izeigerman   (501) staff       (20)       94 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/.gitignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)      129 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/.prettierignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)      403 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev9/web/client/.prettierrc.js
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1076 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/index.html
+-rw-r--r--   0 izeigerman   (501) staff       (20)    36926 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/openapi.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)      330 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/orval.config.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)   408504 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/package-lock.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2395 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/package.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1642 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/playwright.config.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)       82 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/postcss.config.js
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317195 sqlmesh-0.4.2.dev9/web/client/public/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.377287 sqlmesh-0.4.2.dev9/web/client/public/favicons/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2473 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.377655 sqlmesh-0.4.2.dev9/web/client/src/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.378069 sqlmesh-0.4.2.dev9/web/client/src/api/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1220 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/api/channels.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4473 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/api/index.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3247 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/api/instance.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317427 sqlmesh-0.4.2.dev9/web/client/src/assets/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317535 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.379470 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74500 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74524 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74368 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    73964 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    68940 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    67284 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74116 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    73916 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.382391 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    55004 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    56384 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    57104 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    62320 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    56652 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    61688 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    57680 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    53148 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    57060 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    56836 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    61460 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    52820 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    59176 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    63876 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    60768 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    81732 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    60992 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    64792 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383040 sqlmesh-0.4.2.dev9/web/client/src/context/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4198 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/context/context.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3385 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/context/editor.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      923 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/context/fileTree.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2661 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/context/plan.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1562 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/context/theme.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383262 sqlmesh-0.4.2.dev9/web/client/src/hooks/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      308 2023-03-02 00:19:27.000000 sqlmesh-0.4.2.dev9/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      817 2023-02-27 20:28:04.000000 sqlmesh-0.4.2.dev9/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9237 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/src/index.css
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317774 sqlmesh-0.4.2.dev9/web/client/src/library/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.318969 sqlmesh-0.4.2.dev9/web/client/src/library/components/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383377 sqlmesh-0.4.2.dev9/web/client/src/library/components/banner/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1295 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383500 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4517 2023-03-25 06:07:32.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383621 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3516 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383737 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      856 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383856 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      632 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.384996 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1388 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4897 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8064 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2718 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9819 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8190 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3527 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.385303 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5880 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3987 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1538 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.385863 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10852 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6045 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2997 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      562 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.386140 sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2961 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3146 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.386571 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4342 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6011 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    22356 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.386829 sqlmesh-0.4.2.dev9/web/client/src/library/components/input/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2087 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.387203 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2292 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4637 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8042 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.387575 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1560 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1447 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.391353 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7538 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6775 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1312 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10448 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1178 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15001 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9926 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10478 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3444 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2155 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2634 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.391515 sqlmesh-0.4.2.dev9/web/client/src/library/components/progress/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      713 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392026 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      526 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1921 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      443 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392281 sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      788 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392425 sqlmesh-0.4.2.dev9/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11713 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392554 sqlmesh-0.4.2.dev9/web/client/src/library/components/toggle/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1453 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1197 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/main.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.393344 sqlmesh-0.4.2.dev9/web/client/src/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1647 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/models/artifact.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/models/directory.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4190 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev9/web/client/src/models/environment.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1760 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/models/file.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      173 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/models/index.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      766 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/models/initial.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      200 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/routes.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.393603 sqlmesh-0.4.2.dev9/web/client/src/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       35 2023-01-20 18:11:03.000000 sqlmesh-0.4.2.dev9/web/client/src/tests/setup.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev9/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.393855 sqlmesh-0.4.2.dev9/web/client/src/types/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      467 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/types/enum.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      137 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/types/index.d.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394105 sqlmesh-0.4.2.dev9/web/client/src/utils/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4102 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5245 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/utils/index.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394232 sqlmesh-0.4.2.dev9/web/client/src/workers/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      113 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/workers/index.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394473 sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1105 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1578 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5842 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/tailwind.config.js
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394596 sqlmesh-0.4.2.dev9/web/client/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      170 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/tests/initial.spec.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1141 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/tsconfig.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1297 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/vite.config.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.395495 sqlmesh-0.4.2.dev9/web/server/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/web/server/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.395616 sqlmesh-0.4.2.dev9/web/server/api/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/server/api/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.396842 sqlmesh-0.4.2.dev9/web/server/api/endpoints/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      784 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4864 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/commands.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      819 2023-02-27 20:28:04.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/context.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1858 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/directories.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      708 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/environments.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      637 2023-02-15 19:33:57.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/events.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5528 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/files.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1834 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      969 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/models.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3806 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/plan.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3381 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/console.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1374 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/main.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5724 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/models.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      260 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/openapi.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2401 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/web/server/settings.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2114 2023-02-04 22:32:08.000000 sqlmesh-0.4.2.dev9/web/server/sse.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2419 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/server/utils.py
```

### Comparing `sqlmesh-0.4.2.dev11/.circleci/config.yml` & `sqlmesh-0.4.2.dev9/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/.circleci/continue_config.yml` & `sqlmesh-0.4.2.dev9/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/.gitignore` & `sqlmesh-0.4.2.dev9/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/.pre-commit-config.yaml` & `sqlmesh-0.4.2.dev9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/LICENSE` & `sqlmesh-0.4.2.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/Makefile` & `sqlmesh-0.4.2.dev9/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/PKG-INFO` & `sqlmesh-0.4.2.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.4.2.dev11
+Version: 0.4.2.dev9
 Summary: UNKNOWN
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `sqlmesh-0.4.2.dev11/README.md` & `sqlmesh-0.4.2.dev9/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docker-compose.yml` & `sqlmesh-0.4.2.dev9/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/comparisons.md` & `sqlmesh-0.4.2.dev9/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/architecture/serialization.md` & `sqlmesh-0.4.2.dev9/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.4.2.dev9/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/audits.md` & `sqlmesh-0.4.2.dev9/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/environments.md` & `sqlmesh-0.4.2.dev9/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/glossary.md` & `sqlmesh-0.4.2.dev9/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/macros.md` & `sqlmesh-0.4.2.dev9/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/models/model_kinds.md` & `sqlmesh-0.4.2.dev9/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/models/overview.md` & `sqlmesh-0.4.2.dev9/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/models/python_models.md` & `sqlmesh-0.4.2.dev9/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/models/seed_models.md` & `sqlmesh-0.4.2.dev9/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/models/sql_models.md` & `sqlmesh-0.4.2.dev9/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/overview.md` & `sqlmesh-0.4.2.dev9/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.4.2.dev9/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/plans.md` & `sqlmesh-0.4.2.dev9/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/concepts/tests.md` & `sqlmesh-0.4.2.dev9/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/development.md` & `sqlmesh-0.4.2.dev9/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/guides/connections.md` & `sqlmesh-0.4.2.dev9/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/guides/models.md` & `sqlmesh-0.4.2.dev9/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/guides/projects.md` & `sqlmesh-0.4.2.dev9/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/guides/scheduling.md` & `sqlmesh-0.4.2.dev9/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/guides/testing.md` & `sqlmesh-0.4.2.dev9/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/index.md` & `sqlmesh-0.4.2.dev9/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/integrations/airflow.md` & `sqlmesh-0.4.2.dev9/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/integrations/dbt.md` & `sqlmesh-0.4.2.dev9/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/integrations/engines.md` & `sqlmesh-0.4.2.dev9/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/integrations/github.md` & `sqlmesh-0.4.2.dev9/docs/integrations/github.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/prerequisites.md` & `sqlmesh-0.4.2.dev9/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/quick_start.md` & `sqlmesh-0.4.2.dev9/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/reference/cli.md` & `sqlmesh-0.4.2.dev9/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/reference/configuration.md` & `sqlmesh-0.4.2.dev9/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/reference/notebook.md` & `sqlmesh-0.4.2.dev9/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/reference/overview.md` & `sqlmesh-0.4.2.dev9/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/docs/sqlmesh.png` & `sqlmesh-0.4.2.dev9/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/airflow/Dockerfile.template` & `sqlmesh-0.4.2.dev9/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/airflow/Makefile` & `sqlmesh-0.4.2.dev9/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/airflow/README.md` & `sqlmesh-0.4.2.dev9/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.4.2.dev9/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/config.py` & `sqlmesh-0.4.2.dev9/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/helper.py` & `sqlmesh-0.4.2.dev9/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/macros/macros.py` & `sqlmesh-0.4.2.dev9/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.4.2.dev9/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/models/items.py` & `sqlmesh-0.4.2.dev9/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/models/order_items.py` & `sqlmesh-0.4.2.dev9/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/models/orders.py` & `sqlmesh-0.4.2.dev9/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.4.2.dev9/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/macros/macros.py` & `sqlmesh-0.4.2.dev9/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.4.2.dev9/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.4.2.dev9/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/models/src/shared.py` & `sqlmesh-0.4.2.dev9/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.4.2.dev9/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/mkdocs.yml` & `sqlmesh-0.4.2.dev9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/pdoc/cli.py` & `sqlmesh-0.4.2.dev9/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/posts/virtual_environments/change_categorization.png` & `sqlmesh-0.4.2.dev9/posts/virtual_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/posts/virtual_environments/isolated_rigid_envs.png` & `sqlmesh-0.4.2.dev9/posts/virtual_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/posts/virtual_environments/partial_breaking.png` & `sqlmesh-0.4.2.dev9/posts/virtual_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/posts/virtual_environments/stateful_envs.png` & `sqlmesh-0.4.2.dev9/posts/virtual_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/posts/virtual_environments/virtual_envs.png` & `sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/posts/virtual_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/posts/virtual_environments.md` & `sqlmesh-0.4.2.dev9/posts/virtual_environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/pytest.ini` & `sqlmesh-0.4.2.dev9/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/setup.cfg` & `sqlmesh-0.4.2.dev9/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/setup.py` & `sqlmesh-0.4.2.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/cli/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/cli/example_project.py` & `sqlmesh-0.4.2.dev9/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/cli/main.py` & `sqlmesh-0.4.2.dev9/sqlmesh/cli/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/cli/options.py` & `sqlmesh-0.4.2.dev9/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/_typing.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/audit/definition.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/base.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/common.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/connection.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/loader.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/model.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/root.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/console.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,17 +336,15 @@
         """Displays the models with missing dates"""
         if not plan.missing_intervals:
             return
         backfill = Tree("[bold]Models needing backfill (missing dates):")
         for missing in plan.missing_intervals:
             snapshot = plan.context_diff.snapshots[missing.snapshot_name]
             view_name = snapshot.qualified_view_name.for_environment(plan.environment_name)
-            backfill.add(
-                f"{view_name}: {missing.format_missing_range(snapshot.model.interval_unit())}"
-            )
+            backfill.add(f"{view_name}: {missing.format_missing_range()}")
         self._print(backfill)
 
     def _prompt_backfill(self, plan: Plan, auto_apply: bool) -> None:
         is_forward_only_dev = plan.is_dev and plan.forward_only
         backfill_or_preview = "preview" if is_forward_only_dev else "backfill"
 
         if plan.is_start_and_end_allowed:
```

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/constants.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/context.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/context_diff.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/dialect.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/environment.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/hooks.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/loader.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/macros.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/cache.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/common.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/decorator.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/definition.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/kind.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/meta.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/model/seed.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/notification_target.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/plan/definition.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/plan/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from sqlmesh.utils.date import (
     TimeLike,
     make_inclusive,
     make_inclusive_end,
     now,
     to_date,
     to_datetime,
-    to_ds,
     to_timestamp,
     validate_date_range,
     yesterday_ds,
 )
 from sqlmesh.utils.errors import PlanError, SQLMeshError
 from sqlmesh.utils.pydantic import PydanticModel
 
@@ -573,19 +572,16 @@
     snapshot_name: str
     intervals: Intervals
 
     @property
     def merged_intervals(self) -> Intervals:
         return merge_intervals(self.intervals)
 
-    def format_missing_range(self, unit: t.Optional[IntervalUnit] = None) -> str:
+    def format_missing_range(self) -> str:
         intervals = [make_inclusive(start, end) for start, end in self.merged_intervals]
         return ", ".join(
-            f"({_format_date_time(start, unit)}, {_format_date_time(end, unit)})"
-            for start, end in intervals
+            f"({_format_date_time(start)}, {_format_date_time(end)})" for start, end in intervals
         )
 
 
-def _format_date_time(time_like: TimeLike, unit: t.Optional[IntervalUnit]) -> str:
-    if unit is None or unit == IntervalUnit.DAY:
-        return to_ds(time_like)
+def _format_date_time(time_like: TimeLike) -> str:
     return to_datetime(time_like).isoformat()[:19]
```

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/renderer.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/scheduler.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/schema_diff.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,24 +444,22 @@
             start: Start interval to remove.
             end: End interval to remove.
         """
         interval = self._inclusive_exclusive(start, end)
         self.intervals = remove_interval(self.intervals, *interval)
         self.dev_intervals = remove_interval(self.dev_intervals, *interval)
 
-    def _inclusive_exclusive(
-        self, start: TimeLike, end: TimeLike, strict: bool = True
-    ) -> t.Tuple[int, int]:
+    def _inclusive_exclusive(self, start: TimeLike, end: TimeLike) -> t.Tuple[int, int]:
         start_ts = to_timestamp(self.model.cron_floor(start))
         end_ts = to_timestamp(
             self.model.cron_next(end) if is_date(end) else self.model.cron_floor(end)
         )
 
-        if (strict and start_ts >= end_ts) or (start_ts > end_ts):
-            raise ValueError("`end` must be greater than `start`")
+        if start_ts > end_ts:
+            raise ValueError("`end` must be > `start`")
         return (start_ts, end_ts)
 
     def merge_intervals(self, other: Snapshot) -> None:
         """Inherits intervals from the target snapshot.
 
         Args:
             other: The target snapshot to inherit intervals from.
@@ -486,17 +484,15 @@
         Returns:
             A list of all the missing intervals as epoch timestamps.
         """
         if self.is_embedded_kind:
             return []
 
         missing = []
-        start_dt, end_dt = (
-            to_datetime(ts) for ts in self._inclusive_exclusive(start, end, strict=False)
-        )
+        start_dt, end_dt = (to_datetime(ts) for ts in self._inclusive_exclusive(start, end))
         dates = tuple(croniter_range(start_dt, end_dt, self.model.normalized_cron()))
         size = len(dates) - 1
 
         for i in range(size):
             current_ts = to_timestamp(dates[i])
             end_ts = (
                 to_timestamp(dates[i + 1])
```

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/test.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/core/user.py` & `sqlmesh-0.4.2.dev9/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/adapter.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/basemodel.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/builtin.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/column.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/common.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/loader.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/model.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/package.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/package.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/profile.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/project.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/seed.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/source.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/dbt/target.py` & `sqlmesh-0.4.2.dev9/sqlmesh/dbt/target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/engines/commands.py` & `sqlmesh-0.4.2.dev9/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/app.py` & `sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/magics.py` & `sqlmesh-0.4.2.dev9/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.4.2.dev9/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/__init__.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/concurrency.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/dag.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/date.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/errors.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/jinja.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/pandas.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/pydantic.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/rich.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh/utils/yaml.py` & `sqlmesh-0.4.2.dev9/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.4.2.dev9/sqlmesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.4.2.dev11
+Version: 0.4.2.dev9
 Summary: UNKNOWN
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.4.2.dev9/sqlmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.4.2.dev9/sqlmesh.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/sqlmesh.svg` & `sqlmesh-0.4.2.dev9/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/conftest.py` & `sqlmesh-0.4.2.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_audit.py` & `sqlmesh-0.4.2.dev9/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_config.py` & `sqlmesh-0.4.2.dev9/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_connection_config.py` & `sqlmesh-0.4.2.dev9/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_context.py` & `sqlmesh-0.4.2.dev9/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_dialect.py` & `sqlmesh-0.4.2.dev9/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_integration.py` & `sqlmesh-0.4.2.dev9/tests/core/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_macros.py` & `sqlmesh-0.4.2.dev9/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_model.py` & `sqlmesh-0.4.2.dev9/tests/core/test_model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_plan.py` & `sqlmesh-0.4.2.dev9/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_plan_evaluator.py` & `sqlmesh-0.4.2.dev9/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_scheduler.py` & `sqlmesh-0.4.2.dev9/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_schema_diff.py` & `sqlmesh-0.4.2.dev9/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_seed.py` & `sqlmesh-0.4.2.dev9/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_snapshot.py` & `sqlmesh-0.4.2.dev9/tests/core/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.4.2.dev9/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/core/test_state_sync.py` & `sqlmesh-0.4.2.dev9/tests/core/test_state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/dbt/conftest.py` & `sqlmesh-0.4.2.dev9/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/dbt/test_adapter.py` & `sqlmesh-0.4.2.dev9/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/dbt/test_config.py` & `sqlmesh-0.4.2.dev9/tests/dbt/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/dbt/test_transformation.py` & `sqlmesh-0.4.2.dev9/tests/dbt/test_transformation.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/engines/spark/test_db_api.py` & `sqlmesh-0.4.2.dev9/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/migrations/environments.json` & `sqlmesh-0.4.2.dev9/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.4.2.dev9/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.4.2.dev9/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_concurrency.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_connection_pool.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_dag.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_date.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_filesystem.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_jinja.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_metaprogramming.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_pandas.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_pydantic.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_transactional_file.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/utils/test_yaml.py` & `sqlmesh-0.4.2.dev9/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/tests/web/test_main.py` & `sqlmesh-0.4.2.dev9/tests/web/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/.eslintrc.js` & `sqlmesh-0.4.2.dev9/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/index.html` & `sqlmesh-0.4.2.dev9/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/openapi.json` & `sqlmesh-0.4.2.dev9/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/package-lock.json` & `sqlmesh-0.4.2.dev9/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/package.json` & `sqlmesh-0.4.2.dev9/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/playwright.config.ts` & `sqlmesh-0.4.2.dev9/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/public/favicons/favicon.ico` & `sqlmesh-0.4.2.dev9/web/client/public/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/api/channels.ts` & `sqlmesh-0.4.2.dev9/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/api/index.ts` & `sqlmesh-0.4.2.dev9/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/api/instance.ts` & `sqlmesh-0.4.2.dev9/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/context/context.ts` & `sqlmesh-0.4.2.dev9/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/context/editor.ts` & `sqlmesh-0.4.2.dev9/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/context/fileTree.ts` & `sqlmesh-0.4.2.dev9/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/context/plan.ts` & `sqlmesh-0.4.2.dev9/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/context/theme.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.4.2.dev9/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/index.css` & `sqlmesh-0.4.2.dev9/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/Graph.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/main.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/models/artifact.ts` & `sqlmesh-0.4.2.dev9/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/models/directory.ts` & `sqlmesh-0.4.2.dev9/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/models/environment.ts` & `sqlmesh-0.4.2.dev9/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/models/file.ts` & `sqlmesh-0.4.2.dev9/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/models/initial.ts` & `sqlmesh-0.4.2.dev9/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/tests/utils.tsx` & `sqlmesh-0.4.2.dev9/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/utils/index.spec.ts` & `sqlmesh-0.4.2.dev9/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/utils/index.ts` & `sqlmesh-0.4.2.dev9/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/tailwind.config.js` & `sqlmesh-0.4.2.dev9/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/tsconfig.json` & `sqlmesh-0.4.2.dev9/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/client/vite.config.ts` & `sqlmesh-0.4.2.dev9/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/__init__.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/commands.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/context.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/directories.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/environments.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/events.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/files.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/lineage.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/models.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/api/endpoints/plan.py` & `sqlmesh-0.4.2.dev9/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/console.py` & `sqlmesh-0.4.2.dev9/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/main.py` & `sqlmesh-0.4.2.dev9/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/models.py` & `sqlmesh-0.4.2.dev9/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/settings.py` & `sqlmesh-0.4.2.dev9/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/sse.py` & `sqlmesh-0.4.2.dev9/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev11/web/server/utils.py` & `sqlmesh-0.4.2.dev9/web/server/utils.py`

 * *Files identical despite different names*

