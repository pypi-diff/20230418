# Comparing `tmp/tripmaster-1.0.6-py3-none-any.whl.zip` & `tmp/tripmaster-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 139002 bytes, number of entries: 105
+Zip file size: 139184 bytes, number of entries: 105
 -rw-r--r--  2.0 unx      249 b- defN 22-Dec-23 09:48 tripmaster/__init__.py
 -rw-r--r--  2.0 unx        3 b- defN 22-Dec-23 09:48 tripmaster/core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/app/__init__.py
--rw-r--r--  2.0 unx     6114 b- defN 23-Apr-10 13:28 tripmaster/core/app/config.py
--rw-r--r--  2.0 unx     2334 b- defN 22-Dec-23 09:48 tripmaster/core/app/io.py
+-rw-r--r--  2.0 unx     6101 b- defN 23-Apr-18 01:33 tripmaster/core/app/config.py
+-rw-r--r--  2.0 unx     2334 b- defN 23-Apr-18 01:26 tripmaster/core/app/io.py
 -rw-r--r--  2.0 unx     2678 b- defN 22-Dec-23 09:48 tripmaster/core/app/pipeline.py
 -rw-r--r--  2.0 unx     3347 b- defN 22-Dec-23 09:48 tripmaster/core/app/reinforce.py
--rw-r--r--  2.0 unx     5965 b- defN 23-Apr-11 02:18 tripmaster/core/app/standalone.py
+-rw-r--r--  2.0 unx     5965 b- defN 23-Apr-18 01:25 tripmaster/core/app/standalone.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/app/supervise.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/components/__init__.py
 -rw-r--r--  2.0 unx     4572 b- defN 22-Dec-23 09:48 tripmaster/core/components/backend.py
 -rw-r--r--  2.0 unx    11741 b- defN 22-Dec-23 09:48 tripmaster/core/components/contract.py
 -rw-r--r--  2.0 unx    27131 b- defN 22-Dec-23 09:48 tripmaster/core/components/evaluator.py
 -rw-r--r--  2.0 unx    11251 b- defN 22-Dec-23 09:48 tripmaster/core/components/loss.py
 -rw-r--r--  2.0 unx     2901 b- defN 22-Dec-23 09:48 tripmaster/core/components/problem.py
@@ -37,32 +37,32 @@
 -rw-r--r--  2.0 unx     1272 b- defN 22-Dec-23 09:48 tripmaster/core/components/operator/strategies/distributed.py
 -rw-r--r--  2.0 unx     1635 b- defN 22-Dec-23 09:48 tripmaster/core/components/operator/strategies/event_trigger.py
 -rw-r--r--  2.0 unx     4521 b- defN 22-Dec-23 09:48 tripmaster/core/components/operator/strategies/exploration_strategy.py
 -rw-r--r--  2.0 unx     1082 b- defN 22-Dec-23 09:48 tripmaster/core/components/operator/strategies/metric_logging.py
 -rw-r--r--  2.0 unx    16929 b- defN 23-Apr-07 02:55 tripmaster/core/components/operator/strategies/model_selection.py
 -rw-r--r--  2.0 unx     7487 b- defN 22-Dec-23 09:48 tripmaster/core/components/operator/strategies/optimization.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/__init__.py
--rw-r--r--  2.0 unx    16055 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/component.py
+-rw-r--r--  2.0 unx    16055 b- defN 23-Apr-18 01:24 tripmaster/core/concepts/component.py
 -rw-r--r--  2.0 unx     5996 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/contract.py
--rw-r--r--  2.0 unx    10625 b- defN 23-Apr-14 12:53 tripmaster/core/concepts/data.py
+-rw-r--r--  2.0 unx    11491 b- defN 23-Apr-17 13:42 tripmaster/core/concepts/data.py
 -rw-r--r--  2.0 unx     3670 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/evaluator.py
 -rw-r--r--  2.0 unx      470 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/hyper_params.py
 -rw-r--r--  2.0 unx      479 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/loss.py
 -rw-r--r--  2.0 unx      375 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/machine.py
 -rw-r--r--  2.0 unx     3782 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/modeler.py
 -rw-r--r--  2.0 unx      894 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/operator.py
 -rw-r--r--  2.0 unx      990 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/scenario.py
 -rw-r--r--  2.0 unx     3197 b- defN 22-Dec-23 09:48 tripmaster/core/concepts/schema.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/launcher/__init__.py
 -rw-r--r--  2.0 unx     6326 b- defN 22-Dec-23 09:48 tripmaster/core/launcher/job.py
 -rw-r--r--  2.0 unx     3085 b- defN 23-Feb-11 04:05 tripmaster/core/launcher/launcher.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/system/__init__.py
 -rw-r--r--  2.0 unx     3133 b- defN 22-Dec-23 09:48 tripmaster/core/system/reinforce.py
 -rw-r--r--  2.0 unx     2658 b- defN 23-Apr-10 13:37 tripmaster/core/system/supervise.py
--rw-r--r--  2.0 unx    34453 b- defN 23-Apr-12 03:23 tripmaster/core/system/system.py
+-rw-r--r--  2.0 unx    34453 b- defN 23-Apr-18 01:26 tripmaster/core/system/system.py
 -rw-r--r--  2.0 unx     6326 b- defN 22-Dec-23 09:48 tripmaster/core/system/validation.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/system/test/__init__.py
 -rw-r--r--  2.0 unx      268 b- defN 22-Dec-23 09:48 tripmaster/core/system/test/test_multi.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 09:48 tripmaster/core/test/__init__.py
 -rw-r--r--  2.0 unx     2273 b- defN 22-Dec-23 09:48 tripmaster/core/test/test_generic.py
 -rw-r--r--  2.0 unx      142 b- defN 22-Dec-23 09:48 tripmaster/plugins/__init__.py
 -rw-r--r--  2.0 unx      985 b- defN 23-Feb-10 09:13 tripmaster/plugins/load.py
@@ -95,13 +95,13 @@
 -rw-r--r--  2.0 unx       49 b- defN 22-Dec-23 09:48 tripmaster/utils/logging/__init__.py
 -rw-r--r--  2.0 unx     1982 b- defN 22-Dec-23 09:48 tripmaster/utils/logging/capture.py
 -rw-r--r--  2.0 unx     1369 b- defN 22-Dec-23 09:48 tripmaster/utils/logging/config.yaml
 -rw-r--r--  2.0 unx    11217 b- defN 23-Apr-12 12:44 tripmaster/utils/logging/core.py
 -rw-r--r--  2.0 unx     7389 b- defN 22-Dec-23 09:48 tripmaster/utils/logging/inspector.py
 -rw-r--r--  2.0 unx     8502 b- defN 22-Dec-23 09:48 tripmaster/utils/logging/logger.py
 -rw-r--r--  2.0 unx     3483 b- defN 22-Dec-23 09:48 tripmaster/utils/logging/logging.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:12 tripmaster-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      879 b- defN 23-Apr-14 15:12 tripmaster-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 15:12 tripmaster-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-14 15:12 tripmaster-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     9953 b- defN 23-Apr-14 15:12 tripmaster-1.0.6.dist-info/RECORD
-105 files, 514377 bytes uncompressed, 122844 bytes compressed:  76.1%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-18 02:05 tripmaster-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      879 b- defN 23-Apr-18 02:05 tripmaster-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 02:05 tripmaster-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 02:05 tripmaster-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9953 b- defN 23-Apr-18 02:05 tripmaster-1.0.7.dist-info/RECORD
+105 files, 515230 bytes uncompressed, 123026 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -294,23 +294,23 @@
 
 Filename: tripmaster/utils/logging/logger.py
 Comment: 
 
 Filename: tripmaster/utils/logging/logging.py
 Comment: 
 
-Filename: tripmaster-1.0.6.dist-info/LICENSE
+Filename: tripmaster-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: tripmaster-1.0.6.dist-info/METADATA
+Filename: tripmaster-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: tripmaster-1.0.6.dist-info/WHEEL
+Filename: tripmaster-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: tripmaster-1.0.6.dist-info/top_level.txt
+Filename: tripmaster-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: tripmaster-1.0.6.dist-info/RECORD
+Filename: tripmaster-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tripmaster/core/app/config.py

```diff
@@ -9,17 +9,16 @@
 import os
 
 @dataclass
 class Serializable:
     """
     ProblemModeler
     """
-    save: bool = False
-    load: bool = False
-    path: Optional[str] = None
+    save: Optional[str] = False
+    load: Optional[str] = False
     multi_path: Optional[Dict] = None
 
 
 @dataclass
 class Strategy:
     type: str = ""
     strategies: Dict[str, Any] = field(default_factory=lambda: dict())
```

## tripmaster/core/app/io.py

```diff
@@ -20,27 +20,27 @@
     """
     TMOfflineApplicationInput
     """
 
     def data_stream(self):
 
         if self.hyper_params.machine.serialize and self.hyper_params.machine.serialize.load:
-            machine_data = TMDataStream.deserialize(self.hyper_params.machine.serialize.path,
+            machine_data = TMDataStream.deserialize(self.hyper_params.machine.serialize.load,
                                                    self.hyper_params.machine)
             logger.info(f"serialized machine data loaded from {self.hyper_params.machine.serialize} ")
             return machine_data
 
         if self.hyper_params.problem.serialize and self.hyper_params.problem.serialize.load:
-            problem_data = TMDataStream.deserialize(self.hyper_params.problem.serialize.path,
+            problem_data = TMDataStream.deserialize(self.hyper_params.problem.serialize.load,
                                                    self.hyper_params.problem)
             logger.info(f"serialized problem data loaded from {self.hyper_params.problem.serialize} ")
             return problem_data
 
         if self.hyper_params.task.serialize and self.hyper_params.task.serialize.load:
-            task_data = TMDataStream.deserialize(self.hyper_params.task.serialize.path,
+            task_data = TMDataStream.deserialize(self.hyper_params.task.serialize.load,
                                                 self.hyper_params.task)
             logger.info(f"serialized task data loaded from {self.hyper_params.task.serialize}")
             return task_data
 
 
         if "task" in self.hyper_params:
             return self.DataStreamType(self.hyper_params.task)
@@ -58,9 +58,9 @@
 
     def __init__(self, hyper_params):
 
         super().__init__(hyper_params)
 
     def write(self, datastream):
         if self.hyper_params.serialize and self.hyper_params.serialize.save:
-            datastream.serialize(self.hyper_params.serialize.path)
+            datastream.serialize(self.hyper_params.serialize.save)
```

## tripmaster/core/app/standalone.py

```diff
@@ -22,52 +22,52 @@
         if not self.hyper_params.io.input or not self.hyper_params.io.input.task:
             return
 
         task_serialize_config = self.hyper_params.io.input.task.serialize
 
         if task_serialize_config and task_serialize_config.save:
             logger.info(f"Saving task data with serialize config {self.hyper_params.io.input.task.serialize}")
-            task_data.serialize(self.hyper_params.io.input.task.serialize.path)
+            task_data.serialize(self.hyper_params.io.input.task.serialize.save)
 
     def on_problem_data_built(self, problem_data):
         if not self.hyper_params.io.input or not self.hyper_params.io.input.problem:
             return
         problem_serialize_config = self.hyper_params.io.input.problem.serialize
         if problem_serialize_config and problem_serialize_config.save:
             logger.info(f"Saving problem data with serialize config {self.hyper_params.io.input.problem.serialize}")
-            problem_data.serialize(self.hyper_params.io.input.problem.serialize.path)
+            problem_data.serialize(self.hyper_params.io.input.problem.serialize.save)
 
     def on_machine_data_built(self, machine_data):
         if not self.hyper_params.io.input or not self.hyper_params.io.input.machine:
             return
         machine_serialize_config = self.hyper_params.io.input.machine.serialize
         if machine_serialize_config and machine_serialize_config.save:
             logger.info(f"Saving machine data with serialize config {self.hyper_params.io.input.machine.serialize}")
-            machine_data.serialize(self.hyper_params.io.input.machine.serialize.path)
+            machine_data.serialize(self.hyper_params.io.input.machine.serialize.save)
 
     def on_data_phase_finished(self, system):
 
         if to_save(system.hyper_params.task):
-            system.task.serialize(system.hyper_params.task.serialize.path)
+            system.task.serialize(system.hyper_params.task.serialize.save)
             logger.info("task serialized")
 
         if to_save(system.hyper_params.tp_modeler):
-            system.tp_modeler.serialize(system.hyper_params.tp_modeler.serialize.path)
+            system.tp_modeler.serialize(system.hyper_params.tp_modeler.serialize.save)
             logger.info("tp_modeler serialized")
 
         if to_save(system.hyper_params.problem):
-            system.problem.serialize(system.hyper_params.problem.serialize.path)
+            system.problem.serialize(system.hyper_params.problem.serialize.save)
             logger.info("problem serialized")
 
         if to_save(system.hyper_params.pm_modeler):
-            system.pm_modeler.serialize(system.hyper_params.pm_modeler.serialize.path)
+            system.pm_modeler.serialize(system.hyper_params.pm_modeler.serialize.save)
             logger.info("pm_modeler serialized")
 
         if to_save(system.hyper_params):
-            system.serialize(system.hyper_params.serialize.path)
+            system.serialize(system.hyper_params.serialize.save)
             logger.info("system serialized")
 
 
 
 class TMStandaloneApp(TMConfigurable):
 
     InputStreamType = None
```

## tripmaster/core/concepts/component.py

```diff
@@ -344,28 +344,28 @@
         from tripmaster.core.components.repo import TMRepo
 
         if not hyper_param:
             return cls(*args, hyper_params=None, **kwargs)
 
         if hyper_param.serialize and hyper_param.serialize.load:
 
-            serialized_path = os.path.expanduser(hyper_param.serialize.path)
+            serialized_path = os.path.expanduser(hyper_param.serialize.load)
             logger.info(f"trying to load serialized component {serialized_path}")
             if not os.path.exists(serialized_path):
 
                 logger.info(f"{serialized_path} does not exists, try to download from repo")
                 repo_uri = serialized_path
 
                 try:
                     serialized_path = TMRepo().get(repo_uri)
                 except Exception as e:
                     message = f"Failed to obtain component from repo using uri {repo_uri}"
                     logger.error(message)
                     raise Exception(message)
-                hyper_param.serialize.path = serialized_path
+                hyper_param.serialize.load = serialized_path
             component = cls.deserialize(serialized_path, hyper_param)
             logger.info(f"component loaded from {serialized_path}")
         else:
             component = cls(hyper_param, *args, **kwargs)
 
         return component
```

## tripmaster/core/concepts/data.py

```diff
@@ -1,11 +1,12 @@
 """
 base class for data
 """
 import abc
+import copy
 import enum
 from collections import defaultdict
 from typing import Dict, Type
 
 from tripmaster import logging
 from tripmaster.core.concepts.component import TMConfigurable, TMSerializable
 
@@ -145,14 +146,21 @@
         super().__init__(hyper_params)
 
         self.__channels = dict()
         self.__level = level
 
         if states is not None:
             self.load_states(states)
+            logger.info("add sampled training eval channel ")
+
+            if self.hyper_params.train_sample_ratio_for_eval or self.hyper_params.train_sample_ratio_for_eval > 0:
+                ratio = self.hyper_params.train_sample_ratio_for_eval
+                self.add_sampled_training_eval_channels(ratio)
+
+            logger.info("sampled training eval channel added")
 
     @property
     def level(self):
         return self.__level
 
     @level.setter
     def level(self, level):
@@ -165,26 +173,28 @@
     def channels(self):
         return self.__channels.keys()
 
     @property
     def learn_channels(self):
         return self.hyper_params.channels.learn if self.hyper_params.channels.learn else []
 
-    def add_sampled_training_eval_channels(self):
+    def add_sampled_training_eval_channels(self, ratio=None):
 
-        if not self.hyper_params.train_sample_ratio_for_eval or self.hyper_params.train_sample_ratio_for_eval <= 0:
-            return 
+        if ratio is None:
+            ratio = self.hyper_params.train_sample_ratio_for_eval
+            if not ratio or (isinstance(ratio, (int, float)) and ratio < 0):
+                return
 
         import random, copy 
         sampled_channels = []
         for channel in self.learn_channels:
             assert channel in self.__channels
 
             sampled = [copy.deepcopy(sample) for sample in self.__channels[channel]
-                            if random.random() < self.hyper_params.train_sample_ratio_for_eval]
+                            if random.random() < ratio]
             if len(sampled) <= 0:
                 continue
             sampled_channels.append(f"{channel}#sampled")
 
             self.__channels[f"{channel}#sampled"] = TMDataChannel(data=sampled, level=self.__level)
                 
         self.hyper_params.channels.eval = list(set(list(self.hyper_params.channels.eval) + sampled_channels))
@@ -220,25 +230,36 @@
         self.__channels[key] = value
 
     def test(self, test_config):
 
         for k, v in self.__channels.items():
             v.sample_num = test_config.sample_num
 
+        self.add_sampled_training_eval_channels(ratio=1)
+
     def states(self):
         for k, v in self.__channels.items():
             v.degenerate()
 
-        return {"channels": {k: v._data for k, v in self.__channels.items()},
+        return {"channels": {k: v._data for k, v in self.__channels.items() if not k.endswith("#sampled")},
                 "level": self.__level}
 
+    def secure_hparams(self):
+
+        hyper_params = copy.deepcopy(self.hyper_params)
+        for channel in hyper_params.channels:
+            hyper_params.channels[channel] = [k for k in hyper_params.channels[channel]
+                                                   if not k.endswith("#sampled")]
+        return hyper_params
+
+
     def load_states(self, states):
         self.__level = states["level"]
         self.__channels = {k: TMDataChannel(data=v, level=self.__level)
-                           for k, v in states["channels"].items()}
+                           for k, v in states["channels"].items() if not k.endswith("#sampled")}
 
 
 
 class TMSharedDataStream(TMDataStream):
     """
     TMSharedDataStream
     """
```

## tripmaster/core/system/system.py

```diff
@@ -647,15 +647,15 @@
 
         Returns:
 
         """
         for info in info_iter:
             if isinstance(info, SelectedModelInfo):
                 if to_save(self.hyper_params):
-                    self.serialize(self.hyper_params.serialize.path)
+                    self.serialize(self.hyper_params.serialize.save)
             elif isinstance(info, tuple):
                 metric, machine_info = info
                 if to_save(self.hyper_params):
                     self.serialize(self.hyper_params.serialize.multi_path[metric])
             else:
                 raise Exception(f"unknown info type: {type(info)}")
```

## Comparing `tripmaster-1.0.6.dist-info/LICENSE` & `tripmaster-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tripmaster-1.0.6.dist-info/METADATA` & `tripmaster-1.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tripmaster
-Version: 1.0.6
+Version: 1.0.7
 Summary: A High Level Framework for Deep Learning App and Pipelines for Paddle.
 Home-page: https://github.com/baidu-research/tripmaster
 Author: Mingming Sun
 Author-email: sunmingming01@baidu.com
 License: Apache
 Keywords: Deep Learning,Framework,Pipelines
 Description-Content-Type: text/markdown
```

## Comparing `tripmaster-1.0.6.dist-info/RECORD` & `tripmaster-1.0.7.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 tripmaster/__init__.py,sha256=iYCOpjCOFdPW4KItbmM06dw-GdBqOWOJtMhxek3aMD4,249
 tripmaster/core/__init__.py,sha256=ajz1GSNU9xYVrFEDSz6Xwg7amWQ_yvW75tQa1ZvRIWc,3
 tripmaster/core/app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tripmaster/core/app/config.py,sha256=RxOoe6ajTVMuTMC4Hn_vejZdLmJlEMP1BtmmNz4et-Q,6114
-tripmaster/core/app/io.py,sha256=FPLAH5wUydwZWu9VetI6iAXc5461PBYFRLcPUJU9tyU,2334
+tripmaster/core/app/config.py,sha256=H8Ypp5Ef3eduYI2zCwf8QQA-N1Xt9P3qh_-pBRB6aBc,6101
+tripmaster/core/app/io.py,sha256=-41KIwF2--roQj_CNWspXrdkT7lmjs48dVVb5Urf7Ws,2334
 tripmaster/core/app/pipeline.py,sha256=8B6r5HJYuVUS5kmurpK6VjWO22Hw0i2RYD8AeoTXkS8,2678
 tripmaster/core/app/reinforce.py,sha256=W0Cn31iqmmwyQF4WPCB0zdkBTZaHvdXcB9nCoeHCK_U,3347
-tripmaster/core/app/standalone.py,sha256=WwIVgMCXbejNR2kXsF313aXkRx8cCLwFxAPgWIDYvUQ,5965
+tripmaster/core/app/standalone.py,sha256=VbgOKrKWw-TJ_gjUZhAzyeqzaaTbTEEsCFw096YBTtM,5965
 tripmaster/core/app/supervise.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tripmaster/core/components/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tripmaster/core/components/backend.py,sha256=LmLo8cb1o0hu1Ri9gAWhdlKtoQUjob2facpG07IDWd0,4572
 tripmaster/core/components/contract.py,sha256=6vRxYGdBLyKNJw89OzdJO9mJ-1CHp2ERvFwoBzx89j4,11741
 tripmaster/core/components/evaluator.py,sha256=msPO6M2-1mXgN6Mvhh33AGM2ElxqeQ7a2r4oaFTd9aM,27131
 tripmaster/core/components/loss.py,sha256=Gx_SrdW43xdMT5ntjy2RFHYYny6NU1V7yGclMjB4S3E,11251
 tripmaster/core/components/problem.py,sha256=dBU4Jr3kyBCMG8h06IWSyKaWhrfw82OApZb8w0ZkK6c,2901
@@ -36,32 +36,32 @@
 tripmaster/core/components/operator/strategies/distributed.py,sha256=XuJ9PsRLNa5sm3erklsuAcX_Disulf0XhnhYX-rXEyk,1272
 tripmaster/core/components/operator/strategies/event_trigger.py,sha256=XJ_RbSqF3AzkeA-rfB5Idh3xffPPBDy5HH01Uzx44j8,1635
 tripmaster/core/components/operator/strategies/exploration_strategy.py,sha256=Ay-_m7KDW8QXR2pKiV66qR_jGyNhB7lPT7DgXEnXgwU,4521
 tripmaster/core/components/operator/strategies/metric_logging.py,sha256=P6GDPJKlf8nIg5PrMNTDawWSqST6aFwceYvFSKjfFMU,1082
 tripmaster/core/components/operator/strategies/model_selection.py,sha256=CvXKhxBNWX9xmkTKFxzCdeBnwFR_qWI5IMCN64bf_nI,16929
 tripmaster/core/components/operator/strategies/optimization.py,sha256=HetJg2XPZhifxmHLXrRKTH7f80JXcYZq5oWcEwX_j3c,7487
 tripmaster/core/concepts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tripmaster/core/concepts/component.py,sha256=i5eTKRCzCu-zyK-zPzM4QsQtocIdYY83dfN-nMaxpTI,16055
+tripmaster/core/concepts/component.py,sha256=KDn3_qW1vPI3w9m1XYywdFv4kaXwbUvG2m080k6RYhI,16055
 tripmaster/core/concepts/contract.py,sha256=l9csDtejpUSdd_6DvQ7voWe8KiVptYtfzSxat2YvJGE,5996
-tripmaster/core/concepts/data.py,sha256=5Hfx1jbrMssJLpJyPR6MV_AM2iM-SI4tNl6ddqgxCFQ,10625
+tripmaster/core/concepts/data.py,sha256=Gh7BVhN-NRIN8ci_VRfu0fFGFSztcBIjcMwZrdz7Cfg,11491
 tripmaster/core/concepts/evaluator.py,sha256=uPfykwCHquBsSxEh6ee5tjtEQU7YXCElitcpJfRfFVI,3670
 tripmaster/core/concepts/hyper_params.py,sha256=SqEwvNiWAt2FMD1e4_XmkZBifzzAAvXcaztY8_bU0Hc,470
 tripmaster/core/concepts/loss.py,sha256=O_F68_Y6SluazjRRp5dB0tIn6EA3sxPQLG0utfW967Y,479
 tripmaster/core/concepts/machine.py,sha256=SEH-rmVRO7xJOSHn3PWr5h5Br_qGG-bfKiIaWqGaw7s,375
 tripmaster/core/concepts/modeler.py,sha256=BmEQ6yL9fULLtDP3bFSE0lMDtTE_9lQGLddWAcaQjYk,3782
 tripmaster/core/concepts/operator.py,sha256=Gr40avVoA4gThJJ_v97OActOfCbOtfcuDWjNSBgYVzQ,894
 tripmaster/core/concepts/scenario.py,sha256=0Qhk6aeh_9ZmbZcd7bd1nXWUDkZfig-OnVSxMQf3A7k,990
 tripmaster/core/concepts/schema.py,sha256=Gvsf3lAB0ET50omCN13mNhQ9rEB1vJha2QXXthpsTOs,3197
 tripmaster/core/launcher/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tripmaster/core/launcher/job.py,sha256=I4SYoFBPHXLRRiQ4vgGF8o6GGeyXhi0WHxZyve0Wbvw,6326
 tripmaster/core/launcher/launcher.py,sha256=H_zDvyRcyFtzjQYKQ6M8h8Qf-Y_Yw40EpIsUPBDqc5M,3085
 tripmaster/core/system/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tripmaster/core/system/reinforce.py,sha256=SFRQuTLv1ZtL9JVPulhkX_VcozUVPqcRkRSzxZOUxqU,3133
 tripmaster/core/system/supervise.py,sha256=CidS6RoQnsE5NfdwIa__Xqu3-bxwSc7Lvt2F5wu3f6M,2658
-tripmaster/core/system/system.py,sha256=Oz6o37vMrHVvxn_bpRw8qH1yZ8aoUzGtKuyhbyor178,34453
+tripmaster/core/system/system.py,sha256=WtF5ajtMEgR6dN1joGnbguJPN2qFXLk2So13xddBx-M,34453
 tripmaster/core/system/validation.py,sha256=zzAtTHno-Wxf583Fleb5Wk-lhBETYKjgJqbYU_OE2dI,6326
 tripmaster/core/system/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tripmaster/core/system/test/test_multi.py,sha256=t2E9935sUhQFZ3mlDVphvFgIr9rLBZyEZChaSLx_wlE,268
 tripmaster/core/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tripmaster/core/test/test_generic.py,sha256=_QFbahiMgY5KV_lnuGDinSI3foR_LFFIbpkQBaPyaDo,2273
 tripmaster/plugins/__init__.py,sha256=jqFHp4HGB8CZKoF19vIagodw0rfHIdmxUzqyj_1N46g,142
 tripmaster/plugins/load.py,sha256=ETI9RFghmBWfqBLd2_mrwftzEFw5wm-HqOCD3AF5k3M,985
@@ -94,12 +94,12 @@
 tripmaster/utils/logging/__init__.py,sha256=wcvOBO8BH8xNs0KiMp1foAsu5wEh5PJKaS2z4fLJgjY,49
 tripmaster/utils/logging/capture.py,sha256=PpB759dRHLOUDNCJQxw1_aBPYrOTl78frnDDJVltR-k,1982
 tripmaster/utils/logging/config.yaml,sha256=IApV4PVZYOmxP_tpqM5DAL-IAngkc7RslwsvDbJ2i0w,1369
 tripmaster/utils/logging/core.py,sha256=wPOX9boLYlhh3NOxtgP9MpOgtuRK4mwOBigQBDTEx9c,11217
 tripmaster/utils/logging/inspector.py,sha256=cl7_P1mMJdpnugebK5tyNjv8DBaGpb3xsK3ynB3Zuog,7389
 tripmaster/utils/logging/logger.py,sha256=paz1R6JYp7cz6IoOMcbm7JRYXIj0-aRIvoOQaVpINiw,8502
 tripmaster/utils/logging/logging.py,sha256=NNFjOQpOlQzczetyj8MIxqayaWZyEW731vDimKBUNc4,3483
-tripmaster-1.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-tripmaster-1.0.6.dist-info/METADATA,sha256=htXz7v4YufsYbpm6qu0jKuKfXZvmw4tkgI5UxfP_qFo,879
-tripmaster-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-tripmaster-1.0.6.dist-info/top_level.txt,sha256=maHIEfa7B54A9-_P0yed19EnIuL2hK_QI3vWPHPlDoI,11
-tripmaster-1.0.6.dist-info/RECORD,,
+tripmaster-1.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+tripmaster-1.0.7.dist-info/METADATA,sha256=6Oj24U9Px1zb4C8NNUqv9mClnLz7V8mvfk49nBfZJzc,879
+tripmaster-1.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+tripmaster-1.0.7.dist-info/top_level.txt,sha256=maHIEfa7B54A9-_P0yed19EnIuL2hK_QI3vWPHPlDoI,11
+tripmaster-1.0.7.dist-info/RECORD,,
```

