# Comparing `tmp/mmtapi-0.5.1.tar.gz` & `tmp/mmtapi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmtapi-0.5.1.tar", last modified: Mon Sep 14 19:39:34 2020, max compression
+gzip compressed data, was "mmtapi-0.6.1.tar", last modified: Mon Apr 17 22:39:46 2023, max compression
```

## Comparing `mmtapi-0.5.1.tar` & `mmtapi-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 crisp      (501) staff       (20)        0 2020-09-14 19:39:34.000000 mmtapi-0.5.1/
-drwxr-xr-x   0 crisp      (501) staff       (20)        0 2020-09-14 19:39:34.000000 mmtapi-0.5.1/MMTAPI.egg-info/
--rw-r--r--   0 crisp      (501) staff       (20)    10180 2020-09-14 19:39:33.000000 mmtapi-0.5.1/MMTAPI.egg-info/PKG-INFO
--rw-r--r--   0 crisp      (501) staff       (20)      331 2020-09-14 19:39:33.000000 mmtapi-0.5.1/MMTAPI.egg-info/SOURCES.txt
--rw-r--r--   0 crisp      (501) staff       (20)        1 2020-09-14 19:39:33.000000 mmtapi-0.5.1/MMTAPI.egg-info/dependency_links.txt
--rw-r--r--   0 crisp      (501) staff       (20)        7 2020-09-14 19:39:33.000000 mmtapi-0.5.1/MMTAPI.egg-info/top_level.txt
--rw-r--r--   0 crisp      (501) staff       (20)    10180 2020-09-14 19:39:34.000000 mmtapi-0.5.1/PKG-INFO
--rw-r--r--   0 crisp      (501) staff       (20)     8060 2020-08-27 20:13:04.000000 mmtapi-0.5.1/README.md
-drwxr-xr-x   0 crisp      (501) staff       (20)        0 2020-09-14 19:39:34.000000 mmtapi-0.5.1/mmtapi/
--rw-r--r--   0 crisp      (501) staff       (20)     1172 2020-09-14 19:32:35.000000 mmtapi-0.5.1/mmtapi/__init__.py
--rw-r--r--   0 crisp      (501) staff       (20)    19697 2020-09-14 19:33:46.000000 mmtapi-0.5.1/mmtapi/mmtapi.py
--rw-r--r--   0 crisp      (501) staff       (20)      837 2020-07-11 01:06:44.000000 mmtapi-0.5.1/mmtapi/test.py
--rw-r--r--   0 crisp      (501) staff       (20)      148 2020-07-14 21:10:44.000000 mmtapi-0.5.1/mmtapi/upload_test.py
--rw-r--r--   0 crisp      (501) staff       (20)       38 2020-09-14 19:39:34.000000 mmtapi-0.5.1/setup.cfg
--rw-r--r--   0 crisp      (501) staff       (20)      711 2020-09-14 19:38:23.000000 mmtapi-0.5.1/setup.py
+drwxr-xr-x   0 crisp      (501) staff       (20)        0 2023-04-17 22:39:46.478562 mmtapi-0.6.1/
+drwxr-xr-x   0 crisp      (501) staff       (20)        0 2023-04-17 22:39:46.475250 mmtapi-0.6.1/MMTAPI.egg-info/
+-rw-r--r--   0 crisp      (501) staff       (20)     8568 2023-04-17 22:39:46.000000 mmtapi-0.6.1/MMTAPI.egg-info/PKG-INFO
+-rw-r--r--   0 crisp      (501) staff       (20)      423 2023-04-17 22:39:46.000000 mmtapi-0.6.1/MMTAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 crisp      (501) staff       (20)        1 2023-04-17 22:39:46.000000 mmtapi-0.6.1/MMTAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 crisp      (501) staff       (20)        7 2023-04-17 22:39:46.000000 mmtapi-0.6.1/MMTAPI.egg-info/top_level.txt
+-rw-r--r--   0 crisp      (501) staff       (20)     8568 2023-04-17 22:39:46.478199 mmtapi-0.6.1/PKG-INFO
+-rw-r--r--   0 crisp      (501) staff       (20)     8128 2022-07-10 01:23:49.000000 mmtapi-0.6.1/README.md
+drwxr-xr-x   0 crisp      (501) staff       (20)        0 2023-04-17 22:39:46.476352 mmtapi-0.6.1/mmtapi/
+-rw-r--r--   0 crisp      (501) staff       (20)     1561 2023-04-17 22:38:34.000000 mmtapi-0.6.1/mmtapi/__init__.py
+-rw-r--r--   0 crisp      (501) staff       (20)     1545 2022-08-02 22:48:17.000000 mmtapi-0.6.1/mmtapi/download_test.py
+drwxr-xr-x   0 crisp      (501) staff       (20)        0 2023-04-17 22:39:46.477888 mmtapi-0.6.1/mmtapi/instruments/
+-rw-r--r--   0 crisp      (501) staff       (20)       15 2023-04-17 22:38:34.000000 mmtapi-0.6.1/mmtapi/instruments/__init__.py
+-rw-r--r--   0 crisp      (501) staff       (20)     5030 2023-04-17 22:38:34.000000 mmtapi-0.6.1/mmtapi/instruments/binospec.py
+-rw-r--r--   0 crisp      (501) staff       (20)     5308 2023-04-17 22:38:34.000000 mmtapi-0.6.1/mmtapi/instruments/mmirs.py
+-rw-r--r--   0 crisp      (501) staff       (20)    22307 2023-04-17 22:38:34.000000 mmtapi-0.6.1/mmtapi/mmtapi.py
+-rw-r--r--   0 crisp      (501) staff       (20)      837 2020-07-11 01:06:44.000000 mmtapi-0.6.1/mmtapi/test.py
+-rw-r--r--   0 crisp      (501) staff       (20)       38 2023-04-17 22:39:46.478627 mmtapi-0.6.1/setup.cfg
+-rw-r--r--   0 crisp      (501) staff       (20)      711 2023-04-17 22:39:43.000000 mmtapi-0.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mmtapi-0.5.1/README.md` & `mmtapi-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 ## Using the API Wrapper
 
 Here we describe the process to POST, GET, UPDATE, and DELETE a MMT Target. The `Target` class also contains an `api` class that calls each of the API methods. This class contains the request information for each request method so that it can debugged in the command line. 
 
 ```python
 import mmtapi.mmtapi as mmtapi
 
-Target = mmtapi.Target(token=API_TOKEN, ...)
+target = mmtapi.Target(token=API_TOKEN, ...)
 #once a request is made
 
-Target.**action() #post, delete, update... etc
+target.**action() #post, delete, update... etc
 
 #the request response can be viewed by
-Target.api.request
+target.request
 
 #which contains all of the expected request response information:
-#   Target.api.request.content
-#   Target.api.request.text
-#   Target.api.request.status_code
+#   target.request.content
+#   target.request.text
+#   target.request.status_code
 #   etc
 ```
 
 ### Creating a Target
 
 To create a target there are a lot of required fields and conditional parameters based on the observation type. To begin with the metadata for the target itself:
 
@@ -138,14 +138,20 @@
 
 Once a target is either created, or retrieved with the API GET method, a finder image can be uploaded. If an finder image already exists, this will overwrite it. All that is needed the pathway to the finder image.
 
 ```python
 target.upload_finder(finder_path=PATH_TO_IMAGE)
 ```
 
+### Downloading a completed observation
+
+```python
+target.download_exposures()
+```
+
 ### Updating Target Information
 
 Once a target is created, or retrieved with the API GET method, its meta-data can be updated. All that is required is passing in the valid keyword arguments and their respective values. The updated information will be validated before being submitted to the API.
 
 ```python
 #the kwargs can be defined as: KEY_WORD1=VAlUE1, KEY_WORD2=VALUE2... etc 
 target.update(KEY_WORD1=VAlUE1, KEY_WORD2=VALUE2... etc)
```

### Comparing `mmtapi-0.5.1/mmtapi/__init__.py` & `mmtapi-0.6.1/mmtapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+from . import instruments
+
 MMT_JSON_KEYS = ("id", "ra", "objectid", "observationtype", "moon", "seeing", "photometric", "priority", "dec",
                  "ra_decimal", "dec_decimal", "pm_ra", "pm_dec", "magnitude", "exposuretime", "numberexposures",
                  "visits", "onevisitpernight", "filter", "grism", "grating", "centralwavelength", "readtab",
                  "gain", "dithersize", "epoch", "submitted", "modified", "notes", "pa", "maskid", "slitwidth",
                  "slitwidthproperty", "iscomplete", "disabled", "notify", "locked", "findingchartfilename",
                  "instrumentid", "targetofopportunity", "reduced", "exposuretimeremaining", "totallength",
                  "totallengthformatted", "exposuretimeremainingformatted", "exposuretimecompleted",
                  "percentcompleted", "offsetstars", "details", "mask")
 
+LOCAL_TARGET_KEYS = ("partial_download", "downloaded", "local_save", "_id", "delete_date")
+
+MMT_MMIRS_REQUIRED_KEYS = ['ra', 'dec', 'epoch', 'exposuretime', 'observationtype', 'numberexposures', 'filter','grating' \
+    ,'instrumentid','magnitude','maskid','objectid','onevisitpernight','pa','pm_dec','pm_ra','priority','slitwidth','slitwidthproperty','visits']
 MMT_REQUIRED_KEYS = ['ra', 'dec', 'epoch', 'exposuretime', 'observationtype', 'numberexposures', 'observationtype']
 
 def isInt(i):
     try:
         ret = int(i)
         return True
     except:
```

### Comparing `mmtapi-0.5.1/mmtapi/mmtapi.py` & `mmtapi-0.6.1/mmtapi/mmtapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,22 @@
-import os, json, requests, re
-from . import MMT_JSON_KEYS, MMT_REQUIRED_KEYS, isInt, isFloat
+import os, json, requests, re, time
+#import pymongo
+from pathlib import Path
+from . import MMT_JSON_KEYS, LOCAL_TARGET_KEYS, isInt, isFloat
+from .instruments.binospec import validate as bino_validate
+from .instruments.mmirs import validate as mmirs_validate
 from datetime import datetime
 
+#class mmt_database():
+#    def __init__(self, localport="27017", table='mmt_targets'):
+#        self.client = pymongo.MongoClient("mongodb://localhost:{}/".format(str(localport)))
+#        self.db = self.client['mmt_database']
+#        self.mmt_targets = self.db[table]
+
+
 class api():
 
     def __init__(self, target=None, token=None):
 
         self.base = 'https://scheduler.mmto.arizona.edu/APIv2'
         self.target = target
 
@@ -13,99 +24,85 @@
             self.token = os.getenv('MMT_API_TOKEN')
         else:
             self.token = token
 
         self.request = None
 
 
-    def __build_url(self):
+    def _build_url(self, params={}):
         assert self.target is not None, 'Target cannot be None'
         self.url = '{}/{}'.format(self.base, self.target)
+        for p in params:
+            if p in ['targetid', 'datafileid']:
+                self.url = '{}/{}'.format(self.url, params[p])
+            else:
+                self.url = '{}/{}/{}'.format(self.url, p, params[p])
 
 
-    def _post(self, d_json):
-        self.__build_url()
-        self.request = requests.post(self.url, json=d_json)
-
-
-    def _get(self, d_json):
-        self.__build_url()
-        r = requests.get(self.url+'/'+str(d_json['targetid']))
-        self.request = r
-        return r
-
-
-    def _put(self, d_json):
-        self.__build_url()
-        self.request = requests.put(self.url+'/'+str(d_json['targetid']), json=d_json)
+    def _post(self, r_json):
+        self._build_url(r_json['urlparams'])
+        data = r_json['data'] if 'data' in r_json.keys() else None
+        files = r_json['files'] if 'files' in r_json.keys() else None
+        d_json = r_json['d_json'] if 'd_json' in r_json.keys() else None
+        self.request = requests.post(self.url, json=d_json, data=data, files=files)
         return self.request
 
 
-    def _delete(self, d_json):
-        self.__build_url()
-        self.request = requests.delete(self.url+'/'+str(d_json['targetid']))
-
-
-    def _post_finder(self, data, files):
-        self.__build_url()
-        self.request = requests.post(self.url+'/'+str(data['target_id']), data=data, files=files)
-
+    def _get(self, r_json):
+        self._build_url(r_json['urlparams'])
+        d_json = r_json['d_json'] if 'd_json' in r_json.keys() else None
+        self.request = requests.get(self.url, json=d_json)
+        return self.request
 
-    def get_instruments(self, date=None, instrumentid=None):
 
-        if date is None and instrumentid is None:
-            date = datetime.now()
+    def _put(self, r_json):
+        self._build_url(r_json['urlparams'])
+        d_json = r_json['d_json']
+        self.request = requests.put(self.url, json=d_json)
+        return self.request
 
-        self.url = 'https://scheduler.mmto.arizona.edu/APIv2/trimester//schedule/all'
-        self.request = requests.get(self.url)
 
-        schedule = json.loads(self.request.text)
-        published_queues = schedule['published']['queues']
-        ret = []
-
-        for pq in published_queues:
-            start = datetime.strptime(pq['queueruns'][0]['startdate'], '%Y-%m-%d %H:%M:%S-%f')
-            end = datetime.strptime(pq['queueruns'][0]['enddate'], '%Y-%m-%d %H:%M:%S-%f')
-            instid = pq['instrumentid']
-            queuename = pq['name']
-            for qr in pq['queueruns']:
-                start = datetime.strptime(qr['startdate'], '%Y-%m-%d %H:%M:%S-%f')
-                end = datetime.strptime(qr['enddate'], '%Y-%m-%d %H:%M:%S-%f')
-                if instrumentid is None and (date > start and date < end):
-                    ret.append({'instrumentid':instid, 'name':queuename, 'start': start, 'end': end})
-                if date is None and (instrumentid == int(instid)):
-                    ret.append({'instrumentid':instid, 'name':queuename, 'start': start, 'end': end})
+    def _delete(self, r_json):
+        self._build_url(r_json['urlparams'])
+        d_json = r_json['d_json']
+        self.request = requests.delete(self.url, json=d_json)
+        return self.request
 
-        ret = sorted(ret, key=lambda i: i['start'])
-        return ret
 
 class Target(api):
     def __init__(self, token=None, verbose=True, payload={}):
-
         self.verbose = verbose
         self.valid = False
+        self.downloaded = False
+        self.partial_download = False
+        self.message = {
+            'Errors':[],
+            'Warnings':[]
+        }
 
         assert token is not None, 'Token cannot be None'
         super().__init__('catalogTarget', token)
 
         allowed_keys = list(MMT_JSON_KEYS)
         self.__dict__.update((str(key).lower(), value) for key, value in payload.items() if str(key).lower() in allowed_keys)
 
         if 'targetid' in payload.keys():
             self.targetid = payload['targetid']
+            self.id = payload['targetid']
             self.get()
+            #self.database_load()
 
         self.validate(verbose=self.verbose)
 
+
     def validate(self, verbose=True):
         selfkeys = self.__dict__.keys()
         selfdict = self.__dict__
         errors, warnings = [], []
 
-        #validating required keys
         if 'ra' in selfkeys:
             ra = selfdict['ra']
             r = re.compile('.{2}:.{2}:.{2}\.*')
             if not r.match(ra):
                 errors.append('Invalid format for field \'ra\' ['+ra+']. Valid format is dd:dd:dd.d')
         else:
             errors.append('Field \'ra\' is required. Valid format is dd:dd:dd.d')
@@ -122,106 +119,27 @@
                 errors.append('Invalid format for field \'dec\' ['+dec+']. Valid format is [+/-]dd:dd:dd.d')
             dec = '-' + dec if isNeg else '+' + dec
             self.__dict__.update({'dec':dec})
 
         else:
             errors.append('Field \'dec\' is required. Valid format is [+/-]dd:dd:d.d')
 
-        if 'observationtype' in selfkeys:
-            observationtype = selfdict['observationtype']
-            if observationtype not in ['longslit', 'imaging', 'mask']:
-                errors.append('Field \' observationtype\' must be either \'imaging\', \'longslit\', or \'mask\'')
-            if observationtype == 'longslit':
-                if 'grating' in selfkeys:
-                    grating = selfdict['grating']
-                    if grating not in ['270', 270, '600', 600, '1000', 1000]:
-                        errors.append('For observationtype longslit, valid options for field \'grating\' are \'270\', \'600\', and \'1000\'')
-                    if 'centralwavelength' in selfkeys:
-                        centralwavelength = selfdict['centralwavelength']
-                        if isFloat(centralwavelength):
-                            cw = float(centralwavelength)
-                            if grating in ['270', 270] and not (cw >= 5501 and cw <= 7838):
-                                errors.append('For \'grating\' = 270: valid centralwavelength ['+str(centralwavelength)+'] must be between 5501-7838 Angstroms')
-                            if grating in ['600', 600] and not (cw >= 5146 and cw <= 8783):
-                                errors.append('For \'grating\' = 600: valid centralwavelength ['+str(centralwavelength)+'] must be between 5501-7838 Angstroms')
-                            if grating in ['1000', 1000] and not ((cw >= 4108 and cw <= 4683) or (cw >= 5181 and cw <= 7273) or (cw >= 7363 and cw <= 7967) or (cw >= 8153 and cw <= 8772) or (cw >= 8897 and cw <= 9279)):
-                                errors.append('For \'grating\' = 1000: valid centralwavelength must be between 4108-4683, 5181-7273, 7363-7967, 8153-8772 or 8897-9279')
-                        else:
-                            errors.append('Field \'centralwavelength\' must be float')
-                    else:
-                        errors.append('For observationtype: longslit, field \'centralwavelength\' is required \n \
-                            Valid options are dependent on the field \'grating\' \n \
-                            \'grating\' = 270: valid centralwavelength must be between 5501-7838 Angstroms \n \
-                            \'grating\' = 600: valid centralwavelength must be between 5146-8783 Angstroms \n \
-                            \'grating\' = 1000: valid centralwavelength must be between 4108-4683, 5181-7273, 7363-7967, 8153-8772 or 8897-9279')
-
-                else:
-                    errors.append('Field \'grating\' is required for observationtype: longslit \n \
-                        Valid options are \'270\', \'600\', and \'1000\'')
-
-                if 'slitwidth' in selfkeys:
-                    slitwidth = selfdict['slitwidth']
-                    if slitwidth not in ['Longslit0_75', 'Longslit1', 'Longslit1_25', 'Longslit1_5', 'Longslit5']:
-                        errors.append('Field \'slitwidth\' valid options are: Longslit0_75, Longslit1, Longslit1_25, Longslit1_5, and Longslit5')
-                else:
-                    errors.append('For observationtype: longslit, field \'slitwidth\' is required. Valid options are: Longslit0_75, Longslit1, Longslit1_25, Longslit1_5, and Longslit5')
-
-
-            if observationtype == 'imaging':
-                self.__dict__.update({'centralwavelength':None})
-                self.__dict__.update({'grating':None})
-
-            if 'filter' in selfkeys:
-                filt = selfdict['filter']
-                if observationtype == 'imaging' and filt not in ['g', 'r', 'i', 'z']:
-                    errors.append('For observationtype: imaging, valid options for field \'filter\' are: \'g\', \'r\', \'i\', and \'z\'.')
-                if observationtype == 'longslit' and filt not in ['LP3800', 'LP3500']:
-                    warnings.append('For observationtype: longslit, valid options for field \'filter\' are: \'LP3800\' and \'LP3500\' \n \
-                                    Default setting \'filter\' to \'LP3800\'')
-            else:
-                if observationtype == 'longslit':
-                    self.__dict__.update({'filter':'LP3800'})
-                errors.append('Field \'filter\' is required for observation types \'imaging\' and \'longslit\' \n \
-                               For imaging: valid options are \'g\', \'r\', \'i\', and \'z\'. \n \
-                               For longslit: valid options are \'LP3800\' (default) and \'LP3500\'')
-
-            if 'onevisitpernight' not in selfkeys:
-                if observationtype == 'imaging':
-                    self.__dict__.update({'onevisitpernight':0})
-                if observationtype == 'longslit':
-                    self.__dict__.update({'onevisitpernight':1})
-            else:
-                onevisitpernight = selfdict['onevisitpernight']
-                if onevisitpernight not in [0, 1]:
-                    errors.append('Field \'onevisitpernight\' must be either 0 or 1')
-
-        else:
-            errors.append('Field \'observationtype\' is required. Valid values are \'longslit\', \'imaging\', and \'mask\'')
-
         if 'epoch' not in selfkeys:
             warnings.append('Field \'epoch\' default set to 2000.0')
-            self.__dict__.update({'epoch':2000.0})
+            self.__dict__.update({'epoch':'J2000'})
 
         if 'exposuretime' in selfkeys:
             exposuretime = selfdict['exposuretime']
             if not isInt(exposuretime):
                 errors.append('Field \'exposuretime\' valid format is integer (seconds)')
             elif not int(exposuretime) > 0:
                 errors.append('Field \'exposuretime\' must be greater than zero you dingus')
         else:
             errors.append('Field \'exposuretime\' is required. Valid format is integer (seconds)')
 
-        if 'instrumentid' in selfkeys:
-            instrumentid = selfdict['instrumentid']
-            if instrumentid not in [16, '16']:
-                errors.append('Only supported instrument is Binospec: instrumentid=16')
-        else:
-            warnings.append('Only supported instrument right now is Binospec: setting instrumentid to 16')
-            self.__dict__.update({'instrumentid':'16'})
-
         if 'magnitude' in selfkeys:
             magnitude = selfdict['magnitude']
             if not isFloat(magnitude):
                 errors.append('Invalid format for field \'magnitude\'. Must be decimal/float')
         else:
             errors.append('Field \'magnitude\' is required for requested Target')
 
@@ -316,16 +234,38 @@
             if not isInt(too):
                 errors.append('Field \'targetofopportunity\' must be integer. \n \
                     0 = not a target of opportunity. \n \
                     1 = target of opportunity.')
         else:
             self.__dict__.update({'targetofopportunity':0})
 
+        #validating required keys
+        if 'instrumentid' in selfkeys:
+            instrumentid = selfdict['instrumentid']
+
+            #Binospec
+            if instrumentid in [16,'16']:
+                inst_errors, inst_warnings, inst_dict = bino_validate(selfdict)
+                errors.extend(inst_errors)
+                warnings.extend(inst_warnings)
+                self.__dict__.update(inst_dict)
+
+            #MMIRS...
+            if instrumentid in [15,'15']:
+                inst_errors, inst_warnings, inst_dict = mmirs_validate(selfdict)
+                errors.extend(inst_errors)
+                warnings.extend(inst_warnings)
+                self.__dict__.update(inst_dict)
+
+        else:
+            errors.append('Only supported instrument right now is Binospec and MMIRS: Please choose an instrument id')
+            #self.__dict__.update({'instrumentid':'16'})
+
         #Settings for limiting to only Binospec
-        self.__dict__.update({'dithersize':None, 'gain':None, 'grism':None, 'moon':None, 'readtab':None})
+        #self.__dict__.update({'dithersize':None, 'gain':None, 'grism':None, 'moon':None, 'readtab':None})
 
         #Validate instrument on the telescope
         #current_instruments = self.get_instruments()
         #if any(int(ci['instrumentid']) == 16 for ci in current_instruments):
         #    if 'targetofopportunity' not in selfkeys:
         #        self.__dict__.update({'targetofopportunity':1})
         #    if 'priority' not in selfkeys:
@@ -336,14 +276,19 @@
         #    warnings.append('Binospec is currently not on the MMT!\n \
         #        Setting Field: \'targetofopportunity\' to 0\n \
         #        Setting Field \'priority\' to 3\n \
         #        Envoke target.api.get_instruments(instrumentid=16) to see when the next start date is for Binospec')
 
         #Print out Errors and Warnings
         self.valid = (len(errors) == 0)
+        self.message = {
+            'Errors':errors,
+            'Warnings':warnings
+        }
+
         if self.verbose:
             if not self.valid:
                 print('INPUT TARGET ERRORS: ')
                 for e in errors:
                     print(e)
                 print()
             if len(warnings) > 0:
@@ -363,83 +308,290 @@
         self.__dict__.update((key, value) for key, value in kwargs.items() if key in MMT_JSON_KEYS)
         self.validate()
 
         if self.valid:
             kwargs['targetid'] = self.__dict__['id']
             kwargs['token'] = self.token
 
-            self._put(kwargs)
+            data = {
+                'urlparams':{
+                    'targetid':self.__dict__['id']
+                },
+                'd_json':kwargs
+            }
+
+            self._put(r_json=data)
             r = self.request
             print(json.loads(r.text), r.status_code)
 
             if r.status_code == 200:
                 self.__dict__.update((key, value) for key, value in json.loads(r.text).items())
             else:
                 print('Something went wrong with the request. Envoke target.request to see request information')
         else:
             print('Invalid Target. Envoke target.validate() to see errors')
 
 
     def delete(self):
         data = {
-            'token':self.token,
-            'targetid':self.__dict__['id']
+            'urlparams':{
+                'targetid':self.__dict__['id']
+            },
+            'd_json':{
+                'token':self.token
+            }
         }
-        self._delete(d_json=data)
-        r = self.request
+        r = self._delete(r_json=data)
         if r.status_code == 200:
             print("Succesfully Deleted")
         else:
             print('Something went wrong with the request. Envoke target.request to see request information')
         if self.verbose:
             print(json.loads(r.text), r.status_code)
 
 
     def post(self):
         if self.valid:
             payload = dict((key, value) for key, value in self.__dict__.items() if key in MMT_JSON_KEYS)
             payload['token'] = self.token
-            self._post(payload)
-            r = self.request
+            data = {
+                'urlparams':{},
+                'data':None,
+                'files':None,
+                'd_json':payload,
+            }
+            r = self._post(r_json=data)
+
             if self.verbose:
                 print(json.loads(r.text), r.status_code)
             if r.status_code == 200:
                     self.__dict__.update((key, value) for key, value in json.loads(r.text).items())
+                    self.targetid = self.id
             else:
                 print('Something went wrong with the request. Envoke target.request to see request information')
         else:
             print('Invalid Target parameters. Envoke target.validate() to see errors')
 
+
     def get(self):
         data = {
-            'token':self.token,
-            'targetid':self.__dict__['targetid']
+            'urlparams': {
+                'targetid':self.__dict__['targetid']
+            },
+            'd_json':{
+                'token':self.token
+            },
         }
-        self._get(d_json=data)
-        request = self.request
+        request = self._get(r_json=data)
         r = json.loads(request.text)
         if request.status_code == 200:
             self.__dict__.update((key, value) for key, value in r.items())
         else:
             print('Something went wrong with the request. Envoke target.request to see request information')
 
 
     def upload_finder(self, finder_path):
         if self.valid:
+            if isinstance(finder_path, str):
+                finder_file = open(finder_path, 'rb')
+            else:  # if it's already a file object (e.g., from Django)
+                finder_file = finder_path.open('rb')
             data = {
-                'type':'finding_chart',
-                'token':self.token,
-                'target_id':str(self.__dict__['id']),
-            }
-
-            files = {
-                'finding_chart_file': open(finder_path, 'rb')
+                'urlparams': {
+                    'targetid':self.__dict__['targetid']
+                },
+                'data':{
+                    'type':'finding_chart',
+                    'token':self.token,
+                    'target_id':str(self.__dict__['id']),
+                },
+                'files':{
+                    'finding_chart_file': finder_file
+                },
+                'd_json':None
             }
-
-            self._post_finder(data, files)
-            r = self.request
+            r = self._post(r_json=data)
             if r.status_code == 200:
                 self.__dict__.update((key, value) for key, value in json.loads(r.text).items())
             else:
                 print('Something went wrong with the request. Envoke target.request to see request information')
             if self.verbose:
                 print(json.loads(r.text), r.status_code)
+
+
+    def download_exposures(self, force=False):
+        # also check the headers for the individual exposure times adding up to the total requested from api.get(targetid) method
+        # to decide if it is done
+        if (self.valid and self.iscomplete != 1) or force:
+            self.datalist = Datalist(token=self.token)
+            self.datalist.get(targetid=self.__dict__['id'])
+
+            parentdir = self.parentdir if 'parentdir' in self.__dict__.keys() else os.getcwd()
+            print('Length of datalist {}'.format(len(self.datalist.data)))
+            if len(self.datalist.data):
+                for d in self.datalist.data:
+                    name = d['name']
+                    datafiles = d['datafiles']
+                    for df in datafiles:
+                        ftype = df['type']
+                        filepath = '{}/data/{}/{}/{}'.format(parentdir, self.objectid, name, ftype)
+                        Path(filepath).mkdir(parents=True, exist_ok=True)
+                        datafileid = df['id']
+                        filename = df['filename']
+                        download_file = '{}/{}'.format(filepath, filename)
+
+                        if not os.path.exists(download_file):
+                            if self.verbose:
+                                print('Downloading: {}'.format(download_file))
+                            im = Image(token=self.token)
+                            im.get(datafileid=datafileid, filepath=download_file)
+                            self.partial_download = True
+
+                        else:
+                            if self.verbose:
+                                print('File \'{}\' already exists'.format(download_file))
+                                self.partial_download = True
+
+                self.downloaded = True
+                self.partial_download = False
+
+            #else:
+            #    if self.verbose:
+            #        print('Exposures have been take, but are not ready for download')
+
+            else:
+                if self.verbose:
+                    print('Exposures not taken yet.')
+        else:
+            if self.verbose:
+                print('Exposure is completed')
+
+
+class Instruments(api):
+    def __init__(self, token=None, verbose=True, payload={}):
+        self. verbose = verbose
+        super().__init__('trimester//schedule/all/', token)
+
+    def get_instruments(self, date=None, instrumentid=None, getAll=False):
+        if date is None and instrumentid is None:
+            date = datetime.now()
+
+        r_json = {
+            'urlparams':{},
+            'd_json':{
+                'token':self.token
+            }
+        }
+
+        self._get(r_json=r_json)
+
+        schedule = json.loads(self.request.text)
+        published_queues = schedule['published']['queues']
+        ret = []
+
+        for pq in published_queues:
+            start = datetime.strptime(pq['queueruns'][0]['startdate'], '%Y-%m-%d %H:%M:%S-%f')
+            end = datetime.strptime(pq['queueruns'][0]['enddate'], '%Y-%m-%d %H:%M:%S-%f')
+            instid = pq['instrumentid']
+            queuename = pq['name']
+            for qr in pq['queueruns']:
+                start = datetime.strptime(qr['startdate'], '%Y-%m-%d %H:%M:%S-%f')
+                end = datetime.strptime(qr['enddate'], '%Y-%m-%d %H:%M:%S-%f')
+                if getAll:
+                    ret.append({'instrumentid':instid, 'name':queuename, 'start': start, 'end': end})
+                else:
+                    if instrumentid is None and (date > start and date < end):
+                        ret.append({'instrumentid':instid, 'name':queuename, 'start': start, 'end': end})
+                    if date is None and (instrumentid == int(instid)):
+                        ret.append({'instrumentid':instid, 'name':queuename, 'start': start, 'end': end})
+
+        ret = sorted(ret, key=lambda i: i['start'])
+        if self.verbose:
+            for r in ret:
+                print(r)
+        return ret
+
+
+class Datalist(api):
+    def __init__(self, token=None, verbose=True, payload={}):
+        self.verbose = verbose
+        self.data = []
+        super().__init__('data/list/catalogtarget', token)
+
+
+    def get(self, targetid, data_type='raw'):
+        assert data_type in ['raw', 'reduced'], 'data_type must either be raw or reduced'
+        r_json = {
+            'urlparams':{
+                'targetid':targetid,
+                'token':self.token,
+                'type':data_type
+            }
+        }
+
+        self._get(r_json=r_json)
+
+        if self.request.status_code == 200:
+            self.data = self.request.json()
+        else:
+            print('Datalist request error')
+
+
+class Image(api):
+    def __init__(self, token=None, verbose=True, payload={}):
+        self. verbose = verbose
+        super().__init__('data/download/datafile', token)
+
+
+    def get(self, datafileid=None, filepath=os.getcwd()):
+
+        assert datafileid is not None, 'datafileid cannot be None'
+        r_json = {
+            'urlparams':{
+                'datafileid':datafileid,
+                'token':self.token
+            }
+        }
+
+        self._get(r_json=r_json)
+
+        if self.request.status_code == 200:
+            if self.verbose:
+                print('Writing file.')
+            open(filepath, 'wb').write(self.request.content)
+            self.request = None
+        else:
+            print('Image download request error')
+
+
+class Listener():
+    def __init__(self, token=None, targetid=None):
+        assert token is not None, 'token cannot be None'
+        assert targetid is not None, 'targetid cannot be None'
+        self.token = token
+        self.targets = []
+        self.targets.append(Target(token=self.token, payload={'targetid':targetid})) 
+        #self.listener_log = payload['logpath'] if 'logpath' in payload.keys() else os.getcwd()
+
+    def listen(self, Force=True):
+
+        start_time = datetime.now()
+        all_downloaded = all([x.downloaded for x in self.targets])
+
+        run_listener = not all_downloaded or Force
+
+        while run_listener:
+
+            for t in self.targets:
+                t.get()
+                print(t.objectid)
+                t.download_exposures(force=Force)
+
+            run_listener = not all([x.downloaded for x in self.targets])
+
+            if run_listener:
+                print("Sleeping for 60s")
+                time.sleep(60)
+            else:
+                print('Download finished :)')
+
+        pass
```

### Comparing `mmtapi-0.5.1/mmtapi/test.py` & `mmtapi-0.6.1/mmtapi/test.py`

 * *Files identical despite different names*

### Comparing `mmtapi-0.5.1/setup.py` & `mmtapi-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mmtapi", # Replace with your own username
-    version="0.5.1",
+    version="0.6.1",
     author="Samuel Wyatt",
     author_email="swyatt@email.arizona.edu",
     description="An API wrapper for uploading Targets to the MMT observation queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/swyatt7/mmtapi",
     packages=setuptools.find_packages(),
```

