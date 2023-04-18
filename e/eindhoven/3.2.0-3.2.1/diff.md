# Comparing `tmp/eindhoven-3.2.0.tar.gz` & `tmp/eindhoven-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eindhoven-3.2.0.tar", max compression
+gzip compressed data, was "eindhoven-3.2.1.tar", max compression
```

## Comparing `eindhoven-3.2.0.tar` & `eindhoven-3.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-02-28 01:29:32.841655 eindhoven-3.2.0/LICENSE
--rw-r--r--   0        0        0     8068 2023-02-28 01:29:32.841655 eindhoven-3.2.0/README.md
--rw-r--r--   0        0        0      464 2023-02-28 01:29:32.841655 eindhoven-3.2.0/eindhoven/__init__.py
--rw-r--r--   0        0        0     5826 2023-02-28 01:29:32.841655 eindhoven-3.2.0/eindhoven/eindhoven.py
--rw-r--r--   0        0        0      525 2023-02-28 01:29:32.841655 eindhoven-3.2.0/eindhoven/exceptions.py
--rw-r--r--   0        0        0     1212 2023-02-28 01:29:32.841655 eindhoven-3.2.0/eindhoven/models.py
--rw-r--r--   0        0        0        0 2023-02-28 01:29:32.841655 eindhoven-3.2.0/eindhoven/py.typed
--rw-r--r--   0        0        0     3846 2023-02-28 01:29:50.927033 eindhoven-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     9657 1970-01-01 00:00:00.000000 eindhoven-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-18 12:17:52.857619 eindhoven-3.2.1/LICENSE
+-rw-r--r--   0        0        0     8068 2023-04-18 12:17:52.857619 eindhoven-3.2.1/README.md
+-rw-r--r--   0        0        0      464 2023-04-18 12:17:52.861619 eindhoven-3.2.1/eindhoven/__init__.py
+-rw-r--r--   0        0        0     5871 2023-04-18 12:17:52.861619 eindhoven-3.2.1/eindhoven/eindhoven.py
+-rw-r--r--   0        0        0      525 2023-04-18 12:17:52.861619 eindhoven-3.2.1/eindhoven/exceptions.py
+-rw-r--r--   0        0        0     1226 2023-04-18 12:17:52.861619 eindhoven-3.2.1/eindhoven/models.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:17:52.861619 eindhoven-3.2.1/eindhoven/py.typed
+-rw-r--r--   0        0        0     3898 2023-04-18 12:18:07.821795 eindhoven-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9657 1970-01-01 00:00:00.000000 eindhoven-3.2.1/PKG-INFO
```

### Comparing `eindhoven-3.2.0/LICENSE` & `eindhoven-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eindhoven-3.2.0/README.md` & `eindhoven-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `eindhoven-3.2.0/eindhoven/eindhoven.py` & `eindhoven-3.2.1/eindhoven/eindhoven.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,21 +31,22 @@
     _close_session: bool = False
 
     @staticmethod
     async def define_type(parking_type: int) -> str:
         """Define the parking type.
 
         Args:
+        ----
             parking_type: The selected parking type number.
 
-        Returns
+        Returns:
         -------
             The parking type as string.
 
-        Raises
+        Raises:
         ------
             ODPEindhovenTypeError: If the parking type is not listed.
         """
         options = {
             1: "Parkeerplaats",
             2: "Parkeerplaats Vergunning",
             3: "Parkeerplaats Gehandicapten",
@@ -68,24 +69,25 @@
         *,
         method: str = METH_GET,
         params: dict[str, Any] | None = None,
     ) -> Any:
         """Handle a request to the Open Data Platform API of Eindhoven.
 
         Args:
+        ----
             uri: Request URI, without '/', for example, 'status'
             method: HTTP method to use, for example, 'GET'
             params: Extra options to improve or limit the response.
 
-        Returns
+        Returns:
         -------
             A Python dictionary (json) with the response from
             the Open Data Platform API of Eindhoven.
 
-        Raises
+        Raises:
         ------
             ODPEindhovenConnectionError: An error occurred while
                 communicating with the Open Data Platform API
             ODPEindhovenError: Received an unexpected response from
                 the Open Data Platform API.
         """
         version = metadata.version(__package__)
@@ -140,22 +142,23 @@
         self,
         limit: int = 10,
         parking_type: int = 1,
     ) -> list[ParkingSpot]:
         """Get all the parking locations.
 
         Args:
+        ----
             limit: Number of rows to return.
             parking_type: The selected parking type number.
 
-        Returns
+        Returns:
         -------
             A list of ParkingSpot objects.
 
-        Raises
+        Raises:
         ------
             ODPEindhovenResultsError: When no results are found.
         """
         results: list[ParkingSpot] = []
         locations = await self._request(
             "search/",
             params={
```

### Comparing `eindhoven-3.2.0/eindhoven/exceptions.py` & `eindhoven-3.2.1/eindhoven/exceptions.py`

 * *Files identical despite different names*

### Comparing `eindhoven-3.2.0/eindhoven/models.py` & `eindhoven-3.2.1/eindhoven/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,18 @@
     updated_at: datetime
 
     @classmethod
     def from_json(cls: type[ParkingSpot], data: dict[str, Any]) -> ParkingSpot:
         """Return a ParkingSpot object from a JSON dictionary.
 
         Args:
+        ----
             data: The JSON data from the API.
 
-        Returns
+        Returns:
         -------
             A ParkingSpot object.
         """
         attr = data["fields"]
         geo = data["geometry"]["coordinates"]
         return cls(
             spot_id=data["recordid"],
```

### Comparing `eindhoven-3.2.0/pyproject.toml` & `eindhoven-3.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eindhoven"
-version = "3.2.0"
+version = "3.2.1"
 description = "Asynchronous Python client providing Open Data information of Eindhoven"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-eindhoven"
 repository = "https://github.com/klaasnicolaas/python-eindhoven"
@@ -26,37 +26,37 @@
     { include = "eindhoven" }
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
-pytz = "^2022.7.1"
+pytz = ">=2022.7.1,<2024.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-eindhoven/issues"
 Changelog = "https://github.com/klaasnicolaas/python-eindhoven/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.247"
+ruff = ">=0.0.247,<0.0.262"
 aresponses = "^2.1.6"
-black = "^22.12"
+black = ">=22.12,<24.0"
 blacken-docs = "^1.13.0"
 codespell = "^2.2.2"
 coverage = {version = "^7.2", extras = ["toml"]}
 mypy = "^1.0"
 pre-commit = "^3.0.4"
 pre-commit-hooks = "^4.4.0"
 pylint = "^2.16.1"
 pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
 yamllint = "^1.29.0"
 covdefaults = "^2.2.2"
-types-pytz = "^2022.7.1.2"
+types-pytz = ">=2022.7.1.2,<2024.0.0.0"
 
 [tool.black]
 target-version = ['py39']
 
 [tool.coverage.paths]
 source = ["eindhoven"]
 
@@ -149,15 +149,15 @@
 ]
 
 [tool.ruff.flake8-pytest-style]
 mark-parentheses = false
 fixture-parentheses = false
 
 [tool.ruff.isort]
-known-first-party = ["gridnet"]
+known-first-party = ["eindhoven"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eindhoven-3.2.0/PKG-INFO` & `eindhoven-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eindhoven
-Version: 3.2.0
+Version: 3.2.1
 Summary: Asynchronous Python client providing Open Data information of Eindhoven
 Home-page: https://github.com/klaasnicolaas/python-eindhoven
 License: MIT
 Keywords: parking,eindhoven,locations,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
-Requires-Dist: pytz (>=2022.7.1,<2023.0.0)
+Requires-Dist: pytz (>=2022.7.1,<2024.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-eindhoven/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-eindhoven/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-eindhoven
 Project-URL: Repository, https://github.com/klaasnicolaas/python-eindhoven
 Description-Content-Type: text/markdown
```

