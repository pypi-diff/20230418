# Comparing `tmp/block-recurrent-transformer-pytorch-0.3.2.tar.gz` & `tmp/block-recurrent-transformer-pytorch-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.2.tar", last modified: Tue Apr 18 01:45:29 2023, max compression
+gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.3.tar", last modified: Tue Apr 18 18:18:17 2023, max compression
```

## Comparing `block-recurrent-transformer-pytorch-0.3.2.tar` & `block-recurrent-transformer-pytorch-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30065 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:18:17.827175 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/setup.py
```

### Comparing `block-recurrent-transformer-pytorch-0.3.2/LICENSE` & `block-recurrent-transformer-pytorch-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.3.2/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.2
+Version: 0.3.3
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.2/README.md` & `block-recurrent-transformer-pytorch-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py` & `block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from random import random
 from functools import wraps, partial
-from collections import namedtuple
+from collections import namedtuple, defaultdict
 from packaging import version
 
 from einops import rearrange
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
@@ -20,14 +20,17 @@
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
 
+def all_unique(arr):
+    return len(arr) == len(set(arr))
+
 def eval_decorator(fn):
     def inner(self, *args, **kwargs):
         was_training = self.training
         self.eval()
         out = fn(self, *args, **kwargs)
         self.train(was_training)
         return out
@@ -217,26 +220,31 @@
 
         self.state_out_to_gate = nn.Linear(dim, dim)
         self.learned_ema_beta = nn.Parameter(torch.randn(dim))
 
         # since each read should be followed by a write, just store cache in the container
 
         self.cache = None
+        self.next_read_state = None
 
-    def read(
+    def set_next_read_state(
         self,
-        x,
-        *,
-        states = None,
+        states
     ):
-        # use initial state if no states were passed in
-
         if not exists(states):
             states = self.init_state
 
+        self.next_read_state = (states,)
+
+    def read(self, x):
+        assert exists(self.next_read_state), 'states to be read must be set with .set_next_read_state'
+
+        states, = self.next_read_state
+        self.next_read_state = None
+
         # pre norm state for attention
 
         normed_states = self.state_norm(states)
 
         # add the positional ids, as stated in the paper critical for it to work
 
         normed_states = normed_states + self.state_pos_ids
@@ -519,16 +527,18 @@
         self,
         dim,
         block_width,
         dim_head = 64,
         heads = 8,
         qk_rmsnorm = False,
         qk_rmsnorm_scale = 8,
+        use_flash_attn = False,
         num_state_vectors = 0,
-        use_flash_attn = False
+        num_external_state_reads = 0,
+        state_read_before_write = True  # this will be defaulted to on as in the paper, but will be turned off in the case the researcher wants to test out reading the state at a lower layer
     ):
         super().__init__()
         inner_dim = dim_head * heads
         self.heads = heads
 
         self.norm = LayerNorm(dim)
 
@@ -537,19 +547,25 @@
         self.to_kv = nn.Linear(dim, dim_head * 2, bias = False)
 
         self.attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
 
         self.block_width = block_width
         self.is_recurrent_layer = num_state_vectors > 0
 
-        self.to_out = nn.Linear(inner_dim * (2 if self.is_recurrent_layer else 1), dim, bias = False)
+        # decide how many states this attention layer is going to read from
+
+        num_state_reads = int(self.is_recurrent_layer and state_read_before_write) + num_external_state_reads
+
+        self.to_out = nn.Linear(inner_dim * (1 + num_state_reads), dim, bias = False)
 
         if not self.is_recurrent_layer:
             return
 
+        self.state_read_before_write = state_read_before_write
+
         self.state_container = StateContainer(
             dim,
             dim_head = dim_head,
             heads = heads,
             num_state_vectors = num_state_vectors,
             qk_rmsnorm = qk_rmsnorm,
             qk_rmsnorm_scale = qk_rmsnorm_scale,
@@ -563,15 +579,15 @@
     def forward(
         self,
         x,
         rotary_pos_emb = None,
         xpos_scale = None,
         attn_mask = None,
         xl_memories: Optional[torch.Tensor] = None,
-        states: Optional[torch.Tensor] = None
+        read_from_state_containers: List[StateContainer] = []
     ):
         batch, seq_len, _, width, device = *x.shape, self.block_width, self.device
 
         # pre normalization
 
         x = self.norm(x)
 
@@ -611,28 +627,37 @@
 
         # merge heads
 
         out = rearrange(out, 'b h n d -> b n (h d)')
 
         # early return if not a recurrent layer
 
-        if not self.is_recurrent_layer:
+        if not self.is_recurrent_layer and len(read_from_state_containers) == 0:
             return self.to_out(out), memories, None
 
-        # read from the states ...
+        # whether to read from own state container, default to on, but may pass in more
+
+        if self.is_recurrent_layer and self.state_read_before_write:
+            read_from_state_containers = [self.state_container, *read_from_state_containers]
+
+        for read_state_container in read_from_state_containers:
+            # read from the states ...
 
-        to_state_out = self.state_container.read(x, states = states)
+            to_state_out = read_state_container.read(x)
 
-        # and concat it to the output of self-attention
+            # and concat it to the output of self-attention
 
-        out = torch.cat((out, to_state_out), dim = -1)
+            out = torch.cat((out, to_state_out), dim = -1)
 
-        # then write to the states as well
+        new_states = None
 
-        new_states = self.state_container.write(memories = memories)
+        if self.is_recurrent_layer:
+            # then write to the states as well if need be
+
+            new_states = self.state_container.write(memories = memories)
 
         return self.to_out(out), memories, new_states
 
 # classes
 
 @beartype
 class BlockRecurrentTransformer(nn.Module):
@@ -645,57 +670,92 @@
         dim_head = 64,
         heads = 8,
         all_layers_qk_rmsnorm = False,
         ff_mult = 4,
         max_seq_len = 1024,
         block_width = 512,
         recurrent_layers: Optional[Tuple[int, ...]] = None,
+        read_recurrent_layers: Optional[Tuple[int, ...]] = None,
         num_state_vectors = None,
         ignore_index = -100,
         use_flash_attn = False
     ):
         super().__init__()
         num_state_vectors = default(num_state_vectors, block_width)
 
+        # set recurrent layers
+
         recurrent_layers = default(recurrent_layers, (depth // 2,)) # default to one recurent layer at middle of the network
-        self.recurrent_layers = set(recurrent_layers)
 
-        assert all([0 < layer <= depth for layer in recurrent_layers])
+        assert all([0 < layer <= depth for layer in recurrent_layers]), f'recurrent layers must range from 1 to the depth {depth}'
+        assert all_unique(recurrent_layers), 'recurrent layers must be all unique. no duplicate layers'
+
+        self.recurrent_layers = recurrent_layers
+
+        # set read recurrent layers
+
+        read_recurrent_layers = default(read_recurrent_layers, recurrent_layers)
+
+        assert all([read_layer <= write_layer for read_layer, write_layer in zip(read_recurrent_layers, recurrent_layers)]), 'the recurrent read layer must be always less than or equal to the write layer'
+        assert all([0 < layer <= depth for layer in read_recurrent_layers])
+        assert len(read_recurrent_layers) == len(recurrent_layers)
+
+        self.read_recurrent_layers = read_recurrent_layers
+
+        # token embedding
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
         self.rotary_pos_emb = RotaryEmbedding(dim = dim_head)
 
         self.layers = nn.ModuleList([])
 
+        self.write_to_read_map = {write_layer: read_layer for write_layer, read_layer in zip(recurrent_layers, read_recurrent_layers)}
+
+        self.read_state_router = defaultdict(list)
+
         for layer in range(1, depth + 1):
             is_recurrent_layer = layer in self.recurrent_layers
 
             layer_num_state_vectors = num_state_vectors if is_recurrent_layer else 0
 
+            num_external_state_reads = sum([int(layer == read_layer) for read_layer in read_recurrent_layers])
+
             # only layers with xl memories
             # or has recurrence in horizontal direction
             # use qk rmsnorm (in paper, they use cosine sim attention, but i think qk rmsnorm is more proven given Vit 22B paper)
             # one can also override to use all qk rmsnorm by setting all_layers_qk_rmsnorm = True
 
             qk_rmsnorm = all_layers_qk_rmsnorm or is_recurrent_layer
 
+            attn_block = AttentionBlock(
+                dim,
+                block_width = block_width,
+                dim_head = dim_head,
+                heads = heads,
+                qk_rmsnorm = qk_rmsnorm,
+                num_state_vectors = layer_num_state_vectors,
+                use_flash_attn = use_flash_attn,
+                num_external_state_reads = num_external_state_reads,
+                state_read_before_write = False,
+            )
+
+            ff_block = FeedForward(dim, mult = ff_mult)
+
+            if is_recurrent_layer:
+                read_layer = self.write_to_read_map[layer]
+                self.read_state_router[read_layer].append(attn_block.state_container)
+
             self.layers.append(nn.ModuleList([
-                AttentionBlock(
-                    dim,
-                    block_width = block_width,
-                    dim_head = dim_head,
-                    heads = heads,
-                    qk_rmsnorm = qk_rmsnorm,
-                    num_state_vectors = layer_num_state_vectors,
-                    use_flash_attn = use_flash_attn
-                ),
-                FeedForward(dim, mult = ff_mult)
+                attn_block,
+                ff_block
             ]))
 
+        # to logits
+
         self.to_logits = nn.Sequential(
             LayerNorm(dim),
             nn.Linear(dim, num_tokens, bias = False)
         )
 
         self.max_seq_len = max_seq_len
         self.block_width = block_width
@@ -831,35 +891,40 @@
 
             xl_memories = iter(xl_memories)
             states = iter(states)
 
             next_xl_memories = []
             next_states = []
 
+            # set the states on the appropriate state containers
+
+            for attn, _ in self.layers:
+                if not attn.is_recurrent_layer:
+                    continue
+
+                attn.state_container.set_next_read_state(next(states, None))
+
             # go through layers
 
             for ind, (attn, ff) in enumerate(self.layers):
 
                 # determine if the layer requires transformer xl memories
 
                 layer = ind + 1
-                is_state_layer  = attn.is_recurrent_layer
 
                 # whether to pass in xl memories
 
                 attn_kwargs = dict(
                     rotary_pos_emb = rotary_pos_emb,
                     xpos_scale = xpos_scale,
                     attn_mask = attn_mask,
-                    xl_memories = next(xl_memories, None)
+                    xl_memories = next(xl_memories, None),
+                    read_from_state_containers = self.read_state_router[layer]
                 )
 
-                if is_state_layer:
-                    attn_kwargs.update(states = next(states, None))
-
                 # attention layer
 
                 residual = input_block
                 attn_branch_out, layer_xl_memories, layer_next_states = attn(input_block, **attn_kwargs)
 
                 if exists(layer_xl_memories):
                     next_xl_memories.append(layer_xl_memories)
```

### Comparing `block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.2
+Version: 0.3.3
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.2/setup.py` & `block-recurrent-transformer-pytorch-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'block-recurrent-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.2',
+  version = '0.3.3',
   license='MIT',
   description = 'Block Recurrent Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/block-recurrent-transformer-pytorch',
   keywords = [
```

