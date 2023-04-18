# Comparing `tmp/ensembl-prodinf-core-2.0.5.tar.gz` & `tmp/ensembl-prodinf-core-2.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembl-prodinf-core-2.0.5.tar", last modified: Tue Apr 18 10:16:43 2023, max compression
+gzip compressed data, was "ensembl-prodinf-core-2.0.5a2.tar", last modified: Mon Apr 17 16:54:12 2023, max compression
```

## Comparing `ensembl-prodinf-core-2.0.5.tar` & `ensembl-prodinf-core-2.0.5a2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.101485 ensembl-prodinf-core-2.0.5/
--rw-rw-rw-   0 root         (0) root         (0)    11366 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1203 2023-04-18 10:16:43.101485 ensembl-prodinf-core-2.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 10:16:43.101485 ensembl-prodinf-core-2.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2495 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.096485 ensembl-prodinf-core-2.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.095485 ensembl-prodinf-core-2.0.5/src/ensembl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.095485 ensembl-prodinf-core-2.0.5/src/ensembl/production/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.099485 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/
--rw-rw-rw-   0 root         (0) root         (0)     4785 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/amqp_publishing.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/app_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.099485 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6749 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/datachecks.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/dbcopy.py
--rw-rw-rw-   0 root         (0) root         (0)     3271 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/event.py
--rw-rw-rw-   0 root         (0) root         (0)     4613 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/handover.py
--rw-rw-rw-   0 root         (0) root         (0)     4150 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3482 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/db_introspects.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/db_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/es.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.100485 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2849 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/compara.py
--rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/core.py
--rw-rw-rw-   0 root         (0) root         (0)    21611 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/hive.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/perl_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/reporting.py
--rw-rw-rw-   0 root         (0) root         (0)    14102 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/resource_lock.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     5879 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3780 2023-04-18 10:16:17.000000 ensembl-prodinf-core-2.0.5/src/ensembl/production/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:16:43.101485 ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1203 2023-04-18 10:16:43.000000 ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1380 2023-04-18 10:16:43.000000 ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 10:16:43.000000 ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-18 10:16:43.000000 ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-18 10:16:43.000000 ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-18 10:16:43.000000 ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/
+-rw-rw-rw-   0 root         (0) root         (0)    11366 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.828649 ensembl-prodinf-core-2.0.5a2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.827649 ensembl-prodinf-core-2.0.5a2/src/ensembl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.828649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.831649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/
+-rw-rw-rw-   0 root         (0) root         (0)     4785 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/amqp_publishing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/app_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.832649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6749 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/datachecks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/dbcopy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     4613 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/handover.py
+-rw-rw-rw-   0 root         (0) root         (0)     4150 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3482 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_introspects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/es.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.832649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2849 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/compara.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    21611 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/hive.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/perl_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)    14102 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/resource_lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5879 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3780 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.833649 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/top_level.txt
```

### Comparing `ensembl-prodinf-core-2.0.5/LICENSE` & `ensembl-prodinf-core-2.0.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/PKG-INFO` & `ensembl-prodinf-core-2.0.5a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembl-prodinf-core
-Version: 2.0.5
+Version: 2.0.5a2
 Summary: Ensembl Production infrastructure core package
 Home-page: https://github.com/Ensembl/ensembl-prodinf-core
 Author: Marc Chakiachvili,James Allen,Luca Da Rin Fioretto,Vinay Kaikala
 Author-email: mchakiachvili@ebi.ac.uk,jallen@ebi.ac.uk,ldrf@ebi.ac.uk,vkaikala@ebi.ac.uk
 Maintainer: Ensembl Production Team
 Maintainer-email: ensembl-production@ebi.ac.uk
 License: Apache 2.0
```

### Comparing `ensembl-prodinf-core-2.0.5/setup.py` & `ensembl-prodinf-core-2.0.5a2/setup.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/amqp_publishing.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/amqp_publishing.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/app_logging.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/app_logging.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/datachecks.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/datachecks.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/dbcopy.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/dbcopy.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/event.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/event.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/handover.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/handover.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/clients/metadata.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/metadata.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/config.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/config.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/db_introspects.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_introspects.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/db_utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/es.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/es.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/exceptions.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/compara.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/compara.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/core.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/core.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/models/hive.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/hive.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/perl_utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/perl_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/reporting.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/reporting.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/resource_lock.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/resource_lock.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/rest.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/rest.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/server_utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/server_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl/production/core/utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/PKG-INFO` & `ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembl-prodinf-core
-Version: 2.0.5
+Version: 2.0.5a2
 Summary: Ensembl Production infrastructure core package
 Home-page: https://github.com/Ensembl/ensembl-prodinf-core
 Author: Marc Chakiachvili,James Allen,Luca Da Rin Fioretto,Vinay Kaikala
 Author-email: mchakiachvili@ebi.ac.uk,jallen@ebi.ac.uk,ldrf@ebi.ac.uk,vkaikala@ebi.ac.uk
 Maintainer: Ensembl Production Team
 Maintainer-email: ensembl-production@ebi.ac.uk
 License: Apache 2.0
```

### Comparing `ensembl-prodinf-core-2.0.5/src/ensembl_prodinf_core.egg-info/SOURCES.txt` & `ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

