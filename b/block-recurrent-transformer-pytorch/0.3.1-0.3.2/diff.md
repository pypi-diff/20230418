# Comparing `tmp/block-recurrent-transformer-pytorch-0.3.1.tar.gz` & `tmp/block-recurrent-transformer-pytorch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.1.tar", last modified: Mon Apr 17 23:34:27 2023, max compression
+gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.2.tar", last modified: Tue Apr 18 01:45:29 2023, max compression
```

## Comparing `block-recurrent-transformer-pytorch-0.3.1.tar` & `block-recurrent-transformer-pytorch-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 23:34:27.000000 block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:34:27.207910 block-recurrent-transformer-pytorch-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 23:34:16.000000 block-recurrent-transformer-pytorch-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30065 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 01:45:29.000000 block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:45:29.873057 block-recurrent-transformer-pytorch-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-18 01:45:14.000000 block-recurrent-transformer-pytorch-0.3.2/setup.py
```

### Comparing `block-recurrent-transformer-pytorch-0.3.1/LICENSE` & `block-recurrent-transformer-pytorch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.3.1/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.1/README.md` & `block-recurrent-transformer-pytorch-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py` & `block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,14 +172,152 @@
 
 # maybe flash attention, if using pytorch 2.0
 
 # constants
 
 Config = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
+# state container
+
+class StateContainer(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        num_state_vectors,
+        dim_head = 64,
+        heads = 8,
+        qk_rmsnorm = False,
+        qk_rmsnorm_scale = 8,
+        use_flash_attn = False
+    ):
+        super().__init__()
+        assert num_state_vectors > 0
+        self.heads = heads
+        inner_dim = dim_head * heads
+
+        self.state_norm = LayerNorm(dim)
+
+        self.q_to_state = nn.Linear(dim, inner_dim, bias = False)
+        self.q_from_state = nn.Linear(dim, inner_dim, bias = False)
+
+        self.state_to_q = nn.Linear(dim, inner_dim, bias = False)
+        self.state_to_kv = nn.Linear(dim, dim_head * 2, bias = False)
+
+        self.init_state = nn.Parameter(torch.randn(num_state_vectors, dim))
+        self.state_pos_ids = nn.Parameter(torch.randn(num_state_vectors, dim))
+
+        self.to_state_out = nn.Linear(inner_dim * 2, dim, bias = False)
+
+        self.to_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
+
+        self.state_self_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
+        self.from_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
+
+        # gating related parameters - using the fixed simple config
+
+        self.state_out_to_gate = nn.Linear(dim, dim)
+        self.learned_ema_beta = nn.Parameter(torch.randn(dim))
+
+        # since each read should be followed by a write, just store cache in the container
+
+        self.cache = None
+
+    def read(
+        self,
+        x,
+        *,
+        states = None,
+    ):
+        # use initial state if no states were passed in
+
+        if not exists(states):
+            states = self.init_state
+
+        # pre norm state for attention
+
+        normed_states = self.state_norm(states)
+
+        # add the positional ids, as stated in the paper critical for it to work
+
+        normed_states = normed_states + self.state_pos_ids
+
+        # get queries for cross attention, which they do not share, although they share key / values. another intriguing detail
+
+        q_to_state = self.q_to_state(x)
+        q_to_state = rearrange(q_to_state, '... n (h d) -> ... h n d', h = self.heads)
+
+        # self attention qkv for states
+
+        state_k, state_v = self.state_to_kv(normed_states).chunk(2, dim = -1)
+
+        # cross attend to the past states key values
+
+        to_state_out = self.to_state_cross_attn(q_to_state, state_k, state_v)
+
+        to_state_out = rearrange(to_state_out, 'b h n d -> b n (h d)')
+
+        # cache for next write
+
+        self.cache = (states, normed_states, state_k, state_v)
+
+        return to_state_out
+
+    def write(
+        self,
+        *,
+        memories
+    ):
+        assert exists(self.cache)
+
+        k, v = memories
+        batch = k.shape[0]
+
+        # get cached values from the previous read
+
+        states, normed_states, state_k, state_v = self.cache
+
+        self.cache = None
+
+        # derive queries
+
+        q_from_state = self.q_from_state(normed_states)
+        q_from_state = rearrange(q_from_state, '... n (h d) -> ... h n d', h = self.heads)
+
+        state_q = self.state_to_q(normed_states)
+        state_q_einsum = 'n (h d)' if state_q.ndim == 2 else 'b n (h d)'
+        state_q = repeat(state_q, f'{state_q_einsum} -> b h n d', h = self.heads, b = batch)
+
+        # states must also undergo self attention
+
+        if q_from_state.ndim == 3:
+            q_from_state = repeat(q_from_state, '... -> b ...', b = batch)
+
+        state_out = self.state_self_attn(state_q, state_k, state_v)
+
+        from_state_out = self.from_state_cross_attn(q_from_state, k, v)
+
+        state_out = torch.cat((state_out, from_state_out), dim = -1)
+        state_out = rearrange(state_out, 'b h n d -> b n (h d)')
+
+        state_out = self.to_state_out(state_out)
+
+        # use the best performing configuration
+        # fixed simple gate - nothing more than a learned EMA with some resemblance to highway networks
+
+        z = self.state_out_to_gate(state_out)
+        learned_ema_decay = self.learned_ema_beta.sigmoid()
+
+        # set new state with the learned EMA gating
+
+        return learned_ema_decay * z + (1 - learned_ema_decay) * states
+
+    def forward(self, x):
+        raise NotImplementedError
+
 # main class
 
 class Attend(nn.Module):
     def __init__(
         self,
         causal = False,
         use_flash_attn = False
@@ -404,48 +542,34 @@
         self.is_recurrent_layer = num_state_vectors > 0
 
         self.to_out = nn.Linear(inner_dim * (2 if self.is_recurrent_layer else 1), dim, bias = False)
 
         if not self.is_recurrent_layer:
             return
 
-        self.state_norm = LayerNorm(dim)
-
-        self.q_to_state = nn.Linear(dim, inner_dim, bias = False)
-        self.q_from_state = nn.Linear(dim, inner_dim, bias = False)
-
-        self.state_to_q = nn.Linear(dim, inner_dim, bias = False)
-        self.state_to_kv = nn.Linear(dim, dim_head * 2, bias = False)
-
-        self.init_state = nn.Parameter(torch.randn(num_state_vectors, dim))
-        self.state_pos_ids = nn.Parameter(torch.randn(num_state_vectors, dim))
-
-        self.to_state_out = nn.Linear(inner_dim * 2, dim, bias = False)
-
-        self.to_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
-
-        self.state_self_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
-        self.from_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
-
-        # gating related parameters - using the fixed simple config
-
-        self.state_out_to_gate = nn.Linear(dim, dim)
-        self.learned_ema_beta = nn.Parameter(torch.randn(dim))
+        self.state_container = StateContainer(
+            dim,
+            dim_head = dim_head,
+            heads = heads,
+            num_state_vectors = num_state_vectors,
+            qk_rmsnorm = qk_rmsnorm,
+            qk_rmsnorm_scale = qk_rmsnorm_scale,
+            use_flash_attn = use_flash_attn
+        )
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     def forward(
         self,
         x,
         rotary_pos_emb = None,
         xpos_scale = None,
         attn_mask = None,
-        return_memories_and_states = None,
         xl_memories: Optional[torch.Tensor] = None,
         states: Optional[torch.Tensor] = None
     ):
         batch, seq_len, _, width, device = *x.shape, self.block_width, self.device
 
         # pre normalization
 
@@ -456,18 +580,15 @@
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
 
         split_head = partial(rearrange, pattern = 'b n (h d) -> b h n d', h = self.heads)
         q = split_head(q)
 
         # save the last key / values as memories for recurrence
 
-        memories = None
-
-        if return_memories_and_states:
-            memories = torch.stack((k, v))
+        memories = torch.stack((k, v))
 
         mem_len = 0
 
         if exists(xl_memories):
             # if past memories are passed in, concat as the first bucket
             mem_len = xl_memories.shape[-2]
             past_k, past_v = xl_memories
@@ -484,100 +605,36 @@
         out = self.attn(
             q, k, v,
             rotary_pos_emb = rotary_pos_emb,
             xpos_scale = xpos_scale,
             mask = attn_mask
         )
 
-        new_states = None
-
         # merge heads
 
         out = rearrange(out, 'b h n d -> b n (h d)')
 
         # early return if not a recurrent layer
 
         if not self.is_recurrent_layer:
-            return self.to_out(out), memories, new_states
-
-        # if designated a recurrent layer, do all the state logic
-        # it was hard moving this to a separate module, as the attention is closely intertwined between the current tokens and state tokens
-
-        # ready attended output of the input to the state, concatted block by block
+            return self.to_out(out), memories, None
 
-        to_state_out = torch.empty((batch, 0, out.shape[-1]), device = device, dtype = out.dtype)
-
-        # use initial state if no states were passed in
-
-        if not exists(states):
-            states = self.init_state
+        # read from the states ...
 
-        # state residual
+        to_state_out = self.state_container.read(x, states = states)
 
-        residual_states = states
+        # and concat it to the output of self-attention
 
-        # pre norm state for attention
-
-        states = self.state_norm(states)
-
-        # add the positional ids, as stated in the paper critical for it to work
-
-        states = states + self.state_pos_ids
-
-        # get queries for cross attention, which they do not share, although they share key / values. another intriguing detail
-
-        q_to_state = self.q_to_state(x)
-        q_from_state = self.q_from_state(states)
-
-        q_to_state, q_from_state = map(lambda t: rearrange(t, '... n (h d) -> ... h n d', h = self.heads), (q_to_state, q_from_state))
-
-        # self attention qkv for states
-
-        state_q, state_k, state_v = (self.state_to_q(states), *self.state_to_kv(states).chunk(2, dim = -1))
-
-        state_q_einsum = 'n (h d)' if state_q.ndim == 2 else 'b n (h d)'
-        state_q = repeat(state_q, f'{state_q_einsum} -> b h n d', h = self.heads, b = batch)
-
-        # cross attend to the past states key values
-
-        to_state_out_block = self.to_state_cross_attn(q_to_state, state_k, state_v)
-
-        to_state_out_block = rearrange(to_state_out_block, 'b h n d -> b n (h d)')
-
-        to_state_out = torch.cat((to_state_out, to_state_out_block), dim = -2)
-
-        # states must also undergo self attention
-
-        if q_from_state.ndim == 3:
-            q_from_state = repeat(q_from_state, '... -> b ...', b = batch)
-
-        state_out = self.state_self_attn(state_q, state_k, state_v)
-
-        from_state_out = self.from_state_cross_attn(q_from_state, k, v)
-
-        state_out = torch.cat((state_out, from_state_out), dim = -1)
-        state_out = rearrange(state_out, 'b h n d -> b n (h d)')
-
-        state_out = self.to_state_out(state_out)
-
-        # use the best performing configuration
-        # fixed simple gate - nothing more than a learned EMA with some resemblance to highway networks
-
-        z = self.state_out_to_gate(state_out)
-        learned_ema_decay = self.learned_ema_beta.sigmoid()
-
-        # set new state with the learned EMA gating
-
-        states = learned_ema_decay * z + (1 - learned_ema_decay) * residual_states
+        out = torch.cat((out, to_state_out), dim = -1)
 
-        # concat the output of cross attending to the state vectors
+        # then write to the states as well
 
-        out = torch.cat((out, to_state_out), dim = -1)
+        new_states = self.state_container.write(memories = memories)
 
-        return self.to_out(out), memories, states
+        return self.to_out(out), memories, new_states
 
 # classes
 
 @beartype
 class BlockRecurrentTransformer(nn.Module):
     def __init__(
         self,
@@ -789,16 +846,15 @@
 
                 # whether to pass in xl memories
 
                 attn_kwargs = dict(
                     rotary_pos_emb = rotary_pos_emb,
                     xpos_scale = xpos_scale,
                     attn_mask = attn_mask,
-                    xl_memories = next(xl_memories, None),
-                    return_memories_and_states = return_memories_and_states
+                    xl_memories = next(xl_memories, None)
                 )
 
                 if is_state_layer:
                     attn_kwargs.update(states = next(states, None))
 
                 # attention layer
```

### Comparing `block-recurrent-transformer-pytorch-0.3.1/block_recurrent_transformer_pytorch.egg-info/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.1/setup.py` & `block-recurrent-transformer-pytorch-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'block-recurrent-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.1',
+  version = '0.3.2',
   license='MIT',
   description = 'Block Recurrent Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/block-recurrent-transformer-pytorch',
   keywords = [
```

