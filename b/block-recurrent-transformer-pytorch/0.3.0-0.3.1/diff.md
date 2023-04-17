# Comparing `tmp/block-recurrent-transformer-pytorch-0.3.0.tar.gz` & `tmp/block-recurrent-transformer-pytorch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.0.tar", last modified: Mon Apr 17 21:23:56 2023, max compression
+gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.1.tar", last modified: Mon Apr 17 23:34:27 2023, max compression
```

## Comparing `block-recurrent-transformer-pytorch-0.3.0.tar` & `block-recurrent-transformer-pytorch-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/setup.py
```

### Comparing `block-recurrent-transformer-pytorch-0.3.0/LICENSE` & `block-recurrent-transformer-pytorch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.3.0/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.0/README.md` & `block-recurrent-transformer-pytorch-0.3.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     depth = 6,                      # depth
     dim_head = 64,                  # attention head dimensions
     heads = 8,                      # number of attention heads
     max_seq_len = 1024,             # the total receptive field of the transformer, in the paper this was 2 * block size
     block_width = 512,              # block size - total receptive field is max_seq_len, 2 * block size in paper. the block furthest forwards becomes the new cached xl memories, which is a block size of 1 (please open an issue if i am wrong)
     num_state_vectors = 512,        # number of state vectors, i believe this was a single block size in the paper, but can be any amount
     recurrent_layers = (4,),        # where to place the recurrent layer(s) for states with fixed simple gating
-    enhanced_recurrence = True,     # enhanced recurrence from ernie-doc paper, i have seen it to work well on my local machine
     use_flash_attn = True           # use flash attention, if on pytorch 2.0
 )
 
 seq = torch.randint(0, 2000, (1, 1024))
 
 out, mems1, states1 = model(seq)
 out, mems2, states2 = model(seq, xl_memories = mems1, states = states1)
@@ -80,24 +79,14 @@
     journal = {ArXiv},
     year    = {2022},
     volume  = {abs/2203.07852}
 }
 ```
 
 ```bibtex
-@article{Ding2021ERNIEDocAR,
-    title   = {ERNIE-Doc: A Retrospective Long-Document Modeling Transformer},
-    author  = {Siyu Ding and Junyuan Shang and Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang},
-    journal = {ArXiv},
-    year    = {2021},
-    volume  = {abs/2012.15688}
-}
-```
-
-```bibtex
 @article{Shazeer2019FastTD,
     title   = {Fast Transformer Decoding: One Write-Head is All You Need},
     author  = {Noam M. Shazeer},
     journal = {ArXiv},
     year    = {2019},
     volume  = {abs/1911.02150}
 }
```

#### html2text {}

```diff
@@ -12,39 +12,34 @@
 = 8, # number of attention heads max_seq_len = 1024, # the total receptive
 field of the transformer, in the paper this was 2 * block size block_width =
 512, # block size - total receptive field is max_seq_len, 2 * block size in
 paper. the block furthest forwards becomes the new cached xl memories, which is
 a block size of 1 (please open an issue if i am wrong) num_state_vectors = 512,
 # number of state vectors, i believe this was a single block size in the paper,
 but can be any amount recurrent_layers = (4,), # where to place the recurrent
-layer(s) for states with fixed simple gating enhanced_recurrence = True, #
-enhanced recurrence from ernie-doc paper, i have seen it to work well on my
-local machine use_flash_attn = True # use flash attention, if on pytorch 2.0 )
-seq = torch.randint(0, 2000, (1, 1024)) out, mems1, states1 = model(seq) out,
-mems2, states2 = model(seq, xl_memories = mems1, states = states1) out, mems3,
-states3 = model(seq, xl_memories = mems2, states = states2) ``` ## Test on
-Enwik8 First `pip install -r requirements.txt`, then ```bash $ python train.py
-``` ## Todo - [x] use dynamic positional bias - [x] add enhanced recurrence -
-[x] setup local attention blocks, as in the paper - [x] wrapper transformer
-class for training - [x] take care of generation with recurrence in
-`RecurrentTrainWrapper` - [x] add ability to dropout to entire memories and
-states during each segment step during trainng - [x] test full system on enwik8
-locally and ablate states and memories and see effects first hand - [x] make
-sure attention allow for single head key / values too - [x] run a few
-experiments of fixed gating in regular transformers - does not work - [x]
-integrate flash_attention - [x] cache attention mask + rotary embeddings - [ ]
-revisit memformer - [ ] add ability to gate in memorizing transformers knn
-attention layers - [ ] add compressed_memories ## Citations ```bibtex @article
-{Hutchins2022BlockRecurrentT, title = {Block-Recurrent Transformers}, author =
-{DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer and Behnam
-Neyshabur}, journal = {ArXiv}, year = {2022}, volume = {abs/2203.07852} } ```
-```bibtex @article{Ding2021ERNIEDocAR, title = {ERNIE-Doc: A Retrospective
-Long-Document Modeling Transformer}, author = {Siyu Ding and Junyuan Shang and
-Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang}, journal =
-{ArXiv}, year = {2021}, volume = {abs/2012.15688} } ``` ```bibtex @article
+layer(s) for states with fixed simple gating use_flash_attn = True # use flash
+attention, if on pytorch 2.0 ) seq = torch.randint(0, 2000, (1, 1024)) out,
+mems1, states1 = model(seq) out, mems2, states2 = model(seq, xl_memories =
+mems1, states = states1) out, mems3, states3 = model(seq, xl_memories = mems2,
+states = states2) ``` ## Test on Enwik8 First `pip install -
+r requirements.txt`, then ```bash $ python train.py ``` ## Todo - [x] use
+dynamic positional bias - [x] add enhanced recurrence - [x] setup local
+attention blocks, as in the paper - [x] wrapper transformer class for training
+- [x] take care of generation with recurrence in `RecurrentTrainWrapper` - [x]
+add ability to dropout to entire memories and states during each segment step
+during trainng - [x] test full system on enwik8 locally and ablate states and
+memories and see effects first hand - [x] make sure attention allow for single
+head key / values too - [x] run a few experiments of fixed gating in regular
+transformers - does not work - [x] integrate flash_attention - [x] cache
+attention mask + rotary embeddings - [ ] revisit memformer - [ ] add ability to
+gate in memorizing transformers knn attention layers - [ ] add compressed
+memories ## Citations ```bibtex @article{Hutchins2022BlockRecurrentT, title =
+{Block-Recurrent Transformers}, author = {DeLesley S. Hutchins and Imanol
+Schlag and Yuhuai Wu and Ethan Dyer and Behnam Neyshabur}, journal = {ArXiv},
+year = {2022}, volume = {abs/2203.07852} } ``` ```bibtex @article
 {Shazeer2019FastTD, title = {Fast Transformer Decoding: One Write-Head is All
 You Need}, author = {Noam M. Shazeer}, journal = {ArXiv}, year = {2019}, volume
 = {abs/1911.02150} } ``` ```bibtex @inproceedings{Sun2022ALT, title = {A
 Length-Extrapolatable Transformer}, author = {Yutao Sun and Li Dong and Barun
 Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary
 and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex @inproceedings
 {dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
```

### Comparing `block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py` & `block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -589,15 +589,14 @@
         heads = 8,
         all_layers_qk_rmsnorm = False,
         ff_mult = 4,
         max_seq_len = 1024,
         block_width = 512,
         recurrent_layers: Optional[Tuple[int, ...]] = None,
         num_state_vectors = None,
-        enhanced_recurrence = False,
         ignore_index = -100,
         use_flash_attn = False
     ):
         super().__init__()
         num_state_vectors = default(num_state_vectors, block_width)
 
         recurrent_layers = default(recurrent_layers, (depth // 2,)) # default to one recurent layer at middle of the network
@@ -644,16 +643,14 @@
         self.max_seq_len = max_seq_len
         self.block_width = block_width
 
         assert divisible_by(max_seq_len, block_width)
 
         self.ignore_index = ignore_index
 
-        self.enhanced_recurrence = enhanced_recurrence
-
         self.register_buffer('cached_causal_attn_mask', None, persistent = False)
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     def get_causal_attn_mask(self, width):
@@ -769,19 +766,14 @@
 
         input_blocks = x.split(w, dim = -2)
 
         # process each block at a time
 
         for input_block in input_blocks:
 
-            # enhanced recurrence
-
-            if self.enhanced_recurrence and len(xl_memories) > 1:
-                xl_memories = [*xl_memories[1:], xl_memories[0]]
-
             # ready xl memories and states
 
             xl_memories = iter(xl_memories)
             states = iter(states)
 
             next_xl_memories = []
             next_states = []
```

### Comparing `block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.0/setup.py` & `block-recurrent-transformer-pytorch-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'block-recurrent-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.0',
+  version = '0.3.1',
   license='MIT',
   description = 'Block Recurrent Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/block-recurrent-transformer-pytorch',
   keywords = [
```

