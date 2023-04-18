# Comparing `tmp/phidata-1.5.9.tar.gz` & `tmp/phidata-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.5.9.tar", last modified: Tue Apr 11 01:51:39 2023, max compression
+gzip compressed data, was "phidata-1.6.0.tar", last modified: Tue Apr 18 12:16:34 2023, max compression
```

## Comparing `phidata-1.5.9.tar` & `phidata-1.6.0.tar`

### file list

```diff
@@ -1,507 +1,508 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-11 01:51:20.000000 phidata-1.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-11 01:51:39.606932 phidata-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-11 01:51:20.000000 phidata-1.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.562932 phidata-1.5.9/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.562932 phidata-1.5.9/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.562932 phidata-1.5.9/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/assistant/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.566932 phidata-1.5.9/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/k8s/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53160 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/server/app_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58186 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.570932 phidata-1.5.9/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/create/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.574932 phidata-1.5.9/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.578932 phidata-1.5.9/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.582932 phidata-1.5.9/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.586932 phidata-1.5.9/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.590932 phidata-1.5.9/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.594932 phidata-1.5.9/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.594932 phidata-1.5.9/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.594932 phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.594932 phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.594932 phidata-1.5.9/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.594932 phidata-1.5.9/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.594932 phidata-1.5.9/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/llm/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/duckdb/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/duckdb/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/duckdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/duckdb/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/duckdb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.598932 phidata-1.5.9/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.602932 phidata-1.5.9/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/utils/workspace_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 01:51:20.000000 phidata-1.5.9/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.562932 phidata-1.5.9/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-11 01:51:39.000000 phidata-1.5.9/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-11 01:51:39.000000 phidata-1.5.9/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:51:39.000000 phidata-1.5.9/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-11 01:51:39.000000 phidata-1.5.9/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 01:51:39.000000 phidata-1.5.9/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-11 01:51:20.000000 phidata-1.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:51:39.606932 phidata-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 01:51:20.000000 phidata-1.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:51:39.606932 phidata-1.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 01:51:20.000000 phidata-1.5.9/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.358558 phidata-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-18 12:16:08.000000 phidata-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-18 12:16:34.358558 phidata-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-18 12:16:08.000000 phidata-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.238549 phidata-1.6.0/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.242550 phidata-1.6.0/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.242550 phidata-1.6.0/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.242550 phidata-1.6.0/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.242550 phidata-1.6.0/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.242550 phidata-1.6.0/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.242550 phidata-1.6.0/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/assistant/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.246550 phidata-1.6.0/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/k8s/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.250550 phidata-1.6.0/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.250550 phidata-1.6.0/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.250550 phidata-1.6.0/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53160 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.250550 phidata-1.6.0/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.250550 phidata-1.6.0/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/redis/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.250550 phidata-1.6.0/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/server/app_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58187 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.250550 phidata-1.6.0/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.254550 phidata-1.6.0/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.254550 phidata-1.6.0/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.254550 phidata-1.6.0/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.254550 phidata-1.6.0/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.254550 phidata-1.6.0/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.254550 phidata-1.6.0/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.258551 phidata-1.6.0/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.258551 phidata-1.6.0/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.258551 phidata-1.6.0/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.258551 phidata-1.6.0/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/create/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.258551 phidata-1.6.0/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.262551 phidata-1.6.0/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.262551 phidata-1.6.0/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.266551 phidata-1.6.0/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.266551 phidata-1.6.0/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.266551 phidata-1.6.0/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.270552 phidata-1.6.0/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.274552 phidata-1.6.0/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.278552 phidata-1.6.0/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.278552 phidata-1.6.0/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.278552 phidata-1.6.0/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.282552 phidata-1.6.0/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.282552 phidata-1.6.0/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.286553 phidata-1.6.0/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.286553 phidata-1.6.0/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.286553 phidata-1.6.0/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.290553 phidata-1.6.0/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.290553 phidata-1.6.0/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.294553 phidata-1.6.0/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.298554 phidata-1.6.0/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.302554 phidata-1.6.0/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.302554 phidata-1.6.0/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.306554 phidata-1.6.0/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.310554 phidata-1.6.0/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.314555 phidata-1.6.0/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.314555 phidata-1.6.0/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.314555 phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.314555 phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.314555 phidata-1.6.0/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.318555 phidata-1.6.0/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.318555 phidata-1.6.0/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.318555 phidata-1.6.0/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.318555 phidata-1.6.0/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.322555 phidata-1.6.0/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.322555 phidata-1.6.0/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.322555 phidata-1.6.0/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.322555 phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.322555 phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.322555 phidata-1.6.0/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.322555 phidata-1.6.0/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.326556 phidata-1.6.0/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.326556 phidata-1.6.0/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.326556 phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.330556 phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.330556 phidata-1.6.0/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.330556 phidata-1.6.0/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.330556 phidata-1.6.0/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.334556 phidata-1.6.0/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.334556 phidata-1.6.0/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.338556 phidata-1.6.0/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.342557 phidata-1.6.0/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.342557 phidata-1.6.0/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.342557 phidata-1.6.0/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.342557 phidata-1.6.0/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.346557 phidata-1.6.0/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.346557 phidata-1.6.0/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.346557 phidata-1.6.0/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.346557 phidata-1.6.0/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.346557 phidata-1.6.0/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.350557 phidata-1.6.0/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.350557 phidata-1.6.0/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.350557 phidata-1.6.0/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.350557 phidata-1.6.0/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.350557 phidata-1.6.0/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.350557 phidata-1.6.0/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.350557 phidata-1.6.0/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.354558 phidata-1.6.0/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.354558 phidata-1.6.0/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.354558 phidata-1.6.0/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.354558 phidata-1.6.0/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.354558 phidata-1.6.0/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.354558 phidata-1.6.0/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.354558 phidata-1.6.0/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/utils/workspace_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.358558 phidata-1.6.0/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.358558 phidata-1.6.0/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.358558 phidata-1.6.0/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-18 12:16:08.000000 phidata-1.6.0/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.242550 phidata-1.6.0/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-18 12:16:34.000000 phidata-1.6.0/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-04-18 12:16:34.000000 phidata-1.6.0/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:16:34.000000 phidata-1.6.0/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 12:16:34.000000 phidata-1.6.0/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 12:16:34.000000 phidata-1.6.0/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-18 12:16:08.000000 phidata-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:16:34.358558 phidata-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 12:16:08.000000 phidata-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:16:34.358558 phidata-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 12:16:08.000000 phidata-1.6.0/tests/test_placeholder.py
```

### Comparing `phidata-1.5.9/LICENSE` & `phidata-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/PKG-INFO` & `phidata-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.5.9
+Version: 1.6.0
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.5.9 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.0 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.5.9/README.md` & `phidata-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/airflow/operators/empty.py` & `phidata-1.6.0/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/airflow/airflow_base.py` & `phidata-1.6.0/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/airflow/airflow_flower.py` & `phidata-1.6.0/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/airflow/airflow_manager.py` & `phidata-1.6.0/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.6.0/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/airflow/airflow_webserver.py` & `phidata-1.6.0/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/airflow/airflow_worker.py` & `phidata-1.6.0/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/alertmanager/alertmanager.py` & `phidata-1.6.0/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/amundsen/frontend.py` & `phidata-1.6.0/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/amundsen/metadata.py` & `phidata-1.6.0/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/amundsen/search.py` & `phidata-1.6.0/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/assistant/assistant.py` & `phidata-1.6.0/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/cadvisor/cadvisor.py` & `phidata-1.6.0/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/databox/databox.py` & `phidata-1.6.0/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/db/base_db.py` & `phidata-1.6.0/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/elastic/elastic_app.py` & `phidata-1.6.0/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.6.0/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/fastapi/fastapi.py` & `phidata-1.6.0/phidata/app/fastapi/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         name: str = "fast-api",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/fast-api",
-        image_tag: str = "1.5.0",
+        image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
         command: Optional[Union[str, List]] = "api start",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Container Configuration,
```

### Comparing `phidata-1.5.9/phidata/app/grafana/grafana.py` & `phidata-1.6.0/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/group.py` & `phidata-1.6.0/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.6.0/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.6.0/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/k8s/app.py` & `phidata-1.6.0/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/k8s/dir.py` & `phidata-1.6.0/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/k8s/url.py` & `phidata-1.6.0/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/neo4j/neo4j.py` & `phidata-1.6.0/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.6.0/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/phidata_app.py` & `phidata-1.6.0/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/postgres/postgres_db.py` & `phidata-1.6.0/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/prometheus/prometheus.py` & `phidata-1.6.0/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/redis/redis.py` & `phidata-1.6.0/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/server/api_server.py` & `phidata-1.6.0/phidata/app/server/app_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,31 +7,31 @@
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class ApiServerArgs(ServerBaseArgs):
+class AppServerArgs(ServerBaseArgs):
     pass
 
 
-class ApiServer(ServerBase):
+class AppServer(ServerBase):
     def __init__(
         self,
-        name: str = "api-server",
+        name: str = "app-server",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/server",
-        image_tag: str = "1.4.1",
+        image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "api start",
+        command: Optional[Union[str, List]] = "app start",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
@@ -54,19 +54,19 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 9090,
+        container_port: int = 9095,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 9090,
+        container_host_port: int = 9095,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
         # Path to mount the workspace volume inside the container,
         workspace_volume_container_path: str = "/usr/local/server",
```

### Comparing `phidata-1.5.9/phidata/app/server/app_server.py` & `phidata-1.6.0/phidata/app/server/api_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,31 +7,31 @@
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class AppServerArgs(ServerBaseArgs):
+class ApiServerArgs(ServerBaseArgs):
     pass
 
 
-class AppServer(ServerBase):
+class ApiServer(ServerBase):
     def __init__(
         self,
-        name: str = "app-server",
+        name: str = "api-server",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/server",
-        image_tag: str = "1.4.1",
+        image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "app start",
+        command: Optional[Union[str, List]] = "api start",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
@@ -54,19 +54,19 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 9095,
+        container_port: int = 9090,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 9095,
+        container_host_port: int = 9090,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
         # Path to mount the workspace volume inside the container,
         workspace_volume_container_path: str = "/usr/local/server",
```

### Comparing `phidata-1.5.9/phidata/app/server/server_base.py` & `phidata-1.6.0/phidata/app/server/server_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         name: str = "server",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/server",
-        image_tag: str = "1.5.0",
+        image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
         command: Optional[Union[str, List]] = None,
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Container Configuration,
```

### Comparing `phidata-1.5.9/phidata/app/spark/spark_base.py` & `phidata-1.6.0/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/spark/spark_driver.py` & `phidata-1.6.0/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/spark/spark_worker.py` & `phidata-1.6.0/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/streamlit/streamlit.py` & `phidata-1.6.0/phidata/app/streamlit/streamlit.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         name: str = "streamlit-app",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/streamlit-app",
-        image_tag: str = "1.5.0",
+        image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
         command: Optional[Union[str, List]] = "app start",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Container Configuration,
```

### Comparing `phidata-1.5.9/phidata/app/superset/superset_base.py` & `phidata-1.6.0/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/superset/superset_init.py` & `phidata-1.6.0/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/superset/superset_webserver.py` & `phidata-1.6.0/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/superset/superset_worker.py` & `phidata-1.6.0/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/superset/superset_worker_beat.py` & `phidata-1.6.0/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/traefik/crds.py` & `phidata-1.6.0/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/traefik/ingress_route.py` & `phidata-1.6.0/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/app/traefik/router.py` & `phidata-1.6.0/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/asset/aws/aws_asset.py` & `phidata-1.6.0/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/asset/data_asset.py` & `phidata-1.6.0/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/asset/local/file.py` & `phidata-1.6.0/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/asset/local/local_asset.py` & `phidata-1.6.0/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/api_client.py` & `phidata-1.6.0/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/athena/query.py` & `phidata-1.6.0/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/config.py` & `phidata-1.6.0/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.6.0/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/create/iam/role.py` & `phidata-1.6.0/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/enums/manager_status.py` & `phidata-1.6.0/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/manager.py` & `phidata-1.6.0/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/acm/certificate.py` & `phidata-1.6.0/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/athena/query.py` & `phidata-1.6.0/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/base.py` & `phidata-1.6.0/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.6.0/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/ec2/subnet.py` & `phidata-1.6.0/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/ec2/volume.py` & `phidata-1.6.0/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/ecs/cluster.py` & `phidata-1.6.0/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/ecs/container.py` & `phidata-1.6.0/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/ecs/service.py` & `phidata-1.6.0/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.6.0/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/ecs/volume.py` & `phidata-1.6.0/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/eks/addon.py` & `phidata-1.6.0/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/eks/cluster.py` & `phidata-1.6.0/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.6.0/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.6.0/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/eks/node_group.py` & `phidata-1.6.0/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.6.0/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.6.0/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/elb/listener.py` & `phidata-1.6.0/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.6.0/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/elb/target_group.py` & `phidata-1.6.0/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/emr/cluster.py` & `phidata-1.6.0/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/glue/crawler.py` & `phidata-1.6.0/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/group.py` & `phidata-1.6.0/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/iam/group.py` & `phidata-1.6.0/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/iam/policy.py` & `phidata-1.6.0/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/iam/role.py` & `phidata-1.6.0/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.6.0/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/rds/db_instance.py` & `phidata-1.6.0/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.6.0/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/s3/bucket.py` & `phidata-1.6.0/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/secret/manager.py` & `phidata-1.6.0/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/types.py` & `phidata-1.6.0/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/resource/utils.py` & `phidata-1.6.0/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/s3/csv_dataset.py` & `phidata-1.6.0/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/s3/dataset.py` & `phidata-1.6.0/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/s3/dataset_base.py` & `phidata-1.6.0/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/s3/object.py` & `phidata-1.6.0/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/aws/worker.py` & `phidata-1.6.0/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/base.py` & `phidata-1.6.0/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/checks/check.py` & `phidata-1.6.0/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/checks/not_empty.py` & `phidata-1.6.0/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/constants.py` & `phidata-1.6.0/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/decorators/timer.py` & `phidata-1.6.0/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/decorators/validate_env.py` & `phidata-1.6.0/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/api_client.py` & `phidata-1.6.0/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/args.py` & `phidata-1.6.0/phidata/docker/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from phidata.docker.resource.image import DockerImage
 from phidata.docker.resource.container import DockerContainer
 from phidata.docker.resource.volume import DockerVolume
 from phidata.docker.resource.group import DockerResourceGroup
 
 
 class DockerArgs(InfraArgs):
-    network: str = "phi"
+    network: str = "bridge"
     # configure the DockerClient
     # URL to the Docker server. For example, unix:///var/run/docker.sock or tcp://127.0.0.1:1234.
     # when None, phidata use DockerClient.from_env()
     base_url: Optional[str] = None
     apps: Optional[List[PhidataApp]] = None
     # default resources
     images: Optional[List[DockerImage]] = None
```

### Comparing `phidata-1.5.9/phidata/docker/config.py` & `phidata-1.6.0/phidata/docker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class DockerConfig(InfraConfig):
     def __init__(
         self,
         name: Optional[str] = None,
         env: Optional[str] = "dev",
         version: Optional[str] = None,
         enabled: bool = True,
-        network: str = "phi",
+        network: str = "bridge",
         base_url: Optional[str] = None,
         apps: Optional[List[PhidataApp]] = None,
         app_groups: Optional[List[AppGroup]] = None,
         images: Optional[List[DockerImage]] = None,
         containers: Optional[List[DockerContainer]] = None,
         volumes: Optional[List[DockerVolume]] = None,
         resources: Optional[List[DockerResourceGroup]] = None,
```

### Comparing `phidata-1.5.9/phidata/docker/enums.py` & `phidata-1.6.0/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/manager.py` & `phidata-1.6.0/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/base.py` & `phidata-1.6.0/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/container.py` & `phidata-1.6.0/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/group.py` & `phidata-1.6.0/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/image.py` & `phidata-1.6.0/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/network.py` & `phidata-1.6.0/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/types.py` & `phidata-1.6.0/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/utils.py` & `phidata-1.6.0/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/resource/volume.py` & `phidata-1.6.0/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/utils/container.py` & `phidata-1.6.0/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/docker/worker.py` & `phidata-1.6.0/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/infra/args.py` & `phidata-1.6.0/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/infra/config.py` & `phidata-1.6.0/phidata/infra/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,19 @@
         super().__init__()
         self.args: Optional[InfraArgs] = None
 
     @property
     def env(self) -> Optional[str]:
         return self.args.env if self.args else None
 
+    @env.setter
+    def env(self, env: str) -> None:
+        if self.args is not None and env is not None:
+            self.args.env = env
+
     @property
     def workspace_root_path(self) -> Optional[Path]:
         return self.args.workspace_root_path if self.args else None
 
     @workspace_root_path.setter
     def workspace_root_path(self, workspace_root_path: Path) -> None:
         if self.args is not None and workspace_root_path is not None:
```

### Comparing `phidata-1.5.9/phidata/infra/resource.py` & `phidata-1.6.0/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/api_client.py` & `phidata-1.6.0/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/args.py` & `phidata-1.6.0/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/config.py` & `phidata-1.6.0/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.6.0/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/common/port.py` & `phidata-1.6.0/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/container.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/secret.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/service.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/core/v1/volume.py` & `phidata-1.6.0/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.6.0/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/group.py` & `phidata-1.6.0/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/kubeconfig.py` & `phidata-1.6.0/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.6.0/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.0/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/enums/api_version.py` & `phidata-1.6.0/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/enums/kind.py` & `phidata-1.6.0/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/enums/manager_status.py` & `phidata-1.6.0/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/enums/pv.py` & `phidata-1.6.0/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/manager.py` & `phidata-1.6.0/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.6.0/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.6.0/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/base.py` & `phidata-1.6.0/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/container.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/service.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.6.0/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/group.py` & `phidata-1.6.0/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/kubeconfig.py` & `phidata-1.6.0/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.6.0/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.6.0/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.6.0/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.0/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/types.py` & `phidata-1.6.0/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/resource/utils.py` & `phidata-1.6.0/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/utils/pod.py` & `phidata-1.6.0/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/k8s/worker.py` & `phidata-1.6.0/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/llm/duckdb/agent.py` & `phidata-1.6.0/phidata/llm/duckdb/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         ),
     ]
 
     # Step 2: Initialize the agent
     agent = initialize_agent(
         tools,
         llm,
-        agent="zero-shot-react-description",
+        agent="zero-shot-react-description",  # type: ignore
         agent_kwargs={
             "input_variables": ["input", "agent_scratchpad", "table_names"],
             "prefix": prompt_prefix,
             "suffix": prompt_suffix,
         },
         # return_intermediate_steps=True,
         verbose=True,
```

### Comparing `phidata-1.5.9/phidata/llm/duckdb/chain.py` & `phidata-1.6.0/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/llm/duckdb/connection.py` & `phidata-1.6.0/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/llm/duckdb/loader.py` & `phidata-1.6.0/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/llm/duckdb/query.py` & `phidata-1.6.0/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/llm/duckdb/tool.py` & `phidata-1.6.0/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/product/data_product.py` & `phidata-1.6.0/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/local/csv.py` & `phidata-1.6.0/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/local/local_table.py` & `phidata-1.6.0/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/local/parquet.py` & `phidata-1.6.0/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/s3/csv.py` & `phidata-1.6.0/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/s3/parquet.py` & `phidata-1.6.0/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/s3/s3_table.py` & `phidata-1.6.0/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/sql/postgres.py` & `phidata-1.6.0/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/table/sql/sql_table.py` & `phidata-1.6.0/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/aws/athena/run_query.py` & `phidata-1.6.0/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/aws/emr/create_cluster.py` & `phidata-1.6.0/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.6.0/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/aws/glue/start_crawler.py` & `phidata-1.6.0/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/decorator.py` & `phidata-1.6.0/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/download/s3/to_file.py` & `phidata-1.6.0/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/download/url/to_file.py` & `phidata-1.6.0/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/download/url/to_s3.py` & `phidata-1.6.0/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/download/url/to_sql.py` & `phidata-1.6.0/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/plot/sql/query.py` & `phidata-1.6.0/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/python_task.py` & `phidata-1.6.0/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/run/sql/query.py` & `phidata-1.6.0/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/task.py` & `phidata-1.6.0/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/task_relatives.py` & `phidata-1.6.0/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/upload/file/to_s3.py` & `phidata-1.6.0/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/task/upload/file/to_sql.py` & `phidata-1.6.0/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/types/airflow.py` & `phidata-1.6.0/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/types/context.py` & `phidata-1.6.0/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/types/phidata_runtime.py` & `phidata-1.6.0/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/cli_console.py` & `phidata-1.6.0/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/common.py` & `phidata-1.6.0/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/compare.py` & `phidata-1.6.0/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/context.py` & `phidata-1.6.0/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/dttm.py` & `phidata-1.6.0/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/enums.py` & `phidata-1.6.0/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/env_file.py` & `phidata-1.6.0/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/env_var.py` & `phidata-1.6.0/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/filesystem.py` & `phidata-1.6.0/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/log.py` & `phidata-1.6.0/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/prep_infra_config.py` & `phidata-1.6.0/phidata/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/print_table.py` & `phidata-1.6.0/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/utils/workspace_path.py` & `phidata-1.6.0/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/workflow/decorator.py` & `phidata-1.6.0/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/workflow/workflow.py` & `phidata-1.6.0/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/workflow/workflow_relatives.py` & `phidata-1.6.0/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata/workspace/config.py` & `phidata-1.6.0/phidata/workspace/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -132,30 +132,55 @@
             logger.error(f"Args for {self.__class__.__name__} are not valid")
             raise
 
     @property
     def default_env(self) -> Optional[str]:
         return self.args.default_env if self.args else None
 
+    @default_env.setter
+    def default_env(self, default_env: str) -> None:
+        if self.args is not None and default_env is not None:
+            self.args.default_env = default_env
+
     @property
     def default_config(self) -> Optional[str]:
         return self.args.default_config if self.args else None
 
+    @default_config.setter
+    def default_config(self, default_config: str) -> None:
+        if self.args is not None and default_config is not None:
+            self.args.default_config = default_config
+
     @property
     def docker(self) -> Optional[List[Any]]:
         return self.args.docker if self.args else None
 
+    @docker.setter
+    def docker(self, docker: Any) -> None:
+        if self.args is not None and docker is not None:
+            self.args.docker = docker
+
     @property
     def k8s(self) -> Optional[List[Any]]:
         return self.args.k8s if self.args else None
 
+    @k8s.setter
+    def k8s(self, k8s: Any) -> None:
+        if self.args is not None and k8s is not None:
+            self.args.k8s = k8s
+
     @property
     def aws(self) -> Optional[List[Any]]:
         return self.args.aws if self.args else None
 
+    @aws.setter
+    def aws(self, aws: Any) -> None:
+        if self.args is not None and aws is not None:
+            self.args.aws = aws
+
     def is_valid(self) -> bool:
         if self.docker is not None:
             from phidata.docker.config import DockerConfig
 
             if not isinstance(self.docker, list):
                 raise ValueError("docker should be a list")
             for dc in self.docker:
```

### Comparing `phidata-1.5.9/phidata/workspace/settings.py` & `phidata-1.6.0/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.9/phidata.egg-info/PKG-INFO` & `phidata-1.6.0/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.5.9
+Version: 1.6.0
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.5.9 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.0 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.5.9/phidata.egg-info/SOURCES.txt` & `phidata-1.6.0/phidata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 phidata/app/nodeexporter/nodeexporter.py
 phidata/app/postgres/__init__.py
 phidata/app/postgres/postgres_db.py
 phidata/app/prometheus/__init__.py
 phidata/app/prometheus/prometheus.py
 phidata/app/redis/__init__.py
 phidata/app/redis/redis.py
+phidata/app/redis/stack.py
 phidata/app/server/__init__.py
 phidata/app/server/api_server.py
 phidata/app/server/app_server.py
 phidata/app/server/server_base.py
 phidata/app/spark/__init__.py
 phidata/app/spark/spark_base.py
 phidata/app/spark/spark_driver.py
```

### Comparing `phidata-1.5.9/pyproject.toml` & `phidata-1.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "phidata"
-version = "1.5.9"
+version = "1.6.0"
 description = "Building blocks for Data Engineering"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3",
-  "phiterm==1.5.9",
+  "phiterm==1.6.0",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
@@ -53,18 +53,20 @@
 module = [
   "git",
   "setuptools",
   "boto3",
   "boto3.*",
   "botocore",
   "botocore.*",
+  "duckdb.*",
   "typer",
   "tiingo",
   "docker.*",
   "airflow.*",
   "pandas.*",
   "pyarrow.*",
   "kubernetes.*",
+  "langchain.*",
   "sqlalchemy.*",
   "matplotlib.*",
 ]
 ignore_missing_imports = true
```

