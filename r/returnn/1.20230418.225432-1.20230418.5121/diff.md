# Comparing `tmp/returnn-1.20230418.225432.tar.gz` & `tmp/returnn-1.20230418.5121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230418.225432.tar", last modified: Tue Apr 18 21:03:49 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230418.5121.tar", last modified: Mon Apr 17 23:06:30 2023, max compression
```

## Comparing `returnn-1.20230418.225432.tar` & `returnn-1.20230418.5121.tar`

### file list

```diff
@@ -1,433 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 21:03:29.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-18 21:03:33.000000 returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34980 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97345 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32072 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69825 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   588709 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   293047 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49614 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:03:49.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-18 21:03:28.000000 returnn-1.20230418.225432/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 23:06:13.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-17 23:06:15.000000 returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34121 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97355 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155421 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31132 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   588705 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45899 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:06:30.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-17 23:06:12.000000 returnn-1.20230418.5121/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230418.225432/.gitignore` & `returnn-1.20230418.5121/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/.gitmodules` & `returnn-1.20230418.5121/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/CHANGELOG.md` & `returnn-1.20230418.5121/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/CODEOWNERS` & `returnn-1.20230418.5121/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/CONTRIBUTING.md` & `returnn-1.20230418.5121/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/LICENSE` & `returnn-1.20230418.5121/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/MANIFEST.in` & `returnn-1.20230418.5121/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/PKG-INFO` & `returnn-1.20230418.5121/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230418.225432
+Version: 1.20230418.5121
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230418.225432/README.rst` & `returnn-1.20230418.5121/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/__init__.py` & `returnn-1.20230418.5121/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/12AX.cluster_map` & `returnn-1.20230418.5121/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-fwd.config` & `returnn-1.20230418.5121/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-horovod-mpi.py` & `returnn-1.20230418.5121/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230418.5121/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-hyper-param-tuning.config` & `returnn-1.20230418.5121/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-iter-dataset.py` & `returnn-1.20230418.5121/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-list-devices.py` & `returnn-1.20230418.5121/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-lua-torch-layer.config` & `returnn-1.20230418.5121/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230418.5121/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-returnn-as-framework.py` & `returnn-1.20230418.5121/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-rf.config` & `returnn-1.20230418.5121/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-rhn-enwik8.config` & `returnn-1.20230418.5121/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-sprint-interface.py` & `returnn-1.20230418.5121/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-att-copy.config` & `returnn-1.20230418.5121/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-attention.config` & `returnn-1.20230418.5121/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-enc-dec.config` & `returnn-1.20230418.5121/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230418.5121/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230418.5121/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230418.5121/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230418.5121/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230418.5121/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-rec-self-att.config` & `returnn-1.20230418.5121/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230418.5121/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230418.5121/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230418.5121/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-torch.config` & `returnn-1.20230418.5121/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230418.5121/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/demo.sh` & `returnn-1.20230418.5121/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230418.5121/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230418.5121/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230418.5121/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/README.txt` & `returnn-1.20230418.5121/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/config_demo` & `returnn-1.20230418.5121/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230418.5121/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/config_real` & `returnn-1.20230418.5121/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230418.5121/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/decode.py` & `returnn-1.20230418.5121/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230418.5121/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230418.5121/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230418.5121/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230418.5121/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230418.5121/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230418.5121/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230418.5121/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230418.5121/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/__init__.py` & `returnn-1.20230418.5121/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/__main__.py` & `returnn-1.20230418.5121/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/__old_mod_loader__.py` & `returnn-1.20230418.5121/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/__setup__.py` & `returnn-1.20230418.5121/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/config.py` & `returnn-1.20230418.5121/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/audio.py` & `returnn-1.20230418.5121/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/basic.py` & `returnn-1.20230418.5121/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/bundle_file.py` & `returnn-1.20230418.5121/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/cached.py` & `returnn-1.20230418.5121/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/cached2.py` & `returnn-1.20230418.5121/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/generating.py` & `returnn-1.20230418.5121/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/hdf.py` & `returnn-1.20230418.5121/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/lm.py` & `returnn-1.20230418.5121/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/map.py` & `returnn-1.20230418.5121/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/meta.py` & `returnn-1.20230418.5121/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/multi_proc.py` & `returnn-1.20230418.5121/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/normalization_data.py` & `returnn-1.20230418.5121/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/numpy_dump.py` & `returnn-1.20230418.5121/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/raw_wav.py` & `returnn-1.20230418.5121/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/sprint.py` & `returnn-1.20230418.5121/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/stereo.py` & `returnn-1.20230418.5121/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230418.5121/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/datasets/util/vocabulary.py` & `returnn-1.20230418.5121/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/engine/base.py` & `returnn-1.20230418.5121/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/engine/batch.py` & `returnn-1.20230418.5121/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230418.5121/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230418.5121/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/graph_editor/edit.py` & `returnn-1.20230418.5121/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230418.5121/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/graph_editor/select.py` & `returnn-1.20230418.5121/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230418.5121/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/graph_editor/transform.py` & `returnn-1.20230418.5121/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/extern/graph_editor/util.py` & `returnn-1.20230418.5121/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/_backend.py` & `returnn-1.20230418.5121/returnn/frontend/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Backends for the frontend API
 """
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Any, Union, TypeVar, Generic, Type, Sequence, Dict, Tuple
 import contextlib
 import numpy
+
+from returnn.util.basic import NotSpecified
 import returnn.frontend as rf
 
 if TYPE_CHECKING:
     from returnn.tensor import Tensor, Dim
     from .types import RawTensorTypes
 
 T = TypeVar("T")  # tf.Tensor, torch.Tensor or so
@@ -427,29 +429,27 @@
         :param raw_tensor:
         :param func: "tanh", "sigmoid", "relu", ...
         :return: raw tensor with elementwise activation applied
         """
         raise NotImplementedError
 
     @staticmethod
-    def softmax(tensor: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+    def softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """
         :param tensor:
         :param axis:
-        :param use_mask:
         :return: softmax over axis
         """
         raise NotImplementedError
 
     @staticmethod
-    def log_softmax(tensor: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+    def log_softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """
         :param tensor:
         :param axis:
-        :param use_mask:
         :return: log_softmax over axis
         """
         raise NotImplementedError
 
     @staticmethod
     def softmax_cross_entropy_with_logits(*, logits: Tensor, targets: Tensor, axis: Dim):
         """
@@ -708,15 +708,17 @@
         size: Optional[Union[int, Tensor, Dim]] = None,
         out_dim: Dim,
     ) -> Tensor:
         """slice"""
         raise NotImplementedError
 
     @staticmethod
-    def matmul(a: Tensor[T], b: Tensor[T], *, reduce: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+    def matmul(
+        a: Tensor[T], b: Tensor[T], *, reduce: Union[Dim, Sequence[Dim]], disable_masking: bool = False
+    ) -> Tensor[T]:
         """
         This performs a batched matmul of two sources a and b
         (non-batched matmul and dot product are special cases).
         The underlying operation is a batched matmul (shared..., I, J) * (shared..., J, K) -> (shared..., I, K).
         The inputs a and b are transformed internally into the required shapes in the following way:
         The axis J is specified via the Dim given as 'reduce'. If multiple reduce Dims are given the corresponding axes
         are merged into one before the matmul via a reshape. All other matching Dims in a and b will be treated as
@@ -725,17 +727,17 @@
 
         Depending on which Dims exist in a, b and reduce this dot operation can be used to compute scaling, scalar
         product, outer product, matrix-vector multiplication, matrix-matrix multiplication etc. (all possibly batched).
 
         :param a:
         :param b:
         :param reduce: Dims over which to perform the product, have to be present in both a and b
-        :param use_mask: If the reduction is over dynamic axes, to get the correct sum reduction,
+        :param disable_masking: If the reduction is over dynamic axes, to get the correct sum reduction,
             we need to apply masking to one of the inputs. This is done automatically.
-            By disabling this flag, this would be disabled.
+            By enabling this flag, this would be disabled.
         :return: result of dot product, Dim order: common axes as sorted in a, unique axes of a (in order),
             unique axes of b (in order)
         """
         raise NotImplementedError
 
     @staticmethod
     def range_over_dim(dim: Dim, *, dtype: Optional[str] = None) -> Tensor[T]:
@@ -766,23 +768,23 @@
 
     @staticmethod
     def reduce(
         source: Tensor[T],
         *,
         mode: str,
         axis: Union[Dim, Sequence[Dim]],
-        use_mask: bool = True,
+        use_time_mask: bool = NotSpecified,
     ) -> Tensor[T]:
         """
         Reduce the tensor along the given axis
 
         :param source:
         :param mode: "sum", "max", "min", "mean", "logsumexp", "any", "all", "argmin", "argmax"
         :param axis:
-        :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+        :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
         :return: tensor with axis removed
         """
         raise NotImplementedError
 
     @staticmethod
     def random(
         *,
@@ -902,43 +904,14 @@
         strides: Sequence[int],
         in_spatial_dims: Sequence[Dim],
         out_spatial_dims: Optional[Sequence[Dim]] = None,
     ) -> Tuple[Tensor, Sequence[Dim]]:
         """pooling"""
         raise NotImplementedError
 
-    @staticmethod
-    def lstm(
-        source: Tensor,
-        *,
-        state_c: Tensor,
-        state_h: Tensor,
-        ff_weight: Tensor,
-        rec_weight: Tensor,
-        bias: Tensor,
-        spatial_dim: Dim,
-        in_dim: Dim,
-        out_dim: Dim,
-    ) -> Tuple[Tensor, Tuple[Tensor, Tensor]]:
-        """
-        Functional LSTM.
-
-        :param source: Tensor of shape [*, in_dim].
-        :param state_c:
-        :param state_h:
-        :param ff_weight: Parameters for the weights of the feed-forward part.
-        :param rec_weight: Parameters for the weights of the recurrent part.
-        :param bias: Parameters for the bias.
-        :param spatial_dim: Dimension in which the LSTM operates.
-        :param in_dim:
-        :param out_dim:
-        :return: output, (state_h, state_c)
-        """
-        raise NotImplementedError
-
 
 # We use a global instance, and we modify __class__ inplace,
 # such that any reference to this can be updated.
 # This is exposed to the user as `returnn.frontend`.
 # The __class__ assignment is done in `select_engine`.
 # Use object.__new__ because we disallow creating instances of Frontend.
 global_backend = object.__new__(Backend)
```

### Comparing `returnn-1.20230418.225432/returnn/frontend/_numpy_backend.py` & `returnn-1.20230418.5121/returnn/frontend/_numpy_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This backend will probably never be feature-complete.
 It just has the bare minimum such that the user can assign Numpy arrays to Tensor.raw_tensor.
 """
 
 from __future__ import annotations
 from typing import Union, Sequence, Tuple
 import numpy
+from returnn.util.basic import NotSpecified
 from returnn.tensor import Tensor, Dim
 from ._backend import Backend
 
 
 # We do not expect that we will ever implement all the methods of the Backend interface.
 # noinspection PyAbstractClass
 class NumpyBackend(Backend[numpy.ndarray]):
@@ -71,23 +72,22 @@
 
     @staticmethod
     def reduce(
         source: Tensor[numpy.ndarray],
         *,
         mode: str,
         axis: Union[Dim, Sequence[Dim]],
-        use_mask: bool = True,
+        use_time_mask: bool = NotSpecified,
     ) -> Tensor[numpy.ndarray]:
         """reduce"""
         assert mode in Backend._AllowedReduceModes
-        if use_mask:
-            if isinstance(axis, Dim):
-                assert not axis.need_masking()  # not implemented
-            else:
-                assert all(not dim.need_masking() for dim in axis)  # not implemented
+        if isinstance(axis, Dim):
+            assert not axis.need_masking()  # not implemented
+        else:
+            assert all(not dim.need_masking() for dim in axis)  # not implemented
         func = getattr(numpy, mode)
         raw_dims = (
             [source.get_axis_from_description(axis)]
             if isinstance(axis, Dim)
             else [source.get_axis_from_description(dim) for dim in axis]
         )
         res_dims = [dim for i, dim in enumerate(source.dims) if i not in raw_dims]
```

### Comparing `returnn-1.20230418.225432/returnn/frontend/_utils.py` & `returnn-1.20230418.5121/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/array_.py` & `returnn-1.20230418.5121/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/const.py` & `returnn-1.20230418.5121/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/container.py` & `returnn-1.20230418.5121/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/conv.py` & `returnn-1.20230418.5121/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/dims.py` & `returnn-1.20230418.5121/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/dropout.py` & `returnn-1.20230418.5121/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/dtype.py` & `returnn-1.20230418.5121/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/init.py` & `returnn-1.20230418.5121/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/linear.py` & `returnn-1.20230418.5121/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/loss.py` & `returnn-1.20230418.5121/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/math_.py` & `returnn-1.20230418.5121/returnn/frontend/math_.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Math ops
 """
 
 from __future__ import annotations
 import typing
-from typing import Optional, Sequence, Union, Tuple
+from typing import Optional, Sequence, Union
 import numpy
 from returnn.tensor import Tensor, Dim
-import returnn.frontend as rf
 from .types import RawTensorTypes as _RawTensorTypes
 
 __all__ = [
     "compare",
     "combine",
     "combine_bc",
     "equal",
@@ -50,18 +49,16 @@
     "ceil",
     "floor",
     "round",
     "relu",
     "elu",
     "selu",
     "silu",
-    "swish",
     "softmax",
     "log_softmax",
-    "gating",
 ]
 
 
 @typing.overload
 def compare(
     a: Tensor,
     kind: str,
@@ -433,39 +430,17 @@
     # noinspection PyProtectedMember
     return a._raw_backend.activation(a, "silu")
 
 
 swish = silu  # alias
 
 
-def softmax(a: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+def softmax(a: Tensor, *, axis: Dim) -> Tensor:
     """softmax"""
     # noinspection PyProtectedMember
-    return a._raw_backend.softmax(a, axis=axis, use_mask=use_mask)
+    return a._raw_backend.softmax(a, axis=axis)
 
 
-def log_softmax(a: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+def log_softmax(a: Tensor, *, axis: Dim) -> Tensor:
     """log_softmax"""
     # noinspection PyProtectedMember
-    return a._raw_backend.log_softmax(a, axis=axis, use_mask=use_mask)
-
-
-def gating(
-    x: Tensor, *, axis: Optional[Dim] = None, gate_func=sigmoid, act_func=identity, out_dim: Optional[Dim] = None
-) -> Tuple[Tensor, Dim]:
-    """
-    Like in gated linear unit (GLU): https://arxiv.org/abs/1612.08083
-    GLU refers also to the linear transformation before the gating -- this is why this function is not called GLU.
-    GLU uses gate_func=sigmoid and act_func=identity (the defaults here).
-
-    There are other potential gating variants you might be interested at.
-    See for example: https://arxiv.org/abs/2002.05202, e.g. gate_func=gelu.
-    """
-    if axis is None:
-        assert x.feature_dim is not None, f"gating {x}: need tensor with feature dim set, or explicit `axis`"
-        axis = x.feature_dim
-    assert axis.is_static() and axis.dimension % 2 == 0, f"gating {x}: need static dim, and even, got {axis}"
-    if not out_dim:
-        out_dim = axis.div_left(2)
-
-    a, b = rf.split(x, axis=axis, out_dims=[out_dim, out_dim])
-    return act_func(a) * gate_func(b), out_dim
+    return a._raw_backend.log_softmax(a, axis=axis)
```

### Comparing `returnn-1.20230418.225432/returnn/frontend/matmul.py` & `returnn-1.20230418.5121/returnn/frontend/matmul.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 T = TypeVar("T")
 
 __all__ = ["matmul", "dot"]
 
 
 # noinspection PyShadowingNames
-def matmul(a: Tensor[T], b: Tensor[T], *, reduce: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def matmul(
+    a: Tensor[T], b: Tensor[T], *, reduce: Union[Dim, Sequence[Dim]], disable_masking: bool = False
+) -> Tensor[T]:
     """
     This performs a batched matmul of two sources a and b
     (non-batched matmul and dot product are special cases).
     The underlying operation is a batched matmul (shared..., I, J) * (shared..., J, K) -> (shared..., I, K).
     The inputs a and b are transformed internally into the required shapes in the following way:
     The axis J is specified via the Dim given as 'reduce'. If multiple reduce Dims are given the corresponding axes
     are merged into one before the matmul via a reshape. All other matching Dims in a and b will be treated as
@@ -26,19 +28,19 @@
 
     Depending on which Dims exist in a, b and reduce this dot operation can be used to compute scaling, scalar
     product, outer product, matrix-vector multiplication, matrix-matrix multiplication etc. (all possibly batched).
 
     :param a:
     :param b:
     :param reduce: Dims over which to perform the product, have to be present in both a and b
-    :param use_mask: If the reduction is over dynamic axes, to get the correct sum reduction,
+    :param disable_masking: If the reduction is over dynamic axes, to get the correct sum reduction,
         we need to apply masking to one of the inputs. This is done automatically.
-        By disabling this flag, this would be disabled.
+        By enabling this flag, this would be disabled.
     :return: result of dot product, Dim order: common axes as sorted in a, unique axes of a (in order),
         unique axes of b (in order)
     """
     # noinspection PyProtectedMember
-    return a._raw_backend.matmul(a=a, b=b, reduce=reduce, use_mask=use_mask)
+    return a._raw_backend.matmul(a=a, b=b, reduce=reduce, disable_masking=disable_masking)
 
 
 # alias for some older code
 dot = matmul
```

### Comparing `returnn-1.20230418.225432/returnn/frontend/module.py` & `returnn-1.20230418.5121/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/normalization.py` & `returnn-1.20230418.5121/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/parameter.py` & `returnn-1.20230418.5121/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/rand.py` & `returnn-1.20230418.5121/returnn/frontend/rand.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,16 +57,14 @@
     "set_random_seed",
     "get_random_state",
     "set_random_state",
     "reset_step_random_state",
     "get_static_step_based_seed",
     "random",
     "random_uniform",
-    "random_normal",
-    "random_truncated_normal",
 ]
 
 
 def set_random_seed(seed: int):
     """
     Call this at the beginning of the program
     (after the RF backend was selected),
@@ -219,16 +217,16 @@
 
 
 def random_uniform(
     *,
     dims: Sequence[Dim],
     dtype: Optional[str] = None,
     sparse_dim: Optional[Dim] = None,
-    minval: Union[int, float, Tensor] = 0.0,
-    maxval: Union[int, float, Tensor] = 1.0,
+    minval: Union[int, float, Tensor],
+    maxval: Union[int, float, Tensor],
     seed: Optional[Union[int, Sequence[int], numpy.ndarray]] = None,
     algorithm: Optional[str] = None,
     explicit_state: Optional[Tensor] = None,
     auto_update_state: Optional[bool] = None,
     static: Optional[bool] = None,
     out: Optional[Tensor] = None,
 ):
@@ -243,79 +241,9 @@
         minval=minval,
         maxval=maxval,
         seed=seed,
         algorithm=algorithm,
         explicit_state=explicit_state,
         auto_update_state=auto_update_state,
         static=static,
-        out=out,
-    )
-
-
-def random_normal(
-    *,
-    dims: Sequence[Dim],
-    dtype: Optional[str] = None,
-    sparse_dim: Optional[Dim] = None,
-    mean: Optional[Union[int, float, Tensor]] = 0.0,
-    stddev: Optional[Union[int, float, Tensor]] = 1.0,
-    seed: Optional[Union[int, Sequence[int], numpy.ndarray]] = None,
-    algorithm: Optional[str] = None,
-    explicit_state: Optional[Tensor] = None,
-    auto_update_state: Optional[bool] = None,
-    static: Optional[bool] = None,
-    out: Optional[Tensor] = None,
-):
-    """
-    See :func:`random`. :func:`random` with ``distribution="normal"``.
-    """
-    return random(
-        dims=dims,
-        dtype=dtype,
-        sparse_dim=sparse_dim,
-        distribution="normal",
-        mean=mean,
-        stddev=stddev,
-        seed=seed,
-        algorithm=algorithm,
-        explicit_state=explicit_state,
-        auto_update_state=auto_update_state,
-        static=static,
-        out=out,
-    )
-
-
-def random_truncated_normal(
-    *,
-    dims: Sequence[Dim],
-    dtype: Optional[str] = None,
-    sparse_dim: Optional[Dim] = None,
-    mean: Optional[Union[int, float, Tensor]] = 0.0,
-    stddev: Optional[Union[int, float, Tensor]] = 1.0,
-    minval: Union[int, float, Tensor] = None,
-    maxval: Union[int, float, Tensor] = None,
-    seed: Optional[Union[int, Sequence[int], numpy.ndarray]] = None,
-    algorithm: Optional[str] = None,
-    explicit_state: Optional[Tensor] = None,
-    auto_update_state: Optional[bool] = None,
-    static: Optional[bool] = None,
-    out: Optional[Tensor] = None,
-):
-    """
-    See :func:`random`. :func:`random` with ``distribution="truncated_normal"``.
-    """
-    return random(
-        dims=dims,
-        dtype=dtype,
-        sparse_dim=sparse_dim,
-        distribution="truncated_normal",
-        mean=mean,
-        stddev=stddev,
-        minval=minval,
-        maxval=maxval,
-        seed=seed,
-        algorithm=algorithm,
-        explicit_state=explicit_state,
-        auto_update_state=auto_update_state,
-        static=static,
         out=out,
     )
```

### Comparing `returnn-1.20230418.225432/returnn/frontend/reduce.py` & `returnn-1.20230418.5121/returnn/frontend/reduce.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Reduce
 """
 
 from __future__ import annotations
 from typing import Union, TypeVar, Sequence
+from returnn.util.basic import NotSpecified
 from returnn.tensor import Tensor, Dim
 
 T = TypeVar("T")
 
 __all__ = [
     "reduce",
     "reduce_sum",
@@ -23,128 +24,134 @@
 
 
 def reduce(
     source: Tensor[T],
     *,
     mode: str,
     axis: Union[Dim, Sequence[Dim]],
-    use_mask: bool = True,
+    use_time_mask: bool = NotSpecified,
 ) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param mode: "sum", "max", "min", "mean", "logsumexp", "any", "all", "argmin", "argmax"
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
     # noinspection PyProtectedMember
-    return source._raw_backend.reduce(source=source, mode=mode, axis=axis, use_mask=use_mask)
+    return source._raw_backend.reduce(source=source, mode=mode, axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_sum(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_sum(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="sum", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="sum", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_max(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_max(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="max", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="max", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_min(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_min(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="min", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="min", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_mean(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_mean(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="mean", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="mean", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_logsumexp(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_logsumexp(
+    source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified
+) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="logsumexp", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="logsumexp", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_any(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_any(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="any", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="any", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_all(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_all(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="all", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="all", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_argmin(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_argmin(
+    source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified
+) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="argmin", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="argmin", axis=axis, use_time_mask=use_time_mask)
 
 
-def reduce_argmax(source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor[T]:
+def reduce_argmax(
+    source: Tensor[T], *, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified
+) -> Tensor[T]:
     """
     Reduce the tensor along the given axis
 
     :param source:
     :param axis:
-    :param use_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
+    :param use_time_mask: if True (default), use the time mask (part of dim tag) to ignore padding frames
     :return: tensor with axis removed
     """
-    return reduce(source=source, mode="argmax", axis=axis, use_mask=use_mask)
+    return reduce(source=source, mode="argmax", axis=axis, use_time_mask=use_time_mask)
```

### Comparing `returnn-1.20230418.225432/returnn/frontend/run_ctx.py` & `returnn-1.20230418.5121/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/state.py` & `returnn-1.20230418.5121/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/frontend/types.py` & `returnn-1.20230418.5121/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/import_/common.py` & `returnn-1.20230418.5121/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/import_/git.py` & `returnn-1.20230418.5121/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/import_/import_.py` & `returnn-1.20230418.5121/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/learning_rate_control.py` & `returnn-1.20230418.5121/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/log.py` & `returnn-1.20230418.5121/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/native_op.cpp` & `returnn-1.20230418.5121/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/native_op.py` & `returnn-1.20230418.5121/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/pretrain.py` & `returnn-1.20230418.5121/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/sprint/cache.py` & `returnn-1.20230418.5121/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/sprint/control.py` & `returnn-1.20230418.5121/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/sprint/error_signals.py` & `returnn-1.20230418.5121/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/sprint/extern_interface.py` & `returnn-1.20230418.5121/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/sprint/interface.py` & `returnn-1.20230418.5121/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tensor/_dim_extra.py` & `returnn-1.20230418.5121/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,15 +706,15 @@
 
         max_idx = rf.reduce(
             self.dyn_size_ext,
             axis=self.dyn_size_ext.dims,
             mode="max",
             # Masking here is not always possible, e.g. if we have
             # tag = Dim{'self-att-keys'['time:var:extern_data:classes'[B]]}
-            use_mask=False,
+            use_time_mask=False,
         )
         # We use the assumption that self.placeholder.shape[axis] == max_idx.
         # size_ext might have invalid (zero) sizes
         # when it itself has some padding, e.g. when its own shape is dynamic.
         # A zero size can lead to problems in some cases, e.g. in SoftmaxOverSpatialLayer,
         # when everything is masked to -inf, it results in nan,
         # and this likely produces nan in backprop or elsewhere.
@@ -1642,15 +1642,15 @@
         if self.dyn_size_ext and self.dyn_size_ext.placeholder is not None:  # fast path
             if self.dyn_size_ext.batch_ndim > 0:
                 return rf.reduce_max(
                     self.dyn_size_ext,
                     axis=self.dyn_size_ext.dim_tags,
                     # Masking is not always possible here, e.g.
                     # self = Dim{'self-att-keys'['time:var:extern_data:classes'[B]]}.
-                    use_mask=False,
+                    use_time_mask=False,
                 )
             return self.dyn_size_ext
         if self.is_batch_dim():
             res = None
             if self._extra and self._extra.src_data:
                 res = self._extra.src_data.get_batch_dim()
             elif self.batch:
```

### Comparing `returnn-1.20230418.225432/returnn/tensor/_tensor_extra.py` & `returnn-1.20230418.5121/returnn/tensor/_tensor_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -884,31 +884,33 @@
             axis += v.batch_ndim
             assert axis >= 0
         assert 0 <= axis < v.batch_ndim
         if v.feature_dim_axis != axis:
             v.feature_dim_axis = axis
         return v
 
-    def get_default_new_axis_for_dim_tag(self, dim_tag: Dim) -> int:
+    def get_default_new_axis_for_dim_tag(self, dim_tag):
         """
-        :param dim_tag:
+        :param Dim dim_tag:
+        :rtype: int
         """
         if dim_tag.is_batch_dim():
             return 0
         # Note: if dim_tag is feature, but we are sparse, we just treat is as spatial, handled below.
         if dim_tag.is_feature_dim() and not self.sparse:
             if self.feature_dim_axis is not None:
                 return self.feature_dim_axis + 1  # after existing feature-dim
             else:
                 return self.batch_ndim  # at the end
-        if dim_tag.is_dynamic() and self.get_dynamic_axes():
+        assert dim_tag.is_spatial_dim() or (dim_tag.is_feature_dim() and self.sparse)
+        if dim_tag.dimension is None and self.get_dynamic_axes():
             return self.get_dynamic_axes()[-1] + 1  # after existing dynamic axis
-        if dim_tag.is_spatial_dim() and self.get_spatial_batch_axes():
+        if self.get_spatial_batch_axes():
             return self.get_spatial_batch_axes()[-1] + 1  # after the existing spatial dim
-        elif dim_tag.is_spatial_dim() and self.feature_dim_axis is not None:
+        elif self.feature_dim_axis is not None:
             return self.feature_dim_axis  # add it before the feature dim
         else:
             return self.batch_ndim  # add it at the end
 
     def copy_add_dim_by_tag(self, dim_tag, unbroadcast=False, axis=None) -> _t.Tensor:
         """
         :param Dim dim_tag:
```

### Comparing `returnn-1.20230418.225432/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230418.5121/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230418.5121/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230418.5121/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tensor/dim.py` & `returnn-1.20230418.5121/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tensor/marked_dim.py` & `returnn-1.20230418.5121/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tensor/tensor.py` & `returnn-1.20230418.5121/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tensor/tensor_dict.py` & `returnn-1.20230418.5121/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/compat.py` & `returnn-1.20230418.5121/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/data_pipeline.py` & `returnn-1.20230418.5121/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/distributed.py` & `returnn-1.20230418.5121/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/engine.py` & `returnn-1.20230418.5121/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -288,30 +288,23 @@
     def activation_raw(raw_tensor: Layer, func: str) -> Layer:
         """activation"""
         return rfl.make_layer(
             {"class": "activation", "activation": func, "from": raw_tensor.tensor}, name=func
         ).raw_tensor
 
     @staticmethod
-    def softmax(tensor: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+    def softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """softmax"""
-        args = {}
-        if not use_mask:
-            args["use_time_mask"] = False
-        return rfl.make_layer({"class": "softmax_over_spatial", "axis": axis, "from": tensor, **args}, name="softmax")
+        return rfl.make_layer({"class": "softmax_over_spatial", "axis": axis, "from": tensor}, name="softmax")
 
     @staticmethod
-    def log_softmax(tensor: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+    def log_softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """log softmax"""
-        args = {}
-        if not use_mask:
-            args["use_time_mask"] = False
         return rfl.make_layer(
-            {"class": "softmax_over_spatial", "axis": axis, "from": tensor, "log_space": True, **args},
-            name="log_softmax",
+            {"class": "softmax_over_spatial", "axis": axis, "from": tensor, "log_space": True}, name="log_softmax"
         )
 
     @staticmethod
     def softmax_cross_entropy_with_logits(*, logits: Tensor, targets: Tensor, axis: Dim):
         """
         Efficient cross entropy.
 
@@ -503,19 +496,19 @@
         if step is not None:
             args["slice_step"] = step
         return rfl.make_layer(
             {"class": "slice", "from": source, "axis": axis, "out_dim": out_dim, **args}, name="slice"
         )
 
     @staticmethod
-    def matmul(a: Tensor, b: Tensor, *, reduce: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor:
+    def matmul(a: Tensor, b: Tensor, *, reduce: Union[Dim, Sequence[Dim]], disable_masking: bool = False) -> Tensor:
         """matmul"""
         args = {}
-        if not use_mask:
-            args["use_mask"] = False
+        if disable_masking:
+            args["disable_masking"] = True
         return rfl.make_layer({"class": "dot", "from": [a, b], "reduce": reduce, **args}, name="matmul")
 
     @staticmethod
     def range_over_dim(dim: Dim, *, dtype: Optional[str] = None) -> Tensor:
         """range over dim"""
         if not dtype and dim.dyn_size_ext:
             dtype = dim.dyn_size_ext.dtype
@@ -535,20 +528,22 @@
         :return: source with in_dim replaced by out_dim.
         """
         return rfl.make_layer(
             {"class": "reinterpret_data", "set_dim_tags": {in_dim: out_dim}, "from": source}, name="new_dim"
         )
 
     @staticmethod
-    def reduce(source: Tensor, *, mode: str, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> Tensor:
+    def reduce(
+        source: Tensor, *, mode: str, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified
+    ) -> Tensor:
         """Reduce"""
         assert mode in Backend._AllowedReduceModes
         kwargs = {}
-        if not use_mask:
-            kwargs["use_time_mask"] = False
+        if use_time_mask is not NotSpecified:
+            kwargs["use_time_mask"] = use_time_mask
         return rfl.make_layer(
             {"class": "reduce", "from": source, "mode": mode, "axis": axis, **kwargs}, name=f"reduce_{mode}"
         )
 
     @staticmethod
     @contextlib.contextmanager
     def random_journal_replay(journal: Sequence[Dict[str, Any]]):
@@ -823,37 +818,24 @@
                 description_prefix="pool",
                 in_spatial_dims=in_spatial_dims,
                 filter_size=pool_size,
                 strides=strides,
                 dilation_rate=dilation_rate,
                 padding=padding,
             )
-        other_dims = [d for d in source.dims if d not in in_spatial_dims and not d.is_batch_dim()]
-        assert other_dims  # currently not implemented otherwise, need in_dim...
-        if source.feature_dim and source.feature_dim in other_dims:
-            in_dim = source.feature_dim
-        else:
-            in_dim = other_dims[-1]
         args = {
             "mode": mode,
             "pool_size": pool_size,
             "padding": padding,
             "dilation_rate": dilation_rate,
             "strides": strides,
             "in_spatial_dims": in_spatial_dims,
             "out_spatial_dims": out_spatial_dims,
-            "in_dim": in_dim,  # it does not really matter, but we need sth currently
         }
         layer = rfl.make_layer({"class": "pool", "from": source, **args}, name="pool")
-        if source.feature_dim != in_dim:
-            # We want that the feature-dim stays consistent. PoolLayer currently just sets it to the in_dim.
-            layer = rfl.make_layer(
-                {"class": "reinterpret_data", "from": layer, "set_axes": {"F": source.feature_dim}},
-                name="pool_reset_feature",
-            )
         return layer, out_spatial_dims
 
 
 def _random_replay_eval(idx, **_kwargs):
     # noinspection PyProtectedMember
     elem = ReturnnLayersBackend._random_journal[idx]
     assert isinstance(elem, dict)
```

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/dims.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,29 +110,25 @@
         return False
     if dim in _dim_deps:
         return False
     assert dim.dyn_size_ext
     if dim.dyn_size_ext.raw_tensor is None:
         return False
     assert isinstance(dim.dyn_size_ext.raw_tensor, rfl.Layer)
-    dyn_size_ext: Tensor[rfl.Layer] = dim.dyn_size_ext
-    # Check if this was already registered before.
-    if dyn_size_ext.raw_tensor.layer_dict["class"] == "range_from_length":
-        assert dyn_size_ext.raw_tensor.layer_dict["out_spatial_dim"] == dim
-        raise Exception("why not in _dim_deps already?")
     # It means the user probably has created some dynamic dim directly.
     # This is valid.
     # But for the net dict backend, we must handle it differently.
     _dim_deps[dim] = []  # Will be reassigned below. This is just to avoid recursion.
     # Follow the logic as in returnn-common make_dim_from_length.
     # The actual range tensor is never used, but this has the side effect to set up the dim tag.
     layer_with_dim = rfl.make_layer(
         {
             "class": "range_from_length",
-            "from": dyn_size_ext.copy(),
-            "dtype": dyn_size_ext.dtype,
+            "from": dim.dyn_size_ext.copy(),
+            "dtype": dim.dyn_size_ext.dtype,
             "out_spatial_dim": dim,
         },
-        name=dim.name or dyn_size_ext.name or "unnamed_dyn_dim",
+        name=dim.dyn_size_ext.name,
     )
     _dim_deps[dim] = [layer_with_dim]
+    dim.dyn_size_ext.raw_tensor = None
     return True
```

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,31 +320,30 @@
     def _remove_unused_and_handle_subnets(self):
         # Collect all used tensor names.
         used_names = {self}  # type: Set[Layer]
         root = self.root
         queue = [
             (tensor, [])  # (tensor, path), where the path is how we get to the tensor through the graph, for debugging
             for tensor in self.marked_outputs + self.marked_losses
-        ]  # type: List[Tuple[Tensor[Layer],List[Layer]]]
+        ]  # type: List[Tuple[Tensor[Layer],List[Tensor[Layer]]]]
         while queue:
             tensor, src = queue.pop(0)
-            if tensor.raw_tensor is None:
-                raise Exception(f"tensor {tensor} has no layer defined, via {src}")
-            # Parameters usually have no parent assigned at creation time.
-            # However, we should have assigned them in _assign_param_names.
-            if not tensor.raw_tensor.parent and tensor.raw_tensor != root:
-                raise Exception(f"tensor {tensor} has no parent assigned, via {src}")
             if tensor.raw_tensor in used_names:
                 continue
             used_names.add(tensor.raw_tensor)
-            src_ = src + [tensor.raw_tensor]
+            src_ = src + [tensor]
             for dep in tensor.raw_tensor.get_tensor_dependencies():
                 if dep.tensor is not None and dep not in used_names:
                     queue.append((dep.tensor, src_))
 
+            # Parameters usually have no parent assigned at creation time.
+            # However, we should have assigned them in _assign_param_names.
+            if not tensor.raw_tensor.parent and tensor.raw_tensor != root:
+                raise Exception(f"tensor {tensor} has no parent assigned, via {src}")
+
             # Handle subnetworks: Flatten away if just a single entry. Create layer if not created yet.
             ctx = tensor.raw_tensor  # type: Layer
             ctx.make_all_sub_networks_and_optimize()
 
             # Add tensor name including all parents.
             # Do this here after the potential late assign-parent and potential subnet flattening
             # because we need to know the right parents.
```

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/make_layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,73 +50,72 @@
       Some postprocessing step might anyway simplify obsolete subnetworks,
       see :mod:`naming`.
     """
     if isinstance(name, str) or not name:
         parent_ctx = rfl.Layer.current_ctx(ignore_top_stack_frames=name_ctx_ignore_top_stack_frames + 1)
         if not name:
             name = layer_dict["class"]
-        layer = rfl.Layer(suggested_name=name, parent=parent_ctx)
+        name_ctx = rfl.Layer(suggested_name=name, parent=parent_ctx)
         created_name_ctx = True
     elif isinstance(name, rfl.Layer):
-        layer = name
+        name_ctx = name
         created_name_ctx = False
     else:
         raise TypeError(f"name must be str or Layer, not {type(name)}; or you should pass a module")
-    assert not layer.tensor and not layer.layer_dict  # not yet assigned
+    assert not name_ctx.tensor and not name_ctx.layer_dict  # not yet assigned
     layer_dict = layer_dict.copy()
 
     try:
 
         if out is not None:
-            assert isinstance(out, Tensor)
+            layer = out
         elif predefined_out_data is not None:
-            assert isinstance(predefined_out_data, Tensor)
-            out = predefined_out_data.copy_template()
+            layer = predefined_out_data.copy_template()
         else:
-            out = _tensor_from_layer_dict(layer_dict, layer=layer)
+            layer = _tensor_from_layer_dict(layer_dict, layer=name_ctx)
 
         # Do not assign name_ctx.tensor yet because we potentially could raise exceptions later.
-        assert layer.tensor is None
-        assert layer.layer_dict is None
+        assert name_ctx.tensor is None
+        assert name_ctx.layer_dict is None
 
         assert layer_dict is not None
 
-        out.control_flow_ctx = rfl.Layer.inner_control_flow()
-        if out.have_batch_axis() and not out.batch:
+        layer.control_flow_ctx = rfl.Layer.inner_control_flow()
+        if layer.have_batch_axis() and not layer.batch:
             # You could say this is a bug of RETURNN. Or at least RETURNN is just incomplete here.
             # RETURNN usually would fix that later when the layer is actually created,
             # but we don't do that here.
             # We can still try to look at dependencies and use those batch info.
             batches = []
-            for dep in layer.get_tensor_dependencies(_extra_layer_dict=layer_dict):
+            for dep in name_ctx.get_tensor_dependencies(_extra_layer_dict=layer_dict):
                 if dep.tensor is not None and dep.tensor.batch and dep.tensor.batch not in batches:
                     batches.append(dep.tensor.batch)
             if batches:
-                out.batch = BatchInfo.get_common_batch_info(batches)
-            elif layer.root.global_batch:
-                out.batch = layer.root.global_batch
-
-        layer.layer_dict = layer_dict
-        layer.tensor = out
-        out.raw_tensor = layer
+                layer.batch = BatchInfo.get_common_batch_info(batches)
+            elif name_ctx.root.global_batch:
+                layer.batch = name_ctx.root.global_batch
+
+        name_ctx.layer_dict = layer_dict
+        name_ctx.tensor = layer
+        layer.raw_tensor = name_ctx
 
     except Exception as exc:
         # Just forward the exception.
         # However, if we already created a new name_ctx for it, we can clean this up now.
         if created_name_ctx:
-            assert layer.parent
-            layer.parent.children.pop(layer.name)
+            assert name_ctx.parent
+            name_ctx.parent.children.pop(name_ctx.name)
         raise exc
 
-    for tag in out.dim_tags:
+    for tag in layer.dim_tags:
         # noinspection PyProtectedMember
-        _dims._register_dim_deps_when_novel(tag, [out])
+        _dims._register_dim_deps_when_novel(tag, [layer])
     # Debug out. Similar as RETURNN template log. Maybe put this behind a flag? Anyway, useful for now.
-    print(out)
-    return out
+    print(layer)
+    return layer
 
 
 def _get_sub_layer(layer: Tensor[rfl.Layer], name: str, *, data: Tensor) -> Tensor:
     """
     Like the "{layer}/{name}" syntax in RETURNN.
     Normally this should only be needed for internal usage.
     """
```

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230418.5121/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230418.5121/returnn/tf/frontend_low_level/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,43 +397,43 @@
             dtype=dtype,
         )
         dim_value = dim.get_dim_value()
         out.raw_tensor = tf.range(0, dim_value, dtype=out.dtype)
         return out
 
     @staticmethod
-    def reduce(source: _TT, *, mode: str, axis: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> _TT:
+    def reduce(source: _TT, *, mode: str, axis: Union[Dim, Sequence[Dim]], use_time_mask: bool = NotSpecified) -> _TT:
         """Reduce"""
         assert mode in Backend._AllowedReduceModes
         x = source
         axes = x.get_axes_from_description(axis)
-        if use_mask in (None, NotSpecified):
-            use_mask = any(x.has_dynamic_size(a) for a in axes)
+        if use_time_mask in (None, NotSpecified):
+            use_time_mask = any(x.has_dynamic_size(a) for a in axes)
         out_data = x.copy_template()
         dim_tags = [dim_tag for i, dim_tag in enumerate(x.dim_tags) if i not in axes]
         out_data = out_data.copy_template_new_dim_tags(dim_tags)
         sparse_out = mode.lower().startswith("arg")
         if sparse_out:
             assert len(axes) == 1
             out_data.sparse_dim = x.dim_tags[axes[0]]
             out_data.dtype = "int32"
-        assert isinstance(use_mask, bool)
+        assert isinstance(use_time_mask, bool)
         mode = mode.lower()
         reduce_abs_funcs = {
             name: getattr(tf, "reduce_%s" % name) for name in ["max", "min", "sum", "logsumexp", "any", "all"]
         }
         reduce_rel_func = {"mean": tf.reduce_mean}
         arg_funcs = {name: getattr(tf, name) for name in ["argmax", "argmin"]}
         funcs = dict(list(reduce_abs_funcs.items()) + list(reduce_rel_func.items()) + list(arg_funcs.items()))
         assert mode in funcs, "invalid mode %r. choose from: %r" % (mode, funcs)
         f = funcs[mode]
         x_ = x.placeholder
         # Check if we should ignore some frames, e.g. via masking.
         correction_factor = None
-        if use_mask and any(x.has_dynamic_size(a) for a in axes):
+        if use_time_mask and any(x.has_dynamic_size(a) for a in axes):
             if x.batch_dim_axis in axes and x.time_dim_axis in axes and len(axes) == 2:
                 assert mode not in arg_funcs, "unexpected arg reduce for multiple axes"
                 # Flattening.
                 axes = [a if (a < x.time_dim_axis) else (a - 1) for a in axes if a != x.time_dim_axis]
                 x = x.copy_time_flattened()
                 x_ = x.placeholder
```

### Comparing `returnn-1.20230418.225432/returnn/tf/horovod.py` & `returnn-1.20230418.5121/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230418.5121/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/layers/base.py` & `returnn-1.20230418.5121/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/layers/basic.py` & `returnn-1.20230418.5121/returnn/tf/layers/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -3421,17 +3421,16 @@
         :param str dtype:
         :param bool sparse:
         :param Dim|None out_spatial_dim:
         """
         out_spatial_dim  # noqa  # used in get_out_data_from_opts
         super(RangeFromLengthLayer, self).__init__(**kwargs)
         source = self.sources[0].output
-        # Depending on whether the dim tag existed before or not,
-        # we might not always have this condition:
-        # source.placeholder is self.output.dim_tags[0].dyn_size_ext.placeholder
+        if not self.output.dim_tags[0].is_batch_dim():
+            assert source.placeholder is self.output.dim_tags[0].dyn_size_ext.placeholder
         out = tf.range(0, tf.reduce_max(source.placeholder), dtype=dtype)
         self.output.placeholder = out
 
     @classmethod
     def get_out_data_from_opts(cls, name, sources, dtype="int32", sparse=False, out_spatial_dim=None, **kwargs):
         """
         :param str name:
@@ -5587,15 +5586,15 @@
         increase_sparse_dim=None,
         **kwargs,
     ):
         """
         :param str|list[str] switch_axes: e.g. "bt" to switch batch and time axes
         :param LayerBase|None size_base: copy the size_placeholder from the given layer
         :param LayerBase|None batch_dim_base: copy the batch dim from this layer
-        :param dict[str,Dim|str|None] set_axes:
+        :param dict[str,Dim|str] set_axes:
           This can be used to overwrite the special axes like time_dim_axis or feature_dim_axis.
           For that, use keys "B","T" or "F", and a value via :func:`Data.get_axis_from_description`.
         :param dict[str|Dim,Dim]|None set_dim_tags: axis -> new dim tag. assigns new dim tags.
           If the passed dim tag is yet undefined, this will not use same_dim_tags_as (declare_same_as)
           but create a new dim tag.
           This option is useful for generalized self attention (https://github.com/rwth-i6/returnn/issues/391).
         :param bool enforce_batch_major:
@@ -5694,15 +5693,15 @@
     ):
         """
         :param str name:
         :param list[LayerBase] sources:
         :param str|list[str] switch_axes: e.g. "bt" to switch batch and time axes
         :param LayerBase|None size_base: similar as size_target
         :param LayerBase|None batch_dim_base:
-        :param dict[str,Dim|str|None] set_axes:
+        :param dict[str,Dim|str] set_axes:
         :param dict[str|Dim,Dim]|None set_dim_tags:
         :param bool enforce_batch_major:
         :param bool enforce_time_major:
         :param bool|None set_sparse: if bool, set sparse value to this
         :param Dim|int|None|NotSpecified set_sparse_dim: set sparse dim to this. assumes that it is sparse
         :param int|None increase_sparse_dim: add this to the dim. assumes that it is sparse
         """
@@ -5734,17 +5733,18 @@
             for i in range(len(axes)):
                 setattr(out, axes_s[i], axes[(i + 1) % len(axes)])
         if set_axes:
             for s, i in sorted(set_axes.items()):
                 s = map_axis_name(s)
                 if isinstance(i, int):
                     assert enforce_batch_major or enforce_time_major, "%r: explicit set_axes %r" % (name, set_axes)
-                if i is not None:
-                    i = out.get_axis_from_description(i)
+                i = out.get_axis_from_description(i)
                 setattr(out, s, i)
+                if s == "feature_dim_axis":
+                    out.dim = out.batch_shape[out.feature_dim_axis]
         if out.size_placeholder and size_base:  # size_placeholder might be None, e.g. via DataNotAvailableLayer
             assert size_base.output.size_placeholder
             assert len(out.size_placeholder) == len(size_base.output.size_placeholder)
             # Keep same indices. Assumes same order of spatial dims.
             out.size_placeholder = {
                 i: size_base.output.size_placeholder[j]
                 for (i, j) in zip(sorted(out.size_placeholder), sorted(size_base.output.size_placeholder))
@@ -6512,15 +6512,15 @@
             dilation_rate = [dilation_rate] * len(pool_size)
         assert len(dilation_rate) == len(pool_size)
         if strides is None:
             strides = pool_size
         elif isinstance(strides, int):
             strides = [strides] * len(pool_size)
         assert len(strides) == len(pool_size)
-        super(PoolLayer, self).__init__(in_dim=in_dim, out_dim=out_dim, **kwargs)
+        super(PoolLayer, self).__init__(**kwargs)
         assert not self.input_data.sparse
         assert self.input_data.have_batch_axis()
         assert (
             self.input_data.have_feature_axis()
         ), "this should be our single input feature dim now. otherwise use input_add_feature_dim"
         if in_dim and out_dim:
             assert in_dim == out_dim
@@ -8055,28 +8055,28 @@
         self,
         reduce=NotSpecified,
         red1=NotSpecified,
         red2=NotSpecified,
         var1=NotSpecified,
         var2=NotSpecified,
         add_var2_if_empty=NotSpecified,
-        use_mask: bool = True,
+        disable_masking: bool = False,
         debug=False,
         **kwargs,
     ):
         """
         :param str|Dim|tuple[str|Dim]|list[str|Dim] reduce: reduce axes of both sources
         :param str|Dim|tuple[str|Dim]|list[str|Dim] red1: reduce axes of first source
         :param str|Dim|tuple[str|Dim]|list[str|Dim] red2: reduce axes of second source
         :param str|Dim|tuple[str|Dim]|list[str|Dim]|None var1: var axes of first source
         :param str|Dim|tuple[str|Dim]|list[str|Dim]|None var2: var axes of second source
         :param bool add_var2_if_empty: if var2=None, add dim=1 at the end
-        :param use_mask: If the reduction is over dynamic axes, to get the correct sum reduction,
+        :param disable_masking: If the reduction is over dynamic axes, to get the correct sum reduction,
             we need to apply masking to one of the inputs. This is done automatically.
-            By disabling this flag, this would be disabled.
+            By enabling this flag, this would be disabled.
         :param bool debug: will print debug shapes, etc.
 
         Earlier defaults:
           red1=-1, red2=-2, var1=-2, var2=-1, add_var2_if_empty=True.
         However, these are bad, for multiple reasons, like using integers, but also in general.
           See https://github.com/rwth-i6/returnn/issues/627 for details.
         """
@@ -8205,15 +8205,15 @@
                 ]
             )
         a_var_dim = prod(a_var_dims)
         b_var_dim = prod(b_var_dims)
         a_reduce_dyn_axes = [i for i in a_reduce_axes if a_out.batch_shape[i] is None]
         b_reduce_dyn_axes = [i for i in b_reduce_axes if b_out.batch_shape[i] is None]
         assert len(a_reduce_dyn_axes) == len(b_reduce_dyn_axes) or not a_reduce_axes or not b_reduce_axes
-        if not use_mask:
+        if disable_masking:
             self._info_reduce_mask = "disabled"
         elif a_reduce_dyn_axes and b_reduce_dyn_axes:
             a_pad, b_pad = get_padding_info_dict_ref(a), get_padding_info_dict_ref(b)
             a_pad_values = [a_pad.get(a_out.dim_tags[i], None) for i in a_reduce_dyn_axes]
             b_pad_values = [b_pad.get(b_out.dim_tags[i], None) for i in b_reduce_dyn_axes]
             if set(a_pad_values) == {0}:
                 self._info_reduce_mask = "source-0-already-masked"  # it's already masked as needed
```

### Comparing `returnn-1.20230418.225432/returnn/tf/layers/rec.py` & `returnn-1.20230418.5121/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/layers/segmental_model.py` & `returnn-1.20230418.5121/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/layers/signal_processing.py` & `returnn-1.20230418.5121/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/native_op.py` & `returnn-1.20230418.5121/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/network.py` & `returnn-1.20230418.5121/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/sprint.py` & `returnn-1.20230418.5121/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/updater.py` & `returnn-1.20230418.5121/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/util/basic.py` & `returnn-1.20230418.5121/returnn/tf/util/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1457,23 +1457,19 @@
                 return _bin_ops[k](a(x), b(x))
 
             _act_func_with_op_cache[s] = combined_op
             return combined_op
     assert False
 
 
-_ActFuncMap = {"neg": "negative"}
-
-
 def get_activation_function(s):
     """
     :param str|None s:
     :rtype: (tf.Tensor) -> tf.Tensor
     """
-    s = _ActFuncMap.get(s, s)
     if not s or s in ["none", "identity"]:
         return identity
     if "(" in s:
         return eval("lambda x: %s" % s, {"tf": tf})
     if any(k in s for k in _bin_ops):
         return _get_act_func_with_op(s)
     if hasattr(tf.nn, s):
```

### Comparing `returnn-1.20230418.225432/returnn/tf/util/data.py` & `returnn-1.20230418.5121/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/util/ken_lm.py` & `returnn-1.20230418.5121/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/tf/util/open_fst.py` & `returnn-1.20230418.5121/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/torch/data/pipeline.py` & `returnn-1.20230418.5121/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230418.5121/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/torch/data/tensor_utils.py` & `returnn-1.20230418.5121/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/torch/engine.py` & `returnn-1.20230418.5121/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/torch/frontend/_backend.py` & `returnn-1.20230418.5121/returnn/torch/frontend/_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 from typing import Optional, Union, Any, Sequence, Tuple, List, Dict
 import contextlib
 import torch
 import numpy
 
 from returnn.tensor import Tensor, Dim
-from returnn.util.basic import prod, get_global_inf_value
+from returnn.util.basic import prod, NotSpecified, get_global_inf_value
 
 # noinspection PyProtectedMember
 from returnn.frontend._backend import Backend
 from returnn.frontend import RawTensorTypes
 import returnn.frontend as rf
 
 
@@ -156,15 +156,15 @@
         :return: tensor, out_dim
         """
         assert dims
         if len(dims) == 1:
             return source, dims[0]
         first_axis = min(source.dims.index(d) for d in dims)
         pre_dims = source.dims[:first_axis]
-        post_dims = [d for d in source.dims if d not in dims and d not in pre_dims]
+        post_dims = [d for d in source.dims if d not in dims]
         if out_dim is None:
             out_dim = dims[0]
             for d in dims[1:]:
                 out_dim = out_dim * d
         source = source.copy_transpose(tuple(pre_dims) + tuple(dims) + tuple(post_dims), allow_int=False)
         out = Tensor(
             "merge_dims",
@@ -226,15 +226,17 @@
         src_axis_int = source.get_axis_from_description(axis)
         out_raw_list = torch.split(
             source.raw_tensor,
             split_size_or_sections=[d.get_dim_value() for d in out_dims],
             dim=src_axis_int,
         )
         out_tuple = tuple(
-            source.copy_template_replace_dim_tag(axis=src_axis_int, new_dim_tag=dim, name=f"split{i}")
+            source.copy_template_replace_dim_tag(
+                axis=src_axis_int, new_dim_tag=dim, name=f"{source.name}/split:{i}:{dim.description}"
+            )
             for i, dim in enumerate(out_dims)
         )
         for i, out in enumerate(out_tuple):
             out.raw_tensor = out_raw_list[i]
         return out_tuple
 
     @staticmethod
@@ -363,40 +365,38 @@
         elif hasattr(torch.nn.functional, func):
             f = getattr(torch.nn.functional, func)
         else:
             raise ValueError(f"unknown activation function {func!r}")
         return f(raw_tensor)
 
     @staticmethod
-    def softmax(tensor: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+    def softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """
         :param tensor:
         :param axis:
-        :param use_mask:
         :return: softmax over axis
         """
         out = tensor.copy_template("softmax")
-        if use_mask and axis.need_masking():
+        if axis.need_masking():
             tensor = tensor.copy()
             mask = tensor.get_sequence_mask_broadcast(axis=axis)
             inf_value = get_global_inf_value()
             tensor.raw_tensor = torch.where(mask, tensor.raw_tensor, -inf_value)
         out.raw_tensor = torch.softmax(tensor.raw_tensor, dim=tensor.dims.index(axis))
         return out
 
     @staticmethod
-    def log_softmax(tensor: Tensor, *, axis: Dim, use_mask: bool = True) -> Tensor:
+    def log_softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """
         :param tensor:
         :param axis:
-        :param use_mask:
         :return: log_softmax over axis
         """
         out = tensor.copy_template("log_softmax")
-        if use_mask and axis.need_masking():
+        if axis.need_masking():
             tensor = tensor.copy()
             mask = tensor.get_sequence_mask_broadcast(axis=axis)
             inf_value = get_global_inf_value()
             tensor.raw_tensor = torch.where(mask, tensor.raw_tensor, -inf_value)
         out.raw_tensor = torch.log_softmax(tensor.raw_tensor, dim=tensor.dims.index(axis))
         return out
 
@@ -511,16 +511,14 @@
         :param a:
         :param kind: "add", "sub", "mul", "truediv", "floordiv", "mod", "pow",
             "maximum", "minimum", "logical_and", "logical_or", "squared_difference"
         :param b:
         :return: a `kind` b
         """
         assert a.dim() == b.dim()
-        if kind == "squared_difference":
-            return (a - b) ** 2
         kind = {
             "truediv": "true_divide",
             "floordiv": "floor_divide",
             "mod": "remainder",
         }.get(kind, kind)
         op = getattr(torch, kind)  # e.g. torch.add
         return op(a, b)
@@ -606,22 +604,22 @@
                 end = end.raw_tensor
             if end is None:
                 end = axis.get_dim_value()
             out.raw_tensor = torch.narrow(source.raw_tensor, dim=axis_int, start=start, length=end - start)
         return out
 
     @staticmethod
-    def matmul(a: _TT, b: _TT, *, reduce: Union[Dim, Sequence[Dim]], use_mask: bool = True) -> _TT:
+    def matmul(a: _TT, b: _TT, *, reduce: Union[Dim, Sequence[Dim]], disable_masking: bool = False) -> _TT:
         """
         batched matmul of a and b, see base class doc string
         """
         if isinstance(reduce, Dim):
             reduce = [reduce]
 
-        if use_mask and any(dim.dyn_size_ext for dim in reduce):
+        if not disable_masking and any(dim.dyn_size_ext for dim in reduce):
             raise NotImplementedError("masking in matmul reduce not yet implemented")
         assert a.dtype == b.dtype, f"matmul: dtypes do not match: {a} vs {b}"
 
         a_dims = a.dims
         b_dims = b.dims
 
         assert all(
@@ -723,22 +721,22 @@
 
     @staticmethod
     def reduce(
         source: Tensor[torch.Tensor],
         *,
         mode: str,
         axis: Union[Dim, Sequence[Dim]],
-        use_mask: bool = True,
+        use_time_mask: bool = NotSpecified,
     ) -> Tensor[torch.Tensor]:
         """reduce"""
         assert mode in Backend._AllowedReduceModes
         if isinstance(axis, Dim):
             axis = [axis]
         assert all(isinstance(dim, Dim) for dim in axis)
-        if use_mask and any(dim.need_masking() for dim in axis):
+        if use_time_mask is not False and any(dim.need_masking() for dim in axis):
             source = source.copy()
             dtype = source.raw_tensor.dtype
             if mode == "max":
                 mask_value = torch.finfo(dtype).min if dtype.is_floating_point else torch.iinfo(dtype).min
             elif mode == "min":
                 mask_value = torch.finfo(dtype).max if dtype.is_floating_point else torch.iinfo(dtype).max
             elif mode == "sum":
@@ -1089,137 +1087,49 @@
                 description_prefix="pool",
                 in_spatial_dims=in_spatial_dims,
                 filter_size=pool_size,
                 strides=strides,
                 dilation_rate=dilation_rate,
                 padding=padding,
             )
+        assert padding == "valid"  # not implemented otherwise
         batch_dims = [d for d in source.dims if d not in tuple(in_spatial_dims)]
         # Torch conv expects (N,C,<spatial dims>) as shape.
         # batch_dims would actually cover the channel-dim (C) as well,
         # as it does not really matter to differentiate it from other batch dims.
         source = source.copy_transpose(batch_dims + list(in_spatial_dims))
         src_raw = torch.reshape(
             source.raw_tensor,
             # Potentially merge batch dims all together.
             # Keep the last as the channel-dim, but not sure if this is really relevant.
-            [-1, batch_dims[-1].get_dim_value() if batch_dims else 1] + [d.get_dim_value() for d in in_spatial_dims],
+            [-1, batch_dims[-1] if batch_dims else 1] + [d.get_dim_value() for d in in_spatial_dims],
         )
-        ceil_mode = padding.lower() == "same"
         if len(in_spatial_dims) == 1:
             # There is also conv_tbc, but it's a bit limited (no dilation)
             # and also unclear when exactly it is faster.
             out_raw = torch.nn.functional.max_pool1d(
                 src_raw,
                 kernel_size=pool_size,
                 stride=strides,
                 dilation=dilation_rate or 1,
-                ceil_mode=ceil_mode,
             )
         elif len(in_spatial_dims) == 2:
             out_raw = torch.nn.functional.max_pool2d(
                 src_raw,
                 kernel_size=pool_size,
                 stride=strides,
                 dilation=dilation_rate or 1,
-                ceil_mode=ceil_mode,
             )
         elif len(in_spatial_dims) == 3:
             out_raw = torch.nn.functional.max_pool3d(
                 src_raw,
                 kernel_size=pool_size,
                 stride=strides,
                 dilation=dilation_rate or 1,
-                ceil_mode=ceil_mode,
             )
         else:
             raise ValueError(f"invalid number of filter dims {in_spatial_dims}, expected 1, 2, or 3")
         out = Tensor("conv", dims=batch_dims + list(out_spatial_dims), dtype=source.dtype)
         out.raw_tensor = torch.reshape(out_raw, [d.get_dim_value() for d in out.dims])
         if source.feature_dim and source.feature_dim in out.dims:
             out.feature_dim = source.feature_dim
         return out, out_spatial_dims
-
-    @staticmethod
-    def lstm(
-        source: _TT,
-        *,
-        state_h: _TT,
-        state_c: _TT,
-        ff_weight: _TT,
-        rec_weight: _TT,
-        bias: Optional[_TT],
-        spatial_dim: Dim,
-        in_dim: Dim,
-        out_dim: Dim,
-    ) -> Tuple[_TT, Tuple[_TT, _TT]]:
-        """
-        Wraps the functional LSTM from PyTorch.
-
-        :return: Tuple consisting of two elements: the result as a :class:`Tensor`
-            and the new state as a :class:`State` (different from the previous one).
-        """
-        if bias is None:
-            lstm_params = (ff_weight.raw_tensor, rec_weight.raw_tensor)
-            has_biases = False
-        else:
-            # Feed-forward has priority over recurrent, and weights have priority over biases. See the torch docstring
-            # or torch LSTMCell: https://github.com/pytorch/pytorch/blob/4bead64/aten/src/ATen/native/RNN.cpp#L1458
-            lstm_params = (
-                ff_weight.raw_tensor,
-                rec_weight.raw_tensor,
-                bias.raw_tensor * 0.5,
-                bias.raw_tensor * 0.5,
-            )
-            has_biases = True
-
-        batch_dims = [d for d in source.dims if d != spatial_dim and d != in_dim]
-        source = source.copy_transpose([spatial_dim] + batch_dims + [in_dim])
-        state_h = state_h.copy_transpose(batch_dims + [out_dim])
-        state_c = state_c.copy_transpose(batch_dims + [out_dim])
-
-        source_raw = source.raw_tensor
-        state_h_raw = state_h.raw_tensor
-        state_c_raw = state_c.raw_tensor
-        batch_dim = torch.prod(torch.tensor([d.get_dim_value() for d in batch_dims])) if batch_dims else 1
-        if len(batch_dims) != 1:
-            # Torch LSTM expects (seq_len, batch, input_size) as shape.
-            # We need to merge all batch dims together.
-            source_raw = torch.reshape(
-                source_raw, [spatial_dim.get_dim_value()] + [batch_dim] + [in_dim.get_dim_value()]
-            )
-        # Torch LSTM expects (num_layers * num_directions, batch, hidden_size) as shape.
-        state_h_raw = torch.reshape(state_h_raw, [1, batch_dim, out_dim.get_dim_value()])
-        state_c_raw = torch.reshape(state_c_raw, [1, batch_dim, out_dim.get_dim_value()])
-
-        out_raw, new_state_h_raw, new_state_c_raw = torch.lstm(
-            source_raw,
-            (state_h_raw, state_c_raw),
-            lstm_params,
-            has_biases=has_biases,
-            num_layers=1,
-            dropout=0.0,
-            train=rf.get_run_ctx().train_flag,
-            bidirectional=False,
-            batch_first=False,
-        )
-
-        if len(batch_dims) != 1:
-            out_raw = torch.reshape(
-                out_raw,
-                [spatial_dim.get_dim_value()] + [d.get_dim_value() for d in batch_dims] + [out_dim.get_dim_value()],
-            )
-        new_state_h_raw = torch.reshape(new_state_h_raw, [d.get_dim_value() for d in state_h.dims])
-        new_state_c_raw = torch.reshape(new_state_c_raw, [d.get_dim_value() for d in state_c.dims])
-
-        out = source.copy_template_replace_dim_tag(axis=-1, new_dim_tag=out_dim, name="lstm")
-        out.feature_dim = out_dim
-        out.raw_tensor = out_raw
-
-        new_state_h = state_h.copy_template()
-        new_state_h.raw_tensor = new_state_h_raw
-        new_state_h.feature_dim = out_dim
-        new_state_c = state_c.copy_template()
-        new_state_c.raw_tensor = new_state_c_raw
-        new_state_c.feature_dim = out_dim
-
-        return out, (new_state_h, new_state_c)
```

### Comparing `returnn-1.20230418.225432/returnn/torch/frontend/_rand.py` & `returnn-1.20230418.5121/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/torch/frontend/bridge.py` & `returnn-1.20230418.5121/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/torch/updater.py` & `returnn-1.20230418.5121/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/basic.py` & `returnn-1.20230418.5121/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/better_exchook.py` & `returnn-1.20230418.5121/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/bpe.py` & `returnn-1.20230418.5121/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/debug.py` & `returnn-1.20230418.5121/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/debug_helpers.py` & `returnn-1.20230418.5121/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/fsa.py` & `returnn-1.20230418.5121/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230418.5121/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/pprint.py` & `returnn-1.20230418.5121/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/py-to-pickle.cpp` & `returnn-1.20230418.5121/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/sig_proc.py` & `returnn-1.20230418.5121/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn/util/task_system.py` & `returnn-1.20230418.5121/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/returnn.egg-info/PKG-INFO` & `returnn-1.20230418.5121/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230418.225432
+Version: 1.20230418.5121
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230418.225432/returnn.egg-info/SOURCES.txt` & `returnn-1.20230418.5121/returnn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -155,38 +155,32 @@
 returnn/frontend/_numpy_backend.py
 returnn/frontend/_utils.py
 returnn/frontend/array_.py
 returnn/frontend/attention.py
 returnn/frontend/cond.py
 returnn/frontend/const.py
 returnn/frontend/container.py
-returnn/frontend/control_flow_ctx.py
 returnn/frontend/conv.py
 returnn/frontend/dims.py
 returnn/frontend/dropout.py
 returnn/frontend/dtype.py
 returnn/frontend/gradient.py
 returnn/frontend/init.py
 returnn/frontend/linear.py
-returnn/frontend/loop.py
 returnn/frontend/loss.py
 returnn/frontend/math_.py
 returnn/frontend/matmul.py
 returnn/frontend/module.py
 returnn/frontend/normalization.py
 returnn/frontend/parameter.py
 returnn/frontend/rand.py
-returnn/frontend/rec.py
 returnn/frontend/reduce.py
 returnn/frontend/run_ctx.py
 returnn/frontend/state.py
 returnn/frontend/types.py
-returnn/frontend/encoder/__init__.py
-returnn/frontend/encoder/base.py
-returnn/frontend/encoder/conformer.py
 returnn/import_/__init__.py
 returnn/import_/common.py
 returnn/import_/git.py
 returnn/import_/import_.py
 returnn/sprint/__init__.py
 returnn/sprint/cache.py
 returnn/sprint/control.py
@@ -310,18 +304,15 @@
 tests/test_fork_exec.py
 tests/test_hdf_dump.py
 tests/test_rf_array.py
 tests/test_rf_attention.py
 tests/test_rf_base.py
 tests/test_rf_container.py
 tests/test_rf_conv.py
-tests/test_rf_encoder_conformer.py
-tests/test_rf_math.py
 tests/test_rf_normalization.py
-tests/test_rf_rec.py
 tests/test_tensor.py
 tests/test_tools.py
 tests/test_torch_frontend.py
 tests/test_torch_internal_frontend.py
 tests/PyCharm.idea/.gitignore
 tests/PyCharm.idea/.name
 tests/PyCharm.idea/codeStyleSettings.xml
```

### Comparing `returnn-1.20230418.225432/setup.py` & `returnn-1.20230418.5121/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/DummySprintExec.py` & `returnn-1.20230418.5121/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230418.5121/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230418.5121/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230418.5121/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/_set_num_threads1.py` & `returnn-1.20230418.5121/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/_setup_test_env.py` & `returnn-1.20230418.5121/tests/_setup_test_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,29 +196,26 @@
             print("test env hook pytest_sessionfinish")
 
         class _CustomPlugin:
             # noinspection PyShadowingNames
             def pytest_unconfigure(self, config):
                 """hook for pytest_unconfigure."""
                 print("test env hook pytest_unconfigure")
-                # This will get called (potentially) multiple times
-                # via config._ensure_unconfigure in the `finally` block
+                # This will get called (potentially) multiple times via config._ensure_unconfigure in the `finally` block
                 # in certain stages of the pytest call stack.
                 frame_ = get_current_frame()
                 while frame_:
                     assert isinstance(frame_, types.FrameType)
                     # If pytest_cmdline_main is in the call stack trace, we are not yet in the lowest stack.
                     if get_func_str_from_code_object(frame_.f_code) == "pytest_cmdline_main":
                         # We assume there is yet another lower `finally` block in the call stack
                         # which calls to config._ensure_unconfigure.
-                        # However, it would not call pytest_unconfigure again
-                        # when the configured flag is already set to False.
+                        # However, it would not call pytest_unconfigure again when the configured flag is already set to False.
                         # So we again call config._do_configure to set the flag to True again.
-                        # We don't want to run any of the other plugin hooks anymore,
-                        # so unregister them all (except us).
+                        # We don't want to run any of the other plugin hooks anymore, so unregister them all (except us).
                         for plugin in test_session.config.pluginmanager.get_plugins():
                             if plugin != self:
                                 test_session.config.pluginmanager.unregister(plugin)
                         # noinspection PyProtectedMember
                         config._do_configure()  # causes this to run again
                         return
                     frame_ = frame_.f_back
```

### Comparing `returnn-1.20230418.225432/tests/bpe-unicode-demo.codes` & `returnn-1.20230418.5121/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/bpe-unicode-demo.vocab` & `returnn-1.20230418.5121/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/lexicon_opt.isyms` & `returnn-1.20230418.5121/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/lexicon_opt.jpg` & `returnn-1.20230418.5121/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/lint_common.py` & `returnn-1.20230418.5121/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/pycharm-inspect.py` & `returnn-1.20230418.5121/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/pylint.py` & `returnn-1.20230418.5121/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/returnn-as-framework.py` & `returnn-1.20230418.5121/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/rf_utils.py` & `returnn-1.20230418.5121/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/spelling.dic` & `returnn-1.20230418.5121/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_Config.py` & `returnn-1.20230418.5121/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_Dataset.py` & `returnn-1.20230418.5121/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_Fsa.py` & `returnn-1.20230418.5121/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_GeneratingDataset.py` & `returnn-1.20230418.5121/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_HDFDataset.py` & `returnn-1.20230418.5121/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_LearningRateControl.py` & `returnn-1.20230418.5121/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_Log.py` & `returnn-1.20230418.5121/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_MultiProcDataset.py` & `returnn-1.20230418.5121/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_PTDataset.py` & `returnn-1.20230418.5121/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_Pretrain.py` & `returnn-1.20230418.5121/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_ResNet.py` & `returnn-1.20230418.5121/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_SprintDataset.py` & `returnn-1.20230418.5121/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_SprintInterface.py` & `returnn-1.20230418.5121/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TFEngine.py` & `returnn-1.20230418.5121/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TFNativeOp.py` & `returnn-1.20230418.5121/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TFNetworkLayer.py` & `returnn-1.20230418.5121/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230418.5121/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230418.5121/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TFUpdater.py` & `returnn-1.20230418.5121/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TFUtil.py` & `returnn-1.20230418.5121/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TF_determinism.py` & `returnn-1.20230418.5121/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TaskSystem.py` & `returnn-1.20230418.5121/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230418.5121/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_TranslationDataset.py` & `returnn-1.20230418.5121/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_Util.py` & `returnn-1.20230418.5121/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_demos.py` & `returnn-1.20230418.5121/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_fork_exec.py` & `returnn-1.20230418.5121/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_hdf_dump.py` & `returnn-1.20230418.5121/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_rf_array.py` & `returnn-1.20230418.5121/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_rf_attention.py` & `returnn-1.20230418.5121/tests/test_rf_container.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,125 +1,141 @@
 """
 RETURNN frontend (returnn.frontend) tests
 """
 
 from __future__ import annotations
-from typing import Tuple
 import _setup_test_env  # noqa
+from collections import OrderedDict
 import returnn.frontend as rf
 from returnn.tensor import Tensor, Dim, TensorDict, batch_dim
 from rf_utils import run_model
 
 
-def test_dot_attention():
+def test_module_list():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    key_dim = Dim(7, name="key")
-    value_dim = Dim(13, name="value")
+    in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
-            "q": Tensor("q", [batch_dim, time_dim, key_dim], dtype="float32"),
-            "k": Tensor("k", [batch_dim, time_dim, key_dim], dtype="float32"),
-            "v": Tensor("v", [batch_dim, time_dim, value_dim], dtype="float32", feature_dim_axis=2),
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
     )
 
     class _Net(rf.Module):
-        def __call__(self, q: Tensor, k: Tensor, v: Tensor) -> Tensor:
-            kv_axis = Dim(None, name=f"kv-axis")
-            k, _ = rf.replace_dim(k, in_dim=time_dim, out_dim=kv_axis)
-            v, _ = rf.replace_dim(v, in_dim=time_dim, out_dim=kv_axis)
-            return rf.dot_attention(q, k, v, axis=kv_axis, key_dim=key_dim)
+        def __init__(self):
+            super().__init__()
+            self.base_dim = Dim(3, name="linear-out")
+            dims = [self.base_dim + i for i in range(4)]
+            in_dims = [in_dim] + dims[:-1]
+            self.out_dim = dims[-1]
+            self.ls = rf.ModuleList([rf.Linear(in_dim_, out_dim_) for in_dim_, out_dim_ in zip(in_dims, dims)])
+
+        def __call__(self, out: Tensor) -> Tensor:
+            """
+            Forward
+            """
+            for layer in self.ls:
+                out = layer(out)
+            return out
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out = model(q=extern_data["q"], k=extern_data["k"], v=extern_data["v"])
-        out.mark_as_default_output(shape=(batch_dim, time_dim, value_dim))
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=(batch_dim, time_dim, model.out_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
 
 
-def test_self_attention():
+def test_sequential_base_case():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
     in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
     )
 
     class _Net(rf.Module):
         def __init__(self):
             super().__init__()
-            self.self_att = rf.SelfAttention(
-                in_dim=in_dim,
-                proj_dim=Dim(5, name="out"),
-                key_dim_total=Dim(21, name="key-dim-total"),
-                value_dim_total=Dim(33, name="value-dim-total"),
-                num_heads=3,
-            )
-            self.out_dim = self.self_att.out_dim
-
-        def __call__(self, x: Tensor, *, axis: Dim) -> Tensor:
-            """forward"""
-            return self.self_att(x, axis=axis)
+            dims = [Dim(1, name="feat1"), Dim(2, name="feat2"), Dim(3, name="feat3")]
+            in_dims = [in_dim] + dims[:-1]
+            self.out_dim = dims[-1]
+            self.seq = rf.Sequential(rf.Linear(in_dim_, out_dim_) for in_dim_, out_dim_ in zip(in_dims, dims))
+
+        def __call__(self, data: Tensor) -> Tensor:
+            """
+            Forward
+            """
+            seq = self.seq(data)
+            return seq
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out = model(extern_data["data"], axis=time_dim)
+        out = model(extern_data["data"])
         out.mark_as_default_output(shape=(batch_dim, time_dim, model.out_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
 
 
-def test_relative_positional_encoding():
+def test_sequential_named_case():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    in_dim = Dim(8, name="in")
+    in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
     )
 
     class _Net(rf.Module):
-        def __call__(self, x: Tensor, *, axis: Dim) -> Tuple[Tensor, Dim]:
-            x, dim = rf.relative_positional_encoding(axis, in_dim)
-            return x, dim
+        def __init__(self):
+            super().__init__()
+            dims = [Dim(1, name="feat1"), Dim(2, name="feat2"), Dim(3, name="feat3")]
+            self.out_dim = dims[-1]
+            x = OrderedDict()
+            x["one"] = rf.Linear(in_dim, dims[0])
+            x["two"] = rf.Linear(dims[0], dims[1])
+            x["three"] = rf.Linear(dims[1], dims[2])
+            self.seq = rf.Sequential(x)
+
+        def __call__(self, data: Tensor) -> Tensor:
+            """
+            Forward
+            """
+            seq = self.seq(data)
+            return seq
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out, dim = model(extern_data["data"], axis=time_dim)
-        out.mark_as_default_output(shape=(dim, in_dim))
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=(batch_dim, time_dim, model.out_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
 
 
-def test_rel_pos_self_attention():
+def test_parameter_list():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    in_dim = Dim(8, name="in")
+    in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
     )
 
     class _Net(rf.Module):
         def __init__(self):
             super().__init__()
-            self.self_att = rf.RelPosSelfAttention(
-                in_dim=in_dim,
-                proj_dim=Dim(5, name="out"),
-                key_dim_total=Dim(21, name="key-dim-total"),
-                value_dim_total=Dim(33, name="value-dim-total"),
-                num_heads=3,
-            )
-            self.out_dim = self.self_att.out_dim
-
-        def __call__(self, x: Tensor, *, axis: Dim) -> Tensor:
-            """forward"""
-            return self.self_att(x, axis=axis)
+            self.param_list = rf.ParameterList([rf.Parameter([in_dim]) for _ in range(3)])
+
+        def __call__(self, data: Tensor) -> Tensor:
+            """
+            Forward
+            """
+            for param in self.param_list:
+                data += param
+            return data
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out = model(extern_data["data"], axis=time_dim)
-        out.mark_as_default_output(shape=(batch_dim, time_dim, model.out_dim))
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=(batch_dim, time_dim, in_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
```

### Comparing `returnn-1.20230418.225432/tests/test_rf_base.py` & `returnn-1.20230418.5121/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_rf_conv.py` & `returnn-1.20230418.5121/tests/test_rf_conv.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,49 +65,7 @@
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out, spatial_dim = model(extern_data["data"])
         out.mark_as_default_output(shape=(batch_dim, spatial_dim, out_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
-
-
-def test_maxpool1d_padding_valid():
-    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    in_dim = Dim(7, name="in")
-    extern_data = TensorDict(
-        {
-            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
-        }
-    )
-
-    class _Net(rf.Module):
-        def __call__(self, x: rf.Tensor, *, in_spatial_dim: Dim) -> Tuple[Tensor, Dim]:
-            return rf.max_pool1d(x, pool_size=3, padding="valid", in_spatial_dim=in_spatial_dim)
-
-    # noinspection PyShadowingNames
-    def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out, out_spatial_dim = model(extern_data["data"], in_spatial_dim=time_dim)
-        out.mark_as_default_output(shape=(batch_dim, out_spatial_dim, in_dim))
-
-    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
-
-
-def test_maxpool1d_padding_same():
-    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    in_dim = Dim(7, name="in")
-    extern_data = TensorDict(
-        {
-            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
-        }
-    )
-
-    class _Net(rf.Module):
-        def __call__(self, x: rf.Tensor, *, in_spatial_dim: Dim) -> Tuple[Tensor, Dim]:
-            return rf.max_pool1d(x, pool_size=3, padding="same", in_spatial_dim=in_spatial_dim)
-
-    # noinspection PyShadowingNames
-    def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out, out_spatial_dim = model(extern_data["data"], in_spatial_dim=time_dim)
-        out.mark_as_default_output(shape=(batch_dim, out_spatial_dim, in_dim))
-
-    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
```

### Comparing `returnn-1.20230418.225432/tests/test_rf_math.py` & `returnn-1.20230418.5121/tests/test_rf_attention.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,48 +5,32 @@
 from __future__ import annotations
 import _setup_test_env  # noqa
 import returnn.frontend as rf
 from returnn.tensor import Tensor, Dim, TensorDict, batch_dim
 from rf_utils import run_model
 
 
-def test_neg():
+def test_dot_attention():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    in_dim = Dim(7, name="in")
+    key_dim = Dim(7, name="key")
+    value_dim = Dim(13, name="value")
     extern_data = TensorDict(
         {
-            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+            "q": Tensor("q", [batch_dim, time_dim, key_dim], dtype="float32"),
+            "k": Tensor("k", [batch_dim, time_dim, key_dim], dtype="float32"),
+            "v": Tensor("v", [batch_dim, time_dim, value_dim], dtype="float32", feature_dim_axis=2),
         }
     )
 
     class _Net(rf.Module):
-        def __call__(self, x: Tensor) -> Tensor:
-            return -x
+        def __call__(self, q: Tensor, k: Tensor, v: Tensor) -> Tensor:
+            kv_axis = Dim(None, name=f"kv-axis")
+            k, _ = rf.replace_dim(k, in_dim=time_dim, out_dim=kv_axis)
+            v, _ = rf.replace_dim(v, in_dim=time_dim, out_dim=kv_axis)
+            return rf.dot_attention(q, k, v, axis=kv_axis, key_dim=key_dim)
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out = model(extern_data["data"])
-        out.mark_as_default_output(shape=(batch_dim, time_dim, in_dim))
-
-    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
-
-
-def test_squared_difference():
-    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    in_dim = Dim(7, name="in")
-    extern_data = TensorDict(
-        {
-            "a": Tensor("a", [batch_dim, time_dim, in_dim], dtype="float32"),
-            "b": Tensor("b", [batch_dim, time_dim, in_dim], dtype="float32"),
-        }
-    )
-
-    class _Net(rf.Module):
-        def __call__(self, a: Tensor, b: Tensor) -> Tensor:
-            return rf.squared_difference(a, b)
-
-    # noinspection PyShadowingNames
-    def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out = model(extern_data["a"], extern_data["b"])
-        out.mark_as_default_output(shape=(batch_dim, time_dim, in_dim))
+        out = model(q=extern_data["q"], k=extern_data["k"], v=extern_data["v"])
+        out.mark_as_default_output(shape=(batch_dim, time_dim, value_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
```

### Comparing `returnn-1.20230418.225432/tests/test_rf_normalization.py` & `returnn-1.20230418.5121/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_tensor.py` & `returnn-1.20230418.5121/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_tools.py` & `returnn-1.20230418.5121/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_torch_frontend.py` & `returnn-1.20230418.5121/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tests/test_torch_internal_frontend.py` & `returnn-1.20230418.5121/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/analyze-dataset-batches.py` & `returnn-1.20230418.5121/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/bliss-collect-seq-lens.py` & `returnn-1.20230418.5121/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/bliss-dump-text.py` & `returnn-1.20230418.5121/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/bliss-get-segment-names.py` & `returnn-1.20230418.5121/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/bliss-to-ogg-zip.py` & `returnn-1.20230418.5121/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/bpe-create-lexicon.py` & `returnn-1.20230418.5121/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/calculate-word-error-rate.py` & `returnn-1.20230418.5121/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/cleanup-old-models.py` & `returnn-1.20230418.5121/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/collect-orth-symbols.py` & `returnn-1.20230418.5121/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/collect-words.py` & `returnn-1.20230418.5121/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/compile_native_op.py` & `returnn-1.20230418.5121/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/compile_tf_graph.py` & `returnn-1.20230418.5121/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/debug-dump-search-scores.py` & `returnn-1.20230418.5121/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/debug-plot-search-scores.py` & `returnn-1.20230418.5121/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/dump-dataset-raw-strings.py` & `returnn-1.20230418.5121/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/dump-dataset.py` & `returnn-1.20230418.5121/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/dump-forward-stats.py` & `returnn-1.20230418.5121/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/dump-forward.py` & `returnn-1.20230418.5121/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/dump-network-json.py` & `returnn-1.20230418.5121/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/dump-pickle.py` & `returnn-1.20230418.5121/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230418.5121/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/get-attention-weights.py` & `returnn-1.20230418.5121/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/get-best-model-epoch.py` & `returnn-1.20230418.5121/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/hdf_dump.py` & `returnn-1.20230418.5121/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230418.5121/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/import-blocks-mt-model.py` & `returnn-1.20230418.5121/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/import-t2t-mt-model.py` & `returnn-1.20230418.5121/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/Makefile` & `returnn-1.20230418.5121/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/README.md` & `returnn-1.20230418.5121/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/example/README.md` & `returnn-1.20230418.5121/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230418.5121/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230418.5121/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230418.5121/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/file.h` & `returnn-1.20230418.5121/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230418.5121/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230418.5121/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/main.cc` & `returnn-1.20230418.5121/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230418.5121/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230418.5121/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230418.5121/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/tf_avg_checkpoints.py` & `returnn-1.20230418.5121/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/tf_inspect_checkpoint.py` & `returnn-1.20230418.5121/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230418.225432/tools/tf_inspect_summary_log.py` & `returnn-1.20230418.5121/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

