# Comparing `tmp/micado-client-0.12.0a1.tar.gz` & `tmp/micado-client-0.12.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micado-client-0.12.0a1.tar", last modified: Sun Mar  5 22:03:08 2023, max compression
+gzip compressed data, was "micado-client-0.12.0a2.tar", last modified: Mon Mar  6 12:39:20 2023, max compression
```

## Comparing `micado-client-0.12.0a1.tar` & `micado-client-0.12.0a2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.630326 micado-client-0.12.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-05 22:03:08.630326 micado-client-0.12.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.622326 micado-client-0.12.0a1/micado/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.626326 micado-client-0.12.0a1/micado/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/api/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.626326 micado-client-0.12.0a1/micado/installer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/installer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.626326 micado-client-0.12.0a1/micado/installer/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/installer/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/installer/ansible/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/installer/ansible/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.626326 micado-client-0.12.0a1/micado/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/launcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.626326 micado-client-0.12.0a1/micado/launcher/cloudbroker/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/launcher/cloudbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/launcher/cloudbroker/cloudbroker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.626326 micado-client-0.12.0a1/micado/launcher/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/launcher/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/launcher/openstack/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/launcher/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.626326 micado-client-0.12.0a1/micado/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/models/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/models/micado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.630326 micado-client-0.12.0a1/micado/types/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/types/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/types/micado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.630326 micado-client-0.12.0a1/micado/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/micado/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.630326 micado-client-0.12.0a1/micado_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-05 22:03:08.000000 micado-client-0.12.0a1/micado_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-05 22:03:08.000000 micado-client-0.12.0a1/micado_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:03:08.000000 micado-client-0.12.0a1/micado_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-05 22:03:08.000000 micado-client-0.12.0a1/micado_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-05 22:03:08.000000 micado-client-0.12.0a1/micado_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-05 22:03:08.000000 micado-client-0.12.0a1/micado_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 22:03:08.630326 micado-client-0.12.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:03:08.630326 micado-client-0.12.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-05 22:02:57.000000 micado-client-0.12.0a1/tests/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.402119 micado-client-0.12.0a2/micado/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/installer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/installer/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/ansible/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/ansible/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/launcher/cloudbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/cloudbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/cloudbroker/cloudbroker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/launcher/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/openstack/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/micado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/types/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/types/micado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/tests/test_auth.py
```

### Comparing `micado-client-0.12.0a1/LICENSE` & `micado-client-0.12.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/PKG-INFO` & `micado-client-0.12.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-client
-Version: 0.12.0a1
+Version: 0.12.0a2
 Summary: A Python Client Library for MiCADO
 Home-page: https://github.com/micado-scale/micado-client
 Author: Márk Emődi & Jay DesLauriers
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-client/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `micado-client-0.12.0a1/micado/api/application.py` & `micado-client-0.12.0a2/micado/api/application.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/api/client.py` & `micado-client-0.12.0a2/micado/api/client.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/cli.py` & `micado-client-0.12.0a2/micado/cli.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/client.py` & `micado-client-0.12.0a2/micado/client.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/exceptions.py` & `micado-client-0.12.0a2/micado/exceptions.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/installer/ansible/ansible.py` & `micado-client-0.12.0a2/micado/installer/ansible/ansible.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         )
 
         logger.info("Running playbook...")
         self._run_playbook(micado_id, hosts, extravars)
         self._check_port_availability(instance_ip, 443)
         logger.info("MiCADO deployed!")
 
-        #self._get_self_signed_cert(instance_ip, micado_id)
+        self._get_self_signed_cert(instance_ip, micado_id)
         self._store_data(micado_id, self.api_version, micado_user, micado_password)
         logger.info(f"MiCADO ID is: {micado_id}")
 
     def _check_availability(self, instance_ip):
         """Perform availability checks"""
         self._check_port_availability(instance_ip, 22)
         self._remove_know_host()
@@ -115,15 +115,15 @@
             occopus (boolean): Occopus enabled
         """
 
         security_dict = self._generate_credential_data(micado_user, micado_password)
 
         extra_variables = {
             "cloud_cred_path": str(micado_cli_dir / "credentials-cloud-api.yml"),
-            "docker_cred_path": str(micado_cli_dir / "credentials-registries.yml"),
+            "registry_cred_path": str(micado_cli_dir / "credentials-registries.yml"),
             "enable_terraform": terraform,
             "enable_occopus": occopus,
             "security": security_dict,
         }
 
         return extra_variables
 
@@ -250,22 +250,22 @@
 
         Args:
             server_id (string): UUID of the server
             api_version (string): Toscasubmitter API version
             micado_user (string): MiCADO username
             micado_password (string): MiCADO password
         """
-        #cert_path = f"{self.home}{server_id}-ssl.pem"
+        cert_path = f"{self.home}{server_id}-ssl.pem"
         DataHandling.update_data(
             self.home + "data.yml",
             server_id,
             api_version=api_version,
             micado_user=micado_user,
             micado_password=micado_password,
-            #cert_path=cert_path,
+            cert_path=cert_path,
         )
 
     def get_api_version(self):
         """
         Return the MiCADO Submitter API version. Only v2.0 supported.
 
         Returns:
```

### Comparing `micado-client-0.12.0a1/micado/installer/ansible/playbook.py` & `micado-client-0.12.0a2/micado/installer/ansible/playbook.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/launcher/cloudbroker/cloudbroker.py` & `micado-client-0.12.0a2/micado/launcher/cloudbroker/cloudbroker.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/launcher/openstack/auth.py` & `micado-client-0.12.0a2/micado/launcher/openstack/auth.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/launcher/openstack/openstack.py` & `micado-client-0.12.0a2/micado/launcher/openstack/openstack.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/models/application.py` & `micado-client-0.12.0a2/micado/models/application.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/models/base.py` & `micado-client-0.12.0a2/micado/models/base.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/models/micado.py` & `micado-client-0.12.0a2/micado/models/micado.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         Username: {server["micado_user"]}
         Password: {server["micado_password"]}
         """
         
         return SubmitterClient(
             endpoint=server["endpoint"],
             version=server["api_version"],
-            verify=False,
+            verify=server["cert_path"],
             auth=(server["micado_user"], server["micado_password"]),
         )
 
     def attach(self, micado_id):
         """Configure the micado object to handle the instance
         created by the def:create()
```

### Comparing `micado-client-0.12.0a1/micado/types/applications.py` & `micado-client-0.12.0a2/micado/types/applications.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado/utils/utils.py` & `micado-client-0.12.0a2/micado/utils/utils.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/micado_client.egg-info/PKG-INFO` & `micado-client-0.12.0a2/micado_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-client
-Version: 0.12.0a1
+Version: 0.12.0a2
 Summary: A Python Client Library for MiCADO
 Home-page: https://github.com/micado-scale/micado-client
 Author: Márk Emődi & Jay DesLauriers
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-client/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `micado-client-0.12.0a1/micado_client.egg-info/SOURCES.txt` & `micado-client-0.12.0a2/micado_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a1/setup.py` & `micado-client-0.12.0a2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "ansible-runner",
     "click",
     "dicttoxml",
 ]
 
 setup(
     name="micado-client",
-    version="0.12.0a1",
+    version="0.12.0a2",
     description="A Python Client Library for MiCADO",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Márk Emődi & Jay DesLauriers",
     python_requires=">=3.8",
     url="https://github.com/micado-scale/micado-client",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `micado-client-0.12.0a1/tests/test_auth.py` & `micado-client-0.12.0a2/tests/test_auth.py`

 * *Files identical despite different names*

