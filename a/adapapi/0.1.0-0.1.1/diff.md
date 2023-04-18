# Comparing `tmp/adapapi-0.1.0.tar.gz` & `tmp/adapapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapapi-0.1.0.tar", last modified: Wed Jan 18 18:04:43 2023, max compression
+gzip compressed data, was "adapapi-0.1.1.tar", last modified: Tue Apr 18 15:34:27 2023, max compression
```

## Comparing `adapapi-0.1.0.tar` & `adapapi-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gerald     (503) staff       (20)        0 2023-01-18 18:04:43.307289 adapapi-0.1.0/
--rw-r--r--   0 gerald     (503) staff       (20)     8659 2023-01-18 18:04:43.307349 adapapi-0.1.0/PKG-INFO
--rw-r--r--   0 gerald     (503) staff       (20)     7978 2022-12-15 16:57:12.000000 adapapi-0.1.0/README.md
-drwxr-xr-x   0 gerald     (503) staff       (20)        0 2023-01-18 18:04:43.306546 adapapi-0.1.0/adapapi/
--rw-r--r--   0 gerald     (503) staff       (20)     1470 2021-02-08 23:15:04.000000 adapapi-0.1.0/adapapi/__init__.py
--rw-r--r--   0 gerald     (503) staff       (20)    32596 2023-01-18 17:22:19.000000 adapapi-0.1.0/adapapi/adapapi.py
-drwxr-xr-x   0 gerald     (503) staff       (20)        0 2023-01-18 18:04:43.307190 adapapi-0.1.0/adapapi.egg-info/
--rw-r--r--   0 gerald     (503) staff       (20)     8659 2023-01-18 18:04:43.000000 adapapi-0.1.0/adapapi.egg-info/PKG-INFO
--rw-r--r--   0 gerald     (503) staff       (20)      221 2023-01-18 18:04:43.000000 adapapi-0.1.0/adapapi.egg-info/SOURCES.txt
--rw-r--r--   0 gerald     (503) staff       (20)        1 2023-01-18 18:04:43.000000 adapapi-0.1.0/adapapi.egg-info/dependency_links.txt
--rw-r--r--   0 gerald     (503) staff       (20)       21 2023-01-18 18:04:43.000000 adapapi-0.1.0/adapapi.egg-info/requires.txt
--rw-r--r--   0 gerald     (503) staff       (20)        8 2023-01-18 18:04:43.000000 adapapi-0.1.0/adapapi.egg-info/top_level.txt
--rw-r--r--   0 gerald     (503) staff       (20)       38 2023-01-18 18:04:43.307584 adapapi-0.1.0/setup.cfg
--rw-r--r--   0 gerald     (503) staff       (20)     1019 2023-01-18 18:04:21.000000 adapapi-0.1.0/setup.py
+drwxr-xr-x   0 gerald     (503) staff       (20)        0 2023-04-18 15:34:27.346795 adapapi-0.1.1/
+-rw-r--r--   0 gerald     (503) staff       (20)     8659 2023-04-18 15:34:27.346882 adapapi-0.1.1/PKG-INFO
+-rw-r--r--   0 gerald     (503) staff       (20)     7978 2023-04-18 15:33:51.000000 adapapi-0.1.1/README.md
+drwxr-xr-x   0 gerald     (503) staff       (20)        0 2023-04-18 15:34:27.345878 adapapi-0.1.1/adapapi/
+-rw-r--r--   0 gerald     (503) staff       (20)     1470 2021-02-08 23:15:04.000000 adapapi-0.1.1/adapapi/__init__.py
+-rw-r--r--   0 gerald     (503) staff       (20)    32691 2023-04-18 15:28:19.000000 adapapi-0.1.1/adapapi/adapapi.py
+drwxr-xr-x   0 gerald     (503) staff       (20)        0 2023-04-18 15:34:27.346659 adapapi-0.1.1/adapapi.egg-info/
+-rw-r--r--   0 gerald     (503) staff       (20)     8659 2023-04-18 15:34:27.000000 adapapi-0.1.1/adapapi.egg-info/PKG-INFO
+-rw-r--r--   0 gerald     (503) staff       (20)      221 2023-04-18 15:34:27.000000 adapapi-0.1.1/adapapi.egg-info/SOURCES.txt
+-rw-r--r--   0 gerald     (503) staff       (20)        1 2023-04-18 15:34:27.000000 adapapi-0.1.1/adapapi.egg-info/dependency_links.txt
+-rw-r--r--   0 gerald     (503) staff       (20)       21 2023-04-18 15:34:27.000000 adapapi-0.1.1/adapapi.egg-info/requires.txt
+-rw-r--r--   0 gerald     (503) staff       (20)        8 2023-04-18 15:34:27.000000 adapapi-0.1.1/adapapi.egg-info/top_level.txt
+-rw-r--r--   0 gerald     (503) staff       (20)       38 2023-04-18 15:34:27.347249 adapapi-0.1.1/setup.cfg
+-rw-r--r--   0 gerald     (503) staff       (20)     1019 2023-04-18 15:33:25.000000 adapapi-0.1.1/setup.py
```

### Comparing `adapapi-0.1.0/PKG-INFO` & `adapapi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python package using Appen API
 Author: appenps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adapapi-0.1.0/README.md` & `adapapi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adapapi-0.1.0/adapapi/__init__.py` & `adapapi-0.1.1/adapapi/__init__.py`

 * *Files identical despite different names*

### Comparing `adapapi-0.1.0/adapapi/adapapi.py` & `adapapi-0.1.1/adapapi/adapapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,29 +137,31 @@
             int: New ADAP Job ID
         """
         params = {'all_units': str(include_uploaded_rows).lower(), 'gold': str(include_tq).lower()}
         response = requests.get(f'https://api.appen.com/v1/jobs/{job_id}/copy.json', params=params, headers = self.headers) if not self.eu else requests.get(f'https://api.eu.appen.com/v1/jobs/{job_id}/copy.json', params=params, headers = self.headers)
         if response.status_code != 200:
             log.error(f'---- Status code: {response.status_code} \n {response.text}')
         else:
-            return json.loads(response.text)
+            return json.loads(response.text)['id']
 
-    def update_job_json(self, job_id, indict):
+    def update_job_json(self, job_id, indict, title = None):
         """Updating job settings
 
         Args:
             job_id (int): ADAP Job ID
             indict (dict): Dictionary of items to update within job json
         """
         headers = {'content-type': 'application/json'}
         headers.update(self.headers)
         payload = {}
         payload.update({'job': indict})
         payload.update({'ignore_overlapping_names': 'true'})
- 
+        if title:
+            payload['job'].update({'title': title})
+        
         response = requests.put(f'https://api.appen.com/v1/jobs/{job_id}.json', data=json.dumps(payload), headers=headers) if not self.eu else requests.put(f'https://api.eu.appen.com/v1/jobs/{job_id}.json', data=json.dumps(payload), headers=headers)
         if response.status_code != 200:
             log.error(f'---- Status code: {response.status_code} \n {response.text}')
         else:
             read_response = json.loads(response.text)
             try:
                 updated_stuff = [k for k, v in payload['job'].items()]
@@ -479,20 +481,20 @@
             while True:
                 response = requests.get(f'https://api.appen.com/v1/jobs/{jid}.csv', params=params, headers=self.headers) if not self.eu else requests.get(f'https://api.eu.appen.com/v1/jobs/{jid}.csv', params=params, headers=self.headers)
                 counter += 1
                 log.info(f"-- Response: {response.status_code} -- Count:{counter}")
                 if response.status_code == 200:
                     log.info(f"-- Generation for job ID {jid} complete")
                     break
-                time.sleep(30)
+                time.sleep(2)
             response = requests.get(f'https://api.appen.com/v1/jobs/{jid}.csv', params=params, headers=self.headers) if not self.eu else requests.get(f'https://api.eu.appen.com/v1/jobs/{jid}.csv', params=params, headers=self.headers)
             while not response.ok:
                 log.error(f"Download Failed: Attempting re-download {params['type'].upper()} report {jid}")
                 response = requests.get(f'https://api.appen.com/v1/jobs/{jid}.csv', params=params, headers=self.headers) if not self.eu else requests.get(f'https://api.eu.appen.com/v1/jobs/{jid}.csv', params=params, headers=self.headers)
-                time.sleep(30)
+                time.sleep(2)
 
             fname = f'{params["type"]}_{jid}.zip'
             time_end = timeit.default_timer()
             elapsed_minutes = round((time_end - time_start) / 60, 2)
             log.info(f'Download complete for job {jid} Saving report as {fname} ---- Elapsed minutes: {elapsed_minutes}')
             with open(fname, 'wb') as f:
                 f.write(response.content)
```

### Comparing `adapapi-0.1.0/adapapi.egg-info/PKG-INFO` & `adapapi-0.1.1/adapapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python package using Appen API
 Author: appenps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adapapi-0.1.0/setup.py` & `adapapi-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='adapapi',
-    version='0.1.0',
+    version='0.1.1',
     description='A simple Python package using Appen API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='appenps',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

