# Comparing `tmp/pyunicoremanager-0.0.4.tar.gz` & `tmp/pyunicoremanager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/aaron/clonning/PyUnicoreManager/dist/tmp_5x1nrel/pyunicoremanager-0.0.4.tar", last modified: Fri Nov  4 15:08:57 2022, max compression
+gzip compressed data, was "dist/pyunicoremanager-0.0.5.tar", last modified: Mon Apr 17 13:49:45 2023, max compression
```

## Comparing `pyunicoremanager-0.0.4.tar` & `pyunicoremanager-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2022-11-04 15:08:57.257792 pyunicoremanager-0.0.4/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1075 2022-03-18 15:17:57.000000 pyunicoremanager-0.0.4/LICENSE
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2936 2022-11-04 15:08:57.257792 pyunicoremanager-0.0.4/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2487 2022-11-04 15:03:33.000000 pyunicoremanager-0.0.4/README.md
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       84 2022-03-17 16:37:08.000000 pyunicoremanager-0.0.4/pyproject.toml
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2022-11-04 15:08:57.253792 pyunicoremanager-0.0.4/pyunicoremanager/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2022-03-17 17:56:26.000000 pyunicoremanager-0.0.4/pyunicoremanager/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    24861 2022-11-04 15:03:33.000000 pyunicoremanager-0.0.4/pyunicoremanager/core.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2022-11-04 15:08:57.257792 pyunicoremanager-0.0.4/pyunicoremanager.egg-info/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2936 2022-11-04 15:08:57.000000 pyunicoremanager-0.0.4/pyunicoremanager.egg-info/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      255 2022-11-04 15:08:57.000000 pyunicoremanager-0.0.4/pyunicoremanager.egg-info/SOURCES.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2022-11-04 15:08:57.000000 pyunicoremanager-0.0.4/pyunicoremanager.egg-info/dependency_links.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       17 2022-11-04 15:08:57.000000 pyunicoremanager-0.0.4/pyunicoremanager.egg-info/top_level.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2022-11-04 15:08:57.257792 pyunicoremanager-0.0.4/setup.cfg
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      735 2022-11-04 15:03:33.000000 pyunicoremanager-0.0.4/setup.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      735 2023-04-17 13:48:48.000000 pyunicoremanager-0.0.5/setup.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/pyunicoremanager/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    24877 2023-04-17 13:48:48.000000 pyunicoremanager-0.0.5/pyunicoremanager/core.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2023-04-17 13:48:48.000000 pyunicoremanager-0.0.5/pyunicoremanager/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/setup.cfg
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/pyunicoremanager.egg-info/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/pyunicoremanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      232 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/pyunicoremanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       17 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/pyunicoremanager.egg-info/top_level.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3458 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/pyunicoremanager.egg-info/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2519 2023-04-17 13:48:48.000000 pyunicoremanager-0.0.5/README.md
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3458 2023-04-17 13:49:45.000000 pyunicoremanager-0.0.5/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyunicoremanager-0.0.4/PKG-INFO` & `pyunicoremanager-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,27 @@
-Metadata-Version: 2.1
-Name: pyunicoremanager
-Version: 0.0.4
-Summary: Python wrapper of PyUnicore to deploy jobs on UNICORE systems
-Home-page: https://github.com/aperezmartin/PyUnicoreManager
-Author: Aarón Pérez Martín
-Author-email: a.perez.martin@fz-juelich.de
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyUnicoreManager Library
 
 It is a Python wrapper of PyUnicore library (linked to UNICORE) that tries to minimize the lines of code and makes it flexible enough to be a interconnection piece of workflows. It is designed to be used from Notebooks of EBRAINS or a personal laptop with a LDAP authentication. In both cases, the user can launch jobs on the HPC systems, upload and download files and make complex workflow.
 
 Development of this library was funded in part by the Human Brain Project
 
 For more information about the Human Brain Project, see https://www.humanbrainproject.eu/
 
 See LICENSE file for licensing information
 
 # First steps
 
 Install it from Pypi:
 
+    pip install pyunicore==0.14.0
     pip install -U pyunicoremanager
     
 How to use it:
 
-    import pyunicoremanager.core import *
+    from pyunicoremanager.core import *
     
 
 # Important configuration for the framework
 For this example we use a certain Server with a particular partition and project, allocating 1 node for 10 minutes for a single job.
 
     setup={}
     setup["server"] = myServer
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyunicoremanager-0.0.4/pyunicoremanager/core.py` & `pyunicoremanager-0.0.5/pyunicoremanager/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
                 if (cmd_job.properties['status'] == "FAILED"):
                     raise Exception(str(result_job["stderr"]))
                 else:
                     logss.info('Job finished!')
             else:
                 logss.info('Job is running!. You could stop it!')
         except Exception as e:
-            logss.error(str(e))
+            logss.error("Job error:" + str(e))
             return None, None
         return cmd_job, result_job
 
     def uploadFiles(self, filesToUpload):
         try:
             if len(filesToUpload) == 0:
                 logss.info("Nothing to upload")
@@ -377,26 +377,27 @@
         #methods = [e.name for e in Method]
         
         
         #self.servers   = ["JUWELS","JUDAC","JUSUF","JURECA"] # "DAINT-CSCS", "CINECA-M100", "CINECA-MARCONI", "CINECA-G100'"
         #self.endpoints = ["HOME", "PROJECT",  "SCRATCH"]        
         #self.access_list = ['ACCESS_LDAP', 'ACCESS_COLLAB']
         #self.user_info = ""#pym.client.access_info()
+        queues = list(self.pym.client.get_compute()[0].get_queues().keys())
         
         self.user_info = {"username":self.pym.client.access_info()['xlogin']['UID'],
                          "email":self.pym.client.access_info()['dn'].split('=')[-1],
                          "projects":self.pym.client.access_info()['xlogin']['availableGroups'],
                          "def_project":self.pym.client.access_info()['xlogin']['group'],
-                         "queues":self.pym.client.access_info()['queues']['availableQueues'],
+                         "queues": queues,
                          "def_queue":self.pym.client.access_info()['queues']['selected']}
         #self.user = 'perezmartin1' #self.user_info['xlogin']['UID']
         #self.email= "a.perez.martin@fz-juelich.de" #self.user_info['dn'].split('=')[-1]
         #self.projects = ['cslns'] #self.user_info['xlogin']['availableGroups']
         #self.def_project='cslns'# self.user_info['group']
-        #self.queues = ['gpus', 'batch', 'develgpus']#self.user_info['queues']['availableQueues']
+        #self.queues = ['gpus', 'batch', 'develgpus'] #self.user_info['queues']['availableQueues']
         #self.def_queue = 'gpus'#self.user_info['queues']['selected']
         
     def change_children(self,obj):
 
         if not self.job_finish:
             if self.dashboard.children[0].selected_index == 0:
                 self.create_tab_2()
@@ -483,15 +484,15 @@
         self.setup["server_project"] = self.tabs[1][0].value
         
         # to fix the UNICORE naming  project_name != project_folder
         project_correction =""
         if self.setup["server_project"] in UNICORE_projects_errors.keys():
             project_correction = UNICORE_projects_errors[self.setup["server_project"]]
         else:
-            project_correction = UNICORE_projects_errors[self.setup["server_project"]]
+            project_correction = self.setup["server_project"]
         
         self.setup["JobArguments"] = {"Project": project_correction, 'Resources': {"Queue": self.tabs[1][1].value, "Nodes" : str(self.tabs[1][2].value),"Runtime" : str(int(self.tabs[1][3].value*100))+"m"}}
 
         self.progress_bar.value = 2   
         self.authentication = Authentication(token=self.token, access=self.access, server=self.setup['server'])
         self.pym = PyUnicoreManager(environment=Environment_UNICORE(auth=self.authentication, env_from_user= self.setup), clean_job_storages=False, verbose=self.verbose)
         self.progress_bar.value = 3
```

### Comparing `pyunicoremanager-0.0.4/pyunicoremanager.egg-info/PKG-INFO` & `pyunicoremanager-0.0.5/pyunicoremanager.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 Metadata-Version: 2.1
 Name: pyunicoremanager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python wrapper of PyUnicore to deploy jobs on UNICORE systems
 Home-page: https://github.com/aperezmartin/PyUnicoreManager
 Author: Aarón Pérez Martín
 Author-email: a.perez.martin@fz-juelich.de
+License: UNKNOWN
+Description: # PyUnicoreManager Library
+        
+        It is a Python wrapper of PyUnicore library (linked to UNICORE) that tries to minimize the lines of code and makes it flexible enough to be a interconnection piece of workflows. It is designed to be used from Notebooks of EBRAINS or a personal laptop with a LDAP authentication. In both cases, the user can launch jobs on the HPC systems, upload and download files and make complex workflow.
+        
+        Development of this library was funded in part by the Human Brain Project
+        
+        For more information about the Human Brain Project, see https://www.humanbrainproject.eu/
+        
+        See LICENSE file for licensing information
+        
+        # First steps
+        
+        Install it from Pypi:
+        
+            pip install pyunicore==0.14.0
+            pip install -U pyunicoremanager
+            
+        How to use it:
+        
+            from pyunicoremanager.core import *
+            
+        
+        # Important configuration for the framework
+        For this example we use a certain Server with a particular partition and project, allocating 1 node for 10 minutes for a single job.
+        
+            setup={}
+            setup["server"] = myServer
+            setup["server_endpoint"] = myPartition
+            setup["server_project"] = myProject folder
+            setup["JobArguments"] = {"Project": myProject name, 'Resources': {"Queue": myQueue, "Nodes" : "1","Runtime" : "10m"}}
+        
+        # Authentication from EBRAINS notebook on the HPC system
+        
+            authentication = Authentication(token=clb_oauth.get_token(), access=Method.ACCESS_COLLAB, server=setup['server'])
+        
+        # Authentication from personal PC on the HPC system
+        
+            myToken = Utils.generateToken(myLDAPuser, myLDAPpassword)
+            authentication = Authentication(token=myToken, access=Method.ACCESS_LDAP, server=setup['server'])
+        
+        # Environemnt for the framework
+        
+            env = Environment_UNICORE(auth=authentication, env_from_user=setup)
+           
+        # Instanciate the framework
+        
+        It would check if the jobs storage list is full, in that case would clean it up.
+        
+            pym = PyUnicoreManager(environment=env, clean_job_storages=True, verbose=False)
+        
+        # Launching a simple job
+        
+        All the job steps would be a list of command lines. The "job" object contains important information where the user can access later on. Each job has its Storage mapping and an unique identification number, in other words, jobs result can be accessible at any time. The "result" is a dictionary with the keys "stderr" and "stdout" and the whole output accumulated during the execution of the job.
+        
+            job_steps = ["ls -la","pwd"]
+            job, result= pym.one_run(steps=job_steps, parameters=setup["JobArguments"], wait_process=True)
+            print(result)
+            
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyUnicoreManager Library
-
-It is a Python wrapper of PyUnicore library (linked to UNICORE) that tries to minimize the lines of code and makes it flexible enough to be a interconnection piece of workflows. It is designed to be used from Notebooks of EBRAINS or a personal laptop with a LDAP authentication. In both cases, the user can launch jobs on the HPC systems, upload and download files and make complex workflow.
-
-Development of this library was funded in part by the Human Brain Project
-
-For more information about the Human Brain Project, see https://www.humanbrainproject.eu/
-
-See LICENSE file for licensing information
-
-# First steps
-
-Install it from Pypi:
-
-    pip install -U pyunicoremanager
-    
-How to use it:
-
-    import pyunicoremanager.core import *
-    
-
-# Important configuration for the framework
-For this example we use a certain Server with a particular partition and project, allocating 1 node for 10 minutes for a single job.
-
-    setup={}
-    setup["server"] = myServer
-    setup["server_endpoint"] = myPartition
-    setup["server_project"] = myProject folder
-    setup["JobArguments"] = {"Project": myProject name, 'Resources': {"Queue": myQueue, "Nodes" : "1","Runtime" : "10m"}}
-
-# Authentication from EBRAINS notebook on the HPC system
-
-    authentication = Authentication(token=clb_oauth.get_token(), access=Method.ACCESS_COLLAB, server=setup['server'])
-
-# Authentication from personal PC on the HPC system
-
-    myToken = Utils.generateToken(myLDAPuser, myLDAPpassword)
-    authentication = Authentication(token=myToken, access=Method.ACCESS_LDAP, server=setup['server'])
-
-# Environemnt for the framework
-
-    env = Environment_UNICORE(auth=authentication, env_from_user=setup)
-   
-# Instanciate the framework
-
-It would check if the jobs storage list is full, in that case would clean it up.
-
-    pym = PyUnicoreManager(environment=env, clean_job_storages=True, verbose=False)
-
-# Launching a simple job
-
-All the job steps would be a list of command lines. The "job" object contains important information where the user can access later on. Each job has its Storage mapping and an unique identification number, in other words, jobs result can be accessible at any time. The "result" is a dictionary with the keys "stderr" and "stdout" and the whole output accumulated during the execution of the job.
-
-    job_steps = ["ls -la","pwd"]
-    job, result= pym.one_run(steps=job_steps, parameters=setup["JobArguments"], wait_process=True)
-    print(result)
-
```

### Comparing `pyunicoremanager-0.0.4/setup.py` & `pyunicoremanager-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'curlify',
     'pyunicore',
     'psutil'
 ]
 
 setuptools.setup(
     name="pyunicoremanager",
-    version="0.0.4",
+    version="0.0.5",
     author="Aarón Pérez Martín",
     author_email="a.perez.martin@fz-juelich.de",
     description="Python wrapper of PyUnicore to deploy jobs on UNICORE systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aperezmartin/PyUnicoreManager",
     classifiers=[
```

