# Comparing `tmp/st_common_data-0.2.6.0.tar.gz` & `tmp/st_common_data-0.2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_common_data-0.2.6.0.tar", last modified: Tue Apr 11 10:32:17 2023, max compression
+gzip compressed data, was "st_common_data-0.2.6.1.tar", last modified: Tue Apr 18 06:55:35 2023, max compression
```

## Comparing `st_common_data-0.2.6.0.tar` & `st_common_data-0.2.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.6.0/LICENCE
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.6.0/README.md
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.6.0/pyproject.toml
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/setup.cfg
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.645300 st_common_data-0.2.6.0/st_common_data/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/auth/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/auth/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.6.0/st_common_data/auth/apps.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     9562 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/auth/django_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10010 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/auth/fastapi_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/auth/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/auth/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.6.0/st_common_data/auth/views.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    30488 2023-02-16 13:38:13.000000 st_common_data-0.2.6.0/st_common_data/datum.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.6.0/st_common_data/nyse_holidays.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/pagination.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/trading_accounts/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0001_initial.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/models.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/views.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/utils/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.6.0/st_common_data/utils/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.6.0/st_common_data/utils/common.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.645300 st_common_data-0.2.6.0/st_common_data.egg-info/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/SOURCES.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/dependency_links.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/top_level.txt
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.6.1/LICENCE
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.6.1/README.md
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.6.1/pyproject.toml
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/setup.cfg
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-04-18 06:51:07.000000 st_common_data-0.2.6.1/st_common_data/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/auth/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.6.1/st_common_data/auth/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.6.1/st_common_data/auth/apps.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     9561 2023-04-18 06:48:02.000000 st_common_data-0.2.6.1/st_common_data/auth/django_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.6.1/st_common_data/auth/fastapi_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/auth/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/auth/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.6.1/st_common_data/auth/views.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    30488 2023-02-16 13:38:13.000000 st_common_data-0.2.6.1/st_common_data/datum.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.6.1/st_common_data/nyse_holidays.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/pagination.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/trading_accounts/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0001_initial.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/models.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/views.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/utils/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.6.1/st_common_data/utils/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.6.1/st_common_data/utils/common.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data.egg-info/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/top_level.txt
```

### Comparing `st_common_data-0.2.6.0/LICENCE` & `st_common_data-0.2.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/PKG-INFO` & `st_common_data-0.2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.6.0
+Version: 0.2.6.1
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.6.0/README.md` & `st_common_data-0.2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/setup.cfg` & `st_common_data-0.2.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/auth/django_auth.py` & `st_common_data-0.2.6.1/st_common_data/auth/django_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,19 +259,19 @@
                 audience=settings.AUTH0_API_AUDIENCE,
                 grant_type='client_credentials',
                 client_id=settings.AUTH0_SERVICE_CLIENT_ID,
                 client_secret=settings.AUTH0_SERVICE_CLIENT_SECRET,
                 services_token_url=settings.AUTH0_SERVICE_TOKEN_URL)
         elif token_filename == MANAGEMENT_TOKEN_FILENAME:
             obj_to_set = ManagementAuth0Token(
-                audience=f'https://{settings.AUTH0_DOMAIN}/api/v2/',
+                audience=settings.AUTH0_MANAGEMENT_API_AUDIENCE,
                 grant_type='client_credentials',
                 client_id=settings.AUTH0_MANAGEMENT_CLIENT_ID,
                 client_secret=settings.AUTH0_MANAGEMENT_CLIENT_SECRET,
-                services_token_url=settings.AUTH0_SERVICE_TOKEN_URL
+                services_token_url=settings.AUTH0_MANAGEMENT_TOKEN_URL
             )
 
     obj_to_set.token  # Important! In order to set token before saving into file
 
     with open(token_filename, 'wb') as wb_handle:
         pickle.dump(obj_to_set, wb_handle, protocol=pickle.HIGHEST_PROTOCOL)
```

### Comparing `st_common_data-0.2.6.0/st_common_data/auth/fastapi_auth.py` & `st_common_data-0.2.6.1/st_common_data/auth/fastapi_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,19 +269,19 @@
                 audience=config.auth0_oa_api_audience,
                 grant_type='client_credentials',
                 client_id=config.auth0_service_client_id,
                 client_secret=config.auth0_service_client_secret,
                 services_token_url=config.auth0_service_token_url)
         elif token_filename == MANAGEMENT_TOKEN_FILENAME:
             obj_to_set = ManagementAuth0Token(
-                audience=f'https://{config.auth0_domain}/api/v2/',
+                audience=config.auth0_management_api_audience,
                 grant_type='client_credentials',
                 client_id=config.auth0_management_client_id,
                 client_secret=config.auth0_management_client_secret,
-                services_token_url=config.auth0_service_token_url)
+                services_token_url=config.auth0_management_token_url)
 
     obj_to_set.token  # Important! In order to set token before saving into file
 
     with open(token_filename, 'wb') as wb_handle:
         pickle.dump(obj_to_set, wb_handle, protocol=pickle.HIGHEST_PROTOCOL)
```

### Comparing `st_common_data-0.2.6.0/st_common_data/auth/views.py` & `st_common_data-0.2.6.1/st_common_data/auth/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/datum.py` & `st_common_data-0.2.6.1/st_common_data/datum.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/nyse_holidays.py` & `st_common_data-0.2.6.1/st_common_data/nyse_holidays.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0001_initial.py` & `st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py` & `st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/trading_accounts/models.py` & `st_common_data-0.2.6.1/st_common_data/trading_accounts/models.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/trading_accounts/views.py` & `st_common_data-0.2.6.1/st_common_data/trading_accounts/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data/utils/common.py` & `st_common_data-0.2.6.1/st_common_data/utils/common.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.0/st_common_data.egg-info/PKG-INFO` & `st_common_data-0.2.6.1/st_common_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-common-data
-Version: 0.2.6.0
+Version: 0.2.6.1
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.6.0/st_common_data.egg-info/SOURCES.txt` & `st_common_data-0.2.6.1/st_common_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

