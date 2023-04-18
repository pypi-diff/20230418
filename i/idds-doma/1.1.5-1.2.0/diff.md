# Comparing `tmp/idds-doma-1.1.5.tar.gz` & `tmp/idds-doma-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-1.1.5.tar", last modified: Sat Mar  4 21:39:59 2023, max compression
+gzip compressed data, was "idds-doma-1.2.0.tar", last modified: Tue Apr 18 09:36:55 2023, max compression
```

## Comparing `idds-doma-1.1.5.tar` & `idds-doma-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-04 21:39:47.000000 idds-doma-1.1.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-04 21:39:59.901644 idds-doma-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-04 21:39:47.000000 idds-doma-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-03-04 21:39:47.000000 idds-doma-1.1.5/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-03-04 21:39:47.000000 idds-doma-1.1.5/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-doma-1.1.5/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-doma-1.1.5/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-04 21:39:54.000000 idds-doma-1.1.5/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-doma-1.1.5/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-03-04 21:39:47.000000 idds-doma-1.1.5/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-doma-1.1.5/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67908 2023-03-04 21:39:47.000000 idds-doma-1.1.5/lib/idds/doma/workflowv2/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-04 21:39:59.000000 idds-doma-1.1.5/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-04 21:39:59.000000 idds-doma-1.1.5/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 21:39:59.000000 idds-doma-1.1.5/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-04 21:39:59.000000 idds-doma-1.1.5/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-04 21:39:59.000000 idds-doma-1.1.5/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 21:39:59.905644 idds-doma-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-03-04 21:39:47.000000 idds-doma-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.901644 idds-doma-1.1.5/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-04 21:39:54.000000 idds-doma-1.1.5/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.531023 idds-doma-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 09:36:40.000000 idds-doma-1.2.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 09:36:55.531023 idds-doma-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 09:36:40.000000 idds-doma-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.527023 idds-doma-1.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-18 09:36:40.000000 idds-doma-1.2.0/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-18 09:36:40.000000 idds-doma-1.2.0/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.527023 idds-doma-1.2.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.527023 idds-doma-1.2.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-doma-1.2.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.527023 idds-doma-1.2.0/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-doma-1.2.0/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 09:36:49.000000 idds-doma-1.2.0/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.527023 idds-doma-1.2.0/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-doma-1.2.0/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-18 09:36:40.000000 idds-doma-1.2.0/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.527023 idds-doma-1.2.0/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-doma-1.2.0/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-18 09:36:40.000000 idds-doma-1.2.0/lib/idds/doma/workflowv2/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.531023 idds-doma-1.2.0/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 09:36:55.000000 idds-doma-1.2.0/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-18 09:36:55.000000 idds-doma-1.2.0/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:36:55.000000 idds-doma-1.2.0/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 09:36:55.000000 idds-doma-1.2.0/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 09:36:55.000000 idds-doma-1.2.0/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 09:36:55.531023 idds-doma-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-18 09:36:40.000000 idds-doma-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.527023 idds-doma-1.2.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:55.531023 idds-doma-1.2.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-18 09:36:49.000000 idds-doma-1.2.0/tools/env/environment.yml
```

### Comparing `idds-doma-1.1.5/LICENSE.rst` & `idds-doma-1.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-1.1.5/PKG-INFO` & `idds-doma-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.1.5
+Version: 1.2.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.1.5/bin/setup_panda_token` & `idds-doma-1.2.0/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-1.1.5/bin/setup_panda_token.py` & `idds-doma-1.2.0/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.1.5/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-1.2.0/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.1.5/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-1.2.0/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files 0% similar despite different names*

```diff
@@ -473,29 +473,33 @@
 
         :param input_output_maps: new maps from inputs to outputs.
         """
         # avoid duplicated task name
         self.task_name = self.task_name + "_" + str(self.get_request_id()) + "_" + str(self.get_work_id())
 
         in_files = []
+        has_dependencies = False
         if self.dependency_map is None:
             self.dependency_map = {}
         for job in self.dependency_map:
             in_files.append(job['name'])
+            if not has_dependencies and "dependencies" in job and job['dependencies']:
+                has_dependencies = True
 
         task_param_map = {}
         task_param_map['vo'] = self.vo
         if self.task_queue and len(self.task_queue) > 0:
             task_param_map['site'] = self.task_queue
         elif self.queue and len(self.queue) > 0:
             task_param_map['site'] = self.queue
         task_param_map['workingGroup'] = self.working_group
         task_param_map['nFilesPerJob'] = 1
         if in_files:
-            task_param_map['inputPreStaging'] = True
+            if has_dependencies:
+                task_param_map['inputPreStaging'] = True
             task_param_map['nFiles'] = len(in_files)
             task_param_map['noInput'] = True
             task_param_map['pfnList'] = in_files
         else:
             # task_param_map['inputPreStaging'] = True
             in_files = ['pseudo_file']
             task_param_map['nFiles'] = len(in_files)
@@ -928,15 +932,15 @@
         for map_id in input_output_maps:
             inputs = input_output_maps[map_id]['inputs']
             outputs = input_output_maps[map_id]['outputs']
             for content in outputs:
                 if content['substatus'] in [ContentStatus.Available]:
                     if 'panda_id' in content['content_metadata']:
                         finished_jobs.append(content['content_metadata']['panda_id'])
-                elif content['substatus'] in [ContentStatus.Failed, ContentStatus.FinalFailed,
+                elif content['substatus'] in [ContentStatus.FinalFailed,
                                               ContentStatus.Lost, ContentStatus.Deleted,
                                               ContentStatus.Missing]:
                     if 'panda_id' in content['content_metadata']:
                         failed_jobs.append(content['content_metadata']['panda_id'])
             for content in inputs:
                 inputname_mapid_map[content['name']] = {'map_id': map_id,
                                                         'outputs': outputs}
@@ -1024,25 +1028,30 @@
                                  'coll_id': content['coll_id'],
                                  'map_id': content['map_id'],
                                  'status': content['status']}
             for job_info_item in job_info_maps:
                 new_content_ext_d[job_info_item] = getattr(job_info, job_info_maps[job_info_item])
                 if new_content_ext_d[job_info_item] == 'NULL':
                     new_content_ext_d[job_info_item] = None
+                if new_content_ext_d[job_info_item] is None:
+                    del new_content_ext_d[job_info_item]
+
             new_contents_ext_d.append(new_content_ext_d)
 
         for content_id in update_contents_ext:
             content = update_contents_ext[content_id]['content']
             job_info = update_contents_ext[content_id]['job_info']
             update_content_ext_d = {'content_id': content['content_id'],
                                     'status': content['status']}
             for job_info_item in job_info_maps:
                 update_content_ext_d[job_info_item] = getattr(job_info, job_info_maps[job_info_item])
                 if update_content_ext_d[job_info_item] == 'NULL':
                     update_content_ext_d[job_info_item] = None
+                if update_content_ext_d[job_info_item] is None:
+                    del update_content_ext_d[job_info_item]
 
             update_contents_ext_d.append(update_content_ext_d)
 
         return new_contents_ext_d, update_contents_ext_d
 
     def get_contents_ext(self, input_output_maps, contents_ext, contents_ext_full, job_info_maps={}):
         self.logger.debug("get_contents_ext, len(contents_ext): %s" % (str(len(contents_ext))))
@@ -1101,15 +1110,15 @@
         for content_id in update_need_poll_contents_ext:
             left_contents.append(update_need_poll_contents_ext[content_id])
 
         new_contents_ext_d, update_contents_ext_d = self.get_contents_ext_detail(new_contents_ext, update_contents_ext, job_info_maps)
 
         self.logger.debug("get_contents_ext, new_contents_ext_d[:1]: %s" % (str(new_contents_ext_d[:1])))
         self.logger.debug("get_contents_ext, update_contents_ext_d[:1]: %s" % (str(update_contents_ext_d[:1])))
-        self.logger.debug("get_contents_ext, left_contents[:3]: %s" % (str(left_contents[:3])))
+        self.logger.debug("get_contents_ext, left_contents[:1]: %s" % (str(left_contents[:3])))
         return new_contents_ext_d, update_contents_ext_d, left_contents
 
     def poll_panda_task(self, processing=None, input_output_maps=None, contents_ext=None, job_info_maps={}, log_prefix=''):
         task_id = None
         try:
             from pandaclient import Client
```

### Comparing `idds-doma-1.1.5/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-1.2.0/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.1.5
+Version: 1.2.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.1.5/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-1.2.0/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-doma-1.1.5/setup.py` & `idds-doma-1.2.0/setup.py`

 * *Files identical despite different names*

