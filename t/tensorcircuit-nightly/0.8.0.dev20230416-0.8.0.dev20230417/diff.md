# Comparing `tmp/tensorcircuit-nightly-0.8.0.dev20230416.tar.gz` & `tmp/tensorcircuit-nightly-0.8.0.dev20230417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230416.tar", last modified: Sun Apr 16 12:37:33 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230417.tar", last modified: Mon Apr 17 12:41:53 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.8.0.dev20230416.tar` & `tensorcircuit-nightly-0.8.0.dev20230417.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.150962 tensorcircuit-nightly-0.8.0.dev20230416/
--rw-r--r--   0 runner    (1001) docker     (122)    22872 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-16 12:37:33.150962 tensorcircuit-nightly-0.8.0.dev20230416/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.138962 tensorcircuit-nightly-0.8.0.dev20230416/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.142962 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27001 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-16 12:37:33.150962 tensorcircuit-nightly-0.8.0.dev20230416/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-16 12:37:28.000000 tensorcircuit-nightly-0.8.0.dev20230416/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.142962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-16 12:37:28.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.142962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.146962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14559 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36236 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.146962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17566 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.146962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29143 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.146962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     3580 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9975 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34398 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11878 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.146962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31378 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.146962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27351 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.146962 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-16 12:37:33.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-16 12:37:33.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-16 12:37:33.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-16 12:37:33.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-16 12:37:33.000000 tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 12:37:33.150962 tensorcircuit-nightly-0.8.0.dev20230416/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    45002 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    11359 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6597 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-16 12:15:30.000000 tensorcircuit-nightly-0.8.0.dev20230416/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/
+-rw-r--r--   0 runner    (1001) docker     (122)    22872 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.852855 tensorcircuit-nightly-0.8.0.dev20230417/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.856855 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27001 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-17 12:41:48.000000 tensorcircuit-nightly-0.8.0.dev20230417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.856855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-17 12:41:48.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14946 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36236 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17566 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29161 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3580 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9975 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34398 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11878 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.864855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31378 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.864855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27351 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.864855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45826 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11359 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/CHANGELOG.md` & `tensorcircuit-nightly-0.8.0.dev20230417/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/HISTORY.md` & `tensorcircuit-nightly-0.8.0.dev20230417/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/LICENSE` & `tensorcircuit-nightly-0.8.0.dev20230417/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230416
+Version: 0.8.0.dev20230417
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/README.md` & `tensorcircuit-nightly-0.8.0.dev20230417/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/README_cn.md` & `tensorcircuit-nightly-0.8.0.dev20230417/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/advance.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/cnconf.py` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/conf.py` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/contribution.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/faq.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/index.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/infras.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/modules.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/setup.py` & `tensorcircuit-nightly-0.8.0.dev20230417/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0.dev20230416"
+__version__ = "0.8.0.dev20230417"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .about import about
 from .cons import (
     backend,
     set_backend,
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/about.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/cupy_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # pylint: disable=invalid-name
 
 import logging
 import warnings
 from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import numpy as np
+import scipy
 
 try:  # old version tn compatiblity
     from tensornetwork.backends import base_backend
 
     tnbackend = base_backend.BaseBackend
 
 except ImportError:
@@ -58,14 +59,26 @@
         self: Any,
         a: Tensor,
         axis: Optional[Sequence[int]] = None,
         keepdims: bool = False,
     ) -> Tensor:
         return cp.sum(a, axis=axis, keepdims=keepdims)
 
+    def conj(self, tensor: Tensor) -> Tensor:
+        return tensor.conj()
+
+    def sign(self, tensor: Tensor) -> Tensor:
+        return cp.sign(tensor)
+
+    def multiply(self, tensor1: Tensor, tensor2: Tensor) -> Tensor:
+        return tensor1 * tensor2
+
+    def norm(self, tensor: Tensor) -> Tensor:
+        return cp.linalg.norm(tensor)
+
     def shape_tuple(self, tensor: Tensor) -> Tuple[int]:
         return tensor.shape  # type:ignore
 
     def tensordot(
         self, a: Tensor, b: Tensor, axes: Union[int, Sequence[Sequence[int]]]
     ) -> Tensor:
         return cp.tensordot(a, b, axes)
@@ -96,15 +109,15 @@
             dtype = dtypestr
         return cp.zeros(shape, dtype=dtype)
 
     def copy(self, a: Tensor) -> Tensor:
         return a.copy()
 
     def expm(self, a: Tensor) -> Tensor:
-        raise NotImplementedError
+        return self.convert_to_tensor(scipy.linalg.expm(self.numpy(a)))
 
     def abs(self, a: Tensor) -> Tensor:
         return cp.abs(a)
 
     def sin(self, a: Tensor) -> Tensor:
         return cp.sin(a)
 
@@ -303,15 +316,15 @@
         high: float = 1,
         dtype: str = "32",
     ) -> Tensor:
         if isinstance(dtype, str):
             dtype = dtype[-2:]
         if isinstance(shape, int):
             shape = (shape,)
-        r = g.uniform(low=low, high=high, size=shape)
+        r = g.random(shape) * (high - low) + low
         if dtype == "32":
             r = r.astype(np.float32)
         elif dtype == "64":
             r = r.astype(np.float64)
         elif not isinstance(dtype, str):
             r = r.astype(dtype)
         else:
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/gates.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,15 +808,15 @@
     :type unitary: Tensor
     :param theta: angle in radians
     :type theta: float
     :param name: suffix of Gate name
     :return: Exponential Gate
     :rtype: Gate
     """
-    theta = num_to_tensor(theta)
+    theta, unitary = num_to_tensor(theta, unitary)
     mat = backend.expm(-backend.i() * theta * unitary)
     dimension = reduce(mul, mat.shape)
     nolegs = int(np.log(dimension) / np.log(2))
     mat = backend.reshape(mat, shape=[2 for _ in range(nolegs)])
     return Gate(mat, name="exp-" + name)
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230416
+Version: 0.8.0.dev20230417
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/conftest.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,11 +45,23 @@
     except ImportError as e:
         print(e)
         tc.set_backend("numpy")
         pytest.skip("****** No torch backend found, skipping test suit *******")
 
 
 @pytest.fixture(scope="function")
+def cpb():
+    try:
+        tc.set_backend("cupy")
+        yield
+        tc.set_backend("numpy")
+    except ImportError as e:
+        print(e)
+        tc.set_backend("numpy")
+        pytest.skip("****** No cupy backend found, skipping test suit *******")
+
+
+@pytest.fixture(scope="function")
 def highp():
     tc.set_dtype("complex128")
     yield
     tc.set_dtype("complex64")
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_backends.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_calibrating.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_channels.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_circuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 thisfile = os.path.abspath(__file__)
 modulepath = os.path.dirname(os.path.dirname(thisfile))
 
 sys.path.insert(0, modulepath)
 import tensorcircuit as tc
 
 
-def test_wavefunction():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_wavefunction(backend):
     qc = tc.Circuit(2)
     qc.unitary(
         0,
         1,
         unitary=tc.gates.Gate(np.arange(16).reshape(2, 2, 2, 2).astype(np.complex64)),
     )
     assert np.real(qc.wavefunction()[2]) == 8
@@ -37,23 +38,25 @@
     qc.unitary(
         0, unitary=tc.gates.Gate(np.arange(4).reshape(2, 2).astype(np.complex64))
     )
     qc.wavefunction()
     assert np.real(qc.wavefunction()[2]) == 2
 
 
-def test_basics():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_basics(backend):
     c = tc.Circuit(2)
     c.x(0)
-    np.testing.assert_allclose(c.amplitude("10"), np.array(1.0))
+    np.testing.assert_allclose(tc.backend.numpy(c.amplitude("10")), np.array(1.0))
     c.CNOT(0, 1)
-    np.testing.assert_allclose(c.amplitude("11"), np.array(1.0))
+    np.testing.assert_allclose(tc.backend.numpy(c.amplitude("11")), np.array(1.0))
 
 
-def test_measure():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_measure(backend):
     c = tc.Circuit(3)
     c.H(0)
     c.h(1)
     c.toffoli(0, 1, 2)
     assert c.measure(2)[0] in [0, 1]
 
 
@@ -228,21 +231,24 @@
                 tc.backend.norm(f(jax.random.PRNGKey(23))), 1.0, atol=1e-4
             )
             np.testing.assert_allclose(
                 tc.backend.norm(f(jax.random.PRNGKey(24))), 1.0, atol=1e-4
             )
 
 
-def test_expectation():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_expectation(backend):
     c = tc.Circuit(2)
     c.H(0)
-    np.testing.assert_allclose(c.expectation((tc.gates.z(), [0])), 0, atol=1e-7)
+    np.testing.assert_allclose(
+        tc.backend.numpy(c.expectation((tc.gates.z(), [0]))), 0, atol=1e-7
+    )
 
 
-@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb")])
+@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("cpb")])
 def test_exp1(backend):
     @partial(tc.backend.jit, jit_compile=True)
     def sf():
         c = tc.Circuit(2)
         xx = np.array(
             [[0, 0, 0, 1], [0, 0, 1, 0], [0, 1, 0, 0], [1, 0, 0, 0]], dtype=np.complex64
         )
@@ -256,16 +262,16 @@
         xx = np.array(
             [[0, 0, 0, 1], [0, 0, 1, 0], [0, 1, 0, 0], [1, 0, 0, 0]], dtype=np.complex64
         )
         c.exp(0, 1, unitary=xx, theta=tc.num_to_tensor(0.2))
         s1 = c.state()
         return s1
 
-    s = sf()
-    s1 = s1f()
+    s = tc.backend.numpy(sf())
+    s1 = tc.backend.numpy(s1f())
     np.testing.assert_allclose(s, s1, atol=1e-4)
 
 
 def test_complex128(highp, tfb):
     c = tc.Circuit(2)
     c.H(1)
     c.rx(0, theta=tc.gates.num_to_tensor(1j))
@@ -312,58 +318,59 @@
 def test_single_qubit():
     c = tc.Circuit(1)
     c.H(0)
     w = c.state()[0]
     np.testing.assert_allclose(w, np.array([1, 1]) / np.sqrt(2), atol=1e-4)
 
 
-def test_expectation_between_two_states():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_expectation_between_two_states(backend):
     zp = np.array([1.0, 0.0])
     zd = np.array([0.0, 1.0])
     assert tc.expectation((tc.gates.y(), [0]), ket=zp, bra=zd) == 1j
 
     c = tc.Circuit(3)
     c.H(0)
     c.ry(1, theta=tc.num_to_tensor(0.8))
     c.cnot(1, 2)
 
     state = c.wavefunction()
     x1z2 = [(tc.gates.x(), [0]), (tc.gates.z(), [1])]
     e1 = c.expectation(*x1z2)
     e2 = tc.expectation(*x1z2, ket=state, bra=state, normalization=True)
-    np.testing.assert_allclose(e2, e1)
+    np.testing.assert_allclose(tc.backend.numpy(e2), tc.backend.numpy(e1))
 
     c = tc.Circuit(3)
     c.H(0)
     c.ry(1, theta=tc.num_to_tensor(0.8 + 0.7j))
     c.cnot(1, 2)
 
     state = c.wavefunction()
     x1z2 = [(tc.gates.x(), [0]), (tc.gates.z(), [1])]
     e1 = c.expectation(*x1z2) / tc.backend.norm(state) ** 2
     e2 = tc.expectation(*x1z2, ket=state, normalization=True)
-    np.testing.assert_allclose(e2, e1)
+    np.testing.assert_allclose(tc.backend.numpy(e2), tc.backend.numpy(e1))
 
     c = tc.Circuit(2)
     c.X(1)
     s1 = c.state()
     c2 = tc.Circuit(2)
     c2.X(0)
     s2 = c2.state()
     c3 = tc.Circuit(2)
     c3.H(1)
     s3 = c3.state()
     x1x2 = [(tc.gates.x(), [0]), (tc.gates.x(), [1])]
     e = tc.expectation(*x1x2, ket=s1, bra=s2)
-    np.testing.assert_allclose(e, 1.0)
+    np.testing.assert_allclose(tc.backend.numpy(e), 1.0)
     e2 = tc.expectation(*x1x2, ket=s3, bra=s2)
-    np.testing.assert_allclose(e2, 1.0 / np.sqrt(2))
+    np.testing.assert_allclose(tc.backend.numpy(e2), 1.0 / np.sqrt(2))
 
 
-@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb")])
+@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("cpb")])
 def test_any_inputs_state(backend):
     c = tc.Circuit(2, inputs=tc.array_to_tensor(np.array([0.0, 0.0, 0.0, 1.0])))
     c.X(0)
     z0 = c.expectation((tc.gates.z(), [0]))
     assert z0 == 1.0
     c = tc.Circuit(2, inputs=tc.array_to_tensor(np.array([0.0, 0.0, 1.0, 0.0])))
     c.X(0)
@@ -375,46 +382,50 @@
     assert z0 == -1.0
     c = tc.Circuit(
         2,
         inputs=tc.array_to_tensor(np.array([1 / np.sqrt(2), 0.0, 1 / np.sqrt(2), 0.0])),
     )
     c.X(0)
     z0 = c.expectation((tc.gates.z(), [0]))
-    np.testing.assert_allclose(z0, 0.0, rtol=1e-4, atol=1e-4)
+    np.testing.assert_allclose(tc.backend.numpy(z0), 0.0, rtol=1e-4, atol=1e-4)
 
 
-@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb")])
+@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("cpb")])
 def test_postselection(backend):
     c = tc.Circuit(3)
     c.H(1)
     c.H(2)
     c.mid_measurement(1, 1)
     c.mid_measurement(2, 1)
     s = c.wavefunction()
-    np.testing.assert_allclose(tc.backend.real(s[3]), 0.5)
+    np.testing.assert_allclose(tc.backend.numpy(s[3]).real, 0.5)
 
 
-def test_unitary():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_unitary(backend):
     c = tc.Circuit(2, inputs=np.eye(4))
     c.X(0)
     c.Y(1)
-    answer = np.kron(tc.gates.x().tensor, tc.gates.y().tensor)
-    np.testing.assert_allclose(c.wavefunction().reshape([4, 4]), answer, atol=1e-4)
+    answer = tc.backend.numpy(np.kron(tc.gates.x().tensor, tc.gates.y().tensor))
+    np.testing.assert_allclose(
+        tc.backend.numpy(c.wavefunction().reshape([4, 4])), answer, atol=1e-4
+    )
 
 
-def test_expectation_ps():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_expectation_ps(backend):
     c = tc.Circuit(2)
     c.X(0)
     r = c.expectation_ps(z=[0, 1])
-    np.testing.assert_allclose(r, -1, atol=1e-5)
+    np.testing.assert_allclose(tc.backend.numpy(r), -1, atol=1e-5)
 
     c = tc.Circuit(2)
     c.H(0)
     r = c.expectation_ps(z=[1], x=[0])
-    np.testing.assert_allclose(r, 1, atol=1e-5)
+    np.testing.assert_allclose(tc.backend.numpy(r), 1, atol=1e-5)
 
 
 def test_probability():
     for c_cls in [tc.Circuit, tc.DMCircuit]:
         c = c_cls(2)
         c.h(0)
         c.h(1)
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_gates.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_interfaces.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_keras.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_miscs.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_miscs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     ([2, 1], np.kron(y, x)),
     ([3, 1], np.kron(z, x)),
     ([3, 2, 2, 0], np.kron(np.kron(np.kron(z, y), y), i)),
     ([0, 1, 1, 1], np.kron(np.kron(np.kron(i, x), x), x)),
 ]
 
 
+def test_about():
+    print(tc.about())
+
+
 def test_ps2coo(tfb):
     for l, a in check_pairs:
         r1 = PauliString2COO(tf.constant(l, dtype=tf.int64))
         np.testing.assert_allclose(tc.backend.to_dense(r1), a, atol=1e-5)
 
 
 def test_pss2coo(tfb):
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_qaoa.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_results.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_templates.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230416/tests/test_van.py` & `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_van.py`

 * *Files identical despite different names*

