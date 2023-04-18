# Comparing `tmp/zoho_analytics_connector-1.3.6.tar.gz` & `tmp/zoho_analytics_connector-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho_analytics_connector-1.3.6.tar", last modified: Wed Aug  3 03:12:29 2022, max compression
+gzip compressed data, was "zoho_analytics_connector-1.4.1.tar", last modified: Tue Apr 18 12:05:14 2023, max compression
```

## Comparing `zoho_analytics_connector-1.3.6.tar` & `zoho_analytics_connector-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-08-03 03:12:29.573591 zoho_analytics_connector-1.3.6/
--rw-rw-r--   0 tim       (1000) tim       (1000)      217 2022-07-14 03:04:02.000000 zoho_analytics_connector-1.3.6/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)    14347 2022-08-03 03:12:29.573591 zoho_analytics_connector-1.3.6/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)    13574 2022-08-03 03:12:02.000000 zoho_analytics_connector-1.3.6/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2022-08-03 03:12:29.573591 zoho_analytics_connector-1.3.6/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     1697 2022-08-03 03:10:14.000000 zoho_analytics_connector-1.3.6/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-08-03 03:12:29.573591 zoho_analytics_connector-1.3.6/zoho_analytics_connector/
--rw-rw-r--   0 tim       (1000) tim       (1000)     8874 2022-08-03 01:23:38.000000 zoho_analytics_connector-1.3.6/zoho_analytics_connector/enhanced_report_client.py
--rw-rw-r--   0 tim       (1000) tim       (1000)   109566 2022-07-14 06:42:08.000000 zoho_analytics_connector-1.3.6/zoho_analytics_connector/report_client.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-08-03 03:12:29.573591 zoho_analytics_connector-1.3.6/zoho_analytics_connector.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)    14347 2022-08-03 03:12:29.000000 zoho_analytics_connector-1.3.6/zoho_analytics_connector.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      358 2022-08-03 03:12:29.000000 zoho_analytics_connector-1.3.6/zoho_analytics_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-08-03 03:12:29.000000 zoho_analytics_connector-1.3.6/zoho_analytics_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       15 2022-08-03 03:12:29.000000 zoho_analytics_connector-1.3.6/zoho_analytics_connector.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       25 2022-08-03 03:12:29.000000 zoho_analytics_connector-1.3.6/zoho_analytics_connector.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      217 2022-07-14 03:04:02.000000 zoho_analytics_connector-1.4.1/LICENSE
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14323 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13499 2023-04-18 12:04:14.000000 zoho_analytics_connector-1.4.1/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1747 2023-04-18 12:04:14.000000 zoho_analytics_connector-1.4.1/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/zoho_analytics_connector/
+-rw-rw-r--   0 tim       (1000) tim       (1000)   100603 2022-11-23 02:51:47.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector/analytics_client_upstream.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9920 2023-04-18 12:02:16.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector/enhanced_report_client.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)   113880 2023-03-14 04:40:03.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector/report_client.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14323 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      412 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       15 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       25 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/top_level.txt
```

### Comparing `zoho_analytics_connector-1.3.6/PKG-INFO` & `zoho_analytics_connector-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,17 @@
-Metadata-Version: 2.1
-Name: zoho_analytics_connector
-Version: 1.3.6
-Summary: Zoho Analytics connector
-Home-page: https://github.com/timrichardson/zoho_analytics_connector
-Author: Tim Richardson
-Author-email: tim@growthpath.com.au
-License: MPL-2.0
-Keywords: zoho analytics
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Office/Business
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Zoho Analytics Connector for Python
 ========================
 
 Zoho's Python SDK for Zoho Reports is old, however it is very complete.
 This is a version which is Python 3 ready, tested on Python 3.8 and 3.9 and in fairly substantial production use.
 
 A more convenient wrapper class is in enhanced_report_client. This is based on Zoho's ReportClient but provides some more convenient features.
 I use it mostly for uploading data, and creating and modifying tables.
 
-This library uses the Analytics V1 API.
+This library uses the Analytics V1 API and as of v.1.4 will phase in v2 API endpoints bit by bit
 
 Authentication
 ==============
 AuthTokens are now retired, replaced with OAuth2.
 
 OAuth2 notes are below.
 When you create EnhancedZohoAnalyticsClient or ReportClient, you need to pass ClientID, ClientSecret and a RefreshToken.
@@ -118,20 +96,18 @@
 NOTE!!! For Australian-hosted Zoho accounts and other regional variations:
 
 The token URL is adapted for the server location. e.g. for Australia, post to https://accounts.zoho.com.au/oauth/v2/token
 
 Usage
 =====
 
-Zoho's full API is available through the ReportClient API. However, there are bugs in this code.
-Recent 2020 changes have fixed some of these bugs, but I have hardly any test cases; I only have test cases
-for a handful of the standard functions of ReportClient. So proceed carefully if you use them.
+Zoho's full API v1 is available through the ReportClient API. 
+Selectively, v2 API endpoints will be added to the ReportClient if they are useful. 
 
-They are probably worth looking at. For instance, ReportClient.exportData now actually does use the file object you pass.
-But perhaps due to its python2 heritage, it expects a binary file object.
+One example of this is get_metadata_api_v2()
 
 Note that for data import and export, my EnhancedReportClient has its own methods, and these are what I use in production so they are much better tested.
 
 
     class EnhancedZohoAnalyticsClient(ReportClient)
     
 is a higher level layer.
@@ -301,14 +277,17 @@
 
 
 Changes
 -------------
 
 next_version Test updates
 
+1.4.1 Something seems to changed with the UTF encoding returned by the export endpoint. Change decoding to use utf-8-sig 
+1.4.0 some adaptation towards new API from Zoho
+
 1.3.6 Documentation updates, test updates. Added a 'pre-delete function' to calculate how many rows should be deleted.
     deleteData returns an int not a string for the number of rows deleted.
 
 1.3.3 - 1.3.5 Handle some more Zoho exceptions
 
 1.3.2 Under heavy concurrent load, an oauth token error was not being caught. Fixed; new token is generated and a retry occurs.
 
@@ -336,9 +315,7 @@
 1.1.0 Treat "another import is in progress" as a recoverable error (can be retried)
     Move home-made retry logic to low level: report_client.__sendRequest(), and make retry optionally available to the key functions in EnhancedZohoAnalyticsClient. 
     Functions can pass retry_countdown to use retry. The retry handling is coping well under some initial use in high volume production loads.
 
 1.0.4 Documentation improvements
 
 1.0.3 Some slightly better error handling if Zoho returns an empty response
-
-
```

### Comparing `zoho_analytics_connector-1.3.6/README.md` & `zoho_analytics_connector-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,40 @@
+Metadata-Version: 2.1
+Name: zoho_analytics_connector
+Version: 1.4.1
+Summary: Zoho Analytics connector
+Home-page: https://github.com/timrichardson/zoho_analytics_connector
+Author: Tim Richardson
+Author-email: tim@growthpath.com.au
+License: MPL-2.0
+Keywords: zoho analytics
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Office/Business
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Zoho Analytics Connector for Python
 ========================
 
 Zoho's Python SDK for Zoho Reports is old, however it is very complete.
 This is a version which is Python 3 ready, tested on Python 3.8 and 3.9 and in fairly substantial production use.
 
 A more convenient wrapper class is in enhanced_report_client. This is based on Zoho's ReportClient but provides some more convenient features.
 I use it mostly for uploading data, and creating and modifying tables.
 
-This library uses the Analytics V1 API.
+This library uses the Analytics V1 API and as of v.1.4 will phase in v2 API endpoints bit by bit
 
 Authentication
 ==============
 AuthTokens are now retired, replaced with OAuth2.
 
 OAuth2 notes are below.
 When you create EnhancedZohoAnalyticsClient or ReportClient, you need to pass ClientID, ClientSecret and a RefreshToken.
@@ -96,20 +119,18 @@
 NOTE!!! For Australian-hosted Zoho accounts and other regional variations:
 
 The token URL is adapted for the server location. e.g. for Australia, post to https://accounts.zoho.com.au/oauth/v2/token
 
 Usage
 =====
 
-Zoho's full API is available through the ReportClient API. However, there are bugs in this code.
-Recent 2020 changes have fixed some of these bugs, but I have hardly any test cases; I only have test cases
-for a handful of the standard functions of ReportClient. So proceed carefully if you use them.
+Zoho's full API v1 is available through the ReportClient API. 
+Selectively, v2 API endpoints will be added to the ReportClient if they are useful. 
 
-They are probably worth looking at. For instance, ReportClient.exportData now actually does use the file object you pass.
-But perhaps due to its python2 heritage, it expects a binary file object.
+One example of this is get_metadata_api_v2()
 
 Note that for data import and export, my EnhancedReportClient has its own methods, and these are what I use in production so they are much better tested.
 
 
     class EnhancedZohoAnalyticsClient(ReportClient)
     
 is a higher level layer.
@@ -279,14 +300,17 @@
 
 
 Changes
 -------------
 
 next_version Test updates
 
+1.4.1 Something seems to changed with the UTF encoding returned by the export endpoint. Change decoding to use utf-8-sig 
+1.4.0 some adaptation towards new API from Zoho
+
 1.3.6 Documentation updates, test updates. Added a 'pre-delete function' to calculate how many rows should be deleted.
     deleteData returns an int not a string for the number of rows deleted.
 
 1.3.3 - 1.3.5 Handle some more Zoho exceptions
 
 1.3.2 Under heavy concurrent load, an oauth token error was not being caught. Fixed; new token is generated and a retry occurs.
 
@@ -314,7 +338,9 @@
 1.1.0 Treat "another import is in progress" as a recoverable error (can be retried)
     Move home-made retry logic to low level: report_client.__sendRequest(), and make retry optionally available to the key functions in EnhancedZohoAnalyticsClient. 
     Functions can pass retry_countdown to use retry. The retry handling is coping well under some initial use in high volume production loads.
 
 1.0.4 Documentation improvements
 
 1.0.3 Some slightly better error handling if Zoho returns an empty response
+
+
```

### Comparing `zoho_analytics_connector-1.3.6/setup.py` & `zoho_analytics_connector-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 cmdclass = {'build_sphinx': BuildDoc}
 
 # https://pypi.org/classifiers/
 
 name = 'zoho_analytics_connector'
 keywords = 'zoho analytics'
-version = '1.3.6'
+version = '1.4.1'
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=name,
     keywords=keywords,
@@ -25,14 +25,15 @@
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Office/Business',
     ],
     url='https://github.com/timrichardson/zoho_analytics_connector',
     license='MPL-2.0',
     author='Tim Richardson',
     author_email='tim@growthpath.com.au',
     description='Zoho Analytics connector',
```

### Comparing `zoho_analytics_connector-1.3.6/zoho_analytics_connector/enhanced_report_client.py` & `zoho_analytics_connector-1.4.1/zoho_analytics_connector/enhanced_report_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 
 import csv
 import json
 import logging
 import time
-from typing import MutableMapping, Optional
+from typing import MutableMapping, Optional, List
 
 import emoji
 
 from . import report_client as report_client
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -51,17 +51,20 @@
                         col_data[col['columnName'].lower()] = col
                     else:
                         col_data[col['columnName']] = col
 
         return table_data
 
     def __init__(self, login_email_id: str, token: str, default_databasename: str = None, clientId=None,
-                 clientSecret=None, serverURL=None, reportServerURL=None, default_retries=None):
+                 clientSecret=None, serverURL=None, reportServerURL=None, default_retries=None,
+                 error_email_list: Optional[List[str]]=None):
+        """ error email list is not used by the client, but it is available for callers as a convenience"""
         self.login_email_id = login_email_id
         self.default_databasename = default_databasename
+        self.error_email_list = error_email_list or [login_email_id]
         super().__init__(token=token, clientId=clientId, clientSecret=clientSecret, serverURL=serverURL,
                          reportServerURL=reportServerURL, default_retries=default_retries)
 
     def get_database_catalog(self, database_name: str = None) -> MutableMapping:
         db_uri = self.getDBURI(self.login_email_id, database_name or self.default_databasename)
         catalog_info = self.getDatabaseMetadata(requestURI=db_uri, metadata="ZOHO_CATALOG_INFO")
         return catalog_info
@@ -115,15 +118,16 @@
                     date_format=None) -> Optional[report_client.ImportResult]:
         """ data is a csv-style string, newline separated. Matching columns is a comma separated string
         import_mode is one of TRUNCATEADD, APPEND, UPDATEADD
         """
         retry_count = 0
         retry_limit = retry_limit or self.default_retries
         impResult = None
-        import_content_demojized = emoji.demojize(import_content)
+        # import_content_demojized = emoji.demojize(import_content)
+        import_content_demojized = import_content #try without this, move data cleaning to the calling function
         database_name = database_name or self.default_databasename
         uri = self.getURI(dbOwnerName=self.login_email_id, dbName=database_name, tableOrReportName=table_name)
         # import_modes = APPEND / TRUNCATEADD / UPDATEADD
         impResult = self.importData_v2(uri, import_mode=import_mode, import_content=import_content_demojized,
                                        date_format=date_format,
                                        matching_columns=matching_columns, retry_countdown=retry_limit)
 
@@ -142,22 +146,22 @@
             returned_data = None
         if not returned_data:
             database_name = database_name or self.default_databasename
             uri = self.getURI(dbOwnerName=self.login_email_id, dbName=database_name or self.default_databasename,
                               tableOrReportName=table_name)
             callback_data = self.exportDataUsingSQL_v2(tableOrReportURI=uri, format='CSV', sql=sql,
                                                        retry_countdown=retry_countdown)
-            returned_data = callback_data.getvalue().decode('utf-8').splitlines()
+            returned_data = callback_data.getvalue().decode('utf-8-sig').splitlines()
             if cache_object:
                 cache_object.set(sql, returned_data, cache_timeout_seconds)
 
         reader = csv.DictReader(returned_data)
         return reader
 
-    def delete_rows(self, table_name, sql, database_name: Optional[str] = None, retry_countdown=5)->int:
+    def delete_rows(self, table_name, sql, database_name: Optional[str] = None, retry_countdown=5) -> int:
         """ criteria is SQL fragments such as 'a' in ColA, for example,
         sql = f"{id_column} IN ('ce76dc3a-bac0-47dd-841a-70e66613958e')
         return the count of eows
         """
 
         if len(sql) > 5000:
             raise RuntimeError("The SQL passed to delete_rows is too big and will cause Zoho 400 errors")
@@ -171,11 +175,22 @@
         Zoho sometimes gets table corruption which means rows don't delete.
         When the operation is critical, you can use this function to check the nbr of rows deleted is correct.
         """
 
         if len(sql) > 5000:
             raise RuntimeError("The SQL passed to delete_rows is too big and will cause Zoho 400 errors")
         sql = f"select count(*) from {table_name} where {sql}"
-        reader = self.data_export_using_sql(sql,table_name=table_name)
+        reader = self.data_export_using_sql(sql, table_name=table_name)
         result = list(reader)[0]
-        row_count = int(result['count(*)'])
-        return row_count
+        try:
+            row_count = int(result['count(*)'])
+        except KeyError:
+            raise RuntimeError(f"Zoho returned unexpected data, did not found (count(8)) in the result: {result}")
+        return row_count
+
+    def rename_column(self, table_name, old_column_name, new_column_name, database_name: Optional[str] = None,
+                      retry_countdown=5):
+        """ rename a column in a table """
+        uri = self.getURI(dbOwnerName=self.login_email_id, dbName=database_name or self.default_databasename,
+                          tableOrReportName=table_name)
+        self.renameColumn(tableURI=uri, oldColumnName=old_column_name, newColumnName=new_column_name,
+                          retry_countdown=retry_countdown)
```

### Comparing `zoho_analytics_connector-1.3.6/zoho_analytics_connector/report_client.py` & `zoho_analytics_connector-1.4.1/zoho_analytics_connector/report_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,45 +120,66 @@
             resp = respObj.response.json()
             if ("access_token" in resp):
                 self.__token = resp['access_token']
                 return resp["access_token"]
             else:
                 raise ValueError("Error while getting OAuth token ", resp)
 
-    def getResp(self, url: str, httpMethod: str, payLoad,add_token=True):
+    def getResp(self, url: str, httpMethod: str, payLoad,add_token=True,extra_headers=None,**kwargs):
         """
-        Internal method.
+        Internal method. for GET, payLoad is params
         """
         requests_session = self.requests_session or requests_retry_session()
         if httpMethod.upper() == 'POST':
             headers = {}
             if add_token and ReportClient.isOAuth and hasattr(self,'token'): #check for token because this can be called during __init__ and isOAuth could be true.
                 headers["Authorization"] = "Zoho-oauthtoken " + self.token
             headers['User-Agent'] = "ZohoAnalytics Python GrowthPath Library"
+            if extra_headers:
+                headers = {**headers, **extra_headers}
             try:
-                resp = requests_session.post(url, data=payLoad, headers=headers, timeout=self.request_timeout)
+                resp = requests_session.post(url, data=payLoad, headers=headers, timeout=self.request_timeout,**kwargs)
                 if 'invalid client' in resp.text:
                     raise requests.exceptions.RequestException("Invalid Client")
                 respObj = ResponseObj(resp)
             except requests.exceptions.RequestException as e:
                logger.exception(f"{e=}")
                raise e
             return respObj
+        elif httpMethod.upper() == 'GET':
+            headers = {}
+            if add_token and ReportClient.isOAuth and hasattr(self,
+                                                              'token'):  # check for token because this can be called during __init__ and isOAuth could be true.
+                headers["Authorization"] = "Zoho-oauthtoken " + self.token
+            headers['User-Agent'] = "ZohoAnalytics Python GrowthPath Library"
+            if extra_headers:
+                headers = {**headers, **extra_headers}
+            try:
+                resp = requests_session.get(url, params=payLoad, headers=headers, timeout=self.request_timeout,**kwargs)
+                if 'invalid client' in resp.text:
+                    raise requests.exceptions.RequestException("Invalid Client")
+                respObj = ResponseObj(resp)
+            except requests.exceptions.RequestException as e:
+                logger.exception(f"{e=}")
+                raise e
+            return respObj
+
+
         else:
-            raise RuntimeError(f"Unexpected httpMethod in getResp, was expecting POST but got {httpMethod}")
+            raise RuntimeError(f"Unexpected httpMethod in getResp, was expecting POST or GET but got {httpMethod}")
 
-    def __sendRequest(self, url, httpMethod, payLoad, action, callBackData,retry_countdown:int=None):
+    def __sendRequest(self, url, httpMethod, payLoad, action, callBackData=None,retry_countdown:int=None, extra_headers=None,**keywords):
         code = ""
         if not retry_countdown:
             retry_countdown = self.default_retries or 1
         init_retry_countdown = retry_countdown
         while retry_countdown > 0:
             retry_countdown -= 1
             try:
-                respObj = self.getResp(url, httpMethod, payLoad)
+                respObj = self.getResp(url, httpMethod, payLoad, extra_headers=extra_headers,**keywords)
             except Exception as e:
                 logger.exception(f" getResp exception in __sendRequest, {retry_countdown}, {e}")  #connection error
                 if retry_countdown <= 0:
                     raise e
                 else:
                     time.sleep(min(10 - retry_countdown, 1) * 10)
                     continue
@@ -183,15 +204,15 @@
                             code = -1
                             logger.error(f"could not find error code in {respObj.response.text} ")
                             time.sleep(min(10 - retry_countdown, 1) * 10)
                             continue
 
                     logger.debug(f"API returned a 400 result and an error code: {code} ")
                     if code in [6045,]:
-                        logger.error(f"Zoho API Recoverable rate limit (rate limit exceeded) ")
+                        logger.error(f"Zoho API Recoverable rate limit (rate limit exceeded); there are {retry_countdown+1} retries left")
                         if retry_countdown < 0:
                             logger.error(
                                     f"Zoho API Recoverable error (rate limit exceeded), but exhausted retries")
                             raise UnrecoverableRateLimitError(urlResp=respObj,zoho_error_code=code)
                         else:
                             time.sleep(min(10-retry_countdown,1)*10)
                             continue
@@ -203,14 +224,18 @@
                         logger.error(
                             f"6043 error, daily API limit in Zoho plan exceeded {respObj.response.text}")
                         raise UnrecoverableRateLimitError(urlResp=respObj, zoho_error_code=code)
                     elif code in [7103, ]:
                         logger.error(
                             f"7103 error, workspace not found (check authentication) {respObj.response.text}")
                         raise ServerError(urlResp=respObj, zoho_error_code=code)
+                    elif code in [7179, ]:
+                       logger.error(
+                           f"7179 error, workspace reports no view present. Initialise with a dummy table {respObj.response.text}")
+                       raise ServerError(urlResp=respObj, zoho_error_code=code)
                     elif code in [7232, ]:
                         logger.error(
                             f"7232 error,an invalid value has been provided according to the column's data type) {respObj.response.text=} ")
                         raise ServerError(urlResp=respObj, zoho_error_code=code)
                     elif code in [7280, ]:
                         logger.error(f"7280 error, relating to schema errors, return immediately {respObj.response.text}")
                         raise ServerError(urlResp=respObj, zoho_error_code=code)
@@ -237,15 +262,15 @@
                         logger.error(f"Error 8509 encountered, something is wrong with the data format, no retry is attempted")
                         raise BadDataError(respObj,zoho_error_code=code)
                     elif code in [10001,]:  #10001 is "Another import is in progress, so we can try this again"
                         logger.error(f"Zoho API Recoverable error encountered (Another import is in progress), will retry")
                         if retry_countdown < 0:
                             logger.error(
                             f"Zoho API Recoverable error (Another import is in progress) but exhausted retries")
-                            raise UnrecoverableRateLimitError(urlResp=respObj,zoho_error_code=code)
+                            raise UnrecoverableRateLimitError(urlResp=respObj,zoho_error_code=code, message="Zoho error: Another import is in progress")
                         else:
                             time.sleep(min(10 - retry_countdown, 1) * 10)
                             continue
 
                     else:
                         #raise ServerError(respObj,zoho_error_code=code)
                         msg = f"Unexpected status code {code=}, will attempt retry"
@@ -256,15 +281,15 @@
                         logger.exception(msg)
                         time.sleep(min(10 - retry_countdown, 1) * 10)
                         continue
                 except (RecoverableRateLimitError,UnrecoverableRateLimitError,BadDataError):
                     raise
                 except ServerError as e:
                     logger.error(f"ServerError raised on _sendRequest.  {url=} {payLoad=} {action=} ")
-                    import_data = payLoad.get("ZOHO_IMPORT_DATA")
+                    import_data = payLoad.get("ZOHO_IMPORT_DATA") if payLoad else None
                     if import_data:
                         logger.error(f"Import data, a csv file as a string. Row 1 is header, col 0 is first col (id): {import_data} ")
                     raise ServerError(respObj,zoho_error_code=code)
             elif (respObj.status_code in [401,]):
                 try:
                     #j = respObj.response.json(strict=False) #getting decode errors in this and they don't make sense
                     j = json.loads(respObj.response.text,strict=False)
@@ -282,31 +307,35 @@
                     if retry_countdown < 0:
                         logger.error(
                             f"Zoho API Recoverable error (invalid oauth token) exhausted retries")
                         raise UnrecoverableRateLimitError(urlResp=respObj,zoho_error_code=code)
                     else:
                         time.sleep(min(10 - retry_countdown, 1) * 10)
                         continue
+            elif (respObj.status_code in [414,]):
+                msg = f"HTTP response 414 was encountered (URI too large), no retry is attempted. {respObj.response.text} URL for {httpMethod=} {url=} {payLoad=}"
+                logger.error(msg)
+                raise BadDataError(respObj,zoho_error_code=None)
 
             elif (respObj.status_code in [500,]):
                 code = respObj.response.status_code
                 if ":7005" in respObj.response.text:
                     logger.error(f"Error 7005 encountered ('unexpected error'), no retry is attempted. {respObj.response.text}")
                     raise BadDataError(respObj,zoho_error_code=code)
             else:
                 try:
                     response_text = respObj.response.text
                 except Exception as e:
                     response_text = "unreadable response text"
-                msg = f"Unexpected status code in from __sendRequest. Server response code is {respObj.status_code=} {response_text=}. Retry attempts will be made..."
+                msg = f"Unexpected status code in from __sendRequest. Server response code is {respObj.status_code=} {response_text=}.  {url=}, {httpMethod=}, {payLoad=}, {action=} Retry attempts will be made..."
                 logger.exception(msg)
                 time.sleep(min(10 - retry_countdown, 1) * 10)
                 continue
         #fell off while loop
-        raise RuntimeError(f"After starting with {init_retry_countdown} retries allowed, there are now no more retries left in __sendRequest")
+        raise RuntimeError(f"After starting with {init_retry_countdown} retries allowed, there are now no more retries left in __sendRequest.  ")
 
     def invalidOAUTH(self, respObj):
         """
         Internal method to check whether accesstoken expires or not.
         """
         if (respObj.status_code != 200):
             try:
@@ -326,17 +355,22 @@
             raise ServerError(response)
         else:
             return self.handleResponse(response, action, callBackData)
 
     def handleResponse(self, response, action, callBackData) -> Optional[
         Union[MutableMapping, 'ImportResult', 'ShareInfo', 'PlanInfo']]:
         """
-        Internal method. To be used by classes extending this.
+        Internal method. To be used by classes extending this. To phase in V2 api,
+        set action  to be None or "API_V2"
         """
-        if ("ADDROW" == action):
+        if not action or action == "API_V2":
+            resp = response.content
+            resp_json = json.loads(resp)
+            return resp_json
+        elif ("ADDROW" == action):
             resp = response.content
             dom = ReportClientHelper.getAsDOM(resp)
             try:
                 dict = {}
                 cols = dom.getElementsByTagName("column")
                 for el in cols:
                     content = ReportClientHelper.getText(el.childNodes).strip()
@@ -756,14 +790,52 @@
         due to some error.
         @raise ParseError: If the server has responded but client was not able to parse the response.
         """
         payLoad = ReportClientHelper.getAsPayLoad([config], None, None)
         url = ReportClientHelper.addQueryParams(dbURI, self.token, "COPYDATABASE", "JSON")
         return self.__sendRequest(url, "POST", payLoad, "COPYDB", None)
 
+    def copy_workspace_api_v2(self, workspace_id, new_workspace_name, workspace_key, copy_with_data:bool,
+                      source_org_id,
+                      dest_org_id,
+                      copy_with_import_source:bool=False,
+
+                      ):
+        """
+       A v2 API functions
+        """
+        config_dict = {"newWorkspaceName":new_workspace_name,"newWorkspaceDesc":f"copy",
+                                                    "workspaceKey":workspace_key,
+                                                    "copyWithData":copy_with_data,
+                                                    "copyWithImportSource":copy_with_import_source}
+
+        config_data = "CONFIG=" + urllib.parse.quote_plus(json.dumps(config_dict))
+        url = self.getURI_v2() + f"workspaces/{workspace_id}"
+
+        extra_headers = {"ZANALYTICS-ORGID": source_org_id,"ZANALYTICS-DEST-ORGID": dest_org_id}
+        return self.__sendRequest(url, "POST",payLoad=None, params=config_data, action=None,extra_headers=extra_headers)
+
+    def get_orgs_metadata_api_v2(self):
+        url = self.getURI_v2() + f"orgs/"
+        return self.__sendRequest(url, "GET", payLoad=None, action=None)
+
+    def get_all_workspaces_metadata_api_v2(self):
+        url = self.getURI_v2() + f"workspaces/"
+        return self.__sendRequest(url, "GET", payLoad=None, action=None)
+
+    def get_workspace_secretkey_api_v2(self,workspace_id, org_id):
+        extra_headers = {"ZANALYTICS-ORGID": org_id, }
+        url = self.getURI_v2() + f"workspaces/{workspace_id}/secretkey"
+        return self.__sendRequest(url, "GET", payLoad=None, action=None, extra_headers=extra_headers)
+
+    def get_workspace_details_api_v2(self,workspace_id):
+        extra_headers = None
+        url = self.getURI_v2() + f"workspaces/{workspace_id}"
+        return self.__sendRequest(url, "GET", payLoad=None, action=None, extra_headers=extra_headers)
+
     def deleteDatabase(self, userURI, databaseName, config=None):
         """
         Delete the specified database.
         @param userURI: The URI of the user. See L{getUserURI<getUserURI>}.
         @type userURI:string
         @param databaseName: The name of the database to be deleted.
         @type databaseName:string
@@ -1729,14 +1801,21 @@
         """
         url = self.reportServerURL + "/api/" + urllib.parse.quote(dbOwnerName)
         url += "/" + self.splCharReplace(urllib.parse.quote(dbName)) + "/" + self.splCharReplace(
             urllib.parse.quote(tableOrReportName))
 
         return url
 
+    def getURI_v2(self) -> str:
+        """
+        Returns the base URL for v2 api with trailing /
+        """
+        url = self.reportServerURL + "/restapi/v2/"
+
+        return url
     def splCharReplace(self, value):
         """
         Internal method for handling special charecters in tale or database name.
         """
         value = value.replace("/", "(/)")
         value = value.replace("%5C", "(//)")
         return value
```

### Comparing `zoho_analytics_connector-1.3.6/zoho_analytics_connector.egg-info/PKG-INFO` & `zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: zoho-analytics-connector
-Version: 1.3.6
+Version: 1.4.1
 Summary: Zoho Analytics connector
 Home-page: https://github.com/timrichardson/zoho_analytics_connector
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MPL-2.0
 Keywords: zoho analytics
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Zoho Analytics Connector for Python
 ========================
 
 Zoho's Python SDK for Zoho Reports is old, however it is very complete.
 This is a version which is Python 3 ready, tested on Python 3.8 and 3.9 and in fairly substantial production use.
 
 A more convenient wrapper class is in enhanced_report_client. This is based on Zoho's ReportClient but provides some more convenient features.
 I use it mostly for uploading data, and creating and modifying tables.
 
-This library uses the Analytics V1 API.
+This library uses the Analytics V1 API and as of v.1.4 will phase in v2 API endpoints bit by bit
 
 Authentication
 ==============
 AuthTokens are now retired, replaced with OAuth2.
 
 OAuth2 notes are below.
 When you create EnhancedZohoAnalyticsClient or ReportClient, you need to pass ClientID, ClientSecret and a RefreshToken.
@@ -118,20 +119,18 @@
 NOTE!!! For Australian-hosted Zoho accounts and other regional variations:
 
 The token URL is adapted for the server location. e.g. for Australia, post to https://accounts.zoho.com.au/oauth/v2/token
 
 Usage
 =====
 
-Zoho's full API is available through the ReportClient API. However, there are bugs in this code.
-Recent 2020 changes have fixed some of these bugs, but I have hardly any test cases; I only have test cases
-for a handful of the standard functions of ReportClient. So proceed carefully if you use them.
+Zoho's full API v1 is available through the ReportClient API. 
+Selectively, v2 API endpoints will be added to the ReportClient if they are useful. 
 
-They are probably worth looking at. For instance, ReportClient.exportData now actually does use the file object you pass.
-But perhaps due to its python2 heritage, it expects a binary file object.
+One example of this is get_metadata_api_v2()
 
 Note that for data import and export, my EnhancedReportClient has its own methods, and these are what I use in production so they are much better tested.
 
 
     class EnhancedZohoAnalyticsClient(ReportClient)
     
 is a higher level layer.
@@ -301,14 +300,17 @@
 
 
 Changes
 -------------
 
 next_version Test updates
 
+1.4.1 Something seems to changed with the UTF encoding returned by the export endpoint. Change decoding to use utf-8-sig 
+1.4.0 some adaptation towards new API from Zoho
+
 1.3.6 Documentation updates, test updates. Added a 'pre-delete function' to calculate how many rows should be deleted.
     deleteData returns an int not a string for the number of rows deleted.
 
 1.3.3 - 1.3.5 Handle some more Zoho exceptions
 
 1.3.2 Under heavy concurrent load, an oauth token error was not being caught. Fixed; new token is generated and a retry occurs.
```

