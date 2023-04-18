# Comparing `tmp/neuro-connector-api-1.2.2b0.tar.gz` & `tmp/neuro-connector-api-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-connector-api-1.2.2b0.tar", last modified: Thu Mar 16 16:48:12 2023, max compression
+gzip compressed data, was "neuro-connector-api-2.0.0b0.tar", last modified: Tue Apr 18 14:58:59 2023, max compression
```

## Comparing `neuro-connector-api-1.2.2b0.tar` & `neuro-connector-api-2.0.0b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:48:12.499370 neuro-connector-api-1.2.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 16:47:59.000000 neuro-connector-api-1.2.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-16 16:48:12.499370 neuro-connector-api-1.2.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-16 16:47:59.000000 neuro-connector-api-1.2.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:48:12.499370 neuro-connector-api-1.2.2b0/neuro-connector-api/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-03-16 16:47:59.000000 neuro-connector-api-1.2.2b0/neuro-connector-api/NeuroConnector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:48:12.499370 neuro-connector-api-1.2.2b0/neuro_connector_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-16 16:48:12.000000 neuro-connector-api-1.2.2b0/neuro_connector_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-16 16:48:12.000000 neuro-connector-api-1.2.2b0/neuro_connector_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:48:12.000000 neuro-connector-api-1.2.2b0/neuro_connector_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-16 16:48:12.000000 neuro-connector-api-1.2.2b0/neuro_connector_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-16 16:48:12.000000 neuro-connector-api-1.2.2b0/neuro_connector_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:48:12.499370 neuro-connector-api-1.2.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-16 16:47:59.000000 neuro-connector-api-1.2.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/neuro-connector-api/
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/neuro-connector-api/NeuroConnector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 14:58:59.000000 neuro-connector-api-2.0.0b0/neuro_connector_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:58:59.195264 neuro-connector-api-2.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 14:58:45.000000 neuro-connector-api-2.0.0b0/setup.py
```

### Comparing `neuro-connector-api-1.2.2b0/LICENSE` & `neuro-connector-api-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-connector-api-1.2.2b0/neuro-connector-api/NeuroConnector.py` & `neuro-connector-api-2.0.0b0/neuro-connector-api/NeuroConnector.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,47 +8,44 @@
 from time import sleep as pause
 import json
 import requests
 import datetime
 import urllib.parse
 from datetime import datetime as dt
 
-logging.getLogger("neuro-api-client").propagate = False
-logging.basicConfig(filename='neuro-api-client.log', level=logging.INFO,
-                    format='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-
-
 class NeuroConnector:
+    logging.getLogger("neuro-connector-api").propagate = False
+    logging.basicConfig(filename='neuro-connector-api.log', level=logging.DEBUG,
+                        format='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+
     token = ''
     headers = ''
     url = ''
     requestWrapper = None
     connectionId = None
     organization = None
     jobName = None
     jobNumber = None
     projectName = None
 
-    def __init__(self, appToken, url, connectionId, organizationId, jobName, jobNumber=None):
-        self.jobNumber = jobNumber
+    def __init__(self, url, organizationId, appToken=None):
 
-        self.jobName = jobName
-        assert self.jobName, "job name needed"
+        assert url, "need neuro base url"
+        self.url = url
 
         if appToken:
             token = "Bearer " + appToken
         else:
             token = None
 
         self.requestWrapper = RequestWrapper(token=token,
                                              url=url)
 
         assert self.requestWrapper, "couldn't initiate request wrapper"
 
-        self.connectionId = connectionId
         self.organizationId = organizationId
         assert self.organizationId, "organizationId missing"
 
     def delete_record(self, key):
         o = {}
         o['webhookEvent'] = 'jira:issue_deleted'
         o['issue'] = {'key': key, 'id': key}
@@ -76,73 +73,80 @@
 
         # Removes the : symbol from timezone
         parsed = re.sub(r'([+-]\d+):(\d+)$', r'\1\2', currentDateTime)
 
         return parsed
 
     def getEpochTime(self):
-        return str(int(time.time()))
+        return str(int(time.time() * 1000))
 
     def deleteData(self):
         logging.info("deleting existing data")
         endpoint = '/ms-provision-receptor/custom/zephyr/remove-data/' + self.organizationId + '/' + self.connectionId
 
         response = self.requestWrapper.make(endpoint=endpoint, types="DELETE")
         logging.info(response[1]['status'] + " deleting data")
 
         return response
 
     def parseJSONfile(self, filepath):
+        assert filepath is not None, "filepath required"
         payload = ''
         with open(filepath, encoding='utf-8') as json_file:
             payload = json.load(json_file)
         return payload
 
-    def buildTestResultWebhookPayload(self, results, jobName, jobNumber, path):
+    def buildTestResultWebhookPayload(self, results, jobName, jobNumber):
         duration = self.calculateDuration(results)
 
         timestamp = self.getEpochTime()
+        jobNumber = str(jobNumber)
+
         if jobNumber is None:
             jobNumber = str(timestamp)
             id = str(jobName) + "_" + str(timestamp)
         else:
             id = str(jobName) + "_" + str(jobNumber) + "_" + str(timestamp)
 
         return {
             "actions": [
                 {
-                    "path": str(path),
                     "testResult": results
                 }
             ],
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
-            "url": "https://myneuro.ai"
+            "url": self.url
         }
 
     def encodeStringForURL(self, string):
         return urllib.parse.quote(string)
 
-    def sendCucumberTestResultsJson(self, filePath):
-        assert filePath, "file path must not be null"
+    def sendCucumberTestResultsJson(self, filePath,
+                                    jobName, jobNumber=None):
+        print("Sending webhook for cucumber test results to " + self.url)
+
         results = self.parseJSONfile(filePath)
 
-        payload = self.buildTestResultWebhookPayload(results=results, jobName=self.jobName, jobNumber=self.jobNumber,
-                                                     path=filePath)
+        payload = self.buildTestResultWebhookPayload(results=results, jobName=jobName, jobNumber=jobNumber)
         endpoint = "/ms-source-mediator/cucumber/webhook/receive"
         self.send_webhook(endpoint=endpoint, payload=payload)
 
+    def sendTriggerWebhook(self, payload):
+        endpoint = "/???"
+        self.send_webhook(endpoint=endpoint, payload=payload)
+
     def getResult(self, results):
         stepStatuses = []
 
         for scenario in results:
             if 'elements' in scenario:
                 for element in scenario['elements']:
                     if 'steps' in element:
@@ -179,33 +183,70 @@
     #         if 'elements' in scenario:
     #             for element in scenario['elements']:
     #                 if 'steps' in element:
     #                     for step in element['steps']:
     #                         if 'result' in step:
     #                             if 'duration' in step['result']:
     #                                 duration = duration + int(step['result']['duration'])
+    def releaseTrigger(self, projectKey, branch, commitId, label, environmentName, environmentType, vcsProject):
+        payload = self.buildGenericTriggerPayload(projectKey, branch, commitId, label, environmentName, environmentType,
+                                                  vcsProject)
+        payload["triggerType"] = "release"
+        print("Sending webhook for release trigger to " + self.url)
+        self.sendTriggerWebhook(payload)
+
+    def deploymentTrigger(self, projectKey, branch, commitId, label, environmentName, environmentType, vcsProject):
+        payload = self.buildGenericTriggerPayload(projectKey, branch, commitId, label, environmentName, environmentType,
+                                                  vcsProject)
+        payload["triggerType"] = "deployment"
+        print("Sending webhook for deployment trigger to " + self.url)
+        self.sendTriggerWebhook(payload)
+
+    def buildGenericTriggerPayload(self, projectKey, branch, commitId, label, environmentName, environmentType,
+                                   vcsProject):
+
+        assert projectKey is not None, "projectKey needed"
+        assert branch is not None, "branch needed"
+        assert commitId is not None, "commitId needed"
+        assert label is not None, "label needed"
+        assert environmentName is not None, "environmentName needed"
+        assert environmentType is not None, "environmentType needed"
+        assert vcsProject is not None, "vcsProject needed"
+
+        return {
+            "organization": self.organizationId,
+            "url": self.url,
+            "timestamp": self.getEpochTime(),
+            'projectKey': projectKey,
+            'branch': branch,
+            'commitId': commitId,
+            'label': label,
+            'environmentName': environmentName,
+            'environmentType': environmentType,
+            'vcsProject': vcsProject
+        }
 
 
 class RequestWrapper():
     request = None
     logging.getLogger("neuro-api-client").propagate = False
     logging.basicConfig(filename='neuro-api-client.log', level=logging.DEBUG,
                         format='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
-    def __init__(self, url,token=None):
+    def __init__(self, url, token=None):
         self.request = Request(token, url)
         # TO DO - implement certificate verification and remove the below
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         assert self.request
 
     def make(self, endpoint=None, types=None, payload=None):
         attempt = 0
         maxAttempts = 5
         errorMessage = ""
-        waitInSeconds = 60
+        waitInSeconds = 10
 
         assert endpoint
         assert types
 
         while attempt < maxAttempts:
             try:
                 if payload:
@@ -289,68 +330,125 @@
             jsonResponse = response.json()
         except:
             jsonResponse = {}
 
         return response, jsonResponse
 
 
-if __name__ == "__main__":
-    appToken = None
+class Orchestrator:
+    logging.getLogger("neuro-connector-api").propagate = False
+    logging.basicConfig(filename='neuro-connector-api.log', level=logging.INFO,
+                        format='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+
+    opts=[]
+
+    # common
     organizationId = None
     baseUrl = None
+
+    # Function 1 (sendTestResultsJson)
     function = None
     filePath = None
-    connectionId = None
     jobNumber = None
     jobName = None
 
-    instructions = '\nNeuroConnector -f [function] -p [filePath] -u [baseUrl] -a [appToken optional] -o [organizationId] -c [connectonId optional] -n [jobName] -j [jobNumber optional]  \n\nFunctions [1=sendTestResultsJson]\n'
+    # Function 2 (releaseTrigger) & Function 3 (deploymentTrigger)
+    projectKey = None
+    branch = None
+    commitId = None
+    label = None
+    environmentName = None
+    environmentType = None
+    vcsProject = None
+
+    def __init__(self, args):
+
+        self.args = args
+        self.opts = ["-h", "--func=", "--path=", "--url=", "--org=", "--jobName=", "--jobNum=", "--projKey=", "--vcsProj=",
+                "--branch=", "--commitId=", "--label=", "--env=", "--envType=", "--help"]
+
+        self.instructions= '\n-h, --help : Help\n'
+        self.instructions = self.instructions + '\nFunction 1 (sendTestResultsJson)\nNeuroConnector --func 1 --path [filePath] --url [baseUrl] --org [organizationId] --jobName [jobName] --jobNum [jobNumber (optional)]\n'
+        self.instructions = self.instructions + '\nFunction 2 (releaseTrigger)\nNeuroConnector --func 2  --url [baseUrl] --org [organizationId] --projKey [projectKey, e.g jira/management] --vcsProj [vcsProject] --branch [branchName] --commitId [commitId] --label [type label, e.g ms/client]\n'
+        self.instructions = self.instructions + '\nFunction 3 (deploymentTrigger)\nNeuroConnector --func 3 --url [baseUrl] --org [organizationId] --projKey [projectKey, e.g jira/management] --vcsProj [vcsProject] --branch [branchName] --commitId [commitId] --label [type label, e.g ms/client]\n'
+
+    def getParameterPairsForArgs(self):
+        parameterPairs = {}
+        for i, arg in enumerate(self.args):
+            for opt in self.opts:
+                if opt[-1] == "=" and opt[:-1] == arg:
+                    try:
+                        value = self.args[i + 1]
+                        assert value is not None and not value.startswith("-")
+                    except:
+                        raise Exception("no value for key " + arg)
+
+                    parameterPairs.update({arg: value})
+                elif arg == opt and opt[-1] != "=":
+                    parameterPairs.update({arg: None})
+
+        return parameterPairs
 
-    args = sys.argv[1:]
-    try:
-        opts, args = getopt.getopt(args, "f:p:u:a:o:c:n:j:h")
-    except getopt.GetoptError:
-        print(instructions, file=sys.stderr)
-        sys.exit(2)
-    for opt, arg in opts:
-        if opt in ("-c"):
-            connectionId = arg
-        elif opt in ("-o"):
-            organizationId = arg
-        elif opt in ("-u"):
-            baseUrl = arg
-        elif opt in ("-a"):
-            appToken = arg
-        elif opt in ("-f"):
-            function = arg
-        elif opt in ("-p"):
-            filePath = arg
-        elif opt in ("-n"):
-            jobName = arg
-        elif opt in ("-j"):
-            jobNumber = arg
-        elif opt in ("-h"):
-            print("HELP " + instructions, file=sys.stderr)
-            sys.exit()
-        else:
-            print(instructions, file=sys.stderr)
-            sys.exit()
 
-    assert baseUrl, "url must not be none\n" + instructions
-    assert organizationId, "organizationId must not be none\n" + instructions
-    assert function, "function must not be none\n" + instructions
-
-    assert jobName, "jobName must not be none\n" + instructions
-
-    try:
-        nc = NeuroConnector(appToken=appToken, url=baseUrl, connectionId=connectionId, organizationId=organizationId,
-                            jobName=jobName, jobNumber=jobNumber)
+    def orchestrate(self):
+        parameterPairs=self.getParameterPairsForArgs()
+
+        assert "-h" not in parameterPairs and "--help" not in parameterPairs and len(parameterPairs.keys()) >= 3, "\n\nSee instructions\n"+self.instructions
+        assert "--func" in parameterPairs, "function param needed --func\n" + self.instructions
+
+        function = parameterPairs["--func"]
+
         if str(function) == '1':
-            assert filePath, "filePath must not be none\n" + instructions
-            nc.sendCucumberTestResultsJson(filePath=filePath)
-        else:
-            raise Exception("no function configured for " + str(function))
-    except Exception as e:
-        print("NeuroConnector failed for reason " + str(e), file=sys.stderr)
-        logging.error(traceback.format_exc())
-        print(traceback.format_exc(), file=sys.stderr)
-        sys.exit(2)
+            for key in parameterPairs.keys():
+                if key == "--org":
+                    self.organizationId = parameterPairs[key]
+                elif key == "--url":
+                    self.baseUrl = parameterPairs[key]
+                elif key == "--path":
+                    self.filePath = parameterPairs[key]
+                elif key == "--jobName":
+                    self.jobName = parameterPairs[key]
+                elif key == "--jobNum":
+                    self.jobNumber = parameterPairs[key]
+
+        elif str(function) in ['2', '3']:
+            for key in parameterPairs.keys():
+                if key == "--org":
+                    self.organizationId = parameterPairs[key]
+                elif key == "--url":
+                    self.baseUrl = parameterPairs[key]
+                elif key == "--projKey":
+                    self.projectKey = parameterPairs[key]
+                elif key == "--branch":
+                    self.branch = parameterPairs[key]
+                elif key == "--commitId":
+                    self.commitId = parameterPairs[key]
+                elif key == "--label":
+                    self.label = parameterPairs[key]
+                elif key == "--env":
+                    self.environmentName = parameterPairs[key]
+                elif key == "--envType":
+                    self.environmentType = parameterPairs[key]
+                elif key == "--vcsProj":
+                    self.vcsProject = parameterPairs[key]
+
+        try:
+            nc = NeuroConnector(url=self.baseUrl, organizationId=self.organizationId)
+            if str(function) == '1':
+                nc.sendCucumberTestResultsJson(self.filePath, self.jobName, self.jobNumber)
+            elif str(function) == '2':
+                nc.releaseTrigger(self.projectKey, self.branch, self.commitId, self.label, self.environmentName, self.environmentType, self.vcsProject)
+            elif str(function) == '3':
+                nc.deploymentTrigger(self.projectKey, self.branch, self.commitId, self.label, self.environmentName, self.environmentType, self.vcsProject)
+            else:
+                print(self.instructions, file=sys.stderr)
+                raise Exception("function not defined")
+
+        except Exception as e:
+            print("NeuroConnector failed for reason " + str(e), file=sys.stderr)
+            logging.error(traceback.format_exc())
+            print(traceback.format_exc(), file=sys.stderr)
+            sys.exit(2)
+
+
+if __name__ == "__main__":
+    Orchestrator(args=sys.argv[1:]).orchestrate()
```

