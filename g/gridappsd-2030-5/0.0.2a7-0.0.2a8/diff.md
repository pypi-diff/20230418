# Comparing `tmp/gridappsd-2030_5-0.0.2a7.tar.gz` & `tmp/gridappsd-2030_5-0.0.2a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd-2030_5-0.0.2a7.tar", max compression
+gzip compressed data, was "gridappsd-2030_5-0.0.2a8.tar", max compression
```

## Comparing `gridappsd-2030_5-0.0.2a7.tar` & `gridappsd-2030_5-0.0.2a8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-04-17 19:10:38.301839 gridappsd-2030_5-0.0.2a7/LICENSE
--rw-r--r--   0        0        0    22262 2023-04-17 19:10:38.301839 gridappsd-2030_5-0.0.2a7/README.md
--rw-r--r--   0        0        0     9324 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/__main__.py
--rw-r--r--   0        0        0    12455 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/__init__.py
--rw-r--r--   0        0        0     1650 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/dcap.py
--rw-r--r--   0        0        0    18247 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/der.py
--rw-r--r--   0        0        0    23752 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/enddevices.py
--rw-r--r--   0        0        0      450 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/fsa.py
--rw-r--r--   0        0        0     1937 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/log.py
--rw-r--r--   0        0        0    17398 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/mupupt.py
--rw-r--r--   0        0        0      820 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/timeadapter.py
--rw-r--r--   0        0        0     8680 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/basic_proxy.py
--rw-r--r--   0        0        0    13249 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/certs.py
--rw-r--r--   0        0        0       95 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/client/__init__.py
--rw-r--r--   0        0        0    11681 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/client/client.py
--rw-r--r--   0        0        0    10263 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/config.py
--rw-r--r--   0        0        0     3486 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/config_setup.py
--rw-r--r--   0        0        0    11071 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/control.py
--rw-r--r--   0        0        0      102 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/data/__init__.py
--rw-r--r--   0        0        0     2746 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/data/indexer.py
--rw-r--r--   0        0        0     1603 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/execute.py
--rw-r--r--   0        0        0    16684 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/flask_server.py
--rw-r--r--   0        0        0       61 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/gridappsd-2030_5.code-workspace
--rw-r--r--   0        0        0    21242 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/hrefs.py
--rw-r--r--   0        0        0    14061 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/__init__.py
--rw-r--r--   0        0        0     3715 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/constants.py
--rw-r--r--   0        0        0     3736 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/derforecasts.py
--rw-r--r--   0        0        0     3222 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/enums.py
--rw-r--r--   0        0        0   281879 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/sep.py
--rw-r--r--   0        0        0        0 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/timetype.py
--rw-r--r--   0        0        0      171 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/tree.py
--rw-r--r--   0        0        0        0 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/persistance/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/persistance/points.py
--rw-r--r--   0        0        0      704 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/__init__.py
--rw-r--r--   0        0        0    10888 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/admin_endpoints.py
--rw-r--r--   0        0        0     3035 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/base_request.py
--rw-r--r--   0        0        0      533 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/dcapfs.py
--rw-r--r--   0        0        0     2725 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/derfs.py
--rw-r--r--   0        0        0     6670 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/enddevicesfs.py
--rw-r--r--   0        0        0      261 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/exceptions.py
--rw-r--r--   0        0        0     1080 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/logfs.py
--rw-r--r--   0        0        0     3303 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/meteringfs.py
--rw-r--r--   0        0        0    20710 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_constructs.py
--rw-r--r--   0        0        0     8946 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_endpoints.py
--rw-r--r--   0        0        0     1566 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/timefs.py
--rw-r--r--   0        0        0     6817 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/usage_pointfs.py
--rw-r--r--   0        0        0     2125 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/uuid_handler.py
--rw-r--r--   0        0        0     1070 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/service.py
--rw-r--r--   0        0        0        0 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/__init__.py
--rw-r--r--   0        0        0      467 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/auth_context.py
--rw-r--r--   0        0        0     6764 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/gridappsd_pump.py
--rw-r--r--   0        0        0     8909 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/inverter.py
--rw-r--r--   0        0        0     2964 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/types_/__init__.py
--rw-r--r--   0        0        0     2220 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/__init__.py
--rw-r--r--   0        0        0     7829 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/tls_wrapper.py
--rw-r--r--   0        0        0     2008 2023-04-17 19:15:42.017103 gridappsd-2030_5-0.0.2a7/pyproject.toml
--rw-r--r--   0        0        0    24823 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a7/setup.py
--rw-r--r--   0        0        0    23836 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-18 18:22:17.118989 gridappsd-2030_5-0.0.2a8/LICENSE
+-rw-r--r--   0        0        0    22262 2023-04-18 18:22:17.118989 gridappsd-2030_5-0.0.2a8/README.md
+-rw-r--r--   0        0        0     9324 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/__main__.py
+-rw-r--r--   0        0        0    12455 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/__init__.py
+-rw-r--r--   0        0        0     1650 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/dcap.py
+-rw-r--r--   0        0        0    18349 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/der.py
+-rw-r--r--   0        0        0    23752 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/enddevices.py
+-rw-r--r--   0        0        0      450 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/fsa.py
+-rw-r--r--   0        0        0     1937 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/log.py
+-rw-r--r--   0        0        0    17398 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/mupupt.py
+-rw-r--r--   0        0        0      820 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/timeadapter.py
+-rw-r--r--   0        0        0     8680 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/basic_proxy.py
+-rw-r--r--   0        0        0    13249 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/certs.py
+-rw-r--r--   0        0        0       95 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/client/__init__.py
+-rw-r--r--   0        0        0    11681 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/client/client.py
+-rw-r--r--   0        0        0    10263 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/config.py
+-rw-r--r--   0        0        0     3486 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/config_setup.py
+-rw-r--r--   0        0        0    11071 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/control.py
+-rw-r--r--   0        0        0      102 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/data/__init__.py
+-rw-r--r--   0        0        0     2746 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/data/indexer.py
+-rw-r--r--   0        0        0     1603 2023-04-18 18:22:17.122989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/execute.py
+-rw-r--r--   0        0        0    16684 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/flask_server.py
+-rw-r--r--   0        0        0       61 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/gridappsd-2030_5.code-workspace
+-rw-r--r--   0        0        0    21242 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/hrefs.py
+-rw-r--r--   0        0        0    14061 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/__init__.py
+-rw-r--r--   0        0        0     3715 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/constants.py
+-rw-r--r--   0        0        0     3736 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/derforecasts.py
+-rw-r--r--   0        0        0     3222 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/enums.py
+-rw-r--r--   0        0        0   281879 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/sep.py
+-rw-r--r--   0        0        0        0 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/timetype.py
+-rw-r--r--   0        0        0      171 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/tree.py
+-rw-r--r--   0        0        0        0 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/persistance/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/persistance/points.py
+-rw-r--r--   0        0        0      704 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/__init__.py
+-rw-r--r--   0        0        0    10888 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/admin_endpoints.py
+-rw-r--r--   0        0        0     3035 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/base_request.py
+-rw-r--r--   0        0        0      533 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/dcapfs.py
+-rw-r--r--   0        0        0     2725 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/derfs.py
+-rw-r--r--   0        0        0     6670 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/enddevicesfs.py
+-rw-r--r--   0        0        0      261 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/exceptions.py
+-rw-r--r--   0        0        0     1080 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/logfs.py
+-rw-r--r--   0        0        0     3303 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/meteringfs.py
+-rw-r--r--   0        0        0    20710 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/server_constructs.py
+-rw-r--r--   0        0        0     8946 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/server_endpoints.py
+-rw-r--r--   0        0        0     1566 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/timefs.py
+-rw-r--r--   0        0        0     6817 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/usage_pointfs.py
+-rw-r--r--   0        0        0     2125 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/uuid_handler.py
+-rw-r--r--   0        0        0     1070 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/service.py
+-rw-r--r--   0        0        0        0 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/simulation/__init__.py
+-rw-r--r--   0        0        0      467 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/simulation/auth_context.py
+-rw-r--r--   0        0        0     6764 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/simulation/gridappsd_pump.py
+-rw-r--r--   0        0        0     8909 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/simulation/inverter.py
+-rw-r--r--   0        0        0     2964 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/types_/__init__.py
+-rw-r--r--   0        0        0     2220 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/utils/__init__.py
+-rw-r--r--   0        0        0     7829 2023-04-18 18:22:17.126989 gridappsd-2030_5-0.0.2a8/ieee_2030_5/utils/tls_wrapper.py
+-rw-r--r--   0        0        0     2008 2023-04-18 18:25:08.589831 gridappsd-2030_5-0.0.2a8/pyproject.toml
+-rw-r--r--   0        0        0    24823 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a8/setup.py
+-rw-r--r--   0        0        0    23836 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a8/PKG-INFO
```

### Comparing `gridappsd-2030_5-0.0.2a7/LICENSE` & `gridappsd-2030_5-0.0.2a8/LICENSE`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/README.md` & `gridappsd-2030_5-0.0.2a8/README.md`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/__main__.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/__main__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/__init__.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/dcap.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/dcap.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/der.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/der.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,32 +106,33 @@
                     else:
                         ctrl.EventStatus = m.EventStatus(currentStatus=0, dateTime=timestamp, potentiallySuperseded=False, reason="Scheduled") 
                     _log.debug(f"ctrl.EventStatus is {ctrl.EventStatus}")
                 else:
                     ctrl.EventStatus = m.EventStatus(currentStatus=0, dateTime=timestamp, potentiallySuperseded=False, reason="Scheduled") 
                 
             if ctrl.EventStatus:
-                # Active control
-                if ctrl.interval.start < timestamp and timestamp < ctrl.interval.start + ctrl.interval.duration:
-                    if ctrl.EventStatus.currentStatus == 0:
-                        _log.debug(f"Activating control {ctrl_index}")
-                        ctrl.EventStatus.currentStatus = 1 # Active
-                        ctrl.EventStatus.dateTime = timestamp
-                        ctrl.EventStatus.reason = f"Control event active {ctrl.mRID}"
+                if ctrl.interval:
+                    # Active control
+                    if ctrl.interval.start < timestamp and timestamp < ctrl.interval.start + ctrl.interval.duration:
+                        if ctrl.EventStatus.currentStatus == 0:
+                            _log.debug(f"Activating control {ctrl_index}")
+                            ctrl.EventStatus.currentStatus = 1 # Active
+                            ctrl.EventStatus.dateTime = timestamp
+                            ctrl.EventStatus.reason = f"Control event active {ctrl.mRID}"
 
-                    if ctrl.mRID not in [x.mRID for x in current_active]:
-                        DERProgramAdapter.add_child(derp, hrefs.DER_CONTROL_ACTIVE, ctrl)
-                        
-                elif timestamp > ctrl.interval.start + ctrl.interval.duration:
-                    if ctrl.EventStatus.currentStatus == 1:
-                        _log.debug(f"Deactivating control {ctrl_index}")
-                        
-                        ctrl.EventStatus.currentStatus = -1 # for me this means complete
-                        DERProgramAdapter.remove_child(derp, hrefs.DER_CONTROL_ACTIVE, ctrl)
-            
+                        if ctrl.mRID not in [x.mRID for x in current_active]:
+                            DERProgramAdapter.add_child(derp, hrefs.DER_CONTROL_ACTIVE, ctrl)
+                            
+                    elif timestamp > ctrl.interval.start + ctrl.interval.duration:
+                        if ctrl.EventStatus.currentStatus == 1:
+                            _log.debug(f"Deactivating control {ctrl_index}")
+                            
+                            ctrl.EventStatus.currentStatus = -1 # for me this means complete
+                            DERProgramAdapter.remove_child(derp, hrefs.DER_CONTROL_ACTIVE, ctrl)
+                
 
 def initialize_der_program_adapter(sender):
     
     config = BaseAdapter.server_config()
     
     controls: List[m.DERControl] = DERControlAdapter.fetch_all()
     curves: List[m.DERCurve] = DERCurveAdapter.fetch_all()
```

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/enddevices.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/enddevices.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/log.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/log.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/mupupt.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/mupupt.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/timeadapter.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/adapters/timeadapter.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/basic_proxy.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/basic_proxy.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/certs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/certs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/client/client.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/client/client.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/config.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/config.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/config_setup.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/config_setup.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/control.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/control.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/data/indexer.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/data/indexer.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/execute.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/execute.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/flask_server.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/flask_server.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/hrefs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/hrefs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/__init__.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/constants.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/constants.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/derforecasts.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/derforecasts.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/enums.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/enums.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/sep.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/models/sep.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/persistance/points.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/persistance/points.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/__init__.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/admin_endpoints.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/admin_endpoints.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/base_request.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/base_request.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/dcapfs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/dcapfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/derfs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/derfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/enddevicesfs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/enddevicesfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/logfs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/logfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/meteringfs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/meteringfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_constructs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/server_constructs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_endpoints.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/server_endpoints.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/timefs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/timefs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/usage_pointfs.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/usage_pointfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/uuid_handler.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/server/uuid_handler.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/service.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/service.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/gridappsd_pump.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/simulation/gridappsd_pump.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/inverter.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/simulation/inverter.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/types_/__init__.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/types_/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/__init__.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/tls_wrapper.py` & `gridappsd-2030_5-0.0.2a8/ieee_2030_5/utils/tls_wrapper.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a7/pyproject.toml` & `gridappsd-2030_5-0.0.2a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-2030_5"
-version = "0.0.2a7"
+version = "0.0.2a8"
 description = ""
 authors = ["C. Allwardt <3979063+craig8@users.noreply.github.com>"]
 packages = [
     { include = "ieee_2030_5" }
 ]
 license = "BSD-3-Clause"
 maintainers = [
```

### Comparing `gridappsd-2030_5-0.0.2a7/setup.py` & `gridappsd-2030_5-0.0.2a8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                      '2030_5_gridappsd = ieee_2030_5.config_setup:_main',
                      '2030_5_proxy = ieee_2030_5.basic_proxy:_main',
                      '2030_5_server = ieee_2030_5.__main__:_main',
                      '2030_5_shutdown = ieee_2030_5.__main__:_shutdown']}
 
 setup_kwargs = {
     'name': 'gridappsd-2030-5',
-    'version': '0.0.2a7',
+    'version': '0.0.2a8',
     'description': '',
     'long_description': '# GridAPPS-D IEEE 2030.5 Server\n\n## Overview\n\nThe GridAPPS-D IEEE 2030.5 Server implements the Common Smart Inverter Profile (CSIP).  The server\ncan work in both in-band and out-of-band registration models detailed in  CCIP Implementation Guide v2\nsection 6.1.3 and 6.1.4 respectively.  \n\n## Setup\n\n## Installing from pypi\n\nThe recommended way to install this project from pypi is in a virtual environment.  Create a virtual environment and install\n2030.5 server as follows.\n\n```shell\n# creates an environment \'env\' in the current directory\npython3 -m venv env\n\n# Activate the environment in the current shell\nsource env/bin/activate\n\n# Install 2030.5 server\npip install gridappsd_2030_5\n```\n\n## Configuration\n\nThe server requires two configuration files.  The first is for generation of certificates and keys for the system (openssl.cnf).  Currently\nwe shell out to openssl for key/cert/ca generation during runtime.  Each time the server is started up it will attempt to regenerate\nkey/certs/ca unless --no-create-certs is passed to the server startup method.  The second is the configuration for the server itself.  \nThe configuration file holds the definitions for controls, der, end devices and other settings that will be used during the runtime\nof the server.\n\nBoth of these configuration files should be placed in the current working directory where you will start the server.\n\n### Example openssl.cnf\n\n```ini\n#\n# OpenSSL example configuration file.\n# This is mostly being used for generation of certificate requests.\n#\n\n# This definition stops the following lines choking if HOME isn\'t\n# defined.\nHOME                    = .\nRANDFILE                = $ENV::HOME/.rnd\n\n# Extra OBJECT IDENTIFIER info:\n#oid_file               = $ENV::HOME/.oid\noid_section             = new_oids\n\n# To use this configuration file with the "-extfile" option of the\n# "openssl x509" utility, name here the section containing the\n# X.509v3 extensions to use:\n# extensions            =\n# (Alternatively, use a configuration file that has only\n# X.509v3 extensions in its main [= default] section.)\n\n[ new_oids ]\n\n# We can add new OIDs in here for use by \'ca\', \'req\' and \'ts\'.\n# Add a simple OID like this:\n# testoid1=1.2.3.4\n# Or use config file substitution like this:\n# testoid2=${testoid1}.5.6\n\n# Policies used by the TSA examples.\ntsa_policy1 = 1.2.3.4.1\ntsa_policy2 = 1.2.3.4.5.6\ntsa_policy3 = 1.2.3.4.5.7\n\n####################################################################\n[ ca ]\ndefault_ca      = CA_default            # The default ca section\n\n[ CA_default ]\ndir             = /home/gridappsd/tls             # Where everything is kept\ncerts           = $dir/certs            # Where the issued certs are kept\ndatabase        = $dir/index.txt        # database index file.\n                                        # several certs with same subject.\nnew_certs_dir   = $dir/certs            # default place for new certs.\ncertificate     = $dir/certs/ec-cacert.pem       # The CA certificate\nserial          = $dir/serial           # The current serial number\ncrlnumber       = $dir/crlnumber        # the current crl number\n                                        # must be commented out to leave a V1 CRL\nprivate_key     = $dir/private/ec-cakey.pem # The private key\n\nname_opt        = ca_default            # Subject Name options\ncert_opt        = ca_default            # Certificate field options\n\ndefault_days    = 365                   # how long to certify for\ndefault_crl_days= 30                    # how long before next CRL\ndefault_md      = sha256                # use SHA-256 by default\npreserve        = no                    # keep passed DN ordering\npolicy          = policy_match\n\n# For the CA policy\n[ policy_match ]\ncountryName             = optional\nstateOrProvinceName     = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = optional\nemailAddress            = optional\n\n[ policy_anything ]\ncountryName             = optional\nstateOrProvinceName     = optional\nlocalityName            = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = optional\nemailAddress            = optional\n\n####################################################################\n[ req ]\ndefault_bits            = 2048\ndefault_md              = sha256\ndefault_keyfile         = privkey.pem\n#distinguished_name      = req_distinguished_name\n#attributes              = req_attributes\nx509_extensions = v3_ca # The extentions to add to the self signed cert\n\n[ req_distinguished_name ]\n#countryName                     = Country Name (2 letter code)\n#countryName_default             = US\n#countryName_min                 = 2\n#countryName_max                 = 2\n#stateOrProvinceName             = State or Province Name (full name)\n#stateOrProvinceName_default     = Washington\n#localityName                    = Locality Name (eg, city)\n#localityName_default            = Richland\n#0.organizationName              = Organization Name (eg, company)\n#0.organizationName_default      =\n#organizationalUnitName          = Organizational Unit Name (eg, section)\n#commonName                      = Common Name (eg, your name or your server\\\'s hostname)\n#commonName_max                  = 64\n#emailAddress                    = Email Address\n#emailAddress_max                = 64\n\n[ req_attributes ]\nchallengePassword               = A challenge password\nchallengePassword_min           = 4\nchallengePassword_max           = 20\nunstructuredName                = An optional company name\n\n\n[ v3_req ]\n# Extensions to add to a certificate request\nbasicConstraints = CA:FALSE\nkeyUsage = nonRepudiation, digitalSignature, keyEncipherment\n\n[ v3_ca ]\n# Extensions for a typical CA\nsubjectKeyIdentifier=hash\nauthorityKeyIdentifier=keyid:always,issuer\nbasicConstraints = critical,CA:true\n\n[ crl_ext ]\n# issuerAltName=issuer:copy\nauthorityKeyIdentifier=keyid:always#\n# OpenSSL example configuration file.\n# This is mostly being used for generation of certificate requests.\n#\n\n# This definition stops the following lines choking if HOME isn\'t\n# defined.\nHOME                    = .\nRANDFILE                = $ENV::HOME/.rnd\n\n# Extra OBJECT IDENTIFIER info:\n#oid_file               = $ENV::HOME/.oid\noid_section             = new_oids\n\n# To use this configuration file with the "-extfile" option of the\n# "openssl x509" utility, name here the section containing the\n# X.509v3 extensions to use:\n# extensions            =\n# (Alternatively, use a configuration file that has only\n# X.509v3 extensions in its main [= default] section.)\n\n[ new_oids ]\n\n# We can add new OIDs in here for use by \'ca\', \'req\' and \'ts\'.\n# Add a simple OID like this:\n# testoid1=1.2.3.4\n# Or use config file substitution like this:\n# testoid2=${testoid1}.5.6\n\n# Policies used by the TSA examples.\ntsa_policy1 = 1.2.3.4.1\ntsa_policy2 = 1.2.3.4.5.6\ntsa_policy3 = 1.2.3.4.5.7\n\n####################################################################\n[ ca ]\ndefault_ca      = CA_default            # The default ca section\n\n[ CA_default ]\ndir             = /home/gridappsd/tls   # Where everything is kept\ncerts           = $dir/certs            # Where the issued certs are kept\ndatabase        = $dir/index.txt        # database index file.\n                                        # several certs with same subject.\nnew_certs_dir   = $dir/certs            # default place for new certs.\ncertificate     = $dir/certs/ec-cacert.pem       # The CA certificate\nserial          = $dir/serial           # The current serial number\ncrlnumber       = $dir/crlnumber        # the current crl number\n                                        # must be commented out to leave a V1 CRL\nprivate_key     = $dir/private/ec-cakey.pem # The private key\n\nname_opt        = ca_default            # Subject Name options\ncert_opt        = ca_default            # Certificate field options\n\ndefault_days    = 365                   # how long to certify for\ndefault_crl_days= 30                    # how long before next CRL\ndefault_md      = sha256                # use SHA-256 by default\npreserve        = no                    # keep passed DN ordering\npolicy          = policy_match\n\n# For the CA policy\n[ policy_match ]\ncountryName             = optional\nstateOrProvinceName     = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = supplied\nemailAddress            = optional\n\n[ policy_anything ]\ncountryName             = optional\nstateOrProvinceName     = optional\nlocalityName            = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = supplied\nemailAddress            = optional\n\n####################################################################\n[ req ]\ndefault_bits            = 2048\ndefault_md              = sha256\ndefault_keyfile         = privkey.pem\ndistinguished_name      = req_distinguished_name\nattributes              = req_attributes\nx509_extensions = v3_ca # The extentions to add to the self signed cert\n\n[ req_distinguished_name ]\ncountryName                     = Country Name (2 letter code)\ncountryName_default             = IN\ncountryName_min                 = 2\ncountryName_max                 = 2\nstateOrProvinceName             = State or Province Name (full name)\nstateOrProvinceName_default     = Some-State\nlocalityName                    = Locality Name (eg, city)\nlocalityName_default            = BANGALORE\n0.organizationName              = Organization Name (eg, company)\n0.organizationName_default      = GoLinuxCloud\norganizationalUnitName          = Organizational Unit Name (eg, section)\ncommonName                      = Common Name (eg, your name or your server\\\'s hostname)\ncommonName_max                  = 64\nemailAddress                    = Email Address\nemailAddress_max                = 64\n\n[ req_attributes ]\nchallengePassword               = A challenge password\nchallengePassword_min           = 4\nchallengePassword_max           = 20\nunstructuredName                = An optional company name\n\n\n[ v3_req ]\n# Extensions to add to a certificate request\nbasicConstraints = CA:FALSE\nkeyUsage = nonRepudiation, digitalSignature, keyEncipherment\n\n[ v3_ca ]\n# Extensions for a typical CA\nsubjectKeyIdentifier=hash\nauthorityKeyIdentifier=keyid:always,issuer\nbasicConstraints = critical,CA:true\n\n[ crl_ext ]\n# issuerAltName=issuer:copy\nauthorityKeyIdentifier=keyid:always\n```\n\n```yaml\n\n### Example config.yml\n---\n#server_hostname: 0.0.0.0:8443\n\nserver: 127.0.0.1\n# Only include if we need to have dcap be available\n# http_port: 8080\nhttps_port: 7443\n\nproxy_hostname: 0.0.0.0:8443\n#server_hostname: 0.0.0.0:7443\n# server_hostname: gridappsd_dev_2004:7443\n\ntls_repository: "./tls"\nopenssl_cnf: "openssl.cnf"\n\n#server_mode: enddevices_register_access_only\nserver_mode: enddevices_create_on_start\n\n# lfdi_mode: Determines what piece of information is used to calculate the lfdi\n#\n# Options:\n#   lfdi_mode_from_file             - sha256 hash of certificate file\'s content.\n#   lfdi_mode_from_cert_fingerprint - sha256 hash of the certificates fingerprint.\n#\n# default: lfdi_mode_from_cert_fingerprint\n#lfdi_mode: lfdi_mode_from_file\nlfdi_mode: lfdi_mode_from_cert_fingerprint\n\n# Create an administrator certificate that can be used from\n# browser/api to connect to the platform.\ngenerate_admin_cert: True\n\nlog_event_list_poll_rate: 60\ndevice_capability_poll_rate: 60\n\n# End Device\ndevices:\n  # SolarEdge SE6000H HD-Wave SetApp Enabled Inverter\n  - id: dev1\n    # DeviceCategoryType from ieee_2030_5.models.device_category\n    deviceCategory: FUEL_CELL\n    pin: 111115\n\n    programs:\n      - description: Program 1\n\n    # nameplate:\n    #   rtgMaxW: 6000\n    ders:\n      - capabilities:\n        modesSupported: "1110000000000000"\n        type: 83\n\n      - capabilities:\n        # Bitmask with the following structure.\n        # Indication of support for each control mode function DERCapability::modesSupported\n        #\n        # 0 - Charge mode\n        # 1 - Discharge mode\n        # 2 - opModConnect (Connect / Disconnect -\n        # implies galvanic isolation)\n        # 3 - opModEnergize (Energize / De-Energize)\n        # 4 - opModFixedPFAbsorbW (Fixed Power\n        # Factor Setpoint when absorbing active\n        # power)\n        # 5 - opModFixedPFInjectW (Fixed Power\n        # Factor Setpoint when injecting active\n        # power)\n        # 6 - opModFixedVar (Reactive Power\n        # Setpoint)\n        # 7 - opModFixedW (Charge / Discharge\n        # Setpoint)\n        # 8 - opModFreqDroop (Frequency-Watt\n        # Parameterized Mode)\n        # 9 - opModFreqWatt (Frequency-Watt\n        # Curve Mode)\n        # 10 - opModHFRTMayTrip (High Frequency\n        # Ride Through, May Trip Mode)\n        # 11 - opModHFRTMustTrip (High\n        # Frequency Ride Through, Must Trip Mode)\n        # 12 - opModHVRTMayTrip (High Voltage\n        # Ride Through, May Trip Mode)\n        # 13 - opModHVRTMomentaryCessation\n        # (High Voltage Ride Through, Momentary\n        # Cessation Mode)\n        # 14 - opModHVRTMustTrip (High Voltage\n        # Ride Through, Must Trip Mode)\n        # 15 - opModLFRTMayTrip (Low Frequency\n        # Ride Throu\n        modesSupported: "1110000000000000"\n\n        # Item type for the DER.\n        # 0 - Not applicable / Unknown\n        # 1 - Virtual or mixed DER\n        # 2 - Reciprocating engine\n        # 3 - Fuel cell\n        # 4 - Photovoltaic system\n        # 5 - Combined heat and power\n        # 6 - Other generation system\n        # 80 - Other storage system\n        # 81 - Electric vehicle\n        # 82 - EVSE\n        # 83 - Combined PV and storage\n        type: 83\n\n        # Default available nameplate options where at a manufacturer\'s set.\n        # Active power rating in watts an unity power factor\n        rtgMaxW: 600\n\n        # Active power rating in watts at specified over-excited power factor\n        # rtgOverExcitedW:\n\n        # Over-excited power factor DERCapability::rtgOverExcitedPF\n        # rtgOverExcitedPF:\n\n        # Active power rating in watts at specified under-excited power factor DERCapability::rtgUnderExcitedW\n        # rtgUnderExcitedW:\n\n        # Under-excited power factor DERCapability::rtgUnderExcitedPF\n        # rtgUnderExcitedPF:\n\n        # Maximum apparent power rating in voltamperes DERCapability::rtgMaxVA\n        rtgMaxVA: 600\n\n        # Indication of reactive power and voltage/power control capability DERCapability::rtgNormalCategory\n        rtgNormalCategory: 1\n\n        # Indication of voltage and frequencyride-through capability category I, II, or III DERCapability::rtgAbnormalCategory\n        rtgAbnormalCategory: 1\n\n        # Maximum injected reactive power rating in vars DERCapability::rtgMaxVar\n        rtgMaxVar: 600\n\n        # Maximum absorbed reactive power rating in vars DERCapability::rtgMaxVarNeg\n        rtgMaxVarNeg: 600\n\n        # Maximum active power charge rating in watts DERCapability::rtgMaxChargeRateW\n        rtgMaxChargeRateW: 600\n\n        # Maximum apparent power charge rating in voltamperes; may differ from the apparent power maximum rating\n        # DERCapability::rtgMaxChargeRateVA\n        rtgMaxChargeRateVA: 600\n\n        # Nominal ac voltage rating in rms volts DERCapability::rtgVNom\n        rtgVNom: 120\n\n        # Maximum ac voltage rating in rms volts DERCapability::rtgMaxV\n        rtgMaxV: 128\n\n        # Minimum ac voltage rating in rms volts DERCapability::rtgMinV\n        rtgMinV: 116\n\n        # Reactive susceptance that remains connected to the Area EPS in the cease to energize and trip state\n        # DERCapability::rtgReactiveSusceptance\n        # rtgReactiveSusceptance:\n\n        # # Manufacturer DeviceInformation::mfID\n        # mfID:\n\n        # # Model DeviceInformation::mfModel\n        # mfModel:\n\n        # # Serial number DeviceInformation::mfSerNum\n        # mfSerNum:\n\n        # # Version DeviceInformation::mfHwVer DeviceInformation::swVer\n        # mfHwVer:\n        # swVer:\n\n  - id: dev2\n    deviceCategory: FUEL_CELL\n    pin: 12345\n    nameplate:\n\nprograms:\n  - description: Program 1\n    default_control: Control 1\n    controls:\n      - Control 2\n      - Control 3\n    curves:\n      - Curve 1\n    primacy: 89\n\ncontrols:\n  - description: Control 1\n    setESDelay: 30\n    base:\n      opModConnect: True\n      opModMaxLimW: 9500\n\n      # setESHighFreq: UInt16 [0..1]\n      # setESHighVolt: Int16 [0..1]\n      # setESLowFreq: UInt16 [0..1]\n      # setESLowVolt: Int16 [0..1]\n      # setESRampTms: UInt32 [0..1]\n      # setESRandomDelay: UInt32 [0..1]\n      # setGradW: UInt16 [0..1]\n      # setSoftGradW: UInt16 [0..1]\n  - description: Control 2\n  - description: Control 3\n\nevents:\n  - control: 0\n\ncurves:\n  # Each element will can have the following structure.\n  # autonomousVRefEnable: If the curveType is opModVoltVar, then\n  #   this field MAY be present. If the curveType is not opModVoltVar,\n  #   then this field SHALL NOT be present. Enable/disable autonomous\n  #   vRef adjustment. When enabled, the Volt-Var curve characteristic\n  #   SHALL be adjusted autonomously as vRef changes and\n  #   autonomousVRefTimeConstant SHALL be present. If a DER is able to\n  #   support Volt-Var mode but is unable to support autonomous vRef\n  #   adjustment, then the DER SHALL execute the curve without\n  #   autonomous vRef adjustment. If not specified, then the value is\n  #   false.\n  # autonomousVRefTimeConstant: If the curveType is opModVoltVar,\n  #   then this field MAY be present. If the curveType is not\n  #   opModVoltVar, then this field SHALL NOT be present. Adjustment\n  #   range for vRef time constant, in hundredths of a second.\n  # creationTime: The time at which the object was created.\n  # CurveData:\n  # curveType: Specifies the associated curve-based control mode.\n  # openLoopTms: Open loop response time, the time to ramp up to\n  #   90% of the new target in response to the change in voltage, in\n  #   hundredths of a second. Resolution is 1/100 sec. A value of 0 is\n  #   used to mean no limit. When not present, the device SHOULD\n  #   follow its default behavior.\n  # rampDecTms: Decreasing ramp rate, interpreted as a percentage\n  #   change in output capability limit per second (e.g. %setMaxW /\n  #   sec).  Resolution is in hundredths of a percent/second. A value\n  #   of 0 means there is no limit. If absent, ramp rate defaults to\n  #   setGradW.\n  # rampIncTms: Increasing ramp rate, interpreted as a percentage\n  #   change in output capability limit per second (e.g. %setMaxW /\n  #   sec).  Resolution is in hundredths of a percent/second. A value\n  #   of 0 means there is no limit. If absent, ramp rate defaults to\n  #   rampDecTms.\n  # rampPT1Tms: The configuration parameter for a low-pass filter,\n  #   PT1 is a time, in hundredths of a second, in which the filter\n  #   will settle to 95% of a step change in the input value.\n  #   Resolution is 1/100 sec.\n  # vRef: If the curveType is opModVoltVar, then this field MAY be\n  #   present. If the curveType is not opModVoltVar, then this field\n  #   SHALL NOT be present. The nominal AC voltage (RMS) adjustment to\n  #   the voltage curve points for Volt-Var curves.\n  # xMultiplier: Exponent for X-axis value.\n  # yMultiplier: Exponent for Y-axis value.\n  # yRefType: The Y-axis units context.\n  # Each curve MUST have between 1 and 10 elements in the curve_data list.\n  #\n  # DERCurve Type for each curve.\n  # 0 - opModFreqWatt (Frequency-Watt Curve Mode)\n  # 1 - opModHFRTMayTrip (High Frequency Ride Through, May Trip Mode)\n  # 2 - opModHFRTMustTrip (High Frequency Ride Through, Must Trip Mode)\n  # 3 - opModHVRTMayTrip (High Voltage Ride Through, May Trip Mode)\n  # 4 - opModHVRTMomentaryCessation (High Voltage Ride Through, Momentary Cessation\n  # Mode)\n  # 5 - opModHVRTMustTrip (High Voltage Ride Through, Must Trip Mode)\n  # 6 - opModLFRTMayTrip (Low Frequency Ride Through, May Trip Mode)\n  # 7 - opModLFRTMustTrip (Low Frequency Ride Through, Must Trip Mode)\n  # 8 - opModLVRTMayTrip (Low Voltage Ride Through, May Trip Mode)\n  # 9 - opModLVRTMomentaryCessation (Low Voltage Ride Through, Momentary Cessation\n  # Mode)\n  # 10 - opModLVRTMustTrip (Low Voltage Ride Through, Must Trip Mode)\n  # 11 - opModVoltVar (Volt-Var Mode)\n  # 12 - opModVoltWatt (Volt-Watt Mode)\n  # 13 - opModWattPF (Watt-PowerFactor Mode)\n  # 14 - opModWattVar (Watt-Var Mode)\n  - description: Curve 1\n    curveType: opModVoltVar\n    CurveData:\n      - xvalue: 5\n        yvalue: 5\n\n  - description: Curve 2\n    curveType: opModFreqWatt\n    CurveData:\n      # exitation is only available if yvalue is power factor\n      - exitation: 10\n        xvalue: 5\n        yvalue: 5\n```\n\n## Installing from source\n\nThe installation requires poetry version 1.2 or greater.  <https://python-poetry.org/docs/#installation>\n\n 1. Clone the repository\n 2. run `poetry install` from the root of the repository directory.\n\n### Clone the repository\n\n```shell\ngit clone https://github.com/GRIDAPPSD/gridappsd-2030_5 -b develop\ncd gridappsd-2030_5\n```\n\n### Install Requirements\n\n```shell\npoetry install\n```\n\n### Run the Server\n\n```shell\nusage: 2030_5_server [-h] [--no-validate] [--no-create-certs] [--debug] config\n\npositional arguments:\n  config             Configuration file for the server.\n\noptional arguments:\n  -h, --help         show this help message and exit\n  --no-validate      Allows faster startup since the resolving of addresses for devices is not done.\n  --no-create-certs  If specified certificates for for client and server will not be created.\n  --debug            Put server in debug mode (more logging)\n```\n\n### Using the 2030.5 proxy\n\nThe proxy is used to keep a http 1.1 connection alive rather than doing the tls setup\nmore than one time.\n\n```shell\nusage: 2030_5_proxy [-h] [--debug] config\n\npositional arguments:\n  config      Configuration file for the server.\n\noptional arguments:\n  -h, --help  show this help message and exit\n  --debug     Turns debugging on for logging of the proxy.\n```\n\n## Client Connectivity\n\nThe server will expose an endpoint of beginning with <https://myserver/dcap>.  From there\na client will be able to traverse and do any PUT, POST, GET, and DELETE operations specified\nin the 2030.5 test procedures.\n\n## Function Sets Implemented\n',
     'author': 'C. Allwardt',
     'author_email': '3979063+craig8@users.noreply.github.com',
     'maintainer': 'C. Allwardt',
     'maintainer_email': '3979063+craig8@users.noreply.github.com',
     'url': 'https://github.com/GRIDAPPSD/gridappsd-2030_5',
```

### Comparing `gridappsd-2030_5-0.0.2a7/PKG-INFO` & `gridappsd-2030_5-0.0.2a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridappsd-2030-5
-Version: 0.0.2a7
+Version: 0.0.2a8
 Summary: 
 Home-page: https://github.com/GRIDAPPSD/gridappsd-2030_5
 License: BSD-3-Clause
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Maintainer: C. Allwardt
 Maintainer-email: 3979063+craig8@users.noreply.github.com
```

