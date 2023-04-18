# Comparing `tmp/idds-workflow-1.1.5.tar.gz` & `tmp/idds-workflow-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-workflow-1.1.5.tar", last modified: Sat Mar  4 21:39:59 2023, max compression
+gzip compressed data, was "idds-workflow-1.2.0.tar", last modified: Tue Apr 18 09:36:54 2023, max compression
```

## Comparing `idds-workflow-1.1.5.tar` & `idds-workflow-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.193634 idds-workflow-1.1.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/lib/idds/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflow/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflow/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-04 21:39:54.000000 idds-workflow-1.1.5/lib/idds/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    80253 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflow/work.py
--rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/lib/idds/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    81692 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/work.py
--rw-r--r--   0 runner    (1001) docker     (123)   102704 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/lib/idds/workflowv2/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/lib/idds_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-04 21:39:59.000000 idds-workflow-1.1.5/lib/idds_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-04 21:39:59.000000 idds-workflow-1.1.5/lib/idds_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 21:39:59.000000 idds-workflow-1.1.5/lib/idds_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-04 21:39:59.000000 idds-workflow-1.1.5/lib/idds_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-04 21:39:59.000000 idds-workflow-1.1.5/lib/idds_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-03-04 21:39:47.000000 idds-workflow-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:59.197634 idds-workflow-1.1.5/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-04 21:39:54.000000 idds-workflow-1.1.5/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.811010 idds-workflow-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-18 09:36:54.811010 idds-workflow-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.807010 idds-workflow-1.2.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.807010 idds-workflow-1.2.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.807010 idds-workflow-1.2.0/lib/idds/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflow/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflow/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 09:36:49.000000 idds-workflow-1.2.0/lib/idds/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80253 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflow/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.811010 idds-workflow-1.2.0/lib/idds/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81692 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103034 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/lib/idds/workflowv2/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.811010 idds-workflow-1.2.0/lib/idds_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-18 09:36:54.000000 idds-workflow-1.2.0/lib/idds_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 09:36:54.000000 idds-workflow-1.2.0/lib/idds_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:36:54.000000 idds-workflow-1.2.0/lib/idds_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 09:36:54.000000 idds-workflow-1.2.0/lib/idds_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 09:36:54.000000 idds-workflow-1.2.0/lib/idds_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 09:36:54.811010 idds-workflow-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-18 09:36:40.000000 idds-workflow-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.807010 idds-workflow-1.2.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:54.811010 idds-workflow-1.2.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 09:36:49.000000 idds-workflow-1.2.0/tools/env/environment.yml
```

### Comparing `idds-workflow-1.1.5/LICENSE.rst` & `idds-workflow-1.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/PKG-INFO` & `idds-workflow-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
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

### Comparing `idds-workflow-1.1.5/lib/idds/workflow/base.py` & `idds-workflow-1.2.0/lib/idds/workflow/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflow/datawork.py` & `idds-workflow-1.2.0/lib/idds/workflow/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflow/processingwork.py` & `idds-workflow-1.2.0/lib/idds/workflow/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflow/utils.py` & `idds-workflow-1.2.0/lib/idds/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflow/work.py` & `idds-workflow-1.2.0/lib/idds/workflow/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflow/workflow.py` & `idds-workflow-1.2.0/lib/idds/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflowv2/base.py` & `idds-workflow-1.2.0/lib/idds/workflowv2/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflowv2/datawork.py` & `idds-workflow-1.2.0/lib/idds/workflowv2/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflowv2/processingwork.py` & `idds-workflow-1.2.0/lib/idds/workflowv2/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflowv2/utils.py` & `idds-workflow-1.2.0/lib/idds/workflowv2/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflowv2/work.py` & `idds-workflow-1.2.0/lib/idds/workflowv2/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/lib/idds/workflowv2/workflow.py` & `idds-workflow-1.2.0/lib/idds/workflowv2/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -917,15 +917,16 @@
     def sync_global_parameters(self, global_parameters, sliced_global_parameters=None):
         gp = self.global_parameters
         for key in global_parameters:
             gp[key] = global_parameters[key]
         self.global_parameters = gp
 
     def sync_global_parameters_from_work(self, work):
-        self.log_debug("work %s (%s) is_terminated, global_parameters: %s" % (work.get_internal_id(), str(work), str(self.global_parameters)))
+        self.log_debug("work %s (%s) is_terminated, global_parameters: %s" % (work.get_internal_id(), str(work.metadata),
+                                                                              str(self.global_parameters)))
         if isinstance(work, Work):
             if self.global_parameters:
                 for key in self.global_parameters:
                     status, value = work.get_global_parameter_from_output_data(key)
                     self.log_debug("work %s get_global_parameter_from_output_data(key: %s) results(%s:%s)" % (work.get_internal_id(), key, status, value))
                     if status:
                         self.global_parameters[key] = value
@@ -1395,16 +1396,18 @@
 
     def add_next_work(self, work_id):
         next_works = self.next_works
         next_works.append(work_id)
         self.next_works = next_works
 
     def enable_next_works(self, work, cond):
-        self.log_debug("Checking Work %s condition: %s" % (work.get_internal_id(),
-                                                           json_dumps(cond, sort_keys=True, indent=4)))
+        # self.log_debug("Checking Work %s condition: %s" % (work.get_internal_id(),
+        #                                                   json_dumps(cond, sort_keys=True, indent=4)))
+        self.log_debug("Checking Work %s condition: %s" % (work.get_internal_id(), cond.get_internal_id()))
+
         # load_conditions should cover it.
         # if cond and self.is_class_method(cond.cond):
         #     # cond_work_id = self.works[cond.cond['idds_method_class_id']]
         #     cond.cond = getattr(work, cond.cond['idds_method'])
 
         self.log_info("Work %s condition: %s" % (work.get_internal_id(), cond.conditions))
         next_works = cond.get_next_works(trigger=ConditionTrigger.ToTrigger)
@@ -1677,16 +1680,18 @@
                 self.sync_global_parameters_from_work(work)
 
             if work.get_internal_id() in self.work_conds:
                 self.log_debug("Work %s has condition dependencies %s" % (work.get_internal_id(),
                                                                           json_dumps(self.work_conds[work.get_internal_id()], sort_keys=True, indent=4)))
                 for cond_id in self.work_conds[work.get_internal_id()]:
                     cond = self.conditions[cond_id]
-                    self.log_debug("Work %s has condition dependencie %s" % (work.get_internal_id(),
-                                                                             json_dumps(cond, sort_keys=True, indent=4)))
+                    # self.log_debug("Work %s has condition dependencie %s" % (work.get_internal_id(),
+                    #                                                          json_dumps(cond, sort_keys=True, indent=4)))
+                    self.log_debug("Work %s has condition dependencie %s" % (work.get_internal_id(), cond.get_internal_id()))
+
                     self.enable_next_works(work, cond)
 
             if work.is_terminated(synchronize=False):
                 self.log_info("Work %s is terminated(%s)" % (work.get_internal_id(), work.get_status()))
                 self.log_debug("Work conditions: %s" % json_dumps(self.work_conds, sort_keys=True, indent=4))
                 if work.get_internal_id() not in self.work_conds:
                     # has no next work
```

### Comparing `idds-workflow-1.1.5/lib/idds_workflow.egg-info/PKG-INFO` & `idds-workflow-1.2.0/lib/idds_workflow.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
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

### Comparing `idds-workflow-1.1.5/lib/idds_workflow.egg-info/SOURCES.txt` & `idds-workflow-1.2.0/lib/idds_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.1.5/setup.py` & `idds-workflow-1.2.0/setup.py`

 * *Files identical despite different names*

