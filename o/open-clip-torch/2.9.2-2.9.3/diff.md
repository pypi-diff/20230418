# Comparing `tmp/open_clip_torch-2.9.2.tar.gz` & `tmp/open_clip_torch-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_clip_torch-2.9.2.tar", last modified: Thu Jan  5 14:35:26 2023, max compression
+gzip compressed data, was "open_clip_torch-2.9.3.tar", last modified: Mon Jan  9 22:01:39 2023, max compression
```

## Comparing `open_clip_torch-2.9.2.tar` & `open_clip_torch-2.9.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 14:35:26.153121 open_clip_torch-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36652 2023-01-05 14:35:26.153121 open_clip_torch-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30920 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 14:35:26.153121 open_clip_torch-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 14:35:26.141121 open_clip_torch-2.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 14:35:26.145121 open_clip_torch-2.9.2/src/open_clip/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1356917 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/hf_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/hf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 14:35:26.149121 open_clip_torch-2.9.2/src/open_clip/model_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/RN101-quickgelu.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/RN101.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/RN50-quickgelu.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/RN50.json
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/RN50x16.json
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/RN50x4.json
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/RN50x64.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-B-16-plus-240.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-B-16-plus.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-B-16.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-B-32-plus-256.json
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-B-32.json
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-H-14.json
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-H-16.json
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-L-14-280.json
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-L-14-336.json
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-L-14.json
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-L-16-320.json
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-L-16.json
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-M-16-alt.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-M-16.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-M-32-alt.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-M-32.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-S-16-alt.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-S-16.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-S-32-alt.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-S-32.json
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-bigG-14.json
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-e-14.json
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/ViT-g-14.json
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/mt5-base-ViT-B-32.json
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/mt5-xl-ViT-H-14.json
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/roberta-ViT-B-32.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_base_w.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_large.json
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_small.json
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_tiny.json
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_xlarge.json
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_xxlarge.json
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-convnext_xxlarge_320.json
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-efficientnetv2_rw_s.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-resnetaa50d.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-swin_base_patch4_window7_224.json
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-vit_medium_patch16_gap_256.json
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/timm-vit_relpos_medium_patch16_cls_224.json
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/modified_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/timm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/open_clip/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 14:35:26.149121 open_clip_torch-2.9.2/src/open_clip_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36652 2023-01-05 14:35:25.000000 open_clip_torch-2.9.2/src/open_clip_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-01-05 14:35:26.000000 open_clip_torch-2.9.2/src/open_clip_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 14:35:25.000000 open_clip_torch-2.9.2/src/open_clip_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-05 14:35:25.000000 open_clip_torch-2.9.2/src/open_clip_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-05 14:35:25.000000 open_clip_torch-2.9.2/src/open_clip_torch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 14:35:26.149121 open_clip_torch-2.9.2/src/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/imagenet_zeroshot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/params.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-01-05 14:35:16.000000 open_clip_torch-2.9.2/src/training/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:01:39.052929 open_clip_torch-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    36652 2023-01-09 22:01:39.052929 open_clip_torch-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30920 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 22:01:39.052929 open_clip_torch-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:01:39.040929 open_clip_torch-2.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:01:39.044929 open_clip_torch-2.9.3/src/open_clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1356917 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/hf_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/hf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:01:39.048929 open_clip_torch-2.9.3/src/open_clip/model_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/RN101-quickgelu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/RN101.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/RN50-quickgelu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/RN50.json
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/RN50x16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/RN50x4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/RN50x64.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-B-16-plus-240.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-B-16-plus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-B-16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-B-32-plus-256.json
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-B-32.json
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-H-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-H-16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-L-14-280.json
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-L-14-336.json
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-L-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-L-16-320.json
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-L-16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-M-16-alt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-M-16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-M-32-alt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-M-32.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-S-16-alt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-S-16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-S-32-alt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-S-32.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-bigG-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-e-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/ViT-g-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/mt5-base-ViT-B-32.json
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/mt5-xl-ViT-H-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/roberta-ViT-B-32.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_base_w.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_large.json
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_small.json
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_tiny.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_xlarge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_xxlarge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-convnext_xxlarge_320.json
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-efficientnetv2_rw_s.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-resnetaa50d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-swin_base_patch4_window7_224.json
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-vit_medium_patch16_gap_256.json
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/timm-vit_relpos_medium_patch16_cls_224.json
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/modified_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/timm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/open_clip/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:01:39.048929 open_clip_torch-2.9.3/src/open_clip_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36652 2023-01-09 22:01:38.000000 open_clip_torch-2.9.3/src/open_clip_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-01-09 22:01:39.000000 open_clip_torch-2.9.3/src/open_clip_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 22:01:38.000000 open_clip_torch-2.9.3/src/open_clip_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-09 22:01:38.000000 open_clip_torch-2.9.3/src/open_clip_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-09 22:01:38.000000 open_clip_torch-2.9.3/src/open_clip_torch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:01:39.052929 open_clip_torch-2.9.3/src/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/imagenet_zeroshot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-01-09 22:01:29.000000 open_clip_torch-2.9.3/src/training/zero_shot.py
```

### Comparing `open_clip_torch-2.9.2/LICENSE` & `open_clip_torch-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/PKG-INFO` & `open_clip_torch-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_clip_torch
-Version: 2.9.2
+Version: 2.9.3
 Summary: OpenCLIP
 Home-page: https://github.com/mlfoundations/open_clip
 Author: 
 Author-email: 
 License: UNKNOWN
 Description: # OpenCLIP
```

### Comparing `open_clip_torch-2.9.2/README.md` & `open_clip_torch-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/setup.py` & `open_clip_torch-2.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/__init__.py` & `open_clip_torch-2.9.3/src/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/bpe_simple_vocab_16e6.txt.gz` & `open_clip_torch-2.9.3/src/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/factory.py` & `open_clip_torch-2.9.3/src/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/hf_configs.py` & `open_clip_torch-2.9.3/src/open_clip/hf_configs.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/hf_model.py` & `open_clip_torch-2.9.3/src/open_clip/hf_model.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/loss.py` & `open_clip_torch-2.9.3/src/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/model.py` & `open_clip_torch-2.9.3/src/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/modified_resnet.py` & `open_clip_torch-2.9.3/src/open_clip/modified_resnet.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/openai.py` & `open_clip_torch-2.9.3/src/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/pretrained.py` & `open_clip_torch-2.9.3/src/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/timm_model.py` & `open_clip_torch-2.9.3/src/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/tokenizer.py` & `open_clip_torch-2.9.3/src/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/transform.py` & `open_clip_torch-2.9.3/src/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/transformer.py` & `open_clip_torch-2.9.3/src/open_clip/transformer.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip/utils.py` & `open_clip_torch-2.9.3/src/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/open_clip_torch.egg-info/PKG-INFO` & `open_clip_torch-2.9.3/src/open_clip_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-clip-torch
-Version: 2.9.2
+Version: 2.9.3
 Summary: OpenCLIP
 Home-page: https://github.com/mlfoundations/open_clip
 Author: 
 Author-email: 
 License: UNKNOWN
 Description: # OpenCLIP
```

### Comparing `open_clip_torch-2.9.2/src/open_clip_torch.egg-info/SOURCES.txt` & `open_clip_torch-2.9.3/src/open_clip_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/data.py` & `open_clip_torch-2.9.3/src/training/data.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/distributed.py` & `open_clip_torch-2.9.3/src/training/distributed.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/imagenet_zeroshot_data.py` & `open_clip_torch-2.9.3/src/training/imagenet_zeroshot_data.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/logger.py` & `open_clip_torch-2.9.3/src/training/logger.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/main.py` & `open_clip_torch-2.9.3/src/training/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,15 @@
         args.train_sz = data["train"].dataloader.num_samples
         if args.val_data is not None:
             args.val_sz = data["val"].dataloader.num_samples
         # you will have to configure this for your project!
         wandb.init(
             project=args.wandb_project_name,
             name=args.name,
+            id=args.name,
             notes=args.wandb_notes,
             tags=[],
             resume='auto',
             config=vars(args),
         )
         if args.debug:
             wandb.watch(model, log='all')
```

### Comparing `open_clip_torch-2.9.2/src/training/params.py` & `open_clip_torch-2.9.3/src/training/params.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/profile.py` & `open_clip_torch-2.9.3/src/training/profile.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/scheduler.py` & `open_clip_torch-2.9.3/src/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/train.py` & `open_clip_torch-2.9.3/src/training/train.py`

 * *Files identical despite different names*

### Comparing `open_clip_torch-2.9.2/src/training/zero_shot.py` & `open_clip_torch-2.9.3/src/training/zero_shot.py`

 * *Files identical despite different names*

