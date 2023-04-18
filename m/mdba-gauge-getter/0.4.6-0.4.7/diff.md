# Comparing `tmp/mdba_gauge_getter-0.4.6.tar.gz` & `tmp/mdba_gauge_getter-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdba_gauge_getter-0.4.6.tar", last modified: Fri Jan 13 00:01:18 2023, max compression
+gzip compressed data, was "mdba_gauge_getter-0.4.7.tar", last modified: Tue Apr 18 00:32:37 2023, max compression
```

## Comparing `mdba_gauge_getter-0.4.6.tar` & `mdba_gauge_getter-0.4.7.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-13 00:01:16.399771 mdba_gauge_getter-0.4.6/
--rwxrwxrwx   0 root         (0) root         (0)      144 2022-11-24 23:38:59.000000 mdba_gauge_getter-0.4.6/LICENCE
--rwxrwxrwx   0 root         (0) root         (0)     5715 2023-01-13 00:01:17.947198 mdba_gauge_getter-0.4.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4917 2023-01-12 23:58:41.000000 mdba_gauge_getter-0.4.6/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-13 00:01:16.446744 mdba_gauge_getter-0.4.6/mdba_gauge_getter/
--rwxrwxrwx   0 root         (0) root         (0)      165 2022-11-24 23:38:59.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-13 00:01:16.552683 mdba_gauge_getter-0.4.6/mdba_gauge_getter/data/
--rwxrwxrwx   0 root         (0) root         (0)   838861 2022-11-24 23:39:00.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter/data/bom_gauge_data.csv
--rwxrwxrwx   0 root         (0) root         (0)    17302 2023-01-12 23:58:41.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter/gauge_getter.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-01-12 23:58:41.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-13 00:01:16.502712 mdba_gauge_getter-0.4.6/mdba_gauge_getter.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5715 2023-01-13 00:01:15.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      380 2023-01-13 00:01:16.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-01-13 00:01:16.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-01-13 00:01:16.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-01-13 00:01:16.000000 mdba_gauge_getter-0.4.6/mdba_gauge_getter.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      103 2022-11-24 23:39:00.000000 mdba_gauge_getter-0.4.6/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-01-13 00:01:18.027203 mdba_gauge_getter-0.4.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1280 2022-12-14 00:27:06.000000 mdba_gauge_getter-0.4.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 00:32:36.367597 mdba_gauge_getter-0.4.7/
+-rwxrwxrwx   0 root         (0) root         (0)      144 2022-11-24 23:38:59.000000 mdba_gauge_getter-0.4.7/LICENCE
+-rwxrwxrwx   0 root         (0) root         (0)     5715 2023-04-18 00:32:37.866403 mdba_gauge_getter-0.4.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4917 2023-01-12 23:58:41.000000 mdba_gauge_getter-0.4.7/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 00:32:36.391583 mdba_gauge_getter-0.4.7/mdba_gauge_getter/
+-rwxrwxrwx   0 root         (0) root         (0)      165 2022-11-24 23:38:59.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 00:32:36.476535 mdba_gauge_getter-0.4.7/mdba_gauge_getter/data/
+-rwxrwxrwx   0 root         (0) root         (0)   838861 2022-11-24 23:39:00.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter/data/bom_gauge_data.csv
+-rwxrwxrwx   0 root         (0) root         (0)    18904 2023-04-18 00:30:41.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter/gauge_getter.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-18 00:30:41.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 00:32:36.439557 mdba_gauge_getter-0.4.7/mdba_gauge_getter.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5715 2023-04-18 00:32:35.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      407 2023-04-18 00:32:36.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-18 00:32:36.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-18 00:32:36.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-18 00:32:36.000000 mdba_gauge_getter-0.4.7/mdba_gauge_getter.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      103 2022-11-24 23:39:00.000000 mdba_gauge_getter-0.4.7/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-18 00:32:37.926404 mdba_gauge_getter-0.4.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1286 2023-04-18 00:30:41.000000 mdba_gauge_getter-0.4.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 00:32:36.500521 mdba_gauge_getter-0.4.7/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    15336 2023-04-18 00:30:41.000000 mdba_gauge_getter-0.4.7/tests/test_gauge_getter.py
```

### Comparing `mdba_gauge_getter-0.4.6/PKG-INFO` & `mdba_gauge_getter-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdba_gauge_getter
-Version: 0.4.6
+Version: 0.4.7
 Summary: Facilitates waterflow gauge data ingest from several endpoints. Dependency to several other projects.
 Home-page: https://github.com/MDBAuth/MDBA_Gauge_Getter
 Author: Murray Darling Basin Authority
 Author-email: ben.bradshaw@mdba.gov.au
 Project-URL: Bug Tracker, https://github.com/MDBAuth/MDBA_Gauge_Getter/issues
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mdba_gauge_getter-0.4.6/README.md` & `mdba_gauge_getter-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `mdba_gauge_getter-0.4.6/mdba_gauge_getter/data/bom_gauge_data.csv` & `mdba_gauge_getter-0.4.7/mdba_gauge_getter/data/bom_gauge_data.csv`

 * *Files identical despite different names*

### Comparing `mdba_gauge_getter-0.4.6/mdba_gauge_getter/gauge_getter.py` & `mdba_gauge_getter-0.4.7/mdba_gauge_getter/gauge_getter.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,26 @@
 
 STATE_LAKELEVEL_VarTo = {
     'NSW': Decimal('130.00'),
     'VIC' : Decimal('130.00'),
     'QLD' : Decimal('130.00')
 }
 
+STATE_STORAGEVOLUME_VarFrom = {
+    'NSW' : Decimal('130.00'),
+    'VIC' : Decimal('136.00'),
+    'QLD' : Decimal('136.00')
+}
+
+STATE_STORAGEVOLUME_VarTo = {
+    'NSW': Decimal('136.00'),
+    'VIC' : Decimal('136.00'),
+    'QLD' : Decimal('136.00')
+}
+
 MAX_SITES_PER_REQUEST = {
     'NSW': 5,
     'VIC': 5,
     'QLD': 5,
     'SA' : 5 
 }
 
@@ -152,14 +164,21 @@
         var_from = STATE_FLOW_VarFrom[state]
         var_to = STATE_FLOW_VarTo[state]
 
     elif (var=="LL"):
         var_from = STATE_LAKELEVEL_VarFrom[state]
         var_to = STATE_LAKELEVEL_VarTo[state]
 
+    elif (var=="SV"):
+        var_from = STATE_STORAGEVOLUME_VarFrom[state]
+        var_to = STATE_STORAGEVOLUME_VarTo[state]
+
+    else:
+        raise AttributeError("The input 'var' takes 'L', 'F', 'LL' or 'SV' only.") # TODO: Implement a more accurate exception handling
+
     sites = ','.join(indicative_sites)
     data = {
         'params': {
             'site_list': sites,
             'start_time': start_time.strftime('%Y%m%d') + '000000',
             'varfrom': f'{var_from:.2f}',
             'interval': str(interval),
@@ -197,16 +216,15 @@
     if state =="QLD": # replace when QLD upgrades
         req_url = f'https://{url}/cgi/webservice.pl?{json_data}'
 
     req_url = req_url.replace(' ', '%20')
     
     # TODO-idiosyncratic the use of JSON in the query string seems werid, this should be a HTTP POST
     # but requires endpoints to support it..
-    
-    log.debug(f'ending request to URL \'{req_url}\'')
+    log.debug(f'Sending request to URL \'{req_url}\'')
     r = requests.get(req_url)
     if not r.status_code == 200: 
         raise requests.HTTPError(f'Request to \'{url}\' failed with HTTP Response code '
                                  f'{r.status_code} and HTTP Response:\n{r.content}')
     try:
         return json.loads(r.content)
     except json.decoder.JSONDecodeError:
@@ -393,14 +411,15 @@
             elif var.lower() in ['l', 'll', 'sl']:
                 ts["VALUE"] = ts["Value[m]"]
             elif var.lower() == 'sv':
                 ts["VALUE"] = ts["Value[Ml]"]
             ts["QUALITYCODE"] = ts["Quality"]
             ts.reset_index(drop=True, inplace=True)
             collect.append(ts[["DATASOURCEID","SITEID",	"SUBJECTID", "DATETIME", "VALUE", "QUALITYCODE"]])
+            log.info(f'BOM Data DF: {collect}')
 
     output = pd.concat(collect)
     # log.info(f'BOM Data DF: {output}')
     output = output.values.tolist()
     # log.info(f'BOM Data Dict: {output}')
     return output
 
@@ -420,20 +439,40 @@
     if data_source.lower() == 'bom':
         gauges_by_state = {'NSW': [], 'QLD': [], 'VIC': [], 'SA': [], 'rest': [],'BOM': gauge_numbers}
     elif gauges_by_state['SA']:
         gauges_by_state['BOM'] = gauges_by_state['SA']
 
     # log.info(f'Gauges by state is: {gauges_by_state}')
     data: List[List[List[Any]]] = []
-    data += process_gauge_pull(gauges_by_state['NSW'], 'NSW', 'CP', start_time_user,
+    nsw = process_gauge_pull(gauges_by_state['NSW'], 'NSW', 'CP', start_time_user,
                                end_time_user, var, interval, data_type)
-    data += process_gauge_pull(gauges_by_state['VIC'], 'VIC', 'PUBLISH', start_time_user,
+    if not len(nsw) and len(gauges_by_state['NSW']) > 0:
+        log.warn(f'Data not available from NSW API, querying BOM...')
+        gauges_by_state['BOM'] = gauges_by_state['NSW']
+        nsw += gauge_pull_bom(gauges_by_state['BOM'], start_time_user, 
+                               end_time_user, var, interval, data_type)   
+    data += nsw
+
+    vic = process_gauge_pull(gauges_by_state['VIC'], 'VIC', 'PUBLISH', start_time_user,
+                               end_time_user, var, interval, data_type)
+    if not len(vic) and len(gauges_by_state['VIC']) > 0:
+        log.warn(f'Data not available from VIC API, querying BOM...')
+        gauges_by_state['BOM'] = gauges_by_state['VIC']
+        vic += gauge_pull_bom(gauges_by_state['BOM'], start_time_user, 
+                               end_time_user, var, interval, data_type)   
+    data += vic
+
+    qld = process_gauge_pull(gauges_by_state['QLD'], 'QLD', 'AT', start_time_user,
                                end_time_user, var, interval, data_type)
-    data += process_gauge_pull(gauges_by_state['QLD'], 'QLD', 'AT', start_time_user,
-                               end_time_user, var, interval, data_type) 
+    if not len(qld) and len(gauges_by_state['QLD']) > 0:
+        log.warn(f'Data not available from QLD API, querying BOM...')
+        gauges_by_state['BOM'] = gauges_by_state['QLD']
+        qld += gauge_pull_bom(gauges_by_state['BOM'], start_time_user, 
+                               end_time_user, var, interval, data_type)   
+    data += qld
     # log.info(f'State data:{data}')
     if 'BOM' in gauges_by_state:                          
         data += gauge_pull_bom(gauges_by_state['BOM'], start_time_user, 
                                end_time_user, var, interval, data_type)   
         # log.info(f'BOM data:{data}')
    
     cols = ['DATASOURCEID', 'SITEID', 'SUBJECTID', 'DATETIME', 'VALUE', 'QUALITYCODE']
```

### Comparing `mdba_gauge_getter-0.4.6/mdba_gauge_getter.egg-info/PKG-INFO` & `mdba_gauge_getter-0.4.7/mdba_gauge_getter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdba-gauge-getter
-Version: 0.4.6
+Version: 0.4.7
 Summary: Facilitates waterflow gauge data ingest from several endpoints. Dependency to several other projects.
 Home-page: https://github.com/MDBAuth/MDBA_Gauge_Getter
 Author: Murray Darling Basin Authority
 Author-email: ben.bradshaw@mdba.gov.au
 Project-URL: Bug Tracker, https://github.com/MDBAuth/MDBA_Gauge_Getter/issues
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mdba_gauge_getter-0.4.6/setup.py` & `mdba_gauge_getter-0.4.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import setuptools
-
 import sys
 
 sys.path[0:0] = ['mdba_gauge_getter']
 
 from version import __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
@@ -30,14 +29,14 @@
         'Programming Language :: Python :: 3.10',
         'Framework :: Pytest',
     ],
     packages=[
         "mdba_gauge_getter",
     ],
     install_requires=[
-        "pandas",
+        "pandas==1.3.5",
         "requests",
         "bomwater",
     ],
     package_data={"": ["data/*.csv"]},
     python_requires=">=3.6",
 )
```

