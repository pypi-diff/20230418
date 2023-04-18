# Comparing `tmp/birenci-infra-0.0.5.tar.gz` & `tmp/birenci-infra-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birenci-infra-0.0.5.tar", last modified: Tue Apr 18 06:42:50 2023, max compression
+gzip compressed data, was "birenci-infra-0.0.6.tar", last modified: Tue Apr 18 06:59:58 2023, max compression
```

## Comparing `birenci-infra-0.0.5.tar` & `birenci-infra-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,40 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.140806 birenci-infra-0.0.5/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1949 2023-04-18 06:42:50.140806 birenci-infra-0.0.5/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 06:38:29.000000 birenci-infra-0.0.5/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/birenci_infra.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1949 2023-04-18 06:42:50.000000 birenci-infra-0.0.5/birenci_infra.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1949 2023-04-18 06:42:50.000000 birenci-infra-0.0.5/birenci_infra.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 06:42:50.000000 birenci-infra-0.0.5/birenci_infra.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       12 2023-04-18 06:42:50.000000 birenci-infra-0.0.5/birenci_infra.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/sdk/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/sdk/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/sdk/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/sdk/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/run.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/sdk/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/test_hander_perf.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/sdk/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birenci-infra-0.0.5/sdk/utils/xml_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 06:42:50.140806 birenci-infra-0.0.5/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      588 2023-04-18 06:42:44.000000 birenci-infra-0.0.5/setup.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/web_api/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/web_api/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      605 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/apis/hr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3464 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/apis/pdu.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/web_api/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      327 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      424 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      210 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/config/prod.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      420 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/exception.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/web_api/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      127 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2147 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      703 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/handles/component.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1896 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1970 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/handles/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      916 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/handles/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      338 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/handles/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      411 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/main.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.136806 birenci-infra-0.0.5/web_api/models/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      236 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/models/Component.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1261 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/models/JenkinsResult.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      681 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/models/PullRequest.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      712 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/models/PullRequestJob.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      480 2023-04-17 06:45:25.000000 birenci-infra-0.0.5/web_api/models/TestCase.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/models/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      455 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/models/perfResult.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       65 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/mongo.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      402 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/mysql.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.140806 birenci-infra-0.0.5/web_api/routers/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      411 2023-04-13 11:07:11.000000 birenci-infra-0.0.5/web_api/routers/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1126 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/routers/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1612 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/routers/component.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      870 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/routers/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)    19112 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/routers/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3617 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/routers/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2532 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/routers/test_case.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.140806 birenci-infra-0.0.5/web_api/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      252 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/component.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      150 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/hr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      642 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      423 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2989 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1049 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      400 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/schemas/test_case.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:42:50.140806 birenci-infra-0.0.5/web_api/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      162 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/utils/dict_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       40 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/utils/log.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      563 2023-04-12 09:21:26.000000 birenci-infra-0.0.5/web_api/utils/resp.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1949 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birenci-infra-0.0.6/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/birenci_infra.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1949 2023-04-18 06:59:58.000000 birenci-infra-0.0.6/birenci_infra.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      608 2023-04-18 06:59:58.000000 birenci-infra-0.0.6/birenci_infra.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 06:59:58.000000 birenci-infra-0.0.6/birenci_infra.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       34 2023-04-18 06:59:58.000000 birenci-infra-0.0.6/birenci_infra.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/handles/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      588 2023-04-18 06:58:00.000000 birenci-infra-0.0.6/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 06:59:58.655026 birenci-infra-0.0.6/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birenci-infra-0.0.6/utils/xml_utils.py
```

### Comparing `birenci-infra-0.0.5/PKG-INFO` & `birenci-infra-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birenci-infra
-Version: 0.0.5
+Version: 0.0.6
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birenci-infra-0.0.5/README.md` & `birenci-infra-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/birenci_infra.egg-info/PKG-INFO` & `birenci-infra-0.0.6/birenci_infra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birenci-infra
-Version: 0.0.5
+Version: 0.0.6
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birenci-infra-0.0.5/sdk/apis/build.py` & `birenci-infra-0.0.6/apis/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/apis/client.py` & `birenci-infra-0.0.6/apis/client.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/apis/pdu.py` & `birenci-infra-0.0.6/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/apis/perf.py` & `birenci-infra-0.0.6/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/apis/pr.py` & `birenci-infra-0.0.6/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/handles/build.py` & `birenci-infra-0.0.6/handles/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/handles/pdu.py` & `birenci-infra-0.0.6/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/handles/perf.py` & `birenci-infra-0.0.6/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/handles/pr.py` & `birenci-infra-0.0.6/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/schemas/pull_request.py` & `birenci-infra-0.0.6/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/utils/csv_utils.py` & `birenci-infra-0.0.6/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/sdk/utils/xml_utils.py` & `birenci-infra-0.0.6/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.5/setup.py` & `birenci-infra-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="birenci-infra", 
-    version="0.0.5",    
+    version="0.0.6",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
```

