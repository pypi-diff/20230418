# Comparing `tmp/numalogic-0.3.7.tar.gz` & `tmp/numalogic-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.3.7.tar", max compression
+gzip compressed data, was "numalogic-0.3.8.tar", max compression
```

## Comparing `numalogic-0.3.7.tar` & `numalogic-0.3.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-03-27 23:39:46.019156 numalogic-0.3.7/LICENSE
--rw-r--r--   0        0        0     5248 2023-03-27 23:39:46.019156 numalogic-0.3.7/README.md
--rw-r--r--   0        0        0      895 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/__init__.py
--rw-r--r--   0        0        0      729 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/_constants.py
--rw-r--r--   0        0        0     1004 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/config/__init__.py
--rw-r--r--   0        0        0     2315 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/config/_config.py
--rw-r--r--   0        0        0     2660 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/config/factory.py
--rw-r--r--   0        0        0        0 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/__init__.py
--rw-r--r--   0        0        0      683 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     2759 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0     2096 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/trainer.py
--rw-r--r--   0        0        0      581 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11308 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6654 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14372 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8315 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4323 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      211 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     4062 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2518 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0     1235 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/postprocess.py
--rw-r--r--   0        0        0      746 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/preprocess/__init__.py
--rw-r--r--   0        0        0     3654 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/preprocess/transformer.py
--rw-r--r--   0        0        0      906 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/registry/__init__.py
--rw-r--r--   0        0        0     2561 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    11670 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0      841 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    11583 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1651 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     3712 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0      215 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/tools/__init__.py
--rw-r--r--   0        0        0     1506 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0     3197 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/tools/data.py
--rw-r--r--   0        0        0      979 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     1059 2023-03-27 23:39:46.047156 numalogic-0.3.7/numalogic/tools/types.py
--rw-r--r--   0        0        0     1992 2023-03-27 23:39:46.051156 numalogic-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 numalogic-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-18 18:28:11.595020 numalogic-0.3.8/LICENSE
+-rw-r--r--   0        0        0     5248 2023-04-18 18:28:11.595020 numalogic-0.3.8/README.md
+-rw-r--r--   0        0        0      895 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/__init__.py
+-rw-r--r--   0        0        0      729 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/_constants.py
+-rw-r--r--   0        0        0     1004 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     2315 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/config/_config.py
+-rw-r--r--   0        0        0     2824 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/config/factory.py
+-rw-r--r--   0        0        0        0 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      683 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     2759 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0     2065 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/trainer.py
+-rw-r--r--   0        0        0      581 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11308 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6654 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14372 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8315 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4323 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      211 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     4062 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2518 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0     6087 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/postprocess.py
+-rw-r--r--   0        0        0      746 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/preprocess/__init__.py
+-rw-r--r--   0        0        0     3654 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/preprocess/transformer.py
+-rw-r--r--   0        0        0      906 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0     2561 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    11670 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0      841 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    11583 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1651 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     3712 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0      215 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0     1789 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0     5960 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/data.py
+-rw-r--r--   0        0        0      979 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     1059 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/types.py
+-rw-r--r--   0        0        0     2013 2023-04-18 18:28:11.623021 numalogic-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 numalogic-0.3.8/PKG-INFO
```

### Comparing `numalogic-0.3.7/LICENSE` & `numalogic-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/README.md` & `numalogic-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/__init__.py` & `numalogic-0.3.8/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/_constants.py` & `numalogic-0.3.8/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/config/__init__.py` & `numalogic-0.3.8/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/config/_config.py` & `numalogic-0.3.8/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/config/factory.py` & `numalogic-0.3.8/numalogic/config/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler
 
 from numalogic.config._config import ModelInfo
 from numalogic.models.autoencoder.variants import (
     VanillaAE,
     SparseVanillaAE,
     Conv1dAE,
     SparseConv1dAE,
     LSTMAE,
     SparseLSTMAE,
     TransformerAE,
     SparseTransformerAE,
 )
-from numalogic.models.threshold import StdDevThreshold, StaticThreshold
-from numalogic.postprocess import TanhNorm
+from numalogic.models.threshold import StdDevThreshold, StaticThreshold, SigmoidThreshold
+from numalogic.postprocess import TanhNorm, ExpMovingAverage
 from numalogic.preprocess import LogTransformer, StaticPowerTransformer, TanhScaler
 from numalogic.tools.exceptions import UnknownConfigArgsError
 
 
 class _ObjectFactory:
     _CLS_MAP = {}
 
@@ -55,19 +53,26 @@
         "LogTransformer": LogTransformer,
         "StaticPowerTransformer": StaticPowerTransformer,
         "TanhScaler": TanhScaler,
     }
 
 
 class PostprocessFactory(_ObjectFactory):
-    _CLS_MAP = {"TanhNorm": TanhNorm}
+    _CLS_MAP = {
+        "TanhNorm": TanhNorm,
+        "ExpMovingAverage": ExpMovingAverage,
+    }
 
 
 class ThresholdFactory(_ObjectFactory):
-    _CLS_MAP = {"StdDevThreshold": StdDevThreshold, "StaticThreshold": StaticThreshold}
+    _CLS_MAP = {
+        "StdDevThreshold": StdDevThreshold,
+        "StaticThreshold": StaticThreshold,
+        "SigmoidThreshold": SigmoidThreshold,
+    }
 
 
 class ModelFactory(_ObjectFactory):
     _CLS_MAP = {
         "VanillaAE": VanillaAE,
         "SparseVanillaAE": SparseVanillaAE,
         "Conv1dAE": Conv1dAE,
```

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/__init__.py` & `numalogic-0.3.8/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/base.py` & `numalogic-0.3.8/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/trainer.py` & `numalogic-0.3.8/numalogic/models/autoencoder/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
+import sys
+import warnings
 
 import pytorch_lightning as pl
 import torch
 from pytorch_lightning import Trainer
 from torch import Tensor
 
 from numalogic.tools.callbacks import ProgressDetails
@@ -25,34 +27,33 @@
 
 class AutoencoderTrainer(Trainer):
     def __init__(
         self,
         max_epochs=100,
         logger=False,
         check_val_every_n_epoch=5,
-        log_every_n_steps=20,
         enable_checkpointing=False,
         enable_progress_bar=False,
         enable_model_summary=False,
-        limit_val_batches=0,
         callbacks=None,
         **trainer_kw
     ):
         if (not callbacks) and enable_progress_bar:
             callbacks = ProgressDetails()
 
+        if not sys.warnoptions:
+            warnings.simplefilter("ignore", category=UserWarning)
+
         super().__init__(
             logger=logger,
             max_epochs=max_epochs,
-            log_every_n_steps=log_every_n_steps,
             check_val_every_n_epoch=check_val_every_n_epoch,
             enable_checkpointing=enable_checkpointing,
             enable_progress_bar=enable_progress_bar,
             enable_model_summary=enable_model_summary,
-            limit_val_batches=limit_val_batches,
             callbacks=callbacks,
             **trainer_kw
         )
 
     def predict(self, model: pl.LightningModule = None, unbatch=True, **kwargs) -> Tensor:
         recon_err = super().predict(model, **kwargs)
         recon_err = torch.vstack(recon_err)
```

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.3.8/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.3.8/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.3.8/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.3.8/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.3.8/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/forecast/variants/naive.py` & `numalogic-0.3.8/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/threshold/_static.py` & `numalogic-0.3.8/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/models/threshold/_std.py` & `numalogic-0.3.8/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/preprocess/__init__.py` & `numalogic-0.3.8/numalogic/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/preprocess/transformer.py` & `numalogic-0.3.8/numalogic/preprocess/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/registry/__init__.py` & `numalogic-0.3.8/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/registry/artifact.py` & `numalogic-0.3.8/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/registry/mlflow_registry.py` & `numalogic-0.3.8/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/synthetic/__init__.py` & `numalogic-0.3.8/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/synthetic/anomalies.py` & `numalogic-0.3.8/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/synthetic/sparsity.py` & `numalogic-0.3.8/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/synthetic/timeseries.py` & `numalogic-0.3.8/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/tools/callbacks.py` & `numalogic-0.3.8/numalogic/tools/callbacks.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,8 +39,13 @@
         self._enable = False
 
     def on_train_epoch_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         super().on_train_epoch_end(trainer, pl_module)
         metrics = self.get_metrics(trainer, pl_module)
         curr_epoch = trainer.current_epoch
         if curr_epoch % self._log_freq == 0:
-            _LOGGER.info("epoch %s, loss: %s", curr_epoch, metrics["loss"])
+            _LOGGER.info("epoch=%s, training_loss=%s", curr_epoch, metrics["loss"])
+
+    def on_validation_epoch_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
+        super().on_validation_epoch_end(trainer, pl_module)
+        metrics = self.get_metrics(trainer, pl_module)
+        _LOGGER.info("validation_loss=%s", metrics["loss"])
```

### Comparing `numalogic-0.3.7/numalogic/tools/exceptions.py` & `numalogic-0.3.8/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/numalogic/tools/types.py` & `numalogic-0.3.8/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.7/pyproject.toml` & `numalogic-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.3.7"
+version = "0.3.8"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
@@ -47,14 +47,15 @@
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.4.2"
 black = "^22.6"
 pytest = "^7.1"
 pytest-cov = "^4.0"
 pylint = "^2.14.2"
 flake8 = "^5.0"
+torchinfo = "^1.7.2"
 
 [tool.poetry.group.jupyter]
 optional = true
 
 [tool.poetry.group.jupyter.dependencies]
 jupyter = "^1.0.0"
 ipykernel = "^6.15.1"
```

### Comparing `numalogic-0.3.7/PKG-INFO` & `numalogic-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.3.7
+Version: 0.3.8
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.8,<3.11
```

