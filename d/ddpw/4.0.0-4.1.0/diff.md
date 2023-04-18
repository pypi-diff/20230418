# Comparing `tmp/ddpw-4.0.0.tar.gz` & `tmp/ddpw-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddpw-4.0.0.tar", last modified: Sat Apr 15 18:52:06 2023, max compression
+gzip compressed data, was "ddpw-4.1.0.tar", last modified: Tue Apr 18 13:48:36 2023, max compression
```

## Comparing `ddpw-4.0.0.tar` & `ddpw-4.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-15 18:51:52.000000 ddpw-4.0.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 18:52:06.955824 ddpw-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-15 18:51:52.000000 ddpw-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/ddpw/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/artefacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/ddpw/gpu_setup/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__model.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/ddpw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:52:06.955824 ddpw-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-15 18:51:52.000000 ddpw-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:48:36.624667 ddpw-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-18 13:48:20.000000 ddpw-4.1.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-18 13:48:36.624667 ddpw-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-18 13:48:20.000000 ddpw-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:48:36.624667 ddpw-4.1.0/ddpw/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/artefacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:48:36.624667 ddpw-4.1.0/ddpw/gpu_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/gpu_setup/__dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/gpu_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/gpu_setup/__model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/gpu_setup/__seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-18 13:48:20.000000 ddpw-4.1.0/ddpw/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:48:36.624667 ddpw-4.1.0/ddpw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-18 13:48:36.000000 ddpw-4.1.0/ddpw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-18 13:48:36.000000 ddpw-4.1.0/ddpw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:48:36.000000 ddpw-4.1.0/ddpw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 13:48:36.000000 ddpw-4.1.0/ddpw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 13:48:36.000000 ddpw-4.1.0/ddpw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:48:36.624667 ddpw-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-18 13:48:20.000000 ddpw-4.1.0/setup.py
```

### Comparing `ddpw-4.0.0/LICENCE.md` & `ddpw-4.1.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `ddpw-4.0.0/PKG-INFO` & `ddpw-4.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddpw
-Version: 4.0.0
+Version: 4.1.0
 Summary: A utility package to scaffold PyTorch's DDP
 Home-page: https://ddpw.projects.sujal.tv
 Author: Sujal T.V.
 License: UNKNOWN
 Description: # DDPW
         
         [![AWS S3](https://img.shields.io/badge/documentation-sphinx-blue?link=https://ddpw.projects.sujal.tv)](https://ddpw.projects.sujal.tv)
@@ -36,30 +36,30 @@
         ### Usage
         
         ```python
         from ddpw.platform import Platform, PlatformConfig
         from ddpw.artefacts import ArtefactsConfig
         from ddpw.job import JobConfig, JobMode
         from ddpw.wrapper import Wrapper
+        from torchvision.datasets.mnist import MNIST
         
-        from src import MyDataset, MyModel, MyOptimiser, MyTrainer
+        from src import MyModel, MyTrainer
         
-        # datasets
-        train_set = MyDataset(train=True)
-        test_set = MyDataset(train=False)
+        # dataset
+        train_set = MNIST(root='./data/MNSIT', train=True)
         
-        # configure the platform
+        # platform
         p_config = PlatformConfig(platform=Platform.GPU, n_gpus=4, cpus_per_task=2)
         
-        # configure the artefacts (model, dataset, optimiser, etc.)
-        a_config = ArtefactsConfig(train_set=train_set, test_set=test_set,
-            batch_size=64, model=MyModel(), optimiser_loader=MyOptimiser(lr=0.1))
+        # model and dataset
+        a_config = ArtefactsConfig(train_set=train_set, model=MyModel())
         
         # call the job
-        Wrapper(p_config, a_config).start(MyTrainer())
+        wrapper = Wrapper(p_config, a_config)
+        wrapper.start(MyTrainer())
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ddpw-4.0.0/README.md` & `ddpw-4.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 ### Usage
 
 ```python
 from ddpw.platform import Platform, PlatformConfig
 from ddpw.artefacts import ArtefactsConfig
 from ddpw.job import JobConfig, JobMode
 from ddpw.wrapper import Wrapper
+from torchvision.datasets.mnist import MNIST
 
-from src import MyDataset, MyModel, MyOptimiser, MyTrainer
+from src import MyModel, MyTrainer
 
-# datasets
-train_set = MyDataset(train=True)
-test_set = MyDataset(train=False)
+# dataset
+train_set = MNIST(root='./data/MNSIT', train=True)
 
-# configure the platform
+# platform
 p_config = PlatformConfig(platform=Platform.GPU, n_gpus=4, cpus_per_task=2)
 
-# configure the artefacts (model, dataset, optimiser, etc.)
-a_config = ArtefactsConfig(train_set=train_set, test_set=test_set,
-    batch_size=64, model=MyModel(), optimiser_loader=MyOptimiser(lr=0.1))
+# model and dataset
+a_config = ArtefactsConfig(train_set=train_set, model=MyModel())
 
 # call the job
-Wrapper(p_config, a_config).start(MyTrainer())
+wrapper = Wrapper(p_config, a_config)
+wrapper.start(MyTrainer())
 ```
```

### Comparing `ddpw-4.0.0/ddpw/artefacts.py` & `ddpw-4.1.0/ddpw/artefacts.py`

 * *Files identical despite different names*

### Comparing `ddpw-4.0.0/ddpw/gpu_setup/__dataset.py` & `ddpw-4.1.0/ddpw/gpu_setup/__dataset.py`

 * *Files identical despite different names*

### Comparing `ddpw-4.0.0/ddpw/gpu_setup/__init__.py` & `ddpw-4.1.0/ddpw/gpu_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `ddpw-4.0.0/ddpw/gpu_setup/__model.py` & `ddpw-4.1.0/ddpw/gpu_setup/__model.py`

 * *Files identical despite different names*

### Comparing `ddpw-4.0.0/ddpw/job.py` & `ddpw-4.1.0/ddpw/job.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 
 from .artefacts import ArtefactsConfig
 from .platform import PlatformConfig
 
 
 class Job(object):
   r"""
-  This is a template class with abstract methods to be defined by the user. This
-  class provides methods to define training and evaluation procedures. Once the
-  wrapper has moved the model and the dataset to the appropriate device, it
-  calls :py:meth:`.train()` or :py:meth:`.evaluate()` as configured.
+  This is a template class which is to be defined and passed to
+  :py:meth:`ddpw.wrapper.Wrapper.start`.
   """
 
   p_config: PlatformConfig = None
   r"""
   Platform-related configuration. This property may be used in
   :py:meth:`~Job.__call__` other methods to access the models and the datasets.
 
@@ -42,17 +40,16 @@
   def __call__(self, global_rank: int, local_rank: int):
     r"""
     .. admonition:: Definition required
       :class: important
 
       This method needs to be explicitly defined.
 
-    When once the distributed data parallel setups are completed by the wrapper,
-    this method is called. This method locally updates the dataset and model
-    allotted for the current GPU in case of GPU- and SLURM-based platforms.
+    When once the distributed data parallel setup is completed by the wrapper,
+    this method is called.
 
     :param int global_rank: The global rank of the device.
     :param int local_rank: Local rank of the current device.
     :raises NotImplementedError: Evaluation has not been implemented.
     """
 
     raise NotImplementedError
```

### Comparing `ddpw-4.0.0/ddpw/platform.py` & `ddpw-4.1.0/ddpw/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from enum import Enum
 from typing import final, Optional, Callable
 from dataclasses import dataclass
 
 import torch.distributed as dist
 from .utils import Utils
 
-
 @final
 class Platform(Enum):
   r"""The platform on which to train or evaluate."""
 
   CPU = 0
   r"""The platform to run on is a CPU."""
 
@@ -33,15 +32,15 @@
     """
 
     match num:
       case 0: return Platform.CPU
       case 1: return Platform.GPU
       case 2: return Platform.SLURM
       case 3: return Platform.MPS
-      case _: raise ArgumentError("Undefined platform number given")
+      case _: raise ValueError("Undefined platform number given")
 
 
 @final
 @dataclass
 class PlatformConfig(object):
   r"""
   Platform-related configurations such as the environment, communication IP
@@ -68,14 +67,20 @@
   n_nodes: int = 1
   r"""The total number of nodes. For training on a single cluster of GPUs, this
   property is ``1``. Default: ``1``."""
 
   n_gpus: int = 1
   r"""The total number of GPUs allotted in each node. Default: ``1``."""
 
+  mem_gb: int = 32
+  r"""Memory in GB (for SLURM). Default: ``32``."""
+
+  tasks_per_node: int = 2
+  r"""Number of tasks per node (for SLURM). Default: ``2``."""
+
   master_addr: str = 'localhost'
   r"""The IP address of the master GPU through which interprocess communication
   happens. Default: ``localhost``."""
 
   master_port: str = '1889'
   r"""The port at which IPC happens. Default: ``1889``."""
 
@@ -99,15 +104,16 @@
 
   @property
   def world_size(self):
     r"""World size. This is the total number of GPUs across nodes. For SLURM,
     this is implicitly the number of GPUs allotted on each node multiplied by
     the total number of nodes. Default: ``1``."""
 
-    return self.n_nodes * self.n_gpus
+    return (self.n_nodes if self.platform == Platform.SLURM else 1) \
+      * self.n_gpus
 
   @property
   def requires_ipc(self):
     r"""Needs communication. This property tells whether the setup requires IPC.
     IPC is not required for a single CPU, a single GPU, or Apple M1."""
 
     return self.platform not in [Platform.CPU, Platform.MPS] \
```

### Comparing `ddpw-4.0.0/ddpw/utils.py` & `ddpw-4.1.0/ddpw/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   @staticmethod
   def optimiser_to(optimiser: torch.optim.Optimizer, device: torch.device):
     r"""
     This function offers a simple way to move all parameters of an optimiser or,
     effectively the optimiser itself, to the specified device. This method has
     been taken as is from a `solution
     <https://discuss.pytorch.org/t/moving-optimizer-from-cpu-to-gpu/96068/3>`_
-    suggested on PyTorch's Discuss forum.
+    suggested on `PyTorch Discuss <https://discuss.pytorch.org>`_.
 
     :param torch.optim.Optimizer optimiser: The optimiser to move to a device.
     :param torch.device device: The device to which to move the optimiser.
     """
 
     for param in optimiser.state.values():
       # if any global tensors in the state dict
```

### Comparing `ddpw-4.0.0/ddpw/wrapper.py` & `ddpw-4.1.0/ddpw/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     Utils.print('Setting up the SLURM platform.')
     from submitit import AutoExecutor
 
     executor = AutoExecutor(folder=console_logs)
     executor.update_parameters(
       name=self.p_config.name,
-      mem_gb=12*self.p_config.n_nodes,
+      mem_gb=self.p_config.mem_gb,
       gpus_per_node=self.p_config.n_gpus,
-      tasks_per_node=self.p_config.n_gpus,
+      tasks_per_node=self.p_config.tasks_per_node,
       cpus_per_task=self.p_config.cpus_per_task,
       nodes=self.p_config.n_nodes,
       timeout_min=self.p_config.timeout_min,
       slurm_partition=self.p_config.partition
     )
 
     return executor.submit(individual_gpu)
```

### Comparing `ddpw-4.0.0/ddpw.egg-info/PKG-INFO` & `ddpw-4.1.0/ddpw.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddpw
-Version: 4.0.0
+Version: 4.1.0
 Summary: A utility package to scaffold PyTorch's DDP
 Home-page: https://ddpw.projects.sujal.tv
 Author: Sujal T.V.
 License: UNKNOWN
 Description: # DDPW
         
         [![AWS S3](https://img.shields.io/badge/documentation-sphinx-blue?link=https://ddpw.projects.sujal.tv)](https://ddpw.projects.sujal.tv)
@@ -36,30 +36,30 @@
         ### Usage
         
         ```python
         from ddpw.platform import Platform, PlatformConfig
         from ddpw.artefacts import ArtefactsConfig
         from ddpw.job import JobConfig, JobMode
         from ddpw.wrapper import Wrapper
+        from torchvision.datasets.mnist import MNIST
         
-        from src import MyDataset, MyModel, MyOptimiser, MyTrainer
+        from src import MyModel, MyTrainer
         
-        # datasets
-        train_set = MyDataset(train=True)
-        test_set = MyDataset(train=False)
+        # dataset
+        train_set = MNIST(root='./data/MNSIT', train=True)
         
-        # configure the platform
+        # platform
         p_config = PlatformConfig(platform=Platform.GPU, n_gpus=4, cpus_per_task=2)
         
-        # configure the artefacts (model, dataset, optimiser, etc.)
-        a_config = ArtefactsConfig(train_set=train_set, test_set=test_set,
-            batch_size=64, model=MyModel(), optimiser_loader=MyOptimiser(lr=0.1))
+        # model and dataset
+        a_config = ArtefactsConfig(train_set=train_set, model=MyModel())
         
         # call the job
-        Wrapper(p_config, a_config).start(MyTrainer())
+        wrapper = Wrapper(p_config, a_config)
+        wrapper.start(MyTrainer())
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ddpw-4.0.0/setup.py` & `ddpw-4.1.0/setup.py`

 * *Files identical despite different names*

