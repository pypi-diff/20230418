# Comparing `tmp/curated-transformers-0.0.6.tar.gz` & `tmp/curated-transformers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-0.0.6.tar", last modified: Wed Mar 22 10:58:02 2023, max compression
+gzip compressed data, was "curated-transformers-0.0.7.tar", last modified: Tue Apr 18 10:23:30 2023, max compression
```

## Comparing `curated-transformers-0.0.6.tar` & `curated-transformers-0.0.7.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.765108 curated-transformers-0.0.6/
--rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-03-22 10:58:02.765108 curated-transformers-0.0.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.737108 curated-transformers-0.0.6/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.741108 curated-transformers-0.0.6/curated_transformers/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/cli/quantize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4888 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.745108 curated-transformers-0.0.6/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24143 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1206 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4102 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/output.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pooling.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.745108 curated-transformers-0.0.6/curated_transformers/models/pytorch/
--rw-r--r--   0 vsts      (1001) docker     (122)      221 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/activations.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.749108 curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2383 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      894 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2007 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/attention.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.749108 curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1739 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4795 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1182 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/curated_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      890 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10982 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/hf_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)      487 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/linear.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.749108 curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1781 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1882 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/pytorch/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4650 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.753108 curated-transformers-0.0.6/curated_transformers/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17281 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/pipeline/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.753108 curated-transformers-0.0.6/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.757108 curated-transformers-0.0.6/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3052 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4032 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1381 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6086 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3152 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4286 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.757108 curated-transformers-0.0.6/curated_transformers/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17278 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/pipeline/toy-en-corpus.spacy
--rw-r--r--   0 vsts      (1001) docker     (122)      406 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)      727 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.761108 curated-transformers-0.0.6/curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3233 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3924 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2601 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7523 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4423 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy-chars.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (122)      193 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.765108 curated-transformers-0.0.6/curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3612 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3823 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/curated_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 10:58:02.737108 curated-transformers-0.0.6/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-03-22 10:58:02.000000 curated-transformers-0.0.6/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4189 2023-03-22 10:58:02.000000 curated-transformers-0.0.6/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 10:58:02.000000 curated-transformers-0.0.6/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-03-22 10:58:02.000000 curated-transformers-0.0.6/curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-03-22 10:58:02.000000 curated-transformers-0.0.6/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-03-22 10:58:02.000000 curated-transformers-0.0.6/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 10:58:02.000000 curated-transformers-0.0.6/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-03-22 10:58:02.765108 curated-transformers-0.0.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-03-22 10:56:00.000000 curated-transformers-0.0.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.034464 curated-transformers-0.0.7/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.034464 curated-transformers-0.0.7/curated_transformers/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/cli/debug_pieces.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/cli/quantize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.038464 curated-transformers-0.0.7/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24143 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1206 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4102 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/output.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pooling.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.042464 curated-transformers-0.0.7/curated_transformers/models/pytorch/
+-rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/activations.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.042464 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2364 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2259 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/attention.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.042464 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1739 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4775 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/layer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1240 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/curated_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      890 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10982 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/hf_util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.046464 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1781 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1882 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/remove_eos_bos.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4650 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.046464 curated-transformers-0.0.7/curated_transformers/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17281 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/pipeline/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.046464 curated-transformers-0.0.7/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.050464 curated-transformers-0.0.7/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3207 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4550 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1419 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6139 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3176 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4313 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.050464 curated-transformers-0.0.7/curated_transformers/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17306 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/pipeline/test_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/pipeline/toy-en-corpus.spacy
+-rw-r--r--   0 vsts      (1001) docker     (122)      406 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/test_torchscript_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.054464 curated-transformers-0.0.7/curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2737 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7925 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4819 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_xlmr_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-chars.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3612 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_adapters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3823 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.034464 curated-transformers-0.0.7/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4184 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/setup.py
```

### Comparing `curated-transformers-0.0.6/LICENSE` & `curated-transformers-0.0.7/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (C) 2021 ExplosionAI GmbH
+Copyright (C) 2021-2023 ExplosionAI GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `curated-transformers-0.0.6/PKG-INFO` & `curated-transformers-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -33,13 +33,13 @@
 
 This package is experimental and it is possible that the models will still
 change in incompatible ways.
 
 ## ⏳ Install
 
 ```bash
-pip install git+https://github.com/explosion/curated-transformers.git
+pip install curated-transformers
 ```
 
 ## 🚀 Quickstart
 
 An example project is provided in the [`project`](project) directory.
```

### Comparing `curated-transformers-0.0.6/README.md` & `curated-transformers-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 
 This package is experimental and it is possible that the models will still
 change in incompatible ways.
 
 ## ⏳ Install
 
 ```bash
-pip install git+https://github.com/explosion/curated-transformers.git
+pip install curated-transformers
 ```
 
 ## 🚀 Quickstart
 
 An example project is provided in the [`project`](project) directory.
```

### Comparing `curated-transformers-0.0.6/curated_transformers/_compat.py` & `curated-transformers-0.0.7/curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/cli/debug_pieces.py` & `curated-transformers-0.0.7/curated_transformers/cli/debug_pieces.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/cli/quantize.py` & `curated-transformers-0.0.7/curated_transformers/cli/quantize.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/errors.py` & `curated-transformers-0.0.7/curated_transformers/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,14 @@
     E002 = ("The number of hidden layers ({num_hidden_layers}) in the "
             "ALBERT encoder must be divisable by number of hidden groups "
             "({num_hidden_groups})")
     E003 = ("The hidden width of the transformer ({hidden_width}) must be "
             "divisible by the number of self-attention heads ({num_heads})")
     E004 = ("The point-wise feed-forward network in the transformer only "
             "supports the following activation functions: {activation_funcs}")
-    E005 = ("Expected the attention mask to be of dtype 'torch.bool' but "
-            "found it be '{dtype}' instead")
-    E006 = ("The attention mask must be a 2D-tensor of shape [batch, seq_len]")
     E007 = ("Attempting to load the weights of an unsupported Hugging "
             "Face `transformers` model ({unsupported_model}). Currently "
             "supported models: {supported_models}")
     E008 = ("The number of layers in the scalar weighting listener model ({num_layers_scalar_weight})"
             "needs to be the same as the number of hidden layers in the "
             "transformer ({num_layers_transformer}). You can use the config's "
             "interpolation functionality to link the former's `num_layers` "
```

### Comparing `curated-transformers-0.0.6/curated_transformers/models/architectures.py` & `curated-transformers-0.0.7/curated_transformers/models/architectures.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/hf_loader.py` & `curated-transformers-0.0.7/curated_transformers/models/hf_loader.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/listeners.py` & `curated-transformers-0.0.7/curated_transformers/models/listeners.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/output.py` & `curated-transformers-0.0.7/curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pooling.py` & `curated-transformers-0.0.7/curated_transformers/models/pooling.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/activations.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/config.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/encoder.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/encoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,16 +59,15 @@
 
         embeddings = self.embeddings(input_ids, token_type_ids, None)
         layer_output = embeddings
 
         layers_per_group = self.num_hidden_layers // len(self.groups)
 
         layer_outputs = []
-        for i in range(self.num_hidden_layers):
-            layer_output = self.groups[i // layers_per_group](
-                layer_output, attn_mask=attention_mask
-            )
-            layer_outputs.append(layer_output)
+        for group in self.groups:
+            for _ in range(layers_per_group):
+                layer_output = group(layer_output, attn_mask=attention_mask)
+                layer_outputs.append(layer_output)
 
         return PyTorchTransformerOutput(
             embedding_output=embeddings, layer_hidden_states=layer_outputs
         )
```

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/albert/layer_group.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/layer_group.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from torch import Tensor
 from torch.nn import Module, ModuleList
 
+from ..attention import AttentionMask
 from ..bert.config import BertAttentionConfig
 from ..bert.layer import BertAttentionConfig, BertEncoderLayer
 from .config import AlbertLayerConfig
 
 
 class AlbertLayerGroup(Module):
     def __init__(
@@ -15,16 +16,16 @@
         self.group_layers = ModuleList(
             [
                 BertEncoderLayer(layer_config, attention_config)
                 for _ in range(layer_config.inner_group_num)
             ]
         )
 
-    def forward(self, input: Tensor, **kwargs) -> Tensor:
+    def forward(self, input: Tensor, attn_mask: AttentionMask) -> Tensor:
         """
         Shapes:
             input - (batch, seq_len, width)
         """
         layer_output = input
         for layer in self.group_layers:
-            layer_output = layer(layer_output, **kwargs)
+            layer_output = layer(layer_output, attn_mask)
         return layer_output
```

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/attention.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/attention.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-from typing import Optional, Tuple
-from dataclasses import dataclass
+from typing import Optional
 import math
 import torch
 from torch import Tensor
 from torch.nn import Module
 
 from ...errors import Errors
 
 
-@dataclass
 class AttentionMask:
     bool_mask: Tensor
-    _logit_mask: Optional[Tensor] = None
+    _logit_mask: Optional[Tensor]
 
-    def __post_init__(self):
-        if self.bool_mask.dtype != torch.bool:
-            raise ValueError(Errors.E005.format(dtype=self.bool_mask.dtype))
+    def __init__(self, bool_mask: Tensor):
+        if bool_mask.dtype != torch.bool:
+            raise ValueError("Expected the attention mask to be of dtype 'torch.bool'")
+        self.bool_mask = bool_mask
+        self._logit_mask = torch.jit.annotate(Optional[Tensor], None)
 
     @property
     def logit_mask(self) -> Tensor:
         if self._logit_mask is None:
             # The value is `torch.finfo(attn_scores.dype).min`. Unfortunately,
             # we cannot use `torch.finfo` in TorchScript.
             self._logit_mask = (1.0 - self.bool_mask.int()) * -3.4028234663852886e38
-        return self._logit_mask
+
+        # Narrow type for TorchScript.
+        logit_mask = self._logit_mask
+        assert logit_mask is not None
+        return logit_mask
 
     def dim(self) -> int:
         return self.bool_mask.dim()
 
     @property
-    def shape(self) -> Tuple:
+    def shape(self):
         return self.bool_mask.shape
 
 
 # https://www.tensorflow.org/text/tutorials/transformer#scaled_dot_product_attention
 class ScaledDotProductAttention(Module):
     def __init__(self, *, dropout_prob: float = 0.1):
         super().__init__()
@@ -45,15 +49,17 @@
         """
         Shapes:
             k, q, v - (batch, heads, seq_len, width)
             attn_mask - (batch, seq_len)
         """
 
         if attn_mask.dim() != 2:
-            raise ValueError(Errors.E006)
+            raise ValueError(
+                "The attention mask must be a 2D-tensor of shape [batch, seq_len]"
+            )
 
         model_dim = k.shape[-1]
         attn_scores = q @ k.transpose(-2, -1)
         attn_scores /= math.sqrt(model_dim)
 
         # Replace tokens that we don't want to attend to with a large
         # negative value to zero them out during softmax normalization.
```

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/config.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/embeddings.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/encoder.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/bert/layer.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import torch
-from torch.nn import Module
+from torch.nn import Linear, Module
 from torch import Tensor
 
 from .. import GeluNew
 from ..attention import AttentionMask, ScaledDotProductAttention
 from .config import BertAttentionConfig, BertLayerConfig
-from ..linear import Linear
 from ....errors import Errors
 
 
 # https://www.tensorflow.org/text/tutorials/transformer#multi-head_attention
 class BertSelfAttention(Module):
     def __init__(self, config: BertAttentionConfig):
         super().__init__()
```

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/curated_transformer.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/curated_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 CuratedEncoderT = TypeVar("CuratedEncoderT", AlbertEncoder, BertEncoder, RobertaEncoder)
 
 
 class CuratedTransformer(Generic[CuratedEncoderT], Module):
     """Simple wrapper for encoders. Currently only used to add a predictable
     prefix (curated_encoder) to encoders."""
 
-    curated_encoder: CuratedEncoderT
-
-    __slots__ = ["curated_encoder"]
-
     def __init__(self, encoder: CuratedEncoderT) -> None:
         super().__init__()
-        self.curated_encoder = encoder
+
+        # Type ignore, because TorchScript does not allow Module
+        # as a class variable type.
+        self.curated_encoder = encoder  # type: ignore[var-annotated]
 
     def forward(
         self,
         input_ids: Tensor,
         attention_mask: Optional[AttentionMask] = None,
         token_type_ids: Optional[Tensor] = None,
     ) -> PyTorchTransformerOutput:
```

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/embeddings.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/hf_util.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/hf_util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/config.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/embeddings.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/roberta/encoder.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/pytorch/scalar_weight.py` & `curated-transformers-0.0.7/curated_transformers/models/pytorch/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/remove_eos_bos.py` & `curated-transformers-0.0.7/curated_transformers/models/remove_eos_bos.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/scalar_weight.py` & `curated-transformers-0.0.7/curated_transformers/models/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/types.py` & `curated-transformers-0.0.7/curated_transformers/models/types.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/with_non_ws_tokens.py` & `curated-transformers-0.0.7/curated_transformers/models/with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/models/with_strided_spans.py` & `curated-transformers-0.0.7/curated_transformers/models/with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/pipeline/transformer.py` & `curated-transformers-0.0.7/curated_transformers/pipeline/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/conftest.py` & `curated-transformers-0.0.7/curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/models/test_hf_model.py` & `curated-transformers-0.0.7/curated_transformers/tests/models/test_hf_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import Callable
 from dataclasses import dataclass
 import pytest
-import torch
+from thinc.api import get_torch_default_device
 from torch.nn import Module
 
 from curated_transformers._compat import has_hf_transformers, transformers
 from curated_transformers.models.architectures import _pytorch_encoder
 from curated_transformers.models.hf_loader import build_hf_transformer_encoder_loader_v1
 from curated_transformers.models.pytorch.albert import AlbertEncoder
 from curated_transformers.models.pytorch.albert.config import AlbertConfig
 from curated_transformers.models.pytorch.attention import AttentionMask
 from curated_transformers.models.pytorch.bert import BertConfig, BertEncoder
 from curated_transformers.models.pytorch.roberta.config import RobertaConfig
 from curated_transformers.models.pytorch.roberta.encoder import RobertaEncoder
 
+from ..util import torch_assertclose
+
 
 @dataclass
 class ModelConfig:
     config: BertConfig
     encoder: Callable[[BertConfig], Module]
     hf_model_name: str
 
@@ -45,38 +47,44 @@
     assert model
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("model_config", TEST_MODELS)
 def test_model_against_hf_transformers(model_config):
+    torch_device = get_torch_default_device()
+
     model = encoder_from_config(model_config)
     model.initialize()
     encoder = model.shims[0]._model
     encoder.eval()
-    hf_encoder = transformers.AutoModel.from_pretrained(model_config.hf_model_name)
+    hf_encoder = transformers.AutoModel.from_pretrained(model_config.hf_model_name).to(
+        torch_device
+    )
     hf_encoder.eval()
 
     hf_tokenizer = transformers.AutoTokenizer.from_pretrained(
         model_config.hf_model_name
     )
     tokenization = hf_tokenizer(
         ["This is a test.", "Let's match outputs"], padding=True, return_tensors="pt"
-    )
+    ).to(torch_device)
     X = tokenization["input_ids"]
     attention_mask = tokenization["attention_mask"]
 
     # Test with the tokenizer's attention mask
     Y_encoder = encoder(
         X, attention_mask=AttentionMask(bool_mask=attention_mask.bool())
     )
     Y_hf_encoder = hf_encoder(X, attention_mask=attention_mask)
 
-    assert torch.allclose(
-        Y_encoder.last_hidden_layer_states, Y_hf_encoder.last_hidden_state, atol=1e-6
+    torch_assertclose(
+        Y_encoder.last_hidden_layer_states,
+        Y_hf_encoder.last_hidden_state,
     )
 
     # Try to infer the attention mask from padding.
     Y_encoder = encoder(X)
-    assert torch.allclose(
-        Y_encoder.last_hidden_layer_states, Y_hf_encoder.last_hidden_state, atol=1e-6
+    torch_assertclose(
+        Y_encoder.last_hidden_layer_states,
+        Y_hf_encoder.last_hidden_state,
     )
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/models/test_listeners.py` & `curated-transformers-0.0.7/curated_transformers/tests/models/test_listeners.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/models/test_pooling.py` & `curated-transformers-0.0.7/curated_transformers/tests/models/test_pooling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from thinc.api import Ragged, reduce_sum
+from thinc.api import Ragged, reduce_sum, NumpyOps
+from thinc.util import convert_recursive, is_cupy_array
 
 from curated_transformers.models.pooling import (
     with_ragged_last_layer,
     with_ragged_layers,
 )
 
 
@@ -14,46 +15,52 @@
         Ragged(ops.asarray1f([1.0, 2.0, 3.0]), lengths=ops.asarray1i([1, 2])),
         Ragged(ops.asarray1f([4.0, 5.0, 6.0]), lengths=ops.asarray1i([2, 1])),
         Ragged(ops.asarray1f([]), lengths=ops.asarray1i([])),
     ]
 
     Y, backprop = pooler(docs, is_train=True)
 
-    ops.xp.testing.assert_equal(
+    for y, y_h in zip(
         Y,
         [
             ops.asarray2f([[1.0], [5.0]]),
             ops.asarray2f([[9.0], [6.0]]),
             ops.asarray2f([]).reshape(0, 1),
         ],
-    )
+    ):
+        ops.xp.testing.assert_array_equal(y, y_h)
 
     dX = backprop(
         [
             ops.asarray2f([[1.0], [-1.0]]),
             ops.asarray2f([[-1.0], [1.0]]),
             ops.asarray2f([]).reshape(0, 1),
         ],
     )
 
     assert len(dX) == 3
 
-    ops.xp.testing.assert_equal(dX[0].dataXd, ops.asarray2f([[1.0], [-1.0], [-1.0]]))
-    ops.xp.testing.assert_equal(dX[0].lengths, ops.asarray1i([1, 2]))
+    ops.xp.testing.assert_array_equal(
+        dX[0].dataXd, ops.asarray2f([[1.0], [-1.0], [-1.0]])
+    )
+    ops.xp.testing.assert_array_equal(dX[0].lengths, ops.asarray1i([1, 2]))
 
-    ops.xp.testing.assert_equal(dX[1].dataXd, ops.asarray2f([[-1.0], [-1.0], [1.0]]))
-    ops.xp.testing.assert_equal(dX[1].lengths, ops.asarray1i([2, 1]))
+    ops.xp.testing.assert_array_equal(
+        dX[1].dataXd, ops.asarray2f([[-1.0], [-1.0], [1.0]])
+    )
+    ops.xp.testing.assert_array_equal(dX[1].lengths, ops.asarray1i([2, 1]))
 
-    ops.xp.testing.assert_equal(dX[2].dataXd, ops.asarray2f([]).reshape(0, 1))
-    ops.xp.testing.assert_equal(dX[2].lengths, ops.asarray1i([]))
+    ops.xp.testing.assert_array_equal(dX[2].dataXd, ops.asarray2f([]).reshape(0, 1))
+    ops.xp.testing.assert_array_equal(dX[2].lengths, ops.asarray1i([]))
 
 
 def test_with_ragged_layers():
     pooler = with_ragged_layers(reduce_sum())
     ops = pooler.ops
+    numpy = NumpyOps().xp
 
     docs = [
         [
             Ragged(ops.asarray1f([1.0, 2.0, 3.0]), lengths=ops.asarray1i([1, 2])),
             Ragged(ops.asarray1f([3.0, 2.0, 1.0]), lengths=ops.asarray1i([1, 2])),
         ],
         [
@@ -63,29 +70,32 @@
         [
             Ragged(ops.asarray1f([]), lengths=ops.asarray1i([])),
             Ragged(ops.asarray1f([]), lengths=ops.asarray1i([])),
         ],
     ]
 
     Y, backprop = pooler(docs, is_train=True)
+    # Since cupy balks at comparing sequences that mix CPU lists and GPU arrays,
+    # we'll need to convert them to numpy (CPU) arrays first.
+    Y = convert_recursive(is_cupy_array, lambda a: a.get(), Y)
 
-    ops.xp.testing.assert_equal(
+    numpy.testing.assert_equal(
         Y,
         [
             [
-                ops.asarray2f([[1.0], [5.0]]),
-                ops.asarray2f([[3.0], [3.0]]),
+                numpy.array([[1.0], [5.0]]),
+                numpy.array([[3.0], [3.0]]),
             ],
             [
-                ops.asarray2f([[9.0], [6.0]]),
-                ops.asarray2f([[11.0], [4.0]]),
+                numpy.array([[9.0], [6.0]]),
+                numpy.array([[11.0], [4.0]]),
             ],
             [
-                ops.asarray2f([]).reshape(0, 1),
-                ops.asarray2f([]).reshape(0, 1),
+                numpy.array([]).reshape(0, 1),
+                numpy.array([]).reshape(0, 1),
             ],
         ],
     )
 
     dX = backprop(
         [
             [
@@ -102,23 +112,31 @@
             ],
         ],
     )
 
     assert len(dX) == 3
 
     assert len(dX[0]) == 2
-    ops.xp.testing.assert_equal(dX[0][0].dataXd, ops.asarray2f([[1.0], [-1.0], [-1.0]]))
-    ops.xp.testing.assert_equal(dX[0][0].lengths, ops.asarray1i([1, 2]))
-    ops.xp.testing.assert_equal(dX[0][1].dataXd, ops.asarray2f([[2.0], [-2.0], [-2.0]]))
-    ops.xp.testing.assert_equal(dX[0][1].lengths, ops.asarray1i([1, 2]))
+    ops.xp.testing.assert_array_equal(
+        dX[0][0].dataXd, ops.asarray2f([[1.0], [-1.0], [-1.0]])
+    )
+    ops.xp.testing.assert_array_equal(dX[0][0].lengths, ops.asarray1i([1, 2]))
+    ops.xp.testing.assert_array_equal(
+        dX[0][1].dataXd, ops.asarray2f([[2.0], [-2.0], [-2.0]])
+    )
+    ops.xp.testing.assert_array_equal(dX[0][1].lengths, ops.asarray1i([1, 2]))
 
     assert len(dX[1]) == 2
-    ops.xp.testing.assert_equal(dX[1][0].dataXd, ops.asarray2f([[-1.0], [-1.0], [1.0]]))
-    ops.xp.testing.assert_equal(dX[1][1].dataXd, ops.asarray2f([[-2.0], [-2.0], [2.0]]))
-    ops.xp.testing.assert_equal(dX[1][0].lengths, ops.asarray1i([2, 1]))
-    ops.xp.testing.assert_equal(dX[1][1].lengths, ops.asarray1i([2, 1]))
+    ops.xp.testing.assert_array_equal(
+        dX[1][0].dataXd, ops.asarray2f([[-1.0], [-1.0], [1.0]])
+    )
+    ops.xp.testing.assert_array_equal(
+        dX[1][1].dataXd, ops.asarray2f([[-2.0], [-2.0], [2.0]])
+    )
+    ops.xp.testing.assert_array_equal(dX[1][0].lengths, ops.asarray1i([2, 1]))
+    ops.xp.testing.assert_array_equal(dX[1][1].lengths, ops.asarray1i([2, 1]))
 
     assert len(dX[2]) == 2
-    ops.xp.testing.assert_equal(dX[2][0].dataXd, ops.asarray2f([]).reshape(0, 1))
-    ops.xp.testing.assert_equal(dX[2][1].dataXd, ops.asarray2f([]).reshape(0, 1))
-    ops.xp.testing.assert_equal(dX[2][0].lengths, ops.asarray1i([]))
-    ops.xp.testing.assert_equal(dX[2][1].lengths, ops.asarray1i([]))
+    ops.xp.testing.assert_array_equal(dX[2][0].dataXd, ops.asarray2f([]).reshape(0, 1))
+    ops.xp.testing.assert_array_equal(dX[2][1].dataXd, ops.asarray2f([]).reshape(0, 1))
+    ops.xp.testing.assert_array_equal(dX[2][0].lengths, ops.asarray1i([]))
+    ops.xp.testing.assert_array_equal(dX[2][1].lengths, ops.asarray1i([]))
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/models/test_scalar_weight.py` & `curated-transformers-0.0.7/curated_transformers/tests/models/test_scalar_weight.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from thinc.api import NumpyOps, Ragged
+from thinc.api import Ragged, get_current_ops
 import torch
 
 from curated_transformers.models.scalar_weight import build_scalar_weight_v1
 
 
 def test_scalar_weight_model():
-    ops = NumpyOps()
+    ops = get_current_ops()
     model = build_scalar_weight_v1(num_layers=2, dropout_prob=0.0)
 
     with torch.no_grad():
         model.shims[0]._model.layer_weights[0] = 1
         model.shims[0]._model.layer_weights[1] = 1
         model.shims[0]._model.layer_weights[2] = 1
 
@@ -24,32 +24,32 @@
             Ragged(ones.copy(), lens.copy()),
         ]
     ]
     Y = ops.alloc2f(15, 2) + (1.0 / 3.0) * 2
 
     Yh, backprop = model(X, is_train=True)
     assert len(Yh) == 1
-    ops.xp.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
         Yh[0].dataXd,
         Y,
     )
-    ops.xp.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
         Yh[0].lengths,
         lens,
     )
 
     dX = backprop(
         [Ragged(ones.copy(), lengths=lens.copy())],
     )
     dX_expected = ops.alloc2f(15, 2) + (1.0 / 3.0)
 
     assert len(dX) == 1
     assert len(dX[0]) == 3
     for dX_layer in dX[0]:
-        ops.xp.testing.assert_equal(
+        ops.xp.testing.assert_array_equal(
             dX_layer.dataXd,
             dX_expected,
         )
-        ops.xp.testing.assert_equal(
+        ops.xp.testing.assert_array_equal(
             dX_layer.lengths,
             lens,
         )
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/models/test_transformer_model.py` & `curated-transformers-0.0.7/curated_transformers/tests/models/test_transformer_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy
 import pytest
 from cutlery import SentencePieceProcessor
 from thinc.api import CupyOps, NumpyOps, Ragged, registry
 from thinc.compat import has_cupy
 
 from curated_transformers.models.architectures import (
     build_albert_transformer_model_v1,
@@ -59,17 +58,17 @@
     )
     model.initialize(X=sample_docs)
     Y, backprop = model(sample_docs, is_train=False)
     assert isinstance(Y, TransformerModelOutput)
     num_ouputs = Y.num_outputs
     Y = Y.last_hidden_layer_states
     assert len(Y) == 2
-    numpy.testing.assert_equal(Y[0].lengths, [1, 1, 1, 1, 1, 1, 2, 2])
+    model.ops.xp.testing.assert_array_equal(Y[0].lengths, [1, 1, 1, 1, 1, 1, 2, 2])
     assert Y[0].dataXd.shape == (10, hidden_width)
-    numpy.testing.assert_equal(Y[1].lengths, [1, 1, 1, 1, 2, 1, 2])
+    model.ops.xp.testing.assert_array_equal(Y[1].lengths, [1, 1, 1, 1, 2, 1, 2])
     assert Y[1].dataXd.shape == (9, hidden_width)
 
     # Backprop zeros to verify that backprop doesn't fail.
     dY = [
         [
             Ragged(
                 model.ops.alloc2f(10, 768),
@@ -107,17 +106,19 @@
     )
     model.initialize(X=sample_docs_with_spaces)
     Y, backprop = model(sample_docs_with_spaces, is_train=False)
     assert isinstance(Y, TransformerModelOutput)
     num_ouputs = Y.num_outputs
     Y = Y.last_hidden_layer_states
     assert len(Y) == 2
-    numpy.testing.assert_equal(Y[0].lengths, [1, 1, 1, 1, 1, 1, 1, 2, 2])
+    model.ops.xp.testing.assert_array_equal(Y[0].lengths, [1, 1, 1, 1, 1, 1, 1, 2, 2])
     assert Y[0].dataXd.shape == (11, hidden_width)
-    numpy.testing.assert_equal(Y[1].lengths, [1, 1, 1, 1, 1, 1, 2, 1, 2, 1])
+    model.ops.xp.testing.assert_array_equal(
+        Y[1].lengths, [1, 1, 1, 1, 1, 1, 2, 1, 2, 1]
+    )
     assert Y[1].dataXd.shape == (12, hidden_width)
 
     # Backprop zeros to verify that backprop doesn't fail.
     dY = [
         [
             Ragged(
                 model.ops.alloc2f(11, 768),
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/models/test_with_non_ws_tokens.py` & `curated-transformers-0.0.7/curated_transformers/tests/models/test_with_non_ws_tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,22 +38,22 @@
     )
     model.initialize()
     Y, backprop = model(sample_docs_with_spaces, is_train=True)
 
     yl0 = Y.all_outputs[0][0]
     y1_check = model.ops.xp.ones((15, 2))
     y1_check[6, :] = 0.0
-    model.ops.xp.testing.assert_equal(yl0.dataXd, y1_check)
+    model.ops.xp.testing.assert_array_equal(yl0.dataXd, y1_check)
 
     yl1 = Y.all_outputs[1][0]
     y2_check = model.ops.xp.ones((17, 2))
     y2_check[4, :] = 0.0
     y2_check[8, :] = 0.0
     y2_check[16, :] = 0.0
-    model.ops.xp.testing.assert_equal(yl1.dataXd, y2_check)
+    model.ops.xp.testing.assert_array_equal(yl1.dataXd, y2_check)
 
     dY = [
         [
             Ragged(
                 model.ops.xp.arange(float(yl0.dataXd.size)).reshape(yl0.dataXd.shape),
                 lengths=yl0.lengths,
             )
@@ -65,15 +65,15 @@
             )
         ],
     ]
 
     backprop(dY)
 
     transformer_dY = mock_transformer.attrs["last_dY"]
-    model.ops.xp.testing.assert_equal(
+    model.ops.xp.testing.assert_array_equal(
         transformer_dY[0][0].dataXd,
         [
             [0.0, 0.0],
             [0.0, 1.0],
             [2.0, 3.0],
             [4.0, 5.0],
             [6.0, 7.0],
@@ -86,15 +86,15 @@
             [22.0, 23.0],
             [24.0, 25.0],
             [26.0, 27.0],
             [28.0, 29.0],
             [0.0, 0.0],
         ],
     )
-    model.ops.xp.testing.assert_equal(
+    model.ops.xp.testing.assert_array_equal(
         transformer_dY[1][0].dataXd,
         [
             [0.0, 0.0],
             [0.0, 1.0],
             [2.0, 3.0],
             [4.0, 5.0],
             [6.0, 7.0],
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/models/test_with_strided_spans.py` & `curated-transformers-0.0.7/curated_transformers/tests/models/test_with_strided_spans.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 from curated_transformers.models.output import TransformerModelOutput
 import pytest
-from thinc.api import Model, NumpyOps, Ragged, with_array, chain
+from thinc.api import Model, get_current_ops, Ragged, with_array, chain
 from thinc.types import Floats2d
 
 from curated_transformers.models.with_strided_spans import with_strided_spans
 
 
 def relu_activation() -> Model[Floats2d, Floats2d]:
     def forward(model: Model, X: Floats2d, is_train: bool):
@@ -37,15 +37,15 @@
         )
 
     return Model("mock_transformer", forward)
 
 
 @pytest.mark.parametrize("batch_size", [1, 2, 3, 5])
 def test_with_strided_spans(batch_size):
-    ops = NumpyOps()
+    ops = get_current_ops()
     trf = chain(with_array(relu_activation()), _mock_transformer())
     model = with_strided_spans(trf, stride=4, window=4, batch_size=batch_size)
 
     zeros = ops.alloc2f(15, 5)
     ones = ops.alloc2f(15, 5) + 1
     fives = ops.alloc2f(15, 5) + 5
 
@@ -82,27 +82,27 @@
         ops.xp.testing.assert_array_equal(Y[i][0].data, zeros)
         ops.xp.testing.assert_array_equal(Y[i][0].lengths, lengths2)
         ops.xp.testing.assert_array_equal(dX[i].data, zeros)
         ops.xp.testing.assert_array_equal(dX[i].lengths, lengths2)
 
 
 def test_with_strided_spans_averaging():
-    ops = NumpyOps()
+    ops = get_current_ops()
     stateful = chain(with_array(_add_range()), _mock_transformer())
     model = with_strided_spans(stateful, stride=2, window=4)
 
     data = ops.xp.zeros((6, 2))
     lengths = ops.asarray1i([3, 3])
     X = [Ragged(data, lengths=lengths)]
 
     model.initialize(X)
 
     Y, backprop = model(X, is_train=False)
 
-    ops.xp.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
         Y.all_outputs[0][0].dataXd,
         [[0.0, 1.0], [2.0, 3.0], [6.0, 7.0], [8.0, 9.0], [14.0, 15.0], [16.0, 17.0]],
     )
 
     ones = data + 1
     dX = backprop(
         [
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/pipeline/test_transformer.py` & `curated-transformers-0.0.7/curated_transformers/tests/pipeline/test_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     build_hf_piece_encoder_loader_v1,
     build_xlmr_sentencepiece_encoder_v1,
 )
 from curated_transformers.pipeline.transformer import make_transformer
 from curated_transformers.util import create_gradual_transformer_unfreezing
 from curated_transformers._compat import has_hf_transformers, transformers
 
+from ..util import torch_assertclose
+
 
 cfg_string_last_layer_listener = """
     # LastTransformerLayerListener
 
     [nlp]
     lang = "en"
     pipeline = ["transformer","tagger"]
@@ -248,15 +250,15 @@
     hf_ids, attention_mask, lens = _hf_tokenize_per_token(hf_tokenizer, docs)
     hf_encoding = hf_model(hf_ids, attention_mask=attention_mask)
     docs = list(pipe.pipe(docs))
 
     for doc, hf_doc_encoding, encoding_len in zip(
         docs, hf_encoding.last_hidden_state, lens
     ):
-        torch.testing.assert_close(
+        torch_assertclose(
             hf_doc_encoding[:encoding_len][1:-1],
             torch.tensor(doc._.trf_data.last_hidden_layer_state.dataXd),
         )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
@@ -287,15 +289,15 @@
     hf_ids, attention_mask, lens = _hf_tokenize_per_token(hf_tokenizer, docs)
     hf_encoding = hf_model(hf_ids, attention_mask=attention_mask)
     docs = list(pipe.pipe(docs))
 
     for doc, hf_doc_encoding, encoding_len in zip(
         docs, hf_encoding.last_hidden_state, lens
     ):
-        torch.testing.assert_close(
+        torch_assertclose(
             hf_doc_encoding[:encoding_len][1:-1],
             torch.tensor(doc._.trf_data.last_hidden_layer_state.dataXd),
         )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
@@ -328,15 +330,15 @@
     )
     hf_encoding = hf_model(hf_ids, attention_mask=attention_mask)
     docs = list(pipe.pipe(docs))
 
     for doc, hf_doc_encoding, encoding_len in zip(
         docs, hf_encoding.last_hidden_state, lens
     ):
-        torch.testing.assert_close(
+        torch_assertclose(
             hf_doc_encoding[:encoding_len][1:-1],
             torch.tensor(doc._.trf_data.last_hidden_layer_state.dataXd),
         )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
@@ -367,15 +369,15 @@
     hf_ids, attention_mask, lens = _hf_tokenize_per_token(hf_tokenizer, docs)
     hf_encoding = hf_model(hf_ids, attention_mask=attention_mask)
     docs = list(pipe.pipe(docs))
 
     for doc, hf_doc_encoding, encoding_len in zip(
         docs, hf_encoding.last_hidden_state, lens
     ):
-        torch.testing.assert_close(
+        torch_assertclose(
             hf_doc_encoding[:encoding_len][1:-1],
             torch.tensor(doc._.trf_data.last_hidden_layer_state.dataXd),
         )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
@@ -407,15 +409,18 @@
         nlp.update(train_examples, sgd=optimizer, losses=losses)
 
     transformer_trained_params = get_transformer_params_sorted()
     for (old_param, old_vec), (new_param, new_vec) in zip(
         transformer_init_params, transformer_trained_params
     ):
         assert old_param == new_param
-        torch.testing.assert_close(old_vec, new_vec)
+        torch_assertclose(
+            old_vec,
+            new_vec,
+        )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_transformer_pipe_outputs():
     nlp = spacy.blank("en")
     model = build_xlmr_transformer_model_v1(
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/pipeline/toy-en-corpus.spacy` & `curated-transformers-0.0.7/curated_transformers/tests/pipeline/toy-en-corpus.spacy`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/test_torchscript_wrapper.py` & `curated-transformers-0.0.7/curated_transformers/tests/test_torchscript_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import numpy
 from torch.nn import Linear
 from thinc.layers import (
     PyTorchWrapper_v2,
     TorchScriptWrapper_v1,
     pytorch_to_torchscript_wrapper,
 )
+from thinc.api import get_array_module
 
 
 @pytest.mark.parametrize("nN,nI,nO", [(2, 3, 4)])
 def test_pytorch_script(nN, nI, nO):
-
     model = PyTorchWrapper_v2(Linear(nI, nO)).initialize()
 
     script_model = pytorch_to_torchscript_wrapper(model)
 
     X = numpy.random.randn(nN, nI).astype("f")
     Y = model.predict(X)
     Y_script = script_model.predict(X)
-    numpy.testing.assert_allclose(Y, Y_script)
+    xp = get_array_module(Y)
+    xp.testing.assert_array_equal(Y, Y_script)
 
     serialized = script_model.to_bytes()
     script_model2 = TorchScriptWrapper_v1()
     script_model2.from_bytes(serialized)
 
-    numpy.testing.assert_allclose(Y, script_model2.predict(X))
+    xp.testing.assert_array_equal(Y, script_model2.predict(X))
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_bbpe_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_bbpe_encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import numpy.testing
 import pytest
-from thinc.api import Ragged, registry
+from thinc.api import Ragged, registry, get_current_ops
 
 from curated_transformers.tokenization.bbpe_encoder import build_byte_bpe_encoder_v1
 from curated_transformers.tokenization.hf_loader import build_hf_piece_encoder_loader_v1
 from curated_transformers._compat import has_hf_transformers
 
 
 @pytest.fixture
@@ -60,34 +59,40 @@
 
 
 def _check_toy_encoder(encoding):
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 3, 1, 1, 6, 1, 1])
-    numpy.testing.assert_equal(
+    ops = get_current_ops()
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 3, 1, 1, 6, 1, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd,
         [0, 44, 997, 262, 305, 334, 79, 342, 262, 388, 79, 302, 70, 472, 72, 17, 2],
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 3, 1, 1, 2, 4, 3, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 3, 1, 1, 2, 4, 3, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd,
         [0, 55, 841, 321, 362, 579, 324, 294, 291, 494, 131, 106, 270, 307, 79, 17, 2],
     )
 
 
 def _check_roberta_base_encoder(encoding):
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops = get_current_ops()
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [0, 100, 794, 10, 1816, 19, 10, 27608, 4, 2]
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 2, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 2, 1, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd, [0, 5625, 52, 40, 3529, 181, 48344, 5749, 4, 2]
     )
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_char_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_char_encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import numpy
 import pytest
-from thinc.api import Ragged
+from thinc.api import Ragged, get_current_ops
 import spacy
 
 from curated_transformers.tokenization.char_encoder import (
     build_char_encoder_loader_v1,
     build_char_encoder_v1,
 )
 from curated_transformers.tokenization.hf_loader import build_hf_piece_encoder_loader_v1
@@ -12,44 +11,46 @@
     build_wordpiece_encoder_v1,
 )
 from curated_transformers.util import registry
 from curated_transformers._compat import has_fugashi, has_hf_transformers, has_sudachi
 
 
 def test_char_encoder(test_dir):
+    ops = get_current_ops()
     encoder = build_char_encoder_v1()
     encoder.init = build_char_encoder_loader_v1(path=test_dir / "toy-chars.txt")
     encoder.initialize()
 
     nlp = spacy.blank("nl")
     sample_docs = [nlp.make_doc("Zeeën van tijd."), nlp.make_doc("Geïnd geld")]
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 5, 3, 4, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[0].lengths, [1, 5, 3, 4, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [2, 56, 9, 9, 57, 18, 26, 5, 18, 24, 13, 14, 8, 1, 3]
     )
 
     assert isinstance(encoding[1], Ragged)
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 5, 4, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 5, 4, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd, [2, 37, 9, 1, 18, 8, 11, 9, 16, 8, 3]
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.skipif(not has_fugashi, reason="requires fugashi")
 @pytest.mark.skipif(not has_sudachi, reason="requires SudachiPy and SudachiDict-core")
 def test_char_encoder_hf_model():
+    ops = get_current_ops()
     encoder = build_char_encoder_v1()
     encoder.init = registry.model_loaders.get(
         "curated-transformers.HFPieceEncoderLoader.v1"
     )(name="cl-tohoku/bert-base-japanese-char-v2")
     encoder.initialize()
 
     nlp = spacy.blank("ja")
@@ -57,19 +58,21 @@
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 2, 1, 1, 1, 1])
-    numpy.testing.assert_equal(encoding[0].dataXd, [2, 2719, 2828, 4923, 882, 922, 3])
+    ops.xp.testing.assert_array_equal(encoding[0].lengths, [1, 2, 1, 1, 1, 1])
+    ops.xp.testing.assert_array_equal(
+        encoding[0].dataXd, [2, 2719, 2828, 4923, 882, 922, 3]
+    )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 2, 1, 1, 1, 2, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 2, 1, 1, 1, 2, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd, [2, 1583, 5159, 897, 3574, 889, 852, 925, 829, 3]
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.skipif(not has_fugashi, reason="requires fugashi")
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_registry.py` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_registry.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import numpy.testing
 import pytest
-from thinc.api import Ragged, registry
+from thinc.api import Ragged, registry, get_current_ops
 
 from curated_transformers.tokenization.sentencepiece_encoder import (
     build_sentencepiece_encoder_v1,
 )
 from curated_transformers.tokenization.hf_loader import build_hf_piece_encoder_loader_v1
 from curated_transformers._compat import has_hf_transformers
 
@@ -38,21 +37,24 @@
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 2, 2, 1])
-    numpy.testing.assert_equal(
+    ops = get_current_ops()
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 2, 2, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [1, 86, 24123, 9, 23039, 677, 9, 5500, 70819, 5, 4, 2]
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 2, 1, 2, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 2, 1, 2, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd, [1, 38395, 641, 1220, 73202, 159, 7663, 120323, 5, 4, 2]
     )
 
 
 def test_serialize(toy_encoder, sample_docs):
     encoder_bytes = toy_encoder.to_bytes()
     encoder2 = build_sentencepiece_encoder_v1()
@@ -62,19 +64,22 @@
 
 
 def _check_toy_encoder(encoding):
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 6, 2, 1])
-    numpy.testing.assert_equal(
+    ops = get_current_ops()
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 6, 2, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd,
         [1, 8, 465, 10, 947, 41, 10, 170, 168, 110, 28, 20, 143, 7, 4, 2],
     )
 
     assert isinstance(encoding[1], Ragged)
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 2, 1, 1, 1, 4, 3, 2, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 2, 1, 1, 1, 4, 3, 2, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd,
         [1, 483, 546, 112, 171, 567, 62, 20, 45, 0, 84, 115, 27, 7, 4, 2],
     )
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_wordpiece_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_wordpiece_encoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import numpy.testing
 import pytest
 import spacy
 from tempfile import TemporaryDirectory
-from thinc.api import Ragged
+from thinc.api import Ragged, get_current_ops
 
 from curated_transformers.tokenization.hf_loader import build_hf_piece_encoder_loader_v1
 from curated_transformers.tokenization.wordpiece_encoder import (
     build_bert_wordpiece_encoder_v1,
     build_wordpiece_encoder_v1,
     _bert_preprocess,
     build_wordpiece_encoder_loader_v1,
@@ -18,63 +17,70 @@
     encoding = wordpiece_toy_encoder.predict(sample_docs)
     _check_toy_encoder(encoding)
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_wordpiece_encoder_hf_model(sample_docs):
+    ops = get_current_ops()
     encoder = build_wordpiece_encoder_v1()
     encoder.init = build_hf_piece_encoder_loader_v1(name="bert-base-cased")
     encoder.initialize()
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [101, 146, 1486, 170, 1873, 1114, 170, 16737, 119, 102]
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 3, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 3, 1, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd,
         [101, 3570, 1195, 1209, 3940, 185, 5926, 2744, 7329, 119, 102],
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_wordpiece_encoder_hf_model_uncased(sample_docs):
+    ops = get_current_ops()
     encoder = build_wordpiece_encoder_v1()
     encoder.init = build_hf_piece_encoder_loader_v1(name="bert-base-uncased")
     encoder.initialize()
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [101, 1045, 2387, 1037, 2611, 2007, 1037, 12772, 1012, 102]
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd, [101, 2651, 2057, 2097, 4521, 26202, 4605, 1012, 102]
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_wordpiece_encoder_hf_model_german():
+    ops = get_current_ops()
     encoder = build_bert_wordpiece_encoder_v1()
     encoder.init = build_hf_piece_encoder_loader_v1(name="bert-base-german-cased")
     encoder.initialize()
 
     nlp = spacy.blank("de")
     sample_docs = [
         nlp.make_doc("Wir sehen ein AWO-Mitarbeiter."),
@@ -83,57 +89,61 @@
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 5, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[0].lengths, [1, 1, 1, 1, 5, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [3, 655, 2265, 39, 32, 26939, 26962, 26935, 2153, 26914, 4]
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 1, 5, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 1, 5, 1, 1, 1, 1, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd,
         [3, 125, 56, 26915, 26914, 26935, 130, 26914, 4490, 141, 1028, 26914, 4],
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_wordpiece_encoder_loader(sample_docs):
+    ops = get_current_ops()
     encoder = build_wordpiece_encoder_v1()
     hf_tokenizer = transformers.AutoTokenizer.from_pretrained("bert-base-cased")
     with TemporaryDirectory() as d:
         vocab_path = hf_tokenizer.save_vocabulary(d)[0]
         encoder.init = build_wordpiece_encoder_loader_v1(path=vocab_path)
         encoder.initialize()
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [101, 146, 1486, 170, 1873, 1114, 170, 16737, 119, 102]
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 3, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 3, 1, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd,
         [101, 3570, 1195, 1209, 3940, 185, 5926, 2744, 7329, 119, 102],
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_wordpiece_encoder_loader_uncased(sample_docs):
+    ops = get_current_ops()
     encoder = build_wordpiece_encoder_v1()
     hf_tokenizer = transformers.AutoTokenizer.from_pretrained("bert-base-uncased")
     with TemporaryDirectory() as d:
         vocab_path = hf_tokenizer.save_vocabulary(d)[0]
         encoder.init = build_wordpiece_encoder_loader_v1(
             path=vocab_path, lowercase=True, strip_accents=True
         )
@@ -141,21 +151,23 @@
 
     encoding = encoder.predict(sample_docs)
 
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd, [101, 1045, 2387, 1037, 2611, 2007, 1037, 12772, 1012, 102]
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 1, 1, 1, 1, 1, 1, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd, [101, 2651, 2057, 2097, 4521, 26202, 4605, 1012, 102]
     )
 
 
 def test_serialize(wordpiece_toy_encoder):
     encoder_bytes = wordpiece_toy_encoder.to_bytes()
     toy_encoder2 = build_wordpiece_encoder_v1()
@@ -187,22 +199,25 @@
     assert _bert_preprocess("AWO-") == ["AWO", "-"]
     assert _bert_preprocess("-") == ["-"]
     assert _bert_preprocess("") == []
     assert _bert_preprocess("Mw.-St.") == ["Mw", ".", "-", "St", "."]
 
 
 def _check_toy_encoder(encoding):
+    ops = get_current_ops()
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 3, 1, 1, 5, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 3, 1, 1, 5, 1, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd,
         [2, 41, 818, 61, 67, 193, 88, 204, 61, 251, 909, 682, 102, 95, 17, 3],
     )
 
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 3, 1, 1, 2, 3, 3, 1, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 3, 1, 1, 2, 3, 3, 1, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd,
         [2, 824, 98, 189, 311, 417, 65, 155, 503, 99, 1, 416, 117, 88, 17, 3],
     )
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/test_xlmr_adapter.py` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_xlmr_adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 from cutlery import SentencePieceProcessor
-import numpy.testing
 import pytest
-from thinc.api import NumpyOps, Ragged, chain, Model
+from thinc.api import Ragged, chain, Model, get_current_ops, NumpyOps
+from thinc.util import convert_recursive, is_cupy_array
 
 from curated_transformers._compat import has_hf_transformers, transformers
 from curated_transformers.tokenization.sentencepiece_encoder import (
     build_sentencepiece_encoder_v1,
     build_xlmr_sentencepiece_encoder_v1,
 )
 from curated_transformers.tokenization.sentencepiece_adapters import (
@@ -57,23 +57,30 @@
     encoder2 = empty_encoder
     encoder2.from_bytes(encoder_bytes)
     encoding = encoder2.predict(sample_docs)
     _check_encoder(encoding)
 
 
 def _compare_model_hf_output(ops, Y, Y_hf):
+    numpy = NumpyOps().xp
     # Get inputs, removing BOS/EOS from every token.
-    Y_hf = [e[1:-1] for e in Y_hf["input_ids"]]
-    numpy.testing.assert_equal(ops.unflatten(Y.dataXd, Y.lengths), Y_hf)
+    Y_hf = [numpy.array(e[1:-1]) for e in Y_hf["input_ids"]]
+
+    # Since cupy balks at comparing sequences that mix CPU lists and GPU arrays,
+    # we'll need to convert them to numpy (CPU) arrays first.
+    Y = convert_recursive(
+        is_cupy_array, lambda a: a.get(), ops.unflatten(Y.dataXd, Y.lengths)
+    )
+    numpy.testing.assert_equal(Y, Y_hf)
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_sentencepiece_encoder_against_hf(sample_docs):
-    ops = NumpyOps()
+    ops = get_current_ops()
 
     hf_tokenizer = transformers.AutoTokenizer.from_pretrained("xlm-roberta-base")
     encoder = build_sentencepiece_encoder_v1()
     encoder.init = build_hf_piece_encoder_loader_v1(name="xlm-roberta-base")
     encoder.initialize()
     model = chain(encoder, build_xlmr_adapter(), _mock_transformer(), remove_bos_eos())
 
@@ -84,15 +91,15 @@
     hf_encoding = hf_tokenizer([token.text for token in sample_docs[1]])
     _compare_model_hf_output(ops, encoding.all_outputs[1][0], hf_encoding)
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_wordpiece_encoder_against_hf(sample_docs):
-    ops = NumpyOps()
+    ops = get_current_ops()
     encoder = build_wordpiece_encoder_v1()
     encoder.init = build_hf_piece_encoder_loader_v1(name="bert-base-cased")
     encoder.initialize()
     hf_tokenizer = transformers.AutoTokenizer.from_pretrained("bert-base-cased")
     model = chain(encoder, _mock_transformer(), remove_bos_eos())
 
     encoding = model.predict(sample_docs)
@@ -104,19 +111,22 @@
 
 
 def _check_encoder(encoding):
     assert isinstance(encoding, list)
     assert len(encoding) == 2
 
     assert isinstance(encoding[0], Ragged)
-    numpy.testing.assert_equal(encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 6, 2, 1])
-    numpy.testing.assert_equal(
+    ops = get_current_ops()
+    ops.xp.testing.assert_array_equal(
+        encoding[0].lengths, [1, 1, 1, 1, 1, 1, 1, 6, 2, 1]
+    )
+    ops.xp.testing.assert_array_equal(
         encoding[0].dataXd,
         [0, 9, 466, 11, 948, 42, 11, 171, 169, 111, 29, 21, 144, 8, 5, 2],
     )
 
     assert isinstance(encoding[1], Ragged)
-    numpy.testing.assert_equal(encoding[1].lengths, [1, 2, 1, 1, 1, 4, 3, 2, 1])
-    numpy.testing.assert_equal(
+    ops.xp.testing.assert_array_equal(encoding[1].lengths, [1, 2, 1, 1, 1, 4, 3, 2, 1])
+    ops.xp.testing.assert_array_equal(
         encoding[1].dataXd,
         [0, 484, 547, 113, 172, 568, 63, 21, 46, 3, 85, 116, 28, 8, 5, 2],
     )
```

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy-merges.txt` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy-vocab.json` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy.model` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.model`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tests/tokenization/toy.wordpieces` & `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/__init__.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/bbpe_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/char_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/char_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/hf_loader.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/hf_loader.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/sentencepiece_adapters.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_adapters.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/sentencepiece_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/types.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/types.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/tokenization/wordpiece_encoder.py` & `curated-transformers-0.0.7/curated_transformers/tokenization/wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers/util.py` & `curated-transformers-0.0.7/curated_transformers/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-0.0.7/curated_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -33,13 +33,13 @@
 
 This package is experimental and it is possible that the models will still
 change in incompatible ways.
 
 ## ⏳ Install
 
 ```bash
-pip install git+https://github.com/explosion/curated-transformers.git
+pip install curated-transformers
 ```
 
 ## 🚀 Quickstart
 
 An example project is provided in the [`project`](project) directory.
```

### Comparing `curated-transformers-0.0.6/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-0.0.7/curated_transformers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 curated_transformers/models/with_strided_spans.py
 curated_transformers/models/pytorch/__init__.py
 curated_transformers/models/pytorch/activations.py
 curated_transformers/models/pytorch/attention.py
 curated_transformers/models/pytorch/curated_transformer.py
 curated_transformers/models/pytorch/embeddings.py
 curated_transformers/models/pytorch/hf_util.py
-curated_transformers/models/pytorch/linear.py
 curated_transformers/models/pytorch/scalar_weight.py
 curated_transformers/models/pytorch/albert/__init__.py
 curated_transformers/models/pytorch/albert/config.py
 curated_transformers/models/pytorch/albert/encoder.py
 curated_transformers/models/pytorch/albert/layer_group.py
 curated_transformers/models/pytorch/bert/__init__.py
 curated_transformers/models/pytorch/bert/config.py
@@ -50,14 +49,15 @@
 curated_transformers/models/pytorch/roberta/config.py
 curated_transformers/models/pytorch/roberta/embeddings.py
 curated_transformers/models/pytorch/roberta/encoder.py
 curated_transformers/pipeline/__init__.py
 curated_transformers/pipeline/transformer.py
 curated_transformers/tests/__init__.py
 curated_transformers/tests/conftest.py
+curated_transformers/tests/enable_gpu.py
 curated_transformers/tests/test_cli_app.py
 curated_transformers/tests/test_torchscript_wrapper.py
 curated_transformers/tests/util.py
 curated_transformers/tests/models/__init__.py
 curated_transformers/tests/models/test_hf_model.py
 curated_transformers/tests/models/test_listeners.py
 curated_transformers/tests/models/test_pooling.py
```

### Comparing `curated-transformers-0.0.6/curated_transformers.egg-info/entry_points.txt` & `curated-transformers-0.0.7/curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.6/setup.cfg` & `curated-transformers-0.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.6
+version = 0.0.7
 description = Curated transformer models
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
```

