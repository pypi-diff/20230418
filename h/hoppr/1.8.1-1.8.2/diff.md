# Comparing `tmp/hoppr-1.8.1.tar.gz` & `tmp/hoppr-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.1.tar", max compression
+gzip compressed data, was "hoppr-1.8.2.tar", max compression
```

## Comparing `hoppr-1.8.1.tar` & `hoppr-1.8.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-04-12 18:43:58.000000 hoppr-1.8.1/LICENSE
--rw-r--r--   0        0        0     1214 2023-04-12 18:43:58.000000 hoppr-1.8.1/README.md
--rw-r--r--   0        0        0     1035 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    10990 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10732 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12941 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10236 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     3321 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     4082 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6369 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7927 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4472 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3127 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5403 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4577 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     4810 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/in_toto.py
--rw-r--r--   0        0        0     3074 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/base.py
--rw-r--r--   0        0        0     3778 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17044 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/py.typed
--rw-r--r--   0        0        0     3975 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/transfer.py
--rw-r--r--   0        0        0     1353 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    25427 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/result.py
--rw-r--r--   0        0        0     5305 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/utils.py
--rw-r--r--   0        0        0     3613 2023-04-12 18:43:58.000000 hoppr-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-18 17:17:59.000000 hoppr-1.8.2/LICENSE
+-rw-r--r--   0        0        0     1214 2023-04-18 17:17:59.000000 hoppr-1.8.2/README.md
+-rw-r--r--   0        0        0     1035 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    10990 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10732 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12943 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10272 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     3321 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     3992 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6369 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7978 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4429 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3043 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5403 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4577 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     4810 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3074 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/base.py
+-rw-r--r--   0        0        0     3778 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17515 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/py.typed
+-rw-r--r--   0        0        0     3975 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     4118 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    25427 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/result.py
+-rw-r--r--   0        0        0     5305 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/utils.py
+-rw-r--r--   0        0        0     3614 2023-04-18 17:17:59.000000 hoppr-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.2/PKG-INFO
```

### Comparing `hoppr-1.8.1/LICENSE` & `hoppr-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/README.md` & `hoppr-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/__init__.py` & `hoppr-1.8.2/hoppr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.1"
+__version__ = "1.8.2"
```

### Comparing `hoppr-1.8.1/hoppr/base_plugins/collector.py` & `hoppr-1.8.2/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.2/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/cli/hopctl.py` & `hoppr-1.8.2/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/constants.py` & `hoppr-1.8.2/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.2/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         super().__init__(
             context=context,
             config=config,
         )
 
         self.manifest_repos: list[str] = []
 
-        self.manifest_repos = [repo.url for repo in self.context.repositories[PurlType.DEB]]
+        self.manifest_repos = [f"{repo.url}" for repo in self.context.repositories[PurlType.DEB]]
 
         proxy_args = self._repo_proxy()
         self.config_dir = Path(config_dir)
 
         self.apt_paths_dict: Mapping[str, Mapping] = {
             "etc": {
                 "apt": {"auth.conf": None, "preferences.d": {}, "sources.list": None, "sources.list.d": {}},
@@ -187,18 +187,18 @@
 
     def _populate_auth_conf(self, repo_list: list[Repository], file: Path) -> None:
         """
         Populate Apt authentication config file
         """
         creds: list[str] = []
         for repo in repo_list:
-            repo_credentials = Credentials.find(repo.url)
+            repo_credentials = Credentials.find(f"{repo.url}")
             if repo_credentials is not None:
                 creds.append(
-                    f"machine {urlparse(repo.url).netloc} "
+                    f"machine {repo.url.hostname} "
                     f"login {repo_credentials.username} "
                     f"password {repo_credentials.password.get_secret_value()}\n"
                 )
 
         # Set restrictive permissions on Apt authentication config file
         file.chmod(mode=0o600)
```

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import shutil
 
 from configparser import ConfigParser
 from os import PathLike
 from pathlib import Path
 from time import sleep
-from urllib.parse import quote_plus, urljoin, urlparse
+from urllib.parse import quote_plus, urlparse
 
 import requests
 
 from packageurl import PackageURL
 from requests.auth import HTTPBasicAuth
 
 import hoppr.net
@@ -23,15 +23,15 @@
 from hoppr import __version__
 from hoppr.base_plugins.collector import BatchCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_process, hoppr_rerunner
 from hoppr.exceptions import HopprPluginError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import Credentials
 from hoppr.models.manifest import Component
-from hoppr.models.types import PurlType
+from hoppr.models.types import PurlType, RepositoryUrl
 from hoppr.result import Result
 
 
 def _artifact_string(purl: PackageURL) -> str:
     artifact_string = purl.name
 
     if purl.version is not None:
@@ -39,26 +39,26 @@
     if purl.qualifiers.get("arch") is not None:
         artifact_string = ".".join([artifact_string, purl.qualifiers.get("arch")])
 
     return artifact_string
 
 
 def _is_rpm_repo(repo_url: str) -> bool:
-    url = urljoin(f"{repo_url}/", "repodata/repomd.xml")
+    url = RepositoryUrl(url=repo_url) / "repodata/repomd.xml"
 
     basic_auth = None
     creds = Credentials.find(repo_url)
     if creds is not None:
         basic_auth = HTTPBasicAuth(username=creds.username, password=creds.password.get_secret_value())
 
     for attempt in range(3):
         if attempt > 0:
             sleep(5)
 
-        resp = requests.get(url, auth=basic_auth, allow_redirects=False, stream=True, verify=True, timeout=60)
+        resp = requests.get(f"{url}", auth=basic_auth, allow_redirects=False, stream=True, verify=True, timeout=60)
         if resp.status_code < 300:
             return True
         if resp.status_code < 500:
             return False
 
     return False
 
@@ -91,15 +91,15 @@
         context: HopprContext,
         config: dict | None = None,
         config_file: str | PathLike = Path.cwd() / ".hoppr-dnf" / "dnf.conf",
     ) -> None:
         super().__init__(context=context, config=config)
 
         self.password_list: list[str] = []
-        self.manifest_repos: list[str] = [repo.url for repo in self.context.repositories[PurlType.RPM]]
+        self.manifest_repos: list[str] = [f"{repo.url}" for repo in self.context.repositories[PurlType.RPM]]
         self.config_file = Path(config_file)
 
         if self.config and "dnf_command" in self.config:
             self.required_commands = [self.config["dnf_command"]]
 
         self.base_command = [
             self.required_commands[0],
@@ -138,31 +138,31 @@
     @hoppr_process
     def pre_stage_process(self) -> Result:
         repo_config = ConfigParser()
         repo_config["main"] = dict(cachedir=f"{self.config_file.parent / 'cache'}")
 
         for idx, repo in enumerate(self.context.repositories[PurlType.RPM]):
             temp_repo = f"hoppr-tmp-{idx}"
-            creds = Credentials.find(repo.url)
+            creds = Credentials.find(f"{repo.url}")
 
-            if not _is_rpm_repo(repo.url):
+            if not _is_rpm_repo(f"{repo.url}"):
                 self.get_logger().warning(
                     f"Repo {repo.url} is not an RPM repository (repomd.xml file not found), will not be searched"
                 )
                 continue
 
             self.get_logger().debug(f"Creating repo {temp_repo} for url {repo.url}")
 
             # Create temporary repository file
             repo_config[temp_repo] = {
                 "baseurl": f"{repo.url}",
                 "enabled": "1",
                 "name": f"Hoppr temp repository {idx}",
                 "priority": "1",
-                "proxy": _repo_proxy(repo.url),
+                "proxy": _repo_proxy(f"{repo.url}"),
                 "module_hotfixes": "true",
             }
 
             if creds is not None:
                 repo_config[temp_repo]["username"] = f"{creds.username}"
                 repo_config[temp_repo]["password"] = f"{creds.password.get_secret_value()}"
```

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 Collector plugin for helm charts
 """
 from __future__ import annotations
 
-import re
-
 from pathlib import Path
-from urllib.parse import urljoin
 
 from packageurl import PackageURL
 
 from hoppr import __version__, utils
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.exceptions import HopprLoadDataError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
 from hoppr.models.manifest import Component
+from hoppr.models.types import RepositoryUrl
 from hoppr.result import Result
 
 
 class CollectHelmPlugin(SerialCollectorPlugin):
     """
     Class to copy helm charts
     """
@@ -64,30 +62,27 @@
     def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         Collect helm chart
         """
 
         purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
 
-        if not re.match(pattern="^.*/$", string=repo_url):
-            repo_url = f"{repo_url}/"
-
         target_dir = self.directory_for(purl.type, repo_url, subdir=f"{purl.name}_{purl.version}")
 
         for subdir in ["", purl.name]:
-            source_url = urljoin(base=repo_url, url=subdir)
+            source_url = RepositoryUrl(url=repo_url) / subdir
 
             self.get_logger().info(msg="Fetching helm chart:", indent_level=2)
             self.get_logger().info(msg=f"source: {source_url}", indent_level=3)
             self.get_logger().info(msg=f"destination: {target_dir}", indent_level=3)
 
             command = [
                 *self.base_command,
                 "--repo",
-                source_url,
+                f"{source_url}",
                 "--destination",
                 f"{target_dir}",
                 purl.name,
                 "--version",
                 purl.version,
             ]
```

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_nexus_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 import json
 import re
 
 from pathlib import Path
 from time import sleep
 from typing import Any
-from urllib.parse import urljoin, urlparse
+from urllib.parse import urlparse
 
 import requests
 
 from packageurl import PackageURL  # type: ignore
 from requests.auth import HTTPBasicAuth
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
-from hoppr.models.types import PurlType
+from hoppr.models.types import PurlType, RepositoryUrl
 from hoppr.net import download_file
 from hoppr.result import Result
 
 
 class CollectNexusSearch(SerialCollectorPlugin):
     """
     Class to copy artifacts using the Nexus API
@@ -129,23 +129,22 @@
         return target_dir
 
     @staticmethod
     def is_nexus_instance(repo_url: str, auth: HTTPBasicAuth | None = None) -> bool:
         """
         Checks whether or not the repo_url refers to a Nexus instance
         """
-
-        test_url = urljoin(repo_url + "/", "service/rest/v1/status")
+        test_url = RepositoryUrl(url=repo_url) / "service" / "rest" / "v1" / "status"
 
         for attempt in range(3):
             if attempt > 0:
                 sleep(5)
 
             response = requests.get(
-                test_url,
+                f"{test_url}",
                 auth=auth,
                 allow_redirects=True,
                 stream=True,
                 verify=True,
                 timeout=60,
             )
 
@@ -158,16 +157,15 @@
 
     @staticmethod
     def get_download_urls(purl: PackageURL, repo_url: str, auth: HTTPBasicAuth | None = None) -> list[str]:
         """
         Retrieves all urls to be retrieved from Nexus for this component
         """
         nexus_url, nexus_repo = CollectNexusSearch._parse_nexus_url(repo_url)
-
-        search_url = urljoin(nexus_url + "/", "service/rest/v1/search/assets")
+        search_url = RepositoryUrl(url=nexus_url) / "service" / "rest" / "v1" / "search" / "assets"
 
         additional_search_params: list[dict] = [{}]
         nexus_format = purl.type
         match purl.type:
             case "deb":
                 nexus_format = "apt"
             case "gems":
@@ -195,15 +193,15 @@
 
         if nexus_repo is not None:
             base_params["repository"] = nexus_repo
 
         url_list = []
         for extra_search_parms in additional_search_params:
             response = requests.get(
-                search_url,
+                f"{search_url}",
                 auth=auth,
                 allow_redirects=True,
                 stream=True,
                 verify=True,
                 timeout=60,
                 params=base_params | extra_search_parms,
             )
@@ -215,15 +213,14 @@
                         url_list.append(item["downloadUrl"])
                         break
 
         return url_list
 
     @classmethod
     def get_attestation_products(cls, config: dict | None = None) -> list[str]:
-
         products = []
         if config is not None and "purl_types" in config:
             for purl_type in config["purl_types"]:
                 products.append(purl_type + "/*")
 
         else:
             for purl_type in PurlType:
```

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from __future__ import annotations
 
 import importlib.util
 import re
 import sys
 
 from subprocess import CalledProcessError
-from urllib.parse import ParseResult, urljoin, urlparse
 
 from packageurl import PackageURL
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
 from hoppr.models.manifest import Component
+from hoppr.models.types import RepositoryUrl
 from hoppr.result import Result
 
 
 class CollectPypiPlugin(SerialCollectorPlugin):
     """
     Collector plugin for pypi images
     """
@@ -73,39 +73,39 @@
         Copy a component to the local collection directory structure
         """
         if importlib.util.find_spec(name="pip") is None:
             return Result.fail(message="The pip package was not found. Please install and try again.")
 
         purl = PackageURL.from_string(comp.purl)
 
-        source_url = repo_url
-        if not re.match(pattern="^.*simple/?$", string=source_url):
-            source_url = urljoin(base=source_url, url="simple")
+        source_url = RepositoryUrl(url=repo_url)
+        if not re.match(pattern="^.*simple/?$", string=f"{source_url}"):
+            source_url /= "simple"
 
         password_list = []
 
         if creds is not None:
-            parsed_url = urlparse(url=source_url)._asdict()
-            parsed_url["netloc"] = f"{creds.username}:{creds.password.get_secret_value()}@{parsed_url['netloc']}"
-            source_url = ParseResult(**parsed_url).geturl()
-            password_list = [creds.password.get_secret_value()]
+            source_url.username = creds.username
+            source_url.password = creds.password.get_secret_value()
+            source_url.netloc = f"{source_url.username}:{source_url.password}@{source_url.netloc}"
+            password_list = [source_url.password]
 
         target_dir = self.directory_for(purl.type, repo_url, subdir=f"{purl.name}_{purl.version}")
 
         self.get_logger().info(msg=f"Target directory: {target_dir}", indent_level=2)
 
         command = [
             *self.base_command,
             "download",
             "--no-deps",
             "--no-cache",
             "--timeout",
             "60",
             "--index-url",
-            source_url,
+            f"{source_url}",
             "--dest",
             f"{target_dir}",
             f"{purl.name}=={purl.version}",
         ]
 
         base_error_msg = f"Failed to download {purl.name} version {purl.version}"
```

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Collector plugin for raw files
 """
 
 import shutil
 
 from pathlib import Path
 from typing import Any, List
-from urllib.parse import unquote, urljoin, urlparse
+from urllib.parse import unquote
 
 from packageurl import PackageURL
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models.credentials import CredentialRequiredService
+from hoppr.models.types import RepositoryUrl
 from hoppr.net import download_file
 from hoppr.result import Result
 
 
 class CollectRawPlugin(SerialCollectorPlugin):
     """
     Collector plugin for raw files
@@ -30,24 +31,21 @@
         return __version__
 
     @hoppr_rerunner
     def collect(self, comp: Any, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         Copy a component to the local collection directory structure
         """
-        if not repo_url.endswith("/"):
-            repo_url = f"{repo_url}/"
-
-        source_url = urlparse(repo_url)
+        source_url = RepositoryUrl(url=repo_url)
 
         purl = PackageURL.from_string(comp.purl)
 
         subdir = None
         if purl.namespace is not None:
-            source_url = urlparse(urljoin(repo_url, purl.namespace))
+            source_url /= f"{purl.namespace}"
             subdir = unquote(purl.namespace)
 
         target_dir = self.directory_for(purl.type, repo_url, subdir=subdir)
 
         file_name = unquote(purl.name)
 
         if source_url.scheme == "file":
@@ -64,21 +62,21 @@
                 return Result.fail(message=msg)
 
             shutil.copy(source_file, target_dir)
 
             self.set_collection_params(comp, repo_url, target_dir)
             return Result.success(return_obj=comp)
 
-        download_url = urljoin(source_url.geturl() + "/", file_name)
+        download_url = source_url / file_name
 
         self.get_logger().info(msg="Downloading file:", indent_level=2)
         self.get_logger().info(msg=f"source: {download_url}", indent_level=3)
         self.get_logger().info(msg=f"destination: {target_dir.joinpath(file_name)}", indent_level=3)
 
-        response = download_file(download_url, str(target_dir / file_name), creds)
+        response = download_file(f"{download_url}", str(target_dir / file_name), creds)
         result = Result.from_http_response(response)
 
         if result.is_fail():
             msg = f"Unable to download from {download_url}, skipping remaining attempts"
             self.get_logger().error(msg=msg, indent_level=2)
 
         if not result.is_success():
```

### Comparing `hoppr-1.8.1/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.2/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.2/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.2/hoppr/core_plugins/delta_sbom.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.2/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.2/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/in_toto.py` & `hoppr-1.8.2/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/main.py` & `hoppr-1.8.2/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/mem_logger.py` & `hoppr-1.8.2/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/models/__init__.py` & `hoppr-1.8.2/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/models/__main__.py` & `hoppr-1.8.2/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/models/base.py` & `hoppr-1.8.2/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/models/credentials.py` & `hoppr-1.8.2/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/models/manifest.py` & `hoppr-1.8.2/hoppr/models/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,46 @@
 import hoppr.net
 import hoppr.oci_artifacts
 import hoppr.utils
 
 from hoppr.constants import BomProps
 from hoppr.exceptions import HopprLoadDataError
 from hoppr.models.base import HopprBaseModel, HopprBaseSchemaModel
-from hoppr.models.types import PurlType
+from hoppr.models.types import PurlType, RepositoryUrl
 
 if TYPE_CHECKING:
     from pydantic.typing import DictStrAny
 
 
 class Repository(HopprBaseModel):
     """
     Repository data model
     """
 
-    url: HttpUrl | FileUrl | AnyUrl
+    url: RepositoryUrl
     description: NoneStr = None
 
+    @validator("url", pre=True)
+    @classmethod
+    def validate_url(cls, url: RepositoryUrl | str) -> RepositoryUrl:
+        """
+        Validate URL string
+        """
+        if isinstance(url, str):
+            # Normalize URL scheme (e.g. `file:` to `file://`)
+            if url.endswith(":"):
+                url = f"{url}//"
+
+            if "://" not in url:
+                url = f"http://{url}"
+
+            url = RepositoryUrl(url=url)
+
+        return url
+
 
 # Dynamic Repositories model with PurlType values as attribute names
 purl_type_repo_mapping = {str(purl_type): (list[Repository], Field([], unique_items=True)) for purl_type in PurlType}
 RepositoriesMetaclass: ModelMetaclass = create_model(  # type: ignore[call-overload]
     "RepositoriesMetaclass", __base__=HopprBaseModel, **purl_type_repo_mapping
 )
```

### Comparing `hoppr-1.8.1/hoppr/models/transfer.py` & `hoppr-1.8.2/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/net.py` & `hoppr-1.8.2/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/oci_artifacts.py` & `hoppr-1.8.2/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/plugin_utils.py` & `hoppr-1.8.2/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/processor.py` & `hoppr-1.8.2/hoppr/processor.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.2/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.2/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/result.py` & `hoppr-1.8.2/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/hoppr/utils.py` & `hoppr-1.8.2/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.1/pyproject.toml` & `hoppr-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.1"
+version = "1.8.2"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
 
@@ -17,14 +17,15 @@
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Information Technology",
   "Topic :: Communications :: File Sharing",
   "Topic :: Software Development :: Version Control",
   "Topic :: System :: Software Distribution"
+
 ]
 
 [[tool.poetry.packages]]
 include = "hoppr"
 
 [tool.poetry.scripts]
 hopctl = "hoppr.cli.hopctl:app"
```

### Comparing `hoppr-1.8.1/PKG-INFO` & `hoppr-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.1
+Version: 1.8.2
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

