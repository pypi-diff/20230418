# Comparing `tmp/renault-api-0.1.8.tar.gz` & `tmp/renault-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renault-api-0.1.8.tar", max compression
+gzip compressed data, was "renault-api-0.1.9.tar", max compression
```

## Comparing `renault-api-0.1.8.tar` & `renault-api-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1078 2022-02-04 13:54:46.924234 renault-api-0.1.8/LICENSE.rst
--rw-r--r--   0        0        0     5199 2022-02-04 13:54:46.924234 renault-api-0.1.8/README.rst
--rw-r--r--   0        0        0     2724 2022-02-04 13:54:59.300383 renault-api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       19 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/__init__.py
--rw-r--r--   0        0        0       19 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/__init__.py
--rw-r--r--   0        0        0     7178 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/__main__.py
--rw-r--r--   0        0        0       19 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/charge/__init__.py
--rw-r--r--   0        0        0      404 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/charge/commands.py
--rw-r--r--   0        0        0     1660 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/charge/control.py
--rw-r--r--   0        0        0     3485 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/charge/history.py
--rw-r--r--   0        0        0     6996 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/charge/schedule.py
--rw-r--r--   0        0        0     6346 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/helpers.py
--rw-r--r--   0        0        0       19 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/hvac/__init__.py
--rw-r--r--   0        0        0      300 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/hvac/commands.py
--rw-r--r--   0        0        0     1484 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/hvac/control.py
--rw-r--r--   0        0        0     1432 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/hvac/history.py
--rw-r--r--   0        0        0     4202 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/renault_account.py
--rw-r--r--   0        0        0     5635 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/renault_client.py
--rw-r--r--   0        0        0     1821 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/renault_settings.py
--rw-r--r--   0        0        0    12389 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/cli/renault_vehicle.py
--rw-r--r--   0        0        0     8205 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/const.py
--rw-r--r--   0        0        0      760 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/credential.py
--rw-r--r--   0        0        0     4189 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/credential_store.py
--rw-r--r--   0        0        0      289 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/exceptions.py
--rw-r--r--   0        0        0     3102 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/gigya/__init__.py
--rw-r--r--   0        0        0      603 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/gigya/exceptions.py
--rw-r--r--   0        0        0     2829 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/gigya/models.py
--rw-r--r--   0        0        0      616 2022-02-04 13:54:46.924234 renault-api-0.1.8/src/renault_api/gigya/schemas.py
--rw-r--r--   0        0        0     4290 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/helpers.py
--rw-r--r--   0        0        0    10644 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/kamereon/__init__.py
--rw-r--r--   0        0        0      584 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/kamereon/enums.py
--rw-r--r--   0        0        0     1336 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/kamereon/exceptions.py
--rw-r--r--   0        0        0     1785 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/kamereon/helpers.py
--rw-r--r--   0        0        0    20054 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/kamereon/models.py
--rw-r--r--   0        0        0     3947 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/kamereon/schemas.py
--rw-r--r--   0        0        0      672 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/models.py
--rw-r--r--   0        0        0        0 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/py.typed
--rw-r--r--   0        0        0     2807 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/renault_account.py
--rw-r--r--   0        0        0     2410 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/renault_client.py
--rw-r--r--   0        0        0    10287 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/renault_session.py
--rw-r--r--   0        0        0    21363 2022-02-04 13:54:46.928235 renault-api-0.1.8/src/renault_api/renault_vehicle.py
--rw-r--r--   0        0        0     6515 2022-02-04 13:55:01.411492 renault-api-0.1.8/setup.py
--rw-r--r--   0        0        0     6245 2022-02-04 13:55:01.411992 renault-api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-02-22 06:27:35.716303 renault-api-0.1.9/LICENSE.rst
+-rw-r--r--   0        0        0     5199 2022-02-22 06:27:35.716303 renault-api-0.1.9/README.rst
+-rw-r--r--   0        0        0     2724 2022-02-22 06:27:45.332505 renault-api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       19 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/__init__.py
+-rw-r--r--   0        0        0       19 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/__init__.py
+-rw-r--r--   0        0        0     7178 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/__main__.py
+-rw-r--r--   0        0        0       19 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/charge/__init__.py
+-rw-r--r--   0        0        0      404 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/charge/commands.py
+-rw-r--r--   0        0        0     1660 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/charge/control.py
+-rw-r--r--   0        0        0     3485 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/charge/history.py
+-rw-r--r--   0        0        0     6996 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/charge/schedule.py
+-rw-r--r--   0        0        0     6346 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/helpers.py
+-rw-r--r--   0        0        0       19 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/hvac/__init__.py
+-rw-r--r--   0        0        0      300 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/hvac/commands.py
+-rw-r--r--   0        0        0     1484 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/hvac/control.py
+-rw-r--r--   0        0        0     1432 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/hvac/history.py
+-rw-r--r--   0        0        0     4202 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/renault_account.py
+-rw-r--r--   0        0        0     5635 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/renault_client.py
+-rw-r--r--   0        0        0     1821 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/renault_settings.py
+-rw-r--r--   0        0        0    13193 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/cli/renault_vehicle.py
+-rw-r--r--   0        0        0     8205 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/const.py
+-rw-r--r--   0        0        0      760 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/credential.py
+-rw-r--r--   0        0        0     4189 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/credential_store.py
+-rw-r--r--   0        0        0      289 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/exceptions.py
+-rw-r--r--   0        0        0     3102 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/gigya/__init__.py
+-rw-r--r--   0        0        0      603 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/gigya/exceptions.py
+-rw-r--r--   0        0        0     2829 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/gigya/models.py
+-rw-r--r--   0        0        0      616 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/gigya/schemas.py
+-rw-r--r--   0        0        0     4290 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/helpers.py
+-rw-r--r--   0        0        0    10669 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/kamereon/__init__.py
+-rw-r--r--   0        0        0      584 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/kamereon/enums.py
+-rw-r--r--   0        0        0     1336 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/kamereon/exceptions.py
+-rw-r--r--   0        0        0     1785 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/kamereon/helpers.py
+-rw-r--r--   0        0        0    20237 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/kamereon/models.py
+-rw-r--r--   0        0        0     4087 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/kamereon/schemas.py
+-rw-r--r--   0        0        0      672 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/models.py
+-rw-r--r--   0        0        0        0 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/py.typed
+-rw-r--r--   0        0        0     2807 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/renault_account.py
+-rw-r--r--   0        0        0     2410 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/renault_client.py
+-rw-r--r--   0        0        0    10287 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/renault_session.py
+-rw-r--r--   0        0        0    21852 2022-02-22 06:27:35.720303 renault-api-0.1.9/src/renault_api/renault_vehicle.py
+-rw-r--r--   0        0        0     6515 2022-02-22 06:27:47.397943 renault-api-0.1.9/setup.py
+-rw-r--r--   0        0        0     6245 2022-02-22 06:27:47.398406 renault-api-0.1.9/PKG-INFO
```

### Comparing `renault-api-0.1.8/LICENSE.rst` & `renault-api-0.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/README.rst` & `renault-api-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/pyproject.toml` & `renault-api-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "renault-api"
-version = "0.1.8"
+version = "0.1.9"
 description = "Renault API"
 authors = ["epenet"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/hacf-fr/renault-api"
 repository = "https://github.com/hacf-fr/renault-api"
 documentation = "https://renault-api.readthedocs.io"
@@ -25,15 +25,15 @@
 pyjwt = ">=1.7.1,<3.0.0"
 marshmallow-dataclass = "^8.2.0"
 click = { version = "^8.0.1", optional = true }
 tabulate = { version = "^0.8.7", optional = true }
 dateparser = {version = "^1.0.0", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
+pytest = "^7.0.1"
 coverage = {extras = ["toml"], version = "^6.3"}
 safety = "^1.10.3"
 mypy = "^0.931"
 typeguard = "^2.13.3"
 xdoctest = {extras = ["colors"], version = "^0.15.10"}
 sphinx = "^4.3.2"
 sphinx-autobuild = "^2021.3.14"
@@ -45,17 +45,17 @@
 flake8-docstrings = "^1.6.0"
 flake8-rst-docstrings = "^0.2.5"
 pep8-naming = "^0.12.1"
 darglint = "^1.8.1"
 reorder-python-imports = "^2.7.1"
 pre-commit-hooks = "^4.1.0"
 sphinx-rtd-theme = "^1.0.0"
-sphinx-click = "^3.0.3"
+sphinx-click = "^3.1.0"
 Pygments = "^2.11.2"
-pytest-asyncio = "^0.17.2"
+pytest-asyncio = "^0.18.1"
 aioresponses = "^0.7.3"
 pytest-cov = "^3.0.0"
 #ensure urllib3 is greater than 1.26.5 to account for CVE-2021-33503
 urllib3 = "^1.26.8"
 
 [tool.poetry.extras]
 cli = ["click", "tabulate", "dateparser"]
```

### Comparing `renault-api-0.1.8/src/renault_api/cli/__main__.py` & `renault-api-0.1.9/src/renault_api/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/charge/control.py` & `renault-api-0.1.9/src/renault_api/cli/charge/control.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/charge/history.py` & `renault-api-0.1.9/src/renault_api/cli/charge/history.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/charge/schedule.py` & `renault-api-0.1.9/src/renault_api/cli/charge/schedule.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/helpers.py` & `renault-api-0.1.9/src/renault_api/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/hvac/control.py` & `renault-api-0.1.9/src/renault_api/cli/hvac/control.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/hvac/history.py` & `renault-api-0.1.9/src/renault_api/cli/hvac/history.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/renault_account.py` & `renault-api-0.1.9/src/renault_api/cli/renault_account.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/renault_client.py` & `renault-api-0.1.9/src/renault_api/cli/renault_client.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/renault_settings.py` & `renault-api-0.1.9/src/renault_api/cli/renault_settings.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/cli/renault_vehicle.py` & `renault-api-0.1.9/src/renault_api/cli/renault_vehicle.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     status_table: Dict[str, Any] = {}
 
     await update_battery_status(vehicle, status_table)
     await update_charge_mode(vehicle, status_table)
     await update_cockpit(vehicle, status_table)
     await update_location(vehicle, status_table)
     await update_lock_status(vehicle, status_table)
+    await update_res_state(vehicle, status_table)
     await update_hvac_status(vehicle, status_table)
 
     click.echo(tabulate(status_table.items()))
 
 
 def update_status_table(
     status_table: Dict[str, Any],
@@ -311,14 +312,35 @@
             ("Lock last updated", response.lastUpdateTime, "tzdatetime"),
         ]
 
         for key, value, unit in items:
             update_status_table(status_table, key, value, unit)
 
 
+async def update_res_state(
+    vehicle: RenaultVehicle, status_table: Dict[str, Any]
+) -> None:
+    """Update status table from get_vehicle_res_state."""
+    try:
+        if not await vehicle.supports_endpoint("res-state"):  # pragma: no cover
+            return
+        response = await vehicle.get_res_state()
+    except QuotaLimitException as exc:  # pragma: no cover
+        raise click.ClickException(repr(exc)) from exc
+    except KamereonResponseException as exc:  # pragma: no cover
+        click.echo(f"res state: {exc.error_details}", err=True)
+    else:
+        items = [
+            ("Engine state", response.details, None),
+        ]
+
+        for key, value, unit in items:
+            update_status_table(status_table, key, value, unit)
+
+
 async def update_hvac_status(
     vehicle: RenaultVehicle, status_table: Dict[str, str]
 ) -> None:
     """Update status table from get_vehicle_hvac_status."""
     try:
         if not await vehicle.supports_endpoint("hvac-status"):
             return
```

### Comparing `renault-api-0.1.8/src/renault_api/const.py` & `renault-api-0.1.9/src/renault_api/const.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/credential.py` & `renault-api-0.1.9/src/renault_api/credential.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/credential_store.py` & `renault-api-0.1.9/src/renault_api/credential_store.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/gigya/__init__.py` & `renault-api-0.1.9/src/renault_api/gigya/__init__.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/gigya/exceptions.py` & `renault-api-0.1.9/src/renault_api/gigya/exceptions.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/gigya/models.py` & `renault-api-0.1.9/src/renault_api/gigya/models.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/gigya/schemas.py` & `renault-api-0.1.9/src/renault_api/gigya/schemas.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/helpers.py` & `renault-api-0.1.9/src/renault_api/helpers.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/kamereon/__init__.py` & `renault-api-0.1.9/src/renault_api/kamereon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "hvac-history": {"version": 1},
     "hvac-sessions": {"version": 1},
     "hvac-status": {"version": 1},
     "hvac-settings": {"version": 1},
     "location": {"version": 1},
     "lock-status": {"version": 1},
     "notification-settings": {"version": 1},
+    "res-state": {"version": 1},
 }
 _KCA_POST_ENDPOINTS: Dict[str, Any] = {
     "actions/charge-mode": {"version": 1, "type": "ChargeMode"},
     "actions/charge-schedule": {"version": 2, "type": "ChargeSchedule"},
     "actions/charging-start": {"version": 1, "type": "ChargingStart"},
     "actions/hvac-schedule": {"version": 2, "type": "HvacSchedule"},
     "actions/hvac-start": {"version": 1, "type": "HvacStart"},
@@ -139,16 +140,16 @@
             method,
             http_response.url,
             response_text,
         )
 
         # Some endpoints return arrays instead of objects.
         # These need to be wrapped in an object.
-        if response_text.startswith("[") and wrap_array_in:
-            response_text = f'{{"{wrap_array_in}": {response_text}}}'
+        if response_text.startswith("["):
+            response_text = f'{{"{wrap_array_in or "data"}": {response_text}}}'
         kamereon_response: models.KamereonResponse = schema.loads(response_text)
         # Check for Kamereon error
         kamereon_response.raise_for_error_code()
         # Check for HTTP error
         http_response.raise_for_status()
 
         return kamereon_response
```

### Comparing `renault-api-0.1.8/src/renault_api/kamereon/enums.py` & `renault-api-0.1.9/src/renault_api/kamereon/enums.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/kamereon/exceptions.py` & `renault-api-0.1.9/src/renault_api/kamereon/exceptions.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/kamereon/helpers.py` & `renault-api-0.1.9/src/renault_api/kamereon/helpers.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/kamereon/models.py` & `renault-api-0.1.9/src/renault_api/kamereon/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,14 +400,22 @@
     doorStatusDriver: Optional[str]
     doorStatusPassenger: Optional[str]
     hatchStatus: Optional[str]
     lastUpdateTime: Optional[str]
 
 
 @dataclass
+class KamereonVehicleResStateData(KamereonVehicleDataAttributes):
+    """Kamereon vehicle data res-set attributes."""
+
+    details: Optional[str]
+    code: Optional[str]
+
+
+@dataclass
 class KamereonVehicleCarAdapterData(KamereonVehicleDataAttributes):
     """Kamereon vehicle data hvac-status attributes."""
 
     vin: Optional[str]
     vehicleId: Optional[int]
     batteryCode: Optional[str]
     brand: Optional[str]
```

### Comparing `renault-api-0.1.8/src/renault_api/kamereon/schemas.py` & `renault-api-0.1.9/src/renault_api/kamereon/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     models.KamereonVehicleLocationData, base_schema=BaseSchema
 )()
 
 KamereonVehicleLockStatusDataSchema = marshmallow_dataclass.class_schema(
     models.KamereonVehicleLockStatusData, base_schema=BaseSchema
 )()
 
+KamereonVehicleResStateDataSchema = marshmallow_dataclass.class_schema(
+    models.KamereonVehicleResStateData, base_schema=BaseSchema
+)()
+
 KamereonVehicleHvacStatusDataSchema = marshmallow_dataclass.class_schema(
     models.KamereonVehicleHvacStatusData, base_schema=BaseSchema
 )()
 
 
 KamereonVehicleChargeModeDataSchema = marshmallow_dataclass.class_schema(
     models.KamereonVehicleChargeModeData, base_schema=BaseSchema
```

### Comparing `renault-api-0.1.8/src/renault_api/models.py` & `renault-api-0.1.9/src/renault_api/models.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/renault_account.py` & `renault-api-0.1.9/src/renault_api/renault_account.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/renault_client.py` & `renault-api-0.1.9/src/renault_api/renault_client.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/renault_session.py` & `renault-api-0.1.9/src/renault_api/renault_session.py`

 * *Files identical despite different names*

### Comparing `renault-api-0.1.8/src/renault_api/renault_vehicle.py` & `renault-api-0.1.9/src/renault_api/renault_vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,27 @@
             endpoint="lock-status",
         )
         return cast(
             models.KamereonVehicleLockStatusData,
             response.get_attributes(schemas.KamereonVehicleLockStatusDataSchema),
         )
 
+    async def get_res_state(self) -> models.KamereonVehicleResStateData:
+        """Get vehicle res state."""
+        # await self.warn_on_method("get_res_state")
+        response = await self.session.get_vehicle_data(
+            account_id=self.account_id,
+            vin=self.vin,
+            endpoint="res-state",
+        )
+        return cast(
+            models.KamereonVehicleResStateData,
+            response.get_attributes(schemas.KamereonVehicleResStateDataSchema),
+        )
+
     async def get_charging_settings(self) -> models.KamereonVehicleChargingSettingsData:
         """Get vehicle charging settings."""
         # await self.warn_on_method("get_charging_settings")
         response = await self.session.get_vehicle_data(
             account_id=self.account_id,
             vin=self.vin,
             endpoint="charging-settings",
```

### Comparing `renault-api-0.1.8/setup.py` & `renault-api-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
          'dateparser>=1.0.0,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['renault-api = renault_api.cli.__main__:main']}
 
 setup_kwargs = {
     'name': 'renault-api',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Renault API',
     'long_description': 'Renault API\n===========\n\n|PyPI| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/renault-api.svg\n   :target: https://pypi.org/project/renault-api/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/renault-api\n   :target: https://pypi.org/project/renault-api\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/renault-api\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/renault-api/latest.svg?label=Read%20the%20Docs\n   :target: https://renault-api.readthedocs.io/\n   :alt: Read the documentation at https://renault-api.readthedocs.io/\n.. |Tests| image:: https://github.com/hacf-fr/renault-api/workflows/Tests/badge.svg\n   :target: https://github.com/hacf-fr/renault-api/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/hacf-fr/renault-api/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/hacf-fr/renault-api\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n\nFeatures\n--------\n\nThis Python package manages the communication with the private Renault API used by the official MyRenault application.\n\nThe client is able to read various vehicle attributes, such as:\n\n* mileage\n* GPS location\n* fuel autonomy (for fuel vehicles)\n* battery autonomy (for electric vehicles)\n* contracts associated to the vehicle (warranty and connected services)\n\nFor some vehicles, it is also possible to manage:\n\n* hvac/pre-conditionning of the vehicle\n* charge schedule\n\nThis package has been developed to be used with Home-Assistant, but it can be used in other contexts\n\n\nRequirements\n------------\n\n* Python (>= 3.7.1)\n\nAPI Usage\n---------\n\nYou can install *Renault API* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install renault-api\n\n.. code:: python\n\n   import aiohttp\n   import asyncio\n\n   from renault_api.renault_client import RenaultClient\n\n   async def main():\n      async with aiohttp.ClientSession() as websession:\n         client = RenaultClient(websession=websession, locale="fr_FR")\n         await client.session.login(\'email\', \'password\')\n         print(f"Accounts: {await client.get_person()}") # List available accounts, make a note of kamereon account id\n\n         account_id = "Your Kamereon account id"\n         account = await client.get_api_account(account_id)\n         print(f"Vehicles: {await account.get_vehicles()}") # List available vehicles, make a note of vehicle VIN\n\n         vin = "Your vehicle VIN"\n         vehicle = await account.get_api_vehicle(vin)\n         print(f"Cockpit information: {await vehicle.get_cockpit()}")\n         print(f"Battery status information: {await vehicle.get_battery_status()}")\n\n   loop = asyncio.get_event_loop()\n   loop.run_until_complete(main())\n\nCLI Usage\n---------\n\nThe renault-api is also available through a CLI, which requires additional dependencies.\nFor the added dependencies, you can install *Renault API* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install renault-api[cli]\n\nOnce installed, the following command prompts for credentials and settings, displays basic vehicle status information, and generates traces:\n\n.. code:: console\n\n   $ renault-api --log status\n\n* Credentials will automatically be stored in the user home directory (~/.credentials/renault-api.json)\n* Logs will automatically be generated in `logs` subfolder\n\nPlease see the `Command-line Reference <Usage_>`_ for full details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the MIT_ license,\n*Renault API* is free and open source software.\n\n\nDisclaimer\n----------\n\nThis project is not affiliated with, endorsed by, or connected to Renault. I accept no responsibility for any consequences, intended or accidental, as a as a result of interacting with Renault\'s API using this project.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was generated from `@cjolowicz`_\'s `Hypermodern Python Cookiecutter`_ template.\nThis project was heavily based on `@jamesremuscat`_\'s `PyZE`_ python client for the Renault ZE API.\n\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _@jamesremuscat: https://github.com/jamesremuscat\n.. _PyZE: https://github.com/jamesremuscat/pyze\n.. _MIT: http://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _file an issue: https://github.com/hacf-fr/renault-api/issues\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Usage: https://renault-api.readthedocs.io/en/latest/usage.html\n',
     'author': 'epenet',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/hacf-fr/renault-api',
```

### Comparing `renault-api-0.1.8/PKG-INFO` & `renault-api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renault-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Renault API
 Home-page: https://github.com/hacf-fr/renault-api
 License: MIT
 Author: epenet
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

