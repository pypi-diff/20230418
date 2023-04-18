# Comparing `tmp/neuro-connector-api-2.0.0b0.tar.gz` & `tmp/neuro-connector-api-2.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-connector-api-2.0.0b0.tar", last modified: Tue Apr 18 14:58:59 2023, max compression
+gzip compressed data, was "neuro-connector-api-2.0.1b0.tar", last modified: Tue Apr 18 16:13:29 2023, max compression
```

## Comparing `neuro-connector-api-2.0.0b0.tar` & `neuro-connector-api-2.0.1b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/neuro-connector-api/
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/neuro-connector-api/NeuroConnector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:13:29.953517 neuro-connector-api-2.0.1b0/neuro-connector-api/
+-rw-r--r--   0 runner    (1001) docker     (123)    18359 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/neuro-connector-api/NeuroConnector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/setup.py
```

### Comparing `neuro-connector-api-2.0.0b0/LICENSE` & `neuro-connector-api-2.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-connector-api-2.0.0b0/neuro-connector-api/NeuroConnector.py` & `neuro-connector-api-2.0.1b0/neuro-connector-api/NeuroConnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,39 +95,39 @@
             payload = json.load(json_file)
         return payload
 
     def buildTestResultWebhookPayload(self, results, jobName, jobNumber):
         duration = self.calculateDuration(results)
 
         timestamp = self.getEpochTime()
-        jobNumber = str(jobNumber)
 
         if jobNumber is None:
-            jobNumber = str(timestamp)
+            jobNumber = str(timestamp[:-3])
             id = str(jobName) + "_" + str(timestamp)
         else:
             id = str(jobName) + "_" + str(jobNumber) + "_" + str(timestamp)
 
         return {
-            "actions": [
-                {
-                    "testResult": results
-                }
-            ],
+
             "displayName": "#" + jobNumber,
             "duration": 0,
             "estimatedDuration": duration,
             "fullDisplayName": str(jobName) + " #" + jobNumber,
             "id": id,
             "number": int(jobNumber),
             "organization": self.organizationId,
             "projectName": str(jobName),
             "result": self.getResult(results),
             "timestamp": timestamp,
-            "url": self.url
+            "url": self.url,
+            "actions": [
+                {
+                    "testResult": results
+                }
+            ]
         }
 
     def encodeStringForURL(self, string):
         return urllib.parse.quote(string)
 
     def sendCucumberTestResultsJson(self, filePath,
                                     jobName, jobNumber=None):
```

