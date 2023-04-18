# Comparing `tmp/UniTok-3.1.0.tar.gz` & `tmp/UniTok-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.1.0.tar", last modified: Tue Apr 18 12:40:06 2023, max compression
+gzip compressed data, was "UniTok-3.1.1.tar", last modified: Tue Apr 18 12:51:16 2023, max compression
```

## Comparing `UniTok-3.1.0.tar` & `UniTok-3.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.144949 UniTok-3.1.0/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:40:06.144835 UniTok-3.1.0/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.0/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.141334 UniTok-3.1.0/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.0/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.142801 UniTok-3.1.0/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.0/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.0/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.0/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.0/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3770 2023-04-18 12:39:51.000000 UniTok-3.1.0/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.0/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4425 2023-04-18 12:28:32.000000 UniTok-3.1.0/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.144541 UniTok-3.1.0/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.0/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-03-26 10:24:07.000000 UniTok-3.1.0/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.0/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.0/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.1.0/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.0/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.0/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.1.0/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-18 12:30:49.000000 UniTok-3.1.0/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6425 2023-04-18 12:35:51.000000 UniTok-3.1.0/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8552 2023-04-18 12:29:04.000000 UniTok-3.1.0/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-03-28 09:20:42.000000 UniTok-3.1.0/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:40:06.142156 UniTok-3.1.0/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-18 12:40:06.000000 UniTok-3.1.0/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-18 12:40:06.144981 UniTok-3.1.0/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-18 12:39:51.000000 UniTok-3.1.0/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.194331 UniTok-3.1.1/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:51:16.194217 UniTok-3.1.1/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.1/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.190647 UniTok-3.1.1/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.1/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.192128 UniTok-3.1.1/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.1/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.1/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.1/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.1/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3782 2023-04-18 12:51:00.000000 UniTok-3.1.1/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.1/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4444 2023-04-18 12:50:20.000000 UniTok-3.1.1/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.193904 UniTok-3.1.1/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.1/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-03-26 10:24:07.000000 UniTok-3.1.1/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.1/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.1/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.1.1/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.1/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.1/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.1.1/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8829 2023-04-18 12:49:58.000000 UniTok-3.1.1/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6491 2023-04-18 12:49:05.000000 UniTok-3.1.1/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8552 2023-04-18 12:29:04.000000 UniTok-3.1.1/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-04-18 12:43:49.000000 UniTok-3.1.1/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.191414 UniTok-3.1.1/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-18 12:51:16.194363 UniTok-3.1.1/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-18 12:51:12.000000 UniTok-3.1.1/setup.py
```

### Comparing `UniTok-3.1.0/PKG-INFO` & `UniTok-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.0
+Version: 3.1.1
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.0/README.md` & `UniTok-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/analysis/lengths.py` & `UniTok-3.1.1/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/analysis/plot.py` & `UniTok-3.1.1/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/column.py` & `UniTok-3.1.1/UniTok/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Type
-
+from typing import Type, Union
 
 from tqdm import tqdm
 
 from .global_setting import Global
 from .analysis.lengths import Lengths
 from .tok import IdTok, BaseTok
 from .vocab import Vocab
@@ -41,15 +40,15 @@
     A column of data in a DataFrame.
 
     Args:
         name (str): The name of the column.
         tok (BaseTok): The tokenizer of the column.
         operator (SeqOperator): The operator of the column.
     """
-    def __init__(self, tok: BaseTok | Type[BaseTok], name=None, operator: SeqOperator = None, **kwargs):
+    def __init__(self, tok: Union[BaseTok, Type[BaseTok]], name=None, operator: SeqOperator = None, **kwargs):
         self.tok = tok
         self.name = name or tok.vocab.name
         self.operator = operator
 
         if isinstance(tok, type):
             assert issubclass(tok, BaseTok)
             assert name is not None, 'name must be set when tok is a class'
```

### Comparing `UniTok-3.1.0/UniTok/meta.py` & `UniTok-3.1.1/UniTok/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
 import warnings
-from typing import List
+from typing import List, Union
 
 
 class Col:
     def __init__(self, name, voc=None, max_length=None, padding=None, vocab=None):
         self.name: str = name
-        self.voc: Voc | str = voc or vocab
+        self.voc: Union[Voc, str] = voc or vocab
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
-        self.cols: List[Col | str] = cols
+        self.cols: List[Union[Col, str]] = cols
         self.store_dir = store_dir
 
     def __eq__(self, other):
         return self.name == other.name and self.size == other.size
 
     def get_info(self):
         return {
```

### Comparing `UniTok-3.1.0/UniTok/tok/bert_tok.py` & `UniTok-3.1.1/UniTok/tok/bert_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/tok/number_tok.py` & `UniTok-3.1.1/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/tok/split_tok.py` & `UniTok-3.1.1/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/tok/tok.py` & `UniTok-3.1.1/UniTok/tok/tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/unidep.py` & `UniTok-3.1.1/UniTok/unidep.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.print('loaded', self.sample_size, 'samples!')
 
         self._sample_size = len(self.data[self.id_col])
         if self.sample_size != self._sample_size:
             self.print('resize sample_size to', self._sample_size)
             self.sample_size = self._sample_size
 
-        self.vocabs = Vocabs()
+        self.vocabs = Vocabs()  # type: Union[Dict[str, Vocab], Vocabs]
         for vocab_name in self.vocs:
             self.vocabs.append(Vocab(name=vocab_name).load(self.store_dir))
         self.id2index = self.vocabs[self.id_voc.name].o2i
 
         self._indexes = list(range(self.sample_size))
         self.unions = dict()  # type: Dict[str, List[UniDep]]
```

### Comparing `UniTok-3.1.0/UniTok/unitok.py` & `UniTok-3.1.1/UniTok/unitok.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 import warnings
-from typing import Optional, Type
+from typing import Optional, Type, Dict, Union
 
 import numpy as np
 import pandas as pd
 
 from .cols import Cols
 from .column import Column, IndexColumn
 from .tok import BaseTok, BertTok, EntTok, IdTok
@@ -54,25 +54,25 @@
         >>> # tokenize
         >>> tok.read_file(df).tokenize().store_data('news-sample')
     """
     VER = 'v3.0'
 
     def __init__(self):
         self.cols = Cols()
-        self.vocabs = Vocabs()
+        self.vocabs = Vocabs()  # type: Union[Dict[str, Vocab], Vocabs]
         self.id_col = None  # type: Optional[Column]
         self.data = None
 
     @property
     def vocab_depots(self):
         warnings.warn('vocab_depot is deprecated, '
                       'use vocabs instead (will be removed in 4.x version)', DeprecationWarning)
         return self.vocabs
 
-    def add_col(self, col: Column | str, tok: BaseTok | Type[BaseTok] = None):
+    def add_col(self, col: Union[Column, str], tok: Union[BaseTok, Type[BaseTok]] = None):
         """
         Declare a column in the DataFrame to be tokenized.
         """
 
         if isinstance(col, str):
             assert tok is not None, 'tok must be specified when col is a string'
             col = Column(tok, name=col)
```

### Comparing `UniTok-3.1.0/UniTok/vocab.py` & `UniTok-3.1.1/UniTok/vocab.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok/vocabs.py` & `UniTok-3.1.1/UniTok/vocabs.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/UniTok.egg-info/PKG-INFO` & `UniTok-3.1.1/UniTok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.0
+Version: 3.1.1
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.0/UniTok.egg-info/SOURCES.txt` & `UniTok-3.1.1/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.0/setup.py` & `UniTok-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='UniTok',
-    version='3.1.0',
+    version='3.1.1',
     keywords=['token', 'tokenizer', 'bert'],
     description='Unified Tokenizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/UnifiedTokenizer',
     author='Jyonn Liu',
```

