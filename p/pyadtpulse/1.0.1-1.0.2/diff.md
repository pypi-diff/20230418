# Comparing `tmp/pyadtpulse-1.0.1-py3-none-any.whl.zip` & `tmp/pyadtpulse-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20264 bytes, number of entries: 11
--rw-r--r--  2.0 unx    30711 b- defN 23-Apr-15 18:21 pyadtpulse/__init__.py
+Zip file size: 20545 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    31842 b- defN 23-Apr-18 03:32 pyadtpulse/__init__.py
 -rw-r--r--  2.0 unx     1609 b- defN 23-Mar-28 16:07 pyadtpulse/const.py
--rw-r--r--  2.0 unx    24098 b- defN 23-Apr-15 18:21 pyadtpulse/site.py
+-rw-r--r--  2.0 unx    24044 b- defN 23-Apr-18 03:32 pyadtpulse/site.py
 -rw-r--r--  2.0 unx     4803 b- defN 23-Mar-28 16:07 pyadtpulse/util.py
 -rw-r--r--  2.0 unx     5089 b- defN 23-Mar-28 16:07 pyadtpulse/zones.py
--rw-r--r--  2.0 unx      581 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3646 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Nov-23 16:58 pyadtpulse-1.0.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      875 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/RECORD
-11 files, 71516 bytes uncompressed, 18790 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx      581 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3646 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 03:34 pyadtpulse-1.0.2.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      875 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/RECORD
+11 files, 72593 bytes uncompressed, 19071 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pyadtpulse/util.py
 Comment: 
 
 Filename: pyadtpulse/zones.py
 Comment: 
 
-Filename: pyadtpulse-1.0.1.dist-info/LICENSE.md
+Filename: pyadtpulse-1.0.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyadtpulse-1.0.1.dist-info/METADATA
+Filename: pyadtpulse-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pyadtpulse-1.0.1.dist-info/WHEEL
+Filename: pyadtpulse-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyadtpulse-1.0.1.dist-info/top_level.txt
+Filename: pyadtpulse-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyadtpulse-1.0.1.dist-info/zip-safe
+Filename: pyadtpulse-1.0.2.dist-info/zip-safe
 Comment: 
 
-Filename: pyadtpulse-1.0.1.dist-info/RECORD
+Filename: pyadtpulse-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyadtpulse/__init__.py

```diff
@@ -1,15 +1,15 @@
 """Base Python Class for pyadtpulse."""
 
 import logging
 import asyncio
 import re
 import time
 from random import uniform
-from threading import RLock, Thread
+from threading import RLock, Thread, Lock
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import uvloop
 from aiohttp import (
     ClientConnectionError,
     ClientResponse,
     ClientResponseError,
@@ -54,15 +54,14 @@
 
 class PyADTPulse:
     """Base object for ADT Pulse service."""
 
     __slots__ = (
         "_session",
         "_user_agent",
-        "_api_version",
         "_sync_task",
         "_timeout_task",
         "_authenticated",
         "_updates_exist",
         "_loop",
         "_session_thread",
         "_attribute_lock",
@@ -73,14 +72,16 @@
         "_poll_interval",
         "_username",
         "_password",
         "_fingerprint",
         "_login_exception",
         "_gateway_online",
     )
+    _api_version = ADT_DEFAULT_VERSION
+    _class_threadlock = Lock()
 
     def __init__(
         self,
         username: str,
         password: str,
         fingerprint: str,
         service_host: str = DEFAULT_API_HOST,
@@ -107,15 +108,14 @@
                             Should be set to False for asynchronous usage
                             and async_login() should be called instead
                             Setting websession will override this
                             and not login
                         Defaults to True
             poll_interval (float, optional): number of seconds between update checks
         """
-        self._api_version: str = ADT_DEFAULT_VERSION
         self._gateway_online: bool = False
 
         self._session = websession
         if self._session is not None:
             self._session.headers.update(ADT_DEFAULT_HTTP_HEADERS)
 
         self._init_login_info(username, password, fingerprint)
@@ -168,33 +168,56 @@
             raise ValueError("Password is mandatory")
         self._password = password
 
         if fingerprint is None or fingerprint == "":
             raise ValueError("Fingerprint is required")
         self._fingerprint = fingerprint
 
+    def __del__(self) -> None:
+        """Destructor.
+
+        Closes aiohttp session if one exists
+        """
+        if self._session is not None and not self._session.closed:
+            self._session.detach()
+
     def __repr__(self) -> str:
         """Object representation."""
         return "<{}: {}>".format(self.__class__.__name__, self._username)
 
     # ADTPulse API endpoint is configurable (besides default US ADT Pulse endpoint) to
     # support testing as well as alternative ADT Pulse endpoints such as
     # portal-ca.adtpulse.com
-    def set_service_host(self, host: str) -> None:
+
+    @property
+    def service_host(self) -> str:
+        """Get the Pulse host.
+
+        Returns: (str): the ADT Pulse endpoint host
+        """
+        with self._attribute_lock:
+            return self._api_host
+
+    @service_host.setter
+    def service_host(self, host: str) -> None:
         """Override the Pulse host (i.e. to use portal-ca.adpulse.com).
 
         Args:
             host (str): name of Pulse endpoint host
         """
         with self._attribute_lock:
             self._api_host = f"https://{host}"
             if self._session is not None:
                 self._session.headers.update({"Host": host})
                 self._session.headers.update(ADT_DEFAULT_HTTP_HEADERS)
 
+    def set_service_host(self, host: str) -> None:
+        """Backward compatibility for service host property setter."""
+        self.service_host = host
+
     def make_url(self, uri: str) -> str:
         """Create a URL to service host from a URI.
 
         Args:
             uri (str): the URI to convert
 
         Returns:
@@ -236,16 +259,16 @@
     @property
     def version(self) -> str:
         """Get the ADT Pulse site version.
 
         Returns:
             str: a string containing the version
         """
-        with self._attribute_lock:
-            return self._api_version
+        with PyADTPulse._class_threadlock:
+            return PyADTPulse._api_version
 
     @property
     def gateway_online(self) -> bool:
         """Retrieve whether Pulse Gateway is online.
 
         Returns:
             bool: True if gateway is online
@@ -272,63 +295,66 @@
 
             LOG.warning(
                 f"ADT Pulse gateway {status_text}, poll interval={self._poll_interval}"
             )
             self._gateway_online = status
 
     async def _async_fetch_version(self) -> None:
-        with self._attribute_lock:
-            result = None
+        with PyADTPulse._class_threadlock:
+            if PyADTPulse._api_version != ADT_DEFAULT_VERSION:
+                return
+            response = None
+            signin_url = f"{self.service_host}/myhome{ADT_LOGIN_URI}"
             if self._session:
                 try:
-                    async with self._session.get(self._api_host) as response:
-                        result = await response.text()
+                    async with self._session.get(signin_url) as response:
+                        # we only need the headers here, don't parse response
                         response.raise_for_status()
                 except (ClientResponseError, ClientConnectionError):
                     LOG.warning(
                         "Error occurred during API version fetch, defaulting to"
                         f"{ADT_DEFAULT_VERSION}"
                     )
-                    self._api_version = ADT_DEFAULT_VERSION
+                    self._close_response(response)
                     return
 
-            if result is None:
+            if response is None:
                 LOG.warning(
                     "Error occurred during API version fetch, defaulting to"
                     f"{ADT_DEFAULT_VERSION}"
                 )
-                self._api_version = ADT_DEFAULT_VERSION
                 return
 
-            m = re.search("/myhome/(.+)/[a-z]*/", result)
+            m = re.search("/myhome/(.+)/[a-z]*/", response.real_url.path)
+            self._close_response(response)
             if m is not None:
-                self._api_version = m.group(1)
+                PyADTPulse._api_version = m.group(1)
                 LOG.debug(
                     "Discovered ADT Pulse version"
-                    f" {self._api_version} at {self._api_host}"
+                    f" {PyADTPulse._api_version} at {self.service_host}"
                 )
                 return
 
-            self._api_version = ADT_DEFAULT_VERSION
             LOG.warning(
                 "Couldn't auto-detect ADT Pulse version, "
-                f"defaulting to {self._api_version}"
+                f"defaulting to {ADT_DEFAULT_VERSION}"
             )
 
     async def _update_sites(self, soup: BeautifulSoup) -> None:
         with self._attribute_lock:
             if len(self._sites) == 0:
                 await self._initialize_sites(soup)
             else:
                 # FIXME: this will have to be fixed once multiple ADT sites
                 # are supported, since the summary_html only represents the
                 # alarm status of the current site!!
                 if len(self._sites) > 1:
                     LOG.error(
-                        "pyadtpulse lacks support for ADT accounts with multiple sites!!!"
+                        "pyadtpulse lacks support for ADT accounts "
+                        "with multiple sites!!!"
                     )
 
             for site in self._sites:
                 site._update_alarm_from_soup(soup)
                 site._update_zone_from_soup(soup)
 
     async def _initialize_sites(self, soup: BeautifulSoup) -> None:
@@ -420,15 +446,15 @@
         self._attribute_lock.release()
         if result:
             if self._sync_task is not None and self._timeout_task is not None:
                 try:
                     await asyncio.wait((self._sync_task, self._timeout_task))
                 except Exception as e:
                     LOG.exception(
-                        f"Received exception while waiting for ADT Pulse service"
+                        f"Received exception while waiting for ADT Pulse service {e}"
                     )
             else:
                 # we should never get here
                 raise RuntimeError("Background pyadtpulse tasks not created")
 
     def login(self) -> None:
         """Login to ADT Pulse and generate access token.
@@ -493,43 +519,53 @@
         await self._async_fetch_version()
 
         response = await self._async_query(
             ADT_LOGIN_URI,
             method="POST",
             extra_params={
                 "partner": "adt",
-                "usernameForm": self._username,
+                "usernameForm": self.username,
                 "passwordForm": self._password,
                 "fingerprint": self._fingerprint,
                 "sun": "yes",
             },
             force_login=False,
-            timeout=10,
+            timeout=30,
         )
 
         soup = await make_soup(
             response, logging.ERROR, "Could not log into ADT Pulse site"
         )
         if soup is None:
-            await self._session.close()
             return False
 
+        # FIXME: should probably raise exceptions
         error = soup.find("div", {"id": "warnMsgContents"})
         if error:
-            LOG.error(f"Invalid ADT Pulse response: {error}")
-            await self._session.close()
+            LOG.error(f"Invalid ADT Pulse username/password: {error}")
             return False
-
+        error = soup.find("div", "responsiveContainer")
+        if error:
+            LOG.error(
+                f"2FA authentiation required for ADT pulse username {self.username} "
+                f"{error}"
+            )
+            return False
+        # need to set authenticated here to prevent login loop
         self._authenticated.set()
+        await self._update_sites(soup)
+        if len(self._sites) == 0:
+            LOG.error("Could not retrieve any sites, login failed")
+            self._authenticated.clear()
+            return False
         self._last_timeout_reset = time.time()
 
         # since we received fresh data on the status of the alarm, go ahead
         # and update the sites with the alarm status.
 
-        await self._update_sites(soup)
         self._sync_timestamp = time.time()
         if self._sync_task is None:
             self._sync_task = asyncio.create_task(
                 self._sync_check_task(), name="PyADTPulse sync check"
             )
         if self._timeout_task is None:
             self._timeout_task = asyncio.create_task(
@@ -553,17 +589,14 @@
             try:
                 self._sync_task.cancel()
             except asyncio.CancelledError:
                 LOG.debug("Pulse sync check task successfully cancelled")
                 await self._sync_task
         self._timeout_task = self._sync_task = None
         await self._async_query(ADT_LOGOUT_URI, timeout=10)
-        if self._session is not None:
-            if not self._session.closed:
-                await self._session.close()
         self._last_timeout_reset = time.time()
         if self._authenticated is not None:
             self._authenticated.clear()
 
     def logout(self) -> None:
         """Log out of ADT Pulse."""
         with self._attribute_lock:
```

## pyadtpulse/site.py

```diff
@@ -613,15 +613,14 @@
 
                 # update device state from ORB info
                 if not self._zones:
                     LOG.warning("No zones exist")
                     return None
                 if state != "Unknown":
                     gateway_online = True
-                self._zones.update_state(zone, state)
                 self._zones.update_last_activity_timestamp(zone, last_update)
 
                 LOG.debug(f"Set zone {zone} - to {state} with timestamp {last_update}")
 
             self._adt_service._set_gateway_status(gateway_online)
             self._last_updated = datetime.now()
             return self._zones
```

## Comparing `pyadtpulse-1.0.1.dist-info/LICENSE.md` & `pyadtpulse-1.0.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyadtpulse-1.0.1.dist-info/METADATA` & `pyadtpulse-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyadtpulse
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python interface for ADT Pulse security systems
 Home-page: https://github.com/rsnodgrass/pyadtpulse
 Author: 
 Author-email: 
 License: Apache Software License
 Keywords: security system,adt,home automation,security alarm
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyadtpulse-1.0.1.dist-info/RECORD` & `pyadtpulse-1.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyadtpulse/__init__.py,sha256=4v7UmlYB5D99BTWus3kjP9aYqqO70AM9zGXHFRUVYYU,30711
+pyadtpulse/__init__.py,sha256=7jWHJ33ba3uIrwnXmfpggMYO5SMtH5SVcfd4MlhlukM,31842
 pyadtpulse/const.py,sha256=q3xJ93olyh9pNKvywARCwsu9qnr-E8O3SkD8Z4BEGBw,1609
-pyadtpulse/site.py,sha256=LJ6DIpZZTghO4cBbzNItpUipfY5tpjYWBO0IV_hVv8o,24098
+pyadtpulse/site.py,sha256=rXSy25p6n_uofeCwfZ0foCfALJ5Dct0TCu72pF1afpQ,24044
 pyadtpulse/util.py,sha256=aTsrbEWoYkaAxnN0pU_ZoQ6eqyWTx-4_Ukihq8wwb88,4803
 pyadtpulse/zones.py,sha256=ZLdySMMGxMSvKGHqe9cDvFgchXlXnuCc-FFNRQSLqhE,5089
-pyadtpulse-1.0.1.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
-pyadtpulse-1.0.1.dist-info/METADATA,sha256=WoeWuL63GcJsL9FoPNgmmTM0RJvL6NzYLgGB5fBFmvU,3646
-pyadtpulse-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyadtpulse-1.0.1.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
-pyadtpulse-1.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pyadtpulse-1.0.1.dist-info/RECORD,,
+pyadtpulse-1.0.2.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
+pyadtpulse-1.0.2.dist-info/METADATA,sha256=sjO12kMl0nnNhdyP78_UPvOMHp7CCvkvUU7UK2Pn4zg,3646
+pyadtpulse-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyadtpulse-1.0.2.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
+pyadtpulse-1.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyadtpulse-1.0.2.dist-info/RECORD,,
```

