# Comparing `tmp/dvc-studio-client-0.6.2.tar.gz` & `tmp/dvc-studio-client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-studio-client-0.6.2.tar", last modified: Wed Apr 12 08:59:25 2023, max compression
+gzip compressed data, was "dvc-studio-client-0.7.0.tar", last modified: Tue Apr 18 08:23:19 2023, max compression
```

## Comparing `dvc-studio-client-0.6.2.tar` & `dvc-studio-client-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/src/dvc_studio_client/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/post_live_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/tests/test_post_live_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/src/dvc_studio_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/post_live_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/tests/test_post_live_metrics.py
```

### Comparing `dvc-studio-client-0.6.2/.cruft.json` & `dvc-studio-client-0.7.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/.github/dependabot.yml` & `dvc-studio-client-0.7.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/.github/workflows/docs.yml` & `dvc-studio-client-0.7.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/.github/workflows/pre-commit.yml` & `dvc-studio-client-0.7.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/.github/workflows/release.yml` & `dvc-studio-client-0.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/.github/workflows/tests.yml` & `dvc-studio-client-0.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/.gitignore` & `dvc-studio-client-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/.pre-commit-config.yaml` & `dvc-studio-client-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/CODE_OF_CONDUCT.rst` & `dvc-studio-client-0.7.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/CONTRIBUTING.rst` & `dvc-studio-client-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/LICENSE` & `dvc-studio-client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/PKG-INFO` & `dvc-studio-client-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.6.2
+Version: 0.7.0
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/DVC Studio Client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.6.2/README.rst` & `dvc-studio-client-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/docs/assets/logo.svg` & `dvc-studio-client-0.7.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/docs/gen_ref_pages.py` & `dvc-studio-client-0.7.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/mkdocs.yml` & `dvc-studio-client-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/pyproject.toml` & `dvc-studio-client-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/setup.cfg` & `dvc-studio-client-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/src/dvc_studio_client/post_live_metrics.py` & `dvc-studio-client-0.7.0/src/dvc_studio_client/post_live_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import logging
 from functools import lru_cache
 from os import getenv
 from typing import Any, Dict, Literal, Optional
+from urllib.parse import urljoin
 
 import requests
 from requests.exceptions import RequestException
 from voluptuous import Invalid, MultipleInvalid
 from voluptuous.humanize import humanize_error
 
 from .env import (
     DVC_STUDIO_CLIENT_LOGLEVEL,
+    DVC_STUDIO_TOKEN,
+    DVC_STUDIO_URL,
     STUDIO_ENDPOINT,
     STUDIO_REPO_URL,
     STUDIO_TOKEN,
 )
 from .schema import SCHEMAS_BY_TYPE
 
+STUDIO_URL = "https://studio.iterative.ai"
+
 logger = logging.getLogger(__name__)
 logger.setLevel(getenv(DVC_STUDIO_CLIENT_LOGLEVEL, "INFO").upper())
 
 
 def _get_remote_url() -> str:
     from dulwich.porcelain import get_remote_repo
     from dulwich.repo import Repo
@@ -45,17 +50,19 @@
             "You can try manually setting the environment variable `%s`.",
             STUDIO_REPO_URL,
         )
         return None
 
 
 def get_studio_token_and_repo_url():
-    studio_token = getenv(STUDIO_TOKEN, None)
+    studio_token = getenv(DVC_STUDIO_TOKEN) or getenv(STUDIO_TOKEN)
     if studio_token is None:
-        logger.debug("STUDIO_TOKEN not found. Skipping `post_studio_live_metrics`")
+        logger.debug(
+            f"{DVC_STUDIO_TOKEN} not found. Skipping `post_studio_live_metrics`"
+        )
         return None, None
 
     studio_repo_url = getenv(STUDIO_REPO_URL, None)
     if studio_repo_url is None:
         logger.debug(f"`{STUDIO_REPO_URL}` not found. Trying to automatically find it.")
         studio_repo_url = get_studio_repo_url()
     return studio_token, studio_repo_url
@@ -171,17 +178,20 @@
     except (Invalid, MultipleInvalid) as e:
         logger.warning(humanize_error(body, e))
         return None
 
     logger.debug(f"post_studio_live_metrics `{event_type=}`")
     logger.debug(f"JSON body `{body=}`")
 
+    base_url = getenv(DVC_STUDIO_URL) or STUDIO_URL
+    path = getenv(STUDIO_ENDPOINT) or "api/live"
+    url = urljoin(base_url, path)
     try:
         response = requests.post(
-            getenv(STUDIO_ENDPOINT, "https://studio.iterative.ai/api/live"),
+            url,
             json=body,
             headers={
                 "Content-type": "application/json",
                 "Authorization": f"token {studio_token}",
             },
             timeout=5,
         )
```

### Comparing `dvc-studio-client-0.6.2/src/dvc_studio_client/schema.py` & `dvc-studio-client-0.7.0/src/dvc_studio_client/schema.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/PKG-INFO` & `dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.6.2
+Version: 0.7.0
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/DVC Studio Client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/SOURCES.txt` & `dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.2/tests/test_post_live_metrics.py` & `dvc-studio-client-0.7.0/tests/test_post_live_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import logging
 import os
 
+import pytest
 from dulwich.porcelain import clone, init
 from requests import RequestException
 
-from dvc_studio_client.env import STUDIO_ENDPOINT, STUDIO_REPO_URL, STUDIO_TOKEN
+from dvc_studio_client.env import (
+    DVC_STUDIO_TOKEN,
+    DVC_STUDIO_URL,
+    STUDIO_REPO_URL,
+    STUDIO_TOKEN,
+)
 from dvc_studio_client.post_live_metrics import (
     _get_remote_url,
     get_studio_token_and_repo_url,
     post_live_metrics,
 )
 
 
@@ -16,51 +22,58 @@
     source = os.fspath(tmp_path_factory.mktemp("source"))
     target = os.fspath(tmp_path_factory.mktemp("target"))
     with init(source), clone(source, target):
         monkeypatch.chdir(target)
         assert _get_remote_url() == source
 
 
+@pytest.mark.parametrize("var", [DVC_STUDIO_TOKEN, STUDIO_TOKEN])
+def test_studio_token_envvar(monkeypatch, var):
+    monkeypatch.setenv(var, "FOO_TOKEN")
+    monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
+    assert get_studio_token_and_repo_url() == ("FOO_TOKEN", "FOO_REPO_URL")
+
+
 def test_post_live_metrics_skip_on_missing_token(caplog):
     with caplog.at_level(logging.DEBUG, logger="dvc_studio_client.post_live_metrics"):
         assert post_live_metrics("start", "current_rev", "fooname", "fooclient") is None
         assert caplog.records[0].message == (
-            "STUDIO_TOKEN not found. Skipping `post_studio_live_metrics`"
+            "DVC_STUDIO_TOKEN not found. Skipping `post_studio_live_metrics`"
         )
 
 
 def test_post_live_metrics_skip_on_schema_error(caplog, monkeypatch):
-    monkeypatch.setenv(STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
     with caplog.at_level(logging.DEBUG, logger="dvc_studio_client.post_live_metrics"):
         assert post_live_metrics("start", "bad_hash", "fooname", "fooclient") is None
         assert caplog.records[0].message == (
             "expected a length 40 commit sha for dictionary value @ "
             "data['baseline_sha']. Got 'bad_hash'"
         )
 
 
 def test_post_live_metrics_start_event(mocker, monkeypatch):
-    monkeypatch.setenv(STUDIO_ENDPOINT, "https://0.0.0.0")
-    monkeypatch.setenv(STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_URL, "https://0.0.0.0")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
 
     mocked_response = mocker.MagicMock()
     mocked_response.status_code = 200
     mocked_post = mocker.patch("requests.post", return_value=mocked_response)
 
     assert post_live_metrics(
         "start",
         "f" * 40,
         "fooname",
         "fooclient",
     )
 
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "start",
             "repo_url": "FOO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": "fooname",
             "client": "fooclient",
         },
@@ -76,15 +89,15 @@
         "f" * 40,
         "fooname",
         "fooclient",
         params={"params.yaml": {"foo": "bar"}},
     )
 
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "start",
             "repo_url": "FOO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": "fooname",
             "client": "fooclient",
             "params": {"params.yaml": {"foo": "bar"}},
@@ -94,23 +107,23 @@
             "Content-type": "application/json",
         },
         timeout=5,
     )
 
 
 def test_post_live_metrics_data_skip_if_no_step(caplog, monkeypatch):
-    monkeypatch.setenv(STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
 
     assert post_live_metrics("data", "f" * 40, "fooname", "fooclient") is None
     assert caplog.records[0].message == ("Missing `step` in `data` event.")
 
 
 def test_post_live_metrics_data(mocker, monkeypatch):
-    monkeypatch.setenv(STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
 
     mocked_response = mocker.MagicMock()
     mocked_response.status_code = 200
     mocked_post = mocker.patch("requests.post", return_value=mocked_response)
 
     assert post_live_metrics("data", "f" * 40, "fooname", "fooclient", step=0)
@@ -185,15 +198,15 @@
             "Content-type": "application/json",
         },
         timeout=5,
     )
 
 
 def test_post_live_metrics_done(mocker, monkeypatch):
-    monkeypatch.setenv(STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
 
     mocked_response = mocker.MagicMock()
     mocked_response.status_code = 200
     mocked_post = mocker.patch("requests.post", return_value=mocked_response)
 
     assert post_live_metrics(
@@ -260,15 +273,15 @@
             "Content-type": "application/json",
         },
         timeout=5,
     )
 
 
 def test_post_live_metrics_bad_response(mocker, monkeypatch):
-    monkeypatch.setenv(STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
 
     mocked_response = mocker.MagicMock()
     mocked_response.status_code = 400
     mocker.patch("requests.post", return_value=mocked_response)
     assert (
         post_live_metrics(
```

