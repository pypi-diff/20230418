# Comparing `tmp/UniTok-3.0.13.tar.gz` & `tmp/UniTok-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.0.13.tar", last modified: Mon Apr 17 08:15:56 2023, max compression
+gzip compressed data, was "UniTok-3.1.0.tar", last modified: Tue Apr 18 12:40:06 2023, max compression
```

## Comparing `UniTok-3.0.13.tar` & `UniTok-3.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.539966 UniTok-3.0.13/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6585 2023-04-17 08:15:56.539869 UniTok-3.0.13/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.0.13/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.536402 UniTok-3.0.13/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.0.13/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.537639 UniTok-3.0.13/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.0.13/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.0.13/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.0.13/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.0.13/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3519 2023-04-17 08:08:49.000000 UniTok-3.0.13/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.0.13/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4388 2023-03-28 09:39:29.000000 UniTok-3.0.13/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.539590 UniTok-3.0.13/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.0.13/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-03-26 10:24:07.000000 UniTok-3.0.13/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.0.13/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.0.13/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.0.13/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.0.13/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.0.13/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.0.13/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8664 2023-03-28 09:40:52.000000 UniTok-3.0.13/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6267 2023-03-28 08:56:34.000000 UniTok-3.0.13/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8382 2023-04-14 07:07:55.000000 UniTok-3.0.13/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-03-28 09:20:42.000000 UniTok-3.0.13/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.537038 UniTok-3.0.13/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6585 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-17 08:15:56.539996 UniTok-3.0.13/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      725 2023-04-17 08:09:02.000000 UniTok-3.0.13/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.144949 UniTok-3.1.0/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:40:06.144835 UniTok-3.1.0/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.0/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.141334 UniTok-3.1.0/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.0/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.142801 UniTok-3.1.0/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.0/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.0/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.0/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.0/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3770 2023-04-18 12:39:51.000000 UniTok-3.1.0/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.0/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4425 2023-04-18 12:28:32.000000 UniTok-3.1.0/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.144541 UniTok-3.1.0/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.0/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-03-26 10:24:07.000000 UniTok-3.1.0/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.0/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.0/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.1.0/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.0/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.0/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.1.0/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-18 12:30:49.000000 UniTok-3.1.0/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6425 2023-04-18 12:35:51.000000 UniTok-3.1.0/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8552 2023-04-18 12:29:04.000000 UniTok-3.1.0/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-03-28 09:20:42.000000 UniTok-3.1.0/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.142156 UniTok-3.1.0/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-18 12:40:06.144981 UniTok-3.1.0/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-18 12:39:51.000000 UniTok-3.1.0/setup.py
```

### Comparing `UniTok-3.0.13/PKG-INFO` & `UniTok-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.0.13
+Version: 3.1.0
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.0.13/README.md` & `UniTok-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok/analysis/lengths.py` & `UniTok-3.1.0/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok/analysis/plot.py` & `UniTok-3.1.0/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok/column.py` & `UniTok-3.1.0/UniTok/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from UniTok.tok import BaseTok
+from typing import Type
+
+
 from tqdm import tqdm
 
 from .global_setting import Global
 from .analysis.lengths import Lengths
-from .tok import IdTok
+from .tok import IdTok, BaseTok
+from .vocab import Vocab
 
 
 class SeqOperator:
     def __init__(
             self,
             max_length: int = 0,
             padding: bool = False,
@@ -38,19 +41,24 @@
     A column of data in a DataFrame.
 
     Args:
         name (str): The name of the column.
         tok (BaseTok): The tokenizer of the column.
         operator (SeqOperator): The operator of the column.
     """
-    def __init__(self, tok: BaseTok, name=None, operator: SeqOperator = None, **kwargs):
+    def __init__(self, tok: BaseTok | Type[BaseTok], name=None, operator: SeqOperator = None, **kwargs):
         self.tok = tok
         self.name = name or tok.vocab.name
         self.operator = operator
 
+        if isinstance(tok, type):
+            assert issubclass(tok, BaseTok)
+            assert name is not None, 'name must be set when tok is a class'
+            self.tok = tok(vocab=Vocab(name=name))
+
         if kwargs:
             if operator:
                 raise ValueError('operator and kwargs cannot be set at the same time')
             self.operator = SeqOperator(
                 max_length=kwargs.get('max_length', 0),
                 padding=kwargs.get('padding', False),
                 slice_post=kwargs.get('slice_post', False),
```

### Comparing `UniTok-3.0.13/UniTok/meta.py` & `UniTok-3.1.0/UniTok/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import warnings
 from typing import List
 
 
 class Col:
     def __init__(self, name, voc=None, max_length=None, padding=None, vocab=None):
         self.name: str = name
-        self.voc: Voc = voc or vocab
+        self.voc: Voc | str = voc or vocab
         self.max_length = max_length
         self.padding = padding
         self.list = max_length is not None
 
     def __eq__(self, other):
         return self.name == other.name and self.voc.name == other.voc.name and self.max_length == other.max_length
 
@@ -25,15 +25,15 @@
         return info
 
 
 class Voc:
     def __init__(self, name, size, cols, store_dir):
         self.name: str = name
         self.size: int = size
-        self.cols: List[Col] = cols
+        self.cols: List[Col | str] = cols
         self.store_dir = store_dir
 
     def __eq__(self, other):
         return self.name == other.name and self.size == other.size
 
     def get_info(self):
         return {
@@ -42,15 +42,15 @@
         }
 
     def export(self, store_dir):
         from .vocab import Vocab
         vocab = Vocab(name=self.name).load(self.store_dir)
         vocab.save(store_dir)
 
-    def merge(self, other):
+    def merge(self, other: 'Voc'):
         cols = self.cols.copy()
         for col in other.cols:
             for _col in cols:
                 if col.name == _col.name:
                     break
             else:
                 cols.append(col)
@@ -67,21 +67,21 @@
 
     def __init__(self, store_dir):
         self.store_dir = store_dir
         self.path = os.path.join(self.store_dir, 'meta.data.json')
 
         data = self.load()
         self.version = data['version']
-        self.cols = data.get('cols') or data['col_info']
-        self.vocs = data.get('vocs') or data['vocab_info']
+        cols = data.get('cols') or data['col_info']
+        vocs = data.get('vocs') or data['vocab_info']
         self.id_col = data['id_col']
 
         # build col-voc graph
-        self.cols = {col: Col(**self.cols[col], name=col) for col in self.cols}
-        self.vocs = {voc: Voc(**self.vocs[voc], name=voc, store_dir=self.store_dir) for voc in self.vocs}
+        self.cols = {col: Col(**cols[col], name=col) for col in cols}  # type: dict[str, Col]
+        self.vocs = {voc: Voc(**vocs[voc], name=voc, store_dir=self.store_dir) for voc in vocs}  # type: dict[str, Voc]
 
         # connect class objects
         for col in self.cols.values():
             col.voc = self.vocs[col.voc]
         for voc in self.vocs.values():
             voc.cols = [self.cols[col] for col in voc.cols]
```

### Comparing `UniTok-3.0.13/UniTok/tok/bert_tok.py` & `UniTok-3.1.0/UniTok/tok/bert_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok/tok/number_tok.py` & `UniTok-3.1.0/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok/tok/split_tok.py` & `UniTok-3.1.0/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok/tok/tok.py` & `UniTok-3.1.0/UniTok/tok/tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok/unidep.py` & `UniTok-3.1.0/UniTok/unidep.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,19 @@
             self.cached_samples[sample[self.id_col]] = sample
         self.cached = True
 
     def __getitem__(self, index):
         index = self._indexes[index]
         return self.pack_sample(index)
 
+    def __iter__(self):
+        """vocab obj list iterator"""
+        for i in range(len(self)):
+            yield self[i]
+
     def __len__(self):
         return self.sample_size
 
     def __str__(self):
         """        UniDep (dir):
 
         Sample Size: 1000
```

### Comparing `UniTok-3.0.13/UniTok/unitok.py` & `UniTok-3.1.0/UniTok/unitok.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import json
 import os
 import warnings
-from typing import Optional
+from typing import Optional, Type
 
 import numpy as np
 import pandas as pd
 
 from .cols import Cols
 from .column import Column, IndexColumn
-from .tok.bert_tok import BertTok
-from .tok.ent_tok import EntTok
-from .tok.id_tok import IdTok
+from .tok import BaseTok, BertTok, EntTok, IdTok
 from .vocab import Vocab
 from .vocabs import Vocabs
 
 
 class UniTok:
     """
     Unified Tokenizer, which can be used to tokenize different types of data in a DataFrame.
@@ -66,18 +64,23 @@
 
     @property
     def vocab_depots(self):
         warnings.warn('vocab_depot is deprecated, '
                       'use vocabs instead (will be removed in 4.x version)', DeprecationWarning)
         return self.vocabs
 
-    def add_col(self, col: Column):
+    def add_col(self, col: Column | str, tok: BaseTok | Type[BaseTok] = None):
         """
         Declare a column in the DataFrame to be tokenized.
         """
+
+        if isinstance(col, str):
+            assert tok is not None, 'tok must be specified when col is a string'
+            col = Column(tok, name=col)
+
         if isinstance(col.tok, IdTok):
             if self.id_col:
                 raise ValueError(f'already exists id column {self.id_col.name} before adding {col.name}')
             self.id_col = col
 
         self.cols[col.name] = col
         self.vocabs.append(col)
```

### Comparing `UniTok-3.0.13/UniTok/vocab.py` & `UniTok-3.1.0/UniTok/vocab.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,17 +119,23 @@
     def __len__(self):
         return len(self.i2o)
 
     def __bool__(self):
         return True
 
     def __iter__(self):
+        """vocab obj list iterator"""
         for i in range(len(self)):
             yield self.i2o[i]
 
+    def __getitem__(self, item):
+        if isinstance(item, int):
+            return self.i2o[item]
+        return self.o2i[item]
+
     """
     Editable Methods
     """
 
     @property
     def oov_default(self):
         warnings.warn('vocab.oov_default is deprecated, '
```

### Comparing `UniTok-3.0.13/UniTok/vocabs.py` & `UniTok-3.1.0/UniTok/vocabs.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/UniTok.egg-info/PKG-INFO` & `UniTok-3.1.0/UniTok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.0.13
+Version: 3.1.0
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.0.13/UniTok.egg-info/SOURCES.txt` & `UniTok-3.1.0/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.13/setup.py` & `UniTok-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='UniTok',
-    version='3.0.13',
+    version='3.1.0',
     keywords=['token', 'tokenizer', 'bert'],
     description='Unified Tokenizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/UnifiedTokenizer',
     author='Jyonn Liu',
```

