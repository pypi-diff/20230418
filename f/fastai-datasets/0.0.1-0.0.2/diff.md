# Comparing `tmp/fastai-datasets-0.0.1.tar.gz` & `tmp/fastai-datasets-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-datasets-0.0.1.tar", last modified: Thu Apr 13 12:32:30 2023, max compression
+gzip compressed data, was "fastai-datasets-0.0.2.tar", last modified: Tue Apr 18 07:51:35 2023, max compression
```

## Comparing `fastai-datasets-0.0.1.tar` & `fastai-datasets-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:32:30.555302 fastai-datasets-0.0.1/
--rw-rw-rw-   0        0        0    11538 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      116 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1246 2023-04-13 12:32:30.554292 fastai-datasets-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-04-13 12:19:24.000000 fastai-datasets-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 12:32:30.518244 fastai-datasets-0.0.1/fastai_datasets/
--rw-rw-rw-   0        0        0       23 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/__init__.py
--rw-rw-rw-   0        0        0    11588 2023-04-13 12:19:39.000000 fastai-datasets-0.0.1/fastai_datasets/_modidx.py
--rw-rw-rw-   0        0        0      479 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/cifar10.py
--rw-rw-rw-   0        0        0     4661 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/lfw.py
--rw-rw-rw-   0        0        0      886 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/mnist.py
--rw-rw-rw-   0        0        0     3456 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/pairs.py
--rw-rw-rw-   0        0        0     5121 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/patches.py
--rw-rw-rw-   0        0        0      769 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/pfr.py
--rw-rw-rw-   0        0        0      940 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/test.py
--rw-rw-rw-   0        0        0     1693 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/fastai_datasets/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:32:30.551290 fastai-datasets-0.0.1/fastai_datasets.egg-info/
--rw-rw-rw-   0        0        0     1246 2023-04-13 12:32:30.000000 fastai-datasets-0.0.1/fastai_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-04-13 12:32:30.000000 fastai-datasets-0.0.1/fastai_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:32:30.000000 fastai-datasets-0.0.1/fastai_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-13 12:32:30.000000 fastai-datasets-0.0.1/fastai_datasets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 12:18:49.000000 fastai-datasets-0.0.1/fastai_datasets.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2023-04-13 12:32:30.000000 fastai-datasets-0.0.1/fastai_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 12:32:30.000000 fastai-datasets-0.0.1/fastai_datasets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1033 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/settings.ini
--rw-rw-rw-   0        0        0       42 2023-04-13 12:32:30.556298 fastai-datasets-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2617 2023-04-13 12:15:33.000000 fastai-datasets-0.0.1/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-18 07:51:35.308423 fastai-datasets-0.0.2/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.2/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.2/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5790 2023-04-18 07:51:35.304423 fastai-datasets-0.0.2/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4144 2023-04-18 07:11:00.000000 fastai-datasets-0.0.2/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-18 07:51:35.304423 fastai-datasets-0.0.2/fastai_datasets/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       21 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12364 2023-04-18 07:11:00.000000 fastai-datasets-0.0.2/fastai_datasets/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.2/fastai_datasets/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/cifar10.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/imagenette.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/lfw.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/mnist.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3354 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/pairs.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5806 2023-04-18 07:11:00.000000 fastai-datasets-0.0.2/fastai_datasets/patches.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/pfr.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2231 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-18 07:51:35.304423 fastai-datasets-0.0.2/fastai_datasets.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5790 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-04-18 07:51:29.000000 fastai-datasets-0.0.2/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-04-18 07:51:35.308423 fastai-datasets-0.0.2/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.2/setup.py
```

### Comparing `fastai-datasets-0.0.1/fastai_datasets/_modidx.py` & `fastai-datasets-0.0.2/fastai_datasets/_modidx.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,106 @@
-# Autogenerated by nbdev
-
-d = { 'settings': { 'branch': 'main',
-                'doc_baseurl': '/fastai-datasets',
-                'doc_host': 'https://Irad-Zehavi.github.io',
-                'git_url': 'https://github.com/Irad-Zehavi/fastai-datasets',
-                'lib_path': 'fastai_datasets'},
-  'syms': { 'fastai_datasets.cifar10': {'fastai_datasets.cifar10.CIFAR10': ('cifar10.html#cifar10', 'fastai_datasets/cifar10.py')},
-            'fastai_datasets.lfw': { 'fastai_datasets.lfw.LFW': ('Facial Recognition/lfw.html#lfw', 'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFW.__init__': ( 'Facial Recognition/lfw.html#lfw.__init__',
-                                                                           'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFW._fetch_file': ( 'Facial Recognition/lfw.html#lfw._fetch_file',
-                                                                              'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFW._get_path': ( 'Facial Recognition/lfw.html#lfw._get_path',
-                                                                            'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFW._load': ('Facial Recognition/lfw.html#lfw._load', 'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFW._parse_items': ( 'Facial Recognition/lfw.html#lfw._parse_items',
-                                                                               'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFW._url': ('Facial Recognition/lfw.html#lfw._url', 'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFW.test': ('Facial Recognition/lfw.html#lfw.test', 'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWDevMixin': ( 'Facial Recognition/lfw.html#lfwdevmixin',
-                                                                          'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWDevMixin.dev': ( 'Facial Recognition/lfw.html#lfwdevmixin.dev',
-                                                                              'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWPairs': ('Facial Recognition/lfw.html#lfwpairs', 'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWPairsMixin': ( 'Facial Recognition/lfw.html#lfwpairsmixin',
-                                                                            'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWPairsMixin._load': ( 'Facial Recognition/lfw.html#lfwpairsmixin._load',
-                                                                                  'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWPairsMixin._parse_items': ( 'Facial '
-                                                                                         'Recognition/lfw.html#lfwpairsmixin._parse_items',
-                                                                                         'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWPeople': ('Facial Recognition/lfw.html#lfwpeople', 'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWPeople._load': ( 'Facial Recognition/lfw.html#lfwpeople._load',
-                                                                              'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.LFWPeople._parse_items': ( 'Facial Recognition/lfw.html#lfwpeople._parse_items',
-                                                                                     'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.SLLFWPairs': ('Facial Recognition/lfw.html#sllfwpairs', 'fastai_datasets/lfw.py'),
-                                     'fastai_datasets.lfw.SLLFWPairs._parse_items': ( 'Facial Recognition/lfw.html#sllfwpairs._parse_items',
-                                                                                      'fastai_datasets/lfw.py')},
-            'fastai_datasets.mnist': { 'fastai_datasets.mnist.MNIST': ('mnist.html#mnist', 'fastai_datasets/mnist.py'),
-                                       'fastai_datasets.mnist.TinyMNIST': ('mnist.html#tinymnist', 'fastai_datasets/mnist.py')},
-            'fastai_datasets.pairs': { 'fastai_datasets.pairs.ImagePair': ('pairs.html#imagepair', 'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.ImagePair.create': ( 'pairs.html#imagepair.create',
-                                                                                   'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.ImagePair.show': ('pairs.html#imagepair.show', 'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.Pairs': ('pairs.html#pairs', 'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.Sameness': ('pairs.html#sameness', 'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.Sameness.__init__': ( 'pairs.html#sameness.__init__',
-                                                                                    'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.Sameness.encodes': ( 'pairs.html#sameness.encodes',
-                                                                                   'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs._pairs_for_split': ( 'pairs.html#_pairs_for_split',
-                                                                                   'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.show_batch': ('pairs.html#show_batch', 'fastai_datasets/pairs.py')},
-            'fastai_datasets.patches': { 'fastai_datasets.patches.Datasets.__add__': ( 'Core/patches.html#datasets.__add__',
-                                                                                       'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.__sub__': ( 'Core/patches.html#datasets.__sub__',
-                                                                                       'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.by_target': ( 'Core/patches.html#datasets.by_target',
-                                                                                         'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.dl': ( 'Core/patches.html#datasets.dl',
-                                                                                  'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.dls': ( 'Core/patches.html#datasets.dls',
-                                                                                   'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.i2t': ( 'Core/patches.html#datasets.i2t',
-                                                                                   'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.load': ( 'Core/patches.html#datasets.load',
-                                                                                    'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.resplit': ( 'Core/patches.html#datasets.resplit',
-                                                                                       'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.sub_dsets': ( 'Core/patches.html#datasets.sub_dsets',
-                                                                                         'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Datasets.subsets': ( 'Core/patches.html#datasets.subsets',
-                                                                                       'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.ListToTuple': ( 'Core/patches.html#listtotuple',
-                                                                                  'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.ListToTuple.encodes': ( 'Core/patches.html#listtotuple.encodes',
-                                                                                          'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.TfmdLists.__add__': ( 'Core/patches.html#tfmdlists.__add__',
-                                                                                        'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.TfmdLists.sublist': ( 'Core/patches.html#tfmdlists.sublist',
-                                                                                        'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.TfmdLists.subset': ( 'Core/patches.html#tfmdlists.subset',
-                                                                                       'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches.Union[(Pipeline, Transform)].__eq__': ( 'Core/patches.html#union[(pipeline, '
-                                                                                                          'transform)].__eq__',
-                                                                                                          'fastai_datasets/patches.py'),
-                                         'fastai_datasets.patches._dl_args': ('Core/patches.html#_dl_args', 'fastai_datasets/patches.py')},
-            'fastai_datasets.pfr': { 'fastai_datasets.pfr.PinterestFaces': ( 'Facial Recognition/pfr.html#pinterestfaces',
-                                                                             'fastai_datasets/pfr.py')},
-            'fastai_datasets.test': { 'fastai_datasets.test.MNIST': ('Facial Recognition/test.html#mnist', 'fastai_datasets/test.py'),
-                                      'fastai_datasets.test.TinyMNIST': ( 'Facial Recognition/test.html#tinymnist',
-                                                                          'fastai_datasets/test.py')},
-            'fastai_datasets.utils': { 'fastai_datasets.utils.align_facial_images': ( 'Core/utils.html#align_facial_images',
-                                                                                      'fastai_datasets/utils.py'),
-                                       'fastai_datasets.utils.data_path': ('Core/utils.html#data_path', 'fastai_datasets/utils.py'),
-                                       'fastai_datasets.utils.fetch_file': ('Core/utils.html#fetch_file', 'fastai_datasets/utils.py'),
-                                       'fastai_datasets.utils.return_list': ('Core/utils.html#return_list', 'fastai_datasets/utils.py')}}}
+# Autogenerated by nbdev
+
+d = { 'settings': { 'branch': 'main',
+                'doc_baseurl': '/fastai-datasets',
+                'doc_host': 'https://Irad-Zehavi.github.io',
+                'git_url': 'https://github.com/Irad-Zehavi/fastai-datasets',
+                'lib_path': 'fastai_datasets'},
+  'syms': { 'fastai_datasets.all': {},
+            'fastai_datasets.cifar10': {'fastai_datasets.cifar10.CIFAR10': ('cifar10.html#cifar10', 'fastai_datasets/cifar10.py')},
+            'fastai_datasets.imagenette': { 'fastai_datasets.imagenette.Imagenette': ( 'imagenette.html#imagenette',
+                                                                                       'fastai_datasets/imagenette.py')},
+            'fastai_datasets.lfw': { 'fastai_datasets.lfw.LFW': ('Facial Recognition/lfw.html#lfw', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW.__init__': ( 'Facial Recognition/lfw.html#lfw.__init__',
+                                                                           'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW._fetch_file': ( 'Facial Recognition/lfw.html#lfw._fetch_file',
+                                                                              'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW._get_path': ( 'Facial Recognition/lfw.html#lfw._get_path',
+                                                                            'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW._load': ('Facial Recognition/lfw.html#lfw._load', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW._parse_items': ( 'Facial Recognition/lfw.html#lfw._parse_items',
+                                                                               'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW._url': ('Facial Recognition/lfw.html#lfw._url', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFW.test': ('Facial Recognition/lfw.html#lfw.test', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWDevMixin': ( 'Facial Recognition/lfw.html#lfwdevmixin',
+                                                                          'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWDevMixin.dev': ( 'Facial Recognition/lfw.html#lfwdevmixin.dev',
+                                                                              'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWPairs': ('Facial Recognition/lfw.html#lfwpairs', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWPairsMixin': ( 'Facial Recognition/lfw.html#lfwpairsmixin',
+                                                                            'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWPairsMixin._load': ( 'Facial Recognition/lfw.html#lfwpairsmixin._load',
+                                                                                  'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWPairsMixin._parse_items': ( 'Facial '
+                                                                                         'Recognition/lfw.html#lfwpairsmixin._parse_items',
+                                                                                         'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWPeople': ('Facial Recognition/lfw.html#lfwpeople', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWPeople._load': ( 'Facial Recognition/lfw.html#lfwpeople._load',
+                                                                              'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.LFWPeople._parse_items': ( 'Facial Recognition/lfw.html#lfwpeople._parse_items',
+                                                                                     'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.SLLFWPairs': ('Facial Recognition/lfw.html#sllfwpairs', 'fastai_datasets/lfw.py'),
+                                     'fastai_datasets.lfw.SLLFWPairs._parse_items': ( 'Facial Recognition/lfw.html#sllfwpairs._parse_items',
+                                                                                      'fastai_datasets/lfw.py')},
+            'fastai_datasets.mnist': { 'fastai_datasets.mnist.MNIST': ('mnist.html#mnist', 'fastai_datasets/mnist.py'),
+                                       'fastai_datasets.mnist.TinyMNIST': ('mnist.html#tinymnist', 'fastai_datasets/mnist.py')},
+            'fastai_datasets.pairs': { 'fastai_datasets.pairs.ImagePair': ('pairs.html#imagepair', 'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.ImagePair.create': ( 'pairs.html#imagepair.create',
+                                                                                   'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.ImagePair.show': ('pairs.html#imagepair.show', 'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.Pairs': ('pairs.html#pairs', 'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.Sameness': ('pairs.html#sameness', 'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.Sameness.__init__': ( 'pairs.html#sameness.__init__',
+                                                                                    'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.Sameness.encodes': ( 'pairs.html#sameness.encodes',
+                                                                                   'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs._pairs_for_split': ( 'pairs.html#_pairs_for_split',
+                                                                                   'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.show_batch': ('pairs.html#show_batch', 'fastai_datasets/pairs.py')},
+            'fastai_datasets.patches': { 'fastai_datasets.patches.Datasets.__add__': ( 'Core/patches.html#datasets.__add__',
+                                                                                       'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.__repr__': ( 'Core/patches.html#datasets.__repr__',
+                                                                                        'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.__sub__': ( 'Core/patches.html#datasets.__sub__',
+                                                                                       'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.by_target': ( 'Core/patches.html#datasets.by_target',
+                                                                                         'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.dl': ( 'Core/patches.html#datasets.dl',
+                                                                                  'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.dls': ( 'Core/patches.html#datasets.dls',
+                                                                                   'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.i2t': ( 'Core/patches.html#datasets.i2t',
+                                                                                   'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.load': ( 'Core/patches.html#datasets.load',
+                                                                                    'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.plot_class_distribution': ( 'Core/patches.html#datasets.plot_class_distribution',
+                                                                                                       'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.random_sub_dsets': ( 'Core/patches.html#datasets.random_sub_dsets',
+                                                                                                'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.resplit': ( 'Core/patches.html#datasets.resplit',
+                                                                                       'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.sub_dsets': ( 'Core/patches.html#datasets.sub_dsets',
+                                                                                         'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.subsets': ( 'Core/patches.html#datasets.subsets',
+                                                                                       'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.ListToTuple': ( 'Core/patches.html#listtotuple',
+                                                                                  'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.ListToTuple.encodes': ( 'Core/patches.html#listtotuple.encodes',
+                                                                                          'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.TfmdLists.__add__': ( 'Core/patches.html#tfmdlists.__add__',
+                                                                                        'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.TfmdLists.sublist': ( 'Core/patches.html#tfmdlists.sublist',
+                                                                                        'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.TfmdLists.subset': ( 'Core/patches.html#tfmdlists.subset',
+                                                                                       'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Union[(Pipeline, Transform)].__eq__': ( 'Core/patches.html#union[(pipeline, '
+                                                                                                          'transform)].__eq__',
+                                                                                                          'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches._dl_args': ('Core/patches.html#_dl_args', 'fastai_datasets/patches.py')},
+            'fastai_datasets.pfr': { 'fastai_datasets.pfr.PinterestFaces': ( 'Facial Recognition/pfr.html#pinterestfaces',
+                                                                             'fastai_datasets/pfr.py')},
+            'fastai_datasets.utils': { 'fastai_datasets.utils.data_path': ('Core/utils.html#data_path', 'fastai_datasets/utils.py'),
+                                       'fastai_datasets.utils.fetch_file': ('Core/utils.html#fetch_file', 'fastai_datasets/utils.py'),
+                                       'fastai_datasets.utils.fix_notebook_widgets': ( 'Core/utils.html#fix_notebook_widgets',
+                                                                                       'fastai_datasets/utils.py'),
+                                       'fastai_datasets.utils.mtcnn_aligned': ('Core/utils.html#mtcnn_aligned', 'fastai_datasets/utils.py'),
+                                       'fastai_datasets.utils.return_list': ('Core/utils.html#return_list', 'fastai_datasets/utils.py')}}}
```

### Comparing `fastai-datasets-0.0.1/fastai_datasets/lfw.py` & `fastai-datasets-0.0.2/fastai_datasets/lfw.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,144 +1,147 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/Facial Recognition/lfw.ipynb.
-
-# %% auto 0
-__all__ = ['LFWPeople', 'LFWPairs', 'SLLFWPairs']
-
-# %% ../nbs/Facial Recognition/lfw.ipynb 2
-from abc import ABC, abstractmethod
-
-from fastai.vision.all import *
-from sklearn.model_selection import KFold
-
-import fastai_datasets.patches
-from .utils import return_list, fetch_file
-
-# %% ../nbs/Facial Recognition/lfw.ipynb 3
-class LFW(ABC):
-    BASE_URL = 'http://vis-www.cs.umass.edu/lfw'
-    TEST_ITEMS_FILE_NAME: str
-
-    def __init__(self):
-        self.root = untar_data(self._url('lfw.tgz'))
-
-    @classmethod
-    def _url(cls, fname):
-        return f'{cls.BASE_URL}/{fname}'
-
-    def test(self):
-        items = self._parse_items(self.TEST_ITEMS_FILE_NAME)
-        splits = KFold(n_splits=10, shuffle=False).split(range_of(items))
-        return [self._load(items=items, splits=s) for s in splits]
-
-    def _fetch_file(self, fname):
-        return fetch_file(self._url(fname))
-
-    @abstractmethod
-    def _parse_items(self, fname):
-        pass
-
-    @abstractmethod
-    def _load(self, **kwargs):
-        pass
-
-    def _get_path(self, name, num) -> Path:
-        return self.root / name / f'{name}_{num:04d}.jpg'
-
-
-class LFWDevMixin(LFW):
-    DEV_TRAIN_ITEMS_FILE_NAME: str
-    DEV_TEST_ITEMS_FILE_NAME: str
-
-    def dev(self):
-        train_items = self._parse_items(self.DEV_TRAIN_ITEMS_FILE_NAME)
-        valid_items = self._parse_items(self.DEV_TEST_ITEMS_FILE_NAME)
-        items = valid_items+train_items
-
-        return self._load(
-            items=items,
-            splits=IndexSplitter(range_of(valid_items))(items)
-        )
-
-# %% ../nbs/Facial Recognition/lfw.ipynb 4
-class LFWPeople(LFWDevMixin, LFW):
-    """
-    Individual facial images.
-    Splits contain disjoint identities, since they're meant to for constructing pairs (using `Pairs`)
-    """
-    TEST_ITEMS_FILE_NAME = 'people.txt'
-    DEV_TRAIN_ITEMS_FILE_NAME = 'peopleDevTrain.txt'
-    DEV_TEST_ITEMS_FILE_NAME = 'peopleDevTest.txt'
-    
-    @return_list
-    def _parse_items(self, fname):
-        lines = [l.split() for l in self._fetch_file(fname).readlines()]
-        for l in lines[1:]:
-            if len(l) == 1:
-                continue
-            name, num_images = l
-            for i in range(1, int(num_images)+1):
-                yield self._get_path(name, i)
-
-    def _load(self, **kwargs):
-        return Datasets(
-            tfms=[
-                PILImage.create,
-                [parent_label, lambda s: s.replace('_', ' '), Categorize()]
-            ],
-            train_setup=False,
-            **kwargs
-        )
-
-
-# %% ../nbs/Facial Recognition/lfw.ipynb 6
-from .pairs import *
-
-# %% ../nbs/Facial Recognition/lfw.ipynb 7
-class LFWPairsMixin(LFW):
-    """Fixed pairs of facial images"""
-    TEST_ITEMS_FILE_NAME = 'pairs.txt'
-    DEV_TRAIN_ITEMS_FILE_NAME = 'pairsDevTrain.txt'
-    DEV_TEST_ITEMS_FILE_NAME = 'pairsDevTest.txt'
-
-    @return_list
-    def _parse_items(self, fname):
-        lines = self._fetch_file(fname).readlines()
-        for l in lines[1:]:
-            l = l.split()
-            if len(l) == 3:
-                name, num1, num2 = l
-                yield [self._get_path(name, int(num1)),
-                       self._get_path(name, int(num2))]
-            else:
-                name1, num1, name2, num2 = l
-                yield [self._get_path(name1, int(num1)),
-                       self._get_path(name2, int(num2))]
-    
-    def _load(self, **kwargs):
-        return Datasets(
-            tfms=[
-                ImagePair.create,
-                [lambda pair: parent_label(pair[0])==parent_label(pair[1]), Sameness()]
-            ],
-            train_setup=False,
-            **kwargs
-        )
-
-# %% ../nbs/Facial Recognition/lfw.ipynb 8
-class LFWPairs(LFWDevMixin, LFWPairsMixin, LFW):
-    pass
-
-# %% ../nbs/Facial Recognition/lfw.ipynb 10
-class SLLFWPairs(LFWPairsMixin, LFW):
-    """Similar Looking LFW: http://whdeng.cn/SLLFW/index.html"""
-    BASE_URL = f'http://whdeng.cn/SLLFW'
-    TEST_ITEMS_FILE_NAME = 'pair_SLLFW.txt'
-
-    @return_list
-    def _parse_items(self, fname):
-        # Parsed according to http://www.whdeng.cn/SLLFW/index.html#download
-        singles = re.findall(r'(.*)/.*_(\d*)', self._fetch_file(fname).read_text())
-        pairs = [(singles[i], singles[i+1]) for i in range(0, len(singles), 2)]
-        
-        for ((name1, num1), (name2, num2)) in pairs:
-            yield [self._get_path(name1, int(num1)),
-                   self._get_path(name2, int(num2))]
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/Facial Recognition/lfw.ipynb.
+
+# %% auto 0
+__all__ = ['LFWPeople', 'LFWPairs', 'SLLFWPairs']
+
+# %% ../nbs/Facial Recognition/lfw.ipynb 2
+from abc import ABC, abstractmethod
+
+from fastai.vision.all import *
+from sklearn.model_selection import KFold
+
+import fastai_datasets.patches
+from .utils import *
+
+# %% ../nbs/Facial Recognition/lfw.ipynb 3
+class LFW(ABC):
+    BASE_URL = 'http://vis-www.cs.umass.edu/lfw'
+    TEST_ITEMS_FILE_NAME: str
+
+    def __init__(self, mtcnn=True):
+        self.root = untar_data(self._url('lfw.tgz'))
+        if mtcnn:
+            self.root = mtcnn_aligned(self.root)
+
+
+    @classmethod
+    def _url(cls, fname):
+        return f'{cls.BASE_URL}/{fname}'
+
+    def test(self):
+        items = self._parse_items(self.TEST_ITEMS_FILE_NAME)
+        splits = KFold(n_splits=10, shuffle=False).split(range_of(items))
+        return [self._load(items=items, splits=s) for s in splits]
+
+    def _fetch_file(self, fname):
+        return fetch_file(self._url(fname))
+
+    @abstractmethod
+    def _parse_items(self, fname):
+        pass
+
+    @abstractmethod
+    def _load(self, **kwargs):
+        pass
+
+    def _get_path(self, name, num) -> Path:
+        return self.root / name / f'{name}_{num:04d}.jpg'
+
+
+class LFWDevMixin(LFW):
+    DEV_TRAIN_ITEMS_FILE_NAME: str
+    DEV_TEST_ITEMS_FILE_NAME: str
+
+    def dev(self):
+        train_items = self._parse_items(self.DEV_TRAIN_ITEMS_FILE_NAME)
+        valid_items = self._parse_items(self.DEV_TEST_ITEMS_FILE_NAME)
+        items = valid_items+train_items
+
+        return self._load(
+            items=items,
+            splits=IndexSplitter(range_of(valid_items))(items)
+        )
+
+# %% ../nbs/Facial Recognition/lfw.ipynb 4
+class LFWPeople(LFWDevMixin, LFW):
+    """
+    Individual facial images.
+    Splits contain disjoint identities, since they're meant to for constructing pairs (using `Pairs`)
+    """
+    TEST_ITEMS_FILE_NAME = 'people.txt'
+    DEV_TRAIN_ITEMS_FILE_NAME = 'peopleDevTrain.txt'
+    DEV_TEST_ITEMS_FILE_NAME = 'peopleDevTest.txt'
+    
+    @return_list
+    def _parse_items(self, fname):
+        lines = [l.split() for l in self._fetch_file(fname).readlines()]
+        for l in lines[1:]:
+            if len(l) == 1:
+                continue
+            name, num_images = l
+            for i in range(1, int(num_images)+1):
+                yield self._get_path(name, i)
+
+    def _load(self, **kwargs):
+        return Datasets(
+            tfms=[
+                PILImage.create,
+                [parent_label, lambda s: s.replace('_', ' '), Categorize()]
+            ],
+            train_setup=False,
+            **kwargs
+        )
+
+
+# %% ../nbs/Facial Recognition/lfw.ipynb 6
+from .pairs import *
+
+# %% ../nbs/Facial Recognition/lfw.ipynb 7
+class LFWPairsMixin(LFW):
+    """Fixed pairs of facial images"""
+    TEST_ITEMS_FILE_NAME = 'pairs.txt'
+    DEV_TRAIN_ITEMS_FILE_NAME = 'pairsDevTrain.txt'
+    DEV_TEST_ITEMS_FILE_NAME = 'pairsDevTest.txt'
+
+    @return_list
+    def _parse_items(self, fname):
+        lines = self._fetch_file(fname).readlines()
+        for l in lines[1:]:
+            l = l.split()
+            if len(l) == 3:
+                name, num1, num2 = l
+                yield [self._get_path(name, int(num1)),
+                       self._get_path(name, int(num2))]
+            else:
+                name1, num1, name2, num2 = l
+                yield [self._get_path(name1, int(num1)),
+                       self._get_path(name2, int(num2))]
+    
+    def _load(self, **kwargs):
+        return Datasets(
+            tfms=[
+                ImagePair.create,
+                [lambda pair: parent_label(pair[0])==parent_label(pair[1]), Sameness()]
+            ],
+            train_setup=False,
+            **kwargs
+        )
+
+# %% ../nbs/Facial Recognition/lfw.ipynb 8
+class LFWPairs(LFWDevMixin, LFWPairsMixin, LFW):
+    pass
+
+# %% ../nbs/Facial Recognition/lfw.ipynb 10
+class SLLFWPairs(LFWPairsMixin, LFW):
+    """Similar Looking LFW: http://whdeng.cn/SLLFW/index.html"""
+    BASE_URL = f'http://whdeng.cn/SLLFW'
+    TEST_ITEMS_FILE_NAME = 'pair_SLLFW.txt'
+
+    @return_list
+    def _parse_items(self, fname):
+        # Parsed according to http://www.whdeng.cn/SLLFW/index.html#download
+        singles = re.findall(r'(.*)/.*_(\d*)', self._fetch_file(fname).read_text())
+        pairs = [(singles[i], singles[i+1]) for i in range(0, len(singles), 2)]
+        
+        for ((name1, num1), (name2, num2)) in pairs:
+            yield [self._get_path(name1, int(num1)),
+                   self._get_path(name2, int(num2))]
```

### Comparing `fastai-datasets-0.0.1/fastai_datasets/patches.py` & `fastai-datasets-0.0.2/fastai_datasets/patches.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,147 +1,173 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/Core/patches.ipynb.
-
-# %% auto 0
-__all__ = ['dl_defaults', 'ListToTuple']
-
-# %% ../nbs/Core/patches.ipynb 2
-import random
-from collections import defaultdict
-from typing import List, Dict, Sequence, Union
-from functools import partial
-
-from tqdm.auto import tqdm
-from fastai.vision.all import *
-
-# %% ../nbs/Core/patches.ipynb 5
-@patch
-def sublist(self: TfmdLists, indices: Iterable[int]) -> TfmdLists:
-    """a sublist that maintains laziness"""
-    sub = self.new_empty()
-    sub.items = [self.items[i] for i in indices]
-
-    all_indices = L(range_of(self))
-    def subsplit(s):
-        split_idxs = all_indices[s]
-        return [i for i, j in enumerate(indices) if j in split_idxs]
-    sub.splits = [subsplit(s) for s in self.splits]
-    
-    return sub
-
-# %% ../nbs/Core/patches.ipynb 9
-@patch
-def sub_dsets(self: Datasets, indices: Iterable[int]):
-    return Datasets(tls=[t.sublist(indices) for t in self.tls])
-
-# %% ../nbs/Core/patches.ipynb 18
-@patch
-def subset(self: TfmdLists, i):
-    s = self._new(self._get(self.splits[i]), split_idx=i)
-    s.splits = [slice(None), []]  # fastai bugfix
-    return s
-
-@patch
-def __eq__(self: Union[Pipeline, Transform], other: Union[Pipeline, Transform]):
-    """Needed to find shared transforms between TfmdLists"""
-    return type(self) == type(other) and self.__dict__ == other.__dict__
-
-@patch
-def __add__(l1: TfmdLists, l2: TfmdLists):
-    assert l1.split_idx == l2.split_idx
-
-    tfms1, tfms2 = copy(list(l1.tfms)), copy(list(l2.tfms))
-    merged_tfms = []
-    while tfms1 and tfms2 and tfms1[-1] == tfms2[-1]:
-        merged_tfms.insert(0, tfms1.pop())
-        tfms2.pop()
-    tfms1, tfms2 = Pipeline(tfms1), Pipeline(tfms2)
-
-    return TfmdLists(
-        [[i, item] for i, l in enumerate([l1, l2]) for item in l.items],
-        tfms=[lambda o: [tfms1, tfms2][o[0]](o[1]), *merged_tfms],
-        splits=[L(range_of(l1))[s1] + [i+len(l1) for i in L(range_of(l2))[s2]]
-                for s1, s2 in zip_longest(l1.splits, l2.splits, fillvalue=[])],
-        do_setup=False
-    )
-
-# %% ../nbs/Core/patches.ipynb 25
-@patch
-def __add__(self: Datasets, other: Datasets):
-    assert len(self.tls) == len(other.tls)
-    return Datasets(tls=[t1 + t2 for t1, t2 in zip(self.tls, other.tls)])
-
-# %% ../nbs/Core/patches.ipynb 30
-@patch
-def __sub__(self: Datasets, other: Datasets):
-    assert self.tfms == other.tfms
-    assert set(other.items).issubset(self.items)
-    return self.sub_dsets([i for i, o in enumerate(self.items) if o not in set(other.items)])
-
-# %% ../nbs/Core/patches.ipynb 33
-@patch(as_prop=True)
-def i2t(self: Datasets):
-    assert self.n_inp == len(self.tls) - 1
-    return self.tls[-1]
-
-# %% ../nbs/Core/patches.ipynb 35
-@patch(as_prop=True)
-def by_target(self: Datasets) -> Dict[int, Datasets]:
-    if not hasattr(self, '_by_target'):
-        targets = [self.vocab[t] for t in tqdm(self.i2t, desc='Class map: scanning targets')]
-        class_map = groupby(enumerate(targets), key=1, val=0)
-        self._by_target = {c: self.sub_dsets(indices) for c, indices in tqdm(class_map.items(), desc='Class map: partitioning')}
-    return self._by_target
-
-# %% ../nbs/Core/patches.ipynb 39
-class ListToTuple(Transform):
-    """Transforms lists to tuples, useful for fixing a bug in pytorch (pin_memory turns inner tuples into lists)"""
-    def encodes(self, o:list):
-        return tuple(o)
-
-
-# %% ../nbs/Core/patches.ipynb 40
-dl_defaults = {'pin_memory': default_device() != torch.device('cpu'), 'device': default_device(),
-               'after_item': [ToTensor], 'after_batch': [ListToTuple, IntToFloatTensor]}
-
-# %% ../nbs/Core/patches.ipynb 42
-def _dl_args(kwargs):
-    args = deepcopy(dl_defaults)
-    for event in ['after_item', 'after_batch']:
-        if event in kwargs:
-            tfms = kwargs[event]
-            args[event] += tfms if isinstance(tfms, Sequence) else [tfms]
-    return args
-
-
-@patch
-def dls(self: Datasets, **kwargs) -> DataLoaders:
-    """Calls `Datasets.dataloaders` with defaults from `dl_defaults`"""
-    return self.dataloaders(**_dl_args(kwargs))
-
-
-@patch
-def dl(self: Datasets, **kwargs) -> DataLoader:
-    """Creates a `DataLoader` (ignoring splits) with defaults from `dl_defaults`"""
-    return self._dl_type(self, **_dl_args(kwargs))
-
-# %% ../nbs/Core/patches.ipynb 44
-@patch
-def load(self: Datasets, **kwargs):
-    return first(self.dl(bs=len(self), **kwargs))
-
-# %% ../nbs/Core/patches.ipynb 47
-@patch(as_prop=True)
-def subsets(self: Datasets
-            ) -> TfmdLists:  # something
-    """Lazy list of a `Datasets`'s subsets"""
-    return TfmdLists(range(self.n_subsets), self.subset)
-
-# %% ../nbs/Core/patches.ipynb 49
-@patch
-def resplit(self: Datasets,
-            splits: Union[Callable, List[List[int]]]  # a splitter function or a list of splits
-            ):
-    """Sets the splits of a `Datasets`"""
-    if isinstance(splits, Callable):
-        splits = splits(self)
-    for t in self.tls:
-        t.splits = splits
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/Core/patches.ipynb.
+
+# %% auto 0
+__all__ = ['dl_defaults', 'ListToTuple']
+
+# %% ../nbs/Core/patches.ipynb 2
+import random
+from collections import defaultdict
+from typing import List, Dict, Sequence, Union
+from functools import partial
+
+from tqdm.auto import tqdm
+from fastai.vision.all import *
+
+# %% ../nbs/Core/patches.ipynb 5
+@patch
+def sublist(self: TfmdLists, indices: Iterable[int]) -> TfmdLists:
+    """a sublist that maintains laziness"""
+    sub = self.new_empty()
+    sub.items = [self.items[i] for i in indices]
+
+    all_indices = L(range_of(self))
+    def subsplit(s):
+        split_idxs = set(all_indices[s])
+        return [i for i, j in enumerate(indices) if j in split_idxs]
+    sub.splits = [subsplit(s) for s in self.splits]
+    
+    return sub
+
+# %% ../nbs/Core/patches.ipynb 9
+@patch
+def sub_dsets(self: Datasets, indices: Iterable[int]):
+    return Datasets(tls=[t.sublist(indices) for t in self.tls])
+
+# %% ../nbs/Core/patches.ipynb 13
+@patch
+def random_sub_dsets(self: Datasets, size, with_replacement=False, less_ok=False) -> Datasets:
+    if size == 0:
+        return self.subset([])
+    if len(self) < size:
+        assert less_ok
+        size = len(self)
+    sampler = random.choices if with_replacement else random.sample
+    indices = sampler(range(len(self)),  k=size)
+    return self.sub_dsets(indices)
+
+# %% ../nbs/Core/patches.ipynb 18
+@patch
+def subset(self: TfmdLists, i):
+    s = self._new(self._get(self.splits[i]), split_idx=i)
+    s.splits = [slice(None), []]  # fastai bugfix
+    return s
+
+@patch
+def __eq__(self: Union[Pipeline, Transform], other: Union[Pipeline, Transform]):
+    """Needed to find shared transforms between TfmdLists"""
+    return type(self) == type(other) and self.__dict__ == other.__dict__
+
+@patch
+def __add__(l1: TfmdLists, l2: TfmdLists):
+    assert l1.split_idx == l2.split_idx
+
+    tfms1, tfms2 = copy(list(l1.tfms)), copy(list(l2.tfms))
+    merged_tfms = []
+    while tfms1 and tfms2 and tfms1[-1] == tfms2[-1]:
+        merged_tfms.insert(0, tfms1.pop())
+        tfms2.pop()
+    tfms1, tfms2 = Pipeline(tfms1), Pipeline(tfms2)
+
+    return TfmdLists(
+        [[i, item] for i, l in enumerate([l1, l2]) for item in l.items],
+        tfms=[lambda o: [tfms1, tfms2][o[0]](o[1]), *merged_tfms],
+        splits=[L(range_of(l1))[s1] + [i+len(l1) for i in L(range_of(l2))[s2]]
+                for s1, s2 in zip_longest(l1.splits, l2.splits, fillvalue=[])],
+        do_setup=False
+    )
+
+# %% ../nbs/Core/patches.ipynb 25
+@patch
+def __add__(self: Datasets, other: Datasets):
+    assert len(self.tls) == len(other.tls)
+    return Datasets(tls=[t1 + t2 for t1, t2 in zip(self.tls, other.tls)])
+
+# %% ../nbs/Core/patches.ipynb 30
+@patch
+def __sub__(self: Datasets, other: Datasets):
+    assert self.tfms == other.tfms
+    assert set(other.items).issubset(self.items)
+    return self.sub_dsets([i for i, o in enumerate(self.items) if o not in set(other.items)])
+
+# %% ../nbs/Core/patches.ipynb 33
+@patch(as_prop=True)
+def i2t(self: Datasets):
+    assert self.n_inp == len(self.tls) - 1
+    return self.tls[-1]
+
+# %% ../nbs/Core/patches.ipynb 35
+@patch(as_prop=True)
+def by_target(self: Datasets) -> Dict[int, Datasets]:
+    if not hasattr(self, '_by_target'):
+        targets = [int(t) for t in tqdm(self.i2t, desc='Class map: scanning targets')]
+        class_map = groupby(enumerate(targets), key=1, val=0)
+        self._by_target = {self.vocab[c]: self.sub_dsets(indices)
+                           for c, indices in tqdm(class_map.items(), desc='Class map: partitioning')}
+    return self._by_target
+
+
+# %% ../nbs/Core/patches.ipynb 37
+import matplotlib.pyplot as plt
+
+@patch()
+def plot_class_distribution(self: Datasets):
+    for split in self.subsets:
+        plt.bar(self.vocab, [len(split.by_target[c]) for c in self.vocab])
+
+# %% ../nbs/Core/patches.ipynb 41
+class ListToTuple(Transform):
+    """Transforms lists to tuples, useful for fixing a bug in pytorch (pin_memory turns inner tuples into lists)"""
+    def encodes(self, o:list):
+        return tuple(o)
+
+
+# %% ../nbs/Core/patches.ipynb 42
+dl_defaults = {'pin_memory': default_device() != torch.device('cpu'), 'device': default_device(),
+               'after_item': [ToTensor], 'after_batch': [ListToTuple, IntToFloatTensor]}
+
+# %% ../nbs/Core/patches.ipynb 44
+def _dl_args(kwargs):
+    args = deepcopy(dl_defaults)
+    for event in ['after_item', 'after_batch']:
+        if event in kwargs:
+            tfms = kwargs[event]
+            args[event] += tfms if isinstance(tfms, Sequence) else [tfms]
+    return args
+
+
+@patch
+def dls(self: Datasets, **kwargs) -> DataLoaders:
+    """Calls `Datasets.dataloaders` with defaults from `dl_defaults`"""
+    return self.dataloaders(**_dl_args(kwargs))
+
+
+@patch
+def dl(self: Datasets, **kwargs) -> DataLoader:
+    """Creates a `DataLoader` (ignoring splits) with defaults from `dl_defaults`"""
+    return self._dl_type(self, **_dl_args(kwargs))
+
+# %% ../nbs/Core/patches.ipynb 46
+@patch
+def load(self: Datasets, **kwargs):
+    return first(self.dl(bs=len(self), **kwargs))
+
+# %% ../nbs/Core/patches.ipynb 49
+@patch(as_prop=True)
+def subsets(self: Datasets) -> TfmdLists:
+    """Lazy list of a `Datasets`'s subsets"""
+    return TfmdLists(range(self.n_subsets), self.subset)
+
+# %% ../nbs/Core/patches.ipynb 51
+@patch
+def resplit(self: Datasets,
+            splits: Union[Callable, List[List[int]]]  # a splitter function or a list of splits
+            ):
+    """Sets the splits of a `Datasets`"""
+    if isinstance(splits, Callable):
+        splits = splits(self)
+    for t in self.tls:
+        t.splits = splits
+
+# %% ../nbs/Core/patches.ipynb 54
+@patch()
+def __repr__(self: Datasets):
+    return '['+'\n'.join(repr(s) for s in self.subsets)+']' if self.split_idx is None else coll_repr(self)
```

### Comparing `fastai-datasets-0.0.1/fastai_datasets.egg-info/SOURCES.txt` & `fastai-datasets-0.0.2/fastai_datasets.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 fastai_datasets/__init__.py
 fastai_datasets/_modidx.py
+fastai_datasets/all.py
 fastai_datasets/cifar10.py
+fastai_datasets/imagenette.py
 fastai_datasets/lfw.py
 fastai_datasets/mnist.py
 fastai_datasets/pairs.py
 fastai_datasets/patches.py
 fastai_datasets/pfr.py
-fastai_datasets/test.py
 fastai_datasets/utils.py
 fastai_datasets.egg-info/PKG-INFO
 fastai_datasets.egg-info/SOURCES.txt
 fastai_datasets.egg-info/dependency_links.txt
 fastai_datasets.egg-info/entry_points.txt
 fastai_datasets.egg-info/not-zip-safe
 fastai_datasets.egg-info/requires.txt
```

### Comparing `fastai-datasets-0.0.1/setup.py` & `fastai-datasets-0.0.2/setup.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from pkg_resources import parse_version
-from configparser import ConfigParser
-import setuptools, shlex
-assert parse_version(setuptools.__version__)>=parse_version('36.2')
-
-# note: all settings are in settings.ini; edit there, not here
-config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
-cfg = config['DEFAULT']
-
-cfg_keys = 'version description keywords author author_email'.split()
-expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
-for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
-setup_cfg = {o:cfg[o] for o in cfg_keys}
-
-licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
-}
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
-
-requirements = shlex.split(cfg.get('requirements', ''))
-if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
-min_python = cfg['min_python']
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-dev_requirements = (cfg.get('dev_requirements') or '').split()
-
-setuptools.setup(
-    name = cfg['lib_name'],
-    license = lic[0],
-    classifiers = [
-        'Development Status :: ' + statuses[int(cfg['status'])],
-        'Intended Audience :: ' + cfg['audience'].title(),
-        'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
-    url = cfg['git_url'],
-    packages = setuptools.find_packages(),
-    include_package_data = True,
-    install_requires = requirements,
-    extras_require={ 'dev': dev_requirements },
-    dependency_links = cfg.get('dep_links','').split(),
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
-    **setup_cfg)
-
-
+from pkg_resources import parse_version
+from configparser import ConfigParser
+import setuptools, shlex
+assert parse_version(setuptools.__version__)>=parse_version('36.2')
+
+# note: all settings are in settings.ini; edit there, not here
+config = ConfigParser(delimiters=['='])
+config.read('settings.ini')
+cfg = config['DEFAULT']
+
+cfg_keys = 'version description keywords author author_email'.split()
+expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
+for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
+setup_cfg = {o:cfg[o] for o in cfg_keys}
+
+licenses = {
+    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
+}
+statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
+
+requirements = shlex.split(cfg.get('requirements', ''))
+if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
+min_python = cfg['min_python']
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+dev_requirements = (cfg.get('dev_requirements') or '').split()
+
+setuptools.setup(
+    name = cfg['lib_name'],
+    license = lic[0],
+    classifiers = [
+        'Development Status :: ' + statuses[int(cfg['status'])],
+        'Intended Audience :: ' + cfg['audience'].title(),
+        'Natural Language :: ' + cfg['language'].title(),
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
+    url = cfg['git_url'],
+    packages = setuptools.find_packages(),
+    include_package_data = True,
+    install_requires = requirements,
+    extras_require={ 'dev': dev_requirements },
+    dependency_links = cfg.get('dep_links','').split(),
+    python_requires  = '>=' + cfg['min_python'],
+    long_description = open('README.md').read(),
+    long_description_content_type = 'text/markdown',
+    zip_safe = False,
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
+    **setup_cfg)
+
+
```

