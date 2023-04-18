# Comparing `tmp/mantik-0.1.2.tar.gz` & `tmp/mantik-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantik-0.1.2.tar", max compression
+gzip compressed data, was "mantik-0.2.0.tar", max compression
```

## Comparing `mantik-0.1.2.tar` & `mantik-0.2.0.tar`

### file list

```diff
@@ -1,100 +1,177 @@
--rw-r--r--   0        0        0     1247 2022-11-25 09:34:39.569670 mantik-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      217 2022-11-25 09:22:58.618321 mantik-0.1.2/src/mantik/__init__.py
--rw-r--r--   0        0        0       69 2022-11-15 09:00:00.488723 mantik-0.1.2/src/mantik/cli/__init__.py
--rw-r--r--   0        0        0     1230 2022-11-15 09:00:00.488723 mantik-0.1.2/src/mantik/cli/init.py
--rw-r--r--   0        0        0       71 2022-11-15 09:00:00.488723 mantik-0.1.2/src/mantik/cli/main.py
--rw-r--r--   0        0        0      234 2022-11-15 10:05:00.171315 mantik-0.1.2/src/mantik/cli/runs/__init__.py
--rw-r--r--   0        0        0       88 2022-11-15 09:00:00.488723 mantik-0.1.2/src/mantik/cli/runs/_arguments.py
--rw-r--r--   0        0        0      659 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/_callbacks.py
--rw-r--r--   0        0        0     1501 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/_options.py
--rw-r--r--   0        0        0      722 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/cancel.py
--rw-r--r--   0        0        0     1595 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/download.py
--rw-r--r--   0        0        0     1152 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/info.py
--rw-r--r--   0        0        0     2668 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/list.py
--rw-r--r--   0        0        0      722 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/logs.py
--rw-r--r--   0        0        0      116 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/runs.py
--rw-r--r--   0        0        0      695 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/status.py
--rw-r--r--   0        0        0     3017 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/cli/runs/submit.py
--rw-r--r--   0        0        0      269 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/__init__.py
--rw-r--r--   0        0        0     1738 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/_bearer.py
--rw-r--r--   0        0        0     2694 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/api.py
--rw-r--r--   0        0        0      676 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/app.py
--rw-r--r--   0        0        0     3221 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/backend.py
--rw-r--r--   0        0        0     7407 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/client.py
--rw-r--r--   0        0        0      722 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/exceptions.py
--rw-r--r--   0        0        0      324 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/compute_backend_service/models.py
--rw-r--r--   0        0        0        0 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/__init__.py
--rw-r--r--   0        0        0      126 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/__init__.py
--rw-r--r--   0        0        0     1160 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/_header.py
--rw-r--r--   0        0        0       90 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/__init__.py
--rw-r--r--   0        0        0       85 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/_exceptions.py
--rw-r--r--   0        0        0     1339 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/_get.py
--rw-r--r--   0        0        0      454 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/health.py
--rw-r--r--   0        0        0      109 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/models/__init__.py
--rw-r--r--   0        0        0     1327 2022-11-15 09:00:00.492723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/models/requests.py
--rw-r--r--   0        0        0     1341 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/models/responses.py
--rw-r--r--   0        0        0     1870 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/flask/api/tokens.py
--rw-r--r--   0        0        0       46 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/flask/app.py
--rw-r--r--   0        0        0     1795 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/flask/before_requests.py
--rw-r--r--   0        0        0      722 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/flask/skip.py
--rw-r--r--   0        0        0       41 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/gunicorn/__init__.py
--rw-r--r--   0        0        0     1277 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_app.py
--rw-r--r--   0        0        0      882 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_cli_args.py
--rw-r--r--   0        0        0      614 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_env.py
--rw-r--r--   0        0        0      364 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_options.py
--rw-r--r--   0        0        0      961 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_stores.py
--rw-r--r--   0        0        0      508 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/gunicorn/run.py
--rw-r--r--   0        0        0      212 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/__init__.py
--rw-r--r--   0        0        0      256 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/__init__.py
--rw-r--r--   0        0        0     3404 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/_auth.py
--rw-r--r--   0        0        0     1532 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/api.py
--rw-r--r--   0        0        0     2053 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/client.py
--rw-r--r--   0        0        0     1659 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/credentials.py
--rw-r--r--   0        0        0      218 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/exceptions.py
--rw-r--r--   0        0        0     1250 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/tokens.py
--rw-r--r--   0        0        0      604 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/exceptions.py
--rw-r--r--   0        0        0     2126 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/jwks.py
--rw-r--r--   0        0        0     3247 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/jwt.py
--rw-r--r--   0        0        0     3688 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/mlflow_server/tokens/verifier.py
--rw-r--r--   0        0        0      243 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/testing/__init__.py
--rw-r--r--   0        0        0     8518 2022-11-15 09:00:00.496723 mantik-0.1.2/src/mantik/testing/cognito.py
--rw-r--r--   0        0        0     2440 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/testing/config.py
--rw-r--r--   0        0        0      601 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/testing/contexts.py
--rw-r--r--   0        0        0     1251 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/testing/env.py
--rw-r--r--   0        0        0    12408 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/testing/mlflow_server.py
--rw-r--r--   0        0        0     6724 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/testing/pyunicore.py
--rw-r--r--   0        0        0      927 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/testing/requests.py
--rw-r--r--   0        0        0     1110 2022-11-25 09:22:58.618321 mantik-0.1.2/src/mantik/testing/token.py
--rw-r--r--   0        0        0       64 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/tracking/__init__.py
--rw-r--r--   0        0        0       73 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/tracking/_server/__init__.py
--rw-r--r--   0        0        0     1259 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/tracking/_server/_credentials.py
--rw-r--r--   0        0        0     3182 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/tracking/_server/api.py
--rw-r--r--   0        0        0     2591 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/tracking/_server/tokens.py
--rw-r--r--   0        0        0      920 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/tracking/environment.py
--rw-r--r--   0        0        0     2017 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/tracking/track.py
--rw-r--r--   0        0        0      250 2022-11-15 10:05:00.171315 mantik-0.1.2/src/mantik/unicore/__init__.py
--rw-r--r--   0        0        0     2352 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/unicore/_connect.py
--rw-r--r--   0        0        0     7759 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/unicore/backend.py
--rw-r--r--   0        0        0     3185 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/unicore/client.py
--rw-r--r--   0        0        0      188 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/unicore/config/__init__.py
--rw-r--r--   0        0        0      535 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/unicore/config/_base.py
--rw-r--r--   0        0        0     2785 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/unicore/config/_utils.py
--rw-r--r--   0        0        0     4423 2022-11-15 09:00:00.500723 mantik-0.1.2/src/mantik/unicore/config/core.py
--rw-r--r--   0        0        0     2554 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/config/environment.py
--rw-r--r--   0        0        0     6561 2022-11-15 10:05:00.171315 mantik-0.1.2/src/mantik/unicore/config/executable.py
--rw-r--r--   0        0        0      830 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/config/read.py
--rw-r--r--   0        0        0     2739 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/config/resources.py
--rw-r--r--   0        0        0      495 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/exceptions.py
--rw-r--r--   0        0        0     3457 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/job.py
--rw-r--r--   0        0        0     5644 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/properties.py
--rw-r--r--   0        0        0     2945 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/submitted_run.py
--rw-r--r--   0        0        0       67 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/utils/__init__.py
--rw-r--r--   0        0        0     1998 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/utils/upload.py
--rw-r--r--   0        0        0      763 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/utils/zip.py
--rw-r--r--   0        0        0     4054 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/unicore/working_dir.py
--rw-r--r--   0        0        0       76 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/utils/__init__.py
--rw-r--r--   0        0        0     2151 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/utils/env.py
--rw-r--r--   0        0        0      471 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/utils/mlflow.py
--rw-r--r--   0        0        0      282 2022-11-15 09:00:00.504723 mantik-0.1.2/src/mantik/utils/urls.py
--rw-r--r--   0        0        0     1637 2022-11-25 09:34:40.339916 mantik-0.1.2/setup.py
--rw-r--r--   0        0        0      991 2022-11-25 09:34:40.340151 mantik-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-18 14:25:32.607202 mantik-0.2.0/LICENSE
+-rw-r--r--   0        0        0      506 2023-04-18 14:25:32.607202 mantik-0.2.0/README.md
+-rw-r--r--   0        0        0     1925 2023-04-18 14:25:32.627204 mantik-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/__init__.py
+-rw-r--r--   0        0        0       69 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/__init__.py
+-rw-r--r--   0        0        0     1241 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/init.py
+-rw-r--r--   0        0        0       71 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/main.py
+-rw-r--r--   0        0        0      234 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/_arguments.py
+-rw-r--r--   0        0        0      659 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/_callbacks.py
+-rw-r--r--   0        0        0     1427 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/_options.py
+-rw-r--r--   0        0        0      723 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/cancel.py
+-rw-r--r--   0        0        0     1608 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/download.py
+-rw-r--r--   0        0        0     1153 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/info.py
+-rw-r--r--   0        0        0     2669 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/list.py
+-rw-r--r--   0        0        0      723 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/logs.py
+-rw-r--r--   0        0        0      116 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/runs.py
+-rw-r--r--   0        0        0      696 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/status.py
+-rw-r--r--   0        0        0     3026 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/submit.py
+-rw-r--r--   0        0        0      316 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/_bearer.py
+-rw-r--r--   0        0        0     3486 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/api.py
+-rw-r--r--   0        0        0     1648 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/app.py
+-rw-r--r--   0        0        0     3251 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/backend.py
+-rw-r--r--   0        0        0     8072 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/client.py
+-rw-r--r--   0        0        0     3297 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/exceptions.py
+-rw-r--r--   0        0        0      324 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/models.py
+-rw-r--r--   0        0        0     1196 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/settings.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/__init__.py
+-rw-r--r--   0        0        0      126 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/__init__.py
+-rw-r--r--   0        0        0     1160 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/_header.py
+-rw-r--r--   0        0        0       90 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/_exceptions.py
+-rw-r--r--   0        0        0     1339 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/_get.py
+-rw-r--r--   0        0        0      455 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/health.py
+-rw-r--r--   0        0        0      109 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/__init__.py
+-rw-r--r--   0        0        0     1328 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/requests.py
+-rw-r--r--   0        0        0     1342 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/responses.py
+-rw-r--r--   0        0        0     1871 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/tokens.py
+-rw-r--r--   0        0        0       46 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/app.py
+-rw-r--r--   0        0        0     1796 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/before_requests.py
+-rw-r--r--   0        0        0      722 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/skip.py
+-rw-r--r--   0        0        0       41 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/__init__.py
+-rw-r--r--   0        0        0     1278 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_app.py
+-rw-r--r--   0        0        0      882 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_cli_args.py
+-rw-r--r--   0        0        0      614 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_env.py
+-rw-r--r--   0        0        0      364 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_options.py
+-rw-r--r--   0        0        0      961 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_stores.py
+-rw-r--r--   0        0        0      508 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/run.py
+-rw-r--r--   0        0        0      212 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/__init__.py
+-rw-r--r--   0        0        0     3612 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/_auth.py
+-rw-r--r--   0        0        0     1532 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/api.py
+-rw-r--r--   0        0        0     2053 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/client.py
+-rw-r--r--   0        0        0     1659 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/credentials.py
+-rw-r--r--   0        0        0      218 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/exceptions.py
+-rw-r--r--   0        0        0     1250 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/tokens.py
+-rw-r--r--   0        0        0      604 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/exceptions.py
+-rw-r--r--   0        0        0     2127 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/jwks.py
+-rw-r--r--   0        0        0     3248 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/jwt.py
+-rw-r--r--   0        0        0     3688 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/mlflow_server/tokens/verifier.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/py.typed
+-rw-r--r--   0        0        0      243 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/__init__.py
+-rw-r--r--   0        0        0     8518 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/cognito.py
+-rw-r--r--   0        0        0     2438 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/config.py
+-rw-r--r--   0        0        0      601 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/contexts.py
+-rw-r--r--   0        0        0     1251 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/env.py
+-rw-r--r--   0        0        0    12408 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/mlflow_server.py
+-rw-r--r--   0        0        0     6725 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/pyunicore.py
+-rw-r--r--   0        0        0      927 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/requests.py
+-rw-r--r--   0        0        0     1110 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/token.py
+-rw-r--r--   0        0        0       64 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/__init__.py
+-rw-r--r--   0        0        0       73 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/__init__.py
+-rw-r--r--   0        0        0     1259 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/_credentials.py
+-rw-r--r--   0        0        0     3183 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/api.py
+-rw-r--r--   0        0        0     2586 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/tokens.py
+-rw-r--r--   0        0        0      920 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/environment.py
+-rw-r--r--   0        0        0     2017 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/track.py
+-rw-r--r--   0        0        0      250 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/unicore/__init__.py
+-rw-r--r--   0        0        0     2799 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/unicore/_connect.py
+-rw-r--r--   0        0        0     7939 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/backend.py
+-rw-r--r--   0        0        0     3190 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/client.py
+-rw-r--r--   0        0        0      226 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/_base.py
+-rw-r--r--   0        0        0     2776 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/_utils.py
+-rw-r--r--   0        0        0     3886 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/core.py
+-rw-r--r--   0        0        0     2876 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/environment.py
+-rw-r--r--   0        0        0     7445 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/executable.py
+-rw-r--r--   0        0        0     1072 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/read.py
+-rw-r--r--   0        0        0     2739 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/resources.py
+-rw-r--r--   0        0        0     3895 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/validate.py
+-rw-r--r--   0        0        0      542 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/exceptions.py
+-rw-r--r--   0        0        0     3458 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/job.py
+-rw-r--r--   0        0        0     5644 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/properties.py
+-rw-r--r--   0        0        0     2946 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/submitted_run.py
+-rw-r--r--   0        0        0       67 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/utils/__init__.py
+-rw-r--r--   0        0        0     1997 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/utils/upload.py
+-rw-r--r--   0        0        0      763 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/utils/zip.py
+-rw-r--r--   0        0        0     4054 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/working_dir.py
+-rw-r--r--   0        0        0      105 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/utils/__init__.py
+-rw-r--r--   0        0        0     2151 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/utils/env.py
+-rw-r--r--   0        0        0      471 2023-04-18 14:25:32.632205 mantik-0.2.0/src/mantik/utils/mlflow.py
+-rw-r--r--   0        0        0      615 2023-04-18 14:25:32.632205 mantik-0.2.0/src/mantik/utils/temp_dir.py
+-rw-r--r--   0        0        0      320 2023-04-18 14:25:32.632205 mantik-0.2.0/src/mantik/utils/urls.py
+-rw-r--r--   0        0        0      163 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/broken-project/MLproject
+-rw-r--r--   0        0        0       77 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/broken-project/README.md
+-rw-r--r--   0        0        0      248 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/broken-project/unicore-config.md
+-rw-r--r--   0        0        0      574 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/auth-response.json
+-rw-r--r--   0        0        0      159 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/different-client.json
+-rw-r--r--   0        0        0      649 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/incorrect-login-credentials-response.json
+-rw-r--r--   0        0        0      578 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/refresh-response.json
+-rw-r--r--   0        0        0      631 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/refresh-token-expired-response.json
+-rw-r--r--   0        0        0      623 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/refresh-token-invalid-response.json
+-rw-r--r--   0        0        0      614 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/user-not-found-response.json
+-rw-r--r--   0        0        0       57 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/Dockerfile
+-rw-r--r--   0        0        0      182 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/MLproject
+-rw-r--r--   0        0        0      168 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/config-with-errors.yaml
+-rw-r--r--   0        0        0      536 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/main.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/mantik-test.sif
+-rw-r--r--   0        0        0       50 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/recipe.def
+-rw-r--r--   0        0        0        0 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/test_subfolder/test.py
+-rw-r--r--   0        0        0      246 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/unicore-config.json
+-rw-r--r--   0        0        0      193 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/unicore-config.yaml
+-rw-r--r--   0        0        0     2879 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/unicore-responses/job-property-response.json
+-rw-r--r--   0        0        0      193 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/unit/cli/conftest.py
+-rw-r--r--   0        0        0      537 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/conftest.py
+-rw-r--r--   0        0        0      555 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_cancel.py
+-rw-r--r--   0        0        0     3201 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_download.py
+-rw-r--r--   0        0        0     3506 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_info.py
+-rw-r--r--   0        0        0      831 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_list.py
+-rw-r--r--   0        0        0     1564 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_logs.py
+-rw-r--r--   0        0        0      823 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_options.py
+-rw-r--r--   0        0        0     1560 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_status.py
+-rw-r--r--   0        0        0     5434 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_submit.py
+-rw-r--r--   0        0        0      780 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/test_init.py
+-rw-r--r--   0        0        0     3920 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/conftest.py
+-rw-r--r--   0        0        0     5719 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_api.py
+-rw-r--r--   0        0        0      738 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_app.py
+-rw-r--r--   0        0        0     3175 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_client.py
+-rw-r--r--   0        0        0     1168 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_compute_backend.py
+-rw-r--r--   0        0        0     8638 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_exception_handler.py
+-rw-r--r--   0        0        0      327 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_models.py
+-rw-r--r--   0        0        0     1479 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1585 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/mlflow_server/conftest.py
+-rw-r--r--   0        0        0      191 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/api/test_health_api.py
+-rw-r--r--   0        0        0     4375 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/api/test_tokens_api.py
+-rw-r--r--   0        0        0      607 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/conftest.py
+-rw-r--r--   0        0        0      894 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/test_flask_app.py
+-rw-r--r--   0        0        0      469 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/test_skip.py
+-rw-r--r--   0        0        0      391 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/gunicorn/test_run.py
+-rw-r--r--   0        0        0     4139 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/tokens/cognito/test_auth.py
+-rw-r--r--   0        0        0     2807 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/tokens/test_verifier.py
+-rw-r--r--   0        0        0     3121 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/_server/test_server_api.py
+-rw-r--r--   0        0        0     1123 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/_server/test_tokens.py
+-rw-r--r--   0        0        0     1838 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/test_credentials.py
+-rw-r--r--   0        0        0     5525 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/test_track.py
+-rw-r--r--   0        0        0     1211 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/conftest.py
+-rw-r--r--   0        0        0    10055 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_core.py
+-rw-r--r--   0        0        0     3136 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_environment.py
+-rw-r--r--   0        0        0     1765 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_executable.py
+-rw-r--r--   0        0        0     1945 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_read.py
+-rw-r--r--   0        0        0     2981 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_utils.py
+-rw-r--r--   0        0        0     8372 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_validate.py
+-rw-r--r--   0        0        0     2629 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/conftest.py
+-rw-r--r--   0        0        0     4259 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_backend.py
+-rw-r--r--   0        0        0     1231 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_client_wrapper.py
+-rw-r--r--   0        0        0     1870 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_connect.py
+-rw-r--r--   0        0        0      516 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_exceptions.py
+-rw-r--r--   0        0        0     1551 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_properties.py
+-rw-r--r--   0        0        0     3707 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_submitted_run.py
+-rw-r--r--   0        0        0     4240 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/utils/test_upload.py
+-rw-r--r--   0        0        0      775 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/conftest.py
+-rw-r--r--   0        0        0      736 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/test_env.py
+-rw-r--r--   0        0        0      285 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/test_temp_dir.py
+-rw-r--r--   0        0        0      633 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/test_urls.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 mantik-0.2.0/setup.py
+-rw-r--r--   0        0        0     1984 1970-01-01 00:00:00.000000 mantik-0.2.0/PKG-INFO
```

### Comparing `mantik-0.1.2/pyproject.toml` & `mantik-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 [tool.poetry]
 name = "mantik"
-version = "0.1.2"
+version = "0.2.0"
 description = "mantik for mlflow"
 authors = [
     "Fabian Emmerich <fabian.emmerich@4-cast.de>",
-    "Thomas Seidler <thomas.seider@ambrosys.de>"
+    "Thomas Seidler <thomas.seidler@ambrosys.de>",
+]
+maintainers = [
+    "Elia Boscaini <elia.boscaini@ambrosys.de>",
+    "Kristian Ehlert <kristian.ehlert@4-cast.de>",
 ]
 packages = [{ include = "mantik", from = "src"}]
+include = [
+    { path = "src/tests", format = "sdist" }
+]
+readme = "README.md"
+license = "MIT"
 homepage = "https://mantik.ai/"
+repository = "https://gitlab.com/mantik-ai/mantik"
+documentation = "https://mantik-ai.gitlab.io/mantik"
 keywords = ["mlflow", "machine learning", "hpc", "unicore"]
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+]
 
 [tool.poetry.scripts]
 mantik = 'mantik.cli.main:cli'
 
 [tool.poetry.plugins."mlflow.project_backend"]
 "unicore" = "mantik.unicore.backend:UnicoreBackend"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-mlflow = "1.30.0"
+python = "^3.8"
+mlflow = "2.2.2"
 pyunicore = "^0.9.16"
 fastapi = "^0.78.0"
 requests = "^2.27.1"
 pydantic = "^1.9.0"
 python-multipart = "^0.0.5"
 uvicorn = {extras = ["standard"], version = "^0.17.6"}
 boto3 = "^1.23.6"
@@ -34,20 +51,27 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.17.0"
 fastapi = {extras = ["testclient"], version = "^0.78.0"}
 freezegun = "^1.2.1"
 requests-mock = "^1.9.3"
+pytest-custom-exit-code = "^0.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--cov=mantik --cov-report term-missing"
 
 [tool.black]
 line-length = 80
 
+[tool.flake8]
+max-line-length = 80
+per-file-ignores = [
+    "__init__.py:F401,E501",
+]
+
 [mypy]
 ignore_missing_imports = true
```

### Comparing `mantik-0.1.2/src/mantik/cli/init.py` & `mantik-0.2.0/src/mantik/cli/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+
 import mantik.cli.main as main
 import mantik.tracking.track as track
 
 
 @main.cli.command("init")
 @click.option(
     "--no-export",
@@ -19,24 +20,24 @@
     (or shell) from a subprocess (e.g. Python). Thus, the `init` command prints
     the bash export statement with the required environment variable for
     tracking to mantik. As a consequence, the output can be directly used to set
     the environment variable in the parent process by using the `eval` bash
     command:
 
     \b
-    ```
+    ```shell
     eval $(mantik init)
     ```
 
     If you do not want to set the environment variable in the parent process
     but only want to pass it to the command context, use the `env` bash command
     combined with the `--no-export` flag:
 
     \b
-    ```
+    ```shell
     env $(mantik init --no-export) <command>
     ```
 
     """
     environment = track.init_tracking()
 
     click.echo(environment.to_bash_statement(no_export=no_export))
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/_callbacks.py` & `mantik-0.2.0/src/mantik/cli/runs/_callbacks.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/cli/runs/_options.py` & `mantik-0.2.0/src/mantik/cli/runs/_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,46 +8,42 @@
         self.not_required_if = kwargs.pop("not_required_if")
         assert self.not_required_if, "'not_required_if' parameter required"
         kwargs["help"] = (
             f"{kwargs.get('help', '')} "
             f"NOTE: This argument is mutually "
             f"exclusive with {self.not_required_if}"
         )
-        super(NotRequiredIf, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         we_are_present = self.name in opts
         other_present = self.not_required_if in opts
 
         if other_present:
             if we_are_present:
                 raise click.UsageError(
                     f"Illegal usage: `{self.name}` is mutually "
                     f"exclusive with `{self.not_required_if}`"
                 )
             else:
                 self.prompt = None
 
-        return super(NotRequiredIf, self).handle_parse_result(ctx, opts, args)
+        return super().handle_parse_result(ctx, opts, args)
 
 
 API_URL = click.option(
     "--api-url",
     type=str,
     required=False,
     default=None,
-    help="""
-        UNICORE API URL.
-    """,
+    help="UNICORE API URL.",
 )
 BACKEND_CONFIG_ABSOLUTE = click.option(
     "--backend-config",
     type=click.Path(dir_okay=False, resolve_path=True, path_type=pathlib.Path),
     required=False,
     default=None,
     prompt=True,
     cls=NotRequiredIf,
     not_required_if="api_url",
-    help="""
-        Absolute path to the backend config to read the API URL from.
-    """,
+    help="Absolute path to the backend config to read the API URL from.",
 )
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/cancel.py` & `mantik-0.2.0/src/mantik/cli/runs/status.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pathlib
 import typing as t
 
 import click
+
 import mantik.cli.runs._arguments as _arguments
 import mantik.cli.runs._options as _options
 import mantik.cli.runs.runs as runs
 import mantik.unicore as unicore
 
 
-@runs.cli.command("cancel")
+@runs.cli.command("status")
 @_arguments.JOB_ID
 @_options.API_URL
 @_options.BACKEND_CONFIG_ABSOLUTE
-def cancel_job(
+def print_status(
     job_id: str,
     api_url: t.Optional[str],
     backend_config: t.Optional[pathlib.Path],
 ) -> None:
-    """Cancel a submitted job.
+    """Print the run status.
 
     JOB_ID is the job ID assigned by UNICORE.
 
     """
     client = unicore.client.Client.from_api_url_or_config(
         api_url=api_url, config=backend_config
     )
     job = client.get_job(job_id)
-    job.cancel()
-    click.echo(f"Cancelled job {job_id}.")
+    click.echo(job.status.value)
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/download.py` & `mantik-0.2.0/src/mantik/cli/runs/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 import typing as t
 
 import click
+
 import mantik.cli.runs._arguments as _arguments
 import mantik.cli.runs._options as _options
 import mantik.cli.runs.runs as runs
 import mantik.unicore as unicore
 
 
 @runs.cli.command("download")
@@ -13,16 +14,18 @@
 @_options.API_URL
 @_options.BACKEND_CONFIG_ABSOLUTE
 @click.option(
     "--remote-path",
     type=click.Path(path_type=pathlib.Path),
     required=False,
     default=None,
-    help="Path of file or subdir in working directory, "
-    "if not defined the whole working directory is downloaded",
+    help="""Path of file or subdir in working directory.
+
+        If not defined the whole working directory is downloaded.
+    """,
 )
 @click.option(
     "--local-path",
     type=click.Path(writable=True, path_type=pathlib.Path),
     default=".",
     required=False,
     show_default=True,
@@ -31,15 +34,15 @@
 def download_file_or_directory(
     job_id: str,
     api_url: t.Optional[str],
     backend_config: t.Optional[pathlib.Path],
     remote_path: t.Optional[pathlib.Path],
     local_path: t.Optional[pathlib.Path],
 ) -> None:
-    """Download a file or folder from a job's working directory.
+    """Download a file or folder from a run's working directory.
 
     JOB_ID is the job ID assigned by UNICORE.
 
     """
 
     client = unicore.client.Client.from_api_url_or_config(
         api_url=api_url, config=backend_config
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/info.py` & `mantik-0.2.0/src/mantik/cli/runs/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 import typing as t
 
 import click
+
 import mantik.cli.runs._arguments as _arguments
 import mantik.cli.runs._options as _options
 import mantik.cli.runs.runs as runs
 import mantik.unicore as unicore
 
 
 @runs.cli.command("info")
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/list.py` & `mantik-0.2.0/src/mantik/cli/runs/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 import typing as t
 
 import click
+
 import mantik.cli.runs._callbacks as _callbacks
 import mantik.cli.runs._options as _options
 import mantik.cli.runs.runs as runs
 import mantik.unicore as unicore
 
 
 @runs.cli.command("list")
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/logs.py` & `mantik-0.2.0/src/mantik/cli/runs/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 import typing as t
 
 import click
+
 import mantik.cli.runs._arguments as _arguments
 import mantik.cli.runs._options as _options
 import mantik.cli.runs.runs as runs
 import mantik.unicore as unicore
 
 
 @runs.cli.command("logs")
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/status.py` & `mantik-0.2.0/src/mantik/cli/runs/cancel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import pathlib
 import typing as t
 
 import click
+
 import mantik.cli.runs._arguments as _arguments
 import mantik.cli.runs._options as _options
 import mantik.cli.runs.runs as runs
 import mantik.unicore as unicore
 
 
-@runs.cli.command("status")
+@runs.cli.command("cancel")
 @_arguments.JOB_ID
 @_options.API_URL
 @_options.BACKEND_CONFIG_ABSOLUTE
-def print_status(
+def cancel_job(
     job_id: str,
     api_url: t.Optional[str],
     backend_config: t.Optional[pathlib.Path],
 ) -> None:
-    """Print the run status.
+    """Cancel a submitted run.
 
     JOB_ID is the job ID assigned by UNICORE.
 
     """
     client = unicore.client.Client.from_api_url_or_config(
         api_url=api_url, config=backend_config
     )
     job = client.get_job(job_id)
-    click.echo(job.status.value)
+    job.cancel()
+    click.echo(f"Cancelled job {job_id}.")
```

### Comparing `mantik-0.1.2/src/mantik/cli/runs/submit.py` & `mantik-0.2.0/src/mantik/cli/runs/submit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import ast
 import pathlib
 import typing as t
 
 import click
+
 import mantik
 import mantik.cli.runs.runs as runs
 import mantik.compute_backend_service.client as compute_backend_client
 import mantik.utils as utils
 
 
 def set_logging_callback(ctx, param, value) -> None:  # noqa
@@ -26,19 +27,19 @@
     type=click.Path(exists=True, file_okay=False, path_type=pathlib.Path),
     required=True,
 )
 @click.option(
     "--experiment-id",
     default=None,
     type=int,
-    help=f"""
-        Experiment ID on MLflow.
+    help=f"""Experiment ID on MLflow.
 
         If not specified, it is inferred from the environment variable
         {utils.mlflow.EXPERIMENT_ID_ENV_VAR}.
+
     """,
 )
 @click.option(
     "--entry-point",
     required=False,
     default="main",
     show_default=True,
@@ -46,15 +47,17 @@
 )
 @click.option(
     "--backend-config",
     type=click.Path(dir_okay=False, path_type=pathlib.Path),
     required=True,
     help="Relative path to backend config file.",
 )
-@click.option("--parameter", "-P", show_default=True, default=[], multiple=True)
+@click.option(
+    "--parameter", "-P", show_default=True, default=lambda: [], multiple=True
+)
 @click.option(
     "--verbose",
     "-v",
     is_flag=True,
     callback=set_logging_callback,
     help="Set logging to verbose mode.",
 )
@@ -64,15 +67,15 @@
     entry_point: str,
     backend_config: pathlib.Path,
     parameter: t.List[str],
     verbose: bool,  # noqa
 ) -> None:
     """Submit an MLflow project as a run to the Mantik Compute Backend.
 
-    MLPROJECT_PATH is the path to the MLflow project folder.
+    `MLPROJECT_PATH` is the path to the MLflow project folder.
 
     """
     if experiment_id is None:
         experiment_id = utils.env.get_required_env_var(
             utils.mlflow.EXPERIMENT_ID_ENV_VAR
         )
     client = mantik.ComputeBackendClient.from_env()
```

### Comparing `mantik-0.1.2/src/mantik/compute_backend_service/_bearer.py` & `mantik-0.2.0/src/mantik/compute_backend_service/_bearer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing as t
 
 import fastapi
 import fastapi.security as security
-import mantik.mlflow_server.tokens as _tokens
 import starlette.requests as requests
 import starlette.status as status
 
+import mantik.mlflow_server.tokens as _tokens
+
 
 class UnauthorizedException(fastapi.HTTPException):
     """Authentication has failed."""
 
     def __init__(
         self,
         detail: str,
```

### Comparing `mantik-0.1.2/src/mantik/compute_backend_service/app.py` & `mantik-0.2.0/src/tests/unit/compute_backend_service/test_app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import fastapi
-import mantik.compute_backend_service.api as api
-import mantik.compute_backend_service.exceptions as exceptions
-import mantik.unicore.exceptions as unicore_exceptions
 
+import mantik.compute_backend_service.app as _app
+import mantik.compute_backend_service.exceptions as _exceptions
 
-def create_app(
-    docs_url: str, redoc_url: str, openapi_url: str, global_path_prefix: str
-) -> fastapi.FastAPI:
-    app = fastapi.FastAPI(
-        docs_url=global_path_prefix + docs_url,
-        redoc_url=global_path_prefix + redoc_url,
-        openapi_url=global_path_prefix + openapi_url,
-    )
-    app.include_router(api.router, prefix=global_path_prefix)
-    app.add_exception_handler(
-        unicore_exceptions.UnicoreError, exceptions.unicore_exception_handler
+
+def test_create_app():
+    global_path_prefix = "/fizzbuzz"
+    docs_url = "/foo"
+    app = _app.create_app(
+        docs_url=docs_url,
+        redoc_url="/bar",
+        openapi_url="/baz.json",
+        global_path_prefix=global_path_prefix,
     )
-    return app
+    assert isinstance(app, fastapi.FastAPI)
+    route_paths = [route.path for route in app.routes]
+    assert f"{global_path_prefix}/submit/{{experiment_id}}" in route_paths
+    assert global_path_prefix + docs_url in route_paths
+    exception_handlers = app.exception_handlers
+    assert _exceptions.unicore_exception_handler in exception_handlers.values()
```

### Comparing `mantik-0.1.2/src/mantik/compute_backend_service/backend.py` & `mantik-0.2.0/src/mantik/compute_backend_service/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Backend implementation."""
 import pathlib
-import tempfile
 import typing as t
 import zipfile
 
+import mlflow.projects
+
 import mantik.compute_backend_service.models as models
 import mantik.unicore.config.core as core
 import mantik.unicore.config.read as read
 import mantik.utils as utils
-import mlflow.projects
 
 
+@utils.temp_dir.use_temp_dir
 def handle_submit_run_request(
     experiment_id: str,
     entry_point: str,
     mlflow_parameters: t.Dict,
     unicore_user: str,
     unicore_project: str,
     unicore_password: str,
     unicore_backend_config: str,
     mlflow_tracking_uri: str,
     mlflow_tracking_token: str,
     mlproject_zip: t.BinaryIO,
+    temp_dir_name: t.Optional[str] = None,
 ) -> models.SubmitRunResponse:
     """
     Handle the submit run request.
 
     Parameters
     ----------
     experiment_id: experiment id.
@@ -35,36 +37,37 @@
     unicore_project: UNICORE compute project.
     unicore_password: UNICORE password.
     unicore_backend_config: Path to unicore backend config in the zipped
       mlflow project.
     mlflow_tracking_uri: Tracking URI.
     mlflow_tracking_token: Token to permit access to tracking API.
     mlproject_zip: file like object holding zipped mlproject directory.
-
+    temp_dir_name: temporary directory name, used for testing
     Returns
     -------
     Submit run response.
     """
     env_vars = _create_required_env_vars(
         unicore_user=unicore_user,
         unicore_password=unicore_password,
         unicore_project=unicore_project,
         mlflow_tracking_uri=mlflow_tracking_uri,
         experiment_id=experiment_id,
         mlflow_tracking_token=mlflow_tracking_token,
     )
     with utils.env.env_vars_set(env_vars):
-        mlproject_dir = _unzip_to_tmp(mlproject_zip)
+        _unzip_to_file(mlproject_zip, temp_dir_name)
         backend_config = pathlib.Path(
-            f"{mlproject_dir.name}/{unicore_backend_config}"
+            f"{temp_dir_name}/{unicore_backend_config}"
         )
-        # Note: If version is not handed to run method, mlflow throws an error
+        # Note: If version is not handed to run method,
+        # mlflow throws an error
         version = None
         submitted_run = mlflow.projects.run(
-            mlproject_dir.name,
+            temp_dir_name,
             entry_point,
             version,
             experiment_id=experiment_id,
             parameters=mlflow_parameters,
             backend="unicore",
             backend_config=read.read_config(backend_config),
             synchronous=False,
@@ -90,12 +93,10 @@
         core._PASSWORD_ENV_VAR: unicore_password,
         utils.mlflow.TRACKING_URI_ENV_VAR: mlflow_tracking_uri,
         utils.mlflow.EXPERIMENT_ID_ENV_VAR: experiment_id,
         utils.mlflow.TRACKING_TOKEN_ENV_VAR: mlflow_tracking_token,
     }
 
 
-def _unzip_to_tmp(zipped: t.BinaryIO) -> tempfile.TemporaryDirectory:
-    directory = tempfile.TemporaryDirectory()
+def _unzip_to_file(zipped: t.BinaryIO, file: str) -> None:
     with zipfile.ZipFile(zipped, "r") as zip_ref:
-        zip_ref.extractall(directory.name)
-    return directory
+        zip_ref.extractall(file)
```

### Comparing `mantik-0.1.2/src/mantik/compute_backend_service/client.py` & `mantik-0.2.0/src/mantik/compute_backend_service/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import dataclasses
 import json
 import logging
 import pathlib
 import typing as t
 
+import requests
+
 import mantik
 import mantik.compute_backend_service.api as api
 import mantik.unicore.config.core as core
+import mantik.unicore.config.validate as validate
 import mantik.unicore.utils.zip as unicore_zip
 import mantik.utils as utils
-import requests
 
 logger = logging.getLogger(__name__)
 
 _DEFAULT_COMPUTE_BACKEND_API_PATH = "/compute-backend"
 
 
 @dataclasses.dataclass
@@ -96,17 +98,17 @@
         return utils.urls.ensure_https_and_remove_double_slashes_from_path(
             f"{self.url}{api.SUBMIT_PATH}"
         )
 
     def submit_run(
         self,
         experiment_id: int,
-        mlproject_path: pathlib.Path,
+        mlproject_path: t.Union[pathlib.Path, str],
         mlflow_parameters: t.Dict,
-        backend_config: t.Union[str, pathlib.Path],
+        backend_config: t.Union[pathlib.Path, str],
         entry_point: t.Optional[str] = None,
     ) -> requests.Response:
         """Submit a run.
 
         Parameters
         ----------
         experiment_id : int
@@ -130,48 +132,61 @@
         if entry_point is None:
             entry_point = "main"
         logger.debug(
             "Submitting MLproject %s for experiment %s",
             mlproject_path,
             experiment_id,
         )
-
-        if (
-            isinstance(backend_config, pathlib.Path)
-            and backend_config.is_absolute()
-        ):
-            backend_config = backend_config.relative_to(
-                mlproject_path
-            ).as_posix()
-
+        project_validator = validate.ProjectValidator(
+            mlproject_path=mlproject_path,
+            config_path=backend_config,
+            mlflow_parameters=mlflow_parameters,
+            entry_point=entry_point,
+            logger_level=logger.level,
+        )
+        project_validator.validate()
         data = self._generate_request_data(
             entry_point=entry_point,
             mlflow_parameters=mlflow_parameters,
-            unicore_backend_config=backend_config,
+            unicore_backend_config=project_validator.config_relative_path.as_posix(),  # noqa
+        )
+        files = _generate_request_files(
+            mlproject_path=project_validator.mlproject_path,
+            config=project_validator.config,
         )
         logger.debug("Sending request to compute backend %s", self.submit_url)
         response = requests.post(
             url=f"{self.submit_url}/{experiment_id}",
             headers=self._generate_headers(),
             data=data,
-            files=_generate_request_files(mlproject_path, backend_config),
+            files=files,
         )
         if response.status_code == 201:
             (
                 experiment_id,
                 run_id,
                 unicore_job_id,
             ) = _extract_job_info_from_response_json(response.json())
             logger.debug(
                 "Job submitted successfully with experiment_id=%s,"
                 " run_id=%s, unicore_job_id=%s.",
                 experiment_id,
                 run_id,
                 unicore_job_id,
             )
+        elif response.status_code == 413:
+            logger.warning(response.content)
+            logger.warning(
+                "The files you submitted were too large. "
+                "Please consider transferring large files "
+                "(such as image files) manually, e.g. with scp. "
+                "You will also have to change the backend "
+                "configuration to use a remote image. "
+                "Then you can try to re-submit the job."
+            )
         else:
             logger.warning("Job submission failed.")
         return response
 
     def _generate_headers(self):
         return {
             "Authorization": f"Bearer {self.mlflow_tracking_token}",
@@ -193,18 +208,16 @@
             "unicore_backend_config": unicore_backend_config,
             "mlflow_tracking_uri": self.mlflow_tracking_uri,
             "mlflow_tracking_token": self.mlflow_tracking_token,
         }
 
 
 def _generate_request_files(
-    mlproject_path: pathlib.Path,
-    backend_config_path: t.Union[pathlib.Path, str],
+    mlproject_path: pathlib.Path, config: core.Config
 ) -> t.Dict:
-    config = core.Config.from_filepath(mlproject_path / backend_config_path)
     logger.debug("Zipping MLproject directory")
     zipped = unicore_zip.zip_directory_with_exclusion(mlproject_path, config)
     return {"mlproject_zip": zipped.read()}
 
 
 def _extract_job_info_from_response_json(
     response_json: t.Dict,
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/flask/_header.py` & `mantik-0.2.0/src/mantik/mlflow_server/flask/_header.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/flask/api/_get.py` & `mantik-0.2.0/src/mantik/mlflow_server/flask/api/_get.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/flask/api/models/requests.py` & `mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 
-import mantik.mlflow_server.tokens.cognito as _cognito
 import pydantic
 
+import mantik.mlflow_server.tokens.cognito as _cognito
+
 
 class TokenRequest(abc.ABC, pydantic.BaseModel):
     """Credentials required for a token request.
 
     Parameters
     ----------
     username : str
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/flask/api/models/responses.py` & `mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import typing as t
 
-import mantik.mlflow_server.tokens.cognito as cognito
 import pydantic
 
+import mantik.mlflow_server.tokens.cognito as cognito
+
 
 class TokenResponse(pydantic.BaseModel):
     """Response for tokens."""
 
     access_token: str
     expires_at: datetime.datetime
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/flask/api/tokens.py` & `mantik-0.2.0/src/mantik/mlflow_server/flask/api/tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing as t
 
 import flask
+
 import mantik.mlflow_server.flask.api._exceptions as _exceptions
 import mantik.mlflow_server.flask.api._get as _get
 import mantik.mlflow_server.flask.api.models as models
 import mantik.mlflow_server.flask.app as _app
 import mantik.mlflow_server.flask.skip as skip
 
 app = _app.app
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/flask/before_requests.py` & `mantik-0.2.0/src/mantik/mlflow_server/flask/before_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 
 import flask
+
 import mantik.mlflow_server.flask._header as _header
 import mantik.mlflow_server.flask.app as _app
 import mantik.mlflow_server.flask.skip as skip
 import mantik.mlflow_server.tokens as tokens
 
 app = _app.app
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/flask/skip.py` & `mantik-0.2.0/src/mantik/mlflow_server/flask/skip.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_app.py` & `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import typing as t
 
 import flask
 import gunicorn.app.base as base
+
 import mantik.mlflow_server.gunicorn._env as _env
 import mantik.mlflow_server.gunicorn._options as _options
 import mantik.mlflow_server.gunicorn._stores as _stores
 
 
 class MantikMlflowApplication(base.BaseApplication):
     """Gunicorn standalone application."""
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_cli_args.py` & `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_cli_args.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_env.py` & `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/gunicorn/_stores.py` & `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_stores.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/_auth.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import contextlib
 import hashlib
 import hmac
 import logging
 import typing as t
 
 import boto3
+
 import mantik.mlflow_server.tokens.cognito.client as _client
 import mantik.mlflow_server.tokens.cognito.credentials as _credentials
 import mantik.mlflow_server.tokens.cognito.exceptions as exceptions
 
 logger = logging.getLogger(__name__)
 
 
@@ -71,14 +72,18 @@
             raise exceptions.AuthenticationFailedException(
                 exceptions.REFRESH_TOKEN_EXPIRED_ERROR_MESSAGE
             )
         elif "invalid refresh token" in message.lower():
             raise exceptions.AuthenticationFailedException(
                 exceptions.REFRESH_TOKEN_INVALID_ERROR_MESSAGE
             )
+        elif "refresh token has different client" in message.lower():
+            raise exceptions.AuthenticationFailedException(
+                exceptions.REFRESH_TOKEN_INVALID_ERROR_MESSAGE
+            )
         raise e
 
 
 def _add_secret_hash_to_auth_parameters(
     auth_parameters: t.Dict[str, str],
     credentials: _credentials.Credentials,
     cognito: _client.Properties,
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/api.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/client.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/credentials.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/credentials.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/cognito/tokens.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/tokens.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/exceptions.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/exceptions.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/jwks.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/jwks.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 """
 import logging
 import typing as t
 
 import jose.backends
 import jose.jwk
+import pydantic
+import requests
+
 import mantik.mlflow_server.tokens.cognito as _cognito
 import mantik.mlflow_server.tokens.exceptions as exceptions
 import mantik.mlflow_server.tokens.jwt as _jwt
-import pydantic
-import requests
 
 logger = logging.getLogger(__name__)
 
 JWK = t.Dict[str, str]
 
 
 class JWKS(pydantic.BaseModel):
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/jwt.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 """
 import datetime
 import logging
 import typing as t
 
 import jose.jwt
 import jose.utils
+import pydantic
+
 import mantik.mlflow_server.tokens.cognito as _cognito
 import mantik.mlflow_server.tokens.exceptions as exceptions
-import pydantic
 
 logger = logging.getLogger(__name__)
 
 
 class JWT(pydantic.BaseModel):
     """Holds the content of a JWT."""
```

### Comparing `mantik-0.1.2/src/mantik/mlflow_server/tokens/verifier.py` & `mantik-0.2.0/src/mantik/mlflow_server/tokens/verifier.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/testing/cognito.py` & `mantik-0.2.0/src/mantik/testing/cognito.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/testing/config.py` & `mantik-0.2.0/src/mantik/testing/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 def _create_singularity_environment(
     path: pathlib.Path,
     type: str = None,
     variables: t.Optional[t.Dict] = None,
     modules: t.Optional[t.List] = None,
 ):
-
     if type is None:
         type = "local"
     variables = _include_mlflow_env_vars(variables)
 
     return environment.Environment(
         execution=executable.Singularity(
             path=path,
@@ -46,15 +45,14 @@
 
 
 def _create_python_environment(
     path: pathlib.Path,
     variables: t.Optional[t.Dict] = None,
     modules: t.Optional[t.List] = None,
 ):
-
     variables = _include_mlflow_env_vars(variables)
 
     return environment.Environment(
         executable.Python(
             path=path,
         ),
         variables=variables,
```

### Comparing `mantik-0.1.2/src/mantik/testing/contexts.py` & `mantik-0.2.0/src/mantik/testing/contexts.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/testing/env.py` & `mantik-0.2.0/src/mantik/testing/env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/testing/mlflow_server.py` & `mantik-0.2.0/src/mantik/testing/mlflow_server.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/testing/pyunicore.py` & `mantik-0.2.0/src/mantik/testing/pyunicore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime
 import io
 import typing as t
 
+import pyunicore.client
+
 import mantik.unicore as unicore
 import mantik.unicore.job as job_wrapper
 import mantik.unicore.properties as properties_wrapper
 import mantik.unicore.submitted_run as submitted_run
-import pyunicore.client
 
 
 class FakeTransport:
     def __init__(self, auth_token: str = "test_token", oidc: bool = True):
         self.auth_token = auth_token
         self.oidc = oidc
```

### Comparing `mantik-0.1.2/src/mantik/testing/requests.py` & `mantik-0.2.0/src/mantik/testing/requests.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/testing/token.py` & `mantik-0.2.0/src/mantik/testing/token.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/tracking/_server/_credentials.py` & `mantik-0.2.0/src/mantik/tracking/_server/_credentials.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/tracking/_server/api.py` & `mantik-0.2.0/src/mantik/tracking/_server/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing as t
 
+import requests
+
 import mantik.mlflow_server.flask.api as _api
 import mantik.mlflow_server.tokens.cognito.exceptions as exceptions
 import mantik.tracking._server._credentials as _credentials
 import mantik.tracking._server.tokens as _tokens
 import mantik.utils as utils
-import requests
 
 
 def create_tokens(
     credentials: t.Optional[_credentials.Credentials] = None,
 ) -> _tokens.Tokens:
     """Get the required tokens from the Cognito API.
```

### Comparing `mantik-0.1.2/src/mantik/tracking/_server/tokens.py` & `mantik-0.2.0/src/mantik/tracking/_server/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             refresh_token=refresh_token,
             expires_at=expires_at,
         )
 
     @classmethod
     def from_file(cls, path: pathlib.Path) -> "Tokens":
         """Create from a JSON file."""
-        with open(path, "r", encoding=cls.__encoding) as f:
+        with open(path, encoding=cls.__encoding) as f:
             data = json.load(f, object_hook=_deserialize_datetime)
             return cls(**data)
 
     @property
     def has_expired(self) -> bool:
         """Return whether the token has expired."""
         tz = self.expires_at.tzinfo
```

### Comparing `mantik-0.1.2/src/mantik/tracking/environment.py` & `mantik-0.2.0/src/mantik/tracking/environment.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/tracking/track.py` & `mantik-0.2.0/src/mantik/tracking/track.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/unicore/_connect.py` & `mantik-0.2.0/src/mantik/unicore/_connect.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 import logging
 
-import mantik.unicore.exceptions as exceptions
 import pyunicore.client as pyunicore
 
+import mantik.unicore.exceptions as exceptions
+
 logger = logging.getLogger(__name__)
 
 
 def create_unicore_api_connection(
     api_url: str,
     user: str,
     password: str,
@@ -50,15 +51,25 @@
 
 def _connect_to_cluster(
     api_url: str,
     user: str,
     password: str,
 ) -> pyunicore.Client:
     transport = _create_transport(user=user, password=password)
-    client = _create_client(transport=transport, api_url=api_url)
+    try:
+        client = _create_client(transport=transport, api_url=api_url)
+    # In the current version of pyunicore a base Exception is raised
+    # when a client is instantiated when the Auth fails.
+    # In newer versions it should be possible
+    # to catch a pyunicore.credentials.AuthenticationFailedException.
+    except Exception:
+        raise exceptions.AuthenticationFailedException(
+            f"Failed to connect to {api_url} -- "
+            "check if user and password are correct"
+        )
     logger.debug("Connection properties: %s", client.properties)
     return client
 
 
 def _create_transport(user: str, password: str) -> pyunicore.Transport:
     logger.debug("Creating transport for user %s", user)
     token = _create_token(user=user, password=password)
```

### Comparing `mantik-0.1.2/src/mantik/unicore/backend.py` & `mantik-0.2.0/src/mantik/unicore/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+"""Mantik UNICORE plugin for MLflow."""
 import logging
 import pathlib
 import typing as t
 
+import mlflow.projects as projects
+import mlflow.projects._project_spec as _project_spec
+import mlflow.projects.backend as mlflow_backend
+
 import mantik.unicore._connect as _connect
 import mantik.unicore.client as client_wrapper
 import mantik.unicore.config.core as core
 import mantik.unicore.job as job_wrapper
 import mantik.unicore.submitted_run as submitted_run
 import mantik.unicore.utils.upload as upload
-import mlflow.projects as projects
-import mlflow.projects._project_spec as _project_spec
-import mlflow.projects.backend as mlflow_backend
 
 logger = logging.getLogger(__name__)
 
 
 class UnicoreBackend(mlflow_backend.AbstractBackend):
     """UNICORE backend for running MLflow projects."""
 
@@ -32,54 +34,66 @@
 
         It must return a SubmittedRun object to track the execution
 
         Parameters
         ----------
         project_uri : str
             URI of the project to execute.
+
             E.g. a local filesystem path or a Git repository URI like
             https://github.com/mlflow/mlflow-example
         entry_point : str
             Entry point to run within the project.
+
             E.g. for a project that is defined as
-            ```yaml
-            entry_points:
-                main:
-                  parameters:
-                    print: {type: "string", default: "test"}
-                  command: python main.py {print}
-            ```
+
+            .. code-block:: yaml
+               :caption: MLproject entry points
+
+               entry_points:
+                   main:
+                     parameters:
+                       print: {type: "string", default: "test"}
+                     command: python main.py {print}
+
             the `entry_point="main"`.
         params : dict
             Dict of parameters to pass to the entry point.
+
             For the example entrypoint as above, if the project is run as
             `mlflow run --backend unicore <project path> -P print=hi`, this
             would be `{"print": "hi"}`.
         version : str
             For git-based projects, either a commit hash or a branch name.
         backend_config : dict
             The backend config.
+
             By default, mlflow passes the following dict
-            ```
-            {
+
+            .. code-block:: python
+               :caption: Default MLflow ``backend_config``
+
+               {
                 'DOCKER_ARGS': {},
                 'STORAGE_DIR': None,
                 'SYNCHRONOUS': False,
                 'USE_CONDA': True,
-            }
-            ```
+               }
+
             which is extended by the content given in the backend
             config of a user.
         tracking_uri : str
             URI of tracking server against which to log run information.
+
             E.g. for local tracking this may be
             `'file://<home path>/mantik/mlruns'`
         experiment_id : str
             ID of experiment under which to launch the run.
-            E.g. `'0'` for the Default experiment that is created by mlflow..
+
+            E.g. `'0'` for the Default experiment that is created by mlflow.
 
         Returns
         -------
         mlflow.projects.SubmittedRun
 
         """
         project_dir, project = _load_project(
```

### Comparing `mantik-0.1.2/src/mantik/unicore/client.py` & `mantik-0.2.0/src/mantik/unicore/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import pathlib
 import typing as t
 
+import pyunicore.client as pyunicore
+
 import mantik.unicore._connect as _connect
 import mantik.unicore.config.core as core
 import mantik.unicore.exceptions as exceptions
 import mantik.unicore.job as job_wrapper
 import mantik.utils.env as env
-import pyunicore.client as pyunicore
 
 logger = logging.getLogger(__name__)
 
 
 class Client:
     def __init__(self, client: pyunicore.Client):
         self._client = client
@@ -57,15 +58,15 @@
         return cls(client)
 
     def get_job(self, job_id: str) -> job_wrapper.Job:
         """Get a job by ID."""
         for job in self.get_jobs():
             if job_id == job.id:
                 return job
-        raise exceptions.UnicoreError(f"No job with id {id} was found")
+        raise exceptions.UnicoreError(f"No job with id {job_id} was found")
 
     def get_jobs(
         self, offset: int = 0, total: t.Optional[int] = None
     ) -> t.List[job_wrapper.Job]:
         """Get all UNICORE jobs deployed by the user.
 
         Parameters
```

### Comparing `mantik-0.1.2/src/mantik/unicore/config/_base.py` & `mantik-0.2.0/src/mantik/unicore/config/_base.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/unicore/config/_utils.py` & `mantik-0.2.0/src/mantik/unicore/config/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     Returns
     -------
     Any
         The value from the config cast as `value_type`.
 
     """
     if name not in config:
-        raise exceptions.ConfigurationError(
-            f"Backend config is missing entry for key '{name}'."
+        raise exceptions.ConfigValidationError(
+            f"Config is missing entry for key {name!r}"
         )
     return _get_config_value(name=name, value_type=value_type, config=config)
 
 
 def get_optional_config_value(
     name: str,
     value_type: t.Type,
@@ -79,16 +79,16 @@
     return _cast_type(name=name, value=value, value_type=value_type)
 
 
 def _cast_type(name: str, value: str, value_type: t.Type) -> t.Any:
     try:
         return value_type(value)
     except ValueError as e:
-        raise exceptions.ConfigurationError(
-            f"Backend config value for '{name}' has to be of type {value_type}"
+        raise exceptions.ConfigValidationError(
+            f"Config value for {name!r} has to be of type {value_type!r}"
         ) from e
 
 
 def create_dict_with_not_none_values(**kwargs) -> t.Dict:
     """Create a dict which only contains value that are not `None`."""
     return {
         key: _convert_value(value)
```

### Comparing `mantik-0.1.2/src/mantik/unicore/config/core.py` & `mantik-0.2.0/src/mantik/unicore/config/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,27 +46,19 @@
                 and MANTIK_PROJECT are inferred from the environment.
             OPTIONAL:
                 - Resources : dict
                     Dict of parameters specifying the resources
                     to request on the remote system.
                     More info can be found here:
                     https://sourceforge.net/p/unicore/wiki/Job_Description/
-                - SingularityImage : SingularityImage
-                    - path : str
-                        Path to the Singularity image file.
-                    - type : str, default="local"
-                      - `local`: If the given path is relative, it is
-                        assumed to be relative to the MLflow project directory.
-                      - `remote`: The given path must be absolute and
-                        correspond to the path of the Singularity image
-                        already present on the remote system. This path
-                        is checked to be an absolute path.
                 - Environment : dict
-                    Dict of environment variables that are passed
-                    to the remote UNICORE HPC.
+                    Used to build a environment.Environment.
+                - Exclude : list
+                    List of files or file-patterns
+                    that are not sent with the job
 
 
         Returns
         -------
         mantik.unicore._config.core.Config
 
         """
```

### Comparing `mantik-0.1.2/src/mantik/unicore/config/environment.py` & `mantik-0.2.0/src/mantik/unicore/config/environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import os
 import re
 import typing as t
 
 import mantik.unicore.config._base as _base
 import mantik.unicore.config._utils as _utils
 import mantik.unicore.config.executable as executable
+import mantik.unicore.exceptions as exceptions
 
 _MLFLOW_ENV_VAR_PREFIX = "MLFLOW_"
 _ALLOWED_EXECUTABLES = {
     "Singularity": executable.Singularity,
     "Python": executable.Python,
 }
 
 
 @dataclasses.dataclass
 class Environment(_base.ConfigObject):
     """Part of the backend-config where all variables
-    concerning the running enviroment are stored"""
+    concerning the running environment are stored."""
 
     execution: executable.Execution
     variables: t.Optional[dict] = None
     modules: t.Optional[list] = None
 
     @classmethod
     def _from_dict(cls, config: t.Dict) -> "Environment":
@@ -59,18 +60,24 @@
     return _get_only_one_environment(envs)
 
 
 def _get_only_one_environment(
     env_found: t.List,
 ) -> t.Type[executable.Execution]:
     if not env_found:
-        raise ValueError("No execution environment defined in config")
+        raise exceptions.ConfigValidationError(
+            "No execution environment defined in config, "
+            "the allowed environments are: "
+            f"{exceptions.list_to_string(_ALLOWED_EXECUTABLES.keys())}."
+        )
     elif len(env_found) > 1:
-        raise ValueError(
-            f"Multiple execution environments defined in config: {env_found}"
+        raise exceptions.ConfigValidationError(
+            "Only one execution environment is allowed, "
+            "but in config these have been found: "
+            f"{exceptions.list_to_string(env_found)}."
         )
     return _ALLOWED_EXECUTABLES[env_found[0]]
 
 
 def _add_mlflow_env_vars(environment: t.Optional[t.Dict]) -> t.Optional[t.Dict]:
     mlflow_env_vars = _get_mlflow_env_vars()
     if mlflow_env_vars:
```

### Comparing `mantik-0.1.2/src/mantik/unicore/config/executable.py` & `mantik-0.2.0/src/mantik/unicore/config/executable.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,22 +17,27 @@
 
 @dataclasses.dataclass
 class Execution:
     """Execution environment used for executing a python script."""
 
     path: str
 
+    @property
+    @abc.abstractmethod
+    def path_has_to_be_checked(self) -> bool:
+        raise NotImplementedError
+
     @abc.abstractmethod
     def as_execution_command(self) -> str:
-        ...
+        raise NotImplementedError
 
     @classmethod
     @abc.abstractmethod
     def from_dict(cls, config: t.Dict):
-        ...
+        raise NotImplementedError
 
 
 @dataclasses.dataclass
 class Singularity(Execution):
     """Information about a Singularity image.
 
     Parameters
@@ -49,32 +54,38 @@
     type: str = _LOCAL_IMAGE_TYPE
 
     def __post_init__(self) -> None:
         """Check that the given type is correct."""
         self._ensure_valid_path_type()
         self._ensure_path_conform_to_type()
 
+    @property
+    def path_has_to_be_checked(self) -> bool:
+        return self.type == _LOCAL_IMAGE_TYPE
+
     def _ensure_valid_path_type(self) -> None:
         if self.type not in _ALLOWED_IMAGE_TYPES:
-            raise exceptions.ConfigurationError(
-                f"Given image type {self.type} not supported, "
-                f"any of {', '.join(_ALLOWED_IMAGE_TYPES)} required"
+            raise exceptions.ConfigValidationError(
+                f"The given Apptainer image type {self.type!r} "
+                "is not supported, "
+                "the supported ones are: "
+                f"{exceptions.list_to_string(_ALLOWED_IMAGE_TYPES)}."
             )
 
     def _ensure_path_conform_to_type(self) -> None:
         if self._remote_image_and_relative_path_given():
-            raise exceptions.ConfigurationError(
-                f"If path type {self.type!r} is given for the Singularity "
-                "image, the given path must be absolute "
-                f"({self.path.as_posix()} given)"
+            raise exceptions.ConfigValidationError(
+                f"If image type {self.type!r} is given for an Apptainer "
+                "image, the given path must be absolute. "
+                f"The given path is: {self.path.as_posix()!r}."
             )
         elif self._local_image_and_relative_path_given():
             logger.warning(
                 (
-                    "Path for Singularity image of type %s is assumed to be"
+                    "Path for Singularity image of type %s is assumed to be "
                     "relative to the MLflow project directory"
                 ),
                 _LOCAL_IMAGE_TYPE,
             )
 
     def _remote_image_and_relative_path_given(self) -> bool:
         return self.type == _REMOTE_IMAGE_TYPE and not self.path.is_absolute()
@@ -181,14 +192,22 @@
 
 @dataclasses.dataclass
 class Python(Execution):
     """Python virtual environment used for executing a python script."""
 
     path: pathlib.Path
 
+    def __post_init__(self) -> None:
+        """Check that the given type is correct."""
+        self._ensure_venv_path_is_absolute()
+
+    @property
+    def path_has_to_be_checked(self) -> bool:
+        return False
+
     @classmethod
     def from_dict(cls, config: t.Dict) -> "Python":
         if isinstance(config["Python"], dict):
             python_dict = _utils.get_required_config_value(
                 name="Python",
                 value_type=dict,
                 config=config,
@@ -204,9 +223,16 @@
                 value_type=pathlib.Path,
                 config=config,
             )
         return cls(
             path=python_path,
         )
 
+    def _ensure_venv_path_is_absolute(self) -> None:
+        if not self.path.is_absolute():
+            raise exceptions.ConfigValidationError(
+                "The given path to the Python Venv must be absolute. "
+                f"The given path is: {self.path.as_posix()!r}."
+            )
+
     def as_execution_command(self) -> str:
         return f"source {self.path}/bin/activate &&"
```

### Comparing `mantik-0.1.2/src/mantik/unicore/config/resources.py` & `mantik-0.2.0/src/mantik/unicore/config/resources.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/unicore/job.py` & `mantik-0.2.0/src/mantik/unicore/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
 import json
 import pathlib
 import typing as t
 
-import mantik.unicore.properties as properties
-import mantik.unicore.working_dir as working_dir
 import pyunicore.client as pyunicore
 import yaml
 
+import mantik.unicore.properties as properties
+import mantik.unicore.working_dir as working_dir
+
 APPLICATION_LOGS_FILE = "mantik.log"
 
 
 class Job:
     """Job submitted to unicore, wrapper class around pyunicore.client.Job"""
 
     def __init__(self, job: pyunicore.Job):
```

### Comparing `mantik-0.1.2/src/mantik/unicore/properties.py` & `mantik-0.2.0/src/mantik/unicore/properties.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/unicore/submitted_run.py` & `mantik-0.2.0/src/mantik/unicore/submitted_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 import pathlib
 import typing as t
 
+import mlflow.entities as entities
+import mlflow.projects as projects
+
 import mantik.unicore.job as job
 import mantik.unicore.properties as properties
 import mantik.unicore.working_dir as working_dir
-import mlflow.entities as entities
-import mlflow.projects as projects
 
 logger = logging.getLogger(__name__)
 
 
 class SubmittedUnicoreRun(projects.SubmittedRun):
     """A run that was submitted through the UNICORE interface.
```

### Comparing `mantik-0.1.2/src/mantik/unicore/utils/upload.py` & `mantik-0.2.0/src/mantik/unicore/utils/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import mantik.unicore.config.executable as executable
 
 
 def get_files_to_upload(
     project_dir: pathlib.Path,
     config: core.Config,
 ) -> t.List[pathlib.Path]:
-
     """Get all files to be uploaded via UNICORE.
 
     Notes
     -----
     Since MLflow docker backend mounts the MLflow project directory, all
     directory contents are uploaded here as well.
```

### Comparing `mantik-0.1.2/src/mantik/unicore/utils/zip.py` & `mantik-0.2.0/src/mantik/unicore/utils/zip.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/unicore/working_dir.py` & `mantik-0.2.0/src/mantik/unicore/working_dir.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/src/mantik/utils/env.py` & `mantik-0.2.0/src/mantik/utils/env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.1.2/setup.py` & `mantik-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,39 +29,39 @@
 
 install_requires = \
 ['Flask>=2.1.2,<3.0.0',
  'PyYAML>=6.0,<7.0',
  'boto3>=1.23.6,<2.0.0',
  'click>=8.1.3,<9.0.0',
  'fastapi>=0.78.0,<0.79.0',
- 'mlflow==1.30.0',
+ 'mlflow==2.2.2',
  'pydantic>=1.9.0,<2.0.0',
  'python-jose>=3.3.0,<4.0.0',
  'python-multipart>=0.0.5,<0.0.6',
  'pyunicore>=0.9.16,<0.10.0',
  'requests>=2.27.1,<3.0.0',
  'uvicorn[standard]>=0.17.6,<0.18.0']
 
 entry_points = \
 {'console_scripts': ['mantik = mantik.cli.main:cli'],
  'mlflow.project_backend': ['unicore = mantik.unicore.backend:UnicoreBackend']}
 
 setup_kwargs = {
     'name': 'mantik',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'mantik for mlflow',
-    'long_description': None,
+    'long_description': '# mantik - plugin for MLflow with HPC (UNICORE)\n\n[Documentation](https://mantik-ai.gitlab.io/mantik)\n\nMantik allows to manage the full Machine Learning workflow on HPC by\nsupporting MLflow and deployment of applications to HPC.\n\n```shell\nmlflow run --backend unicore --backend-config <path to config> <path to project>\n```\n\nFor a quickstart see [our documentation](https://mantik-ai.gitlab.io/mantik/quickstart.html)\n\nService desk email: contact-project+mantik-ai-mantik-42525397-issue-@incoming.gitlab.com',
     'author': 'Fabian Emmerich',
     'author_email': 'fabian.emmerich@4-cast.de',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'Elia Boscaini',
+    'maintainer_email': 'elia.boscaini@ambrosys.de',
     'url': 'https://mantik.ai/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

