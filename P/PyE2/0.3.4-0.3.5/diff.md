# Comparing `tmp/pye2-0.3.4.tar.gz` & `tmp/pye2-0.3.5.tar.gz`

## Comparing `pye2-0.3.4.tar` & `pye2-0.3.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.3.4/TODOs.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.3.4/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pye2-0.3.4/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.3.4/winrun.bat
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/version.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/__init__.py
--rw-r--r--   0        0        0    21174 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/logger.py
--rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/pipeline.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/base.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/comms.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/misc.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/default/__init__.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/consts.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/mixins/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/mixins/plugins_manager_mixin.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/utils/code.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/.example_env
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/attach_example.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/ex1.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/hello.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/remote_exec.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/decentralized/dedist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/decentralized/dedist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/decentralized/dedist_example_worker.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.3.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.3.4/LICENSE
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 pye2-0.3.4/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pye2-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 pye2-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.3.5/TODOs.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.3.5/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pye2-0.3.5/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.3.5/winrun.bat
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/version.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    21169 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/logger.py
+-rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/base.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/comms.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/misc.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/consts.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/mixins/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/mixins/plugins_manager_mixin.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/.example_env
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/attach_example.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/ex1.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/hello.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/remote_exec.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/decentralized/dedist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/decentralized/dedist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/decentralized/dedist_example_worker.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.3.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.3.5/LICENSE
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 pye2-0.3.5/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pye2-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 pye2-0.3.5/PKG-INFO
```

### Comparing `pye2-0.3.4/.github/workflows/python-publish.yml` & `pye2-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/base/__init__.py` & `pye2-0.3.5/PyE2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/base/generic_session.py` & `pye2-0.3.5/PyE2/base/generic_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
       if e2id in avail_workers:
         found = True
         break
       sleep(0.1)
 
     if not found:
       self.P("WARNING: could not find worker '{}' in {:.1f}s. The job may not have a valid active worker.".format(
-          self.e2id, tm() - _start
+          e2id, tm() - _start
       ), color='r')
     pipeline = Pipeline(
         self,
         self.log,
         e2id=e2id,
         name=name,
         data_source=data_source,
```

### Comparing `pye2-0.3.4/PyE2/base/logger.py` & `pye2-0.3.5/PyE2/base/logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/base/pipeline.py` & `pye2-0.3.5/PyE2/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/base/payload/payload.py` & `pye2-0.3.5/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/comm/__init__.py` & `pye2-0.3.5/PyE2/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/comm/amqp_wrapper.py` & `pye2-0.3.5/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/comm/mqtt_wrapper.py` & `pye2-0.3.5/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/const/__init__.py` & `pye2-0.3.5/PyE2/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/const/base.py` & `pye2-0.3.5/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/const/comms.py` & `pye2-0.3.5/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/const/heartbeat.py` & `pye2-0.3.5/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/const/misc.py` & `pye2-0.3.5/PyE2/const/misc.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/const/payload.py` & `pye2-0.3.5/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/default/mqtt_session.py` & `pye2-0.3.5/PyE2/default/mqtt_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/__init__.py` & `pye2-0.3.5/PyE2/io_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/consts.py` & `pye2-0.3.5/PyE2/io_formatter/consts.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.3.5/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/base/__init__.py` & `pye2-0.3.5/PyE2/io_formatter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.3.5/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/default/__init__.py` & `pye2-0.3.5/PyE2/io_formatter/default/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.3.5/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/default/cavi2.py` & `pye2-0.3.5/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/io_formatter/mixins/plugins_manager_mixin.py` & `pye2-0.3.5/PyE2/io_formatter/mixins/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/utils/code.py` & `pye2-0.3.5/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/PyE2/utils/code_exec.py` & `pye2-0.3.5/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/xperimental/attach_example.py` & `pye2-0.3.5/xperimental/attach_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/xperimental/ex1.py` & `pye2-0.3.5/xperimental/ex1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/xperimental/remote_exec.py` & `pye2-0.3.5/xperimental/remote_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/xperimental/decentralized/dedist_example.py` & `pye2-0.3.5/xperimental/decentralized/dedist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/xperimental/decentralized/dedist_example_initiator.py` & `pye2-0.3.5/xperimental/decentralized/dedist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/.gitignore` & `pye2-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/LICENSE` & `pye2-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/README.md` & `pye2-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pye2-0.3.4/pyproject.toml` & `pye2-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pika", "paho-mqtt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@global-technical.com" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@global-technical.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
 ]
 description = "PyE2 is an SDK used to communicate with the AiXpand network"
 readme = "README.md"
```

### Comparing `pye2-0.3.4/PKG-INFO` & `pye2-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyE2
-Version: 0.3.4
+Version: 0.3.5
 Summary: PyE2 is an SDK used to communicate with the AiXpand network
 Project-URL: Homepage, https://github.com/AiXpand/PyE2
 Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
 Author-email: Stefan Saraev <stefan.saraev@global-technical.com>, Cristan Bleotiu <cristan.bleotiu@global-technical.com>, Andrei Ionut Damian <andrei.damian@lummetry.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

