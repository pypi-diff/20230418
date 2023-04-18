# Comparing `tmp/dcicutils-7.2.0.1b1.tar.gz` & `tmp/dcicutils-7.2.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.2.0.1b1.tar", max compression
+gzip compressed data, was "dcicutils-7.2.0.1b2.tar", max compression
```

## Comparing `dcicutils-7.2.0.1b1.tar` & `dcicutils-7.2.0.1b2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1166 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/README.rst
--rw-r--r--   0        0        0        0 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9257 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    11502 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-18 15:10:17.742924 dcicutils-7.2.0.1b1/dcicutils/log_utils.py
--rw-r--r--   0        0        0    87196 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   120743 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    19745 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0    10090 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     1769 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3680 2023-04-18 15:10:17.746924 dcicutils-7.2.0.1b1/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 dcicutils-7.2.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-18 15:27:06.157824 dcicutils-7.2.0.1b2/README.rst
+-rw-r--r--   0        0        0        0 2023-04-18 15:27:06.157824 dcicutils-7.2.0.1b2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    52659 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    13639 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     1649 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9257 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    37025 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    87196 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20232 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   120743 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    19745 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0    10025 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3680 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 dcicutils-7.2.0.1b2/PKG-INFO
```

### Comparing `dcicutils-7.2.0.1b1/README.rst` & `dcicutils-7.2.0.1b2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/base.py` & `dcicutils-7.2.0.1b2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/beanstalk_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/cloudformation_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/codebuild_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/command_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/common.py` & `dcicutils-7.2.0.1b2/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/creds_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/data_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/deployment_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/diff_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/docker_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/ecr_scripts.py` & `dcicutils-7.2.0.1b2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/ecr_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/ecs_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/env_base.py` & `dcicutils-7.2.0.1b2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/env_manager.py` & `dcicutils-7.2.0.1b2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/env_scripts.py` & `dcicutils-7.2.0.1b2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/env_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/env_utils_legacy.py` & `dcicutils-7.2.0.1b2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/es_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/exceptions.py` & `dcicutils-7.2.0.1b2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/ff_mocks.py` & `dcicutils-7.2.0.1b2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/ff_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/jh_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/kibana/dashboards.json` & `dcicutils-7.2.0.1b2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/kibana/readme.md` & `dcicutils-7.2.0.1b2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/lang_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/log_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/misc_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/obfuscation_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/opensearch_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/qa_checkers.py` & `dcicutils-7.2.0.1b2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/qa_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/redis_tools.py` & `dcicutils-7.2.0.1b2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/redis_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/s3_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/secrets_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/snapshot_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/ssl_certificate_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cryptography.hazmat.primitives import serialization
 from datetime import datetime, timedelta
 import OpenSSL
 import socket
 import ssl
-from typing import Any, Optional, Tuple, Union
+from typing import Optional, Tuple
 
 
 def get_ssl_certificate_info(hostname: str,
                              raise_exception: bool = False,
                              test_mode_certificate_expiration_warning_days: int = 0) -> Optional[dict]:
     """
     Returns a dictionary containing various data points for the SSL certificate of the given
@@ -62,15 +62,15 @@
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
             with context.wrap_socket(socket_connection, server_hostname=hostname) as socket_context:
                 certificate = socket_context.getpeercert(binary_form=True)
                 return ssl.DER_cert_to_PEM_cert(certificate)
     except Exception as e:
         if raise_exception:
-            raise ee
+            raise e
         return None
 
 
 def _get_ssl_certificate_info_from_pem(pem_string: str,
                                        raise_exception: bool = False,
                                        test_mode_certificate_expiration_warning_days: int = 0) -> Optional[dict]:
     """
@@ -110,15 +110,14 @@
         """
         return (d - now) <= timedelta(days=ndays) if d >= now else False
 
     try:
         certificate = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, pem_string)
 
         subject = certificate.get_subject()
-        components = subject.get_components()
         common_name = subject.commonName
         hostnames = get_hostnames(certificate)
         owner_country = subject.countryName
         owner_state = subject.stateOrProvinceName
         owner_city = subject.localityName
         owner_entity = subject.organizationName
         owner = subject.organizationalUnitName or owner_entity
@@ -134,25 +133,25 @@
 
         not_before = certificate.get_notBefore().decode("UTF-8")
         not_after = certificate.get_notAfter().decode("UTF-8")
         active_at = datetime.strptime(not_before, "%Y%m%d%H%M%SZ")
         expires_at = datetime.strptime(not_after, "%Y%m%d%H%M%SZ")
         expires_soon = is_datetime_within_ndays(expires_at, expires_soon_days)
 
-        expired = now >= expires_at 
-        inactive = now <= active_at 
+        expired = now >= expires_at
+        inactive = now <= active_at
         valid = not inactive and not expired
 
         # Note we could not currently get detect specifically if the certificate is revoked;
         # could not get the recommeneded code working consistently; no great matter.
 
         serial_number = str(certificate.get_serial_number())
         public_key_pem = certificate.get_pubkey().to_cryptography_key().public_bytes(
-            encoding = serialization.Encoding.PEM,
-            format = serialization.PublicFormat.SubjectPublicKeyInfo
+            encoding=serialization.Encoding.PEM,
+            format=serialization.PublicFormat.SubjectPublicKeyInfo
         ).decode("UTF-8")
 
         return {
             "common_name": common_name,
             "hostnames": hostnames,
             "owner": owner,
             "owner_entity": owner_entity,
```

### Comparing `dcicutils-7.2.0.1b1/dcicutils/trace_utils.py` & `dcicutils-7.2.0.1b2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b1/pyproject.toml` & `dcicutils-7.2.0.1b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.2.0.1b1"
+version = "7.2.0.1b2"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.2.0.1b1/PKG-INFO` & `dcicutils-7.2.0.1b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.2.0.1b1
+Version: 7.2.0.1b2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

