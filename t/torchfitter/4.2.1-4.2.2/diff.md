# Comparing `tmp/torchfitter-4.2.1.tar.gz` & `tmp/torchfitter-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchfitter-4.2.1.tar", last modified: Sat Sep 10 15:40:30 2022, max compression
+gzip compressed data, was "torchfitter-4.2.2.tar", last modified: Tue Apr 18 14:07:18 2023, max compression
```

## Comparing `torchfitter-4.2.1.tar` & `torchfitter-4.2.2.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.568268 torchfitter-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-10 15:40:23.000000 torchfitter-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7844 2022-09-10 15:40:30.568268 torchfitter-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7645 2022-09-10 15:40:23.000000 torchfitter-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-10 15:40:30.568268 torchfitter-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-09-10 15:40:23.000000 torchfitter-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.564268 torchfitter-4.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.568268 torchfitter-4.2.1/src/torchfitter/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-10 15:40:30.568268 torchfitter-4.2.1/src/torchfitter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.568268 torchfitter-4.2.1/src/torchfitter/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24173 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/callbacks/_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)    16925 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.568268 torchfitter-4.2.1/src/torchfitter/manager/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.568268 torchfitter-4.2.1/src/torchfitter/trainer/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23113 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/trainer/_trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)    11683 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/trainer/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.568268 torchfitter-4.2.1/src/torchfitter/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/utils/convenience.py
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7593 2022-09-10 15:40:23.000000 torchfitter-4.2.1/src/torchfitter/utils/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:40:30.568268 torchfitter-4.2.1/src/torchfitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7844 2022-09-10 15:40:30.000000 torchfitter-4.2.1/src/torchfitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-09-10 15:40:30.000000 torchfitter-4.2.1/src/torchfitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-10 15:40:30.000000 torchfitter-4.2.1/src/torchfitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-10 15:40:30.000000 torchfitter-4.2.1/src/torchfitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-10 15:40:30.000000 torchfitter-4.2.1/src/torchfitter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    70466 2022-09-10 15:40:23.000000 torchfitter-4.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 14:07:03.000000 torchfitter-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-18 14:07:18.131214 torchfitter-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-18 14:07:03.000000 torchfitter-4.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 14:07:18.131214 torchfitter-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-18 14:07:03.000000 torchfitter-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.127214 torchfitter-4.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/progress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/regularization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/trainer/_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/trainer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    70466 2023-04-18 14:07:03.000000 torchfitter-4.2.2/versioneer.py
```

### Comparing `torchfitter-4.2.1/PKG-INFO` & `torchfitter-4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchfitter
-Version: 4.2.1
+Version: 4.2.2
 Summary: Trainer to optimize PyTorch models
 Author: Alejandro Pérez-Sanjuán
 Requires-Python: >=3.7,
 Description-Content-Type: text/markdown
 
 
 <p align="center">
@@ -81,43 +81,42 @@
 trainer along the PyTorch model. You can also add a regularization procedure if 
 you need/want to do it. The same goes for callbacks: create the desired
 callbacks and pass them to the trainer as a list.
 ```python
 import torch.nn as nn
 import torch.optim as optim
 from torchfitter.trainer import Trainer
-from torchfitter.regularization import L1Regularization
 from torchfitter.callbacks import (
     LoggerCallback,
     EarlyStopping,
-    LearningRateScheduler
+    LearningRateScheduler,
+    L1Regularization,
 )
 
 model = nn.Linear(in_features=1, out_features=1)
 criterion = nn.MSELoss()
 optimizer = optim.Adam(model.parameters())
-regularizer = L1Regularization(regularization_rate=0.01, biases=False)
+l1_reg = L1Regularization(regularization_rate=0.01, biases=False)
 
 # callbacks
 logger = LoggerCallback(update_step=50)
 early_stopping = EarlyStopping(patience=50, load_best=True, path='checkpoint.pt')
 scheduler = LearningRateScheduler(
     scheduler=optim.lr_scheduler.StepLR(optimizer, step_size=500, gamma=0.9)
 )
 
 trainer = Trainer(
     model=model, 
     criterion=criterion,
-    optimizer=optimizer, 
-    regularizer=regularizer,
+    optimizer=optimizer,
     mixed_precision=True,
     accumulate_iter=4, # accumulate gradient every 4 iterations,
     gradient_clipping='norm',
     gradient_clipping_kwrgs={'max_norm': 1.0, 'norm_type': 2.0},
-    callbacks=[logger, early_stopping, scheduler]
+    callbacks=[l1_reg, scheduler, early_stopping, logger]
 )
 
 history = trainer.fit(train_loader, val_loader, epochs=1000)
 ```
 
 Since `torchfitter` leverages the power of `accelerate`, the device management
 will rely on the latter. You can pass your own `accelerate.Accelerator`
```

### Comparing `torchfitter-4.2.1/README.md` & `torchfitter-4.2.2/src/torchfitter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: torchfitter
+Version: 4.2.2
+Summary: Trainer to optimize PyTorch models
+Author: Alejandro Pérez-Sanjuán
+Requires-Python: >=3.7,
+Description-Content-Type: text/markdown
+
 
 <p align="center">
   <img src="assets/logo.png" width="650">
 </p>
 
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/Xylambda/torchfitter?label=VERSION&style=badge)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Xylambda/torchfitter?style=badge)
@@ -73,43 +81,42 @@
 trainer along the PyTorch model. You can also add a regularization procedure if 
 you need/want to do it. The same goes for callbacks: create the desired
 callbacks and pass them to the trainer as a list.
 ```python
 import torch.nn as nn
 import torch.optim as optim
 from torchfitter.trainer import Trainer
-from torchfitter.regularization import L1Regularization
 from torchfitter.callbacks import (
     LoggerCallback,
     EarlyStopping,
-    LearningRateScheduler
+    LearningRateScheduler,
+    L1Regularization,
 )
 
 model = nn.Linear(in_features=1, out_features=1)
 criterion = nn.MSELoss()
 optimizer = optim.Adam(model.parameters())
-regularizer = L1Regularization(regularization_rate=0.01, biases=False)
+l1_reg = L1Regularization(regularization_rate=0.01, biases=False)
 
 # callbacks
 logger = LoggerCallback(update_step=50)
 early_stopping = EarlyStopping(patience=50, load_best=True, path='checkpoint.pt')
 scheduler = LearningRateScheduler(
     scheduler=optim.lr_scheduler.StepLR(optimizer, step_size=500, gamma=0.9)
 )
 
 trainer = Trainer(
     model=model, 
     criterion=criterion,
-    optimizer=optimizer, 
-    regularizer=regularizer,
+    optimizer=optimizer,
     mixed_precision=True,
     accumulate_iter=4, # accumulate gradient every 4 iterations,
     gradient_clipping='norm',
     gradient_clipping_kwrgs={'max_norm': 1.0, 'norm_type': 2.0},
-    callbacks=[logger, early_stopping, scheduler]
+    callbacks=[l1_reg, scheduler, early_stopping, logger]
 )
 
 history = trainer.fit(train_loader, val_loader, epochs=1000)
 ```
 
 Since `torchfitter` leverages the power of `accelerate`, the device management
 will rely on the latter. You can pass your own `accelerate.Accelerator` 
@@ -220,8 +227,8 @@
 ```latex
 @misc{alejandro2019torchfitter,
   title={torchfitter - Simple Trainer to Optimize PyTorch Models},
   author={Alejandro Pérez-Sanjuán},
   year={2020},
   howpublished={\url{https://github.com/Xylambda/torchfitter}},
 }
-```
+```
```

### Comparing `torchfitter-4.2.1/setup.py` & `torchfitter-4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/callbacks/_callbacks.py` & `torchfitter-4.2.2/src/torchfitter/trainer/_trainer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,712 +1,695 @@
-""" Callbacks for the manager class """
-import subprocess
-from typing import List
+import statistics
+import time
+from typing import List, Tuple, Union
 
 import torch
-from rich.progress import BarColumn, Progress, TimeRemainingColumn
-from torch.optim.swa_utils import AveragedModel
+import torchmetrics
+from accelerate import Accelerator
+from numpy import ndarray
+from torch.utils.data.dataloader import DataLoader
 
+from torchfitter.callbacks.base import Callback, CallbackHandler
 from torchfitter.conventions import ParamsDict
-from torchfitter.callbacks.base import Callback
+from torchfitter.trainer._utils import MetricsHandler, TrainerInternalState
 
 
-class EarlyStopping(Callback):
-    """Callback to handle early stopping.
+class Trainer:
+    """Class that eases the training of a PyTorch model.
 
-    `EarlyStopping` will be performed on the validation loss (as it should be).
-    The best observed model will be loaded if `load_best` is True.
+    This class leverages the power of 'accelerate' to handle the device
+    management and the model optimization.
 
-    Paramaters
-    ----------
-    patience : int, optional, default: 50
-        Number of epochs to wait after min has been reached. After 'patience'
-        number of epochs without improvemente, the training stops.
-    load_best : bool, optional, deafult: True
-        Whether to load the best observed parameters (True) or not (False).
-    path : str or Path, optional, default: 'checkpoint.pt'
-        Path to store the best observed parameters.
-    """
-
-    def __init__(self, patience=50, load_best=True, path="checkpoint.pt"):
-        super(EarlyStopping, self).__init__()
-        self.path = path
-        self.patience = patience
-        self.load_best = load_best
-
-        self.log_name = "EarlyStopping"
-
-    def __repr__(self) -> str:
-        return (
-            f"EarlyStopping(patience={self.patience}, "
-            f"load_best={self.load_best})"
-        )
-
-    def on_fit_start(self, params_dict: dict) -> None:
-        self.wait = 0
-        self.stopped_epoch = 0
-        self.best = float("inf")
-
-    def on_epoch_end(self, params_dict: dict) -> None:
-        current_loss = params_dict[ParamsDict.VAL_LOSS]
-        epoch_number = params_dict[ParamsDict.EPOCH_NUMBER]
-        model = params_dict[ParamsDict.MODEL]
-
-        if current_loss < self.best:
-            self.best = current_loss
-            self.wait = 0
-            # save weights
-            best_params = model.state_dict().copy()
-            torch.save(best_params, self.path)
-        else:
-            self.wait += 1
-
-            if self.wait >= self.patience:
-                self.stopped_epoch = epoch_number
-                # send signal to stop training
-                params_dict[ParamsDict.STOP_TRAINING] = True
-                # load best weights
-                if self.load_best:
-                    best_params = torch.load(self.path)
-                    model.load_state_dict(best_params)
-                    self.logger.info("Best observed parameters loaded.")
-
-    def on_fit_end(self, params_dict: dict) -> None:
-        if self.stopped_epoch > 0:
-            self.logger.info(
-                f"Early stopping applied at epoch: {self.stopped_epoch}"
-            )
-
-
-class LoggerCallback(Callback):
-    """
-    `LoggerCallback` is used to log some of the parameters dict in order to
-    monitor the fitting process. The logged parameters are:
-        - Current epoch.
-        - Number of epochs.
-        - Train loss.
-        - Validation loss.
-        - Time / epoch.
-
-    It also outputs the total training time once the fitting process ends.
+    To perform the forward and backward steps the Trainer assumes a batch of
+    tensors is passed where the last tensor contains the labels and all others
+    contain the features, implicitly assuming the model can handle multiple
+    inputs if needed.
+
+    The trainer tracks its state using a
+    'torchfitter.trainer.TrainerInternalState' object. You can also pass a list
+    of callbacks and/or metrics to the trainer. The callbacks will be runned
+    at different points depending on the methods that were filled. The metrics
+    will be runned in the train and validation steps.
+
+    The callbacks will run in the passed order. Meaning, if a callback modifies
+    the loss value after the logging has been performed, the new loss value
+    won't be showed in the logging process. This is a bug and will be fixed in
+    future versions.
 
     Parameters
     ----------
-    update_step : int, optional, default: 50
-        Logs will be performed every 'update_step'.
-    precision : int, optional, default: 2
-        Number of decimals in the numbers.
-    """
-
-    def __init__(self, update_step: int, precision: int = 2):
-        super(LoggerCallback, self).__init__()
-        self.update_step = update_step
-        self.prec = precision
-
-        self.log_name = "LoggerCallback"
-
-    def __repr__(self) -> str:
-        return (
-            f"LoggerCallback(update_step={self.update_step}, "
-            f"precision={self.prec})"
-        )
-
-    def on_fit_start(self, params_dict: dict) -> None:
-        dev = params_dict[ParamsDict.DEVICE]
-        self.logger.info(f"Starting training process on {dev}")
-
-    def on_epoch_end(self, params_dict: dict) -> None:
-        epoch_number = params_dict[ParamsDict.EPOCH_NUMBER]
-        total_epochs = params_dict[ParamsDict.TOTAL_EPOCHS]
-        val_loss = params_dict[ParamsDict.VAL_LOSS]
-        train_loss = params_dict[ParamsDict.TRAIN_LOSS]
-        epoch_time = params_dict[ParamsDict.EPOCH_TIME]
-
-        prec = self.prec
-        msg = (
-            f"Epoch {epoch_number}/{total_epochs} | Train loss: "
-            f"{train_loss:.{prec}e} | Validation loss {val_loss:.{prec}e} | "
-            f"Time/epoch: {epoch_time:.{prec}e} s"
-        )
-
-        if epoch_number % self.update_step == 0 or epoch_number == 1:
-            self.logger.info(msg)
-
-    def on_fit_end(self, params_dict: dict) -> None:
-        total_time = params_dict[ParamsDict.TOTAL_TIME]
-        # final message
-        self.logger.info(
-            f"""End of training. Total time: {total_time:0.5f} seconds"""
-        )
-
-
-class LearningRateScheduler(Callback):
-    """Callback to schedule learning rate.
-
-    `LearningRateScheduler` provides an easy abstraction to schedule the
-    learning rate of the optimizer by calling `scheduler.step()` after the
-    training step has been performed; i.e., `on_train_step_end`.
-
-    If you were to use a learning rate scheduler in addition to stochastic
-    averaging, you must pass both to an instance of `StochasticWeightAveraging`
-    callback instance of creating an instance of `LearningRateScheduler`.
-
-    Parameters
-    ----------
-    scheduler : torch.optim.lr_scheduler._LRScheduler
-        Scheduler use to perform the lr reduction.
-    metric : str, optional, default : torchfitter.conventions.ParamsDict.LOSS
-        Metric to track in order to reduce the learning rate. If you want to
-        use one of the passed metrics you must pass the class name. See
-        examples section.
-    on_train : bool, optional, default: True
-        Whether to watch the train version of the metric (True) or the
-        validation version of the metric (False)
-
-    Examples
-    --------
-    Assume we already have the `kwargs` for the trainer and the necessary
-    imports:
-
-    >>> import torchmetrics
-    >>> from torch.optim.lr_scheduler import ReduceLROnPlateau
-    >>> from torchfitter.callbacks import LearningRateScheduler
-    >>> sch = ReduceLROnPlateau(optimizer, factor=0.1, patience=50)
-
-    The default metric is the loss. You can choose the validation or the
-    training loss or you can pass another metric by doing:
-
-    >>> lr_sch = LearningRateScheduler(
-    ...     scheduler=sch, metric='MeanSquaredError', on_train=False)
-    >>> metrics = [torchmetrics.MeanSquaredError]
-    >>> trainer = Trainer(callbacks=[lr_sch], metrics=metrics, **kwargs)
-
-    References
-    ----------
-    ..[1] PyTorch - How to adjust learning rate
-       https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate
+    model : torch.Module
+        The model to train.
+    criterion : torch.Module
+        Loss function criterion used to optimize the model.
+    optimizer : torch.optim
+        Optimizer to perform the parameters update.
+    mixed_precision : str, optional, {'no', 'fp16', 'bf16'}, default: None
+        Whether or not to use mixed precision training (fp16 or bfloat16). From
+        Accelerate DOC: choose from 'no', 'fp16', 'bf16'. Will default to the
+        value in the environment variable MIXED_PRECISION, which will use the
+        default value in the accelerate config of the current system or the
+        flag passed with the accelerate.launch command. 'fp16' requires pytorch
+        1.6 or higher. 'bf16' requires pytorch 1.10 or higher.
+    callbacks : list of torchfitter.callback.Callback
+        Callbacks to use during the training process. They will be run in the
+        same orther than they are passed.
+    metrics : list of torchmetrics.Metric, optional, default: None
+        List of metrics to compute in the fitting process. Any arbitrary metric
+        can be used as long as it uses the `torchmetrics` API. The metrics will
+        be registered in the internal state using the name of the class. For
+        example, passing `[MeanSquaredError()]` will be registered as
+        `MeanSquaredError`.
+    accelerator : accelerate.Accelerator
+        Accelerator object from 'accelerate'. If no object is passed, the
+        trainer will create an instance with the default parameters.
+    accumulate_iter : int, optional, default: 1
+        Accumulate gradients every 'accumulate_iter' iterations. The default
+        value does not accumulate the gradients. If an instance of Accelerator
+        is passed to the trainer, this parameter will be ignored.
+    gradient_clipping : {None, 'norm', 'value'}
+        Norm gradient clipping or value gradient clipping. If None, gradient
+        clipping won't be applied.
+    gradient_clipping_kwargs : dict, optional, default: None
+        Dictionary containing keyword arguments for gradient clipping
+        algorithm. Example: {max_norm=1, norm_type=2}. See
+        https://huggingface.co/docs/accelerate/accelerator.html for more
+        information.
+
+    Attributes
+    ----------
+    callback_handler : torchfitter.callback.CallbackHandler
+        Handles the passed callbacks.
+    internal_state : torchfitter.trainer.TrainerInternalState
+        Trainer internal parameters state.
+    metrics_handler : torchfitter.trainer.MetricsHandler
+        Handles the passed metrics.
+    gradient_clipping_algo_ : callable
+        Gradient clipping algorithm or None.
 
+    TODO
+    ----
+    - Make callbacks with priority and sort them at the beginning.
     """
 
     def __init__(
         self,
-        scheduler: torch.optim.lr_scheduler._LRScheduler,
-        metric: str = ParamsDict.LOSS,
-        on_train: bool = True,
+        model: torch.nn.Module,
+        criterion: torch.nn.Module,
+        optimizer: torch.optim.Optimizer,
+        mixed_precision: str = None,
+        callbacks: List[Callback] = None,
+        metrics: List[torchmetrics.Metric] = None,
+        accelerator: Accelerator = None,
+        accumulate_iter: int = 1,
+        gradient_clipping: str = None,
+        gradient_clipping_kwargs: dict = None,
     ):
-        super(LearningRateScheduler, self).__init__()
-
-        self.scheduler = scheduler
-        self.metric = metric
-        self.on_train = on_train
-
-    def __repr__(self) -> str:
-        sch = type(self.scheduler).__name__
-        return (
-            f"LearningRateScheduler(scheduler={sch}, metric={self.metric}), "
-            f"on_train={self.on_train}"
-        )
-
-    def on_fit_start(self, params_dict: dict) -> None:
-        accelerator = params_dict[ParamsDict.ACCELERATOR]
-        self.scheduler = accelerator.prepare(self.scheduler)
-
-    def on_train_step_end(self, params_dict: dict) -> None:
-        if self.metric is not None:
-            key = "train" if self.on_train else "validation"
-            epoch_hist = params_dict[ParamsDict.EPOCH_HISTORY]
-            epoch_number = params_dict[ParamsDict.EPOCH_NUMBER]
-
-            # avoid failing in first epoch when on_train=False
-            if epoch_number > 1:
-                metric = epoch_hist[self.metric][key][-1]
-                self.scheduler.step(metric)
+        self.criterion = criterion
+        self.callbacks_list = callbacks
+        self.metrics_list = metrics
+        self.accumulate_iter = accumulate_iter
+        self.gradient_clipping = gradient_clipping
+        self.gradient_clipping_kwargs = gradient_clipping_kwargs
+
+        if accelerator is None:
+            self.accelerator = Accelerator(
+                mixed_precision=mixed_precision,
+                gradient_accumulation_steps=accumulate_iter,
+                step_scheduler_with_optimizer=True,
+            )
         else:
-            self.scheduler.step()
-
+            self.accelerator = accelerator
 
-class GPUStats(Callback):
-    """GPU stats logger.
-
-    The list of available queries can be found on NVIDIA smi queries. See
-    `Notes` section for more information.
+        # wrap withing accelerate environment
+        self.optimizer = self.accelerator.prepare_optimizer(optimizer)
+        self.model = self.accelerator.prepare_model(model)
+
+        # ----- attributes -----
+        self.internal_state = TrainerInternalState(
+            model=self.model, accelerator=self.accelerator, optimizer=optimizer
+        )
+        self.callback_handler = CallbackHandler(
+            callbacks_list=self.callbacks_list
+        )
 
-    Parameters
-    ----------
-    queries : list of str
-        List of queries to log
-    format : str
-        Queries format.
-    update_step : int, optional, default: 50
-        Logs will be performed every 'update_step'.
-
-    Notes
-    -----
-    To check the list of available queries, see
-    https://nvidia.custhelp.com/app/answers/detail/a_id/3751/~/useful-nvidia-smi-queries
+        self.metrics_handler = MetricsHandler(
+            metrics_list=self.metrics_list,
+            criterion=criterion,
+            device=self.internal_state.get_single_param(ParamsDict.DEVICE),
+        )
+        self.gradient_clipping_algo_ = self._prepare_gradient_clipping()
 
-    """
+        if self.metrics_handler.metric_names is not None:
+            names = self.metrics_handler.metric_names
+            self.internal_state.add_metrics(*names)
 
-    def __init__(
+    def fit(
         self,
-        format: str = "csv, nounits, noheader",
-        queries: List[str] = [
-            "name",
-            "temperature.gpu",
-            "utilization.gpu",
-            "utilization.memory",
-            "memory.used",
-        ],
-        update_step=50,
-    ):
-        super(GPUStats, self).__init__()
+        train_loader: DataLoader,
+        val_loader: DataLoader,
+        epochs: int,
+    ) -> dict:
+        """Fit the model.
+
+        Fit the model using the given loaders for the given number of epochs.
+        By default, the trainer does not display any information about the
+        fitting process, but you can use any of the callbacks designed for that
+        purpose or create your own callbacks.
+
+        Parameters
+        ----------
+        train_loader : torch.DataLoader
+            DataLoader to iterate over the train dataset.
+        val_loader : torch.DataLoader
+            DataLoader to iterate over the validation dataset.
+        epochs : int
+            Number of training epochs.
 
-        self.queries = queries
-        self.format = format
-        self.update_step = update_step
+        Returns
+        -------
+        history : dict
+            Dictionay with epoch and batch metrics. The metrics contained in
+            the dictionary will be the passed metrics + criterion results.
 
-        self.log_name = "GPU Stats"
+        """
+        initial_epoch = self.internal_state.get_single_param(
+            key=ParamsDict.EPOCH_NUMBER
+        )
 
-    def __repr__(self) -> str:
-        return (
-            f"GPUStats(format={self.format}, queries={self.queries}, "
-            f"queries={self.queries})"
+        # wrap loaders within accelerate environment
+        train_loader = self.accelerator.prepare_data_loader(train_loader)
+        val_loader = self.accelerator.prepare_data_loader(val_loader)
+
+        # update internal state with loaders
+        self.internal_state.update_params(
+            **{
+                ParamsDict.TRAIN_LOADER: train_loader,
+                ParamsDict.VAL_LOADER: val_loader,
+                ParamsDict.TOTAL_EPOCHS: epochs,
+            }
         )
 
-    def on_epoch_end(self, params_dict: dict) -> None:
-        epoch_number = params_dict[ParamsDict.EPOCH_NUMBER]
+        # track total training time
+        total_start_time = time.perf_counter()
+        self.callback_handler.on_fit_start(self.state_dict())
+
+        # ---- fitting process ----
+        epoch = initial_epoch
+        stop = False
+        while epoch <= epochs and not stop:
+            self.callback_handler.on_epoch_start(self.state_dict())
+
+            # track epoch time
+            epoch_start_time = time.perf_counter()
+
+            # ------- train step -------
+            self.callback_handler.on_train_step_start(self.state_dict())
+            tr_loss = self.train_step(train_loader)  # actual step
+            self.callback_handler.on_train_step_end(self.state_dict())
+
+            # ------- validation step -------
+            self.callback_handler.on_validation_step_start(self.state_dict())
+            val_loss = self.validation_step(val_loader)
+            self.callback_handler.on_validation_step_end(self.state_dict())
+
+            # -------- update internal state to track training --------
+            self.internal_state.update_lr_history(
+                value=self.optimizer.param_groups[0]["lr"], is_batch=False
+            )
 
-        if epoch_number == 1 or epoch_number % self.update_step == 0:
-            stdout = self._get_queries(
-                queries=self.queries, format=self.format
+            # synchronize before measuring time
+            self.accelerator.wait_for_everyone()
+            epoch_time = time.perf_counter() - epoch_start_time
+            self.internal_state.update_params(
+                **{
+                    ParamsDict.VAL_LOSS: val_loss,
+                    ParamsDict.TRAIN_LOSS: tr_loss,
+                    ParamsDict.EPOCH_TIME: epoch_time,
+                }
             )
-            msg = " | ".join(map(str, stdout))  # unpack and format
-            self.logger.info(msg)
 
-    def _get_queries(self, queries, format):
-        stdout = []
+            self.callback_handler.on_epoch_end(self.state_dict())
 
-        for query in queries:
-            out = (
-                subprocess.run(
-                    f"nvidia-smi --query-gpu={query} --format={format}",
-                    stdout=subprocess.PIPE,
-                    encoding="utf-8",
-                )
-                .stdout.replace("\r", " ")
-                .replace("\n", " ")
+            epoch += 1
+            stop = self.internal_state.get_single_param(
+                key=ParamsDict.STOP_TRAINING
+            )
+            self.internal_state.update_params(
+                **{ParamsDict.EPOCH_NUMBER: epoch}
             )
 
-            stdout.append(out)
-
-        return stdout
+        total_time = time.perf_counter() - total_start_time
 
+        self.internal_state.update_params(
+            **{ParamsDict.TOTAL_TIME: total_time}
+        )
+        self.callback_handler.on_fit_end(self.state_dict())
 
-class RichProgressBar(Callback):
-    """
-    This callback displays a progress bar to report the state of the training
-    process: on each epoch, a new bar will be created and stacked below the
-    previous bars.
+        history = self.get_history()
+        return history
 
-    Metrics are logged using the library logger.
+    @torch.no_grad()
+    def predict(
+        self,
+        X: Union[DataLoader, torch.Tensor, ndarray],
+        as_array=False,
+        dtype: str = "float",
+    ) -> Union[torch.Tensor, ndarray]:
+        """
+        Predict function.
 
-    Parameters
-    ----------
-    display_step : int
-        Number of epochs to wait to display the progress bar.
-    precision : int, optional, default: 2
-        Number of decimals to use in the log.
-    log_lr : bool, optional, default: False
-        Whether to log the learning rate (True) or not (False).
-    """
+        Parameters
+        ----------
+        X : torch.Tensor or numpy.ndarray
+            Data to use to make inference.
+        as_array : bool, optional, default: False
+            Whether to output the predictions as a numpy.narray or not.
+        dtype : str, optional, default: "float"
+            Data type to cast input tensor to.
 
-    def __init__(
-        self, display_step: int = 1, log_lr: bool = False, precision: int = 2
-    ):
-        super(RichProgressBar, self).__init__()
+        Returns
+        -------
+        predictions : torch.Tensor or numpy.ndarray
+            Predicted values.
+        """
+        if isinstance(X, DataLoader):
+            _tensor = self.__predict_loader(X)
+            predictions = getattr(_tensor, dtype)()
+
+        elif isinstance(X, ndarray):
+            _numpy = torch.from_numpy(X)
+            X = getattr(_numpy, dtype)()
+            predictions = self.__predict_tensor(X)
+
+        elif isinstance(X, torch.Tensor):
+            _tensor = self.__predict_tensor(X)
+            predictions = getattr(_tensor, dtype)()
 
-        self.display_step = display_step
-        self.prec = precision
-        self.log_lr = log_lr
-
-        self.log_name = "Rich Bar"
-
-    def __repr__(self) -> str:
-        return (
-            f"RichProgressBar(display_step={self.display_step}, "
-            f"log_lr={self.log_lr}, precision={self.precision})"
-        )
-
-    def on_fit_start(self, params_dict: dict) -> None:
-        dev = params_dict[ParamsDict.DEVICE]
-        self.logger.info(f"Starting training process on {dev}\n")
-
-    def on_train_batch_end(self, params_dict: dict) -> None:
-        epoch = params_dict[ParamsDict.EPOCH_NUMBER]
-        accelerator = params_dict[ParamsDict.ACCELERATOR]
-
-        if epoch % self.display_step == 0 or epoch == 1:
-            accelerator.wait_for_everyone()
-            self.progress_bar.advance(self.epoch_task, 1)
-
-    def on_validation_batch_end(self, params_dict: dict) -> None:
-        epoch = params_dict[ParamsDict.EPOCH_NUMBER]
-        accelerator = params_dict[ParamsDict.ACCELERATOR]
-
-        if epoch % self.display_step == 0 or epoch == 1:
-            accelerator.wait_for_everyone()
-            self.progress_bar.advance(self.epoch_task, 1)
-
-    def on_epoch_start(self, params_dict: dict) -> None:
-        # gather necessary objects
-        train_loader = params_dict[ParamsDict.TRAIN_LOADER]
-        val_loader = params_dict[ParamsDict.VAL_LOADER]
-        epoch = params_dict[ParamsDict.EPOCH_NUMBER]
-        total_epochs = params_dict[ParamsDict.TOTAL_EPOCHS]
-
-        # compute number of batches
-        n_elements = len(train_loader) + len(val_loader)
-
-        if epoch % self.display_step == 0 or epoch == 1:
-            self.progress_bar = Progress(
-                "[progress.description]{task.description}",
-                "•",
-                BarColumn(),
-                "•",
-                "[progress.percentage]{task.percentage:>3.0f}%",
-                "•",
-                TimeRemainingColumn(),
-            )
-
-            self.epoch_task = self.progress_bar.add_task(
-                description=f"Epoch {epoch}/{total_epochs}",
-                total=n_elements,
-            )
-            self.progress_bar.start()
-
-    def on_epoch_end(self, params_dict: dict) -> None:
-        epoch = params_dict[ParamsDict.EPOCH_NUMBER]
-
-        if epoch % self.display_step == 0 or epoch == 1:
-            # update metrics
-            text = self.render_text(params_dict[ParamsDict.EPOCH_HISTORY])
-            self.logger.info(text)  # DISC: use included Rich logger?
-            self.progress_bar.stop()
-
-    def on_fit_end(self, params_dict):
-        total_time = params_dict[ParamsDict.TOTAL_TIME]
-        # final message
-        self.logger.info(
-            f"""\nEnd of training. Total time: {total_time:0.5f} seconds"""
-        )
-
-    def render_text(self, update_dict):
-        text_format = ""
-
-        for metric in update_dict:
-            if metric != ParamsDict.HISTORY_LR:
-                train_metric = update_dict[metric]["train"][-1]
-                val_metric = update_dict[metric]["validation"][-1]
-
-                if text_format:  # not empty
-                    text_format = (
-                        f"{text_format} • {metric} -> Train: "
-                        f"{train_metric:.{self.prec}e} | "
-                        f"Validation: {val_metric:.{self.prec}e}"
-                    )
-                else:
-                    text_format = (
-                        f"{metric} -> Train: "
-                        f"{train_metric:.{self.prec}e} | Validation: "
-                        f"{val_metric:.{self.prec}e}"
-                    )
-            else:
-                if self.log_lr:
-                    text_format = (
-                        f"{text_format} • Learning Rate: "
-                        f"{update_dict[metric][-1]}"
-                    )
-
-        return text_format
-
-
-class StochasticWeightAveraging(Callback):
-    """Applies a stochastic weight averaging to the training process.
-
-    If you were to use a learning rate scheduler in addition to stochastic
-    averaging, you must pass both to the constructor of this class instead of
-    creating an individual callback for the standard lr scheduler. See
-    `Examples` section.
+        if as_array:
+            return predictions.cpu().numpy()
+        else:
+            return predictions
 
-    Parameters
-    -----------
-    swa_scheduler : torch.optim.lr_scheduler.Scheduler
-        Stochastic weight averaging scheduler.
-    start_epoch : int
-        Epoch from which to start applying stochastic weight average.
-    scheduler : torch.optim.lr_scheduler._LRScheduler
-        Scheduler use to perform the lr reduction.
-    metric : str, optional, default : torchfitter.conventions.ParamsDict.LOSS
-        Metric to track in order to reduce the learning rate. If you want to
-        use one of the passed metrics you must pass the class name. See
-        examples section.
-    on_train : bool, optional, default: True
-        Whether to watch the train version of the metric (True) or the
-        validation version of the metric (False)
+    def __predict_tensor(self, tensor: torch.Tensor) -> torch.Tensor:
+        """Make prediction for a given torch tensor.
 
-    References
-    ----------
-    .. [1] Pavel Izmailov, Andrew Gordon Wilson and Vincent Queneneville-Belair
-       PyTorch 1.6 now includes Stochastic Weight Averaging
-       https://pytorch.org/blog/pytorch-1.6-now-includes-stochastic-weight-averaging/
-
-    .. [2] PyTorch - Stochastic Weight Averaging
-       https://pytorch.org/docs/stable/optim.html#stochastic-weight-averaging
-
-    Examples
-    --------
-    >>> optimizer, model, criterion = ...
-    >>> swa_model = torch.optim.swa_utils.AveragedModel(model)
-    >>> swa_start = 160
-    >>> scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(
-    ...    optimizer, T_max=300)
-    >>> swa_scheduler = SWALR(optimizer, swa_lr=0.05)
-    >>> swa_callback = StochasticWeightAveraging(
-    ...     swa_scheduler, swa_start, scheduler=scheduler)
-    >>> trainer = Trainer(callbacks=[swa_callback], **kwargs)
-    >>> history = trainer.fit(...)
+        The passed tensor will be moved to the device the accelerator chose at
+        the beginning of the training process.
 
-    Now we can get the SWA model by simply calling:
-    >>> swa_model = swa_callback.get_swa_model()
-    """
+        Parameters
+        ----------
+        tensor : torch.Tensor
+            Tensor to use to make inference.
 
-    def __init__(
-        self,
-        swa_scheduler: torch.optim.swa_utils.SWALR,
-        start_epoch: int,
-        scheduler: torch.optim.lr_scheduler._LRScheduler = None,
-        metric: str = None,
-        on_train: bool = True,
-    ):
-        super(StochasticWeightAveraging, self).__init__()
+        Returns
+        -------
+        torch.Tensor
+            Predicted values.
+        """
+        device = self.accelerator.device
+        tensor = tensor.to(device)
+        return self.model(tensor)
 
-        self.swa_scheduler = swa_scheduler
-        self.start_epoch = start_epoch
-        self.scheduler = scheduler
-        self.metric = metric
-        self.on_train = on_train
+    def __predict_loader(self, loader: DataLoader) -> torch.Tensor:
+        """Make inference prediction for a given torch.DataLoader.
 
-        self.__swa_model = None
+        Useful when the tensor of features does not fit into memory.
+        """
+        _predictions = []
+        loader = self.accelerator.prepare_data_loader(loader)
+        for idx, (feat, lab) in enumerate(loader):
+            _pred = self.model(feat)
+            _predictions.append(_pred)
 
-    def __repr__(self) -> str:
-        return (
-            f"StochasticWeightAveraging(swa_scheduler={self.swa_scheduler}, "
-            f"start_epoch={self.start_epoch})"
-        )
+        predictions = torch.cat(_predictions)
+        return predictions
 
-    def on_fit_start(self, params_dict: dict) -> None:
-        model = params_dict[ParamsDict.MODEL]
-        accelerator = params_dict[ParamsDict.ACCELERATOR]
+    def _prepare_gradient_clipping(self) -> callable:
+        """
+        Identify the gradient clipping algorithm to use.
 
-        self.scheduler = accelerator.prepare(self.scheduler)
-        self.swa_scheduler = accelerator.prepare(self.swa_scheduler)
-        self.__swa_model = AveragedModel(model)
+        Returns
+        -------
+        algo : callable
+            Callable function that wraps the gradient clipping funcionality.
+        """
+        if self.gradient_clipping == "value":
+            algo = self.accelerator.clip_grad_value_
 
-    def on_train_step_end(self, params_dict: dict) -> None:
-        self.__run_scheduler(params_dict=params_dict)
+        elif self.gradient_clipping == "norm":
+            algo = self.accelerator.clip_grad_norm_
 
-    def __run_scheduler(self, params_dict: dict) -> None:
-        """
-        Run appropiate scheduler depending on the epoch number.
-        """
-        epoch = params_dict[ParamsDict.EPOCH_NUMBER]
-        model = params_dict[ParamsDict.MODEL]
+        elif self.gradient_clipping is None:
+            algo = None
 
-        if epoch >= self.start_epoch:
-            # run swa scheduler
-            self.__swa_model.update_parameters(model)
-            self.swa_scheduler.step()
         else:
-            # run "standard" scheduler
-            if self.metric is not None:
-                key = "train" if self.on_train else "validation"
-                epoch_hist = params_dict[ParamsDict.EPOCH_HISTORY]
-                metric = epoch_hist[self.metric][key][-1]
-                self.scheduler.step(metric)
-            else:
-                self.scheduler.step()
+            raise ValueError(
+                "Not supported gradient "
+                f"gradient clipping algorithm: '{self.gradient_clipping}'"
+            )
+        return algo
 
-    def on_fit_end(self, params_dict: dict) -> None:
-        train_loader = params_dict[ParamsDict.TRAIN_LOADER]
-        torch.optim.swa_utils.update_bn(train_loader, self.__swa_model)
+    def reset_parameters(self, reset_model: bool = False) -> None:
+        """
+        Reset the internal dictionary that keeps track of the parameters state.
 
-    def get_swa_model(self) -> torch.nn.Module:
+        Parameters
+        ----------
+        reset_model : bool, optional, default: False
+            True to reset the model state.
         """
-        Getter method for the Stochastic Weight Averaged model.
+        restart_dict = self.internal_state.reset_parameters(
+            reset_model=reset_model
+        )
+        self.params_dict = restart_dict
+
+    def train_step(
+        self, loader: torch.utils.data.dataloader.DataLoader
+    ) -> float:
+        """Perform a train step using the given dataloader.
+
+        A train step consists of running and optimizing the model for each
+        batch in the given train dataloader.
+
+        Parameters
+        ----------
+        loader: torch.utils.data.dataloader.DataLoader
+            Dataloader for train set.
 
         Returns
         -------
-        swa_model : torch.nn.Module
-            SWA model.
+        epoch_loss : float
+            Mean loss of the batch.
         """
-        return self.__swa_model
-
-
-class L1Regularization(Callback):
-    """Applies L1 regularization over the model parameters.
+        self.model.train()
 
-    L1 is usually called 'Lasso Regression' (Least Absolute Shrinkage and
-    Selection Operator). This callbacks is only applied to the train loss.
+        losses = []  # loss as mean of batch losses
+        for batch_idx, batch in enumerate(loader):
+            self.callback_handler.on_train_batch_start(self.state_dict())
+            loss = self.batch_train_step(batch_index=batch_idx, batch=batch)
+            self.callback_handler.on_train_batch_end(self.state_dict())
+
+            losses.append(loss.item())
+
+        # compute accumulated metrics (metric.compute())
+        metrics_accumulated = (
+            self.metrics_handler.accumulated_batch_computation()
+        )
 
-    Parameters
-    ----------
-    regularization_rate : float
-        Regularization rate. Also called `lambda`.
-    biases : bool, optional, default: False
-        Whether to apply regularization over bias terms (True) or not (False).
+        if metrics_accumulated is not None:
+            self.internal_state.update_metrics(
+                is_train=True, is_batch=False, **metrics_accumulated
+            )
 
-    Note
-    ----
-    The penalty term already handles the product by the lambda regularization
-    rate.
+        epoch_loss = statistics.mean(losses)
+        self.internal_state.update_loss_history(
+            value=epoch_loss, is_train=True, is_batch=False
+        )
 
-    """
+        # reset metrics
+        self.metrics_handler.reset_metrics()
+        return epoch_loss
 
-    def __init__(self, regularization_rate: float, biases: bool = False):
-        super().__init__()
+    def batch_train_step(
+        self,
+        batch_index,
+        batch: Tuple[torch.Tensor, torch.Tensor],
+    ) -> torch.Tensor:
+        """Define the computations to perform on each batch for the training
+        loop.
+
+        This step assumes the features are contained in all tensors in the
+        batch but the last, which is assumed to contain the labels.
+
+        Parameters
+        ----------
+        batch_index : int
+            Batch index.
+        batch : tuple
+            Batch to process.
 
-        self.rate = regularization_rate
-        self.biases = biases
+        Returns
+        -------
+        loss : torch.Tensor
+            Train loss graph.
+        """
+        with self.accelerator.accumulate(self.model):
+            # assume last tensor in batch are labels
+            batch_len = len(batch)
+            features, labels = batch[: batch_len - 1], batch[-1]
+
+            # forward propagation
+            out = self.model(*features)
+            loss = self.loss_step(out, labels, is_validation=False)
+
+            # backpropagation
+            self.accelerator.backward(loss)
+
+            # gradient clipping
+            if self.gradient_clipping_algo_ is not None:
+                self.gradient_clipping_algo_(
+                    self.model.parameters(), **self.gradient_clipping_kwargs
+                )
 
-    def on_loss_step_end(self, params_dict: dict) -> None:
-        batch_tr_loss = params_dict[ParamsDict.BATCH_TRAIN_LOSS]
-        device = params_dict[ParamsDict.DEVICE]
-        model = params_dict[ParamsDict.MODEL]
+            self.optimizer.step()
+            self.optimizer.zero_grad()
 
-        # Initialize with tensor, cannot be scalar
-        penalty_term = torch.zeros(1, 1, requires_grad=True).to(device)
+        # compute metrics, needed for accumulated computation
+        metrics_single = self.metrics_handler.single_batch_computation(
+            predictions=out, target=labels
+        )
 
-        for name, param in model.named_parameters():
-            if not self.biases and name.endswith("bias"):
-                continue
+        # ----------- internal state updated ------------
+        if metrics_single is not None:
+            self.internal_state.update_metrics(
+                is_train=True, is_batch=True, **metrics_single
+            )
 
-            penalty_term = penalty_term + param.norm(p=1)
+        # update history
+        self.internal_state.update_loss_history(
+            value=loss.item(), is_train=True, is_batch=True
+        )
 
-        total_penalty = self.rate * penalty_term
-        loss = total_penalty + batch_tr_loss
+        self.internal_state.update_lr_history(
+            value=self.optimizer.param_groups[0]["lr"], is_batch=True
+        )
 
-        # set loss
-        params_dict[ParamsDict.BATCH_TRAIN_LOSS] = loss
+        # update internal state
+        self.internal_state.update_params(
+            **{
+                ParamsDict.TRAIN_BATCH: batch,
+                ParamsDict.TRAIN_BATCH_IDX: batch_index,
+            }
+        )
 
+        return loss
 
-class L2Regularization(Callback):
-    """Applies L2 regularization over the model parameters.
+    @torch.no_grad()
+    def validation_step(
+        self, loader: torch.utils.data.dataloader.DataLoader
+    ) -> float:
+        """Perform a validation step using the given dataloader.
+
+        A validation step consists of running the model for each batch in the
+        given validation dataloader.
+
+        This method runs under the context of "torch.no_grad", which means
+        gradients won't be tracked.
+
+        Parameters
+        ----------
+        loader: torch.utils.data.dataloader.DataLoader
+            Dataloader for validation set.
 
-    L2 is usually called 'Ridge Regression'. This callbacks is only applied to
-    the train loss.
+        Returns
+        -------
+        epoch_loss : float
+            Mean loss of the batch.
+        """
+        self.model.eval()
 
-    Parameters
-    ----------
-    regularization_rate : float
-        Regularization rate. Also called `lambda`.
-    biases : bool, optional, default: False
-        Whether to apply regularization over bias terms (True) or not (False).
+        losses = []  # loss as mean of batch losses
+        for batch_idx, batch in enumerate(loader):
+            self.callback_handler.on_validation_batch_start(self.state_dict())
+            loss = self.batch_validation_step(
+                batch_index=batch_idx, batch=batch
+            )
+            self.callback_handler.on_validation_batch_end(self.state_dict())
+            losses.append(loss.item())
 
-    Note
-    ----
-    The penalty term already handles the product by the lambda regularization
-    rate.
+        # compute accumulated metrics
+        metrics_accumulated = (
+            self.metrics_handler.accumulated_batch_computation()
+        )
 
-    """
+        if metrics_accumulated is not None:
+            self.internal_state.update_metrics(
+                is_train=False, **metrics_accumulated
+            )
 
-    def __init__(self, regularization_rate: float, biases: bool = False):
-        super().__init__()
+        epoch_loss = statistics.mean(losses)
+        self.internal_state.update_loss_history(
+            value=epoch_loss, is_train=False, is_batch=False
+        )
 
-        self.rate = regularization_rate
-        self.biases = biases
+        # reset metrics
+        self.metrics_handler.reset_metrics()
 
-    def on_loss_step_end(self, params_dict: dict) -> None:
-        batch_tr_loss = params_dict[ParamsDict.BATCH_TRAIN_LOSS]
-        device = params_dict[ParamsDict.DEVICE]
-        model = params_dict[ParamsDict.MODEL]
+        return epoch_loss
 
-        # Initialize with tensor, cannot be scalar
-        penalty_term = torch.zeros(1, 1, requires_grad=True).to(device)
+    def batch_validation_step(
+        self, batch_index, batch: Tuple[torch.Tensor, torch.Tensor]
+    ) -> torch.Tensor:
+        """Define the computations to perform on each batch for the validation
+        loop.
+
+        This step assumes the features are contained in all tensors in the
+        batch but the last, which is assumed to contain the labels.
+
+        Parameters
+        ----------
+        batch_index : int
+            Batch index.
+        batch : tuple
+            Batch to process.
 
-        for name, param in model.named_parameters():
-            if not self.biases and name.endswith("bias"):
-                continue
+        Returns
+        -------
+        loss : torch.Tensor
+            Validation loss graph.
+        """
+        # assume last tensor in batch are labels
+        batch_len = len(batch)
+        features, labels = batch[: batch_len - 1], batch[-1]
+
+        out = self.model(*features)
+        loss = self.loss_step(out, labels, is_validation=True)
+
+        # compute metrics, needed for accumulated computation
+        metrics_single = self.metrics_handler.single_batch_computation(
+            predictions=out, target=labels
+        )
 
-            penalty_term = penalty_term + param.norm(p=2)
+        # ----------- internal state updated ------------
+        # update metrics dict
+        if metrics_single is not None:
+            self.internal_state.update_metrics(
+                is_train=False, is_batch=True, **metrics_single
+            )
 
-        total_penalty = self.rate * penalty_term
-        loss = total_penalty + batch_tr_loss
+        # update internal state
+        self.internal_state.update_loss_history(
+            value=loss.item(), is_train=False, is_batch=True
+        )
 
-        # set loss
-        params_dict[ParamsDict.BATCH_TRAIN_LOSS] = loss
+        self.internal_state.update_lr_history(
+            value=self.optimizer.param_groups[0]["lr"], is_batch=True
+        )
 
+        self.internal_state.update_params(
+            **{
+                ParamsDict.VAL_BATCH: batch,
+                ParamsDict.VAL_BATCH_IDX: batch_index,
+            }
+        )
 
-class ElasticNetRegularization(Callback):
-    r"""Linear combination of L1 and L2.
+        return loss
 
-    According to [1], the lasso penalty is somewhat indifferent to the choice
-    among a set of strong but correlated variables. The ridge penalty, on the
-    other hand, tends to shrink the coefficients of correlated variables toward
-    each other. Elastic net combines both using a weighting factor:
+    def loss_step(
+        self, real: torch.Tensor, target: torch.Tensor, is_validation: bool
+    ) -> torch.Tensor:
+        """Compute loss graph.
+
+        If you override this method the passed regularizer algorithms won't be
+        applied unless they are specifically added.
+
+        Parameters
+        ----------
+        real : torch.Tensor
+            Obtained tensor after performing a forward pass.
+        target : torch.Tensor
+            Target tensor to compute loss.
 
-    .. math::
+        Returns
+        -------
+        loss : torch.Tensor
+            Loss graph contained in a (1 x 1) torch.Tensor.
+        """
+        self.callback_handler.on_loss_step_begin(self.state_dict())
+        with self.accelerator.autocast():
+            loss = self.criterion(real, target)
+
+        # select key to update
+        if is_validation:
+            key = ParamsDict.BATCH_VAL_LOSS
+        else:
+            key = ParamsDict.BATCH_TRAIN_LOSS
 
-        \sum_{j=1}^{p} ( \alpha |\beta_{j}| + (1 + \alpha) \beta_{j}^{2} )
+        # store loss graph
+        self.internal_state.update_params(**{key: loss})
 
-    Parameters
-    ----------
-    regularization_rate : float
-        Regularization rate. Also called `lambda`.
-    alpha : float
-        Parameter to determine the mix of the penalties.
-    biases : bool, optional, default: False
-        Whether to apply regularization over bias terms (True) or not (False).
+        # callback and retrieval in case loss was modified
+        self.callback_handler.on_loss_step_end(self.state_dict())
+        loss = self.internal_state.get_single_param(key)
 
-    Note
-    ----
-    The penalty term already handles the product by the lambda regularization
-    rate.
+        return loss
 
-    References
-    ----------
-    .. [1] Trevor Hastie, Robert Tibshirani, Jerome Friedman - The Elements of
-       Statistical Learning.
+    def save_model(self, path):
+        """
+        Convenient method to save the model ensuring it is unwrapped and
+        all processes are done.
 
-    """
+        Parameters
+        ----------
+        path : path-like
+            Path to save the model.
+        """
+        self.accelerator.wait_for_everyone()
+        unwrapped_model = self.accelerator.unwrap_model(self.model)
+        self.accelerator.save(unwrapped_model.state_dict(), path)
 
-    def __init__(
-        self, regularization_rate: float, alpha: float, biases: bool = False
-    ):
-        super().__init__()
+    def load_model(self, path):
+        """
+        Convenient method to load the model ensuring it is unwrapped.
 
-        self.rate = regularization_rate
-        self.biases = biases
-        self.alpha = alpha
+        Parameters
+        ----------
+        path : path-like
+            Path to load the model from.
+        """
+        unwrapped_model = self.accelerator.unwrap_model(self.model)
+        unwrapped_model.load_state_dict(torch.load(path))
+        self.model = unwrapped_model
 
-    def on_loss_step_end(self, params_dict: dict) -> None:
-        batch_tr_loss = params_dict[ParamsDict.BATCH_TRAIN_LOSS]
-        device = params_dict[ParamsDict.DEVICE]
-        model = params_dict[ParamsDict.MODEL]
+    def state_dict(self) -> dict:
+        """Return current state dict.
 
-        # Initialize with tensor, cannot be scalar
-        penalty_term = torch.zeros(1, 1, requires_grad=True).to(device)
+        The state dict will change as the training progresses.
 
-        for name, param in model.named_parameters():
-            if not self.biases and name.endswith("bias"):
-                continue
+        Returns
+        -------
+        state : dict
+            A dictionary containing the current state of the trainer.
+        """
+        state = self.internal_state.get_state_dict()
+        return state
 
-            l1 = param.norm(p=1)
-            l2 = param.norm(p=2)
-            penalty_term = penalty_term + (
-                self.alpha * l1 + (1 - self.alpha) * l2
-            )
+    def get_history(self) -> dict:
+        """Return the training history.
 
-        total_penalty = self.rate * penalty_term
-        loss = total_penalty + batch_tr_loss
+        The history will be created up to the last epoch.
 
-        # set loss
-        params_dict[ParamsDict.BATCH_TRAIN_LOSS] = loss
+        Returns
+        -------
+        history : dict
+            Dictionary containing the history up to the last epoch.
+        """
+        history = {
+            ParamsDict.EPOCH_HISTORY: self.internal_state.get_single_param(
+                key=ParamsDict.EPOCH_HISTORY
+            ),
+            ParamsDict.BATCH_HISTORY: self.internal_state.get_single_param(
+                key=ParamsDict.BATCH_HISTORY
+            ),
+        }
+        return history
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `torchfitter-4.2.1/src/torchfitter/callbacks/base.py` & `torchfitter-4.2.2/src/torchfitter/callbacks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Base callbacks class """
 import logging
 from abc import ABC
 from typing import List
 
-from torchfitter.utils.convenience import get_logger
+from accelerate.logging import get_logger
 
 __all__ = ["Callback", "CallbackHandler"]
 
 
 class Callback(ABC):
     """Base callbacks class.
 
@@ -30,28 +30,22 @@
     .. [1] Keras - keras.callbacks
        https://github.com/keras-team/keras/blob/master/keras/callbacks.py#L609
     """
 
     def __init__(self):
         self.log_name: str = "Callback"
         self.logger: logging.Logger = get_logger(name=self.log_name)
-        level: int = self.logger.level
-        logging.basicConfig(level=level)
 
-    def set_log_level(self, log_level) -> None:
-        """
-        Set the logging level this callback instance.
+    def set_log_level(self, level):
+        # infor level logging
+        logging.basicConfig(level=level)
+        self.logger.setLevel(level)
 
-        Parameters
-        ----------
-        log_level : int
-            Logging level.
-        """
-        self.logger.setLevel(level=log_level)
-        logging.basicConfig(level=log_level)
+    def set_log_name(self, name):
+        self.logger.logger.name = name
 
     def on_train_step_start(self, params_dict: dict) -> None:
         """Called at the start of a training step.
 
         A train step will involve the processing of all train batches included
         in the train dataloader.
 
@@ -278,28 +272,14 @@
         if callbacks_list is None:
             self.handle_callbacks = False
         elif not isinstance(callbacks_list, list):
             raise TypeError("Callbacks must be a list of callbacks")
 
         self.callbacks_list: List[Callback] = callbacks_list
 
-    def set_log_level(self, log_level: int) -> None:
-        """
-        Set the logging level for all callbacks contained in this instance of
-        CallbacksHandler.
-
-        Parameters
-        ----------
-        log_level : int
-            Logging level.
-        """
-        if self.handle_callbacks:
-            for callback in self.callbacks_list:
-                callback.set_log_level(log_level=log_level)
-
     def on_train_step_start(self, params_dict: dict) -> None:
         """Called at the start of a training step.
 
         Call this method for all given callbacks list. Any returned values will
         be ignored by the trainer.
 
         Parameters
```

### Comparing `torchfitter-4.2.1/src/torchfitter/conventions.py` & `torchfitter-4.2.2/src/torchfitter/conventions.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/io.py` & `torchfitter-4.2.2/src/torchfitter/io.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/manager/_manager.py` & `torchfitter-4.2.2/src/torchfitter/manager/_manager.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/testing.py` & `torchfitter-4.2.2/src/torchfitter/testing.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/trainer/_utils.py` & `torchfitter-4.2.2/src/torchfitter/trainer/_utils.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/utils/convenience.py` & `torchfitter-4.2.2/src/torchfitter/utils/convenience.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/utils/data.py` & `torchfitter-4.2.2/src/torchfitter/utils/data.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.1/src/torchfitter/utils/preprocessing.py` & `torchfitter-4.2.2/src/torchfitter/utils/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,19 +215,18 @@
     ----
     * Allow spliting by percentage.
     * Allow single-feature forecasting instead of multi-forecasting.
     * Use `train_test_val_split` to abstract the splitting.
     * Allow selecting the target column.
     """
 
-    def get_train_and_test(array, n_past, n_future):
+    def get_features_and_labels(array, n_past, n_future):
         """
-        Convenient sub-function that wraps to functionality to
-        create a rolling view and select the past as features
-        and the future as labels.
+        Convenient sub-function that wraps the functionality to create a
+        rolling view and select the past as features and the future as labels.
         """
         window_length = n_past + n_future
         roll_view = np.lib.stride_tricks.sliding_window_view(
             array, window_length, axis=0
         )
         X = roll_view[:, :, :n_past]
         y = roll_view[:, :, n_past:]
@@ -249,15 +248,15 @@
         train = scaler.transform(train)
         validation = scaler.transform(validation)
         test = scaler.transform(test)
 
     # get a rolling view of each data chunk
     output = []
     for chunk in [train, validation, test]:
-        X, y = get_train_and_test(
+        X, y = get_features_and_labels(
             array=chunk, n_past=n_past, n_future=n_future
         )
 
         # make a copy to generate a writable array
         if make_writable:
             _tup = (X.copy(), y.copy())
         else:
```

### Comparing `torchfitter-4.2.1/src/torchfitter.egg-info/PKG-INFO` & `torchfitter-4.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: torchfitter
-Version: 4.2.1
-Summary: Trainer to optimize PyTorch models
-Author: Alejandro Pérez-Sanjuán
-Requires-Python: >=3.7,
-Description-Content-Type: text/markdown
-
 
 <p align="center">
   <img src="assets/logo.png" width="650">
 </p>
 
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/Xylambda/torchfitter?label=VERSION&style=badge)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Xylambda/torchfitter?style=badge)
@@ -81,43 +73,42 @@
 trainer along the PyTorch model. You can also add a regularization procedure if 
 you need/want to do it. The same goes for callbacks: create the desired
 callbacks and pass them to the trainer as a list.
 ```python
 import torch.nn as nn
 import torch.optim as optim
 from torchfitter.trainer import Trainer
-from torchfitter.regularization import L1Regularization
 from torchfitter.callbacks import (
     LoggerCallback,
     EarlyStopping,
-    LearningRateScheduler
+    LearningRateScheduler,
+    L1Regularization,
 )
 
 model = nn.Linear(in_features=1, out_features=1)
 criterion = nn.MSELoss()
 optimizer = optim.Adam(model.parameters())
-regularizer = L1Regularization(regularization_rate=0.01, biases=False)
+l1_reg = L1Regularization(regularization_rate=0.01, biases=False)
 
 # callbacks
 logger = LoggerCallback(update_step=50)
 early_stopping = EarlyStopping(patience=50, load_best=True, path='checkpoint.pt')
 scheduler = LearningRateScheduler(
     scheduler=optim.lr_scheduler.StepLR(optimizer, step_size=500, gamma=0.9)
 )
 
 trainer = Trainer(
     model=model, 
     criterion=criterion,
-    optimizer=optimizer, 
-    regularizer=regularizer,
+    optimizer=optimizer,
     mixed_precision=True,
     accumulate_iter=4, # accumulate gradient every 4 iterations,
     gradient_clipping='norm',
     gradient_clipping_kwrgs={'max_norm': 1.0, 'norm_type': 2.0},
-    callbacks=[logger, early_stopping, scheduler]
+    callbacks=[l1_reg, scheduler, early_stopping, logger]
 )
 
 history = trainer.fit(train_loader, val_loader, epochs=1000)
 ```
 
 Since `torchfitter` leverages the power of `accelerate`, the device management
 will rely on the latter. You can pass your own `accelerate.Accelerator` 
@@ -228,8 +219,8 @@
 ```latex
 @misc{alejandro2019torchfitter,
   title={torchfitter - Simple Trainer to Optimize PyTorch Models},
   author={Alejandro Pérez-Sanjuán},
   year={2020},
   howpublished={\url{https://github.com/Xylambda/torchfitter}},
 }
-```
+```
```

### Comparing `torchfitter-4.2.1/versioneer.py` & `torchfitter-4.2.2/versioneer.py`

 * *Files identical despite different names*

