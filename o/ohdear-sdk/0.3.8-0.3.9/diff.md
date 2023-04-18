# Comparing `tmp/ohdear_sdk-0.3.8.tar.gz` & `tmp/ohdear_sdk-0.3.9.tar.gz`

## Comparing `ohdear_sdk-0.3.8.tar` & `ohdear_sdk-0.3.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/.editorconfig
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/.gitattributes
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/ohdear/__init__.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/ohdear/ohdear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/ohdear/py.typed
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/ohdear/types.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/.gitignore
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/LICENSE.md
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/README.md
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/.editorconfig
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/.gitattributes
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/ohdear/__init__.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/ohdear/ohdear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/ohdear/py.typed
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/ohdear/types.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/LICENSE.md
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/README.md
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 ohdear_sdk-0.3.9/PKG-INFO
```

### Comparing `ohdear_sdk-0.3.8/CHANGELOG.md` & `ohdear_sdk-0.3.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com), and this project adheres to [Semantic Versioning](https://semver.org).
 
 ## Unreleased
 
+## [v0.3.9 - 2023-04-18](https://github.com/owenvoke/ohdear-python-sdk/compare/v0.3.8...v0.3.9)
+
+### Added
+- Add support for domain monitoring ([#4](https://github.com/owenvoke/ohdear-python-sdk/pull/4))
+
 ## [v0.3.8 - 2022-11-18](https://github.com/owenvoke/ohdear-python-sdk/compare/v0.3.7...v0.3.8)
 
 ### Added
 - Enforce types with `py.typed` file ([#3](https://github.com/owenvoke/ohdear-python-sdk/pull/3))
 
 ## [v0.3.7 - 2022-11-16](https://github.com/owenvoke/ohdear-python-sdk/compare/v0.3.6...v0.3.7)
```

### Comparing `ohdear_sdk-0.3.8/ohdear/ohdear.py` & `ohdear_sdk-0.3.9/ohdear/ohdear.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import requests
 
 from ohdear.types import (
     BrokenLinksCollection,
     CertificateHealth,
     CronChecksCollection,
+    Domain,
     MixedContentsCollection,
     Site,
     SitesCollection,
     UserInfo,
 )
 
 TIMEOUT = 3
@@ -34,14 +35,15 @@
         self.base_uri: str = base_uri
         self.headers: dict = {"Authorization": "Bearer {0}".format(self.api_token)}
 
         self.broken_links: BrokenLinks = BrokenLinks(self)
         self.certificates: Certificates = Certificates(self)
         self.checks: Checks = Checks(self)
         self.cron_checks: CronChecks = CronChecks(self)
+        self.domain_monitoring: DomainMonitoring = DomainMonitoring(self)
         self.mixed_contents: MixedContents = MixedContents(self)
         self.sites: Sites = Sites(self)
 
     def authenticated(self) -> bool:
         try:
             return self.me().get("id") is not None
         except UnauthorizedException:
@@ -117,14 +119,22 @@
 
     def show(self, site_id: int) -> CronChecksCollection:
         return cast(
             CronChecksCollection, self.client.get(f"/sites/{site_id}/cron-checks")
         )
 
 
+class DomainMonitoring:
+    def __init__(self, client: OhDear):
+        self.client = client
+
+    def domain(self, site_id: int) -> Domain:
+        return cast(Domain, self.client.get(f"/sites/{site_id}/domain"))
+
+
 class MixedContents:
     def __init__(self, client: OhDear):
         self.client = client
 
     def show(self, site_id: int) -> MixedContentsCollection:
         return cast(
             MixedContentsCollection, self.client.get(f"/mixed-content/{site_id}")
```

### Comparing `ohdear_sdk-0.3.8/ohdear/types.py` & `ohdear_sdk-0.3.9/ohdear/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -90,14 +90,24 @@
 
 class CertificateHealth(TypedDict):
     certificate_details: CertificateDetails
     certificate_checks: list[CertificateCheck]
     certificate_chain_issuers: list[str]
 
 
+class Domain(TypedDict):
+    expires_at: datetime
+    registered_at: datetime
+    last_changed_at: datetime
+    last_updated_in_rdap_db_at: datetime
+    domain_statuses: dict[str, bool]
+    rdap_domain_response: dict
+    created_at: datetime
+
+
 class MixedContent(TypedDict):
     element_name: str
     mixed_content_url: str
     found_on_url: str
 
 
 class MixedContentsCollection(TypedDict):
```

### Comparing `ohdear_sdk-0.3.8/LICENSE.md` & `ohdear_sdk-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ohdear_sdk-0.3.8/README.md` & `ohdear_sdk-0.3.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 from ohdear import OhDear
 
 ohdear = OhDear(api_token="your-token")
 
 sites = ohdear.sites.all()
 ```
 
-| Available Methods                 | Description                                                                                         |
-|:----------------------------------|:----------------------------------------------------------------------------------------------------|
-| `ohdear.me()`                     | Retrieve a `UserInfo` dict with details about the currently authenticated user.                     |
-| `ohdear.authenticated()`          | Retrieve a `boolean` response indicating whether the current user is authenticated.                 |
-| `ohdear.broken_links.show(123)`   | Retrieve a `BrokenLinksCollection` dict with details about broken links for a specific site.        |
-| `ohdear.certificates.enable(123)` | Retrieve a `CertificateHealth` dict containing details about the certificate and it's health.       |
-| `ohdear.checks.enable(123)`       | Retrieve a `boolean` indicating whether a check was enabled successfully.                           |
-| `ohdear.checks.disable(123)`      | Retrieve a `boolean` indicating whether a check was disabled successfully.                          |
-| `ohdear.cron_checks.show(123)`    | Retrieve a `CronChecksCollection` dict with details about the cron checks for a specific site.      |
-| `ohdear.mixed_contents.show(123)` | Retrieve a `MixedContentsCollection` dict with details about the mixed content for a specific site. |
-| `ohdear.sites.all()`              | Retrieve a `SitesCollection` dict with details about all sites.                                     |
-| `ohdear.sites.show(123)`          | Retrieve a `Site` dict with details about a specific site.                                          |
+| Available Methods                      | Description                                                                                         |
+|:---------------------------------------|:----------------------------------------------------------------------------------------------------|
+| `ohdear.me()`                          | Retrieve a `UserInfo` dict with details about the currently authenticated user.                     |
+| `ohdear.authenticated()`               | Retrieve a `boolean` response indicating whether the current user is authenticated.                 |
+| `ohdear.broken_links.show(123)`        | Retrieve a `BrokenLinksCollection` dict with details about broken links for a specific site.        |
+| `ohdear.certificates.enable(123)`      | Retrieve a `CertificateHealth` dict containing details about the certificate and it's health.       |
+| `ohdear.checks.enable(123)`            | Retrieve a `boolean` indicating whether a check was enabled successfully.                           |
+| `ohdear.checks.disable(123)`           | Retrieve a `boolean` indicating whether a check was disabled successfully.                          |
+| `ohdear.cron_checks.show(123)`         | Retrieve a `CronChecksCollection` dict with details about the cron checks for a specific site.      |
+| `ohdear.domain_monitoring.domain(123)` | Retrieve a `Domain` dict with details about the domain for a specific site.                         |
+| `ohdear.mixed_contents.show(123)`      | Retrieve a `MixedContentsCollection` dict with details about the mixed content for a specific site. |
+| `ohdear.sites.all()`                   | Retrieve a `SitesCollection` dict with details about all sites.                                     |
+| `ohdear.sites.show(123)`               | Retrieve a `Site` dict with details about a specific site.                                          |
 
 ## Change log
 
 Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.
 
 ## Testing
 
@@ -71,15 +72,15 @@
 
 You can buy trees [here][link-treeware-gifting].
 
 Read more about Treeware at [treeware.earth][link-treeware].
 
 [ico-version]: https://img.shields.io/pypi/v/ohdear-sdk.svg?style=flat-square
 [ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
-[ico-github-actions]: https://img.shields.io/github/workflow/status/owenvoke/ohdear-python-sdk/Tests.svg?style=flat-square
+[ico-github-actions]: https://img.shields.io/github/actions/workflow/status/owenvoke/ohdear-python-sdk/tests.yml?branch=main&style=flat-square
 [ico-treeware-gifting]: https://img.shields.io/badge/Treeware-%F0%9F%8C%B3-lightgreen?style=flat-square
 
 [link-pypi]: https://pypi.org/project/ohdear-sdk
 [link-github-actions]: https://github.com/owenvoke/ohdear-python-sdk/actions
 [link-treeware]: https://treeware.earth
 [link-treeware-gifting]: https://ecologi.com/owenvoke?gift-trees
 [link-author]: https://github.com/owenvoke
```

### Comparing `ohdear_sdk-0.3.8/pyproject.toml` & `ohdear_sdk-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ohdear_sdk-0.3.8/PKG-INFO` & `ohdear_sdk-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: ohdear-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: Oh Dear Python SDK
 Project-URL: Source Code, https://github.com/owenvoke/ohdear-python-sdk
 Project-URL: Issues, https://github.com/owenvoke/ohdear-python-sdk/issues
 Author-email: Owen Voke <development@voke.dev>
+License-Expression: MIT
 License-File: LICENSE.md
 Keywords: ohdear,sdk
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Requires-Dist: requests>=2.28.1
@@ -37,26 +38,27 @@
 from ohdear import OhDear
 
 ohdear = OhDear(api_token="your-token")
 
 sites = ohdear.sites.all()
 ```
 
-| Available Methods                 | Description                                                                                         |
-|:----------------------------------|:----------------------------------------------------------------------------------------------------|
-| `ohdear.me()`                     | Retrieve a `UserInfo` dict with details about the currently authenticated user.                     |
-| `ohdear.authenticated()`          | Retrieve a `boolean` response indicating whether the current user is authenticated.                 |
-| `ohdear.broken_links.show(123)`   | Retrieve a `BrokenLinksCollection` dict with details about broken links for a specific site.        |
-| `ohdear.certificates.enable(123)` | Retrieve a `CertificateHealth` dict containing details about the certificate and it's health.       |
-| `ohdear.checks.enable(123)`       | Retrieve a `boolean` indicating whether a check was enabled successfully.                           |
-| `ohdear.checks.disable(123)`      | Retrieve a `boolean` indicating whether a check was disabled successfully.                          |
-| `ohdear.cron_checks.show(123)`    | Retrieve a `CronChecksCollection` dict with details about the cron checks for a specific site.      |
-| `ohdear.mixed_contents.show(123)` | Retrieve a `MixedContentsCollection` dict with details about the mixed content for a specific site. |
-| `ohdear.sites.all()`              | Retrieve a `SitesCollection` dict with details about all sites.                                     |
-| `ohdear.sites.show(123)`          | Retrieve a `Site` dict with details about a specific site.                                          |
+| Available Methods                      | Description                                                                                         |
+|:---------------------------------------|:----------------------------------------------------------------------------------------------------|
+| `ohdear.me()`                          | Retrieve a `UserInfo` dict with details about the currently authenticated user.                     |
+| `ohdear.authenticated()`               | Retrieve a `boolean` response indicating whether the current user is authenticated.                 |
+| `ohdear.broken_links.show(123)`        | Retrieve a `BrokenLinksCollection` dict with details about broken links for a specific site.        |
+| `ohdear.certificates.enable(123)`      | Retrieve a `CertificateHealth` dict containing details about the certificate and it's health.       |
+| `ohdear.checks.enable(123)`            | Retrieve a `boolean` indicating whether a check was enabled successfully.                           |
+| `ohdear.checks.disable(123)`           | Retrieve a `boolean` indicating whether a check was disabled successfully.                          |
+| `ohdear.cron_checks.show(123)`         | Retrieve a `CronChecksCollection` dict with details about the cron checks for a specific site.      |
+| `ohdear.domain_monitoring.domain(123)` | Retrieve a `Domain` dict with details about the domain for a specific site.                         |
+| `ohdear.mixed_contents.show(123)`      | Retrieve a `MixedContentsCollection` dict with details about the mixed content for a specific site. |
+| `ohdear.sites.all()`                   | Retrieve a `SitesCollection` dict with details about all sites.                                     |
+| `ohdear.sites.show(123)`               | Retrieve a `Site` dict with details about a specific site.                                          |
 
 ## Change log
 
 Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.
 
 ## Testing
 
@@ -87,15 +89,15 @@
 
 You can buy trees [here][link-treeware-gifting].
 
 Read more about Treeware at [treeware.earth][link-treeware].
 
 [ico-version]: https://img.shields.io/pypi/v/ohdear-sdk.svg?style=flat-square
 [ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
-[ico-github-actions]: https://img.shields.io/github/workflow/status/owenvoke/ohdear-python-sdk/Tests.svg?style=flat-square
+[ico-github-actions]: https://img.shields.io/github/actions/workflow/status/owenvoke/ohdear-python-sdk/tests.yml?branch=main&style=flat-square
 [ico-treeware-gifting]: https://img.shields.io/badge/Treeware-%F0%9F%8C%B3-lightgreen?style=flat-square
 
 [link-pypi]: https://pypi.org/project/ohdear-sdk
 [link-github-actions]: https://github.com/owenvoke/ohdear-python-sdk/actions
 [link-treeware]: https://treeware.earth
 [link-treeware-gifting]: https://ecologi.com/owenvoke?gift-trees
 [link-author]: https://github.com/owenvoke
```

