# Comparing `tmp/onediff-0.8.0-py3-none-any.whl.zip` & `tmp/onediff-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 56116 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1034 b- defN 23-Apr-12 01:35 onediff/__init__.py
--rw-r--r--  2.0 unx     5519 b- defN 23-Apr-12 01:35 onediff/graph_utils.py
+Zip file size: 56248 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1034 b- defN 23-Apr-18 09:44 onediff/__init__.py
+-rw-r--r--  2.0 unx     5711 b- defN 23-Apr-17 03:55 onediff/graph_utils.py
 -rw-r--r--  2.0 unx     7755 b- defN 23-Feb-17 07:48 onediff/oneflow_graph_compile_cache.py
--rw-r--r--  2.0 unx    33943 b- defN 23-Apr-12 01:35 onediff/pipeline_alt_diffusion_oneflow.py
--rw-r--r--  2.0 unx    39449 b- defN 23-Mar-27 07:40 onediff/pipeline_stable_diffusion_controlnet_oneflow.py
--rw-r--r--  2.0 unx    36019 b- defN 23-Apr-12 01:35 onediff/pipeline_stable_diffusion_img2img_oneflow.py
--rw-r--r--  2.0 unx    42338 b- defN 23-Apr-12 01:35 onediff/pipeline_stable_diffusion_inpaint_oneflow.py
--rw-r--r--  2.0 unx    34444 b- defN 23-Apr-12 01:35 onediff/pipeline_stable_diffusion_oneflow.py
+-rw-r--r--  2.0 unx    34025 b- defN 23-Apr-18 09:43 onediff/pipeline_alt_diffusion_oneflow.py
+-rw-r--r--  2.0 unx    39531 b- defN 23-Apr-18 09:43 onediff/pipeline_stable_diffusion_controlnet_oneflow.py
+-rw-r--r--  2.0 unx    36101 b- defN 23-Apr-18 09:43 onediff/pipeline_stable_diffusion_img2img_oneflow.py
+-rw-r--r--  2.0 unx    42420 b- defN 23-Apr-18 09:43 onediff/pipeline_stable_diffusion_inpaint_oneflow.py
+-rw-r--r--  2.0 unx    34526 b- defN 23-Apr-18 09:43 onediff/pipeline_stable_diffusion_oneflow.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-22 07:03 onediff/demo/__init__.py
 -rw-r--r--  2.0 unx     1180 b- defN 23-Feb-17 07:48 onediff/demo/__main__.py
--rw-r--r--  2.0 unx      884 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1239 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/RECORD
-14 files, 203904 bytes uncompressed, 54032 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx      884 b- defN 23-Apr-18 09:44 onediff-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 09:44 onediff-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-18 09:44 onediff-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1239 b- defN 23-Apr-18 09:44 onediff-0.9.0.dist-info/RECORD
+14 files, 204506 bytes uncompressed, 54164 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: onediff/demo/__init__.py
 Comment: 
 
 Filename: onediff/demo/__main__.py
 Comment: 
 
-Filename: onediff-0.8.0.dist-info/METADATA
+Filename: onediff-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: onediff-0.8.0.dist-info/WHEEL
+Filename: onediff-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: onediff-0.8.0.dist-info/top_level.txt
+Filename: onediff-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: onediff-0.8.0.dist-info/RECORD
+Filename: onediff-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onediff/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __author__ = "OneFlow"
 __credits__ = "OneFlow contributors"
 import oneflow as flow
 
 
 # monkey patch hacks
 flow.strided = None
```

## onediff/graph_utils.py

```diff
@@ -102,28 +102,32 @@
             state_dict = flow.load(os.path.join(path, "vae"))
             vae_graph = get_vae_graph(
                 cache_size=self.cache_size,
                 enable_shared=self.enable_shared,
                 enable_save=self.enable_save,
                 vae_post_process=vae_post_process,
             )
+            flow._oneflow_internal.eager.Sync()
             vae_graph.load_runtime_state_dict(state_dict)
+            flow._oneflow_internal.eager.Sync()
             self.graph_dict["vae"] = vae_graph
 
         # compile unet graph
         unet_graph = None
         if compile_unet:
             state_dict = flow.load(os.path.join(path, "unet"))
             unet_graph = get_unet_graph(
                 cache_size=self.cache_size,
                 enable_shared=self.enable_shared,
                 enable_save=self.enable_save,
                 unet=self.unet,
             )
+            flow._oneflow_internal.eager.Sync()
             unet_graph.load_runtime_state_dict(state_dict)
+            flow._oneflow_internal.eager.Sync()
             self.graph_dict["unet"] = unet_graph
 
     def get_graph(self, graph_class, graph):
         if graph_class == "unet":
             if graph_class not in self.graph_dict:
                 self.graph_dict[graph_class] = get_unet_graph(
                     cache_size=self.cache_size,
```

## onediff/pipeline_alt_diffusion_oneflow.py

```diff
@@ -97,14 +97,15 @@
         os.environ["ONEFLOW_MLIR_FUSE_OPS_WITH_BACKWARD_IMPL"] = "1"
         os.environ["ONEFLOW_MLIR_GROUP_MATMUL"] = "1"
         os.environ["ONEFLOW_MLIR_PREFER_NHWC"] = "1"
 
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_CONV_BIAS"] = "1"
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_LINEAR"] = "1"
 
+        os.environ["ONEFLOW_KERNEL_CONV_CUTLASS_IMPL_ENABLE_TUNING_WARMUP"] = "1"
         os.environ["ONEFLOW_KERENL_CONV_ENABLE_CUTLASS_IMPL"] = "1"
         # NOTE: avoid overflow
         if "upcast_attention" in unet.config and unet.config.upcast_attention:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "0"
         else:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "1"
         os.environ["ONEFLOW_KERNEL_GLU_ENABLE_DUAL_GEMM_IMPL"] = "1"
```

## onediff/pipeline_stable_diffusion_controlnet_oneflow.py

```diff
@@ -102,14 +102,15 @@
         os.environ["ONEFLOW_MLIR_FUSE_FORWARD_OPS"] = "1"
         os.environ["ONEFLOW_MLIR_GROUP_MATMUL"] = "1"
         os.environ["ONEFLOW_MLIR_PREFER_NHWC"] = "1"
 
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_CONV_BIAS"] = "1"
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_LINEAR"] = "1"
 
+        os.environ["ONEFLOW_KERNEL_CONV_CUTLASS_IMPL_ENABLE_TUNING_WARMUP"] = "1"
         os.environ["ONEFLOW_KERENL_CONV_ENABLE_CUTLASS_IMPL"] = "1"
         # NOTE: avoid overflow
         if "upcast_attention" in unet.config and unet.config.upcast_attention:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "0"
         else:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "1"
         os.environ["ONEFLOW_KERNEL_GLU_ENABLE_DUAL_GEMM_IMPL"] = "1"
```

## onediff/pipeline_stable_diffusion_img2img_oneflow.py

```diff
@@ -119,14 +119,15 @@
         os.environ["ONEFLOW_MLIR_FUSE_FORWARD_OPS"] = "1"
         os.environ["ONEFLOW_MLIR_GROUP_MATMUL"] = "1"
         os.environ["ONEFLOW_MLIR_PREFER_NHWC"] = "1"
 
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_CONV_BIAS"] = "1"
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_LINEAR"] = "1"
 
+        os.environ["ONEFLOW_KERNEL_CONV_CUTLASS_IMPL_ENABLE_TUNING_WARMUP"] = "1"
         os.environ["ONEFLOW_KERENL_CONV_ENABLE_CUTLASS_IMPL"] = "1"
         # NOTE: avoid overflow
         if "upcast_attention" in unet.config and unet.config.upcast_attention:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "0"
         else:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "1"
         os.environ["ONEFLOW_KERNEL_GLU_ENABLE_DUAL_GEMM_IMPL"] = "1"
```

## onediff/pipeline_stable_diffusion_inpaint_oneflow.py

```diff
@@ -174,14 +174,15 @@
         os.environ["ONEFLOW_MLIR_FUSE_OPS_WITH_BACKWARD_IMPL"] = "1"
         os.environ["ONEFLOW_MLIR_GROUP_MATMUL"] = "1"
         os.environ["ONEFLOW_MLIR_PREFER_NHWC"] = "1"
 
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_CONV_BIAS"] = "1"
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_LINEAR"] = "1"
 
+        os.environ["ONEFLOW_KERNEL_CONV_CUTLASS_IMPL_ENABLE_TUNING_WARMUP"] = "1"
         os.environ["ONEFLOW_KERENL_CONV_ENABLE_CUTLASS_IMPL"] = "1"
         # NOTE: avoid overflow
         if "upcast_attention" in unet.config and unet.config.upcast_attention:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "0"
         else:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "1"
         os.environ["ONEFLOW_KERNEL_GLU_ENABLE_DUAL_GEMM_IMPL"] = "1"
```

## onediff/pipeline_stable_diffusion_oneflow.py

```diff
@@ -89,14 +89,15 @@
         os.environ["ONEFLOW_MLIR_FUSE_OPS_WITH_BACKWARD_IMPL"] = "1"
         os.environ["ONEFLOW_MLIR_GROUP_MATMUL"] = "1"
         os.environ["ONEFLOW_MLIR_PREFER_NHWC"] = "1"
 
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_CONV_BIAS"] = "1"
         os.environ["ONEFLOW_KERNEL_ENABLE_FUSED_LINEAR"] = "1"
 
+        os.environ["ONEFLOW_KERNEL_CONV_CUTLASS_IMPL_ENABLE_TUNING_WARMUP"] = "1"
         os.environ["ONEFLOW_KERENL_CONV_ENABLE_CUTLASS_IMPL"] = "1"
         # NOTE: avoid overflow
         if "upcast_attention" in unet.config and unet.config.upcast_attention:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "0"
         else:
             os.environ["ONEFLOW_KERENL_FMHA_ENABLE_TRT_FLASH_ATTN_IMPL"] = "1"
         os.environ["ONEFLOW_KERNEL_GLU_ENABLE_DUAL_GEMM_IMPL"] = "1"
```

## Comparing `onediff-0.8.0.dist-info/METADATA` & `onediff-0.9.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 0.8.0
+Version: 0.9.0
 Summary: OneFlow backend for diffusers
 Home-page: https://github.com/Oneflow-Inc/oneflow
 Author: OneFlow contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `onediff-0.8.0.dist-info/RECORD` & `onediff-0.9.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-onediff/__init__.py,sha256=CtlTHEuGToe0bjNBdcsvTX77fb61CXchTJqBNt0dOjc,1034
-onediff/graph_utils.py,sha256=9sf3v84zTDUSdpaIG6xZee7OFr7xzydSX7vvdGJDr8g,5519
+onediff/__init__.py,sha256=ptVpFAYvVojNBqllIZwYiDwQy-chzDclhzD_89E9tew,1034
+onediff/graph_utils.py,sha256=Q2bbnWa2Oa5zeCcc2ghkTe-ntQn9QROW5ZoCcwvqlxo,5711
 onediff/oneflow_graph_compile_cache.py,sha256=MEyY_r1NPy0lTzHxWPaUCIqkqO6a5m5pQpsVZx9-Mps,7755
-onediff/pipeline_alt_diffusion_oneflow.py,sha256=4WjJE84kCtJIzYc8JMT2Y2WxssaPRJfuYRcHIDcaDDM,33943
-onediff/pipeline_stable_diffusion_controlnet_oneflow.py,sha256=fzdNRCEjI2T4RKlaLyYwPAn7fRiaSkiEMK0m2YHBggo,39449
-onediff/pipeline_stable_diffusion_img2img_oneflow.py,sha256=e9Fa4y_GkrA0-thhBJhvjgB_WvwYn8CBX_JTLr5w8Wg,36019
-onediff/pipeline_stable_diffusion_inpaint_oneflow.py,sha256=ZrMsqZslPr9a5G34m8GoHwADx6-vgkElQ4jWIpS4i5U,42338
-onediff/pipeline_stable_diffusion_oneflow.py,sha256=ILui5Dz6koZ00MDviyNj8_Rvq2LNWT1MaUA1XMDlKYk,34444
+onediff/pipeline_alt_diffusion_oneflow.py,sha256=mxd9rQ94GuLuRbK9ZVbaSmyaXLUU5FzsB6PO791vA24,34025
+onediff/pipeline_stable_diffusion_controlnet_oneflow.py,sha256=Zji-mNzH6ktHakwRn0khNmDye4gxVqszsp-ADSacKsI,39531
+onediff/pipeline_stable_diffusion_img2img_oneflow.py,sha256=3O8ItL9Wr6an20L4PuGNBxIltj1nXSPfY19OQvTE294,36101
+onediff/pipeline_stable_diffusion_inpaint_oneflow.py,sha256=wQiFl77xcmj7n7ALPnJ4geFugr84Y4_zIFpt3InpSRY,42420
+onediff/pipeline_stable_diffusion_oneflow.py,sha256=0TGKjUuErt8fKe9nQsL9Ql13U-YRjL9bGcgfIOeYaD8,34526
 onediff/demo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 onediff/demo/__main__.py,sha256=Aiw2Qp8JXovxf39OrTlqAbuThcs-oQoLJcalCK45ND8,1180
-onediff-0.8.0.dist-info/METADATA,sha256=k5q7XspIkSQpSMvl8RXu4j7RVBCYFU9RrJBFXD-wJ-Y,884
-onediff-0.8.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-onediff-0.8.0.dist-info/top_level.txt,sha256=Xpq1rI4xb3FC5zjKRboGD55jUQ_MY6BbDhKch1Biat0,8
-onediff-0.8.0.dist-info/RECORD,,
+onediff-0.9.0.dist-info/METADATA,sha256=jPYSlHDFBlhhwUGayDM1aJoga0RTyvBhzet7yeWVk_Y,884
+onediff-0.9.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+onediff-0.9.0.dist-info/top_level.txt,sha256=Xpq1rI4xb3FC5zjKRboGD55jUQ_MY6BbDhKch1Biat0,8
+onediff-0.9.0.dist-info/RECORD,,
```

