# Comparing `tmp/pyhanko-certvalidator-0.21.1.tar.gz` & `tmp/pyhanko-certvalidator-0.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhanko-certvalidator-0.21.1.tar", last modified: Sun Apr  2 08:41:07 2023, max compression
+gzip compressed data, was "pyhanko-certvalidator-0.21.2.tar", last modified: Mon Apr 17 21:55:20 2023, max compression
```

## Comparing `pyhanko-certvalidator-0.21.1.tar` & `pyhanko-certvalidator-0.21.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.492749 pyhanko-certvalidator-0.21.1/
--rw-r--r--   0 matthias   (501) staff       (20)     1138 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/LICENSE
--rw-r--r--   0 matthias   (501) staff       (20)     4817 2023-04-02 08:41:07.492616 pyhanko-certvalidator-0.21.1/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)     3864 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/README.md
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.484738 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/
--rw-r--r--   0 matthias   (501) staff       (20)    11707 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     1141 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/_asyncio_compat.py
--rw-r--r--   0 matthias   (501) staff       (20)     2578 2023-04-01 15:28:48.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/_state.py
--rw-r--r--   0 matthias   (501) staff       (20)      481 2022-05-24 17:45:42.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/_types.py
--rw-r--r--   0 matthias   (501) staff       (20)     2909 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/asn1_types.py
--rw-r--r--   0 matthias   (501) staff       (20)     8798 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/authority.py
--rw-r--r--   0 matthias   (501) staff       (20)    24845 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/context.py
--rw-r--r--   0 matthias   (501) staff       (20)     5209 2023-04-02 08:38:49.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/errors.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.485957 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/
--rw-r--r--   0 matthias   (501) staff       (20)      491 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/__init__.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.487031 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/
--rw-r--r--   0 matthias   (501) staff       (20)     1257 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     4955 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     3983 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     4424 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     1846 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py
--rw-r--r--   0 matthias   (501) staff       (20)     6622 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/api.py
--rw-r--r--   0 matthias   (501) staff       (20)    10682 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/common_utils.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.488121 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/
--rw-r--r--   0 matthias   (501) staff       (20)     1019 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     4516 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     2603 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     3482 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     2464 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/util.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.489086 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     6053 2023-04-02 08:38:49.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/ades_past.py
--rw-r--r--   0 matthias   (501) staff       (20)      235 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/errors.py
--rw-r--r--   0 matthias   (501) staff       (20)     3280 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/poe.py
--rw-r--r--   0 matthias   (501) staff       (20)    16108 2023-03-21 22:12:59.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/time_slide.py
--rw-r--r--   0 matthias   (501) staff       (20)     1464 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/types.py
--rw-r--r--   0 matthias   (501) staff       (20)    13166 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/name_trees.py
--rw-r--r--   0 matthias   (501) staff       (20)    12224 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/path.py
--rw-r--r--   0 matthias   (501) staff       (20)    19124 2023-04-02 08:38:49.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/policy_decl.py
--rw-r--r--   0 matthias   (501) staff       (20)    10970 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/policy_tree.py
--rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/py.typed
--rw-r--r--   0 matthias   (501) staff       (20)    22057 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/registry.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.490443 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)    14102 2023-04-02 08:38:49.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/archival.py
--rw-r--r--   0 matthias   (501) staff       (20)      567 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/constants.py
--rw-r--r--   0 matthias   (501) staff       (20)     8178 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/manager.py
--rw-r--r--   0 matthias   (501) staff       (20)    47720 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/validate_crl.py
--rw-r--r--   0 matthias   (501) staff       (20)    23041 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/validate_ocsp.py
--rw-r--r--   0 matthias   (501) staff       (20)    10347 2023-04-01 15:33:21.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/util.py
--rw-r--r--   0 matthias   (501) staff       (20)    55273 2023-04-02 08:38:49.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/validate.py
--rw-r--r--   0 matthias   (501) staff       (20)       71 2023-04-02 08:40:19.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/version.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.485394 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/
--rw-r--r--   0 matthias   (501) staff       (20)     4817 2023-04-02 08:41:07.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)     2307 2023-04-02 08:41:07.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/SOURCES.txt
--rw-r--r--   0 matthias   (501) staff       (20)        1 2023-04-02 08:41:07.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/dependency_links.txt
--rw-r--r--   0 matthias   (501) staff       (20)      218 2023-04-02 08:41:07.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/requires.txt
--rw-r--r--   0 matthias   (501) staff       (20)       22 2023-04-02 08:41:07.000000 pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/top_level.txt
--rw-r--r--   0 matthias   (501) staff       (20)     2099 2023-03-08 19:43:30.000000 pyhanko-certvalidator-0.21.1/pyproject.toml
--rw-r--r--   0 matthias   (501) staff       (20)       38 2023-04-02 08:41:07.492797 pyhanko-certvalidator-0.21.1/setup.cfg
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-02 08:41:07.492367 pyhanko-certvalidator-0.21.1/tests/
--rw-r--r--   0 matthias   (501) staff       (20)    18398 2023-04-01 15:28:58.000000 pyhanko-certvalidator-0.21.1/tests/test_ac_validate.py
--rw-r--r--   0 matthias   (501) staff       (20)    12665 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/tests/test_ades_time_slide.py
--rw-r--r--   0 matthias   (501) staff       (20)     5291 2023-04-01 15:28:58.000000 pyhanko-certvalidator-0.21.1/tests/test_certificate_validator.py
--rw-r--r--   0 matthias   (501) staff       (20)     1247 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/tests/test_crl_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     7376 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/tests/test_freshness.py
--rw-r--r--   0 matthias   (501) staff       (20)     3220 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/tests/test_ocsp_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     7054 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/tests/test_policy_proc.py
--rw-r--r--   0 matthias   (501) staff       (20)     2042 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.1/tests/test_registry.py
--rw-r--r--   0 matthias   (501) staff       (20)    22095 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.1/tests/test_validate.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.102492 pyhanko-certvalidator-0.21.2/
+-rw-r--r--   0 matthias   (501) staff       (20)     1138 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/LICENSE
+-rw-r--r--   0 matthias   (501) staff       (20)     4817 2023-04-17 21:55:20.102348 pyhanko-certvalidator-0.21.2/PKG-INFO
+-rw-r--r--   0 matthias   (501) staff       (20)     3864 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/README.md
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.096996 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/
+-rw-r--r--   0 matthias   (501) staff       (20)    11707 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1141 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_asyncio_compat.py
+-rw-r--r--   0 matthias   (501) staff       (20)     2578 2023-04-01 15:28:48.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_state.py
+-rw-r--r--   0 matthias   (501) staff       (20)      481 2022-05-24 17:45:42.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_types.py
+-rw-r--r--   0 matthias   (501) staff       (20)     2909 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/asn1_types.py
+-rw-r--r--   0 matthias   (501) staff       (20)     8798 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/authority.py
+-rw-r--r--   0 matthias   (501) staff       (20)    24845 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/context.py
+-rw-r--r--   0 matthias   (501) staff       (20)     5209 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/errors.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.097972 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/
+-rw-r--r--   0 matthias   (501) staff       (20)      491 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/__init__.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.098594 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/
+-rw-r--r--   0 matthias   (501) staff       (20)     1257 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     4955 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     3983 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     4424 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1846 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py
+-rw-r--r--   0 matthias   (501) staff       (20)     6622 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/api.py
+-rw-r--r--   0 matthias   (501) staff       (20)    10682 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/common_utils.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.099275 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/
+-rw-r--r--   0 matthias   (501) staff       (20)     1019 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     4510 2023-04-17 21:02:32.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     2603 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     3482 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     2464 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/util.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.100149 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     6053 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/ades_past.py
+-rw-r--r--   0 matthias   (501) staff       (20)      235 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/errors.py
+-rw-r--r--   0 matthias   (501) staff       (20)     3280 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/poe.py
+-rw-r--r--   0 matthias   (501) staff       (20)    16108 2023-03-21 22:12:59.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/time_slide.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1464 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/types.py
+-rw-r--r--   0 matthias   (501) staff       (20)    13166 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/name_trees.py
+-rw-r--r--   0 matthias   (501) staff       (20)    12224 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/path.py
+-rw-r--r--   0 matthias   (501) staff       (20)    19124 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_decl.py
+-rw-r--r--   0 matthias   (501) staff       (20)    10970 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_tree.py
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/py.typed
+-rw-r--r--   0 matthias   (501) staff       (20)    22057 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/registry.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.100964 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)    13846 2023-04-17 21:02:32.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/archival.py
+-rw-r--r--   0 matthias   (501) staff       (20)      567 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/constants.py
+-rw-r--r--   0 matthias   (501) staff       (20)     8178 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/manager.py
+-rw-r--r--   0 matthias   (501) staff       (20)    47720 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_crl.py
+-rw-r--r--   0 matthias   (501) staff       (20)    23041 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_ocsp.py
+-rw-r--r--   0 matthias   (501) staff       (20)    10347 2023-04-01 15:33:21.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/util.py
+-rw-r--r--   0 matthias   (501) staff       (20)    55273 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/validate.py
+-rw-r--r--   0 matthias   (501) staff       (20)       71 2023-04-17 21:53:26.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/version.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.097613 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/
+-rw-r--r--   0 matthias   (501) staff       (20)     4817 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/PKG-INFO
+-rw-r--r--   0 matthias   (501) staff       (20)     2307 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias   (501) staff       (20)        1 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias   (501) staff       (20)      218 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/requires.txt
+-rw-r--r--   0 matthias   (501) staff       (20)       22 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/top_level.txt
+-rw-r--r--   0 matthias   (501) staff       (20)     2099 2023-03-08 19:43:30.000000 pyhanko-certvalidator-0.21.2/pyproject.toml
+-rw-r--r--   0 matthias   (501) staff       (20)       38 2023-04-17 21:55:20.102534 pyhanko-certvalidator-0.21.2/setup.cfg
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.102123 pyhanko-certvalidator-0.21.2/tests/
+-rw-r--r--   0 matthias   (501) staff       (20)    18398 2023-04-01 15:28:58.000000 pyhanko-certvalidator-0.21.2/tests/test_ac_validate.py
+-rw-r--r--   0 matthias   (501) staff       (20)    12665 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/tests/test_ades_time_slide.py
+-rw-r--r--   0 matthias   (501) staff       (20)     5291 2023-04-01 15:28:58.000000 pyhanko-certvalidator-0.21.2/tests/test_certificate_validator.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1247 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_crl_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     7376 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_freshness.py
+-rw-r--r--   0 matthias   (501) staff       (20)     3220 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_ocsp_client.py
+-rw-r--r--   0 matthias   (501) staff       (20)     7054 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_policy_proc.py
+-rw-r--r--   0 matthias   (501) staff       (20)     2042 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_registry.py
+-rw-r--r--   0 matthias   (501) staff       (20)    22461 2023-04-17 21:36:08.000000 pyhanko-certvalidator-0.21.2/tests/test_validate.py
```

### Comparing `pyhanko-certvalidator-0.21.1/LICENSE` & `pyhanko-certvalidator-0.21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/PKG-INFO` & `pyhanko-certvalidator-0.21.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhanko-certvalidator
-Version: 0.21.1
+Version: 0.21.2
 Summary: Validates X.509 certificates and paths; forked from wbond/certvalidator
 Author-email: Matthias Valvekens <dev@mvalvekens.be>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthiasValvekens/certvalidator
 Keywords: crypto,pki,x509,certificate,crl,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pyhanko-certvalidator-0.21.1/README.md` & `pyhanko-certvalidator-0.21.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/__init__.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/_asyncio_compat.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_asyncio_compat.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/_state.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_state.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/asn1_types.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/asn1_types.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/authority.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/authority.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/context.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/context.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/errors.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/errors.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/api.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/api.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/common_utils.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/common_utils.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             target = cert.subject.human_friendly
         else:
             # TODO log audit ID
             target = "attribute certificate"
         logger.info(f"Retrieving issuer certs for {target}...")
         return complete_certificate_fetch_jobs(fetch_jobs)
 
-    async def fetch_crl_issuers(self, certificate_list):
+    def fetch_crl_issuers(self, certificate_list):
         fetch_jobs = [
             self.fetch_certs(url, url_origin_type='CRL')
             for url in certificate_list.issuer_cert_urls
         ]
         return complete_certificate_fetch_jobs(fetch_jobs)
 
     def fetched_certs(self) -> Iterable[x509.Certificate]:
```

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/fetchers/requests_fetchers/util.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/ades_past.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/ades_past.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/poe.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/poe.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/time_slide.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/time_slide.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/ltv/types.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/types.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/name_trees.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/name_trees.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/path.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/path.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/policy_decl.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_decl.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/policy_tree.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_tree.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/registry.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/registry.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/archival.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/archival.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,27 +166,22 @@
     next_update: Optional[datetime],
     policy: CertRevTrustPolicy,
     timing_params: ValidationTimingParams,
 ) -> RevinfoUsability:
     if this_update is None:
         return RevinfoUsability(RevinfoUsabilityRating.UNCLEAR)
 
+    validation_time = timing_params.validation_time
+    time_tolerance = timing_params.time_tolerance
+
     # Revinfo issued after the validation time may need to be considered
     # in AdES point-in-time validation.
     # In the legacy "default" policy, this is controlled by the retroactive
     # revinfo switch.
-    if timing_params.validation_time < this_update:
-        if (
-            not policy.retroactive_revinfo
-            and policy.freshness_req_type == FreshnessReqType.DEFAULT
-        ):
-            return RevinfoUsability(RevinfoUsabilityRating.TOO_NEW)
 
-    validation_time = timing_params.validation_time
-    time_tolerance = timing_params.time_tolerance
     # see 5.2.5.4 in ETSI EN 319 102-1
     if policy.freshness_req_type == FreshnessReqType.TIME_AFTER_SIGNATURE:
         # check whether the revinfo was generated sufficiently long _after_
         # the (presumptive) signature time
         freshness_delta = _freshness_delta(
             policy, this_update, next_update, time_tolerance
         )
```

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/constants.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/constants.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/manager.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/manager.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/validate_crl.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_crl.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/revinfo/validate_ocsp.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_ocsp.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/util.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator/validate.py` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/validate.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/PKG-INFO` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhanko-certvalidator
-Version: 0.21.1
+Version: 0.21.2
 Summary: Validates X.509 certificates and paths; forked from wbond/certvalidator
 Author-email: Matthias Valvekens <dev@mvalvekens.be>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthiasValvekens/certvalidator
 Keywords: crypto,pki,x509,certificate,crl,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pyhanko-certvalidator-0.21.1/pyhanko_certvalidator.egg-info/SOURCES.txt` & `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/pyproject.toml` & `pyhanko-certvalidator-0.21.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_ac_validate.py` & `pyhanko-certvalidator-0.21.2/tests/test_ac_validate.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_ades_time_slide.py` & `pyhanko-certvalidator-0.21.2/tests/test_ades_time_slide.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_certificate_validator.py` & `pyhanko-certvalidator-0.21.2/tests/test_certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_crl_client.py` & `pyhanko-certvalidator-0.21.2/tests/test_crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_freshness.py` & `pyhanko-certvalidator-0.21.2/tests/test_freshness.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_ocsp_client.py` & `pyhanko-certvalidator-0.21.2/tests/test_ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_policy_proc.py` & `pyhanko-certvalidator-0.21.2/tests/test_policy_proc.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_registry.py` & `pyhanko-certvalidator-0.21.2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.1/tests/test_validate.py` & `pyhanko-certvalidator-0.21.2/tests/test_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,21 @@
         raise CRLFetchError("No connection")
 
 
 class MockCertFetcher(CertificateFetcher):
     def fetched_certs(self) -> Iterable[x509.Certificate]:
         return ()
 
-    async def fetch_cert_issuers(self, cert):
-        raise CertificateFetchError("No connection")
+    def fetch_cert_issuers(self, cert):
+        return self
+
+    def fetch_crl_issuers(self, certificate_list):
+        return self
 
-    async def fetch_crl_issuers(self, certificate_list):
+    def __aiter__(self):
         raise CertificateFetchError("No connection")
 
 
 class MockFetcherBackend(FetcherBackend):
     def get_fetchers(self) -> Fetchers:
         return Fetchers(
             ocsp_fetcher=MockOCSPFetcher(),
@@ -98,14 +101,15 @@
 
 @dataclass(frozen=True)
 class PKITSTestCaseErrorResult:
     err_class: Type[Exception]
     msg_regex: str
 
 
+@pytest.mark.skip("annoying to maintain; replace with certomancer test")
 def test_revocation_mode_soft():
     cert = load_cert_object(
         'digicert-ecc-p384-root-g5-revoked-chain-demos-digicert-com.crt'
     )
     ca_certs = [load_cert_object('digicert-root-g5.crt')]
     other_certs = [
         load_cert_object('digicert-g5-ecc-sha384-2021-ca1.crt'),
@@ -122,14 +126,15 @@
     assert 1 == len(paths)
     path = paths[0]
     assert 3 == len(path)
 
     validate_path(context, path)
 
 
+@pytest.mark.skip("annoying to maintain; replace with certomancer test")
 def test_revocation_mode_hard():
     cert = load_cert_object(
         'digicert-ecc-p384-root-g5-revoked-chain-demos-digicert-com.crt'
     )
     ca_certs = [load_cert_object('digicert-root-g5.crt')]
     other_certs = [
         load_cert_object('digicert-g5-ecc-sha384-2021-ca1.crt'),
@@ -155,14 +160,15 @@
         'revoked at \\d\\d:\\d\\d:\\d\\d on \\d\\d\\d\\d-\\d\\d-\\d\\d'
         ', due to an unspecified reason'
     )
     with pytest.raises(RevokedError, match=expected):
         validate_path(context, path)
 
 
+@pytest.mark.skip("annoying to maintain; replace with certomancer test")
 @pytest.mark.asyncio
 async def test_revocation_mode_hard_async():
     cert = load_cert_object(
         'digicert-ecc-p384-root-g5-revoked-chain-demos-digicert-com.crt'
     )
     ca_certs = [load_cert_object('digicert-root-g5.crt')]
     other_certs = [
@@ -190,14 +196,15 @@
             'revoked at \\d\\d:\\d\\d:\\d\\d on \\d\\d\\d\\d-\\d\\d-\\d\\d'
             ', due to an unspecified reason'
         )
         with pytest.raises(RevokedError, match=expected):
             await async_validate_path(context, path)
 
 
+@pytest.mark.skip("annoying to maintain; replace with certomancer test")
 @pytest.mark.asyncio
 async def test_revocation_mode_hard_aiohttp_autofetch():
     cert = load_cert_object(
         'digicert-ecc-p384-root-g5-revoked-chain-demos-digicert-com.crt'
     )
     ca_certs = [load_cert_object('digicert-root-g5.crt')]
 
@@ -222,14 +229,15 @@
             'revoked at \\d\\d:\\d\\d:\\d\\d on \\d\\d\\d\\d-\\d\\d-\\d\\d'
             ', due to an unspecified reason'
         )
         with pytest.raises(RevokedError, match=expected):
             await async_validate_path(context, path)
 
 
+@pytest.mark.skip("annoying to maintain; replace with certomancer test")
 @pytest.mark.asyncio
 async def test_revocation_mode_hard_requests_autofetch():
     cert = load_cert_object(
         'digicert-ecc-p384-root-g5-revoked-chain-demos-digicert-com.crt'
     )
     ca_certs = [load_cert_object('digicert-root-g5.crt')]
```

