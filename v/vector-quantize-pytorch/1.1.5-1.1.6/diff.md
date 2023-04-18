# Comparing `tmp/vector_quantize_pytorch-1.1.5.tar.gz` & `tmp/vector_quantize_pytorch-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.1.5.tar", last modified: Thu Apr 13 20:21:35 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.1.6.tar", last modified: Tue Apr 18 14:58:19 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.1.5.tar` & `vector_quantize_pytorch-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.1.5/LICENSE` & `vector_quantize_pytorch-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.5/PKG-INFO` & `vector_quantize_pytorch-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.1.5
+Version: 1.1.6
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.1.5/README.md` & `vector_quantize_pytorch-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.5/setup.py` & `vector_quantize_pytorch-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.1.5',
+  version = '1.1.6',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,23 +588,26 @@
                     commit_loss = F.mse_loss(detached_quantize, x)
 
                 loss = loss + commit_loss * self.commitment_weight
 
             if self.orthogonal_reg_weight > 0:
                 codebook = self._codebook.embed
 
+                # only calculate orthogonal loss for the activated codes for this batch
+
                 if self.orthogonal_reg_active_codes_only:
-                    # only calculate orthogonal loss for the activated codes for this batch
+                    assert not (is_multiheaded and self.separate_codebook_per_head), 'orthogonal regularization for only active codes not compatible with multi-headed with separate codebooks yet'
                     unique_code_ids = torch.unique(embed_ind)
-                    codebook = codebook[unique_code_ids]
+                    codebook = codebook[:, unique_code_ids]
+
+                num_codes = codebook.shape[-2]
 
-                num_codes = codebook.shape[0]
                 if exists(self.orthogonal_reg_max_codes) and num_codes > self.orthogonal_reg_max_codes:
                     rand_ids = torch.randperm(num_codes, device = device)[:self.orthogonal_reg_max_codes]
-                    codebook = codebook[rand_ids]
+                    codebook = codebook[:, rand_ids]
 
                 orthogonal_reg_loss = orthogonal_loss_fn(codebook)
                 loss = loss + orthogonal_reg_loss * self.orthogonal_reg_weight
 
         if is_multiheaded:
             if self.separate_codebook_per_head:
                 quantize = rearrange(quantize, 'h b n d -> b n (h d)', h = heads)
```

### Comparing `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.1.5
+Version: 1.1.6
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

