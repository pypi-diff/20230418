# Comparing `tmp/ds_caselaw_marklogic_api_client-5.3.2.tar.gz` & `tmp/ds_caselaw_marklogic_api_client-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_caselaw_marklogic_api_client-5.3.2.tar", max compression
+gzip compressed data, was "ds_caselaw_marklogic_api_client-6.0.0.tar", max compression
```

## Comparing `ds_caselaw_marklogic_api_client-5.3.2.tar` & `ds_caselaw_marklogic_api_client-6.0.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1108 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/LICENSE.md
--rw-r--r--   0        0        0     3139 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/README.md
--rw-r--r--   0        0        0      853 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/pyproject.toml
--rw-r--r--   0        0        0    25434 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/Client.py
--rw-r--r--   0        0        0        0 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/__init__.py
--rw-r--r--   0        0        0     1954 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/content_hash.py
--rw-r--r--   0        0        0     2318 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/errors.py
--rw-r--r--   0        0        0        0 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/models/__init__.py
--rw-r--r--   0        0        0     5268 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/models/judgments.py
--rw-r--r--   0        0        0     1128 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/models/utilities/__init__.py
--rw-r--r--   0        0        0     3453 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/models/utilities/aws.py
--rw-r--r--   0        0        0        0 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/py.typed
--rw-r--r--   0        0        0     3580 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xml_tools.py
--rw-r--r--   0        0        0      220 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/break_judgment_checkout.xqy
--rw-r--r--   0        0        0      197 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/checkin_judgment.xqy
--rw-r--r--   0        0        0      385 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/checkout_judgment.xqy
--rw-r--r--   0        0        0      318 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/copy_judgment.xqy
--rw-r--r--   0        0        0      302 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/delete_judgment.xqy
--rw-r--r--   0        0        0      715 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_judgment.xqy
--rw-r--r--   0        0        0      193 2023-04-14 10:07:54.938698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_judgment_checkout_status.xqy
--rw-r--r--   0        0        0      292 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_judgment_version.xqy
--rw-r--r--   0        0        0      172 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_last_modified.xqy
--rw-r--r--   0        0        0      338 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_metadata_citation.xqy
--rw-r--r--   0        0        0      339 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_metadata_court.xqy
--rw-r--r--   0        0        0      221 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_metadata_name.xqy
--rw-r--r--   0        0        0      358 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_metadata_work_date.xqy
--rw-r--r--   0        0        0      594 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_properties_for_search_results.xqy
--rw-r--r--   0        0        0      209 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_property.xqy
--rw-r--r--   0        0        0      326 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/insert_judgment.xqy
--rw-r--r--   0        0        0      190 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/list_judgment_versions.xqy
--rw-r--r--   0        0        0      355 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_boolean_property.xqy
--rw-r--r--   0        0        0      659 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_citation.xqy
--rw-r--r--   0        0        0     1013 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_court.xqy
--rw-r--r--   0        0        0      756 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_name.xqy
--rw-r--r--   0        0        0     1762 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_this_uri.xqy
--rw-r--r--   0        0        0      939 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
--rw-r--r--   0        0        0      343 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_property.xqy
--rw-r--r--   0        0        0      420 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/update_judgment.xqy
--rw-r--r--   0        0        0      556 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/update_locked_judgment.xqy
--rw-r--r--   0        0        0      371 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/user_has_privilege.xqy
--rw-r--r--   0        0        0      246 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/user_has_role.xqy
--rw-r--r--   0        0        0      156 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/validate_all_documents.xqy
--rw-r--r--   0        0        0      199 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/xslt.xqy
--rw-r--r--   0        0        0     1381 2023-04-14 10:07:54.942698 ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/xslt_transform.xqy
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-5.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3139 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/README.md
+-rw-r--r--   0        0        0      909 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0    28243 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/Client.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/__init__.py
+-rw-r--r--   0        0        0     2236 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/content_hash.py
+-rw-r--r--   0        0        0     2318 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/errors.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/models/__init__.py
+-rw-r--r--   0        0        0     5301 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/models/judgments.py
+-rw-r--r--   0        0        0     1341 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/models/utilities/__init__.py
+-rw-r--r--   0        0        0     4098 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/models/utilities/aws.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/py.typed
+-rw-r--r--   0        0        0     3821 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xml_tools.py
+-rw-r--r--   0        0        0      220 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/break_judgment_checkout.xqy
+-rw-r--r--   0        0        0      197 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/checkin_judgment.xqy
+-rw-r--r--   0        0        0      385 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/checkout_judgment.xqy
+-rw-r--r--   0        0        0      318 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/copy_judgment.xqy
+-rw-r--r--   0        0        0      302 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/delete_judgment.xqy
+-rw-r--r--   0        0        0      715 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_judgment.xqy
+-rw-r--r--   0        0        0      193 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
+-rw-r--r--   0        0        0      292 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_judgment_version.xqy
+-rw-r--r--   0        0        0      172 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_last_modified.xqy
+-rw-r--r--   0        0        0      338 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_metadata_citation.xqy
+-rw-r--r--   0        0        0      339 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_metadata_court.xqy
+-rw-r--r--   0        0        0      221 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_metadata_name.xqy
+-rw-r--r--   0        0        0      358 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_metadata_work_date.xqy
+-rw-r--r--   0        0        0      594 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
+-rw-r--r--   0        0        0      209 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_property.xqy
+-rw-r--r--   0        0        0      326 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/insert_judgment.xqy
+-rw-r--r--   0        0        0      190 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/list_judgment_versions.xqy
+-rw-r--r--   0        0        0      355 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_boolean_property.xqy
+-rw-r--r--   0        0        0      659 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_citation.xqy
+-rw-r--r--   0        0        0     1013 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_court.xqy
+-rw-r--r--   0        0        0      756 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_name.xqy
+-rw-r--r--   0        0        0     1762 2023-04-18 14:09:57.682345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
+-rw-r--r--   0        0        0      939 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
+-rw-r--r--   0        0        0      343 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_property.xqy
+-rw-r--r--   0        0        0      420 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/update_judgment.xqy
+-rw-r--r--   0        0        0      556 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/update_locked_judgment.xqy
+-rw-r--r--   0        0        0      371 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/user_has_privilege.xqy
+-rw-r--r--   0        0        0      246 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/user_has_role.xqy
+-rw-r--r--   0        0        0      156 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/validate_all_documents.xqy
+-rw-r--r--   0        0        0      199 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/xslt.xqy
+-rw-r--r--   0        0        0     1381 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/xslt_transform.xqy
+-rw-r--r--   0        0        0     3455 2023-04-18 14:09:57.686345 ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery_type_dicts.py
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-6.0.0/PKG-INFO
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/LICENSE.md` & `ds_caselaw_marklogic_api_client-6.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/README.md` & `ds_caselaw_marklogic_api_client-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/pyproject.toml` & `ds_caselaw_marklogic_api_client-6.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ds-caselaw-marklogic-api-client"
-version = "5.3.2"
+version = "6.0.0"
 description = "An API client for interacting with the underlying data in Find Caselaw."
 authors = ["The National Archives"]
 homepage = "https://github.com/nationalarchives/ds-caselaw-custom-api-client"
 keywords = ["national archives", "caselaw"]
 readme = "README.md"
 packages = [
     { include = "caselawclient", from = "src" },
@@ -23,12 +23,14 @@
 lxml = "4.9.2"
 ds-caselaw-utils = "^1.0.0"
 boto3 = "^1.26.112"
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.3"
-pytest = "7.3.0"
+pytest = "7.3.1"
+mypy-boto3-s3 = "^1.26.104"
+mypy-boto3-sns = "^1.26.69"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/Client.py` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/Client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 import logging
 import os
 import re
 import warnings
 from datetime import datetime, time, timedelta
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Union
+from typing import Any, Optional, Set, Type, Union
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element
 
 import environ
 import requests
-from memoization import cached
 from requests.auth import HTTPBasicAuth
 from requests.structures import CaseInsensitiveDict
 from requests_toolbelt.multipart import decoder
 
 from . import xml_tools
+from . import xquery_type_dicts as query_dicts
 from .content_hash import validate_content_hash
 from .errors import MarklogicAPIError  # noqa: F401
 from .errors import (
     MarklogicBadRequestError,
     MarklogicCheckoutConflictError,
     MarklogicCommunicationError,
     MarklogicNotPermittedError,
@@ -34,59 +34,60 @@
 
 env = environ.Env()
 RESULTS_PER_PAGE = 10
 ROOT_DIR = os.path.dirname(os.path.realpath(__file__))
 DEFAULT_XSL_TRANSFORM = "accessible-html.xsl"
 
 
-def decode_multipart(response):
+def decode_multipart(response: requests.Response) -> str:
     """Decode a multipart response and return just the text inside it.
     Note that it is possible for multiple responses to be returned, if
     multiple top-level returns exist in the XQuery."""
     if not (response.content):
         return ""
     multipart_data = decoder.MultipartDecoder.from_response(response)
     part_count = len(multipart_data.parts)
     if part_count > 1:
         logging.warning(
             f"Throwing away multipart data ({part_count} items, expected 1)"
         )
-    return multipart_data.parts[0].text
+    return str(multipart_data.parts[0].text)
 
 
 class MarklogicApiClient:
-
-    http_error_classes = {
+    http_error_classes: dict[int, Type[MarklogicAPIError]] = {
         400: MarklogicBadRequestError,
         401: MarklogicUnauthorizedError,
         403: MarklogicNotPermittedError,
         404: MarklogicResourceNotFoundError,
     }
-    error_code_classes = {
+    error_code_classes: dict[str, Type[MarklogicAPIError]] = {
         "XDMP-DOCNOTFOUND": MarklogicResourceNotFoundError,
         "XDMP-LOCKCONFLICT": MarklogicResourceLockedError,
         "DLS-UNMANAGED": MarklogicResourceUnmanagedError,
         "DLS-NOTCHECKEDOUT": MarklogicResourceNotCheckedOutError,
         "DLS-CHECKOUTCONFLICT": MarklogicCheckoutConflictError,
         "SEC-PRIVDNE": MarklogicNotPermittedError,
         "XDMP-VALIDATE.*": MarklogicValidationFailedError,
     }
 
     default_http_error_class = MarklogicCommunicationError
 
-    def __init__(self, host: str, username: str, password: str, use_https: bool):
+    def __init__(
+        self, host: str, username: str, password: str, use_https: bool
+    ) -> None:
         self.host = host
         self.username = username
         self.password = password
         self.base_url = f"{'https' if use_https else 'http'}://{self.host}:8011"
         # Apply auth / common headers to the session
         self.session = requests.Session()
         self.session.auth = HTTPBasicAuth(username, password)
 
-    def _get_error_code_class(self, error_code):
+    def _get_error_code_class(self, error_code: str) -> Type[MarklogicAPIError]:
         """
         Get the exception type for a MarkLogic error code, or the first part of one
         """
         for regex, error in self.error_code_classes.items():
             if re.fullmatch(regex, error_code):
                 return error
         print(f"No error code match found for {error_code}")
@@ -94,15 +95,15 @@
 
     def _path_to_request_url(self, path: str) -> str:
         return f"{self.base_url}/{path.lstrip('/')}"
 
     def _court_list_splitter(self, court_text: str) -> Set[str]:
         return set(court_text.lower().replace(" ", "").split(","))
 
-    def _court_list(self, court_text: str) -> Optional[List[str]]:
+    def _court_list(self, court_text: str) -> Optional[list[str]]:
         if not court_text.strip():
             return None
         alt_names = {
             "ewhc/qb": "ewhc/kb",
             "ewhc/kb": "ewhc/qb",
             "ewhc/scco": "ewhc/costs",
             "ewhc/costs": "ewhc/scco",
@@ -135,34 +136,40 @@
 
             new_exception = new_error_class(
                 "{}. Response body:\n{}".format(e, response_body)
             )
             new_exception.response = response
             raise new_exception
 
-    def _format_uri_for_marklogic(self, uri):
+    def _format_uri_for_marklogic(self, uri: str) -> str:
         """
         Marklogic requires a document URI that begins with a slash `/` and ends in `.xml`.
         This method ensures any URI passed into the client matches this format.
         """
         return f"/{uri.lstrip('/').rstrip('/')}.xml"
 
-    def _xquery_path(self, xquery_file_name):
+    def _xquery_path(self, xquery_file_name: str) -> str:
         return os.path.join(ROOT_DIR, "xquery", xquery_file_name)
 
-    def _send_to_eval(self, vars, xquery_file_name):
+    def _send_to_eval(
+        self, vars: query_dicts.MarkLogicAPIDict, xquery_file_name: str
+    ) -> requests.Response:
         return self.eval(
             self._xquery_path(xquery_file_name),
             vars=json.dumps(vars),
             accept_header="application/xml",
         )
 
     def prepare_request_kwargs(
-        self, method: str, path: str, body=None, data: Optional[Dict[str, Any]] = None
-    ) -> Dict[str, Any]:
+        self,
+        method: str,
+        path: str,
+        body: Optional[str] = None,
+        data: Optional[dict[str, Any]] = None,
+    ) -> dict[str, Any]:
         kwargs = dict(url=self._path_to_request_url(path))
         if data is not None:
             data = {k: v for k, v in data.items() if v is not None}
             if method == "GET":
                 kwargs["params"] = data  # type: ignore
             else:
                 kwargs["data"] = json.dumps(data)
@@ -172,191 +179,203 @@
 
     def make_request(
         self,
         method: str,
         path: str,
         headers: CaseInsensitiveDict[Union[str, Any]],
         body: Optional[str] = None,
-        data: Optional[Dict[str, Any]] = None,
+        data: Optional[dict[str, Any]] = None,
     ) -> requests.Response:
         kwargs = self.prepare_request_kwargs(method, path, body, data)
         self.session.headers = headers
         response = self.session.request(method, **kwargs)
         # Raise relevant exception for an erroneous response
         self._raise_for_status(response)
         return response
 
-    def GET(self, path: str, headers: Dict[str, Any], **data: Any) -> requests.Response:
+    def GET(self, path: str, headers: dict[str, Any], **data: Any) -> requests.Response:
         logging.warning("GET() is deprecated, use eval() or invoke()")
         return self.make_request("GET", path, headers, data)  # type: ignore
 
     def POST(
-        self, path: str, headers: Dict[str, Any], **data: Any
+        self, path: str, headers: dict[str, Any], **data: Any
     ) -> requests.Response:
         logging.warning("POST() is deprecated, use eval() or invoke()")
         return self.make_request("POST", path, headers, data)  # type: ignore
 
     def get_judgment_xml(
-        self, judgment_uri, version_uri=None, show_unpublished=False
+        self,
+        judgment_uri: str,
+        version_uri: Optional[str] = None,
+        show_unpublished: bool = False,
     ) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
         show_unpublished = self.verify_show_unpublished(show_unpublished)
         if version_uri:
             version_uri = f"/{version_uri.lstrip('/')}.xml"
-        vars = {
+        vars: query_dicts.GetJudgmentDict = {
             "uri": uri,
             "version_uri": version_uri,
-            "show_unpublished": str(show_unpublished).lower(),
+            "show_unpublished": show_unpublished,
         }
 
         response = self._send_to_eval(vars, "get_judgment.xqy")
 
         if not response.text:
             raise MarklogicNotPermittedError(
                 "The document is not published and show_unpublished was not set"
             )
 
         return decode_multipart(response)
 
-    def get_judgment_name(self, judgment_uri) -> str:
+    def get_judgment_name(self, judgment_uri: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.GetMetadataNameDict = {"uri": uri}
 
         response = self._send_to_eval(vars, "get_metadata_name.xqy")
         if not response.text:
             return ""
 
         return decode_multipart(response)
 
-    def set_judgment_name(self, judgment_uri, content):
+    def set_judgment_name(self, judgment_uri: str, content: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri, "content": content}
+        vars: query_dicts.SetMetadataNameDict = {"uri": uri, "content": content}
 
         return self._send_to_eval(vars, "set_metadata_name.xqy")
 
-    def set_judgment_date(self, judgment_uri, content):
+    def set_judgment_date(self, judgment_uri: str, content: str) -> requests.Response:
         warnings.warn(
             "set_judgment_date() is deprecated, use set_judgment_work_expression_date()",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.set_judgment_work_expression_date(judgment_uri, content)
 
-    def set_judgment_work_expression_date(self, judgment_uri, content):
+    def set_judgment_work_expression_date(
+        self, judgment_uri: str, content: str
+    ) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri, "content": content}
+        vars: query_dicts.SetMetadataWorkExpressionDateDict = {
+            "uri": uri,
+            "content": content,
+        }
 
         return self._send_to_eval(vars, "set_metadata_work_expression_date.xqy")
 
-    def set_judgment_citation(self, judgment_uri, content):
+    def set_judgment_citation(
+        self, judgment_uri: str, content: str
+    ) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri, "content": content}
+        vars: query_dicts.SetMetadataCitationDict = {"uri": uri, "content": content}
 
         return self._send_to_eval(vars, "set_metadata_citation.xqy")
 
-    def set_judgment_court(self, judgment_uri, content):
+    def set_judgment_court(self, judgment_uri: str, content: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri, "content": content}
+        vars: query_dicts.SetMetadataCourtDict = {"uri": uri, "content": content}
 
         return self._send_to_eval(vars, "set_metadata_court.xqy")
 
-    def set_judgment_this_uri(self, judgment_uri):
+    def set_judgment_this_uri(self, judgment_uri: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
         content_with_id = (
             f"https://caselaw.nationalarchives.gov.uk/id/{judgment_uri.lstrip('/')}"
         )
         content_without_id = (
             f"https://caselaw.nationalarchives.gov.uk/{judgment_uri.lstrip('/')}"
         )
         content_with_xml = f"https://caselaw.nationalarchives.gov.uk/{judgment_uri.lstrip('/')}/data.xml"
-        vars = {
+        vars: query_dicts.SetMetadataThisUriDict = {
             "uri": uri,
             "content_with_id": content_with_id,
             "content_without_id": content_without_id,
             "content_with_xml": content_with_xml,
         }
 
         return self._send_to_eval(vars, "set_metadata_this_uri.xqy")
 
     def save_locked_judgment_xml(
-        self, judgment_uri: str, judgment_xml: bytes, annotation=None
+        self, judgment_uri: str, judgment_xml: bytes, annotation: Optional[str] = None
     ) -> requests.Response:
         """assumes the judgment is already locked, does not unlock/check in
         note this version assumes the XML is raw bytes, rather than a tree..."""
         validate_content_hash(judgment_xml)
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {
+        vars: query_dicts.UpdateLockedJudgmentDict = {
             "uri": uri,
             "judgment": judgment_xml.decode("utf-8"),
-            "annotation": annotation or "edited by save_judgment_xml",
+            "annotation": annotation or "edited by save_locked_judgment_xml",
         }
 
         return self._send_to_eval(vars, "update_locked_judgment.xqy")
 
     def save_judgment_xml(
-        self, judgment_uri: str, judgment_xml: Element, annotation=None
+        self, judgment_uri: str, judgment_xml: Element, annotation: Optional[str] = None
     ) -> requests.Response:
         """update_judgment uses dls:document-checkout-update-checkin as a single operation"""
         xml = ElementTree.tostring(judgment_xml)
 
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {
+        vars: query_dicts.UpdateJudgmentDict = {
             "uri": uri,
             "judgment": xml.decode("utf-8"),
             "annotation": annotation or "edited by save_judgment_xml",
         }
 
         return self._send_to_eval(vars, "update_judgment.xqy")
 
     def insert_judgment_xml(
         self, judgment_uri: str, judgment_xml: Element
     ) -> requests.Response:
         xml = ElementTree.tostring(judgment_xml)
 
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri, "judgment": xml.decode("utf-8"), "annotation": ""}
+        vars: query_dicts.InsertJudgmentDict = {
+            "uri": uri,
+            "judgment": xml.decode("utf-8"),
+        }
 
         return self._send_to_eval(vars, "insert_judgment.xqy")
 
     def list_judgment_versions(self, judgment_uri: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.ListJudgmentVersionsDict = {"uri": uri}
 
         return self._send_to_eval(vars, "list_judgment_versions.xqy")
 
     def checkout_judgment(
-        self, judgment_uri: str, annotation="", expires_at_midnight=False
+        self, judgment_uri: str, annotation: str = "", expires_at_midnight: bool = False
     ) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {
+        vars: query_dicts.CheckoutJudgmentDict = {
             "uri": uri,
             "annotation": annotation,
+            "timeout": -1,
         }
 
         if expires_at_midnight:
             timeout = self.calculate_seconds_until_midnight()
             vars["timeout"] = timeout
-        else:
-            vars["timeout"] = -1
 
         return self._send_to_eval(vars, "checkout_judgment.xqy")
 
     def checkin_judgment(self, judgment_uri: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.CheckinJudgmentDict = {"uri": uri}
 
         return self._send_to_eval(vars, "checkin_judgment.xqy")
 
     def get_judgment_checkout_status(self, judgment_uri: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.GetJudgmentCheckoutStatusDict = {"uri": uri}
 
         return self._send_to_eval(vars, "get_judgment_checkout_status.xqy")
 
-    def get_judgment_checkout_status_message(self, judgment_uri: str):
+    def get_judgment_checkout_status_message(self, judgment_uri: str) -> Optional[str]:
         """Return the annotation of the lock or `None` if there is no lock."""
         response = self.get_judgment_checkout_status(judgment_uri)
         if not response.content:
             return None
         content = decoder.MultipartDecoder.from_response(response).parts[0].text
         if content == "":
             return None
@@ -365,19 +384,21 @@
             "dls:annotation", namespaces={"dls": "http://marklogic.com/xdmp/dls"}
         ).text  # type: ignore
 
     def get_judgment_version(
         self, judgment_uri: str, version: int
     ) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri, "version": str(version)}
+        vars: query_dicts.GetJudgmentVersionDict = {"uri": uri, "version": str(version)}
 
         return self._send_to_eval(vars, "get_judgment_version.xqy")
 
-    def eval(self, xquery_path, vars, accept_header="multipart/mixed"):
+    def eval(
+        self, xquery_path: str, vars: str, accept_header: str = "multipart/mixed"
+    ) -> requests.Response:
         headers = {
             "Content-type": "application/x-www-form-urlencoded",
             "Accept": accept_header,
         }
         data = {
             "xquery": Path(xquery_path).read_text(),
             "vars": vars,
@@ -386,15 +407,17 @@
         response = self.session.request(
             "POST", url=self._path_to_request_url(path), headers=headers, data=data
         )
         # Raise relevant exception for an erroneous response
         self._raise_for_status(response)
         return response
 
-    def invoke(self, module, vars, accept_header="multipart/mixed"):
+    def invoke(
+        self, module: str, vars: str, accept_header: str = "multipart/mixed"
+    ) -> requests.Response:
         headers = {
             "Content-type": "application/x-www-form-urlencoded",
             "Accept": accept_header,
         }
         data = {
             "module": module,
             "vars": vars,
@@ -405,27 +428,27 @@
         )
         # Raise relevant exception for an erroneous response
         self._raise_for_status(response)
         return response
 
     def advanced_search(
         self,
-        q=None,
-        court=None,
-        judge=None,
-        party=None,
-        neutral_citation=None,
-        specific_keyword=None,
-        order=None,
-        date_from=None,
-        date_to=None,
-        page=1,
-        page_size=RESULTS_PER_PAGE,
-        show_unpublished=False,
-        only_unpublished=False,
+        q: Optional[str] = None,
+        court: Optional[str] = None,
+        judge: Optional[str] = None,
+        party: Optional[str] = None,
+        neutral_citation: Optional[str] = None,
+        specific_keyword: Optional[str] = None,
+        order: Optional[str] = None,
+        date_from: Optional[str] = None,
+        date_to: Optional[str] = None,
+        page: int = 1,
+        page_size: int = RESULTS_PER_PAGE,
+        show_unpublished: bool = False,
+        only_unpublished: bool = False,
     ) -> requests.Response:
         """
         Performs a search on the entire document set.
 
         :param q:
         :param court:
         :param judge:
@@ -460,242 +483,260 @@
                 "only_unpublished": str(only_unpublished).lower(),
             }
         )
         return self.invoke(module, vars)
 
     def eval_xslt(
         self,
-        judgment_uri,
-        version_uri=None,
-        show_unpublished=False,
-        xsl_filename=DEFAULT_XSL_TRANSFORM,
+        judgment_uri: str,
+        version_uri: Optional[str] = None,
+        show_unpublished: bool = False,
+        xsl_filename: str = DEFAULT_XSL_TRANSFORM,
     ) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
         if version_uri:
             version_uri = self._format_uri_for_marklogic(version_uri)
         if os.getenv("XSLT_IMAGE_LOCATION"):
             image_location = os.getenv("XSLT_IMAGE_LOCATION")
         else:
             image_location = ""
 
         show_unpublished = self.verify_show_unpublished(show_unpublished)
 
-        vars = {
+        vars: query_dicts.XsltTransformDict = {
             "uri": uri,
             "version_uri": version_uri,
-            "show_unpublished": str(show_unpublished).lower(),
+            "show_unpublished": show_unpublished,
             "img_location": image_location,
             "xsl_filename": xsl_filename,
         }
 
         return self._send_to_eval(vars, "xslt_transform.xqy")
 
     def accessible_judgment_transformation(
-        self, judgment_uri, version_uri=None, show_unpublished=False
-    ):
+        self,
+        judgment_uri: str,
+        version_uri: Optional[str] = None,
+        show_unpublished: bool = False,
+    ) -> requests.Response:
         return self.eval_xslt(
             judgment_uri,
             version_uri,
             show_unpublished,
             xsl_filename=DEFAULT_XSL_TRANSFORM,
         )
 
     def original_judgment_transformation(
-        self, judgment_uri, version_uri=None, show_unpublished=False
-    ):
+        self,
+        judgment_uri: str,
+        version_uri: Optional[str] = None,
+        show_unpublished: bool = False,
+    ) -> requests.Response:
         return self.eval_xslt(
             judgment_uri,
             version_uri,
             show_unpublished,
             xsl_filename="as-handed-down.xsl",
         )
 
-    def get_property(self, judgment_uri, name):
+    def get_property(self, judgment_uri: str, name: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {
+        vars: query_dicts.GetPropertyDict = {
             "uri": uri,
             "name": name,
         }
         response = self._send_to_eval(vars, "get_property.xqy")
 
         if not response.text:
             return ""
 
-        content = decoder.MultipartDecoder.from_response(response).parts[0].text
+        content = str(decoder.MultipartDecoder.from_response(response).parts[0].text)
         return content
 
-    def set_property(self, judgment_uri, name, value):
+    def set_property(
+        self, judgment_uri: str, name: str, value: str
+    ) -> requests.Response:
         uri = f"/{judgment_uri.lstrip('/')}.xml"
-        vars = {
+        vars: query_dicts.SetPropertyDict = {
             "uri": uri,
             "value": value,
             "name": name,
         }
 
         return self._send_to_eval(vars, "set_property.xqy")
 
-    def set_boolean_property(self, judgment_uri, name, value):
+    def set_boolean_property(
+        self, judgment_uri: str, name: str, value: bool
+    ) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
         string_value = "true" if value else "false"
-        vars = {
+        vars: query_dicts.SetBooleanPropertyDict = {
             "uri": uri,
             "value": string_value,
             "name": name,
         }
         return self._send_to_eval(vars, "set_boolean_property.xqy")
 
-    def get_boolean_property(self, judgment_uri, name):
+    def get_boolean_property(self, judgment_uri: str, name: str) -> bool:
         content = self.get_property(judgment_uri, name)
         return content == "true"
 
-    def set_published(self, judgment_uri, published=False):
+    def set_published(
+        self, judgment_uri: str, published: bool = False
+    ) -> requests.Response:
         return self.set_boolean_property(judgment_uri, "published", published)
 
-    def set_sensitive(self, judgment_uri, sensitive=False):
+    def set_sensitive(
+        self, judgment_uri: str, sensitive: bool = False
+    ) -> requests.Response:
         return self.set_boolean_property(judgment_uri, "sensitive", sensitive)
 
-    def set_supplemental(self, judgment_uri, supplemental=False):
+    def set_supplemental(
+        self, judgment_uri: str, supplemental: bool = False
+    ) -> requests.Response:
         return self.set_boolean_property(judgment_uri, "supplemental", supplemental)
 
-    def set_anonymised(self, judgment_uri, anonymised=False):
+    def set_anonymised(
+        self, judgment_uri: str, anonymised: bool = False
+    ) -> requests.Response:
         return self.set_boolean_property(judgment_uri, "anonymised", anonymised)
 
-    def get_published(self, judgment_uri):
+    def get_published(self, judgment_uri: str) -> bool:
         return self.get_boolean_property(judgment_uri, "published")
 
-    def get_sensitive(self, judgment_uri):
+    def get_sensitive(self, judgment_uri: str) -> bool:
         return self.get_boolean_property(judgment_uri, "sensitive")
 
-    def get_supplemental(self, judgment_uri):
+    def get_supplemental(self, judgment_uri: str) -> bool:
         return self.get_boolean_property(judgment_uri, "supplemental")
 
-    def get_anonymised(self, judgment_uri):
+    def get_anonymised(self, judgment_uri: str) -> bool:
         return self.get_boolean_property(judgment_uri, "anonymised")
 
-    def get_last_modified(self, judgment_uri):
+    def get_last_modified(self, judgment_uri: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {
+        vars: query_dicts.GetLastModifiedDict = {
             "uri": uri,
         }
 
         response = self._send_to_eval(vars, "get_last_modified.xqy")
 
         if not response.text:
             return ""
 
-        content = decoder.MultipartDecoder.from_response(response).parts[0].text
+        content = str(decoder.MultipartDecoder.from_response(response).parts[0].text)
         return content
 
-    def delete_judgment(self, judgment_uri):
+    def delete_judgment(self, judgment_uri: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.DeleteJudgmentDict = {"uri": uri}
         return self._send_to_eval(vars, "delete_judgment.xqy")
 
-    def copy_judgment(self, old, new):
+    def copy_judgment(self, old: str, new: str) -> requests.Response:
         old_uri = self._format_uri_for_marklogic(old)
         new_uri = self._format_uri_for_marklogic(new)
 
-        vars = {
+        vars: query_dicts.CopyJudgmentDict = {
             "old_uri": old_uri,
             "new_uri": new_uri,
         }
         return self._send_to_eval(vars, "copy_judgment.xqy")
 
-    def break_checkout(self, judgment_uri):
+    def break_checkout(self, judgment_uri: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {
+        vars: query_dicts.BreakJudgmentCheckoutDict = {
             "uri": uri,
         }
         return self._send_to_eval(vars, "break_judgment_checkout.xqy")
 
-    def user_has_privilege(self, username, privilege_uri, privilege_action):
-        vars = {
+    def user_has_privilege(
+        self, username: str, privilege_uri: str, privilege_action: str
+    ) -> requests.Response:
+        vars: query_dicts.UserHasPrivilegeDict = {
             "user": username,
             "privilege_uri": privilege_uri,
             "privilege_action": privilege_action,
         }
         return self._send_to_eval(vars, "user_has_privilege.xqy")
 
-    @cached
-    def user_can_view_unpublished_judgments(self, username):
+    def user_can_view_unpublished_judgments(self, username: str) -> bool:
         if self.user_has_admin_role(username):
             return True
 
         check_privilege = self.user_has_privilege(
             username,
             "https://caselaw.nationalarchives.gov.uk/custom/privileges/can-view-unpublished-documents",
             "execute",
         )
         return decode_multipart(check_privilege).lower() == "true"
 
-    def user_has_role(self, username, role):
-        vars = {
+    def user_has_role(self, username: str, role: str) -> requests.Response:
+        vars: query_dicts.UserHasRoleDict = {
             "user": username,
             "role": role,
         }
         return self._send_to_eval(vars, "user_has_role.xqy")
 
-    @cached
-    def user_has_admin_role(self, username):
+    def user_has_admin_role(self, username: str) -> bool:
         check_role = self.user_has_role(
             username,
             "admin",
         )
         multipart_data = decoder.MultipartDecoder.from_response(check_role)
-        result = multipart_data.parts[0].text
+        result = str(multipart_data.parts[0].text)
         return result.lower() == "true"
 
-    def calculate_seconds_until_midnight(self, now=None):
+    def calculate_seconds_until_midnight(self, now: Optional[datetime] = None) -> int:
         """
         Get timedelta until end of day on the datetime passed, or current time.
         https://stackoverflow.com/questions/45986035/seconds-until-end-of-day-in-python
         """
         if not now:
             now = datetime.now()
         tomorrow = now + timedelta(days=1)
         difference = datetime.combine(tomorrow, time.min) - now
 
         return difference.seconds
 
-    def verify_show_unpublished(self, show_unpublished):
+    def verify_show_unpublished(self, show_unpublished: bool) -> bool:
         if show_unpublished and not self.user_can_view_unpublished_judgments(
             self.username
         ):
             # The user cannot view unpublished judgments but is requesting to see them
             logging.warning(
                 f"User {self.username} is attempting to view unpublished judgments but does not have that privilege."
             )
             return False
         return show_unpublished
 
-    def get_judgment_citation(self, judgment_uri) -> str:
+    def get_judgment_citation(self, judgment_uri: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.GetMetadataCitationDict = {"uri": uri}
 
         response = self._send_to_eval(vars, "get_metadata_citation.xqy")
         return decode_multipart(response)
 
-    def get_judgment_court(self, judgment_uri):
+    def get_judgment_court(self, judgment_uri: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.GetMetadataCourtDict = {"uri": uri}
         response = self._send_to_eval(vars, "get_metadata_court.xqy")
         return decode_multipart(response)
 
-    def get_judgment_work_date(self, judgment_uri):
+    def get_judgment_work_date(self, judgment_uri: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
-        vars = {"uri": uri}
+        vars: query_dicts.GetMetadataWorkDateDict = {"uri": uri}
         response = self._send_to_eval(vars, "get_metadata_work_date.xqy")
         return decode_multipart(response)
 
-    def get_properties_for_search_results(self, judgment_uris):
+    def get_properties_for_search_results(self, judgment_uris: list[str]) -> str:
         uris = [
             self._format_uri_for_marklogic(judgment_uri)
             for judgment_uri in judgment_uris
         ]
-        vars = {"uris": uris}
+        vars: query_dicts.GetPropertiesForSearchResultsDict = {"uris": uris}
         response = self._send_to_eval(vars, "get_properties_for_search_results.xqy")
         return decode_multipart(response)
 
 
 api_client = MarklogicApiClient(
     host=env("MARKLOGIC_HOST", default=None),
     username=env("MARKLOGIC_USER", default=None),
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/content_hash.py` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/content_hash.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,20 +12,15 @@
 from hashlib import sha256
 
 import lxml.etree
 
 from .errors import InvalidContentHashError
 
 
-def hash_of_content(doc: bytes) -> str:
-    """Return the content hash for a document"""
-    return sha256(hashable_text(doc)).hexdigest()
-
-
-def hashable_text(doc: bytes) -> bytes:
+def get_hashable_text(doc: bytes) -> bytes:
     """Extract the text (as UTF-8 bytes) that would be hashed"""
     root = lxml.etree.fromstring(doc)
     metadatas = root.xpath(
         "//akn:meta",
         namespaces={"akn": "http://docs.oasis-open.org/legaldocml/ns/akn/3.0"},
     )
     for (
@@ -33,23 +28,35 @@
     ) in metadatas:  # there should be no more than one, but handle zero case gracefully
         metadata.getparent().remove(metadata)
     text = "".join(root.itertext())
     spaceless = re.sub(r"\s", "", text)
     return spaceless.encode("utf-8")
 
 
-def validate_content_hash(doc: bytes) -> str:
-    """Check a document's self-described content hash is the same as the hash of its content, raise an error if not"""
+def get_hash_from_document(doc: bytes) -> str:
+    """Get the content hash of an XML document from its contents"""
+    return sha256(get_hashable_text(doc)).hexdigest()
+
+
+def get_hash_from_tag(doc: bytes) -> str:
+    """Get the content hash of an XML document from its uk:hash tag (if present)."""
     root = lxml.etree.fromstring(doc)
     try:
         hash_from_tag = root.xpath(
             "//uk:hash/text()",
             namespaces={"uk": "https://caselaw.nationalarchives.gov.uk/akn"},
         )[0]
     except IndexError:
         raise InvalidContentHashError("Document did not have a content hash tag")
-    content_hash = hash_of_content(doc)
-    if hash_from_tag != content_hash:
+
+    return str(hash_from_tag)
+
+
+def validate_content_hash(doc: bytes) -> str:
+    """Check a document's self-described content hash is the same as the hash of its content, raise an error if not"""
+    hash_from_document = get_hash_from_document(doc)
+    hash_from_tag = get_hash_from_tag(doc)
+    if hash_from_document != hash_from_tag:
         raise InvalidContentHashError(
-            f"Hash of document was {hash_from_tag} but the content hash was {content_hash}"
+            f'Hash of existing tag is "{hash_from_tag}" but the hash of the document is "{hash_from_document}"'
         )
-    return content_hash
+    return hash_from_document
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/errors.py` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/errors.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/models/judgments.py` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/models/judgments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from functools import cached_property
 
 from requests_toolbelt.multipart import decoder
 
 from caselawclient.Client import MarklogicApiClient
 
-from .utilities import get_judgment_root, render_versions
+from .utilities import VersionsDict, get_judgment_root, render_versions
 from .utilities.aws import (
     generate_docx_url,
     generate_pdf_url,
     notify_changed,
     publish_documents,
     unpublish_documents,
     uri_for_s3,
@@ -99,15 +99,15 @@
         return generate_pdf_url(uri_for_s3(self.uri))
 
     @cached_property
     def assigned_to(self) -> str:
         return self.api_client.get_property(self.uri, "assigned-to")
 
     @cached_property
-    def versions(self) -> list:
+    def versions(self) -> list[VersionsDict]:
         versions_response = self.api_client.list_judgment_versions(self.uri)
 
         try:
             decoded_versions = decoder.MultipartDecoder.from_response(versions_response)
             return render_versions(decoded_versions.parts)
         except AttributeError:
             return []
@@ -116,15 +116,15 @@
         return self.api_client.get_judgment_xml(self.uri, show_unpublished=True)
 
     def content_as_html(self, version_uri: str) -> str:
         results = self.api_client.eval_xslt(
             self.uri, version_uri, show_unpublished=True
         )
         multipart_data = decoder.MultipartDecoder.from_response(results)
-        return multipart_data.parts[0].text
+        return str(multipart_data.parts[0].text)
 
     @cached_property
     def is_failure(self) -> bool:
         if "failures" in self.uri:
             return True
         return False
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/models/utilities/__init__.py` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/models/utilities/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import re
 import xml.etree.ElementTree as ET
+from typing import TypedDict
+
+from requests_toolbelt.multipart.decoder import BodyPart
 
 VERSION_REGEX = r"xml_versions/(\d{1,10})-(\d{1,10}|TDR)"
 # Here we limit the number of digits in the version and document reference to 10 on purpose, see
 # https://owasp.org/www-community/attacks/Regular_expression_Denial_of_Service_-_ReDoS for an explanation of why.
 
 akn_namespace = {"akn": "http://docs.oasis-open.org/legaldocml/ns/akn/3.0"}
 uk_namespace = {"uk": "https://caselaw.nationalarchives.gov.uk/akn"}
 
 
-def get_judgment_root(judgment_xml) -> str:
+def get_judgment_root(judgment_xml: str) -> str:
     try:
         parsed_xml = ET.XML(bytes(judgment_xml, encoding="utf-8"))
         return parsed_xml.tag
     except ET.ParseError:
         return "error"
 
 
-def render_versions(decoded_versions):
-    versions = [
+class VersionsDict(TypedDict):
+    uri: str
+    version: int
+
+
+def render_versions(decoded_versions: list[BodyPart]) -> list[VersionsDict]:
+    versions: list[VersionsDict] = [
         {
             "uri": part.text.rstrip(".xml"),
             "version": extract_version(part.text),
         }
         for part in decoded_versions
     ]
     sorted_versions = sorted(versions, key=lambda d: -d["version"])
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/models/utilities/aws.py` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/models/utilities/aws.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,91 @@
 import json
 import logging
+from typing import Any, Literal, Union, overload
 
 import boto3
 import botocore.client
 import environ
+from mypy_boto3_s3.client import S3Client
+from mypy_boto3_s3.type_defs import CopySourceTypeDef, ObjectIdentifierTypeDef
+from mypy_boto3_sns.client import SNSClient
+from mypy_boto3_sns.type_defs import MessageAttributeValueTypeDef
 
 env = environ.Env()
 
 
-def create_aws_client(service: str):  # service
-    """@param: service The AWS service, e.g. 's3'"""
+@overload
+def create_aws_client(service: Literal["s3"]) -> S3Client:
+    ...
+
+
+@overload
+def create_aws_client(service: Literal["sns"]) -> SNSClient:
+    ...
+
+
+def create_aws_client(service: Union[Literal["s3"], Literal["sns"]]) -> Any:
     aws = boto3.session.Session(
         aws_access_key_id=env("AWS_ACCESS_KEY_ID", default=None),
         aws_secret_access_key=env("AWS_SECRET_KEY", default=None),
     )
     return aws.client(
         service,
         endpoint_url=env("AWS_ENDPOINT_URL", default=None),
         region_name=env("PRIVATE_ASSET_BUCKET_REGION", default=None),
         config=botocore.client.Config(signature_version="s3v4"),
     )
 
 
-def create_s3_client():
+def create_s3_client() -> S3Client:
     return create_aws_client("s3")
 
 
-def uri_for_s3(uri: str):
+def create_sns_client() -> SNSClient:
+    return create_aws_client("sns")
+
+
+def uri_for_s3(uri: str) -> str:
     return uri.lstrip("/")
 
 
-def generate_signed_asset_url(key: str):
+def generate_signed_asset_url(key: str) -> str:
     # If there isn't a PRIVATE_ASSET_BUCKET, don't try to get the bucket.
     # This helps local environment setup where we don't use S3.
     bucket = env("PRIVATE_ASSET_BUCKET", None)
     if not bucket:
         return ""
 
     client = create_s3_client()
 
-    return client.generate_presigned_url(
-        "get_object", Params={"Bucket": bucket, "Key": key}
+    return str(
+        client.generate_presigned_url(
+            "get_object", Params={"Bucket": bucket, "Key": key}
+        )
     )
 
 
-def generate_docx_url(uri: str):
+def generate_docx_url(uri: str) -> str:
     key = f'{uri}/{uri.replace("/", "_")}.docx'
 
     return generate_signed_asset_url(key)
 
 
-def generate_pdf_url(uri: str):
+def generate_pdf_url(uri: str) -> str:
     key = f'{uri}/{uri.replace("/", "_")}.pdf'
 
     return generate_signed_asset_url(key)
 
 
 def delete_from_bucket(uri: str, bucket: str) -> None:
     client = create_s3_client()
     response = client.list_objects(Bucket=bucket, Prefix=uri)
 
     if response.get("Contents"):
-        objects_to_delete = [
+        objects_to_delete: list[ObjectIdentifierTypeDef] = [
             {"Key": obj["Key"]} for obj in response.get("Contents", [])
         ]
         client.delete_objects(
             Bucket=bucket,
             Delete={
                 "Objects": objects_to_delete,
             },
@@ -80,32 +100,32 @@
 
     response = client.list_objects(Bucket=private_bucket, Prefix=uri)
 
     for result in response.get("Contents", []):
         key = str(result["Key"])
 
         if not key.endswith("parser.log") and not key.endswith(".tar.gz"):
-            source = {"Bucket": private_bucket, "Key": key}
+            source: CopySourceTypeDef = {"Bucket": private_bucket, "Key": key}
             extra_args = {"ACL": "public-read"}
             try:
                 client.copy(source, public_bucket, key, extra_args)
             except botocore.client.ClientError as e:
                 logging.warning(
                     f"Unable to copy file {key} to new location {public_bucket}, error: {e}"
                 )
 
 
 def unpublish_documents(uri: str) -> None:
     delete_from_bucket(uri, env("PUBLIC_ASSET_BUCKET"))
 
 
 def notify_changed(uri: str, status: str, enrich: bool = False) -> None:
-    client = create_aws_client("sns")
+    client = create_sns_client()
 
-    message_attributes = {}
+    message_attributes: dict[str, MessageAttributeValueTypeDef] = {}
     message_attributes["update_type"] = {
         "DataType": "String",
         "StringValue": status,
     }
     message_attributes["uri_reference"] = {
         "DataType": "String",
         "StringValue": uri,
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xml_tools.py` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xml_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,128 @@
 import logging
-from typing import List
-from xml.etree import ElementTree
-from xml.etree.ElementTree import Element, ParseError
+from typing import List, Optional
+from xml.etree.ElementTree import (
+    Element,
+    ElementTree,
+    ParseError,
+    QName,
+    fromstring,
+    tostring,
+)
 
 akn_uk_namespaces = {
     "akn": "http://docs.oasis-open.org/legaldocml/ns/akn/3.0",
     "uk": "https://caselaw.nationalarchives.gov.uk/akn",
 }
 akn_namespace_uri = "http://docs.oasis-open.org/legaldocml/ns/akn/3.0"
 uk_namespace_uri = "https://caselaw.nationalarchives.gov.uk/akn"
 search_namespace = {"search": "http://marklogic.com/appservices/search"}
 
 
 class JudgmentMissingMetadataError(IndexError):
     pass
 
 
-def get_metadata_name_value(xml: Element) -> str:
-    name = get_metadata_name_element(xml)
-    value = name.attrib["value"]
-    if value is None:
-        return ""
-    return value
-
-
 def get_element(
-    xml: Element,
-    xpath,
-    element_name="FRBRname",
-    element_namespace=akn_namespace_uri,
-    has_value_attribute=True,
+    xml: ElementTree,
+    xpath: str,
+    element_name: str = "FRBRname",
+    element_namespace: str = akn_namespace_uri,
+    has_value_attribute: bool = True,
 ) -> Element:
     logging.warning(
         "XMLTools is deprecated and will be removed in later versions. "
         "Use methods from MarklogicApiClient.Client instead."
     )
     name = xml.find(
         xpath,
         namespaces=akn_uk_namespaces,
     )
 
     if name is None:
-        element = ElementTree.Element(
-            ElementTree.QName(element_namespace, element_name)  # type: ignore
-        )
+        element = Element(QName(element_namespace, element_name))  # type: ignore
         if has_value_attribute:
             element.set("value", "")
         return element
 
     return name
 
 
-def get_neutral_citation_name_value(xml):
-    return get_neutral_citation_element(xml).text
-
-
-def get_judgment_date_value(xml):
-    return get_judgment_date_element(xml).attrib["date"]
-
-
-def get_court_value(xml):
-    return get_court_element(xml).text
-
-
-def get_metadata_name_element(xml) -> Element:
-    return get_element(xml, ".//akn:FRBRname", "FRBRname", akn_namespace_uri, True)
+def get_neutral_citation_element(xml: ElementTree) -> Element:
+    return get_element(xml, ".//uk:cite", "cite", uk_namespace_uri, False)
 
 
-def get_neutral_citation_element(xml) -> Element:
-    return get_element(xml, ".//uk:cite", "cite", uk_namespace_uri, False)
+def get_neutral_citation_name_value(xml: ElementTree) -> Optional[str]:
+    return get_neutral_citation_element(xml).text
 
 
-def get_judgment_date_element(xml) -> Element:
+def get_judgment_date_element(xml: ElementTree) -> Element:
     logging.warning(
         "XMLTools is deprecated and will be removed in later versions. "
         "Use methods from MarklogicApiClient.Client instead."
     )
     name = xml.find(
         ".//akn:FRBRWork/akn:FRBRdate",
         namespaces=akn_uk_namespaces,
     )
 
     if name is None:
-        element = ElementTree.Element(ElementTree.QName(akn_namespace_uri, "FRBRdate"))  # type: ignore
+        element = Element(QName(akn_namespace_uri, "FRBRdate"))  # type: ignore
         element.set("date", "")
         element.set("name", "judgment")
 
         return element
 
     return name
 
 
-def get_court_element(xml) -> Element:
+def get_judgment_date_value(xml: ElementTree) -> str:
+    return get_judgment_date_element(xml).attrib["date"]
+
+
+def get_court_element(xml: ElementTree) -> Element:
     return get_element(xml, ".//uk:court", "court", uk_namespace_uri, False)
 
 
-def get_search_matches(element: Element) -> List[str]:
+def get_court_value(xml: ElementTree) -> Optional[str]:
+    return get_court_element(xml).text
+
+
+def get_metadata_name_element(xml: ElementTree) -> Element:
+    return get_element(xml, ".//akn:FRBRname", "FRBRname", akn_namespace_uri, True)
+
+
+def get_metadata_name_value(xml: ElementTree) -> str:
+    name = get_metadata_name_element(xml)
+    value = name.attrib["value"]
+    if value is None:
+        return ""
+    return value
+
+
+def get_search_matches(element: ElementTree) -> List[str]:
     logging.warning(
         "XMLTools is deprecated and will be removed in later versions. "
         "Use methods from MarklogicApiClient.Client instead."
     )
     nodes = element.findall(".//search:match", namespaces=search_namespace)
     results = []
     for node in nodes:
-        text = ElementTree.tostring(node, method="text", encoding="UTF-8")
+        text = tostring(node, method="text", encoding="UTF-8")
         results.append(text.decode("UTF-8").strip())
     return results
 
 
-def get_error_code(xml_content: str):
+def get_error_code(xml_content: Optional[str]) -> str:
     logging.warning(
         "XMLTools is deprecated and will be removed in later versions. "
         "Use methods from MarklogicApiClient.Client instead."
     )
+    if not xml_content:
+        return "Unknown error, Marklogic returned a null or empty response"
     try:
-        xml = ElementTree.fromstring(xml_content)
+        xml = fromstring(xml_content)
         return xml.find(
             "message-code", namespaces={"": "http://marklogic.com/xdmp/error"}
         ).text  # type: ignore
     except (ParseError, TypeError, AttributeError):
         return "Unknown error, Marklogic returned a null or empty response"
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_judgment.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/get_properties_for_search_results.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_citation.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_citation.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_court.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_court.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_name.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_name.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_this_uri.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/set_metadata_work_expression_date.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/update_locked_judgment.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/update_locked_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/src/caselawclient/xquery/xslt_transform.xqy` & `ds_caselaw_marklogic_api_client-6.0.0/src/caselawclient/xquery/xslt_transform.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.2/PKG-INFO` & `ds_caselaw_marklogic_api_client-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-marklogic-api-client
-Version: 5.3.2
+Version: 6.0.0
 Summary: An API client for interacting with the underlying data in Find Caselaw.
 Home-page: https://github.com/nationalarchives/ds-caselaw-custom-api-client
 Keywords: national archives,caselaw
 Author: The National Archives
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

