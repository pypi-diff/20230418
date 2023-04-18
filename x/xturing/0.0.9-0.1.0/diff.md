# Comparing `tmp/xturing-0.0.9.tar.gz` & `tmp/xturing-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.0.9.tar", last modified: Thu Apr  6 13:16:21 2023, max compression
+gzip compressed data, was "xturing-0.1.0.tar", last modified: Tue Apr 18 12:33:56 2023, max compression
```

## Comparing `xturing-0.0.9.tar` & `xturing-0.1.0.tar`

### file list

```diff
@@ -1,108 +1,114 @@
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.495084 xturing-0.0.9/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    11357 2023-03-20 07:53:44.000000 xturing-0.0.9/LICENSE
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       34 2023-03-29 09:34:15.000000 xturing-0.0.9/MANIFEST.in
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    21067 2023-04-06 13:16:21.494447 xturing-0.0.9/PKG-INFO
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6626 2023-04-05 17:10:03.000000 xturing-0.0.9/README.md
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2135 2023-04-06 13:15:31.000000 xturing-0.0.9/pyproject.toml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       38 2023-04-06 13:16:21.495257 xturing-0.0.9/setup.cfg
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.436669 xturing-0.0.9/src/
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.441722 xturing-0.0.9/src/xturing/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       22 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/__about__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      438 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/__init__.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.449702 xturing-0.0.9/src/xturing/cli/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      561 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/cli/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2042 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/cli/api.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      989 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/cli/chat.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      131 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/cli/ui.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.452891 xturing-0.0.9/src/xturing/config/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      569 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/config/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      972 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/config/config_data_classes.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2503 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/config/finetuning_config.yaml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2627 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/config/generation_config.yaml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1502 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/config/read_config.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.456789 xturing-0.0.9/src/xturing/datasets/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      436 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/datasets/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      199 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/datasets/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     8179 2023-04-05 17:10:03.000000 xturing-0.0.9/src/xturing/datasets/instruction_dataset.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      222 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/datasets/text2image_dataset.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/datasets/text_dataset.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.465559 xturing-0.0.9/src/xturing/engines/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3076 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/engines/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      272 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/engines/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1871 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/bloom_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6273 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/causal.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1923 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/cerebras_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      804 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/distilgpt2_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1755 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/galactica_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1446 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/gpt2_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2912 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/gptj_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.466532 xturing-0.0.9/src/xturing/engines/gptj_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/engines/gptj_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7690 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/engines/gptj_utils/gptj.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3647 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/llama_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.468647 xturing-0.0.9/src/xturing/engines/llama_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       65 2023-03-26 14:55:44.000000 xturing-0.0.9/src/xturing/engines/llama_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    44486 2023-03-26 14:55:44.000000 xturing-0.0.9/src/xturing/engines/llama_utils/llama.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.471063 xturing-0.0.9/src/xturing/engines/lora_engine/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       73 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/lora_engine/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    33454 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/lora_engine/lora.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/engines/opt_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.474463 xturing-0.0.9/src/xturing/model_apis/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      864 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/model_apis/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1827 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/model_apis/ai21.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      573 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/model_apis/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1847 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/model_apis/cohere.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     4600 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/model_apis/openai.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.480404 xturing-0.0.9/src/xturing/models/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2483 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2067 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/models/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1084 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/bloom.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7132 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/causal.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1135 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/cerebras.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      579 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/distilgpt2.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1152 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/galactica.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1033 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/gpt2.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1067 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/gptj.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1097 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/llama.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1050 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/models/opt.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      542 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/models/stable_diffusion.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.482792 xturing-0.0.9/src/xturing/preprocessors/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      137 2023-03-26 14:55:44.000000 xturing-0.0.9/src/xturing/preprocessors/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      484 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/preprocessors/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     4582 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/preprocessors/instruction_collator.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2252 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/preprocessors/text_collator.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      642 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/registry.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.485328 xturing-0.0.9/src/xturing/self_instruct/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/self_instruct/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     9891 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/self_instruct/bootstrap_instructions.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     5490 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/self_instruct/generate_instances.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3737 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/self_instruct/identify_if_classification.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    14280 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2198 2023-04-05 17:10:03.000000 xturing-0.0.9/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.486519 xturing-0.0.9/src/xturing/self_instruct/templates/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3580 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/self_instruct/templates/clf_task_template.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    12674 2023-03-29 10:14:08.000000 xturing-0.0.9/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.488270 xturing-0.0.9/src/xturing/trainers/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       78 2023-03-26 14:55:44.000000 xturing-0.0.9/src/xturing/trainers/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      233 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/trainers/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     5856 2023-04-06 13:15:31.000000 xturing-0.0.9/src/xturing/trainers/lightning_trainer.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.488937 xturing-0.0.9/src/xturing/ui/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/ui/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    13646 2023-04-03 17:19:47.000000 xturing-0.0.9/src/xturing/ui/playground.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.493432 xturing-0.0.9/src/xturing/utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      215 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/utils/external_loggers.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3013 2023-04-03 17:26:37.000000 xturing-0.0.9/src/xturing/utils/hub.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      304 2023-03-26 14:55:44.000000 xturing-0.0.9/src/xturing/utils/interactive.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2147 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/utils/logging.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      621 2023-03-24 13:26:24.000000 xturing-0.0.9/src/xturing/utils/loss_fns.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1366 2023-04-03 17:19:41.000000 xturing-0.0.9/src/xturing/utils/notebooks.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6980 2023-04-05 17:10:03.000000 xturing-0.0.9/src/xturing/utils/text_splitter.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3803 2023-04-05 17:10:03.000000 xturing-0.0.9/src/xturing/utils/utils.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-06 13:16:21.445406 xturing-0.0.9/src/xturing.egg-info/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    21067 2023-04-06 13:16:21.000000 xturing-0.0.9/src/xturing.egg-info/PKG-INFO
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2976 2023-04-06 13:16:21.000000 xturing-0.0.9/src/xturing.egg-info/SOURCES.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        1 2023-04-06 13:16:21.000000 xturing-0.0.9/src/xturing.egg-info/dependency_links.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       48 2023-04-06 13:16:21.000000 xturing-0.0.9/src/xturing.egg-info/entry_points.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      212 2023-04-06 13:16:21.000000 xturing-0.0.9/src/xturing.egg-info/requires.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        8 2023-04-06 13:16:21.000000 xturing-0.0.9/src/xturing.egg-info/top_level.txt
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.512836 xturing-0.1.0/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    11357 2023-03-20 07:53:44.000000 xturing-0.1.0/LICENSE
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       34 2023-03-29 09:34:15.000000 xturing-0.1.0/MANIFEST.in
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-18 12:33:56.512284 xturing-0.1.0/PKG-INFO
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     7162 2023-04-18 12:33:45.000000 xturing-0.1.0/README.md
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2203 2023-04-18 12:33:45.000000 xturing-0.1.0/pyproject.toml
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       38 2023-04-18 12:33:56.512979 xturing-0.1.0/setup.cfg
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.456961 xturing-0.1.0/src/
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.463750 xturing-0.1.0/src/xturing/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       22 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/__about__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      438 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/__init__.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.469370 xturing-0.1.0/src/xturing/cli/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      561 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/cli/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2042 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/cli/api.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      989 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/cli/chat.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      131 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/cli/ui.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.472261 xturing-0.1.0/src/xturing/config/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      569 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/config/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      972 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/config/config_data_classes.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2701 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/config/finetuning_config.yaml
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2739 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/config/generation_config.yaml
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1862 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/config/read_config.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.476892 xturing-0.1.0/src/xturing/datasets/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      436 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/datasets/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      199 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/datasets/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     8179 2023-04-05 17:10:03.000000 xturing-0.1.0/src/xturing/datasets/instruction_dataset.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      222 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/datasets/text2image_dataset.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/datasets/text_dataset.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.483206 xturing-0.1.0/src/xturing/engines/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3182 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      272 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/engines/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1871 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/bloom_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6746 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/causal.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1923 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/cerebras_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      804 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/distilgpt2_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1755 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/galactica_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1446 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/gpt2_engine.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2885 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/engines/gptj_engine.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.484177 xturing-0.1.0/src/xturing/engines/gptj_utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/engines/gptj_utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     7690 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/engines/gptj_utils/gptj.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6256 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/llama_engine.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.485311 xturing-0.1.0/src/xturing/engines/llama_utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       65 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/engines/llama_utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    44486 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/engines/llama_utils/llama.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.487872 xturing-0.1.0/src/xturing/engines/lora_engine/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       73 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/lora_engine/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    42467 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/lora_engine/lora.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3556 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/engines/lora_engine/save_and_load.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-15 21:30:16.000000 xturing-0.1.0/src/xturing/engines/lora_engine/test.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-06 13:15:31.000000 xturing-0.1.0/src/xturing/engines/opt_engine.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.489720 xturing-0.1.0/src/xturing/engines/quant_utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       59 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/quant_utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6803 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    23551 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/engines/quant_utils/quant.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.492493 xturing-0.1.0/src/xturing/model_apis/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      864 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1827 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/ai21.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      573 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1847 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/cohere.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     4600 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/model_apis/openai.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.498464 xturing-0.1.0/src/xturing/models/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2566 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/models/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2067 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/models/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1084 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/bloom.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     7132 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/causal.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1135 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/cerebras.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      579 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/distilgpt2.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1152 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/galactica.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1033 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/gpt2.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1067 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/gptj.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2100 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/models/llama.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1050 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/models/opt.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      542 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/models/stable_diffusion.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.500499 xturing-0.1.0/src/xturing/preprocessors/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      137 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/preprocessors/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      484 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/preprocessors/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     4582 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/preprocessors/instruction_collator.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2252 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/preprocessors/text_collator.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      642 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/registry.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.503058 xturing-0.1.0/src/xturing/self_instruct/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     9891 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     5490 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/self_instruct/generate_instances.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3737 2023-04-03 17:26:37.000000 xturing-0.1.0/src/xturing/self_instruct/identify_if_classification.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    14280 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2198 2023-04-05 17:10:03.000000 xturing-0.1.0/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.504210 xturing-0.1.0/src/xturing/self_instruct/templates/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3580 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    12674 2023-03-29 10:14:08.000000 xturing-0.1.0/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.505864 xturing-0.1.0/src/xturing/trainers/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       78 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/trainers/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      233 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/trainers/base.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     5983 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/trainers/lightning_trainer.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.506795 xturing-0.1.0/src/xturing/ui/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/ui/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    13646 2023-04-03 17:19:47.000000 xturing-0.1.0/src/xturing/ui/playground.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.511469 xturing-0.1.0/src/xturing/utils/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/utils/__init__.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      215 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/utils/external_loggers.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3075 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/utils/hub.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      304 2023-03-26 14:55:44.000000 xturing-0.1.0/src/xturing/utils/interactive.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     2147 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/utils/logging.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      621 2023-03-24 13:26:24.000000 xturing-0.1.0/src/xturing/utils/loss_fns.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     1366 2023-04-03 17:19:41.000000 xturing-0.1.0/src/xturing/utils/notebooks.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     6886 2023-04-18 12:33:45.000000 xturing-0.1.0/src/xturing/utils/text_splitter.py
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3803 2023-04-05 17:10:03.000000 xturing-0.1.0/src/xturing/utils/utils.py
+drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-18 12:33:56.467361 xturing-0.1.0/src/xturing.egg-info/
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/PKG-INFO
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)     3201 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/SOURCES.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        1 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/dependency_links.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)       48 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/entry_points.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)      237 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/requires.txt
+-rw-r--r--   0 sarthaklangde   (501) staff       (20)        8 2023-04-18 12:33:56.000000 xturing-0.1.0/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.0.9/LICENSE` & `xturing-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/PKG-INFO` & `xturing-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.0.9
+Version: 0.1.0
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,59 +219,70 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: int4
 License-File: LICENSE
 
 <p align="center">
   <img src=".github/stochastic_logo_light.svg#gh-light-mode-only" width="250" alt="Stochastic.ai"/>
   <img src=".github/stochastic_logo_dark.svg#gh-dark-mode-only" width="250" alt="Stochastic.ai"/>
 </p>
-<h3 align="center">Build and control your own LLMs</h3>
+<h3 align="center">Build, customize and control your own personal LLMs</h3>
 
-___
-
-`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, GPT-2,
-OPT, Cerebras-GPT, Galactica, and more.
-By providing an easy-to-use interface for personalizing LLMs to your own data and application,
-xTuring makes it simple to build and control LLMs.
-The entire process can be done inside your computer or in your private cloud,
-ensuring data privacy and security.
-
-With `xturing` you can,
-- Ingest data from different sources and preprocess them to a format LLMs can understand
-- Scale from single to multiple GPUs for faster fine-tuning
-- Leverage memory-efficient techniques (i.e. LoRA fine-tuning) to reduce your hardware costs by up to 90% of the time
-- Explore different fine-tuning methods and benchmark them to find the best performing model
-- Evaluate fine-tuned models on well-defined metrics for in-depth analysis
-
-<br>
 <p align="center">
   <a href="https://pypi.org/project/xturing/">
     <img src="https://img.shields.io/pypi/v/xturing?style=for-the-badge" />
   </a>
   <a href="https://xturing.stochastic.ai/">
     <img src="https://img.shields.io/badge/Documentation-blue?logo=GitBook&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://discord.gg/TgHXuSJEk6">
     <img src="https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-the-badge"/>
   </a>
 </p>
+<br>
+
+___
+
+`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
+By providing an easy-to-use interface for fine-tuning LLMs to your own data and application, xTuring makes it
+simple to build, customize and control LLMs. The entire process can be done inside your computer or in your
+private cloud, ensuring data privacy and security.
+
+With `xturing` you can,
+- Ingest data from different sources and preprocess them to a format LLMs can understand
+- Scale from single to multiple GPUs for faster fine-tuning
+- Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
+- Explore different fine-tuning methods and benchmark them to find the best performing model
+- Evaluate fine-tuned models on well-defined metrics for in-depth analysis
+
+<br>
+
+## 🌟 INT4 fine-tuning and generation with LLaMA LoRA
+
+We are excited to announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and generation integration. With this update, you can fine-tune LLMs like LLaMA with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This breakthrough significantly reduces memory requirements and accelerates the fine-tuning process, allowing you to achieve state-of-the-art performance with less computational resources.
+
+More information about INT4 fine-tuning and benchmarks can be found in the [INT4 README](examples/int4_finetuning/README.md).
+
+You can check out the [LLaMA INT4 fine-tuning example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
 
 <br>
 
 ## CLI playground
 <img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
 
 ## UI playground
 <img src=".github/ui-playground2.gif" width="100%" style="margin: 0 1%;"/>
 
+<br>
+
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
 
 <br>
 
@@ -295,30 +306,24 @@
 print("Generated output by the model: {}".format(output))
 ```
 
 You can find the data folder [here](examples/llama/alpaca_data).
 
 <br>
 
-
 ## 📚 Tutorials
 - [Preparing your dataset](examples/llama/preparing_your_dataset.py)
-- [Cerebras-GPT efficient fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
-- [Cerebras-GPT efficient fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
-- [LLaMA efficient fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
-- [LLaMA efficient fine-tuning with LoRA](examples/llama/llama_lora.py)
+- [Cerebras-GPT fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
+- [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
+- [LLaMA fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
+- [LLaMA fine-tuning with LoRA](examples/llama/llama_lora.py)
 - [LLaMA fine-tuning](examples/llama/llama.py)
-- [GPT-J efficient fine-tuning with LoRA and INT8](examples/gptj/gptj_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing)
-- [GPT-J efficient fine-tuning with LoRA](examples/gptj/gptj_lora.py)
-- [Galactica efficient fine-tuning with LoRA and INT8](examples/galactica/galactica_lora_int8.py)
-- [Galactica efficient fine-tuning with LoRA](examples/galactica/galactica_lora.py)
-- [OPT efficient fine-tuning with LoRA and INT8](examples/opt/opt_lora_int8.py)
-- [OPT efficient fine-tuning with LoRA](examples/opt/opt_lora.py)
-- [GPT-2 efficient fine-tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
-
+- [GPT-J fine-tuning with LoRA and INT8](examples/gptj/gptj_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing)
+- [GPT-J fine-tuning with LoRA](examples/gptj/gptj_lora.py)
+- [GPT-2 fine-tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
 
 <br>
 
 ## 📊 Performance
 
 Here is a comparison for the performance of different fine-tuning techniques on the LLaMA 7B model. We use the [Alpaca dataset](examples/llama/alpaca_data/) for fine-tuning. The dataset contains 52K instructions.
 
@@ -337,16 +342,17 @@
 
 |      LLaMA 7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
 | --------- | ---- | ---- | ---- |
 | GPU | 33.5 GB | 23.7 GB | 21.9 GB |
 | CPU | 190 GB  | 10.2 GB | 14.9 GB |
 | Time per epoch | 21 hours  | 20 mins | 20 mins |
 
-Please submit your performance results on other GPUs.
-<br >
+Contribute to this by submitting your performance results on other GPUs by creating an issue with your hardware specifications, memory consumption and time per epoch.
+
+<br>
 
 ## 📎 Fine-tuned model checkpoints
 We have already fine-tuned some models that you can use as your base or start playing with.
 Here is how you would load them:
 
 ```python
 from xturing.models import BaseModel
@@ -354,21 +360,25 @@
 ```
 
 | model               | dataset | Path          |
 |---------------------|--------|---------------|
 | DistilGPT-2 LoRA | alpaca | `x/distilgpt2_lora_finetuned_alpaca` |
 | LLaMA LoRA          | alpaca | `x/llama_lora_finetuned_alpaca` |
 
+<br>
+
 ## 📈 Roadmap
 - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
 - [x] Dataset generation using self-instruction
-- [x] 2x more memory-efficient fine-tuning vs LoRA and unsupervised fine-tuning
+- [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
-- [x] Supports OpenAI, Cohere and AI21 Studio model APIs for dataset generation
+- [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
+- [x] INT4 LLaMA LoRA fine-tuning demo
+- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation 
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.0.9/README.md` & `xturing-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 <p align="center">
   <img src=".github/stochastic_logo_light.svg#gh-light-mode-only" width="250" alt="Stochastic.ai"/>
   <img src=".github/stochastic_logo_dark.svg#gh-dark-mode-only" width="250" alt="Stochastic.ai"/>
 </p>
-<h3 align="center">Build and control your own LLMs</h3>
+<h3 align="center">Build, customize and control your own personal LLMs</h3>
 
-___
-
-`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, GPT-2,
-OPT, Cerebras-GPT, Galactica, and more.
-By providing an easy-to-use interface for personalizing LLMs to your own data and application,
-xTuring makes it simple to build and control LLMs.
-The entire process can be done inside your computer or in your private cloud,
-ensuring data privacy and security.
-
-With `xturing` you can,
-- Ingest data from different sources and preprocess them to a format LLMs can understand
-- Scale from single to multiple GPUs for faster fine-tuning
-- Leverage memory-efficient techniques (i.e. LoRA fine-tuning) to reduce your hardware costs by up to 90% of the time
-- Explore different fine-tuning methods and benchmark them to find the best performing model
-- Evaluate fine-tuned models on well-defined metrics for in-depth analysis
-
-<br>
 <p align="center">
   <a href="https://pypi.org/project/xturing/">
     <img src="https://img.shields.io/pypi/v/xturing?style=for-the-badge" />
   </a>
   <a href="https://xturing.stochastic.ai/">
     <img src="https://img.shields.io/badge/Documentation-blue?logo=GitBook&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://discord.gg/TgHXuSJEk6">
     <img src="https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-the-badge"/>
   </a>
 </p>
+<br>
+
+___
+
+`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
+By providing an easy-to-use interface for fine-tuning LLMs to your own data and application, xTuring makes it
+simple to build, customize and control LLMs. The entire process can be done inside your computer or in your
+private cloud, ensuring data privacy and security.
+
+With `xturing` you can,
+- Ingest data from different sources and preprocess them to a format LLMs can understand
+- Scale from single to multiple GPUs for faster fine-tuning
+- Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
+- Explore different fine-tuning methods and benchmark them to find the best performing model
+- Evaluate fine-tuned models on well-defined metrics for in-depth analysis
+
+<br>
+
+## 🌟 INT4 fine-tuning and generation with LLaMA LoRA
+
+We are excited to announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and generation integration. With this update, you can fine-tune LLMs like LLaMA with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This breakthrough significantly reduces memory requirements and accelerates the fine-tuning process, allowing you to achieve state-of-the-art performance with less computational resources.
+
+More information about INT4 fine-tuning and benchmarks can be found in the [INT4 README](examples/int4_finetuning/README.md).
+
+You can check out the [LLaMA INT4 fine-tuning example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
 
 <br>
 
 ## CLI playground
 <img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
 
 ## UI playground
 <img src=".github/ui-playground2.gif" width="100%" style="margin: 0 1%;"/>
 
+<br>
+
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
 
 <br>
 
@@ -68,30 +78,24 @@
 print("Generated output by the model: {}".format(output))
 ```
 
 You can find the data folder [here](examples/llama/alpaca_data).
 
 <br>
 
-
 ## 📚 Tutorials
 - [Preparing your dataset](examples/llama/preparing_your_dataset.py)
-- [Cerebras-GPT efficient fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
-- [Cerebras-GPT efficient fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
-- [LLaMA efficient fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
-- [LLaMA efficient fine-tuning with LoRA](examples/llama/llama_lora.py)
+- [Cerebras-GPT fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
+- [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
+- [LLaMA fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
+- [LLaMA fine-tuning with LoRA](examples/llama/llama_lora.py)
 - [LLaMA fine-tuning](examples/llama/llama.py)
-- [GPT-J efficient fine-tuning with LoRA and INT8](examples/gptj/gptj_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing)
-- [GPT-J efficient fine-tuning with LoRA](examples/gptj/gptj_lora.py)
-- [Galactica efficient fine-tuning with LoRA and INT8](examples/galactica/galactica_lora_int8.py)
-- [Galactica efficient fine-tuning with LoRA](examples/galactica/galactica_lora.py)
-- [OPT efficient fine-tuning with LoRA and INT8](examples/opt/opt_lora_int8.py)
-- [OPT efficient fine-tuning with LoRA](examples/opt/opt_lora.py)
-- [GPT-2 efficient fine-tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
-
+- [GPT-J fine-tuning with LoRA and INT8](examples/gptj/gptj_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing)
+- [GPT-J fine-tuning with LoRA](examples/gptj/gptj_lora.py)
+- [GPT-2 fine-tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
 
 <br>
 
 ## 📊 Performance
 
 Here is a comparison for the performance of different fine-tuning techniques on the LLaMA 7B model. We use the [Alpaca dataset](examples/llama/alpaca_data/) for fine-tuning. The dataset contains 52K instructions.
 
@@ -110,16 +114,17 @@
 
 |      LLaMA 7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
 | --------- | ---- | ---- | ---- |
 | GPU | 33.5 GB | 23.7 GB | 21.9 GB |
 | CPU | 190 GB  | 10.2 GB | 14.9 GB |
 | Time per epoch | 21 hours  | 20 mins | 20 mins |
 
-Please submit your performance results on other GPUs.
-<br >
+Contribute to this by submitting your performance results on other GPUs by creating an issue with your hardware specifications, memory consumption and time per epoch.
+
+<br>
 
 ## 📎 Fine-tuned model checkpoints
 We have already fine-tuned some models that you can use as your base or start playing with.
 Here is how you would load them:
 
 ```python
 from xturing.models import BaseModel
@@ -127,21 +132,25 @@
 ```
 
 | model               | dataset | Path          |
 |---------------------|--------|---------------|
 | DistilGPT-2 LoRA | alpaca | `x/distilgpt2_lora_finetuned_alpaca` |
 | LLaMA LoRA          | alpaca | `x/llama_lora_finetuned_alpaca` |
 
+<br>
+
 ## 📈 Roadmap
 - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
 - [x] Dataset generation using self-instruction
-- [x] 2x more memory-efficient fine-tuning vs LoRA and unsupervised fine-tuning
+- [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
-- [x] Supports OpenAI, Cohere and AI21 Studio model APIs for dataset generation
+- [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
+- [x] INT4 LLaMA LoRA fine-tuning demo
+- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation 
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

#### html2text {}

```diff
@@ -1,84 +1,93 @@
                         [Stochastic.ai] [Stochastic.ai]
-                   **** Build and control your own LLMs ****
-___ `xturing` provides fast, efficient and simple fine-tuning of LLMs, such as
-LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica, and more. By providing an
-easy-to-use interface for personalizing LLMs to your own data and application,
-xTuring makes it simple to build and control LLMs. The entire process can be
-done inside your computer or in your private cloud, ensuring data privacy and
-security. With `xturing` you can, - Ingest data from different sources and
-preprocess them to a format LLMs can understand - Scale from single to multiple
-GPUs for faster fine-tuning - Leverage memory-efficient techniques (i.e. LoRA
-fine-tuning) to reduce your hardware costs by up to 90% of the time - Explore
-different fine-tuning methods and benchmark them to find the best performing
-model - Evaluate fine-tuned models on well-defined metrics for in-depth
-analysis
+         **** Build, customize and control your own personal LLMs ****
      [https://img.shields.io/pypi/v/xturing?style=for-the-badge] [https://
 img.shields.io/badge/Documentation-blue?logo=GitBook&logoColor=white&style=for-
  the-badge] [https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-
                                   the-badge]
 
+___ `xturing` provides fast, efficient and simple fine-tuning of LLMs, such as
+LLaMA, GPT-J, Galactica, and more. By providing an easy-to-use interface for
+fine-tuning LLMs to your own data and application, xTuring makes it simple to
+build, customize and control LLMs. The entire process can be done inside your
+computer or in your private cloud, ensuring data privacy and security. With
+`xturing` you can, - Ingest data from different sources and preprocess them to
+a format LLMs can understand - Scale from single to multiple GPUs for faster
+fine-tuning - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning)
+to reduce hardware costs by up to 90% - Explore different fine-tuning methods
+and benchmark them to find the best performing model - Evaluate fine-tuned
+models on well-defined metrics for in-depth analysis
+## ð INT4 fine-tuning and generation with LLaMA LoRA We are excited to
+announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and
+generation integration. With this update, you can fine-tune LLMs like LLaMA
+with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This
+breakthrough significantly reduces memory requirements and accelerates the
+fine-tuning process, allowing you to achieve state-of-the-art performance with
+less computational resources. More information about INT4 fine-tuning and
+benchmarks can be found in the [INT4 README](examples/int4_finetuning/
+README.md). You can check out the [LLaMA INT4 fine-tuning example](examples/
+int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
 ## CLI playground [.github/cli-playground.gif] ## UI playground [.github/ui-
-playground2.gif] ## âï¸ Installation ```bash pip install xturing ```
+playground2.gif]
+## âï¸ Installation ```bash pip install xturing ```
 ## ð Quickstart ```python from xturing.datasets import InstructionDataset
 from xturing.models import BaseModel # Load the dataset instruction_dataset =
 InstructionDataset("./alpaca_data") # Initialize the model model =
 BaseModel.create("llama_lora") # Finetune the model model.finetune
 (dataset=instruction_dataset) # Perform inference output = model.generate
 (texts=["Why LLM models are becoming so important?"]) print("Generated output
 by the model: {}".format(output)) ``` You can find the data folder [here]
 (examples/llama/alpaca_data).
 ## ð Tutorials - [Preparing your dataset](examples/llama/
-preparing_your_dataset.py) - [Cerebras-GPT efficient fine-tuning with LoRA and
-INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open In Colab]
-(https://colab.research.google.com/assets/colab-badge.svg)](https://
+preparing_your_dataset.py) - [Cerebras-GPT fine-tuning with LoRA and INT8]
+(examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
-- [Cerebras-GPT efficient fine-tuning with LoRA](examples/cerebras/
-cerebras_lora.ipynb) &ensp; [![Open In Colab](https://
+- [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb)
+&ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/
+1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing) - [LLaMA fine-tuning with LoRA
+and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open in Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
+- [LLaMA fine-tuning with LoRA](examples/llama/llama_lora.py) - [LLaMA fine-
+tuning](examples/llama/llama.py) - [GPT-J fine-tuning with LoRA and INT8]
+(examples/gptj/gptj_lora_int8.py) &ensp; [![Open in Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
-- [LLaMA efficient fine-tuning with LoRA and INT8](examples/llama/
-llama_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing) - [LLaMA efficient fine-tuning
-with LoRA](examples/llama/llama_lora.py) - [LLaMA fine-tuning](examples/llama/
-llama.py) - [GPT-J efficient fine-tuning with LoRA and INT8](examples/gptj/
-gptj_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing) - [GPT-J efficient fine-tuning
-with LoRA](examples/gptj/gptj_lora.py) - [Galactica efficient fine-tuning with
-LoRA and INT8](examples/galactica/galactica_lora_int8.py) - [Galactica
-efficient fine-tuning with LoRA](examples/galactica/galactica_lora.py) - [OPT
-efficient fine-tuning with LoRA and INT8](examples/opt/opt_lora_int8.py) - [OPT
-efficient fine-tuning with LoRA](examples/opt/opt_lora.py) - [GPT-2 efficient
-fine-tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open In Colab]
-(https://colab.research.google.com/assets/colab-badge.svg)](https://
-drive.google.com/file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
+colab.research.google.com/drive/1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing)
+- [GPT-J fine-tuning with LoRA](examples/gptj/gptj_lora.py) - [GPT-2 fine-
+tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open in Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/
+file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
 ## ð Performance Here is a comparison for the performance of different fine-
 tuning techniques on the LLaMA 7B model. We use the [Alpaca dataset](examples/
 llama/alpaca_data/) for fine-tuning. The dataset contains 52K instructions.
 Hardware: 4xA100 40GB GPU, 335GB CPU RAM Fine-tuning parameters: ```javascript
 { 'maximum sequence length': 512, 'batch size': 1, } ``` | LLaMA 7B | DeepSpeed
 + CPU Offloading | LoRA + DeepSpeed | LoRA + DeepSpeed + CPU Offloading | | ---
 ------ | ---- | ---- | ---- | | GPU | 33.5 GB | 23.7 GB | 21.9 GB | | CPU | 190
 GB | 10.2 GB | 14.9 GB | | Time per epoch | 21 hours | 20 mins | 20 mins |
-Please submit your performance results on other GPUs.
+Contribute to this by submitting your performance results on other GPUs by
+creating an issue with your hardware specifications, memory consumption and
+time per epoch.
 ## ð Fine-tuned model checkpoints We have already fine-tuned some models
 that you can use as your base or start playing with. Here is how you would load
 them: ```python from xturing.models import BaseModel model = BaseModel.load("x/
 distilgpt2_lora_finetuned_alpaca") ``` | model | dataset | Path | |------------
 ---------|--------|---------------| | DistilGPT-2 LoRA | alpaca | `x/
 distilgpt2_lora_finetuned_alpaca` | | LLaMA LoRA | alpaca | `x/
-llama_lora_finetuned_alpaca` | ## ð Roadmap - [x] Support for LLaMA, GPT-J,
-GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models - [x] Dataset generation
-using self-instruction - [x] 2x more memory-efficient fine-tuning vs LoRA and
-unsupervised fine-tuning - [x] INT8 low-precision fine-tuning support - [x]
-Supports OpenAI, Cohere and AI21 Studio model APIs for dataset generation - [x]
-Added fine-tuned checkpoints for some models to the hub - [ ] Evaluation of LLM
-models - [ ] Support for Stable Diffusion
+llama_lora_finetuned_alpaca` |
+## ð Roadmap - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT,
+Galactica and Bloom models - [x] Dataset generation using self-instruction -
+[x] Low-precision LoRA fine-tuning and unsupervised fine-tuning - [x] INT8 low-
+precision fine-tuning support - [x] OpenAI, Cohere and AI21 Studio model APIs
+for dataset generation - [x] Added fine-tuned checkpoints for some models to
+the hub - [x] INT4 LLaMA LoRA fine-tuning demo - [x] INT4 LLaMA LoRA fine-
+tuning with INT4 generation - [ ] Evaluation of LLM models - [ ] Support for
+Stable Diffusion
 ## ð¤ Help and Support If you have any questions, you can create an issue on
 this repository. You can also join our [Discord server](https://discord.gg/
 TgHXuSJEk6) and start a discussion in the `#xturing` channel.
 ## ð License This project is licensed under the Apache License 2.0 - see the
 [LICENSE](LICENSE) file for details.
 ## ð Contributing As an open source project in a rapidly evolving field, we
 welcome contributions of all kinds, including new features and better
```

### Comparing `xturing-0.0.9/pyproject.toml` & `xturing-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.0.9"
+version = "0.1.0"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
@@ -42,32 +42,36 @@
 ]
 dependencies = [
     "torch >= 1.9.0",
     "pytorch-lightning",
     "transformers==4.27.3",
     "datasets",
     "evaluate",
-    "bitsandbytes",
+    "bitsandbytes==0.37.2",
     "sentencepiece",
     "deepspeed",
     "gradio",
-    "bitsandbytes",
     "click",
     "wget",
     "ai21",
     "cohere",
     "ipywidgets",
     "openai >= 0.27.0",
     "pydantic >= 1.10.0",
     "rouge-score >= 0.1.2",
+    "accelerate",
 ]
 
 [project.scripts]
 xturing = "xturing.cli:xturing"
 
+[project.optional-dependencies]
+int4 = [
+    "torch >= 2.0"
+]
 
 [project.urls]
 homepage = "https://xturing.stochastic.ai/"
 documentation = "https://github.com/stochasticai/xturing-docs"
 repository = "https://github.com/stochasticai/xturing"
```

### Comparing `xturing-0.0.9/src/xturing/cli/__init__.py` & `xturing-0.1.0/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/cli/api.py` & `xturing-0.1.0/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/cli/chat.py` & `xturing-0.1.0/src/xturing/cli/chat.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/config/__init__.py` & `xturing-0.1.0/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/config/config_data_classes.py` & `xturing-0.1.0/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.0/src/xturing/config/finetuning_config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,41 @@
   optimizer_name: adamw
   output_dir: saved_model
 
 llama:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
+  optimizer_name: cpu_adam
 
 llama_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 1
 
 llama_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
 
+llama_lora_int4:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 8
+  max_length: 256
+
 gptj:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
+  optimizer_name: cpu_adam
 
 gptj_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 1
 
@@ -80,14 +89,15 @@
   num_train_epochs: 3
   batch_size: 16
 
 galactica:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
+  optimizer_name: cpu_adam
 
 galactica_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 1
```

### Comparing `xturing-0.0.9/src/xturing/config/generation_config.yaml` & `xturing-0.1.0/src/xturing/config/generation_config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 llama_lora_int8:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
+llama_lora_int4:
+  penalty_alpha: 0.6
+  top_k: 4
+  max_new_tokens: 256
+  do_sample: false
+
+# Contrastive search
 gptj:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
```

### Comparing `xturing-0.0.9/src/xturing/config/read_config.py` & `xturing-0.1.0/src/xturing/config/read_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,27 @@
     )
 
     xturing_config_file_path = dir_path / "xturing.json"
 
     return xturing_config_file_path.is_file()
 
 
+def exists_lora_config_file(dir_path: Union[Path, str] = None):
+    if dir_path is None:
+        return False
+    dir_path = Path(dir_path)
+    assert dir_path.is_dir(), "The following path {} should be a directory".format(
+        str(dir_path)
+    )
+
+    lora_config_file_path = dir_path / "adapter_config.json"
+
+    return lora_config_file_path.is_file()
+
+
 def read_xturing_config_file(dir_path: Union[Path, str]):
     dir_path = Path(dir_path)
     assert dir_path.is_dir(), "The following path {} should be a directory".format(
         str(dir_path)
     )
 
     xturing_config_file_path = dir_path / "xturing.json"
```

### Comparing `xturing-0.0.9/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.0/src/xturing/datasets/instruction_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/datasets/text_dataset.py` & `xturing-0.1.0/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/__init__.py` & `xturing-0.1.0/src/xturing/engines/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .gpt2_engine import GPT2Engine, GPT2Int8Engine, GPT2LoraEngine, GPT2LoraInt8Engine
 from .gptj_engine import GPTJEngine, GPTJInt8Engine, GPTJLoraEngine, GPTJLoraInt8Engine
 from .llama_engine import (
     LLamaEngine,
     LLamaInt8Engine,
     LlamaLoraEngine,
     LlamaLoraInt8Engine,
+    LlamaLoraInt4Engine,
 )
 from .opt_engine import OPTEngine, OPTInt8Engine, OPTLoraEngine, OPTLoraInt8Engine
 
 BaseEngine.add_to_registry(DistilGPT2Engine.config_name, DistilGPT2Engine)
 BaseEngine.add_to_registry(DistilGPT2LoraEngine.config_name, DistilGPT2LoraEngine)
 BaseEngine.add_to_registry(GPTJEngine.config_name, GPTJEngine)
 BaseEngine.add_to_registry(GPTJLoraEngine.config_name, GPTJLoraEngine)
@@ -38,14 +39,15 @@
 BaseEngine.add_to_registry(GPT2LoraEngine.config_name, GPT2LoraEngine)
 BaseEngine.add_to_registry(GPT2Int8Engine.config_name, GPT2Int8Engine)
 BaseEngine.add_to_registry(GPT2LoraInt8Engine.config_name, GPT2LoraInt8Engine)
 BaseEngine.add_to_registry(LLamaEngine.config_name, LLamaEngine)
 BaseEngine.add_to_registry(LlamaLoraEngine.config_name, LlamaLoraEngine)
 BaseEngine.add_to_registry(LLamaInt8Engine.config_name, LLamaInt8Engine)
 BaseEngine.add_to_registry(LlamaLoraInt8Engine.config_name, LlamaLoraInt8Engine)
+BaseEngine.add_to_registry(LlamaLoraInt4Engine.config_name, LlamaLoraInt4Engine)
 BaseEngine.add_to_registry(GalacticaEngine.config_name, GalacticaEngine)
 BaseEngine.add_to_registry(GalacticaInt8Engine.config_name, GalacticaInt8Engine)
 BaseEngine.add_to_registry(GalacticaLoraEngine.config_name, GalacticaLoraEngine)
 BaseEngine.add_to_registry(GalacticaLoraInt8Engine.config_name, GalacticaLoraInt8Engine)
 BaseEngine.add_to_registry(OPTEngine.config_name, OPTEngine)
 BaseEngine.add_to_registry(OPTLoraEngine.config_name, OPTLoraEngine)
 BaseEngine.add_to_registry(OPTInt8Engine.config_name, OPTInt8Engine)
```

### Comparing `xturing-0.0.9/src/xturing/engines/bloom_engine.py` & `xturing-0.1.0/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/causal.py` & `xturing-0.1.0/src/xturing/engines/causal.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from typing import Any, List, Optional, Union
 
 import evaluate
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from xturing.config import DEFAULT_DEVICE, DEFAULT_DTYPE
-from xturing.config.read_config import exists_xturing_config_file
+from xturing.config.read_config import (
+    exists_lora_config_file,
+    exists_xturing_config_file,
+)
 from xturing.engines.base import BaseEngine
 from xturing.engines.lora_engine import (
     LoraConfig,
     LoraModel,
     prepare_model_for_int8_training,
 )
 from xturing.utils.loss_fns import CrossEntropyLoss
@@ -139,40 +142,48 @@
         )
 
         # The model before applying LoRA
         self.base_model = self.model
 
         lora_config = LoraConfig(
             r=8,
-            lora_alpha=32,
+            lora_alpha=16,
             target_modules=target_modules,
             lora_dropout=0.05,
             bias="none",
             inference_mode=False,
+            base_model_name_or_path=self.base_model.__dict__.get("name_or_path", None),
         )
 
         if len(target_modules) == 1:
             lora_config.fan_in_fan_out = True
             lora_config.enable_lora = [True, False, True]
+        # self.model = LoraModel(lora_config, self.model)
 
-        self.model = LoraModel(lora_config, self.base_model)
-
-        if weights_path is not None and exists_xturing_config_file(weights_path):
+        if weights_path is not None and exists_lora_config_file(weights_path):
+            self.model = LoraModel.from_pretrained(self.base_model, weights_path)
+        elif weights_path is not None and exists_xturing_config_file(weights_path):
+            self.model = LoraModel(lora_config, self.model)
             model_weights_path = str(Path(weights_path).resolve() / "pytorch_model.bin")
             self.model.load_state_dict(
                 torch.load(
                     model_weights_path  # , map_location=torch.device(DEFAULT_DEVICE)
                 )
             )
         else:
+            self.model = LoraModel(lora_config, self.model)
             self.model.print_trainable_parameters()
 
         self.loss_fct = CrossEntropyLoss()
 
     def save(self, saving_path: Union[str, Path]):
         # Save HF config file
-        self.base_model.config.save_pretrained(str(saving_path))
+        self.model.config.save_pretrained(str(saving_path))
         # Save model weights
         model_weights = str(Path(saving_path).resolve() / "pytorch_model.bin")
+
         torch.save(self.model.state_dict(), model_weights)
+        # save adapter
+        self.model.save_pretrained(saving_path)
+
         # Save tokenizer
         self.tokenizer.save_pretrained(saving_path)
```

### Comparing `xturing-0.0.9/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.0/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.0/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/galactica_engine.py` & `xturing-0.1.0/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.0/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/gptj_engine.py` & `xturing-0.1.0/src/xturing/engines/gptj_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,16 @@
         transformers.models.gptj.modeling_gptj.GPTJAttention = GPTJAttention
 
         device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
         model = AutoModelForCausalLM.from_pretrained(
             "philschmid/gpt-j-6B-fp16-sharded", load_in_8bit=True, device_map=device_map
         )
 
-        tokenizer = AutoTokenizer.from_pretrained(
-            "philschmid/gpt-j-6B-fp16-sharded"
-        )
-        tokenizer.pad_token = self.tokenizer.eos_token
+        tokenizer = AutoTokenizer.from_pretrained("philschmid/gpt-j-6B-fp16-sharded")
+        tokenizer.pad_token = tokenizer.eos_token
         super().__init__(
             weights_path=weights_path, model=model, tokenizer=tokenizer, load_8bit=True
         )
 
 
 class GPTJLoraInt8Engine(CausalLoraEngine):
     config_name: str = "gptj_lora_int8_engine"
```

### Comparing `xturing-0.0.9/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.0/src/xturing/engines/gptj_utils/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.0/src/xturing/engines/llama_utils/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.0/src/xturing/engines/lora_engine/lora.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,85 +9,99 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import importlib
+import json
 import math
+import os
 import re
 import warnings
 from dataclasses import asdict, dataclass, field
 from enum import Enum
 from typing import List, Optional, Union
+import enum
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from transformers.pytorch_utils import Conv1D
 
+from xturing.engines.lora_engine.save_and_load import (
+    get_peft_model_state_dict,
+    set_peft_model_state_dict,
+)
+
 
 def is_bnb_available():
     return importlib.util.find_spec("bitsandbytes") is not None
 
 
 if is_bnb_available():
     import bitsandbytes as bnb
 
 
 def transpose(weight, fan_in_fan_out):
     return weight.T if fan_in_fan_out else weight
 
+def is_gptq_available():
+    return importlib.util.find_spec("xturing.engines.quant_utils") is not None
+
+if is_gptq_available():
+    from ..quant_utils import QuantLinear
+
+class PeftType(str, enum.Enum):
+    PROMPT_TUNING = "PROMPT_TUNING"
+    P_TUNING = "P_TUNING"
+    PREFIX_TUNING = "PREFIX_TUNING"
+    LORA = "LORA"
+
+WEIGHTS_NAME = "adapter_model.bin"
+CONFIG_NAME = "adapter_config.json"
+
 
 @dataclass
 class LoraConfig:
     """
-    This is the configuration class to store the configuration of a [`LoraModel`].
-
+    This is the configuration class to store the configuration of a [`~peft.Lora`].
     Args:
-        r (`int`): Lora attention dimension.
+        r (`int`): Lora attention dimension
         target_modules (`Union[List[str],str]`): The names of the modules to apply Lora to.
         lora_alpha (`float`): The alpha parameter for Lora scaling.
         lora_dropout (`float`): The dropout probability for Lora layers.
         merge_weights (`bool`):
             Whether to merge the weights of the Lora layers with the base transformer model in `eval` mode.
-        fan_in_fan_out (`bool`): Set this to True if the layer to replace stores weight like (`fan_in`, `fan_out`).
-        enable_lora ( `List[bool]`): Used with [`lora.MergedLinear`].
-        bias (`str`): Bias type for Lora. Can be `none`, `all` or `lora_only`.
-        modules_to_save (`List[str]`): List of modules apart from Lora layers to be set as trainable
+        fan_in_fan_out (`bool`): Set this to True if the layer to replace stores weight like (fan_in, fan_out)
+        enable_lora ( `List[bool]`): Used with `lora.MergedLinear`.
+        bias (`str`): Bias type for Lora. Can be 'none', 'all' or 'lora_only'
+        modules_to_save (`List[str]`):List of modules apart from LoRA layers to be set as trainable
             and saved in the final checkpoint.
     """
 
     r: int = field(default=8, metadata={"help": "Lora attention dimension"})
     target_modules: Optional[Union[List[str], str]] = field(
         default=None,
         metadata={
             "help": "List of module names or regex expression of the module names to replace with Lora."
             "For example, ['q', 'v'] or '.*decoder.*(SelfAttention|EncDecAttention).*(q|v)$' "
         },
     )
     lora_alpha: int = field(default=None, metadata={"help": "Lora alpha"})
     lora_dropout: float = field(default=None, metadata={"help": "Lora dropout"})
     merge_weights: bool = field(
-        default=False,
-        metadata={"help": "Merge weights of the original model and the Lora model"},
+        default=False, metadata={"help": "Merge weights of the original model and the Lora model"}
     )
     fan_in_fan_out: bool = field(
         default=False,
-        metadata={
-            "help": "Set this to True if the layer to replace stores weight like (fan_in, fan_out)"
-        },
-    )
-    enable_lora: Optional[List[bool]] = field(
-        default=None, metadata={"help": "Used with `lora.MergedLinear`."}
-    )
-    bias: str = field(
-        default="none",
-        metadata={"help": "Bias type for Lora. Can be 'none', 'all' or 'lora_only'"},
+        metadata={"help": "Set this to True if the layer to replace stores weight like (fan_in, fan_out)"},
     )
+    enable_lora: Optional[List[bool]] = field(default=None, metadata={"help": "Used with `lora.MergedLinear`."})
+    bias: str = field(default="none", metadata={"help": "Bias type for Lora. Can be 'none', 'all' or 'lora_only'"})
     modules_to_save: Optional[List[str]] = field(
         default=None,
         metadata={
             "help": "List of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint. "
             "For example, in Sequence Classification or Token Classification tasks, "
             "the final layer `classifier/score` are randomly initialized and as such need to be trainable and saved."
         },
@@ -95,88 +109,155 @@
     init_lora_weights: bool = field(
         default=True,
         metadata={"help": "Whether to initialize the weights of the Lora layers."},
     )
     inference_mode: bool = field(
         default=False, metadata={"help": "Whether to use inference mode"}
     )
+    peft_type: PeftType = PeftType.LORA
+
+    base_model_name_or_path: str = field(
+        default=None, metadata={"help": "The name of the base model to use."}
+    )
+
+    @property
+    def __dict__(self):
+        return asdict(self)
+
+    def to_dict(self):
+        return self.__dict__
+
+    def save_pretrained(self, save_directory, **kwargs):
+        r"""
+        This method saves the configuration of your adapter model in a directory.
+
+        Args:
+            save_directory (`str`):
+                The directory where the configuration will be saved.
+            kwargs (additional keyword arguments, *optional*):
+                Additional keyword arguments passed along to the [`~transformers.utils.PushToHubMixin.push_to_hub`]
+                method.
+        """
+        if os.path.isfile(save_directory):
+            raise AssertionError(
+                f"Provided path ({save_directory}) should be a directory, not a file"
+            )
+
+        os.makedirs(save_directory, exist_ok=True)
+
+        output_dict = self.__dict__
+        output_path = os.path.join(save_directory, CONFIG_NAME)
+
+        # save it
+        with open(output_path, "w") as writer:
+            writer.write(json.dumps(output_dict, indent=2, sort_keys=True))
+
+    @classmethod
+    def from_pretrained(cls, pretrained_model_name_or_path, subfolder=None, **kwargs):
+        r"""
+        This method loads the configuration of your adapter model from a directory.
+
+        Args:
+            pretrained_model_name_or_path (`str`):
+                The directory or the Hub repository id where the configuration is saved.
+            kwargs (additional keyword arguments, *optional*):
+                Additional keyword arguments passed along to the child class initialization.
+        """
+        path = (
+            os.path.join(pretrained_model_name_or_path, subfolder)
+            if subfolder is not None
+            else pretrained_model_name_or_path
+        )
+        if os.path.isfile(os.path.join(path, CONFIG_NAME)):
+            config_file = os.path.join(path, CONFIG_NAME)
+        else:
+            # try:
+            #     config_file = hf_hub_download(pretrained_model_name_or_path, CONFIG_NAME, subfolder=subfolder)
+            # except Exception:
+            raise ValueError(
+                f"Can't find '{CONFIG_NAME}' at '{pretrained_model_name_or_path}'"
+            )
+
+        loaded_attributes = cls.from_json_file(config_file)
+
+        config = cls(**kwargs)
+
+        for key, value in loaded_attributes.items():
+            if hasattr(config, key):
+                setattr(config, key, value)
+
+        return config
+
+    @classmethod
+    def from_json_file(cls, path_json_file, **kwargs):
+        r"""
+        Loads a configuration file from a json file.
+
+        Args:
+            path_json_file (`str`):
+                The path to the json file.
+        """
+        with open(path_json_file, "r") as file:
+            json_object = json.load(file)
+
+        return json_object
 
 
 class LoraModel(torch.nn.Module):
     """
     Creates Low Rank Adapter (Lora) model from a pretrained transformers model.
-
     Args:
-        model ([`~transformers.PreTrainedModel`]): The model to be adapted.
+        model ([`transformers.PreTrainedModel`]): The model to be adapted.
         config ([`LoraConfig`]): The configuration of the Lora model.
-
     Returns:
         `torch.nn.Module`: The Lora model.
-
-    Example:
-
-        ```py
-        >>> from transformers import AutoModelForSeq2SeqLM, LoraConfig
-        >>> from peft import LoraModel, LoraConfig
-
-        >>> config = LoraConfig(
-        ...     peft_type="LORA",
-        ...     task_type="SEQ_2_SEQ_LM",
-        ...     r=8,
-        ...     lora_alpha=32,
-        ...     target_modules=["q", "v"],
-        ...     lora_dropout=0.01,
-        ... )
-
-        >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base")
-        >>> lora_model = LoraModel(config, model)
-        ```
-
+    Example::
+        >>> from transformers import AutoModelForSeq2SeqLM, LoraConfig >>> from peft import LoraModel, LoraConfig >>>
+        config = LoraConfig(
+            peft_type="LORA", task_type="SEQ_2_SEQ_LM", r=8, lora_alpha=32, target_modules=["q", "v"],
+            lora_dropout=0.01, )
+        >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base") >>> lora_model = LoraModel(config, model)
     **Attributes**:
-        - **model** ([`~transformers.PreTrainedModel`]) -- The model to be adapted.
+        - **model** ([`transformers.PreTrainedModel`]) -- The model to be adapted.
         - **peft_config** ([`LoraConfig`]): The configuration of the Lora model.
     """
 
     def __init__(self, config, model):
         super().__init__()
         self.peft_config = config
         self.model = model
         self._find_and_replace()
         mark_only_lora_as_trainable(self.model, self.peft_config.bias)
         self.forward = self.model.forward
 
     def _find_and_replace(self):
         loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
+        is_gtq_quantized = getattr(self.model, "gptq", False)  # Step 1: Check if the model is GTQ quantized
+
         if loaded_in_8bit and not is_bnb_available():
             raise ImportError(
                 "To use Lora with 8-bit quantization, please install the `bitsandbytes` package. "
                 "You can install it with `pip install bitsandbytes`."
             )
         is_target_modules_in_base_model = False
         is_hf_device_map_available = hasattr(self.model, "hf_device_map")
         kwargs = {
             "r": self.peft_config.r,
             "lora_alpha": self.peft_config.lora_alpha,
             "lora_dropout": self.peft_config.lora_dropout,
             "fan_in_fan_out": self.peft_config.fan_in_fan_out,
-            "merge_weights": (
-                self.peft_config.merge_weights or self.peft_config.inference_mode
-            )
+            "merge_weights": (self.peft_config.merge_weights or self.peft_config.inference_mode)
             and not is_hf_device_map_available,
-            "init_lora_weights": self.peft_config.init_lora_weights,
         }
         key_list = [key for key, _ in self.model.named_modules()]
         for key in key_list:
             if isinstance(self.peft_config.target_modules, str):
                 target_module_found = re.fullmatch(self.peft_config.target_modules, key)
             else:
-                target_module_found = any(
-                    key.endswith(target_key)
-                    for target_key in self.peft_config.target_modules
-                )
+                target_module_found = any(key.endswith(target_key) for target_key in self.peft_config.target_modules)
             if target_module_found:
                 if not is_target_modules_in_base_model:
                     is_target_modules_in_base_model = True
                 parent, target, target_name = self._get_submodules(key)
                 bias = target.bias is not None
                 if loaded_in_8bit and isinstance(target, bnb.nn.Linear8bitLt):
                     kwargs.update(
@@ -184,53 +265,57 @@
                             "has_fp16_weights": target.state.has_fp16_weights,
                             "memory_efficient_backward": target.state.memory_efficient_backward,
                             "threshold": target.state.threshold,
                             "index": target.index,
                         }
                     )
                     if self.peft_config.enable_lora is None:
-                        new_module = Linear8bitLt(
-                            target.in_features, target.out_features, bias=bias, **kwargs
-                        )
+                        new_module = Linear8bitLt(target.in_features, target.out_features, bias=bias, **kwargs)
                     else:
                         kwargs.update({"enable_lora": self.peft_config.enable_lora})
-                        new_module = MergedLinear8bitLt(
-                            target.in_features, target.out_features, bias=bias, **kwargs
-                        )
-                elif (
-                    isinstance(target, torch.nn.Linear)
-                    and self.peft_config.enable_lora is None
-                ):
-                    new_module = Linear(
-                        target.in_features, target.out_features, bias=bias, **kwargs
+                        new_module = MergedLinear8bitLt(target.in_features, target.out_features, bias=bias, **kwargs)
+                elif is_gptq_available() and isinstance(target, QuantLinear):
+                    kwargs.update(
+                        {
+                            "bits": target.bits,
+                            "groupsize": target.groupsize,
+                        }
                     )
+                    if self.peft_config.enable_lora is None:
+                        new_module = LinearqbitLt(target.infeatures, target.outfeatures, bias=bias, **kwargs)
+                        new_module.scales = target.scales
+                        new_module.qzeros = target.qzeros
+                        new_module.g_idx = target.g_idx
+                        if target.bias:
+                            new_module.bias = target.bias
+                    else:
+                        kwargs.update({"enable_lora": self.peft_config.enable_lora})
+                        new_module = MergedLinearqbitLt(target.infeatures, target.outfeatures, bias=bias, **kwargs)
+                        new_module.scales = target.scales
+                        new_module.qzeros = target.qzeros
+                        new_module.g_idx = target.g_idx
+                        if target.bias:
+                            new_module.bias = target.bias
+                elif isinstance(target, torch.nn.Linear) and self.peft_config.enable_lora is None:
+                    new_module = Linear(target.in_features, target.out_features, bias=bias, **kwargs)
                 elif self.peft_config.enable_lora is not None:
                     kwargs.update({"enable_lora": self.peft_config.enable_lora})
                     if isinstance(target, Conv1D):
                         in_features, out_features = (
-                            target.weight.ds_shape
-                            if hasattr(target.weight, "ds_shape")
-                            else target.weight.shape
+                            target.weight.ds_shape if hasattr(target.weight, "ds_shape") else target.weight.shape
                         )
                     else:
-                        in_features, out_features = (
-                            target.in_features,
-                            target.out_features,
-                        )
+                        in_features, out_features = target.in_features, target.out_features
                         if kwargs["fan_in_fan_out"]:
                             warnings.warn(
                                 "fan_in_fan_out is set to True but the target module is not a Conv1D. "
                                 "Setting fan_in_fan_out to False."
                             )
-                            kwargs[
-                                "fan_in_fan_out"
-                            ] = self.peft_config.fan_in_fan_out = False
-                    new_module = MergedLinear(
-                        in_features, out_features, bias=bias, **kwargs
-                    )
+                            kwargs["fan_in_fan_out"] = self.peft_config.fan_in_fan_out = False
+                    new_module = MergedLinear(in_features, out_features, bias=bias, **kwargs)
                 self._replace_module(parent, target_name, new_module, target)
         if not is_target_modules_in_base_model:
             raise ValueError(
                 f"Target modules {self.peft_config.target_modules} not found in the base model. "
                 f"Please check the target modules and try again."
             )
 
@@ -238,42 +323,52 @@
         parent = self.model.get_submodule(".".join(key.split(".")[:-1]))
         target_name = key.split(".")[-1]
         target = self.model.get_submodule(key)
         return parent, target, target_name
 
     def _replace_module(self, parent_module, child_name, new_module, old_module):
         setattr(parent_module, child_name, new_module)
-        new_module.weight = old_module.weight
-        if old_module.bias is not None:
-            new_module.bias = old_module.bias
-        if getattr(old_module, "state", None) is not None:
-            new_module.state = old_module.state
-            new_module.to(old_module.weight.device)
-
-        # dispatch to correct device
-        for name, module in new_module.named_modules():
-            if "lora_" in name:
-                module.to(old_module.weight.device)
+        if is_gptq_available() and isinstance(old_module, QuantLinear):
+            new_module.qweight = old_module.qweight
+            if old_module.bias is not None:
+                new_module.bias = old_module.bias
+            if getattr(old_module, "state", None) is not None:
+                new_module.state = old_module.state
+                new_module.to(old_module.qweight.device)
+
+            # dispatch to correct device
+            for name, module in new_module.named_modules():
+                if "lora_" in name:
+                    module.to(old_module.qweight.device)
+        else:
+            new_module.weight = old_module.weight
+            if old_module.bias is not None:
+                new_module.bias = old_module.bias
+            if getattr(old_module, "state", None) is not None:
+                new_module.state = old_module.state
+                new_module.to(old_module.weight.device)
+
+            # dispatch to correct device
+            for name, module in new_module.named_modules():
+                if "lora_" in name:
+                    module.to(old_module.weight.device)
 
     def __getattr__(self, name: str):
         """Forward missing attributes to the wrapped module."""
         try:
             return super().__getattr__(name)  # defer to nn.Module's logic
         except AttributeError:
             return getattr(self.model, name)
 
     @property
     def modules_to_save(self):
         return None
 
     def get_peft_config_as_dict(self, inference: bool = False):
-        config = {
-            k: v.value if isinstance(v, Enum) else v
-            for k, v in asdict(self.peft_config).items()
-        }
+        config = {k: v.value if isinstance(v, Enum) else v for k, v in asdict(self.peft_config).items()}
         if inference:
             config["inference_mode"] = True
         return config
 
     def _set_adapter_layers(self, enabled=True):
         for module in self.model.modules():
             if isinstance(module, LoraLayer):
@@ -281,52 +376,14 @@
 
     def enable_adapter_layers(self):
         self._set_adapter_layers(enabled=True)
 
     def disable_adapter_layers(self):
         self._set_adapter_layers(enabled=False)
 
-    def merge_and_unload(self):
-        r"""
-        This method merges the LoRa layers into the base model. This is needed if someone wants to use the base model
-        as a standalone model.
-        """
-        if self.config.model_type == "gpt2":
-            raise ValueError("GPT2 models are not supported for merging LORA layers")
-
-        if getattr(self.model, "is_loaded_in_8bit", False):
-            raise ValueError(
-                "Cannot merge LORA layers when the model is loaded in 8-bit mode"
-            )
-
-        key_list = [key for key, _ in self.model.named_modules() if "lora" not in key]
-        for key in key_list:
-            parent, target, target_name = self._get_submodules(key)
-            if isinstance(target, LoraLayer):
-                bias = target.bias is not None
-                new_module = torch.nn.Linear(
-                    target.in_features, target.out_features, bias=bias
-                )
-
-                # manually merge if not merged
-                if not target.merged:
-                    # merge weights per: https://arxiv.org/pdf/2106.09685.pdf / page 4
-                    if target.r > 0:
-                        target.weight.data += (
-                            transpose(
-                                target.lora_B.weight @ target.lora_A.weight,
-                                target.fan_in_fan_out,
-                            )
-                            * target.scaling
-                        ).to(target.weight.dtype)
-                    target.merged = True
-
-                self._replace_module(parent, target_name, new_module, target)
-        return self.model
-
     def print_trainable_parameters(self):
         """
         Prints the number of trainable parameters in the model.
         """
         trainable_params = 0
         all_param = 0
         for _, param in self.named_parameters():
@@ -338,14 +395,62 @@
             all_param += num_params
             if param.requires_grad:
                 trainable_params += num_params
         print(
             f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}"
         )
 
+    def save_pretrained(self, save_directory, **kwargs):
+        if os.path.isfile(save_directory):
+            raise ValueError(
+                f"Provided path ({save_directory}) should be a directory, not a file"
+            )
+        os.makedirs(save_directory, exist_ok=True)
+
+        # for adapter_name, peft_config in self.peft_config.items():
+        # save only the trainable weights
+        output_state_dict = get_peft_model_state_dict(
+            self, kwargs.get("state_dict", None)
+        )
+        output_dir = save_directory
+        os.makedirs(output_dir, exist_ok=True)
+        torch.save(output_state_dict, os.path.join(output_dir, WEIGHTS_NAME))
+
+        # save the config and change the inference mode to `True`
+        if self.peft_config.base_model_name_or_path is None:
+            self.peft_config.base_model_name_or_path = self.model.__dict__.get(
+                "name_or_path", None
+            )
+
+        inference_mode = self.peft_config.inference_mode
+        self.peft_config.inference_mode = True
+        self.peft_config.save_pretrained(output_dir)
+        self.peft_config.inference_mode = inference_mode
+
+    @classmethod
+    def from_pretrained(cls, model, saved_dir):
+        config = LoraConfig.from_pretrained(saved_dir)
+        model = cls(config, model)
+
+        if os.path.exists(os.path.join(saved_dir, WEIGHTS_NAME)):
+            filename = os.path.join(saved_dir, WEIGHTS_NAME)
+        else:
+            raise ValueError(
+                f"Please check that the file {WEIGHTS_NAME} is present at {saved_dir}."
+            )
+
+        adapters_weights = torch.load(
+            filename,
+            map_location=torch.device("cuda" if torch.cuda.is_available() else "cpu"),
+        )
+        # load the weights into the model
+        set_peft_model_state_dict(model, adapters_weights)
+        model.eval()
+        return model
+
 
 # Below code is based on https://github.com/microsoft/LoRA/blob/main/loralib/layers.py
 # and modified to work with PyTorch FSDP
 
 
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
@@ -402,35 +507,26 @@
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         fan_in_fan_out: bool = False,  # Set this to True if the layer to replace stores weight like (fan_in, fan_out)
         merge_weights: bool = True,
         **kwargs,
     ):
-        init_lora_weights = kwargs.pop("init_lora_weights", True)
-
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoraLayer.__init__(
-            self,
-            r=r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            merge_weights=merge_weights,
-        )
+        LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=merge_weights)
 
         self.fan_in_fan_out = fan_in_fan_out
         # Actual trainable parameters
         if r > 0:
             self.lora_A = nn.Linear(in_features, r, bias=False)
             self.lora_B = nn.Linear(r, out_features, bias=False)
             self.scaling = self.lora_alpha / self.r
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
-        if init_lora_weights:
-            self.reset_parameters()
+        self.reset_parameters()
         if fan_in_fan_out:
             self.weight.data = self.weight.data.T
 
     def reset_parameters(self):
         nn.Linear.reset_parameters(self)
         if hasattr(self, "lora_A"):
             # initialize A the same way as the default for nn.Linear and B to zero
@@ -441,61 +537,47 @@
         nn.Linear.train(self, mode)
         self.lora_A.train(mode)
         self.lora_B.train(mode)
         if not mode and self.merge_weights and not self.merged:
             # Merge the weights and mark it
             if self.r > 0:
                 self.weight.data += (
-                    transpose(
-                        self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out
-                    )
-                    * self.scaling
+                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
                 )
             self.merged = True
         elif self.merge_weights and self.merged:
             # Make sure that the weights are not merged
             if self.r > 0:
                 self.weight.data -= (
-                    transpose(
-                        self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out
-                    )
-                    * self.scaling
+                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
                 )
             self.merged = False
 
     def eval(self):
         nn.Linear.eval(self)
         self.lora_A.eval()
         self.lora_B.eval()
 
     def forward(self, x: torch.Tensor):
         if self.disable_adapters:
             if self.r > 0 and self.merged:
                 self.weight.data -= (
-                    transpose(
-                        self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out
-                    )
-                    * self.scaling
+                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
                 )
                 self.merged = False
 
-            return F.linear(
-                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
-            )
+            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
         elif self.r > 0 and not self.merged:
-            result = F.linear(
-                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
-            )
+            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
             if self.r > 0:
-                result += self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
+                loraoutput = self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
+                result = result + loraoutput
             return result
         else:
-            return F.linear(
-                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
-            )
+            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
 
 
 class MergedLinear(nn.Linear, LoraLayer):
     # Lora implemented in a dense layer
     def __init__(
         self,
         in_features: int,
@@ -504,24 +586,16 @@
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         enable_lora: List[bool] = [False],
         fan_in_fan_out: bool = False,
         merge_weights: bool = True,
         **kwargs,
     ):
-        init_lora_weights = kwargs.pop("init_lora_weights", True)
-
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoraLayer.__init__(
-            self,
-            r=r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            merge_weights=merge_weights,
-        )
+        LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=merge_weights)
         if out_features % len(enable_lora) != 0:
             raise ValueError("The length of enable_lora must divide out_features")
         self.enable_lora = enable_lora
         self.fan_in_fan_out = fan_in_fan_out
         # Actual trainable parameters
         if r > 0 and any(enable_lora):
             self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
@@ -532,38 +606,32 @@
                 groups=2,
                 bias=False,
             )
             self.scaling = self.lora_alpha / self.r
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
             # Compute the indices
-            self.lora_ind = self.weight.new_zeros(
-                (out_features,), dtype=torch.bool
-            ).view(len(enable_lora), -1)
+            self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
             self.lora_ind[enable_lora, :] = True
             self.lora_ind = self.lora_ind.view(-1)
-
-        if init_lora_weights:
-            self.reset_parameters()
+        self.reset_parameters()
         if fan_in_fan_out:
             self.weight.data = self.weight.data.T
 
     def reset_parameters(self):
         nn.Linear.reset_parameters(self)
         if hasattr(self, "lora_A"):
             # initialize A the same way as the default for nn.Linear and B to zero
             nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
             nn.init.zeros_(self.lora_B.weight)
 
     def zero_pad(self, x):
         result = x.new_zeros((*x.shape[:-1], self.out_features))
         result = result.view(-1, self.out_features)
-        result[:, self.lora_ind] = x.reshape(
-            -1, self.out_features // len(self.enable_lora) * sum(self.enable_lora)
-        )
+        result[:, self.lora_ind] = x.reshape(-1, self.out_features // len(self.enable_lora) * sum(self.enable_lora))
         return result.view((*x.shape[:-1], self.out_features))
 
     def train(self, mode: bool = True):
         nn.Linear.train(self, mode)
         self.lora_A.train(mode)
         self.lora_B.train(mode)
         if not mode and self.merge_weights and not self.merged:
@@ -574,33 +642,29 @@
                         self.lora_A.weight.data.unsqueeze(0),
                         self.lora_B.weight.data,
                         groups=sum(self.enable_lora),
                     )
                     .squeeze(0)
                     .transpose(-2, -1)
                 )
-                self.weight.data += transpose(
-                    self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out
-                )
+                self.weight.data += transpose(self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out)
             self.merged = True
         elif self.merge_weights and self.merged:
             # Make sure that the weights are not merged
             if self.r > 0 and any(self.enable_lora):
                 delta_w = (
                     F.conv1d(
                         self.lora_A.weight.data.unsqueeze(0),
                         self.lora_B.weight.data,
                         groups=sum(self.enable_lora),
                     )
                     .squeeze(0)
                     .transpose(-2, -1)
                 )
-                self.weight.data -= transpose(
-                    self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out
-                )
+                self.weight.data -= transpose(self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out)
             self.merged = False
 
     def eval(self):
         nn.Linear.eval(self)
         self.lora_A.eval()
         self.lora_B.eval()
 
@@ -612,29 +676,21 @@
                         self.lora_A.weight.data.unsqueeze(0),
                         self.lora_B.weight.data,
                         groups=sum(self.enable_lora),
                     )
                     .squeeze(0)
                     .transpose(-2, -1)
                 )
-                self.weight.data -= transpose(
-                    self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out
-                )
+                self.weight.data -= transpose(self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out)
                 self.merged = False
-            return F.linear(
-                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
-            )
+            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
         elif self.merged:
-            return F.linear(
-                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
-            )
+            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
         else:
-            result = F.linear(
-                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
-            )
+            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
             if self.r > 0:
                 after_A = self.lora_A(self.lora_dropout(x))
                 after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
                 result += self.zero_pad(after_B) * self.scaling
             return result
 
 
@@ -653,27 +709,19 @@
         ):
             bnb.nn.Linear8bitLt.__init__(
                 self,
                 in_features,
                 out_features,
                 bias=kwargs.get("bias", True),
                 has_fp16_weights=kwargs.get("has_fp16_weights", True),
-                memory_efficient_backward=kwargs.get(
-                    "memory_efficient_backward", False
-                ),
+                memory_efficient_backward=kwargs.get("memory_efficient_backward", False),
                 threshold=kwargs.get("threshold", 0.0),
                 index=kwargs.get("index", None),
             )
-            LoraLayer.__init__(
-                self,
-                r=r,
-                lora_alpha=lora_alpha,
-                lora_dropout=lora_dropout,
-                merge_weights=False,
-            )
+            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
             # Actual trainable parameters
             if r > 0:
                 self.lora_A = nn.Linear(in_features, r, bias=False)
                 self.lora_B = nn.Linear(r, out_features, bias=False)
                 self.scaling = self.lora_alpha / self.r
                 # Freezing the pre-trained weight matrix
                 self.weight.requires_grad = False
@@ -692,25 +740,18 @@
                 return result
             elif self.r > 0:
                 if not torch.is_autocast_enabled():
                     expected_dtype = result.dtype
 
                     if x.dtype != torch.float32:
                         x = x.float()
-                    output = (
-                        self.lora_B(self.lora_A(self.lora_dropout(x))).to(
-                            expected_dtype
-                        )
-                        * self.scaling
-                    )
+                    output = self.lora_B(self.lora_A(self.lora_dropout(x))).to(expected_dtype) * self.scaling
                     result += output
                 else:
-                    output = (
-                        self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
-                    )
+                    output = self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
                     result += output
             return result
 
     class MergedLinear8bitLt(bnb.nn.Linear8bitLt, LoraLayer):
         # Lora implemented in a dense layer
         def __init__(
             self,
@@ -724,27 +765,19 @@
         ):
             bnb.nn.Linear8bitLt.__init__(
                 self,
                 in_features,
                 out_features,
                 bias=kwargs.get("bias", True),
                 has_fp16_weights=kwargs.get("has_fp16_weights", True),
-                memory_efficient_backward=kwargs.get(
-                    "memory_efficient_backward", False
-                ),
+                memory_efficient_backward=kwargs.get("memory_efficient_backward", False),
                 threshold=kwargs.get("threshold", 0.0),
                 index=kwargs.get("index", None),
             )
-            LoraLayer.__init__(
-                self,
-                r=r,
-                lora_alpha=lora_alpha,
-                lora_dropout=lora_dropout,
-                merge_weights=False,
-            )
+            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
             if out_features % len(enable_lora) != 0:
                 raise ValueError("The length of enable_lora must divide out_features")
             self.enable_lora = enable_lora
             # Actual trainable parameters
             if r > 0 and any(enable_lora):
                 self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
                 self.lora_B = nn.Conv1d(
@@ -754,17 +787,15 @@
                     groups=2,
                     bias=False,
                 )
                 self.scaling = self.lora_alpha / self.r
                 # Freezing the pre-trained weight matrix
                 self.weight.requires_grad = False
                 # Compute the indices
-                self.lora_ind = self.weight.new_zeros(
-                    (out_features,), dtype=torch.bool
-                ).view(len(enable_lora), -1)
+                self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
                 self.lora_ind[enable_lora, :] = True
                 self.lora_ind = self.lora_ind.view(-1)
             self.reset_parameters()
 
         def reset_parameters(self):
             if hasattr(self, "lora_A"):
                 # initialize A the same way as the default for nn.Linear and B to zero
@@ -795,26 +826,152 @@
                 else:
                     after_A = self.lora_A(self.lora_dropout(x))
                     after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
                     output = self.zero_pad(after_B) * self.scaling
                     result += output
             return result
 
+if is_gptq_available():
+    class LinearqbitLt(QuantLinear, LoraLayer):
+        # Lora implemented in a dense layer
+        def __init__(
+            self,
+            in_features,
+            out_features,
+            r: int = 0,
+            lora_alpha: int = 1,
+            lora_dropout: float = 0.0,
+            **kwargs,
+        ):
+            
+            QuantLinear.__init__(
+                self,
+                kwargs.get('bits', 4),
+                kwargs.get('groupsize', 128),
+                in_features,
+                out_features,
+                kwargs.get('bias', False),
+            )
+
+            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
+            # Actual trainable parameters
+            if r > 0:
+                self.lora_A = nn.Linear(in_features, r, bias=False)
+                self.lora_B = nn.Linear(r, out_features, bias=False)
+                self.scaling = self.lora_alpha / self.r
+                # Freezing the pre-trained weight matrix
+                self.qweight.requires_grad = False
+                self.scales.requires_grad = False
+                self.qzeros.requires_grad = False
+            self.reset_parameters()
+
+        def reset_parameters(self):
+            if hasattr(self, "lora_A"):
+                # initialize A the same way as the default for nn.Linear and B to zero
+                # nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
+                self.lora_A.weight = torch.nn.Parameter(torch.nn.init.kaiming_uniform(self.lora_A.weight, a=math.sqrt(5)))
+                nn.init.zeros_(self.lora_B.weight)
+
+        def forward(self, x: torch.Tensor):
+            # x = x.detach()
+            custom_layer_output = super().forward(x)
+            
+            dtype = custom_layer_output.dtype
+            x = x.float()
+            lora_output = self.lora_B(self.lora_A(self.lora_dropout(x))).to(dtype) * self.scaling
+            result = custom_layer_output + lora_output
+            return result
+
+    class MergedLinearqbitLt(QuantLinear, LoraLayer):
+        # Lora implemented in a dense layer
+        def __init__(
+            self,
+            in_features: int,
+            out_features: int,
+            r: int = 0,
+            lora_alpha: int = 1,
+            lora_dropout: float = 0.0,
+            enable_lora: List[bool] = [False],
+            **kwargs,
+        ):
+            QuantLinear.__init__(
+                self,
+                kwargs.get('bits', 4),
+                kwargs.get('groupsize', 128),
+                in_features,
+                out_features,
+            )
+            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
+            if out_features % len(enable_lora) != 0:
+                raise ValueError("The length of enable_lora must divide out_features")
+            self.enable_lora = enable_lora
+            # Actual trainable parameters
+            if r > 0 and any(enable_lora):
+                self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
+                self.lora_B = nn.Conv1d(
+                    r * sum(enable_lora),
+                    out_features // len(enable_lora) * sum(enable_lora),
+                    kernel_size=1,
+                    groups=2,
+                    bias=False,
+                )
+                self.scaling = self.lora_alpha / self.r
+                # Freezing the pre-trained weight matrix
+                self.qweight.requires_grad = False
+                # Compute the indices
+                self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
+                self.lora_ind[enable_lora, :] = True
+                self.lora_ind = self.lora_ind.view(-1)
+            self.reset_parameters()
+
+        def reset_parameters(self):
+            if hasattr(self, "lora_A"):
+                # initialize A the same way as the default for nn.Linear and B to zero
+                nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
+                nn.init.zeros_(self.lora_B.weight)
+
+        def zero_pad(self, x):
+            result = x.new_zeros((*x.shape[:-1], self.out_features))
+            result = result.view(-1, self.out_features)
+            result[:, self.lora_ind] = x.reshape(
+                -1, self.out_features // len(self.enable_lora) * sum(self.enable_lora)
+            )
+            return result.view((*x.shape[:-1], self.out_features))
+
+        def forward(self, x: torch.Tensor):
+            result = super().forward(x)#.detach()
+            if self.disable_adapters:
+                return result
+            elif self.r > 0:
+                if not torch.is_autocast_enabled():
+                    expected_dtype = result.dtype
+                    if x.dtype != torch.float32:
+                        x = x.float()
+                    after_A = self.lora_A(self.lora_dropout(x))
+                    after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
+                    output = self.zero_pad(after_B).to(expected_dtype) * self.scaling
+                    result += output
+                else:
+                    after_A = self.lora_A(self.lora_dropout(x))
+                    after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
+                    output = self.zero_pad(after_B) * self.scaling
+                    result += output
+            return result
+
 
 def prepare_model_for_int8_training(
     model,
     output_embedding_layer_name="lm_head",
     use_gradient_checkpointing=True,
     layer_norm_names=["layer_norm"],
 ):
     r"""
     This method wrapps the entire protocol for preparing a model before running a training. This includes:
         1- Cast the layernorm in fp32 2- making output embedding layer require grads 3- Add the upcasting of the lm
         head to fp32
-
     Args:
         model, (`transformers.PreTrainedModel`):
             The loaded model from `transformers`
     """
     loaded_in_8bit = getattr(model, "is_loaded_in_8bit", False)
 
     for name, param in model.named_parameters():
@@ -846,15 +1003,14 @@
         output_embedding_layer = getattr(model, output_embedding_layer_name)
         input_dtype = output_embedding_layer.weight.dtype
 
         class CastOutputToFloat(torch.nn.Sequential):
             r"""
             Manually cast to the expected dtype of the lm_head as sometimes there is a final layer norm that is casted
             in fp32
-
             """
 
             def forward(self, x):
                 return super().forward(x.to(input_dtype)).to(torch.float32)
 
         setattr(
             model,
```

### Comparing `xturing-0.0.9/src/xturing/engines/opt_engine.py` & `xturing-0.1.0/src/xturing/engines/opt_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/model_apis/__init__.py` & `xturing-0.1.0/src/xturing/model_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/model_apis/ai21.py` & `xturing-0.1.0/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/model_apis/base.py` & `xturing-0.1.0/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/model_apis/cohere.py` & `xturing-0.1.0/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/model_apis/openai.py` & `xturing-0.1.0/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/__init__.py` & `xturing-0.1.0/src/xturing/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .base import BaseModel
 from .bloom import Bloom, BloomInt8, BloomLora, BloomLoraInt8
 from .cerebras import Cerebras, CerebrasInt8, CerebrasLora, CerebrasLoraInt8
 from .distilgpt2 import DistilGPT2, DistilGPT2Lora
 from .galactica import Galactica, GalacticaInt8, GalacticaLora, GalacticaLoraInt8
 from .gpt2 import GPT2, GPT2Int8, GPT2Lora, GPT2LoraInt8
 from .gptj import GPTJ, GPTJInt8, GPTJLora, GPTJLoraInt8
-from .llama import Llama, LlamaInt8, LlamaLora, LlamaLoraInt8
+from .llama import Llama, LlamaInt8, LlamaLora, LlamaLoraInt8, LlamaLoraInt4
 from .opt import OPT, OPTInt8, OPTLora, OPTLoraInt8
 from .stable_diffusion import StableDiffusion
 
 BaseModel.add_to_registry(DistilGPT2.config_name, DistilGPT2)
 BaseModel.add_to_registry(DistilGPT2Lora.config_name, DistilGPT2Lora)
 BaseModel.add_to_registry(GPT2.config_name, GPT2)
 BaseModel.add_to_registry(GPT2Lora.config_name, GPT2Lora)
@@ -19,14 +19,15 @@
 BaseModel.add_to_registry(GPTJLora.config_name, GPTJLora)
 BaseModel.add_to_registry(GPTJInt8.config_name, GPTJInt8)
 BaseModel.add_to_registry(GPTJLoraInt8.config_name, GPTJLoraInt8)
 BaseModel.add_to_registry(Llama.config_name, Llama)
 BaseModel.add_to_registry(LlamaLora.config_name, LlamaLora)
 BaseModel.add_to_registry(LlamaInt8.config_name, LlamaInt8)
 BaseModel.add_to_registry(LlamaLoraInt8.config_name, LlamaLoraInt8)
+BaseModel.add_to_registry(LlamaLoraInt4.config_name, LlamaLoraInt4)
 BaseModel.add_to_registry(Galactica.config_name, Galactica)
 BaseModel.add_to_registry(GalacticaLora.config_name, GalacticaLora)
 BaseModel.add_to_registry(GalacticaInt8.config_name, GalacticaInt8)
 BaseModel.add_to_registry(GalacticaLoraInt8.config_name, GalacticaLoraInt8)
 BaseModel.add_to_registry(OPT.config_name, OPT)
 BaseModel.add_to_registry(OPTLora.config_name, OPTLora)
 BaseModel.add_to_registry(OPTInt8.config_name, OPTInt8)
```

### Comparing `xturing-0.0.9/src/xturing/models/base.py` & `xturing-0.1.0/src/xturing/models/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/bloom.py` & `xturing-0.1.0/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/causal.py` & `xturing-0.1.0/src/xturing/models/causal.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/cerebras.py` & `xturing-0.1.0/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/distilgpt2.py` & `xturing-0.1.0/src/xturing/models/distilgpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/galactica.py` & `xturing-0.1.0/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/gpt2.py` & `xturing-0.1.0/src/xturing/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/gptj.py` & `xturing-0.1.0/src/xturing/models/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/models/llama.py` & `xturing-0.1.0/src/xturing/models/opt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from typing import List, Optional, Union
+from typing import Optional
 
-from xturing.engines.llama_engine import (
-    LLamaEngine,
-    LLamaInt8Engine,
-    LlamaLoraEngine,
-    LlamaLoraInt8Engine,
+from xturing.engines.opt_engine import (
+    OPTEngine,
+    OPTInt8Engine,
+    OPTLoraEngine,
+    OPTLoraInt8Engine,
 )
 from xturing.models.causal import (
     CausalInt8Model,
     CausalLoraInt8Model,
     CausalLoraModel,
     CausalModel,
 )
 
 
-class Llama(CausalModel):
-    config_name: str = "llama"
+class OPT(CausalModel):
+    config_name: str = "opt"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(LLamaEngine.config_name, weights_path)
+        super().__init__(OPTEngine.config_name, weights_path)
 
 
-class LlamaLora(CausalLoraModel):
-    config_name: str = "llama_lora"
+class OPTLora(CausalLoraModel):
+    config_name: str = "opt_lora"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(LlamaLoraEngine.config_name, weights_path)
+        super().__init__(OPTLoraEngine.config_name, weights_path)
 
 
-class LlamaInt8(CausalInt8Model):
-    config_name: str = "llama_int8"
+class OPTInt8(CausalInt8Model):
+    config_name: str = "opt_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(LLamaInt8Engine.config_name, weights_path)
+        super().__init__(OPTInt8Engine.config_name, weights_path)
 
 
-class LlamaLoraInt8(CausalLoraInt8Model):
-    config_name: str = "llama_lora_int8"
+class OPTLoraInt8(CausalLoraInt8Model):
+    config_name: str = "opt_lora_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(LlamaLoraInt8Engine.config_name, weights_path)
+        super().__init__(OPTLoraInt8Engine.config_name, weights_path)
```

### Comparing `xturing-0.0.9/src/xturing/models/stable_diffusion.py` & `xturing-0.1.0/src/xturing/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.0/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.0/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/registry.py` & `xturing-0.1.0/src/xturing/registry.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.0/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.0/src/xturing/self_instruct/generate_instances.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.0/src/xturing/self_instruct/identify_if_classification.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.0/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.0/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.0/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.0/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.0/src/xturing/trainers/lightning_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         max_epochs: int = 3,
         batch_size: int = 2,
         learning_rate: float = 1e-3,
         optimizer_name: str = "adamw",
         use_lora: bool = False,
         use_deepspeed: bool = False,
         max_training_time_in_secs: Optional[int] = None,
+        lora_type: int = 16,
     ):
         self.lightning_model = TuringLightningModule(
             model_engine=model_engine,
             train_dataset=train_dataset,
             preprocessor=preprocessor,
             batch_size=batch_size,
             learning_rate=learning_rate,
@@ -125,14 +126,16 @@
 
         if max_training_time_in_secs is not None:
             training_callbacks.append(
                 callbacks.Timer(
                     duration=datetime.timedelta(seconds=max_training_time_in_secs)
                 )
             )
+        model_engine.model.train()
+        model_engine.model.print_trainable_parameters()
 
         if DEFAULT_DEVICE.type == "cpu":
             self.trainer = Trainer(
                 num_nodes=1,
                 accelerator="cpu",
                 max_epochs=max_epochs,
                 callbacks=training_callbacks,
@@ -163,15 +166,15 @@
                     else "deepspeed_stage_2"
                 )
 
             self.trainer = Trainer(
                 num_nodes=1,
                 accelerator="gpu",
                 strategy=strategy,
-                precision=16,
+                precision=lora_type,
                 max_epochs=max_epochs,
                 callbacks=training_callbacks,
                 enable_checkpointing=True,
                 log_every_n_steps=50,
             )
 
     def fit(self):
```

### Comparing `xturing-0.0.9/src/xturing/ui/playground.py` & `xturing-0.1.0/src/xturing/ui/playground.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/utils/hub.py` & `xturing-0.1.0/src/xturing/utils/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,11 +84,12 @@
         "distilgpt2": make_model_url("distilgpt2"),
         "distilgpt2_lora": make_model_url("distilgpt2_lora"),
         "llama_lora": make_model_url("llama_lora"),
         "distilgpt2_lora_finetuned_alpaca": make_model_url(
             "distilgpt2_lora_finetuned_alpaca"
         ),
         "llama_lora_finetuned_alpaca": make_model_url("llama_lora_finetuned_alpaca"),
+        "llama_lora_int4": make_model_url("llama_lora_int4"),
     }
 
     def __init__(self):
         super().__init__("x/", Path("models"))
```

### Comparing `xturing-0.0.9/src/xturing/utils/logging.py` & `xturing-0.1.0/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/utils/loss_fns.py` & `xturing-0.1.0/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/utils/notebooks.py` & `xturing-0.1.0/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing/utils/text_splitter.py` & `xturing-0.1.0/src/xturing/utils/text_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import (
     AbstractSet,
     Any,
     Callable,
     Collection,
     Iterable,
     List,
-    Literal,
     Optional,
     Union,
 )
 
 logger = logging.getLogger()
 
 
@@ -114,16 +113,16 @@
             )
         return cls(length_function=_huggingface_tokenizer_length, **kwargs)
 
     @classmethod
     def from_tiktoken_encoder(
         cls,
         encoding_name: str = "gpt2",
-        allowed_special: Union[Literal["all"], AbstractSet[str]] = set(),
-        disallowed_special: Union[Literal["all"], Collection[str]] = "all",
+        allowed_special = set(),
+        disallowed_special = set(),
         **kwargs: Any,
     ) -> TextSplitter:
         """Text splitter that uses tiktoken encoder to count length."""
         try:
             import tiktoken
         except ImportError:
             raise ValueError(
```

### Comparing `xturing-0.0.9/src/xturing/utils/utils.py` & `xturing-0.1.0/src/xturing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xturing-0.0.9/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.0/src/xturing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.0.9
+Version: 0.1.0
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,59 +219,70 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: int4
 License-File: LICENSE
 
 <p align="center">
   <img src=".github/stochastic_logo_light.svg#gh-light-mode-only" width="250" alt="Stochastic.ai"/>
   <img src=".github/stochastic_logo_dark.svg#gh-dark-mode-only" width="250" alt="Stochastic.ai"/>
 </p>
-<h3 align="center">Build and control your own LLMs</h3>
+<h3 align="center">Build, customize and control your own personal LLMs</h3>
 
-___
-
-`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, GPT-2,
-OPT, Cerebras-GPT, Galactica, and more.
-By providing an easy-to-use interface for personalizing LLMs to your own data and application,
-xTuring makes it simple to build and control LLMs.
-The entire process can be done inside your computer or in your private cloud,
-ensuring data privacy and security.
-
-With `xturing` you can,
-- Ingest data from different sources and preprocess them to a format LLMs can understand
-- Scale from single to multiple GPUs for faster fine-tuning
-- Leverage memory-efficient techniques (i.e. LoRA fine-tuning) to reduce your hardware costs by up to 90% of the time
-- Explore different fine-tuning methods and benchmark them to find the best performing model
-- Evaluate fine-tuned models on well-defined metrics for in-depth analysis
-
-<br>
 <p align="center">
   <a href="https://pypi.org/project/xturing/">
     <img src="https://img.shields.io/pypi/v/xturing?style=for-the-badge" />
   </a>
   <a href="https://xturing.stochastic.ai/">
     <img src="https://img.shields.io/badge/Documentation-blue?logo=GitBook&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://discord.gg/TgHXuSJEk6">
     <img src="https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-the-badge"/>
   </a>
 </p>
+<br>
+
+___
+
+`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
+By providing an easy-to-use interface for fine-tuning LLMs to your own data and application, xTuring makes it
+simple to build, customize and control LLMs. The entire process can be done inside your computer or in your
+private cloud, ensuring data privacy and security.
+
+With `xturing` you can,
+- Ingest data from different sources and preprocess them to a format LLMs can understand
+- Scale from single to multiple GPUs for faster fine-tuning
+- Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
+- Explore different fine-tuning methods and benchmark them to find the best performing model
+- Evaluate fine-tuned models on well-defined metrics for in-depth analysis
+
+<br>
+
+## 🌟 INT4 fine-tuning and generation with LLaMA LoRA
+
+We are excited to announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and generation integration. With this update, you can fine-tune LLMs like LLaMA with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This breakthrough significantly reduces memory requirements and accelerates the fine-tuning process, allowing you to achieve state-of-the-art performance with less computational resources.
+
+More information about INT4 fine-tuning and benchmarks can be found in the [INT4 README](examples/int4_finetuning/README.md).
+
+You can check out the [LLaMA INT4 fine-tuning example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
 
 <br>
 
 ## CLI playground
 <img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
 
 ## UI playground
 <img src=".github/ui-playground2.gif" width="100%" style="margin: 0 1%;"/>
 
+<br>
+
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
 
 <br>
 
@@ -295,30 +306,24 @@
 print("Generated output by the model: {}".format(output))
 ```
 
 You can find the data folder [here](examples/llama/alpaca_data).
 
 <br>
 
-
 ## 📚 Tutorials
 - [Preparing your dataset](examples/llama/preparing_your_dataset.py)
-- [Cerebras-GPT efficient fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
-- [Cerebras-GPT efficient fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
-- [LLaMA efficient fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
-- [LLaMA efficient fine-tuning with LoRA](examples/llama/llama_lora.py)
+- [Cerebras-GPT fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
+- [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
+- [LLaMA fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
+- [LLaMA fine-tuning with LoRA](examples/llama/llama_lora.py)
 - [LLaMA fine-tuning](examples/llama/llama.py)
-- [GPT-J efficient fine-tuning with LoRA and INT8](examples/gptj/gptj_lora_int8.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing)
-- [GPT-J efficient fine-tuning with LoRA](examples/gptj/gptj_lora.py)
-- [Galactica efficient fine-tuning with LoRA and INT8](examples/galactica/galactica_lora_int8.py)
-- [Galactica efficient fine-tuning with LoRA](examples/galactica/galactica_lora.py)
-- [OPT efficient fine-tuning with LoRA and INT8](examples/opt/opt_lora_int8.py)
-- [OPT efficient fine-tuning with LoRA](examples/opt/opt_lora.py)
-- [GPT-2 efficient fine-tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
-
+- [GPT-J fine-tuning with LoRA and INT8](examples/gptj/gptj_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hB_8s1V9K4IzifmlmN2AovGEJzTB1c7e?usp=sharing)
+- [GPT-J fine-tuning with LoRA](examples/gptj/gptj_lora.py)
+- [GPT-2 fine-tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
 
 <br>
 
 ## 📊 Performance
 
 Here is a comparison for the performance of different fine-tuning techniques on the LLaMA 7B model. We use the [Alpaca dataset](examples/llama/alpaca_data/) for fine-tuning. The dataset contains 52K instructions.
 
@@ -337,16 +342,17 @@
 
 |      LLaMA 7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
 | --------- | ---- | ---- | ---- |
 | GPU | 33.5 GB | 23.7 GB | 21.9 GB |
 | CPU | 190 GB  | 10.2 GB | 14.9 GB |
 | Time per epoch | 21 hours  | 20 mins | 20 mins |
 
-Please submit your performance results on other GPUs.
-<br >
+Contribute to this by submitting your performance results on other GPUs by creating an issue with your hardware specifications, memory consumption and time per epoch.
+
+<br>
 
 ## 📎 Fine-tuned model checkpoints
 We have already fine-tuned some models that you can use as your base or start playing with.
 Here is how you would load them:
 
 ```python
 from xturing.models import BaseModel
@@ -354,21 +360,25 @@
 ```
 
 | model               | dataset | Path          |
 |---------------------|--------|---------------|
 | DistilGPT-2 LoRA | alpaca | `x/distilgpt2_lora_finetuned_alpaca` |
 | LLaMA LoRA          | alpaca | `x/llama_lora_finetuned_alpaca` |
 
+<br>
+
 ## 📈 Roadmap
 - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
 - [x] Dataset generation using self-instruction
-- [x] 2x more memory-efficient fine-tuning vs LoRA and unsupervised fine-tuning
+- [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
-- [x] Supports OpenAI, Cohere and AI21 Studio model APIs for dataset generation
+- [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
+- [x] INT4 LLaMA LoRA fine-tuning demo
+- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation 
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.0.9/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.0/src/xturing.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 src/xturing/engines/opt_engine.py
 src/xturing/engines/gptj_utils/__init__.py
 src/xturing/engines/gptj_utils/gptj.py
 src/xturing/engines/llama_utils/__init__.py
 src/xturing/engines/llama_utils/llama.py
 src/xturing/engines/lora_engine/__init__.py
 src/xturing/engines/lora_engine/lora.py
+src/xturing/engines/lora_engine/save_and_load.py
+src/xturing/engines/lora_engine/test.py
+src/xturing/engines/quant_utils/__init__.py
+src/xturing/engines/quant_utils/custom_autotune.py
+src/xturing/engines/quant_utils/quant.py
 src/xturing/model_apis/__init__.py
 src/xturing/model_apis/ai21.py
 src/xturing/model_apis/base.py
 src/xturing/model_apis/cohere.py
 src/xturing/model_apis/openai.py
 src/xturing/models/__init__.py
 src/xturing/models/base.py
```

