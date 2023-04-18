# Comparing `tmp/dcicutils-7.2.0.1b0.tar.gz` & `tmp/dcicutils-7.2.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.2.0.1b0.tar", max compression
+gzip compressed data, was "dcicutils-7.2.0.1b1.tar", max compression
```

## Comparing `dcicutils-7.2.0.1b0.tar` & `dcicutils-7.2.0.1b1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1166 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/README.rst
--rw-r--r--   0        0        0        0 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9257 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    11502 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/log_utils.py
--rw-r--r--   0        0        0    87196 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   120743 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    19745 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9633 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     1769 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3680 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 dcicutils-7.2.0.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/README.rst
+-rw-r--r--   0        0        0        0 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/base.py
+-rwxr-xr-x   0        0        0    52659 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    13639 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     1649 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9257 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    37025 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    87196 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20232 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   120743 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    19745 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0    10090 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3680 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 dcicutils-7.2.0.1b1/PKG-INFO
```

### Comparing `dcicutils-7.2.0.1b0/README.rst` & `dcicutils-7.2.0.1b1/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/base.py` & `dcicutils-7.2.0.1b1/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/beanstalk_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/cloudformation_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/codebuild_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/command_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/common.py` & `dcicutils-7.2.0.1b1/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/creds_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/data_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/deployment_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/diff_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/docker_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/ecr_scripts.py` & `dcicutils-7.2.0.1b1/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/ecr_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/ecs_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/env_base.py` & `dcicutils-7.2.0.1b1/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/env_manager.py` & `dcicutils-7.2.0.1b1/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/env_scripts.py` & `dcicutils-7.2.0.1b1/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/env_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/env_utils_legacy.py` & `dcicutils-7.2.0.1b1/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/es_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/exceptions.py` & `dcicutils-7.2.0.1b1/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/ff_mocks.py` & `dcicutils-7.2.0.1b1/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/ff_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/jh_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/kibana/dashboards.json` & `dcicutils-7.2.0.1b1/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/kibana/readme.md` & `dcicutils-7.2.0.1b1/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/lang_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/log_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/misc_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/obfuscation_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/opensearch_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/qa_checkers.py` & `dcicutils-7.2.0.1b1/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/qa_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/redis_tools.py` & `dcicutils-7.2.0.1b1/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/redis_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/s3_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/secrets_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/snapshot_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/ssl_certificate_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from datetime import datetime, timedelta
 import OpenSSL
 import socket
 import ssl
 from typing import Any, Optional, Tuple, Union
 
 
-def get_ssl_certificate_info(hostname: str, raise_exception: bool = False, expires_soon_days: int = 0) -> Optional[dict]:
+def get_ssl_certificate_info(hostname: str,
+                             raise_exception: bool = False,
+                             test_mode_certificate_expiration_warning_days: int = 0) -> Optional[dict]:
     """
     Returns a dictionary containing various data points for the SSL certificate of the given
     hostname. If an error is encountered then returns None, or, if the given raise_exception
     argument is True then raises an exception. Returned dictionary contains (alphabetical order):
 
         active_at    issuer           owner_country
         exception    issuer_city      owner_entity
@@ -19,18 +21,22 @@
         hostname     issuer_state     public_key_pem
         hostnames    owner            serial_number
         inactive     owner_city       valid
     """
     hostname = _normalize_hostname(hostname)
     try:
         certificate_pem = _get_ssl_certificate_pem(hostname, raise_exception=False)
-        certificate_info = _get_ssl_certificate_info_from_pem(certificate_pem,
-                                                              raise_exception=raise_exception,
-                                                              expires_soon_days=expires_soon_days)
+        certificate_info = _get_ssl_certificate_info_from_pem(
+            certificate_pem,
+            raise_exception=raise_exception,
+            test_mode_certificate_expiration_warning_days=test_mode_certificate_expiration_warning_days
+        )
         certificate_okay, certificate_exception = _is_ssl_certificate_okay(hostname, raise_exception=raise_exception)
+        # The hostname from _get_ssl_certificate_info_from_pem is not necessarily exactly correct;
+        # for example, for cgap-wolf.hms.harvard.edu it is imperva.com.
         certificate_info["hostname"] = hostname
         certificate_info["valid"] = certificate_info["valid"] and certificate_okay
         if certificate_exception:
             certificate_info["exception"] = str(certificate_exception)
         return certificate_info
     except Exception as e:
         if raise_exception:
@@ -47,37 +53,39 @@
     Returns the SSL certificate as a PEM string for the given hostname. If an error is encountered
     then returns None, or, if the given raise_exception argument is True then raises an exception.
     """
     try:
         with ssl.create_connection((hostname, _SSL_PORT)) as socket_connection:
             # Note that we turn off certificate verification for getting the PEM here,
             # because we want the PEM regardless of whether or not the certificate is
-            # valid; we do the real certificate sanity check in  _is_ssl_certificate_okay.
+            # valid; we do the real certificate sanity check in _is_ssl_certificate_okay.
             context = ssl.create_default_context()
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
             with context.wrap_socket(socket_connection, server_hostname=hostname) as socket_context:
                 certificate = socket_context.getpeercert(binary_form=True)
                 return ssl.DER_cert_to_PEM_cert(certificate)
     except Exception as e:
         if raise_exception:
             raise ee
         return None
 
 
 def _get_ssl_certificate_info_from_pem(pem_string: str,
                                        raise_exception: bool = False,
-                                       expires_soon_days: int = 0) -> Optional[dict]:
+                                       test_mode_certificate_expiration_warning_days: int = 0) -> Optional[dict]:
     """
     Returns a dictionary containing various data points for the given SSL certificate string
     string in PEM format. If an error is encountered in parsing this given string then returns
     None by default, or raises and exception of the given raise_exception argument is True.
     """
     now = datetime.now()
-    if not expires_soon_days or expires_soon_days <= 0:
+    if test_mode_certificate_expiration_warning_days > 0:
+        expires_soon_days = test_mode_certificate_expiration_warning_days
+    else:
         expires_soon_days = _SSL_CERTIFICATE_EXPIRES_SOON_WARNING_DAYS
 
     def get_hostnames(certificate: OpenSSL.crypto.X509) -> list:
         """
         Returns the list of hostnames associated with the given SSL certificate. There can indeed
         be more than one hostname associated with a certificate, and we cannot determine the one
         primary one associated with it, so the caller (get_ssl_certificate_info) of this (outer)
@@ -102,21 +110,24 @@
         """
         return (d - now) <= timedelta(days=ndays) if d >= now else False
 
     try:
         certificate = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, pem_string)
 
         subject = certificate.get_subject()
-        hostname = subject.commonName
+        components = subject.get_components()
+        common_name = subject.commonName
         hostnames = get_hostnames(certificate)
         owner_country = subject.countryName
         owner_state = subject.stateOrProvinceName
         owner_city = subject.localityName
         owner_entity = subject.organizationName
         owner = subject.organizationalUnitName or owner_entity
+        if not owner:
+            owner = common_name
 
         issuer = certificate.get_issuer()
         issuer_country = issuer.countryName
         issuer_state = issuer.stateOrProvinceName
         issuer_city = issuer.localityName
         issuer_entity = issuer.organizationName
         issuer = issuer.organizationalUnitName or issuer_entity
@@ -137,15 +148,15 @@
         serial_number = str(certificate.get_serial_number())
         public_key_pem = certificate.get_pubkey().to_cryptography_key().public_bytes(
             encoding = serialization.Encoding.PEM,
             format = serialization.PublicFormat.SubjectPublicKeyInfo
         ).decode("UTF-8")
 
         return {
-            "hostname": hostname,
+            "common_name": common_name,
             "hostnames": hostnames,
             "owner": owner,
             "owner_entity": owner_entity,
             "owner_country": owner_country,
             "owner_state": owner_state,
             "owner_city": owner_city,
             "issuer": issuer,
```

### Comparing `dcicutils-7.2.0.1b0/dcicutils/trace_utils.py` & `dcicutils-7.2.0.1b1/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b0/pyproject.toml` & `dcicutils-7.2.0.1b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.2.0.1b0"
+version = "7.2.0.1b1"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.2.0.1b0/PKG-INFO` & `dcicutils-7.2.0.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.2.0.1b0
+Version: 7.2.0.1b1
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

