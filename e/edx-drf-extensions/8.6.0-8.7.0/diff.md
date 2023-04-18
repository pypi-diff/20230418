# Comparing `tmp/edx-drf-extensions-8.6.0.tar.gz` & `tmp/edx-drf-extensions-8.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-drf-extensions-8.6.0.tar", last modified: Wed Apr 12 20:38:48 2023, max compression
+gzip compressed data, was "edx-drf-extensions-8.7.0.tar", last modified: Tue Apr 18 20:28:33 2023, max compression
```

## Comparing `edx-drf-extensions-8.6.0.tar` & `edx-drf-extensions-8.7.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     6371 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9807 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9807 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)    13020 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)    13147 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    19910 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)    17320 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     6622 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10058 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.983485 edx-drf-extensions-8.7.0/csrf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.983485 edx-drf-extensions-8.7.0/csrf/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/csrf/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/csrf/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10058 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13117 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13147 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9944 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10793 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17320 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-18 20:28:32.999486 edx-drf-extensions-8.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/setup.py
```

### Comparing `edx-drf-extensions-8.6.0/CHANGELOG.rst` & `edx-drf-extensions-8.7.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,27 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.7.0] - 2023-04-14
+--------------------
+
+Added
+~~~~~
+
+* Add ``edx_drf_extensions_version`` to help with rollout of changes in this library across services.
+
+Removed
+~~~~~~~
+
+* Removed exception case for ``InvalidTokenError`` that was never invoked.
+
 [8.6.0] - 2023-04-12
 --------------------
 
 Added
 ~~~~~
 
 * Added ``jwt_auth_check_symmetric_key``, ``jwt_auth_asymmetric_verified``, ``jwt_auth_symmetric_verified``, and ``jwt_auth_verification_failed`` custom attributes to aid in deprecation and removal of symmetric keys.
@@ -157,15 +170,15 @@
 
 * Added a new custom attribute `request_is_staff_or_superuser`
 
 [6.3.0] - 2021-01-12
 --------------------
 
 Removed
-~~~~~~~~
+~~~~~~~
 
 * Drop support for Python 3.5
 
 [6.2.0] - 2020-08-24
 --------------------
 
 Updated
```

### Comparing `edx-drf-extensions-8.6.0/LICENSE.txt` & `edx-drf-extensions-8.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/PKG-INFO` & `edx-drf-extensions-8.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-drf-extensions
-Version: 8.6.0
+Version: 8.7.0
 Summary: edX extensions of Django REST Framework
 Home-page: https://github.com/openedx/edx-drf-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -94,14 +94,27 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.7.0] - 2023-04-14
+--------------------
+
+Added
+~~~~~
+
+* Add ``edx_drf_extensions_version`` to help with rollout of changes in this library across services.
+
+Removed
+~~~~~~~
+
+* Removed exception case for ``InvalidTokenError`` that was never invoked.
+
 [8.6.0] - 2023-04-12
 --------------------
 
 Added
 ~~~~~
 
 * Added ``jwt_auth_check_symmetric_key``, ``jwt_auth_asymmetric_verified``, ``jwt_auth_symmetric_verified``, and ``jwt_auth_verification_failed`` custom attributes to aid in deprecation and removal of symmetric keys.
@@ -243,15 +256,15 @@
 
 * Added a new custom attribute `request_is_staff_or_superuser`
 
 [6.3.0] - 2021-01-12
 --------------------
 
 Removed
-~~~~~~~~
+~~~~~~~
 
 * Drop support for Python 3.5
 
 [6.2.0] - 2020-08-24
 --------------------
 
 Updated
```

### Comparing `edx-drf-extensions-8.6.0/README.rst` & `edx-drf-extensions-8.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/csrf/api/v1/views.py` & `edx-drf-extensions-8.7.0/csrf/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/csrf/tests/test_api.py` & `edx-drf-extensions-8.7.0/csrf/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/docs/conf.py` & `edx-drf-extensions-8.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/PKG-INFO` & `edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-drf-extensions
-Version: 8.6.0
+Version: 8.7.0
 Summary: edX extensions of Django REST Framework
 Home-page: https://github.com/openedx/edx-drf-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -94,14 +94,27 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.7.0] - 2023-04-14
+--------------------
+
+Added
+~~~~~
+
+* Add ``edx_drf_extensions_version`` to help with rollout of changes in this library across services.
+
+Removed
+~~~~~~~
+
+* Removed exception case for ``InvalidTokenError`` that was never invoked.
+
 [8.6.0] - 2023-04-12
 --------------------
 
 Added
 ~~~~~
 
 * Added ``jwt_auth_check_symmetric_key``, ``jwt_auth_asymmetric_verified``, ``jwt_auth_symmetric_verified``, and ``jwt_auth_verification_failed`` custom attributes to aid in deprecation and removal of symmetric keys.
@@ -243,15 +256,15 @@
 
 * Added a new custom attribute `request_is_staff_or_superuser`
 
 [6.3.0] - 2021-01-12
 --------------------
 
 Removed
-~~~~~~~~
+~~~~~~~
 
 * Drop support for Python 3.5
 
 [6.2.0] - 2020-08-24
 --------------------
 
 Updated
```

### Comparing `edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/SOURCES.txt` & `edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/authentication.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/authentication.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ JWT Authentication class. """
 
 import logging
 
-import jwt
 from django.contrib.auth import get_user_model
 from django.middleware.csrf import CsrfViewMiddleware
 from edx_django_utils.monitoring import set_custom_attribute
 from rest_framework import exceptions
 from rest_framework_jwt.authentication import JSONWebTokenAuthentication
 
 from edx_rest_framework_extensions.auth.jwt.constants import USE_JWT_COOKIE_HEADER
@@ -73,18 +72,14 @@
                 return user_and_auth
 
             self.enforce_csrf(request)
 
             # CSRF passed validation with authenticated user
             return user_and_auth
 
-        except jwt.InvalidTokenError as token_error:
-            # Note: I think this case is not used, but will monitor the custom attribute to verify.
-            set_custom_attribute('jwt_auth_failed', 'InvalidTokenError:{}'.format(repr(token_error)))
-            raise exceptions.AuthenticationFailed() from token_error
         except Exception as exception:
             # Errors in production do not need to be logged (as they may be noisy),
             # but debug logging can help quickly resolve issues during development.
             logger.debug('Failed JWT Authentication,', exc_info=exception)
             # Note: I think this case should only include AuthenticationFailed and PermissionDenied,
             #   but will monitor the custom attribute to verify.
             set_custom_attribute('jwt_auth_failed', 'Exception:{}'.format(repr(exception)))
```

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/cookies.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/decoder.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,29 +254,30 @@
     as the signature is actually checked in a different function.
     """
     options = {
         'require': ["exp", "iat"],
 
         'verify_exp': api_settings.JWT_VERIFY_EXPIRATION,
         'verify_aud': settings.JWT_AUTH.get('JWT_VERIFY_AUDIENCE', True),
-        'verify_iss': False,  # TODO (ARCH-204): manually verify until issuer is configured correctly.
+        # See https://github.com/openedx/edx-drf-extensions/issues/327 for removing manual issuer verification.
+        'verify_iss': False,  # Verified manually below
         'verify_signature': False,  # Verified with JWS already
     }
 
     decoded_token = jwt.decode(
         token,
         jwt_issuer['SECRET_KEY'],
         options=options,
         leeway=api_settings.JWT_LEEWAY,
         audience=jwt_issuer['AUDIENCE'],
         issuer=jwt_issuer['ISSUER'],
         algorithms=[api_settings.JWT_ALGORITHM],
     )
 
-    # TODO (ARCH-204): verify issuer manually until it is properly configured.
+    # See https://github.com/openedx/edx-drf-extensions/issues/327 for removing this manual issuer validation.
     token_issuer = decoded_token.get('iss')
     # .. custom_attribute_name: jwt_auth_issuer
     # .. custom_attribute_description: Value set to the JWT auth issuer.
     set_custom_attribute('jwt_auth_issuer', token_issuer)
     issuer_matched = any(issuer['ISSUER'] == token_issuer for issuer in get_jwt_issuers())
     if token_issuer == jwt_issuer['ISSUER']:
         # .. custom_attribute_name: jwt_auth_issuer_verification
```

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/middleware.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         views = {
             "class_view": SomeClassView,
             "view_set": SomeClassViewSet.as_view({'get': 'list'}),
             "function_view": some_function_view
         }
         view_classes = {
             "class_view": SomeClassView,
-            "view_set": views['view_set'].cls,  # pylint: disable=no-member
+            "view_set": views['view_set'].cls,
             "function_view": views['function_view'].view_class,
         }
         view = views[view_type]
         view_class = view_classes[view_type]
 
         # verify pre-conditions
         self._assert_included(
```

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/authentication.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/config.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/config.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/middleware.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import warnings
 
 from django.utils.deprecation import MiddlewareMixin
 from edx_django_utils import monitoring
 from edx_django_utils.cache import DEFAULT_REQUEST_CACHE
 
+import edx_rest_framework_extensions
 from edx_rest_framework_extensions.auth.jwt.constants import USE_JWT_COOKIE_HEADER
 from edx_rest_framework_extensions.auth.jwt.cookies import jwt_cookie_name
 
 
 class RequestCustomAttributesMiddleware(MiddlewareMixin):
     """
     Adds various request related custom attributes.
@@ -68,14 +69,21 @@
         self._cache_if_authenticated_user_found_in_middleware(request, 'process_exception')
         self._set_all_request_attributes(request)
 
     def _set_all_request_attributes(self, request):
         """
         Sets all the request custom attributes
         """
+        # .. custom_attribute_name: edx_drf_extensions_version
+        # .. custom_attribute_description: The version of the edx-drf-extensions library installed, which may be
+        #   useful when trying to rollout important changes to all services. Note that RequestCustomAttributesMiddleware
+        #   must be installed for this to work. Also, versions before 8.7.0 will not include this attribute, but
+        #   should have ``request_auth_type_guess``.
+        monitoring.set_custom_attribute('edx_drf_extensions_version', edx_rest_framework_extensions.__version__)
+
         self._set_request_auth_type_guess_attribute(request)
         self._set_request_user_agent_attributes(request)
         self._set_request_referer_attribute(request)
         self._set_request_user_id_attribute(request)
         self._set_request_authenticated_user_found_in_middleware_attribute()
         self._set_request_is_staff_or_superuser(request)
```

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/paginators.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/permissions.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/settings.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_middleware.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Unit tests for middlewares.
 """
+import re
 from unittest.mock import call, patch
 
 import ddt
 from django.contrib.auth.models import AnonymousUser
 from django.test import RequestFactory, TestCase
 from edx_django_utils.cache import RequestCache
 
@@ -22,34 +23,46 @@
     def setUp(self):
         super().setUp()
         RequestCache.clear_all_namespaces()
         self.request = RequestFactory().get('/')
         self.middleware = RequestCustomAttributesMiddleware()  # pylint: disable=no-value-for-parameter
 
     @patch('edx_django_utils.monitoring.set_custom_attribute')
+    def test_edx_drf_extensions_version_attribute(self, mock_set_custom_attribute):
+        self.request.user = AnonymousUser()
+
+        self.middleware.process_response(self.request, None)
+        # if call_args_list contains call('edx_drf_extensions_version', '8.7.0'), then version_list = ['8.7.0']
+        version_list = [
+            x.args[1] for x in mock_set_custom_attribute.call_args_list if x.args[0] == 'edx_drf_extensions_version'
+        ]
+        assert len(version_list) == 1
+        assert re.search(r'\d+\.\d+\.\d+', version_list[0])
+
+    @patch('edx_django_utils.monitoring.set_custom_attribute')
     def test_request_auth_type_guess_anonymous_attribute(self, mock_set_custom_attribute):
         self.request.user = AnonymousUser()
 
         self.middleware.process_response(self.request, None)
-        mock_set_custom_attribute.assert_called_once_with('request_auth_type_guess', 'unauthenticated')
+        mock_set_custom_attribute.assert_called_with('request_auth_type_guess', 'unauthenticated')
 
     @patch('edx_django_utils.monitoring.set_custom_attribute')
     def test_request_no_headers(self, mock_set_custom_attribute):
         self.request.user = None
         self.middleware.process_response(self.request, None)
-        mock_set_custom_attribute.assert_called_once_with('request_auth_type_guess', 'no-user')
+        mock_set_custom_attribute.assert_called_with('request_auth_type_guess', 'no-user')
 
     @patch('edx_django_utils.monitoring.set_custom_attribute')
     def test_request_blank_headers(self, mock_set_custom_attribute):
         self.request.META['HTTP_USER_AGENT'] = ''
         self.request.META['HTTP_REFERER'] = ''
         self.request.META['HTTP_AUTHORIZATION'] = ''
 
         self.middleware.process_response(self.request, None)
-        mock_set_custom_attribute.assert_called_once_with('request_auth_type_guess', 'no-user')
+        mock_set_custom_attribute.assert_called_with('request_auth_type_guess', 'no-user')
 
     @patch('edx_django_utils.monitoring.set_custom_attribute')
     def test_request_referer_attribute(self, mock_set_custom_attribute):
         self.request.META['HTTP_REFERER'] = 'test-http-referer'
 
         self.middleware.process_response(self.request, None)
         expected_calls = [
@@ -220,8 +233,8 @@
         self.middleware = RequestMetricsMiddleware()
 
     @patch('edx_django_utils.monitoring.set_custom_attribute')
     def test_request_auth_type_guess_anonymous_attribute(self, mock_set_custom_attribute):
         self.request.user = AnonymousUser()
 
         self.middleware.process_response(self.request, None)
-        mock_set_custom_attribute.assert_called_once_with('request_auth_type_guess', 'unauthenticated')
+        mock_set_custom_attribute.assert_called_with('request_auth_type_guess', 'unauthenticated')
```

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_paginators.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_permissions.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_settings.py` & `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/requirements/constraints.txt` & `edx-drf-extensions-8.7.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.6.0/setup.py` & `edx-drf-extensions-8.7.0/setup.py`

 * *Files identical despite different names*

