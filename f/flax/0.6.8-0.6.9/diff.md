# Comparing `tmp/flax-0.6.8.tar.gz` & `tmp/flax-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flax-0.6.8.tar", last modified: Tue Mar 28 21:15:08 2023, max compression
+gzip compressed data, was "flax-0.6.9.tar", last modified: Tue Apr 18 21:02:47 2023, max compression
```

## Comparing `flax-0.6.8.tar` & `flax-0.6.9.tar`

### file list

```diff
@@ -1,78 +1,416 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.673181 flax-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-28 21:14:59.000000 flax-0.6.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-03-28 21:14:59.000000 flax-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-28 21:15:08.673181 flax-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-03-28 21:14:59.000000 flax-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.669181 flax-0.6.8/flax/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-28 21:14:59.000000 flax-0.6.8/flax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-03-28 21:14:59.000000 flax-0.6.8/flax/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.673181 flax-0.6.8/flax/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/axes_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/frozen_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    56619 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/lift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.673181 flax-0.6.8/flax/core/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/nn/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/nn/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/nn/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/partial_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    35706 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/tracers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-28 21:14:59.000000 flax-0.6.8/flax/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    29793 2023-03-28 21:14:59.000000 flax-0.6.8/flax/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-28 21:14:59.000000 flax-0.6.8/flax/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-03-28 21:14:59.000000 flax-0.6.8/flax/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-03-28 21:14:59.000000 flax-0.6.8/flax/jax_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.673181 flax-0.6.8/flax/linen/
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/dotgetter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/kw_only_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    32974 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    85510 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/partitioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)    36844 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    19162 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    59698 2023-03-28 21:14:59.000000 flax-0.6.8/flax/linen/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.673181 flax-0.6.8/flax/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-28 21:14:59.000000 flax-0.6.8/flax/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-03-28 21:14:59.000000 flax-0.6.8/flax/metrics/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-28 21:14:59.000000 flax-0.6.8/flax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-03-28 21:14:59.000000 flax-0.6.8/flax/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-03-28 21:14:59.000000 flax-0.6.8/flax/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.673181 flax-0.6.8/flax/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-28 21:14:59.000000 flax-0.6.8/flax/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-03-28 21:14:59.000000 flax-0.6.8/flax/testing/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-28 21:14:59.000000 flax-0.6.8/flax/traceback_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.673181 flax-0.6.8/flax/training/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41383 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/dynamic_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/lr_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/orbax_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/prefetch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-28 21:14:59.000000 flax-0.6.8/flax/training/train_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-03-28 21:14:59.000000 flax-0.6.8/flax/traverse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-28 21:14:59.000000 flax-0.6.8/flax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:15:08.669181 flax-0.6.8/flax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-28 21:15:08.000000 flax-0.6.8/flax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-28 21:15:08.000000 flax-0.6.8/flax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 21:15:08.000000 flax-0.6.8/flax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 21:15:08.000000 flax-0.6.8/flax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-28 21:15:08.000000 flax-0.6.8/flax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-28 21:15:08.000000 flax-0.6.8/flax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-28 21:15:08.673181 flax-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-28 21:14:59.000000 flax-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.017206 flax-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.929206 flax-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.929206 flax-0.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-18 21:02:27.000000 flax-0.6.9/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.933206 flax-0.6.9/.github/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-18 21:02:27.000000 flax-0.6.9/.github/analytics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-04-18 21:02:27.000000 flax-0.6.9/.github/analytics/get_repo_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-18 21:02:27.000000 flax-0.6.9/.github/analytics/issue_activity_since_date.gql
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-18 21:02:27.000000 flax-0.6.9/.github/analytics/pr_data_query.gql
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 21:02:27.000000 flax-0.6.9/.github/analytics/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-18 21:02:27.000000 flax-0.6.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.933206 flax-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-18 21:02:27.000000 flax-0.6.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 21:02:27.000000 flax-0.6.9/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 21:02:27.000000 flax-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-18 21:02:27.000000 flax-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-18 21:02:27.000000 flax-0.6.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-18 21:02:27.000000 flax-0.6.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    18804 2023-04-18 21:02:27.000000 flax-0.6.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-04-18 21:02:27.000000 flax-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-18 21:02:47.017206 flax-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-18 21:02:27.000000 flax-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 21:02:27.000000 flax-0.6.9/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.933206 flax-0.6.9/dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.933206 flax-0.6.9/dev/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-18 21:02:27.000000 flax-0.6.9/dev/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-18 21:02:27.000000 flax-0.6.9/dev/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-18 21:02:27.000000 flax-0.6.9/dev/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-18 21:02:27.000000 flax-0.6.9/dev/update_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.937206 flax-0.6.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 21:02:27.000000 flax-0.6.9/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-18 21:02:27.000000 flax-0.6.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-18 21:02:27.000000 flax-0.6.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.941207 flax-0.6.9/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-18 21:02:27.000000 flax-0.6.9/docs/_ext/codediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-18 21:02:27.000000 flax-0.6.9/docs/_ext/codediff_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.917207 flax-0.6.9/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.941207 flax-0.6.9/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-18 21:02:27.000000 flax-0.6.9/docs/_static/css/flax_theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.917207 flax-0.6.9/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.941207 flax-0.6.9/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-18 21:02:27.000000 flax-0.6.9/docs/_templates/autosummary/flax_module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.941207 flax-0.6.9/docs/advanced_topics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/arguments.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/convert_pytorch_to_flax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/lift.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/linen_design_principles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/linen_upgrade_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/module_lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/optax_update_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-18 21:02:27.000000 flax-0.6.9/docs/advanced_topics/philosophy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.945206 flax-0.6.9/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.core.frozen_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.jax_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.linen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.struct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.traceback_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/flax.traverse_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 21:02:27.000000 flax-0.6.9/docs/api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-18 21:02:27.000000 flax-0.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-18 21:02:27.000000 flax-0.6.9/docs/conf_sphinx_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-18 21:02:27.000000 flax-0.6.9/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.945206 flax-0.6.9/docs/developer_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 21:02:27.000000 flax-0.6.9/docs/developer_notes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-04-18 21:02:27.000000 flax-0.6.9/docs/developer_notes/lift.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21998 2023-04-18 21:02:27.000000 flax-0.6.9/docs/developer_notes/module_lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-18 21:02:27.000000 flax-0.6.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-18 21:02:27.000000 flax-0.6.9/docs/examples_community_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-18 21:02:27.000000 flax-0.6.9/docs/examples_core_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22578 2023-04-18 21:02:27.000000 flax-0.6.9/docs/examples_google_research_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-18 21:02:27.000000 flax-0.6.9/docs/examples_repositories_that_use_flax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-04-18 21:02:27.000000 flax-0.6.9/docs/flax.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.949206 flax-0.6.9/docs/flip/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 21:02:27.000000 flax-0.6.9/docs/flip/0000-template.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-04-18 21:02:27.000000 flax-0.6.9/docs/flip/1009-optimizer-api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-04-18 21:02:27.000000 flax-0.6.9/docs/flip/1777-default-dtype.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-04-18 21:02:27.000000 flax-0.6.9/docs/flip/2434-general-metadata.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-18 21:02:27.000000 flax-0.6.9/docs/flip/2974-kw-only-dataclasses.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-18 21:02:27.000000 flax-0.6.9/docs/flip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   102609 2023-04-18 21:02:27.000000 flax-0.6.9/docs/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-04-18 21:02:27.000000 flax-0.6.9/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-18 21:02:27.000000 flax-0.6.9/docs/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.957206 flax-0.6.9/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/arguments.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/batch_norm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/convert_pytorch_to_flax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/dropout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/ensembling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/extracting_intermediates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    40409 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/flax_basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22504 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/flax_basics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    38147 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/flax_on_pjit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22791 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/flax_on_pjit.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/full_eval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/index_converting_and_upgrading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/index_data_preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/index_flax_fundamentals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/index_model_inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/index_parallel_training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/index_training_techniques.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38261 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/jax_for_the_impatient.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/jax_for_the_impatient.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/linen_upgrade_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/lr_schedule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/model_surgery.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/model_surgery.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/optax_update_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/orbax_upgrade_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/setup_or_nncompact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/state_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/transfer_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/transfer_learning.md
+-rw-r--r--   0 runner    (1001) docker     (123)    53165 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/use_checkpointing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26620 2023-04-18 21:02:27.000000 flax-0.6.9/docs/guides/use_checkpointing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-18 21:02:27.000000 flax-0.6.9/docs/howtos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-04-18 21:02:27.000000 flax-0.6.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-18 21:02:27.000000 flax-0.6.9/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-18 21:02:27.000000 flax-0.6.9/docs/mission.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.961206 flax-0.6.9/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/flax_sharp_bits.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/flax_sharp_bits.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/full_eval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/full_eval.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    40238 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/linen_intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21869 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/linen_intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/optax_update_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/optax_update_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/orbax_upgrade_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/orbax_upgrade_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/state_params.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-18 21:02:27.000000 flax-0.6.9/docs/notebooks/state_params.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-18 21:02:27.000000 flax-0.6.9/docs/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-18 21:02:27.000000 flax-0.6.9/docs/philosophy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 21:02:27.000000 flax-0.6.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.961206 flax-0.6.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 21:02:27.000000 flax-0.6.9/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.961206 flax-0.6.9/examples/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-18 21:02:27.000000 flax-0.6.9/examples/cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-18 21:02:27.000000 flax-0.6.9/examples/cloud/launch_gce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-18 21:02:27.000000 flax-0.6.9/examples/cloud/startup_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.965206 flax-0.6.9/examples/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.965206 flax-0.6.9/examples/imagenet/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/configs/fake_data_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/configs/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/configs/v100_x8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/configs/v100_x8_mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)   294628 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/imagenet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/imagenet_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/imagenet_fake_data_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-18 21:02:27.000000 flax-0.6.9/examples/imagenet/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.969206 flax-0.6.9/examples/linen_design_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/attention_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/mlp_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/mlp_inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/mlp_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/tied_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-18 21:02:27.000000 flax-0.6.9/examples/linen_design_test/weight_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.973206 flax-0.6.9/examples/lm1b/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.973206 flax-0.6.9/examples/lm1b/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/temperature_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/temperature_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-18 21:02:27.000000 flax-0.6.9/examples/lm1b/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.973206 flax-0.6.9/examples/mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.973206 flax-0.6.9/examples/mnist/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99011 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/mnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/mnist_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-18 21:02:27.000000 flax-0.6.9/examples/mnist/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.977206 flax-0.6.9/examples/nlp_seq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-18 21:02:27.000000 flax-0.6.9/examples/nlp_seq/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-04-18 21:02:27.000000 flax-0.6.9/examples/nlp_seq/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-18 21:02:27.000000 flax-0.6.9/examples/nlp_seq/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-18 21:02:27.000000 flax-0.6.9/examples/nlp_seq/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 21:02:27.000000 flax-0.6.9/examples/nlp_seq/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14128 2023-04-18 21:02:27.000000 flax-0.6.9/examples/nlp_seq/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.981206 flax-0.6.9/examples/ogbg_molpcba/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.981206 flax-0.6.9/examples/ogbg_molpcba/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/configs/default_graph_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/configs/hparam_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/configs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1111228 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/ogbg_molpcba.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/ogbg_molpcba_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ogbg_molpcba/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.985206 flax-0.6.9/examples/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.985206 flax-0.6.9/examples/ppo/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/ppo_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/ppo_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/ppo_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/seed_rl_atari_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-18 21:02:27.000000 flax-0.6.9/examples/ppo/test_episodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.985206 flax-0.6.9/examples/seq2seq/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-18 21:02:27.000000 flax-0.6.9/examples/seq2seq/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-04-18 21:02:27.000000 flax-0.6.9/examples/seq2seq/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-18 21:02:27.000000 flax-0.6.9/examples/seq2seq/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 21:02:27.000000 flax-0.6.9/examples/seq2seq/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-04-18 21:02:27.000000 flax-0.6.9/examples/seq2seq/seq2seq.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-18 21:02:27.000000 flax-0.6.9/examples/seq2seq/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-18 21:02:27.000000 flax-0.6.9/examples/seq2seq/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.989206 flax-0.6.9/examples/sst2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/build_vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.989206 flax-0.6.9/examples/sst2/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/configs/default.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10057 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/sst2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/train_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117898 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/vocab.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4421 2023-04-18 21:02:27.000000 flax-0.6.9/examples/sst2/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.993206 flax-0.6.9/examples/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 21:02:27.000000 flax-0.6.9/examples/vae/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 21:02:27.000000 flax-0.6.9/examples/vae/reconstruction.png
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 21:02:27.000000 flax-0.6.9/examples/vae/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.993206 flax-0.6.9/examples/vae/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 21:02:27.000000 flax-0.6.9/examples/vae/results/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    43139 2023-04-18 21:02:27.000000 flax-0.6.9/examples/vae/sample.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-04-18 21:02:27.000000 flax-0.6.9/examples/vae/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-18 21:02:27.000000 flax-0.6.9/examples/vae/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.997206 flax-0.6.9/examples/wmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/bleu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:46.997206 flax-0.6.9/examples/wmt/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19064 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-18 21:02:27.000000 flax-0.6.9/examples/wmt/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.001206 flax-0.6.9/flax/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-18 21:02:27.000000 flax-0.6.9/flax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-18 21:02:27.000000 flax-0.6.9/flax/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.005206 flax-0.6.9/flax/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/axes_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/flax_functional_engine.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/frozen_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56619 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/lift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.005206 flax-0.6.9/flax/core/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/nn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/nn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/nn/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/nn/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/partial_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35706 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/tracers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 21:02:27.000000 flax-0.6.9/flax/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29793 2023-04-18 21:02:27.000000 flax-0.6.9/flax/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 21:02:27.000000 flax-0.6.9/flax/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-18 21:02:27.000000 flax-0.6.9/flax/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-04-18 21:02:27.000000 flax-0.6.9/flax/jax_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.009206 flax-0.6.9/flax/linen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/dotgetter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.009206 flax-0.6.9/flax/linen/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/experimental/layers_with_named_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/kw_only_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32979 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86133 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36844 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19162 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59698 2023-04-18 21:02:27.000000 flax-0.6.9/flax/linen/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.009206 flax-0.6.9/flax/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 21:02:27.000000 flax-0.6.9/flax/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-18 21:02:27.000000 flax-0.6.9/flax/metrics/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.009206 flax-0.6.9/flax/oss/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 21:02:27.000000 flax-0.6.9/flax/oss/ .git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 21:02:27.000000 flax-0.6.9/flax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-18 21:02:27.000000 flax-0.6.9/flax/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-18 21:02:27.000000 flax-0.6.9/flax/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.009206 flax-0.6.9/flax/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-18 21:02:27.000000 flax-0.6.9/flax/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-18 21:02:27.000000 flax-0.6.9/flax/testing/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-18 21:02:27.000000 flax-0.6.9/flax/traceback_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.013206 flax-0.6.9/flax/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43229 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/dynamic_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/lr_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/orbax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/prefetch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-18 21:02:27.000000 flax-0.6.9/flax/training/train_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-18 21:02:27.000000 flax-0.6.9/flax/traverse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-18 21:02:27.000000 flax-0.6.9/flax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.001206 flax-0.6.9/flax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-18 21:02:46.000000 flax-0.6.9/flax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-04-18 21:02:46.000000 flax-0.6.9/flax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:02:46.000000 flax-0.6.9/flax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 21:02:46.000000 flax-0.6.9/flax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 21:02:46.000000 flax-0.6.9/flax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.013206 flax-0.6.9/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    80407 2023-04-18 21:02:27.000000 flax-0.6.9/images/flax_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-18 21:02:27.000000 flax-0.6.9/images/flax_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-04-18 21:02:27.000000 flax-0.6.9/images/flax_logo_250px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29095 2023-04-18 21:02:27.000000 flax-0.6.9/images/flax_logo_500px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-04-18 21:02:27.000000 flax-0.6.9/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-18 21:02:27.000000 flax-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:02:47.017206 flax-0.6.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.013206 flax-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-04-18 21:02:27.000000 flax-0.6.9/tests/checkpoints_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-18 21:02:27.000000 flax-0.6.9/tests/colab_tpu_jax_version.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.013206 flax-0.6.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/core_frozen_dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/core_lift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/core_meta_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/core_scope_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.017206 flax-0.6.9/tests/core/design/
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_auto_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_big_resnets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_custom_vjp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_flow_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_scan_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_tied_autoencoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_vmap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-18 21:02:27.000000 flax-0.6.9/tests/core/design/core_weight_std_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-18 21:02:27.000000 flax-0.6.9/tests/download_dataset_metadata.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-18 21:02:27.000000 flax-0.6.9/tests/early_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-18 21:02:27.000000 flax-0.6.9/tests/import_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-04-18 21:02:27.000000 flax-0.6.9/tests/io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-18 21:02:27.000000 flax-0.6.9/tests/jax_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:47.017206 flax-0.6.9/tests/linen/
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/dotgetter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/initializers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/kw_only_dataclasses_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_activation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_combinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_dtypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35451 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_meta_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61569 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_module_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53644 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/linen_transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17800 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/partitioning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/summary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-18 21:02:27.000000 flax-0.6.9/tests/linen/toplevel_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3960 2023-04-18 21:02:27.000000 flax-0.6.9/tests/run_all_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-04-18 21:02:27.000000 flax-0.6.9/tests/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-18 21:02:27.000000 flax-0.6.9/tests/struct_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-04-18 21:02:27.000000 flax-0.6.9/tests/tensorboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-18 21:02:27.000000 flax-0.6.9/tests/traceback_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-04-18 21:02:27.000000 flax-0.6.9/tests/traverse_util_test.py
```

### Comparing `flax-0.6.8/LICENSE` & `flax-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flax-0.6.8/PKG-INFO` & `flax-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: flax
-Version: 0.6.8
+Version: 0.6.9
 Summary: Flax: A neural network library for JAX designed for flexibility
-Home-page: https://github.com/google/flax
-Author: Flax team
-Author-email: flax-dev@google.com
+Author-email: Flax team <flax-dev@google.com>
+Project-URL: homepage, https://github.com/google/flax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 Provides-Extra: all
+Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/google/flax/main/images/flax_logo_250px.png" alt="logo"></img>
 </div>
 
@@ -198,29 +197,29 @@
 decoded = model.apply(variables, encoded, method=model.decode)
 ```
 
 ## 🤗 Hugging Face
 
 In-detail examples to train and evaluate a variety of Flax models for
 Natural Language Processing, Computer Vision, and Speech Recognition are
-actively maintained in the [🤗 Transformers repository](https://github.com/huggingface/transformers/tree/master/examples/flax).
+actively maintained in the [🤗 Transformers repository](https://github.com/huggingface/transformers/tree/main/examples/flax).
 
 As of October 2021, the [19 most-used Transformer architectures](https://huggingface.co/transformers/#supported-frameworks) are supported in Flax
 and over 5000 pretrained checkpoints in Flax have been uploaded to the [🤗 Hub](https://huggingface.co/models?library=jax&sort=downloads).
 
 ## Citing Flax
 
 To cite this repository:
 
 ```
 @software{flax2020github,
   author = {Jonathan Heek and Anselm Levskaya and Avital Oliver and Marvin Ritter and Bertrand Rondepierre and Andreas Steiner and Marc van {Z}ee},
   title = {{F}lax: A neural network library and ecosystem for {JAX}},
   url = {http://github.com/google/flax},
-  version = {0.6.8},
+  version = {0.6.9},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, names are in alphabetical order, the version number
 is intended to be that from [flax/version.py](https://github.com/google/flax/blob/main/flax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `flax-0.6.8/README.md` & `flax-0.6.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -179,29 +179,29 @@
 decoded = model.apply(variables, encoded, method=model.decode)
 ```
 
 ## 🤗 Hugging Face
 
 In-detail examples to train and evaluate a variety of Flax models for
 Natural Language Processing, Computer Vision, and Speech Recognition are
-actively maintained in the [🤗 Transformers repository](https://github.com/huggingface/transformers/tree/master/examples/flax).
+actively maintained in the [🤗 Transformers repository](https://github.com/huggingface/transformers/tree/main/examples/flax).
 
 As of October 2021, the [19 most-used Transformer architectures](https://huggingface.co/transformers/#supported-frameworks) are supported in Flax
 and over 5000 pretrained checkpoints in Flax have been uploaded to the [🤗 Hub](https://huggingface.co/models?library=jax&sort=downloads).
 
 ## Citing Flax
 
 To cite this repository:
 
 ```
 @software{flax2020github,
   author = {Jonathan Heek and Anselm Levskaya and Avital Oliver and Marvin Ritter and Bertrand Rondepierre and Andreas Steiner and Marc van {Z}ee},
   title = {{F}lax: A neural network library and ecosystem for {JAX}},
   url = {http://github.com/google/flax},
-  version = {0.6.8},
+  version = {0.6.9},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, names are in alphabetical order, the version number
 is intended to be that from [flax/version.py](https://github.com/google/flax/blob/main/flax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `flax-0.6.8/flax/__init__.py` & `flax-0.6.9/flax/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/configurations.py` & `flax-0.6.9/flax/configurations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/__init__.py` & `flax-0.6.9/flax/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,16 @@
 
 from .axes_scan import broadcast as broadcast
 from .frozen_dict import (
   FrozenDict as FrozenDict,
   freeze as freeze,
   unfreeze as unfreeze,
   copy as copy,
-  pop as pop
+  pop as pop,
+  pretty_repr as pretty_repr
 )
 
 from .tracers import (
   current_trace as current_trace,
   trace_level as trace_level,
   check_trace_level as check_trace_level
 )
```

### Comparing `flax-0.6.8/flax/core/axes_scan.py` & `flax-0.6.9/flax/core/axes_scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Wrapper around jax.lax.scan with in_axes/out_axes API."""
 import functools
 from typing import Any, Callable, Optional
 
 import jax
+from jax import core
 from jax import lax
 from jax import linear_util as lu
 from jax.interpreters import partial_eval as pe
 import jax.numpy as jnp
 import numpy as np
 
 
@@ -120,18 +121,18 @@
       else:
         ys = jax.tree_util.tree_map(
             lambda ax, y: (() if ax is broadcast else y), out_axes, ys)
         return c, ys
     broadcast_body = functools.partial(body_fn, init_mode=True)
 
     carry_avals = jax.tree_util.tree_map(
-        lambda x: jax.ShapedArray(jnp.shape(x), jnp.result_type(x)),
+        lambda x: core.ShapedArray(jnp.shape(x), jnp.result_type(x)),
         init)
     scan_avals = jax.tree_util.tree_map(
-        lambda x: jax.ShapedArray(jnp.shape(x)[1:], jnp.result_type(x)),
+        lambda x: core.ShapedArray(jnp.shape(x)[1:], jnp.result_type(x)),
         xs)
     input_avals = (carry_avals, scan_avals)
 
     in_avals, in_tree = jax.tree_util.tree_flatten(input_avals)
     f_flat, out_tree = jax.api_util.flatten_fun_nokwargs(
         lu.wrap_init(broadcast_body), in_tree)
     in_pvals = list(map(pe.PartialVal.unknown, in_avals))
```

### Comparing `flax-0.6.8/flax/core/frozen_dict.py` & `flax-0.6.9/flax/core/frozen_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -264,14 +264,43 @@
   elif isinstance(x, dict):
     new_dict = jax.tree_map(lambda x: x, x) # make a deep copy of dict x
     value = new_dict.pop(key)
     return new_dict, value
   raise TypeError(f'Expected FrozenDict or dict, got {type(x)}')
 
 
+def pretty_repr(x: Any, num_spaces: int = 4) -> str:
+  """Returns an indented representation of the nested dictionary.
+  This is a utility function that can act on either a FrozenDict or
+  regular dict and mimics the behavior of `FrozenDict.pretty_repr`.
+  If x is any other dtype, this function will return `repr(x)`.
+
+  Args:
+    x: the dictionary to be represented
+    num_spaces: the number of space characters in each indentation level
+  Returns:
+    An indented string representation of the nested dictionary.
+  """
+
+  if isinstance(x, FrozenDict):
+    return x.pretty_repr()
+  else:
+    def pretty_dict(x):
+      if not isinstance(x, dict):
+        return repr(x)
+      rep = ''
+      for key, val in x.items():
+        rep += f'{key}: {pretty_dict(val)},\n'
+      if rep:
+        return '{\n' + _indent(rep, num_spaces) + '}'
+      else:
+        return '{}'
+    return pretty_dict(x)
+
+
 def _frozen_dict_state_dict(xs):
   return {key: serialization.to_state_dict(value) for key, value in xs.items()}
 
 
 def _restore_frozen_dict(xs, states):
   diff = set(map(str, xs.keys())).difference(states.keys())
   if diff:
```

### Comparing `flax-0.6.8/flax/core/lift.py` & `flax-0.6.9/flax/core/lift.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/meta.py` & `flax-0.6.9/flax/core/meta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,14 @@
 import functools
 from typing import Any, Callable, Dict, Mapping, Optional, Tuple, TypeVar, Union
 
 from flax import errors
 from flax import struct
 import jax
 from jax.experimental import maps
-from jax.experimental import pjit
 
 
 TAxisMetadata = Any # TypeVar('TAxisMetadata', bound='AxisMetadata')
 
 
 class AxisMetadata(metaclass=abc.ABCMeta):
   """Abstract base class for boxed Metadata.
@@ -267,14 +266,18 @@
     assert names.pop(index) == axis_name
     return self.replace(names=tuple(names))
 
   def get_partition_spec(self) -> jax.sharding.PartitionSpec:
     """Returns the ``Partitionspec`` for this partitioned value."""
     return jax.sharding.PartitionSpec(*self.names)
 
+  def get_sharding(self, mesh: jax.sharding.Mesh) -> jax.sharding.Sharding:
+    """Returns the ``NamedSharding`` for this partitioned value."""
+    return jax.sharding.NamedSharding(mesh, self.get_partition_spec())
+
 
 def with_partitioning(
     fn: Callable[..., Any],
     names: LogicalNames,
     mesh: Optional[jax.sharding.Mesh] = None,
   ) ->  Callable[..., Partitioned]:
   """Wraps a function's return value with Partitioned.
@@ -300,11 +303,20 @@
 
 
 def get_partition_spec(tree: Any) -> Any:
   """Extracts a PartitionSpec tree from a PyTree containing ``Partitioned`` values."""
   def f(x):
     if isinstance(x, Partitioned):
       return x.get_partition_spec()
+    # Unboxed arrays, which should be replicated across all devices
+    elif hasattr(x, 'shape'):
+      return jax.sharding.PartitionSpec()
     else:
       return None
   return jax.tree_map(f, tree,
                       is_leaf=lambda x: isinstance(x, Partitioned))
+
+
+def get_sharding(tree: Any, mesh: jax.sharding.Mesh) -> Any:
+  """Extracts a jax.sharding tree from a PyTree containing ``Partitioned`` values and a mesh."""
+  pspec_tree = get_partition_spec(tree)
+  return jax.tree_map(lambda x: jax.sharding.NamedSharding(mesh, x), pspec_tree)
```

### Comparing `flax-0.6.8/flax/core/nn/__init__.py` & `flax-0.6.9/flax/core/nn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/nn/attention.py` & `flax-0.6.9/flax/core/nn/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/nn/linear.py` & `flax-0.6.9/flax/core/nn/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/nn/normalization.py` & `flax-0.6.9/flax/core/nn/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/nn/stochastic.py` & `flax-0.6.9/flax/core/nn/stochastic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/partial_eval.py` & `flax-0.6.9/flax/core/partial_eval.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,23 +13,24 @@
 # limitations under the License.
 
 from typing import Any
 
 import functools
 
 import jax
+from jax import core
 from jax import linear_util as lu
 from jax.interpreters import partial_eval as pe
 
 from flax import errors
 
 
 def _maybe_unknown(x: Any) -> pe.PartialVal:
   if isinstance(x, jax.ShapeDtypeStruct):
-    return pe.PartialVal.unknown(jax.ShapedArray(x.shape, x.dtype))
+    return pe.PartialVal.unknown(core.ShapedArray(x.shape, x.dtype))
   else:
     return pe.PartialVal.known(x)
 
 
 def lazy_init(fn):
   """Lazily evaluates a function by using the shapes of the inputs.
```

### Comparing `flax-0.6.8/flax/core/scope.py` & `flax-0.6.9/flax/core/scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/tracers.py` & `flax-0.6.9/flax/core/tracers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/core/variables.py` & `flax-0.6.9/flax/core/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/errors.py` & `flax-0.6.9/flax/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/ids.py` & `flax-0.6.9/flax/ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/io.py` & `flax-0.6.9/flax/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -183,7 +183,17 @@
   """Remove a directory and recursively all contents inside. Might fail if used on a file path."""
   if io_mode == BackendMode.DEFAULT:
     return shutil.rmtree(path)
   elif io_mode == BackendMode.TF:
     return gfile.rmtree(path)
   else:
     raise ValueError("Unknown IO Backend Mode.")
+
+
+def getsize(path):
+  """Return the size, in bytes, of path."""
+  if io_mode == BackendMode.DEFAULT:
+    return os.path.getsize(path)
+  elif io_mode == BackendMode.TF:
+    return gfile.stat(path).length
+  else:
+    raise ValueError("Unknown IO Backend Mode.")
```

### Comparing `flax-0.6.8/flax/jax_utils.py` & `flax-0.6.9/flax/jax_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,14 +17,15 @@
 
 import collections
 from collections.abc import Iterable  # pylint: disable=g-importing-member
 import itertools
 import warnings
 
 import jax
+from jax import core
 from jax import lax
 from jax import linear_util as lu
 from jax.interpreters import partial_eval as pe
 import jax.numpy as jnp
 import numpy as np
 
 
@@ -78,15 +79,15 @@
   # output cannot be returned in lazy_create because jax.eval_shape will only
   # return the shape and dtype.
   # TODO(mattjj,jheek): use a public JAX API
   f = lambda *inputs: fn(*inputs, *args, **kwargs)
   input_structs = [_parse_spec(spec) for spec in input_spec]
   inputs_flat, in_tree = jax.tree_util.tree_flatten(input_structs)
   f_flat, out_tree = jax.api_util.flatten_fun_nokwargs(lu.wrap_init(f), in_tree)
-  in_pvals = [pe.PartialVal.unknown(jax.ShapedArray(x.shape, x.dtype))
+  in_pvals = [pe.PartialVal.unknown(core.ShapedArray(x.shape, x.dtype))
               for x in inputs_flat]
   _, out_pvals, _ = pe.trace_to_jaxpr_nounits(f_flat, in_pvals)
   out_flat = [const if pv is None else jax.ShapeDtypeStruct(pv.shape, pv.dtype)
               for pv, const in out_pvals]
   return jax.tree_util.tree_unflatten(out_tree(), out_flat)
```

### Comparing `flax-0.6.8/flax/linen/__init__.py` & `flax-0.6.9/flax/linen/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -61,23 +61,25 @@
   broadcast as broadcast,
   meta as meta,
 )
 from ..core.meta import (
     Partitioned as Partitioned,
     with_partitioning as with_partitioning,
     get_partition_spec as get_partition_spec,
+    get_sharding as get_sharding,
     unbox as unbox,
     PARTITION_NAME as PARTITION_NAME,
 )
 from .spmd import (
     logical_axis_rules as logical_axis_rules,
     set_logical_axis_rules as set_logical_axis_rules,
     get_logical_axis_rules as get_logical_axis_rules,
     logical_to_mesh_axes,
     logical_to_mesh,
+    logical_to_mesh_sharding,
     with_logical_constraint,
     LogicallyPartitioned as LogicallyPartitioned,
     with_logical_partitioning as with_logical_partitioning,
 )
 from .initializers import (
   ones as ones,
   ones_init as ones_init,
```

### Comparing `flax-0.6.8/flax/linen/activation.py` & `flax-0.6.9/flax/linen/activation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/attention.py` & `flax-0.6.9/flax/linen/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/combinators.py` & `flax-0.6.9/flax/linen/combinators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/dotgetter.py` & `flax-0.6.9/flax/linen/dotgetter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/dtypes.py` & `flax-0.6.9/flax/linen/dtypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/initializers.py` & `flax-0.6.9/flax/linen/initializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/kw_only_dataclasses.py` & `flax-0.6.9/flax/linen/kw_only_dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/linear.py` & `flax-0.6.9/flax/linen/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,15 +22,15 @@
 from flax.linen import initializers
 from flax.linen.module import compact
 from flax.linen.module import Module
 from flax.linen.dtypes import promote_dtype
 from jax import eval_shape
 from jax import lax
 from jax import random
-from jax import ShapedArray
+from jax.core import ShapedArray
 import jax.numpy as jnp
 import numpy as np
 import jax
 
 
 PRNGKey = Any
 Shape = Tuple[int, ...]
```

### Comparing `flax-0.6.8/flax/linen/module.py` & `flax-0.6.9/flax/linen/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 2320 436f 7079 7269 6768 7420 3230 3232  # Copyright 2022
+00000000: 2320 436f 7079 7269 6768 7420 3230 3233  # Copyright 2023
 00000010: 2054 6865 2046 6c61 7820 4175 7468 6f72   The Flax Author
 00000020: 732e 0a23 0a23 204c 6963 656e 7365 6420  s..#.# Licensed 
 00000030: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
 00000040: 204c 6963 656e 7365 2c20 5665 7273 696f   License, Versio
 00000050: 6e20 322e 3020 2874 6865 2022 4c69 6365  n 2.0 (the "Lice
 00000060: 6e73 6522 293b 0a23 2079 6f75 206d 6179  nse");.# you may
 00000070: 206e 6f74 2075 7365 2074 6869 7320 6669   not use this fi
@@ -37,5309 +37,5348 @@
 00000240: 6e73 652e 0a0a 2222 2246 6c61 7820 4d6f  nse..."""Flax Mo
 00000250: 6475 6c65 2e22 2222 0a69 6d70 6f72 7420  dule.""".import 
 00000260: 636f 6e74 6578 746c 6962 0a69 6d70 6f72  contextlib.impor
 00000270: 7420 6461 7461 636c 6173 7365 730a 696d  t dataclasses.im
 00000280: 706f 7274 2065 6e75 6d0a 696d 706f 7274  port enum.import
 00000290: 2066 756e 6374 6f6f 6c73 0a69 6d70 6f72   functools.impor
 000002a0: 7420 696e 7370 6563 740a 696d 706f 7274  t inspect.import
-000002b0: 2072 650a 696d 706f 7274 2074 6872 6561   re.import threa
-000002c0: 6469 6e67 0a69 6d70 6f72 7420 7479 7069  ding.import typi
-000002d0: 6e67 0a69 6d70 6f72 7420 7765 616b 7265  ng.import weakre
-000002e0: 660a 6672 6f6d 2074 7970 696e 6720 696d  f.from typing im
-000002f0: 706f 7274 2028 416e 792c 2043 616c 6c61  port (Any, Calla
-00000300: 626c 652c 2044 6963 742c 2049 7465 7261  ble, Dict, Itera
-00000310: 626c 652c 204c 6973 742c 2053 6571 7565  ble, List, Seque
-00000320: 6e63 652c 204e 616d 6564 5475 706c 652c  nce, NamedTuple,
-00000330: 204d 6170 7069 6e67 2c0a 2020 2020 2020   Mapping,.      
-00000340: 2020 2020 2020 2020 2020 2020 2020 4f70                Op
-00000350: 7469 6f6e 616c 2c20 5365 742c 2054 7570  tional, Set, Tup
-00000360: 6c65 2c20 5479 7065 2c20 5479 7065 5661  le, Type, TypeVa
-00000370: 722c 2055 6e69 6f6e 2c20 6f76 6572 6c6f  r, Union, overlo
-00000380: 6164 290a 0a69 6d70 6f72 7420 6a61 780a  ad)..import jax.
-00000390: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-000003a0: 6e70 0a69 6d70 6f72 7420 6a61 782e 6e75  np.import jax.nu
-000003b0: 6d70 7920 6173 206a 6e70 0a66 726f 6d20  mpy as jnp.from 
-000003c0: 7479 7069 6e67 5f65 7874 656e 7369 6f6e  typing_extension
-000003d0: 7320 696d 706f 7274 2050 726f 746f 636f  s import Protoco
-000003e0: 6c2c 205c 0a20 2064 6174 6163 6c61 7373  l, \.  dataclass
-000003f0: 5f74 7261 6e73 666f 726d 2020 2320 7079  _transform  # py
-00000400: 7479 7065 3a20 6469 7361 626c 653d 6e6f  type: disable=no
-00000410: 742d 7375 7070 6f72 7465 642d 7965 740a  t-supported-yet.
-00000420: 0a69 6d70 6f72 7420 666c 6178 0a66 726f  .import flax.fro
-00000430: 6d20 666c 6178 2069 6d70 6f72 7420 2863  m flax import (c
-00000440: 6f6e 6669 672c 2063 6f72 652c 2065 7272  onfig, core, err
-00000450: 6f72 732c 2073 6572 6961 6c69 7a61 7469  ors, serializati
-00000460: 6f6e 2c20 7472 6163 6562 6163 6b5f 7574  on, traceback_ut
-00000470: 696c 2c0a 2020 2020 2020 2020 2020 2020  il,.            
-00000480: 2020 2020 2020 7472 6176 6572 7365 5f75        traverse_u
-00000490: 7469 6c29 0a66 726f 6d20 666c 6178 2e63  til).from flax.c
-000004a0: 6f72 6520 696d 706f 7274 2053 636f 7065  ore import Scope
-000004b0: 0a66 726f 6d20 666c 6178 2e63 6f72 6520  .from flax.core 
-000004c0: 696d 706f 7274 2070 6172 7469 616c 5f65  import partial_e
-000004d0: 7661 6c0a 6672 6f6d 2066 6c61 782e 636f  val.from flax.co
-000004e0: 7265 2e66 726f 7a65 6e5f 6469 6374 2069  re.frozen_dict i
-000004f0: 6d70 6f72 7420 4672 6f7a 656e 4469 6374  mport FrozenDict
-00000500: 0a66 726f 6d20 666c 6178 2e63 6f72 652e  .from flax.core.
-00000510: 7363 6f70 6520 696d 706f 7274 2028 2020  scope import (  
-00000520: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00000530: 653d 672d 6d75 6c74 6970 6c65 2d69 6d70  e=g-multiple-imp
-00000540: 6f72 740a 2020 2020 436f 6c6c 6563 7469  ort.    Collecti
-00000550: 6f6e 4669 6c74 6572 2c20 4465 6e79 4c69  onFilter, DenyLi
-00000560: 7374 2c20 4672 6f7a 656e 5661 7269 6162  st, FrozenVariab
-00000570: 6c65 4469 6374 2c20 5661 7269 6162 6c65  leDict, Variable
-00000580: 2c20 5661 7269 6162 6c65 4469 6374 2c0a  , VariableDict,.
-00000590: 2020 2020 756e 696f 6e5f 6669 6c74 6572      union_filter
-000005a0: 7329 0a66 726f 6d20 666c 6178 2e69 6473  s).from flax.ids
-000005b0: 2069 6d70 6f72 7420 466c 6178 4964 0a66   import FlaxId.f
-000005c0: 726f 6d20 666c 6178 2e69 6473 2069 6d70  rom flax.ids imp
-000005d0: 6f72 7420 7575 6964 0a66 726f 6d20 666c  ort uuid.from fl
-000005e0: 6178 2e6c 696e 656e 2069 6d70 6f72 7420  ax.linen import 
-000005f0: 6b77 5f6f 6e6c 795f 6461 7461 636c 6173  kw_only_dataclas
-00000600: 7365 730a 0a0a 7472 6163 6562 6163 6b5f  ses...traceback_
-00000610: 7574 696c 2e72 6567 6973 7465 725f 6578  util.register_ex
-00000620: 636c 7573 696f 6e28 5f5f 6669 6c65 5f5f  clusion(__file__
-00000630: 290a 0a50 524e 474b 6579 203d 2041 6e79  )..PRNGKey = Any
-00000640: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-00000650: 626c 653d 696e 7661 6c69 642d 6e61 6d65  ble=invalid-name
-00000660: 0a52 4e47 5365 7175 656e 6365 7320 3d20  .RNGSequences = 
-00000670: 4469 6374 5b73 7472 2c20 5052 4e47 4b65  Dict[str, PRNGKe
-00000680: 795d 0a41 7272 6179 203d 2041 6e79 2020  y].Array = Any  
-00000690: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-000006a0: 626c 653d 696e 7661 6c69 642d 6e61 6d65  ble=invalid-name
-000006b0: 0a0a 0a54 203d 2054 7970 6556 6172 2827  ...T = TypeVar('
-000006c0: 5427 290a 4b20 3d20 5479 7065 5661 7228  T').K = TypeVar(
-000006d0: 274b 2729 0a4d 203d 2054 7970 6556 6172  'K').M = TypeVar
-000006e0: 2827 4d27 2c20 626f 756e 643d 274d 6f64  ('M', bound='Mod
-000006f0: 756c 6527 290a 5f43 616c 6c61 626c 6554  ule')._CallableT
-00000700: 203d 2054 7970 6556 6172 2827 5f43 616c   = TypeVar('_Cal
-00000710: 6c61 626c 6554 272c 2062 6f75 6e64 3d43  lableT', bound=C
-00000720: 616c 6c61 626c 6529 0a0a 0a23 2055 7365  allable)...# Use
-00000730: 6420 666f 7220 6162 7374 7261 6374 6c79  d for abstractly
-00000740: 2074 6573 7469 6e67 206d 6f64 756c 6520   testing module 
-00000750: 6265 6861 7669 6f72 2e0a 5465 7374 5363  behavior..TestSc
-00000760: 6f70 6520 3d20 7479 7065 2827 5465 7374  ope = type('Test
-00000770: 5363 6f70 6527 2c0a 2020 2020 2020 2020  Scope',.        
-00000780: 2020 2020 2020 2020 2028 5363 6f70 652c           (Scope,
-00000790: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000007a0: 2020 2020 7b27 6d61 6b65 5f72 6e67 273a      {'make_rng':
-000007b0: 206c 616d 6264 6120 7365 6c66 2c20 6e61   lambda self, na
-000007c0: 6d65 3a20 6a61 782e 7261 6e64 6f6d 2e50  me: jax.random.P
-000007d0: 524e 474b 6579 2830 297d 290a 0a0a 2320  RNGKey(0)})...# 
-000007e0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-000007f0: 7072 6f74 6563 7465 642d 6163 6365 7373  protected-access
-00000800: 2c61 7474 7269 6275 7465 2d64 6566 696e  ,attribute-defin
-00000810: 6564 2d6f 7574 7369 6465 2d69 6e69 740a  ed-outside-init.
-00000820: 0a64 6566 205f 696e 6465 6e74 2878 3a20  .def _indent(x: 
-00000830: 7374 722c 206e 756d 5f73 7061 6365 733a  str, num_spaces:
-00000840: 2069 6e74 293a 0a20 2069 6e64 656e 745f   int):.  indent_
-00000850: 7374 7220 3d20 2720 2720 2a20 6e75 6d5f  str = ' ' * num_
-00000860: 7370 6163 6573 0a20 206c 696e 6573 203d  spaces.  lines =
-00000870: 2078 2e73 706c 6974 2827 5c6e 2729 0a20   x.split('\n'). 
-00000880: 2023 2073 6b69 7020 6c61 7374 206c 696e   # skip last lin
-00000890: 6520 6265 6361 7573 6520 6974 2069 7320  e because it is 
-000008a0: 616c 7761 7973 2065 6d70 7479 2061 6e64  always empty and
-000008b0: 2073 686f 756c 6420 6e6f 7420 6265 2069   should not be i
-000008c0: 6e64 656e 7465 642e 0a20 2061 7373 6572  ndented..  asser
-000008d0: 7420 6e6f 7420 6c69 6e65 735b 2d31 5d0a  t not lines[-1].
-000008e0: 2020 7265 7475 726e 2027 5c6e 272e 6a6f    return '\n'.jo
-000008f0: 696e 2869 6e64 656e 745f 7374 7220 2b20  in(indent_str + 
-00000900: 6c69 6e65 2066 6f72 206c 696e 6520 696e  line for line in
-00000910: 206c 696e 6573 5b3a 2d31 5d29 202b 2027   lines[:-1]) + '
-00000920: 5c6e 270a 0a0a 6465 6620 5f61 7474 725f  \n'...def _attr_
-00000930: 7265 7072 2876 616c 7565 3a20 416e 7929  repr(value: Any)
-00000940: 3a0a 2020 6966 2063 616c 6c61 626c 6528  :.  if callable(
-00000950: 7661 6c75 6529 2061 6e64 2067 6574 6174  value) and getat
-00000960: 7472 2876 616c 7565 2c20 275f 5f6e 616d  tr(value, '__nam
-00000970: 655f 5f27 2c20 4e6f 6e65 293a 0a20 2020  e__', None):.   
-00000980: 2076 616c 7565 5f72 6570 203d 2076 616c   value_rep = val
-00000990: 7565 2e5f 5f6e 616d 655f 5f0a 2020 656c  ue.__name__.  el
-000009a0: 7365 3a0a 2020 2020 7661 6c75 655f 7265  se:.    value_re
-000009b0: 7020 3d20 7265 7072 2876 616c 7565 290a  p = repr(value).
-000009c0: 2020 7265 7475 726e 2076 616c 7565 5f72    return value_r
-000009d0: 6570 0a0a 0a64 6566 205f 6d6f 6475 6c65  ep...def _module
-000009e0: 5f72 6570 7228 6d6f 6475 6c65 3a20 274d  _repr(module: 'M
-000009f0: 6f64 756c 6527 2c20 6e75 6d5f 7370 6163  odule', num_spac
-00000a00: 6573 3a20 696e 7420 3d20 3429 3a0a 2020  es: int = 4):.  
-00000a10: 2222 2252 6574 7572 6e73 2061 2070 7265  """Returns a pre
-00000a20: 7474 7920 7072 696e 7465 6420 7265 7072  tty printed repr
-00000a30: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-00000a40: 6520 6d6f 6475 6c65 2e22 2222 0a20 2063  e module.""".  c
-00000a50: 6c73 203d 2074 7970 6528 6d6f 6475 6c65  ls = type(module
-00000a60: 290a 2020 636c 735f 6e61 6d65 203d 2063  ).  cls_name = c
-00000a70: 6c73 2e5f 5f6e 616d 655f 5f0a 2020 7265  ls.__name__.  re
-00000a80: 7020 3d20 2727 0a0a 2020 6174 7472 6962  p = ''..  attrib
-00000a90: 7574 6573 203d 207b 0a20 2020 2020 2066  utes = {.      f
-00000aa0: 2e6e 616d 653a 2066 2e74 7970 650a 2020  .name: f.type.  
-00000ab0: 2020 2020 666f 7220 6620 696e 2064 6174      for f in dat
-00000ac0: 6163 6c61 7373 6573 2e66 6965 6c64 7328  aclasses.fields(
-00000ad0: 636c 7329 0a20 2020 2020 2069 6620 662e  cls).      if f.
-00000ae0: 6e61 6d65 206e 6f74 2069 6e20 2827 7061  name not in ('pa
-00000af0: 7265 6e74 272c 2027 6e61 6d65 2729 2061  rent', 'name') a
-00000b00: 6e64 2066 2e72 6570 720a 2020 7d0a 2020  nd f.repr.  }.  
-00000b10: 6368 696c 645f 6d6f 6475 6c65 7320 3d20  child_modules = 
-00000b20: 7b6b 3a20 7620 666f 7220 6b2c 2076 2069  {k: v for k, v i
-00000b30: 6e20 6d6f 6475 6c65 2e5f 7374 6174 652e  n module._state.
-00000b40: 6368 696c 6472 656e 2e69 7465 6d73 2829  children.items()
-00000b50: 2020 2320 7079 7479 7065 3a20 6469 7361    # pytype: disa
-00000b60: 626c 653d 6174 7472 6962 7574 652d 6572  ble=attribute-er
-00000b70: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
-00000b80: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00000b90: 616e 6365 2876 2c20 4d6f 6475 6c65 297d  ance(v, Module)}
-00000ba0: 0a20 2069 6620 6174 7472 6962 7574 6573  .  if attributes
-00000bb0: 3a0a 2020 2020 7265 7020 2b3d 2027 2320  :.    rep += '# 
-00000bc0: 6174 7472 6962 7574 6573 5c6e 270a 2020  attributes\n'.  
-00000bd0: 2020 666f 7220 6174 7472 2069 6e20 6174    for attr in at
-00000be0: 7472 6962 7574 6573 2e6b 6579 7328 293a  tributes.keys():
-00000bf0: 0a20 2020 2020 2023 2054 4f44 4f28 6a68  .      # TODO(jh
-00000c00: 6565 6b29 3a20 6361 6e20 7765 2067 6574  eek): can we get
-00000c10: 2061 206e 6963 6520 7374 7269 6e67 2072   a nice string r
-00000c20: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00000c30: 2061 7474 7269 6275 7465 2074 7970 6573   attribute types
-00000c40: 3f0a 2020 2020 2020 7661 6c75 6520 3d20  ?.      value = 
-00000c50: 6765 7461 7474 7228 6d6f 6475 6c65 2c20  getattr(module, 
-00000c60: 6174 7472 2c20 4e6f 6e65 290a 2020 2020  attr, None).    
-00000c70: 2020 7661 6c75 655f 7265 7020 3d20 5f61    value_rep = _a
-00000c80: 7474 725f 7265 7072 2876 616c 7565 290a  ttr_repr(value).
-00000c90: 2020 2020 2020 7265 7020 2b3d 2066 277b        rep += f'{
-00000ca0: 6174 7472 7d20 3d20 7b76 616c 7565 5f72  attr} = {value_r
-00000cb0: 6570 7d5c 6e27 0a20 2069 6620 6368 696c  ep}\n'.  if chil
-00000cc0: 645f 6d6f 6475 6c65 733a 0a20 2020 2072  d_modules:.    r
-00000cd0: 6570 202b 3d20 2723 2063 6869 6c64 7265  ep += '# childre
-00000ce0: 6e5c 6e27 0a20 2020 2066 6f72 206e 616d  n\n'.    for nam
-00000cf0: 652c 2063 6869 6c64 2069 6e20 6368 696c  e, child in chil
-00000d00: 645f 6d6f 6475 6c65 732e 6974 656d 7328  d_modules.items(
-00000d10: 293a 0a20 2020 2020 2063 6869 6c64 5f72  ):.      child_r
-00000d20: 6570 203d 205f 6d6f 6475 6c65 5f72 6570  ep = _module_rep
-00000d30: 7228 6368 696c 642c 206e 756d 5f73 7061  r(child, num_spa
-00000d40: 6365 7329 0a20 2020 2020 2072 6570 202b  ces).      rep +
-00000d50: 3d20 6627 7b6e 616d 657d 203d 207b 6368  = f'{name} = {ch
-00000d60: 696c 645f 7265 707d 5c6e 270a 2020 6966  ild_rep}\n'.  if
-00000d70: 2072 6570 3a0a 2020 2020 7265 7475 726e   rep:.    return
-00000d80: 2066 277b 636c 735f 6e61 6d65 7d28 5c6e   f'{cls_name}(\n
-00000d90: 7b5f 696e 6465 6e74 2872 6570 2c20 6e75  {_indent(rep, nu
-00000da0: 6d5f 7370 6163 6573 297d 2927 0a20 2065  m_spaces)})'.  e
-00000db0: 6c73 653a 0a20 2020 2072 6574 7572 6e20  lse:.    return 
-00000dc0: 6627 7b63 6c73 5f6e 616d 657d 2829 270a  f'{cls_name}()'.
-00000dd0: 0a23 2054 6162 756c 6174 696f 6e20 7574  .# Tabulation ut
-00000de0: 696c 6974 6965 732e 0a23 202d 2d2d 2d2d  ilities..# -----
-00000df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000002b0: 2072 650a 696d 706f 7274 2073 7973 0a69   re.import sys.i
+000002c0: 6d70 6f72 7420 7468 7265 6164 696e 670a  mport threading.
+000002d0: 696d 706f 7274 2074 7970 696e 670a 696d  import typing.im
+000002e0: 706f 7274 2077 6561 6b72 6566 0a66 726f  port weakref.fro
+000002f0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000300: 2841 6e79 2c20 4361 6c6c 6162 6c65 2c20  (Any, Callable, 
+00000310: 4469 6374 2c20 4974 6572 6162 6c65 2c20  Dict, Iterable, 
+00000320: 4c69 7374 2c20 5365 7175 656e 6365 2c20  List, Sequence, 
+00000330: 4e61 6d65 6454 7570 6c65 2c20 4d61 7070  NamedTuple, Mapp
+00000340: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+00000350: 2020 2020 2020 2020 204f 7074 696f 6e61           Optiona
+00000360: 6c2c 2053 6574 2c20 5475 706c 652c 2054  l, Set, Tuple, T
+00000370: 7970 652c 2054 7970 6556 6172 2c20 556e  ype, TypeVar, Un
+00000380: 696f 6e2c 206f 7665 726c 6f61 6429 0a0a  ion, overload)..
+00000390: 696d 706f 7274 206a 6178 0a69 6d70 6f72  import jax.impor
+000003a0: 7420 6e75 6d70 7920 6173 206e 700a 696d  t numpy as np.im
+000003b0: 706f 7274 206a 6178 2e6e 756d 7079 2061  port jax.numpy a
+000003c0: 7320 6a6e 700a 6672 6f6d 2074 7970 696e  s jnp.from typin
+000003d0: 675f 6578 7465 6e73 696f 6e73 2069 6d70  g_extensions imp
+000003e0: 6f72 7420 5072 6f74 6f63 6f6c 2c20 5c0a  ort Protocol, \.
+000003f0: 2020 6461 7461 636c 6173 735f 7472 616e    dataclass_tran
+00000400: 7366 6f72 6d20 2023 2070 7974 7970 653a  sform  # pytype:
+00000410: 2064 6973 6162 6c65 3d6e 6f74 2d73 7570   disable=not-sup
+00000420: 706f 7274 6564 2d79 6574 0a0a 696d 706f  ported-yet..impo
+00000430: 7274 2066 6c61 780a 6672 6f6d 2066 6c61  rt flax.from fla
+00000440: 7820 696d 706f 7274 2028 636f 6e66 6967  x import (config
+00000450: 2c20 636f 7265 2c20 6572 726f 7273 2c20  , core, errors, 
+00000460: 7365 7269 616c 697a 6174 696f 6e2c 2074  serialization, t
+00000470: 7261 6365 6261 636b 5f75 7469 6c2c 0a20  raceback_util,. 
+00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000490: 2074 7261 7665 7273 655f 7574 696c 290a   traverse_util).
+000004a0: 6672 6f6d 2066 6c61 782e 636f 7265 2069  from flax.core i
+000004b0: 6d70 6f72 7420 5363 6f70 650a 6672 6f6d  mport Scope.from
+000004c0: 2066 6c61 782e 636f 7265 2069 6d70 6f72   flax.core impor
+000004d0: 7420 7061 7274 6961 6c5f 6576 616c 0a66  t partial_eval.f
+000004e0: 726f 6d20 666c 6178 2e63 6f72 652e 6672  rom flax.core.fr
+000004f0: 6f7a 656e 5f64 6963 7420 696d 706f 7274  ozen_dict import
+00000500: 2046 726f 7a65 6e44 6963 740a 6672 6f6d   FrozenDict.from
+00000510: 2066 6c61 782e 636f 7265 2e73 636f 7065   flax.core.scope
+00000520: 2069 6d70 6f72 7420 2820 2023 2070 796c   import (  # pyl
+00000530: 696e 743a 2064 6973 6162 6c65 3d67 2d6d  int: disable=g-m
+00000540: 756c 7469 706c 652d 696d 706f 7274 0a20  ultiple-import. 
+00000550: 2020 2043 6f6c 6c65 6374 696f 6e46 696c     CollectionFil
+00000560: 7465 722c 2044 656e 794c 6973 742c 2046  ter, DenyList, F
+00000570: 726f 7a65 6e56 6172 6961 626c 6544 6963  rozenVariableDic
+00000580: 742c 2056 6172 6961 626c 652c 2056 6172  t, Variable, Var
+00000590: 6961 626c 6544 6963 742c 0a20 2020 2075  iableDict,.    u
+000005a0: 6e69 6f6e 5f66 696c 7465 7273 290a 6672  nion_filters).fr
+000005b0: 6f6d 2066 6c61 782e 6964 7320 696d 706f  om flax.ids impo
+000005c0: 7274 2046 6c61 7849 640a 6672 6f6d 2066  rt FlaxId.from f
+000005d0: 6c61 782e 6964 7320 696d 706f 7274 2075  lax.ids import u
+000005e0: 7569 640a 6672 6f6d 2066 6c61 782e 6c69  uid.from flax.li
+000005f0: 6e65 6e20 696d 706f 7274 206b 775f 6f6e  nen import kw_on
+00000600: 6c79 5f64 6174 6163 6c61 7373 6573 0a0a  ly_dataclasses..
+00000610: 0a74 7261 6365 6261 636b 5f75 7469 6c2e  .traceback_util.
+00000620: 7265 6769 7374 6572 5f65 7863 6c75 7369  register_exclusi
+00000630: 6f6e 285f 5f66 696c 655f 5f29 0a0a 5052  on(__file__)..PR
+00000640: 4e47 4b65 7920 3d20 416e 7920 2023 2070  NGKey = Any  # p
+00000650: 796c 696e 743a 2064 6973 6162 6c65 3d69  ylint: disable=i
+00000660: 6e76 616c 6964 2d6e 616d 650a 524e 4753  nvalid-name.RNGS
+00000670: 6571 7565 6e63 6573 203d 2044 6963 745b  equences = Dict[
+00000680: 7374 722c 2050 524e 474b 6579 5d0a 4172  str, PRNGKey].Ar
+00000690: 7261 7920 3d20 416e 7920 2020 2023 2070  ray = Any    # p
+000006a0: 796c 696e 743a 2064 6973 6162 6c65 3d69  ylint: disable=i
+000006b0: 6e76 616c 6964 2d6e 616d 650a 0a0a 5420  nvalid-name...T 
+000006c0: 3d20 5479 7065 5661 7228 2754 2729 0a4b  = TypeVar('T').K
+000006d0: 203d 2054 7970 6556 6172 2827 4b27 290a   = TypeVar('K').
+000006e0: 4d20 3d20 5479 7065 5661 7228 274d 272c  M = TypeVar('M',
+000006f0: 2062 6f75 6e64 3d27 4d6f 6475 6c65 2729   bound='Module')
+00000700: 0a5f 4361 6c6c 6162 6c65 5420 3d20 5479  ._CallableT = Ty
+00000710: 7065 5661 7228 275f 4361 6c6c 6162 6c65  peVar('_Callable
+00000720: 5427 2c20 626f 756e 643d 4361 6c6c 6162  T', bound=Callab
+00000730: 6c65 290a 0a0a 2320 5573 6564 2066 6f72  le)...# Used for
+00000740: 2061 6273 7472 6163 746c 7920 7465 7374   abstractly test
+00000750: 696e 6720 6d6f 6475 6c65 2062 6568 6176  ing module behav
+00000760: 696f 722e 0a54 6573 7453 636f 7065 203d  ior..TestScope =
+00000770: 2074 7970 6528 2754 6573 7453 636f 7065   type('TestScope
+00000780: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00000790: 2020 2020 2853 636f 7065 2c29 2c0a 2020      (Scope,),.  
+000007a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000007b0: 276d 616b 655f 726e 6727 3a20 6c61 6d62  'make_rng': lamb
+000007c0: 6461 2073 656c 662c 206e 616d 653a 206a  da self, name: j
+000007d0: 6178 2e72 616e 646f 6d2e 5052 4e47 4b65  ax.random.PRNGKe
+000007e0: 7928 3029 7d29 0a0a 0a23 2070 796c 696e  y(0)})...# pylin
+000007f0: 743a 2064 6973 6162 6c65 3d70 726f 7465  t: disable=prote
+00000800: 6374 6564 2d61 6363 6573 732c 6174 7472  cted-access,attr
+00000810: 6962 7574 652d 6465 6669 6e65 642d 6f75  ibute-defined-ou
+00000820: 7473 6964 652d 696e 6974 0a0a 6465 6620  tside-init..def 
+00000830: 5f69 6e64 656e 7428 783a 2073 7472 2c20  _indent(x: str, 
+00000840: 6e75 6d5f 7370 6163 6573 3a20 696e 7429  num_spaces: int)
+00000850: 3a0a 2020 696e 6465 6e74 5f73 7472 203d  :.  indent_str =
+00000860: 2027 2027 202a 206e 756d 5f73 7061 6365   ' ' * num_space
+00000870: 730a 2020 6c69 6e65 7320 3d20 782e 7370  s.  lines = x.sp
+00000880: 6c69 7428 275c 6e27 290a 2020 2320 736b  lit('\n').  # sk
+00000890: 6970 206c 6173 7420 6c69 6e65 2062 6563  ip last line bec
+000008a0: 6175 7365 2069 7420 6973 2061 6c77 6179  ause it is alway
+000008b0: 7320 656d 7074 7920 616e 6420 7368 6f75  s empty and shou
+000008c0: 6c64 206e 6f74 2062 6520 696e 6465 6e74  ld not be indent
+000008d0: 6564 2e0a 2020 6173 7365 7274 206e 6f74  ed..  assert not
+000008e0: 206c 696e 6573 5b2d 315d 0a20 2072 6574   lines[-1].  ret
+000008f0: 7572 6e20 275c 6e27 2e6a 6f69 6e28 696e  urn '\n'.join(in
+00000900: 6465 6e74 5f73 7472 202b 206c 696e 6520  dent_str + line 
+00000910: 666f 7220 6c69 6e65 2069 6e20 6c69 6e65  for line in line
+00000920: 735b 3a2d 315d 2920 2b20 275c 6e27 0a0a  s[:-1]) + '\n'..
+00000930: 0a64 6566 205f 6174 7472 5f72 6570 7228  .def _attr_repr(
+00000940: 7661 6c75 653a 2041 6e79 293a 0a20 2069  value: Any):.  i
+00000950: 6620 6361 6c6c 6162 6c65 2876 616c 7565  f callable(value
+00000960: 2920 616e 6420 6765 7461 7474 7228 7661  ) and getattr(va
+00000970: 6c75 652c 2027 5f5f 6e61 6d65 5f5f 272c  lue, '__name__',
+00000980: 204e 6f6e 6529 3a0a 2020 2020 7661 6c75   None):.    valu
+00000990: 655f 7265 7020 3d20 7661 6c75 652e 5f5f  e_rep = value.__
+000009a0: 6e61 6d65 5f5f 0a20 2065 6c73 653a 0a20  name__.  else:. 
+000009b0: 2020 2076 616c 7565 5f72 6570 203d 2072     value_rep = r
+000009c0: 6570 7228 7661 6c75 6529 0a20 2072 6574  epr(value).  ret
+000009d0: 7572 6e20 7661 6c75 655f 7265 700a 0a0a  urn value_rep...
+000009e0: 6465 6620 5f6d 6f64 756c 655f 7265 7072  def _module_repr
+000009f0: 286d 6f64 756c 653a 2027 4d6f 6475 6c65  (module: 'Module
+00000a00: 272c 206e 756d 5f73 7061 6365 733a 2069  ', num_spaces: i
+00000a10: 6e74 203d 2034 293a 0a20 2022 2222 5265  nt = 4):.  """Re
+00000a20: 7475 726e 7320 6120 7072 6574 7479 2070  turns a pretty p
+00000a30: 7269 6e74 6564 2072 6570 7265 7365 6e74  rinted represent
+00000a40: 6174 696f 6e20 6f66 2074 6865 206d 6f64  ation of the mod
+00000a50: 756c 652e 2222 220a 2020 636c 7320 3d20  ule.""".  cls = 
+00000a60: 7479 7065 286d 6f64 756c 6529 0a20 2063  type(module).  c
+00000a70: 6c73 5f6e 616d 6520 3d20 636c 732e 5f5f  ls_name = cls.__
+00000a80: 6e61 6d65 5f5f 0a20 2072 6570 203d 2027  name__.  rep = '
+00000a90: 270a 0a20 2061 7474 7269 6275 7465 7320  '..  attributes 
+00000aa0: 3d20 7b0a 2020 2020 2020 662e 6e61 6d65  = {.      f.name
+00000ab0: 3a20 662e 7479 7065 0a20 2020 2020 2066  : f.type.      f
+00000ac0: 6f72 2066 2069 6e20 6461 7461 636c 6173  or f in dataclas
+00000ad0: 7365 732e 6669 656c 6473 2863 6c73 290a  ses.fields(cls).
+00000ae0: 2020 2020 2020 6966 2066 2e6e 616d 6520        if f.name 
+00000af0: 6e6f 7420 696e 2028 2770 6172 656e 7427  not in ('parent'
+00000b00: 2c20 276e 616d 6527 2920 616e 6420 662e  , 'name') and f.
+00000b10: 7265 7072 0a20 207d 0a20 2063 6869 6c64  repr.  }.  child
+00000b20: 5f6d 6f64 756c 6573 203d 207b 6b3a 2076  _modules = {k: v
+00000b30: 2066 6f72 206b 2c20 7620 696e 206d 6f64   for k, v in mod
+00000b40: 756c 652e 5f73 7461 7465 2e63 6869 6c64  ule._state.child
+00000b50: 7265 6e2e 6974 656d 7328 2920 2023 2070  ren.items()  # p
+00000b60: 7974 7970 653a 2064 6973 6162 6c65 3d61  ytype: disable=a
+00000b70: 7474 7269 6275 7465 2d65 7272 6f72 0a20  ttribute-error. 
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00000ba0: 762c 204d 6f64 756c 6529 7d0a 2020 6966  v, Module)}.  if
+00000bb0: 2061 7474 7269 6275 7465 733a 0a20 2020   attributes:.   
+00000bc0: 2072 6570 202b 3d20 2723 2061 7474 7269   rep += '# attri
+00000bd0: 6275 7465 735c 6e27 0a20 2020 2066 6f72  butes\n'.    for
+00000be0: 2061 7474 7220 696e 2061 7474 7269 6275   attr in attribu
+00000bf0: 7465 732e 6b65 7973 2829 3a0a 2020 2020  tes.keys():.    
+00000c00: 2020 2320 544f 444f 286a 6865 656b 293a    # TODO(jheek):
+00000c10: 2063 616e 2077 6520 6765 7420 6120 6e69   can we get a ni
+00000c20: 6365 2073 7472 696e 6720 7265 7072 6573  ce string repres
+00000c30: 656e 7461 7469 6f6e 206f 6620 6174 7472  entation of attr
+00000c40: 6962 7574 6520 7479 7065 733f 0a20 2020  ibute types?.   
+00000c50: 2020 2076 616c 7565 203d 2067 6574 6174     value = getat
+00000c60: 7472 286d 6f64 756c 652c 2061 7474 722c  tr(module, attr,
+00000c70: 204e 6f6e 6529 0a20 2020 2020 2076 616c   None).      val
+00000c80: 7565 5f72 6570 203d 205f 6174 7472 5f72  ue_rep = _attr_r
+00000c90: 6570 7228 7661 6c75 6529 0a20 2020 2020  epr(value).     
+00000ca0: 2072 6570 202b 3d20 6627 7b61 7474 727d   rep += f'{attr}
+00000cb0: 203d 207b 7661 6c75 655f 7265 707d 5c6e   = {value_rep}\n
+00000cc0: 270a 2020 6966 2063 6869 6c64 5f6d 6f64  '.  if child_mod
+00000cd0: 756c 6573 3a0a 2020 2020 7265 7020 2b3d  ules:.    rep +=
+00000ce0: 2027 2320 6368 696c 6472 656e 5c6e 270a   '# children\n'.
+00000cf0: 2020 2020 666f 7220 6e61 6d65 2c20 6368      for name, ch
+00000d00: 696c 6420 696e 2063 6869 6c64 5f6d 6f64  ild in child_mod
+00000d10: 756c 6573 2e69 7465 6d73 2829 3a0a 2020  ules.items():.  
+00000d20: 2020 2020 6368 696c 645f 7265 7020 3d20      child_rep = 
+00000d30: 5f6d 6f64 756c 655f 7265 7072 2863 6869  _module_repr(chi
+00000d40: 6c64 2c20 6e75 6d5f 7370 6163 6573 290a  ld, num_spaces).
+00000d50: 2020 2020 2020 7265 7020 2b3d 2066 277b        rep += f'{
+00000d60: 6e61 6d65 7d20 3d20 7b63 6869 6c64 5f72  name} = {child_r
+00000d70: 6570 7d5c 6e27 0a20 2069 6620 7265 703a  ep}\n'.  if rep:
+00000d80: 0a20 2020 2072 6574 7572 6e20 6627 7b63  .    return f'{c
+00000d90: 6c73 5f6e 616d 657d 285c 6e7b 5f69 6e64  ls_name}(\n{_ind
+00000da0: 656e 7428 7265 702c 206e 756d 5f73 7061  ent(rep, num_spa
+00000db0: 6365 7329 7d29 270a 2020 656c 7365 3a0a  ces)})'.  else:.
+00000dc0: 2020 2020 7265 7475 726e 2066 277b 636c      return f'{cl
+00000dd0: 735f 6e61 6d65 7d28 2927 0a0a 2320 5461  s_name}()'..# Ta
+00000de0: 6275 6c61 7469 6f6e 2075 7469 6c69 7469  bulation utiliti
+00000df0: 6573 2e0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  es..# ----------
 00000e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e30: 2d2d 2d2d 2d2d 2d2d 0a0a 5f66 696e 645f  --------.._find_
-00000e40: 6e6f 6e5f 6c69 6674 6564 5f6d 6f64 756c  non_lifted_modul
-00000e50: 6520 3d20 7265 2e63 6f6d 7069 6c65 2872  e = re.compile(r
-00000e60: 272e 2a5c 2828 2e2a 295c 2927 290a 0a64  '.*\((.*)\)')..d
-00000e70: 6566 205f 6669 785f 7061 7468 5f70 6172  ef _fix_path_par
-00000e80: 7428 7061 7274 3a20 7374 7229 3a0a 2020  t(part: str):.  
-00000e90: 2222 2246 6978 6573 2061 2070 6174 6820  """Fixes a path 
-00000ea0: 7061 7274 2062 7920 7265 6d6f 7669 6e67  part by removing
-00000eb0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
-00000ec0: 6e61 6d65 2061 6e64 2070 6172 656e 7468  name and parenth
-00000ed0: 6573 6973 2073 6f6d 6574 696d 6573 0a20  esis sometimes. 
-00000ee0: 2069 6e73 6572 7465 6420 6279 206c 6966   inserted by lif
-00000ef0: 7465 6420 7472 616e 7366 6f72 6d61 7469  ted transformati
-00000f00: 6f6e 7322 2222 0a20 206d 6174 6368 203d  ons""".  match =
-00000f10: 205f 6669 6e64 5f6e 6f6e 5f6c 6966 7465   _find_non_lifte
-00000f20: 645f 6d6f 6475 6c65 2e6d 6174 6368 2870  d_module.match(p
-00000f30: 6172 7429 0a20 2069 6620 6d61 7463 683a  art).  if match:
-00000f40: 0a20 2020 2072 6574 7572 6e20 6d61 7463  .    return matc
-00000f50: 682e 6772 6f75 7028 3129 0a20 2072 6574  h.group(1).  ret
-00000f60: 7572 6e20 7061 7274 0a0a 4064 6174 6163  urn part..@datac
-00000f70: 6c61 7373 6573 2e64 6174 6163 6c61 7373  lasses.dataclass
-00000f80: 0a63 6c61 7373 205f 4361 6c6c 496e 666f  .class _CallInfo
-00000f90: 3a0a 2020 696e 6465 783a 2069 6e74 0a20  :.  index: int. 
-00000fa0: 2070 6174 683a 2054 7570 6c65 5b73 7472   path: Tuple[str
-00000fb0: 2c20 2e2e 2e5d 0a20 206d 6f64 756c 655f  , ...].  module_
-00000fc0: 7479 7065 3a20 5479 7065 5b27 4d6f 6475  type: Type['Modu
-00000fd0: 6c65 275d 0a20 206d 6574 686f 643a 2073  le'].  method: s
-00000fe0: 7472 0a20 2061 7267 733a 2054 7570 6c65  tr.  args: Tuple
-00000ff0: 5b41 6e79 2c20 2e2e 2e5d 0a20 206b 7761  [Any, ...].  kwa
-00001000: 7267 733a 2044 6963 745b 7374 722c 2041  rgs: Dict[str, A
-00001010: 6e79 5d0a 2020 6f75 7470 7574 733a 2041  ny].  outputs: A
-00001020: 6e79 0a0a 4064 6174 6163 6c61 7373 6573  ny..@dataclasses
-00001030: 2e64 6174 6163 6c61 7373 0a63 6c61 7373  .dataclass.class
-00001040: 205f 4361 6c6c 496e 666f 436f 6e74 6578   _CallInfoContex
-00001050: 7428 7468 7265 6164 696e 672e 6c6f 6361  t(threading.loca
-00001060: 6c29 3a0a 2020 696e 6465 783a 2069 6e74  l):.  index: int
-00001070: 0a20 2063 616c 6c73 3a20 4c69 7374 5b5f  .  calls: List[_
-00001080: 4361 6c6c 496e 666f 5d0a 0a20 2064 6566  CallInfo]..  def
-00001090: 2067 6574 5f63 616c 6c5f 696e 6465 7828   get_call_index(
-000010a0: 7365 6c66 2c20 6d6f 6475 6c65 3a20 274d  self, module: 'M
-000010b0: 6f64 756c 6527 2920 2d3e 2069 6e74 3a0a  odule') -> int:.
-000010c0: 2020 2020 696e 6465 7820 3d20 7365 6c66      index = self
-000010d0: 2e69 6e64 6578 0a20 2020 2073 656c 662e  .index.    self.
-000010e0: 696e 6465 7820 2b3d 2031 0a20 2020 2072  index += 1.    r
-000010f0: 6574 7572 6e20 696e 6465 780a 0a40 636f  eturn index..@co
-00001100: 6e74 6578 746c 6962 2e63 6f6e 7465 7874  ntextlib.context
-00001110: 6d61 6e61 6765 720a 6465 6620 5f74 6162  manager.def _tab
-00001120: 756c 6174 655f 636f 6e74 6578 7428 293a  ulate_context():
-00001130: 0a20 205f 636f 6e74 6578 742e 6361 6c6c  .  _context.call
-00001140: 5f69 6e66 6f5f 7374 6163 6b2e 6170 7065  _info_stack.appe
-00001150: 6e64 285f 4361 6c6c 496e 666f 436f 6e74  nd(_CallInfoCont
-00001160: 6578 7428 302c 205b 5d29 290a 2020 7472  ext(0, [])).  tr
-00001170: 793a 0a20 2020 2079 6965 6c64 0a20 2066  y:.    yield.  f
-00001180: 696e 616c 6c79 3a0a 2020 2020 5f63 6f6e  inally:.    _con
-00001190: 7465 7874 2e63 616c 6c5f 696e 666f 5f73  text.call_info_s
-000011a0: 7461 636b 2e70 6f70 2829 0a0a 2320 5472  tack.pop()..# Tr
-000011b0: 6163 6b20 7061 7265 6e74 2072 656c 6174  ack parent relat
-000011c0: 696f 6e73 6869 7020 6163 726f 7373 204d  ionship across M
-000011d0: 6f64 756c 6573 2e0a 2320 2d2d 2d2d 2d2d  odules..# ------
-000011e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e40: 2d2d 2d0a 0a5f 6669 6e64 5f6e 6f6e 5f6c  ---.._find_non_l
+00000e50: 6966 7465 645f 6d6f 6475 6c65 203d 2072  ifted_module = r
+00000e60: 652e 636f 6d70 696c 6528 7227 2e2a 5c28  e.compile(r'.*\(
+00000e70: 282e 2a29 5c29 2729 0a0a 6465 6620 5f66  (.*)\)')..def _f
+00000e80: 6978 5f70 6174 685f 7061 7274 2870 6172  ix_path_part(par
+00000e90: 743a 2073 7472 293a 0a20 2022 2222 4669  t: str):.  """Fi
+00000ea0: 7865 7320 6120 7061 7468 2070 6172 7420  xes a path part 
+00000eb0: 6279 2072 656d 6f76 696e 6720 7472 616e  by removing tran
+00000ec0: 7366 6f72 6d61 7469 6f6e 206e 616d 6520  sformation name 
+00000ed0: 616e 6420 7061 7265 6e74 6865 7369 7320  and parenthesis 
+00000ee0: 736f 6d65 7469 6d65 730a 2020 696e 7365  sometimes.  inse
+00000ef0: 7274 6564 2062 7920 6c69 6674 6564 2074  rted by lifted t
+00000f00: 7261 6e73 666f 726d 6174 696f 6e73 2222  ransformations""
+00000f10: 220a 2020 6d61 7463 6820 3d20 5f66 696e  ".  match = _fin
+00000f20: 645f 6e6f 6e5f 6c69 6674 6564 5f6d 6f64  d_non_lifted_mod
+00000f30: 756c 652e 6d61 7463 6828 7061 7274 290a  ule.match(part).
+00000f40: 2020 6966 206d 6174 6368 3a0a 2020 2020    if match:.    
+00000f50: 7265 7475 726e 206d 6174 6368 2e67 726f  return match.gro
+00000f60: 7570 2831 290a 2020 7265 7475 726e 2070  up(1).  return p
+00000f70: 6172 740a 0a40 6461 7461 636c 6173 7365  art..@dataclasse
+00000f80: 732e 6461 7461 636c 6173 730a 636c 6173  s.dataclass.clas
+00000f90: 7320 5f43 616c 6c49 6e66 6f3a 0a20 2069  s _CallInfo:.  i
+00000fa0: 6e64 6578 3a20 696e 740a 2020 7061 7468  ndex: int.  path
+00000fb0: 3a20 5475 706c 655b 7374 722c 202e 2e2e  : Tuple[str, ...
+00000fc0: 5d0a 2020 6d6f 6475 6c65 5f74 7970 653a  ].  module_type:
+00000fd0: 2054 7970 655b 274d 6f64 756c 6527 5d0a   Type['Module'].
+00000fe0: 2020 6d65 7468 6f64 3a20 7374 720a 2020    method: str.  
+00000ff0: 6172 6773 3a20 5475 706c 655b 416e 792c  args: Tuple[Any,
+00001000: 202e 2e2e 5d0a 2020 6b77 6172 6773 3a20   ...].  kwargs: 
+00001010: 4469 6374 5b73 7472 2c20 416e 795d 0a20  Dict[str, Any]. 
+00001020: 206f 7574 7075 7473 3a20 416e 790a 0a40   outputs: Any..@
+00001030: 6461 7461 636c 6173 7365 732e 6461 7461  dataclasses.data
+00001040: 636c 6173 730a 636c 6173 7320 5f43 616c  class.class _Cal
+00001050: 6c49 6e66 6f43 6f6e 7465 7874 2874 6872  lInfoContext(thr
+00001060: 6561 6469 6e67 2e6c 6f63 616c 293a 0a20  eading.local):. 
+00001070: 2069 6e64 6578 3a20 696e 740a 2020 6361   index: int.  ca
+00001080: 6c6c 733a 204c 6973 745b 5f43 616c 6c49  lls: List[_CallI
+00001090: 6e66 6f5d 0a0a 2020 6465 6620 6765 745f  nfo]..  def get_
+000010a0: 6361 6c6c 5f69 6e64 6578 2873 656c 662c  call_index(self,
+000010b0: 206d 6f64 756c 653a 2027 4d6f 6475 6c65   module: 'Module
+000010c0: 2729 202d 3e20 696e 743a 0a20 2020 2069  ') -> int:.    i
+000010d0: 6e64 6578 203d 2073 656c 662e 696e 6465  ndex = self.inde
+000010e0: 780a 2020 2020 7365 6c66 2e69 6e64 6578  x.    self.index
+000010f0: 202b 3d20 310a 2020 2020 7265 7475 726e   += 1.    return
+00001100: 2069 6e64 6578 0a0a 4063 6f6e 7465 7874   index..@context
+00001110: 6c69 622e 636f 6e74 6578 746d 616e 6167  lib.contextmanag
+00001120: 6572 0a64 6566 205f 7461 6275 6c61 7465  er.def _tabulate
+00001130: 5f63 6f6e 7465 7874 2829 3a0a 2020 5f63  _context():.  _c
+00001140: 6f6e 7465 7874 2e63 616c 6c5f 696e 666f  ontext.call_info
+00001150: 5f73 7461 636b 2e61 7070 656e 6428 5f43  _stack.append(_C
+00001160: 616c 6c49 6e66 6f43 6f6e 7465 7874 2830  allInfoContext(0
+00001170: 2c20 5b5d 2929 0a20 2074 7279 3a0a 2020  , [])).  try:.  
+00001180: 2020 7969 656c 640a 2020 6669 6e61 6c6c    yield.  finall
+00001190: 793a 0a20 2020 205f 636f 6e74 6578 742e  y:.    _context.
+000011a0: 6361 6c6c 5f69 6e66 6f5f 7374 6163 6b2e  call_info_stack.
+000011b0: 706f 7028 290a 0a23 2054 7261 636b 2070  pop()..# Track p
+000011c0: 6172 656e 7420 7265 6c61 7469 6f6e 7368  arent relationsh
+000011d0: 6970 2061 6372 6f73 7320 4d6f 6475 6c65  ip across Module
+000011e0: 732e 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  s..# -----------
 000011f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001220: 2d2d 2d2d 2d2d 2d0a 636c 6173 7320 5f44  -------.class _D
-00001230: 796e 616d 6963 436f 6e74 6578 7428 7468  ynamicContext(th
-00001240: 7265 6164 696e 672e 6c6f 6361 6c29 3a0a  reading.local):.
-00001250: 2020 2222 2244 796e 616d 6963 2063 6f6e    """Dynamic con
-00001260: 7465 7874 2e22 2222 0a20 2023 2054 4f44  text.""".  # TOD
-00001270: 4f28 6d61 7263 7661 6e7a 6565 293a 2073  O(marcvanzee): s
-00001280: 7769 7463 6820 746f 2075 7369 6e67 2063  witch to using c
-00001290: 6f6e 7465 7874 7661 7273 206f 6e63 6520  ontextvars once 
-000012a0: 6d69 6e69 6d75 6d20 7079 7468 6f6e 2076  minimum python v
-000012b0: 6572 7369 6f6e 2069 730a 2020 2320 332e  ersion is.  # 3.
-000012c0: 370a 0a20 2064 6566 205f 5f69 6e69 745f  7..  def __init_
-000012d0: 5f28 7365 6c66 293a 0a20 2020 2073 656c  _(self):.    sel
-000012e0: 662e 6d6f 6475 6c65 5f73 7461 636b 203d  f.module_stack =
-000012f0: 205b 4e6f 6e65 2c5d 0a20 2020 2073 656c   [None,].    sel
-00001300: 662e 6361 7074 7572 655f 7374 6163 6b20  f.capture_stack 
-00001310: 3d20 5b5d 0a20 2020 2073 656c 662e 6361  = [].    self.ca
-00001320: 6c6c 5f69 6e66 6f5f 7374 6163 6b20 3d20  ll_info_stack = 
-00001330: 5b5d 0a0a 2320 5468 6520 676c 6f62 616c  []..# The global
-00001340: 2063 6f6e 7465 7874 0a5f 636f 6e74 6578   context._contex
-00001350: 7420 3d20 5f44 796e 616d 6963 436f 6e74  t = _DynamicCont
-00001360: 6578 7428 290a 0a0a 636c 6173 7320 5f53  ext()...class _S
-00001370: 656e 7469 6e65 6c3a 0a0a 2020 6465 6620  entinel:..  def 
-00001380: 5f5f 636f 7079 5f5f 2873 656c 6629 3a0a  __copy__(self):.
-00001390: 2020 2020 7265 7475 726e 2073 656c 6620      return self 
-000013a0: 2023 2044 6f20 6e6f 7420 636f 7079 2073   # Do not copy s
-000013b0: 696e 676c 6574 6f6e 2073 656e 7469 6e65  ingleton sentine
-000013c0: 6c2e 0a0a 2020 6465 6620 5f5f 6465 6570  l...  def __deep
-000013d0: 636f 7079 5f5f 2873 656c 662c 206d 656d  copy__(self, mem
-000013e0: 6f29 3a0a 2020 2020 6465 6c20 6d65 6d6f  o):.    del memo
-000013f0: 0a20 2020 2072 6574 7572 6e20 7365 6c66  .    return self
-00001400: 2020 2320 446f 206e 6f74 2063 6f70 7920    # Do not copy 
-00001410: 7369 6e67 6c65 746f 6e20 7365 6e74 696e  singleton sentin
-00001420: 656c 2e0a 0a0a 5f75 6e73 7065 6369 6669  el...._unspecifi
-00001430: 6564 5f70 6172 656e 7420 3d20 5f53 656e  ed_parent = _Sen
-00001440: 7469 6e65 6c28 290a 0a0a 2320 456e 6162  tinel()...# Enab
-00001450: 6c65 2061 7574 6f6d 6174 6963 206e 616d  le automatic nam
-00001460: 6564 5f63 616c 6c20 7772 6170 7069 6e67  ed_call wrapping
-00001470: 2066 6f72 206c 6162 656c 6c69 6e67 2070   for labelling p
-00001480: 726f 6669 6c65 2074 7261 6365 732e 0a23  rofile traces..#
-00001490: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00001220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001230: 2d2d 0a63 6c61 7373 205f 4479 6e61 6d69  --.class _Dynami
+00001240: 6343 6f6e 7465 7874 2874 6872 6561 6469  cContext(threadi
+00001250: 6e67 2e6c 6f63 616c 293a 0a20 2022 2222  ng.local):.  """
+00001260: 4479 6e61 6d69 6320 636f 6e74 6578 742e  Dynamic context.
+00001270: 2222 220a 2020 2320 544f 444f 286d 6172  """.  # TODO(mar
+00001280: 6376 616e 7a65 6529 3a20 7377 6974 6368  cvanzee): switch
+00001290: 2074 6f20 7573 696e 6720 636f 6e74 6578   to using contex
+000012a0: 7476 6172 7320 6f6e 6365 206d 696e 696d  tvars once minim
+000012b0: 756d 2070 7974 686f 6e20 7665 7273 696f  um python versio
+000012c0: 6e20 6973 0a20 2023 2033 2e37 0a0a 2020  n is.  # 3.7..  
+000012d0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000012e0: 6629 3a0a 2020 2020 7365 6c66 2e6d 6f64  f):.    self.mod
+000012f0: 756c 655f 7374 6163 6b20 3d20 5b4e 6f6e  ule_stack = [Non
+00001300: 652c 5d0a 2020 2020 7365 6c66 2e63 6170  e,].    self.cap
+00001310: 7475 7265 5f73 7461 636b 203d 205b 5d0a  ture_stack = [].
+00001320: 2020 2020 7365 6c66 2e63 616c 6c5f 696e      self.call_in
+00001330: 666f 5f73 7461 636b 203d 205b 5d0a 0a23  fo_stack = []..#
+00001340: 2054 6865 2067 6c6f 6261 6c20 636f 6e74   The global cont
+00001350: 6578 740a 5f63 6f6e 7465 7874 203d 205f  ext._context = _
+00001360: 4479 6e61 6d69 6343 6f6e 7465 7874 2829  DynamicContext()
+00001370: 0a0a 0a63 6c61 7373 205f 5365 6e74 696e  ...class _Sentin
+00001380: 656c 3a0a 0a20 2064 6566 205f 5f63 6f70  el:..  def __cop
+00001390: 795f 5f28 7365 6c66 293a 0a20 2020 2072  y__(self):.    r
+000013a0: 6574 7572 6e20 7365 6c66 2020 2320 446f  eturn self  # Do
+000013b0: 206e 6f74 2063 6f70 7920 7369 6e67 6c65   not copy single
+000013c0: 746f 6e20 7365 6e74 696e 656c 2e0a 0a20  ton sentinel... 
+000013d0: 2064 6566 205f 5f64 6565 7063 6f70 795f   def __deepcopy_
+000013e0: 5f28 7365 6c66 2c20 6d65 6d6f 293a 0a20  _(self, memo):. 
+000013f0: 2020 2064 656c 206d 656d 6f0a 2020 2020     del memo.    
+00001400: 7265 7475 726e 2073 656c 6620 2023 2044  return self  # D
+00001410: 6f20 6e6f 7420 636f 7079 2073 696e 676c  o not copy singl
+00001420: 6574 6f6e 2073 656e 7469 6e65 6c2e 0a0a  eton sentinel...
+00001430: 0a5f 756e 7370 6563 6966 6965 645f 7061  ._unspecified_pa
+00001440: 7265 6e74 203d 205f 5365 6e74 696e 656c  rent = _Sentinel
+00001450: 2829 0a0a 0a23 2045 6e61 626c 6520 6175  ()...# Enable au
+00001460: 746f 6d61 7469 6320 6e61 6d65 645f 6361  tomatic named_ca
+00001470: 6c6c 2077 7261 7070 696e 6720 666f 7220  ll wrapping for 
+00001480: 6c61 6265 6c6c 696e 6720 7072 6f66 696c  labelling profil
+00001490: 6520 7472 6163 6573 2e0a 2320 2d2d 2d2d  e traces..# ----
 000014a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000014b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000014c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a5f  --------------._
-000014e0: 7573 655f 6e61 6d65 645f 6361 6c6c 203d  use_named_call =
-000014f0: 2063 6f6e 6669 672e 666c 6178 5f70 726f   config.flax_pro
-00001500: 6669 6c65 0a0a 0a64 6566 205f 6465 7269  file...def _deri
-00001510: 7665 5f70 726f 6669 6c69 6e67 5f6e 616d  ve_profiling_nam
-00001520: 6528 6d6f 6475 6c65 2c20 666e 293a 0a20  e(module, fn):. 
-00001530: 2064 6566 205f 6765 745f 666e 5f6e 616d   def _get_fn_nam
-00001540: 6528 666e 293a 0a20 2020 2069 6620 6973  e(fn):.    if is
-00001550: 696e 7374 616e 6365 2866 6e2c 2066 756e  instance(fn, fun
-00001560: 6374 6f6f 6c73 2e70 6172 7469 616c 293a  ctools.partial):
-00001570: 0a20 2020 2020 2072 6574 7572 6e20 5f67  .      return _g
-00001580: 6574 5f66 6e5f 6e61 6d65 2866 6e2e 6675  et_fn_name(fn.fu
-00001590: 6e63 290a 2020 2020 7265 7475 726e 2066  nc).    return f
-000015a0: 6e2e 5f5f 6e61 6d65 5f5f 0a20 2066 6e5f  n.__name__.  fn_
-000015b0: 6e61 6d65 203d 205f 6765 745f 666e 5f6e  name = _get_fn_n
-000015c0: 616d 6528 666e 290a 2020 6d65 7468 6f64  ame(fn).  method
-000015d0: 5f73 7566 6669 7820 3d20 6627 2e7b 666e  _suffix = f'.{fn
-000015e0: 5f6e 616d 657d 2720 6966 2066 6e5f 6e61  _name}' if fn_na
-000015f0: 6d65 2021 3d20 275f 5f63 616c 6c5f 5f27  me != '__call__'
-00001600: 2065 6c73 6520 2727 0a20 206d 6f64 756c   else ''.  modul
-00001610: 655f 6e61 6d65 203d 206d 6f64 756c 652e  e_name = module.
-00001620: 6e61 6d65 206f 7220 6d6f 6475 6c65 2e5f  name or module._
-00001630: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
-00001640: 5f0a 2020 7265 7475 726e 2066 277b 6d6f  _.  return f'{mo
-00001650: 6475 6c65 5f6e 616d 657d 7b6d 6574 686f  dule_name}{metho
-00001660: 645f 7375 6666 6978 7d27 0a0a 0a64 6566  d_suffix}'...def
-00001670: 2065 6e61 626c 655f 6e61 6d65 645f 6361   enable_named_ca
-00001680: 6c6c 2829 3a0a 2020 2222 2245 6e61 626c  ll():.  """Enabl
-00001690: 6573 206e 616d 6564 2063 616c 6c20 7772  es named call wr
-000016a0: 6170 7069 6e67 2066 6f72 206c 6162 656c  apping for label
-000016b0: 6c69 6e67 2070 726f 6669 6c65 2074 7261  ling profile tra
-000016c0: 6365 732e 0a0a 2020 5768 656e 206e 616d  ces...  When nam
-000016d0: 6564 2063 616c 6c20 7772 6170 7069 6e67  ed call wrapping
-000016e0: 2069 7320 656e 6162 6c65 6420 616c 6c20   is enabled all 
-000016f0: 4a41 5820 6f70 7320 6578 6563 7574 6564  JAX ops executed
-00001700: 2069 6e20 6120 4d6f 6475 6c65 0a20 2077   in a Module.  w
-00001710: 696c 6c20 6265 2072 756e 2075 6e64 6572  ill be run under
-00001720: 2060 606a 6178 2e6e 616d 6564 5f73 636f   ``jax.named_sco
-00001730: 7065 6060 2e20 5468 6520 6060 4d6f 6475  pe``. The ``Modu
-00001740: 6c65 6060 2063 6c61 7373 206e 616d 6520  le`` class name 
-00001750: 7769 6c6c 0a20 2073 686f 7720 7570 2061  will.  show up a
-00001760: 726f 756e 6420 7468 6520 6f70 6572 6174  round the operat
-00001770: 696f 6e73 2062 656c 6f6e 6769 6e67 2074  ions belonging t
-00001780: 6f20 7468 6174 204d 6f64 756c 6520 696e  o that Module in
-00001790: 2074 6865 0a20 2054 656e 736f 7262 6f61   the.  Tensorboa
-000017a0: 7264 2070 726f 6669 6c69 6e67 2055 492c  rd profiling UI,
-000017b0: 2073 696d 706c 6966 7969 6e67 2074 6865   simplifying the
-000017c0: 2070 726f 6669 6c69 6e67 2070 726f 6365   profiling proce
-000017d0: 7373 2e0a 0a20 204e 6f74 6520 7468 6174  ss...  Note that
-000017e0: 2060 606a 6178 2e6e 616d 6564 5f73 636f   ``jax.named_sco
-000017f0: 7065 6060 206f 6e6c 7920 776f 726b 7320  pe`` only works 
-00001800: 666f 720a 2020 636f 6d70 696c 6564 2066  for.  compiled f
-00001810: 756e 6374 696f 6e73 2028 652e 672e 3a20  unctions (e.g.: 
-00001820: 7573 696e 6720 6a61 782e 6a69 7420 6f72  using jax.jit or
-00001830: 206a 6178 2e70 6d61 7029 2e0a 2020 2222   jax.pmap)..  ""
-00001840: 220a 2020 676c 6f62 616c 205f 7573 655f  ".  global _use_
-00001850: 6e61 6d65 645f 6361 6c6c 0a20 205f 7573  named_call.  _us
-00001860: 655f 6e61 6d65 645f 6361 6c6c 203d 2054  e_named_call = T
-00001870: 7275 650a 0a0a 6465 6620 6469 7361 626c  rue...def disabl
-00001880: 655f 6e61 6d65 645f 6361 6c6c 2829 3a0a  e_named_call():.
-00001890: 2020 2222 2244 6973 6162 6c65 7320 6e61    """Disables na
-000018a0: 6d65 6420 6361 6c6c 2077 7261 7070 696e  med call wrappin
-000018b0: 672e 0a0a 2020 5365 6520 6060 656e 6162  g...  See ``enab
-000018c0: 6c65 5f6e 616d 6564 5f63 616c 6c60 600a  le_named_call``.
-000018d0: 2020 2222 220a 2020 676c 6f62 616c 205f    """.  global _
-000018e0: 7573 655f 6e61 6d65 645f 6361 6c6c 0a20  use_named_call. 
-000018f0: 205f 7573 655f 6e61 6d65 645f 6361 6c6c   _use_named_call
-00001900: 203d 2046 616c 7365 0a0a 0a40 636f 6e74   = False...@cont
-00001910: 6578 746c 6962 2e63 6f6e 7465 7874 6d61  extlib.contextma
-00001920: 6e61 6765 720a 6465 6620 6f76 6572 7269  nager.def overri
-00001930: 6465 5f6e 616d 6564 5f63 616c 6c28 656e  de_named_call(en
-00001940: 6162 6c65 3a20 626f 6f6c 203d 2054 7275  able: bool = Tru
-00001950: 6529 3a0a 2020 2320 7079 6c69 6e74 3a20  e):.  # pylint: 
-00001960: 6469 7361 626c 653d 672d 646f 632d 7265  disable=g-doc-re
-00001970: 7475 726e 2d6f 722d 7969 656c 640a 2020  turn-or-yield.  
-00001980: 2222 2252 6574 7572 6e73 2061 2063 6f6e  """Returns a con
-00001990: 7465 7874 206d 616e 6167 6572 2074 6861  text manager tha
-000019a0: 7420 656e 6162 6c65 732f 6469 7361 626c  t enables/disabl
-000019b0: 6573 206e 616d 6564 2063 616c 6c20 7772  es named call wr
-000019c0: 6170 7069 6e67 2e0a 0a20 2041 7267 733a  apping...  Args:
-000019d0: 0a20 2020 2065 6e61 626c 653a 2049 6620  .    enable: If 
-000019e0: 7472 7565 2c20 656e 6162 6c65 7320 6e61  true, enables na
-000019f0: 6d65 6420 6361 6c6c 2077 7261 7070 696e  med call wrappin
-00001a00: 6720 666f 7220 6c61 6265 6c6c 696e 6720  g for labelling 
-00001a10: 7072 6f66 696c 6520 7472 6163 6573 2e0a  profile traces..
-00001a20: 2020 2020 2020 2873 6565 2060 6065 6e61        (see ``ena
-00001a30: 626c 6564 5f6e 616d 6564 5f63 616c 6c60  bled_named_call`
-00001a40: 6029 2e0a 2020 2222 220a 2020 2320 7079  `)..  """.  # py
-00001a50: 6c69 6e74 3a20 656e 6162 6c65 3d67 2d64  lint: enable=g-d
-00001a60: 6f63 2d72 6574 7572 6e2d 6f72 2d79 6965  oc-return-or-yie
-00001a70: 6c64 0a20 2067 6c6f 6261 6c20 5f75 7365  ld.  global _use
-00001a80: 5f6e 616d 6564 5f63 616c 6c0a 2020 7573  _named_call.  us
-00001a90: 655f 6e61 6d65 645f 6361 6c6c 5f70 7265  e_named_call_pre
-00001aa0: 7620 3d20 5f75 7365 5f6e 616d 6564 5f63  v = _use_named_c
-00001ab0: 616c 6c0a 2020 5f75 7365 5f6e 616d 6564  all.  _use_named
-00001ac0: 5f63 616c 6c20 3d20 656e 6162 6c65 0a20  _call = enable. 
-00001ad0: 2074 7279 3a0a 2020 2020 7969 656c 640a   try:.    yield.
-00001ae0: 2020 6669 6e61 6c6c 793a 0a20 2020 205f    finally:.    _
-00001af0: 7573 655f 6e61 6d65 645f 6361 6c6c 203d  use_named_call =
-00001b00: 2075 7365 5f6e 616d 6564 5f63 616c 6c5f   use_named_call_
-00001b10: 7072 6576 0a0a 0a23 2055 7469 6c69 7469  prev...# Utiliti
-00001b20: 6573 2066 6f72 2070 7974 7265 6573 206f  es for pytrees o
-00001b30: 6620 4d6f 6475 6c65 7320 6465 6669 6e65  f Modules define
-00001b40: 6420 696e 7369 6465 2073 6574 7570 2829  d inside setup()
-00001b50: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
+000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014e0: 2d2d 2d2d 2d2d 2d2d 2d0a 5f75 7365 5f6e  ---------._use_n
+000014f0: 616d 6564 5f63 616c 6c20 3d20 636f 6e66  amed_call = conf
+00001500: 6967 2e66 6c61 785f 7072 6f66 696c 650a  ig.flax_profile.
+00001510: 0a0a 6465 6620 5f64 6572 6976 655f 7072  ..def _derive_pr
+00001520: 6f66 696c 696e 675f 6e61 6d65 286d 6f64  ofiling_name(mod
+00001530: 756c 652c 2066 6e29 3a0a 2020 6465 6620  ule, fn):.  def 
+00001540: 5f67 6574 5f66 6e5f 6e61 6d65 2866 6e29  _get_fn_name(fn)
+00001550: 3a0a 2020 2020 6966 2069 7369 6e73 7461  :.    if isinsta
+00001560: 6e63 6528 666e 2c20 6675 6e63 746f 6f6c  nce(fn, functool
+00001570: 732e 7061 7274 6961 6c29 3a0a 2020 2020  s.partial):.    
+00001580: 2020 7265 7475 726e 205f 6765 745f 666e    return _get_fn
+00001590: 5f6e 616d 6528 666e 2e66 756e 6329 0a20  _name(fn.func). 
+000015a0: 2020 2072 6574 7572 6e20 666e 2e5f 5f6e     return fn.__n
+000015b0: 616d 655f 5f0a 2020 666e 5f6e 616d 6520  ame__.  fn_name 
+000015c0: 3d20 5f67 6574 5f66 6e5f 6e61 6d65 2866  = _get_fn_name(f
+000015d0: 6e29 0a20 206d 6574 686f 645f 7375 6666  n).  method_suff
+000015e0: 6978 203d 2066 272e 7b66 6e5f 6e61 6d65  ix = f'.{fn_name
+000015f0: 7d27 2069 6620 666e 5f6e 616d 6520 213d  }' if fn_name !=
+00001600: 2027 5f5f 6361 6c6c 5f5f 2720 656c 7365   '__call__' else
+00001610: 2027 270a 2020 6d6f 6475 6c65 5f6e 616d   ''.  module_nam
+00001620: 6520 3d20 6d6f 6475 6c65 2e6e 616d 6520  e = module.name 
+00001630: 6f72 206d 6f64 756c 652e 5f5f 636c 6173  or module.__clas
+00001640: 735f 5f2e 5f5f 6e61 6d65 5f5f 0a20 2072  s__.__name__.  r
+00001650: 6574 7572 6e20 6627 7b6d 6f64 756c 655f  eturn f'{module_
+00001660: 6e61 6d65 7d7b 6d65 7468 6f64 5f73 7566  name}{method_suf
+00001670: 6669 787d 270a 0a0a 6465 6620 656e 6162  fix}'...def enab
+00001680: 6c65 5f6e 616d 6564 5f63 616c 6c28 293a  le_named_call():
+00001690: 0a20 2022 2222 456e 6162 6c65 7320 6e61  .  """Enables na
+000016a0: 6d65 6420 6361 6c6c 2077 7261 7070 696e  med call wrappin
+000016b0: 6720 666f 7220 6c61 6265 6c6c 696e 6720  g for labelling 
+000016c0: 7072 6f66 696c 6520 7472 6163 6573 2e0a  profile traces..
+000016d0: 0a20 2057 6865 6e20 6e61 6d65 6420 6361  .  When named ca
+000016e0: 6c6c 2077 7261 7070 696e 6720 6973 2065  ll wrapping is e
+000016f0: 6e61 626c 6564 2061 6c6c 204a 4158 206f  nabled all JAX o
+00001700: 7073 2065 7865 6375 7465 6420 696e 2061  ps executed in a
+00001710: 204d 6f64 756c 650a 2020 7769 6c6c 2062   Module.  will b
+00001720: 6520 7275 6e20 756e 6465 7220 6060 6a61  e run under ``ja
+00001730: 782e 6e61 6d65 645f 7363 6f70 6560 602e  x.named_scope``.
+00001740: 2054 6865 2060 604d 6f64 756c 6560 6020   The ``Module`` 
+00001750: 636c 6173 7320 6e61 6d65 2077 696c 6c0a  class name will.
+00001760: 2020 7368 6f77 2075 7020 6172 6f75 6e64    show up around
+00001770: 2074 6865 206f 7065 7261 7469 6f6e 7320   the operations 
+00001780: 6265 6c6f 6e67 696e 6720 746f 2074 6861  belonging to tha
+00001790: 7420 4d6f 6475 6c65 2069 6e20 7468 650a  t Module in the.
+000017a0: 2020 5465 6e73 6f72 626f 6172 6420 7072    Tensorboard pr
+000017b0: 6f66 696c 696e 6720 5549 2c20 7369 6d70  ofiling UI, simp
+000017c0: 6c69 6679 696e 6720 7468 6520 7072 6f66  lifying the prof
+000017d0: 696c 696e 6720 7072 6f63 6573 732e 0a0a  iling process...
+000017e0: 2020 4e6f 7465 2074 6861 7420 6060 6a61    Note that ``ja
+000017f0: 782e 6e61 6d65 645f 7363 6f70 6560 6020  x.named_scope`` 
+00001800: 6f6e 6c79 2077 6f72 6b73 2066 6f72 0a20  only works for. 
+00001810: 2063 6f6d 7069 6c65 6420 6675 6e63 7469   compiled functi
+00001820: 6f6e 7320 2865 2e67 2e3a 2075 7369 6e67  ons (e.g.: using
+00001830: 206a 6178 2e6a 6974 206f 7220 6a61 782e   jax.jit or jax.
+00001840: 706d 6170 292e 0a20 2022 2222 0a20 2067  pmap)..  """.  g
+00001850: 6c6f 6261 6c20 5f75 7365 5f6e 616d 6564  lobal _use_named
+00001860: 5f63 616c 6c0a 2020 5f75 7365 5f6e 616d  _call.  _use_nam
+00001870: 6564 5f63 616c 6c20 3d20 5472 7565 0a0a  ed_call = True..
+00001880: 0a64 6566 2064 6973 6162 6c65 5f6e 616d  .def disable_nam
+00001890: 6564 5f63 616c 6c28 293a 0a20 2022 2222  ed_call():.  """
+000018a0: 4469 7361 626c 6573 206e 616d 6564 2063  Disables named c
+000018b0: 616c 6c20 7772 6170 7069 6e67 2e0a 0a20  all wrapping... 
+000018c0: 2053 6565 2060 6065 6e61 626c 655f 6e61   See ``enable_na
+000018d0: 6d65 645f 6361 6c6c 6060 0a20 2022 2222  med_call``.  """
+000018e0: 0a20 2067 6c6f 6261 6c20 5f75 7365 5f6e  .  global _use_n
+000018f0: 616d 6564 5f63 616c 6c0a 2020 5f75 7365  amed_call.  _use
+00001900: 5f6e 616d 6564 5f63 616c 6c20 3d20 4661  _named_call = Fa
+00001910: 6c73 650a 0a0a 4063 6f6e 7465 7874 6c69  lse...@contextli
+00001920: 622e 636f 6e74 6578 746d 616e 6167 6572  b.contextmanager
+00001930: 0a64 6566 206f 7665 7272 6964 655f 6e61  .def override_na
+00001940: 6d65 645f 6361 6c6c 2865 6e61 626c 653a  med_call(enable:
+00001950: 2062 6f6f 6c20 3d20 5472 7565 293a 0a20   bool = True):. 
+00001960: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00001970: 6c65 3d67 2d64 6f63 2d72 6574 7572 6e2d  le=g-doc-return-
+00001980: 6f72 2d79 6965 6c64 0a20 2022 2222 5265  or-yield.  """Re
+00001990: 7475 726e 7320 6120 636f 6e74 6578 7420  turns a context 
+000019a0: 6d61 6e61 6765 7220 7468 6174 2065 6e61  manager that ena
+000019b0: 626c 6573 2f64 6973 6162 6c65 7320 6e61  bles/disables na
+000019c0: 6d65 6420 6361 6c6c 2077 7261 7070 696e  med call wrappin
+000019d0: 672e 0a0a 2020 4172 6773 3a0a 2020 2020  g...  Args:.    
+000019e0: 656e 6162 6c65 3a20 4966 2074 7275 652c  enable: If true,
+000019f0: 2065 6e61 626c 6573 206e 616d 6564 2063   enables named c
+00001a00: 616c 6c20 7772 6170 7069 6e67 2066 6f72  all wrapping for
+00001a10: 206c 6162 656c 6c69 6e67 2070 726f 6669   labelling profi
+00001a20: 6c65 2074 7261 6365 732e 0a20 2020 2020  le traces..     
+00001a30: 2028 7365 6520 6060 656e 6162 6c65 645f   (see ``enabled_
+00001a40: 6e61 6d65 645f 6361 6c6c 6060 292e 0a20  named_call``).. 
+00001a50: 2022 2222 0a20 2023 2070 796c 696e 743a   """.  # pylint:
+00001a60: 2065 6e61 626c 653d 672d 646f 632d 7265   enable=g-doc-re
+00001a70: 7475 726e 2d6f 722d 7969 656c 640a 2020  turn-or-yield.  
+00001a80: 676c 6f62 616c 205f 7573 655f 6e61 6d65  global _use_name
+00001a90: 645f 6361 6c6c 0a20 2075 7365 5f6e 616d  d_call.  use_nam
+00001aa0: 6564 5f63 616c 6c5f 7072 6576 203d 205f  ed_call_prev = _
+00001ab0: 7573 655f 6e61 6d65 645f 6361 6c6c 0a20  use_named_call. 
+00001ac0: 205f 7573 655f 6e61 6d65 645f 6361 6c6c   _use_named_call
+00001ad0: 203d 2065 6e61 626c 650a 2020 7472 793a   = enable.  try:
+00001ae0: 0a20 2020 2079 6965 6c64 0a20 2066 696e  .    yield.  fin
+00001af0: 616c 6c79 3a0a 2020 2020 5f75 7365 5f6e  ally:.    _use_n
+00001b00: 616d 6564 5f63 616c 6c20 3d20 7573 655f  amed_call = use_
+00001b10: 6e61 6d65 645f 6361 6c6c 5f70 7265 760a  named_call_prev.
+00001b20: 0a0a 2320 5574 696c 6974 6965 7320 666f  ..# Utilities fo
+00001b30: 7220 7079 7472 6565 7320 6f66 204d 6f64  r pytrees of Mod
+00001b40: 756c 6573 2064 6566 696e 6564 2069 6e73  ules defined ins
+00001b50: 6964 6520 7365 7475 7028 290a 2320 2d2d  ide setup().# --
 00001b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ba0: 0a0a 0a64 6566 205f 736f 7274 6564 5f69  ...def _sorted_i
-00001bb0: 7465 6d73 2878 293a 0a20 2022 2222 5265  tems(x):.  """Re
-00001bc0: 7475 726e 7320 6974 656d 7320 6f66 2061  turns items of a
-00001bd0: 2064 6963 7420 6f72 6465 7265 6420 6279   dict ordered by
-00001be0: 206b 6579 732e 2222 220a 2020 7265 7475   keys.""".  retu
-00001bf0: 726e 2073 6f72 7465 6428 782e 6974 656d  rn sorted(x.item
-00001c00: 7328 292c 206b 6579 3d6c 616d 6264 6120  s(), key=lambda 
-00001c10: 783a 2078 5b30 5d29 0a0a 0a64 6566 205f  x: x[0])...def _
-00001c20: 6765 745f 7375 6666 6978 5f76 616c 7565  get_suffix_value
-00001c30: 5f70 6169 7273 280a 2020 2020 7472 6565  _pairs(.    tree
-00001c40: 5f6f 725f 6c65 6166 3a20 416e 7929 202d  _or_leaf: Any) -
-00001c50: 3e20 4c69 7374 5b54 7570 6c65 5b73 7472  > List[Tuple[str
-00001c60: 2c20 5479 7065 5b27 4d6f 6475 6c65 275d  , Type['Module']
-00001c70: 5d5d 3a0a 2020 2222 2248 656c 7065 7220  ]]:.  """Helper 
-00001c80: 666f 7220 6e61 6d69 6e67 2070 7974 7265  for naming pytre
-00001c90: 6573 206f 6620 7375 626d 6f64 756c 6573  es of submodules
-00001ca0: 2e22 2222 0a20 2064 6963 745f 6f72 5f6c  .""".  dict_or_l
-00001cb0: 6561 6620 3d20 7365 7269 616c 697a 6174  eaf = serializat
-00001cc0: 696f 6e2e 746f 5f73 7461 7465 5f64 6963  ion.to_state_dic
-00001cd0: 7428 7472 6565 5f6f 725f 6c65 6166 290a  t(tree_or_leaf).
-00001ce0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00001cf0: 6e63 6528 6469 6374 5f6f 725f 6c65 6166  nce(dict_or_leaf
-00001d00: 2c20 6469 6374 2920 6f72 206e 6f74 2064  , dict) or not d
-00001d10: 6963 745f 6f72 5f6c 6561 663a 0a20 2020  ict_or_leaf:.   
-00001d20: 2072 6574 7572 6e20 5b28 2727 2c20 7472   return [('', tr
-00001d30: 6565 5f6f 725f 6c65 6166 295d 0a20 2065  ee_or_leaf)].  e
-00001d40: 6c73 653a 0a20 2020 2066 6c61 745f 6469  lse:.    flat_di
-00001d50: 6374 203d 2074 7261 7665 7273 655f 7574  ct = traverse_ut
-00001d60: 696c 2e66 6c61 7474 656e 5f64 6963 7428  il.flatten_dict(
-00001d70: 6469 6374 5f6f 725f 6c65 6166 290a 2020  dict_or_leaf).  
-00001d80: 2020 7265 7475 726e 205b 2827 5f27 202b    return [('_' +
-00001d90: 2027 5f27 2e6a 6f69 6e28 6b29 2c20 7629   '_'.join(k), v)
-00001da0: 2066 6f72 206b 2c20 7620 696e 205f 736f   for k, v in _so
-00001db0: 7274 6564 5f69 7465 6d73 2866 6c61 745f  rted_items(flat_
-00001dc0: 6469 6374 295d 0a0a 0a64 6566 205f 6d61  dict)]...def _ma
-00001dd0: 705f 6f76 6572 5f6d 6f64 756c 6573 5f69  p_over_modules_i
-00001de0: 6e5f 7472 6565 2866 6e2c 2074 7265 655f  n_tree(fn, tree_
-00001df0: 6f72 5f6c 6561 6629 3a0a 2020 2222 2248  or_leaf):.  """H
-00001e00: 656c 7065 7220 666f 7220 6d61 7070 696e  elper for mappin
-00001e10: 6720 6675 6e63 7469 6f6e 206f 7665 7220  g function over 
-00001e20: 7375 626d 6f64 756c 6573 2e22 2222 0a20  submodules.""". 
-00001e30: 2064 6963 745f 6f72 5f6c 6561 6620 3d20   dict_or_leaf = 
-00001e40: 7365 7269 616c 697a 6174 696f 6e2e 746f  serialization.to
-00001e50: 5f73 7461 7465 5f64 6963 7428 7472 6565  _state_dict(tree
-00001e60: 5f6f 725f 6c65 6166 290a 2020 6966 206e  _or_leaf).  if n
-00001e70: 6f74 2069 7369 6e73 7461 6e63 6528 6469  ot isinstance(di
-00001e80: 6374 5f6f 725f 6c65 6166 2c20 6469 6374  ct_or_leaf, dict
-00001e90: 2920 6f72 206e 6f74 2064 6963 745f 6f72  ) or not dict_or
-00001ea0: 5f6c 6561 663a 0a20 2020 2072 6574 7572  _leaf:.    retur
-00001eb0: 6e20 666e 2827 272c 2074 7265 655f 6f72  n fn('', tree_or
-00001ec0: 5f6c 6561 6629 0a20 2065 6c73 653a 0a20  _leaf).  else:. 
-00001ed0: 2020 2066 6c61 745f 6469 6374 203d 2074     flat_dict = t
-00001ee0: 7261 7665 7273 655f 7574 696c 2e66 6c61  raverse_util.fla
-00001ef0: 7474 656e 5f64 6963 7428 6469 6374 5f6f  tten_dict(dict_o
-00001f00: 725f 6c65 6166 2c20 6b65 6570 5f65 6d70  r_leaf, keep_emp
-00001f10: 7479 5f6e 6f64 6573 3d54 7275 6529 0a20  ty_nodes=True). 
-00001f20: 2020 206d 6170 7065 645f 666c 6174 5f64     mapped_flat_d
-00001f30: 6963 7420 3d20 7b6b 3a20 666e 2827 5f27  ict = {k: fn('_'
-00001f40: 202b 2027 5f27 2e6a 6f69 6e28 6b29 2c20   + '_'.join(k), 
-00001f50: 7629 0a20 2020 2020 2020 2020 2020 2020  v).             
-00001f60: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00001f70: 2c20 7620 696e 205f 736f 7274 6564 5f69  , v in _sorted_i
-00001f80: 7465 6d73 2866 6c61 745f 6469 6374 297d  tems(flat_dict)}
-00001f90: 0a20 2020 2072 6574 7572 6e20 7365 7269  .    return seri
-00001fa0: 616c 697a 6174 696f 6e2e 6672 6f6d 5f73  alization.from_s
-00001fb0: 7461 7465 5f64 6963 7428 0a20 2020 2020  tate_dict(.     
-00001fc0: 2020 2074 7265 655f 6f72 5f6c 6561 662c     tree_or_leaf,
-00001fd0: 2074 7261 7665 7273 655f 7574 696c 2e75   traverse_util.u
-00001fe0: 6e66 6c61 7474 656e 5f64 6963 7428 6d61  nflatten_dict(ma
-00001ff0: 7070 6564 5f66 6c61 745f 6469 6374 2929  pped_flat_dict))
-00002000: 0a0a 0a64 6566 205f 616c 6c5f 6e61 6d65  ...def _all_name
-00002010: 735f 6f6e 5f6f 626a 6563 7428 6f62 6a3a  s_on_object(obj:
-00002020: 2041 6e79 2920 2d3e 2053 6574 5b73 7472   Any) -> Set[str
-00002030: 5d3a 0a20 2022 2222 4765 7473 2061 6c6c  ]:.  """Gets all
-00002040: 206e 616d 6573 206f 6620 6174 7472 6962   names of attrib
-00002050: 7574 6573 206f 6e20 606f 626a 6020 616e  utes on `obj` an
-00002060: 6420 6974 7320 636c 6173 7365 7320 7468  d its classes th
-00002070: 726f 7567 686f 7574 204d 524f 2e0a 0a20  roughout MRO... 
-00002080: 2041 7267 733a 0a20 2020 206f 626a 3a20   Args:.    obj: 
-00002090: 5468 6520 6f62 6a65 6374 2074 6f20 6765  The object to ge
-000020a0: 7420 6e61 6d65 7320 666f 722e 0a20 2052  t names for..  R
-000020b0: 6574 7572 6e73 3a0a 2020 2020 4120 7365  eturns:.    A se
-000020c0: 7420 6f66 206e 616d 6573 206f 6620 6174  t of names of at
-000020d0: 7472 6962 7574 6573 206f 6620 606f 626a  tributes of `obj
-000020e0: 6020 616e 6420 6974 7320 636c 6173 7365  ` and its classe
-000020f0: 732e 0a20 2022 2222 0a20 206e 616d 6573  s..  """.  names
-00002100: 6574 203d 2073 6574 286f 626a 2e5f 5f64  et = set(obj.__d
-00002110: 6963 745f 5f2e 6b65 7973 2829 290a 2020  ict__.keys()).  
-00002120: 666f 7220 636c 7320 696e 206f 626a 2e5f  for cls in obj._
-00002130: 5f63 6c61 7373 5f5f 2e5f 5f6d 726f 5f5f  _class__.__mro__
-00002140: 3a0a 2020 2020 6e61 6d65 7365 7420 3d20  :.    nameset = 
-00002150: 6e61 6d65 7365 742e 756e 696f 6e28 7365  nameset.union(se
-00002160: 7428 636c 732e 5f5f 6469 6374 5f5f 2e6b  t(cls.__dict__.k
-00002170: 6579 7328 2929 290a 2020 7265 7475 726e  eys())).  return
-00002180: 206e 616d 6573 6574 0a0a 0a64 6566 205f   nameset...def _
-00002190: 6672 6565 7a65 5f61 7474 7228 7661 6c3a  freeze_attr(val:
-000021a0: 2041 6e79 2920 2d3e 2041 6e79 3a0a 2020   Any) -> Any:.  
-000021b0: 2222 2252 6563 7572 7369 7665 6c79 2077  """Recursively w
-000021c0: 7261 7020 7468 6520 6769 7665 6e20 6174  rap the given at
-000021d0: 7472 6962 7574 6520 6076 6172 6020 696e  tribute `var` in
-000021e0: 2060 6046 726f 7a65 6e44 6963 7460 602e   ``FrozenDict``.
-000021f0: 2222 220a 2020 6966 2069 7369 6e73 7461  """.  if isinsta
-00002200: 6e63 6528 7661 6c2c 2028 6469 6374 2c20  nce(val, (dict, 
-00002210: 4672 6f7a 656e 4469 6374 2929 3a0a 2020  FrozenDict)):.  
-00002220: 2020 7265 7475 726e 2046 726f 7a65 6e44    return FrozenD
-00002230: 6963 7428 7b6b 3a20 5f66 7265 657a 655f  ict({k: _freeze_
-00002240: 6174 7472 2876 2920 666f 7220 6b2c 2076  attr(v) for k, v
-00002250: 2069 6e20 7661 6c2e 6974 656d 7328 297d   in val.items()}
-00002260: 290a 2020 656c 6966 2069 7369 6e73 7461  ).  elif isinsta
-00002270: 6e63 6528 7661 6c2c 2074 7570 6c65 293a  nce(val, tuple):
-00002280: 0a20 2020 2023 2053 7065 6369 616c 2063  .    # Special c
-00002290: 6173 6520 6e61 6d65 6474 7570 6c65 7320  ase namedtuples 
-000022a0: 616e 6420 7370 6563 6961 6c20 4a41 5820  and special JAX 
-000022b0: 7475 706c 6520 7374 7275 6374 7572 6573  tuple structures
-000022c0: 206f 7468 6572 7769 7365 2074 6865 790a   otherwise they.
-000022d0: 2020 2020 2320 776f 756c 6420 6265 2064      # would be d
-000022e0: 6f77 6e67 7261 6465 6420 746f 206e 6f72  owngraded to nor
-000022f0: 6d61 6c20 7475 706c 6573 2e0a 2020 2020  mal tuples..    
-00002300: 6966 2068 6173 6174 7472 2876 616c 2c20  if hasattr(val, 
-00002310: 275f 6669 656c 6473 2729 206f 7220 7479  '_fields') or ty
-00002320: 7065 2876 616c 292e 5f5f 6e61 6d65 5f5f  pe(val).__name__
-00002330: 203d 3d20 2750 6172 7469 7469 6f6e 5370   == 'PartitionSp
-00002340: 6563 273a 0a20 2020 2020 2072 6574 7572  ec':.      retur
-00002350: 6e20 7479 7065 2876 616c 2928 2a5b 5f66  n type(val)(*[_f
-00002360: 7265 657a 655f 6174 7472 2876 2920 666f  reeze_attr(v) fo
-00002370: 7220 7620 696e 2076 616c 5d29 0a20 2020  r v in val]).   
-00002380: 2065 6c73 653a 0a20 2020 2020 2072 6574   else:.      ret
-00002390: 7572 6e20 7475 706c 6528 5f66 7265 657a  urn tuple(_freez
-000023a0: 655f 6174 7472 2876 2920 666f 7220 7620  e_attr(v) for v 
-000023b0: 696e 2076 616c 290a 2020 656c 6966 2069  in val).  elif i
-000023c0: 7369 6e73 7461 6e63 6528 7661 6c2c 206c  sinstance(val, l
-000023d0: 6973 7429 3a0a 2020 2020 7265 7475 726e  ist):.    return
-000023e0: 2074 7570 6c65 285f 6672 6565 7a65 5f61   tuple(_freeze_a
-000023f0: 7474 7228 7629 2066 6f72 2076 2069 6e20  ttr(v) for v in 
-00002400: 7661 6c29 0a20 2065 6c73 653a 0a20 2020  val).  else:.   
-00002410: 2072 6574 7572 6e20 7661 6c0a 0a0a 2320   return val...# 
-00002420: 4d65 7468 6f64 2077 7261 7070 696e 6720  Method wrapping 
-00002430: 6f66 2022 636f 6d70 6163 7420 6d65 7468  of "compact meth
-00002440: 6f64 7322 2061 6e64 2073 6574 7570 2829  ods" and setup()
-00002450: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
+00001ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a0a 6465  -----------...de
+00001bb0: 6620 5f73 6f72 7465 645f 6974 656d 7328  f _sorted_items(
+00001bc0: 7829 3a0a 2020 2222 2252 6574 7572 6e73  x):.  """Returns
+00001bd0: 2069 7465 6d73 206f 6620 6120 6469 6374   items of a dict
+00001be0: 206f 7264 6572 6564 2062 7920 6b65 7973   ordered by keys
+00001bf0: 2e22 2222 0a20 2072 6574 7572 6e20 736f  .""".  return so
+00001c00: 7274 6564 2878 2e69 7465 6d73 2829 2c20  rted(x.items(), 
+00001c10: 6b65 793d 6c61 6d62 6461 2078 3a20 785b  key=lambda x: x[
+00001c20: 305d 290a 0a0a 6465 6620 5f67 6574 5f73  0])...def _get_s
+00001c30: 7566 6669 785f 7661 6c75 655f 7061 6972  uffix_value_pair
+00001c40: 7328 0a20 2020 2074 7265 655f 6f72 5f6c  s(.    tree_or_l
+00001c50: 6561 663a 2041 6e79 2920 2d3e 204c 6973  eaf: Any) -> Lis
+00001c60: 745b 5475 706c 655b 7374 722c 2054 7970  t[Tuple[str, Typ
+00001c70: 655b 274d 6f64 756c 6527 5d5d 5d3a 0a20  e['Module']]]:. 
+00001c80: 2022 2222 4865 6c70 6572 2066 6f72 206e   """Helper for n
+00001c90: 616d 696e 6720 7079 7472 6565 7320 6f66  aming pytrees of
+00001ca0: 2073 7562 6d6f 6475 6c65 732e 2222 220a   submodules.""".
+00001cb0: 2020 6469 6374 5f6f 725f 6c65 6166 203d    dict_or_leaf =
+00001cc0: 2073 6572 6961 6c69 7a61 7469 6f6e 2e74   serialization.t
+00001cd0: 6f5f 7374 6174 655f 6469 6374 2874 7265  o_state_dict(tre
+00001ce0: 655f 6f72 5f6c 6561 6629 0a20 2069 6620  e_or_leaf).  if 
+00001cf0: 6e6f 7420 6973 696e 7374 616e 6365 2864  not isinstance(d
+00001d00: 6963 745f 6f72 5f6c 6561 662c 2064 6963  ict_or_leaf, dic
+00001d10: 7429 206f 7220 6e6f 7420 6469 6374 5f6f  t) or not dict_o
+00001d20: 725f 6c65 6166 3a0a 2020 2020 7265 7475  r_leaf:.    retu
+00001d30: 726e 205b 2827 272c 2074 7265 655f 6f72  rn [('', tree_or
+00001d40: 5f6c 6561 6629 5d0a 2020 656c 7365 3a0a  _leaf)].  else:.
+00001d50: 2020 2020 666c 6174 5f64 6963 7420 3d20      flat_dict = 
+00001d60: 7472 6176 6572 7365 5f75 7469 6c2e 666c  traverse_util.fl
+00001d70: 6174 7465 6e5f 6469 6374 2864 6963 745f  atten_dict(dict_
+00001d80: 6f72 5f6c 6561 6629 0a20 2020 2072 6574  or_leaf).    ret
+00001d90: 7572 6e20 5b28 275f 2720 2b20 275f 272e  urn [('_' + '_'.
+00001da0: 6a6f 696e 286b 292c 2076 2920 666f 7220  join(k), v) for 
+00001db0: 6b2c 2076 2069 6e20 5f73 6f72 7465 645f  k, v in _sorted_
+00001dc0: 6974 656d 7328 666c 6174 5f64 6963 7429  items(flat_dict)
+00001dd0: 5d0a 0a0a 6465 6620 5f6d 6170 5f6f 7665  ]...def _map_ove
+00001de0: 725f 6d6f 6475 6c65 735f 696e 5f74 7265  r_modules_in_tre
+00001df0: 6528 666e 2c20 7472 6565 5f6f 725f 6c65  e(fn, tree_or_le
+00001e00: 6166 293a 0a20 2022 2222 4865 6c70 6572  af):.  """Helper
+00001e10: 2066 6f72 206d 6170 7069 6e67 2066 756e   for mapping fun
+00001e20: 6374 696f 6e20 6f76 6572 2073 7562 6d6f  ction over submo
+00001e30: 6475 6c65 732e 2222 220a 2020 6469 6374  dules.""".  dict
+00001e40: 5f6f 725f 6c65 6166 203d 2073 6572 6961  _or_leaf = seria
+00001e50: 6c69 7a61 7469 6f6e 2e74 6f5f 7374 6174  lization.to_stat
+00001e60: 655f 6469 6374 2874 7265 655f 6f72 5f6c  e_dict(tree_or_l
+00001e70: 6561 6629 0a20 2069 6620 6e6f 7420 6973  eaf).  if not is
+00001e80: 696e 7374 616e 6365 2864 6963 745f 6f72  instance(dict_or
+00001e90: 5f6c 6561 662c 2064 6963 7429 206f 7220  _leaf, dict) or 
+00001ea0: 6e6f 7420 6469 6374 5f6f 725f 6c65 6166  not dict_or_leaf
+00001eb0: 3a0a 2020 2020 7265 7475 726e 2066 6e28  :.    return fn(
+00001ec0: 2727 2c20 7472 6565 5f6f 725f 6c65 6166  '', tree_or_leaf
+00001ed0: 290a 2020 656c 7365 3a0a 2020 2020 666c  ).  else:.    fl
+00001ee0: 6174 5f64 6963 7420 3d20 7472 6176 6572  at_dict = traver
+00001ef0: 7365 5f75 7469 6c2e 666c 6174 7465 6e5f  se_util.flatten_
+00001f00: 6469 6374 2864 6963 745f 6f72 5f6c 6561  dict(dict_or_lea
+00001f10: 662c 206b 6565 705f 656d 7074 795f 6e6f  f, keep_empty_no
+00001f20: 6465 733d 5472 7565 290a 2020 2020 6d61  des=True).    ma
+00001f30: 7070 6564 5f66 6c61 745f 6469 6374 203d  pped_flat_dict =
+00001f40: 207b 6b3a 2066 6e28 275f 2720 2b20 275f   {k: fn('_' + '_
+00001f50: 272e 6a6f 696e 286b 292c 2076 290a 2020  '.join(k), v).  
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 2020 666f 7220 6b2c 2076 2069        for k, v i
+00001f80: 6e20 5f73 6f72 7465 645f 6974 656d 7328  n _sorted_items(
+00001f90: 666c 6174 5f64 6963 7429 7d0a 2020 2020  flat_dict)}.    
+00001fa0: 7265 7475 726e 2073 6572 6961 6c69 7a61  return serializa
+00001fb0: 7469 6f6e 2e66 726f 6d5f 7374 6174 655f  tion.from_state_
+00001fc0: 6469 6374 280a 2020 2020 2020 2020 7472  dict(.        tr
+00001fd0: 6565 5f6f 725f 6c65 6166 2c20 7472 6176  ee_or_leaf, trav
+00001fe0: 6572 7365 5f75 7469 6c2e 756e 666c 6174  erse_util.unflat
+00001ff0: 7465 6e5f 6469 6374 286d 6170 7065 645f  ten_dict(mapped_
+00002000: 666c 6174 5f64 6963 7429 290a 0a0a 6465  flat_dict))...de
+00002010: 6620 5f61 6c6c 5f6e 616d 6573 5f6f 6e5f  f _all_names_on_
+00002020: 6f62 6a65 6374 286f 626a 3a20 416e 7929  object(obj: Any)
+00002030: 202d 3e20 5365 745b 7374 725d 3a0a 2020   -> Set[str]:.  
+00002040: 2222 2247 6574 7320 616c 6c20 6e61 6d65  """Gets all name
+00002050: 7320 6f66 2061 7474 7269 6275 7465 7320  s of attributes 
+00002060: 6f6e 2060 6f62 6a60 2061 6e64 2069 7473  on `obj` and its
+00002070: 2063 6c61 7373 6573 2074 6872 6f75 6768   classes through
+00002080: 6f75 7420 4d52 4f2e 0a0a 2020 4172 6773  out MRO...  Args
+00002090: 3a0a 2020 2020 6f62 6a3a 2054 6865 206f  :.    obj: The o
+000020a0: 626a 6563 7420 746f 2067 6574 206e 616d  bject to get nam
+000020b0: 6573 2066 6f72 2e0a 2020 5265 7475 726e  es for..  Return
+000020c0: 733a 0a20 2020 2041 2073 6574 206f 6620  s:.    A set of 
+000020d0: 6e61 6d65 7320 6f66 2061 7474 7269 6275  names of attribu
+000020e0: 7465 7320 6f66 2060 6f62 6a60 2061 6e64  tes of `obj` and
+000020f0: 2069 7473 2063 6c61 7373 6573 2e0a 2020   its classes..  
+00002100: 2222 220a 2020 6e61 6d65 7365 7420 3d20  """.  nameset = 
+00002110: 7365 7428 6f62 6a2e 5f5f 6469 6374 5f5f  set(obj.__dict__
+00002120: 2e6b 6579 7328 2929 0a20 2066 6f72 2063  .keys()).  for c
+00002130: 6c73 2069 6e20 6f62 6a2e 5f5f 636c 6173  ls in obj.__clas
+00002140: 735f 5f2e 5f5f 6d72 6f5f 5f3a 0a20 2020  s__.__mro__:.   
+00002150: 206e 616d 6573 6574 203d 206e 616d 6573   nameset = names
+00002160: 6574 2e75 6e69 6f6e 2873 6574 2863 6c73  et.union(set(cls
+00002170: 2e5f 5f64 6963 745f 5f2e 6b65 7973 2829  .__dict__.keys()
+00002180: 2929 0a20 2072 6574 7572 6e20 6e61 6d65  )).  return name
+00002190: 7365 740a 0a0a 6465 6620 5f66 7265 657a  set...def _freez
+000021a0: 655f 6174 7472 2876 616c 3a20 416e 7929  e_attr(val: Any)
+000021b0: 202d 3e20 416e 793a 0a20 2022 2222 5265   -> Any:.  """Re
+000021c0: 6375 7273 6976 656c 7920 7772 6170 2074  cursively wrap t
+000021d0: 6865 2067 6976 656e 2061 7474 7269 6275  he given attribu
+000021e0: 7465 2060 7661 7260 2069 6e20 6060 4672  te `var` in ``Fr
+000021f0: 6f7a 656e 4469 6374 6060 2e22 2222 0a20  ozenDict``.""". 
+00002200: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
+00002210: 616c 2c20 2864 6963 742c 2046 726f 7a65  al, (dict, Froze
+00002220: 6e44 6963 7429 293a 0a20 2020 2072 6574  nDict)):.    ret
+00002230: 7572 6e20 4672 6f7a 656e 4469 6374 287b  urn FrozenDict({
+00002240: 6b3a 205f 6672 6565 7a65 5f61 7474 7228  k: _freeze_attr(
+00002250: 7629 2066 6f72 206b 2c20 7620 696e 2076  v) for k, v in v
+00002260: 616c 2e69 7465 6d73 2829 7d29 0a20 2065  al.items()}).  e
+00002270: 6c69 6620 6973 696e 7374 616e 6365 2876  lif isinstance(v
+00002280: 616c 2c20 7475 706c 6529 3a0a 2020 2020  al, tuple):.    
+00002290: 2320 5370 6563 6961 6c20 6361 7365 206e  # Special case n
+000022a0: 616d 6564 7475 706c 6573 2061 6e64 2073  amedtuples and s
+000022b0: 7065 6369 616c 204a 4158 2074 7570 6c65  pecial JAX tuple
+000022c0: 2073 7472 7563 7475 7265 7320 6f74 6865   structures othe
+000022d0: 7277 6973 6520 7468 6579 0a20 2020 2023  rwise they.    #
+000022e0: 2077 6f75 6c64 2062 6520 646f 776e 6772   would be downgr
+000022f0: 6164 6564 2074 6f20 6e6f 726d 616c 2074  aded to normal t
+00002300: 7570 6c65 732e 0a20 2020 2069 6620 6861  uples..    if ha
+00002310: 7361 7474 7228 7661 6c2c 2027 5f66 6965  sattr(val, '_fie
+00002320: 6c64 7327 2920 6f72 2074 7970 6528 7661  lds') or type(va
+00002330: 6c29 2e5f 5f6e 616d 655f 5f20 3d3d 2027  l).__name__ == '
+00002340: 5061 7274 6974 696f 6e53 7065 6327 3a0a  PartitionSpec':.
+00002350: 2020 2020 2020 7265 7475 726e 2074 7970        return typ
+00002360: 6528 7661 6c29 282a 5b5f 6672 6565 7a65  e(val)(*[_freeze
+00002370: 5f61 7474 7228 7629 2066 6f72 2076 2069  _attr(v) for v i
+00002380: 6e20 7661 6c5d 290a 2020 2020 656c 7365  n val]).    else
+00002390: 3a0a 2020 2020 2020 7265 7475 726e 2074  :.      return t
+000023a0: 7570 6c65 285f 6672 6565 7a65 5f61 7474  uple(_freeze_att
+000023b0: 7228 7629 2066 6f72 2076 2069 6e20 7661  r(v) for v in va
+000023c0: 6c29 0a20 2065 6c69 6620 6973 696e 7374  l).  elif isinst
+000023d0: 616e 6365 2876 616c 2c20 6c69 7374 293a  ance(val, list):
+000023e0: 0a20 2020 2072 6574 7572 6e20 7475 706c  .    return tupl
+000023f0: 6528 5f66 7265 657a 655f 6174 7472 2876  e(_freeze_attr(v
+00002400: 2920 666f 7220 7620 696e 2076 616c 290a  ) for v in val).
+00002410: 2020 656c 7365 3a0a 2020 2020 7265 7475    else:.    retu
+00002420: 726e 2076 616c 0a0a 0a23 204d 6574 686f  rn val...# Metho
+00002430: 6420 7772 6170 7069 6e67 206f 6620 2263  d wrapping of "c
+00002440: 6f6d 7061 6374 206d 6574 686f 6473 2220  ompact methods" 
+00002450: 616e 6420 7365 7475 7028 290a 2320 2d2d  and setup().# --
 00002460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024a0: 0a64 6566 2063 6f6d 7061 6374 2866 756e  .def compact(fun
-000024b0: 3a20 5f43 616c 6c61 626c 6554 2920 2d3e  : _CallableT) ->
-000024c0: 205f 4361 6c6c 6162 6c65 543a 0a20 2022   _CallableT:.  "
-000024d0: 2222 4d61 726b 7320 7468 6520 6769 7665  ""Marks the give
-000024e0: 6e20 6d6f 6475 6c65 206d 6574 686f 6420  n module method 
-000024f0: 616c 6c6f 7769 6e67 2069 6e6c 696e 6564  allowing inlined
-00002500: 2073 7562 6d6f 6475 6c65 732e 0a0a 2020   submodules...  
-00002510: 4d65 7468 6f64 7320 7772 6170 7065 6420  Methods wrapped 
-00002520: 696e 2040 636f 6d70 6163 7420 6361 6e20  in @compact can 
-00002530: 6465 6669 6e65 2073 7562 6d6f 6475 6c65  define submodule
-00002540: 7320 6469 7265 6374 6c79 2077 6974 6869  s directly withi
-00002550: 6e20 7468 6520 6d65 7468 6f64 2e0a 0a20  n the method... 
-00002560: 2046 6f72 2069 6e73 7461 6e63 653a 3a0a   For instance::.
-00002570: 0a20 2020 2040 636f 6d70 6163 740a 2020  .    @compact.  
-00002580: 2020 5f5f 6361 6c6c 5f5f 2873 656c 662c    __call__(self,
-00002590: 2078 2c20 6665 6174 7572 6573 293a 0a20   x, features):. 
-000025a0: 2020 2020 2078 203d 206e 6e2e 4465 6e73       x = nn.Dens
-000025b0: 6528 6665 6174 7572 6573 2928 7829 0a20  e(features)(x). 
-000025c0: 2020 2020 202e 2e2e 0a0a 2020 4174 206d       .....  At m
-000025d0: 6f73 7420 6f6e 6520 6d65 7468 6f64 2069  ost one method i
-000025e0: 6e20 6561 6368 204d 6f64 756c 6520 6d61  n each Module ma
-000025f0: 7920 6265 2077 7261 7070 6564 2077 6974  y be wrapped wit
-00002600: 6820 4063 6f6d 7061 6374 2e0a 0a20 2041  h @compact...  A
-00002610: 7267 733a 0a20 2020 2066 756e 3a20 5468  rgs:.    fun: Th
-00002620: 6520 4d6f 6475 6c65 206d 6574 686f 6420  e Module method 
-00002630: 746f 206d 6172 6b20 6173 2063 6f6d 7061  to mark as compa
-00002640: 6374 2e0a 2020 5265 7475 726e 733a 0a20  ct..  Returns:. 
-00002650: 2020 2054 6865 2067 6976 656e 2066 756e     The given fun
-00002660: 6374 696f 6e20 6066 756e 6020 6d61 726b  ction `fun` mark
-00002670: 6564 2061 7320 636f 6d70 6163 742e 0a20  ed as compact.. 
-00002680: 2022 2222 0a20 2066 756e 2e63 6f6d 7061   """.  fun.compa
-00002690: 6374 203d 2054 7275 6520 2023 2074 7970  ct = True  # typ
-000026a0: 653a 2069 676e 6f72 655b 6174 7472 2d64  e: ignore[attr-d
-000026b0: 6566 696e 6564 5d0a 2020 7265 7475 726e  efined].  return
-000026c0: 2066 756e 0a0a 0a64 6566 206e 6f77 7261   fun...def nowra
-000026d0: 7028 6675 6e3a 205f 4361 6c6c 6162 6c65  p(fun: _Callable
-000026e0: 5429 202d 3e20 5f43 616c 6c61 626c 6554  T) -> _CallableT
-000026f0: 3a0a 2020 2222 224d 6172 6b73 2074 6865  :.  """Marks the
-00002700: 2067 6976 656e 206d 6f64 756c 6520 6d65   given module me
-00002710: 7468 6f64 2061 7320 6120 6865 6c70 6572  thod as a helper
-00002720: 206d 6574 686f 6420 7468 6174 206e 6565   method that nee
-00002730: 646e 2774 2062 6520 7772 6170 7065 642e  dn't be wrapped.
-00002740: 0a0a 2020 4d65 7468 6f64 7320 7772 6170  ..  Methods wrap
-00002750: 7065 6420 696e 2040 6e6f 7772 6170 2061  ped in @nowrap a
-00002760: 7265 2070 7269 7661 7465 2068 656c 7065  re private helpe
-00002770: 7220 6d65 7468 6f64 7320 7468 6174 206e  r methods that n
-00002780: 6565 646e 2774 2062 6520 7772 6170 7065  eedn't be wrappe
-00002790: 640a 2020 7769 7468 2074 6865 2073 7461  d.  with the sta
-000027a0: 7465 2068 616e 646c 6572 206f 7220 6120  te handler or a 
-000027b0: 7365 7061 7261 7465 206e 616d 6564 5f63  separate named_c
-000027c0: 616c 6c20 7472 616e 7366 6f72 6d2e 0a0a  all transform...
-000027d0: 2020 5468 6973 2069 7320 6e65 6564 6564    This is needed
-000027e0: 2069 6e20 7365 7665 7261 6c20 636f 6e63   in several conc
-000027f0: 7265 7465 2069 6e73 7461 6e63 6573 3a0a  rete instances:.
-00002800: 2020 202d 2069 6620 796f 7527 7265 2073     - if you're s
-00002810: 7562 636c 6173 7369 6e67 2061 206d 6574  ubclassing a met
-00002820: 686f 6420 6c69 6b65 204d 6f64 756c 652e  hod like Module.
-00002830: 7061 7261 6d20 616e 6420 646f 6e27 7420  param and don't 
-00002840: 7761 6e74 2074 6869 730a 2020 2020 206f  want this.     o
-00002850: 7665 7272 6964 656e 2063 6f72 6520 6675  verriden core fu
-00002860: 6e63 7469 6f6e 2064 6563 6f72 6174 6564  nction decorated
-00002870: 2077 6974 6820 7468 6520 7374 6174 6520   with the state 
-00002880: 6d61 6e61 6765 6d65 6e74 2077 7261 7070  management wrapp
-00002890: 6572 2e0a 2020 202d 2049 6620 796f 7520  er..   - If you 
-000028a0: 7761 6e74 2061 206d 6574 686f 6420 746f  want a method to
-000028b0: 2062 6520 6361 6c6c 6162 6c65 2066 726f   be callable fro
-000028c0: 6d20 616e 2075 6e62 6f75 6e64 204d 6f64  m an unbound Mod
-000028d0: 756c 6520 2865 2e67 2e3a 2061 0a20 2020  ule (e.g.: a.   
-000028e0: 2020 6675 6e63 7469 6f6e 206f 6620 636f    function of co
-000028f0: 6e73 7472 7563 7469 6f6e 206f 6620 6172  nstruction of ar
-00002900: 6775 6d65 6e74 7320 7468 6174 2064 6f65  guments that doe
-00002910: 736e 2774 2064 6570 656e 6420 6f6e 2070  sn't depend on p
-00002920: 6172 616d 732f 524e 4773 290a 0a20 2046  arams/RNGs)..  F
-00002930: 6f72 2069 6e73 7461 6e63 653a 3a0a 0a20  or instance::.. 
-00002940: 2020 2040 6e6f 7772 6170 0a20 2020 2064     @nowrap.    d
-00002950: 6566 205f 6d61 6b65 5f64 656e 7365 2873  ef _make_dense(s
-00002960: 656c 662c 206e 756d 5f66 6561 7475 7265  elf, num_feature
-00002970: 7329 3a0a 2020 2020 2020 7265 7475 726e  s):.      return
-00002980: 206e 6e2e 4465 6e73 6528 6e75 6d5f 6665   nn.Dense(num_fe
-00002990: 6174 7572 6573 290a 0a20 2020 2040 636f  atures)..    @co
-000029a0: 6d70 6163 740a 2020 2020 6465 6620 5f5f  mpact.    def __
-000029b0: 6361 6c6c 5f5f 2873 656c 662c 2078 293a  call__(self, x):
-000029c0: 0a20 2020 2020 2023 206e 6f77 2073 6166  .      # now saf
-000029d0: 6520 746f 2075 7365 2063 6f6e 7374 7275  e to use constru
-000029e0: 6374 6f72 2068 656c 7065 7220 6576 656e  ctor helper even
-000029f0: 2069 6620 7573 696e 6720 6e61 6d65 645f   if using named_
-00002a00: 6361 6c6c 0a20 2020 2020 2064 656e 7365  call.      dense
-00002a10: 203d 2073 656c 662e 5f6d 616b 655f 6465   = self._make_de
-00002a20: 6e73 6528 7365 6c66 2e6e 756d 5f66 6561  nse(self.num_fea
-00002a30: 7475 7265 7329 0a20 2020 2020 2072 6574  tures).      ret
-00002a40: 7572 6e20 6465 6e73 6528 7829 0a0a 2020  urn dense(x)..  
-00002a50: 4172 6773 3a0a 2020 2020 6675 6e3a 2054  Args:.    fun: T
-00002a60: 6865 204d 6f64 756c 6520 6d65 7468 6f64  he Module method
-00002a70: 2074 6f20 6d61 726b 2061 7320 6e6f 7772   to mark as nowr
-00002a80: 6170 2e0a 2020 5265 7475 726e 733a 0a20  ap..  Returns:. 
-00002a90: 2020 2054 6865 2067 6976 656e 2066 756e     The given fun
-00002aa0: 6374 696f 6e20 6066 756e 6020 6d61 726b  ction `fun` mark
-00002ab0: 6564 2061 7320 6e6f 7772 6170 2e0a 2020  ed as nowrap..  
-00002ac0: 2222 220a 2020 6675 6e2e 6e6f 7772 6170  """.  fun.nowrap
-00002ad0: 203d 2054 7275 6520 2023 2074 7970 653a   = True  # type:
-00002ae0: 2069 676e 6f72 655b 6174 7472 2d64 6566   ignore[attr-def
-00002af0: 696e 6564 5d0a 2020 7265 7475 726e 2066  ined].  return f
-00002b00: 756e 0a0a 0a64 6566 205f 6765 745f 6c6f  un...def _get_lo
-00002b10: 6361 6c5f 6d65 7468 6f64 5f6e 616d 6573  cal_method_names
-00002b20: 2863 6c73 3a20 416e 792c 0a20 2020 2020  (cls: Any,.     
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2065 7863 6c75 6465 3a20         exclude: 
-00002b50: 4974 6572 6162 6c65 5b73 7472 5d20 3d20  Iterable[str] = 
-00002b60: 2829 2920 2d3e 2054 7570 6c65 5b73 7472  ()) -> Tuple[str
-00002b70: 2c20 2e2e 2e5d 3a0a 2020 2222 2247 6574  , ...]:.  """Get
-00002b80: 7320 6d65 7468 6f64 206e 616d 6573 206f  s method names o
-00002b90: 6620 6120 636c 6173 732c 2065 7863 6c75  f a class, exclu
-00002ba0: 6469 6e67 2063 6c61 7373 2061 6e64 2073  ding class and s
-00002bb0: 7461 7469 6320 6d65 7468 6f64 732e 0a0a  tatic methods...
-00002bc0: 2020 4172 6773 3a0a 2020 2020 636c 733a    Args:.    cls:
-00002bd0: 2054 6865 2063 6c61 7373 2074 6f20 6765   The class to ge
-00002be0: 7420 6d65 7468 6f64 206e 616d 6573 2066  t method names f
-00002bf0: 6f72 2e0a 2020 2020 6578 636c 7564 653a  or..    exclude:
-00002c00: 204e 616d 6573 2074 6f20 6578 636c 7564   Names to exclud
-00002c10: 6520 6672 6f6d 206f 7574 7075 742e 0a20  e from output.. 
-00002c20: 2052 6574 7572 6e73 3a0a 2020 2020 4120   Returns:.    A 
-00002c30: 6c69 7374 206f 6620 6d65 7468 6f64 206e  list of method n
-00002c40: 616d 6573 2e0a 2020 2222 220a 2020 7472  ames..  """.  tr
-00002c50: 7565 5f6d 6574 686f 6473 203d 2073 6574  ue_methods = set
-00002c60: 2829 0a20 2066 6f72 206d 2069 6e20 636c  ().  for m in cl
-00002c70: 732e 5f5f 6469 6374 5f5f 3a0a 2020 2020  s.__dict__:.    
-00002c80: 6966 2063 616c 6c61 626c 6528 636c 732e  if callable(cls.
-00002c90: 5f5f 6469 6374 5f5f 5b6d 5d29 2061 6e64  __dict__[m]) and
-00002ca0: 206e 6f74 2069 6e73 7065 6374 2e69 7363   not inspect.isc
-00002cb0: 6c61 7373 2863 6c73 2e5f 5f64 6963 745f  lass(cls.__dict_
-00002cc0: 5f5b 6d5d 293a 2020 2320 7079 7479 7065  _[m]):  # pytype
-00002cd0: 3a20 6469 7361 626c 653d 6e6f 742d 7375  : disable=not-su
-00002ce0: 7070 6f72 7465 642d 7965 740a 2020 2020  pported-yet.    
-00002cf0: 2020 6d74 7970 6520 3d20 7479 7065 2863    mtype = type(c
-00002d00: 6c73 2e5f 5f64 6963 745f 5f5b 6d5d 290a  ls.__dict__[m]).
-00002d10: 2020 2020 2020 6966 206d 7479 7065 2021        if mtype !
-00002d20: 3d20 7374 6174 6963 6d65 7468 6f64 2061  = staticmethod a
-00002d30: 6e64 206d 7479 7065 2021 3d20 636c 6173  nd mtype != clas
-00002d40: 736d 6574 686f 643a 0a20 2020 2020 2020  smethod:.       
-00002d50: 2074 7275 655f 6d65 7468 6f64 732e 6164   true_methods.ad
-00002d60: 6428 6d29 0a20 2072 6574 7572 6e20 7475  d(m).  return tu
-00002d70: 706c 6528 7472 7565 5f6d 6574 686f 6473  ple(true_methods
-00002d80: 2e64 6966 6665 7265 6e63 6528 7365 7428  .difference(set(
-00002d90: 6578 636c 7564 6529 2929 0a0a 6465 6620  exclude)))..def 
-00002da0: 5f67 6574 5f6c 6f63 616c 5f64 6573 6372  _get_local_descr
-00002db0: 6970 746f 725f 6e61 6d65 7328 636c 733a  iptor_names(cls:
-00002dc0: 2041 6e79 2c0a 2020 2020 2020 2020 2020   Any,.          
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 2020 2020 6578 636c 7564 653a 2049        exclude: I
-00002df0: 7465 7261 626c 655b 7374 725d 203d 2028  terable[str] = (
-00002e00: 2929 202d 3e20 5475 706c 655b 7374 722c  )) -> Tuple[str,
-00002e10: 202e 2e2e 5d3a 0a20 2022 2222 4765 7473   ...]:.  """Gets
-00002e20: 2064 6573 6372 6970 746f 7220 6e61 6d65   descriptor name
-00002e30: 7320 6f66 2061 2063 6c61 7373 2e0a 0a20  s of a class... 
-00002e40: 2041 7267 733a 0a20 2020 2063 6c73 3a20   Args:.    cls: 
-00002e50: 5468 6520 636c 6173 7320 746f 2067 6574  The class to get
-00002e60: 2070 726f 7065 7274 7920 6e61 6d65 7320   property names 
-00002e70: 666f 722e 0a20 2020 2065 7863 6c75 6465  for..    exclude
-00002e80: 3a20 4e61 6d65 7320 746f 2065 7863 6c75  : Names to exclu
-00002e90: 6465 2066 726f 6d20 6f75 7470 7574 2e0a  de from output..
-00002ea0: 2020 5265 7475 726e 733a 0a20 2020 2041    Returns:.    A
-00002eb0: 206c 6973 7420 6f66 2070 726f 7065 7274   list of propert
-00002ec0: 7920 6e61 6d65 732e 0a20 2022 2222 0a20  y names..  """. 
-00002ed0: 2074 7275 655f 7072 6f70 6572 7469 6573   true_properties
-00002ee0: 203d 2073 6574 2829 0a20 2066 6f72 206d   = set().  for m
-00002ef0: 2c20 6174 7472 2069 6e20 636c 732e 5f5f  , attr in cls.__
-00002f00: 6469 6374 5f5f 2e69 7465 6d73 2829 3a0a  dict__.items():.
-00002f10: 2020 2020 6966 206e 6f74 2063 616c 6c61      if not calla
-00002f20: 626c 6528 6174 7472 2920 616e 6420 280a  ble(attr) and (.
-00002f30: 2020 2020 2020 6861 7361 7474 7228 6174        hasattr(at
-00002f40: 7472 2c20 275f 5f67 6574 5f5f 2729 206f  tr, '__get__') o
-00002f50: 7220 6861 7361 7474 7228 6174 7472 2c20  r hasattr(attr, 
-00002f60: 275f 5f73 6574 5f5f 2729 206f 720a 2020  '__set__') or.  
-00002f70: 2020 2020 6861 7361 7474 7228 6174 7472      hasattr(attr
-00002f80: 2c20 275f 5f64 656c 6574 655f 5f27 290a  , '__delete__').
-00002f90: 2020 2020 293a 0a20 2020 2020 206d 7479      ):.      mty
-00002fa0: 7065 203d 2074 7970 6528 6174 7472 290a  pe = type(attr).
-00002fb0: 2020 2020 2020 6966 206d 7479 7065 2021        if mtype !
-00002fc0: 3d20 7374 6174 6963 6d65 7468 6f64 2061  = staticmethod a
-00002fd0: 6e64 206d 7479 7065 2021 3d20 636c 6173  nd mtype != clas
-00002fe0: 736d 6574 686f 643a 0a20 2020 2020 2020  smethod:.       
-00002ff0: 2074 7275 655f 7072 6f70 6572 7469 6573   true_properties
-00003000: 2e61 6464 286d 290a 2020 7265 7475 726e  .add(m).  return
-00003010: 2074 7570 6c65 2874 7275 655f 7072 6f70   tuple(true_prop
-00003020: 6572 7469 6573 2e64 6966 6665 7265 6e63  erties.differenc
-00003030: 6528 7365 7428 6578 636c 7564 6529 2929  e(set(exclude)))
-00003040: 0a0a 0a64 6566 2077 7261 705f 6d65 7468  ...def wrap_meth
-00003050: 6f64 5f6f 6e63 6528 6675 6e3a 2043 616c  od_once(fun: Cal
-00003060: 6c61 626c 655b 2e2e 2e2c 2041 6e79 5d29  lable[..., Any])
-00003070: 202d 3e20 4361 6c6c 6162 6c65 5b2e 2e2e   -> Callable[...
-00003080: 2c20 416e 795d 3a0a 2020 2222 224d 616e  , Any]:.  """Man
-00003090: 6167 6573 204d 6f64 756c 6520 7374 6174  ages Module stat
-000030a0: 6520 666f 7220 6120 6769 7665 6e20 7573  e for a given us
-000030b0: 6572 2d64 6566 696e 6564 206d 6574 686f  er-defined metho
-000030c0: 642e 0a0a 2020 4172 6773 3a0a 2020 2020  d...  Args:.    
-000030d0: 6675 6e3a 2055 7365 722d 6465 6669 6e65  fun: User-define
-000030e0: 6420 4d6f 6475 6c65 206d 6574 686f 6420  d Module method 
-000030f0: 746f 206d 616e 6167 6520 7374 6174 6520  to manage state 
-00003100: 666f 722e 0a20 2052 6574 7572 6e73 3a0a  for..  Returns:.
-00003110: 2020 2020 5772 6170 7065 6420 6d65 7468      Wrapped meth
-00003120: 6f64 2e0a 2020 2222 220a 2020 2320 446f  od..  """.  # Do
-00003130: 6e27 7420 7265 7772 6170 206d 6574 686f  n't rewrap metho
-00003140: 6473 2074 6861 7420 6861 7665 2061 6c72  ds that have alr
-00003150: 6561 6479 2068 6164 2074 6865 2073 7461  eady had the sta
-00003160: 7465 206d 616e 6167 656d 656e 7420 7772  te management wr
-00003170: 6170 7065 720a 2020 2320 6170 706c 6965  apper.  # applie
-00003180: 6420 696e 2074 6865 2064 6563 6f72 6174  d in the decorat
-00003190: 6f72 2073 7461 636b 2e20 2054 6869 7320  or stack.  This 
-000031a0: 7772 6170 7065 7220 7368 6f75 6c64 2061  wrapper should a
-000031b0: 6c77 6179 7320 6265 2061 7070 6c69 6564  lways be applied
-000031c0: 0a20 2023 2062 6566 6f72 6520 7472 616e  .  # before tran
-000031d0: 7366 6f72 6d61 7469 6f6e 2077 7261 7070  sformation wrapp
-000031e0: 6572 732e 0a20 2069 6620 6861 7361 7474  ers..  if hasatt
-000031f0: 7228 6675 6e2c 2027 6d65 7468 6f64 5f68  r(fun, 'method_h
-00003200: 616e 646c 6572 5f77 7261 7070 6564 2729  andler_wrapped')
-00003210: 3a0a 2020 2020 7265 7475 726e 2066 756e  :.    return fun
-00003220: 0a0a 2020 4066 756e 6374 6f6f 6c73 2e77  ..  @functools.w
-00003230: 7261 7073 2866 756e 290a 2020 6465 6620  raps(fun).  def 
-00003240: 7772 6170 7065 645f 6d6f 6475 6c65 5f6d  wrapped_module_m
-00003250: 6574 686f 6428 2a61 7267 732c 202a 2a6b  ethod(*args, **k
-00003260: 7761 7267 7329 3a0a 2020 2020 2320 5765  wargs):.    # We
-00003270: 206d 6967 6874 2068 6176 6520 696e 636f   might have inco
-00003280: 7272 6563 746c 7920 7772 6170 7070 6564  rrectly wrappped
-00003290: 2061 2063 616c 6c61 626c 650a 2020 2020   a callable.    
-000032a0: 2320 7468 6174 2069 7320 6e6f 7420 6120  # that is not a 
-000032b0: 6d65 7468 6f64 2e20 4368 6563 6b20 7768  method. Check wh
-000032c0: 6574 6865 7220 7468 6520 6669 7273 7420  ether the first 
-000032d0: 6172 6720 6973 2073 656c 662c 0a20 2020  arg is self,.   
-000032e0: 2023 206f 7468 6572 7769 7365 2063 616c   # otherwise cal
-000032f0: 6c20 7468 6520 7772 6170 7065 6420 6675  l the wrapped fu
-00003300: 6e63 7469 6f6e 2061 7320 6973 2e0a 2020  nction as is..  
-00003310: 2020 6966 2061 7267 7320 616e 6420 6973    if args and is
-00003320: 696e 7374 616e 6365 2861 7267 735b 305d  instance(args[0]
-00003330: 2c20 4d6f 6475 6c65 293a 0a20 2020 2020  , Module):.     
-00003340: 2073 656c 662c 2061 7267 7320 3d20 6172   self, args = ar
-00003350: 6773 5b30 5d2c 2061 7267 735b 313a 5d0a  gs[0], args[1:].
-00003360: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003370: 662e 5f63 616c 6c5f 7772 6170 7065 645f  f._call_wrapped_
-00003380: 6d65 7468 6f64 2866 756e 2c20 6172 6773  method(fun, args
-00003390: 2c20 6b77 6172 6773 290a 2020 2020 656c  , kwargs).    el
-000033a0: 7365 3a0a 2020 2020 2020 7265 7475 726e  se:.      return
-000033b0: 2066 756e 282a 6172 6773 2c20 2a2a 6b77   fun(*args, **kw
-000033c0: 6172 6773 290a 2020 7772 6170 7065 645f  args).  wrapped_
-000033d0: 6d6f 6475 6c65 5f6d 6574 686f 642e 6d65  module_method.me
-000033e0: 7468 6f64 5f68 616e 646c 6572 5f77 7261  thod_handler_wra
-000033f0: 7070 6564 203d 2054 7275 6520 2023 2074  pped = True  # t
-00003400: 7970 653a 2069 676e 6f72 655b 6174 7472  ype: ignore[attr
-00003410: 2d64 6566 696e 6564 5d0a 2020 7265 7475  -defined].  retu
-00003420: 726e 2077 7261 7070 6564 5f6d 6f64 756c  rn wrapped_modul
-00003430: 655f 6d65 7468 6f64 0a0a 6465 6620 7772  e_method..def wr
-00003440: 6170 5f64 6573 6372 6970 746f 725f 6f6e  ap_descriptor_on
-00003450: 6365 2864 6573 6372 6970 746f 7229 202d  ce(descriptor) -
-00003460: 3e20 2244 6573 6372 6970 746f 7257 7261  > "DescriptorWra
-00003470: 7070 6572 223a 0a20 2022 2222 5772 6170  pper":.  """Wrap
-00003480: 7320 6120 6465 7363 7269 7074 6f72 2074  s a descriptor t
-00003490: 6f20 6769 7665 2062 6574 7465 7220 6572  o give better er
-000034a0: 726f 7220 6d65 7373 6167 6573 2e0a 0a20  ror messages... 
-000034b0: 2041 7267 733a 0a20 2020 2070 726f 703a   Args:.    prop:
-000034c0: 2055 7365 722d 6465 6669 6e65 6420 4d6f   User-defined Mo
-000034d0: 6475 6c65 2061 7474 7269 6275 7465 2064  dule attribute d
-000034e0: 6573 6372 6970 746f 722e 0a20 2052 6574  escriptor..  Ret
-000034f0: 7572 6e73 3a0a 2020 2020 5772 6170 7065  urns:.    Wrappe
-00003500: 6420 6465 7363 7269 7074 6f72 2e0a 2020  d descriptor..  
-00003510: 2222 220a 2020 2320 446f 6e27 7420 7265  """.  # Don't re
-00003520: 7772 6170 2064 6573 6372 6970 746f 7273  wrap descriptors
-00003530: 2e0a 2020 6966 2069 7369 6e73 7461 6e63  ..  if isinstanc
-00003540: 6528 6465 7363 7269 7074 6f72 2c20 4465  e(descriptor, De
-00003550: 7363 7269 7074 6f72 5772 6170 7065 7229  scriptorWrapper)
-00003560: 3a0a 2020 2020 7265 7475 726e 2064 6573  :.    return des
-00003570: 6372 6970 746f 720a 0a20 2072 6574 7572  criptor..  retur
-00003580: 6e20 6372 6561 7465 5f64 6573 6372 6970  n create_descrip
-00003590: 746f 725f 7772 6170 7065 7228 6465 7363  tor_wrapper(desc
-000035a0: 7269 7074 6f72 290a 0a0a 6465 6620 5f77  riptor)...def _w
-000035b0: 7261 705f 6861 7368 2868 6173 685f 666e  rap_hash(hash_fn
-000035c0: 3a20 4361 6c6c 6162 6c65 5b2e 2e2e 2c20  : Callable[..., 
-000035d0: 416e 795d 2920 2d3e 2043 616c 6c61 626c  Any]) -> Callabl
-000035e0: 655b 2e2e 2e2c 2041 6e79 5d3a 0a20 2022  e[..., Any]:.  "
-000035f0: 2222 5772 6170 7320 6120 6861 7368 2066  ""Wraps a hash f
-00003600: 756e 6374 696f 6e20 7769 7468 2073 6f6d  unction with som
-00003610: 6520 6368 6563 6b20 666f 7220 466c 6178  e check for Flax
-00003620: 204d 6f64 756c 6573 2e22 2222 0a20 2040   Modules.""".  @
-00003630: 6675 6e63 746f 6f6c 732e 7772 6170 7328  functools.wraps(
-00003640: 6861 7368 5f66 6e29 0a20 2064 6566 2077  hash_fn).  def w
-00003650: 7261 7070 6564 2873 656c 6629 3a0a 2020  rapped(self):.  
-00003660: 2020 6966 2073 656c 662e 7363 6f70 6520    if self.scope 
-00003670: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00003680: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-00003690: 6f72 2827 4361 6e5c 2774 2063 616c 6c20  or('Can\'t call 
-000036a0: 5f5f 6861 7368 5f5f 206f 6e20 6d6f 6475  __hash__ on modu
-000036b0: 6c65 7320 7468 6174 2068 6f6c 6420 7661  les that hold va
-000036c0: 7269 6162 6c65 732e 2729 0a20 2020 2074  riables.').    t
-000036d0: 7279 3a0a 2020 2020 2020 6861 7368 5f76  ry:.      hash_v
-000036e0: 616c 7565 203d 2068 6173 685f 666e 2873  alue = hash_fn(s
-000036f0: 656c 6629 0a20 2020 2065 7863 6570 7420  elf).    except 
-00003700: 5479 7065 4572 726f 7220 6173 2065 7863  TypeError as exc
-00003710: 3a0a 2020 2020 2020 7261 6973 6520 5479  :.      raise Ty
-00003720: 7065 4572 726f 7228 2746 6169 6c65 6420  peError('Failed 
-00003730: 746f 2068 6173 6820 466c 6178 204d 6f64  to hash Flax Mod
-00003740: 756c 652e 2020 270a 2020 2020 2020 2020  ule.  '.        
-00003750: 2020 2020 2020 2020 2020 2020 2020 2754                'T
-00003760: 6865 206d 6f64 756c 6520 7072 6f62 6162  he module probab
-00003770: 6c79 2063 6f6e 7461 696e 7320 756e 6861  ly contains unha
-00003780: 7368 6162 6c65 2061 7474 7269 6275 7465  shable attribute
-00003790: 732e 2020 270a 2020 2020 2020 2020 2020  s.  '.          
-000037a0: 2020 2020 2020 2020 2020 2020 6627 4d6f              f'Mo
-000037b0: 6475 6c65 3d7b 7365 6c66 7d27 2920 6672  dule={self}') fr
-000037c0: 6f6d 2065 7863 0a20 2020 2072 6574 7572  om exc.    retur
-000037d0: 6e20 6861 7368 5f76 616c 7565 0a20 2072  n hash_value.  r
-000037e0: 6574 7572 6e20 7772 6170 7065 640a 0a0a  eturn wrapped...
-000037f0: 6465 6620 5f67 6574 5f75 6e62 6f75 6e64  def _get_unbound
-00003800: 5f66 6e28 6d65 7468 6f64 5f6f 725f 666e  _fn(method_or_fn
-00003810: 3a20 4361 6c6c 6162 6c65 5b2e 2e2e 2c20  : Callable[..., 
-00003820: 416e 795d 2920 2d3e 2043 616c 6c61 626c  Any]) -> Callabl
-00003830: 655b 2e2e 2e2c 2041 6e79 5d3a 0a20 2022  e[..., Any]:.  "
-00003840: 2222 5265 7475 726e 7320 616e 2075 6e62  ""Returns an unb
-00003850: 6f75 6e64 2066 756e 6374 696f 6e20 6672  ound function fr
-00003860: 6f6d 2061 206d 6574 686f 6420 7468 6174  om a method that
-00003870: 2069 7320 706f 7373 6962 6c79 2062 6f75   is possibly bou
-00003880: 6e64 2e0a 0a20 2054 6869 7320 6d65 616e  nd...  This mean
-00003890: 7320 7468 6174 2069 6620 7468 6520 7061  s that if the pa
-000038a0: 7373 6564 2066 756e 6374 696f 6e20 6265  ssed function be
-000038b0: 6c6f 6e67 7320 6f66 2061 6e20 696e 7374  longs of an inst
-000038c0: 616e 6365 206f 6620 6120 636c 6173 732c  ance of a class,
-000038d0: 2074 6865 6e0a 2020 7468 6520 7265 7475   then.  the retu
-000038e0: 726e 6564 2066 756e 6374 696f 6e20 646f  rned function do
-000038f0: 6573 206e 6f20 6c6f 6e67 6572 2064 6570  es no longer dep
-00003900: 656e 6420 6f6e 2074 6865 2069 6e73 7461  end on the insta
-00003910: 6e63 652c 2077 6869 6368 2069 7320 7061  nce, which is pa
-00003920: 7373 6564 0a20 2061 7320 7468 6520 6669  ssed.  as the fi
-00003930: 7273 7420 6172 6775 6d65 6e74 2074 6f20  rst argument to 
-00003940: 7468 6520 6675 6e63 7469 6f6e 2e0a 0a20  the function... 
-00003950: 2041 7267 733a 0a20 2020 206d 6574 686f   Args:.    metho
-00003960: 645f 6f72 5f66 6e3a 2041 2063 6c61 7373  d_or_fn: A class
-00003970: 206d 6574 686f 6420 6f72 2066 756e 6374   method or funct
-00003980: 696f 6e2e 0a20 2052 6574 7572 6e73 3a0a  ion..  Returns:.
-00003990: 2020 2020 416e 2075 6e62 6f75 6e64 2076      An unbound v
-000039a0: 6572 7369 6f6e 206f 6620 696e 7075 7420  ersion of input 
-000039b0: 6675 6e63 7469 6f6e 2e0a 2020 2222 220a  function..  """.
-000039c0: 2020 6966 2028 696e 7370 6563 742e 6973    if (inspect.is
-000039d0: 6d65 7468 6f64 286d 6574 686f 645f 6f72  method(method_or
-000039e0: 5f66 6e29 2061 6e64 0a20 2020 2020 2069  _fn) and.      i
-000039f0: 7369 6e73 7461 6e63 6528 6d65 7468 6f64  sinstance(method
-00003a00: 5f6f 725f 666e 2e5f 5f73 656c 665f 5f2c  _or_fn.__self__,
-00003a10: 204d 6f64 756c 6529 293a 2020 2320 7079   Module)):  # py
-00003a20: 7479 7065 3a20 6469 7361 626c 653d 6174  type: disable=at
-00003a30: 7472 6962 7574 652d 6572 726f 720a 2020  tribute-error.  
-00003a40: 2020 6d65 7468 6f64 5f6f 725f 666e 203d    method_or_fn =
-00003a50: 206d 6574 686f 645f 6f72 5f66 6e2e 5f5f   method_or_fn.__
-00003a60: 6675 6e63 5f5f 2020 2320 7079 7479 7065  func__  # pytype
-00003a70: 3a20 6469 7361 626c 653d 6174 7472 6962  : disable=attrib
-00003a80: 7574 652d 6572 726f 720a 0a20 2023 2054  ute-error..  # T
-00003a90: 6865 206d 6574 686f 6420 7368 6f75 6c64  he method should
-00003aa0: 2062 6520 6361 6c6c 6162 6c65 2c20 616e   be callable, an
-00003ab0: 6420 6974 2073 686f 756c 6420 6861 7665  d it should have
-00003ac0: 2061 7420 6c65 6173 7420 6f6e 6520 6172   at least one ar
-00003ad0: 6775 6d65 6e74 0a20 2023 2072 6570 7265  gument.  # repre
-00003ae0: 7365 6e74 696e 6720 7468 6520 636c 6173  senting the clas
-00003af0: 7320 7468 6174 2069 7320 7061 7373 6564  s that is passed
-00003b00: 2069 6e2e 0a20 2069 6620 286e 6f74 2063   in..  if (not c
-00003b10: 616c 6c61 626c 6528 6d65 7468 6f64 5f6f  allable(method_o
-00003b20: 725f 666e 2920 6f72 0a20 2020 2020 206c  r_fn) or.      l
-00003b30: 656e 2869 6e73 7065 6374 2e73 6967 6e61  en(inspect.signa
-00003b40: 7475 7265 286d 6574 686f 645f 6f72 5f66  ture(method_or_f
-00003b50: 6e29 2e70 6172 616d 6574 6572 7329 203c  n).parameters) <
-00003b60: 2031 293a 0a20 2020 2072 6169 7365 2065   1):.    raise e
-00003b70: 7272 6f72 732e 4170 706c 794d 6f64 756c  rrors.ApplyModul
-00003b80: 6549 6e76 616c 6964 4d65 7468 6f64 4572  eInvalidMethodEr
-00003b90: 726f 7228 6d65 7468 6f64 5f6f 725f 666e  ror(method_or_fn
-00003ba0: 290a 0a20 2072 6574 7572 6e20 6d65 7468  )..  return meth
-00003bb0: 6f64 5f6f 725f 666e 0a0a 0a63 6c61 7373  od_or_fn...class
-00003bc0: 2053 6574 7570 5374 6174 6528 656e 756d   SetupState(enum
-00003bd0: 2e49 6e74 456e 756d 293a 0a20 2023 2073  .IntEnum):.  # s
-00003be0: 6574 7570 2829 2068 6173 206e 6f74 2062  etup() has not b
-00003bf0: 6565 6e20 6361 6c6c 6564 2e0a 2020 4e45  een called..  NE
-00003c00: 5720 3d20 300a 2020 2320 7365 7475 7028  W = 0.  # setup(
-00003c10: 2920 6861 7320 6265 656e 2063 616c 6c65  ) has been calle
-00003c20: 6420 6f75 7473 6964 6520 6120 7472 616e  d outside a tran
-00003c30: 7366 6f72 6d20 626f 756e 6461 7279 2e0a  sform boundary..
-00003c40: 2020 5452 414e 5346 4f52 4d45 4420 3d20    TRANSFORMED = 
-00003c50: 310a 2020 2320 7365 7475 7028 2920 6861  1.  # setup() ha
-00003c60: 7320 6265 656e 2063 616c 6c65 642e 0a20  s been called.. 
-00003c70: 2044 4f4e 4520 3d20 320a 0a0a 4064 6174   DONE = 2...@dat
-00003c80: 6163 6c61 7373 6573 2e64 6174 6163 6c61  aclasses.datacla
-00003c90: 7373 0a63 6c61 7373 205f 4d6f 6475 6c65  ss.class _Module
-00003ca0: 496e 7465 726e 616c 5374 6174 653a 0a20  InternalState:. 
-00003cb0: 2022 2222 4570 6865 6d65 7261 6c20 4d6f   """Ephemeral Mo
-00003cc0: 6475 6c65 2045 7661 6c75 6174 696f 6e20  dule Evaluation 
-00003cd0: 5374 6174 652e 0a0a 2020 466f 7220 636c  State...  For cl
-00003ce0: 6172 6974 792c 2077 6520 636f 6c6c 6563  arity, we collec
-00003cf0: 7420 616c 6c20 6f66 2074 6865 2074 656d  t all of the tem
-00003d00: 706f 7261 7279 2066 6c61 6773 2061 6e64  porary flags and
-00003d10: 2065 7068 656d 6572 616c 2073 7461 7465   ephemeral state
-00003d20: 2075 7365 6420 6279 0a20 204d 6f64 756c   used by.  Modul
-00003d30: 6573 2066 6f72 2061 7574 6f6e 616d 696e  es for autonamin
-00003d40: 6720 616e 6420 6572 726f 7220 6d65 7373  g and error mess
-00003d50: 6167 6573 2068 6572 652c 2061 6c6f 6e67  ages here, along
-00003d60: 7369 6465 2074 6865 2072 756c 6573 2075  side the rules u
-00003d70: 7365 640a 2020 746f 2070 6173 7320 7468  sed.  to pass th
-00003d80: 6973 2065 7068 656d 6572 616c 2073 7461  is ephemeral sta
-00003d90: 7465 2061 6372 6f73 7320 7472 616e 7366  te across transf
-00003da0: 6f72 6d20 626f 756e 6461 7269 6573 2e0a  orm boundaries..
-00003db0: 2020 2222 220a 2020 696e 5f63 6f6d 7061    """.  in_compa
-00003dc0: 6374 5f6d 6574 686f 643a 2062 6f6f 6c20  ct_method: bool 
-00003dd0: 3d20 4661 6c73 650a 2020 696e 5f73 6574  = False.  in_set
-00003de0: 7570 3a20 626f 6f6c 203d 2046 616c 7365  up: bool = False
-00003df0: 0a20 2073 6574 7570 5f63 616c 6c65 643a  .  setup_called:
-00003e00: 2053 6574 7570 5374 6174 6520 3d20 5365   SetupState = Se
-00003e10: 7475 7053 7461 7465 2e4e 4557 0a20 2069  tupState.NEW.  i
-00003e20: 735f 696e 6974 6961 6c69 7a65 643a 2062  s_initialized: b
-00003e30: 6f6f 6c20 3d20 4661 6c73 650a 2020 6175  ool = False.  au
-00003e40: 746f 6e61 6d65 5f63 7572 736f 723a 2044  toname_cursor: D
-00003e50: 6963 745b 7374 722c 2069 6e74 5d20 3d20  ict[str, int] = 
-00003e60: 6461 7461 636c 6173 7365 732e 6669 656c  dataclasses.fiel
-00003e70: 6428 6465 6661 756c 745f 6661 6374 6f72  d(default_factor
-00003e80: 793d 6469 6374 290a 2020 6368 696c 6472  y=dict).  childr
-00003e90: 656e 3a20 4469 6374 5b73 7472 2c20 556e  en: Dict[str, Un
-00003ea0: 696f 6e5b 7374 722c 2027 4d6f 6475 6c65  ion[str, 'Module
-00003eb0: 275d 5d20 3d20 6461 7461 636c 6173 7365  ']] = dataclasse
-00003ec0: 732e 6669 656c 6428 0a20 2020 2020 2064  s.field(.      d
-00003ed0: 6566 6175 6c74 5f66 6163 746f 7279 3d64  efault_factory=d
-00003ee0: 6963 7429 0a0a 2020 6465 6620 7265 7365  ict)..  def rese
-00003ef0: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
-00003f00: 0a20 2020 2022 2222 5265 7365 7473 2074  .    """Resets t
-00003f10: 7261 6e73 6965 6e74 2073 7461 7465 2e0a  ransient state..
-00003f20: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
-00003f30: 6f6e 2069 7320 6361 6c6c 6564 2061 6674  on is called aft
-00003f40: 6572 2065 6163 6820 6d6f 6475 6c65 206d  er each module m
-00003f50: 6574 686f 642c 2073 6f20 6f6e 6c79 2061  ethod, so only a
-00003f60: 7474 7269 6275 7465 7320 7468 6174 0a20  ttributes that. 
-00003f70: 2020 2061 7265 206d 6574 686f 642d 6465     are method-de
-00003f80: 7065 6e64 656e 7420 6172 6520 7265 7365  pendent are rese
-00003f90: 742e 0a20 2020 2022 2222 0a20 2020 2073  t..    """.    s
-00003fa0: 656c 662e 696e 5f63 6f6d 7061 6374 5f6d  elf.in_compact_m
-00003fb0: 6574 686f 6420 3d20 4661 6c73 650a 2020  ethod = False.  
-00003fc0: 2020 7365 6c66 2e69 6e5f 7365 7475 7020    self.in_setup 
-00003fd0: 3d20 4661 6c73 650a 2020 2020 7365 6c66  = False.    self
-00003fe0: 2e61 7574 6f6e 616d 655f 6375 7273 6f72  .autoname_cursor
-00003ff0: 203d 2064 6963 7428 290a 0a20 2064 6566   = dict()..  def
-00004000: 2065 7870 6f72 7428 7365 6c66 2920 2d3e   export(self) ->
-00004010: 2027 5f4d 6f64 756c 6549 6e74 6572 6e61   '_ModuleInterna
-00004020: 6c53 7461 7465 273a 0a20 2020 2022 2222  lState':.    """
-00004030: 4578 706f 7274 7320 7472 616e 7366 6f72  Exports transfor
-00004040: 6d2d 7072 6573 6572 7665 6420 7374 6174  m-preserved stat
-00004050: 6520 6163 726f 7373 2074 7261 6e73 666f  e across transfo
-00004060: 726d 2062 6f75 6e64 6172 792e 2222 220a  rm boundary.""".
-00004070: 2020 2020 7365 7475 705f 7374 6174 6520      setup_state 
-00004080: 3d20 5365 7475 7053 7461 7465 2e54 5241  = SetupState.TRA
-00004090: 4e53 464f 524d 4544 2069 6620 7365 6c66  NSFORMED if self
-000040a0: 2e73 6574 7570 5f63 616c 6c65 6420 656c  .setup_called el
-000040b0: 7365 2053 6574 7570 5374 6174 652e 4e45  se SetupState.NE
-000040c0: 570a 2020 2020 636c 6f6e 6564 203d 205f  W.    cloned = _
-000040d0: 4d6f 6475 6c65 496e 7465 726e 616c 5374  ModuleInternalSt
-000040e0: 6174 6528 0a20 2020 2020 2020 2069 6e5f  ate(.        in_
-000040f0: 636f 6d70 6163 745f 6d65 7468 6f64 3d73  compact_method=s
-00004100: 656c 662e 696e 5f63 6f6d 7061 6374 5f6d  elf.in_compact_m
-00004110: 6574 686f 642c 0a20 2020 2020 2020 2069  ethod,.        i
-00004120: 6e5f 7365 7475 703d 7365 6c66 2e69 6e5f  n_setup=self.in_
-00004130: 7365 7475 702c 0a20 2020 2020 2020 2073  setup,.        s
-00004140: 6574 7570 5f63 616c 6c65 643d 7365 7475  etup_called=setu
-00004150: 705f 7374 6174 652c 0a20 2020 2020 2020  p_state,.       
-00004160: 2069 735f 696e 6974 6961 6c69 7a65 643d   is_initialized=
-00004170: 7365 6c66 2e69 735f 696e 6974 6961 6c69  self.is_initiali
-00004180: 7a65 642c 0a20 2020 2020 2020 2061 7574  zed,.        aut
-00004190: 6f6e 616d 655f 6375 7273 6f72 3d64 6963  oname_cursor=dic
-000041a0: 7428 7365 6c66 2e61 7574 6f6e 616d 655f  t(self.autoname_
-000041b0: 6375 7273 6f72 2929 0a20 2020 2072 6574  cursor)).    ret
-000041c0: 7572 6e20 636c 6f6e 6564 0a0a 2020 6465  urn cloned..  de
-000041d0: 6620 7265 696d 706f 7274 2873 656c 662c  f reimport(self,
-000041e0: 206f 7468 6572 3a20 275f 4d6f 6475 6c65   other: '_Module
-000041f0: 496e 7465 726e 616c 5374 6174 6527 2920  InternalState') 
-00004200: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-00004210: 5265 2d69 6d70 6f72 7473 2074 7261 6e73  Re-imports trans
-00004220: 666f 726d 2d70 7265 7365 7276 6564 2073  form-preserved s
-00004230: 7461 7465 2066 726f 6d20 6163 726f 7373  tate from across
-00004240: 2074 7261 6e73 666f 726d 2062 6f75 6e64   transform bound
-00004250: 6172 792e 2222 220a 2020 2020 7365 6c66  ary.""".    self
-00004260: 2e69 6e5f 636f 6d70 6163 745f 6d65 7468  .in_compact_meth
-00004270: 6f64 203d 206f 7468 6572 2e69 6e5f 636f  od = other.in_co
-00004280: 6d70 6163 745f 6d65 7468 6f64 0a20 2020  mpact_method.   
-00004290: 2073 656c 662e 696e 5f73 6574 7570 203d   self.in_setup =
-000042a0: 206f 7468 6572 2e69 6e5f 7365 7475 700a   other.in_setup.
-000042b0: 2020 2020 7365 6c66 2e69 735f 696e 6974      self.is_init
-000042c0: 6961 6c69 7a65 6420 3d20 6f74 6865 722e  ialized = other.
-000042d0: 6973 5f69 6e69 7469 616c 697a 6564 0a20  is_initialized. 
-000042e0: 2020 2073 656c 662e 6175 746f 6e61 6d65     self.autoname
-000042f0: 5f63 7572 736f 7220 3d20 6469 6374 286f  _cursor = dict(o
-00004300: 7468 6572 2e61 7574 6f6e 616d 655f 6375  ther.autoname_cu
-00004310: 7273 6f72 290a 0a5f 756e 696e 6974 6961  rsor).._uninitia
-00004320: 6c69 7a65 645f 6d6f 6475 6c65 5f69 6e74  lized_module_int
-00004330: 6572 6e61 6c5f 7374 6174 6520 3d20 5f4d  ernal_state = _M
-00004340: 6f64 756c 6549 6e74 6572 6e61 6c53 7461  oduleInternalSta
-00004350: 7465 2829 0a0a 0a5f 554e 4445 4649 4e45  te()..._UNDEFINE
-00004360: 445f 434f 5059 5f50 4943 4b4c 455f 4d45  D_COPY_PICKLE_ME
-00004370: 5448 4f44 5320 3d20 280a 2020 2020 275f  THODS = (.    '_
-00004380: 5f67 6574 7374 6174 655f 5f27 2c20 275f  _getstate__', '_
-00004390: 5f73 6574 7374 6174 655f 5f27 2c20 275f  _setstate__', '_
-000043a0: 5f67 6574 6e65 7761 7267 735f 6578 5f5f  _getnewargs_ex__
-000043b0: 272c 0a20 2020 2027 5f5f 7265 6475 6365  ',.    '__reduce
-000043c0: 5f5f 272c 2027 5f5f 7265 6475 6365 5f65  __', '__reduce_e
-000043d0: 785f 5f27 2c20 275f 5f63 6f70 795f 5f27  x__', '__copy__'
-000043e0: 2c20 275f 5f64 6565 7063 6f70 795f 5f27  , '__deepcopy__'
-000043f0: 290a 0a0a 5f63 6163 6865 733a 2027 7765  )..._caches: 'we
-00004400: 616b 7265 662e 5765 616b 4b65 7944 6963  akref.WeakKeyDic
-00004410: 7469 6f6e 6172 795b 5363 6f70 652c 2077  tionary[Scope, w
-00004420: 6561 6b72 6566 2e57 6561 6b56 616c 7565  eakref.WeakValue
-00004430: 4469 6374 696f 6e61 7279 5b46 6c61 7849  Dictionary[FlaxI
-00004440: 642c 204d 6f64 756c 655d 5d27 203d 2028  d, Module]]' = (
-00004450: 0a20 2020 2077 6561 6b72 6566 2e57 6561  .    weakref.Wea
-00004460: 6b4b 6579 4469 6374 696f 6e61 7279 2829  kKeyDictionary()
-00004470: 290a 0a0a 7475 706c 655f 7265 6475 6365  )...tuple_reduce
-00004480: 203d 206c 616d 6264 6120 7873 2c20 783a   = lambda xs, x:
-00004490: 2078 7320 2b20 2878 2c29 0a74 7570 6c65   xs + (x,).tuple
-000044a0: 5f69 6e69 7420 3d20 6c61 6d62 6461 3a20  _init = lambda: 
-000044b0: 2829 0a0a 0a63 6170 7475 7265 5f63 616c  ()...capture_cal
-000044c0: 6c5f 696e 7465 726d 6564 6961 7465 7320  l_intermediates 
-000044d0: 3d20 6c61 6d62 6461 205f 2c20 6d65 7468  = lambda _, meth
-000044e0: 6f64 5f6e 616d 653a 206d 6574 686f 645f  od_name: method_
-000044f0: 6e61 6d65 203d 3d20 275f 5f63 616c 6c5f  name == '__call_
-00004500: 5f27 0a0a 0a63 6c61 7373 2050 6172 656e  _'...class Paren
-00004510: 7444 6573 6372 6970 746f 723a 0a20 2022  tDescriptor:.  "
-00004520: 2222 5772 6170 7320 7061 7265 6e74 206d  ""Wraps parent m
-00004530: 6f64 756c 6520 7265 6665 7265 6e63 6573  odule references
-00004540: 2069 6e20 7765 616b 2072 6566 732e 0a0a   in weak refs...
-00004550: 2020 5468 6973 2070 7265 7665 6e74 7320    This prevents 
-00004560: 7265 6665 7265 6e63 6520 6379 636c 6573  reference cycles
-00004570: 2066 726f 6d20 666f 726d 696e 6720 7669   from forming vi
-00004580: 6120 7061 7265 6e74 206c 696e 6b73 2077  a parent links w
-00004590: 6869 6368 2063 616e 206c 6561 640a 2020  hich can lead.  
-000045a0: 746f 2061 6363 6964 656e 7461 6c20 4f4f  to accidental OO
-000045b0: 4d73 2069 6e20 6561 6765 7220 6d6f 6465  Ms in eager mode
-000045c0: 2064 7565 2074 6f20 736c 6f77 2067 6172   due to slow gar
-000045d0: 6261 6765 2063 6f6c 6c65 6374 696f 6e20  bage collection 
-000045e0: 6173 2077 656c 6c20 6173 0a20 2073 7075  as well as.  spu
-000045f0: 7269 6f75 7320 7472 6163 6572 206c 6561  rious tracer lea
-00004600: 6b73 2064 7572 696e 6720 6a69 7420 636f  ks during jit co
-00004610: 6d70 696c 6174 696f 6e2e 0a0a 2020 4e6f  mpilation...  No
-00004620: 7465 3a20 2264 6573 6372 6970 746f 7273  te: "descriptors
-00004630: 2220 6172 6520 7468 6520 756e 6465 726c  " are the underl
-00004640: 7969 6e67 2070 7974 686f 6e20 6d65 6368  ying python mech
-00004650: 616e 6973 6d20 666f 7220 696d 706c 656d  anism for implem
-00004660: 656e 7469 6e67 0a20 2064 796e 616d 6963  enting.  dynamic
-00004670: 2040 7072 6f70 6572 7479 2064 6563 6f72   @property decor
-00004680: 6174 6f72 732e 2020 5765 206e 6565 6420  ators.  We need 
-00004690: 746f 2075 7365 2061 2072 6177 2064 6573  to use a raw des
-000046a0: 6372 6970 746f 7220 696e 7374 6561 6420  criptor instead 
-000046b0: 6f66 2074 6865 0a20 206d 6f72 6520 636f  of the.  more co
-000046c0: 6d6d 6f6e 2064 6563 6f72 6174 6f72 2069  mmon decorator i
-000046d0: 6e20 6f72 6465 7220 746f 2066 6f72 6365  n order to force
-000046e0: 2074 6861 7420 7468 6520 6170 7072 6f70   that the approp
-000046f0: 7269 6174 6520 6765 7474 6572 2f73 6574  riate getter/set
-00004700: 7465 720a 2020 6c6f 6769 6320 6170 706c  ter.  logic appl
-00004710: 6965 7320 696e 2073 7562 636c 6173 7365  ies in subclasse
-00004720: 7320 6576 656e 2061 6674 6572 2076 6172  s even after var
-00004730: 696f 7573 2064 6174 6163 6c61 7373 2074  ious dataclass t
-00004740: 7261 6e73 666f 726d 732e 0a20 2022 2222  ransforms..  """
-00004750: 0a20 2064 6566 205f 5f67 6574 5f5f 2873  .  def __get__(s
-00004760: 656c 662c 206f 626a 2c20 6f62 6a74 7970  elf, obj, objtyp
-00004770: 653d 4e6f 6e65 293a 0a20 2020 2023 2063  e=None):.    # c
-00004780: 6865 636b 2069 6620 6f62 6a20 6973 204e  heck if obj is N
-00004790: 6f6e 652c 2068 6170 7065 6e73 2064 7572  one, happens dur
-000047a0: 696e 6720 2561 7574 6f72 656c 6f61 640a  ing %autoreload.
-000047b0: 2020 2020 6966 206f 626a 2069 7320 4e6f      if obj is No
-000047c0: 6e65 3a0a 2020 2020 2020 7265 7475 726e  ne:.      return
-000047d0: 204e 6f6e 650a 2020 2020 7061 7265 6e74   None.    parent
-000047e0: 203d 206f 626a 6563 742e 5f5f 6765 7461   = object.__geta
-000047f0: 7474 7269 6275 7465 5f5f 286f 626a 2c20  ttribute__(obj, 
-00004800: 225f 7061 7265 6e74 5f72 6566 2229 0a20  "_parent_ref"). 
-00004810: 2020 2072 6574 7572 6e20 7061 7265 6e74     return parent
-00004820: 2829 2069 6620 6973 696e 7374 616e 6365  () if isinstance
-00004830: 2870 6172 656e 742c 2077 6561 6b72 6566  (parent, weakref
-00004840: 2e52 6566 6572 656e 6365 5479 7065 2920  .ReferenceType) 
-00004850: 656c 7365 2070 6172 656e 740a 0a20 2064  else parent..  d
-00004860: 6566 205f 5f73 6574 5f5f 2873 656c 662c  ef __set__(self,
-00004870: 206f 626a 2c20 7661 6c75 6529 3a0a 2020   obj, value):.  
-00004880: 2020 6d61 7962 655f 7765 616b 203d 2077    maybe_weak = w
-00004890: 6561 6b72 6566 2e72 6566 2876 616c 7565  eakref.ref(value
-000048a0: 2920 6966 2069 7369 6e73 7461 6e63 6528  ) if isinstance(
-000048b0: 7661 6c75 652c 204d 6f64 756c 6529 2065  value, Module) e
-000048c0: 6c73 6520 7661 6c75 650a 2020 2020 6f62  lse value.    ob
-000048d0: 6a65 6374 2e5f 5f73 6574 6174 7472 5f5f  ject.__setattr__
-000048e0: 286f 626a 2c20 225f 7061 7265 6e74 5f72  (obj, "_parent_r
-000048f0: 6566 222c 206d 6179 6265 5f77 6561 6b29  ef", maybe_weak)
-00004900: 0a0a 0a63 6c61 7373 2044 6573 6372 6970  ...class Descrip
-00004910: 746f 7228 5072 6f74 6f63 6f6c 293a 0a20  tor(Protocol):. 
-00004920: 205f 5f69 7361 6273 7472 6163 746d 6574   __isabstractmet
-00004930: 686f 645f 5f3a 2062 6f6f 6c0a 2020 6465  hod__: bool.  de
-00004940: 6620 5f5f 6765 745f 5f28 7365 6c66 2c20  f __get__(self, 
-00004950: 6f62 6a2c 206f 626a 7479 7065 3d4e 6f6e  obj, objtype=Non
-00004960: 6529 202d 3e20 416e 793a 202e 2e2e 0a20  e) -> Any: .... 
-00004970: 2064 6566 205f 5f73 6574 5f5f 2873 656c   def __set__(sel
-00004980: 662c 206f 626a 2c20 7661 6c75 6529 202d  f, obj, value) -
-00004990: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 6465  > None: ....  de
-000049a0: 6620 5f5f 6465 6c65 7465 5f5f 2873 656c  f __delete__(sel
-000049b0: 662c 206f 626a 2920 2d3e 204e 6f6e 653a  f, obj) -> None:
-000049c0: 202e 2e2e 0a20 2064 6566 205f 5f73 6574   ....  def __set
-000049d0: 5f6e 616d 655f 5f28 7365 6c66 2c20 6f77  _name__(self, ow
-000049e0: 6e65 722c 206e 616d 6529 202d 3e20 4e6f  ner, name) -> No
-000049f0: 6e65 3a20 2e2e 2e0a 0a63 6c61 7373 2044  ne: .....class D
-00004a00: 6573 6372 6970 746f 7257 7261 7070 6572  escriptorWrapper
-00004a10: 3a0a 2020 7061 7373 0a0a 6465 6620 6372  :.  pass..def cr
-00004a20: 6561 7465 5f64 6573 6372 6970 746f 725f  eate_descriptor_
-00004a30: 7772 6170 7065 7228 6465 7363 7269 7074  wrapper(descript
-00004a40: 6f72 3a20 4465 7363 7269 7074 6f72 293a  or: Descriptor):
-00004a50: 0a20 2022 2222 4372 6561 7465 7320 6120  .  """Creates a 
-00004a60: 6465 7363 7269 7074 6f72 2077 7261 7070  descriptor wrapp
-00004a70: 6572 2074 6861 7420 6361 6c6c 7320 6120  er that calls a 
-00004a80: 6765 745f 666e 206f 6e20 7468 6520 6465  get_fn on the de
-00004a90: 7363 7269 7074 6f72 2e22 2222 0a0a 2020  scriptor."""..  
-00004aa0: 636c 6173 7320 5f44 6573 6372 6970 746f  class _Descripto
-00004ab0: 7257 7261 7070 6572 2844 6573 6372 6970  rWrapper(Descrip
-00004ac0: 746f 7257 7261 7070 6572 293a 0a20 2020  torWrapper):.   
-00004ad0: 2022 2222 4120 6465 7363 7269 7074 6f72   """A descriptor
-00004ae0: 2074 6861 7420 6361 6e20 7772 6170 2061   that can wrap a
-00004af0: 6e79 2064 6573 6372 6970 746f 7222 2222  ny descriptor"""
-00004b00: 0a0a 2020 2020 6966 2068 6173 6174 7472  ..    if hasattr
-00004b10: 2864 6573 6372 6970 746f 722c 2027 5f5f  (descriptor, '__
-00004b20: 6973 6162 7374 7261 6374 6d65 7468 6f64  isabstractmethod
-00004b30: 5f5f 2729 3a0a 2020 2020 2020 5f5f 6973  __'):.      __is
-00004b40: 6162 7374 7261 6374 6d65 7468 6f64 5f5f  abstractmethod__
-00004b50: 203d 2064 6573 6372 6970 746f 722e 5f5f   = descriptor.__
-00004b60: 6973 6162 7374 7261 6374 6d65 7468 6f64  isabstractmethod
-00004b70: 5f5f 0a0a 2020 2020 6465 6620 5f5f 696e  __..    def __in
-00004b80: 6974 5f5f 2873 656c 662c 2077 7261 7070  it__(self, wrapp
-00004b90: 6564 3a20 4465 7363 7269 7074 6f72 293a  ed: Descriptor):
-00004ba0: 0a20 2020 2020 2073 656c 662e 7772 6170  .      self.wrap
-00004bb0: 7065 6420 3d20 7772 6170 7065 640a 0a20  ped = wrapped.. 
-00004bc0: 2020 2023 2063 6f6e 6469 7469 6f6e 616c     # conditional
-00004bd0: 6c79 2064 6566 696e 6520 6465 7363 7269  ly define descri
-00004be0: 7074 6f72 206d 6574 686f 6473 0a20 2020  ptor methods.   
-00004bf0: 2069 6620 6861 7361 7474 7228 6465 7363   if hasattr(desc
-00004c00: 7269 7074 6f72 2c20 275f 5f67 6574 5f5f  riptor, '__get__
-00004c10: 2729 3a0a 2020 2020 2020 6465 6620 5f5f  '):.      def __
-00004c20: 6765 745f 5f28 7365 6c66 2c20 2a61 7267  get__(self, *arg
-00004c30: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
-00004c40: 2020 2020 2020 2320 6865 7265 2077 6520        # here we 
-00004c50: 7769 6c6c 2063 6174 6368 2069 6e74 6572  will catch inter
-00004c60: 6e61 6c20 4174 7472 6962 7574 6545 7272  nal AttributeErr
-00004c70: 6f72 2061 6e64 2072 652d 7261 6973 6520  or and re-raise 
-00004c80: 6974 2061 7320 610a 2020 2020 2020 2020  it as a.        
-00004c90: 2320 6d6f 7265 2069 6e66 6f72 6d61 7469  # more informati
-00004ca0: 7665 2061 6e64 2063 6f72 7265 6374 2065  ve and correct e
-00004cb0: 7272 6f72 206d 6573 7361 6765 2e0a 2020  rror message..  
-00004cc0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00004cd0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00004ce0: 2e77 7261 7070 6564 2e5f 5f67 6574 5f5f  .wrapped.__get__
-00004cf0: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-00004d00: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00004d10: 2041 7474 7269 6275 7465 4572 726f 7220   AttributeError 
-00004d20: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00004d30: 7261 6973 6520 6572 726f 7273 2e44 6573  raise errors.Des
-00004d40: 6372 6970 746f 7241 7474 7269 6275 7465  criptorAttribute
-00004d50: 4572 726f 7228 2920 6672 6f6d 2065 0a0a  Error() from e..
-00004d60: 2020 2020 6966 2068 6173 6174 7472 2864      if hasattr(d
-00004d70: 6573 6372 6970 746f 722c 2027 5f5f 7365  escriptor, '__se
-00004d80: 745f 5f27 293a 0a20 2020 2020 2064 6566  t__'):.      def
-00004d90: 205f 5f73 6574 5f5f 2873 656c 662c 202a   __set__(self, *
-00004da0: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-00004db0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004dc0: 7365 6c66 2e77 7261 7070 6564 2e5f 5f73  self.wrapped.__s
-00004dd0: 6574 5f5f 282a 6172 6773 2c20 2a2a 6b77  et__(*args, **kw
-00004de0: 6172 6773 290a 0a20 2020 2069 6620 6861  args)..    if ha
-00004df0: 7361 7474 7228 6465 7363 7269 7074 6f72  sattr(descriptor
-00004e00: 2c20 275f 5f64 656c 6574 655f 5f27 293a  , '__delete__'):
-00004e10: 0a20 2020 2020 2064 6566 205f 5f64 656c  .      def __del
-00004e20: 6574 655f 5f28 7365 6c66 2c20 2a61 7267  ete__(self, *arg
-00004e30: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
-00004e40: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004e50: 662e 7772 6170 7065 642e 5f5f 6465 6c65  f.wrapped.__dele
-00004e60: 7465 5f5f 282a 6172 6773 2c20 2a2a 6b77  te__(*args, **kw
-00004e70: 6172 6773 290a 0a20 2020 2069 6620 6861  args)..    if ha
-00004e80: 7361 7474 7228 6465 7363 7269 7074 6f72  sattr(descriptor
-00004e90: 2c20 275f 5f73 6574 5f6e 616d 655f 5f27  , '__set_name__'
-00004ea0: 293a 0a20 2020 2020 2064 6566 205f 5f73  ):.      def __s
-00004eb0: 6574 5f6e 616d 655f 5f28 7365 6c66 2c20  et_name__(self, 
-00004ec0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-00004ed0: 3a0a 2020 2020 2020 2020 7365 6c66 2e77  :.        self.w
-00004ee0: 7261 7070 6564 2e5f 5f73 6574 5f6e 616d  rapped.__set_nam
-00004ef0: 655f 5f28 2a61 7267 732c 202a 2a6b 7761  e__(*args, **kwa
-00004f00: 7267 7329 0a0a 2020 2020 6465 6620 5f5f  rgs)..    def __
-00004f10: 6765 7461 7474 725f 5f28 7365 6c66 2c20  getattr__(self, 
-00004f20: 6e61 6d65 293a 0a20 2020 2020 2072 6574  name):.      ret
-00004f30: 7572 6e20 6765 7461 7474 7228 7365 6c66  urn getattr(self
-00004f40: 2e77 7261 7070 6564 2c20 6e61 6d65 290a  .wrapped, name).
-00004f50: 0a20 2072 6574 7572 6e20 5f44 6573 6372  .  return _Descr
-00004f60: 6970 746f 7257 7261 7070 6572 2864 6573  iptorWrapper(des
-00004f70: 6372 6970 746f 7229 0a0a 2320 4261 7365  criptor)..# Base
-00004f80: 204d 6f64 756c 6520 6465 6669 6e69 7469   Module definiti
-00004f90: 6f6e 2e0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  on..# ----------
-00004fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000024a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 6465 6620  -----------.def 
+000024b0: 636f 6d70 6163 7428 6675 6e3a 205f 4361  compact(fun: _Ca
+000024c0: 6c6c 6162 6c65 5429 202d 3e20 5f43 616c  llableT) -> _Cal
+000024d0: 6c61 626c 6554 3a0a 2020 2222 224d 6172  lableT:.  """Mar
+000024e0: 6b73 2074 6865 2067 6976 656e 206d 6f64  ks the given mod
+000024f0: 756c 6520 6d65 7468 6f64 2061 6c6c 6f77  ule method allow
+00002500: 696e 6720 696e 6c69 6e65 6420 7375 626d  ing inlined subm
+00002510: 6f64 756c 6573 2e0a 0a20 204d 6574 686f  odules...  Metho
+00002520: 6473 2077 7261 7070 6564 2069 6e20 4063  ds wrapped in @c
+00002530: 6f6d 7061 6374 2063 616e 2064 6566 696e  ompact can defin
+00002540: 6520 7375 626d 6f64 756c 6573 2064 6972  e submodules dir
+00002550: 6563 746c 7920 7769 7468 696e 2074 6865  ectly within the
+00002560: 206d 6574 686f 642e 0a0a 2020 466f 7220   method...  For 
+00002570: 696e 7374 616e 6365 3a3a 0a0a 2020 2020  instance::..    
+00002580: 4063 6f6d 7061 6374 0a20 2020 205f 5f63  @compact.    __c
+00002590: 616c 6c5f 5f28 7365 6c66 2c20 782c 2066  all__(self, x, f
+000025a0: 6561 7475 7265 7329 3a0a 2020 2020 2020  eatures):.      
+000025b0: 7820 3d20 6e6e 2e44 656e 7365 2866 6561  x = nn.Dense(fea
+000025c0: 7475 7265 7329 2878 290a 2020 2020 2020  tures)(x).      
+000025d0: 2e2e 2e0a 0a20 2041 7420 6d6f 7374 206f  .....  At most o
+000025e0: 6e65 206d 6574 686f 6420 696e 2065 6163  ne method in eac
+000025f0: 6820 4d6f 6475 6c65 206d 6179 2062 6520  h Module may be 
+00002600: 7772 6170 7065 6420 7769 7468 2040 636f  wrapped with @co
+00002610: 6d70 6163 742e 0a0a 2020 4172 6773 3a0a  mpact...  Args:.
+00002620: 2020 2020 6675 6e3a 2054 6865 204d 6f64      fun: The Mod
+00002630: 756c 6520 6d65 7468 6f64 2074 6f20 6d61  ule method to ma
+00002640: 726b 2061 7320 636f 6d70 6163 742e 0a20  rk as compact.. 
+00002650: 2052 6574 7572 6e73 3a0a 2020 2020 5468   Returns:.    Th
+00002660: 6520 6769 7665 6e20 6675 6e63 7469 6f6e  e given function
+00002670: 2060 6675 6e60 206d 6172 6b65 6420 6173   `fun` marked as
+00002680: 2063 6f6d 7061 6374 2e0a 2020 2222 220a   compact..  """.
+00002690: 2020 6675 6e2e 636f 6d70 6163 7420 3d20    fun.compact = 
+000026a0: 5472 7565 2020 2320 7479 7065 3a20 6967  True  # type: ig
+000026b0: 6e6f 7265 5b61 7474 722d 6465 6669 6e65  nore[attr-define
+000026c0: 645d 0a20 2072 6574 7572 6e20 6675 6e0a  d].  return fun.
+000026d0: 0a0a 6465 6620 6e6f 7772 6170 2866 756e  ..def nowrap(fun
+000026e0: 3a20 5f43 616c 6c61 626c 6554 2920 2d3e  : _CallableT) ->
+000026f0: 205f 4361 6c6c 6162 6c65 543a 0a20 2022   _CallableT:.  "
+00002700: 2222 4d61 726b 7320 7468 6520 6769 7665  ""Marks the give
+00002710: 6e20 6d6f 6475 6c65 206d 6574 686f 6420  n module method 
+00002720: 6173 2061 2068 656c 7065 7220 6d65 7468  as a helper meth
+00002730: 6f64 2074 6861 7420 6e65 6564 6e27 7420  od that needn't 
+00002740: 6265 2077 7261 7070 6564 2e0a 0a20 204d  be wrapped...  M
+00002750: 6574 686f 6473 2077 7261 7070 6564 2069  ethods wrapped i
+00002760: 6e20 406e 6f77 7261 7020 6172 6520 7072  n @nowrap are pr
+00002770: 6976 6174 6520 6865 6c70 6572 206d 6574  ivate helper met
+00002780: 686f 6473 2074 6861 7420 6e65 6564 6e27  hods that needn'
+00002790: 7420 6265 2077 7261 7070 6564 0a20 2077  t be wrapped.  w
+000027a0: 6974 6820 7468 6520 7374 6174 6520 6861  ith the state ha
+000027b0: 6e64 6c65 7220 6f72 2061 2073 6570 6172  ndler or a separ
+000027c0: 6174 6520 6e61 6d65 645f 6361 6c6c 2074  ate named_call t
+000027d0: 7261 6e73 666f 726d 2e0a 0a20 2054 6869  ransform...  Thi
+000027e0: 7320 6973 206e 6565 6465 6420 696e 2073  s is needed in s
+000027f0: 6576 6572 616c 2063 6f6e 6372 6574 6520  everal concrete 
+00002800: 696e 7374 616e 6365 733a 0a20 2020 2d20  instances:.   - 
+00002810: 6966 2079 6f75 2772 6520 7375 6263 6c61  if you're subcla
+00002820: 7373 696e 6720 6120 6d65 7468 6f64 206c  ssing a method l
+00002830: 696b 6520 4d6f 6475 6c65 2e70 6172 616d  ike Module.param
+00002840: 2061 6e64 2064 6f6e 2774 2077 616e 7420   and don't want 
+00002850: 7468 6973 0a20 2020 2020 6f76 6572 7269  this.     overri
+00002860: 6465 6e20 636f 7265 2066 756e 6374 696f  den core functio
+00002870: 6e20 6465 636f 7261 7465 6420 7769 7468  n decorated with
+00002880: 2074 6865 2073 7461 7465 206d 616e 6167   the state manag
+00002890: 656d 656e 7420 7772 6170 7065 722e 0a20  ement wrapper.. 
+000028a0: 2020 2d20 4966 2079 6f75 2077 616e 7420    - If you want 
+000028b0: 6120 6d65 7468 6f64 2074 6f20 6265 2063  a method to be c
+000028c0: 616c 6c61 626c 6520 6672 6f6d 2061 6e20  allable from an 
+000028d0: 756e 626f 756e 6420 4d6f 6475 6c65 2028  unbound Module (
+000028e0: 652e 672e 3a20 610a 2020 2020 2066 756e  e.g.: a.     fun
+000028f0: 6374 696f 6e20 6f66 2063 6f6e 7374 7275  ction of constru
+00002900: 6374 696f 6e20 6f66 2061 7267 756d 656e  ction of argumen
+00002910: 7473 2074 6861 7420 646f 6573 6e27 7420  ts that doesn't 
+00002920: 6465 7065 6e64 206f 6e20 7061 7261 6d73  depend on params
+00002930: 2f52 4e47 7329 0a0a 2020 466f 7220 696e  /RNGs)..  For in
+00002940: 7374 616e 6365 3a3a 0a0a 2020 2020 406e  stance::..    @n
+00002950: 6f77 7261 700a 2020 2020 6465 6620 5f6d  owrap.    def _m
+00002960: 616b 655f 6465 6e73 6528 7365 6c66 2c20  ake_dense(self, 
+00002970: 6e75 6d5f 6665 6174 7572 6573 293a 0a20  num_features):. 
+00002980: 2020 2020 2072 6574 7572 6e20 6e6e 2e44       return nn.D
+00002990: 656e 7365 286e 756d 5f66 6561 7475 7265  ense(num_feature
+000029a0: 7329 0a0a 2020 2020 4063 6f6d 7061 6374  s)..    @compact
+000029b0: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
+000029c0: 5f28 7365 6c66 2c20 7829 3a0a 2020 2020  _(self, x):.    
+000029d0: 2020 2320 6e6f 7720 7361 6665 2074 6f20    # now safe to 
+000029e0: 7573 6520 636f 6e73 7472 7563 746f 7220  use constructor 
+000029f0: 6865 6c70 6572 2065 7665 6e20 6966 2075  helper even if u
+00002a00: 7369 6e67 206e 616d 6564 5f63 616c 6c0a  sing named_call.
+00002a10: 2020 2020 2020 6465 6e73 6520 3d20 7365        dense = se
+00002a20: 6c66 2e5f 6d61 6b65 5f64 656e 7365 2873  lf._make_dense(s
+00002a30: 656c 662e 6e75 6d5f 6665 6174 7572 6573  elf.num_features
+00002a40: 290a 2020 2020 2020 7265 7475 726e 2064  ).      return d
+00002a50: 656e 7365 2878 290a 0a20 2041 7267 733a  ense(x)..  Args:
+00002a60: 0a20 2020 2066 756e 3a20 5468 6520 4d6f  .    fun: The Mo
+00002a70: 6475 6c65 206d 6574 686f 6420 746f 206d  dule method to m
+00002a80: 6172 6b20 6173 206e 6f77 7261 702e 0a20  ark as nowrap.. 
+00002a90: 2052 6574 7572 6e73 3a0a 2020 2020 5468   Returns:.    Th
+00002aa0: 6520 6769 7665 6e20 6675 6e63 7469 6f6e  e given function
+00002ab0: 2060 6675 6e60 206d 6172 6b65 6420 6173   `fun` marked as
+00002ac0: 206e 6f77 7261 702e 0a20 2022 2222 0a20   nowrap..  """. 
+00002ad0: 2066 756e 2e6e 6f77 7261 7020 3d20 5472   fun.nowrap = Tr
+00002ae0: 7565 2020 2320 7479 7065 3a20 6967 6e6f  ue  # type: igno
+00002af0: 7265 5b61 7474 722d 6465 6669 6e65 645d  re[attr-defined]
+00002b00: 0a20 2072 6574 7572 6e20 6675 6e0a 0a0a  .  return fun...
+00002b10: 6465 6620 5f67 6574 5f6c 6f63 616c 5f6d  def _get_local_m
+00002b20: 6574 686f 645f 6e61 6d65 7328 636c 733a  ethod_names(cls:
+00002b30: 2041 6e79 2c0a 2020 2020 2020 2020 2020   Any,.          
+00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b50: 2020 6578 636c 7564 653a 2049 7465 7261    exclude: Itera
+00002b60: 626c 655b 7374 725d 203d 2028 2929 202d  ble[str] = ()) -
+00002b70: 3e20 5475 706c 655b 7374 722c 202e 2e2e  > Tuple[str, ...
+00002b80: 5d3a 0a20 2022 2222 4765 7473 206d 6574  ]:.  """Gets met
+00002b90: 686f 6420 6e61 6d65 7320 6f66 2061 2063  hod names of a c
+00002ba0: 6c61 7373 2c20 6578 636c 7564 696e 6720  lass, excluding 
+00002bb0: 636c 6173 7320 616e 6420 7374 6174 6963  class and static
+00002bc0: 206d 6574 686f 6473 2e0a 0a20 2041 7267   methods...  Arg
+00002bd0: 733a 0a20 2020 2063 6c73 3a20 5468 6520  s:.    cls: The 
+00002be0: 636c 6173 7320 746f 2067 6574 206d 6574  class to get met
+00002bf0: 686f 6420 6e61 6d65 7320 666f 722e 0a20  hod names for.. 
+00002c00: 2020 2065 7863 6c75 6465 3a20 4e61 6d65     exclude: Name
+00002c10: 7320 746f 2065 7863 6c75 6465 2066 726f  s to exclude fro
+00002c20: 6d20 6f75 7470 7574 2e0a 2020 5265 7475  m output..  Retu
+00002c30: 726e 733a 0a20 2020 2041 206c 6973 7420  rns:.    A list 
+00002c40: 6f66 206d 6574 686f 6420 6e61 6d65 732e  of method names.
+00002c50: 0a20 2022 2222 0a20 2074 7275 655f 6d65  .  """.  true_me
+00002c60: 7468 6f64 7320 3d20 7365 7428 290a 2020  thods = set().  
+00002c70: 666f 7220 6d20 696e 2063 6c73 2e5f 5f64  for m in cls.__d
+00002c80: 6963 745f 5f3a 0a20 2020 2069 6620 6361  ict__:.    if ca
+00002c90: 6c6c 6162 6c65 2863 6c73 2e5f 5f64 6963  llable(cls.__dic
+00002ca0: 745f 5f5b 6d5d 2920 616e 6420 6e6f 7420  t__[m]) and not 
+00002cb0: 696e 7370 6563 742e 6973 636c 6173 7328  inspect.isclass(
+00002cc0: 636c 732e 5f5f 6469 6374 5f5f 5b6d 5d29  cls.__dict__[m])
+00002cd0: 3a20 2023 2070 7974 7970 653a 2064 6973  :  # pytype: dis
+00002ce0: 6162 6c65 3d6e 6f74 2d73 7570 706f 7274  able=not-support
+00002cf0: 6564 2d79 6574 0a20 2020 2020 206d 7479  ed-yet.      mty
+00002d00: 7065 203d 2074 7970 6528 636c 732e 5f5f  pe = type(cls.__
+00002d10: 6469 6374 5f5f 5b6d 5d29 0a20 2020 2020  dict__[m]).     
+00002d20: 2069 6620 6d74 7970 6520 213d 2073 7461   if mtype != sta
+00002d30: 7469 636d 6574 686f 6420 616e 6420 6d74  ticmethod and mt
+00002d40: 7970 6520 213d 2063 6c61 7373 6d65 7468  ype != classmeth
+00002d50: 6f64 3a0a 2020 2020 2020 2020 7472 7565  od:.        true
+00002d60: 5f6d 6574 686f 6473 2e61 6464 286d 290a  _methods.add(m).
+00002d70: 2020 7265 7475 726e 2074 7570 6c65 2874    return tuple(t
+00002d80: 7275 655f 6d65 7468 6f64 732e 6469 6666  rue_methods.diff
+00002d90: 6572 656e 6365 2873 6574 2865 7863 6c75  erence(set(exclu
+00002da0: 6465 2929 290a 0a64 6566 205f 6765 745f  de)))..def _get_
+00002db0: 6c6f 6361 6c5f 6465 7363 7269 7074 6f72  local_descriptor
+00002dc0: 5f6e 616d 6573 2863 6c73 3a20 416e 792c  _names(cls: Any,
+00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002df0: 2065 7863 6c75 6465 3a20 4974 6572 6162   exclude: Iterab
+00002e00: 6c65 5b73 7472 5d20 3d20 2829 2920 2d3e  le[str] = ()) ->
+00002e10: 2054 7570 6c65 5b73 7472 2c20 2e2e 2e5d   Tuple[str, ...]
+00002e20: 3a0a 2020 2222 2247 6574 7320 6465 7363  :.  """Gets desc
+00002e30: 7269 7074 6f72 206e 616d 6573 206f 6620  riptor names of 
+00002e40: 6120 636c 6173 732e 0a0a 2020 4172 6773  a class...  Args
+00002e50: 3a0a 2020 2020 636c 733a 2054 6865 2063  :.    cls: The c
+00002e60: 6c61 7373 2074 6f20 6765 7420 7072 6f70  lass to get prop
+00002e70: 6572 7479 206e 616d 6573 2066 6f72 2e0a  erty names for..
+00002e80: 2020 2020 6578 636c 7564 653a 204e 616d      exclude: Nam
+00002e90: 6573 2074 6f20 6578 636c 7564 6520 6672  es to exclude fr
+00002ea0: 6f6d 206f 7574 7075 742e 0a20 2052 6574  om output..  Ret
+00002eb0: 7572 6e73 3a0a 2020 2020 4120 6c69 7374  urns:.    A list
+00002ec0: 206f 6620 7072 6f70 6572 7479 206e 616d   of property nam
+00002ed0: 6573 2e0a 2020 2222 220a 2020 7472 7565  es..  """.  true
+00002ee0: 5f70 726f 7065 7274 6965 7320 3d20 7365  _properties = se
+00002ef0: 7428 290a 2020 666f 7220 6d2c 2061 7474  t().  for m, att
+00002f00: 7220 696e 2063 6c73 2e5f 5f64 6963 745f  r in cls.__dict_
+00002f10: 5f2e 6974 656d 7328 293a 0a20 2020 2069  _.items():.    i
+00002f20: 6620 6e6f 7420 6361 6c6c 6162 6c65 2861  f not callable(a
+00002f30: 7474 7229 2061 6e64 2028 0a20 2020 2020  ttr) and (.     
+00002f40: 2068 6173 6174 7472 2861 7474 722c 2027   hasattr(attr, '
+00002f50: 5f5f 6765 745f 5f27 2920 6f72 2068 6173  __get__') or has
+00002f60: 6174 7472 2861 7474 722c 2027 5f5f 7365  attr(attr, '__se
+00002f70: 745f 5f27 2920 6f72 0a20 2020 2020 2068  t__') or.      h
+00002f80: 6173 6174 7472 2861 7474 722c 2027 5f5f  asattr(attr, '__
+00002f90: 6465 6c65 7465 5f5f 2729 0a20 2020 2029  delete__').    )
+00002fa0: 3a0a 2020 2020 2020 6d74 7970 6520 3d20  :.      mtype = 
+00002fb0: 7479 7065 2861 7474 7229 0a20 2020 2020  type(attr).     
+00002fc0: 2069 6620 6d74 7970 6520 213d 2073 7461   if mtype != sta
+00002fd0: 7469 636d 6574 686f 6420 616e 6420 6d74  ticmethod and mt
+00002fe0: 7970 6520 213d 2063 6c61 7373 6d65 7468  ype != classmeth
+00002ff0: 6f64 3a0a 2020 2020 2020 2020 7472 7565  od:.        true
+00003000: 5f70 726f 7065 7274 6965 732e 6164 6428  _properties.add(
+00003010: 6d29 0a20 2072 6574 7572 6e20 7475 706c  m).  return tupl
+00003020: 6528 7472 7565 5f70 726f 7065 7274 6965  e(true_propertie
+00003030: 732e 6469 6666 6572 656e 6365 2873 6574  s.difference(set
+00003040: 2865 7863 6c75 6465 2929 290a 0a0a 6465  (exclude)))...de
+00003050: 6620 7772 6170 5f6d 6574 686f 645f 6f6e  f wrap_method_on
+00003060: 6365 2866 756e 3a20 4361 6c6c 6162 6c65  ce(fun: Callable
+00003070: 5b2e 2e2e 2c20 416e 795d 2920 2d3e 2043  [..., Any]) -> C
+00003080: 616c 6c61 626c 655b 2e2e 2e2c 2041 6e79  allable[..., Any
+00003090: 5d3a 0a20 2022 2222 4d61 6e61 6765 7320  ]:.  """Manages 
+000030a0: 4d6f 6475 6c65 2073 7461 7465 2066 6f72  Module state for
+000030b0: 2061 2067 6976 656e 2075 7365 722d 6465   a given user-de
+000030c0: 6669 6e65 6420 6d65 7468 6f64 2e0a 0a20  fined method... 
+000030d0: 2041 7267 733a 0a20 2020 2066 756e 3a20   Args:.    fun: 
+000030e0: 5573 6572 2d64 6566 696e 6564 204d 6f64  User-defined Mod
+000030f0: 756c 6520 6d65 7468 6f64 2074 6f20 6d61  ule method to ma
+00003100: 6e61 6765 2073 7461 7465 2066 6f72 2e0a  nage state for..
+00003110: 2020 5265 7475 726e 733a 0a20 2020 2057    Returns:.    W
+00003120: 7261 7070 6564 206d 6574 686f 642e 0a20  rapped method.. 
+00003130: 2022 2222 0a20 2023 2044 6f6e 2774 2072   """.  # Don't r
+00003140: 6577 7261 7020 6d65 7468 6f64 7320 7468  ewrap methods th
+00003150: 6174 2068 6176 6520 616c 7265 6164 7920  at have already 
+00003160: 6861 6420 7468 6520 7374 6174 6520 6d61  had the state ma
+00003170: 6e61 6765 6d65 6e74 2077 7261 7070 6572  nagement wrapper
+00003180: 0a20 2023 2061 7070 6c69 6564 2069 6e20  .  # applied in 
+00003190: 7468 6520 6465 636f 7261 746f 7220 7374  the decorator st
+000031a0: 6163 6b2e 2020 5468 6973 2077 7261 7070  ack.  This wrapp
+000031b0: 6572 2073 686f 756c 6420 616c 7761 7973  er should always
+000031c0: 2062 6520 6170 706c 6965 640a 2020 2320   be applied.  # 
+000031d0: 6265 666f 7265 2074 7261 6e73 666f 726d  before transform
+000031e0: 6174 696f 6e20 7772 6170 7065 7273 2e0a  ation wrappers..
+000031f0: 2020 6966 2068 6173 6174 7472 2866 756e    if hasattr(fun
+00003200: 2c20 276d 6574 686f 645f 6861 6e64 6c65  , 'method_handle
+00003210: 725f 7772 6170 7065 6427 293a 0a20 2020  r_wrapped'):.   
+00003220: 2072 6574 7572 6e20 6675 6e0a 0a20 2040   return fun..  @
+00003230: 6675 6e63 746f 6f6c 732e 7772 6170 7328  functools.wraps(
+00003240: 6675 6e29 0a20 2064 6566 2077 7261 7070  fun).  def wrapp
+00003250: 6564 5f6d 6f64 756c 655f 6d65 7468 6f64  ed_module_method
+00003260: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
+00003270: 293a 0a20 2020 2023 2057 6520 6d69 6768  ):.    # We migh
+00003280: 7420 6861 7665 2069 6e63 6f72 7265 6374  t have incorrect
+00003290: 6c79 2077 7261 7070 7065 6420 6120 6361  ly wrappped a ca
+000032a0: 6c6c 6162 6c65 0a20 2020 2023 2074 6861  llable.    # tha
+000032b0: 7420 6973 206e 6f74 2061 206d 6574 686f  t is not a metho
+000032c0: 642e 2043 6865 636b 2077 6865 7468 6572  d. Check whether
+000032d0: 2074 6865 2066 6972 7374 2061 7267 2069   the first arg i
+000032e0: 7320 7365 6c66 2c0a 2020 2020 2320 6f74  s self,.    # ot
+000032f0: 6865 7277 6973 6520 6361 6c6c 2074 6865  herwise call the
+00003300: 2077 7261 7070 6564 2066 756e 6374 696f   wrapped functio
+00003310: 6e20 6173 2069 732e 0a20 2020 2069 6620  n as is..    if 
+00003320: 6172 6773 2061 6e64 2069 7369 6e73 7461  args and isinsta
+00003330: 6e63 6528 6172 6773 5b30 5d2c 204d 6f64  nce(args[0], Mod
+00003340: 756c 6529 3a0a 2020 2020 2020 7365 6c66  ule):.      self
+00003350: 2c20 6172 6773 203d 2061 7267 735b 305d  , args = args[0]
+00003360: 2c20 6172 6773 5b31 3a5d 0a20 2020 2020  , args[1:].     
+00003370: 2072 6574 7572 6e20 7365 6c66 2e5f 6361   return self._ca
+00003380: 6c6c 5f77 7261 7070 6564 5f6d 6574 686f  ll_wrapped_metho
+00003390: 6428 6675 6e2c 2061 7267 732c 206b 7761  d(fun, args, kwa
+000033a0: 7267 7329 0a20 2020 2065 6c73 653a 0a20  rgs).    else:. 
+000033b0: 2020 2020 2072 6574 7572 6e20 6675 6e28       return fun(
+000033c0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+000033d0: 0a20 2077 7261 7070 6564 5f6d 6f64 756c  .  wrapped_modul
+000033e0: 655f 6d65 7468 6f64 2e6d 6574 686f 645f  e_method.method_
+000033f0: 6861 6e64 6c65 725f 7772 6170 7065 6420  handler_wrapped 
+00003400: 3d20 5472 7565 2020 2320 7479 7065 3a20  = True  # type: 
+00003410: 6967 6e6f 7265 5b61 7474 722d 6465 6669  ignore[attr-defi
+00003420: 6e65 645d 0a20 2072 6574 7572 6e20 7772  ned].  return wr
+00003430: 6170 7065 645f 6d6f 6475 6c65 5f6d 6574  apped_module_met
+00003440: 686f 640a 0a64 6566 2077 7261 705f 6465  hod..def wrap_de
+00003450: 7363 7269 7074 6f72 5f6f 6e63 6528 6465  scriptor_once(de
+00003460: 7363 7269 7074 6f72 2920 2d3e 2022 4465  scriptor) -> "De
+00003470: 7363 7269 7074 6f72 5772 6170 7065 7222  scriptorWrapper"
+00003480: 3a0a 2020 2222 2257 7261 7073 2061 2064  :.  """Wraps a d
+00003490: 6573 6372 6970 746f 7220 746f 2067 6976  escriptor to giv
+000034a0: 6520 6265 7474 6572 2065 7272 6f72 206d  e better error m
+000034b0: 6573 7361 6765 732e 0a0a 2020 4172 6773  essages...  Args
+000034c0: 3a0a 2020 2020 7072 6f70 3a20 5573 6572  :.    prop: User
+000034d0: 2d64 6566 696e 6564 204d 6f64 756c 6520  -defined Module 
+000034e0: 6174 7472 6962 7574 6520 6465 7363 7269  attribute descri
+000034f0: 7074 6f72 2e0a 2020 5265 7475 726e 733a  ptor..  Returns:
+00003500: 0a20 2020 2057 7261 7070 6564 2064 6573  .    Wrapped des
+00003510: 6372 6970 746f 722e 0a20 2022 2222 0a20  criptor..  """. 
+00003520: 2023 2044 6f6e 2774 2072 6577 7261 7020   # Don't rewrap 
+00003530: 6465 7363 7269 7074 6f72 732e 0a20 2069  descriptors..  i
+00003540: 6620 6973 696e 7374 616e 6365 2864 6573  f isinstance(des
+00003550: 6372 6970 746f 722c 2044 6573 6372 6970  criptor, Descrip
+00003560: 746f 7257 7261 7070 6572 293a 0a20 2020  torWrapper):.   
+00003570: 2072 6574 7572 6e20 6465 7363 7269 7074   return descript
+00003580: 6f72 0a0a 2020 7265 7475 726e 2063 7265  or..  return cre
+00003590: 6174 655f 6465 7363 7269 7074 6f72 5f77  ate_descriptor_w
+000035a0: 7261 7070 6572 2864 6573 6372 6970 746f  rapper(descripto
+000035b0: 7229 0a0a 0a64 6566 205f 7772 6170 5f68  r)...def _wrap_h
+000035c0: 6173 6828 6861 7368 5f66 6e3a 2043 616c  ash(hash_fn: Cal
+000035d0: 6c61 626c 655b 2e2e 2e2c 2041 6e79 5d29  lable[..., Any])
+000035e0: 202d 3e20 4361 6c6c 6162 6c65 5b2e 2e2e   -> Callable[...
+000035f0: 2c20 416e 795d 3a0a 2020 2222 2257 7261  , Any]:.  """Wra
+00003600: 7073 2061 2068 6173 6820 6675 6e63 7469  ps a hash functi
+00003610: 6f6e 2077 6974 6820 736f 6d65 2063 6865  on with some che
+00003620: 636b 2066 6f72 2046 6c61 7820 4d6f 6475  ck for Flax Modu
+00003630: 6c65 732e 2222 220a 2020 4066 756e 6374  les.""".  @funct
+00003640: 6f6f 6c73 2e77 7261 7073 2868 6173 685f  ools.wraps(hash_
+00003650: 666e 290a 2020 6465 6620 7772 6170 7065  fn).  def wrappe
+00003660: 6428 7365 6c66 293a 0a20 2020 2069 6620  d(self):.    if 
+00003670: 7365 6c66 2e73 636f 7065 2069 7320 6e6f  self.scope is no
+00003680: 7420 4e6f 6e65 3a0a 2020 2020 2020 7261  t None:.      ra
+00003690: 6973 6520 5479 7065 4572 726f 7228 2743  ise TypeError('C
+000036a0: 616e 5c27 7420 6361 6c6c 205f 5f68 6173  an\'t call __has
+000036b0: 685f 5f20 6f6e 206d 6f64 756c 6573 2074  h__ on modules t
+000036c0: 6861 7420 686f 6c64 2076 6172 6961 626c  hat hold variabl
+000036d0: 6573 2e27 290a 2020 2020 7472 793a 0a20  es.').    try:. 
+000036e0: 2020 2020 2068 6173 685f 7661 6c75 6520       hash_value 
+000036f0: 3d20 6861 7368 5f66 6e28 7365 6c66 290a  = hash_fn(self).
+00003700: 2020 2020 6578 6365 7074 2054 7970 6545      except TypeE
+00003710: 7272 6f72 2061 7320 6578 633a 0a20 2020  rror as exc:.   
+00003720: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00003730: 6f72 2827 4661 696c 6564 2074 6f20 6861  or('Failed to ha
+00003740: 7368 2046 6c61 7820 4d6f 6475 6c65 2e20  sh Flax Module. 
+00003750: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00003760: 2020 2020 2020 2020 2027 5468 6520 6d6f           'The mo
+00003770: 6475 6c65 2070 726f 6261 626c 7920 636f  dule probably co
+00003780: 6e74 6169 6e73 2075 6e68 6173 6861 626c  ntains unhashabl
+00003790: 6520 6174 7472 6962 7574 6573 2e20 2027  e attributes.  '
+000037a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000037b0: 2020 2020 2020 2066 274d 6f64 756c 653d         f'Module=
+000037c0: 7b73 656c 667d 2729 2066 726f 6d20 6578  {self}') from ex
+000037d0: 630a 2020 2020 7265 7475 726e 2068 6173  c.    return has
+000037e0: 685f 7661 6c75 650a 2020 7265 7475 726e  h_value.  return
+000037f0: 2077 7261 7070 6564 0a0a 0a64 6566 205f   wrapped...def _
+00003800: 6765 745f 756e 626f 756e 645f 666e 286d  get_unbound_fn(m
+00003810: 6574 686f 645f 6f72 5f66 6e3a 2043 616c  ethod_or_fn: Cal
+00003820: 6c61 626c 655b 2e2e 2e2c 2041 6e79 5d29  lable[..., Any])
+00003830: 202d 3e20 4361 6c6c 6162 6c65 5b2e 2e2e   -> Callable[...
+00003840: 2c20 416e 795d 3a0a 2020 2222 2252 6574  , Any]:.  """Ret
+00003850: 7572 6e73 2061 6e20 756e 626f 756e 6420  urns an unbound 
+00003860: 6675 6e63 7469 6f6e 2066 726f 6d20 6120  function from a 
+00003870: 6d65 7468 6f64 2074 6861 7420 6973 2070  method that is p
+00003880: 6f73 7369 626c 7920 626f 756e 642e 0a0a  ossibly bound...
+00003890: 2020 5468 6973 206d 6561 6e73 2074 6861    This means tha
+000038a0: 7420 6966 2074 6865 2070 6173 7365 6420  t if the passed 
+000038b0: 6675 6e63 7469 6f6e 2062 656c 6f6e 6773  function belongs
+000038c0: 206f 6620 616e 2069 6e73 7461 6e63 6520   of an instance 
+000038d0: 6f66 2061 2063 6c61 7373 2c20 7468 656e  of a class, then
+000038e0: 0a20 2074 6865 2072 6574 7572 6e65 6420  .  the returned 
+000038f0: 6675 6e63 7469 6f6e 2064 6f65 7320 6e6f  function does no
+00003900: 206c 6f6e 6765 7220 6465 7065 6e64 206f   longer depend o
+00003910: 6e20 7468 6520 696e 7374 616e 6365 2c20  n the instance, 
+00003920: 7768 6963 6820 6973 2070 6173 7365 640a  which is passed.
+00003930: 2020 6173 2074 6865 2066 6972 7374 2061    as the first a
+00003940: 7267 756d 656e 7420 746f 2074 6865 2066  rgument to the f
+00003950: 756e 6374 696f 6e2e 0a0a 2020 4172 6773  unction...  Args
+00003960: 3a0a 2020 2020 6d65 7468 6f64 5f6f 725f  :.    method_or_
+00003970: 666e 3a20 4120 636c 6173 7320 6d65 7468  fn: A class meth
+00003980: 6f64 206f 7220 6675 6e63 7469 6f6e 2e0a  od or function..
+00003990: 2020 5265 7475 726e 733a 0a20 2020 2041    Returns:.    A
+000039a0: 6e20 756e 626f 756e 6420 7665 7273 696f  n unbound versio
+000039b0: 6e20 6f66 2069 6e70 7574 2066 756e 6374  n of input funct
+000039c0: 696f 6e2e 0a20 2022 2222 0a20 2069 6620  ion..  """.  if 
+000039d0: 2869 6e73 7065 6374 2e69 736d 6574 686f  (inspect.ismetho
+000039e0: 6428 6d65 7468 6f64 5f6f 725f 666e 2920  d(method_or_fn) 
+000039f0: 616e 640a 2020 2020 2020 6973 696e 7374  and.      isinst
+00003a00: 616e 6365 286d 6574 686f 645f 6f72 5f66  ance(method_or_f
+00003a10: 6e2e 5f5f 7365 6c66 5f5f 2c20 4d6f 6475  n.__self__, Modu
+00003a20: 6c65 2929 3a20 2023 2070 7974 7970 653a  le)):  # pytype:
+00003a30: 2064 6973 6162 6c65 3d61 7474 7269 6275   disable=attribu
+00003a40: 7465 2d65 7272 6f72 0a20 2020 206d 6574  te-error.    met
+00003a50: 686f 645f 6f72 5f66 6e20 3d20 6d65 7468  hod_or_fn = meth
+00003a60: 6f64 5f6f 725f 666e 2e5f 5f66 756e 635f  od_or_fn.__func_
+00003a70: 5f20 2023 2070 7974 7970 653a 2064 6973  _  # pytype: dis
+00003a80: 6162 6c65 3d61 7474 7269 6275 7465 2d65  able=attribute-e
+00003a90: 7272 6f72 0a0a 2020 2320 5468 6520 6d65  rror..  # The me
+00003aa0: 7468 6f64 2073 686f 756c 6420 6265 2063  thod should be c
+00003ab0: 616c 6c61 626c 652c 2061 6e64 2069 7420  allable, and it 
+00003ac0: 7368 6f75 6c64 2068 6176 6520 6174 206c  should have at l
+00003ad0: 6561 7374 206f 6e65 2061 7267 756d 656e  east one argumen
+00003ae0: 740a 2020 2320 7265 7072 6573 656e 7469  t.  # representi
+00003af0: 6e67 2074 6865 2063 6c61 7373 2074 6861  ng the class tha
+00003b00: 7420 6973 2070 6173 7365 6420 696e 2e0a  t is passed in..
+00003b10: 2020 6966 2028 6e6f 7420 6361 6c6c 6162    if (not callab
+00003b20: 6c65 286d 6574 686f 645f 6f72 5f66 6e29  le(method_or_fn)
+00003b30: 206f 720a 2020 2020 2020 6c65 6e28 696e   or.      len(in
+00003b40: 7370 6563 742e 7369 676e 6174 7572 6528  spect.signature(
+00003b50: 6d65 7468 6f64 5f6f 725f 666e 292e 7061  method_or_fn).pa
+00003b60: 7261 6d65 7465 7273 2920 3c20 3129 3a0a  rameters) < 1):.
+00003b70: 2020 2020 7261 6973 6520 6572 726f 7273      raise errors
+00003b80: 2e41 7070 6c79 4d6f 6475 6c65 496e 7661  .ApplyModuleInva
+00003b90: 6c69 644d 6574 686f 6445 7272 6f72 286d  lidMethodError(m
+00003ba0: 6574 686f 645f 6f72 5f66 6e29 0a0a 2020  ethod_or_fn)..  
+00003bb0: 7265 7475 726e 206d 6574 686f 645f 6f72  return method_or
+00003bc0: 5f66 6e0a 0a0a 636c 6173 7320 5365 7475  _fn...class Setu
+00003bd0: 7053 7461 7465 2865 6e75 6d2e 496e 7445  pState(enum.IntE
+00003be0: 6e75 6d29 3a0a 2020 2320 7365 7475 7028  num):.  # setup(
+00003bf0: 2920 6861 7320 6e6f 7420 6265 656e 2063  ) has not been c
+00003c00: 616c 6c65 642e 0a20 204e 4557 203d 2030  alled..  NEW = 0
+00003c10: 0a20 2023 2073 6574 7570 2829 2068 6173  .  # setup() has
+00003c20: 2062 6565 6e20 6361 6c6c 6564 206f 7574   been called out
+00003c30: 7369 6465 2061 2074 7261 6e73 666f 726d  side a transform
+00003c40: 2062 6f75 6e64 6172 792e 0a20 2054 5241   boundary..  TRA
+00003c50: 4e53 464f 524d 4544 203d 2031 0a20 2023  NSFORMED = 1.  #
+00003c60: 2073 6574 7570 2829 2068 6173 2062 6565   setup() has bee
+00003c70: 6e20 6361 6c6c 6564 2e0a 2020 444f 4e45  n called..  DONE
+00003c80: 203d 2032 0a0a 0a40 6461 7461 636c 6173   = 2...@dataclas
+00003c90: 7365 732e 6461 7461 636c 6173 730a 636c  ses.dataclass.cl
+00003ca0: 6173 7320 5f4d 6f64 756c 6549 6e74 6572  ass _ModuleInter
+00003cb0: 6e61 6c53 7461 7465 3a0a 2020 2222 2245  nalState:.  """E
+00003cc0: 7068 656d 6572 616c 204d 6f64 756c 6520  phemeral Module 
+00003cd0: 4576 616c 7561 7469 6f6e 2053 7461 7465  Evaluation State
+00003ce0: 2e0a 0a20 2046 6f72 2063 6c61 7269 7479  ...  For clarity
+00003cf0: 2c20 7765 2063 6f6c 6c65 6374 2061 6c6c  , we collect all
+00003d00: 206f 6620 7468 6520 7465 6d70 6f72 6172   of the temporar
+00003d10: 7920 666c 6167 7320 616e 6420 6570 6865  y flags and ephe
+00003d20: 6d65 7261 6c20 7374 6174 6520 7573 6564  meral state used
+00003d30: 2062 790a 2020 4d6f 6475 6c65 7320 666f   by.  Modules fo
+00003d40: 7220 6175 746f 6e61 6d69 6e67 2061 6e64  r autonaming and
+00003d50: 2065 7272 6f72 206d 6573 7361 6765 7320   error messages 
+00003d60: 6865 7265 2c20 616c 6f6e 6773 6964 6520  here, alongside 
+00003d70: 7468 6520 7275 6c65 7320 7573 6564 0a20  the rules used. 
+00003d80: 2074 6f20 7061 7373 2074 6869 7320 6570   to pass this ep
+00003d90: 6865 6d65 7261 6c20 7374 6174 6520 6163  hemeral state ac
+00003da0: 726f 7373 2074 7261 6e73 666f 726d 2062  ross transform b
+00003db0: 6f75 6e64 6172 6965 732e 0a20 2022 2222  oundaries..  """
+00003dc0: 0a20 2069 6e5f 636f 6d70 6163 745f 6d65  .  in_compact_me
+00003dd0: 7468 6f64 3a20 626f 6f6c 203d 2046 616c  thod: bool = Fal
+00003de0: 7365 0a20 2069 6e5f 7365 7475 703a 2062  se.  in_setup: b
+00003df0: 6f6f 6c20 3d20 4661 6c73 650a 2020 7365  ool = False.  se
+00003e00: 7475 705f 6361 6c6c 6564 3a20 5365 7475  tup_called: Setu
+00003e10: 7053 7461 7465 203d 2053 6574 7570 5374  pState = SetupSt
+00003e20: 6174 652e 4e45 570a 2020 6973 5f69 6e69  ate.NEW.  is_ini
+00003e30: 7469 616c 697a 6564 3a20 626f 6f6c 203d  tialized: bool =
+00003e40: 2046 616c 7365 0a20 2061 7574 6f6e 616d   False.  autonam
+00003e50: 655f 6375 7273 6f72 3a20 4469 6374 5b73  e_cursor: Dict[s
+00003e60: 7472 2c20 696e 745d 203d 2064 6174 6163  tr, int] = datac
+00003e70: 6c61 7373 6573 2e66 6965 6c64 2864 6566  lasses.field(def
+00003e80: 6175 6c74 5f66 6163 746f 7279 3d64 6963  ault_factory=dic
+00003e90: 7429 0a20 2063 6869 6c64 7265 6e3a 2044  t).  children: D
+00003ea0: 6963 745b 7374 722c 2055 6e69 6f6e 5b73  ict[str, Union[s
+00003eb0: 7472 2c20 274d 6f64 756c 6527 5d5d 203d  tr, 'Module']] =
+00003ec0: 2064 6174 6163 6c61 7373 6573 2e66 6965   dataclasses.fie
+00003ed0: 6c64 280a 2020 2020 2020 6465 6661 756c  ld(.      defaul
+00003ee0: 745f 6661 6374 6f72 793d 6469 6374 290a  t_factory=dict).
+00003ef0: 0a20 2064 6566 2072 6573 6574 2873 656c  .  def reset(sel
+00003f00: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00003f10: 2222 2252 6573 6574 7320 7472 616e 7369  """Resets transi
+00003f20: 656e 7420 7374 6174 652e 0a0a 2020 2020  ent state...    
+00003f30: 5468 6973 2066 756e 6374 696f 6e20 6973  This function is
+00003f40: 2063 616c 6c65 6420 6166 7465 7220 6561   called after ea
+00003f50: 6368 206d 6f64 756c 6520 6d65 7468 6f64  ch module method
+00003f60: 2c20 736f 206f 6e6c 7920 6174 7472 6962  , so only attrib
+00003f70: 7574 6573 2074 6861 740a 2020 2020 6172  utes that.    ar
+00003f80: 6520 6d65 7468 6f64 2d64 6570 656e 6465  e method-depende
+00003f90: 6e74 2061 7265 2072 6573 6574 2e0a 2020  nt are reset..  
+00003fa0: 2020 2222 220a 2020 2020 7365 6c66 2e69    """.    self.i
+00003fb0: 6e5f 636f 6d70 6163 745f 6d65 7468 6f64  n_compact_method
+00003fc0: 203d 2046 616c 7365 0a20 2020 2073 656c   = False.    sel
+00003fd0: 662e 696e 5f73 6574 7570 203d 2046 616c  f.in_setup = Fal
+00003fe0: 7365 0a20 2020 2073 656c 662e 6175 746f  se.    self.auto
+00003ff0: 6e61 6d65 5f63 7572 736f 7220 3d20 6469  name_cursor = di
+00004000: 6374 2829 0a0a 2020 6465 6620 6578 706f  ct()..  def expo
+00004010: 7274 2873 656c 6629 202d 3e20 275f 4d6f  rt(self) -> '_Mo
+00004020: 6475 6c65 496e 7465 726e 616c 5374 6174  duleInternalStat
+00004030: 6527 3a0a 2020 2020 2222 2245 7870 6f72  e':.    """Expor
+00004040: 7473 2074 7261 6e73 666f 726d 2d70 7265  ts transform-pre
+00004050: 7365 7276 6564 2073 7461 7465 2061 6372  served state acr
+00004060: 6f73 7320 7472 616e 7366 6f72 6d20 626f  oss transform bo
+00004070: 756e 6461 7279 2e22 2222 0a20 2020 2073  undary.""".    s
+00004080: 6574 7570 5f73 7461 7465 203d 2053 6574  etup_state = Set
+00004090: 7570 5374 6174 652e 5452 414e 5346 4f52  upState.TRANSFOR
+000040a0: 4d45 4420 6966 2073 656c 662e 7365 7475  MED if self.setu
+000040b0: 705f 6361 6c6c 6564 2065 6c73 6520 5365  p_called else Se
+000040c0: 7475 7053 7461 7465 2e4e 4557 0a20 2020  tupState.NEW.   
+000040d0: 2063 6c6f 6e65 6420 3d20 5f4d 6f64 756c   cloned = _Modul
+000040e0: 6549 6e74 6572 6e61 6c53 7461 7465 280a  eInternalState(.
+000040f0: 2020 2020 2020 2020 696e 5f63 6f6d 7061          in_compa
+00004100: 6374 5f6d 6574 686f 643d 7365 6c66 2e69  ct_method=self.i
+00004110: 6e5f 636f 6d70 6163 745f 6d65 7468 6f64  n_compact_method
+00004120: 2c0a 2020 2020 2020 2020 696e 5f73 6574  ,.        in_set
+00004130: 7570 3d73 656c 662e 696e 5f73 6574 7570  up=self.in_setup
+00004140: 2c0a 2020 2020 2020 2020 7365 7475 705f  ,.        setup_
+00004150: 6361 6c6c 6564 3d73 6574 7570 5f73 7461  called=setup_sta
+00004160: 7465 2c0a 2020 2020 2020 2020 6973 5f69  te,.        is_i
+00004170: 6e69 7469 616c 697a 6564 3d73 656c 662e  nitialized=self.
+00004180: 6973 5f69 6e69 7469 616c 697a 6564 2c0a  is_initialized,.
+00004190: 2020 2020 2020 2020 6175 746f 6e61 6d65          autoname
+000041a0: 5f63 7572 736f 723d 6469 6374 2873 656c  _cursor=dict(sel
+000041b0: 662e 6175 746f 6e61 6d65 5f63 7572 736f  f.autoname_curso
+000041c0: 7229 290a 2020 2020 7265 7475 726e 2063  r)).    return c
+000041d0: 6c6f 6e65 640a 0a20 2064 6566 2072 6569  loned..  def rei
+000041e0: 6d70 6f72 7428 7365 6c66 2c20 6f74 6865  mport(self, othe
+000041f0: 723a 2027 5f4d 6f64 756c 6549 6e74 6572  r: '_ModuleInter
+00004200: 6e61 6c53 7461 7465 2729 202d 3e20 4e6f  nalState') -> No
+00004210: 6e65 3a0a 2020 2020 2222 2252 652d 696d  ne:.    """Re-im
+00004220: 706f 7274 7320 7472 616e 7366 6f72 6d2d  ports transform-
+00004230: 7072 6573 6572 7665 6420 7374 6174 6520  preserved state 
+00004240: 6672 6f6d 2061 6372 6f73 7320 7472 616e  from across tran
+00004250: 7366 6f72 6d20 626f 756e 6461 7279 2e22  sform boundary."
+00004260: 2222 0a20 2020 2073 656c 662e 696e 5f63  "".    self.in_c
+00004270: 6f6d 7061 6374 5f6d 6574 686f 6420 3d20  ompact_method = 
+00004280: 6f74 6865 722e 696e 5f63 6f6d 7061 6374  other.in_compact
+00004290: 5f6d 6574 686f 640a 2020 2020 7365 6c66  _method.    self
+000042a0: 2e69 6e5f 7365 7475 7020 3d20 6f74 6865  .in_setup = othe
+000042b0: 722e 696e 5f73 6574 7570 0a20 2020 2073  r.in_setup.    s
+000042c0: 656c 662e 6973 5f69 6e69 7469 616c 697a  elf.is_initializ
+000042d0: 6564 203d 206f 7468 6572 2e69 735f 696e  ed = other.is_in
+000042e0: 6974 6961 6c69 7a65 640a 2020 2020 7365  itialized.    se
+000042f0: 6c66 2e61 7574 6f6e 616d 655f 6375 7273  lf.autoname_curs
+00004300: 6f72 203d 2064 6963 7428 6f74 6865 722e  or = dict(other.
+00004310: 6175 746f 6e61 6d65 5f63 7572 736f 7229  autoname_cursor)
+00004320: 0a0a 5f75 6e69 6e69 7469 616c 697a 6564  .._uninitialized
+00004330: 5f6d 6f64 756c 655f 696e 7465 726e 616c  _module_internal
+00004340: 5f73 7461 7465 203d 205f 4d6f 6475 6c65  _state = _Module
+00004350: 496e 7465 726e 616c 5374 6174 6528 290a  InternalState().
+00004360: 0a0a 5f55 4e44 4546 494e 4544 5f43 4f50  .._UNDEFINED_COP
+00004370: 595f 5049 434b 4c45 5f4d 4554 484f 4453  Y_PICKLE_METHODS
+00004380: 203d 2028 0a20 2020 2027 5f5f 6765 7473   = (.    '__gets
+00004390: 7461 7465 5f5f 272c 2027 5f5f 7365 7473  tate__', '__sets
+000043a0: 7461 7465 5f5f 272c 2027 5f5f 6765 746e  tate__', '__getn
+000043b0: 6577 6172 6773 5f65 785f 5f27 2c0a 2020  ewargs_ex__',.  
+000043c0: 2020 275f 5f72 6564 7563 655f 5f27 2c20    '__reduce__', 
+000043d0: 275f 5f72 6564 7563 655f 6578 5f5f 272c  '__reduce_ex__',
+000043e0: 2027 5f5f 636f 7079 5f5f 272c 2027 5f5f   '__copy__', '__
+000043f0: 6465 6570 636f 7079 5f5f 2729 0a0a 0a5f  deepcopy__')..._
+00004400: 6361 6368 6573 3a20 2777 6561 6b72 6566  caches: 'weakref
+00004410: 2e57 6561 6b4b 6579 4469 6374 696f 6e61  .WeakKeyDictiona
+00004420: 7279 5b53 636f 7065 2c20 7765 616b 7265  ry[Scope, weakre
+00004430: 662e 5765 616b 5661 6c75 6544 6963 7469  f.WeakValueDicti
+00004440: 6f6e 6172 795b 466c 6178 4964 2c20 4d6f  onary[FlaxId, Mo
+00004450: 6475 6c65 5d5d 2720 3d20 280a 2020 2020  dule]]' = (.    
+00004460: 7765 616b 7265 662e 5765 616b 4b65 7944  weakref.WeakKeyD
+00004470: 6963 7469 6f6e 6172 7928 2929 0a0a 0a74  ictionary())...t
+00004480: 7570 6c65 5f72 6564 7563 6520 3d20 6c61  uple_reduce = la
+00004490: 6d62 6461 2078 732c 2078 3a20 7873 202b  mbda xs, x: xs +
+000044a0: 2028 782c 290a 7475 706c 655f 696e 6974   (x,).tuple_init
+000044b0: 203d 206c 616d 6264 613a 2028 290a 0a0a   = lambda: ()...
+000044c0: 6361 7074 7572 655f 6361 6c6c 5f69 6e74  capture_call_int
+000044d0: 6572 6d65 6469 6174 6573 203d 206c 616d  ermediates = lam
+000044e0: 6264 6120 5f2c 206d 6574 686f 645f 6e61  bda _, method_na
+000044f0: 6d65 3a20 6d65 7468 6f64 5f6e 616d 6520  me: method_name 
+00004500: 3d3d 2027 5f5f 6361 6c6c 5f5f 270a 0a0a  == '__call__'...
+00004510: 636c 6173 7320 5061 7265 6e74 4465 7363  class ParentDesc
+00004520: 7269 7074 6f72 3a0a 2020 2222 2257 7261  riptor:.  """Wra
+00004530: 7073 2070 6172 656e 7420 6d6f 6475 6c65  ps parent module
+00004540: 2072 6566 6572 656e 6365 7320 696e 2077   references in w
+00004550: 6561 6b20 7265 6673 2e0a 0a20 2054 6869  eak refs...  Thi
+00004560: 7320 7072 6576 656e 7473 2072 6566 6572  s prevents refer
+00004570: 656e 6365 2063 7963 6c65 7320 6672 6f6d  ence cycles from
+00004580: 2066 6f72 6d69 6e67 2076 6961 2070 6172   forming via par
+00004590: 656e 7420 6c69 6e6b 7320 7768 6963 6820  ent links which 
+000045a0: 6361 6e20 6c65 6164 0a20 2074 6f20 6163  can lead.  to ac
+000045b0: 6369 6465 6e74 616c 204f 4f4d 7320 696e  cidental OOMs in
+000045c0: 2065 6167 6572 206d 6f64 6520 6475 6520   eager mode due 
+000045d0: 746f 2073 6c6f 7720 6761 7262 6167 6520  to slow garbage 
+000045e0: 636f 6c6c 6563 7469 6f6e 2061 7320 7765  collection as we
+000045f0: 6c6c 2061 730a 2020 7370 7572 696f 7573  ll as.  spurious
+00004600: 2074 7261 6365 7220 6c65 616b 7320 6475   tracer leaks du
+00004610: 7269 6e67 206a 6974 2063 6f6d 7069 6c61  ring jit compila
+00004620: 7469 6f6e 2e0a 0a20 204e 6f74 653a 2022  tion...  Note: "
+00004630: 6465 7363 7269 7074 6f72 7322 2061 7265  descriptors" are
+00004640: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
+00004650: 7079 7468 6f6e 206d 6563 6861 6e69 736d  python mechanism
+00004660: 2066 6f72 2069 6d70 6c65 6d65 6e74 696e   for implementin
+00004670: 670a 2020 6479 6e61 6d69 6320 4070 726f  g.  dynamic @pro
+00004680: 7065 7274 7920 6465 636f 7261 746f 7273  perty decorators
+00004690: 2e20 2057 6520 6e65 6564 2074 6f20 7573  .  We need to us
+000046a0: 6520 6120 7261 7720 6465 7363 7269 7074  e a raw descript
+000046b0: 6f72 2069 6e73 7465 6164 206f 6620 7468  or instead of th
+000046c0: 650a 2020 6d6f 7265 2063 6f6d 6d6f 6e20  e.  more common 
+000046d0: 6465 636f 7261 746f 7220 696e 206f 7264  decorator in ord
+000046e0: 6572 2074 6f20 666f 7263 6520 7468 6174  er to force that
+000046f0: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
+00004700: 2067 6574 7465 722f 7365 7474 6572 0a20   getter/setter. 
+00004710: 206c 6f67 6963 2061 7070 6c69 6573 2069   logic applies i
+00004720: 6e20 7375 6263 6c61 7373 6573 2065 7665  n subclasses eve
+00004730: 6e20 6166 7465 7220 7661 7269 6f75 7320  n after various 
+00004740: 6461 7461 636c 6173 7320 7472 616e 7366  dataclass transf
+00004750: 6f72 6d73 2e0a 2020 2222 220a 2020 6465  orms..  """.  de
+00004760: 6620 5f5f 6765 745f 5f28 7365 6c66 2c20  f __get__(self, 
+00004770: 6f62 6a2c 206f 626a 7479 7065 3d4e 6f6e  obj, objtype=Non
+00004780: 6529 3a0a 2020 2020 2320 6368 6563 6b20  e):.    # check 
+00004790: 6966 206f 626a 2069 7320 4e6f 6e65 2c20  if obj is None, 
+000047a0: 6861 7070 656e 7320 6475 7269 6e67 2025  happens during %
+000047b0: 6175 746f 7265 6c6f 6164 0a20 2020 2069  autoreload.    i
+000047c0: 6620 6f62 6a20 6973 204e 6f6e 653a 0a20  f obj is None:. 
+000047d0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000047e0: 0a20 2020 2070 6172 656e 7420 3d20 6f62  .    parent = ob
+000047f0: 6a65 6374 2e5f 5f67 6574 6174 7472 6962  ject.__getattrib
+00004800: 7574 655f 5f28 6f62 6a2c 2022 5f70 6172  ute__(obj, "_par
+00004810: 656e 745f 7265 6622 290a 2020 2020 7265  ent_ref").    re
+00004820: 7475 726e 2070 6172 656e 7428 2920 6966  turn parent() if
+00004830: 2069 7369 6e73 7461 6e63 6528 7061 7265   isinstance(pare
+00004840: 6e74 2c20 7765 616b 7265 662e 5265 6665  nt, weakref.Refe
+00004850: 7265 6e63 6554 7970 6529 2065 6c73 6520  renceType) else 
+00004860: 7061 7265 6e74 0a0a 2020 6465 6620 5f5f  parent..  def __
+00004870: 7365 745f 5f28 7365 6c66 2c20 6f62 6a2c  set__(self, obj,
+00004880: 2076 616c 7565 293a 0a20 2020 206d 6179   value):.    may
+00004890: 6265 5f77 6561 6b20 3d20 7765 616b 7265  be_weak = weakre
+000048a0: 662e 7265 6628 7661 6c75 6529 2069 6620  f.ref(value) if 
+000048b0: 6973 696e 7374 616e 6365 2876 616c 7565  isinstance(value
+000048c0: 2c20 4d6f 6475 6c65 2920 656c 7365 2076  , Module) else v
+000048d0: 616c 7565 0a20 2020 206f 626a 6563 742e  alue.    object.
+000048e0: 5f5f 7365 7461 7474 725f 5f28 6f62 6a2c  __setattr__(obj,
+000048f0: 2022 5f70 6172 656e 745f 7265 6622 2c20   "_parent_ref", 
+00004900: 6d61 7962 655f 7765 616b 290a 0a0a 636c  maybe_weak)...cl
+00004910: 6173 7320 4465 7363 7269 7074 6f72 2850  ass Descriptor(P
+00004920: 726f 746f 636f 6c29 3a0a 2020 5f5f 6973  rotocol):.  __is
+00004930: 6162 7374 7261 6374 6d65 7468 6f64 5f5f  abstractmethod__
+00004940: 3a20 626f 6f6c 0a20 2064 6566 205f 5f67  : bool.  def __g
+00004950: 6574 5f5f 2873 656c 662c 206f 626a 2c20  et__(self, obj, 
+00004960: 6f62 6a74 7970 653d 4e6f 6e65 2920 2d3e  objtype=None) ->
+00004970: 2041 6e79 3a20 2e2e 2e0a 2020 6465 6620   Any: ....  def 
+00004980: 5f5f 7365 745f 5f28 7365 6c66 2c20 6f62  __set__(self, ob
+00004990: 6a2c 2076 616c 7565 2920 2d3e 204e 6f6e  j, value) -> Non
+000049a0: 653a 202e 2e2e 0a20 2064 6566 205f 5f64  e: ....  def __d
+000049b0: 656c 6574 655f 5f28 7365 6c66 2c20 6f62  elete__(self, ob
+000049c0: 6a29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  j) -> None: ....
+000049d0: 2020 6465 6620 5f5f 7365 745f 6e61 6d65    def __set_name
+000049e0: 5f5f 2873 656c 662c 206f 776e 6572 2c20  __(self, owner, 
+000049f0: 6e61 6d65 2920 2d3e 204e 6f6e 653a 202e  name) -> None: .
+00004a00: 2e2e 0a0a 636c 6173 7320 4465 7363 7269  ....class Descri
+00004a10: 7074 6f72 5772 6170 7065 723a 0a20 2070  ptorWrapper:.  p
+00004a20: 6173 730a 0a64 6566 2063 7265 6174 655f  ass..def create_
+00004a30: 6465 7363 7269 7074 6f72 5f77 7261 7070  descriptor_wrapp
+00004a40: 6572 2864 6573 6372 6970 746f 723a 2044  er(descriptor: D
+00004a50: 6573 6372 6970 746f 7229 3a0a 2020 2222  escriptor):.  ""
+00004a60: 2243 7265 6174 6573 2061 2064 6573 6372  "Creates a descr
+00004a70: 6970 746f 7220 7772 6170 7065 7220 7468  iptor wrapper th
+00004a80: 6174 2063 616c 6c73 2061 2067 6574 5f66  at calls a get_f
+00004a90: 6e20 6f6e 2074 6865 2064 6573 6372 6970  n on the descrip
+00004aa0: 746f 722e 2222 220a 0a20 2063 6c61 7373  tor."""..  class
+00004ab0: 205f 4465 7363 7269 7074 6f72 5772 6170   _DescriptorWrap
+00004ac0: 7065 7228 4465 7363 7269 7074 6f72 5772  per(DescriptorWr
+00004ad0: 6170 7065 7229 3a0a 2020 2020 2222 2241  apper):.    """A
+00004ae0: 2064 6573 6372 6970 746f 7220 7468 6174   descriptor that
+00004af0: 2063 616e 2077 7261 7020 616e 7920 6465   can wrap any de
+00004b00: 7363 7269 7074 6f72 2222 220a 0a20 2020  scriptor"""..   
+00004b10: 2069 6620 6861 7361 7474 7228 6465 7363   if hasattr(desc
+00004b20: 7269 7074 6f72 2c20 275f 5f69 7361 6273  riptor, '__isabs
+00004b30: 7472 6163 746d 6574 686f 645f 5f27 293a  tractmethod__'):
+00004b40: 0a20 2020 2020 205f 5f69 7361 6273 7472  .      __isabstr
+00004b50: 6163 746d 6574 686f 645f 5f20 3d20 6465  actmethod__ = de
+00004b60: 7363 7269 7074 6f72 2e5f 5f69 7361 6273  scriptor.__isabs
+00004b70: 7472 6163 746d 6574 686f 645f 5f0a 0a20  tractmethod__.. 
+00004b80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00004b90: 7365 6c66 2c20 7772 6170 7065 643a 2044  self, wrapped: D
+00004ba0: 6573 6372 6970 746f 7229 3a0a 2020 2020  escriptor):.    
+00004bb0: 2020 7365 6c66 2e77 7261 7070 6564 203d    self.wrapped =
+00004bc0: 2077 7261 7070 6564 0a0a 2020 2020 2320   wrapped..    # 
+00004bd0: 636f 6e64 6974 696f 6e61 6c6c 7920 6465  conditionally de
+00004be0: 6669 6e65 2064 6573 6372 6970 746f 7220  fine descriptor 
+00004bf0: 6d65 7468 6f64 730a 2020 2020 6966 2068  methods.    if h
+00004c00: 6173 6174 7472 2864 6573 6372 6970 746f  asattr(descripto
+00004c10: 722c 2027 5f5f 6765 745f 5f27 293a 0a20  r, '__get__'):. 
+00004c20: 2020 2020 2064 6566 205f 5f67 6574 5f5f       def __get__
+00004c30: 2873 656c 662c 202a 6172 6773 2c20 2a2a  (self, *args, **
+00004c40: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00004c50: 2023 2068 6572 6520 7765 2077 696c 6c20   # here we will 
+00004c60: 6361 7463 6820 696e 7465 726e 616c 2041  catch internal A
+00004c70: 7474 7269 6275 7465 4572 726f 7220 616e  ttributeError an
+00004c80: 6420 7265 2d72 6169 7365 2069 7420 6173  d re-raise it as
+00004c90: 2061 0a20 2020 2020 2020 2023 206d 6f72   a.        # mor
+00004ca0: 6520 696e 666f 726d 6174 6976 6520 616e  e informative an
+00004cb0: 6420 636f 7272 6563 7420 6572 726f 7220  d correct error 
+00004cc0: 6d65 7373 6167 652e 0a20 2020 2020 2020  message..       
+00004cd0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00004ce0: 7265 7475 726e 2073 656c 662e 7772 6170  return self.wrap
+00004cf0: 7065 642e 5f5f 6765 745f 5f28 2a61 7267  ped.__get__(*arg
+00004d00: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
+00004d10: 2020 2020 2065 7863 6570 7420 4174 7472       except Attr
+00004d20: 6962 7574 6545 7272 6f72 2061 7320 653a  ibuteError as e:
+00004d30: 0a20 2020 2020 2020 2020 2072 6169 7365  .          raise
+00004d40: 2065 7272 6f72 732e 4465 7363 7269 7074   errors.Descript
+00004d50: 6f72 4174 7472 6962 7574 6545 7272 6f72  orAttributeError
+00004d60: 2829 2066 726f 6d20 650a 0a20 2020 2069  () from e..    i
+00004d70: 6620 6861 7361 7474 7228 6465 7363 7269  f hasattr(descri
+00004d80: 7074 6f72 2c20 275f 5f73 6574 5f5f 2729  ptor, '__set__')
+00004d90: 3a0a 2020 2020 2020 6465 6620 5f5f 7365  :.      def __se
+00004da0: 745f 5f28 7365 6c66 2c20 2a61 7267 732c  t__(self, *args,
+00004db0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+00004dc0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00004dd0: 7772 6170 7065 642e 5f5f 7365 745f 5f28  wrapped.__set__(
+00004de0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00004df0: 0a0a 2020 2020 6966 2068 6173 6174 7472  ..    if hasattr
+00004e00: 2864 6573 6372 6970 746f 722c 2027 5f5f  (descriptor, '__
+00004e10: 6465 6c65 7465 5f5f 2729 3a0a 2020 2020  delete__'):.    
+00004e20: 2020 6465 6620 5f5f 6465 6c65 7465 5f5f    def __delete__
+00004e30: 2873 656c 662c 202a 6172 6773 2c20 2a2a  (self, *args, **
+00004e40: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00004e50: 2072 6574 7572 6e20 7365 6c66 2e77 7261   return self.wra
+00004e60: 7070 6564 2e5f 5f64 656c 6574 655f 5f28  pped.__delete__(
+00004e70: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00004e80: 0a0a 2020 2020 6966 2068 6173 6174 7472  ..    if hasattr
+00004e90: 2864 6573 6372 6970 746f 722c 2027 5f5f  (descriptor, '__
+00004ea0: 7365 745f 6e61 6d65 5f5f 2729 3a0a 2020  set_name__'):.  
+00004eb0: 2020 2020 6465 6620 5f5f 7365 745f 6e61      def __set_na
+00004ec0: 6d65 5f5f 2873 656c 662c 202a 6172 6773  me__(self, *args
+00004ed0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00004ee0: 2020 2020 2073 656c 662e 7772 6170 7065       self.wrappe
+00004ef0: 642e 5f5f 7365 745f 6e61 6d65 5f5f 282a  d.__set_name__(*
+00004f00: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+00004f10: 0a20 2020 2064 6566 205f 5f67 6574 6174  .    def __getat
+00004f20: 7472 5f5f 2873 656c 662c 206e 616d 6529  tr__(self, name)
+00004f30: 3a0a 2020 2020 2020 7265 7475 726e 2067  :.      return g
+00004f40: 6574 6174 7472 2873 656c 662e 7772 6170  etattr(self.wrap
+00004f50: 7065 642c 206e 616d 6529 0a0a 2020 7265  ped, name)..  re
+00004f60: 7475 726e 205f 4465 7363 7269 7074 6f72  turn _Descriptor
+00004f70: 5772 6170 7065 7228 6465 7363 7269 7074  Wrapper(descript
+00004f80: 6f72 290a 0a23 2042 6173 6520 4d6f 6475  or)..# Base Modu
+00004f90: 6c65 2064 6566 696e 6974 696f 6e2e 0a23  le definition..#
+00004fa0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 00004fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00004fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00004fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004fe0: 2d2d 2d0a 0a23 2054 6865 204d 6f64 756c  ---..# The Modul
-00004ff0: 6542 6173 6520 636c 6173 7320 6973 2063  eBase class is c
-00005000: 7265 6174 6564 206f 6e6c 7920 746f 206d  reated only to m
-00005010: 616b 6520 7374 6174 6963 2061 6e61 6c79  ake static analy
-00005020: 7a65 7273 2068 6170 7079 0a23 206d 6169  zers happy.# mai
-00005030: 6e6c 7920 7079 7479 7065 2061 6e64 2070  nly pytype and p
-00005040: 7972 6967 6874 2e20 536f 6d65 206e 6f74  yright. Some not
-00005050: 6573 3a0a 2320 2a20 7079 7269 6768 7420  es:.# * pyright 
-00005060: 2863 6f72 7265 6374 6c79 2920 636f 6d70  (correctly) comp
-00005070: 6c61 696e 7320 7468 6174 204d 6f64 756c  lains that Modul
-00005080: 6520 6974 7365 6c66 2069 7320 6e6f 7420  e itself is not 
-00005090: 6120 6461 7461 636c 6173 732c 2065 7665  a dataclass, eve
-000050a0: 6e0a 2320 2020 7468 6f75 6768 2061 6c6c  n.#   though all
-000050b0: 2069 7473 2073 7562 636c 6173 7365 7320   its subclasses 
-000050c0: 616e 6420 696e 7461 6e63 6573 2041 5245  and intances ARE
-000050d0: 2064 6174 6163 6c61 7373 6573 2e20 4265   dataclasses. Be
-000050e0: 6361 7573 6520 7468 6572 6520 6973 206e  cause there is n
-000050f0: 6f0a 2320 2020 7761 7920 746f 2061 6e6e  o.#   way to ann
-00005100: 6f74 6174 6520 7468 6973 2069 6e20 6120  otate this in a 
-00005110: 7761 7920 7468 6174 2070 7972 6967 6874  way that pyright
-00005120: 2075 6e64 6572 7374 616e 6473 2c20 7765   understands, we
-00005130: 2063 7265 6174 6520 610a 2320 2020 4d6f   create a.#   Mo
-00005140: 6475 6c65 4261 7365 2063 6c61 7373 2064  duleBase class d
-00005150: 6563 6f72 6174 6564 2077 6974 6820 6064  ecorated with `d
-00005160: 6174 6163 6c61 7373 5f74 7261 6e73 666f  ataclass_transfo
-00005170: 726d 6020 7375 6368 2074 6861 7420 7079  rm` such that py
-00005180: 7269 6768 740a 2320 2020 7468 696e 6b73  right.#   thinks
-00005190: 204d 6f64 756c 6520 6973 2061 2064 6174   Module is a dat
-000051a0: 6163 6c61 7373 2028 696e 2072 6561 6c69  aclass (in reali
-000051b0: 7479 206f 6e6c 7920 7375 6263 6c61 7373  ty only subclass
-000051c0: 6573 2061 7265 2069 6e73 7461 6e74 6961  es are instantia
-000051d0: 7465 640a 2320 2020 736f 2074 6869 7320  ted.#   so this 
-000051e0: 6973 2066 696e 6529 2e0a 2320 2a20 5468  is fine)..# * Th
-000051f0: 6520 605f 5f64 6174 6163 6c61 7373 5f66  e `__dataclass_f
-00005200: 6965 6c64 735f 5f60 2061 7474 7269 6275  ields__` attribu
-00005210: 7465 2069 7320 6e65 6564 6564 2062 6563  te is needed bec
-00005220: 6175 7365 2070 7974 7970 6520 7365 656d  ause pytype seem
-00005230: 7320 746f 0a23 2020 206e 6f74 2075 6e64  s to.#   not und
-00005240: 6572 7374 616e 6420 7468 6520 6064 6174  erstand the `dat
-00005250: 6163 6c61 7373 5f74 7261 6e73 666f 726d  aclass_transform
-00005260: 6020 6465 636f 7261 746f 722c 2074 6865  ` decorator, the
-00005270: 7265 666f 7265 2077 6520 6e65 6564 0a23  refore we need.#
-00005280: 2020 2074 6f20 6164 6420 7468 6520 6174     to add the at
-00005290: 7472 6962 7574 6520 6d61 6e75 616c 6c79  tribute manually
-000052a0: 2e0a 2320 2a20 4f74 6865 7220 6174 7472  ..# * Other attr
-000052b0: 6962 7574 6573 2061 7265 2061 6e6e 6f74  ibutes are annot
-000052c0: 6174 6564 2066 6f72 2063 6f6d 706c 6574  ated for complet
-000052d0: 656e 6573 732e 2042 6563 6175 7365 2077  eness. Because w
-000052e0: 6520 6172 6520 7573 696e 670a 2320 2020  e are using.#   
-000052f0: 7468 6520 6069 6620 7479 7069 6e67 2e54  the `if typing.T
-00005300: 5950 455f 4348 4543 4b49 4e47 6020 7061  YPE_CHECKING` pa
-00005310: 7474 6572 6e2c 2074 6865 7365 2061 6e6e  ttern, these ann
-00005320: 6f74 6174 696f 6e73 2061 7265 206e 6f74  otations are not
-00005330: 2070 7265 7365 6e74 0a23 2020 2061 7420   present.#   at 
-00005340: 7275 6e74 696d 6520 736f 2074 6865 7920  runtime so they 
-00005350: 646f 6e27 7420 6166 6665 6374 2074 6865  don't affect the
-00005360: 2064 6174 6163 6c61 7373 2062 6568 6176   dataclass behav
-00005370: 696f 722e 0a40 6461 7461 636c 6173 735f  ior..@dataclass_
-00005380: 7472 616e 7366 6f72 6d28 290a 636c 6173  transform().clas
-00005390: 7320 4d6f 6475 6c65 4261 7365 3a0a 2020  s ModuleBase:.  
-000053a0: 6966 2074 7970 696e 672e 5459 5045 5f43  if typing.TYPE_C
-000053b0: 4845 434b 494e 473a 0a20 2020 2073 636f  HECKING:.    sco
-000053c0: 7065 3a20 4f70 7469 6f6e 616c 5b53 636f  pe: Optional[Sco
-000053d0: 7065 5d0a 2020 2020 5f73 7461 7465 3a20  pe].    _state: 
-000053e0: 5f4d 6f64 756c 6549 6e74 6572 6e61 6c53  _ModuleInternalS
-000053f0: 7461 7465 0a20 2020 205f 7061 7265 6e74  tate.    _parent
-00005400: 5f72 6566 3a20 556e 696f 6e5b 274d 6f64  _ref: Union['Mod
-00005410: 756c 6527 2c20 7765 616b 7265 662e 5265  ule', weakref.Re
-00005420: 6665 7265 6e63 6554 7970 655b 274d 6f64  ferenceType['Mod
-00005430: 756c 6527 5d2c 204e 6f6e 655d 0a20 2020  ule'], None].   
-00005440: 2070 6172 656e 743a 2055 6e69 6f6e 5b27   parent: Union['
-00005450: 4d6f 6475 6c65 272c 205f 5365 6e74 696e  Module', _Sentin
-00005460: 656c 2c20 4e6f 6e65 5d0a 2020 2020 5f5f  el, None].    __
-00005470: 6461 7461 636c 6173 735f 6669 656c 6473  dataclass_fields
-00005480: 5f5f 3a20 4469 6374 5b73 7472 2c20 6461  __: Dict[str, da
-00005490: 7461 636c 6173 7365 732e 4669 656c 645d  taclasses.Field]
-000054a0: 0a0a 636c 6173 7320 4d6f 6475 6c65 284d  ..class Module(M
-000054b0: 6f64 756c 6542 6173 6529 3a0a 2020 2222  oduleBase):.  ""
-000054c0: 2242 6173 6520 636c 6173 7320 666f 7220  "Base class for 
-000054d0: 616c 6c20 6e65 7572 616c 206e 6574 776f  all neural netwo
-000054e0: 726b 206d 6f64 756c 6573 2e20 4c61 7965  rk modules. Laye
-000054f0: 7273 2061 6e64 206d 6f64 656c 7320 7368  rs and models sh
-00005500: 6f75 6c64 2073 7562 636c 6173 7320 7468  ould subclass th
-00005510: 6973 2063 6c61 7373 2e0a 0a20 2041 6c6c  is class...  All
-00005520: 2046 6c61 7820 4d6f 6475 6c65 7320 6172   Flax Modules ar
-00005530: 6520 5079 7468 6f6e 2033 2e37 0a20 2060  e Python 3.7.  `
-00005540: 6461 7461 636c 6173 7365 7320 3c68 7474  dataclasses <htt
-00005550: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
-00005560: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f64  .org/3/library/d
-00005570: 6174 6163 6c61 7373 6573 2e68 746d 6c3e  ataclasses.html>
-00005580: 605f 2e20 5369 6e63 650a 2020 6461 7461  `_. Since.  data
-00005590: 636c 6173 7365 7320 7461 6b65 206f 7665  classes take ove
-000055a0: 7220 6060 5f5f 696e 6974 5f5f 6060 2c20  r ``__init__``, 
-000055b0: 796f 7520 7368 6f75 6c64 2069 6e73 7465  you should inste
-000055c0: 6164 206f 7665 7272 6964 6520 3a6d 6574  ad override :met
-000055d0: 683a 6073 6574 7570 602c 0a20 2077 6869  h:`setup`,.  whi
-000055e0: 6368 2069 7320 6175 746f 6d61 7469 6361  ch is automatica
-000055f0: 6c6c 7920 6361 6c6c 6564 2074 6f20 696e  lly called to in
-00005600: 6974 6961 6c69 7a65 2074 6865 206d 6f64  itialize the mod
-00005610: 756c 652e 0a0a 2020 4d6f 6475 6c65 7320  ule...  Modules 
-00005620: 6361 6e20 636f 6e74 6169 6e20 7375 626d  can contain subm
-00005630: 6f64 756c 6573 2c20 616e 6420 696e 2074  odules, and in t
-00005640: 6869 7320 7761 7920 6361 6e20 6265 206e  his way can be n
-00005650: 6573 7465 6420 696e 2061 2074 7265 650a  ested in a tree.
-00005660: 2020 7374 7275 6374 7572 652e 2053 7562    structure. Sub
-00005670: 6d6f 6465 6c73 2063 616e 2062 6520 6173  models can be as
-00005680: 7369 676e 6564 2061 7320 7265 6775 6c61  signed as regula
-00005690: 7220 6174 7472 6962 7574 6573 2069 6e73  r attributes ins
-000056a0: 6964 6520 7468 650a 2020 3a6d 6574 683a  ide the.  :meth:
-000056b0: 6073 6574 7570 6020 6d65 7468 6f64 2e0a  `setup` method..
-000056c0: 0a20 2059 6f75 2063 616e 2064 6566 696e  .  You can defin
-000056d0: 6520 6172 6269 7472 6172 7920 2266 6f72  e arbitrary "for
-000056e0: 7761 7264 2070 6173 7322 206d 6574 686f  ward pass" metho
-000056f0: 6473 206f 6e20 796f 7572 204d 6f64 756c  ds on your Modul
-00005700: 6520 7375 6263 6c61 7373 2e0a 2020 5768  e subclass..  Wh
-00005710: 696c 6520 6e6f 206d 6574 686f 6473 2061  ile no methods a
-00005720: 7265 2073 7065 6369 616c 2d63 6173 6564  re special-cased
-00005730: 2c20 6060 5f5f 6361 6c6c 5f5f 6060 2069  , ``__call__`` i
-00005740: 7320 6120 706f 7075 6c61 7220 6368 6f69  s a popular choi
-00005750: 6365 2062 6563 6175 7365 0a20 2069 7420  ce because.  it 
-00005760: 616c 6c6f 7773 2079 6f75 2074 6f20 7573  allows you to us
-00005770: 6520 6d6f 6475 6c65 2069 6e73 7461 6e63  e module instanc
-00005780: 6573 2061 7320 6966 2074 6865 7920 6172  es as if they ar
-00005790: 6520 6675 6e63 7469 6f6e 733a 3a0a 0a20  e functions::.. 
-000057a0: 2020 2066 726f 6d20 666c 6178 2069 6d70     from flax imp
-000057b0: 6f72 7420 6c69 6e65 6e20 6173 206e 6e0a  ort linen as nn.
-000057c0: 0a20 2020 2063 6c61 7373 204d 6f64 756c  .    class Modul
-000057d0: 6528 6e6e 2e4d 6f64 756c 6529 3a0a 2020  e(nn.Module):.  
-000057e0: 2020 2020 6665 6174 7572 6573 3a20 5475      features: Tu
-000057f0: 706c 655b 696e 742c 202e 2e2e 5d20 3d20  ple[int, ...] = 
-00005800: 2831 362c 2034 290a 0a20 2020 2020 2064  (16, 4)..      d
-00005810: 6566 2073 6574 7570 2873 656c 6629 3a0a  ef setup(self):.
-00005820: 2020 2020 2020 2020 7365 6c66 2e64 656e          self.den
-00005830: 7365 3120 3d20 4465 6e73 6528 7365 6c66  se1 = Dense(self
-00005840: 2e66 6561 7475 7265 735b 305d 290a 2020  .features[0]).  
-00005850: 2020 2020 2020 7365 6c66 2e64 656e 7365        self.dense
-00005860: 3220 3d20 4465 6e73 6528 7365 6c66 2e66  2 = Dense(self.f
-00005870: 6561 7475 7265 735b 315d 290a 0a20 2020  eatures[1])..   
-00005880: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-00005890: 7365 6c66 2c20 7829 3a0a 2020 2020 2020  self, x):.      
-000058a0: 2020 7265 7475 726e 2073 656c 662e 6465    return self.de
-000058b0: 6e73 6532 286e 6e2e 7265 6c75 2873 656c  nse2(nn.relu(sel
-000058c0: 662e 6465 6e73 6531 2878 2929 290a 0a20  f.dense1(x))).. 
-000058d0: 204f 7074 696f 6e61 6c6c 792c 2066 6f72   Optionally, for
-000058e0: 206d 6f72 6520 636f 6e63 6973 6520 6d6f   more concise mo
-000058f0: 6475 6c65 2069 6d70 6c65 6d65 6e74 6174  dule implementat
-00005900: 696f 6e73 2077 6865 7265 2073 7562 6d6f  ions where submo
-00005910: 6475 6c65 730a 2020 6465 6669 6e69 7469  dules.  definiti
-00005920: 6f6e 7320 6172 6520 636f 2d6c 6f63 6174  ons are co-locat
-00005930: 6564 2077 6974 6820 7468 6569 7220 7573  ed with their us
-00005940: 6167 652c 2079 6f75 2063 616e 2075 7365  age, you can use
-00005950: 2074 6865 0a20 203a 6d65 7468 3a60 636f   the.  :meth:`co
-00005960: 6d70 6163 7460 2077 7261 7070 6572 2e0a  mpact` wrapper..
-00005970: 2020 2222 220a 0a20 2069 6620 7479 7069    """..  if typi
-00005980: 6e67 2e54 5950 455f 4348 4543 4b49 4e47  ng.TYPE_CHECKING
-00005990: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000059a0: 5f5f 2873 656c 662c 202a 6172 6773 2c20  __(self, *args, 
-000059b0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-000059c0: 2023 2074 6869 7320 7374 7562 206d 616b   # this stub mak
-000059d0: 6573 2073 7572 6520 7079 7479 7065 2061  es sure pytype a
-000059e0: 6363 6570 7473 2063 6f6e 7374 7275 6374  ccepts construct
-000059f0: 6f72 2061 7267 756d 656e 7473 2e0a 2020  or arguments..  
-00005a00: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00005a10: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
-00005a20: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00005a30: 2920 2d3e 2041 6e79 3a0a 2020 2020 2020  ) -> Any:.      
-00005a40: 2320 7468 6973 2073 7475 6220 616c 6c6f  # this stub allo
-00005a50: 7773 2070 7974 7970 6520 746f 2061 6363  ws pytype to acc
-00005a60: 6570 7420 4d6f 6475 6c65 7320 6173 2043  ept Modules as C
-00005a70: 616c 6c61 626c 6573 2e0a 2020 2020 2020  allables..      
-00005a80: 7061 7373 0a0a 2020 4063 6c61 7373 6d65  pass..  @classme
-00005a90: 7468 6f64 0a20 2064 6566 205f 5f69 6e69  thod.  def __ini
-00005aa0: 745f 7375 6263 6c61 7373 5f5f 2863 6c73  t_subclass__(cls
-00005ab0: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
-00005ac0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-00005ad0: 2241 7574 6f6d 6174 6963 616c 6c79 2069  "Automatically i
-00005ae0: 6e69 7469 616c 697a 6573 2061 6c6c 2073  nitializes all s
-00005af0: 7562 636c 6173 7365 7320 6173 2063 7573  ubclasses as cus
-00005b00: 746f 6d20 6461 7461 636c 6173 7365 732e  tom dataclasses.
-00005b10: 2222 220a 2020 2020 7375 7065 7228 292e  """.    super().
-00005b20: 5f5f 696e 6974 5f73 7562 636c 6173 735f  __init_subclass_
-00005b30: 5f28 2a2a 6b77 6172 6773 290a 2020 2020  _(**kwargs).    
-00005b40: 2320 416c 6c20 466c 6178 204d 6f64 756c  # All Flax Modul
-00005b50: 6573 2061 7265 2064 6174 6163 6c61 7373  es are dataclass
-00005b60: 6573 2e20 2057 6520 666f 7263 6520 7468  es.  We force th
-00005b70: 6973 2063 6f6e 7665 6e74 696f 6e20 7369  is convention si
-00005b80: 6e63 650a 2020 2020 2320 6974 2065 6e63  nce.    # it enc
-00005b90: 6f75 7261 6765 7320 7468 6520 7374 6174  ourages the stat
-00005ba0: 656c 6573 7320 6265 6861 7669 6f72 206e  eless behavior n
-00005bb0: 6565 6465 6420 746f 2063 6c6f 6e65 206d  eeded to clone m
-00005bc0: 6f64 756c 6520 696e 7374 616e 6365 7320  odule instances 
-00005bd0: 666f 720a 2020 2020 2320 6675 6e63 7469  for.    # functi
-00005be0: 6f6e 616c 2074 7261 6e73 666f 726d 6174  onal transformat
-00005bf0: 696f 6e2e 2020 496e 7374 6561 6420 6f66  ion.  Instead of
-00005c00: 2075 7369 6e67 2061 2070 7974 686f 6e20   using a python 
-00005c10: 6d65 7461 636c 6173 732c 2077 650a 2020  metaclass, we.  
-00005c20: 2020 2320 6175 746f 6d61 7469 6361 6c6c    # automaticall
-00005c30: 7920 7472 616e 7366 6f72 6d20 4d6f 6475  y transform Modu
-00005c40: 6c65 7320 696e 746f 2064 6174 6163 6c61  les into datacla
-00005c50: 7373 6573 2061 7420 7375 6263 6c61 7373  sses at subclass
-00005c60: 2063 7265 6174 696f 6e0a 2020 2020 2320   creation.    # 
-00005c70: 7469 6d65 2c20 616e 6420 7765 2073 6574  time, and we set
-00005c80: 2074 6865 206c 6173 7420 6461 7461 636c   the last datacl
-00005c90: 6173 7320 6172 6775 6d65 6e74 7320 746f  ass arguments to
-00005ca0: 2060 7061 7265 6e74 6020 616e 6420 606e   `parent` and `n
-00005cb0: 616d 6560 2e0a 2020 2020 636c 732e 5f63  ame`..    cls._c
-00005cc0: 7573 746f 6d69 7a65 645f 6461 7461 636c  ustomized_datacl
-00005cd0: 6173 735f 7472 616e 7366 6f72 6d28 290a  ass_transform().
-00005ce0: 2020 2020 2320 5765 2077 7261 7020 7573      # We wrap us
-00005cf0: 6572 2d64 6566 696e 6564 206d 6574 686f  er-defined metho
-00005d00: 6473 2069 6e63 6c75 6469 6e67 2073 6574  ds including set
-00005d10: 7570 2061 6e64 205f 5f63 616c 6c5f 5f20  up and __call__ 
-00005d20: 746f 2065 6e66 6f72 6365 0a20 2020 2023  to enforce.    #
-00005d30: 2061 206e 756d 6265 7220 6f66 2064 6966   a number of dif
-00005d40: 6665 7265 6e74 2063 6865 636b 7320 616e  ferent checks an
-00005d50: 6420 746f 2070 726f 7669 6465 2063 6c65  d to provide cle
-00005d60: 6172 2065 7272 6f72 206d 6573 7361 6765  ar error message
-00005d70: 732e 0a20 2020 2063 6c73 2e5f 7665 7269  s..    cls._veri
-00005d80: 6679 5f73 696e 676c 655f 6f72 5f6e 6f5f  fy_single_or_no_
-00005d90: 636f 6d70 6163 7428 290a 2020 2020 636c  compact().    cl
-00005da0: 732e 5f77 7261 705f 6d6f 6475 6c65 5f61  s._wrap_module_a
-00005db0: 7474 7269 6275 7465 7328 290a 2020 2020  ttributes().    
-00005dc0: 2320 5365 7420 656d 7074 7920 636c 6173  # Set empty clas
-00005dd0: 7320 6465 6661 756c 7473 2e0a 2020 2020  s defaults..    
-00005de0: 636c 732e 5f73 7461 7465 203d 205f 756e  cls._state = _un
-00005df0: 696e 6974 6961 6c69 7a65 645f 6d6f 6475  initialized_modu
-00005e00: 6c65 5f69 6e74 6572 6e61 6c5f 7374 6174  le_internal_stat
-00005e10: 6520 2320 7479 7065 3a20 6967 6e6f 7265  e # type: ignore
-00005e20: 5b61 7474 722d 6465 6669 6e65 645d 0a20  [attr-defined]. 
-00005e30: 2020 2063 6c73 2e73 636f 7065 3a20 4f70     cls.scope: Op
-00005e40: 7469 6f6e 616c 5b53 636f 7065 5d20 3d20  tional[Scope] = 
-00005e50: 4e6f 6e65 2023 2074 7970 653a 2069 676e  None # type: ign
-00005e60: 6f72 650a 2020 2020 2320 4861 6e64 6c65  ore.    # Handle
-00005e70: 7320 7765 616b 2072 6566 6572 656e 6369  s weak referenci
-00005e80: 6e67 206f 6620 7061 7265 6e74 204d 6f64  ng of parent Mod
-00005e90: 756c 6573 2074 6f20 7072 6576 656e 7420  ules to prevent 
-00005ea0: 7265 6665 7265 6e63 6520 6379 636c 6573  reference cycles
-00005eb0: 2e0a 2020 2020 636c 732e 5f70 6172 656e  ..    cls._paren
-00005ec0: 745f 7265 6620 3d20 4e6f 6e65 2023 2074  t_ref = None # t
-00005ed0: 7970 653a 2069 676e 6f72 655b 6174 7472  ype: ignore[attr
-00005ee0: 2d64 6566 696e 6564 5d0a 2020 2020 636c  -defined].    cl
-00005ef0: 732e 7061 7265 6e74 203d 2050 6172 656e  s.parent = Paren
-00005f00: 7444 6573 6372 6970 746f 7228 2920 2320  tDescriptor() # 
-00005f10: 7479 7065 3a20 6967 6e6f 7265 5b61 7373  type: ignore[ass
-00005f20: 6967 6e6d 656e 745d 0a0a 2020 4063 6c61  ignment]..  @cla
-00005f30: 7373 6d65 7468 6f64 0a20 2064 6566 205f  ssmethod.  def _
-00005f40: 6375 7374 6f6d 697a 6564 5f64 6174 6163  customized_datac
-00005f50: 6c61 7373 5f74 7261 6e73 666f 726d 2863  lass_transform(c
-00005f60: 6c73 293a 0a20 2020 2022 2222 5472 616e  ls):.    """Tran
-00005f70: 7366 6f72 6d73 2060 636c 7360 2069 6e74  sforms `cls` int
-00005f80: 6f20 6120 6461 7461 636c 6173 732c 2077  o a dataclass, w
-00005f90: 6974 6820 6375 7374 6f6d 2061 6464 6974  ith custom addit
-00005fa0: 696f 6e61 6c20 6265 6861 7669 6f72 2e0a  ional behavior..
-00005fb0: 0a20 2020 2031 2e20 496e 6a65 6374 2060  .    1. Inject `
-00005fc0: 7061 7265 6e74 6020 616e 6420 606e 616d  parent` and `nam
-00005fd0: 6560 2066 6965 6c64 732e 2020 2849 6620  e` fields.  (If 
-00005fe0: 7468 6579 2061 7265 2061 6c72 6561 6479  they are already
-00005ff0: 2070 7265 7365 6e74 2c0a 2020 2020 2020   present,.      
-00006000: 2074 6865 6e20 6368 6563 6b20 7468 6174   then check that
-00006010: 2074 6865 7920 6861 7665 2074 6865 2065   they have the e
-00006020: 7870 6563 7465 6420 7479 7065 732e 290a  xpected types.).
-00006030: 2020 2020 322e 2053 6574 2063 6f6d 7061      2. Set compa
-00006040: 7265 2c20 6861 7368 2c20 616e 6420 7265  re, hash, and re
-00006050: 7072 2074 6f20 4661 6c73 6520 666f 7220  pr to False for 
-00006060: 6e6f 6e2d 696e 6974 2066 6965 6c64 732e  non-init fields.
-00006070: 0a20 2020 2033 2e20 4765 6e65 7261 7465  .    3. Generate
-00006080: 2061 2068 6173 6820 6675 6e63 7469 6f6e   a hash function
-00006090: 2028 6966 206e 6f74 2070 726f 7669 6465   (if not provide
-000060a0: 6420 6279 2063 6c73 292e 0a20 2020 2022  d by cls)..    "
-000060b0: 2222 0a20 2020 2023 2043 6865 636b 2072  "".    # Check r
-000060c0: 6573 6572 7665 6420 6174 7472 6962 7574  eserved attribut
-000060d0: 6573 2068 6176 6520 6578 7065 6374 6564  es have expected
-000060e0: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
-000060f0: 732e 0a20 2020 2061 6e6e 6f74 6174 696f  s..    annotatio
-00006100: 6e73 203d 2064 6963 7428 636c 732e 5f5f  ns = dict(cls.__
-00006110: 6469 6374 5f5f 2e67 6574 2827 5f5f 616e  dict__.get('__an
-00006120: 6e6f 7461 7469 6f6e 735f 5f27 2c20 7b7d  notations__', {}
-00006130: 2929 0a20 2020 2069 6620 616e 6e6f 7461  )).    if annota
-00006140: 7469 6f6e 732e 6765 7428 2770 6172 656e  tions.get('paren
-00006150: 7427 2c20 5f50 6172 656e 7454 7970 6529  t', _ParentType)
-00006160: 2021 3d20 5f50 6172 656e 7454 7970 653a   != _ParentType:
-00006170: 0a20 2020 2020 2072 6169 7365 2065 7272  .      raise err
-00006180: 6f72 732e 5265 7365 7276 6564 4d6f 6475  ors.ReservedModu
-00006190: 6c65 4174 7472 6962 7574 6545 7272 6f72  leAttributeError
-000061a0: 2861 6e6e 6f74 6174 696f 6e73 290a 2020  (annotations).  
-000061b0: 2020 6966 2061 6e6e 6f74 6174 696f 6e73    if annotations
-000061c0: 2e67 6574 2827 6e61 6d65 272c 2073 7472  .get('name', str
-000061d0: 2920 6e6f 7420 696e 2028 2773 7472 272c  ) not in ('str',
-000061e0: 2073 7472 2c20 4f70 7469 6f6e 616c 5b73   str, Optional[s
-000061f0: 7472 5d29 3a0a 2020 2020 2020 7261 6973  tr]):.      rais
-00006200: 6520 6572 726f 7273 2e52 6573 6572 7665  e errors.Reserve
-00006210: 644d 6f64 756c 6541 7474 7269 6275 7465  dModuleAttribute
-00006220: 4572 726f 7228 616e 6e6f 7461 7469 6f6e  Error(annotation
-00006230: 7329 0a0a 2020 2020 2320 616e 7920 6e6f  s)..    # any no
-00006240: 6e2d 696e 6974 2066 6965 6c64 2077 696c  n-init field wil
-00006250: 6c20 6f6e 6c79 2062 6520 7365 7420 696e  l only be set in
-00006260: 2073 6574 7570 0a20 2020 2023 2044 7572   setup.    # Dur
-00006270: 696e 6720 5f5f 6861 7368 5f5f 2061 6e64  ing __hash__ and
-00006280: 205f 5f65 715f 5f20 7468 6520 6669 656c   __eq__ the fiel
-00006290: 6420 6973 206e 6f74 2073 6574 2079 6574  d is not set yet
-000062a0: 0a20 2020 2023 2073 6f20 6974 2073 686f  .    # so it sho
-000062b0: 756c 6420 6e6f 7420 6265 2075 7365 6420  uld not be used 
-000062c0: 696e 2063 6f6d 7061 7265 2c20 6861 7368  in compare, hash
-000062d0: 206f 7220 7265 7072 2e0a 2020 2020 666f   or repr..    fo
-000062e0: 7220 6669 656c 6420 696e 2061 6e6e 6f74  r field in annot
-000062f0: 6174 696f 6e73 3a0a 2020 2020 2020 6669  ations:.      fi
-00006300: 656c 645f 6d65 7461 203d 2067 6574 6174  eld_meta = getat
-00006310: 7472 2863 6c73 2c20 6669 656c 642c 204e  tr(cls, field, N
-00006320: 6f6e 6529 0a20 2020 2020 2069 6620 6973  one).      if is
-00006330: 696e 7374 616e 6365 2866 6965 6c64 5f6d  instance(field_m
-00006340: 6574 612c 2064 6174 6163 6c61 7373 6573  eta, dataclasses
-00006350: 2e46 6965 6c64 2920 616e 6420 6e6f 7420  .Field) and not 
-00006360: 6669 656c 645f 6d65 7461 2e69 6e69 743a  field_meta.init:
-00006370: 0a20 2020 2020 2020 2066 6965 6c64 5f6d  .        field_m
-00006380: 6574 612e 636f 6d70 6172 6520 3d20 4661  eta.compare = Fa
-00006390: 6c73 650a 2020 2020 2020 2020 6669 656c  lse.        fiel
-000063a0: 645f 6d65 7461 2e68 6173 6820 3d20 4661  d_meta.hash = Fa
-000063b0: 6c73 650a 2020 2020 2020 2020 6669 656c  lse.        fiel
-000063c0: 645f 6d65 7461 2e72 6570 7220 3d20 4661  d_meta.repr = Fa
-000063d0: 6c73 650a 0a20 2020 2065 7874 7261 5f66  lse..    extra_f
-000063e0: 6965 6c64 7320 3d20 5b28 2770 6172 656e  ields = [('paren
-000063f0: 7427 2c20 5f50 6172 656e 7454 7970 652c  t', _ParentType,
-00006400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006410: 2020 2020 2020 6b77 5f6f 6e6c 795f 6461        kw_only_da
-00006420: 7461 636c 6173 7365 732e 6669 656c 6428  taclasses.field(
-00006430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006440: 2020 2020 2020 2020 2020 7265 7072 3d46            repr=F
-00006450: 616c 7365 2c20 6465 6661 756c 743d 5f75  alse, default=_u
-00006460: 6e73 7065 6369 6669 6564 5f70 6172 656e  nspecified_paren
-00006470: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00006480: 2020 2020 2020 2020 2020 2020 6b77 5f6f              kw_o
-00006490: 6e6c 793d 5472 7565 2929 2c0a 2020 2020  nly=True)),.    
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 2827 6e61 6d65 272c 204f 7074 696f 6e61  ('name', Optiona
-000064c0: 6c5b 7374 725d 2c0a 2020 2020 2020 2020  l[str],.        
-000064d0: 2020 2020 2020 2020 2020 2020 206b 775f               kw_
-000064e0: 6f6e 6c79 5f64 6174 6163 6c61 7373 6573  only_dataclasses
-000064f0: 2e66 6965 6c64 2864 6566 6175 6c74 3d4e  .field(default=N
-00006500: 6f6e 652c 206b 775f 6f6e 6c79 3d54 7275  one, kw_only=Tru
-00006510: 6529 295d 0a0a 2020 2020 2320 4e6f 7720  e))]..    # Now 
-00006520: 6170 706c 7920 6461 7461 636c 6173 7320  apply dataclass 
-00006530: 7472 616e 7366 6f72 6d20 2877 6869 6368  transform (which
-00006540: 206f 7065 7261 7465 7320 696e 2d70 6c61   operates in-pla
-00006550: 6365 292e 0a20 2020 2023 2044 6f20 6765  ce)..    # Do ge
-00006560: 6e65 7261 7465 2061 2068 6173 6820 6675  nerate a hash fu
-00006570: 6e63 7469 6f6e 206f 6e6c 7920 6966 206e  nction only if n
-00006580: 6f74 2070 726f 7669 6465 6420 6279 2074  ot provided by t
-00006590: 6865 2063 6c61 7373 2e0a 2020 2020 6b77  he class..    kw
-000065a0: 5f6f 6e6c 795f 6461 7461 636c 6173 7365  _only_dataclasse
-000065b0: 732e 6461 7461 636c 6173 7328 0a20 2020  s.dataclass(.   
-000065c0: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
-000065d0: 2020 756e 7361 6665 5f68 6173 683d 275f    unsafe_hash='_
-000065e0: 5f68 6173 685f 5f27 206e 6f74 2069 6e20  _hash__' not in 
-000065f0: 636c 732e 5f5f 6469 6374 5f5f 2c0a 2020  cls.__dict__,.  
-00006600: 2020 2020 2020 7265 7072 3d46 616c 7365        repr=False
-00006610: 2c0a 2020 2020 2020 2020 6578 7472 615f  ,.        extra_
-00006620: 6669 656c 6473 3d65 7874 7261 5f66 6965  fields=extra_fie
-00006630: 6c64 7329 2020 2320 7079 7479 7065 3a20  lds)  # pytype: 
-00006640: 6469 7361 626c 653d 7772 6f6e 672d 6b65  disable=wrong-ke
-00006650: 7977 6f72 642d 6172 6773 0a20 2020 2063  yword-args.    c
-00006660: 6c73 2e5f 5f68 6173 685f 5f20 3d20 5f77  ls.__hash__ = _w
-00006670: 7261 705f 6861 7368 2863 6c73 2e5f 5f68  rap_hash(cls.__h
-00006680: 6173 685f 5f29 0a0a 2020 4063 6c61 7373  ash__)..  @class
-00006690: 6d65 7468 6f64 0a20 2064 6566 205f 7665  method.  def _ve
-000066a0: 7269 6679 5f73 696e 676c 655f 6f72 5f6e  rify_single_or_n
-000066b0: 6f5f 636f 6d70 6163 7428 636c 7329 3a0a  o_compact(cls):.
-000066c0: 2020 2020 2222 2253 7461 7469 6361 6c6c      """Staticall
-000066d0: 7920 7665 7269 6669 6573 2074 6861 7420  y verifies that 
-000066e0: 6174 206d 6f73 7420 6120 7369 6e67 6c65  at most a single
-000066f0: 206d 6574 686f 6420 6973 206c 6162 656c   method is label
-00006700: 6c65 6420 636f 6d70 6163 742e 2222 220a  led compact.""".
-00006710: 2020 2020 6d65 7468 6f64 7320 3d20 5b6d      methods = [m
-00006720: 5b30 5d20 666f 7220 6d20 696e 2069 6e73  [0] for m in ins
-00006730: 7065 6374 2e67 6574 6d65 6d62 6572 7328  pect.getmembers(
-00006740: 636c 732c 2070 7265 6469 6361 7465 3d63  cls, predicate=c
-00006750: 616c 6c61 626c 6529 5d0a 2020 2020 6e5f  allable)].    n_
-00006760: 636f 6d70 6163 745f 666e 7320 3d20 6c65  compact_fns = le
-00006770: 6e28 5b6d 6574 686f 645f 6e61 6d65 2066  n([method_name f
-00006780: 6f72 206d 6574 686f 645f 6e61 6d65 2069  or method_name i
-00006790: 6e20 6d65 7468 6f64 730a 2020 2020 2020  n methods.      
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2069 6620 6861 7361 7474 7228 6765     if hasattr(ge
-000067c0: 7461 7474 7228 636c 732c 206d 6574 686f  tattr(cls, metho
-000067d0: 645f 6e61 6d65 292c 2027 636f 6d70 6163  d_name), 'compac
-000067e0: 7427 295d 290a 2020 2020 6966 206e 5f63  t')]).    if n_c
-000067f0: 6f6d 7061 6374 5f66 6e73 203e 2031 3a0a  ompact_fns > 1:.
-00006800: 2020 2020 2020 7261 6973 6520 6572 726f        raise erro
-00006810: 7273 2e4d 756c 7469 706c 654d 6574 686f  rs.MultipleMetho
-00006820: 6473 436f 6d70 6163 7445 7272 6f72 2829  dsCompactError()
-00006830: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
-00006840: 0a20 2064 6566 205f 7772 6170 5f6d 6f64  .  def _wrap_mod
-00006850: 756c 655f 6174 7472 6962 7574 6573 2863  ule_attributes(c
-00006860: 6c73 293a 0a20 2020 2022 2222 5772 6170  ls):.    """Wrap
-00006870: 7320 7573 6572 2d64 6566 696e 6564 206e  s user-defined n
-00006880: 6f6e 2d69 6e68 6572 6974 6564 206d 6574  on-inherited met
-00006890: 686f 6473 2061 6e64 2064 6573 6372 6970  hods and descrip
-000068a0: 746f 7273 2077 6974 6820 7374 6174 650a  tors with state.
-000068b0: 2020 2020 6d61 6e61 6765 6d65 6e74 2066      management f
-000068c0: 756e 6374 696f 6e73 2e0a 2020 2020 2222  unctions..    ""
-000068d0: 220a 2020 2020 2320 7772 6170 206d 6574  ".    # wrap met
-000068e0: 686f 6473 0a20 2020 206d 6574 686f 645f  hods.    method_
-000068f0: 6578 636c 7573 696f 6e73 203d 2028 5b66  exclusions = ([f
-00006900: 2e6e 616d 6520 666f 7220 6620 696e 2064  .name for f in d
-00006910: 6174 6163 6c61 7373 6573 2e66 6965 6c64  ataclasses.field
-00006920: 7328 636c 7329 5d20 2b0a 2020 2020 2020  s(cls)] +.      
-00006930: 2020 2020 2020 2020 2020 2020 5b27 5f5f              ['__
-00006940: 6571 5f5f 272c 2027 5f5f 7265 7072 5f5f  eq__', '__repr__
-00006950: 272c 2027 5f5f 696e 6974 5f5f 272c 2027  ', '__init__', '
-00006960: 5f5f 6861 7368 5f5f 272c 0a20 2020 2020  __hash__',.     
-00006970: 2020 2020 2020 2020 2020 2020 2020 275f                '_
-00006980: 5f70 6f73 745f 696e 6974 5f5f 275d 290a  _post_init__']).
-00006990: 2020 2020 666f 7220 6b65 7920 696e 205f      for key in _
-000069a0: 6765 745f 6c6f 6361 6c5f 6d65 7468 6f64  get_local_method
-000069b0: 5f6e 616d 6573 2863 6c73 2c20 6578 636c  _names(cls, excl
-000069c0: 7564 653d 6d65 7468 6f64 5f65 7863 6c75  ude=method_exclu
-000069d0: 7369 6f6e 7329 3a0a 2020 2020 2020 6d65  sions):.      me
-000069e0: 7468 6f64 203d 2067 6574 6174 7472 2863  thod = getattr(c
-000069f0: 6c73 2c20 6b65 7929 0a20 2020 2020 2069  ls, key).      i
-00006a00: 6620 6861 7361 7474 7228 6d65 7468 6f64  f hasattr(method
-00006a10: 2c20 276e 6f77 7261 7027 293a 0a20 2020  , 'nowrap'):.   
-00006a20: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00006a30: 2020 2020 7365 7461 7474 7228 636c 732c      setattr(cls,
-00006a40: 206b 6579 2c20 7772 6170 5f6d 6574 686f   key, wrap_metho
-00006a50: 645f 6f6e 6365 286d 6574 686f 6429 290a  d_once(method)).
-00006a60: 0a20 2020 2023 2077 7261 7020 6465 7363  .    # wrap desc
-00006a70: 7269 7074 6f72 730a 2020 2020 6465 7363  riptors.    desc
-00006a80: 7269 7074 6f72 5f65 7863 6c75 7369 6f6e  riptor_exclusion
-00006a90: 7320 3d20 285b 662e 6e61 6d65 2066 6f72  s = ([f.name for
-00006aa0: 2066 2069 6e20 6461 7461 636c 6173 7365   f in dataclasse
-00006ab0: 732e 6669 656c 6473 2863 6c73 295d 202b  s.fields(cls)] +
-00006ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006ad0: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00006ae0: 7061 7265 6e74 272c 2027 5f5f 6469 6374  parent', '__dict
-00006af0: 5f5f 275d 290a 2020 2020 666f 7220 6b65  __']).    for ke
-00006b00: 7920 696e 205f 6765 745f 6c6f 6361 6c5f  y in _get_local_
-00006b10: 6465 7363 7269 7074 6f72 5f6e 616d 6573  descriptor_names
-00006b20: 2863 6c73 2c20 6465 7363 7269 7074 6f72  (cls, descriptor
-00006b30: 5f65 7863 6c75 7369 6f6e 7329 3a0a 2020  _exclusions):.  
-00006b40: 2020 2020 2320 646f 6e27 7420 7573 6520      # don't use 
-00006b50: 6765 7461 7474 7220 6865 7265 2c20 7369  getattr here, si
-00006b60: 6e63 6520 6974 2077 696c 6c20 6361 6c6c  nce it will call
-00006b70: 2074 6865 2064 6573 6372 6970 746f 720a   the descriptor.
-00006b80: 2020 2020 2020 6465 7363 7269 7074 6f72        descriptor
-00006b90: 203d 2063 6c73 2e5f 5f64 6963 745f 5f5b   = cls.__dict__[
-00006ba0: 6b65 795d 0a20 2020 2020 2069 6620 6861  key].      if ha
-00006bb0: 7361 7474 7228 6465 7363 7269 7074 6f72  sattr(descriptor
-00006bc0: 2c20 276e 6f77 7261 7027 293a 0a20 2020  , 'nowrap'):.   
-00006bd0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00006be0: 2020 2020 7365 7461 7474 7228 636c 732c      setattr(cls,
-00006bf0: 206b 6579 2c20 7772 6170 5f64 6573 6372   key, wrap_descr
-00006c00: 6970 746f 725f 6f6e 6365 2864 6573 6372  iptor_once(descr
-00006c10: 6970 746f 7229 290a 2020 2020 7265 7475  iptor)).    retu
-00006c20: 726e 2063 6c73 0a0a 2020 6465 6620 5f63  rn cls..  def _c
-00006c30: 616c 6c5f 7772 6170 7065 645f 6d65 7468  all_wrapped_meth
-00006c40: 6f64 2873 656c 662c 2066 756e 2c20 6172  od(self, fun, ar
-00006c50: 6773 2c20 6b77 6172 6773 293a 0a20 2020  gs, kwargs):.   
-00006c60: 2022 2222 2243 616c 6c73 2061 2077 7261   """"Calls a wra
-00006c70: 7070 6564 206d 6574 686f 642e 0a0a 2020  pped method...  
-00006c80: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00006c90: 6973 2072 6573 706f 6e73 6962 6c65 2066  is responsible f
-00006ca0: 6f72 2073 6574 7469 6e67 2075 7020 7468  or setting up th
-00006cb0: 6520 7468 7265 6164 206c 6f63 616c 2073  e thread local s
-00006cc0: 7461 7465 0a20 2020 2063 6f72 7265 6374  tate.    correct
-00006cd0: 6c79 2062 6566 6f72 6520 6361 6c6c 696e  ly before callin
-00006ce0: 6720 7468 6520 6d65 7468 6f64 2061 6e64  g the method and
-00006cf0: 2063 6c65 616e 696e 6720 7570 2061 6674   cleaning up aft
-00006d00: 6572 7761 7264 732e 0a20 2020 2054 6869  erwards..    Thi
-00006d10: 7320 696e 636c 7564 6573 2073 746f 7269  s includes stori
-00006d20: 6e67 2069 6e74 6572 6d65 6469 6174 6573  ng intermediates
-00006d30: 2c20 7365 7475 7020 6f66 2074 6865 2063  , setup of the c
-00006d40: 6f6d 7061 6374 2073 636f 7065 2c0a 2020  ompact scope,.  
-00006d50: 2020 616e 6420 6d61 6b69 6e67 2073 7572    and making sur
-00006d60: 6520 7365 7475 7020 6973 2063 616c 6c65  e setup is calle
-00006d70: 6420 6265 666f 7265 2061 6e79 206f 7468  d before any oth
-00006d80: 6572 206d 6574 686f 642e 0a0a 2020 2020  er method...    
-00006d90: 4172 6773 3a0a 2020 2020 2020 6675 6e3a  Args:.      fun:
-00006da0: 2054 6865 2077 7261 7070 6564 206d 6574   The wrapped met
-00006db0: 686f 642e 0a20 2020 2020 2061 7267 733a  hod..      args:
-00006dc0: 204e 616d 6564 2061 7267 756d 656e 7473   Named arguments
-00006dd0: 2070 6173 7365 6420 746f 2060 6066 756e   passed to ``fun
-00006de0: 6060 2e0a 2020 2020 2020 6b77 6172 6773  ``..      kwargs
-00006df0: 3a20 4b65 7977 6f72 6420 6172 6775 6d65  : Keyword argume
-00006e00: 6e74 7320 7061 7373 6564 2074 6f20 6060  nts passed to ``
-00006e10: 6675 6e60 602e 0a0a 2020 2020 5265 7475  fun``...    Retu
-00006e20: 726e 733a 0a20 2020 2020 2054 6865 2072  rns:.      The r
-00006e30: 6573 756c 7473 206f 6620 6361 6c6c 696e  esults of callin
-00006e40: 6720 6060 6675 6e60 602e 0a20 2020 2022  g ``fun``..    "
-00006e50: 2222 0a20 2020 2069 735f 636f 6d70 6163  "".    is_compac
-00006e60: 745f 6d65 7468 6f64 203d 2068 6173 6174  t_method = hasat
-00006e70: 7472 2866 756e 2c20 2763 6f6d 7061 6374  tr(fun, 'compact
-00006e80: 2729 0a20 2020 2066 756e 5f6e 616d 6520  ').    fun_name 
-00006e90: 3d20 6765 7461 7474 7228 6675 6e2c 2027  = getattr(fun, '
-00006ea0: 5f5f 6e61 6d65 5f5f 272c 2027 756e 6e61  __name__', 'unna
-00006eb0: 6d65 645f 6675 6e63 7469 6f6e 2729 0a20  med_function'). 
-00006ec0: 2020 2069 735f 7365 7475 705f 6d65 7468     is_setup_meth
-00006ed0: 6f64 203d 2066 756e 5f6e 616d 6520 3d3d  od = fun_name ==
-00006ee0: 2027 7365 7475 7027 0a20 2020 2061 6464   'setup'.    add
-00006ef0: 5f63 616c 6c5f 696e 666f 203d 206e 6f74  _call_info = not
-00006f00: 2069 735f 7365 7475 705f 6d65 7468 6f64   is_setup_method
-00006f10: 2061 6e64 206c 656e 285f 636f 6e74 6578   and len(_contex
-00006f20: 742e 6361 6c6c 5f69 6e66 6f5f 7374 6163  t.call_info_stac
-00006f30: 6b29 203e 2030 0a20 2020 2023 2057 6520  k) > 0.    # We 
-00006f40: 6c61 7a69 6c79 2063 616c 6c20 7365 7475  lazily call setu
-00006f50: 7028 2920 6f6e 6c79 2077 6865 6e20 6e65  p() only when ne
-00006f60: 6564 6564 2e0a 2020 2020 6966 2069 735f  eded..    if is_
-00006f70: 7365 7475 705f 6d65 7468 6f64 3a0a 2020  setup_method:.  
-00006f80: 2020 2020 6966 2073 656c 662e 7363 6f70      if self.scop
-00006f90: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00006fa0: 2020 2072 6169 7365 2065 7272 6f72 732e     raise errors.
-00006fb0: 4361 6c6c 5365 7475 7055 6e62 6f75 6e64  CallSetupUnbound
-00006fc0: 4d6f 6475 6c65 4572 726f 7228 290a 2020  ModuleError().  
-00006fd0: 2020 2020 6973 5f72 6563 7572 7265 6e74      is_recurrent
-00006fe0: 203d 2073 656c 662e 5f73 7461 7465 2e69   = self._state.i
-00006ff0: 6e5f 7365 7475 700a 2020 2020 2020 7365  n_setup.      se
-00007000: 6c66 2e5f 7374 6174 652e 696e 5f73 6574  lf._state.in_set
-00007010: 7570 203d 2054 7275 650a 2020 2020 656c  up = True.    el
-00007020: 7365 3a0a 2020 2020 2020 7365 6c66 2e5f  se:.      self._
-00007030: 7472 795f 7365 7475 7028 290a 0a20 2020  try_setup()..   
-00007040: 2069 6620 6973 5f63 6f6d 7061 6374 5f6d   if is_compact_m
-00007050: 6574 686f 643a 0a20 2020 2020 2069 6620  ethod:.      if 
-00007060: 7365 6c66 2e73 636f 7065 2069 7320 4e6f  self.scope is No
-00007070: 6e65 3a0a 2020 2020 2020 2020 7261 6973  ne:.        rais
-00007080: 6520 6572 726f 7273 2e43 616c 6c43 6f6d  e errors.CallCom
-00007090: 7061 6374 556e 626f 756e 644d 6f64 756c  pactUnboundModul
-000070a0: 6545 7272 6f72 2829 0a20 2020 2020 2069  eError().      i
-000070b0: 735f 7265 6375 7272 656e 7420 3d20 7365  s_recurrent = se
-000070c0: 6c66 2e5f 7374 6174 652e 696e 5f63 6f6d  lf._state.in_com
-000070d0: 7061 6374 5f6d 6574 686f 640a 2020 2020  pact_method.    
-000070e0: 2020 7365 6c66 2e5f 7374 6174 652e 696e    self._state.in
-000070f0: 5f63 6f6d 7061 6374 5f6d 6574 686f 6420  _compact_method 
-00007100: 3d20 5472 7565 0a20 2020 205f 636f 6e74  = True.    _cont
-00007110: 6578 742e 6d6f 6475 6c65 5f73 7461 636b  ext.module_stack
-00007120: 2e61 7070 656e 6428 7365 6c66 290a 2020  .append(self).  
-00007130: 2020 7472 793a 0a20 2020 2020 2023 2067    try:.      # g
-00007140: 6574 2063 616c 6c20 696e 666f 0a20 2020  et call info.   
-00007150: 2020 2069 6620 6164 645f 6361 6c6c 5f69     if add_call_i
-00007160: 6e66 6f3a 0a20 2020 2020 2020 2061 7373  nfo:.        ass
-00007170: 6572 7420 7365 6c66 2e73 636f 7065 2069  ert self.scope i
-00007180: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00007190: 2020 2063 616c 6c5f 696e 6465 7820 3d20     call_index = 
-000071a0: 5f63 6f6e 7465 7874 2e63 616c 6c5f 696e  _context.call_in
-000071b0: 666f 5f73 7461 636b 5b2d 315d 2e67 6574  fo_stack[-1].get
-000071c0: 5f63 616c 6c5f 696e 6465 7828 7365 6c66  _call_index(self
-000071d0: 290a 2020 2020 2020 2020 7363 6f70 655f  ).        scope_
-000071e0: 7061 7468 203d 206a 6178 2e74 7265 655f  path = jax.tree_
-000071f0: 7574 696c 2e74 7265 655f 6d61 7028 5f66  util.tree_map(_f
-00007200: 6978 5f70 6174 685f 7061 7274 2c20 7365  ix_path_part, se
-00007210: 6c66 2e73 636f 7065 2e70 6174 6829 0a0a  lf.scope.path)..
-00007220: 2020 2020 2020 2320 6361 6c6c 206d 6574        # call met
-00007230: 686f 640a 2020 2020 2020 6966 205f 7573  hod.      if _us
-00007240: 655f 6e61 6d65 645f 6361 6c6c 3a0a 2020  e_named_call:.  
-00007250: 2020 2020 2020 7769 7468 206a 6178 2e6e        with jax.n
-00007260: 616d 6564 5f73 636f 7065 285f 6465 7269  amed_scope(_deri
-00007270: 7665 5f70 726f 6669 6c69 6e67 5f6e 616d  ve_profiling_nam
-00007280: 6528 7365 6c66 2c20 6675 6e29 293a 0a20  e(self, fun)):. 
-00007290: 2020 2020 2020 2020 2079 203d 2066 756e           y = fun
-000072a0: 2873 656c 662c 202a 6172 6773 2c20 2a2a  (self, *args, **
-000072b0: 6b77 6172 6773 290a 2020 2020 2020 656c  kwargs).      el
-000072c0: 7365 3a0a 2020 2020 2020 2020 7920 3d20  se:.        y = 
-000072d0: 6675 6e28 7365 6c66 2c20 2a61 7267 732c  fun(self, *args,
-000072e0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-000072f0: 2020 6966 205f 636f 6e74 6578 742e 6361    if _context.ca
-00007300: 7074 7572 655f 7374 6163 6b3a 0a20 2020  pture_stack:.   
-00007310: 2020 2020 2066 696c 7465 725f 666e 203d       filter_fn =
-00007320: 205f 636f 6e74 6578 742e 6361 7074 7572   _context.captur
-00007330: 655f 7374 6163 6b5b 2d31 5d0a 2020 2020  e_stack[-1].    
-00007340: 2020 2020 6966 2066 696c 7465 725f 666e      if filter_fn
-00007350: 2061 6e64 2066 696c 7465 725f 666e 2873   and filter_fn(s
-00007360: 656c 662c 2066 756e 5f6e 616d 6529 3a0a  elf, fun_name):.
-00007370: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00007380: 6f77 2827 696e 7465 726d 6564 6961 7465  ow('intermediate
-00007390: 7327 2c20 6675 6e5f 6e61 6d65 2c20 7929  s', fun_name, y)
-000073a0: 0a20 2020 2020 2069 6620 6164 645f 6361  .      if add_ca
-000073b0: 6c6c 5f69 6e66 6f3a 0a20 2020 2020 2020  ll_info:.       
-000073c0: 205f 6172 6773 2c20 5f6b 7761 7267 732c   _args, _kwargs,
-000073d0: 205f 7920 3d20 666c 6178 2e6c 696e 656e   _y = flax.linen
-000073e0: 2e73 756d 6d61 7279 2e5f 7265 7072 6573  .summary._repres
-000073f0: 656e 745f 7472 6565 2828 6172 6773 2c20  ent_tree((args, 
-00007400: 6b77 6172 6773 2c20 7929 290a 2020 2020  kwargs, y)).    
-00007410: 2020 2020 5f63 6f6e 7465 7874 2e63 616c      _context.cal
-00007420: 6c5f 696e 666f 5f73 7461 636b 5b2d 315d  l_info_stack[-1]
-00007430: 2e63 616c 6c73 2e61 7070 656e 6428 0a20  .calls.append(. 
-00007440: 2020 2020 2020 2020 205f 4361 6c6c 496e           _CallIn
-00007450: 666f 2863 616c 6c5f 696e 6465 782c 2073  fo(call_index, s
-00007460: 636f 7065 5f70 6174 682c 2074 7970 6528  cope_path, type(
-00007470: 7365 6c66 292c 2066 756e 2e5f 5f6e 616d  self), fun.__nam
-00007480: 655f 5f2c 205f 6172 6773 2c20 5f6b 7761  e__, _args, _kwa
-00007490: 7267 732c 205f 7929 290a 2020 2020 2020  rgs, _y)).      
-000074a0: 7265 7475 726e 2079 0a20 2020 2066 696e  return y.    fin
-000074b0: 616c 6c79 3a0a 2020 2020 2020 5f63 6f6e  ally:.      _con
-000074c0: 7465 7874 2e6d 6f64 756c 655f 7374 6163  text.module_stac
-000074d0: 6b2e 706f 7028 290a 2020 2020 2020 6966  k.pop().      if
-000074e0: 2069 735f 636f 6d70 6163 745f 6d65 7468   is_compact_meth
-000074f0: 6f64 3a0a 2020 2020 2020 2020 6f62 6a65  od:.        obje
-00007500: 6374 2e5f 5f73 6574 6174 7472 5f5f 2873  ct.__setattr__(s
-00007510: 656c 662c 2027 7363 6f70 6527 2c20 7365  elf, 'scope', se
-00007520: 6c66 2e73 636f 7065 2e72 6577 6f75 6e64  lf.scope.rewound
-00007530: 2829 290a 2020 2020 2020 2320 7365 7475  ()).      # setu
-00007540: 7020 6f72 2063 6f6d 7061 6374 2063 616c  p or compact cal
-00007550: 6c73 2063 616e 2062 6520 7265 6375 7272  ls can be recurr
-00007560: 656e 7420 666f 7220 6578 616d 706c 6520  ent for example 
-00007570: 6475 6520 746f 2073 7570 6572 2063 616c  due to super cal
-00007580: 6c73 0a20 2020 2020 2023 2072 6573 6574  ls.      # reset
-00007590: 7469 6e67 2074 6865 2073 7461 7465 2077  ting the state w
-000075a0: 6f75 6c64 2063 6175 7365 2069 7320 636f  ould cause is co
-000075b0: 6d70 6163 742f 7365 7475 7020 6d65 7468  mpact/setup meth
-000075c0: 6f64 0a20 2020 2020 2023 2074 6f20 6265  od.      # to be
-000075d0: 2073 6574 2074 6f20 4661 6c73 6520 7072   set to False pr
-000075e0: 656d 6174 7572 656c 792e 0a20 2020 2020  ematurely..     
-000075f0: 2069 6620 2869 735f 636f 6d70 6163 745f   if (is_compact_
-00007600: 6d65 7468 6f64 206f 7220 6973 5f73 6574  method or is_set
-00007610: 7570 5f6d 6574 686f 6429 2061 6e64 206e  up_method) and n
-00007620: 6f74 2069 735f 7265 6375 7272 656e 743a  ot is_recurrent:
-00007630: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-00007640: 7461 7465 2e72 6573 6574 2829 0a0a 2020  tate.reset()..  
-00007650: 6465 6620 5f5f 7365 7461 7474 725f 5f28  def __setattr__(
-00007660: 7365 6c66 2c20 6e61 6d65 3a20 7374 722c  self, name: str,
-00007670: 2076 616c 3a20 416e 7929 3a0a 2020 2020   val: Any):.    
-00007680: 2222 2253 6574 7320 616e 2061 7474 7269  """Sets an attri
-00007690: 6275 7465 206f 6e20 7468 6973 204d 6f64  bute on this Mod
-000076a0: 756c 652e 0a0a 2020 2020 5765 206f 7665  ule...    We ove
-000076b0: 726c 6f61 6420 7365 7461 7474 7220 736f  rload setattr so
-000076c0: 6c65 6c79 2074 6f20 7375 7070 6f72 7420  lely to support 
-000076d0: 7079 7468 6f6e 6963 206e 616d 696e 6720  pythonic naming 
-000076e0: 7669 6120 6173 7369 676e 6d65 6e74 206f  via assignment o
-000076f0: 660a 2020 2020 7375 626d 6f64 756c 6573  f.    submodules
-00007700: 2069 6e20 7468 6520 7370 6563 6961 6c20   in the special 
-00007710: 3a6d 6574 683a 6073 6574 7570 6020 6675  :meth:`setup` fu
-00007720: 6e63 7469 6f6e 3a3a 0a0a 2020 2020 2020  nction::..      
-00007730: 7365 6c66 2e73 7562 6d6f 6475 6c65 5f6e  self.submodule_n
-00007740: 616d 6520 3d20 4d79 4d6f 6475 6c65 282e  ame = MyModule(.
-00007750: 2e2e 290a 0a20 2020 2057 6520 616c 736f  ..)..    We also
-00007760: 2073 7570 706f 7274 206c 6973 7473 2061   support lists a
-00007770: 6e64 206f 7468 6572 2067 656e 6572 616c  nd other general
-00007780: 2070 7974 7265 6573 2c20 652e 672e 3a3a   pytrees, e.g.::
-00007790: 0a0a 2020 2020 2020 7365 6c66 2e73 7562  ..      self.sub
-000077a0: 6d6f 6475 6c65 7320 3d20 5b4d 794d 6f64  modules = [MyMod
-000077b0: 756c 6530 282e 2e29 2c20 4d79 4d6f 6475  ule0(..), MyModu
-000077c0: 6c65 3128 2e2e 292c 202e 2e2e 5d0a 0a20  le1(..), ...].. 
-000077d0: 2020 2041 7267 733a 0a20 2020 2020 206e     Args:.      n
-000077e0: 616d 653a 2041 7474 7269 6275 7465 2074  ame: Attribute t
-000077f0: 6f20 7365 742e 0a20 2020 2020 2076 616c  o set..      val
-00007800: 3a20 5661 6c75 6520 6f66 2074 6865 2061  : Value of the a
-00007810: 7474 7269 6275 7465 2e0a 2020 2020 2222  ttribute..    ""
-00007820: 220a 2020 2020 6669 656c 6473 203d 2073  ".    fields = s
-00007830: 656c 662e 5f5f 6461 7461 636c 6173 735f  elf.__dataclass_
-00007840: 6669 656c 6473 5f5f 2020 2320 7079 7479  fields__  # pyty
-00007850: 7065 3a20 6469 7361 626c 653d 6174 7472  pe: disable=attr
-00007860: 6962 7574 652d 6572 726f 720a 2020 2020  ibute-error.    
-00007870: 6973 5f64 6174 6163 6c61 7373 5f61 7474  is_dataclass_att
-00007880: 7220 3d20 6e61 6d65 2069 6e20 6669 656c  r = name in fiel
-00007890: 6473 2061 6e64 2066 6965 6c64 735b 6e61  ds and fields[na
-000078a0: 6d65 5d2e 696e 6974 0a0a 2020 2020 6966  me].init..    if
-000078b0: 206e 6f74 2073 656c 662e 5f73 7461 7465   not self._state
-000078c0: 2e69 6e5f 7365 7475 703a 0a20 2020 2020  .in_setup:.     
-000078d0: 2069 6620 6e6f 7420 7365 6c66 2e5f 7374   if not self._st
-000078e0: 6174 652e 6973 5f69 6e69 7469 616c 697a  ate.is_initializ
-000078f0: 6564 3a0a 2020 2020 2020 2020 2320 5365  ed:.        # Se
-00007900: 7474 696e 6720 6174 7472 6962 7574 6573  tting attributes
-00007910: 2062 6566 6f72 6520 656e 6420 6f66 204d   before end of M
-00007920: 6f64 756c 652e 5f5f 706f 7374 5f69 6e69  odule.__post_ini
-00007930: 745f 5f28 290a 2020 2020 2020 2020 6f62  t__().        ob
-00007940: 6a65 6374 2e5f 5f73 6574 6174 7472 5f5f  ject.__setattr__
-00007950: 2873 656c 662c 206e 616d 652c 2076 616c  (self, name, val
-00007960: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00007970: 0a20 2020 2020 2065 6c73 653a 0a20 2020  .      else:.   
-00007980: 2020 2020 2023 2057 6527 7265 2070 6173       # We're pas
-00007990: 7420 616c 6c20 696e 6974 6961 6c69 7a61  t all initializa
-000079a0: 7469 6f6e 2061 6e64 2073 6574 7570 206c  tion and setup l
-000079b0: 6f67 6963 3a0a 2020 2020 2020 2020 2320  ogic:.        # 
-000079c0: 5261 6973 6573 2061 2054 7970 6545 7272  Raises a TypeErr
-000079d0: 6f72 206a 7573 7420 6c69 6b65 2066 726f  or just like fro
-000079e0: 7a65 6e20 7079 7468 6f6e 2064 6174 6163  zen python datac
-000079f0: 6c61 7373 6573 2e0a 2020 2020 2020 2020  lasses..        
-00007a00: 7261 6973 6520 6572 726f 7273 2e53 6574  raise errors.Set
-00007a10: 4174 7472 6962 7574 6546 726f 7a65 6e4d  AttributeFrozenM
-00007a20: 6f64 756c 6545 7272 6f72 280a 2020 2020  oduleError(.    
-00007a30: 2020 2020 2020 2020 7365 6c66 2e5f 5f63          self.__c
-00007a40: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f2c  lass__.__name__,
-00007a50: 206e 616d 652c 2076 616c 290a 0a20 2020   name, val)..   
-00007a60: 2023 2057 6527 7265 2069 6e73 6964 6520   # We're inside 
-00007a70: 7468 6520 7365 7475 7028 2920 6d65 7468  the setup() meth
-00007a80: 6f64 3a0a 2020 2020 6966 2069 735f 6461  od:.    if is_da
-00007a90: 7461 636c 6173 735f 6174 7472 3a0a 2020  taclass_attr:.  
-00007aa0: 2020 2020 2320 5468 6573 6520 6e61 6d65      # These name
-00007ab0: 7320 6172 6520 7370 6563 6966 6965 6420  s are specified 
-00007ac0: 6173 2064 6174 6163 6c61 7373 2066 6965  as dataclass fie
-00007ad0: 6c64 732e 2054 6865 7920 7368 6f75 6c64  lds. They should
-00007ae0: 206e 6f74 2062 650a 2020 2020 2020 2320   not be.      # 
-00007af0: 696e 6974 6961 6c69 7a65 6420 7769 7468  initialized with
-00007b00: 696e 2074 6865 2073 6574 7570 2829 206d  in the setup() m
-00007b10: 6574 686f 642c 2062 7574 2063 616e 2062  ethod, but can b
-00007b20: 6520 6d6f 6469 6669 6564 2066 7265 656c  e modified freel
-00007b30: 790a 2020 2020 2020 2320 6265 666f 7265  y.      # before
-00007b40: 2069 742e 0a20 2020 2020 2072 6169 7365   it..      raise
-00007b50: 2065 7272 6f72 732e 5365 7441 7474 7269   errors.SetAttri
-00007b60: 6275 7465 496e 4d6f 6475 6c65 5365 7475  buteInModuleSetu
-00007b70: 7045 7272 6f72 2829 0a0a 2020 2020 2320  pError()..    # 
-00007b80: 5661 6c75 6573 2028 7468 6174 206d 6179  Values (that may
-00007b90: 2062 6520 7661 7269 6162 6c65 7320 6f72   be variables or
-00007ba0: 2073 7562 6d6f 6475 6c65 7329 2061 7265   submodules) are
-00007bb0: 2062 6569 6e67 2064 6566 696e 6564 2061   being defined a
-00007bc0: 6e64 0a20 2020 2023 2061 7474 6163 6865  nd.    # attache
-00007bd0: 6420 696e 2073 6574 7570 2829 2c20 7765  d in setup(), we
-00007be0: 2072 756e 2073 6f6d 6520 6578 7472 6120   run some extra 
-00007bf0: 6c6f 6769 6320 696e 2074 6861 7420 6361  logic in that ca
-00007c00: 7365 2e0a 2020 2020 7365 6c66 2e5f 7265  se..    self._re
-00007c10: 6769 7374 6572 5f73 7562 6d6f 6475 6c65  gister_submodule
-00007c20: 7328 6e61 6d65 2c20 7661 6c29 0a0a 2020  s(name, val)..  
-00007c30: 6465 6620 5f5f 6765 7461 7474 725f 5f28  def __getattr__(
-00007c40: 7365 6c66 2c20 6e61 6d65 3a20 7374 7229  self, name: str)
-00007c50: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-00007c60: 4361 6c6c 2073 6574 7570 2829 2062 6566  Call setup() bef
-00007c70: 6f72 6520 6765 7474 696e 6720 616e 7920  ore getting any 
-00007c80: 7365 7475 702d 6465 6669 6e65 6420 6174  setup-defined at
-00007c90: 7472 6962 7574 6573 2e22 2222 0a20 2020  tributes.""".   
-00007ca0: 2023 2057 6520 646f 6e27 7420 7761 6e74   # We don't want
-00007cb0: 2074 6f20 7265 7475 726e 2061 6e79 7468   to return anyth
-00007cc0: 696e 6720 666f 7220 7079 7468 6f6e 2063  ing for python c
-00007cd0: 6f70 7920 2f20 7069 636b 6c65 206d 6574  opy / pickle met
-00007ce0: 686f 6473 2e0a 2020 2020 6966 206e 616d  hods..    if nam
-00007cf0: 6520 696e 205f 554e 4445 4649 4e45 445f  e in _UNDEFINED_
-00007d00: 434f 5059 5f50 4943 4b4c 455f 4d45 5448  COPY_PICKLE_METH
-00007d10: 4f44 533a 0a20 2020 2020 2072 6169 7365  ODS:.      raise
-00007d20: 2041 7474 7269 6275 7465 4572 726f 7228   AttributeError(
-00007d30: 290a 2020 2020 7365 6c66 2e5f 7472 795f  ).    self._try_
-00007d40: 7365 7475 7028 290a 2020 2020 6966 206e  setup().    if n
-00007d50: 616d 6520 696e 2073 656c 662e 5f5f 6469  ame in self.__di
-00007d60: 6374 5f5f 3a0a 2020 2020 2020 7265 7475  ct__:.      retu
-00007d70: 726e 2073 656c 662e 5f5f 6469 6374 5f5f  rn self.__dict__
-00007d80: 5b6e 616d 655d 0a20 2020 2065 6c73 653a  [name].    else:
-00007d90: 0a20 2020 2020 206d 7367 203d 2066 2722  .      msg = f'"
-00007da0: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
-00007db0: 5f5f 6e61 6d65 5f5f 7d22 206f 626a 6563  __name__}" objec
-00007dc0: 7420 6861 7320 6e6f 2061 7474 7269 6275  t has no attribu
-00007dd0: 7465 2022 7b6e 616d 657d 222e 270a 2020  te "{name}".'.  
-00007de0: 2020 2020 6966 2073 656c 662e 7363 6f70      if self.scop
-00007df0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00007e00: 2020 206d 7367 202b 3d20 2866 2720 4966     msg += (f' If
-00007e10: 2022 7b6e 616d 657d 2220 6973 2064 6566   "{name}" is def
-00007e20: 696e 6564 2069 6e20 5c27 2e73 6574 7570  ined in \'.setup
-00007e30: 2829 5c27 2c20 7265 6d65 6d62 6572 2074  ()\', remember t
-00007e40: 6865 7365 2066 6965 6c64 7320 270a 2020  hese fields '.  
-00007e50: 2020 2020 2020 2020 2761 7265 206f 6e6c          'are onl
-00007e60: 7920 6163 6365 7373 6962 6c65 2066 726f  y accessible fro
-00007e70: 6d20 696e 7369 6465 205c 2769 6e69 745c  m inside \'init\
-00007e80: 2720 6f72 205c 2761 7070 6c79 5c27 2e27  ' or \'apply\'.'
-00007e90: 290a 2020 2020 2020 7261 6973 6520 4174  ).      raise At
-00007ea0: 7472 6962 7574 6545 7272 6f72 286d 7367  tributeError(msg
-00007eb0: 290a 0a20 2064 6566 205f 5f64 6972 5f5f  )..  def __dir__
-00007ec0: 2873 656c 6629 202d 3e20 4c69 7374 5b73  (self) -> List[s
-00007ed0: 7472 5d3a 0a20 2020 2022 2222 4361 6c6c  tr]:.    """Call
-00007ee0: 2073 6574 7570 2829 2062 6566 6f72 6520   setup() before 
-00007ef0: 6c69 7374 696e 6720 6174 7472 6962 7574  listing attribut
-00007f00: 6573 2e22 2222 0a20 2020 2073 656c 662e  es.""".    self.
-00007f10: 5f74 7279 5f73 6574 7570 2829 0a20 2020  _try_setup().   
-00007f20: 2072 6574 7572 6e20 6f62 6a65 6374 2e5f   return object._
-00007f30: 5f64 6972 5f5f 2873 656c 6629 2020 2320  _dir__(self)  # 
-00007f40: 7479 7065 3a20 6967 6e6f 7265 0a0a 2020  type: ignore..  
-00007f50: 6465 6620 5f5f 706f 7374 5f69 6e69 745f  def __post_init_
-00007f60: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
-00007f70: 0a20 2020 2023 2044 4f20 4e4f 5420 5245  .    # DO NOT RE
-00007f80: 4d4f 5645 202d 204d 6172 6b65 7220 666f  MOVE - Marker fo
-00007f90: 7220 696e 7465 726e 616c 206c 6f67 6769  r internal loggi
-00007fa0: 6e67 2e0a 2020 2020 2320 496e 2064 6174  ng..    # In dat
-00007fb0: 6163 6c61 7373 6573 2c20 5f5f 696e 6974  aclasses, __init
-00007fc0: 5f5f 2069 7320 6f76 6572 7269 6464 656e  __ is overridden
-00007fd0: 2074 6f20 7072 6f63 6573 7320 6461 7461   to process data
-00007fe0: 636c 6173 7320 6172 6775 6d65 6e74 732c  class arguments,
-00007ff0: 0a20 2020 2023 2061 6e64 205f 5f70 6f73  .    # and __pos
-00008000: 745f 696e 6974 5f5f 2069 7320 6361 6c6c  t_init__ is call
-00008010: 6564 2069 6d6d 6564 6961 7465 6c79 2061  ed immediately a
-00008020: 6674 6572 7761 7264 732e 2048 6572 652c  fterwards. Here,
-00008030: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
-00008040: 650a 2020 2020 2320 7479 7065 206f 6620  e.    # type of 
-00008050: 6070 6172 656e 7460 2070 6173 7365 6420  `parent` passed 
-00008060: 746f 2069 6e69 7469 616c 697a 6520 7468  to initialize th
-00008070: 6520 4d6f 6475 6c65 2c20 7765 2065 6974  e Module, we eit
-00008080: 6865 7220 6465 6665 720a 2020 2020 2320  her defer.    # 
-00008090: 696e 6974 6961 6c69 7a61 7469 6f6e 2c20  initialization, 
-000080a0: 6174 7461 6368 2074 6869 7320 4d6f 6475  attach this Modu
-000080b0: 6c65 2061 7320 6120 7375 626d 6f64 756c  le as a submodul
-000080c0: 6520 6f66 2061 2070 6172 656e 742c 206f  e of a parent, o
-000080d0: 7220 6269 6e64 0a20 2020 2023 2074 6869  r bind.    # thi
-000080e0: 7320 4d6f 6475 6c65 2061 7420 7468 6520  s Module at the 
-000080f0: 746f 702d 6c65 7665 6c20 746f 2076 6172  top-level to var
-00008100: 6961 626c 6573 2061 6e64 2072 6e67 732e  iables and rngs.
-00008110: 0a0a 2020 2020 6f62 6a65 6374 2e5f 5f73  ..    object.__s
-00008120: 6574 6174 7472 5f5f 2873 656c 662c 2027  etattr__(self, '
-00008130: 5f69 6427 2c20 7575 6964 2829 290a 2020  _id', uuid()).  
-00008140: 2020 6f62 6a65 6374 2e5f 5f73 6574 6174    object.__setat
-00008150: 7472 5f5f 2873 656c 662c 2027 5f73 7461  tr__(self, '_sta
-00008160: 7465 272c 205f 4d6f 6475 6c65 496e 7465  te', _ModuleInte
-00008170: 726e 616c 5374 6174 6528 2929 0a0a 2020  rnalState())..  
-00008180: 2020 2320 5479 7069 6361 6c6c 7920 7765    # Typically we
-00008190: 2073 6574 2074 6865 2070 6172 656e 7420   set the parent 
-000081a0: 6261 7365 6420 6f6e 2074 6865 2064 796e  based on the dyn
-000081b0: 616d 6963 206d 6f64 756c 6520 636f 6e74  amic module cont
-000081c0: 6578 742e 0a20 2020 2069 6620 7365 6c66  ext..    if self
-000081d0: 2e70 6172 656e 7420 6973 205f 756e 7370  .parent is _unsp
-000081e0: 6563 6966 6965 645f 7061 7265 6e74 3a20  ecified_parent: 
-000081f0: 2023 2070 7974 7970 653a 2064 6973 6162   # pytype: disab
-00008200: 6c65 3d61 7474 7269 6275 7465 2d65 7272  le=attribute-err
-00008210: 6f72 0a20 2020 2020 206f 626a 6563 742e  or.      object.
-00008220: 5f5f 7365 7461 7474 725f 5f28 7365 6c66  __setattr__(self
-00008230: 2c20 2770 6172 656e 7427 2c20 5f63 6f6e  , 'parent', _con
-00008240: 7465 7874 2e6d 6f64 756c 655f 7374 6163  text.module_stac
-00008250: 6b5b 2d31 5d29 0a0a 2020 2020 2320 496e  k[-1])..    # In
-00008260: 6974 6961 6c69 7a61 7469 6f6e 2069 7320  itialization is 
-00008270: 6465 6665 7272 6564 2066 6f72 2074 6f70  deferred for top
-00008280: 206c 6576 656c 204d 6f64 756c 6573 206f   level Modules o
-00008290: 7220 616e 7920 6f74 6865 7220 226f 7270  r any other "orp
-000082a0: 6861 6e22 0a20 2020 2023 204d 6f64 756c  han".    # Modul
-000082b0: 6573 2075 6e74 696c 2061 7474 6163 686d  es until attachm
-000082c0: 656e 7420 6279 205f 5f73 6574 6174 7472  ent by __setattr
-000082d0: 5f5f 2069 2e65 2e20 4d79 4d6f 6475 6c65  __ i.e. MyModule
-000082e0: 282e 2e2e 2c20 7061 7265 6e74 3d4e 6f6e  (..., parent=Non
-000082f0: 6529 0a20 2020 2069 6620 7365 6c66 2e70  e).    if self.p
-00008300: 6172 656e 7420 6973 204e 6f6e 653a 0a20  arent is None:. 
-00008310: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00008320: 2023 2052 6567 6973 7465 7220 7375 626d   # Register subm
-00008330: 6f64 756c 6520 6f6e 2070 6172 656e 7420  odule on parent 
-00008340: 4d6f 6475 6c65 2e0a 2020 2020 6966 2069  Module..    if i
-00008350: 7369 6e73 7461 6e63 6528 7365 6c66 2e70  sinstance(self.p
-00008360: 6172 656e 742c 204d 6f64 756c 6529 3a0a  arent, Module):.
-00008370: 2020 2020 2020 2320 5768 656e 2069 6e69        # When ini
-00008380: 7469 616c 697a 696e 6720 616e 2075 6e6e  tializing an unn
-00008390: 616d 6564 204d 6f64 756c 6520 696e 7369  amed Module insi
-000083a0: 6465 2073 6574 7570 2829 0a20 2020 2020  de setup().     
-000083b0: 2023 2069 6e69 7469 616c 697a 6174 696f   # initializatio
-000083c0: 6e20 6973 2064 6566 6572 7265 6420 756e  n is deferred un
-000083d0: 7469 6c20 6174 7461 6368 6d65 6e74 2062  til attachment b
-000083e0: 7920 5f5f 7365 7461 7474 725f 5f0a 2020  y __setattr__.  
-000083f0: 2020 2020 2320 692e 652e 2073 656c 662e      # i.e. self.
-00008400: 6d79 6d6f 6475 6c65 203d 204d 794d 6f64  mymodule = MyMod
-00008410: 756c 6528 2e2e 2e29 0a20 2020 2020 2073  ule(...).      s
-00008420: 656c 662e 6e61 6d65 3a20 4f70 7469 6f6e  elf.name: Option
-00008430: 616c 5b73 7472 5d0a 2020 2020 2020 6966  al[str].      if
-00008440: 2073 656c 662e 7061 7265 6e74 2e5f 7374   self.parent._st
-00008450: 6174 652e 696e 5f73 6574 7570 2061 6e64  ate.in_setup and
-00008460: 2073 656c 662e 6e61 6d65 2069 7320 4e6f   self.name is No
-00008470: 6e65 3a20 2023 2070 7974 7970 653a 2064  ne:  # pytype: d
-00008480: 6973 6162 6c65 3d61 7474 7269 6275 7465  isable=attribute
-00008490: 2d65 7272 6f72 0a20 2020 2020 2020 2072  -error.        r
-000084a0: 6574 7572 6e0a 2020 2020 2020 6966 206e  eturn.      if n
-000084b0: 6f74 2073 656c 662e 7061 7265 6e74 2e5f  ot self.parent._
-000084c0: 696e 6974 6961 6c69 7a61 7469 6f6e 5f61  initialization_a
-000084d0: 6c6c 6f77 6564 3a0a 2020 2020 2020 2020  llowed:.        
-000084e0: 7261 6973 6520 6572 726f 7273 2e41 7373  raise errors.Ass
-000084f0: 6967 6e53 7562 4d6f 6475 6c65 4572 726f  ignSubModuleErro
-00008500: 7228 7365 6c66 2e5f 5f63 6c61 7373 5f5f  r(self.__class__
-00008510: 2e5f 5f6e 616d 655f 5f29 0a20 2020 2020  .__name__).     
-00008520: 2023 2041 7574 6f6e 616d 696e 6720 6f66   # Autonaming of
-00008530: 2073 7562 6d6f 6475 6c65 732e 0a20 2020   submodules..   
-00008540: 2020 2069 6620 7365 6c66 2e6e 616d 6520     if self.name 
-00008550: 6973 204e 6f6e 653a 2020 2320 7079 7479  is None:  # pyty
-00008560: 7065 3a20 6469 7361 626c 653d 6174 7472  pe: disable=attr
-00008570: 6962 7574 652d 6572 726f 720a 2020 2020  ibute-error.    
-00008580: 2020 2020 7072 6566 6978 203d 2066 277b      prefix = f'{
-00008590: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
-000085a0: 5f6e 616d 655f 5f7d 270a 2020 2020 2020  _name__}'.      
-000085b0: 2020 6375 7273 6f72 203d 2073 656c 662e    cursor = self.
-000085c0: 7061 7265 6e74 2e5f 7374 6174 652e 6175  parent._state.au
-000085d0: 746f 6e61 6d65 5f63 7572 736f 722e 6765  toname_cursor.ge
-000085e0: 7428 7072 6566 6978 2c20 3029 0a20 2020  t(prefix, 0).   
-000085f0: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
-00008600: 2066 277b 7072 6566 6978 7d5f 7b63 7572   f'{prefix}_{cur
-00008610: 736f 727d 270a 2020 2020 2020 2020 7365  sor}'.        se
-00008620: 6c66 2e70 6172 656e 742e 5f73 7461 7465  lf.parent._state
-00008630: 2e61 7574 6f6e 616d 655f 6375 7273 6f72  .autoname_cursor
-00008640: 5b70 7265 6669 785d 203d 2063 7572 736f  [prefix] = curso
-00008650: 7220 2b20 310a 2020 2020 2020 2320 416c  r + 1.      # Al
-00008660: 6c6f 7720 7363 6f70 6520 616c 6961 7369  low scope aliasi
-00008670: 6e67 2075 6e64 6572 2074 7261 6e73 666f  ng under transfo
-00008680: 726d 7320 666f 7220 7375 626d 6f64 756c  rms for submodul
-00008690: 6573 2064 6566 696e 6564 2069 6e20 7365  es defined in se
-000086a0: 7475 702e 0a20 2020 2020 2072 6575 7365  tup..      reuse
-000086b0: 5f73 636f 7065 7320 3d20 2873 656c 662e  _scopes = (self.
-000086c0: 7061 7265 6e74 2e5f 7374 6174 652e 696e  parent._state.in
-000086d0: 5f73 6574 7570 2061 6e64 0a20 2020 2020  _setup and.     
-000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086f0: 2073 656c 662e 7061 7265 6e74 2e5f 7374   self.parent._st
-00008700: 6174 652e 7365 7475 705f 6361 6c6c 6564  ate.setup_called
-00008710: 203d 3d20 5365 7475 7053 7461 7465 2e54   == SetupState.T
-00008720: 5241 4e53 464f 524d 4544 290a 2020 2020  RANSFORMED).    
-00008730: 2020 2320 5065 7266 6f72 6d20 6e61 6d65    # Perform name
-00008740: 2d63 6f6c 6c69 7369 6f6e 2063 6865 636b  -collision check
-00008750: 2e0a 2020 2020 2020 6966 2073 656c 662e  ..      if self.
-00008760: 7061 7265 6e74 2e5f 6e61 6d65 5f74 616b  parent._name_tak
-00008770: 656e 2873 656c 662e 6e61 6d65 2c20 7365  en(self.name, se
-00008780: 6c66 2c20 7265 7573 655f 7363 6f70 6573  lf, reuse_scopes
-00008790: 3d72 6575 7365 5f73 636f 7065 7329 3a0a  =reuse_scopes):.
-000087a0: 2020 2020 2020 2020 7061 7265 6e74 5f63          parent_c
-000087b0: 6c61 7373 203d 2073 656c 662e 7061 7265  lass = self.pare
-000087c0: 6e74 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  nt.__class__.__n
-000087d0: 616d 655f 5f0a 2020 2020 2020 2020 7261  ame__.        ra
-000087e0: 6973 6520 6572 726f 7273 2e4e 616d 6549  ise errors.NameI
-000087f0: 6e55 7365 4572 726f 7228 2773 7562 6d6f  nUseError('submo
-00008800: 6475 6c65 272c 2073 656c 662e 6e61 6d65  dule', self.name
-00008810: 2c20 7061 7265 6e74 5f63 6c61 7373 290a  , parent_class).
-00008820: 2020 2020 2020 2320 4669 6e61 6c69 7a65        # Finalize
-00008830: 2061 7474 6163 686d 656e 7420 746f 2070   attachment to p
-00008840: 6172 656e 7420 616e 6420 7363 6f70 6520  arent and scope 
-00008850: 696e 6974 6961 6c69 7a61 7469 6f6e 2e0a  initialization..
-00008860: 2020 2020 2020 7365 6c66 2e70 6172 656e        self.paren
-00008870: 742e 5f73 7461 7465 2e63 6869 6c64 7265  t._state.childre
-00008880: 6e5b 7365 6c66 2e6e 616d 655d 203d 2073  n[self.name] = s
-00008890: 656c 660a 2020 2020 2020 6173 7365 7274  elf.      assert
-000088a0: 2073 656c 662e 7061 7265 6e74 2e73 636f   self.parent.sco
-000088b0: 7065 2069 7320 6e6f 7420 4e6f 6e65 0a20  pe is not None. 
-000088c0: 2020 2020 206f 626a 6563 742e 5f5f 7365       object.__se
-000088d0: 7461 7474 725f 5f28 0a20 2020 2020 2020  tattr__(.       
-000088e0: 2020 2073 656c 662c 2027 7363 6f70 6527     self, 'scope'
-000088f0: 2c20 7365 6c66 2e70 6172 656e 742e 7363  , self.parent.sc
-00008900: 6f70 652e 7075 7368 2873 656c 662e 6e61  ope.push(self.na
-00008910: 6d65 2c20 7265 7573 653d 7265 7573 655f  me, reuse=reuse_
-00008920: 7363 6f70 6573 2929 0a0a 2020 2020 2320  scopes))..    # 
-00008930: 546f 702d 6c65 7665 6c20 696e 766f 6361  Top-level invoca
-00008940: 7469 6f6e 2077 6974 6820 6120 6675 6e63  tion with a func
-00008950: 7469 6f6e 616c 2053 636f 7065 2e0a 2020  tional Scope..  
-00008960: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00008970: 6528 7365 6c66 2e70 6172 656e 742c 2053  e(self.parent, S
-00008980: 636f 7065 293a 0a20 2020 2020 206f 626a  cope):.      obj
-00008990: 6563 742e 5f5f 7365 7461 7474 725f 5f28  ect.__setattr__(
-000089a0: 7365 6c66 2c20 2773 636f 7065 272c 2073  self, 'scope', s
-000089b0: 656c 662e 7061 7265 6e74 290a 2020 2020  elf.parent).    
-000089c0: 656c 7365 3a0a 2020 2020 2020 7261 6973  else:.      rais
-000089d0: 6520 5661 6c75 6545 7272 6f72 2827 7061  e ValueError('pa
-000089e0: 7265 6e74 206d 7573 7420 6265 204e 6f6e  rent must be Non
-000089f0: 652c 204d 6f64 756c 6520 6f72 2053 636f  e, Module or Sco
-00008a00: 7065 2729 0a0a 2020 2020 7365 6c66 2e5f  pe')..    self._
-00008a10: 7374 6174 652e 6973 5f69 6e69 7469 616c  state.is_initial
-00008a20: 697a 6564 203d 2054 7275 650a 0a20 2064  ized = True..  d
-00008a30: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
-00008a40: 2920 2d3e 2073 7472 3a0a 2020 2020 7265  ) -> str:.    re
-00008a50: 7475 726e 205f 6d6f 6475 6c65 5f72 6570  turn _module_rep
-00008a60: 7228 7365 6c66 290a 0a20 2064 6566 2073  r(self)..  def s
-00008a70: 6574 7570 2873 656c 6629 202d 3e20 4e6f  etup(self) -> No
-00008a80: 6e65 3a0a 2020 2020 2222 2249 6e69 7469  ne:.    """Initi
-00008a90: 616c 697a 6573 2061 204d 6f64 756c 6520  alizes a Module 
-00008aa0: 6c61 7a69 6c79 2028 7369 6d69 6c61 7220  lazily (similar 
-00008ab0: 746f 2061 206c 617a 7920 6060 5f5f 696e  to a lazy ``__in
-00008ac0: 6974 5f5f 6060 292e 0a0a 2020 2020 6060  it__``)...    ``
-00008ad0: 7365 7475 7060 6020 6973 2063 616c 6c65  setup`` is calle
-00008ae0: 6420 6f6e 6365 206c 617a 696c 7920 6f6e  d once lazily on
-00008af0: 2061 206d 6f64 756c 6520 696e 7374 616e   a module instan
-00008b00: 6365 2077 6865 6e20 6120 6d6f 6475 6c65  ce when a module
-00008b10: 0a20 2020 2069 7320 626f 756e 642c 2069  .    is bound, i
-00008b20: 6d6d 6564 6961 7465 6c79 2062 6566 6f72  mmediately befor
-00008b30: 6520 616e 7920 6f74 6865 7220 6d65 7468  e any other meth
-00008b40: 6f64 7320 6c69 6b65 2060 605f 5f63 616c  ods like ``__cal
-00008b50: 6c5f 5f60 6020 6172 650a 2020 2020 696e  l__`` are.    in
-00008b60: 766f 6b65 642c 206f 7220 6265 666f 7265  voked, or before
-00008b70: 2061 2060 6073 6574 7570 6060 2d64 6566   a ``setup``-def
-00008b80: 696e 6564 2061 7474 7269 6275 7465 206f  ined attribute o
-00008b90: 6e20 6073 656c 6660 2069 7320 6163 6365  n `self` is acce
-00008ba0: 7373 6564 2e0a 0a20 2020 2054 6869 7320  ssed...    This 
-00008bb0: 6361 6e20 6861 7070 656e 2069 6e20 7468  can happen in th
-00008bc0: 7265 6520 6361 7365 733a 0a0a 2020 2020  ree cases:..    
-00008bd0: 2020 312e 2049 6d6d 6564 6961 7465 6c79    1. Immediately
-00008be0: 2077 6865 6e20 696e 766f 6b69 6e67 203a   when invoking :
-00008bf0: 6d65 7468 3a60 6170 706c 7960 2c20 3a6d  meth:`apply`, :m
-00008c00: 6574 683a 6069 6e69 7460 206f 720a 2020  eth:`init` or.  
-00008c10: 2020 2020 2020 203a 6d65 7468 3a60 696e         :meth:`in
-00008c20: 6974 5f61 6e64 5f6f 7574 7075 7460 2e0a  it_and_output`..
-00008c30: 0a20 2020 2020 2032 2e20 4f6e 6365 2074  .      2. Once t
-00008c40: 6865 206d 6f64 756c 6520 6973 2067 6976  he module is giv
-00008c50: 656e 2061 206e 616d 6520 6279 2062 6569  en a name by bei
-00008c60: 6e67 2061 7373 6967 6e65 6420 746f 2061  ng assigned to a
-00008c70: 6e20 6174 7472 6962 7574 6520 6f66 0a20  n attribute of. 
-00008c80: 2020 2020 2020 2020 616e 6f74 6865 7220          another 
-00008c90: 6d6f 6475 6c65 2069 6e73 6964 6520 7468  module inside th
-00008ca0: 6520 6f74 6865 7220 6d6f 6475 6c65 2773  e other module's
-00008cb0: 2060 6073 6574 7570 6060 206d 6574 686f   ``setup`` metho
-00008cc0: 640a 2020 2020 2020 2020 2028 7365 6520  d.         (see 
-00008cd0: 3a6d 6574 683a 605f 5f73 6574 6174 7472  :meth:`__setattr
-00008ce0: 5f5f 6029 3a3a 0a0a 2020 2020 2020 2020  __`)::..        
-00008cf0: 2020 2063 6c61 7373 204d 794d 6f64 756c     class MyModul
-00008d00: 6528 6e6e 2e4d 6f64 756c 6529 3a0a 2020  e(nn.Module):.  
-00008d10: 2020 2020 2020 2020 2020 2064 6566 2073             def s
-00008d20: 6574 7570 2873 656c 6629 3a0a 2020 2020  etup(self):.    
-00008d30: 2020 2020 2020 2020 2020 2073 7562 6d6f             submo
-00008d40: 6475 6c65 203d 2043 6f6e 7628 2e2e 2e29  dule = Conv(...)
-00008d50: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008d60: 2023 2041 6363 6573 7369 6e67 2060 7375   # Accessing `su
-00008d70: 626d 6f64 756c 6560 2061 7474 7269 6275  bmodule` attribu
-00008d80: 7465 7320 646f 6573 206e 6f74 2079 6574  tes does not yet
-00008d90: 2077 6f72 6b20 6865 7265 2e0a 0a20 2020   work here...   
-00008da0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00008db0: 6520 666f 6c6c 6f77 696e 6720 6c69 6e65  e following line
-00008dc0: 2069 6e76 6f6b 6573 2060 7365 6c66 2e5f   invokes `self._
-00008dd0: 5f73 6574 6174 7472 5f5f 602c 2077 6869  _setattr__`, whi
-00008de0: 6368 2067 6976 6573 0a20 2020 2020 2020  ch gives.       
-00008df0: 2020 2020 2020 2020 2320 6073 7562 6d6f          # `submo
-00008e00: 6475 6c65 6020 7468 6520 6e61 6d65 2022  dule` the name "
-00008e10: 636f 6e76 3122 2e0a 2020 2020 2020 2020  conv1"..        
-00008e20: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-00008e30: 3120 3d20 7375 626d 6f64 756c 650a 0a20  1 = submodule.. 
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008e50: 4163 6365 7373 696e 6720 6073 7562 6d6f  Accessing `submo
-00008e60: 6475 6c65 6020 6174 7472 6962 7574 6573  dule` attributes
-00008e70: 206f 7220 6d65 7468 6f64 7320 6973 206e   or methods is n
-00008e80: 6f77 2073 6166 6520 616e 640a 2020 2020  ow safe and.    
-00008e90: 2020 2020 2020 2020 2020 2023 2065 6974             # eit
-00008ea0: 6865 7220 6361 7573 6573 2073 6574 7570  her causes setup
-00008eb0: 2829 2074 6f20 6265 2063 616c 6c65 6420  () to be called 
-00008ec0: 6f6e 6365 2e0a 0a20 2020 2020 2033 2e20  once...      3. 
-00008ed0: 4f6e 6365 2061 206d 6f64 756c 6520 6973  Once a module is
-00008ee0: 2063 6f6e 7374 7275 6374 6564 2069 6e73   constructed ins
-00008ef0: 6964 6520 6120 6d65 7468 6f64 2077 7261  ide a method wra
-00008f00: 7070 6564 2077 6974 680a 2020 2020 2020  pped with.      
-00008f10: 2020 203a 6d65 7468 3a60 636f 6d70 6163     :meth:`compac
-00008f20: 7460 2c20 696d 6d65 6469 6174 656c 7920  t`, immediately 
-00008f30: 6265 666f 7265 2061 6e6f 7468 6572 206d  before another m
-00008f40: 6574 686f 6420 6973 2063 616c 6c65 6420  ethod is called 
-00008f50: 6f72 0a20 2020 2020 2020 2020 6060 7365  or.         ``se
-00008f60: 7475 7060 6020 6465 6669 6e65 6420 6174  tup`` defined at
-00008f70: 7472 6962 7574 6520 6973 2061 6363 6573  tribute is acces
-00008f80: 7365 642e 0a20 2020 2022 2222 0a20 2020  sed..    """.   
-00008f90: 2070 6173 730a 0a20 2064 6566 205f 7265   pass..  def _re
-00008fa0: 6769 7374 6572 5f73 7562 6d6f 6475 6c65  gister_submodule
-00008fb0: 7328 7365 6c66 2c20 6e61 6d65 2c20 7661  s(self, name, va
-00008fc0: 6c29 3a0a 2020 2020 2222 2252 6567 6973  l):.    """Regis
-00008fd0: 7465 7273 2061 2073 7562 6d6f 6475 6c65  ters a submodule
-00008fe0: 2e22 2222 0a20 2020 2061 7373 6572 7420  .""".    assert 
-00008ff0: 7365 6c66 2e73 636f 7065 2c20 2754 7279  self.scope, 'Try
-00009000: 696e 6720 746f 2072 6567 6973 7465 7220  ing to register 
-00009010: 7375 626d 6f64 756c 6573 206f 6e20 756e  submodules on un
-00009020: 626f 756e 6420 7363 6f70 652e 270a 2020  bound scope.'.  
-00009030: 2020 726f 6f74 203d 2073 656c 662e 7363    root = self.sc
-00009040: 6f70 652e 726f 6f74 0a20 2020 2063 6163  ope.root.    cac
-00009050: 6865 203d 205f 6361 6368 6573 2e67 6574  he = _caches.get
-00009060: 2872 6f6f 742c 2077 6561 6b72 6566 2e57  (root, weakref.W
-00009070: 6561 6b56 616c 7565 4469 6374 696f 6e61  eakValueDictiona
-00009080: 7279 2829 290a 2020 2020 5f63 6163 6865  ry()).    _cache
-00009090: 735b 726f 6f74 5d20 3d20 6361 6368 650a  s[root] = cache.
-000090a0: 2020 2020 7175 6575 6520 3d20 5b5d 0a20      queue = []. 
-000090b0: 2020 2070 7265 7365 7276 655f 6164 6f70     preserve_adop
-000090c0: 7465 645f 6e61 6d65 7320 3d20 636f 6e66  ted_names = conf
-000090d0: 6967 2e66 6c61 785f 7072 6573 6572 7665  ig.flax_preserve
-000090e0: 5f61 646f 7074 6564 5f6e 616d 6573 0a20  _adopted_names. 
-000090f0: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
-00009100: 6c66 2c20 2770 7265 7365 7276 655f 6164  lf, 'preserve_ad
-00009110: 6f70 7465 645f 6e61 6d65 7327 293a 0a20  opted_names'):. 
-00009120: 2020 2020 2020 7072 6573 6572 7665 5f61        preserve_a
-00009130: 646f 7074 6564 5f6e 616d 6573 203d 2073  dopted_names = s
-00009140: 656c 662e 7072 6573 6572 7665 5f61 646f  elf.preserve_ado
-00009150: 7074 6564 5f6e 616d 6573 0a20 2020 2064  pted_names.    d
-00009160: 6566 2061 646f 7074 5f61 7474 725f 6d6f  ef adopt_attr_mo
-00009170: 6475 6c65 7328 6361 6368 652c 2071 7565  dules(cache, que
-00009180: 7565 2c20 7375 6666 6978 2c20 7375 6276  ue, suffix, subv
-00009190: 616c 7565 293a 0a20 2020 2020 2069 6620  alue):.      if 
-000091a0: 6973 696e 7374 616e 6365 2873 7562 7661  isinstance(subva
-000091b0: 6c75 652c 204d 6f64 756c 6529 3a0a 2020  lue, Module):.  
-000091c0: 2020 2020 2020 6164 6f70 7465 645f 6e61        adopted_na
-000091d0: 6d65 203d 204e 6f6e 650a 2020 2020 2020  me = None.      
-000091e0: 2020 6966 2073 7562 7661 6c75 652e 7061    if subvalue.pa
-000091f0: 7265 6e74 2069 7320 4e6f 6e65 3a0a 2020  rent is None:.  
-00009200: 2020 2020 2020 2020 2320 5072 6573 6572          # Preser
-00009210: 7665 2073 6861 7269 6e67 2d62 792d 7265  ve sharing-by-re
-00009220: 6665 7265 6e63 6520 7265 6c61 7469 6f6e  ference relation
-00009230: 7368 6970 7320 6475 7269 6e67 2061 646f  ships during ado
-00009240: 7074 696f 6e0a 2020 2020 2020 2020 2020  ption.          
-00009250: 2320 7669 6120 6361 6368 6520 6b65 7965  # via cache keye
-00009260: 6420 6f6e 2075 6e69 7175 6520 696e 7374  d on unique inst
-00009270: 616e 6365 2069 6473 2e0a 2020 2020 2020  ance ids..      
-00009280: 2020 2020 6b65 7920 3d20 7375 6276 616c      key = subval
-00009290: 7565 2e5f 6964 0a20 2020 2020 2020 2020  ue._id.         
-000092a0: 2023 204d 6f64 756c 6520 7761 7320 7061   # Module was pa
-000092b0: 7373 6564 2066 726f 6d20 6f75 7473 6964  ssed from outsid
-000092c0: 652e 2049 7420 6e65 6564 7320 746f 2062  e. It needs to b
-000092d0: 6520 636c 6f6e 6564 2e0a 2020 2020 2020  e cloned..      
-000092e0: 2020 2020 2320 4f75 7473 6964 6520 6d6f      # Outside mo
-000092f0: 6475 6c65 7320 6172 6520 6e61 6d65 6420  dules are named 
-00009300: 6279 2061 7474 6163 686d 656e 742c 206e  by attachment, n
-00009310: 6f74 2061 6e20 6f75 7465 7220 6e61 6d65  ot an outer name
-00009320: 2c0a 2020 2020 2020 2020 2020 2320 554e  ,.          # UN
-00009330: 4c45 5353 2077 6527 7265 2075 7369 6e67  LESS we're using
-00009340: 206e 6577 2061 646f 7074 6564 206e 616d   new adopted nam
-00009350: 6520 706f 6c69 6379 2c20 696e 2077 6869  e policy, in whi
-00009360: 6368 2063 6173 6520 616e 2065 7869 7374  ch case an exist
-00009370: 696e 670a 2020 2020 2020 2020 2020 2320  ing.          # 
-00009380: 6e61 6d65 2077 696c 6c20 6265 2075 7365  name will be use
-00009390: 642c 2061 7320 6973 206f 6674 656e 2073  d, as is often s
-000093a0: 7570 706c 6965 6420 6279 2063 6f6e 6669  upplied by confi
-000093b0: 6720 7379 7374 656d 732e 0a20 2020 2020  g systems..     
-000093c0: 2020 2020 2069 6620 7072 6573 6572 7665       if preserve
-000093d0: 5f61 646f 7074 6564 5f6e 616d 6573 3a0a  _adopted_names:.
-000093e0: 2020 2020 2020 2020 2020 2020 6164 6f70              adop
-000093f0: 7465 645f 6e61 6d65 203d 206f 626a 6563  ted_name = objec
-00009400: 742e 5f5f 6765 7461 7474 7269 6275 7465  t.__getattribute
-00009410: 5f5f 2873 7562 7661 6c75 652c 2027 6e61  __(subvalue, 'na
-00009420: 6d65 2729 0a20 2020 2020 2020 2020 2069  me').          i
-00009430: 6620 6b65 7920 696e 2063 6163 6865 3a0a  f key in cache:.
-00009440: 2020 2020 2020 2020 2020 2020 7375 6276              subv
-00009450: 616c 7565 203d 2063 6163 6865 5b6b 6579  alue = cache[key
-00009460: 5d0a 2020 2020 2020 2020 2020 656c 7365  ].          else
-00009470: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
-00009480: 6276 616c 7565 203d 2073 7562 7661 6c75  bvalue = subvalu
-00009490: 652e 636c 6f6e 6528 6e61 6d65 3d4e 6f6e  e.clone(name=Non
-000094a0: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
-000094b0: 6163 6865 5b6b 6579 5d20 3d20 7375 6276  ache[key] = subv
-000094c0: 616c 7565 0a20 2020 2020 2020 2069 6620  alue.        if 
-000094d0: 7375 6276 616c 7565 2e6e 616d 6520 6973  subvalue.name is
-000094e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000094f0: 206f 626a 6563 742e 5f5f 7365 7461 7474   object.__setatt
-00009500: 725f 5f28 7375 6276 616c 7565 2c20 2770  r__(subvalue, 'p
-00009510: 6172 656e 7427 2c20 7365 6c66 290a 2020  arent', self).  
-00009520: 2020 2020 2020 2020 6966 2061 646f 7074          if adopt
-00009530: 6564 5f6e 616d 6520 6973 204e 6f6e 653a  ed_name is None:
-00009540: 0a20 2020 2020 2020 2020 2020 2061 646f  .            ado
-00009550: 7074 6564 5f6e 616d 6520 3d20 6627 7b6e  pted_name = f'{n
-00009560: 616d 657d 7b73 7566 6669 787d 270a 2020  ame}{suffix}'.  
-00009570: 2020 2020 2020 2020 6f62 6a65 6374 2e5f          object._
-00009580: 5f73 6574 6174 7472 5f5f 2873 7562 7661  _setattr__(subva
-00009590: 6c75 652c 2027 6e61 6d65 272c 2061 646f  lue, 'name', ado
-000095a0: 7074 6564 5f6e 616d 6529 0a20 2020 2020  pted_name).     
-000095b0: 2020 2020 2071 7565 7565 2e61 7070 656e       queue.appen
-000095c0: 6428 7375 6276 616c 7565 290a 2020 2020  d(subvalue).    
-000095d0: 2020 7265 7475 726e 2073 7562 7661 6c75    return subvalu
-000095e0: 650a 2020 2020 7661 6c20 3d20 5f66 7265  e.    val = _fre
-000095f0: 657a 655f 6174 7472 285f 6d61 705f 6f76  eze_attr(_map_ov
-00009600: 6572 5f6d 6f64 756c 6573 5f69 6e5f 7472  er_modules_in_tr
-00009610: 6565 280a 2020 2020 2020 2020 6675 6e63  ee(.        func
-00009620: 746f 6f6c 732e 7061 7274 6961 6c28 6164  tools.partial(ad
-00009630: 6f70 745f 6174 7472 5f6d 6f64 756c 6573  opt_attr_modules
-00009640: 2c20 6361 6368 652c 2071 7565 7565 292c  , cache, queue),
-00009650: 2076 616c 2929 0a20 2020 206f 626a 6563   val)).    objec
-00009660: 742e 5f5f 7365 7461 7474 725f 5f28 7365  t.__setattr__(se
-00009670: 6c66 2c20 6e61 6d65 2c20 7661 6c29 0a20  lf, name, val). 
-00009680: 2020 2066 6f72 2078 2069 6e20 7175 6575     for x in queu
-00009690: 653a 0a20 2020 2020 2078 2e5f 5f70 6f73  e:.      x.__pos
-000096a0: 745f 696e 6974 5f5f 2829 0a0a 2020 6465  t_init__()..  de
-000096b0: 6620 5f74 7279 5f73 6574 7570 2873 656c  f _try_setup(sel
-000096c0: 662c 2073 6861 6c6c 6f77 3a20 626f 6f6c  f, shallow: bool
-000096d0: 203d 2046 616c 7365 2920 2d3e 204e 6f6e   = False) -> Non
-000096e0: 653a 0a20 2020 2022 2222 5472 6965 7320  e:.    """Tries 
-000096f0: 746f 2073 6574 7570 206d 6f64 756c 6520  to setup module 
-00009700: 6966 2073 636f 7065 2069 7320 6176 6169  if scope is avai
-00009710: 6c61 626c 6520 616e 6420 7365 7475 7020  lable and setup 
-00009720: 6861 7320 6e6f 7420 6265 656e 2063 616c  has not been cal
-00009730: 6c65 6420 7965 742e 2222 220a 2020 2020  led yet.""".    
-00009740: 6966 2028 7365 6c66 2e73 636f 7065 0a20  if (self.scope. 
-00009750: 2020 2020 2020 2061 6e64 206e 6f74 2073         and not s
-00009760: 656c 662e 5f73 7461 7465 2e69 6e5f 7365  elf._state.in_se
-00009770: 7475 700a 2020 2020 2020 2020 616e 6420  tup.        and 
-00009780: 7365 6c66 2e5f 7374 6174 652e 7365 7475  self._state.setu
-00009790: 705f 6361 6c6c 6564 2021 3d20 5365 7475  p_called != Setu
-000097a0: 7053 7461 7465 2e44 4f4e 4529 3a0a 2020  pState.DONE):.  
-000097b0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000097c0: 2073 656c 662e 5f73 7461 7465 2e69 6e5f   self._state.in_
-000097d0: 7365 7475 7020 3d20 5472 7565 0a20 2020  setup = True.   
-000097e0: 2020 2020 2023 2041 2073 6861 6c6c 6f77       # A shallow
-000097f0: 2073 6574 7570 2077 696c 6c20 6f6e 6c79   setup will only
-00009800: 2072 6567 6973 7465 7220 6174 7472 6962   register attrib
-00009810: 7574 6520 7375 626d 6f64 756c 6573 2062  ute submodules b
-00009820: 7574 2069 7420 646f 6573 0a20 2020 2020  ut it does.     
-00009830: 2020 2023 206e 6f74 2063 616c 6c20 7468     # not call th
-00009840: 6520 7573 6572 2773 2073 6574 7570 2e20  e user's setup. 
-00009850: 5468 6973 2061 766f 6964 7320 7275 6e6e  This avoids runn
-00009860: 696e 6720 6265 666f 7265 2061 0a20 2020  ing before a.   
-00009870: 2020 2020 2023 2074 7261 6e73 666f 726d       # transform
-00009880: 6174 696f 6e2e 0a20 2020 2020 2020 2066  ation..        f
-00009890: 6f72 2066 6965 6c64 2069 6e20 6461 7461  or field in data
-000098a0: 636c 6173 7365 732e 6669 656c 6473 2873  classes.fields(s
-000098b0: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
-000098c0: 6966 2066 6965 6c64 2e6e 616d 6520 213d  if field.name !=
-000098d0: 2027 7061 7265 6e74 2720 616e 6420 6669   'parent' and fi
-000098e0: 656c 642e 696e 6974 3a0a 2020 2020 2020  eld.init:.      
-000098f0: 2020 2020 2020 7365 6c66 2e5f 7265 6769        self._regi
-00009900: 7374 6572 5f73 7562 6d6f 6475 6c65 7328  ster_submodules(
-00009910: 6669 656c 642e 6e61 6d65 2c20 6765 7461  field.name, geta
-00009920: 7474 7228 7365 6c66 2c20 6669 656c 642e  ttr(self, field.
-00009930: 6e61 6d65 2929 0a20 2020 2020 2020 2069  name)).        i
-00009940: 6620 6e6f 7420 7368 616c 6c6f 773a 0a20  f not shallow:. 
-00009950: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00009960: 7475 7028 290a 2020 2020 2020 2020 2320  tup().        # 
-00009970: 5765 2072 756e 2073 7461 7469 6320 6368  We run static ch
-00009980: 6563 6b73 2061 6273 7472 6163 746c 7920  ecks abstractly 
-00009990: 6f6e 6365 2066 6f72 2073 6574 7570 2062  once for setup b
-000099a0: 6566 6f72 6520 616e 7920 7472 616e 7366  efore any transf
-000099b0: 6f72 6d73 0a20 2020 2020 2020 2023 2074  orms.        # t
-000099c0: 6f20 6465 7465 6374 206e 616d 6520 636f  o detect name co
-000099d0: 6c6c 6973 696f 6e73 2061 6e64 206f 7468  llisions and oth
-000099e0: 6572 2070 7974 686f 6e20 6572 726f 7273  er python errors
-000099f0: 2e0a 2020 2020 2020 2020 656c 6966 2073  ..        elif s
-00009a00: 656c 662e 5f73 7461 7465 2e73 6574 7570  elf._state.setup
-00009a10: 5f63 616c 6c65 6420 3d3d 2053 6574 7570  _called == Setup
-00009a20: 5374 6174 652e 4e45 573a 0a20 2020 2020  State.NEW:.     
-00009a30: 2020 2020 2073 656c 662e 5f76 616c 6964       self._valid
-00009a40: 6174 655f 7365 7475 7028 290a 2020 2020  ate_setup().    
-00009a50: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
-00009a60: 2020 2073 656c 662e 5f73 7461 7465 2e69     self._state.i
-00009a70: 6e5f 7365 7475 7020 3d20 4661 6c73 650a  n_setup = False.
-00009a80: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
-00009a90: 6174 652e 7365 7475 705f 6361 6c6c 6564  ate.setup_called
-00009aa0: 203d 2053 6574 7570 5374 6174 652e 444f   = SetupState.DO
-00009ab0: 4e45 0a0a 2020 6465 6620 5f76 616c 6964  NE..  def _valid
-00009ac0: 6174 655f 7365 7475 7028 7365 6c66 2920  ate_setup(self) 
-00009ad0: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-00009ae0: 4162 7374 7261 6374 6c79 2065 7661 6c75  Abstractly evalu
-00009af0: 6174 6573 2073 6574 7570 206f 6e6c 7920  ates setup only 
-00009b00: 746f 2072 756e 2073 7461 7469 6320 6368  to run static ch
-00009b10: 6563 6b73 2e22 2222 0a20 2020 2064 6566  ecks.""".    def
-00009b20: 2072 756e 5f73 6574 7570 5f6f 6e6c 7928   run_setup_only(
-00009b30: 7829 3a0a 2020 2020 2020 7772 6170 7065  x):.      wrappe
-00009b40: 645f 6964 203d 2077 7261 705f 6d65 7468  d_id = wrap_meth
-00009b50: 6f64 5f6f 6e63 6528 6c61 6d62 6461 206d  od_once(lambda m
-00009b60: 2c20 783a 2078 290a 2020 2020 2020 7769  , x: x).      wi
-00009b70: 7468 2054 6573 7453 636f 7065 287b 7d2c  th TestScope({},
-00009b80: 2072 6e67 733d 7b7d 2c20 6d75 7461 626c   rngs={}, mutabl
-00009b90: 653d 5472 7565 292e 7465 6d70 6f72 6172  e=True).temporar
-00009ba0: 7928 2920 6173 2072 6f6f 743a 0a20 2020  y() as root:.   
-00009bb0: 2020 2020 2072 6574 7572 6e20 7772 6170       return wrap
-00009bc0: 7065 645f 6964 2873 656c 662e 636c 6f6e  ped_id(self.clon
-00009bd0: 6528 7061 7265 6e74 3d72 6f6f 7429 2c20  e(parent=root), 
-00009be0: 7829 0a20 2020 205f 203d 206a 6178 2e65  x).    _ = jax.e
-00009bf0: 7661 6c5f 7368 6170 6528 7275 6e5f 7365  val_shape(run_se
-00009c00: 7475 705f 6f6e 6c79 2c20 3029 0a0a 2020  tup_only, 0)..  
-00009c10: 6465 6620 5f6e 616d 655f 7461 6b65 6e28  def _name_taken(
-00009c20: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00009c30: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
-00009c40: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00009c50: 2020 2020 206d 6f64 756c 653a 204f 7074       module: Opt
-00009c60: 696f 6e61 6c5b 274d 6f64 756c 6527 5d20  ional['Module'] 
-00009c70: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00009c80: 2020 2020 2020 2020 2020 7265 7573 655f            reuse_
-00009c90: 7363 6f70 6573 3a20 626f 6f6c 203d 2046  scopes: bool = F
-00009ca0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00009cb0: 2020 2020 2020 2020 636f 6c6c 6563 7469          collecti
-00009cc0: 6f6e 3a20 4f70 7469 6f6e 616c 5b73 7472  on: Optional[str
-00009cd0: 5d20 3d20 4e6f 6e65 2920 2d3e 2062 6f6f  ] = None) -> boo
-00009ce0: 6c3a 0a20 2020 2061 7373 6572 7420 7365  l:.    assert se
-00009cf0: 6c66 2e73 636f 7065 2069 7320 6e6f 7420  lf.scope is not 
-00009d00: 4e6f 6e65 0a20 2020 2023 2077 6974 6820  None.    # with 
-00009d10: 7265 6c61 7865 6420 6e61 6d69 6e67 2064  relaxed naming d
-00009d20: 6f6e 2774 2066 6f72 6365 206e 6f6e 2d6f  on't force non-o
-00009d30: 7665 726c 6170 2077 6974 6820 7079 7468  verlap with pyth
-00009d40: 6f6e 2061 7474 7269 6275 7465 206e 616d  on attribute nam
-00009d50: 6573 2e0a 2020 2020 6966 2063 6f6e 6669  es..    if confi
-00009d60: 672e 666c 6178 5f72 656c 6178 6564 5f6e  g.flax_relaxed_n
-00009d70: 616d 696e 673a 0a20 2020 2020 2069 6620  aming:.      if 
-00009d80: 7265 7573 655f 7363 6f70 6573 3a0a 2020  reuse_scopes:.  
-00009d90: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00009da0: 7365 0a20 2020 2020 2072 6574 7572 6e20  se.      return 
-00009db0: 7365 6c66 2e73 636f 7065 2e6e 616d 655f  self.scope.name_
-00009dc0: 7265 7365 7276 6564 286e 616d 652c 2063  reserved(name, c
-00009dd0: 6f6c 6c65 6374 696f 6e29 0a20 2020 2069  ollection).    i
-00009de0: 6620 6e61 6d65 2069 6e20 5f61 6c6c 5f6e  f name in _all_n
-00009df0: 616d 6573 5f6f 6e5f 6f62 6a65 6374 2873  ames_on_object(s
-00009e00: 656c 6629 3a0a 2020 2020 2020 7661 6c20  elf):.      val 
-00009e10: 3d20 6765 7461 7474 7228 7365 6c66 2c20  = getattr(self, 
-00009e20: 6e61 6d65 2c20 4e6f 6e65 290a 2020 2020  name, None).    
-00009e30: 2020 6966 206d 6f64 756c 6520 6973 206e    if module is n
-00009e40: 6f74 204e 6f6e 6520 616e 6420 7661 6c20  ot None and val 
-00009e50: 6973 206d 6f64 756c 653a 0a20 2020 2020  is module:.     
-00009e60: 2020 2023 206e 616d 6520 6973 2074 616b     # name is tak
-00009e70: 656e 2062 7920 7468 6520 7661 6c75 6520  en by the value 
-00009e80: 6974 7365 6c66 2062 6563 6175 7365 0a20  itself because. 
-00009e90: 2020 2020 2020 2023 2066 6965 6c64 2061         # field a
-00009ea0: 7373 6967 6e6d 656e 7420 6861 7070 656e  ssignment happen
-00009eb0: 6564 2062 6566 6f72 6520 6e61 6d69 6e67  ed before naming
-00009ec0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009ed0: 4661 6c73 650a 2020 2020 2020 7265 7475  False.      retu
-00009ee0: 726e 2054 7275 650a 2020 2020 2320 4368  rn True.    # Ch
-00009ef0: 6563 6b20 666f 7220 7468 6520 6578 6973  eck for the exis
-00009f00: 7465 6e63 6520 6f66 206e 616d 6520 696e  tence of name in
-00009f10: 2074 6865 2073 636f 7065 206f 626a 6563   the scope objec
-00009f20: 742e 0a20 2020 2069 6620 7265 7573 655f  t..    if reuse_
-00009f30: 7363 6f70 6573 3a0a 2020 2020 2020 7265  scopes:.      re
-00009f40: 7475 726e 2046 616c 7365 0a20 2020 2072  turn False.    r
-00009f50: 6574 7572 6e20 6e61 6d65 2069 6e20 7365  eturn name in se
-00009f60: 6c66 2e73 636f 7065 2e72 6573 6572 7661  lf.scope.reserva
-00009f70: 7469 6f6e 730a 0a20 2040 7072 6f70 6572  tions..  @proper
-00009f80: 7479 0a20 2064 6566 205f 696e 6974 6961  ty.  def _initia
-00009f90: 6c69 7a61 7469 6f6e 5f61 6c6c 6f77 6564  lization_allowed
-00009fa0: 2873 656c 6629 3a0a 2020 2020 7265 7475  (self):.    retu
-00009fb0: 726e 2073 656c 662e 5f73 7461 7465 2e69  rn self._state.i
-00009fc0: 6e5f 7365 7475 7020 6f72 2073 656c 662e  n_setup or self.
-00009fd0: 5f73 7461 7465 2e69 6e5f 636f 6d70 6163  _state.in_compac
-00009fe0: 745f 6d65 7468 6f64 0a0a 2020 6465 6620  t_method..  def 
-00009ff0: 636c 6f6e 6528 7365 6c66 3a20 4d2c 202a  clone(self: M, *
-0000a000: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-0000a010: 7265 6e74 3a20 4f70 7469 6f6e 616c 5b55  rent: Optional[U
-0000a020: 6e69 6f6e 5b53 636f 7065 2c20 274d 6f64  nion[Scope, 'Mod
-0000a030: 756c 6527 5d5d 203d 204e 6f6e 652c 0a20  ule']] = None,. 
-0000a040: 2020 2020 2020 2020 2020 202a 2a75 7064             **upd
-0000a050: 6174 6573 2920 2d3e 204d 3a0a 2020 2020  ates) -> M:.    
-0000a060: 2222 2243 7265 6174 6573 2061 2063 6c6f  """Creates a clo
-0000a070: 6e65 206f 6620 7468 6973 204d 6f64 756c  ne of this Modul
-0000a080: 652c 2077 6974 6820 6f70 7469 6f6e 616c  e, with optional
-0000a090: 6c79 2075 7064 6174 6564 2061 7267 756d  ly updated argum
-0000a0a0: 656e 7473 2e0a 0a20 2020 2041 7267 733a  ents...    Args:
-0000a0b0: 0a20 2020 2020 2070 6172 656e 743a 2054  .      parent: T
-0000a0c0: 6865 2070 6172 656e 7420 6f66 2074 6865  he parent of the
-0000a0d0: 2063 6c6f 6e65 2e20 5468 6520 636c 6f6e   clone. The clon
-0000a0e0: 6520 7769 6c6c 2068 6176 6520 6e6f 2070  e will have no p
-0000a0f0: 6172 656e 7420 6966 206e 6f0a 2020 2020  arent if no.    
-0000a100: 2020 2020 6578 706c 6963 6974 2070 6172      explicit par
-0000a110: 656e 7420 6973 2073 7065 6369 6669 6564  ent is specified
-0000a120: 2e0a 2020 2020 2020 2a2a 7570 6461 7465  ..      **update
-0000a130: 733a 2041 7474 7269 6275 7465 2075 7064  s: Attribute upd
-0000a140: 6174 6573 2e0a 2020 2020 5265 7475 726e  ates..    Return
-0000a150: 733a 0a20 2020 2020 2041 2063 6c6f 6e65  s:.      A clone
-0000a160: 206f 6620 7468 6520 7468 6973 204d 6f64   of the this Mod
-0000a170: 756c 6520 7769 7468 2074 6865 2075 7064  ule with the upd
-0000a180: 6174 6564 2061 7474 7269 6275 7465 7320  ated attributes 
-0000a190: 616e 6420 7061 7265 6e74 2e0a 2020 2020  and parent..    
-0000a1a0: 2222 220a 2020 2020 6174 7472 7320 3d20  """.    attrs = 
-0000a1b0: 7b66 2e6e 616d 653a 2067 6574 6174 7472  {f.name: getattr
-0000a1c0: 2873 656c 662c 2066 2e6e 616d 6529 2066  (self, f.name) f
-0000a1d0: 6f72 2066 2069 6e20 6461 7461 636c 6173  or f in dataclas
-0000a1e0: 7365 732e 6669 656c 6473 2873 656c 6629  ses.fields(self)
-0000a1f0: 2069 6620 662e 696e 6974 7d0a 2020 2020   if f.init}.    
-0000a200: 6174 7472 732e 7570 6461 7465 2870 6172  attrs.update(par
-0000a210: 656e 743d 7061 7265 6e74 2c20 2a2a 7570  ent=parent, **up
-0000a220: 6461 7465 7329 0a20 2020 2072 6574 7572  dates).    retur
-0000a230: 6e20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  n self.__class__
-0000a240: 282a 2a61 7474 7273 290a 0a20 2064 6566  (**attrs)..  def
-0000a250: 2076 6172 6961 626c 6528 7365 6c66 2c20   variable(self, 
-0000a260: 636f 6c3a 2073 7472 2c20 6e61 6d65 3a20  col: str, name: 
-0000a270: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0000a280: 2020 2020 696e 6974 5f66 6e3a 204f 7074      init_fn: Opt
-0000a290: 696f 6e61 6c5b 4361 6c6c 6162 6c65 5b2e  ional[Callable[.
-0000a2a0: 2e2e 2c20 416e 795d 5d20 3d20 4e6f 6e65  .., Any]] = None
-0000a2b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a2c0: 202a 696e 6974 5f61 7267 732c 0a20 2020   *init_args,.   
-0000a2d0: 2020 2020 2020 2020 2020 2020 756e 626f              unbo
-0000a2e0: 783a 2062 6f6f 6c20 3d20 5472 7565 2920  x: bool = True) 
-0000a2f0: 2d3e 2056 6172 6961 626c 653a 0a20 2020  -> Variable:.   
-0000a300: 2022 2222 4465 636c 6172 6573 2061 6e64   """Declares and
-0000a310: 2072 6574 7572 6e73 2061 2076 6172 6961   returns a varia
-0000a320: 626c 6520 696e 2074 6869 7320 4d6f 6475  ble in this Modu
-0000a330: 6c65 2e0a 0a20 2020 2053 6565 203a 6d6f  le...    See :mo
-0000a340: 643a 6066 6c61 782e 636f 7265 2e76 6172  d:`flax.core.var
-0000a350: 6961 626c 6573 6020 666f 7220 6d6f 7265  iables` for more
-0000a360: 2069 6e66 6f72 6d61 7469 6f6e 2e20 5365   information. Se
-0000a370: 6520 616c 736f 203a 6d65 7468 3a60 7061  e also :meth:`pa
-0000a380: 7261 6d60 0a20 2020 2066 6f72 2061 2073  ram`.    for a s
-0000a390: 686f 7274 6861 6e64 2077 6179 2074 6f20  horthand way to 
-0000a3a0: 6465 6669 6e65 2072 6561 642d 6f6e 6c79  define read-only
-0000a3b0: 2076 6172 6961 626c 6573 2069 6e20 7468   variables in th
-0000a3c0: 6520 2270 6172 616d 7322 0a20 2020 2063  e "params".    c
-0000a3d0: 6f6c 6c65 6374 696f 6e2e 0a0a 2020 2020  ollection...    
-0000a3e0: 436f 6e74 7261 7279 2074 6f20 3a6d 6574  Contrary to :met
-0000a3f0: 683a 6070 6172 616d 602c 2061 6c6c 2061  h:`param`, all a
-0000a400: 7267 756d 656e 7473 2070 6173 7369 6e67  rguments passing
-0000a410: 2075 7369 6e67 2060 696e 6974 5f66 6e60   using `init_fn`
-0000a420: 2073 686f 756c 6420 6265 0a20 2020 2070   should be.    p
-0000a430: 6173 7365 6420 6f6e 2065 7870 6c69 6369  assed on explici
-0000a440: 746c 793a 3a0a 0a20 2020 2020 206b 6579  tly::..      key
-0000a450: 203d 2073 656c 662e 6d61 6b65 5f72 6e67   = self.make_rng
-0000a460: 2827 7374 6174 7327 290a 2020 2020 2020  ('stats').      
-0000a470: 6d65 616e 203d 2073 656c 662e 7661 7269  mean = self.vari
-0000a480: 6162 6c65 2827 7374 6174 7327 2c20 276d  able('stats', 'm
-0000a490: 6561 6e27 2c20 6c65 6375 6e5f 6e6f 726d  ean', lecun_norm
-0000a4a0: 616c 2829 2c20 6b65 792c 2028 322c 2032  al(), key, (2, 2
-0000a4b0: 2929 0a0a 2020 2020 496e 2074 6865 2065  ))..    In the e
-0000a4c0: 7861 6d70 6c65 2061 626f 7665 2c20 7468  xample above, th
-0000a4d0: 6520 6675 6e63 7469 6f6e 2060 6c65 6375  e function `lecu
-0000a4e0: 6e5f 6e6f 726d 616c 6020 6578 7065 6374  n_normal` expect
-0000a4f0: 7320 7477 6f20 6172 6775 6d65 6e74 733a  s two arguments:
-0000a500: 0a20 2020 2060 6b65 7960 2061 6e64 2060  .    `key` and `
-0000a510: 7368 6170 6560 2c20 616e 6420 626f 7468  shape`, and both
-0000a520: 2068 6176 6520 746f 2062 6520 7061 7373   have to be pass
-0000a530: 6564 206f 6e2e 2054 6865 2050 524e 4720  ed on. The PRNG 
-0000a540: 666f 7220 6073 7461 7473 6020 6861 730a  for `stats` has.
-0000a550: 2020 2020 746f 2062 6520 7072 6f76 6964      to be provid
-0000a560: 6564 2065 7870 6c69 6369 746c 7920 7768  ed explicitly wh
-0000a570: 656e 2063 616c 6c69 6e67 203a 6d65 7468  en calling :meth
-0000a580: 3a60 696e 6974 6020 616e 6420 3a6d 6574  :`init` and :met
-0000a590: 683a 6061 7070 6c79 602e 0a0a 2020 2020  h:`apply`...    
-0000a5a0: 4172 6773 3a0a 2020 2020 2020 636f 6c3a  Args:.      col:
-0000a5b0: 2054 6865 2076 6172 6961 626c 6520 636f   The variable co
-0000a5c0: 6c6c 6563 7469 6f6e 206e 616d 652e 0a20  llection name.. 
-0000a5d0: 2020 2020 206e 616d 653a 2054 6865 2076       name: The v
-0000a5e0: 6172 6961 626c 6520 6e61 6d65 2e0a 2020  ariable name..  
-0000a5f0: 2020 2020 696e 6974 5f66 6e3a 2054 6865      init_fn: The
-0000a600: 2066 756e 6374 696f 6e20 7468 6174 2077   function that w
-0000a610: 696c 6c20 6265 2063 616c 6c65 6420 746f  ill be called to
-0000a620: 2063 6f6d 7075 7465 2074 6865 2069 6e69   compute the ini
-0000a630: 7469 616c 2076 616c 7565 0a20 2020 2020  tial value.     
-0000a640: 2020 206f 6620 7468 6973 2076 6172 6961     of this varia
-0000a650: 626c 652e 2054 6869 7320 6675 6e63 7469  ble. This functi
-0000a660: 6f6e 2077 696c 6c20 6f6e 6c79 2062 6520  on will only be 
-0000a670: 6361 6c6c 6564 2074 6865 2066 6972 7374  called the first
-0000a680: 2074 696d 650a 2020 2020 2020 2020 7468   time.        th
-0000a690: 6973 2076 6172 6961 626c 6520 6973 2075  is variable is u
-0000a6a0: 7365 6420 696e 2074 6869 7320 6d6f 6475  sed in this modu
-0000a6b0: 6c65 2e20 4966 204e 6f6e 652c 2074 6865  le. If None, the
-0000a6c0: 2076 6172 6961 626c 6520 6d75 7374 0a20   variable must. 
-0000a6d0: 2020 2020 2020 2061 6c72 6561 6479 2062         already b
-0000a6e0: 6520 696e 6974 6961 6c69 7a65 6420 6f74  e initialized ot
-0000a6f0: 6865 7277 6973 6520 616e 2065 7272 6f72  herwise an error
-0000a700: 2069 7320 7261 6973 6564 2e0a 2020 2020   is raised..    
-0000a710: 2020 2a69 6e69 745f 6172 6773 3a20 5468    *init_args: Th
-0000a720: 6520 6172 6775 6d65 6e74 7320 746f 2070  e arguments to p
-0000a730: 6173 7320 746f 2069 6e69 745f 666e 2e0a  ass to init_fn..
-0000a740: 2020 2020 2020 756e 626f 783a 2049 6620        unbox: If 
-0000a750: 5472 7565 2c20 6060 4178 6973 4d65 7461  True, ``AxisMeta
-0000a760: 6461 7461 6060 2069 6e73 7461 6e63 6573  data`` instances
-0000a770: 2061 7265 2072 6570 6c61 6365 6420 6279   are replaced by
-0000a780: 2074 6865 6972 2075 6e62 6f78 6564 0a20   their unboxed. 
-0000a790: 2020 2020 2020 2076 616c 7565 2c20 7365         value, se
-0000a7a0: 6520 6060 666c 6178 2e6e 6e2e 6d65 7461  e ``flax.nn.meta
-0000a7b0: 2e75 6e62 6f78 6060 2028 6465 6661 756c  .unbox`` (defaul
-0000a7c0: 743a 2054 7275 6529 2e0a 0a20 2020 2052  t: True)...    R
-0000a7d0: 6574 7572 6e73 3a0a 2020 2020 2020 4120  eturns:.      A 
-0000a7e0: 3a63 6c61 7373 3a60 666c 6178 2e63 6f72  :class:`flax.cor
-0000a7f0: 652e 7661 7269 6162 6c65 732e 5661 7269  e.variables.Vari
-0000a800: 6162 6c65 6020 7468 6174 2063 616e 2062  able` that can b
-0000a810: 6520 7265 6164 206f 7220 7365 7420 7669  e read or set vi
-0000a820: 610a 2020 2020 2020 222e 7661 6c75 6522  a.      ".value"
-0000a830: 2061 7474 7269 6275 7465 2e20 5468 726f   attribute. Thro
-0000a840: 7773 2061 6e20 6572 726f 7220 6966 2074  ws an error if t
-0000a850: 6865 2076 6172 6961 626c 6520 6578 6973  he variable exis
-0000a860: 7473 2061 6c72 6561 6479 2e0a 2020 2020  ts already..    
-0000a870: 2222 220a 2020 2020 6966 206e 6f74 2073  """.    if not s
-0000a880: 656c 662e 5f69 6e69 7469 616c 697a 6174  elf._initializat
-0000a890: 696f 6e5f 616c 6c6f 7765 643a 0a20 2020  ion_allowed:.   
-0000a8a0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000a8b0: 726f 7228 0a20 2020 2020 2020 2020 2027  ror(.          '
-0000a8c0: 5661 7269 6162 6c65 7320 6d75 7374 2062  Variables must b
-0000a8d0: 6520 696e 6974 6961 6c69 7a65 6420 696e  e initialized in
-0000a8e0: 2060 7365 7475 7028 2960 206f 7220 696e   `setup()` or in
-0000a8f0: 2061 206d 6574 686f 6420 270a 2020 2020   a method '.    
-0000a900: 2020 2020 2020 2777 7261 7070 6564 2069        'wrapped i
-0000a910: 6e20 6040 636f 6d70 6163 7460 2729 0a20  n `@compact`'). 
-0000a920: 2020 2069 6620 7365 6c66 2e5f 6e61 6d65     if self._name
-0000a930: 5f74 616b 656e 286e 616d 652c 2063 6f6c  _taken(name, col
-0000a940: 6c65 6374 696f 6e3d 636f 6c29 3a0a 2020  lection=col):.  
-0000a950: 2020 2020 7261 6973 6520 6572 726f 7273      raise errors
-0000a960: 2e4e 616d 6549 6e55 7365 4572 726f 7228  .NameInUseError(
-0000a970: 2776 6172 6961 626c 6527 2c20 6e61 6d65  'variable', name
-0000a980: 2c20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  , self.__class__
-0000a990: 2e5f 5f6e 616d 655f 5f29 0a20 2020 2061  .__name__).    a
-0000a9a0: 7373 6572 7420 7365 6c66 2e73 636f 7065  ssert self.scope
-0000a9b0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000a9c0: 2076 203d 2073 656c 662e 7363 6f70 652e   v = self.scope.
-0000a9d0: 7661 7269 6162 6c65 2863 6f6c 2c20 6e61  variable(col, na
-0000a9e0: 6d65 2c20 696e 6974 5f66 6e2c 202a 696e  me, init_fn, *in
-0000a9f0: 6974 5f61 7267 732c 2075 6e62 6f78 3d75  it_args, unbox=u
-0000aa00: 6e62 6f78 290a 2020 2020 7365 6c66 2e5f  nbox).    self._
-0000aa10: 7374 6174 652e 6368 696c 6472 656e 5b6e  state.children[n
-0000aa20: 616d 655d 203d 2063 6f6c 0a20 2020 2072  ame] = col.    r
-0000aa30: 6574 7572 6e20 760a 0a20 2064 6566 2070  eturn v..  def p
-0000aa40: 6172 616d 2873 656c 662c 206e 616d 653a  aram(self, name:
-0000aa50: 2073 7472 2c20 696e 6974 5f66 6e3a 2043   str, init_fn: C
-0000aa60: 616c 6c61 626c 655b 2e2e 2e2c 2054 5d2c  allable[..., T],
-0000aa70: 202a 696e 6974 5f61 7267 732c 0a20 2020   *init_args,.   
-0000aa80: 2020 2020 2020 2020 2075 6e62 6f78 3a20           unbox: 
-0000aa90: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
-0000aaa0: 543a 0a20 2020 2022 2222 4465 636c 6172  T:.    """Declar
-0000aab0: 6573 2061 6e64 2072 6574 7572 6e73 2061  es and returns a
-0000aac0: 2070 6172 616d 6574 6572 2069 6e20 7468   parameter in th
-0000aad0: 6973 204d 6f64 756c 652e 0a0a 2020 2020  is Module...    
-0000aae0: 5061 7261 6d65 7465 7273 2061 7265 2072  Parameters are r
-0000aaf0: 6561 642d 6f6e 6c79 2076 6172 6961 626c  ead-only variabl
-0000ab00: 6573 2069 6e20 7468 6520 636f 6c6c 6563  es in the collec
-0000ab10: 7469 6f6e 206e 616d 6564 2022 7061 7261  tion named "para
-0000ab20: 6d73 222e 2053 6565 0a20 2020 203a 6d6f  ms". See.    :mo
-0000ab30: 643a 6066 6c61 782e 636f 7265 2e76 6172  d:`flax.core.var
-0000ab40: 6961 626c 6573 6020 666f 7220 6d6f 7265  iables` for more
-0000ab50: 2064 6574 6169 6c73 206f 6e20 7661 7269   details on vari
-0000ab60: 6162 6c65 732e 0a0a 2020 2020 5468 6520  ables...    The 
-0000ab70: 6669 7273 7420 6172 6775 6d65 6e74 206f  first argument o
-0000ab80: 6620 6069 6e69 745f 666e 6020 6973 2061  f `init_fn` is a
-0000ab90: 7373 756d 6564 2074 6f20 6265 2061 2050  ssumed to be a P
-0000aba0: 524e 4720 6b65 792c 2077 6869 6368 2069  RNG key, which i
-0000abb0: 730a 2020 2020 7072 6f76 6964 6564 2061  s.    provided a
-0000abc0: 7574 6f6d 6174 6963 616c 6c79 2061 6e64  utomatically and
-0000abd0: 2064 6f65 7320 6e6f 7420 6861 7665 2074   does not have t
-0000abe0: 6f20 6265 2070 6173 7365 6420 7573 696e  o be passed usin
-0000abf0: 6720 6069 6e69 745f 6172 6773 603a 3a0a  g `init_args`::.
-0000ac00: 0a20 2020 2020 206d 6561 6e20 3d20 7365  .      mean = se
-0000ac10: 6c66 2e70 6172 616d 2827 6d65 616e 272c  lf.param('mean',
-0000ac20: 206c 6563 756e 5f6e 6f72 6d61 6c28 292c   lecun_normal(),
-0000ac30: 2028 322c 2032 2929 0a0a 2020 2020 496e   (2, 2))..    In
-0000ac40: 2074 6865 2065 7861 6d70 6c65 2061 626f   the example abo
-0000ac50: 7665 2c20 7468 6520 6675 6e63 7469 6f6e  ve, the function
-0000ac60: 2060 6c65 6375 6e5f 6e6f 726d 616c 6020   `lecun_normal` 
-0000ac70: 6578 7065 6374 7320 7477 6f20 6172 6775  expects two argu
-0000ac80: 6d65 6e74 733a 0a20 2020 2060 6b65 7960  ments:.    `key`
-0000ac90: 2061 6e64 2060 7368 6170 6560 2c20 6275   and `shape`, bu
-0000aca0: 7420 6f6e 6c79 2060 7368 6170 6560 2068  t only `shape` h
-0000acb0: 6173 2074 6f20 6265 2070 726f 7669 6465  as to be provide
-0000acc0: 6420 6578 706c 6963 6974 6c79 3b20 606b  d explicitly; `k
-0000acd0: 6579 600a 2020 2020 6973 2073 6574 2061  ey`.    is set a
-0000ace0: 7574 6f6d 6174 6963 616c 6c79 2075 7369  utomatically usi
-0000acf0: 6e67 2074 6865 2050 524e 4720 666f 7220  ng the PRNG for 
-0000ad00: 6070 6172 616d 7360 2074 6861 7420 6973  `params` that is
-0000ad10: 2070 6173 7365 6420 7768 656e 0a20 2020   passed when.   
-0000ad20: 2069 6e69 7469 616c 697a 696e 6720 7468   initializing th
-0000ad30: 6520 6d6f 6475 6c65 2075 7369 6e67 203a  e module using :
-0000ad40: 6d65 7468 3a60 696e 6974 602e 0a0a 2020  meth:`init`...  
-0000ad50: 2020 4172 6773 3a0a 2020 2020 2020 6e61    Args:.      na
-0000ad60: 6d65 3a20 5468 6520 7061 7261 6d65 7465  me: The paramete
-0000ad70: 7220 6e61 6d65 2e0a 2020 2020 2020 696e  r name..      in
-0000ad80: 6974 5f66 6e3a 2054 6865 2066 756e 6374  it_fn: The funct
-0000ad90: 696f 6e20 7468 6174 2077 696c 6c20 6265  ion that will be
-0000ada0: 2063 616c 6c65 6420 746f 2063 6f6d 7075   called to compu
-0000adb0: 7465 2074 6865 2069 6e69 7469 616c 2076  te the initial v
-0000adc0: 616c 7565 0a20 2020 2020 2020 206f 6620  alue.        of 
-0000add0: 7468 6973 2076 6172 6961 626c 652e 2054  this variable. T
-0000ade0: 6869 7320 6675 6e63 7469 6f6e 2077 696c  his function wil
-0000adf0: 6c20 6f6e 6c79 2062 6520 6361 6c6c 6564  l only be called
-0000ae00: 2074 6865 2066 6972 7374 2074 696d 650a   the first time.
-0000ae10: 2020 2020 2020 2020 7468 6973 2070 6172          this par
-0000ae20: 616d 6574 6572 2069 7320 7573 6564 2069  ameter is used i
-0000ae30: 6e20 7468 6973 206d 6f64 756c 652e 0a20  n this module.. 
-0000ae40: 2020 2020 202a 696e 6974 5f61 7267 733a       *init_args:
-0000ae50: 2054 6865 2061 7267 756d 656e 7473 2074   The arguments t
-0000ae60: 6f20 7061 7373 2074 6f20 696e 6974 5f66  o pass to init_f
-0000ae70: 6e2e 0a20 2020 2020 2075 6e62 6f78 3a20  n..      unbox: 
-0000ae80: 4966 2054 7275 652c 2060 6041 7869 734d  If True, ``AxisM
-0000ae90: 6574 6164 6174 6160 6020 696e 7374 616e  etadata`` instan
-0000aea0: 6365 7320 6172 6520 7265 706c 6163 6564  ces are replaced
-0000aeb0: 2062 7920 7468 6569 7220 756e 626f 7865   by their unboxe
-0000aec0: 640a 2020 2020 2020 2020 7661 6c75 652c  d.        value,
-0000aed0: 2073 6565 2060 6066 6c61 782e 6e6e 2e6d   see ``flax.nn.m
-0000aee0: 6574 612e 756e 626f 7860 6020 2864 6566  eta.unbox`` (def
-0000aef0: 6175 6c74 3a20 5472 7565 292e 0a0a 2020  ault: True)...  
-0000af00: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000af10: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
-0000af20: 6520 696e 6974 6961 6c69 7a65 6420 7061  e initialized pa
-0000af30: 7261 6d65 7465 722e 2054 6872 6f77 7320  rameter. Throws 
-0000af40: 616e 2065 7272 6f72 2069 6620 7468 6520  an error if the 
-0000af50: 7061 7261 6d65 7465 720a 2020 2020 2020  parameter.      
-0000af60: 6578 6973 7473 2061 6c72 6561 6479 2e0a  exists already..
-0000af70: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
-0000af80: 6f74 2073 656c 662e 5f69 6e69 7469 616c  ot self._initial
-0000af90: 697a 6174 696f 6e5f 616c 6c6f 7765 643a  ization_allowed:
-0000afa0: 0a20 2020 2020 2072 6169 7365 2056 616c  .      raise Val
-0000afb0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-0000afc0: 2020 2027 5061 7261 6d65 7465 7273 206d     'Parameters m
-0000afd0: 7573 7420 6265 2069 6e69 7469 616c 697a  ust be initializ
-0000afe0: 6564 2069 6e20 6073 6574 7570 2829 6020  ed in `setup()` 
-0000aff0: 6f72 2069 6e20 6120 6d65 7468 6f64 2027  or in a method '
-0000b000: 0a20 2020 2020 2020 2020 2027 7772 6170  .          'wrap
-0000b010: 7065 6420 696e 2060 4063 6f6d 7061 6374  ped in `@compact
-0000b020: 6027 290a 2020 2020 6966 2073 656c 662e  `').    if self.
-0000b030: 5f6e 616d 655f 7461 6b65 6e28 6e61 6d65  _name_taken(name
-0000b040: 2c20 636f 6c6c 6563 7469 6f6e 3d27 7061  , collection='pa
-0000b050: 7261 6d73 2729 3a0a 2020 2020 2020 7261  rams'):.      ra
-0000b060: 6973 6520 6572 726f 7273 2e4e 616d 6549  ise errors.NameI
-0000b070: 6e55 7365 4572 726f 7228 2770 6172 616d  nUseError('param
-0000b080: 272c 206e 616d 652c 2073 656c 662e 5f5f  ', name, self.__
-0000b090: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-0000b0a0: 290a 2020 2020 6173 7365 7274 2073 656c  ).    assert sel
-0000b0b0: 662e 7363 6f70 6520 6973 206e 6f74 204e  f.scope is not N
-0000b0c0: 6f6e 650a 2020 2020 7620 3d20 7365 6c66  one.    v = self
-0000b0d0: 2e73 636f 7065 2e70 6172 616d 286e 616d  .scope.param(nam
-0000b0e0: 652c 2069 6e69 745f 666e 2c20 2a69 6e69  e, init_fn, *ini
-0000b0f0: 745f 6172 6773 2c20 756e 626f 783d 756e  t_args, unbox=un
-0000b100: 626f 7829 0a20 2020 2073 656c 662e 5f73  box).    self._s
-0000b110: 7461 7465 2e63 6869 6c64 7265 6e5b 6e61  tate.children[na
-0000b120: 6d65 5d20 3d20 2770 6172 616d 7327 0a20  me] = 'params'. 
-0000b130: 2020 2072 6574 7572 6e20 760a 0a20 2064     return v..  d
-0000b140: 6566 2068 6173 5f76 6172 6961 626c 6528  ef has_variable(
-0000b150: 7365 6c66 2c20 636f 6c3a 2073 7472 2c20  self, col: str, 
-0000b160: 6e61 6d65 3a20 7374 7229 202d 3e20 626f  name: str) -> bo
-0000b170: 6f6c 3a0a 2020 2020 2222 2243 6865 636b  ol:.    """Check
-0000b180: 7320 6966 2061 2076 6172 6961 626c 6520  s if a variable 
-0000b190: 6f66 2067 6976 656e 2063 6f6c 6c65 6374  of given collect
-0000b1a0: 696f 6e20 616e 6420 6e61 6d65 2065 7869  ion and name exi
-0000b1b0: 7374 7320 696e 2074 6869 7320 4d6f 6475  sts in this Modu
-0000b1c0: 6c65 2e0a 0a20 2020 2053 6565 203a 6d6f  le...    See :mo
-0000b1d0: 643a 6066 6c61 782e 636f 7265 2e76 6172  d:`flax.core.var
-0000b1e0: 6961 626c 6573 6020 666f 7220 6d6f 7265  iables` for more
-0000b1f0: 2065 7870 6c61 6e61 7469 6f6e 206f 6e20   explanation on 
-0000b200: 7661 7269 6162 6c65 7320 616e 640a 2020  variables and.  
-0000b210: 2020 636f 6c6c 6563 7469 6f6e 732e 0a0a    collections...
-0000b220: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000b230: 636f 6c3a 2054 6865 2076 6172 6961 626c  col: The variabl
-0000b240: 6520 636f 6c6c 6563 7469 6f6e 206e 616d  e collection nam
-0000b250: 652e 0a20 2020 2020 206e 616d 653a 2054  e..      name: T
-0000b260: 6865 206e 616d 6520 6f66 2074 6865 2076  he name of the v
-0000b270: 6172 6961 626c 652e 0a20 2020 2052 6574  ariable..    Ret
-0000b280: 7572 6e73 3a0a 2020 2020 2020 5472 7565  urns:.      True
-0000b290: 2069 6620 7468 6520 7661 7269 6162 6c65   if the variable
-0000b2a0: 2065 7869 7374 732e 0a20 2020 2022 2222   exists..    """
-0000b2b0: 0a20 2020 2069 6620 7365 6c66 2e73 636f  .    if self.sco
-0000b2c0: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
-0000b2d0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000b2e0: 6f72 2822 4361 6e27 7420 6163 6365 7373  or("Can't access
-0000b2f0: 2076 6172 6961 626c 6573 206f 6e20 756e   variables on un
-0000b300: 626f 756e 6420 6d6f 6475 6c65 7322 290a  bound modules").
-0000b310: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000b320: 7363 6f70 652e 6861 735f 7661 7269 6162  scope.has_variab
-0000b330: 6c65 2863 6f6c 2c20 6e61 6d65 290a 0a20  le(col, name).. 
-0000b340: 2064 6566 2069 735f 6d75 7461 626c 655f   def is_mutable_
-0000b350: 636f 6c6c 6563 7469 6f6e 2873 656c 662c  collection(self,
-0000b360: 2063 6f6c 3a20 7374 7229 202d 3e20 626f   col: str) -> bo
-0000b370: 6f6c 3a0a 2020 2020 2222 2252 6574 7572  ol:.    """Retur
-0000b380: 6e73 2074 7275 6520 6966 2074 6865 2063  ns true if the c
-0000b390: 6f6c 6c65 6374 696f 6e20 6063 6f6c 6020  ollection `col` 
-0000b3a0: 6973 206d 7574 6162 6c65 2e22 2222 0a20  is mutable.""". 
-0000b3b0: 2020 2069 6620 7365 6c66 2e73 636f 7065     if self.scope
-0000b3c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000b3d0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000b3e0: 2822 4361 6e27 7420 6368 6563 6b20 6d75  ("Can't check mu
-0000b3f0: 7461 6269 6c69 7479 206f 6e20 756e 626f  tability on unbo
-0000b400: 756e 6420 6d6f 6475 6c65 7322 290a 2020  und modules").  
-0000b410: 2020 7265 7475 726e 2073 656c 662e 7363    return self.sc
-0000b420: 6f70 652e 6973 5f6d 7574 6162 6c65 5f63  ope.is_mutable_c
-0000b430: 6f6c 6c65 6374 696f 6e28 636f 6c29 0a0a  ollection(col)..
-0000b440: 2020 6465 6620 6861 735f 726e 6728 7365    def has_rng(se
-0000b450: 6c66 2c20 6e61 6d65 3a20 7374 7229 202d  lf, name: str) -
-0000b460: 3e20 626f 6f6c 3a0a 2020 2020 2222 2252  > bool:.    """R
-0000b470: 6574 7572 6e73 2074 7275 6520 6966 2061  eturns true if a
-0000b480: 2050 524e 4753 6571 7565 6e63 6520 7769   PRNGSequence wi
-0000b490: 7468 206e 616d 6520 606e 616d 6560 2065  th name `name` e
-0000b4a0: 7869 7374 732e 2222 220a 2020 2020 6966  xists.""".    if
-0000b4b0: 2073 656c 662e 7363 6f70 6520 6973 204e   self.scope is N
-0000b4c0: 6f6e 653a 0a20 2020 2020 2072 6169 7365  one:.      raise
-0000b4d0: 2056 616c 7565 4572 726f 7228 2243 616e   ValueError("Can
-0000b4e0: 2774 2071 7565 7279 2066 6f72 2052 4e47  't query for RNG
-0000b4f0: 7320 6f6e 2075 6e62 6f75 6e64 206d 6f64  s on unbound mod
-0000b500: 756c 6573 2229 0a20 2020 2072 6574 7572  ules").    retur
-0000b510: 6e20 7365 6c66 2e73 636f 7065 2e68 6173  n self.scope.has
-0000b520: 5f72 6e67 286e 616d 6529 0a0a 2020 6465  _rng(name)..  de
-0000b530: 6620 6d61 6b65 5f72 6e67 2873 656c 662c  f make_rng(self,
-0000b540: 206e 616d 653a 2073 7472 2920 2d3e 2050   name: str) -> P
-0000b550: 524e 474b 6579 3a0a 2020 2020 2222 2252  RNGKey:.    """R
-0000b560: 6574 7572 6e73 2061 206e 6577 2052 4e47  eturns a new RNG
-0000b570: 206b 6579 2066 726f 6d20 6120 6769 7665   key from a give
-0000b580: 6e20 524e 4720 7365 7175 656e 6365 2066  n RNG sequence f
-0000b590: 6f72 2074 6869 7320 4d6f 6475 6c65 2e0a  or this Module..
-0000b5a0: 0a20 2020 2054 6865 206e 6577 2052 4e47  .    The new RNG
-0000b5b0: 206b 6579 2069 7320 7370 6c69 7420 6672   key is split fr
-0000b5c0: 6f6d 2074 6865 2070 7265 7669 6f75 7320  om the previous 
-0000b5d0: 6f6e 652e 2054 6875 732c 2065 7665 7279  one. Thus, every
-0000b5e0: 2063 616c 6c20 746f 0a20 2020 2060 6d61   call to.    `ma
-0000b5f0: 6b65 5f72 6e67 6020 7265 7475 726e 7320  ke_rng` returns 
-0000b600: 6120 6e65 7720 524e 4720 6b65 792c 2077  a new RNG key, w
-0000b610: 6869 6c65 2073 7469 6c6c 2067 7561 7261  hile still guara
-0000b620: 6e74 6565 696e 6720 6675 6c6c 0a20 2020  nteeing full.   
-0000b630: 2072 6570 726f 6475 6369 6269 6c69 7479   reproducibility
-0000b640: 2e0a 0a20 2020 2054 4f44 4f3a 204c 696e  ...    TODO: Lin
-0000b650: 6b20 746f 2046 6c61 7820 524e 4720 6465  k to Flax RNG de
-0000b660: 7369 676e 206e 6f74 652e 0a0a 2020 2020  sign note...    
-0000b670: 4172 6773 3a0a 2020 2020 2020 6e61 6d65  Args:.      name
-0000b680: 3a20 5468 6520 524e 4720 7365 7175 656e  : The RNG sequen
-0000b690: 6365 206e 616d 652e 0a20 2020 2052 6574  ce name..    Ret
-0000b6a0: 7572 6e73 3a0a 2020 2020 2020 5468 6520  urns:.      The 
-0000b6b0: 6e65 776c 7920 6765 6e65 7261 7465 6420  newly generated 
-0000b6c0: 524e 4720 6b65 792e 0a20 2020 2022 2222  RNG key..    """
-0000b6d0: 0a20 2020 2069 6620 7365 6c66 2e73 636f  .    if self.sco
-0000b6e0: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
-0000b6f0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000b700: 6f72 2822 4361 6e27 7420 7573 6520 524e  or("Can't use RN
-0000b710: 4773 206f 6e20 756e 626f 756e 6420 6d6f  Gs on unbound mo
-0000b720: 6475 6c65 7322 290a 2020 2020 7265 7475  dules").    retu
-0000b730: 726e 2073 656c 662e 7363 6f70 652e 6d61  rn self.scope.ma
-0000b740: 6b65 5f72 6e67 286e 616d 6529 0a0a 2020  ke_rng(name)..  
-0000b750: 6465 6620 6973 5f69 6e69 7469 616c 697a  def is_initializ
-0000b760: 696e 6728 7365 6c66 2920 2d3e 2062 6f6f  ing(self) -> boo
-0000b770: 6c3a 0a20 2020 2022 2222 5265 7475 726e  l:.    """Return
-0000b780: 7320 5472 7565 2069 6620 7275 6e6e 696e  s True if runnin
-0000b790: 6720 756e 6465 7220 7365 6c66 2e69 6e69  g under self.ini
-0000b7a0: 7428 2e2e 2e29 206f 7220 6e6e 2e69 6e69  t(...) or nn.ini
-0000b7b0: 7428 2e2e 2e29 2829 2e0a 0a20 2020 2054  t(...)()...    T
-0000b7c0: 6869 7320 6973 2061 2068 656c 7065 7220  his is a helper 
-0000b7d0: 6d65 7468 6f64 2074 6f20 6861 6e64 6c65  method to handle
-0000b7e0: 2074 6865 2063 6f6d 6d6f 6e20 6361 7365   the common case
-0000b7f0: 206f 6620 7369 6d70 6c65 2069 6e69 7469   of simple initi
-0000b800: 616c 697a 6174 696f 6e0a 2020 2020 7768  alization.    wh
-0000b810: 6572 6520 7765 2077 6973 6820 746f 2068  ere we wish to h
-0000b820: 6176 6520 7365 7475 7020 6c6f 6769 6320  ave setup logic 
-0000b830: 6f63 6375 7220 7768 656e 206f 6e6c 7920  occur when only 
-0000b840: 6361 6c6c 6564 2075 6e64 6572 0a20 2020  called under.   
-0000b850: 2060 606d 6f64 756c 652e 696e 6974 6060   ``module.init``
-0000b860: 206f 7220 6060 6e6e 2e69 6e69 7460 602e   or ``nn.init``.
-0000b870: 2020 466f 7220 6d6f 7265 2063 6f6d 706c    For more compl
-0000b880: 6963 6174 6564 206d 756c 7469 2d70 6861  icated multi-pha
-0000b890: 7365 0a20 2020 2069 6e69 7469 616c 697a  se.    initializ
-0000b8a0: 6174 696f 6e20 7363 656e 6172 696f 7320  ation scenarios 
-0000b8b0: 6974 2069 7320 6265 7474 6572 2074 6f20  it is better to 
-0000b8c0: 7465 7374 2066 6f72 2074 6865 206d 7574  test for the mut
-0000b8d0: 6162 696c 6974 7920 6f66 0a20 2020 2070  ability of.    p
-0000b8e0: 6172 7469 6375 6c61 7220 7661 7269 6162  articular variab
-0000b8f0: 6c65 2063 6f6c 6c65 6374 696f 6e73 206f  le collections o
-0000b900: 7220 666f 7220 7468 6520 7072 6573 656e  r for the presen
-0000b910: 6365 206f 6620 7061 7274 6963 756c 6172  ce of particular
-0000b920: 0a20 2020 2076 6172 6961 626c 6573 2074  .    variables t
-0000b930: 6861 7420 706f 7465 6e74 6961 6c6c 7920  hat potentially 
-0000b940: 6e65 6564 2074 6f20 6265 2069 6e69 7469  need to be initi
-0000b950: 616c 697a 6564 2e0a 2020 2020 2222 220a  alized..    """.
-0000b960: 2020 2020 6966 2073 656c 662e 7363 6f70      if self.scop
-0000b970: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-0000b980: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000b990: 7228 2243 616e 2774 2063 6865 636b 2069  r("Can't check i
-0000b9a0: 6620 7275 6e6e 696e 6720 756e 6465 7220  f running under 
-0000b9b0: 696e 6974 2829 206f 6e20 756e 626f 756e  init() on unboun
-0000b9c0: 6420 6d6f 6475 6c65 7322 290a 2020 2020  d modules").    
-0000b9d0: 7265 7475 726e 2073 656c 662e 7363 6f70  return self.scop
-0000b9e0: 652e 6765 745f 666c 6167 2827 696e 6974  e.get_flag('init
-0000b9f0: 6961 6c69 7a69 6e67 272c 2046 616c 7365  ializing', False
-0000ba00: 290a 0a20 2064 6566 205f 6d6f 6475 6c65  )..  def _module
-0000ba10: 5f63 6865 636b 7328 7365 6c66 293a 0a20  _checks(self):. 
-0000ba20: 2020 2022 2222 5275 6e20 7374 616e 6461     """Run standa
-0000ba30: 7264 2072 756e 7469 6d65 2063 6865 636b  rd runtime check
-0000ba40: 732e 2222 220a 0a20 2020 2069 6620 6e6f  s."""..    if no
-0000ba50: 7420 6973 696e 7374 616e 6365 2873 656c  t isinstance(sel
-0000ba60: 662c 204d 6f64 756c 6529 3a0a 2020 2020  f, Module):.    
-0000ba70: 2020 7261 6973 6520 6572 726f 7273 2e49    raise errors.I
-0000ba80: 6e76 616c 6964 496e 7374 616e 6365 4d6f  nvalidInstanceMo
-0000ba90: 6475 6c65 4572 726f 7228 290a 0a20 2020  duleError()..   
-0000baa0: 206f 7665 7272 6964 6465 6e5f 706f 7374   overridden_post
-0000bab0: 5f69 6e69 7420 3d20 7365 6c66 2e5f 5f70  _init = self.__p
-0000bac0: 6f73 745f 696e 6974 5f5f 2021 3d20 4d6f  ost_init__ != Mo
-0000bad0: 6475 6c65 2e5f 5f70 6f73 745f 696e 6974  dule.__post_init
-0000bae0: 5f5f 0a20 2020 2069 6620 6f76 6572 7269  __.    if overri
-0000baf0: 6464 656e 5f70 6f73 745f 696e 6974 2061  dden_post_init a
-0000bb00: 6e64 206e 6f74 2068 6173 6174 7472 2873  nd not hasattr(s
-0000bb10: 656c 662c 2022 5f69 6422 293a 0a20 2020  elf, "_id"):.   
-0000bb20: 2020 2072 6169 7365 2065 7272 6f72 732e     raise errors.
-0000bb30: 496e 636f 7272 6563 7450 6f73 7449 6e69  IncorrectPostIni
-0000bb40: 744f 7665 7272 6964 6545 7272 6f72 2829  tOverrideError()
-0000bb50: 0a0a 2020 4074 7261 6365 6261 636b 5f75  ..  @traceback_u
-0000bb60: 7469 6c2e 6170 695f 626f 756e 6461 7279  til.api_boundary
-0000bb70: 0a20 2064 6566 2062 696e 6428 7365 6c66  .  def bind(self
-0000bb80: 3a20 4d2c 0a20 2020 2020 2020 2020 2020  : M,.           
-0000bb90: 7661 7269 6162 6c65 733a 2056 6172 6961  variables: Varia
-0000bba0: 626c 6544 6963 742c 0a20 2020 2020 2020  bleDict,.       
-0000bbb0: 2020 2020 2a61 7267 732c 0a20 2020 2020      *args,.     
-0000bbc0: 2020 2020 2020 726e 6773 3a20 4f70 7469        rngs: Opti
-0000bbd0: 6f6e 616c 5b52 4e47 5365 7175 656e 6365  onal[RNGSequence
-0000bbe0: 735d 203d 204e 6f6e 652c 0a20 2020 2020  s] = None,.     
-0000bbf0: 2020 2020 2020 6d75 7461 626c 653a 2043        mutable: C
-0000bc00: 6f6c 6c65 6374 696f 6e46 696c 7465 7220  ollectionFilter 
-0000bc10: 3d20 4661 6c73 6529 202d 3e20 4d3a 0a20  = False) -> M:. 
-0000bc20: 2020 2022 2222 4372 6561 7465 7320 616e     """Creates an
-0000bc30: 2069 6e74 6572 6163 7469 7665 204d 6f64   interactive Mod
-0000bc40: 756c 6520 696e 7374 616e 6365 2062 7920  ule instance by 
-0000bc50: 6269 6e64 696e 6720 7661 7269 6162 6c65  binding variable
-0000bc60: 7320 616e 6420 524e 4773 2e0a 0a20 2020  s and RNGs...   
-0000bc70: 2060 6062 696e 6460 6020 7072 6f76 6964   ``bind`` provid
-0000bc80: 6573 2061 6e20 2269 6e74 6572 6163 7469  es an "interacti
-0000bc90: 7665 2220 696e 7374 616e 6365 206f 6620  ve" instance of 
-0000bca0: 6120 4d6f 6475 6c65 2064 6972 6563 746c  a Module directl
-0000bcb0: 7920 7769 7468 6f75 740a 2020 2020 7472  y without.    tr
-0000bcc0: 616e 7366 6f72 6d69 6e67 2061 2066 756e  ansforming a fun
-0000bcd0: 6374 696f 6e20 7769 7468 2060 6061 7070  ction with ``app
-0000bce0: 6c79 6060 2e20 5468 6973 2069 7320 7061  ly``. This is pa
-0000bcf0: 7274 6963 756c 6172 6c79 2075 7365 6675  rticularly usefu
-0000bd00: 6c20 666f 720a 2020 2020 6465 6275 6767  l for.    debugg
-0000bd10: 696e 6720 7a61 6e64 2069 6e74 6572 6163  ing zand interac
-0000bd20: 7469 7665 2075 7365 2063 6173 6573 206c  tive use cases l
-0000bd30: 696b 6520 6e6f 7465 626f 6f6b 7320 7768  ike notebooks wh
-0000bd40: 6572 6520 6120 6675 6e63 7469 6f6e 2077  ere a function w
-0000bd50: 6f75 6c64 0a20 2020 206c 696d 6974 2074  ould.    limit t
-0000bd60: 6865 2061 6269 6c69 7479 2074 6f20 7370  he ability to sp
-0000bd70: 6c69 7420 7570 2063 6f64 6520 696e 746f  lit up code into
-0000bd80: 2064 6966 6665 7265 6e74 2063 656c 6c73   different cells
-0000bd90: 2e0a 0a20 2020 204f 6e63 6520 7468 6520  ...    Once the 
-0000bda0: 7661 7269 6162 6c65 7320 2861 6e64 206f  variables (and o
-0000bdb0: 7074 696f 6e61 6c6c 7920 524e 4773 2920  ptionally RNGs) 
-0000bdc0: 6172 6520 626f 756e 6420 746f 2061 2060  are bound to a `
-0000bdd0: 604d 6f64 756c 6560 6020 6974 0a20 2020  `Module`` it.   
-0000bde0: 2062 6563 6f6d 6573 2061 2073 7461 7465   becomes a state
-0000bdf0: 6675 6c20 6f62 6a65 6374 2e20 4e6f 7465  ful object. Note
-0000be00: 2074 6861 7420 6964 696f 6d61 7469 6320   that idiomatic 
-0000be10: 4a41 5820 6973 2066 756e 6374 696f 6e61  JAX is functiona
-0000be20: 6c20 616e 640a 2020 2020 7468 6572 6566  l and.    theref
-0000be30: 6f72 6520 616e 2069 6e74 6572 6163 7469  ore an interacti
-0000be40: 7665 2069 6e73 7461 6e63 6520 646f 6573  ve instance does
-0000be50: 206e 6f74 206d 6978 2077 656c 6c20 7769   not mix well wi
-0000be60: 7468 2076 616e 696c 6c61 204a 4158 2041  th vanilla JAX A
-0000be70: 5049 732e 0a20 2020 2060 6062 696e 6428  PIs..    ``bind(
-0000be80: 2960 6020 7368 6f75 6c64 206f 6e6c 7920  )`` should only 
-0000be90: 6265 2075 7365 6420 666f 7220 696e 7465  be used for inte
-0000bea0: 7261 6374 6976 6520 6578 7065 7269 6d65  ractive experime
-0000beb0: 6e74 6174 696f 6e2c 2061 6e64 2069 6e20  ntation, and in 
-0000bec0: 616c 6c0a 2020 2020 6f74 6865 7220 6361  all.    other ca
-0000bed0: 7365 7320 7765 2073 7472 6f6e 676c 7920  ses we strongly 
-0000bee0: 656e 636f 7572 6167 6520 7573 6572 7320  encourage users 
-0000bef0: 746f 2075 7365 2060 6061 7070 6c79 2829  to use ``apply()
-0000bf00: 6060 2069 6e73 7465 6164 2e0a 0a20 2020  `` instead...   
-0000bf10: 2045 7861 6d70 6c65 3a3a 0a0a 2020 2020   Example::..    
-0000bf20: 2020 696d 706f 7274 206a 6178 0a20 2020    import jax.   
-0000bf30: 2020 2069 6d70 6f72 7420 6a61 782e 6e75     import jax.nu
-0000bf40: 6d70 7920 6173 206a 6e70 0a20 2020 2020  mpy as jnp.     
-0000bf50: 2069 6d70 6f72 7420 666c 6178 2e6c 696e   import flax.lin
-0000bf60: 656e 2061 7320 6e6e 0a0a 2020 2020 2020  en as nn..      
-0000bf70: 636c 6173 7320 4175 746f 456e 636f 6465  class AutoEncode
-0000bf80: 7228 6e6e 2e4d 6f64 756c 6529 3a0a 2020  r(nn.Module):.  
-0000bf90: 2020 2020 2020 6465 6620 7365 7475 7028        def setup(
-0000bfa0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-0000bfb0: 2073 656c 662e 656e 636f 6465 7220 3d20   self.encoder = 
-0000bfc0: 6e6e 2e44 656e 7365 2833 290a 2020 2020  nn.Dense(3).    
-0000bfd0: 2020 2020 2020 7365 6c66 2e64 6563 6f64        self.decod
-0000bfe0: 6572 203d 206e 6e2e 4465 6e73 6528 3529  er = nn.Dense(5)
-0000bff0: 0a0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
-0000c000: 6361 6c6c 5f5f 2873 656c 662c 2078 293a  call__(self, x):
-0000c010: 0a20 2020 2020 2020 2020 2072 6574 7572  .          retur
-0000c020: 6e20 7365 6c66 2e64 6563 6f64 6572 2873  n self.decoder(s
-0000c030: 656c 662e 656e 636f 6465 7228 7829 290a  elf.encoder(x)).
-0000c040: 0a20 2020 2020 2078 203d 206a 6e70 2e6f  .      x = jnp.o
-0000c050: 6e65 7328 2831 362c 2039 2929 0a20 2020  nes((16, 9)).   
-0000c060: 2020 2061 6520 3d20 4175 746f 456e 636f     ae = AutoEnco
-0000c070: 6465 7228 290a 2020 2020 2020 7661 7269  der().      vari
-0000c080: 6162 6c65 7320 3d20 6165 2e69 6e69 7428  ables = ae.init(
-0000c090: 6a61 782e 7261 6e64 6f6d 2e50 524e 474b  jax.random.PRNGK
-0000c0a0: 6579 2830 292c 2078 290a 2020 2020 2020  ey(0), x).      
-0000c0b0: 6d6f 6465 6c20 3d20 6165 2e62 696e 6428  model = ae.bind(
-0000c0c0: 7661 7269 6162 6c65 7329 0a20 2020 2020  variables).     
-0000c0d0: 207a 203d 206d 6f64 656c 2e65 6e63 6f64   z = model.encod
-0000c0e0: 6572 2878 290a 2020 2020 2020 785f 7265  er(x).      x_re
-0000c0f0: 636f 6e73 7472 7563 7465 6420 3d20 6d6f  constructed = mo
-0000c100: 6465 6c2e 6465 636f 6465 7228 7a29 0a0a  del.decoder(z)..
-0000c110: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000c120: 7661 7269 6162 6c65 733a 2041 2064 6963  variables: A dic
-0000c130: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-0000c140: 6e67 2076 6172 6961 626c 6573 206b 6579  ng variables key
-0000c150: 6564 2062 7920 7661 7269 6162 6c65 0a20  ed by variable. 
-0000c160: 2020 2020 2020 2063 6f6c 6c65 6374 696f         collectio
-0000c170: 6e73 2e20 5365 6520 3a6d 6f64 3a60 666c  ns. See :mod:`fl
-0000c180: 6178 2e63 6f72 652e 7661 7269 6162 6c65  ax.core.variable
-0000c190: 7360 2066 6f72 206d 6f72 6520 6465 7461  s` for more deta
-0000c1a0: 696c 730a 2020 2020 2020 2020 6162 6f75  ils.        abou
-0000c1b0: 7420 7661 7269 6162 6c65 732e 0a20 2020  t variables..   
-0000c1c0: 2020 202a 6172 6773 3a20 4e61 6d65 6420     *args: Named 
-0000c1d0: 6172 6775 6d65 6e74 7320 286e 6f74 2075  arguments (not u
-0000c1e0: 7365 6429 2e0a 2020 2020 2020 726e 6773  sed)..      rngs
-0000c1f0: 3a20 6120 6469 6374 206f 6620 5052 4e47  : a dict of PRNG
-0000c200: 4b65 7973 2074 6f20 696e 6974 6961 6c69  Keys to initiali
-0000c210: 7a65 2074 6865 2050 524e 4720 7365 7175  ze the PRNG sequ
-0000c220: 656e 6365 732e 0a20 2020 2020 206d 7574  ences..      mut
-0000c230: 6162 6c65 3a20 4361 6e20 6265 2062 6f6f  able: Can be boo
-0000c240: 6c2c 2073 7472 2c20 6f72 206c 6973 742e  l, str, or list.
-0000c250: 2053 7065 6369 6669 6573 2077 6869 6368   Specifies which
-0000c260: 2063 6f6c 6c65 6374 696f 6e73 2073 686f   collections sho
-0000c270: 756c 6420 6265 0a20 2020 2020 2020 2074  uld be.        t
-0000c280: 7265 6174 6564 2061 7320 6d75 7461 626c  reated as mutabl
-0000c290: 653a 0a20 2020 2020 2020 2020 2060 6062  e:.          ``b
-0000c2a0: 6f6f 6c60 603a 2061 6c6c 2f6e 6f20 636f  ool``: all/no co
-0000c2b0: 6c6c 6563 7469 6f6e 7320 6172 6520 6d75  llections are mu
-0000c2c0: 7461 626c 652e 0a20 2020 2020 2020 2020  table..         
-0000c2d0: 2060 6073 7472 6060 3a20 5468 6520 6e61   ``str``: The na
-0000c2e0: 6d65 206f 6620 6120 7369 6e67 6c65 206d  me of a single m
-0000c2f0: 7574 6162 6c65 2063 6f6c 6c65 6374 696f  utable collectio
-0000c300: 6e2e 0a20 2020 2020 2020 2020 2060 606c  n..          ``l
-0000c310: 6973 7460 603a 2041 206c 6973 7420 6f66  ist``: A list of
-0000c320: 206e 616d 6573 206f 6620 6d75 7461 626c   names of mutabl
-0000c330: 6520 636f 6c6c 6563 7469 6f6e 732e 0a0a  e collections...
-0000c340: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000c350: 2020 2041 2063 6f70 7920 6f66 2074 6869     A copy of thi
-0000c360: 7320 696e 7374 616e 6365 2077 6974 6820  s instance with 
-0000c370: 626f 756e 6420 7661 7269 6162 6c65 7320  bound variables 
-0000c380: 616e 6420 524e 4773 2e0a 2020 2020 2222  and RNGs..    ""
-0000c390: 220a 2020 2020 4d6f 6475 6c65 2e5f 6d6f  ".    Module._mo
-0000c3a0: 6475 6c65 5f63 6865 636b 7328 7365 6c66  dule_checks(self
-0000c3b0: 290a 0a20 2020 2064 656c 2061 7267 730a  )..    del args.
-0000c3c0: 2020 2020 7363 6f70 6520 3d20 636f 7265      scope = core
-0000c3d0: 2e62 696e 6428 7661 7269 6162 6c65 732c  .bind(variables,
-0000c3e0: 2072 6e67 733d 726e 6773 2c20 6d75 7461   rngs=rngs, muta
-0000c3f0: 626c 653d 6d75 7461 626c 6529 0a20 2020  ble=mutable).   
-0000c400: 2072 6574 7572 6e20 7365 6c66 2e63 6c6f   return self.clo
-0000c410: 6e65 2870 6172 656e 743d 7363 6f70 6529  ne(parent=scope)
-0000c420: 0a0a 2020 6465 6620 756e 6269 6e64 2873  ..  def unbind(s
-0000c430: 656c 663a 204d 2920 2d3e 2054 7570 6c65  elf: M) -> Tuple
-0000c440: 5b4d 2c20 5661 7269 6162 6c65 4469 6374  [M, VariableDict
-0000c450: 5d3a 0a20 2020 2022 2222 5265 7475 726e  ]:.    """Return
-0000c460: 7320 616e 2075 6e62 6f75 6e64 2063 6f70  s an unbound cop
-0000c470: 7920 6f66 2061 204d 6f64 756c 6520 616e  y of a Module an
-0000c480: 6420 6974 7320 7661 7269 6162 6c65 732e  d its variables.
-0000c490: 0a0a 2020 2020 6060 756e 6269 6e64 6060  ..    ``unbind``
-0000c4a0: 2068 656c 7073 2063 7265 6174 6520 6120   helps create a 
-0000c4b0: 7374 6174 656c 6573 7320 7665 7273 696f  stateless versio
-0000c4c0: 6e20 6f66 2061 2062 6f75 6e64 204d 6f64  n of a bound Mod
-0000c4d0: 756c 652e 0a0a 2020 2020 416e 2065 7861  ule...    An exa
-0000c4e0: 6d70 6c65 206f 6620 6120 636f 6d6d 6f6e  mple of a common
-0000c4f0: 2075 7365 2063 6173 653a 2074 6f20 6578   use case: to ex
-0000c500: 7472 6163 7420 6120 7375 622d 4d6f 6475  tract a sub-Modu
-0000c510: 6c65 2064 6566 696e 6564 2069 6e73 6964  le defined insid
-0000c520: 650a 2020 2020 6060 7365 7475 7028 2960  e.    ``setup()`
-0000c530: 6020 616e 6420 6974 7320 636f 7272 6573  ` and its corres
-0000c540: 706f 6e64 696e 6720 7661 7269 6162 6c65  ponding variable
-0000c550: 733a 2031 2920 7465 6d70 6f72 6172 696c  s: 1) temporaril
-0000c560: 7920 6060 6269 6e64 6060 2074 6865 2070  y ``bind`` the p
-0000c570: 6172 656e 740a 2020 2020 4d6f 6475 6c65  arent.    Module
-0000c580: 3b20 616e 6420 7468 656e 2032 2920 6060  ; and then 2) ``
-0000c590: 756e 6269 6e64 6060 2074 6865 2064 6573  unbind`` the des
-0000c5a0: 6972 6564 2073 7562 2d4d 6f64 756c 652e  ired sub-Module.
-0000c5b0: 2028 5265 6361 6c6c 2074 6861 7420 6060   (Recall that ``
-0000c5c0: 7365 7475 7028 2960 600a 2020 2020 6973  setup()``.    is
-0000c5d0: 206f 6e6c 7920 6361 6c6c 6564 2077 6865   only called whe
-0000c5e0: 6e20 7468 6520 4d6f 6475 6c65 2069 7320  n the Module is 
-0000c5f0: 626f 756e 642e 293a 3a0a 0a20 2020 2020  bound.)::..     
-0000c600: 2063 6c61 7373 2041 7574 6f45 6e63 6f64   class AutoEncod
-0000c610: 6572 286e 6e2e 4d6f 6475 6c65 293a 0a20  er(nn.Module):. 
-0000c620: 2020 2020 2020 2064 6566 2073 6574 7570         def setup
-0000c630: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000c640: 2020 7365 6c66 2e65 6e63 6f64 6572 203d    self.encoder =
-0000c650: 2045 6e63 6f64 6572 2829 0a20 2020 2020   Encoder().     
-0000c660: 2020 2020 2073 656c 662e 6465 636f 6465       self.decode
-0000c670: 7220 3d20 4465 636f 6465 7228 290a 0a20  r = Decoder().. 
-0000c680: 2020 2020 2020 2064 6566 205f 5f63 616c         def __cal
-0000c690: 6c5f 5f28 7365 6c66 2c20 7829 3a0a 2020  l__(self, x):.  
-0000c6a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000c6b0: 656c 662e 6465 636f 6465 7228 7365 6c66  elf.decoder(self
-0000c6c0: 2e65 6e63 6f64 6572 2878 2929 0a0a 2020  .encoder(x))..  
-0000c6d0: 2020 2020 6d6f 6475 6c65 203d 2041 7574      module = Aut
-0000c6e0: 6f45 6e63 6f64 6572 2829 0a20 2020 2020  oEncoder().     
-0000c6f0: 2076 6172 6961 626c 6573 203d 206d 6f64   variables = mod
-0000c700: 756c 652e 696e 6974 286a 6178 2e72 616e  ule.init(jax.ran
-0000c710: 646f 6d2e 5052 4e47 4b65 7928 3029 2c20  dom.PRNGKey(0), 
-0000c720: 6a6e 702e 6f6e 6573 2828 312c 2037 3834  jnp.ones((1, 784
-0000c730: 2929 290a 2020 2020 2020 2e2e 2e0a 2020  ))).      ....  
-0000c740: 2020 2020 2320 4578 7472 6163 7420 7468      # Extract th
-0000c750: 6520 456e 636f 6465 7220 7375 622d 4d6f  e Encoder sub-Mo
-0000c760: 6475 6c65 2061 6e64 2069 7473 2076 6172  dule and its var
-0000c770: 6961 626c 6573 0a20 2020 2020 2065 6e63  iables.      enc
-0000c780: 6f64 6572 2c20 656e 636f 6465 725f 7661  oder, encoder_va
-0000c790: 7273 203d 206d 6f64 756c 652e 6269 6e64  rs = module.bind
-0000c7a0: 2876 6172 6961 626c 6573 292e 656e 636f  (variables).enco
-0000c7b0: 6465 722e 756e 6269 6e64 2829 0a0a 2020  der.unbind()..  
-0000c7c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000c7d0: 2041 2074 7570 6c65 2077 6974 6820 616e   A tuple with an
-0000c7e0: 2075 6e62 6f75 6e64 2063 6f70 7920 6f66   unbound copy of
-0000c7f0: 2074 6869 7320 4d6f 6475 6c65 2061 6e64   this Module and
-0000c800: 2069 7473 2076 6172 6961 626c 6573 2e0a   its variables..
-0000c810: 2020 2020 2222 220a 2020 2020 4d6f 6475      """.    Modu
-0000c820: 6c65 2e5f 6d6f 6475 6c65 5f63 6865 636b  le._module_check
-0000c830: 7328 7365 6c66 290a 0a20 2020 2069 6620  s(self)..    if 
-0000c840: 7365 6c66 2e73 636f 7065 2069 7320 4e6f  self.scope is No
-0000c850: 6e65 3a0a 2020 2020 2020 7261 6973 6520  ne:.      raise 
-0000c860: 6572 726f 7273 2e43 616c 6c55 6e62 696e  errors.CallUnbin
-0000c870: 644f 6e55 6e62 6f75 6e64 4d6f 6475 6c65  dOnUnboundModule
-0000c880: 4572 726f 7228 290a 0a20 2020 2076 6172  Error()..    var
-0000c890: 6961 626c 6573 203d 2073 656c 662e 7661  iables = self.va
-0000c8a0: 7269 6162 6c65 730a 2020 2020 6d6f 6475  riables.    modu
-0000c8b0: 6c65 203d 2073 656c 662e 636c 6f6e 6528  le = self.clone(
-0000c8c0: 290a 2020 2020 7265 7475 726e 206d 6f64  ).    return mod
-0000c8d0: 756c 652c 2076 6172 6961 626c 6573 0a0a  ule, variables..
-0000c8e0: 2020 4074 7261 6365 6261 636b 5f75 7469    @traceback_uti
-0000c8f0: 6c2e 6170 695f 626f 756e 6461 7279 0a20  l.api_boundary. 
-0000c900: 2064 6566 2061 7070 6c79 2873 656c 662c   def apply(self,
-0000c910: 0a20 2020 2020 2020 2020 2020 2076 6172  .            var
-0000c920: 6961 626c 6573 3a20 5661 7269 6162 6c65  iables: Variable
-0000c930: 4469 6374 2c0a 2020 2020 2020 2020 2020  Dict,.          
-0000c940: 2020 2a61 7267 732c 0a20 2020 2020 2020    *args,.       
-0000c950: 2020 2020 2072 6e67 733a 204f 7074 696f       rngs: Optio
-0000c960: 6e61 6c5b 524e 4753 6571 7565 6e63 6573  nal[RNGSequences
-0000c970: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000c980: 2020 2020 2020 6d65 7468 6f64 3a20 556e        method: Un
-0000c990: 696f 6e5b 4361 6c6c 6162 6c65 5b2e 2e2e  ion[Callable[...
-0000c9a0: 2c20 416e 795d 2c20 7374 722c 204e 6f6e  , Any], str, Non
-0000c9b0: 655d 203d 204e 6f6e 652c 0a20 2020 2020  e] = None,.     
-0000c9c0: 2020 2020 2020 206d 7574 6162 6c65 3a20         mutable: 
-0000c9d0: 436f 6c6c 6563 7469 6f6e 4669 6c74 6572  CollectionFilter
-0000c9e0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-0000c9f0: 2020 2020 2020 6361 7074 7572 655f 696e        capture_in
-0000ca00: 7465 726d 6564 6961 7465 733a 2055 6e69  termediates: Uni
-0000ca10: 6f6e 5b62 6f6f 6c2c 2043 616c 6c61 626c  on[bool, Callabl
-0000ca20: 655b 5b27 4d6f 6475 6c65 272c 2073 7472  e[['Module', str
-0000ca30: 5d2c 2062 6f6f 6c5d 5d20 3d20 4661 6c73  ], bool]] = Fals
-0000ca40: 652c 0a20 2020 2020 2020 2020 2020 202a  e,.            *
-0000ca50: 2a6b 7761 7267 7329 202d 3e20 556e 696f  *kwargs) -> Unio
-0000ca60: 6e5b 416e 792c 2054 7570 6c65 5b41 6e79  n[Any, Tuple[Any
-0000ca70: 2c20 556e 696f 6e5b 4672 6f7a 656e 5661  , Union[FrozenVa
-0000ca80: 7269 6162 6c65 4469 6374 2c20 4469 6374  riableDict, Dict
-0000ca90: 5b73 7472 2c20 416e 795d 5d5d 5d3a 0a20  [str, Any]]]]:. 
-0000caa0: 2020 2022 2222 4170 706c 6965 7320 6120     """Applies a 
-0000cab0: 6d6f 6475 6c65 206d 6574 686f 6420 746f  module method to
-0000cac0: 2076 6172 6961 626c 6573 2061 6e64 2072   variables and r
-0000cad0: 6574 7572 6e73 206f 7574 7075 7420 616e  eturns output an
-0000cae0: 6420 6d6f 6469 6669 6564 2076 6172 6961  d modified varia
-0000caf0: 626c 6573 2e0a 0a20 2020 204e 6f74 6520  bles...    Note 
-0000cb00: 7468 6174 2060 6d65 7468 6f64 6020 7368  that `method` sh
-0000cb10: 6f75 6c64 2062 6520 7365 7420 6966 206f  ould be set if o
-0000cb20: 6e65 2077 6f75 6c64 206c 696b 6520 746f  ne would like to
-0000cb30: 2063 616c 6c20 6061 7070 6c79 6020 6f6e   call `apply` on
-0000cb40: 2061 0a20 2020 2064 6966 6665 7265 6e74   a.    different
-0000cb50: 2063 6c61 7373 206d 6574 686f 6420 7468   class method th
-0000cb60: 616e 2060 605f 5f63 616c 6c5f 5f60 602e  an ``__call__``.
-0000cb70: 2046 6f72 2069 6e73 7461 6e63 652c 2073   For instance, s
-0000cb80: 7570 706f 7365 2061 0a20 2020 2054 7261  uppose a.    Tra
-0000cb90: 6e73 666f 726d 6572 206d 6f64 756c 6573  nsformer modules
-0000cba0: 2068 6173 2061 206d 6574 686f 6420 6361   has a method ca
-0000cbb0: 6c6c 6564 2060 656e 636f 6465 602c 2074  lled `encode`, t
-0000cbc0: 6865 6e20 7468 6520 666f 6c6c 6f77 696e  hen the followin
-0000cbd0: 6720 6361 6c6c 730a 2020 2020 6061 7070  g calls.    `app
-0000cbe0: 6c79 6020 6f6e 2074 6861 7420 6d65 7468  ly` on that meth
-0000cbf0: 6f64 3a3a 0a0a 2020 2020 2020 6d6f 6465  od::..      mode
-0000cc00: 6c20 3d20 5472 616e 7366 6f72 6d65 7228  l = Transformer(
-0000cc10: 290a 2020 2020 2020 656e 636f 6465 6420  ).      encoded 
-0000cc20: 3d20 6d6f 6465 6c2e 6170 706c 7928 7b27  = model.apply({'
-0000cc30: 7061 7261 6d73 273a 2070 6172 616d 737d  params': params}
-0000cc40: 2c20 782c 206d 6574 686f 643d 5472 616e  , x, method=Tran
-0000cc50: 7366 6f72 6d65 722e 656e 636f 6465 290a  sformer.encode).
-0000cc60: 0a20 2020 2049 6620 6120 6675 6e63 7469  .    If a functi
-0000cc70: 6f6e 2069 6e73 7461 6e63 6520 6973 2070  on instance is p
-0000cc80: 726f 7669 6465 642c 2074 6865 2075 6e62  rovided, the unb
-0000cc90: 6f75 6e64 2066 756e 6374 696f 6e20 6973  ound function is
-0000cca0: 2075 7365 642e 2046 6f72 0a20 2020 2069   used. For.    i
-0000ccb0: 6e73 7461 6e63 652c 2074 6865 2065 7861  nstance, the exa
-0000ccc0: 6d70 6c65 2062 656c 6f77 2069 7320 6571  mple below is eq
-0000ccd0: 7569 7661 6c65 6e74 2074 6f20 7468 6520  uivalent to the 
-0000cce0: 6f6e 6520 6162 6f76 653a 3a0a 0a20 2020  one above::..   
-0000ccf0: 2020 2065 6e63 6f64 6564 203d 206d 6f64     encoded = mod
-0000cd00: 656c 2e61 7070 6c79 287b 2770 6172 616d  el.apply({'param
-0000cd10: 7327 3a20 7061 7261 6d73 7d2c 2078 2c20  s': params}, x, 
-0000cd20: 6d65 7468 6f64 3d6d 6f64 656c 2e65 6e63  method=model.enc
-0000cd30: 6f64 6529 0a0a 2020 2020 596f 7520 6361  ode)..    You ca
-0000cd40: 6e20 616c 736f 2070 6173 7320 6120 7374  n also pass a st
-0000cd50: 7269 6e67 2074 6f20 6120 6361 6c6c 6162  ring to a callab
-0000cd60: 6c65 2061 7474 7269 6275 7465 206f 6620  le attribute of 
-0000cd70: 7468 6520 6d6f 6475 6c65 2e20 466f 720a  the module. For.
-0000cd80: 2020 2020 6578 616d 706c 652c 2074 6865      example, the
-0000cd90: 2070 7265 7669 6f75 7320 6361 6e20 6265   previous can be
-0000cda0: 2077 7269 7474 656e 2061 733a 3a0a 0a20   written as::.. 
-0000cdb0: 2020 2020 2065 6e63 6f64 6564 203d 206d       encoded = m
-0000cdc0: 6f64 656c 2e61 7070 6c79 287b 2770 6172  odel.apply({'par
-0000cdd0: 616d 7327 3a20 7061 7261 6d73 7d2c 2078  ams': params}, x
-0000cde0: 2c20 6d65 7468 6f64 3d27 656e 636f 6465  , method='encode
-0000cdf0: 2729 0a0a 2020 2020 4e6f 7465 2060 606d  ')..    Note ``m
-0000ce00: 6574 686f 6460 6020 6361 6e20 616c 736f  ethod`` can also
-0000ce10: 2062 6520 6120 6675 6e63 7469 6f6e 2074   be a function t
-0000ce20: 6861 7420 6973 206e 6f74 2064 6566 696e  hat is not defin
-0000ce30: 6564 2069 6e0a 2020 2020 6060 5472 616e  ed in.    ``Tran
-0000ce40: 7366 6f72 6d65 7260 602e 2049 6e20 7468  sformer``. In th
-0000ce50: 6174 2063 6173 652c 2074 6865 2066 756e  at case, the fun
-0000ce60: 6374 696f 6e20 7368 6f75 6c64 2068 6176  ction should hav
-0000ce70: 6520 6174 206c 6561 7374 206f 6e65 0a20  e at least one. 
-0000ce80: 2020 2061 7267 756d 656e 7420 7265 7072     argument repr
-0000ce90: 6573 656e 7469 6e67 2061 6e20 696e 7374  esenting an inst
-0000cea0: 616e 6365 206f 6620 7468 6520 4d6f 6475  ance of the Modu
-0000ceb0: 6c65 2063 6c61 7373 3a3a 0a0a 2020 2020  le class::..    
-0000cec0: 2020 6465 6620 6f74 6865 725f 666e 2869    def other_fn(i
-0000ced0: 6e73 7461 6e63 652c 202e 2e2e 293a 0a20  nstance, ...):. 
-0000cee0: 2020 2020 2020 2069 6e73 7461 6e63 652e         instance.
-0000cef0: 736f 6d65 5f6d 6f64 756c 655f 6174 7472  some_module_attr
-0000cf00: 282e 2e2e 290a 2020 2020 2020 2020 2e2e  (...).        ..
-0000cf10: 2e0a 0a20 2020 2020 206d 6f64 656c 2e61  ...      model.a
-0000cf20: 7070 6c79 287b 2770 6172 616d 7327 3a20  pply({'params': 
-0000cf30: 7061 7261 6d73 7d2c 2078 2c20 6d65 7468  params}, x, meth
-0000cf40: 6f64 3d6f 7468 6572 5f66 6e29 0a0a 2020  od=other_fn)..  
-0000cf50: 2020 4172 6773 3a0a 2020 2020 2020 7661    Args:.      va
-0000cf60: 7269 6162 6c65 733a 2041 2064 6963 7469  riables: A dicti
-0000cf70: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
-0000cf80: 2076 6172 6961 626c 6573 206b 6579 6564   variables keyed
-0000cf90: 2062 7920 7661 7269 6162 6c65 0a20 2020   by variable.   
-0000cfa0: 2020 2020 2063 6f6c 6c65 6374 696f 6e73       collections
-0000cfb0: 2e20 5365 6520 3a6d 6f64 3a60 666c 6178  . See :mod:`flax
-0000cfc0: 2e63 6f72 652e 7661 7269 6162 6c65 7360  .core.variables`
-0000cfd0: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
-0000cfe0: 730a 2020 2020 2020 2020 6162 6f75 7420  s.        about 
-0000cff0: 7661 7269 6162 6c65 732e 0a20 2020 2020  variables..     
-0000d000: 202a 6172 6773 3a20 4e61 6d65 6420 6172   *args: Named ar
-0000d010: 6775 6d65 6e74 7320 7061 7373 6564 2074  guments passed t
-0000d020: 6f20 7468 6520 7370 6563 6966 6965 6420  o the specified 
-0000d030: 6170 706c 7920 6d65 7468 6f64 2e0a 2020  apply method..  
-0000d040: 2020 2020 726e 6773 3a20 6120 6469 6374      rngs: a dict
-0000d050: 206f 6620 5052 4e47 4b65 7973 2074 6f20   of PRNGKeys to 
-0000d060: 696e 6974 6961 6c69 7a65 2074 6865 2050  initialize the P
-0000d070: 524e 4720 7365 7175 656e 6365 732e 0a20  RNG sequences.. 
-0000d080: 2020 2020 2020 2054 6865 2022 7061 7261         The "para
-0000d090: 6d73 2220 5052 4e47 2073 6571 7565 6e63  ms" PRNG sequenc
-0000d0a0: 6520 6973 2075 7365 6420 746f 2069 6e69  e is used to ini
-0000d0b0: 7469 616c 697a 6520 7061 7261 6d65 7465  tialize paramete
-0000d0c0: 7273 2e0a 2020 2020 2020 6d65 7468 6f64  rs..      method
-0000d0d0: 3a20 4120 6675 6e63 7469 6f6e 2074 6f20  : A function to 
-0000d0e0: 6361 6c6c 2061 7070 6c79 206f 6e2e 2054  call apply on. T
-0000d0f0: 6869 7320 6973 2067 656e 6572 616c 6c79  his is generally
-0000d100: 2061 2066 756e 6374 696f 6e20 696e 2074   a function in t
-0000d110: 6865 0a20 2020 2020 2020 206d 6f64 756c  he.        modul
-0000d120: 652e 2049 6620 7072 6f76 6964 6564 2c20  e. If provided, 
-0000d130: 6170 706c 6965 7320 7468 6973 206d 6574  applies this met
-0000d140: 686f 642e 2049 6620 6e6f 7420 7072 6f76  hod. If not prov
-0000d150: 6964 6564 2c20 6170 706c 6965 7320 7468  ided, applies th
-0000d160: 650a 2020 2020 2020 2020 6060 5f5f 6361  e.        ``__ca
-0000d170: 6c6c 5f5f 6060 206d 6574 686f 6420 6f66  ll__`` method of
-0000d180: 2074 6865 206d 6f64 756c 652e 2041 2073   the module. A s
-0000d190: 7472 696e 6720 6361 6e20 616c 736f 2062  tring can also b
-0000d1a0: 6520 7072 6f76 6964 6564 2074 6f0a 2020  e provided to.  
-0000d1b0: 2020 2020 2020 7370 6563 6966 7920 6120        specify a 
-0000d1c0: 6d65 7468 6f64 2062 7920 6e61 6d65 2e0a  method by name..
-0000d1d0: 2020 2020 2020 6d75 7461 626c 653a 2043        mutable: C
-0000d1e0: 616e 2062 6520 626f 6f6c 2c20 7374 722c  an be bool, str,
-0000d1f0: 206f 7220 6c69 7374 2e20 5370 6563 6966   or list. Specif
-0000d200: 6965 7320 7768 6963 6820 636f 6c6c 6563  ies which collec
-0000d210: 7469 6f6e 7320 7368 6f75 6c64 2062 650a  tions should be.
-0000d220: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d230: 7265 6174 6564 2061 7320 6d75 7461 626c  reated as mutabl
-0000d240: 653a 2060 6062 6f6f 6c60 603a 2061 6c6c  e: ``bool``: all
-0000d250: 2f6e 6f20 636f 6c6c 6563 7469 6f6e 7320  /no collections 
-0000d260: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
-0000d270: 2020 2020 2020 2020 2020 2020 6060 7374              ``st
-0000d280: 7260 603a 2054 6865 206e 616d 6520 6f66  r``: The name of
-0000d290: 2061 2073 696e 676c 6520 6d75 7461 626c   a single mutabl
-0000d2a0: 6520 636f 6c6c 6563 7469 6f6e 2e20 6060  e collection. ``
-0000d2b0: 6c69 7374 6060 3a20 410a 2020 2020 2020  list``: A.      
-0000d2c0: 2020 2020 2020 2020 206c 6973 7420 6f66           list of
-0000d2d0: 206e 616d 6573 206f 6620 6d75 7461 626c   names of mutabl
-0000d2e0: 6520 636f 6c6c 6563 7469 6f6e 732e 0a20  e collections.. 
-0000d2f0: 2020 2020 2063 6170 7475 7265 5f69 6e74       capture_int
-0000d300: 6572 6d65 6469 6174 6573 3a20 4966 2060  ermediates: If `
-0000d310: 5472 7565 602c 2063 6170 7475 7265 7320  True`, captures 
-0000d320: 696e 7465 726d 6564 6961 7465 2072 6574  intermediate ret
-0000d330: 7572 6e20 7661 6c75 6573 0a20 2020 2020  urn values.     
-0000d340: 2020 206f 6620 616c 6c20 4d6f 6475 6c65     of all Module
-0000d350: 7320 696e 7369 6465 2074 6865 2022 696e  s inside the "in
-0000d360: 7465 726d 6564 6961 7465 7322 2063 6f6c  termediates" col
-0000d370: 6c65 6374 696f 6e2e 2042 7920 6465 6661  lection. By defa
-0000d380: 756c 7420 6f6e 6c79 0a20 2020 2020 2020  ult only.       
-0000d390: 2074 6865 2072 6574 7572 6e20 7661 6c75   the return valu
-0000d3a0: 6573 206f 6620 616c 6c20 6060 5f5f 6361  es of all ``__ca
-0000d3b0: 6c6c 5f5f 6060 206d 6574 686f 6473 2061  ll__`` methods a
-0000d3c0: 7265 2073 746f 7265 642e 2041 2066 756e  re stored. A fun
-0000d3d0: 6374 696f 6e20 6361 6e0a 2020 2020 2020  ction can.      
-0000d3e0: 2020 6265 2070 6173 7365 6420 746f 2063    be passed to c
-0000d3f0: 6861 6e67 6520 7468 6520 6669 6c74 6572  hange the filter
-0000d400: 2062 6568 6176 696f 722e 2054 6865 2066   behavior. The f
-0000d410: 696c 7465 7220 6675 6e63 7469 6f6e 2074  ilter function t
-0000d420: 616b 6573 0a20 2020 2020 2020 2074 6865  akes.        the
-0000d430: 204d 6f64 756c 6520 696e 7374 616e 6365   Module instance
-0000d440: 2061 6e64 206d 6574 686f 6420 6e61 6d65   and method name
-0000d450: 2061 6e64 2072 6574 7572 6e73 2061 2062   and returns a b
-0000d460: 6f6f 6c20 696e 6469 6361 7469 6e67 0a20  ool indicating. 
-0000d470: 2020 2020 2020 2077 6865 7468 6572 2074         whether t
-0000d480: 6865 206f 7574 7075 7420 6f66 2074 6861  he output of tha
-0000d490: 7420 6d65 7468 6f64 2069 6e76 6f63 6174  t method invocat
-0000d4a0: 696f 6e20 7368 6f75 6c64 2062 6520 7374  ion should be st
-0000d4b0: 6f72 6564 2e0a 2020 2020 2020 2a2a 6b77  ored..      **kw
-0000d4c0: 6172 6773 3a20 4b65 7977 6f72 6420 6172  args: Keyword ar
-0000d4d0: 6775 6d65 6e74 7320 7061 7373 6564 2074  guments passed t
-0000d4e0: 6f20 7468 6520 7370 6563 6966 6965 6420  o the specified 
-0000d4f0: 6170 706c 7920 6d65 7468 6f64 2e0a 2020  apply method..  
-0000d500: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000d510: 2049 6620 6060 6d75 7461 626c 6560 6020   If ``mutable`` 
-0000d520: 6973 2046 616c 7365 2c20 7265 7475 726e  is False, return
-0000d530: 7320 6f75 7470 7574 2e20 4966 2061 6e79  s output. If any
-0000d540: 2063 6f6c 6c65 6374 696f 6e73 2061 7265   collections are
-0000d550: 0a20 2020 2020 206d 7574 6162 6c65 2c20  .      mutable, 
-0000d560: 7265 7475 726e 7320 6060 286f 7574 7075  returns ``(outpu
-0000d570: 742c 2076 6172 7329 6060 2c20 7768 6572  t, vars)``, wher
-0000d580: 6520 6060 7661 7273 6060 2061 7265 2069  e ``vars`` are i
-0000d590: 7320 6120 6469 6374 0a20 2020 2020 206f  s a dict.      o
-0000d5a0: 6620 7468 6520 6d6f 6469 6669 6564 2063  f the modified c
-0000d5b0: 6f6c 6c65 6374 696f 6e73 2e0a 2020 2020  ollections..    
-0000d5c0: 2222 220a 2020 2020 4d6f 6475 6c65 2e5f  """.    Module._
-0000d5d0: 6d6f 6475 6c65 5f63 6865 636b 7328 7365  module_checks(se
-0000d5e0: 6c66 290a 0a20 2020 2069 6620 6973 696e  lf)..    if isin
-0000d5f0: 7374 616e 6365 286d 6574 686f 642c 2073  stance(method, s
-0000d600: 7472 293a 0a20 2020 2020 2061 7474 7269  tr):.      attri
-0000d610: 6275 7465 5f6e 616d 6520 3d20 6d65 7468  bute_name = meth
-0000d620: 6f64 0a20 2020 2020 206d 6574 686f 6420  od.      method 
-0000d630: 3d20 6765 7461 7474 7228 7365 6c66 2c20  = getattr(self, 
-0000d640: 6174 7472 6962 7574 655f 6e61 6d65 290a  attribute_name).
-0000d650: 2020 2020 2020 6966 206e 6f74 2063 616c        if not cal
-0000d660: 6c61 626c 6528 6d65 7468 6f64 293a 0a20  lable(method):. 
-0000d670: 2020 2020 2020 2063 6c61 7373 5f6e 616d         class_nam
-0000d680: 6520 3d20 7479 7065 2873 656c 6629 2e5f  e = type(self)._
-0000d690: 5f6e 616d 655f 5f0a 2020 2020 2020 2020  _name__.        
-0000d6a0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-0000d6b0: 6627 5c27 7b63 6c61 7373 5f6e 616d 657d  f'\'{class_name}
-0000d6c0: 2e7b 6174 7472 6962 7574 655f 6e61 6d65  .{attribute_name
-0000d6d0: 7d5c 2720 6d75 7374 2062 6520 6120 6361  }\' must be a ca
-0000d6e0: 6c6c 6162 6c65 2c20 676f 7420 7b74 7970  llable, got {typ
-0000d6f0: 6528 6d65 7468 6f64 297d 2e27 290a 2020  e(method)}.').  
-0000d700: 2020 656c 6966 206d 6574 686f 6420 6973    elif method is
-0000d710: 204e 6f6e 653a 0a20 2020 2020 206d 6574   None:.      met
-0000d720: 686f 6420 3d20 7365 6c66 2e5f 5f63 616c  hod = self.__cal
-0000d730: 6c5f 5f0a 2020 2020 6d65 7468 6f64 203d  l__.    method =
-0000d740: 205f 6765 745f 756e 626f 756e 645f 666e   _get_unbound_fn
-0000d750: 286d 6574 686f 6429 0a20 2020 2072 6574  (method).    ret
-0000d760: 7572 6e20 6170 706c 7928 0a20 2020 2020  urn apply(.     
-0000d770: 2020 206d 6574 686f 642c 2073 656c 662c     method, self,
-0000d780: 0a20 2020 2020 2020 206d 7574 6162 6c65  .        mutable
-0000d790: 3d6d 7574 6162 6c65 2c0a 2020 2020 2020  =mutable,.      
-0000d7a0: 2020 6361 7074 7572 655f 696e 7465 726d    capture_interm
-0000d7b0: 6564 6961 7465 733d 6361 7074 7572 655f  ediates=capture_
-0000d7c0: 696e 7465 726d 6564 6961 7465 732c 0a20  intermediates,. 
-0000d7d0: 2020 2029 2876 6172 6961 626c 6573 2c20     )(variables, 
-0000d7e0: 2a61 7267 732c 202a 2a6b 7761 7267 732c  *args, **kwargs,
-0000d7f0: 2072 6e67 733d 726e 6773 290a 0a20 2040   rngs=rngs)..  @
-0000d800: 7472 6163 6562 6163 6b5f 7574 696c 2e61  traceback_util.a
-0000d810: 7069 5f62 6f75 6e64 6172 790a 2020 6465  pi_boundary.  de
-0000d820: 6620 696e 6974 5f77 6974 685f 6f75 7470  f init_with_outp
-0000d830: 7574 2873 656c 662c 0a20 2020 2020 2020  ut(self,.       
-0000d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d850: 726e 6773 3a20 556e 696f 6e5b 5052 4e47  rngs: Union[PRNG
-0000d860: 4b65 792c 2052 4e47 5365 7175 656e 6365  Key, RNGSequence
-0000d870: 735d 2c0a 2020 2020 2020 2020 2020 2020  s],.            
-0000d880: 2020 2020 2020 2020 2020 202a 6172 6773             *args
-0000d890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d8a0: 2020 2020 2020 2020 206d 6574 686f 643a           method:
-0000d8b0: 2055 6e69 6f6e 5b43 616c 6c61 626c 655b   Union[Callable[
-0000d8c0: 2e2e 2e2c 2041 6e79 5d2c 2073 7472 2c20  ..., Any], str, 
-0000d8d0: 4e6f 6e65 5d20 3d20 4e6f 6e65 2c0a 2020  None] = None,.  
-0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8f0: 2020 2020 206d 7574 6162 6c65 3a20 436f       mutable: Co
-0000d900: 6c6c 6563 7469 6f6e 4669 6c74 6572 203d  llectionFilter =
-0000d910: 2044 656e 794c 6973 7428 2769 6e74 6572   DenyList('inter
-0000d920: 6d65 6469 6174 6573 2729 2c0a 2020 2020  mediates'),.    
-0000d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d940: 2020 2063 6170 7475 7265 5f69 6e74 6572     capture_inter
-0000d950: 6d65 6469 6174 6573 3a20 556e 696f 6e5b  mediates: Union[
-0000d960: 626f 6f6c 2c20 4361 6c6c 6162 6c65 5b5b  bool, Callable[[
-0000d970: 274d 6f64 756c 6527 2c20 7374 725d 2c20  'Module', str], 
-0000d980: 626f 6f6c 5d5d 203d 2046 616c 7365 2c0a  bool]] = False,.
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 2020 2020 2020 202a 2a6b 7761 7267 7329         **kwargs)
-0000d9b0: 202d 3e20 5475 706c 655b 416e 792c 2055   -> Tuple[Any, U
-0000d9c0: 6e69 6f6e 5b46 726f 7a65 6e56 6172 6961  nion[FrozenVaria
-0000d9d0: 626c 6544 6963 742c 2044 6963 745b 7374  bleDict, Dict[st
-0000d9e0: 722c 2041 6e79 5d5d 5d3a 0a20 2020 2022  r, Any]]]:.    "
-0000d9f0: 2222 496e 6974 6961 6c69 7a65 7320 6120  ""Initializes a 
-0000da00: 6d6f 6475 6c65 206d 6574 686f 6420 7769  module method wi
-0000da10: 7468 2076 6172 6961 626c 6573 2061 6e64  th variables and
-0000da20: 2072 6574 7572 6e73 206f 7574 7075 7420   returns output 
-0000da30: 616e 6420 6d6f 6469 6669 6564 2076 6172  and modified var
-0000da40: 6961 626c 6573 2e0a 0a20 2020 2041 7267  iables...    Arg
-0000da50: 733a 0a20 2020 2020 2072 6e67 733a 2054  s:.      rngs: T
-0000da60: 6865 2072 6e67 7320 666f 7220 7468 6520  he rngs for the 
-0000da70: 7661 7269 6162 6c65 2063 6f6c 6c65 6374  variable collect
-0000da80: 696f 6e73 2e0a 2020 2020 2020 2a61 7267  ions..      *arg
-0000da90: 733a 204e 616d 6564 2061 7267 756d 656e  s: Named argumen
-0000daa0: 7473 2070 6173 7365 6420 746f 2074 6865  ts passed to the
-0000dab0: 2069 6e69 7420 6675 6e63 7469 6f6e 2e0a   init function..
-0000dac0: 2020 2020 2020 6d65 7468 6f64 3a20 416e        method: An
-0000dad0: 206f 7074 696f 6e61 6c20 6d65 7468 6f64   optional method
-0000dae0: 2e20 4966 2070 726f 7669 6465 642c 2061  . If provided, a
-0000daf0: 7070 6c69 6573 2074 6869 7320 6d65 7468  pplies this meth
-0000db00: 6f64 2e20 4966 206e 6f74 0a20 2020 2020  od. If not.     
-0000db10: 2020 2070 726f 7669 6465 642c 2061 7070     provided, app
-0000db20: 6c69 6573 2074 6865 2060 605f 5f63 616c  lies the ``__cal
-0000db30: 6c5f 5f60 6020 6d65 7468 6f64 2e20 4120  l__`` method. A 
-0000db40: 7374 7269 6e67 2063 616e 2061 6c73 6f20  string can also 
-0000db50: 6265 270a 2020 2020 2020 2020 7072 6f76  be'.        prov
-0000db60: 6964 6564 2074 6f20 7370 6563 6966 7920  ided to specify 
-0000db70: 6120 6d65 7468 6f64 2062 7920 6e61 6d65  a method by name
-0000db80: 2e0a 2020 2020 2020 6d75 7461 626c 653a  ..      mutable:
-0000db90: 2043 616e 2062 6520 626f 6f6c 2c20 7374   Can be bool, st
-0000dba0: 722c 206f 7220 6c69 7374 2e20 5370 6563  r, or list. Spec
-0000dbb0: 6966 6965 7320 7768 6963 6820 636f 6c6c  ifies which coll
-0000dbc0: 6563 7469 6f6e 7320 7368 6f75 6c64 2062  ections should b
-0000dbd0: 650a 2020 2020 2020 2020 7472 6561 7465  e.        treate
-0000dbe0: 6420 6173 206d 7574 6162 6c65 3a20 6060  d as mutable: ``
-0000dbf0: 626f 6f6c 6060 3a20 616c 6c2f 6e6f 2063  bool``: all/no c
-0000dc00: 6f6c 6c65 6374 696f 6e73 2061 7265 206d  ollections are m
-0000dc10: 7574 6162 6c65 2e0a 2020 2020 2020 2020  utable..        
-0000dc20: 6060 7374 7260 603a 2054 6865 206e 616d  ``str``: The nam
-0000dc30: 6520 6f66 2061 2073 696e 676c 6520 6d75  e of a single mu
-0000dc40: 7461 626c 6520 636f 6c6c 6563 7469 6f6e  table collection
-0000dc50: 2e20 6060 6c69 7374 6060 3a20 410a 2020  . ``list``: A.  
-0000dc60: 2020 2020 2020 6c69 7374 206f 6620 6e61        list of na
-0000dc70: 6d65 7320 6f66 206d 7574 6162 6c65 2063  mes of mutable c
-0000dc80: 6f6c 6c65 6374 696f 6e73 2e20 4279 2064  ollections. By d
-0000dc90: 6566 6175 6c74 2061 6c6c 2063 6f6c 6c65  efault all colle
-0000dca0: 6374 696f 6e73 0a20 2020 2020 2020 2065  ctions.        e
-0000dcb0: 7863 6570 7420 2269 6e74 6572 6d65 6469  xcept "intermedi
-0000dcc0: 6174 6573 2220 6172 6520 6d75 7461 626c  ates" are mutabl
-0000dcd0: 652e 0a20 2020 2020 2063 6170 7475 7265  e..      capture
-0000dce0: 5f69 6e74 6572 6d65 6469 6174 6573 3a20  _intermediates: 
-0000dcf0: 4966 2060 5472 7565 602c 2063 6170 7475  If `True`, captu
-0000dd00: 7265 7320 696e 7465 726d 6564 6961 7465  res intermediate
-0000dd10: 2072 6574 7572 6e20 7661 6c75 6573 0a20   return values. 
-0000dd20: 2020 2020 2020 206f 6620 616c 6c20 4d6f         of all Mo
-0000dd30: 6475 6c65 7320 696e 7369 6465 2074 6865  dules inside the
-0000dd40: 2022 696e 7465 726d 6564 6961 7465 7322   "intermediates"
-0000dd50: 2063 6f6c 6c65 6374 696f 6e2e 2042 7920   collection. By 
-0000dd60: 6465 6661 756c 7420 6f6e 6c79 0a20 2020  default only.   
-0000dd70: 2020 2020 2074 6865 2072 6574 7572 6e20       the return 
-0000dd80: 7661 6c75 6573 206f 6620 616c 6c20 6060  values of all ``
-0000dd90: 5f5f 6361 6c6c 5f5f 6060 206d 6574 686f  __call__`` metho
-0000dda0: 6473 2061 7265 2073 746f 7265 642e 2041  ds are stored. A
-0000ddb0: 2066 756e 6374 696f 6e20 6361 6e0a 2020   function can.  
-0000ddc0: 2020 2020 2020 6265 2070 6173 7365 6420        be passed 
-0000ddd0: 746f 2063 6861 6e67 6520 7468 6520 6669  to change the fi
-0000dde0: 6c74 6572 2062 6568 6176 696f 722e 2054  lter behavior. T
-0000ddf0: 6865 2066 696c 7465 7220 6675 6e63 7469  he filter functi
-0000de00: 6f6e 2074 616b 6573 0a20 2020 2020 2020  on takes.       
-0000de10: 2074 6865 204d 6f64 756c 6520 696e 7374   the Module inst
-0000de20: 616e 6365 2061 6e64 206d 6574 686f 6420  ance and method 
-0000de30: 6e61 6d65 2061 6e64 2072 6574 7572 6e73  name and returns
-0000de40: 2061 2062 6f6f 6c20 696e 6469 6361 7469   a bool indicati
-0000de50: 6e67 0a20 2020 2020 2020 2077 6865 7468  ng.        wheth
-0000de60: 6572 2074 6865 206f 7574 7075 7420 6f66  er the output of
-0000de70: 2074 6861 7420 6d65 7468 6f64 2069 6e76   that method inv
-0000de80: 6f63 6174 696f 6e20 7368 6f75 6c64 2062  ocation should b
-0000de90: 6520 7374 6f72 6564 2e0a 2020 2020 2020  e stored..      
-0000dea0: 2a2a 6b77 6172 6773 3a20 4b65 7977 6f72  **kwargs: Keywor
-0000deb0: 6420 6172 6775 6d65 6e74 7320 7061 7373  d arguments pass
-0000dec0: 6564 2074 6f20 7468 6520 696e 6974 2066  ed to the init f
-0000ded0: 756e 6374 696f 6e2e 0a20 2020 2052 6574  unction..    Ret
-0000dee0: 7572 6e73 3a0a 2020 2020 2020 6028 6f75  urns:.      `(ou
-0000def0: 7470 7574 2c20 7661 7273 2960 602c 2077  tput, vars)``, w
-0000df00: 6865 7265 2060 6076 6172 7360 6020 6172  here ``vars`` ar
-0000df10: 6520 6973 2061 2064 6963 7420 6f66 2074  e is a dict of t
-0000df20: 6865 206d 6f64 6966 6965 640a 2020 2020  he modified.    
-0000df30: 2020 636f 6c6c 6563 7469 6f6e 732e 0a20    collections.. 
-0000df40: 2020 2022 2222 0a20 2020 204d 6f64 756c     """.    Modul
-0000df50: 652e 5f6d 6f64 756c 655f 6368 6563 6b73  e._module_checks
-0000df60: 2873 656c 6629 0a0a 2020 2020 6966 206e  (self)..    if n
-0000df70: 6f74 2069 7369 6e73 7461 6e63 6528 726e  ot isinstance(rn
-0000df80: 6773 2c20 6469 6374 293a 0a20 2020 2020  gs, dict):.     
-0000df90: 2069 6620 6e6f 7420 636f 7265 2e73 636f   if not core.sco
-0000dfa0: 7065 2e5f 6973 5f76 616c 6964 5f72 6e67  pe._is_valid_rng
-0000dfb0: 2872 6e67 7329 3a0a 2020 2020 2020 2020  (rngs):.        
-0000dfc0: 7261 6973 6520 6572 726f 7273 2e49 6e76  raise errors.Inv
-0000dfd0: 616c 6964 526e 6745 7272 6f72 280a 2020  alidRngError(.  
-0000dfe0: 2020 2020 2020 2020 2020 2752 4e47 7320            'RNGs 
-0000dff0: 7368 6f75 6c64 2062 6520 6f66 2073 6861  should be of sha
-0000e000: 7065 2028 322c 2920 6f72 204b 6579 4172  pe (2,) or KeyAr
-0000e010: 7261 7920 696e 204d 6f64 756c 6520 270a  ray in Module '.
-0000e020: 2020 2020 2020 2020 2020 2020 6627 7b73              f'{s
-0000e030: 656c 662e 5f5f 636c 6173 735f 5f2e 5f5f  elf.__class__.__
-0000e040: 6e61 6d65 5f5f 7d2c 2062 7574 2072 6e67  name__}, but rng
-0000e050: 7320 6172 653a 207b 726e 6773 7d27 290a  s are: {rngs}').
-0000e060: 2020 2020 2020 726e 6773 203d 207b 2770        rngs = {'p
-0000e070: 6172 616d 7327 3a20 726e 6773 7d0a 0a20  arams': rngs}.. 
-0000e080: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000e090: 286d 6574 686f 642c 2073 7472 293a 0a20  (method, str):. 
-0000e0a0: 2020 2020 2061 7474 7269 6275 7465 5f6e       attribute_n
-0000e0b0: 616d 6520 3d20 6d65 7468 6f64 0a20 2020  ame = method.   
-0000e0c0: 2020 206d 6574 686f 6420 3d20 6765 7461     method = geta
-0000e0d0: 7474 7228 7365 6c66 2c20 6174 7472 6962  ttr(self, attrib
-0000e0e0: 7574 655f 6e61 6d65 290a 2020 2020 2020  ute_name).      
-0000e0f0: 6966 206e 6f74 2063 616c 6c61 626c 6528  if not callable(
-0000e100: 6d65 7468 6f64 293a 0a20 2020 2020 2020  method):.       
-0000e110: 2063 6c61 7373 5f6e 616d 6520 3d20 7479   class_name = ty
-0000e120: 7065 2873 656c 6629 2e5f 5f6e 616d 655f  pe(self).__name_
-0000e130: 5f0a 2020 2020 2020 2020 7261 6973 6520  _.        raise 
-0000e140: 5479 7065 4572 726f 7228 6627 5c27 7b63  TypeError(f'\'{c
-0000e150: 6c61 7373 5f6e 616d 657d 2e7b 6174 7472  lass_name}.{attr
-0000e160: 6962 7574 655f 6e61 6d65 7d5c 2720 6d75  ibute_name}\' mu
-0000e170: 7374 2062 6520 6120 6361 6c6c 6162 6c65  st be a callable
-0000e180: 2c20 676f 7420 7b74 7970 6528 6d65 7468  , got {type(meth
-0000e190: 6f64 297d 2e27 290a 2020 2020 656c 6966  od)}.').    elif
-0000e1a0: 206d 6574 686f 6420 6973 204e 6f6e 653a   method is None:
-0000e1b0: 0a20 2020 2020 206d 6574 686f 6420 3d20  .      method = 
-0000e1c0: 7365 6c66 2e5f 5f63 616c 6c5f 5f0a 2020  self.__call__.  
-0000e1d0: 2020 6d65 7468 6f64 203d 205f 6765 745f    method = _get_
-0000e1e0: 756e 626f 756e 645f 666e 286d 6574 686f  unbound_fn(metho
-0000e1f0: 6429 0a20 2020 2072 6574 7572 6e20 696e  d).    return in
-0000e200: 6974 5f77 6974 685f 6f75 7470 7574 280a  it_with_output(.
-0000e210: 2020 2020 2020 2020 6d65 7468 6f64 2c0a          method,.
-0000e220: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000e230: 2020 2020 2020 6d75 7461 626c 653d 6d75        mutable=mu
-0000e240: 7461 626c 652c 0a20 2020 2020 2020 2063  table,.        c
-0000e250: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
-0000e260: 6174 6573 3d63 6170 7475 7265 5f69 6e74  ates=capture_int
-0000e270: 6572 6d65 6469 6174 6573 0a20 2020 2029  ermediates.    )
-0000e280: 2872 6e67 732c 202a 6172 6773 2c20 2a2a  (rngs, *args, **
-0000e290: 6b77 6172 6773 290a 0a20 2040 7472 6163  kwargs)..  @trac
-0000e2a0: 6562 6163 6b5f 7574 696c 2e61 7069 5f62  eback_util.api_b
-0000e2b0: 6f75 6e64 6172 790a 2020 6465 6620 696e  oundary.  def in
-0000e2c0: 6974 2873 656c 662c 0a20 2020 2020 2020  it(self,.       
-0000e2d0: 2020 2020 726e 6773 3a20 556e 696f 6e5b      rngs: Union[
-0000e2e0: 5052 4e47 4b65 792c 2052 4e47 5365 7175  PRNGKey, RNGSequ
-0000e2f0: 656e 6365 735d 2c0a 2020 2020 2020 2020  ences],.        
-0000e300: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
-0000e310: 2020 2020 206d 6574 686f 643a 2055 6e69       method: Uni
-0000e320: 6f6e 5b43 616c 6c61 626c 655b 2e2e 2e2c  on[Callable[...,
-0000e330: 2041 6e79 5d2c 2073 7472 2c20 4e6f 6e65   Any], str, None
-0000e340: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000e350: 2020 2020 206d 7574 6162 6c65 3a20 436f       mutable: Co
-0000e360: 6c6c 6563 7469 6f6e 4669 6c74 6572 203d  llectionFilter =
-0000e370: 2044 656e 794c 6973 7428 2769 6e74 6572   DenyList('inter
-0000e380: 6d65 6469 6174 6573 2729 2c0a 2020 2020  mediates'),.    
-0000e390: 2020 2020 2020 2063 6170 7475 7265 5f69         capture_i
-0000e3a0: 6e74 6572 6d65 6469 6174 6573 3a20 556e  ntermediates: Un
-0000e3b0: 696f 6e5b 626f 6f6c 2c20 4361 6c6c 6162  ion[bool, Callab
-0000e3c0: 6c65 5b5b 274d 6f64 756c 6527 2c20 7374  le[['Module', st
-0000e3d0: 725d 2c20 626f 6f6c 5d5d 203d 2046 616c  r], bool]] = Fal
-0000e3e0: 7365 2c0a 2020 2020 2020 2020 2020 202a  se,.           *
-0000e3f0: 2a6b 7761 7267 7329 202d 3e20 556e 696f  *kwargs) -> Unio
-0000e400: 6e5b 4672 6f7a 656e 5661 7269 6162 6c65  n[FrozenVariable
-0000e410: 4469 6374 2c20 4469 6374 5b73 7472 2c20  Dict, Dict[str, 
-0000e420: 416e 795d 5d3a 0a20 2020 2022 2222 496e  Any]]:.    """In
-0000e430: 6974 6961 6c69 7a65 7320 6120 6d6f 6475  itializes a modu
-0000e440: 6c65 206d 6574 686f 6420 7769 7468 2076  le method with v
-0000e450: 6172 6961 626c 6573 2061 6e64 2072 6574  ariables and ret
-0000e460: 7572 6e73 206d 6f64 6966 6965 6420 7661  urns modified va
-0000e470: 7269 6162 6c65 732e 0a0a 2020 2020 6060  riables...    ``
-0000e480: 696e 6974 6060 2074 616b 6573 2061 7320  init`` takes as 
-0000e490: 6669 7273 7420 6172 6775 6d65 6e74 2065  first argument e
-0000e4a0: 6974 6865 7220 6120 7369 6e67 6c65 2060  ither a single `
-0000e4b0: 6050 524e 474b 6579 6060 2c20 6f72 2061  `PRNGKey``, or a
-0000e4c0: 2064 6963 7469 6f6e 6172 7920 6d61 7070   dictionary mapp
-0000e4d0: 696e 6720 7661 7269 6162 6c65 2063 6f6c  ing variable col
-0000e4e0: 6c65 6374 696f 6e73 206e 616d 6573 2074  lections names t
-0000e4f0: 6f20 7468 6569 7220 6060 5052 4e47 4b65  o their ``PRNGKe
-0000e500: 7973 6060 2c20 616e 6420 7769 6c6c 2063  ys``, and will c
-0000e510: 616c 6c20 6060 6d65 7468 6f64 6060 2028  all ``method`` (
-0000e520: 7768 6963 6820 6973 2074 6865 206d 6f64  which is the mod
-0000e530: 756c 6527 7320 6060 5f5f 6361 6c6c 5f5f  ule's ``__call__
-0000e540: 6060 2066 756e 6374 696f 6e20 6279 2064  `` function by d
-0000e550: 6566 6175 6c74 2920 7061 7373 696e 6720  efault) passing 
-0000e560: 6060 2a61 7267 7360 6020 616e 6420 6060  ``*args`` and ``
-0000e570: 2a2a 6b77 6172 6773 6060 2c20 616e 6420  **kwargs``, and 
-0000e580: 7265 7475 726e 730a 2020 2020 6120 6469  returns.    a di
-0000e590: 6374 696f 6e61 7279 206f 6620 696e 6974  ctionary of init
-0000e5a0: 6961 6c69 7a65 6420 7661 7269 6162 6c65  ialized variable
-0000e5b0: 732e 0a0a 2020 2020 4578 616d 706c 653a  s...    Example:
-0000e5c0: 3a0a 0a20 2020 2020 203e 3e3e 2069 6d70  :..      >>> imp
-0000e5d0: 6f72 7420 666c 6178 2e6c 696e 656e 2061  ort flax.linen a
-0000e5e0: 7320 6e6e 0a20 2020 2020 203e 3e3e 2069  s nn.      >>> i
-0000e5f0: 6d70 6f72 7420 6a61 782e 6e75 6d70 7920  mport jax.numpy 
-0000e600: 6173 206a 6e70 0a20 2020 2020 203e 3e3e  as jnp.      >>>
-0000e610: 2069 6d70 6f72 7420 6a61 780a 2020 2020   import jax.    
-0000e620: 2020 2e2e 2e0a 2020 2020 2020 3e3e 3e20    ....      >>> 
-0000e630: 636c 6173 7320 466f 6f28 6e6e 2e4d 6f64  class Foo(nn.Mod
-0000e640: 756c 6529 3a0a 2020 2020 2020 2e2e 2e20  ule):.      ... 
-0000e650: 2020 406e 6e2e 636f 6d70 6163 740a 2020    @nn.compact.  
-0000e660: 2020 2020 2e2e 2e20 2020 6465 6620 5f5f      ...   def __
-0000e670: 6361 6c6c 5f5f 2873 656c 662c 2078 2c20  call__(self, x, 
-0000e680: 7472 6169 6e29 3a0a 2020 2020 2020 2e2e  train):.      ..
-0000e690: 2e20 2020 2020 7820 3d20 6e6e 2e44 656e  .     x = nn.Den
-0000e6a0: 7365 2831 3629 2878 290a 2020 2020 2020  se(16)(x).      
-0000e6b0: 2e2e 2e20 2020 2020 7820 3d20 6e6e 2e42  ...     x = nn.B
-0000e6c0: 6174 6368 4e6f 726d 2875 7365 5f72 756e  atchNorm(use_run
-0000e6d0: 6e69 6e67 5f61 7665 7261 6765 3d6e 6f74  ning_average=not
-0000e6e0: 2074 7261 696e 2928 7829 0a20 2020 2020   train)(x).     
-0000e6f0: 202e 2e2e 2020 2020 2078 203d 206e 6e2e   ...     x = nn.
-0000e700: 7265 6c75 2878 290a 2020 2020 2020 2e2e  relu(x).      ..
-0000e710: 2e20 2020 2020 7265 7475 726e 206e 6e2e  .     return nn.
-0000e720: 4465 6e73 6528 3129 2878 290a 2020 2020  Dense(1)(x).    
-0000e730: 2020 2e2e 2e0a 2020 2020 2020 3e3e 3e20    ....      >>> 
-0000e740: 6d6f 6475 6c65 203d 2046 6f6f 2829 0a20  module = Foo(). 
-0000e750: 2020 2020 203e 3e3e 206b 6579 203d 206a       >>> key = j
-0000e760: 6178 2e72 616e 646f 6d2e 5052 4e47 4b65  ax.random.PRNGKe
-0000e770: 7928 3029 0a20 2020 2020 203e 3e3e 2076  y(0).      >>> v
-0000e780: 6172 6961 626c 6573 203d 206d 6f64 756c  ariables = modul
-0000e790: 652e 696e 6974 286b 6579 2c20 6a6e 702e  e.init(key, jnp.
-0000e7a0: 656d 7074 7928 2831 2c20 3729 292c 2074  empty((1, 7)), t
-0000e7b0: 7261 696e 3d46 616c 7365 290a 0a20 2020  rain=False)..   
-0000e7c0: 2049 6620 796f 7520 7061 7373 2061 2073   If you pass a s
-0000e7d0: 696e 676c 6520 6060 5052 4e47 4b65 7960  ingle ``PRNGKey`
-0000e7e0: 602c 2046 6c61 7820 7769 6c6c 2075 7365  `, Flax will use
-0000e7f0: 2069 7420 746f 2066 6565 6420 7468 6520   it to feed the 
-0000e800: 6060 2770 6172 616d 7327 6060 2052 4e47  ``'params'`` RNG
-0000e810: 2073 7472 6561 6d2e 0a20 2020 2049 6620   stream..    If 
-0000e820: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-0000e830: 6120 6469 6666 6572 656e 7420 524e 4720  a different RNG 
-0000e840: 7374 7265 616d 206f 7220 6e65 6564 2074  stream or need t
-0000e850: 6f20 7573 6520 6d75 6c74 6970 6c65 2073  o use multiple s
-0000e860: 7472 6561 6d73 2c20 796f 7520 6d75 7374  treams, you must
-0000e870: 2070 6173 7320 610a 2020 2020 6469 6374   pass a.    dict
-0000e880: 696f 6e61 7279 206d 6170 7069 6e67 2065  ionary mapping e
-0000e890: 6163 6820 524e 4720 7374 7265 616d 206e  ach RNG stream n
-0000e8a0: 616d 6520 746f 2069 7473 2063 6f72 7265  ame to its corre
-0000e8b0: 7370 6f6e 6469 6e67 2060 6050 524e 474b  sponding ``PRNGK
-0000e8c0: 6579 6060 2074 6f20 6060 696e 6974 6060  ey`` to ``init``
-0000e8d0: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a3a  ...    Example::
-0000e8e0: 0a0a 2020 2020 2020 3e3e 3e20 636c 6173  ..      >>> clas
-0000e8f0: 7320 466f 6f28 6e6e 2e4d 6f64 756c 6529  s Foo(nn.Module)
-0000e900: 3a0a 2020 2020 2020 2e2e 2e20 2020 406e  :.      ...   @n
-0000e910: 6e2e 636f 6d70 6163 740a 2020 2020 2020  n.compact.      
-0000e920: 2e2e 2e20 2020 6465 6620 5f5f 6361 6c6c  ...   def __call
-0000e930: 5f5f 2873 656c 662c 2078 2c20 7472 6169  __(self, x, trai
-0000e940: 6e29 3a0a 2020 2020 2020 2e2e 2e20 2020  n):.      ...   
-0000e950: 2020 7820 3d20 6e6e 2e44 656e 7365 2831    x = nn.Dense(1
-0000e960: 3629 2878 290a 2020 2020 2020 2e2e 2e20  6)(x).      ... 
-0000e970: 2020 2020 7820 3d20 6e6e 2e42 6174 6368      x = nn.Batch
-0000e980: 4e6f 726d 2875 7365 5f72 756e 6e69 6e67  Norm(use_running
-0000e990: 5f61 7665 7261 6765 3d6e 6f74 2074 7261  _average=not tra
-0000e9a0: 696e 2928 7829 0a20 2020 2020 202e 2e2e  in)(x).      ...
-0000e9b0: 2020 2020 2078 203d 206e 6e2e 7265 6c75       x = nn.relu
-0000e9c0: 2878 290a 2020 2020 2020 2e2e 2e0a 2020  (x).      ....  
-0000e9d0: 2020 2020 2e2e 2e20 2020 2020 2320 4164      ...     # Ad
-0000e9e0: 6420 6761 7573 7369 616e 206e 6f69 7365  d gaussian noise
-0000e9f0: 0a20 2020 2020 202e 2e2e 2020 2020 206e  .      ...     n
-0000ea00: 6f69 7365 5f6b 6579 203d 2073 656c 662e  oise_key = self.
-0000ea10: 6d61 6b65 5f72 6e67 2827 6e6f 6973 6527  make_rng('noise'
-0000ea20: 290a 2020 2020 2020 2e2e 2e20 2020 2020  ).      ...     
-0000ea30: 7820 3d20 7820 2b20 6a61 782e 7261 6e64  x = x + jax.rand
-0000ea40: 6f6d 2e6e 6f72 6d61 6c28 6e6f 6973 655f  om.normal(noise_
-0000ea50: 6b65 792c 2078 2e73 6861 7065 290a 2020  key, x.shape).  
-0000ea60: 2020 2020 2e2e 2e0a 2020 2020 2020 2e2e      ....      ..
-0000ea70: 2e20 2020 2020 7265 7475 726e 206e 6e2e  .     return nn.
-0000ea80: 4465 6e73 6528 3129 2878 290a 2020 2020  Dense(1)(x).    
-0000ea90: 2020 2e2e 2e0a 2020 2020 2020 3e3e 3e20    ....      >>> 
-0000eaa0: 6d6f 6475 6c65 203d 2046 6f6f 2829 0a20  module = Foo(). 
-0000eab0: 2020 2020 203e 3e3e 2072 6e67 7320 3d20       >>> rngs = 
-0000eac0: 7b27 7061 7261 6d73 273a 206a 6178 2e72  {'params': jax.r
-0000ead0: 616e 646f 6d2e 5052 4e47 4b65 7928 3029  andom.PRNGKey(0)
-0000eae0: 2c20 276e 6f69 7365 273a 206a 6178 2e72  , 'noise': jax.r
-0000eaf0: 616e 646f 6d2e 5052 4e47 4b65 7928 3129  andom.PRNGKey(1)
-0000eb00: 7d0a 2020 2020 2020 3e3e 3e20 7661 7269  }.      >>> vari
-0000eb10: 6162 6c65 7320 3d20 6d6f 6475 6c65 2e69  ables = module.i
-0000eb20: 6e69 7428 726e 6773 2c20 6a6e 702e 656d  nit(rngs, jnp.em
-0000eb30: 7074 7928 2831 2c20 3729 292c 2074 7261  pty((1, 7)), tra
-0000eb40: 696e 3d46 616c 7365 290a 0a20 2020 204a  in=False)..    J
-0000eb50: 6974 7469 6e67 2060 696e 6974 6020 696e  itting `init` in
-0000eb60: 6974 6961 6c69 7a65 7320 6120 6d6f 6465  itializes a mode
-0000eb70: 6c20 6c61 7a69 6c79 2075 7369 6e67 206f  l lazily using o
-0000eb80: 6e6c 7920 7468 6520 7368 6170 6573 206f  nly the shapes o
-0000eb90: 6620 7468 650a 2020 2020 7072 6f76 6964  f the.    provid
-0000eba0: 6564 2061 7267 756d 656e 7473 2c20 616e  ed arguments, an
-0000ebb0: 6420 6176 6f69 6473 2063 6f6d 7075 7469  d avoids computi
-0000ebc0: 6e67 2074 6865 2066 6f72 7761 7264 2070  ng the forward p
-0000ebd0: 6173 7320 7769 7468 2061 6374 7561 6c0a  ass with actual.
-0000ebe0: 2020 2020 7661 6c75 6573 2e20 4578 616d      values. Exam
-0000ebf0: 706c 653a 3a0a 0a20 2020 2020 203e 3e3e  ple::..      >>>
-0000ec00: 206d 6f64 756c 6520 3d20 6e6e 2e44 656e   module = nn.Den
-0000ec10: 7365 2831 290a 2020 2020 2020 3e3e 3e20  se(1).      >>> 
-0000ec20: 696e 6974 5f6a 6974 203d 206a 6178 2e6a  init_jit = jax.j
-0000ec30: 6974 286d 6f64 756c 652e 696e 6974 290a  it(module.init).
-0000ec40: 2020 2020 2020 3e3e 3e20 7661 7269 6162        >>> variab
-0000ec50: 6c65 7320 3d20 696e 6974 5f6a 6974 286a  les = init_jit(j
-0000ec60: 6178 2e72 616e 646f 6d2e 5052 4e47 4b65  ax.random.PRNGKe
-0000ec70: 7928 3029 2c20 6a6e 702e 656d 7074 7928  y(0), jnp.empty(
-0000ec80: 2831 2c20 3729 2929 0a0a 2020 2020 6060  (1, 7)))..    ``
-0000ec90: 696e 6974 6060 2069 7320 6120 6c69 6768  init`` is a ligh
-0000eca0: 7420 7772 6170 7065 7220 6f76 6572 2060  t wrapper over `
-0000ecb0: 6061 7070 6c79 6060 2c20 736f 206f 7468  `apply``, so oth
-0000ecc0: 6572 2060 6061 7070 6c79 6060 2061 7267  er ``apply`` arg
-0000ecd0: 756d 656e 7473 206c 696b 650a 2020 2020  uments like.    
-0000ece0: 6060 6d65 7468 6f64 6060 2c20 6060 6d75  ``method``, ``mu
-0000ecf0: 7461 626c 6560 602c 2061 6e64 2060 6063  table``, and ``c
-0000ed00: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
-0000ed10: 6174 6573 6060 2061 7265 2061 6c73 6f20  ates`` are also 
-0000ed20: 6176 6169 6c61 626c 652e 0a0a 2020 2020  available...    
-0000ed30: 4172 6773 3a0a 2020 2020 2020 726e 6773  Args:.      rngs
-0000ed40: 3a20 5468 6520 726e 6773 2066 6f72 2074  : The rngs for t
-0000ed50: 6865 2076 6172 6961 626c 6520 636f 6c6c  he variable coll
-0000ed60: 6563 7469 6f6e 732e 0a20 2020 2020 202a  ections..      *
-0000ed70: 6172 6773 3a20 4e61 6d65 6420 6172 6775  args: Named argu
-0000ed80: 6d65 6e74 7320 7061 7373 6564 2074 6f20  ments passed to 
-0000ed90: 7468 6520 696e 6974 2066 756e 6374 696f  the init functio
-0000eda0: 6e2e 0a20 2020 2020 206d 6574 686f 643a  n..      method:
-0000edb0: 2041 6e20 6f70 7469 6f6e 616c 206d 6574   An optional met
-0000edc0: 686f 642e 2049 6620 7072 6f76 6964 6564  hod. If provided
-0000edd0: 2c20 6170 706c 6965 7320 7468 6973 206d  , applies this m
-0000ede0: 6574 686f 642e 2049 6620 6e6f 740a 2020  ethod. If not.  
-0000edf0: 2020 2020 2020 7072 6f76 6964 6564 2c20        provided, 
-0000ee00: 6170 706c 6965 7320 7468 6520 6060 5f5f  applies the ``__
-0000ee10: 6361 6c6c 5f5f 6060 206d 6574 686f 642e  call__`` method.
-0000ee20: 2041 2073 7472 696e 6720 6361 6e20 616c   A string can al
-0000ee30: 736f 2062 650a 2020 2020 2020 2020 7072  so be.        pr
-0000ee40: 6f76 6964 6564 2074 6f20 7370 6563 6966  ovided to specif
-0000ee50: 7920 6120 6d65 7468 6f64 2062 7920 6e61  y a method by na
-0000ee60: 6d65 2e0a 2020 2020 2020 6d75 7461 626c  me..      mutabl
-0000ee70: 653a 2043 616e 2062 6520 626f 6f6c 2c20  e: Can be bool, 
-0000ee80: 7374 722c 206f 7220 6c69 7374 2e20 5370  str, or list. Sp
-0000ee90: 6563 6966 6965 7320 7768 6963 6820 636f  ecifies which co
-0000eea0: 6c6c 6563 7469 6f6e 7320 7368 6f75 6c64  llections should
-0000eeb0: 2062 650a 2020 2020 2020 2020 7472 6561   be.        trea
-0000eec0: 7465 6420 6173 206d 7574 6162 6c65 3a20  ted as mutable: 
-0000eed0: 6060 626f 6f6c 6060 3a20 616c 6c2f 6e6f  ``bool``: all/no
-0000eee0: 2063 6f6c 6c65 6374 696f 6e73 2061 7265   collections are
-0000eef0: 206d 7574 6162 6c65 2e0a 2020 2020 2020   mutable..      
-0000ef00: 2020 6060 7374 7260 603a 2054 6865 206e    ``str``: The n
-0000ef10: 616d 6520 6f66 2061 2073 696e 676c 6520  ame of a single 
-0000ef20: 6d75 7461 626c 6520 636f 6c6c 6563 7469  mutable collecti
-0000ef30: 6f6e 2e20 6060 6c69 7374 6060 3a20 410a  on. ``list``: A.
-0000ef40: 2020 2020 2020 2020 6c69 7374 206f 6620          list of 
-0000ef50: 6e61 6d65 7320 6f66 206d 7574 6162 6c65  names of mutable
-0000ef60: 2063 6f6c 6c65 6374 696f 6e73 2e20 4279   collections. By
-0000ef70: 2064 6566 6175 6c74 2061 6c6c 2063 6f6c   default all col
-0000ef80: 6c65 6374 696f 6e73 0a20 2020 2020 2020  lections.       
-0000ef90: 2065 7863 6570 7420 2269 6e74 6572 6d65   except "interme
-0000efa0: 6469 6174 6573 2220 6172 6520 6d75 7461  diates" are muta
-0000efb0: 626c 652e 0a20 2020 2020 2063 6170 7475  ble..      captu
-0000efc0: 7265 5f69 6e74 6572 6d65 6469 6174 6573  re_intermediates
-0000efd0: 3a20 4966 2060 5472 7565 602c 2063 6170  : If `True`, cap
-0000efe0: 7475 7265 7320 696e 7465 726d 6564 6961  tures intermedia
-0000eff0: 7465 2072 6574 7572 6e20 7661 6c75 6573  te return values
-0000f000: 0a20 2020 2020 2020 206f 6620 616c 6c20  .        of all 
-0000f010: 4d6f 6475 6c65 7320 696e 7369 6465 2074  Modules inside t
-0000f020: 6865 2022 696e 7465 726d 6564 6961 7465  he "intermediate
-0000f030: 7322 2063 6f6c 6c65 6374 696f 6e2e 2042  s" collection. B
-0000f040: 7920 6465 6661 756c 7420 6f6e 6c79 0a20  y default only. 
-0000f050: 2020 2020 2020 2074 6865 2072 6574 7572         the retur
-0000f060: 6e20 7661 6c75 6573 206f 6620 616c 6c20  n values of all 
-0000f070: 6060 5f5f 6361 6c6c 5f5f 6060 206d 6574  ``__call__`` met
-0000f080: 686f 6473 2061 7265 2073 746f 7265 642e  hods are stored.
-0000f090: 2041 2066 756e 6374 696f 6e20 6361 6e0a   A function can.
-0000f0a0: 2020 2020 2020 2020 6265 2070 6173 7365          be passe
-0000f0b0: 6420 746f 2063 6861 6e67 6520 7468 6520  d to change the 
-0000f0c0: 6669 6c74 6572 2062 6568 6176 696f 722e  filter behavior.
-0000f0d0: 2054 6865 2066 696c 7465 7220 6675 6e63   The filter func
-0000f0e0: 7469 6f6e 2074 616b 6573 0a20 2020 2020  tion takes.     
-0000f0f0: 2020 2074 6865 204d 6f64 756c 6520 696e     the Module in
-0000f100: 7374 616e 6365 2061 6e64 206d 6574 686f  stance and metho
-0000f110: 6420 6e61 6d65 2061 6e64 2072 6574 7572  d name and retur
-0000f120: 6e73 2061 2062 6f6f 6c20 696e 6469 6361  ns a bool indica
-0000f130: 7469 6e67 0a20 2020 2020 2020 2077 6865  ting.        whe
-0000f140: 7468 6572 2074 6865 206f 7574 7075 7420  ther the output 
-0000f150: 6f66 2074 6861 7420 6d65 7468 6f64 2069  of that method i
-0000f160: 6e76 6f63 6174 696f 6e20 7368 6f75 6c64  nvocation should
-0000f170: 2062 6520 7374 6f72 6564 2e0a 2020 2020   be stored..    
-0000f180: 2020 2a2a 6b77 6172 6773 3a20 4b65 7977    **kwargs: Keyw
-0000f190: 6f72 6420 6172 6775 6d65 6e74 7320 7061  ord arguments pa
-0000f1a0: 7373 6564 2074 6f20 7468 6520 696e 6974  ssed to the init
-0000f1b0: 2066 756e 6374 696f 6e2e 0a20 2020 2052   function..    R
-0000f1c0: 6574 7572 6e73 3a0a 2020 2020 2020 5468  eturns:.      Th
-0000f1d0: 6520 696e 6974 6961 6c69 7a65 6420 7661  e initialized va
-0000f1e0: 7269 6162 6c65 2064 6963 742e 0a20 2020  riable dict..   
-0000f1f0: 2022 2222 0a20 2020 204d 6f64 756c 652e   """.    Module.
-0000f200: 5f6d 6f64 756c 655f 6368 6563 6b73 2873  _module_checks(s
-0000f210: 656c 6629 0a0a 2020 2020 5f2c 2076 5f6f  elf)..    _, v_o
-0000f220: 7574 203d 2073 656c 662e 696e 6974 5f77  ut = self.init_w
-0000f230: 6974 685f 6f75 7470 7574 280a 2020 2020  ith_output(.    
-0000f240: 2020 2020 726e 6773 2c0a 2020 2020 2020      rngs,.      
-0000f250: 2020 2a61 7267 732c 0a20 2020 2020 2020    *args,.       
-0000f260: 206d 6574 686f 643d 6d65 7468 6f64 2c0a   method=method,.
-0000f270: 2020 2020 2020 2020 6d75 7461 626c 653d          mutable=
-0000f280: 6d75 7461 626c 652c 0a20 2020 2020 2020  mutable,.       
-0000f290: 2063 6170 7475 7265 5f69 6e74 6572 6d65   capture_interme
-0000f2a0: 6469 6174 6573 3d63 6170 7475 7265 5f69  diates=capture_i
-0000f2b0: 6e74 6572 6d65 6469 6174 6573 2c0a 2020  ntermediates,.  
-0000f2c0: 2020 2020 2020 2a2a 6b77 6172 6773 290a        **kwargs).
-0000f2d0: 2020 2020 7265 7475 726e 2076 5f6f 7574      return v_out
-0000f2e0: 0a0a 2020 4074 7261 6365 6261 636b 5f75  ..  @traceback_u
-0000f2f0: 7469 6c2e 6170 695f 626f 756e 6461 7279  til.api_boundary
-0000f300: 0a20 2064 6566 206c 617a 795f 696e 6974  .  def lazy_init
-0000f310: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-0000f320: 2020 726e 6773 3a20 556e 696f 6e5b 5052    rngs: Union[PR
-0000f330: 4e47 4b65 792c 2052 4e47 5365 7175 656e  NGKey, RNGSequen
-0000f340: 6365 735d 2c0a 2020 2020 2020 2020 2020  ces],.          
-0000f350: 202a 6172 6773 2c0a 2020 2020 2020 2020   *args,.        
-0000f360: 2020 206d 6574 686f 643a 204f 7074 696f     method: Optio
-0000f370: 6e61 6c5b 4361 6c6c 6162 6c65 5b2e 2e2e  nal[Callable[...
-0000f380: 2c20 416e 795d 5d20 3d20 4e6f 6e65 2c0a  , Any]] = None,.
-0000f390: 2020 2020 2020 2020 2020 206d 7574 6162             mutab
-0000f3a0: 6c65 3a20 436f 6c6c 6563 7469 6f6e 4669  le: CollectionFi
-0000f3b0: 6c74 6572 203d 2044 656e 794c 6973 7428  lter = DenyList(
-0000f3c0: 2769 6e74 6572 6d65 6469 6174 6573 2729  'intermediates')
-0000f3d0: 2c0a 2020 2020 2020 2020 2020 202a 2a6b  ,.           **k
-0000f3e0: 7761 7267 7329 202d 3e20 4672 6f7a 656e  wargs) -> Frozen
-0000f3f0: 5661 7269 6162 6c65 4469 6374 3a0a 2020  VariableDict:.  
-0000f400: 2020 2222 2249 6e69 7469 616c 697a 6573    """Initializes
-0000f410: 2061 206d 6f64 756c 6520 7769 7468 6f75   a module withou
-0000f420: 7420 636f 6d70 7574 696e 6720 6f6e 2061  t computing on a
-0000f430: 6e20 6163 7475 616c 2069 6e70 7574 2e0a  n actual input..
-0000f440: 0a20 2020 206c 617a 795f 696e 6974 2077  .    lazy_init w
-0000f450: 696c 6c20 696e 6974 6961 6c69 7a65 2074  ill initialize t
-0000f460: 6865 2076 6172 6961 626c 6573 2077 6974  he variables wit
-0000f470: 686f 7574 2064 6f69 6e67 2075 6e6e 6563  hout doing unnec
-0000f480: 6573 7361 7279 2063 6f6d 7075 7465 2e0a  essary compute..
-0000f490: 2020 2020 5468 6520 696e 7075 7420 6461      The input da
-0000f4a0: 7461 2073 686f 756c 6420 6265 2070 6173  ta should be pas
-0000f4b0: 7365 6420 6173 2061 2060 606a 6178 2e53  sed as a ``jax.S
-0000f4c0: 6861 7065 4474 7970 6553 7472 7563 7460  hapeDtypeStruct`
-0000f4d0: 6020 7768 6963 6820 7370 6563 6966 6965  ` which specifie
-0000f4e0: 730a 2020 2020 7468 6520 7368 6170 6520  s.    the shape 
-0000f4f0: 616e 6420 6474 7970 6520 6f66 2074 6865  and dtype of the
-0000f500: 2069 6e70 7574 2062 7574 206e 6f20 636f   input but no co
-0000f510: 6e63 7265 7465 2064 6174 612e 0a0a 2020  ncrete data...  
-0000f520: 2020 4578 616d 706c 653a 3a0a 0a20 2020    Example::..   
-0000f530: 2020 206d 6f64 656c 203d 206e 6e2e 4465     model = nn.De
-0000f540: 6e73 6528 6665 6174 7572 6573 3d32 3536  nse(features=256
-0000f550: 290a 2020 2020 2020 7661 7269 6162 6c65  ).      variable
-0000f560: 7320 3d20 6d6f 6465 6c2e 6c61 7a79 5f69  s = model.lazy_i
-0000f570: 6e69 7428 726e 672c 206a 6178 2e53 6861  nit(rng, jax.Sha
-0000f580: 7065 4474 7970 6553 7472 7563 7428 2831  peDtypeStruct((1
-0000f590: 2c20 3132 3829 2c20 6a6e 702e 666c 6f61  , 128), jnp.floa
-0000f5a0: 7433 3229 290a 0a20 2020 2054 6865 2061  t32))..    The a
-0000f5b0: 7267 7320 616e 6420 6b77 6172 6773 2061  rgs and kwargs a
-0000f5c0: 7267 7320 7061 7373 6564 2074 6f20 6060  rgs passed to ``
-0000f5d0: 6c61 7a79 5f69 6e69 7460 6020 6361 6e20  lazy_init`` can 
-0000f5e0: 6265 2061 206d 6978 206f 660a 2020 2020  be a mix of.    
-0000f5f0: 636f 6e63 7265 7465 2028 6a61 7820 6172  concrete (jax ar
-0000f600: 7261 7973 2c20 7363 616c 6172 732c 2062  rays, scalars, b
-0000f610: 6f6f 6c73 2920 616e 6420 6162 7374 7261  ools) and abstra
-0000f620: 6374 2028 5368 6170 6544 7479 7065 5374  ct (ShapeDtypeSt
-0000f630: 7275 6374 2920 7661 6c75 6573 2e0a 2020  ruct) values..  
-0000f640: 2020 436f 6e63 7265 7465 2076 616c 7565    Concrete value
-0000f650: 7320 6172 6520 6f6e 6c79 206e 6563 6573  s are only neces
-0000f660: 7361 7279 2066 6f72 2061 7267 756d 656e  sary for argumen
-0000f670: 7473 2074 6861 7420 6166 6665 6374 0a20  ts that affect. 
-0000f680: 2020 2074 6865 2069 6e69 7469 616c 697a     the initializ
-0000f690: 6174 696f 6e20 6f66 2076 6172 6961 626c  ation of variabl
-0000f6a0: 6573 2e20 466f 7220 6578 616d 706c 652c  es. For example,
-0000f6b0: 2074 6865 206d 6f64 656c 206d 6967 6874   the model might
-0000f6c0: 2065 7870 6563 740a 2020 2020 6120 6b65   expect.    a ke
-0000f6d0: 7977 6f72 6420 6172 6720 7468 6174 2065  yword arg that e
-0000f6e0: 6e61 626c 6573 2f64 6973 6162 6c65 7320  nables/disables 
-0000f6f0: 6120 7375 6270 6172 7420 6f66 2074 6865  a subpart of the
-0000f700: 206d 6f64 656c 2e0a 2020 2020 496e 2074   model..    In t
-0000f710: 6869 7320 6361 7365 2c20 616e 2065 7870  his case, an exp
-0000f720: 6c69 6369 7420 7661 6c75 6520 2854 7275  licit value (Tru
-0000f730: 652f 466c 6173 6529 2073 686f 756c 6420  e/Flase) should 
-0000f740: 6265 2070 6173 7365 6420 6f74 6865 7277  be passed otherw
-0000f750: 6973 650a 2020 2020 6060 6c61 7a79 5f69  ise.    ``lazy_i
-0000f760: 6e69 7460 6020 6361 6e6e 6f74 2069 6e66  nit`` cannot inf
-0000f770: 6572 2077 6869 6368 2076 6172 6961 626c  er which variabl
-0000f780: 6573 2073 686f 756c 6420 6265 2069 6e69  es should be ini
-0000f790: 7469 616c 697a 6564 2e0a 0a20 2020 2041  tialized...    A
-0000f7a0: 7267 733a 0a20 2020 2020 2072 6e67 733a  rgs:.      rngs:
-0000f7b0: 2054 6865 2072 6e67 7320 666f 7220 7468   The rngs for th
-0000f7c0: 6520 7661 7269 6162 6c65 2063 6f6c 6c65  e variable colle
-0000f7d0: 6374 696f 6e73 2e0a 2020 2020 2020 2a61  ctions..      *a
-0000f7e0: 7267 733a 2061 7267 756d 656e 7473 2070  rgs: arguments p
-0000f7f0: 6173 7365 6420 746f 2074 6865 2069 6e69  assed to the ini
-0000f800: 7420 6675 6e63 7469 6f6e 2e0a 2020 2020  t function..    
-0000f810: 2020 6d65 7468 6f64 3a20 416e 206f 7074    method: An opt
-0000f820: 696f 6e61 6c20 6d65 7468 6f64 2e20 4966  ional method. If
-0000f830: 2070 726f 7669 6465 642c 2061 7070 6c69   provided, appli
-0000f840: 6573 2074 6869 7320 6d65 7468 6f64 2e20  es this method. 
-0000f850: 4966 206e 6f74 0a20 2020 2020 2020 2070  If not.        p
-0000f860: 726f 7669 6465 642c 2061 7070 6c69 6573  rovided, applies
-0000f870: 2074 6865 2060 605f 5f63 616c 6c5f 5f60   the ``__call__`
-0000f880: 6020 6d65 7468 6f64 2e0a 2020 2020 2020  ` method..      
-0000f890: 6d75 7461 626c 653a 2043 616e 2062 6520  mutable: Can be 
-0000f8a0: 626f 6f6c 2c20 7374 722c 206f 7220 6c69  bool, str, or li
-0000f8b0: 7374 2e20 5370 6563 6966 6965 7320 7768  st. Specifies wh
-0000f8c0: 6963 6820 636f 6c6c 6563 7469 6f6e 7320  ich collections 
-0000f8d0: 7368 6f75 6c64 2062 650a 2020 2020 2020  should be.      
-0000f8e0: 2020 7472 6561 7465 6420 6173 206d 7574    treated as mut
-0000f8f0: 6162 6c65 3a20 6060 626f 6f6c 6060 3a20  able: ``bool``: 
-0000f900: 616c 6c2f 6e6f 2063 6f6c 6c65 6374 696f  all/no collectio
-0000f910: 6e73 2061 7265 206d 7574 6162 6c65 2e0a  ns are mutable..
-0000f920: 2020 2020 2020 2020 6060 7374 7260 603a          ``str``:
-0000f930: 2054 6865 206e 616d 6520 6f66 2061 2073   The name of a s
-0000f940: 696e 676c 6520 6d75 7461 626c 6520 636f  ingle mutable co
-0000f950: 6c6c 6563 7469 6f6e 2e20 6060 6c69 7374  llection. ``list
-0000f960: 6060 3a20 410a 2020 2020 2020 2020 6c69  ``: A.        li
-0000f970: 7374 206f 6620 6e61 6d65 7320 6f66 206d  st of names of m
-0000f980: 7574 6162 6c65 2063 6f6c 6c65 6374 696f  utable collectio
-0000f990: 6e73 2e20 4279 2064 6566 6175 6c74 2061  ns. By default a
-0000f9a0: 6c6c 2063 6f6c 6c65 6374 696f 6e73 0a20  ll collections. 
-0000f9b0: 2020 2020 2020 2065 7863 6570 7420 2269         except "i
-0000f9c0: 6e74 6572 6d65 6469 6174 6573 2220 6172  ntermediates" ar
-0000f9d0: 6520 6d75 7461 626c 652e 0a20 2020 2020  e mutable..     
-0000f9e0: 202a 2a6b 7761 7267 733a 204b 6579 776f   **kwargs: Keywo
-0000f9f0: 7264 2061 7267 756d 656e 7473 2070 6173  rd arguments pas
-0000fa00: 7365 6420 746f 2074 6865 2069 6e69 7420  sed to the init 
-0000fa10: 6675 6e63 7469 6f6e 2e0a 2020 2020 5265  function..    Re
-0000fa20: 7475 726e 733a 0a20 2020 2020 2054 6865  turns:.      The
-0000fa30: 2069 6e69 7469 616c 697a 6564 2076 6172   initialized var
-0000fa40: 6961 626c 6520 6469 6374 2e0a 2020 2020  iable dict..    
-0000fa50: 2222 220a 2020 2020 4d6f 6475 6c65 2e5f  """.    Module._
-0000fa60: 6d6f 6475 6c65 5f63 6865 636b 7328 7365  module_checks(se
-0000fa70: 6c66 290a 2020 2020 6465 6620 6c61 7a79  lf).    def lazy
-0000fa80: 5f77 7261 7070 6572 2872 6e67 732c 202a  _wrapper(rngs, *
-0000fa90: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-0000faa0: 0a20 2020 2020 2072 6574 7572 6e20 7365  .      return se
-0000fab0: 6c66 2e69 6e69 7428 726e 6773 2c20 2a61  lf.init(rngs, *a
-0000fac0: 7267 732c 206d 6574 686f 643d 6d65 7468  rgs, method=meth
-0000fad0: 6f64 2c20 6d75 7461 626c 653d 6d75 7461  od, mutable=muta
-0000fae0: 626c 652c 202a 2a6b 7761 7267 7329 0a20  ble, **kwargs). 
-0000faf0: 2020 2072 6574 7572 6e20 7061 7274 6961     return partia
-0000fb00: 6c5f 6576 616c 2e6c 617a 795f 696e 6974  l_eval.lazy_init
-0000fb10: 286c 617a 795f 7772 6170 7065 7229 2872  (lazy_wrapper)(r
-0000fb20: 6e67 732c 202a 6172 6773 2c20 2a2a 6b77  ngs, *args, **kw
-0000fb30: 6172 6773 290a 0a20 2040 7072 6f70 6572  args)..  @proper
-0000fb40: 7479 0a20 2064 6566 2076 6172 6961 626c  ty.  def variabl
-0000fb50: 6573 2873 656c 6629 202d 3e20 5661 7269  es(self) -> Vari
-0000fb60: 6162 6c65 4469 6374 3a0a 2020 2020 2222  ableDict:.    ""
-0000fb70: 2252 6574 7572 6e73 2074 6865 2076 6172  "Returns the var
-0000fb80: 6961 626c 6573 2069 6e20 7468 6973 206d  iables in this m
-0000fb90: 6f64 756c 652e 2222 220a 2020 2020 6966  odule.""".    if
-0000fba0: 2073 656c 662e 7363 6f70 6520 6973 204e   self.scope is N
-0000fbb0: 6f6e 653a 0a20 2020 2020 2072 6169 7365  one:.      raise
-0000fbc0: 2056 616c 7565 4572 726f 7228 2243 616e   ValueError("Can
-0000fbd0: 2774 2061 6363 6573 7320 7661 7269 6162  't access variab
-0000fbe0: 6c65 7320 6f6e 2075 6e62 6f75 6e64 206d  les on unbound m
-0000fbf0: 6f64 756c 6573 2229 0a20 2020 2072 6574  odules").    ret
-0000fc00: 7572 6e20 7365 6c66 2e73 636f 7065 2e76  urn self.scope.v
-0000fc10: 6172 6961 626c 6573 2829 0a0a 2020 6465  ariables()..  de
-0000fc20: 6620 6765 745f 7661 7269 6162 6c65 2873  f get_variable(s
-0000fc30: 656c 662c 2063 6f6c 3a20 7374 722c 206e  elf, col: str, n
-0000fc40: 616d 653a 2073 7472 2c20 6465 6661 756c  ame: str, defaul
-0000fc50: 743a 204f 7074 696f 6e61 6c5b 545d 203d  t: Optional[T] =
-0000fc60: 204e 6f6e 6529 202d 3e20 543a 0a20 2020   None) -> T:.   
-0000fc70: 2022 2222 5265 7472 6965 7665 7320 7468   """Retrieves th
-0000fc80: 6520 7661 6c75 6520 6f66 2061 2056 6172  e value of a Var
-0000fc90: 6961 626c 652e 0a0a 2020 2020 4172 6773  iable...    Args
-0000fca0: 3a0a 2020 2020 2020 636f 6c3a 2074 6865  :.      col: the
-0000fcb0: 2076 6172 6961 626c 6520 636f 6c6c 6563   variable collec
-0000fcc0: 7469 6f6e 2e0a 2020 2020 2020 6e61 6d65  tion..      name
-0000fcd0: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
-0000fce0: 6520 7661 7269 6162 6c65 2e0a 2020 2020  e variable..    
-0000fcf0: 2020 6465 6661 756c 743a 2074 6865 2064    default: the d
-0000fd00: 6566 6175 6c74 2076 616c 7565 2074 6f20  efault value to 
-0000fd10: 7265 7475 726e 2069 6620 7468 6520 7661  return if the va
-0000fd20: 7269 6162 6c65 2064 6f65 7320 6e6f 7420  riable does not 
-0000fd30: 6578 6973 7420 696e 0a20 2020 2020 2020  exist in.       
-0000fd40: 2074 6869 7320 7363 6f70 652e 0a0a 2020   this scope...  
-0000fd50: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000fd60: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
-0000fd70: 6520 696e 7075 7420 7661 7269 6162 6c65  e input variable
-0000fd80: 2c20 6f66 2074 6865 2064 6566 6175 6c74  , of the default
-0000fd90: 2076 616c 7565 2069 6620 7468 6520 7661   value if the va
-0000fda0: 7269 6162 6c65 0a20 2020 2020 2064 6f65  riable.      doe
-0000fdb0: 736e 2774 2065 7869 7374 2069 6e20 7468  sn't exist in th
-0000fdc0: 6973 2073 636f 7065 2e0a 2020 2020 2222  is scope..    ""
-0000fdd0: 220a 2020 2020 6966 2073 656c 662e 7363  ".    if self.sc
-0000fde0: 6f70 6520 6973 204e 6f6e 653a 0a20 2020  ope is None:.   
-0000fdf0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000fe00: 726f 7228 2243 616e 2774 2061 6363 6573  ror("Can't acces
-0000fe10: 7320 7661 7269 6162 6c65 7320 6f6e 2075  s variables on u
-0000fe20: 6e62 6f75 6e64 206d 6f64 756c 6573 2229  nbound modules")
-0000fe30: 0a20 2020 2072 6574 7572 6e20 7365 6c66  .    return self
-0000fe40: 2e73 636f 7065 2e67 6574 5f76 6172 6961  .scope.get_varia
-0000fe50: 626c 6528 636f 6c2c 206e 616d 652c 2064  ble(col, name, d
-0000fe60: 6566 6175 6c74 290a 0a20 2064 6566 2070  efault)..  def p
-0000fe70: 7574 5f76 6172 6961 626c 6528 7365 6c66  ut_variable(self
-0000fe80: 2c20 636f 6c3a 2073 7472 2c20 6e61 6d65  , col: str, name
-0000fe90: 3a20 7374 722c 2076 616c 7565 3a20 416e  : str, value: An
-0000fea0: 7929 3a0a 2020 2020 2222 2255 7064 6174  y):.    """Updat
-0000feb0: 6573 2074 6865 2076 616c 7565 206f 6620  es the value of 
-0000fec0: 7468 6520 6769 7665 6e20 7661 7269 6162  the given variab
-0000fed0: 6c65 2069 6620 6974 2069 7320 6d75 7461  le if it is muta
-0000fee0: 626c 652c 206f 7220 616e 2065 7272 6f72  ble, or an error
-0000fef0: 206f 7468 6572 7769 7365 2e0a 0a20 2020   otherwise...   
-0000ff00: 2041 7267 733a 0a20 2020 2020 2063 6f6c   Args:.      col
-0000ff10: 3a20 7468 6520 7661 7269 6162 6c65 2063  : the variable c
-0000ff20: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-0000ff30: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
-0000ff40: 6f66 2074 6865 2076 6172 6961 626c 652e  of the variable.
-0000ff50: 0a20 2020 2020 2076 616c 7565 3a20 7468  .      value: th
-0000ff60: 6520 6e65 7720 7661 6c75 6520 6f66 2074  e new value of t
-0000ff70: 6865 2076 6172 6961 626c 652e 0a20 2020  he variable..   
-0000ff80: 2022 2222 0a20 2020 2069 6620 7365 6c66   """.    if self
-0000ff90: 2e73 636f 7065 2069 7320 4e6f 6e65 3a0a  .scope is None:.
-0000ffa0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000ffb0: 6545 7272 6f72 2822 4361 6e27 7420 6163  eError("Can't ac
-0000ffc0: 6365 7373 2076 6172 6961 626c 6573 206f  cess variables o
-0000ffd0: 6e20 756e 626f 756e 6420 6d6f 6475 6c65  n unbound module
-0000ffe0: 7322 290a 2020 2020 7365 6c66 2e73 636f  s").    self.sco
-0000fff0: 7065 2e70 7574 5f76 6172 6961 626c 6528  pe.put_variable(
-00010000: 636f 6c2c 206e 616d 652c 2076 616c 7565  col, name, value
-00010010: 290a 0a20 2040 6f76 6572 6c6f 6164 0a20  )..  @overload. 
-00010020: 2064 6566 2073 6f77 2873 656c 662c 2063   def sow(self, c
-00010030: 6f6c 3a20 7374 722c 206e 616d 653a 2073  ol: str, name: s
-00010040: 7472 2c20 7661 6c75 653a 2041 6e79 2920  tr, value: Any) 
-00010050: 2d3e 2062 6f6f 6c3a 0a20 2020 202e 2e2e  -> bool:.    ...
-00010060: 0a0a 2020 406f 7665 726c 6f61 640a 2020  ..  @overload.  
-00010070: 6465 6620 736f 7728 7365 6c66 2c20 636f  def sow(self, co
-00010080: 6c3a 2073 7472 2c20 6e61 6d65 3a20 7374  l: str, name: st
-00010090: 722c 2076 616c 7565 3a20 542c 0a20 2020  r, value: T,.   
-000100a0: 2020 2020 2020 2072 6564 7563 655f 666e         reduce_fn
-000100b0: 3a20 4361 6c6c 6162 6c65 5b5b 4b2c 2054  : Callable[[K, T
-000100c0: 5d2c 204b 5d20 3d20 7475 706c 655f 7265  ], K] = tuple_re
-000100d0: 6475 6365 2c0a 2020 2020 2020 2020 2020  duce,.          
-000100e0: 696e 6974 5f66 6e3a 2043 616c 6c61 626c  init_fn: Callabl
-000100f0: 655b 5b5d 2c20 4b5d 203d 2074 7570 6c65  e[[], K] = tuple
-00010100: 5f69 6e69 7429 202d 3e20 626f 6f6c 3a20  _init) -> bool: 
-00010110: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
-00010120: 2020 202e 2e2e 0a0a 2020 6465 6620 736f     .....  def so
-00010130: 7728 7365 6c66 2c20 636f 6c3a 2073 7472  w(self, col: str
-00010140: 2c20 6e61 6d65 3a20 7374 722c 2076 616c  , name: str, val
-00010150: 7565 3a20 542c 0a20 2020 2020 2020 2020  ue: T,.         
-00010160: 2072 6564 7563 655f 666e 3a20 4361 6c6c   reduce_fn: Call
-00010170: 6162 6c65 5b5b 4b2c 2054 5d2c 204b 5d20  able[[K, T], K] 
-00010180: 3d20 7475 706c 655f 7265 6475 6365 2c0a  = tuple_reduce,.
-00010190: 2020 2020 2020 2020 2020 696e 6974 5f66            init_f
-000101a0: 6e3a 2043 616c 6c61 626c 655b 5b5d 2c20  n: Callable[[], 
-000101b0: 4b5d 203d 2074 7570 6c65 5f69 6e69 7429  K] = tuple_init)
-000101c0: 202d 3e20 626f 6f6c 3a20 2320 7479 7065   -> bool: # type
-000101d0: 3a20 6967 6e6f 7265 0a20 2020 2022 2222  : ignore.    """
-000101e0: 5374 6f72 6573 2061 2076 616c 7565 2069  Stores a value i
-000101f0: 6e20 6120 636f 6c6c 6563 7469 6f6e 2e0a  n a collection..
-00010200: 0a20 2020 2043 6f6c 6c65 6374 696f 6e73  .    Collections
-00010210: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00010220: 636f 6c6c 6563 7420 696e 7465 726d 6564  collect intermed
-00010230: 6961 7465 2076 616c 7565 7320 7769 7468  iate values with
-00010240: 6f75 740a 2020 2020 7468 6520 6f76 6572  out.    the over
-00010250: 6865 6164 206f 6620 6578 706c 6963 6974  head of explicit
-00010260: 6c79 2070 6173 7369 6e67 2061 2063 6f6e  ly passing a con
-00010270: 7461 696e 6572 2074 6872 6f75 6768 2065  tainer through e
-00010280: 6163 6820 4d6f 6475 6c65 2063 616c 6c2e  ach Module call.
-00010290: 0a0a 2020 2020 4966 2074 6865 2074 6172  ..    If the tar
-000102a0: 6765 7420 636f 6c6c 6563 7469 6f6e 2069  get collection i
-000102b0: 7320 6e6f 7420 6d75 7461 626c 6520 6073  s not mutable `s
-000102c0: 6f77 6020 6265 6861 7665 7320 6c69 6b65  ow` behaves like
-000102d0: 2061 206e 6f2d 6f70 0a20 2020 2061 6e64   a no-op.    and
-000102e0: 2072 6574 7572 6e73 2060 4661 6c73 6560   returns `False`
-000102f0: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a3a  ...    Example::
-00010300: 0a0a 2020 2020 2020 696d 706f 7274 206a  ..      import j
-00010310: 6178 0a20 2020 2020 2069 6d70 6f72 7420  ax.      import 
-00010320: 6a61 782e 6e75 6d70 7920 6173 206a 6e70  jax.numpy as jnp
-00010330: 0a20 2020 2020 2069 6d70 6f72 7420 666c  .      import fl
-00010340: 6178 2e6c 696e 656e 2061 7320 6e6e 0a0a  ax.linen as nn..
-00010350: 2020 2020 2020 636c 6173 7320 466f 6f28        class Foo(
-00010360: 6e6e 2e4d 6f64 756c 6529 3a0a 2020 2020  nn.Module):.    
-00010370: 2020 2020 406e 6e2e 636f 6d70 6163 740a      @nn.compact.
-00010380: 2020 2020 2020 2020 6465 6620 5f5f 6361          def __ca
-00010390: 6c6c 5f5f 2873 656c 662c 2078 293a 0a20  ll__(self, x):. 
-000103a0: 2020 2020 2020 2020 2068 203d 206e 6e2e           h = nn.
-000103b0: 4465 6e73 6528 3429 2878 290a 2020 2020  Dense(4)(x).    
-000103c0: 2020 2020 2020 7365 6c66 2e73 6f77 2827        self.sow('
-000103d0: 696e 7465 726d 6564 6961 7465 7327 2c20  intermediates', 
-000103e0: 2768 272c 2068 290a 2020 2020 2020 2020  'h', h).        
-000103f0: 2020 7265 7475 726e 206e 6e2e 4465 6e73    return nn.Dens
-00010400: 6528 3229 2868 290a 0a20 2020 2020 2078  e(2)(h)..      x
-00010410: 203d 206a 6e70 2e6f 6e65 7328 2831 362c   = jnp.ones((16,
-00010420: 2039 2929 0a20 2020 2020 206d 6f64 656c   9)).      model
-00010430: 203d 2046 6f6f 2829 0a20 2020 2020 2076   = Foo().      v
-00010440: 6172 6961 626c 6573 203d 206d 6f64 656c  ariables = model
-00010450: 2e69 6e69 7428 6a61 782e 7261 6e64 6f6d  .init(jax.random
-00010460: 2e50 524e 474b 6579 2830 292c 2078 290a  .PRNGKey(0), x).
-00010470: 2020 2020 2020 792c 2073 7461 7465 203d        y, state =
-00010480: 206d 6f64 656c 2e61 7070 6c79 2876 6172   model.apply(var
-00010490: 6961 626c 6573 2c20 782c 206d 7574 6162  iables, x, mutab
-000104a0: 6c65 3d5b 2769 6e74 6572 6d65 6469 6174  le=['intermediat
-000104b0: 6573 275d 290a 2020 2020 2020 7072 696e  es']).      prin
-000104c0: 7428 7374 6174 655b 2769 6e74 6572 6d65  t(state['interme
-000104d0: 6469 6174 6573 275d 2920 2023 207b 2768  diates'])  # {'h
-000104e0: 273a 2028 2e2e 2e2c 297d 0a0a 2020 2020  ': (...,)}..    
-000104f0: 4279 2064 6566 6175 6c74 2074 6865 2076  By default the v
-00010500: 616c 7565 7320 6172 6520 7374 6f72 6564  alues are stored
-00010510: 2069 6e20 6120 7475 706c 6520 616e 6420   in a tuple and 
-00010520: 6561 6368 2073 746f 7265 6420 7661 6c75  each stored valu
-00010530: 650a 2020 2020 6973 2061 7070 656e 6465  e.    is appende
-00010540: 6420 6174 2074 6865 2065 6e64 2e20 5468  d at the end. Th
-00010550: 6973 2077 6179 2061 6c6c 2069 6e74 6572  is way all inter
-00010560: 6d65 6469 6174 6573 2063 616e 2062 6520  mediates can be 
-00010570: 7472 6163 6b65 6420 7768 656e 0a20 2020  tracked when.   
-00010580: 2074 6865 2073 616d 6520 6d6f 6475 6c65   the same module
-00010590: 2069 7320 6361 6c6c 6564 206d 756c 7469   is called multi
-000105a0: 706c 6520 7469 6d65 732e 2041 6c74 6572  ple times. Alter
-000105b0: 6e61 7469 7665 6c79 2c20 6120 6375 7374  natively, a cust
-000105c0: 6f6d 0a20 2020 2069 6e69 742f 7265 6475  om.    init/redu
-000105d0: 6365 2066 756e 6374 696f 6e20 6361 6e20  ce function can 
-000105e0: 6265 2070 6173 7365 643a 3a0a 0a20 2020  be passed::..   
-000105f0: 2020 2063 6c61 7373 2046 6f6f 3228 6e6e     class Foo2(nn
-00010600: 2e4d 6f64 756c 6529 3a0a 2020 2020 2020  .Module):.      
-00010610: 2020 406e 6e2e 636f 6d70 6163 740a 2020    @nn.compact.  
-00010620: 2020 2020 2020 6465 6620 5f5f 6361 6c6c        def __call
-00010630: 5f5f 2873 656c 662c 2078 293a 0a20 2020  __(self, x):.   
-00010640: 2020 2020 2020 2069 6e69 745f 666e 203d         init_fn =
-00010650: 206c 616d 6264 613a 2030 0a20 2020 2020   lambda: 0.     
-00010660: 2020 2020 2072 6564 7563 655f 666e 203d       reduce_fn =
-00010670: 206c 616d 6264 6120 612c 2062 3a20 6120   lambda a, b: a 
-00010680: 2b20 620a 2020 2020 2020 2020 2020 7365  + b.          se
-00010690: 6c66 2e73 6f77 2827 696e 7465 726d 6564  lf.sow('intermed
-000106a0: 6961 7465 7327 2c20 2768 272c 2078 2c0a  iates', 'h', x,.
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2069 6e69 745f 666e 3d69 6e69 745f     init_fn=init_
-000106d0: 666e 2c20 7265 6475 6365 5f66 6e3d 7265  fn, reduce_fn=re
-000106e0: 6475 6365 5f66 6e29 0a20 2020 2020 2020  duce_fn).       
-000106f0: 2020 2073 656c 662e 736f 7728 2769 6e74     self.sow('int
-00010700: 6572 6d65 6469 6174 6573 272c 2027 6827  ermediates', 'h'
-00010710: 2c20 7820 2a20 322c 0a20 2020 2020 2020  , x * 2,.       
-00010720: 2020 2020 2020 2020 2020 2020 696e 6974              init
-00010730: 5f66 6e3d 696e 6974 5f66 6e2c 2072 6564  _fn=init_fn, red
-00010740: 7563 655f 666e 3d72 6564 7563 655f 666e  uce_fn=reduce_fn
-00010750: 290a 2020 2020 2020 2020 2020 7265 7475  ).          retu
-00010760: 726e 2078 0a0a 2020 2020 2020 6d6f 6465  rn x..      mode
-00010770: 6c20 3d20 466f 6f32 2829 0a20 2020 2020  l = Foo2().     
-00010780: 2076 6172 6961 626c 6573 203d 206d 6f64   variables = mod
-00010790: 656c 2e69 6e69 7428 6a61 782e 7261 6e64  el.init(jax.rand
-000107a0: 6f6d 2e50 524e 474b 6579 2830 292c 2078  om.PRNGKey(0), x
-000107b0: 290a 2020 2020 2020 792c 2073 7461 7465  ).      y, state
-000107c0: 203d 206d 6f64 656c 2e61 7070 6c79 2876   = model.apply(v
-000107d0: 6172 6961 626c 6573 2c20 6a6e 702e 6f6e  ariables, jnp.on
-000107e0: 6573 2828 312c 2031 2929 2c20 6d75 7461  es((1, 1)), muta
-000107f0: 626c 653d 5b27 696e 7465 726d 6564 6961  ble=['intermedia
-00010800: 7465 7327 5d29 0a20 2020 2020 2070 7269  tes']).      pri
-00010810: 6e74 2873 7461 7465 5b27 696e 7465 726d  nt(state['interm
-00010820: 6564 6961 7465 7327 5d29 2020 2320 3d3d  ediates'])  # ==
-00010830: 3e20 7b27 6827 3a20 5b5b 332e 5d5d 7d0a  > {'h': [[3.]]}.
-00010840: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00010850: 2063 6f6c 3a20 5468 6520 6e61 6d65 206f   col: The name o
-00010860: 6620 7468 6520 7661 7269 6162 6c65 2063  f the variable c
-00010870: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00010880: 206e 616d 653a 2054 6865 206e 616d 6520   name: The name 
-00010890: 6f66 2074 6865 2076 6172 6961 626c 652e  of the variable.
-000108a0: 0a20 2020 2020 2076 616c 7565 3a20 5468  .      value: Th
-000108b0: 6520 7661 6c75 6520 6f66 2074 6865 2076  e value of the v
-000108c0: 6172 6961 626c 652e 0a20 2020 2020 2072  ariable..      r
-000108d0: 6564 7563 655f 666e 3a20 5468 6520 6675  educe_fn: The fu
-000108e0: 6e63 7469 6f6e 2075 7365 6420 746f 2063  nction used to c
-000108f0: 6f6d 6269 6e65 2074 6865 2065 7869 7374  ombine the exist
-00010900: 696e 6720 7661 6c75 6520 7769 7468 0a20  ing value with. 
-00010910: 2020 2020 2020 2074 6865 206e 6577 2076         the new v
-00010920: 616c 7565 2e20 5468 6520 6465 6661 756c  alue. The defaul
-00010930: 7420 6973 2074 6f20 6170 7065 6e64 2074  t is to append t
-00010940: 6865 2076 616c 7565 2074 6f20 6120 7475  he value to a tu
-00010950: 706c 652e 0a20 2020 2020 2069 6e69 745f  ple..      init_
-00010960: 666e 3a20 466f 7220 7468 6520 6669 7273  fn: For the firs
-00010970: 7420 7661 6c75 6520 7374 6f72 6564 2c20  t value stored, 
-00010980: 6072 6564 7563 655f 666e 6020 7769 6c6c  `reduce_fn` will
-00010990: 2062 6520 7061 7373 6564 0a20 2020 2020   be passed.     
-000109a0: 2020 2074 6865 2072 6573 756c 7420 6f66     the result of
-000109b0: 2060 696e 6974 5f66 6e60 2074 6f67 6574   `init_fn` toget
-000109c0: 6865 7220 7769 7468 2074 6865 2076 616c  her with the val
-000109d0: 7565 2074 6f20 6265 2073 746f 7265 642e  ue to be stored.
-000109e0: 0a20 2020 2020 2020 2054 6865 2064 6566  .        The def
-000109f0: 6175 6c74 2069 7320 616e 2065 6d70 7479  ault is an empty
-00010a00: 2074 7570 6c65 2e0a 0a20 2020 2052 6574   tuple...    Ret
-00010a10: 7572 6e73 3a0a 2020 2020 2020 6054 7275  urns:.      `Tru
-00010a20: 6560 2069 6620 7468 6520 7661 6c75 6520  e` if the value 
-00010a30: 6861 7320 6265 656e 2073 746f 7265 6420  has been stored 
-00010a40: 7375 6363 6573 7366 756c 6c79 2c20 6046  successfully, `F
-00010a50: 616c 7365 6020 6f74 6865 7277 6973 652e  alse` otherwise.
-00010a60: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-00010a70: 7365 6c66 2e73 636f 7065 2069 7320 4e6f  self.scope is No
-00010a80: 6e65 3a0a 2020 2020 2020 7261 6973 6520  ne:.      raise 
-00010a90: 5661 6c75 6545 7272 6f72 2822 4361 6e27  ValueError("Can'
-00010aa0: 7420 7374 6f72 6520 7661 7269 6162 6c65  t store variable
-00010ab0: 7320 6f6e 2075 6e62 6f75 6e64 206d 6f64  s on unbound mod
-00010ac0: 756c 6573 2229 0a20 2020 2069 6620 6e6f  ules").    if no
-00010ad0: 7420 7365 6c66 2e73 636f 7065 2e69 735f  t self.scope.is_
-00010ae0: 6d75 7461 626c 655f 636f 6c6c 6563 7469  mutable_collecti
-00010af0: 6f6e 2863 6f6c 293a 0a20 2020 2020 2072  on(col):.      r
-00010b00: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00010b10: 6966 2073 656c 662e 7363 6f70 652e 6861  if self.scope.ha
-00010b20: 735f 7661 7269 6162 6c65 2863 6f6c 2c20  s_variable(col, 
-00010b30: 6e61 6d65 293a 0a20 2020 2020 2078 7320  name):.      xs 
-00010b40: 3d20 7365 6c66 2e73 636f 7065 2e67 6574  = self.scope.get
-00010b50: 5f76 6172 6961 626c 6528 636f 6c2c 206e  _variable(col, n
-00010b60: 616d 6529 0a20 2020 2065 6c73 653a 0a20  ame).    else:. 
-00010b70: 2020 2020 2073 656c 662e 7363 6f70 652e       self.scope.
-00010b80: 7265 7365 7276 6528 6e61 6d65 290a 2020  reserve(name).  
-00010b90: 2020 2020 7365 6c66 2e5f 7374 6174 652e      self._state.
-00010ba0: 6368 696c 6472 656e 5b6e 616d 655d 203d  children[name] =
-00010bb0: 2063 6f6c 0a20 2020 2020 2078 7320 3d20   col.      xs = 
-00010bc0: 696e 6974 5f66 6e28 290a 2020 2020 7873  init_fn().    xs
-00010bd0: 203d 2072 6564 7563 655f 666e 2878 732c   = reduce_fn(xs,
-00010be0: 2076 616c 7565 290a 2020 2020 7365 6c66   value).    self
-00010bf0: 2e73 636f 7065 2e70 7574 5f76 6172 6961  .scope.put_varia
-00010c00: 626c 6528 636f 6c2c 206e 616d 652c 2078  ble(col, name, x
-00010c10: 7329 0a20 2020 2072 6574 7572 6e20 5472  s).    return Tr
-00010c20: 7565 0a0a 2020 6465 6620 7065 7274 7572  ue..  def pertur
-00010c30: 6228 7365 6c66 2c20 6e61 6d65 3a20 7374  b(self, name: st
-00010c40: 722c 2076 616c 7565 3a20 542c 2063 6f6c  r, value: T, col
-00010c50: 6c65 6374 696f 6e3a 2073 7472 203d 2027  lection: str = '
-00010c60: 7065 7274 7572 6261 7469 6f6e 7327 2920  perturbations') 
-00010c70: 2d3e 2054 3a0a 2020 2020 2222 2241 6464  -> T:.    """Add
-00010c80: 2061 6e20 7a65 726f 2d76 616c 7565 2076   an zero-value v
-00010c90: 6172 6961 626c 6520 2827 7065 7274 7572  ariable ('pertur
-00010ca0: 6261 7469 6f6e 2729 2074 6f20 7468 6520  bation') to the 
-00010cb0: 696e 7465 726d 6564 6961 7465 2076 616c  intermediate val
-00010cc0: 7565 2e0a 0a20 2020 2054 6865 2067 7261  ue...    The gra
-00010cd0: 6469 656e 7420 6f66 2060 7661 6c75 6560  dient of `value`
-00010ce0: 2077 6f75 6c64 2062 6520 7468 6520 7361   would be the sa
-00010cf0: 6d65 2061 7320 7468 6520 6772 6164 6965  me as the gradie
-00010d00: 6e74 206f 6620 7468 6973 0a20 2020 2070  nt of this.    p
-00010d10: 6572 7475 7262 6174 696f 6e20 7661 7269  erturbation vari
-00010d20: 6162 6c65 2e20 5468 6572 6566 6f72 652c  able. Therefore,
-00010d30: 2069 6620 796f 7520 6465 6669 6e65 2079   if you define y
-00010d40: 6f75 7220 6c6f 7373 2066 756e 6374 696f  our loss functio
-00010d50: 6e20 7769 7468 0a20 2020 2062 6f74 6820  n with.    both 
-00010d60: 7061 7261 6d73 2061 6e64 2070 6572 7475  params and pertu
-00010d70: 7262 6174 696f 6e73 2061 7320 7374 616e  rbations as stan
-00010d80: 6461 6c6f 6e65 2061 7267 756d 656e 7473  dalone arguments
-00010d90: 2c20 796f 7520 6361 6e20 6765 7420 7468  , you can get th
-00010da0: 650a 2020 2020 696e 7465 726d 6564 6961  e.    intermedia
-00010db0: 7465 2067 7261 6469 656e 7473 206f 6620  te gradients of 
-00010dc0: 6076 616c 7565 6020 6279 2072 756e 6e69  `value` by runni
-00010dd0: 6e67 2060 6a61 782e 6772 6164 6020 6f6e  ng `jax.grad` on
-00010de0: 2074 6865 2070 6572 7475 7262 6174 696f   the perturbatio
-00010df0: 6e0a 2020 2020 6172 6775 6d65 6e74 2e0a  n.    argument..
-00010e00: 0a20 2020 204e 6f74 653a 2074 6869 7320  .    Note: this 
-00010e10: 6973 2061 6e20 6578 7065 7269 6d65 6e74  is an experiment
-00010e20: 616c 2041 5049 2061 6e64 206d 6179 2062  al API and may b
-00010e30: 6520 7477 6561 6b65 6420 6c61 7465 7220  e tweaked later 
-00010e40: 666f 7220 6265 7474 6572 0a20 2020 2070  for better.    p
-00010e50: 6572 666f 726d 616e 6365 2061 6e64 2075  erformance and u
-00010e60: 7361 6269 6c69 7479 2e0a 2020 2020 4174  sability..    At
-00010e70: 2069 7473 2063 7572 7265 6e74 2073 7461   its current sta
-00010e80: 6765 2c20 6974 2063 7265 6174 6573 2065  ge, it creates e
-00010e90: 7874 7261 2064 756d 6d79 2076 6172 6961  xtra dummy varia
-00010ea0: 626c 6573 2074 6861 7420 6f63 6375 7069  bles that occupi
-00010eb0: 6573 2065 7874 7261 0a20 2020 206d 656d  es extra.    mem
-00010ec0: 6f72 7920 7370 6163 652e 2055 7365 2069  ory space. Use i
-00010ed0: 7420 6f6e 6c79 2074 6f20 6465 6275 6720  t only to debug 
-00010ee0: 6772 6164 6965 6e74 7320 696e 2074 7261  gradients in tra
-00010ef0: 696e 696e 672e 0a0a 2020 2020 4578 616d  ining...    Exam
-00010f00: 706c 653a 3a0a 0a20 2020 2020 2069 6d70  ple::..      imp
-00010f10: 6f72 7420 6a61 780a 2020 2020 2020 696d  ort jax.      im
-00010f20: 706f 7274 206a 6178 2e6e 756d 7079 2061  port jax.numpy a
-00010f30: 7320 6a6e 700a 2020 2020 2020 696d 706f  s jnp.      impo
-00010f40: 7274 2066 6c61 782e 6c69 6e65 6e20 6173  rt flax.linen as
-00010f50: 206e 6e0a 0a20 2020 2020 2063 6c61 7373   nn..      class
-00010f60: 2046 6f6f 286e 6e2e 4d6f 6475 6c65 293a   Foo(nn.Module):
-00010f70: 0a20 2020 2020 2020 2020 2040 6e6e 2e63  .          @nn.c
-00010f80: 6f6d 7061 6374 0a20 2020 2020 2020 2020  ompact.         
-00010f90: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
-00010fa0: 6c66 2c20 7829 3a0a 2020 2020 2020 2020  lf, x):.        
-00010fb0: 2020 2020 2020 7820 3d20 6e6e 2e44 656e        x = nn.Den
-00010fc0: 7365 2833 2928 7829 0a20 2020 2020 2020  se(3)(x).       
-00010fd0: 2020 2020 2020 2078 203d 2073 656c 662e         x = self.
-00010fe0: 7065 7274 7572 6228 2764 656e 7365 3327  perturb('dense3'
-00010ff0: 2c20 7829 0a20 2020 2020 2020 2020 2020  , x).           
-00011000: 2020 2072 6574 7572 6e20 6e6e 2e44 656e     return nn.Den
-00011010: 7365 2832 2928 7829 0a0a 2020 2020 2020  se(2)(x)..      
-00011020: 6465 6620 6c6f 7373 2870 6172 616d 732c  def loss(params,
-00011030: 2070 6572 7475 7262 6174 696f 6e73 2c20   perturbations, 
-00011040: 696e 7075 7473 2c20 7461 7267 6574 7329  inputs, targets)
-00011050: 3a0a 2020 2020 2020 2020 7661 7269 6162  :.        variab
-00011060: 6c65 7320 3d20 7b27 7061 7261 6d73 273a  les = {'params':
-00011070: 2070 6172 616d 732c 2027 7065 7274 7572   params, 'pertur
-00011080: 6261 7469 6f6e 7327 3a20 7065 7274 7572  bations': pertur
-00011090: 6261 7469 6f6e 737d 0a20 2020 2020 2020  bations}.       
-000110a0: 2070 7265 6473 203d 206d 6f64 656c 2e61   preds = model.a
-000110b0: 7070 6c79 2876 6172 6961 626c 6573 2c20  pply(variables, 
-000110c0: 696e 7075 7473 290a 2020 2020 2020 2020  inputs).        
-000110d0: 7265 7475 726e 206a 6e70 2e73 7175 6172  return jnp.squar
-000110e0: 6528 7072 6564 7320 2d20 7461 7267 6574  e(preds - target
-000110f0: 7329 2e6d 6561 6e28 290a 0a20 2020 2020  s).mean()..     
-00011100: 2078 203d 206a 6e70 2e6f 6e65 7328 2832   x = jnp.ones((2
-00011110: 2c20 3929 290a 2020 2020 2020 7920 3d20  , 9)).      y = 
-00011120: 6a6e 702e 6f6e 6573 2828 322c 2032 2929  jnp.ones((2, 2))
-00011130: 0a20 2020 2020 206d 6f64 656c 203d 2046  .      model = F
-00011140: 6f6f 2829 0a20 2020 2020 2076 6172 6961  oo().      varia
-00011150: 626c 6573 203d 206d 6f64 656c 2e69 6e69  bles = model.ini
-00011160: 7428 6a61 782e 7261 6e64 6f6d 2e50 524e  t(jax.random.PRN
-00011170: 474b 6579 2830 292c 2078 290a 2020 2020  GKey(0), x).    
-00011180: 2020 696e 746d 5f67 7261 6473 203d 206a    intm_grads = j
-00011190: 6178 2e67 7261 6428 6c6f 7373 2c20 6172  ax.grad(loss, ar
-000111a0: 676e 756d 733d 3129 2876 6172 6961 626c  gnums=1)(variabl
-000111b0: 6573 5b27 7061 7261 6d73 275d 2c20 7661  es['params'], va
-000111c0: 7269 6162 6c65 735b 2770 6572 7475 7262  riables['perturb
-000111d0: 6174 696f 6e73 275d 2c20 782c 2079 290a  ations'], x, y).
-000111e0: 2020 2020 2020 7072 696e 7428 696e 746d        print(intm
-000111f0: 5f67 7261 6473 5b27 6465 6e73 6533 275d  _grads['dense3']
-00011200: 2920 2320 3d3d 3e20 5b5b 2d31 2e34 3536  ) # ==> [[-1.456
-00011210: 3932 3420 2020 2d30 2e34 3433 3332 3533  924   -0.4433253
-00011220: 3720 2030 2e30 3234 3232 3834 375d 0a20  7  0.02422847]. 
-00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011250: 2023 2020 2020 2020 5b2d 312e 3435 3639   #      [-1.4569
-00011260: 3234 2020 202d 302e 3434 3333 3235 3337  24   -0.44332537
-00011270: 2020 302e 3032 3432 3238 3437 5d5d 0a0a    0.02422847]]..
-00011280: 2020 2020 4966 2070 6572 7475 7262 6174      If perturbat
-00011290: 696f 6e73 2061 7265 206e 6f74 2070 6173  ions are not pas
-000112a0: 7365 6420 746f 2060 6170 706c 7960 2c20  sed to `apply`, 
-000112b0: 6070 6572 7475 7262 6020 6265 6861 7665  `perturb` behave
-000112c0: 7320 6c69 6b65 2061 206e 6f2d 6f70 0a20  s like a no-op. 
-000112d0: 2020 2073 6f20 796f 7520 6361 6e20 6561     so you can ea
-000112e0: 7369 6c79 2064 6973 6162 6c65 2074 6865  sily disable the
-000112f0: 2062 6568 6176 696f 7220 7768 656e 206e   behavior when n
-00011300: 6f74 206e 6565 6465 643a 3a0a 0a20 2020  ot needed::..   
-00011310: 2020 206d 6f64 656c 2e61 7070 6c79 287b     model.apply({
-00011320: 2770 6172 616d 7327 3a20 7061 7261 6d73  'params': params
-00011330: 2c20 2770 6572 7475 7262 6174 696f 6e73  , 'perturbations
-00011340: 273a 2070 6572 7475 7262 6174 696f 6e73  ': perturbations
-00011350: 7d2c 2078 2920 2320 776f 726b 7320 6173  }, x) # works as
-00011360: 2065 7870 6563 7465 640a 2020 2020 2020   expected.      
-00011370: 6d6f 6465 6c2e 6170 706c 7928 7b27 7061  model.apply({'pa
-00011380: 7261 6d73 273a 2070 6172 616d 737d 2c20  rams': params}, 
-00011390: 7829 2023 2062 6568 6176 6573 206c 696b  x) # behaves lik
-000113a0: 6520 6120 6e6f 2d6f 700a 0a20 2020 2022  e a no-op..    "
-000113b0: 2222 0a20 2020 2064 6566 205f 726f 6f74  "".    def _root
-000113c0: 5f68 6173 5f63 6f6c 6c65 6374 696f 6e28  _has_collection(
-000113d0: 293a 0a20 2020 2020 2022 2222 5265 7475  ):.      """Retu
-000113e0: 726e 7320 5472 7565 2069 6620 7468 6520  rns True if the 
-000113f0: 726f 6f74 2073 636f 7065 2068 6173 2074  root scope has t
-00011400: 6865 2063 6f6c 6c65 6374 696f 6e2e 2222  he collection.""
-00011410: 220a 2020 2020 2020 6173 7365 7274 2073  ".      assert s
-00011420: 656c 662e 7363 6f70 6520 6973 206e 6f74  elf.scope is not
-00011430: 204e 6f6e 650a 2020 2020 2020 7265 7475   None.      retu
-00011440: 726e 2063 6f6c 6c65 6374 696f 6e20 696e  rn collection in
-00011450: 2073 656c 662e 7363 6f70 652e 726f 6f74   self.scope.root
-00011460: 2e5f 7661 7269 6162 6c65 730a 2020 2020  ._variables.    
-00011470: 2320 7765 2077 696c 6c20 6f6e 6c79 2061  # we will only a
-00011480: 6464 2074 6865 2070 6572 7475 7262 6174  dd the perturbat
-00011490: 696f 6e20 7661 7269 6162 6c65 2069 6620  ion variable if 
-000114a0: 7468 6520 636f 6c6c 6563 7469 6f6e 2069  the collection i
-000114b0: 7320 6d75 7461 626c 650a 2020 2020 2320  s mutable.    # 
-000114c0: 2865 2e67 2e20 6475 7269 6e67 2060 696e  (e.g. during `in
-000114d0: 6974 6029 206f 7220 6966 2074 6865 2063  it`) or if the c
-000114e0: 6f6c 6c65 6374 696f 6e20 7761 7320 7061  ollection was pa
-000114f0: 7373 6564 2074 6f20 6061 7070 6c79 6020  ssed to `apply` 
-00011500: 2863 6f6e 7461 696e 6564 2069 6e0a 2020  (contained in.  
-00011510: 2020 2320 7468 6520 726f 6f74 2073 636f    # the root sco
-00011520: 7065 292e 0a20 2020 2069 6620 7365 6c66  pe)..    if self
-00011530: 2e69 735f 6d75 7461 626c 655f 636f 6c6c  .is_mutable_coll
-00011540: 6563 7469 6f6e 2863 6f6c 6c65 6374 696f  ection(collectio
-00011550: 6e29 206f 7220 5f72 6f6f 745f 6861 735f  n) or _root_has_
-00011560: 636f 6c6c 6563 7469 6f6e 2829 3a0a 2020  collection():.  
-00011570: 2020 2020 7661 6c75 6520 2b3d 2073 656c      value += sel
-00011580: 662e 7661 7269 6162 6c65 2863 6f6c 6c65  f.variable(colle
-00011590: 6374 696f 6e2c 206e 616d 652c 206c 616d  ction, name, lam
-000115a0: 6264 613a 206a 6e70 2e7a 6572 6f73 5f6c  bda: jnp.zeros_l
-000115b0: 696b 6528 7661 6c75 6529 292e 7661 6c75  ike(value)).valu
-000115c0: 6520 2320 7479 7065 3a20 6967 6e6f 7265  e # type: ignore
-000115d0: 0a20 2020 2072 6574 7572 6e20 7661 6c75  .    return valu
-000115e0: 650a 0a20 2064 6566 2074 6162 756c 6174  e..  def tabulat
-000115f0: 6528 0a20 2020 2073 656c 662c 0a20 2020  e(.    self,.   
-00011600: 2072 6e67 733a 2055 6e69 6f6e 5b50 524e   rngs: Union[PRN
-00011610: 474b 6579 2c20 524e 4753 6571 7565 6e63  GKey, RNGSequenc
-00011620: 6573 5d2c 0a20 2020 202a 6172 6773 2c0a  es],.    *args,.
-00011630: 2020 2020 6465 7074 683a 204f 7074 696f      depth: Optio
-00011640: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-00011650: 0a20 2020 2073 686f 775f 7265 7065 6174  .    show_repeat
-00011660: 6564 3a20 626f 6f6c 203d 2046 616c 7365  ed: bool = False
-00011670: 2c0a 2020 2020 6d75 7461 626c 653a 2043  ,.    mutable: C
-00011680: 6f6c 6c65 6374 696f 6e46 696c 7465 7220  ollectionFilter 
-00011690: 3d20 5472 7565 2c0a 2020 2020 636f 6e73  = True,.    cons
-000116a0: 6f6c 655f 6b77 6172 6773 3a20 4f70 7469  ole_kwargs: Opti
-000116b0: 6f6e 616c 5b4d 6170 7069 6e67 5b73 7472  onal[Mapping[str
-000116c0: 2c20 416e 795d 5d20 3d20 4e6f 6e65 2c0a  , Any]] = None,.
-000116d0: 2020 2020 2a2a 6b77 6172 6773 2920 2d3e      **kwargs) ->
-000116e0: 2073 7472 3a0a 2020 2020 2222 2243 7265   str:.    """Cre
-000116f0: 6174 6573 2061 2073 756d 6d61 7279 206f  ates a summary o
-00011700: 6620 7468 6520 4d6f 6475 6c65 2072 6570  f the Module rep
-00011710: 7265 7365 6e74 6564 2061 7320 6120 7461  resented as a ta
-00011720: 626c 652e 0a0a 2020 2020 5468 6973 206d  ble...    This m
-00011730: 6574 686f 6420 6861 7320 7468 6520 7361  ethod has the sa
-00011740: 6d65 2073 6967 6e61 7475 7265 2061 6e64  me signature and
-00011750: 2069 6e74 6572 6e61 6c6c 7920 6361 6c6c   internally call
-00011760: 7320 604d 6f64 756c 652e 696e 6974 602c  s `Module.init`,
-00011770: 0a20 2020 2062 7574 2069 6e73 7465 6164  .    but instead
-00011780: 206f 6620 7265 7475 726e 696e 6720 7468   of returning th
-00011790: 6520 7661 7269 6162 6c65 732c 2069 7420  e variables, it 
-000117a0: 7265 7475 726e 7320 7468 6520 7374 7269  returns the stri
-000117b0: 6e67 2073 756d 6d61 7269 7a69 6e67 0a20  ng summarizing. 
-000117c0: 2020 2074 6865 204d 6f64 756c 6520 696e     the Module in
-000117d0: 2061 2074 6162 6c65 2e20 6074 6162 756c   a table. `tabul
-000117e0: 6174 6560 2075 7365 7320 606a 6178 2e65  ate` uses `jax.e
-000117f0: 7661 6c5f 7368 6170 6560 2074 6f20 7275  val_shape` to ru
-00011800: 6e20 7468 6520 666f 7277 6172 640a 2020  n the forward.  
-00011810: 2020 636f 6d70 7574 6174 696f 6e20 7769    computation wi
-00011820: 7468 6f75 7420 636f 6e73 756d 696e 6720  thout consuming 
-00011830: 616e 7920 464c 4f50 7320 6f72 2061 6c6c  any FLOPs or all
-00011840: 6f63 6174 696e 6720 6d65 6d6f 7279 2e0a  ocating memory..
-00011850: 0a20 2020 2041 6464 6974 696f 6e61 6c20  .    Additional 
-00011860: 6172 6775 6d65 6e74 7320 6361 6e20 6265  arguments can be
-00011870: 2070 6173 7365 6420 696e 746f 2074 6865   passed into the
-00011880: 2060 636f 6e73 6f6c 655f 6b77 6172 6773   `console_kwargs
-00011890: 6020 6172 6775 6d65 6e74 2c20 666f 7220  ` argument, for 
-000118a0: 6578 616d 706c 652c 0a20 2020 2060 7b27  example,.    `{'
-000118b0: 7769 6474 6827 3a20 3132 307d 602e 2046  width': 120}`. F
-000118c0: 6f72 2061 2066 756c 6c20 6c69 7374 206f  or a full list o
-000118d0: 6620 6063 6f6e 736f 6c65 5f6b 7761 7267  f `console_kwarg
-000118e0: 7360 2061 7267 756d 656e 7473 2c20 7365  s` arguments, se
-000118f0: 653a 0a20 2020 2068 7474 7073 3a2f 2f72  e:.    https://r
-00011900: 6963 682e 7265 6164 7468 6564 6f63 732e  ich.readthedocs.
-00011910: 696f 2f65 6e2f 7374 6162 6c65 2f72 6566  io/en/stable/ref
-00011920: 6572 656e 6365 2f63 6f6e 736f 6c65 2e68  erence/console.h
-00011930: 746d 6c23 7269 6368 2e63 6f6e 736f 6c65  tml#rich.console
-00011940: 2e43 6f6e 736f 6c65 0a0a 2020 2020 4578  .Console..    Ex
-00011950: 616d 706c 653a 3a0a 0a20 2020 2020 2069  ample::..      i
-00011960: 6d70 6f72 7420 6a61 780a 2020 2020 2020  mport jax.      
-00011970: 696d 706f 7274 206a 6178 2e6e 756d 7079  import jax.numpy
-00011980: 2061 7320 6a6e 700a 2020 2020 2020 696d   as jnp.      im
-00011990: 706f 7274 2066 6c61 782e 6c69 6e65 6e20  port flax.linen 
-000119a0: 6173 206e 6e0a 0a20 2020 2020 2063 6c61  as nn..      cla
-000119b0: 7373 2046 6f6f 286e 6e2e 4d6f 6475 6c65  ss Foo(nn.Module
-000119c0: 293a 0a20 2020 2020 2020 2020 2040 6e6e  ):.          @nn
-000119d0: 2e63 6f6d 7061 6374 0a20 2020 2020 2020  .compact.       
-000119e0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-000119f0: 7365 6c66 2c20 7829 3a0a 2020 2020 2020  self, x):.      
-00011a00: 2020 2020 2020 2020 6820 3d20 6e6e 2e44          h = nn.D
-00011a10: 656e 7365 2834 2928 7829 0a20 2020 2020  ense(4)(x).     
-00011a20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011a30: 6e6e 2e44 656e 7365 2832 2928 6829 0a0a  nn.Dense(2)(h)..
-00011a40: 2020 2020 2020 7820 3d20 6a6e 702e 6f6e        x = jnp.on
-00011a50: 6573 2828 3136 2c20 3929 290a 0a20 2020  es((16, 9))..   
-00011a60: 2020 2070 7269 6e74 2846 6f6f 2829 2e74     print(Foo().t
-00011a70: 6162 756c 6174 6528 6a61 782e 7261 6e64  abulate(jax.rand
-00011a80: 6f6d 2e50 524e 474b 6579 2830 292c 2078  om.PRNGKey(0), x
-00011a90: 2929 0a0a 0a20 2020 2054 6869 7320 6769  ))...    This gi
-00011aa0: 7665 7320 7468 6520 666f 6c6c 6f77 696e  ves the followin
-00011ab0: 6720 6f75 7470 7574 3a3a 0a0a 2020 2020  g output::..    
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ae0: 2020 466f 6f20 5375 6d6d 6172 790a 2020    Foo Summary.  
-00011af0: 2020 2020 e294 8fe2 9481 e294 81e2 9481      ............
-00011b00: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00011b10: 9481 e294 b3e2 9481 e294 81e2 9481 e294  ................
-00011b20: 81e2 9481 e294 81e2 9481 e294 81e2 94b3  ................
-00011b30: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00011b40: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00011b50: 81e2 9481 e294 81e2 9481 e294 81e2 94b3  ................
-00011b60: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00011b70: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00011b80: 81e2 9481 e294 81e2 9481 e294 81e2 94b3  ................
-00011b90: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00011ba0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00011bb0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00011bc0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00011bd0: 9481 e294 930a 2020 2020 2020 e294 8320  ......      ... 
-00011be0: 7061 7468 2020 2020 e294 8320 6d6f 6475  path    ... modu
-00011bf0: 6c65 20e2 9483 2069 6e70 7574 7320 2020  le ... inputs   
-00011c00: 2020 2020 20e2 9483 206f 7574 7075 7473       ... outputs
-00011c10: 2020 2020 2020 20e2 9483 2070 6172 616d         ... param
-00011c20: 7320 2020 2020 2020 2020 2020 2020 2020  s               
-00011c30: e294 830a 2020 2020 2020 e294 a1e2 9481  ....      ......
-00011c40: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00011c50: 9481 e294 81e2 9481 e295 87e2 9481 e294  ................
-00011c60: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00011c70: e294 81e2 9587 e294 81e2 9481 e294 81e2  ................
-00011c80: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00011c90: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00011ca0: e294 81e2 9587 e294 81e2 9481 e294 81e2  ................
-00011cb0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00011cc0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00011cd0: e294 81e2 9587 e294 81e2 9481 e294 81e2  ................
-00011ce0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00011cf0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00011d00: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00011d10: 9481 e294 81e2 9481 e294 a90a 2020 2020  ............    
-00011d20: 2020 e294 8220 2020 2020 2020 2020 e294    ...         ..
-00011d30: 8220 466f 6f20 2020 20e2 9482 2066 6c6f  . Foo    ... flo
-00011d40: 6174 3332 5b31 362c 395d 20e2 9482 2066  at32[16,9] ... f
-00011d50: 6c6f 6174 3332 5b31 362c 325d 20e2 9482  loat32[16,2] ...
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 2020 2020 e294 820a 2020 2020 2020        ....      
-00011d80: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
-00011d90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00011da0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00011db0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00011dc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00011dd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00011de0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00011df0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00011e00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00011e10: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00011e20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00011e30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00011e40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00011e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00011e60: a40a 2020 2020 2020 e294 8220 4465 6e73  ..      ... Dens
-00011e70: 655f 3020 e294 8220 4465 6e73 6520 20e2  e_0 ... Dense  .
-00011e80: 9482 2066 6c6f 6174 3332 5b31 362c 395d  .. float32[16,9]
-00011e90: 20e2 9482 2066 6c6f 6174 3332 5b31 362c   ... float32[16,
-00011ea0: 345d 20e2 9482 2062 6961 733a 2066 6c6f  4] ... bias: flo
-00011eb0: 6174 3332 5b34 5d20 2020 2020 e294 820a  at32[4]     ....
-00011ec0: 2020 2020 2020 e294 8220 2020 2020 2020        ...       
-00011ed0: 2020 e294 8220 2020 2020 2020 20e2 9482    ...        ...
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00011ef0: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00011f00: 20e2 9482 206b 6572 6e65 6c3a 2066 6c6f   ... kernel: flo
-00011f10: 6174 3332 5b39 2c34 5d20 e294 820a 2020  at32[9,4] ....  
-00011f20: 2020 2020 e294 8220 2020 2020 2020 2020      ...         
-00011f30: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
-00011f40: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00011f50: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00011f60: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00011f70: 2020 2020 2020 2020 e294 820a 2020 2020          ....    
-00011f80: 2020 e294 8220 2020 2020 2020 2020 e294    ...         ..
-00011f90: 8220 2020 2020 2020 20e2 9482 2020 2020  .        ...    
-00011fa0: 2020 2020 2020 2020 2020 20e2 9482 2020             ...  
-00011fb0: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00011fc0: 2034 3020 2831 3630 2042 2920 2020 2020   40 (160 B)     
-00011fd0: 2020 2020 2020 e294 820a 2020 2020 2020        ....      
-00011fe0: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
-00011ff0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012000: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012010: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00012020: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00004ff0: 2320 5468 6520 4d6f 6475 6c65 4261 7365  # The ModuleBase
+00005000: 2063 6c61 7373 2069 7320 6372 6561 7465   class is create
+00005010: 6420 6f6e 6c79 2074 6f20 6d61 6b65 2073  d only to make s
+00005020: 7461 7469 6320 616e 616c 797a 6572 7320  tatic analyzers 
+00005030: 6861 7070 790a 2320 6d61 696e 6c79 2070  happy.# mainly p
+00005040: 7974 7970 6520 616e 6420 7079 7269 6768  ytype and pyrigh
+00005050: 742e 2053 6f6d 6520 6e6f 7465 733a 0a23  t. Some notes:.#
+00005060: 202a 2070 7972 6967 6874 2028 636f 7272   * pyright (corr
+00005070: 6563 746c 7929 2063 6f6d 706c 6169 6e73  ectly) complains
+00005080: 2074 6861 7420 4d6f 6475 6c65 2069 7473   that Module its
+00005090: 656c 6620 6973 206e 6f74 2061 2064 6174  elf is not a dat
+000050a0: 6163 6c61 7373 2c20 6576 656e 0a23 2020  aclass, even.#  
+000050b0: 2074 686f 7567 6820 616c 6c20 6974 7320   though all its 
+000050c0: 7375 6263 6c61 7373 6573 2061 6e64 2069  subclasses and i
+000050d0: 6e74 616e 6365 7320 4152 4520 6461 7461  ntances ARE data
+000050e0: 636c 6173 7365 732e 2042 6563 6175 7365  classes. Because
+000050f0: 2074 6865 7265 2069 7320 6e6f 0a23 2020   there is no.#  
+00005100: 2077 6179 2074 6f20 616e 6e6f 7461 7465   way to annotate
+00005110: 2074 6869 7320 696e 2061 2077 6179 2074   this in a way t
+00005120: 6861 7420 7079 7269 6768 7420 756e 6465  hat pyright unde
+00005130: 7273 7461 6e64 732c 2077 6520 6372 6561  rstands, we crea
+00005140: 7465 2061 0a23 2020 204d 6f64 756c 6542  te a.#   ModuleB
+00005150: 6173 6520 636c 6173 7320 6465 636f 7261  ase class decora
+00005160: 7465 6420 7769 7468 2060 6461 7461 636c  ted with `datacl
+00005170: 6173 735f 7472 616e 7366 6f72 6d60 2073  ass_transform` s
+00005180: 7563 6820 7468 6174 2070 7972 6967 6874  uch that pyright
+00005190: 0a23 2020 2074 6869 6e6b 7320 4d6f 6475  .#   thinks Modu
+000051a0: 6c65 2069 7320 6120 6461 7461 636c 6173  le is a dataclas
+000051b0: 7320 2869 6e20 7265 616c 6974 7920 6f6e  s (in reality on
+000051c0: 6c79 2073 7562 636c 6173 7365 7320 6172  ly subclasses ar
+000051d0: 6520 696e 7374 616e 7469 6174 6564 0a23  e instantiated.#
+000051e0: 2020 2073 6f20 7468 6973 2069 7320 6669     so this is fi
+000051f0: 6e65 292e 0a23 202a 2054 6865 2060 5f5f  ne)..# * The `__
+00005200: 6461 7461 636c 6173 735f 6669 656c 6473  dataclass_fields
+00005210: 5f5f 6020 6174 7472 6962 7574 6520 6973  __` attribute is
+00005220: 206e 6565 6465 6420 6265 6361 7573 6520   needed because 
+00005230: 7079 7479 7065 2073 6565 6d73 2074 6f0a  pytype seems to.
+00005240: 2320 2020 6e6f 7420 756e 6465 7273 7461  #   not understa
+00005250: 6e64 2074 6865 2060 6461 7461 636c 6173  nd the `dataclas
+00005260: 735f 7472 616e 7366 6f72 6d60 2064 6563  s_transform` dec
+00005270: 6f72 6174 6f72 2c20 7468 6572 6566 6f72  orator, therefor
+00005280: 6520 7765 206e 6565 640a 2320 2020 746f  e we need.#   to
+00005290: 2061 6464 2074 6865 2061 7474 7269 6275   add the attribu
+000052a0: 7465 206d 616e 7561 6c6c 792e 0a23 202a  te manually..# *
+000052b0: 204f 7468 6572 2061 7474 7269 6275 7465   Other attribute
+000052c0: 7320 6172 6520 616e 6e6f 7461 7465 6420  s are annotated 
+000052d0: 666f 7220 636f 6d70 6c65 7465 6e65 7373  for completeness
+000052e0: 2e20 4265 6361 7573 6520 7765 2061 7265  . Because we are
+000052f0: 2075 7369 6e67 0a23 2020 2074 6865 2060   using.#   the `
+00005300: 6966 2074 7970 696e 672e 5459 5045 5f43  if typing.TYPE_C
+00005310: 4845 434b 494e 4760 2070 6174 7465 726e  HECKING` pattern
+00005320: 2c20 7468 6573 6520 616e 6e6f 7461 7469  , these annotati
+00005330: 6f6e 7320 6172 6520 6e6f 7420 7072 6573  ons are not pres
+00005340: 656e 740a 2320 2020 6174 2072 756e 7469  ent.#   at runti
+00005350: 6d65 2073 6f20 7468 6579 2064 6f6e 2774  me so they don't
+00005360: 2061 6666 6563 7420 7468 6520 6461 7461   affect the data
+00005370: 636c 6173 7320 6265 6861 7669 6f72 2e0a  class behavior..
+00005380: 4064 6174 6163 6c61 7373 5f74 7261 6e73  @dataclass_trans
+00005390: 666f 726d 2829 0a63 6c61 7373 204d 6f64  form().class Mod
+000053a0: 756c 6542 6173 653a 0a20 2069 6620 7479  uleBase:.  if ty
+000053b0: 7069 6e67 2e54 5950 455f 4348 4543 4b49  ping.TYPE_CHECKI
+000053c0: 4e47 3a0a 2020 2020 7363 6f70 653a 204f  NG:.    scope: O
+000053d0: 7074 696f 6e61 6c5b 5363 6f70 655d 0a20  ptional[Scope]. 
+000053e0: 2020 205f 7374 6174 653a 205f 4d6f 6475     _state: _Modu
+000053f0: 6c65 496e 7465 726e 616c 5374 6174 650a  leInternalState.
+00005400: 2020 2020 5f70 6172 656e 745f 7265 663a      _parent_ref:
+00005410: 2055 6e69 6f6e 5b27 4d6f 6475 6c65 272c   Union['Module',
+00005420: 2077 6561 6b72 6566 2e52 6566 6572 656e   weakref.Referen
+00005430: 6365 5479 7065 5b27 4d6f 6475 6c65 275d  ceType['Module']
+00005440: 2c20 4e6f 6e65 5d0a 2020 2020 7061 7265  , None].    pare
+00005450: 6e74 3a20 556e 696f 6e5b 274d 6f64 756c  nt: Union['Modul
+00005460: 6527 2c20 5f53 656e 7469 6e65 6c2c 204e  e', _Sentinel, N
+00005470: 6f6e 655d 0a20 2020 205f 5f64 6174 6163  one].    __datac
+00005480: 6c61 7373 5f66 6965 6c64 735f 5f3a 2044  lass_fields__: D
+00005490: 6963 745b 7374 722c 2064 6174 6163 6c61  ict[str, datacla
+000054a0: 7373 6573 2e46 6965 6c64 5d0a 0a63 6c61  sses.Field]..cla
+000054b0: 7373 204d 6f64 756c 6528 4d6f 6475 6c65  ss Module(Module
+000054c0: 4261 7365 293a 0a20 2022 2222 4261 7365  Base):.  """Base
+000054d0: 2063 6c61 7373 2066 6f72 2061 6c6c 206e   class for all n
+000054e0: 6575 7261 6c20 6e65 7477 6f72 6b20 6d6f  eural network mo
+000054f0: 6475 6c65 732e 204c 6179 6572 7320 616e  dules. Layers an
+00005500: 6420 6d6f 6465 6c73 2073 686f 756c 6420  d models should 
+00005510: 7375 6263 6c61 7373 2074 6869 7320 636c  subclass this cl
+00005520: 6173 732e 0a0a 2020 416c 6c20 466c 6178  ass...  All Flax
+00005530: 204d 6f64 756c 6573 2061 7265 2050 7974   Modules are Pyt
+00005540: 686f 6e20 332e 370a 2020 6064 6174 6163  hon 3.7.  `datac
+00005550: 6c61 7373 6573 203c 6874 7470 733a 2f2f  lasses <https://
+00005560: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00005570: 332f 6c69 6272 6172 792f 6461 7461 636c  3/library/datacl
+00005580: 6173 7365 732e 6874 6d6c 3e60 5f2e 2053  asses.html>`_. S
+00005590: 696e 6365 0a20 2064 6174 6163 6c61 7373  ince.  dataclass
+000055a0: 6573 2074 616b 6520 6f76 6572 2060 605f  es take over ``_
+000055b0: 5f69 6e69 745f 5f60 602c 2079 6f75 2073  _init__``, you s
+000055c0: 686f 756c 6420 696e 7374 6561 6420 6f76  hould instead ov
+000055d0: 6572 7269 6465 203a 6d65 7468 3a60 7365  erride :meth:`se
+000055e0: 7475 7060 2c0a 2020 7768 6963 6820 6973  tup`,.  which is
+000055f0: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
+00005600: 616c 6c65 6420 746f 2069 6e69 7469 616c  alled to initial
+00005610: 697a 6520 7468 6520 6d6f 6475 6c65 2e0a  ize the module..
+00005620: 0a20 204d 6f64 756c 6573 2063 616e 2063  .  Modules can c
+00005630: 6f6e 7461 696e 2073 7562 6d6f 6475 6c65  ontain submodule
+00005640: 732c 2061 6e64 2069 6e20 7468 6973 2077  s, and in this w
+00005650: 6179 2063 616e 2062 6520 6e65 7374 6564  ay can be nested
+00005660: 2069 6e20 6120 7472 6565 0a20 2073 7472   in a tree.  str
+00005670: 7563 7475 7265 2e20 5375 626d 6f64 656c  ucture. Submodel
+00005680: 7320 6361 6e20 6265 2061 7373 6967 6e65  s can be assigne
+00005690: 6420 6173 2072 6567 756c 6172 2061 7474  d as regular att
+000056a0: 7269 6275 7465 7320 696e 7369 6465 2074  ributes inside t
+000056b0: 6865 0a20 203a 6d65 7468 3a60 7365 7475  he.  :meth:`setu
+000056c0: 7060 206d 6574 686f 642e 0a0a 2020 596f  p` method...  Yo
+000056d0: 7520 6361 6e20 6465 6669 6e65 2061 7262  u can define arb
+000056e0: 6974 7261 7279 2022 666f 7277 6172 6420  itrary "forward 
+000056f0: 7061 7373 2220 6d65 7468 6f64 7320 6f6e  pass" methods on
+00005700: 2079 6f75 7220 4d6f 6475 6c65 2073 7562   your Module sub
+00005710: 636c 6173 732e 0a20 2057 6869 6c65 206e  class..  While n
+00005720: 6f20 6d65 7468 6f64 7320 6172 6520 7370  o methods are sp
+00005730: 6563 6961 6c2d 6361 7365 642c 2060 605f  ecial-cased, ``_
+00005740: 5f63 616c 6c5f 5f60 6020 6973 2061 2070  _call__`` is a p
+00005750: 6f70 756c 6172 2063 686f 6963 6520 6265  opular choice be
+00005760: 6361 7573 650a 2020 6974 2061 6c6c 6f77  cause.  it allow
+00005770: 7320 796f 7520 746f 2075 7365 206d 6f64  s you to use mod
+00005780: 756c 6520 696e 7374 616e 6365 7320 6173  ule instances as
+00005790: 2069 6620 7468 6579 2061 7265 2066 756e   if they are fun
+000057a0: 6374 696f 6e73 3a3a 0a0a 2020 2020 6672  ctions::..    fr
+000057b0: 6f6d 2066 6c61 7820 696d 706f 7274 206c  om flax import l
+000057c0: 696e 656e 2061 7320 6e6e 0a0a 2020 2020  inen as nn..    
+000057d0: 636c 6173 7320 4d6f 6475 6c65 286e 6e2e  class Module(nn.
+000057e0: 4d6f 6475 6c65 293a 0a20 2020 2020 2066  Module):.      f
+000057f0: 6561 7475 7265 733a 2054 7570 6c65 5b69  eatures: Tuple[i
+00005800: 6e74 2c20 2e2e 2e5d 203d 2028 3136 2c20  nt, ...] = (16, 
+00005810: 3429 0a0a 2020 2020 2020 6465 6620 7365  4)..      def se
+00005820: 7475 7028 7365 6c66 293a 0a20 2020 2020  tup(self):.     
+00005830: 2020 2073 656c 662e 6465 6e73 6531 203d     self.dense1 =
+00005840: 2044 656e 7365 2873 656c 662e 6665 6174   Dense(self.feat
+00005850: 7572 6573 5b30 5d29 0a20 2020 2020 2020  ures[0]).       
+00005860: 2073 656c 662e 6465 6e73 6532 203d 2044   self.dense2 = D
+00005870: 656e 7365 2873 656c 662e 6665 6174 7572  ense(self.featur
+00005880: 6573 5b31 5d29 0a0a 2020 2020 2020 6465  es[1])..      de
+00005890: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
+000058a0: 2078 293a 0a20 2020 2020 2020 2072 6574   x):.        ret
+000058b0: 7572 6e20 7365 6c66 2e64 656e 7365 3228  urn self.dense2(
+000058c0: 6e6e 2e72 656c 7528 7365 6c66 2e64 656e  nn.relu(self.den
+000058d0: 7365 3128 7829 2929 0a0a 2020 4f70 7469  se1(x)))..  Opti
+000058e0: 6f6e 616c 6c79 2c20 666f 7220 6d6f 7265  onally, for more
+000058f0: 2063 6f6e 6369 7365 206d 6f64 756c 6520   concise module 
+00005900: 696d 706c 656d 656e 7461 7469 6f6e 7320  implementations 
+00005910: 7768 6572 6520 7375 626d 6f64 756c 6573  where submodules
+00005920: 0a20 2064 6566 696e 6974 696f 6e73 2061  .  definitions a
+00005930: 7265 2063 6f2d 6c6f 6361 7465 6420 7769  re co-located wi
+00005940: 7468 2074 6865 6972 2075 7361 6765 2c20  th their usage, 
+00005950: 796f 7520 6361 6e20 7573 6520 7468 650a  you can use the.
+00005960: 2020 3a6d 6574 683a 6063 6f6d 7061 6374    :meth:`compact
+00005970: 6020 7772 6170 7065 722e 0a20 2022 2222  ` wrapper..  """
+00005980: 0a0a 2020 6966 2074 7970 696e 672e 5459  ..  if typing.TY
+00005990: 5045 5f43 4845 434b 494e 473a 0a20 2020  PE_CHECKING:.   
+000059a0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000059b0: 6c66 2c20 2a61 7267 732c 202a 2a6b 7761  lf, *args, **kwa
+000059c0: 7267 7329 3a0a 2020 2020 2020 2320 7468  rgs):.      # th
+000059d0: 6973 2073 7475 6220 6d61 6b65 7320 7375  is stub makes su
+000059e0: 7265 2070 7974 7970 6520 6163 6365 7074  re pytype accept
+000059f0: 7320 636f 6e73 7472 7563 746f 7220 6172  s constructor ar
+00005a00: 6775 6d65 6e74 732e 0a20 2020 2020 2070  guments..      p
+00005a10: 6173 730a 0a20 2020 2064 6566 205f 5f63  ass..    def __c
+00005a20: 616c 6c5f 5f28 7365 6c66 2c20 2a61 7267  all__(self, *arg
+00005a30: 732c 202a 2a6b 7761 7267 7329 202d 3e20  s, **kwargs) -> 
+00005a40: 416e 793a 0a20 2020 2020 2023 2074 6869  Any:.      # thi
+00005a50: 7320 7374 7562 2061 6c6c 6f77 7320 7079  s stub allows py
+00005a60: 7479 7065 2074 6f20 6163 6365 7074 204d  type to accept M
+00005a70: 6f64 756c 6573 2061 7320 4361 6c6c 6162  odules as Callab
+00005a80: 6c65 732e 0a20 2020 2020 2070 6173 730a  les..      pass.
+00005a90: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
+00005aa0: 2020 6465 6620 5f5f 696e 6974 5f73 7562    def __init_sub
+00005ab0: 636c 6173 735f 5f28 636c 732c 206b 775f  class__(cls, kw_
+00005ac0: 6f6e 6c79 3a20 626f 6f6c 203d 2046 616c  only: bool = Fal
+00005ad0: 7365 2c20 2a2a 6b77 6172 6773 3a20 416e  se, **kwargs: An
+00005ae0: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
+00005af0: 2222 2241 7574 6f6d 6174 6963 616c 6c79  """Automatically
+00005b00: 2069 6e69 7469 616c 697a 6573 2061 6c6c   initializes all
+00005b10: 2073 7562 636c 6173 7365 7320 6173 2063   subclasses as c
+00005b20: 7573 746f 6d20 6461 7461 636c 6173 7365  ustom dataclasse
+00005b30: 732e 2222 220a 2020 2020 7375 7065 7228  s.""".    super(
+00005b40: 292e 5f5f 696e 6974 5f73 7562 636c 6173  ).__init_subclas
+00005b50: 735f 5f28 2a2a 6b77 6172 6773 290a 2020  s__(**kwargs).  
+00005b60: 2020 2320 416c 6c20 466c 6178 204d 6f64    # All Flax Mod
+00005b70: 756c 6573 2061 7265 2064 6174 6163 6c61  ules are datacla
+00005b80: 7373 6573 2e20 2057 6520 666f 7263 6520  sses.  We force 
+00005b90: 7468 6973 2063 6f6e 7665 6e74 696f 6e20  this convention 
+00005ba0: 7369 6e63 650a 2020 2020 2320 6974 2065  since.    # it e
+00005bb0: 6e63 6f75 7261 6765 7320 7468 6520 7374  ncourages the st
+00005bc0: 6174 656c 6573 7320 6265 6861 7669 6f72  ateless behavior
+00005bd0: 206e 6565 6465 6420 746f 2063 6c6f 6e65   needed to clone
+00005be0: 206d 6f64 756c 6520 696e 7374 616e 6365   module instance
+00005bf0: 7320 666f 720a 2020 2020 2320 6675 6e63  s for.    # func
+00005c00: 7469 6f6e 616c 2074 7261 6e73 666f 726d  tional transform
+00005c10: 6174 696f 6e2e 2020 496e 7374 6561 6420  ation.  Instead 
+00005c20: 6f66 2075 7369 6e67 2061 2070 7974 686f  of using a pytho
+00005c30: 6e20 6d65 7461 636c 6173 732c 2077 650a  n metaclass, we.
+00005c40: 2020 2020 2320 6175 746f 6d61 7469 6361      # automatica
+00005c50: 6c6c 7920 7472 616e 7366 6f72 6d20 4d6f  lly transform Mo
+00005c60: 6475 6c65 7320 696e 746f 2064 6174 6163  dules into datac
+00005c70: 6c61 7373 6573 2061 7420 7375 6263 6c61  lasses at subcla
+00005c80: 7373 2063 7265 6174 696f 6e0a 2020 2020  ss creation.    
+00005c90: 2320 7469 6d65 2c20 616e 6420 7765 2073  # time, and we s
+00005ca0: 6574 2074 6865 206c 6173 7420 6461 7461  et the last data
+00005cb0: 636c 6173 7320 6172 6775 6d65 6e74 7320  class arguments 
+00005cc0: 746f 2060 7061 7265 6e74 6020 616e 6420  to `parent` and 
+00005cd0: 606e 616d 6560 2e0a 2020 2020 636c 732e  `name`..    cls.
+00005ce0: 5f63 7573 746f 6d69 7a65 645f 6461 7461  _customized_data
+00005cf0: 636c 6173 735f 7472 616e 7366 6f72 6d28  class_transform(
+00005d00: 6b77 5f6f 6e6c 7929 0a20 2020 2023 2057  kw_only).    # W
+00005d10: 6520 7772 6170 2075 7365 722d 6465 6669  e wrap user-defi
+00005d20: 6e65 6420 6d65 7468 6f64 7320 696e 636c  ned methods incl
+00005d30: 7564 696e 6720 7365 7475 7020 616e 6420  uding setup and 
+00005d40: 5f5f 6361 6c6c 5f5f 2074 6f20 656e 666f  __call__ to enfo
+00005d50: 7263 650a 2020 2020 2320 6120 6e75 6d62  rce.    # a numb
+00005d60: 6572 206f 6620 6469 6666 6572 656e 7420  er of different 
+00005d70: 6368 6563 6b73 2061 6e64 2074 6f20 7072  checks and to pr
+00005d80: 6f76 6964 6520 636c 6561 7220 6572 726f  ovide clear erro
+00005d90: 7220 6d65 7373 6167 6573 2e0a 2020 2020  r messages..    
+00005da0: 636c 732e 5f76 6572 6966 795f 7369 6e67  cls._verify_sing
+00005db0: 6c65 5f6f 725f 6e6f 5f63 6f6d 7061 6374  le_or_no_compact
+00005dc0: 2829 0a20 2020 2063 6c73 2e5f 7772 6170  ().    cls._wrap
+00005dd0: 5f6d 6f64 756c 655f 6174 7472 6962 7574  _module_attribut
+00005de0: 6573 2829 0a20 2020 2023 2053 6574 2065  es().    # Set e
+00005df0: 6d70 7479 2063 6c61 7373 2064 6566 6175  mpty class defau
+00005e00: 6c74 732e 0a20 2020 2063 6c73 2e5f 7374  lts..    cls._st
+00005e10: 6174 6520 3d20 5f75 6e69 6e69 7469 616c  ate = _uninitial
+00005e20: 697a 6564 5f6d 6f64 756c 655f 696e 7465  ized_module_inte
+00005e30: 726e 616c 5f73 7461 7465 2023 2074 7970  rnal_state # typ
+00005e40: 653a 2069 676e 6f72 655b 6174 7472 2d64  e: ignore[attr-d
+00005e50: 6566 696e 6564 5d0a 2020 2020 636c 732e  efined].    cls.
+00005e60: 7363 6f70 653a 204f 7074 696f 6e61 6c5b  scope: Optional[
+00005e70: 5363 6f70 655d 203d 204e 6f6e 6520 2320  Scope] = None # 
+00005e80: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00005e90: 2023 2048 616e 646c 6573 2077 6561 6b20   # Handles weak 
+00005ea0: 7265 6665 7265 6e63 696e 6720 6f66 2070  referencing of p
+00005eb0: 6172 656e 7420 4d6f 6475 6c65 7320 746f  arent Modules to
+00005ec0: 2070 7265 7665 6e74 2072 6566 6572 656e   prevent referen
+00005ed0: 6365 2063 7963 6c65 732e 0a20 2020 2063  ce cycles..    c
+00005ee0: 6c73 2e5f 7061 7265 6e74 5f72 6566 203d  ls._parent_ref =
+00005ef0: 204e 6f6e 6520 2320 7479 7065 3a20 6967   None # type: ig
+00005f00: 6e6f 7265 5b61 7474 722d 6465 6669 6e65  nore[attr-define
+00005f10: 645d 0a20 2020 2063 6c73 2e70 6172 656e  d].    cls.paren
+00005f20: 7420 3d20 5061 7265 6e74 4465 7363 7269  t = ParentDescri
+00005f30: 7074 6f72 2829 2023 2074 7970 653a 2069  ptor() # type: i
+00005f40: 676e 6f72 655b 6173 7369 676e 6d65 6e74  gnore[assignment
+00005f50: 5d0a 0a20 2040 636c 6173 736d 6574 686f  ]..  @classmetho
+00005f60: 640a 2020 6465 6620 5f63 7573 746f 6d69  d.  def _customi
+00005f70: 7a65 645f 6461 7461 636c 6173 735f 7472  zed_dataclass_tr
+00005f80: 616e 7366 6f72 6d28 636c 732c 206b 775f  ansform(cls, kw_
+00005f90: 6f6e 6c79 3a20 626f 6f6c 293a 0a20 2020  only: bool):.   
+00005fa0: 2022 2222 5472 616e 7366 6f72 6d73 2060   """Transforms `
+00005fb0: 636c 7360 2069 6e74 6f20 6120 6461 7461  cls` into a data
+00005fc0: 636c 6173 732c 2077 6974 6820 6375 7374  class, with cust
+00005fd0: 6f6d 2061 6464 6974 696f 6e61 6c20 6265  om additional be
+00005fe0: 6861 7669 6f72 2e0a 0a20 2020 2031 2e20  havior...    1. 
+00005ff0: 496e 6a65 6374 2060 7061 7265 6e74 6020  Inject `parent` 
+00006000: 616e 6420 606e 616d 6560 2066 6965 6c64  and `name` field
+00006010: 732e 2020 2849 6620 7468 6579 2061 7265  s.  (If they are
+00006020: 2061 6c72 6561 6479 2070 7265 7365 6e74   already present
+00006030: 2c0a 2020 2020 2020 2074 6865 6e20 6368  ,.       then ch
+00006040: 6563 6b20 7468 6174 2074 6865 7920 6861  eck that they ha
+00006050: 7665 2074 6865 2065 7870 6563 7465 6420  ve the expected 
+00006060: 7479 7065 732e 290a 2020 2020 322e 2053  types.).    2. S
+00006070: 6574 2063 6f6d 7061 7265 2c20 6861 7368  et compare, hash
+00006080: 2c20 616e 6420 7265 7072 2074 6f20 4661  , and repr to Fa
+00006090: 6c73 6520 666f 7220 6e6f 6e2d 696e 6974  lse for non-init
+000060a0: 2066 6965 6c64 732e 0a20 2020 2033 2e20   fields..    3. 
+000060b0: 4765 6e65 7261 7465 2061 2068 6173 6820  Generate a hash 
+000060c0: 6675 6e63 7469 6f6e 2028 6966 206e 6f74  function (if not
+000060d0: 2070 726f 7669 6465 6420 6279 2063 6c73   provided by cls
+000060e0: 292e 0a20 2020 2022 2222 0a20 2020 2023  )..    """.    #
+000060f0: 2043 6865 636b 2072 6573 6572 7665 6420   Check reserved 
+00006100: 6174 7472 6962 7574 6573 2068 6176 6520  attributes have 
+00006110: 6578 7065 6374 6564 2074 7970 6520 616e  expected type an
+00006120: 6e6f 7461 7469 6f6e 732e 0a20 2020 2061  notations..    a
+00006130: 6e6e 6f74 6174 696f 6e73 203d 2064 6963  nnotations = dic
+00006140: 7428 636c 732e 5f5f 6469 6374 5f5f 2e67  t(cls.__dict__.g
+00006150: 6574 2827 5f5f 616e 6e6f 7461 7469 6f6e  et('__annotation
+00006160: 735f 5f27 2c20 7b7d 2929 0a20 2020 2069  s__', {})).    i
+00006170: 6620 616e 6e6f 7461 7469 6f6e 732e 6765  f annotations.ge
+00006180: 7428 2770 6172 656e 7427 2c20 5f50 6172  t('parent', _Par
+00006190: 656e 7454 7970 6529 2021 3d20 5f50 6172  entType) != _Par
+000061a0: 656e 7454 7970 653a 0a20 2020 2020 2072  entType:.      r
+000061b0: 6169 7365 2065 7272 6f72 732e 5265 7365  aise errors.Rese
+000061c0: 7276 6564 4d6f 6475 6c65 4174 7472 6962  rvedModuleAttrib
+000061d0: 7574 6545 7272 6f72 2861 6e6e 6f74 6174  uteError(annotat
+000061e0: 696f 6e73 290a 2020 2020 6966 2061 6e6e  ions).    if ann
+000061f0: 6f74 6174 696f 6e73 2e67 6574 2827 6e61  otations.get('na
+00006200: 6d65 272c 2073 7472 2920 6e6f 7420 696e  me', str) not in
+00006210: 2028 2773 7472 272c 2073 7472 2c20 4f70   ('str', str, Op
+00006220: 7469 6f6e 616c 5b73 7472 5d29 3a0a 2020  tional[str]):.  
+00006230: 2020 2020 7261 6973 6520 6572 726f 7273      raise errors
+00006240: 2e52 6573 6572 7665 644d 6f64 756c 6541  .ReservedModuleA
+00006250: 7474 7269 6275 7465 4572 726f 7228 616e  ttributeError(an
+00006260: 6e6f 7461 7469 6f6e 7329 0a0a 2020 2020  notations)..    
+00006270: 2320 616e 7920 6e6f 6e2d 696e 6974 2066  # any non-init f
+00006280: 6965 6c64 2077 696c 6c20 6f6e 6c79 2062  ield will only b
+00006290: 6520 7365 7420 696e 2073 6574 7570 0a20  e set in setup. 
+000062a0: 2020 2023 2044 7572 696e 6720 5f5f 6861     # During __ha
+000062b0: 7368 5f5f 2061 6e64 205f 5f65 715f 5f20  sh__ and __eq__ 
+000062c0: 7468 6520 6669 656c 6420 6973 206e 6f74  the field is not
+000062d0: 2073 6574 2079 6574 0a20 2020 2023 2073   set yet.    # s
+000062e0: 6f20 6974 2073 686f 756c 6420 6e6f 7420  o it should not 
+000062f0: 6265 2075 7365 6420 696e 2063 6f6d 7061  be used in compa
+00006300: 7265 2c20 6861 7368 206f 7220 7265 7072  re, hash or repr
+00006310: 2e0a 2020 2020 666f 7220 6669 656c 6420  ..    for field 
+00006320: 696e 2061 6e6e 6f74 6174 696f 6e73 3a0a  in annotations:.
+00006330: 2020 2020 2020 6669 656c 645f 6d65 7461        field_meta
+00006340: 203d 2067 6574 6174 7472 2863 6c73 2c20   = getattr(cls, 
+00006350: 6669 656c 642c 204e 6f6e 6529 0a20 2020  field, None).   
+00006360: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00006370: 2866 6965 6c64 5f6d 6574 612c 2064 6174  (field_meta, dat
+00006380: 6163 6c61 7373 6573 2e46 6965 6c64 2920  aclasses.Field) 
+00006390: 616e 6420 6e6f 7420 6669 656c 645f 6d65  and not field_me
+000063a0: 7461 2e69 6e69 743a 0a20 2020 2020 2020  ta.init:.       
+000063b0: 2066 6965 6c64 5f6d 6574 612e 636f 6d70   field_meta.comp
+000063c0: 6172 6520 3d20 4661 6c73 650a 2020 2020  are = False.    
+000063d0: 2020 2020 6669 656c 645f 6d65 7461 2e68      field_meta.h
+000063e0: 6173 6820 3d20 4661 6c73 650a 2020 2020  ash = False.    
+000063f0: 2020 2020 6669 656c 645f 6d65 7461 2e72      field_meta.r
+00006400: 6570 7220 3d20 4661 6c73 650a 0a20 2020  epr = False..   
+00006410: 2065 7874 7261 5f66 6965 6c64 7320 3d20   extra_fields = 
+00006420: 5b28 2770 6172 656e 7427 2c20 5f50 6172  [('parent', _Par
+00006430: 656e 7454 7970 652c 0a20 2020 2020 2020  entType,.       
+00006440: 2020 2020 2020 2020 2020 2020 2020 6b77                kw
+00006450: 5f6f 6e6c 795f 6461 7461 636c 6173 7365  _only_dataclasse
+00006460: 732e 6669 656c 6428 0a20 2020 2020 2020  s.field(.       
+00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006480: 2020 7265 7072 3d46 616c 7365 2c20 6465    repr=False, de
+00006490: 6661 756c 743d 5f75 6e73 7065 6369 6669  fault=_unspecifi
+000064a0: 6564 5f70 6172 656e 742c 0a20 2020 2020  ed_parent,.     
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 2020 2020 6b77 5f6f 6e6c 793d 5472 7565      kw_only=True
+000064d0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+000064e0: 2020 2020 2020 2020 2827 6e61 6d65 272c          ('name',
+000064f0: 204f 7074 696f 6e61 6c5b 7374 725d 2c0a   Optional[str],.
+00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006510: 2020 2020 206b 775f 6f6e 6c79 5f64 6174       kw_only_dat
+00006520: 6163 6c61 7373 6573 2e66 6965 6c64 2864  aclasses.field(d
+00006530: 6566 6175 6c74 3d4e 6f6e 652c 206b 775f  efault=None, kw_
+00006540: 6f6e 6c79 3d54 7275 6529 295d 0a0a 2020  only=True))]..  
+00006550: 2020 6966 206b 775f 6f6e 6c79 3a0a 2020    if kw_only:.  
+00006560: 2020 2020 6966 2074 7570 6c65 2873 7973      if tuple(sys
+00006570: 2e76 6572 7369 6f6e 5f69 6e66 6f29 5b3a  .version_info)[:
+00006580: 335d 203e 3d20 2833 2c20 3130 2c20 3029  3] >= (3, 10, 0)
+00006590: 3a0a 2020 2020 2020 2020 666f 7220 6e61  :.        for na
+000065a0: 6d65 2c20 616e 6e6f 7461 7469 6f6e 2c20  me, annotation, 
+000065b0: 6465 6661 756c 7420 696e 2065 7874 7261  default in extra
+000065c0: 5f66 6965 6c64 733a 2020 2320 7079 7479  _fields:  # pyty
+000065d0: 7065 3a20 6469 7361 626c 653d 696e 7661  pe: disable=inva
+000065e0: 6c69 642d 616e 6e6f 7461 7469 6f6e 0a20  lid-annotation. 
+000065f0: 2020 2020 2020 2020 2073 6574 6174 7472           setattr
+00006600: 2863 6c73 2c20 6e61 6d65 2c20 6465 6661  (cls, name, defa
+00006610: 756c 7429 0a20 2020 2020 2020 2020 2063  ult).          c
+00006620: 6c73 2e5f 5f61 6e6e 6f74 6174 696f 6e73  ls.__annotations
+00006630: 5f5f 5b6e 616d 655d 203d 2061 6e6e 6f74  __[name] = annot
+00006640: 6174 696f 6e0a 2020 2020 2020 2020 6461  ation.        da
+00006650: 7461 636c 6173 7365 732e 6461 7461 636c  taclasses.datacl
+00006660: 6173 7328 0a20 2020 2020 2020 2020 2020  ass(.           
+00006670: 2075 6e73 6166 655f 6861 7368 3d27 5f5f   unsafe_hash='__
+00006680: 6861 7368 5f5f 2720 6e6f 7420 696e 2063  hash__' not in c
+00006690: 6c73 2e5f 5f64 6963 745f 5f2c 0a20 2020  ls.__dict__,.   
+000066a0: 2020 2020 2020 2020 2072 6570 723d 4661           repr=Fa
+000066b0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000066c0: 206b 775f 6f6e 6c79 3d54 7275 652c 0a20   kw_only=True,. 
+000066d0: 2020 2020 2020 2029 2863 6c73 2920 2023         )(cls)  #
+000066e0: 2074 7970 653a 2069 676e 6f72 655b 6361   type: ignore[ca
+000066f0: 6c6c 2d6f 7665 726c 6f61 645d 0a20 2020  ll-overload].   
+00006700: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006710: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+00006720: 2827 606b 775f 6f6e 6c79 6020 6973 206e  ('`kw_only` is n
+00006730: 6f74 2061 7661 696c 6162 6c65 2062 6566  ot available bef
+00006740: 6f72 6520 5079 2033 2e31 302e 2729 0a20  ore Py 3.10.'). 
+00006750: 2020 2065 6c73 653a 0a20 2020 2020 2023     else:.      #
+00006760: 204e 6f77 2061 7070 6c79 2064 6174 6163   Now apply datac
+00006770: 6c61 7373 2074 7261 6e73 666f 726d 2028  lass transform (
+00006780: 7768 6963 6820 6f70 6572 6174 6573 2069  which operates i
+00006790: 6e2d 706c 6163 6529 2e0a 2020 2020 2020  n-place)..      
+000067a0: 2320 446f 2067 656e 6572 6174 6520 6120  # Do generate a 
+000067b0: 6861 7368 2066 756e 6374 696f 6e20 6f6e  hash function on
+000067c0: 6c79 2069 6620 6e6f 7420 7072 6f76 6964  ly if not provid
+000067d0: 6564 2062 7920 7468 6520 636c 6173 732e  ed by the class.
+000067e0: 0a20 2020 2020 206b 775f 6f6e 6c79 5f64  .      kw_only_d
+000067f0: 6174 6163 6c61 7373 6573 2e64 6174 6163  ataclasses.datac
+00006800: 6c61 7373 280a 2020 2020 2020 2020 2020  lass(.          
+00006810: 636c 732c 0a20 2020 2020 2020 2020 2075  cls,.          u
+00006820: 6e73 6166 655f 6861 7368 3d27 5f5f 6861  nsafe_hash='__ha
+00006830: 7368 5f5f 2720 6e6f 7420 696e 2063 6c73  sh__' not in cls
+00006840: 2e5f 5f64 6963 745f 5f2c 0a20 2020 2020  .__dict__,.     
+00006850: 2020 2020 2072 6570 723d 4661 6c73 652c       repr=False,
+00006860: 0a20 2020 2020 2020 2020 2065 7874 7261  .          extra
+00006870: 5f66 6965 6c64 733d 6578 7472 615f 6669  _fields=extra_fi
+00006880: 656c 6473 2920 2023 2070 7974 7970 653a  elds)  # pytype:
+00006890: 2064 6973 6162 6c65 3d77 726f 6e67 2d6b   disable=wrong-k
+000068a0: 6579 776f 7264 2d61 7267 730a 0a20 2020  eyword-args..   
+000068b0: 2063 6c73 2e5f 5f68 6173 685f 5f20 3d20   cls.__hash__ = 
+000068c0: 5f77 7261 705f 6861 7368 2863 6c73 2e5f  _wrap_hash(cls._
+000068d0: 5f68 6173 685f 5f29 2020 2320 7479 7065  _hash__)  # type
+000068e0: 3a20 6967 6e6f 7265 5b6d 6574 686f 642d  : ignore[method-
+000068f0: 6173 7369 676e 5d0a 0a20 2040 636c 6173  assign]..  @clas
+00006900: 736d 6574 686f 640a 2020 6465 6620 5f76  smethod.  def _v
+00006910: 6572 6966 795f 7369 6e67 6c65 5f6f 725f  erify_single_or_
+00006920: 6e6f 5f63 6f6d 7061 6374 2863 6c73 293a  no_compact(cls):
+00006930: 0a20 2020 2022 2222 5374 6174 6963 616c  .    """Statical
+00006940: 6c79 2076 6572 6966 6965 7320 7468 6174  ly verifies that
+00006950: 2061 7420 6d6f 7374 2061 2073 696e 676c   at most a singl
+00006960: 6520 6d65 7468 6f64 2069 7320 6c61 6265  e method is labe
+00006970: 6c6c 6564 2063 6f6d 7061 6374 2e22 2222  lled compact."""
+00006980: 0a20 2020 206d 6574 686f 6473 203d 205b  .    methods = [
+00006990: 6d5b 305d 2066 6f72 206d 2069 6e20 696e  m[0] for m in in
+000069a0: 7370 6563 742e 6765 746d 656d 6265 7273  spect.getmembers
+000069b0: 2863 6c73 2c20 7072 6564 6963 6174 653d  (cls, predicate=
+000069c0: 6361 6c6c 6162 6c65 295d 0a20 2020 206e  callable)].    n
+000069d0: 5f63 6f6d 7061 6374 5f66 6e73 203d 206c  _compact_fns = l
+000069e0: 656e 285b 6d65 7468 6f64 5f6e 616d 6520  en([method_name 
+000069f0: 666f 7220 6d65 7468 6f64 5f6e 616d 6520  for method_name 
+00006a00: 696e 206d 6574 686f 6473 0a20 2020 2020  in methods.     
+00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a20: 2020 2020 6966 2068 6173 6174 7472 2867      if hasattr(g
+00006a30: 6574 6174 7472 2863 6c73 2c20 6d65 7468  etattr(cls, meth
+00006a40: 6f64 5f6e 616d 6529 2c20 2763 6f6d 7061  od_name), 'compa
+00006a50: 6374 2729 5d29 0a20 2020 2069 6620 6e5f  ct')]).    if n_
+00006a60: 636f 6d70 6163 745f 666e 7320 3e20 313a  compact_fns > 1:
+00006a70: 0a20 2020 2020 2072 6169 7365 2065 7272  .      raise err
+00006a80: 6f72 732e 4d75 6c74 6970 6c65 4d65 7468  ors.MultipleMeth
+00006a90: 6f64 7343 6f6d 7061 6374 4572 726f 7228  odsCompactError(
+00006aa0: 290a 0a20 2040 636c 6173 736d 6574 686f  )..  @classmetho
+00006ab0: 640a 2020 6465 6620 5f77 7261 705f 6d6f  d.  def _wrap_mo
+00006ac0: 6475 6c65 5f61 7474 7269 6275 7465 7328  dule_attributes(
+00006ad0: 636c 7329 3a0a 2020 2020 2222 2257 7261  cls):.    """Wra
+00006ae0: 7073 2075 7365 722d 6465 6669 6e65 6420  ps user-defined 
+00006af0: 6e6f 6e2d 696e 6865 7269 7465 6420 6d65  non-inherited me
+00006b00: 7468 6f64 7320 616e 6420 6465 7363 7269  thods and descri
+00006b10: 7074 6f72 7320 7769 7468 2073 7461 7465  ptors with state
+00006b20: 0a20 2020 206d 616e 6167 656d 656e 7420  .    management 
+00006b30: 6675 6e63 7469 6f6e 732e 0a20 2020 2022  functions..    "
+00006b40: 2222 0a20 2020 2023 2077 7261 7020 6d65  "".    # wrap me
+00006b50: 7468 6f64 730a 2020 2020 6d65 7468 6f64  thods.    method
+00006b60: 5f65 7863 6c75 7369 6f6e 7320 3d20 285b  _exclusions = ([
+00006b70: 662e 6e61 6d65 2066 6f72 2066 2069 6e20  f.name for f in 
+00006b80: 6461 7461 636c 6173 7365 732e 6669 656c  dataclasses.fiel
+00006b90: 6473 2863 6c73 295d 202b 0a20 2020 2020  ds(cls)] +.     
+00006ba0: 2020 2020 2020 2020 2020 2020 205b 275f               ['_
+00006bb0: 5f65 715f 5f27 2c20 275f 5f72 6570 725f  _eq__', '__repr_
+00006bc0: 5f27 2c20 275f 5f69 6e69 745f 5f27 2c20  _', '__init__', 
+00006bd0: 275f 5f68 6173 685f 5f27 2c0a 2020 2020  '__hash__',.    
+00006be0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006bf0: 5f5f 706f 7374 5f69 6e69 745f 5f27 5d29  __post_init__'])
+00006c00: 0a20 2020 2066 6f72 206b 6579 2069 6e20  .    for key in 
+00006c10: 5f67 6574 5f6c 6f63 616c 5f6d 6574 686f  _get_local_metho
+00006c20: 645f 6e61 6d65 7328 636c 732c 2065 7863  d_names(cls, exc
+00006c30: 6c75 6465 3d6d 6574 686f 645f 6578 636c  lude=method_excl
+00006c40: 7573 696f 6e73 293a 0a20 2020 2020 206d  usions):.      m
+00006c50: 6574 686f 6420 3d20 6765 7461 7474 7228  ethod = getattr(
+00006c60: 636c 732c 206b 6579 290a 2020 2020 2020  cls, key).      
+00006c70: 6966 2068 6173 6174 7472 286d 6574 686f  if hasattr(metho
+00006c80: 642c 2027 6e6f 7772 6170 2729 3a0a 2020  d, 'nowrap'):.  
+00006c90: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00006ca0: 2020 2020 2073 6574 6174 7472 2863 6c73       setattr(cls
+00006cb0: 2c20 6b65 792c 2077 7261 705f 6d65 7468  , key, wrap_meth
+00006cc0: 6f64 5f6f 6e63 6528 6d65 7468 6f64 2929  od_once(method))
+00006cd0: 0a0a 2020 2020 2320 7772 6170 2064 6573  ..    # wrap des
+00006ce0: 6372 6970 746f 7273 0a20 2020 2064 6573  criptors.    des
+00006cf0: 6372 6970 746f 725f 6578 636c 7573 696f  criptor_exclusio
+00006d00: 6e73 203d 2028 5b66 2e6e 616d 6520 666f  ns = ([f.name fo
+00006d10: 7220 6620 696e 2064 6174 6163 6c61 7373  r f in dataclass
+00006d20: 6573 2e66 6965 6c64 7328 636c 7329 5d20  es.fields(cls)] 
+00006d30: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
+00006d40: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00006d50: 2770 6172 656e 7427 2c20 275f 5f64 6963  'parent', '__dic
+00006d60: 745f 5f27 5d29 0a20 2020 2066 6f72 206b  t__']).    for k
+00006d70: 6579 2069 6e20 5f67 6574 5f6c 6f63 616c  ey in _get_local
+00006d80: 5f64 6573 6372 6970 746f 725f 6e61 6d65  _descriptor_name
+00006d90: 7328 636c 732c 2064 6573 6372 6970 746f  s(cls, descripto
+00006da0: 725f 6578 636c 7573 696f 6e73 293a 0a20  r_exclusions):. 
+00006db0: 2020 2020 2023 2064 6f6e 2774 2075 7365       # don't use
+00006dc0: 2067 6574 6174 7472 2068 6572 652c 2073   getattr here, s
+00006dd0: 696e 6365 2069 7420 7769 6c6c 2063 616c  ince it will cal
+00006de0: 6c20 7468 6520 6465 7363 7269 7074 6f72  l the descriptor
+00006df0: 0a20 2020 2020 2064 6573 6372 6970 746f  .      descripto
+00006e00: 7220 3d20 636c 732e 5f5f 6469 6374 5f5f  r = cls.__dict__
+00006e10: 5b6b 6579 5d0a 2020 2020 2020 6966 2068  [key].      if h
+00006e20: 6173 6174 7472 2864 6573 6372 6970 746f  asattr(descripto
+00006e30: 722c 2027 6e6f 7772 6170 2729 3a0a 2020  r, 'nowrap'):.  
+00006e40: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00006e50: 2020 2020 2073 6574 6174 7472 2863 6c73       setattr(cls
+00006e60: 2c20 6b65 792c 2077 7261 705f 6465 7363  , key, wrap_desc
+00006e70: 7269 7074 6f72 5f6f 6e63 6528 6465 7363  riptor_once(desc
+00006e80: 7269 7074 6f72 2929 0a20 2020 2072 6574  riptor)).    ret
+00006e90: 7572 6e20 636c 730a 0a20 2064 6566 205f  urn cls..  def _
+00006ea0: 6361 6c6c 5f77 7261 7070 6564 5f6d 6574  call_wrapped_met
+00006eb0: 686f 6428 7365 6c66 2c20 6675 6e2c 2061  hod(self, fun, a
+00006ec0: 7267 732c 206b 7761 7267 7329 3a0a 2020  rgs, kwargs):.  
+00006ed0: 2020 2222 2222 4361 6c6c 7320 6120 7772    """"Calls a wr
+00006ee0: 6170 7065 6420 6d65 7468 6f64 2e0a 0a20  apped method... 
+00006ef0: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+00006f00: 2069 7320 7265 7370 6f6e 7369 626c 6520   is responsible 
+00006f10: 666f 7220 7365 7474 696e 6720 7570 2074  for setting up t
+00006f20: 6865 2074 6872 6561 6420 6c6f 6361 6c20  he thread local 
+00006f30: 7374 6174 650a 2020 2020 636f 7272 6563  state.    correc
+00006f40: 746c 7920 6265 666f 7265 2063 616c 6c69  tly before calli
+00006f50: 6e67 2074 6865 206d 6574 686f 6420 616e  ng the method an
+00006f60: 6420 636c 6561 6e69 6e67 2075 7020 6166  d cleaning up af
+00006f70: 7465 7277 6172 6473 2e0a 2020 2020 5468  terwards..    Th
+00006f80: 6973 2069 6e63 6c75 6465 7320 7374 6f72  is includes stor
+00006f90: 696e 6720 696e 7465 726d 6564 6961 7465  ing intermediate
+00006fa0: 732c 2073 6574 7570 206f 6620 7468 6520  s, setup of the 
+00006fb0: 636f 6d70 6163 7420 7363 6f70 652c 0a20  compact scope,. 
+00006fc0: 2020 2061 6e64 206d 616b 696e 6720 7375     and making su
+00006fd0: 7265 2073 6574 7570 2069 7320 6361 6c6c  re setup is call
+00006fe0: 6564 2062 6566 6f72 6520 616e 7920 6f74  ed before any ot
+00006ff0: 6865 7220 6d65 7468 6f64 2e0a 0a20 2020  her method...   
+00007000: 2041 7267 733a 0a20 2020 2020 2066 756e   Args:.      fun
+00007010: 3a20 5468 6520 7772 6170 7065 6420 6d65  : The wrapped me
+00007020: 7468 6f64 2e0a 2020 2020 2020 6172 6773  thod..      args
+00007030: 3a20 4e61 6d65 6420 6172 6775 6d65 6e74  : Named argument
+00007040: 7320 7061 7373 6564 2074 6f20 6060 6675  s passed to ``fu
+00007050: 6e60 602e 0a20 2020 2020 206b 7761 7267  n``..      kwarg
+00007060: 733a 204b 6579 776f 7264 2061 7267 756d  s: Keyword argum
+00007070: 656e 7473 2070 6173 7365 6420 746f 2060  ents passed to `
+00007080: 6066 756e 6060 2e0a 0a20 2020 2052 6574  `fun``...    Ret
+00007090: 7572 6e73 3a0a 2020 2020 2020 5468 6520  urns:.      The 
+000070a0: 7265 7375 6c74 7320 6f66 2063 616c 6c69  results of calli
+000070b0: 6e67 2060 6066 756e 6060 2e0a 2020 2020  ng ``fun``..    
+000070c0: 2222 220a 2020 2020 6973 5f63 6f6d 7061  """.    is_compa
+000070d0: 6374 5f6d 6574 686f 6420 3d20 6861 7361  ct_method = hasa
+000070e0: 7474 7228 6675 6e2c 2027 636f 6d70 6163  ttr(fun, 'compac
+000070f0: 7427 290a 2020 2020 6675 6e5f 6e61 6d65  t').    fun_name
+00007100: 203d 2067 6574 6174 7472 2866 756e 2c20   = getattr(fun, 
+00007110: 275f 5f6e 616d 655f 5f27 2c20 2775 6e6e  '__name__', 'unn
+00007120: 616d 6564 5f66 756e 6374 696f 6e27 290a  amed_function').
+00007130: 2020 2020 6973 5f73 6574 7570 5f6d 6574      is_setup_met
+00007140: 686f 6420 3d20 6675 6e5f 6e61 6d65 203d  hod = fun_name =
+00007150: 3d20 2773 6574 7570 270a 2020 2020 6164  = 'setup'.    ad
+00007160: 645f 6361 6c6c 5f69 6e66 6f20 3d20 6e6f  d_call_info = no
+00007170: 7420 6973 5f73 6574 7570 5f6d 6574 686f  t is_setup_metho
+00007180: 6420 616e 6420 6c65 6e28 5f63 6f6e 7465  d and len(_conte
+00007190: 7874 2e63 616c 6c5f 696e 666f 5f73 7461  xt.call_info_sta
+000071a0: 636b 2920 3e20 300a 2020 2020 2320 5765  ck) > 0.    # We
+000071b0: 206c 617a 696c 7920 6361 6c6c 2073 6574   lazily call set
+000071c0: 7570 2829 206f 6e6c 7920 7768 656e 206e  up() only when n
+000071d0: 6565 6465 642e 0a20 2020 2069 6620 6973  eeded..    if is
+000071e0: 5f73 6574 7570 5f6d 6574 686f 643a 0a20  _setup_method:. 
+000071f0: 2020 2020 2069 6620 7365 6c66 2e73 636f       if self.sco
+00007200: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+00007210: 2020 2020 7261 6973 6520 6572 726f 7273      raise errors
+00007220: 2e43 616c 6c53 6574 7570 556e 626f 756e  .CallSetupUnboun
+00007230: 644d 6f64 756c 6545 7272 6f72 2829 0a20  dModuleError(). 
+00007240: 2020 2020 2069 735f 7265 6375 7272 656e       is_recurren
+00007250: 7420 3d20 7365 6c66 2e5f 7374 6174 652e  t = self._state.
+00007260: 696e 5f73 6574 7570 0a20 2020 2020 2073  in_setup.      s
+00007270: 656c 662e 5f73 7461 7465 2e69 6e5f 7365  elf._state.in_se
+00007280: 7475 7020 3d20 5472 7565 0a20 2020 2065  tup = True.    e
+00007290: 6c73 653a 0a20 2020 2020 2073 656c 662e  lse:.      self.
+000072a0: 5f74 7279 5f73 6574 7570 2829 0a0a 2020  _try_setup()..  
+000072b0: 2020 6966 2069 735f 636f 6d70 6163 745f    if is_compact_
+000072c0: 6d65 7468 6f64 3a0a 2020 2020 2020 6966  method:.      if
+000072d0: 2073 656c 662e 7363 6f70 6520 6973 204e   self.scope is N
+000072e0: 6f6e 653a 0a20 2020 2020 2020 2072 6169  one:.        rai
+000072f0: 7365 2065 7272 6f72 732e 4361 6c6c 436f  se errors.CallCo
+00007300: 6d70 6163 7455 6e62 6f75 6e64 4d6f 6475  mpactUnboundModu
+00007310: 6c65 4572 726f 7228 290a 2020 2020 2020  leError().      
+00007320: 6973 5f72 6563 7572 7265 6e74 203d 2073  is_recurrent = s
+00007330: 656c 662e 5f73 7461 7465 2e69 6e5f 636f  elf._state.in_co
+00007340: 6d70 6163 745f 6d65 7468 6f64 0a20 2020  mpact_method.   
+00007350: 2020 2073 656c 662e 5f73 7461 7465 2e69     self._state.i
+00007360: 6e5f 636f 6d70 6163 745f 6d65 7468 6f64  n_compact_method
+00007370: 203d 2054 7275 650a 2020 2020 5f63 6f6e   = True.    _con
+00007380: 7465 7874 2e6d 6f64 756c 655f 7374 6163  text.module_stac
+00007390: 6b2e 6170 7065 6e64 2873 656c 6629 0a20  k.append(self). 
+000073a0: 2020 2074 7279 3a0a 2020 2020 2020 2320     try:.      # 
+000073b0: 6765 7420 6361 6c6c 2069 6e66 6f0a 2020  get call info.  
+000073c0: 2020 2020 6966 2061 6464 5f63 616c 6c5f      if add_call_
+000073d0: 696e 666f 3a0a 2020 2020 2020 2020 6173  info:.        as
+000073e0: 7365 7274 2073 656c 662e 7363 6f70 6520  sert self.scope 
+000073f0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+00007400: 2020 2020 6361 6c6c 5f69 6e64 6578 203d      call_index =
+00007410: 205f 636f 6e74 6578 742e 6361 6c6c 5f69   _context.call_i
+00007420: 6e66 6f5f 7374 6163 6b5b 2d31 5d2e 6765  nfo_stack[-1].ge
+00007430: 745f 6361 6c6c 5f69 6e64 6578 2873 656c  t_call_index(sel
+00007440: 6629 0a20 2020 2020 2020 2073 636f 7065  f).        scope
+00007450: 5f70 6174 6820 3d20 6a61 782e 7472 6565  _path = jax.tree
+00007460: 5f75 7469 6c2e 7472 6565 5f6d 6170 285f  _util.tree_map(_
+00007470: 6669 785f 7061 7468 5f70 6172 742c 2073  fix_path_part, s
+00007480: 656c 662e 7363 6f70 652e 7061 7468 290a  elf.scope.path).
+00007490: 0a20 2020 2020 2023 2063 616c 6c20 6d65  .      # call me
+000074a0: 7468 6f64 0a20 2020 2020 2069 6620 5f75  thod.      if _u
+000074b0: 7365 5f6e 616d 6564 5f63 616c 6c3a 0a20  se_named_call:. 
+000074c0: 2020 2020 2020 2077 6974 6820 6a61 782e         with jax.
+000074d0: 6e61 6d65 645f 7363 6f70 6528 5f64 6572  named_scope(_der
+000074e0: 6976 655f 7072 6f66 696c 696e 675f 6e61  ive_profiling_na
+000074f0: 6d65 2873 656c 662c 2066 756e 2929 3a0a  me(self, fun)):.
+00007500: 2020 2020 2020 2020 2020 7920 3d20 6675            y = fu
+00007510: 6e28 7365 6c66 2c20 2a61 7267 732c 202a  n(self, *args, *
+00007520: 2a6b 7761 7267 7329 0a20 2020 2020 2065  *kwargs).      e
+00007530: 6c73 653a 0a20 2020 2020 2020 2079 203d  lse:.        y =
+00007540: 2066 756e 2873 656c 662c 202a 6172 6773   fun(self, *args
+00007550: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+00007560: 2020 2069 6620 5f63 6f6e 7465 7874 2e63     if _context.c
+00007570: 6170 7475 7265 5f73 7461 636b 3a0a 2020  apture_stack:.  
+00007580: 2020 2020 2020 6669 6c74 6572 5f66 6e20        filter_fn 
+00007590: 3d20 5f63 6f6e 7465 7874 2e63 6170 7475  = _context.captu
+000075a0: 7265 5f73 7461 636b 5b2d 315d 0a20 2020  re_stack[-1].   
+000075b0: 2020 2020 2069 6620 6669 6c74 6572 5f66       if filter_f
+000075c0: 6e20 616e 6420 6669 6c74 6572 5f66 6e28  n and filter_fn(
+000075d0: 7365 6c66 2c20 6675 6e5f 6e61 6d65 293a  self, fun_name):
+000075e0: 0a20 2020 2020 2020 2020 2073 656c 662e  .          self.
+000075f0: 736f 7728 2769 6e74 6572 6d65 6469 6174  sow('intermediat
+00007600: 6573 272c 2066 756e 5f6e 616d 652c 2079  es', fun_name, y
+00007610: 290a 2020 2020 2020 6966 2061 6464 5f63  ).      if add_c
+00007620: 616c 6c5f 696e 666f 3a0a 2020 2020 2020  all_info:.      
+00007630: 2020 5f61 7267 732c 205f 6b77 6172 6773    _args, _kwargs
+00007640: 2c20 5f79 203d 2066 6c61 782e 6c69 6e65  , _y = flax.line
+00007650: 6e2e 7375 6d6d 6172 792e 5f72 6570 7265  n.summary._repre
+00007660: 7365 6e74 5f74 7265 6528 2861 7267 732c  sent_tree((args,
+00007670: 206b 7761 7267 732c 2079 2929 0a20 2020   kwargs, y)).   
+00007680: 2020 2020 205f 636f 6e74 6578 742e 6361       _context.ca
+00007690: 6c6c 5f69 6e66 6f5f 7374 6163 6b5b 2d31  ll_info_stack[-1
+000076a0: 5d2e 6361 6c6c 732e 6170 7065 6e64 280a  ].calls.append(.
+000076b0: 2020 2020 2020 2020 2020 5f43 616c 6c49            _CallI
+000076c0: 6e66 6f28 6361 6c6c 5f69 6e64 6578 2c20  nfo(call_index, 
+000076d0: 7363 6f70 655f 7061 7468 2c20 7479 7065  scope_path, type
+000076e0: 2873 656c 6629 2c20 6675 6e2e 5f5f 6e61  (self), fun.__na
+000076f0: 6d65 5f5f 2c20 5f61 7267 732c 205f 6b77  me__, _args, _kw
+00007700: 6172 6773 2c20 5f79 2929 0a20 2020 2020  args, _y)).     
+00007710: 2072 6574 7572 6e20 790a 2020 2020 6669   return y.    fi
+00007720: 6e61 6c6c 793a 0a20 2020 2020 205f 636f  nally:.      _co
+00007730: 6e74 6578 742e 6d6f 6475 6c65 5f73 7461  ntext.module_sta
+00007740: 636b 2e70 6f70 2829 0a20 2020 2020 2069  ck.pop().      i
+00007750: 6620 6973 5f63 6f6d 7061 6374 5f6d 6574  f is_compact_met
+00007760: 686f 643a 0a20 2020 2020 2020 206f 626a  hod:.        obj
+00007770: 6563 742e 5f5f 7365 7461 7474 725f 5f28  ect.__setattr__(
+00007780: 7365 6c66 2c20 2773 636f 7065 272c 2073  self, 'scope', s
+00007790: 656c 662e 7363 6f70 652e 7265 776f 756e  elf.scope.rewoun
+000077a0: 6428 2929 0a20 2020 2020 2023 2073 6574  d()).      # set
+000077b0: 7570 206f 7220 636f 6d70 6163 7420 6361  up or compact ca
+000077c0: 6c6c 7320 6361 6e20 6265 2072 6563 7572  lls can be recur
+000077d0: 7265 6e74 2066 6f72 2065 7861 6d70 6c65  rent for example
+000077e0: 2064 7565 2074 6f20 7375 7065 7220 6361   due to super ca
+000077f0: 6c6c 730a 2020 2020 2020 2320 7265 7365  lls.      # rese
+00007800: 7474 696e 6720 7468 6520 7374 6174 6520  tting the state 
+00007810: 776f 756c 6420 6361 7573 6520 6973 2063  would cause is c
+00007820: 6f6d 7061 6374 2f73 6574 7570 206d 6574  ompact/setup met
+00007830: 686f 640a 2020 2020 2020 2320 746f 2062  hod.      # to b
+00007840: 6520 7365 7420 746f 2046 616c 7365 2070  e set to False p
+00007850: 7265 6d61 7475 7265 6c79 2e0a 2020 2020  rematurely..    
+00007860: 2020 6966 2028 6973 5f63 6f6d 7061 6374    if (is_compact
+00007870: 5f6d 6574 686f 6420 6f72 2069 735f 7365  _method or is_se
+00007880: 7475 705f 6d65 7468 6f64 2920 616e 6420  tup_method) and 
+00007890: 6e6f 7420 6973 5f72 6563 7572 7265 6e74  not is_recurrent
+000078a0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+000078b0: 7374 6174 652e 7265 7365 7428 290a 0a20  state.reset().. 
+000078c0: 2064 6566 205f 5f73 6574 6174 7472 5f5f   def __setattr__
+000078d0: 2873 656c 662c 206e 616d 653a 2073 7472  (self, name: str
+000078e0: 2c20 7661 6c3a 2041 6e79 293a 0a20 2020  , val: Any):.   
+000078f0: 2022 2222 5365 7473 2061 6e20 6174 7472   """Sets an attr
+00007900: 6962 7574 6520 6f6e 2074 6869 7320 4d6f  ibute on this Mo
+00007910: 6475 6c65 2e0a 0a20 2020 2057 6520 6f76  dule...    We ov
+00007920: 6572 6c6f 6164 2073 6574 6174 7472 2073  erload setattr s
+00007930: 6f6c 656c 7920 746f 2073 7570 706f 7274  olely to support
+00007940: 2070 7974 686f 6e69 6320 6e61 6d69 6e67   pythonic naming
+00007950: 2076 6961 2061 7373 6967 6e6d 656e 7420   via assignment 
+00007960: 6f66 0a20 2020 2073 7562 6d6f 6475 6c65  of.    submodule
+00007970: 7320 696e 2074 6865 2073 7065 6369 616c  s in the special
+00007980: 203a 6d65 7468 3a60 7365 7475 7060 2066   :meth:`setup` f
+00007990: 756e 6374 696f 6e3a 3a0a 0a20 2020 2020  unction::..     
+000079a0: 2073 656c 662e 7375 626d 6f64 756c 655f   self.submodule_
+000079b0: 6e61 6d65 203d 204d 794d 6f64 756c 6528  name = MyModule(
+000079c0: 2e2e 2e29 0a0a 2020 2020 5765 2061 6c73  ...)..    We als
+000079d0: 6f20 7375 7070 6f72 7420 6c69 7374 7320  o support lists 
+000079e0: 616e 6420 6f74 6865 7220 6765 6e65 7261  and other genera
+000079f0: 6c20 7079 7472 6565 732c 2065 2e67 2e3a  l pytrees, e.g.:
+00007a00: 3a0a 0a20 2020 2020 2073 656c 662e 7375  :..      self.su
+00007a10: 626d 6f64 756c 6573 203d 205b 4d79 4d6f  bmodules = [MyMo
+00007a20: 6475 6c65 3028 2e2e 292c 204d 794d 6f64  dule0(..), MyMod
+00007a30: 756c 6531 282e 2e29 2c20 2e2e 2e5d 0a0a  ule1(..), ...]..
+00007a40: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00007a50: 6e61 6d65 3a20 4174 7472 6962 7574 6520  name: Attribute 
+00007a60: 746f 2073 6574 2e0a 2020 2020 2020 7661  to set..      va
+00007a70: 6c3a 2056 616c 7565 206f 6620 7468 6520  l: Value of the 
+00007a80: 6174 7472 6962 7574 652e 0a20 2020 2022  attribute..    "
+00007a90: 2222 0a20 2020 2066 6965 6c64 7320 3d20  "".    fields = 
+00007aa0: 7365 6c66 2e5f 5f64 6174 6163 6c61 7373  self.__dataclass
+00007ab0: 5f66 6965 6c64 735f 5f20 2023 2070 7974  _fields__  # pyt
+00007ac0: 7970 653a 2064 6973 6162 6c65 3d61 7474  ype: disable=att
+00007ad0: 7269 6275 7465 2d65 7272 6f72 0a20 2020  ribute-error.   
+00007ae0: 2069 735f 6461 7461 636c 6173 735f 6174   is_dataclass_at
+00007af0: 7472 203d 206e 616d 6520 696e 2066 6965  tr = name in fie
+00007b00: 6c64 7320 616e 6420 6669 656c 6473 5b6e  lds and fields[n
+00007b10: 616d 655d 2e69 6e69 740a 0a20 2020 2069  ame].init..    i
+00007b20: 6620 6e6f 7420 7365 6c66 2e5f 7374 6174  f not self._stat
+00007b30: 652e 696e 5f73 6574 7570 3a0a 2020 2020  e.in_setup:.    
+00007b40: 2020 6966 206e 6f74 2073 656c 662e 5f73    if not self._s
+00007b50: 7461 7465 2e69 735f 696e 6974 6961 6c69  tate.is_initiali
+00007b60: 7a65 643a 0a20 2020 2020 2020 2023 2053  zed:.        # S
+00007b70: 6574 7469 6e67 2061 7474 7269 6275 7465  etting attribute
+00007b80: 7320 6265 666f 7265 2065 6e64 206f 6620  s before end of 
+00007b90: 4d6f 6475 6c65 2e5f 5f70 6f73 745f 696e  Module.__post_in
+00007ba0: 6974 5f5f 2829 0a20 2020 2020 2020 206f  it__().        o
+00007bb0: 626a 6563 742e 5f5f 7365 7461 7474 725f  bject.__setattr_
+00007bc0: 5f28 7365 6c66 2c20 6e61 6d65 2c20 7661  _(self, name, va
+00007bd0: 6c29 0a20 2020 2020 2020 2072 6574 7572  l).        retur
+00007be0: 6e0a 2020 2020 2020 656c 7365 3a0a 2020  n.      else:.  
+00007bf0: 2020 2020 2020 2320 5765 2772 6520 7061        # We're pa
+00007c00: 7374 2061 6c6c 2069 6e69 7469 616c 697a  st all initializ
+00007c10: 6174 696f 6e20 616e 6420 7365 7475 7020  ation and setup 
+00007c20: 6c6f 6769 633a 0a20 2020 2020 2020 2023  logic:.        #
+00007c30: 2052 6169 7365 7320 6120 5479 7065 4572   Raises a TypeEr
+00007c40: 726f 7220 6a75 7374 206c 696b 6520 6672  ror just like fr
+00007c50: 6f7a 656e 2070 7974 686f 6e20 6461 7461  ozen python data
+00007c60: 636c 6173 7365 732e 0a20 2020 2020 2020  classes..       
+00007c70: 2072 6169 7365 2065 7272 6f72 732e 5365   raise errors.Se
+00007c80: 7441 7474 7269 6275 7465 4672 6f7a 656e  tAttributeFrozen
+00007c90: 4d6f 6475 6c65 4572 726f 7228 0a20 2020  ModuleError(.   
+00007ca0: 2020 2020 2020 2020 2073 656c 662e 5f5f           self.__
+00007cb0: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+00007cc0: 2c20 6e61 6d65 2c20 7661 6c29 0a0a 2020  , name, val)..  
+00007cd0: 2020 2320 5765 2772 6520 696e 7369 6465    # We're inside
+00007ce0: 2074 6865 2073 6574 7570 2829 206d 6574   the setup() met
+00007cf0: 686f 643a 0a20 2020 2069 6620 6973 5f64  hod:.    if is_d
+00007d00: 6174 6163 6c61 7373 5f61 7474 723a 0a20  ataclass_attr:. 
+00007d10: 2020 2020 2023 2054 6865 7365 206e 616d       # These nam
+00007d20: 6573 2061 7265 2073 7065 6369 6669 6564  es are specified
+00007d30: 2061 7320 6461 7461 636c 6173 7320 6669   as dataclass fi
+00007d40: 656c 6473 2e20 5468 6579 2073 686f 756c  elds. They shoul
+00007d50: 6420 6e6f 7420 6265 0a20 2020 2020 2023  d not be.      #
+00007d60: 2069 6e69 7469 616c 697a 6564 2077 6974   initialized wit
+00007d70: 6869 6e20 7468 6520 7365 7475 7028 2920  hin the setup() 
+00007d80: 6d65 7468 6f64 2c20 6275 7420 6361 6e20  method, but can 
+00007d90: 6265 206d 6f64 6966 6965 6420 6672 6565  be modified free
+00007da0: 6c79 0a20 2020 2020 2023 2062 6566 6f72  ly.      # befor
+00007db0: 6520 6974 2e0a 2020 2020 2020 7261 6973  e it..      rais
+00007dc0: 6520 6572 726f 7273 2e53 6574 4174 7472  e errors.SetAttr
+00007dd0: 6962 7574 6549 6e4d 6f64 756c 6553 6574  ibuteInModuleSet
+00007de0: 7570 4572 726f 7228 290a 0a20 2020 2023  upError()..    #
+00007df0: 2056 616c 7565 7320 2874 6861 7420 6d61   Values (that ma
+00007e00: 7920 6265 2076 6172 6961 626c 6573 206f  y be variables o
+00007e10: 7220 7375 626d 6f64 756c 6573 2920 6172  r submodules) ar
+00007e20: 6520 6265 696e 6720 6465 6669 6e65 6420  e being defined 
+00007e30: 616e 640a 2020 2020 2320 6174 7461 6368  and.    # attach
+00007e40: 6564 2069 6e20 7365 7475 7028 292c 2077  ed in setup(), w
+00007e50: 6520 7275 6e20 736f 6d65 2065 7874 7261  e run some extra
+00007e60: 206c 6f67 6963 2069 6e20 7468 6174 2063   logic in that c
+00007e70: 6173 652e 0a20 2020 2073 656c 662e 5f72  ase..    self._r
+00007e80: 6567 6973 7465 725f 7375 626d 6f64 756c  egister_submodul
+00007e90: 6573 286e 616d 652c 2076 616c 290a 0a20  es(name, val).. 
+00007ea0: 2064 6566 205f 5f67 6574 6174 7472 5f5f   def __getattr__
+00007eb0: 2873 656c 662c 206e 616d 653a 2073 7472  (self, name: str
+00007ec0: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
+00007ed0: 2243 616c 6c20 7365 7475 7028 2920 6265  "Call setup() be
+00007ee0: 666f 7265 2067 6574 7469 6e67 2061 6e79  fore getting any
+00007ef0: 2073 6574 7570 2d64 6566 696e 6564 2061   setup-defined a
+00007f00: 7474 7269 6275 7465 732e 2222 220a 2020  ttributes.""".  
+00007f10: 2020 2320 5765 2064 6f6e 2774 2077 616e    # We don't wan
+00007f20: 7420 746f 2072 6574 7572 6e20 616e 7974  t to return anyt
+00007f30: 6869 6e67 2066 6f72 2070 7974 686f 6e20  hing for python 
+00007f40: 636f 7079 202f 2070 6963 6b6c 6520 6d65  copy / pickle me
+00007f50: 7468 6f64 732e 0a20 2020 2069 6620 6e61  thods..    if na
+00007f60: 6d65 2069 6e20 5f55 4e44 4546 494e 4544  me in _UNDEFINED
+00007f70: 5f43 4f50 595f 5049 434b 4c45 5f4d 4554  _COPY_PICKLE_MET
+00007f80: 484f 4453 3a0a 2020 2020 2020 7261 6973  HODS:.      rais
+00007f90: 6520 4174 7472 6962 7574 6545 7272 6f72  e AttributeError
+00007fa0: 2829 0a20 2020 2073 656c 662e 5f74 7279  ().    self._try
+00007fb0: 5f73 6574 7570 2829 0a20 2020 2069 6620  _setup().    if 
+00007fc0: 6e61 6d65 2069 6e20 7365 6c66 2e5f 5f64  name in self.__d
+00007fd0: 6963 745f 5f3a 0a20 2020 2020 2072 6574  ict__:.      ret
+00007fe0: 7572 6e20 7365 6c66 2e5f 5f64 6963 745f  urn self.__dict_
+00007ff0: 5f5b 6e61 6d65 5d0a 2020 2020 656c 7365  _[name].    else
+00008000: 3a0a 2020 2020 2020 6d73 6720 3d20 6627  :.      msg = f'
+00008010: 227b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  "{self.__class__
+00008020: 2e5f 5f6e 616d 655f 5f7d 2220 6f62 6a65  .__name__}" obje
+00008030: 6374 2068 6173 206e 6f20 6174 7472 6962  ct has no attrib
+00008040: 7574 6520 227b 6e61 6d65 7d22 2e27 0a20  ute "{name}".'. 
+00008050: 2020 2020 2069 6620 7365 6c66 2e73 636f       if self.sco
+00008060: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+00008070: 2020 2020 6d73 6720 2b3d 2028 6627 2049      msg += (f' I
+00008080: 6620 227b 6e61 6d65 7d22 2069 7320 6465  f "{name}" is de
+00008090: 6669 6e65 6420 696e 205c 272e 7365 7475  fined in \'.setu
+000080a0: 7028 295c 272c 2072 656d 656d 6265 7220  p()\', remember 
+000080b0: 7468 6573 6520 6669 656c 6473 2027 0a20  these fields '. 
+000080c0: 2020 2020 2020 2020 2027 6172 6520 6f6e           'are on
+000080d0: 6c79 2061 6363 6573 7369 626c 6520 6672  ly accessible fr
+000080e0: 6f6d 2069 6e73 6964 6520 5c27 696e 6974  om inside \'init
+000080f0: 5c27 206f 7220 5c27 6170 706c 795c 272e  \' or \'apply\'.
+00008100: 2729 0a20 2020 2020 2072 6169 7365 2041  ').      raise A
+00008110: 7474 7269 6275 7465 4572 726f 7228 6d73  ttributeError(ms
+00008120: 6729 0a0a 2020 6465 6620 5f5f 6469 725f  g)..  def __dir_
+00008130: 5f28 7365 6c66 2920 2d3e 204c 6973 745b  _(self) -> List[
+00008140: 7374 725d 3a0a 2020 2020 2222 2243 616c  str]:.    """Cal
+00008150: 6c20 7365 7475 7028 2920 6265 666f 7265  l setup() before
+00008160: 206c 6973 7469 6e67 2061 7474 7269 6275   listing attribu
+00008170: 7465 732e 2222 220a 2020 2020 7365 6c66  tes.""".    self
+00008180: 2e5f 7472 795f 7365 7475 7028 290a 2020  ._try_setup().  
+00008190: 2020 7265 7475 726e 206f 626a 6563 742e    return object.
+000081a0: 5f5f 6469 725f 5f28 7365 6c66 2920 2023  __dir__(self)  #
+000081b0: 2074 7970 653a 2069 676e 6f72 650a 0a20   type: ignore.. 
+000081c0: 2064 6566 205f 5f70 6f73 745f 696e 6974   def __post_init
+000081d0: 5f5f 2873 656c 6629 202d 3e20 4e6f 6e65  __(self) -> None
+000081e0: 3a0a 2020 2020 2320 444f 204e 4f54 2052  :.    # DO NOT R
+000081f0: 454d 4f56 4520 2d20 4d61 726b 6572 2066  EMOVE - Marker f
+00008200: 6f72 2069 6e74 6572 6e61 6c20 6c6f 6767  or internal logg
+00008210: 696e 672e 0a20 2020 2023 2049 6e20 6461  ing..    # In da
+00008220: 7461 636c 6173 7365 732c 205f 5f69 6e69  taclasses, __ini
+00008230: 745f 5f20 6973 206f 7665 7272 6964 6465  t__ is overridde
+00008240: 6e20 746f 2070 726f 6365 7373 2064 6174  n to process dat
+00008250: 6163 6c61 7373 2061 7267 756d 656e 7473  aclass arguments
+00008260: 2c0a 2020 2020 2320 616e 6420 5f5f 706f  ,.    # and __po
+00008270: 7374 5f69 6e69 745f 5f20 6973 2063 616c  st_init__ is cal
+00008280: 6c65 6420 696d 6d65 6469 6174 656c 7920  led immediately 
+00008290: 6166 7465 7277 6172 6473 2e20 4865 7265  afterwards. Here
+000082a0: 2c20 6465 7065 6e64 696e 6720 6f6e 2074  , depending on t
+000082b0: 6865 0a20 2020 2023 2074 7970 6520 6f66  he.    # type of
+000082c0: 2060 7061 7265 6e74 6020 7061 7373 6564   `parent` passed
+000082d0: 2074 6f20 696e 6974 6961 6c69 7a65 2074   to initialize t
+000082e0: 6865 204d 6f64 756c 652c 2077 6520 6569  he Module, we ei
+000082f0: 7468 6572 2064 6566 6572 0a20 2020 2023  ther defer.    #
+00008300: 2069 6e69 7469 616c 697a 6174 696f 6e2c   initialization,
+00008310: 2061 7474 6163 6820 7468 6973 204d 6f64   attach this Mod
+00008320: 756c 6520 6173 2061 2073 7562 6d6f 6475  ule as a submodu
+00008330: 6c65 206f 6620 6120 7061 7265 6e74 2c20  le of a parent, 
+00008340: 6f72 2062 696e 640a 2020 2020 2320 7468  or bind.    # th
+00008350: 6973 204d 6f64 756c 6520 6174 2074 6865  is Module at the
+00008360: 2074 6f70 2d6c 6576 656c 2074 6f20 7661   top-level to va
+00008370: 7269 6162 6c65 7320 616e 6420 726e 6773  riables and rngs
+00008380: 2e0a 0a20 2020 206f 626a 6563 742e 5f5f  ...    object.__
+00008390: 7365 7461 7474 725f 5f28 7365 6c66 2c20  setattr__(self, 
+000083a0: 275f 6964 272c 2075 7569 6428 2929 0a20  '_id', uuid()). 
+000083b0: 2020 206f 626a 6563 742e 5f5f 7365 7461     object.__seta
+000083c0: 7474 725f 5f28 7365 6c66 2c20 275f 7374  ttr__(self, '_st
+000083d0: 6174 6527 2c20 5f4d 6f64 756c 6549 6e74  ate', _ModuleInt
+000083e0: 6572 6e61 6c53 7461 7465 2829 290a 0a20  ernalState()).. 
+000083f0: 2020 2023 2054 7970 6963 616c 6c79 2077     # Typically w
+00008400: 6520 7365 7420 7468 6520 7061 7265 6e74  e set the parent
+00008410: 2062 6173 6564 206f 6e20 7468 6520 6479   based on the dy
+00008420: 6e61 6d69 6320 6d6f 6475 6c65 2063 6f6e  namic module con
+00008430: 7465 7874 2e0a 2020 2020 6966 2073 656c  text..    if sel
+00008440: 662e 7061 7265 6e74 2069 7320 5f75 6e73  f.parent is _uns
+00008450: 7065 6369 6669 6564 5f70 6172 656e 743a  pecified_parent:
+00008460: 2020 2320 7079 7479 7065 3a20 6469 7361    # pytype: disa
+00008470: 626c 653d 6174 7472 6962 7574 652d 6572  ble=attribute-er
+00008480: 726f 720a 2020 2020 2020 6f62 6a65 6374  ror.      object
+00008490: 2e5f 5f73 6574 6174 7472 5f5f 2873 656c  .__setattr__(sel
+000084a0: 662c 2027 7061 7265 6e74 272c 205f 636f  f, 'parent', _co
+000084b0: 6e74 6578 742e 6d6f 6475 6c65 5f73 7461  ntext.module_sta
+000084c0: 636b 5b2d 315d 290a 0a20 2020 2023 2049  ck[-1])..    # I
+000084d0: 6e69 7469 616c 697a 6174 696f 6e20 6973  nitialization is
+000084e0: 2064 6566 6572 7265 6420 666f 7220 746f   deferred for to
+000084f0: 7020 6c65 7665 6c20 4d6f 6475 6c65 7320  p level Modules 
+00008500: 6f72 2061 6e79 206f 7468 6572 2022 6f72  or any other "or
+00008510: 7068 616e 220a 2020 2020 2320 4d6f 6475  phan".    # Modu
+00008520: 6c65 7320 756e 7469 6c20 6174 7461 6368  les until attach
+00008530: 6d65 6e74 2062 7920 5f5f 7365 7461 7474  ment by __setatt
+00008540: 725f 5f20 692e 652e 204d 794d 6f64 756c  r__ i.e. MyModul
+00008550: 6528 2e2e 2e2c 2070 6172 656e 743d 4e6f  e(..., parent=No
+00008560: 6e65 290a 2020 2020 6966 2073 656c 662e  ne).    if self.
+00008570: 7061 7265 6e74 2069 7320 4e6f 6e65 3a0a  parent is None:.
+00008580: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00008590: 2020 2320 5265 6769 7374 6572 2073 7562    # Register sub
+000085a0: 6d6f 6475 6c65 206f 6e20 7061 7265 6e74  module on parent
+000085b0: 204d 6f64 756c 652e 0a20 2020 2069 6620   Module..    if 
+000085c0: 6973 696e 7374 616e 6365 2873 656c 662e  isinstance(self.
+000085d0: 7061 7265 6e74 2c20 4d6f 6475 6c65 293a  parent, Module):
+000085e0: 0a20 2020 2020 2023 2057 6865 6e20 696e  .      # When in
+000085f0: 6974 6961 6c69 7a69 6e67 2061 6e20 756e  itializing an un
+00008600: 6e61 6d65 6420 4d6f 6475 6c65 2069 6e73  named Module ins
+00008610: 6964 6520 7365 7475 7028 290a 2020 2020  ide setup().    
+00008620: 2020 2320 696e 6974 6961 6c69 7a61 7469    # initializati
+00008630: 6f6e 2069 7320 6465 6665 7272 6564 2075  on is deferred u
+00008640: 6e74 696c 2061 7474 6163 686d 656e 7420  ntil attachment 
+00008650: 6279 205f 5f73 6574 6174 7472 5f5f 0a20  by __setattr__. 
+00008660: 2020 2020 2023 2069 2e65 2e20 7365 6c66       # i.e. self
+00008670: 2e6d 796d 6f64 756c 6520 3d20 4d79 4d6f  .mymodule = MyMo
+00008680: 6475 6c65 282e 2e2e 290a 2020 2020 2020  dule(...).      
+00008690: 7365 6c66 2e6e 616d 653a 204f 7074 696f  self.name: Optio
+000086a0: 6e61 6c5b 7374 725d 0a20 2020 2020 2069  nal[str].      i
+000086b0: 6620 7365 6c66 2e70 6172 656e 742e 5f73  f self.parent._s
+000086c0: 7461 7465 2e69 6e5f 7365 7475 7020 616e  tate.in_setup an
+000086d0: 6420 7365 6c66 2e6e 616d 6520 6973 204e  d self.name is N
+000086e0: 6f6e 653a 2020 2320 7079 7479 7065 3a20  one:  # pytype: 
+000086f0: 6469 7361 626c 653d 6174 7472 6962 7574  disable=attribut
+00008700: 652d 6572 726f 720a 2020 2020 2020 2020  e-error.        
+00008710: 7265 7475 726e 0a20 2020 2020 2069 6620  return.      if 
+00008720: 6e6f 7420 7365 6c66 2e70 6172 656e 742e  not self.parent.
+00008730: 5f69 6e69 7469 616c 697a 6174 696f 6e5f  _initialization_
+00008740: 616c 6c6f 7765 643a 0a20 2020 2020 2020  allowed:.       
+00008750: 2072 6169 7365 2065 7272 6f72 732e 4173   raise errors.As
+00008760: 7369 676e 5375 624d 6f64 756c 6545 7272  signSubModuleErr
+00008770: 6f72 2873 656c 662e 5f5f 636c 6173 735f  or(self.__class_
+00008780: 5f2e 5f5f 6e61 6d65 5f5f 290a 2020 2020  _.__name__).    
+00008790: 2020 2320 4175 746f 6e61 6d69 6e67 206f    # Autonaming o
+000087a0: 6620 7375 626d 6f64 756c 6573 2e0a 2020  f submodules..  
+000087b0: 2020 2020 6966 2073 656c 662e 6e61 6d65      if self.name
+000087c0: 2069 7320 4e6f 6e65 3a20 2023 2070 7974   is None:  # pyt
+000087d0: 7970 653a 2064 6973 6162 6c65 3d61 7474  ype: disable=att
+000087e0: 7269 6275 7465 2d65 7272 6f72 0a20 2020  ribute-error.   
+000087f0: 2020 2020 2070 7265 6669 7820 3d20 6627       prefix = f'
+00008800: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
+00008810: 5f5f 6e61 6d65 5f5f 7d27 0a20 2020 2020  __name__}'.     
+00008820: 2020 2063 7572 736f 7220 3d20 7365 6c66     cursor = self
+00008830: 2e70 6172 656e 742e 5f73 7461 7465 2e61  .parent._state.a
+00008840: 7574 6f6e 616d 655f 6375 7273 6f72 2e67  utoname_cursor.g
+00008850: 6574 2870 7265 6669 782c 2030 290a 2020  et(prefix, 0).  
+00008860: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
+00008870: 3d20 6627 7b70 7265 6669 787d 5f7b 6375  = f'{prefix}_{cu
+00008880: 7273 6f72 7d27 0a20 2020 2020 2020 2073  rsor}'.        s
+00008890: 656c 662e 7061 7265 6e74 2e5f 7374 6174  elf.parent._stat
+000088a0: 652e 6175 746f 6e61 6d65 5f63 7572 736f  e.autoname_curso
+000088b0: 725b 7072 6566 6978 5d20 3d20 6375 7273  r[prefix] = curs
+000088c0: 6f72 202b 2031 0a20 2020 2020 2023 2041  or + 1.      # A
+000088d0: 6c6c 6f77 2073 636f 7065 2061 6c69 6173  llow scope alias
+000088e0: 696e 6720 756e 6465 7220 7472 616e 7366  ing under transf
+000088f0: 6f72 6d73 2066 6f72 2073 7562 6d6f 6475  orms for submodu
+00008900: 6c65 7320 6465 6669 6e65 6420 696e 2073  les defined in s
+00008910: 6574 7570 2e0a 2020 2020 2020 7265 7573  etup..      reus
+00008920: 655f 7363 6f70 6573 203d 2028 7365 6c66  e_scopes = (self
+00008930: 2e70 6172 656e 742e 5f73 7461 7465 2e69  .parent._state.i
+00008940: 6e5f 7365 7475 7020 616e 640a 2020 2020  n_setup and.    
+00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008960: 2020 7365 6c66 2e70 6172 656e 742e 5f73    self.parent._s
+00008970: 7461 7465 2e73 6574 7570 5f63 616c 6c65  tate.setup_calle
+00008980: 6420 3d3d 2053 6574 7570 5374 6174 652e  d == SetupState.
+00008990: 5452 414e 5346 4f52 4d45 4429 0a20 2020  TRANSFORMED).   
+000089a0: 2020 2023 2050 6572 666f 726d 206e 616d     # Perform nam
+000089b0: 652d 636f 6c6c 6973 696f 6e20 6368 6563  e-collision chec
+000089c0: 6b2e 0a20 2020 2020 2069 6620 7365 6c66  k..      if self
+000089d0: 2e70 6172 656e 742e 5f6e 616d 655f 7461  .parent._name_ta
+000089e0: 6b65 6e28 7365 6c66 2e6e 616d 652c 2073  ken(self.name, s
+000089f0: 656c 662c 2072 6575 7365 5f73 636f 7065  elf, reuse_scope
+00008a00: 733d 7265 7573 655f 7363 6f70 6573 293a  s=reuse_scopes):
+00008a10: 0a20 2020 2020 2020 2070 6172 656e 745f  .        parent_
+00008a20: 636c 6173 7320 3d20 7365 6c66 2e70 6172  class = self.par
+00008a30: 656e 742e 5f5f 636c 6173 735f 5f2e 5f5f  ent.__class__.__
+00008a40: 6e61 6d65 5f5f 0a20 2020 2020 2020 2072  name__.        r
+00008a50: 6169 7365 2065 7272 6f72 732e 4e61 6d65  aise errors.Name
+00008a60: 496e 5573 6545 7272 6f72 2827 7375 626d  InUseError('subm
+00008a70: 6f64 756c 6527 2c20 7365 6c66 2e6e 616d  odule', self.nam
+00008a80: 652c 2070 6172 656e 745f 636c 6173 7329  e, parent_class)
+00008a90: 0a20 2020 2020 2023 2046 696e 616c 697a  .      # Finaliz
+00008aa0: 6520 6174 7461 6368 6d65 6e74 2074 6f20  e attachment to 
+00008ab0: 7061 7265 6e74 2061 6e64 2073 636f 7065  parent and scope
+00008ac0: 2069 6e69 7469 616c 697a 6174 696f 6e2e   initialization.
+00008ad0: 0a20 2020 2020 2073 656c 662e 7061 7265  .      self.pare
+00008ae0: 6e74 2e5f 7374 6174 652e 6368 696c 6472  nt._state.childr
+00008af0: 656e 5b73 656c 662e 6e61 6d65 5d20 3d20  en[self.name] = 
+00008b00: 7365 6c66 0a20 2020 2020 2061 7373 6572  self.      asser
+00008b10: 7420 7365 6c66 2e70 6172 656e 742e 7363  t self.parent.sc
+00008b20: 6f70 6520 6973 206e 6f74 204e 6f6e 650a  ope is not None.
+00008b30: 2020 2020 2020 6f62 6a65 6374 2e5f 5f73        object.__s
+00008b40: 6574 6174 7472 5f5f 280a 2020 2020 2020  etattr__(.      
+00008b50: 2020 2020 7365 6c66 2c20 2773 636f 7065      self, 'scope
+00008b60: 272c 2073 656c 662e 7061 7265 6e74 2e73  ', self.parent.s
+00008b70: 636f 7065 2e70 7573 6828 7365 6c66 2e6e  cope.push(self.n
+00008b80: 616d 652c 2072 6575 7365 3d72 6575 7365  ame, reuse=reuse
+00008b90: 5f73 636f 7065 7329 290a 0a20 2020 2023  _scopes))..    #
+00008ba0: 2054 6f70 2d6c 6576 656c 2069 6e76 6f63   Top-level invoc
+00008bb0: 6174 696f 6e20 7769 7468 2061 2066 756e  ation with a fun
+00008bc0: 6374 696f 6e61 6c20 5363 6f70 652e 0a20  ctional Scope.. 
+00008bd0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00008be0: 6365 2873 656c 662e 7061 7265 6e74 2c20  ce(self.parent, 
+00008bf0: 5363 6f70 6529 3a0a 2020 2020 2020 6f62  Scope):.      ob
+00008c00: 6a65 6374 2e5f 5f73 6574 6174 7472 5f5f  ject.__setattr__
+00008c10: 2873 656c 662c 2027 7363 6f70 6527 2c20  (self, 'scope', 
+00008c20: 7365 6c66 2e70 6172 656e 7429 0a20 2020  self.parent).   
+00008c30: 2065 6c73 653a 0a20 2020 2020 2072 6169   else:.      rai
+00008c40: 7365 2056 616c 7565 4572 726f 7228 2770  se ValueError('p
+00008c50: 6172 656e 7420 6d75 7374 2062 6520 4e6f  arent must be No
+00008c60: 6e65 2c20 4d6f 6475 6c65 206f 7220 5363  ne, Module or Sc
+00008c70: 6f70 6527 290a 0a20 2020 2073 656c 662e  ope')..    self.
+00008c80: 5f73 7461 7465 2e69 735f 696e 6974 6961  _state.is_initia
+00008c90: 6c69 7a65 6420 3d20 5472 7565 0a0a 2020  lized = True..  
+00008ca0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+00008cb0: 6629 202d 3e20 7374 723a 0a20 2020 2072  f) -> str:.    r
+00008cc0: 6574 7572 6e20 5f6d 6f64 756c 655f 7265  eturn _module_re
+00008cd0: 7072 2873 656c 6629 0a0a 2020 6465 6620  pr(self)..  def 
+00008ce0: 7365 7475 7028 7365 6c66 2920 2d3e 204e  setup(self) -> N
+00008cf0: 6f6e 653a 0a20 2020 2022 2222 496e 6974  one:.    """Init
+00008d00: 6961 6c69 7a65 7320 6120 4d6f 6475 6c65  ializes a Module
+00008d10: 206c 617a 696c 7920 2873 696d 696c 6172   lazily (similar
+00008d20: 2074 6f20 6120 6c61 7a79 2060 605f 5f69   to a lazy ``__i
+00008d30: 6e69 745f 5f60 6029 2e0a 0a20 2020 2060  nit__``)...    `
+00008d40: 6073 6574 7570 6060 2069 7320 6361 6c6c  `setup`` is call
+00008d50: 6564 206f 6e63 6520 6c61 7a69 6c79 206f  ed once lazily o
+00008d60: 6e20 6120 6d6f 6475 6c65 2069 6e73 7461  n a module insta
+00008d70: 6e63 6520 7768 656e 2061 206d 6f64 756c  nce when a modul
+00008d80: 650a 2020 2020 6973 2062 6f75 6e64 2c20  e.    is bound, 
+00008d90: 696d 6d65 6469 6174 656c 7920 6265 666f  immediately befo
+00008da0: 7265 2061 6e79 206f 7468 6572 206d 6574  re any other met
+00008db0: 686f 6473 206c 696b 6520 6060 5f5f 6361  hods like ``__ca
+00008dc0: 6c6c 5f5f 6060 2061 7265 0a20 2020 2069  ll__`` are.    i
+00008dd0: 6e76 6f6b 6564 2c20 6f72 2062 6566 6f72  nvoked, or befor
+00008de0: 6520 6120 6060 7365 7475 7060 602d 6465  e a ``setup``-de
+00008df0: 6669 6e65 6420 6174 7472 6962 7574 6520  fined attribute 
+00008e00: 6f6e 2060 7365 6c66 6020 6973 2061 6363  on `self` is acc
+00008e10: 6573 7365 642e 0a0a 2020 2020 5468 6973  essed...    This
+00008e20: 2063 616e 2068 6170 7065 6e20 696e 2074   can happen in t
+00008e30: 6872 6565 2063 6173 6573 3a0a 0a20 2020  hree cases:..   
+00008e40: 2020 2031 2e20 496d 6d65 6469 6174 656c     1. Immediatel
+00008e50: 7920 7768 656e 2069 6e76 6f6b 696e 6720  y when invoking 
+00008e60: 3a6d 6574 683a 6061 7070 6c79 602c 203a  :meth:`apply`, :
+00008e70: 6d65 7468 3a60 696e 6974 6020 6f72 0a20  meth:`init` or. 
+00008e80: 2020 2020 2020 2020 3a6d 6574 683a 6069          :meth:`i
+00008e90: 6e69 745f 616e 645f 6f75 7470 7574 602e  nit_and_output`.
+00008ea0: 0a0a 2020 2020 2020 322e 204f 6e63 6520  ..      2. Once 
+00008eb0: 7468 6520 6d6f 6475 6c65 2069 7320 6769  the module is gi
+00008ec0: 7665 6e20 6120 6e61 6d65 2062 7920 6265  ven a name by be
+00008ed0: 696e 6720 6173 7369 676e 6564 2074 6f20  ing assigned to 
+00008ee0: 616e 2061 7474 7269 6275 7465 206f 660a  an attribute of.
+00008ef0: 2020 2020 2020 2020 2061 6e6f 7468 6572           another
+00008f00: 206d 6f64 756c 6520 696e 7369 6465 2074   module inside t
+00008f10: 6865 206f 7468 6572 206d 6f64 756c 6527  he other module'
+00008f20: 7320 6060 7365 7475 7060 6020 6d65 7468  s ``setup`` meth
+00008f30: 6f64 0a20 2020 2020 2020 2020 2873 6565  od.         (see
+00008f40: 203a 6d65 7468 3a60 5f5f 7365 7461 7474   :meth:`__setatt
+00008f50: 725f 5f60 293a 3a0a 0a20 2020 2020 2020  r__`)::..       
+00008f60: 2020 2020 636c 6173 7320 4d79 4d6f 6475      class MyModu
+00008f70: 6c65 286e 6e2e 4d6f 6475 6c65 293a 0a20  le(nn.Module):. 
+00008f80: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00008f90: 7365 7475 7028 7365 6c66 293a 0a20 2020  setup(self):.   
+00008fa0: 2020 2020 2020 2020 2020 2020 7375 626d              subm
+00008fb0: 6f64 756c 6520 3d20 436f 6e76 282e 2e2e  odule = Conv(...
+00008fc0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008fd0: 2020 2320 4163 6365 7373 696e 6720 6073    # Accessing `s
+00008fe0: 7562 6d6f 6475 6c65 6020 6174 7472 6962  ubmodule` attrib
+00008ff0: 7574 6573 2064 6f65 7320 6e6f 7420 7965  utes does not ye
+00009000: 7420 776f 726b 2068 6572 652e 0a0a 2020  t work here...  
+00009010: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+00009020: 6865 2066 6f6c 6c6f 7769 6e67 206c 696e  he following lin
+00009030: 6520 696e 766f 6b65 7320 6073 656c 662e  e invokes `self.
+00009040: 5f5f 7365 7461 7474 725f 5f60 2c20 7768  __setattr__`, wh
+00009050: 6963 6820 6769 7665 730a 2020 2020 2020  ich gives.      
+00009060: 2020 2020 2020 2020 2023 2060 7375 626d           # `subm
+00009070: 6f64 756c 6560 2074 6865 206e 616d 6520  odule` the name 
+00009080: 2263 6f6e 7631 222e 0a20 2020 2020 2020  "conv1"..       
+00009090: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000090a0: 7631 203d 2073 7562 6d6f 6475 6c65 0a0a  v1 = submodule..
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000090c0: 2041 6363 6573 7369 6e67 2060 7375 626d   Accessing `subm
+000090d0: 6f64 756c 6560 2061 7474 7269 6275 7465  odule` attribute
+000090e0: 7320 6f72 206d 6574 686f 6473 2069 7320  s or methods is 
+000090f0: 6e6f 7720 7361 6665 2061 6e64 0a20 2020  now safe and.   
+00009100: 2020 2020 2020 2020 2020 2020 2320 6569              # ei
+00009110: 7468 6572 2063 6175 7365 7320 7365 7475  ther causes setu
+00009120: 7028 2920 746f 2062 6520 6361 6c6c 6564  p() to be called
+00009130: 206f 6e63 652e 0a0a 2020 2020 2020 332e   once...      3.
+00009140: 204f 6e63 6520 6120 6d6f 6475 6c65 2069   Once a module i
+00009150: 7320 636f 6e73 7472 7563 7465 6420 696e  s constructed in
+00009160: 7369 6465 2061 206d 6574 686f 6420 7772  side a method wr
+00009170: 6170 7065 6420 7769 7468 0a20 2020 2020  apped with.     
+00009180: 2020 2020 3a6d 6574 683a 6063 6f6d 7061      :meth:`compa
+00009190: 6374 602c 2069 6d6d 6564 6961 7465 6c79  ct`, immediately
+000091a0: 2062 6566 6f72 6520 616e 6f74 6865 7220   before another 
+000091b0: 6d65 7468 6f64 2069 7320 6361 6c6c 6564  method is called
+000091c0: 206f 720a 2020 2020 2020 2020 2060 6073   or.         ``s
+000091d0: 6574 7570 6060 2064 6566 696e 6564 2061  etup`` defined a
+000091e0: 7474 7269 6275 7465 2069 7320 6163 6365  ttribute is acce
+000091f0: 7373 6564 2e0a 2020 2020 2222 220a 2020  ssed..    """.  
+00009200: 2020 7061 7373 0a0a 2020 6465 6620 5f72    pass..  def _r
+00009210: 6567 6973 7465 725f 7375 626d 6f64 756c  egister_submodul
+00009220: 6573 2873 656c 662c 206e 616d 652c 2076  es(self, name, v
+00009230: 616c 293a 0a20 2020 2022 2222 5265 6769  al):.    """Regi
+00009240: 7374 6572 7320 6120 7375 626d 6f64 756c  sters a submodul
+00009250: 652e 2222 220a 2020 2020 6173 7365 7274  e.""".    assert
+00009260: 2073 656c 662e 7363 6f70 652c 2027 5472   self.scope, 'Tr
+00009270: 7969 6e67 2074 6f20 7265 6769 7374 6572  ying to register
+00009280: 2073 7562 6d6f 6475 6c65 7320 6f6e 2075   submodules on u
+00009290: 6e62 6f75 6e64 2073 636f 7065 2e27 0a20  nbound scope.'. 
+000092a0: 2020 2072 6f6f 7420 3d20 7365 6c66 2e73     root = self.s
+000092b0: 636f 7065 2e72 6f6f 740a 2020 2020 6361  cope.root.    ca
+000092c0: 6368 6520 3d20 5f63 6163 6865 732e 6765  che = _caches.ge
+000092d0: 7428 726f 6f74 2c20 7765 616b 7265 662e  t(root, weakref.
+000092e0: 5765 616b 5661 6c75 6544 6963 7469 6f6e  WeakValueDiction
+000092f0: 6172 7928 2929 0a20 2020 205f 6361 6368  ary()).    _cach
+00009300: 6573 5b72 6f6f 745d 203d 2063 6163 6865  es[root] = cache
+00009310: 0a20 2020 2071 7565 7565 203d 205b 5d0a  .    queue = [].
+00009320: 2020 2020 7072 6573 6572 7665 5f61 646f      preserve_ado
+00009330: 7074 6564 5f6e 616d 6573 203d 2063 6f6e  pted_names = con
+00009340: 6669 672e 666c 6178 5f70 7265 7365 7276  fig.flax_preserv
+00009350: 655f 6164 6f70 7465 645f 6e61 6d65 730a  e_adopted_names.
+00009360: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
+00009370: 656c 662c 2027 7072 6573 6572 7665 5f61  elf, 'preserve_a
+00009380: 646f 7074 6564 5f6e 616d 6573 2729 3a0a  dopted_names'):.
+00009390: 2020 2020 2020 7072 6573 6572 7665 5f61        preserve_a
+000093a0: 646f 7074 6564 5f6e 616d 6573 203d 2073  dopted_names = s
+000093b0: 656c 662e 7072 6573 6572 7665 5f61 646f  elf.preserve_ado
+000093c0: 7074 6564 5f6e 616d 6573 0a20 2020 2064  pted_names.    d
+000093d0: 6566 2061 646f 7074 5f61 7474 725f 6d6f  ef adopt_attr_mo
+000093e0: 6475 6c65 7328 6361 6368 652c 2071 7565  dules(cache, que
+000093f0: 7565 2c20 7375 6666 6978 2c20 7375 6276  ue, suffix, subv
+00009400: 616c 7565 293a 0a20 2020 2020 2069 6620  alue):.      if 
+00009410: 6973 696e 7374 616e 6365 2873 7562 7661  isinstance(subva
+00009420: 6c75 652c 204d 6f64 756c 6529 3a0a 2020  lue, Module):.  
+00009430: 2020 2020 2020 6164 6f70 7465 645f 6e61        adopted_na
+00009440: 6d65 203d 204e 6f6e 650a 2020 2020 2020  me = None.      
+00009450: 2020 6966 2073 7562 7661 6c75 652e 7061    if subvalue.pa
+00009460: 7265 6e74 2069 7320 4e6f 6e65 3a0a 2020  rent is None:.  
+00009470: 2020 2020 2020 2020 2320 5072 6573 6572          # Preser
+00009480: 7665 2073 6861 7269 6e67 2d62 792d 7265  ve sharing-by-re
+00009490: 6665 7265 6e63 6520 7265 6c61 7469 6f6e  ference relation
+000094a0: 7368 6970 7320 6475 7269 6e67 2061 646f  ships during ado
+000094b0: 7074 696f 6e0a 2020 2020 2020 2020 2020  ption.          
+000094c0: 2320 7669 6120 6361 6368 6520 6b65 7965  # via cache keye
+000094d0: 6420 6f6e 2075 6e69 7175 6520 696e 7374  d on unique inst
+000094e0: 616e 6365 2069 6473 2e0a 2020 2020 2020  ance ids..      
+000094f0: 2020 2020 6b65 7920 3d20 7375 6276 616c      key = subval
+00009500: 7565 2e5f 6964 0a20 2020 2020 2020 2020  ue._id.         
+00009510: 2023 204d 6f64 756c 6520 7761 7320 7061   # Module was pa
+00009520: 7373 6564 2066 726f 6d20 6f75 7473 6964  ssed from outsid
+00009530: 652e 2049 7420 6e65 6564 7320 746f 2062  e. It needs to b
+00009540: 6520 636c 6f6e 6564 2e0a 2020 2020 2020  e cloned..      
+00009550: 2020 2020 2320 4f75 7473 6964 6520 6d6f      # Outside mo
+00009560: 6475 6c65 7320 6172 6520 6e61 6d65 6420  dules are named 
+00009570: 6279 2061 7474 6163 686d 656e 742c 206e  by attachment, n
+00009580: 6f74 2061 6e20 6f75 7465 7220 6e61 6d65  ot an outer name
+00009590: 2c0a 2020 2020 2020 2020 2020 2320 554e  ,.          # UN
+000095a0: 4c45 5353 2077 6527 7265 2075 7369 6e67  LESS we're using
+000095b0: 206e 6577 2061 646f 7074 6564 206e 616d   new adopted nam
+000095c0: 6520 706f 6c69 6379 2c20 696e 2077 6869  e policy, in whi
+000095d0: 6368 2063 6173 6520 616e 2065 7869 7374  ch case an exist
+000095e0: 696e 670a 2020 2020 2020 2020 2020 2320  ing.          # 
+000095f0: 6e61 6d65 2077 696c 6c20 6265 2075 7365  name will be use
+00009600: 642c 2061 7320 6973 206f 6674 656e 2073  d, as is often s
+00009610: 7570 706c 6965 6420 6279 2063 6f6e 6669  upplied by confi
+00009620: 6720 7379 7374 656d 732e 0a20 2020 2020  g systems..     
+00009630: 2020 2020 2069 6620 7072 6573 6572 7665       if preserve
+00009640: 5f61 646f 7074 6564 5f6e 616d 6573 3a0a  _adopted_names:.
+00009650: 2020 2020 2020 2020 2020 2020 6164 6f70              adop
+00009660: 7465 645f 6e61 6d65 203d 206f 626a 6563  ted_name = objec
+00009670: 742e 5f5f 6765 7461 7474 7269 6275 7465  t.__getattribute
+00009680: 5f5f 2873 7562 7661 6c75 652c 2027 6e61  __(subvalue, 'na
+00009690: 6d65 2729 0a20 2020 2020 2020 2020 2069  me').          i
+000096a0: 6620 6b65 7920 696e 2063 6163 6865 3a0a  f key in cache:.
+000096b0: 2020 2020 2020 2020 2020 2020 7375 6276              subv
+000096c0: 616c 7565 203d 2063 6163 6865 5b6b 6579  alue = cache[key
+000096d0: 5d0a 2020 2020 2020 2020 2020 656c 7365  ].          else
+000096e0: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
+000096f0: 6276 616c 7565 203d 2073 7562 7661 6c75  bvalue = subvalu
+00009700: 652e 636c 6f6e 6528 6e61 6d65 3d4e 6f6e  e.clone(name=Non
+00009710: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
+00009720: 6163 6865 5b6b 6579 5d20 3d20 7375 6276  ache[key] = subv
+00009730: 616c 7565 0a20 2020 2020 2020 2069 6620  alue.        if 
+00009740: 7375 6276 616c 7565 2e6e 616d 6520 6973  subvalue.name is
+00009750: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00009760: 206f 626a 6563 742e 5f5f 7365 7461 7474   object.__setatt
+00009770: 725f 5f28 7375 6276 616c 7565 2c20 2770  r__(subvalue, 'p
+00009780: 6172 656e 7427 2c20 7365 6c66 290a 2020  arent', self).  
+00009790: 2020 2020 2020 2020 6966 2061 646f 7074          if adopt
+000097a0: 6564 5f6e 616d 6520 6973 204e 6f6e 653a  ed_name is None:
+000097b0: 0a20 2020 2020 2020 2020 2020 2061 646f  .            ado
+000097c0: 7074 6564 5f6e 616d 6520 3d20 6627 7b6e  pted_name = f'{n
+000097d0: 616d 657d 7b73 7566 6669 787d 270a 2020  ame}{suffix}'.  
+000097e0: 2020 2020 2020 2020 6f62 6a65 6374 2e5f          object._
+000097f0: 5f73 6574 6174 7472 5f5f 2873 7562 7661  _setattr__(subva
+00009800: 6c75 652c 2027 6e61 6d65 272c 2061 646f  lue, 'name', ado
+00009810: 7074 6564 5f6e 616d 6529 0a20 2020 2020  pted_name).     
+00009820: 2020 2020 2071 7565 7565 2e61 7070 656e       queue.appen
+00009830: 6428 7375 6276 616c 7565 290a 2020 2020  d(subvalue).    
+00009840: 2020 7265 7475 726e 2073 7562 7661 6c75    return subvalu
+00009850: 650a 2020 2020 7661 6c20 3d20 5f66 7265  e.    val = _fre
+00009860: 657a 655f 6174 7472 285f 6d61 705f 6f76  eze_attr(_map_ov
+00009870: 6572 5f6d 6f64 756c 6573 5f69 6e5f 7472  er_modules_in_tr
+00009880: 6565 280a 2020 2020 2020 2020 6675 6e63  ee(.        func
+00009890: 746f 6f6c 732e 7061 7274 6961 6c28 6164  tools.partial(ad
+000098a0: 6f70 745f 6174 7472 5f6d 6f64 756c 6573  opt_attr_modules
+000098b0: 2c20 6361 6368 652c 2071 7565 7565 292c  , cache, queue),
+000098c0: 2076 616c 2929 0a20 2020 206f 626a 6563   val)).    objec
+000098d0: 742e 5f5f 7365 7461 7474 725f 5f28 7365  t.__setattr__(se
+000098e0: 6c66 2c20 6e61 6d65 2c20 7661 6c29 0a20  lf, name, val). 
+000098f0: 2020 2066 6f72 2078 2069 6e20 7175 6575     for x in queu
+00009900: 653a 0a20 2020 2020 2078 2e5f 5f70 6f73  e:.      x.__pos
+00009910: 745f 696e 6974 5f5f 2829 0a0a 2020 6465  t_init__()..  de
+00009920: 6620 5f74 7279 5f73 6574 7570 2873 656c  f _try_setup(sel
+00009930: 662c 2073 6861 6c6c 6f77 3a20 626f 6f6c  f, shallow: bool
+00009940: 203d 2046 616c 7365 2920 2d3e 204e 6f6e   = False) -> Non
+00009950: 653a 0a20 2020 2022 2222 5472 6965 7320  e:.    """Tries 
+00009960: 746f 2073 6574 7570 206d 6f64 756c 6520  to setup module 
+00009970: 6966 2073 636f 7065 2069 7320 6176 6169  if scope is avai
+00009980: 6c61 626c 6520 616e 6420 7365 7475 7020  lable and setup 
+00009990: 6861 7320 6e6f 7420 6265 656e 2063 616c  has not been cal
+000099a0: 6c65 6420 7965 742e 2222 220a 2020 2020  led yet.""".    
+000099b0: 6966 2028 7365 6c66 2e73 636f 7065 0a20  if (self.scope. 
+000099c0: 2020 2020 2020 2061 6e64 206e 6f74 2073         and not s
+000099d0: 656c 662e 5f73 7461 7465 2e69 6e5f 7365  elf._state.in_se
+000099e0: 7475 700a 2020 2020 2020 2020 616e 6420  tup.        and 
+000099f0: 7365 6c66 2e5f 7374 6174 652e 7365 7475  self._state.setu
+00009a00: 705f 6361 6c6c 6564 2021 3d20 5365 7475  p_called != Setu
+00009a10: 7053 7461 7465 2e44 4f4e 4529 3a0a 2020  pState.DONE):.  
+00009a20: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00009a30: 2073 656c 662e 5f73 7461 7465 2e69 6e5f   self._state.in_
+00009a40: 7365 7475 7020 3d20 5472 7565 0a20 2020  setup = True.   
+00009a50: 2020 2020 2023 2041 2073 6861 6c6c 6f77       # A shallow
+00009a60: 2073 6574 7570 2077 696c 6c20 6f6e 6c79   setup will only
+00009a70: 2072 6567 6973 7465 7220 6174 7472 6962   register attrib
+00009a80: 7574 6520 7375 626d 6f64 756c 6573 2062  ute submodules b
+00009a90: 7574 2069 7420 646f 6573 0a20 2020 2020  ut it does.     
+00009aa0: 2020 2023 206e 6f74 2063 616c 6c20 7468     # not call th
+00009ab0: 6520 7573 6572 2773 2073 6574 7570 2e20  e user's setup. 
+00009ac0: 5468 6973 2061 766f 6964 7320 7275 6e6e  This avoids runn
+00009ad0: 696e 6720 6265 666f 7265 2061 0a20 2020  ing before a.   
+00009ae0: 2020 2020 2023 2074 7261 6e73 666f 726d       # transform
+00009af0: 6174 696f 6e2e 0a20 2020 2020 2020 2066  ation..        f
+00009b00: 6f72 2066 6965 6c64 2069 6e20 6461 7461  or field in data
+00009b10: 636c 6173 7365 732e 6669 656c 6473 2873  classes.fields(s
+00009b20: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+00009b30: 6966 2066 6965 6c64 2e6e 616d 6520 213d  if field.name !=
+00009b40: 2027 7061 7265 6e74 2720 616e 6420 6669   'parent' and fi
+00009b50: 656c 642e 696e 6974 3a0a 2020 2020 2020  eld.init:.      
+00009b60: 2020 2020 2020 7365 6c66 2e5f 7265 6769        self._regi
+00009b70: 7374 6572 5f73 7562 6d6f 6475 6c65 7328  ster_submodules(
+00009b80: 6669 656c 642e 6e61 6d65 2c20 6765 7461  field.name, geta
+00009b90: 7474 7228 7365 6c66 2c20 6669 656c 642e  ttr(self, field.
+00009ba0: 6e61 6d65 2929 0a20 2020 2020 2020 2069  name)).        i
+00009bb0: 6620 6e6f 7420 7368 616c 6c6f 773a 0a20  f not shallow:. 
+00009bc0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00009bd0: 7475 7028 290a 2020 2020 2020 2020 2320  tup().        # 
+00009be0: 5765 2072 756e 2073 7461 7469 6320 6368  We run static ch
+00009bf0: 6563 6b73 2061 6273 7472 6163 746c 7920  ecks abstractly 
+00009c00: 6f6e 6365 2066 6f72 2073 6574 7570 2062  once for setup b
+00009c10: 6566 6f72 6520 616e 7920 7472 616e 7366  efore any transf
+00009c20: 6f72 6d73 0a20 2020 2020 2020 2023 2074  orms.        # t
+00009c30: 6f20 6465 7465 6374 206e 616d 6520 636f  o detect name co
+00009c40: 6c6c 6973 696f 6e73 2061 6e64 206f 7468  llisions and oth
+00009c50: 6572 2070 7974 686f 6e20 6572 726f 7273  er python errors
+00009c60: 2e0a 2020 2020 2020 2020 656c 6966 2073  ..        elif s
+00009c70: 656c 662e 5f73 7461 7465 2e73 6574 7570  elf._state.setup
+00009c80: 5f63 616c 6c65 6420 3d3d 2053 6574 7570  _called == Setup
+00009c90: 5374 6174 652e 4e45 573a 0a20 2020 2020  State.NEW:.     
+00009ca0: 2020 2020 2073 656c 662e 5f76 616c 6964       self._valid
+00009cb0: 6174 655f 7365 7475 7028 290a 2020 2020  ate_setup().    
+00009cc0: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
+00009cd0: 2020 2073 656c 662e 5f73 7461 7465 2e69     self._state.i
+00009ce0: 6e5f 7365 7475 7020 3d20 4661 6c73 650a  n_setup = False.
+00009cf0: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
+00009d00: 6174 652e 7365 7475 705f 6361 6c6c 6564  ate.setup_called
+00009d10: 203d 2053 6574 7570 5374 6174 652e 444f   = SetupState.DO
+00009d20: 4e45 0a0a 2020 6465 6620 5f76 616c 6964  NE..  def _valid
+00009d30: 6174 655f 7365 7475 7028 7365 6c66 2920  ate_setup(self) 
+00009d40: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00009d50: 4162 7374 7261 6374 6c79 2065 7661 6c75  Abstractly evalu
+00009d60: 6174 6573 2073 6574 7570 206f 6e6c 7920  ates setup only 
+00009d70: 746f 2072 756e 2073 7461 7469 6320 6368  to run static ch
+00009d80: 6563 6b73 2e22 2222 0a20 2020 2064 6566  ecks.""".    def
+00009d90: 2072 756e 5f73 6574 7570 5f6f 6e6c 7928   run_setup_only(
+00009da0: 7829 3a0a 2020 2020 2020 7772 6170 7065  x):.      wrappe
+00009db0: 645f 6964 203d 2077 7261 705f 6d65 7468  d_id = wrap_meth
+00009dc0: 6f64 5f6f 6e63 6528 6c61 6d62 6461 206d  od_once(lambda m
+00009dd0: 2c20 783a 2078 290a 2020 2020 2020 7769  , x: x).      wi
+00009de0: 7468 2054 6573 7453 636f 7065 287b 7d2c  th TestScope({},
+00009df0: 2072 6e67 733d 7b7d 2c20 6d75 7461 626c   rngs={}, mutabl
+00009e00: 653d 5472 7565 292e 7465 6d70 6f72 6172  e=True).temporar
+00009e10: 7928 2920 6173 2072 6f6f 743a 0a20 2020  y() as root:.   
+00009e20: 2020 2020 2072 6574 7572 6e20 7772 6170       return wrap
+00009e30: 7065 645f 6964 2873 656c 662e 636c 6f6e  ped_id(self.clon
+00009e40: 6528 7061 7265 6e74 3d72 6f6f 7429 2c20  e(parent=root), 
+00009e50: 7829 0a20 2020 205f 203d 206a 6178 2e65  x).    _ = jax.e
+00009e60: 7661 6c5f 7368 6170 6528 7275 6e5f 7365  val_shape(run_se
+00009e70: 7475 705f 6f6e 6c79 2c20 3029 0a0a 2020  tup_only, 0)..  
+00009e80: 6465 6620 5f6e 616d 655f 7461 6b65 6e28  def _name_taken(
+00009e90: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00009ea0: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
+00009eb0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00009ec0: 2020 2020 206d 6f64 756c 653a 204f 7074       module: Opt
+00009ed0: 696f 6e61 6c5b 274d 6f64 756c 6527 5d20  ional['Module'] 
+00009ee0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00009ef0: 2020 2020 2020 2020 2020 7265 7573 655f            reuse_
+00009f00: 7363 6f70 6573 3a20 626f 6f6c 203d 2046  scopes: bool = F
+00009f10: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00009f20: 2020 2020 2020 2020 636f 6c6c 6563 7469          collecti
+00009f30: 6f6e 3a20 4f70 7469 6f6e 616c 5b73 7472  on: Optional[str
+00009f40: 5d20 3d20 4e6f 6e65 2920 2d3e 2062 6f6f  ] = None) -> boo
+00009f50: 6c3a 0a20 2020 2061 7373 6572 7420 7365  l:.    assert se
+00009f60: 6c66 2e73 636f 7065 2069 7320 6e6f 7420  lf.scope is not 
+00009f70: 4e6f 6e65 0a20 2020 2023 2077 6974 6820  None.    # with 
+00009f80: 7265 6c61 7865 6420 6e61 6d69 6e67 2064  relaxed naming d
+00009f90: 6f6e 2774 2066 6f72 6365 206e 6f6e 2d6f  on't force non-o
+00009fa0: 7665 726c 6170 2077 6974 6820 7079 7468  verlap with pyth
+00009fb0: 6f6e 2061 7474 7269 6275 7465 206e 616d  on attribute nam
+00009fc0: 6573 2e0a 2020 2020 6966 2063 6f6e 6669  es..    if confi
+00009fd0: 672e 666c 6178 5f72 656c 6178 6564 5f6e  g.flax_relaxed_n
+00009fe0: 616d 696e 673a 0a20 2020 2020 2069 6620  aming:.      if 
+00009ff0: 7265 7573 655f 7363 6f70 6573 3a0a 2020  reuse_scopes:.  
+0000a000: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000a010: 7365 0a20 2020 2020 2072 6574 7572 6e20  se.      return 
+0000a020: 7365 6c66 2e73 636f 7065 2e6e 616d 655f  self.scope.name_
+0000a030: 7265 7365 7276 6564 286e 616d 652c 2063  reserved(name, c
+0000a040: 6f6c 6c65 6374 696f 6e29 0a20 2020 2069  ollection).    i
+0000a050: 6620 6e61 6d65 2069 6e20 5f61 6c6c 5f6e  f name in _all_n
+0000a060: 616d 6573 5f6f 6e5f 6f62 6a65 6374 2873  ames_on_object(s
+0000a070: 656c 6629 3a0a 2020 2020 2020 7661 6c20  elf):.      val 
+0000a080: 3d20 6765 7461 7474 7228 7365 6c66 2c20  = getattr(self, 
+0000a090: 6e61 6d65 2c20 4e6f 6e65 290a 2020 2020  name, None).    
+0000a0a0: 2020 6966 206d 6f64 756c 6520 6973 206e    if module is n
+0000a0b0: 6f74 204e 6f6e 6520 616e 6420 7661 6c20  ot None and val 
+0000a0c0: 6973 206d 6f64 756c 653a 0a20 2020 2020  is module:.     
+0000a0d0: 2020 2023 206e 616d 6520 6973 2074 616b     # name is tak
+0000a0e0: 656e 2062 7920 7468 6520 7661 6c75 6520  en by the value 
+0000a0f0: 6974 7365 6c66 2062 6563 6175 7365 0a20  itself because. 
+0000a100: 2020 2020 2020 2023 2066 6965 6c64 2061         # field a
+0000a110: 7373 6967 6e6d 656e 7420 6861 7070 656e  ssignment happen
+0000a120: 6564 2062 6566 6f72 6520 6e61 6d69 6e67  ed before naming
+0000a130: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000a140: 4661 6c73 650a 2020 2020 2020 7265 7475  False.      retu
+0000a150: 726e 2054 7275 650a 2020 2020 2320 4368  rn True.    # Ch
+0000a160: 6563 6b20 666f 7220 7468 6520 6578 6973  eck for the exis
+0000a170: 7465 6e63 6520 6f66 206e 616d 6520 696e  tence of name in
+0000a180: 2074 6865 2073 636f 7065 206f 626a 6563   the scope objec
+0000a190: 742e 0a20 2020 2069 6620 7265 7573 655f  t..    if reuse_
+0000a1a0: 7363 6f70 6573 3a0a 2020 2020 2020 7265  scopes:.      re
+0000a1b0: 7475 726e 2046 616c 7365 0a20 2020 2072  turn False.    r
+0000a1c0: 6574 7572 6e20 6e61 6d65 2069 6e20 7365  eturn name in se
+0000a1d0: 6c66 2e73 636f 7065 2e72 6573 6572 7661  lf.scope.reserva
+0000a1e0: 7469 6f6e 730a 0a20 2040 7072 6f70 6572  tions..  @proper
+0000a1f0: 7479 0a20 2064 6566 205f 696e 6974 6961  ty.  def _initia
+0000a200: 6c69 7a61 7469 6f6e 5f61 6c6c 6f77 6564  lization_allowed
+0000a210: 2873 656c 6629 3a0a 2020 2020 7265 7475  (self):.    retu
+0000a220: 726e 2073 656c 662e 5f73 7461 7465 2e69  rn self._state.i
+0000a230: 6e5f 7365 7475 7020 6f72 2073 656c 662e  n_setup or self.
+0000a240: 5f73 7461 7465 2e69 6e5f 636f 6d70 6163  _state.in_compac
+0000a250: 745f 6d65 7468 6f64 0a0a 2020 6465 6620  t_method..  def 
+0000a260: 636c 6f6e 6528 7365 6c66 3a20 4d2c 202a  clone(self: M, *
+0000a270: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+0000a280: 7265 6e74 3a20 4f70 7469 6f6e 616c 5b55  rent: Optional[U
+0000a290: 6e69 6f6e 5b53 636f 7065 2c20 274d 6f64  nion[Scope, 'Mod
+0000a2a0: 756c 6527 5d5d 203d 204e 6f6e 652c 0a20  ule']] = None,. 
+0000a2b0: 2020 2020 2020 2020 2020 202a 2a75 7064             **upd
+0000a2c0: 6174 6573 2920 2d3e 204d 3a0a 2020 2020  ates) -> M:.    
+0000a2d0: 2222 2243 7265 6174 6573 2061 2063 6c6f  """Creates a clo
+0000a2e0: 6e65 206f 6620 7468 6973 204d 6f64 756c  ne of this Modul
+0000a2f0: 652c 2077 6974 6820 6f70 7469 6f6e 616c  e, with optional
+0000a300: 6c79 2075 7064 6174 6564 2061 7267 756d  ly updated argum
+0000a310: 656e 7473 2e0a 0a20 2020 2041 7267 733a  ents...    Args:
+0000a320: 0a20 2020 2020 2070 6172 656e 743a 2054  .      parent: T
+0000a330: 6865 2070 6172 656e 7420 6f66 2074 6865  he parent of the
+0000a340: 2063 6c6f 6e65 2e20 5468 6520 636c 6f6e   clone. The clon
+0000a350: 6520 7769 6c6c 2068 6176 6520 6e6f 2070  e will have no p
+0000a360: 6172 656e 7420 6966 206e 6f0a 2020 2020  arent if no.    
+0000a370: 2020 2020 6578 706c 6963 6974 2070 6172      explicit par
+0000a380: 656e 7420 6973 2073 7065 6369 6669 6564  ent is specified
+0000a390: 2e0a 2020 2020 2020 2a2a 7570 6461 7465  ..      **update
+0000a3a0: 733a 2041 7474 7269 6275 7465 2075 7064  s: Attribute upd
+0000a3b0: 6174 6573 2e0a 2020 2020 5265 7475 726e  ates..    Return
+0000a3c0: 733a 0a20 2020 2020 2041 2063 6c6f 6e65  s:.      A clone
+0000a3d0: 206f 6620 7468 6520 7468 6973 204d 6f64   of the this Mod
+0000a3e0: 756c 6520 7769 7468 2074 6865 2075 7064  ule with the upd
+0000a3f0: 6174 6564 2061 7474 7269 6275 7465 7320  ated attributes 
+0000a400: 616e 6420 7061 7265 6e74 2e0a 2020 2020  and parent..    
+0000a410: 2222 220a 2020 2020 6174 7472 7320 3d20  """.    attrs = 
+0000a420: 7b66 2e6e 616d 653a 2067 6574 6174 7472  {f.name: getattr
+0000a430: 2873 656c 662c 2066 2e6e 616d 6529 2066  (self, f.name) f
+0000a440: 6f72 2066 2069 6e20 6461 7461 636c 6173  or f in dataclas
+0000a450: 7365 732e 6669 656c 6473 2873 656c 6629  ses.fields(self)
+0000a460: 2069 6620 662e 696e 6974 7d0a 2020 2020   if f.init}.    
+0000a470: 6174 7472 732e 7570 6461 7465 2870 6172  attrs.update(par
+0000a480: 656e 743d 7061 7265 6e74 2c20 2a2a 7570  ent=parent, **up
+0000a490: 6461 7465 7329 0a20 2020 2072 6574 7572  dates).    retur
+0000a4a0: 6e20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  n self.__class__
+0000a4b0: 282a 2a61 7474 7273 290a 0a20 2064 6566  (**attrs)..  def
+0000a4c0: 2076 6172 6961 626c 6528 7365 6c66 2c20   variable(self, 
+0000a4d0: 636f 6c3a 2073 7472 2c20 6e61 6d65 3a20  col: str, name: 
+0000a4e0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0000a4f0: 2020 2020 696e 6974 5f66 6e3a 204f 7074      init_fn: Opt
+0000a500: 696f 6e61 6c5b 4361 6c6c 6162 6c65 5b2e  ional[Callable[.
+0000a510: 2e2e 2c20 416e 795d 5d20 3d20 4e6f 6e65  .., Any]] = None
+0000a520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a530: 202a 696e 6974 5f61 7267 732c 0a20 2020   *init_args,.   
+0000a540: 2020 2020 2020 2020 2020 2020 756e 626f              unbo
+0000a550: 783a 2062 6f6f 6c20 3d20 5472 7565 2920  x: bool = True) 
+0000a560: 2d3e 2056 6172 6961 626c 653a 0a20 2020  -> Variable:.   
+0000a570: 2022 2222 4465 636c 6172 6573 2061 6e64   """Declares and
+0000a580: 2072 6574 7572 6e73 2061 2076 6172 6961   returns a varia
+0000a590: 626c 6520 696e 2074 6869 7320 4d6f 6475  ble in this Modu
+0000a5a0: 6c65 2e0a 0a20 2020 2053 6565 203a 6d6f  le...    See :mo
+0000a5b0: 643a 6066 6c61 782e 636f 7265 2e76 6172  d:`flax.core.var
+0000a5c0: 6961 626c 6573 6020 666f 7220 6d6f 7265  iables` for more
+0000a5d0: 2069 6e66 6f72 6d61 7469 6f6e 2e20 5365   information. Se
+0000a5e0: 6520 616c 736f 203a 6d65 7468 3a60 7061  e also :meth:`pa
+0000a5f0: 7261 6d60 0a20 2020 2066 6f72 2061 2073  ram`.    for a s
+0000a600: 686f 7274 6861 6e64 2077 6179 2074 6f20  horthand way to 
+0000a610: 6465 6669 6e65 2072 6561 642d 6f6e 6c79  define read-only
+0000a620: 2076 6172 6961 626c 6573 2069 6e20 7468   variables in th
+0000a630: 6520 2270 6172 616d 7322 0a20 2020 2063  e "params".    c
+0000a640: 6f6c 6c65 6374 696f 6e2e 0a0a 2020 2020  ollection...    
+0000a650: 436f 6e74 7261 7279 2074 6f20 3a6d 6574  Contrary to :met
+0000a660: 683a 6070 6172 616d 602c 2061 6c6c 2061  h:`param`, all a
+0000a670: 7267 756d 656e 7473 2070 6173 7369 6e67  rguments passing
+0000a680: 2075 7369 6e67 2060 696e 6974 5f66 6e60   using `init_fn`
+0000a690: 2073 686f 756c 6420 6265 0a20 2020 2070   should be.    p
+0000a6a0: 6173 7365 6420 6f6e 2065 7870 6c69 6369  assed on explici
+0000a6b0: 746c 793a 3a0a 0a20 2020 2020 206b 6579  tly::..      key
+0000a6c0: 203d 2073 656c 662e 6d61 6b65 5f72 6e67   = self.make_rng
+0000a6d0: 2827 7374 6174 7327 290a 2020 2020 2020  ('stats').      
+0000a6e0: 6d65 616e 203d 2073 656c 662e 7661 7269  mean = self.vari
+0000a6f0: 6162 6c65 2827 7374 6174 7327 2c20 276d  able('stats', 'm
+0000a700: 6561 6e27 2c20 6c65 6375 6e5f 6e6f 726d  ean', lecun_norm
+0000a710: 616c 2829 2c20 6b65 792c 2028 322c 2032  al(), key, (2, 2
+0000a720: 2929 0a0a 2020 2020 496e 2074 6865 2065  ))..    In the e
+0000a730: 7861 6d70 6c65 2061 626f 7665 2c20 7468  xample above, th
+0000a740: 6520 6675 6e63 7469 6f6e 2060 6c65 6375  e function `lecu
+0000a750: 6e5f 6e6f 726d 616c 6020 6578 7065 6374  n_normal` expect
+0000a760: 7320 7477 6f20 6172 6775 6d65 6e74 733a  s two arguments:
+0000a770: 0a20 2020 2060 6b65 7960 2061 6e64 2060  .    `key` and `
+0000a780: 7368 6170 6560 2c20 616e 6420 626f 7468  shape`, and both
+0000a790: 2068 6176 6520 746f 2062 6520 7061 7373   have to be pass
+0000a7a0: 6564 206f 6e2e 2054 6865 2050 524e 4720  ed on. The PRNG 
+0000a7b0: 666f 7220 6073 7461 7473 6020 6861 730a  for `stats` has.
+0000a7c0: 2020 2020 746f 2062 6520 7072 6f76 6964      to be provid
+0000a7d0: 6564 2065 7870 6c69 6369 746c 7920 7768  ed explicitly wh
+0000a7e0: 656e 2063 616c 6c69 6e67 203a 6d65 7468  en calling :meth
+0000a7f0: 3a60 696e 6974 6020 616e 6420 3a6d 6574  :`init` and :met
+0000a800: 683a 6061 7070 6c79 602e 0a0a 2020 2020  h:`apply`...    
+0000a810: 4172 6773 3a0a 2020 2020 2020 636f 6c3a  Args:.      col:
+0000a820: 2054 6865 2076 6172 6961 626c 6520 636f   The variable co
+0000a830: 6c6c 6563 7469 6f6e 206e 616d 652e 0a20  llection name.. 
+0000a840: 2020 2020 206e 616d 653a 2054 6865 2076       name: The v
+0000a850: 6172 6961 626c 6520 6e61 6d65 2e0a 2020  ariable name..  
+0000a860: 2020 2020 696e 6974 5f66 6e3a 2054 6865      init_fn: The
+0000a870: 2066 756e 6374 696f 6e20 7468 6174 2077   function that w
+0000a880: 696c 6c20 6265 2063 616c 6c65 6420 746f  ill be called to
+0000a890: 2063 6f6d 7075 7465 2074 6865 2069 6e69   compute the ini
+0000a8a0: 7469 616c 2076 616c 7565 0a20 2020 2020  tial value.     
+0000a8b0: 2020 206f 6620 7468 6973 2076 6172 6961     of this varia
+0000a8c0: 626c 652e 2054 6869 7320 6675 6e63 7469  ble. This functi
+0000a8d0: 6f6e 2077 696c 6c20 6f6e 6c79 2062 6520  on will only be 
+0000a8e0: 6361 6c6c 6564 2074 6865 2066 6972 7374  called the first
+0000a8f0: 2074 696d 650a 2020 2020 2020 2020 7468   time.        th
+0000a900: 6973 2076 6172 6961 626c 6520 6973 2075  is variable is u
+0000a910: 7365 6420 696e 2074 6869 7320 6d6f 6475  sed in this modu
+0000a920: 6c65 2e20 4966 204e 6f6e 652c 2074 6865  le. If None, the
+0000a930: 2076 6172 6961 626c 6520 6d75 7374 0a20   variable must. 
+0000a940: 2020 2020 2020 2061 6c72 6561 6479 2062         already b
+0000a950: 6520 696e 6974 6961 6c69 7a65 6420 6f74  e initialized ot
+0000a960: 6865 7277 6973 6520 616e 2065 7272 6f72  herwise an error
+0000a970: 2069 7320 7261 6973 6564 2e0a 2020 2020   is raised..    
+0000a980: 2020 2a69 6e69 745f 6172 6773 3a20 5468    *init_args: Th
+0000a990: 6520 6172 6775 6d65 6e74 7320 746f 2070  e arguments to p
+0000a9a0: 6173 7320 746f 2069 6e69 745f 666e 2e0a  ass to init_fn..
+0000a9b0: 2020 2020 2020 756e 626f 783a 2049 6620        unbox: If 
+0000a9c0: 5472 7565 2c20 6060 4178 6973 4d65 7461  True, ``AxisMeta
+0000a9d0: 6461 7461 6060 2069 6e73 7461 6e63 6573  data`` instances
+0000a9e0: 2061 7265 2072 6570 6c61 6365 6420 6279   are replaced by
+0000a9f0: 2074 6865 6972 2075 6e62 6f78 6564 0a20   their unboxed. 
+0000aa00: 2020 2020 2020 2076 616c 7565 2c20 7365         value, se
+0000aa10: 6520 6060 666c 6178 2e6e 6e2e 6d65 7461  e ``flax.nn.meta
+0000aa20: 2e75 6e62 6f78 6060 2028 6465 6661 756c  .unbox`` (defaul
+0000aa30: 743a 2054 7275 6529 2e0a 0a20 2020 2052  t: True)...    R
+0000aa40: 6574 7572 6e73 3a0a 2020 2020 2020 4120  eturns:.      A 
+0000aa50: 3a63 6c61 7373 3a60 666c 6178 2e63 6f72  :class:`flax.cor
+0000aa60: 652e 7661 7269 6162 6c65 732e 5661 7269  e.variables.Vari
+0000aa70: 6162 6c65 6020 7468 6174 2063 616e 2062  able` that can b
+0000aa80: 6520 7265 6164 206f 7220 7365 7420 7669  e read or set vi
+0000aa90: 610a 2020 2020 2020 222e 7661 6c75 6522  a.      ".value"
+0000aaa0: 2061 7474 7269 6275 7465 2e20 5468 726f   attribute. Thro
+0000aab0: 7773 2061 6e20 6572 726f 7220 6966 2074  ws an error if t
+0000aac0: 6865 2076 6172 6961 626c 6520 6578 6973  he variable exis
+0000aad0: 7473 2061 6c72 6561 6479 2e0a 2020 2020  ts already..    
+0000aae0: 2222 220a 2020 2020 6966 206e 6f74 2073  """.    if not s
+0000aaf0: 656c 662e 5f69 6e69 7469 616c 697a 6174  elf._initializat
+0000ab00: 696f 6e5f 616c 6c6f 7765 643a 0a20 2020  ion_allowed:.   
+0000ab10: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000ab20: 726f 7228 0a20 2020 2020 2020 2020 2027  ror(.          '
+0000ab30: 5661 7269 6162 6c65 7320 6d75 7374 2062  Variables must b
+0000ab40: 6520 696e 6974 6961 6c69 7a65 6420 696e  e initialized in
+0000ab50: 2060 7365 7475 7028 2960 206f 7220 696e   `setup()` or in
+0000ab60: 2061 206d 6574 686f 6420 270a 2020 2020   a method '.    
+0000ab70: 2020 2020 2020 2777 7261 7070 6564 2069        'wrapped i
+0000ab80: 6e20 6040 636f 6d70 6163 7460 2729 0a20  n `@compact`'). 
+0000ab90: 2020 2069 6620 7365 6c66 2e5f 6e61 6d65     if self._name
+0000aba0: 5f74 616b 656e 286e 616d 652c 2063 6f6c  _taken(name, col
+0000abb0: 6c65 6374 696f 6e3d 636f 6c29 3a0a 2020  lection=col):.  
+0000abc0: 2020 2020 7261 6973 6520 6572 726f 7273      raise errors
+0000abd0: 2e4e 616d 6549 6e55 7365 4572 726f 7228  .NameInUseError(
+0000abe0: 2776 6172 6961 626c 6527 2c20 6e61 6d65  'variable', name
+0000abf0: 2c20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  , self.__class__
+0000ac00: 2e5f 5f6e 616d 655f 5f29 0a20 2020 2061  .__name__).    a
+0000ac10: 7373 6572 7420 7365 6c66 2e73 636f 7065  ssert self.scope
+0000ac20: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+0000ac30: 2076 203d 2073 656c 662e 7363 6f70 652e   v = self.scope.
+0000ac40: 7661 7269 6162 6c65 2863 6f6c 2c20 6e61  variable(col, na
+0000ac50: 6d65 2c20 696e 6974 5f66 6e2c 202a 696e  me, init_fn, *in
+0000ac60: 6974 5f61 7267 732c 2075 6e62 6f78 3d75  it_args, unbox=u
+0000ac70: 6e62 6f78 290a 2020 2020 7365 6c66 2e5f  nbox).    self._
+0000ac80: 7374 6174 652e 6368 696c 6472 656e 5b6e  state.children[n
+0000ac90: 616d 655d 203d 2063 6f6c 0a20 2020 2072  ame] = col.    r
+0000aca0: 6574 7572 6e20 760a 0a20 2064 6566 2070  eturn v..  def p
+0000acb0: 6172 616d 2873 656c 662c 206e 616d 653a  aram(self, name:
+0000acc0: 2073 7472 2c20 696e 6974 5f66 6e3a 2043   str, init_fn: C
+0000acd0: 616c 6c61 626c 655b 2e2e 2e2c 2054 5d2c  allable[..., T],
+0000ace0: 202a 696e 6974 5f61 7267 732c 0a20 2020   *init_args,.   
+0000acf0: 2020 2020 2020 2020 2075 6e62 6f78 3a20           unbox: 
+0000ad00: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
+0000ad10: 543a 0a20 2020 2022 2222 4465 636c 6172  T:.    """Declar
+0000ad20: 6573 2061 6e64 2072 6574 7572 6e73 2061  es and returns a
+0000ad30: 2070 6172 616d 6574 6572 2069 6e20 7468   parameter in th
+0000ad40: 6973 204d 6f64 756c 652e 0a0a 2020 2020  is Module...    
+0000ad50: 5061 7261 6d65 7465 7273 2061 7265 2072  Parameters are r
+0000ad60: 6561 642d 6f6e 6c79 2076 6172 6961 626c  ead-only variabl
+0000ad70: 6573 2069 6e20 7468 6520 636f 6c6c 6563  es in the collec
+0000ad80: 7469 6f6e 206e 616d 6564 2022 7061 7261  tion named "para
+0000ad90: 6d73 222e 2053 6565 0a20 2020 203a 6d6f  ms". See.    :mo
+0000ada0: 643a 6066 6c61 782e 636f 7265 2e76 6172  d:`flax.core.var
+0000adb0: 6961 626c 6573 6020 666f 7220 6d6f 7265  iables` for more
+0000adc0: 2064 6574 6169 6c73 206f 6e20 7661 7269   details on vari
+0000add0: 6162 6c65 732e 0a0a 2020 2020 5468 6520  ables...    The 
+0000ade0: 6669 7273 7420 6172 6775 6d65 6e74 206f  first argument o
+0000adf0: 6620 6069 6e69 745f 666e 6020 6973 2061  f `init_fn` is a
+0000ae00: 7373 756d 6564 2074 6f20 6265 2061 2050  ssumed to be a P
+0000ae10: 524e 4720 6b65 792c 2077 6869 6368 2069  RNG key, which i
+0000ae20: 730a 2020 2020 7072 6f76 6964 6564 2061  s.    provided a
+0000ae30: 7574 6f6d 6174 6963 616c 6c79 2061 6e64  utomatically and
+0000ae40: 2064 6f65 7320 6e6f 7420 6861 7665 2074   does not have t
+0000ae50: 6f20 6265 2070 6173 7365 6420 7573 696e  o be passed usin
+0000ae60: 6720 6069 6e69 745f 6172 6773 603a 3a0a  g `init_args`::.
+0000ae70: 0a20 2020 2020 206d 6561 6e20 3d20 7365  .      mean = se
+0000ae80: 6c66 2e70 6172 616d 2827 6d65 616e 272c  lf.param('mean',
+0000ae90: 206c 6563 756e 5f6e 6f72 6d61 6c28 292c   lecun_normal(),
+0000aea0: 2028 322c 2032 2929 0a0a 2020 2020 496e   (2, 2))..    In
+0000aeb0: 2074 6865 2065 7861 6d70 6c65 2061 626f   the example abo
+0000aec0: 7665 2c20 7468 6520 6675 6e63 7469 6f6e  ve, the function
+0000aed0: 2060 6c65 6375 6e5f 6e6f 726d 616c 6020   `lecun_normal` 
+0000aee0: 6578 7065 6374 7320 7477 6f20 6172 6775  expects two argu
+0000aef0: 6d65 6e74 733a 0a20 2020 2060 6b65 7960  ments:.    `key`
+0000af00: 2061 6e64 2060 7368 6170 6560 2c20 6275   and `shape`, bu
+0000af10: 7420 6f6e 6c79 2060 7368 6170 6560 2068  t only `shape` h
+0000af20: 6173 2074 6f20 6265 2070 726f 7669 6465  as to be provide
+0000af30: 6420 6578 706c 6963 6974 6c79 3b20 606b  d explicitly; `k
+0000af40: 6579 600a 2020 2020 6973 2073 6574 2061  ey`.    is set a
+0000af50: 7574 6f6d 6174 6963 616c 6c79 2075 7369  utomatically usi
+0000af60: 6e67 2074 6865 2050 524e 4720 666f 7220  ng the PRNG for 
+0000af70: 6070 6172 616d 7360 2074 6861 7420 6973  `params` that is
+0000af80: 2070 6173 7365 6420 7768 656e 0a20 2020   passed when.   
+0000af90: 2069 6e69 7469 616c 697a 696e 6720 7468   initializing th
+0000afa0: 6520 6d6f 6475 6c65 2075 7369 6e67 203a  e module using :
+0000afb0: 6d65 7468 3a60 696e 6974 602e 0a0a 2020  meth:`init`...  
+0000afc0: 2020 4172 6773 3a0a 2020 2020 2020 6e61    Args:.      na
+0000afd0: 6d65 3a20 5468 6520 7061 7261 6d65 7465  me: The paramete
+0000afe0: 7220 6e61 6d65 2e0a 2020 2020 2020 696e  r name..      in
+0000aff0: 6974 5f66 6e3a 2054 6865 2066 756e 6374  it_fn: The funct
+0000b000: 696f 6e20 7468 6174 2077 696c 6c20 6265  ion that will be
+0000b010: 2063 616c 6c65 6420 746f 2063 6f6d 7075   called to compu
+0000b020: 7465 2074 6865 2069 6e69 7469 616c 2076  te the initial v
+0000b030: 616c 7565 0a20 2020 2020 2020 206f 6620  alue.        of 
+0000b040: 7468 6973 2076 6172 6961 626c 652e 2054  this variable. T
+0000b050: 6869 7320 6675 6e63 7469 6f6e 2077 696c  his function wil
+0000b060: 6c20 6f6e 6c79 2062 6520 6361 6c6c 6564  l only be called
+0000b070: 2074 6865 2066 6972 7374 2074 696d 650a   the first time.
+0000b080: 2020 2020 2020 2020 7468 6973 2070 6172          this par
+0000b090: 616d 6574 6572 2069 7320 7573 6564 2069  ameter is used i
+0000b0a0: 6e20 7468 6973 206d 6f64 756c 652e 0a20  n this module.. 
+0000b0b0: 2020 2020 202a 696e 6974 5f61 7267 733a       *init_args:
+0000b0c0: 2054 6865 2061 7267 756d 656e 7473 2074   The arguments t
+0000b0d0: 6f20 7061 7373 2074 6f20 696e 6974 5f66  o pass to init_f
+0000b0e0: 6e2e 0a20 2020 2020 2075 6e62 6f78 3a20  n..      unbox: 
+0000b0f0: 4966 2054 7275 652c 2060 6041 7869 734d  If True, ``AxisM
+0000b100: 6574 6164 6174 6160 6020 696e 7374 616e  etadata`` instan
+0000b110: 6365 7320 6172 6520 7265 706c 6163 6564  ces are replaced
+0000b120: 2062 7920 7468 6569 7220 756e 626f 7865   by their unboxe
+0000b130: 640a 2020 2020 2020 2020 7661 6c75 652c  d.        value,
+0000b140: 2073 6565 2060 6066 6c61 782e 6e6e 2e6d   see ``flax.nn.m
+0000b150: 6574 612e 756e 626f 7860 6020 2864 6566  eta.unbox`` (def
+0000b160: 6175 6c74 3a20 5472 7565 292e 0a0a 2020  ault: True)...  
+0000b170: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000b180: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
+0000b190: 6520 696e 6974 6961 6c69 7a65 6420 7061  e initialized pa
+0000b1a0: 7261 6d65 7465 722e 2054 6872 6f77 7320  rameter. Throws 
+0000b1b0: 616e 2065 7272 6f72 2069 6620 7468 6520  an error if the 
+0000b1c0: 7061 7261 6d65 7465 720a 2020 2020 2020  parameter.      
+0000b1d0: 6578 6973 7473 2061 6c72 6561 6479 2e0a  exists already..
+0000b1e0: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
+0000b1f0: 6f74 2073 656c 662e 5f69 6e69 7469 616c  ot self._initial
+0000b200: 697a 6174 696f 6e5f 616c 6c6f 7765 643a  ization_allowed:
+0000b210: 0a20 2020 2020 2072 6169 7365 2056 616c  .      raise Val
+0000b220: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+0000b230: 2020 2027 5061 7261 6d65 7465 7273 206d     'Parameters m
+0000b240: 7573 7420 6265 2069 6e69 7469 616c 697a  ust be initializ
+0000b250: 6564 2069 6e20 6073 6574 7570 2829 6020  ed in `setup()` 
+0000b260: 6f72 2069 6e20 6120 6d65 7468 6f64 2027  or in a method '
+0000b270: 0a20 2020 2020 2020 2020 2027 7772 6170  .          'wrap
+0000b280: 7065 6420 696e 2060 4063 6f6d 7061 6374  ped in `@compact
+0000b290: 6027 290a 2020 2020 6966 2073 656c 662e  `').    if self.
+0000b2a0: 5f6e 616d 655f 7461 6b65 6e28 6e61 6d65  _name_taken(name
+0000b2b0: 2c20 636f 6c6c 6563 7469 6f6e 3d27 7061  , collection='pa
+0000b2c0: 7261 6d73 2729 3a0a 2020 2020 2020 7261  rams'):.      ra
+0000b2d0: 6973 6520 6572 726f 7273 2e4e 616d 6549  ise errors.NameI
+0000b2e0: 6e55 7365 4572 726f 7228 2770 6172 616d  nUseError('param
+0000b2f0: 272c 206e 616d 652c 2073 656c 662e 5f5f  ', name, self.__
+0000b300: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+0000b310: 290a 2020 2020 6173 7365 7274 2073 656c  ).    assert sel
+0000b320: 662e 7363 6f70 6520 6973 206e 6f74 204e  f.scope is not N
+0000b330: 6f6e 650a 2020 2020 7620 3d20 7365 6c66  one.    v = self
+0000b340: 2e73 636f 7065 2e70 6172 616d 286e 616d  .scope.param(nam
+0000b350: 652c 2069 6e69 745f 666e 2c20 2a69 6e69  e, init_fn, *ini
+0000b360: 745f 6172 6773 2c20 756e 626f 783d 756e  t_args, unbox=un
+0000b370: 626f 7829 0a20 2020 2073 656c 662e 5f73  box).    self._s
+0000b380: 7461 7465 2e63 6869 6c64 7265 6e5b 6e61  tate.children[na
+0000b390: 6d65 5d20 3d20 2770 6172 616d 7327 0a20  me] = 'params'. 
+0000b3a0: 2020 2072 6574 7572 6e20 760a 0a20 2064     return v..  d
+0000b3b0: 6566 2068 6173 5f76 6172 6961 626c 6528  ef has_variable(
+0000b3c0: 7365 6c66 2c20 636f 6c3a 2073 7472 2c20  self, col: str, 
+0000b3d0: 6e61 6d65 3a20 7374 7229 202d 3e20 626f  name: str) -> bo
+0000b3e0: 6f6c 3a0a 2020 2020 2222 2243 6865 636b  ol:.    """Check
+0000b3f0: 7320 6966 2061 2076 6172 6961 626c 6520  s if a variable 
+0000b400: 6f66 2067 6976 656e 2063 6f6c 6c65 6374  of given collect
+0000b410: 696f 6e20 616e 6420 6e61 6d65 2065 7869  ion and name exi
+0000b420: 7374 7320 696e 2074 6869 7320 4d6f 6475  sts in this Modu
+0000b430: 6c65 2e0a 0a20 2020 2053 6565 203a 6d6f  le...    See :mo
+0000b440: 643a 6066 6c61 782e 636f 7265 2e76 6172  d:`flax.core.var
+0000b450: 6961 626c 6573 6020 666f 7220 6d6f 7265  iables` for more
+0000b460: 2065 7870 6c61 6e61 7469 6f6e 206f 6e20   explanation on 
+0000b470: 7661 7269 6162 6c65 7320 616e 640a 2020  variables and.  
+0000b480: 2020 636f 6c6c 6563 7469 6f6e 732e 0a0a    collections...
+0000b490: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000b4a0: 636f 6c3a 2054 6865 2076 6172 6961 626c  col: The variabl
+0000b4b0: 6520 636f 6c6c 6563 7469 6f6e 206e 616d  e collection nam
+0000b4c0: 652e 0a20 2020 2020 206e 616d 653a 2054  e..      name: T
+0000b4d0: 6865 206e 616d 6520 6f66 2074 6865 2076  he name of the v
+0000b4e0: 6172 6961 626c 652e 0a20 2020 2052 6574  ariable..    Ret
+0000b4f0: 7572 6e73 3a0a 2020 2020 2020 5472 7565  urns:.      True
+0000b500: 2069 6620 7468 6520 7661 7269 6162 6c65   if the variable
+0000b510: 2065 7869 7374 732e 0a20 2020 2022 2222   exists..    """
+0000b520: 0a20 2020 2069 6620 7365 6c66 2e73 636f  .    if self.sco
+0000b530: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+0000b540: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000b550: 6f72 2822 4361 6e27 7420 6163 6365 7373  or("Can't access
+0000b560: 2076 6172 6961 626c 6573 206f 6e20 756e   variables on un
+0000b570: 626f 756e 6420 6d6f 6475 6c65 7322 290a  bound modules").
+0000b580: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000b590: 7363 6f70 652e 6861 735f 7661 7269 6162  scope.has_variab
+0000b5a0: 6c65 2863 6f6c 2c20 6e61 6d65 290a 0a20  le(col, name).. 
+0000b5b0: 2064 6566 2069 735f 6d75 7461 626c 655f   def is_mutable_
+0000b5c0: 636f 6c6c 6563 7469 6f6e 2873 656c 662c  collection(self,
+0000b5d0: 2063 6f6c 3a20 7374 7229 202d 3e20 626f   col: str) -> bo
+0000b5e0: 6f6c 3a0a 2020 2020 2222 2252 6574 7572  ol:.    """Retur
+0000b5f0: 6e73 2074 7275 6520 6966 2074 6865 2063  ns true if the c
+0000b600: 6f6c 6c65 6374 696f 6e20 6063 6f6c 6020  ollection `col` 
+0000b610: 6973 206d 7574 6162 6c65 2e22 2222 0a20  is mutable.""". 
+0000b620: 2020 2069 6620 7365 6c66 2e73 636f 7065     if self.scope
+0000b630: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000b640: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000b650: 2822 4361 6e27 7420 6368 6563 6b20 6d75  ("Can't check mu
+0000b660: 7461 6269 6c69 7479 206f 6e20 756e 626f  tability on unbo
+0000b670: 756e 6420 6d6f 6475 6c65 7322 290a 2020  und modules").  
+0000b680: 2020 7265 7475 726e 2073 656c 662e 7363    return self.sc
+0000b690: 6f70 652e 6973 5f6d 7574 6162 6c65 5f63  ope.is_mutable_c
+0000b6a0: 6f6c 6c65 6374 696f 6e28 636f 6c29 0a0a  ollection(col)..
+0000b6b0: 2020 6465 6620 6861 735f 726e 6728 7365    def has_rng(se
+0000b6c0: 6c66 2c20 6e61 6d65 3a20 7374 7229 202d  lf, name: str) -
+0000b6d0: 3e20 626f 6f6c 3a0a 2020 2020 2222 2252  > bool:.    """R
+0000b6e0: 6574 7572 6e73 2074 7275 6520 6966 2061  eturns true if a
+0000b6f0: 2050 524e 4753 6571 7565 6e63 6520 7769   PRNGSequence wi
+0000b700: 7468 206e 616d 6520 606e 616d 6560 2065  th name `name` e
+0000b710: 7869 7374 732e 2222 220a 2020 2020 6966  xists.""".    if
+0000b720: 2073 656c 662e 7363 6f70 6520 6973 204e   self.scope is N
+0000b730: 6f6e 653a 0a20 2020 2020 2072 6169 7365  one:.      raise
+0000b740: 2056 616c 7565 4572 726f 7228 2243 616e   ValueError("Can
+0000b750: 2774 2071 7565 7279 2066 6f72 2052 4e47  't query for RNG
+0000b760: 7320 6f6e 2075 6e62 6f75 6e64 206d 6f64  s on unbound mod
+0000b770: 756c 6573 2229 0a20 2020 2072 6574 7572  ules").    retur
+0000b780: 6e20 7365 6c66 2e73 636f 7065 2e68 6173  n self.scope.has
+0000b790: 5f72 6e67 286e 616d 6529 0a0a 2020 6465  _rng(name)..  de
+0000b7a0: 6620 6d61 6b65 5f72 6e67 2873 656c 662c  f make_rng(self,
+0000b7b0: 206e 616d 653a 2073 7472 2920 2d3e 2050   name: str) -> P
+0000b7c0: 524e 474b 6579 3a0a 2020 2020 2222 2252  RNGKey:.    """R
+0000b7d0: 6574 7572 6e73 2061 206e 6577 2052 4e47  eturns a new RNG
+0000b7e0: 206b 6579 2066 726f 6d20 6120 6769 7665   key from a give
+0000b7f0: 6e20 524e 4720 7365 7175 656e 6365 2066  n RNG sequence f
+0000b800: 6f72 2074 6869 7320 4d6f 6475 6c65 2e0a  or this Module..
+0000b810: 0a20 2020 2054 6865 206e 6577 2052 4e47  .    The new RNG
+0000b820: 206b 6579 2069 7320 7370 6c69 7420 6672   key is split fr
+0000b830: 6f6d 2074 6865 2070 7265 7669 6f75 7320  om the previous 
+0000b840: 6f6e 652e 2054 6875 732c 2065 7665 7279  one. Thus, every
+0000b850: 2063 616c 6c20 746f 0a20 2020 2060 6d61   call to.    `ma
+0000b860: 6b65 5f72 6e67 6020 7265 7475 726e 7320  ke_rng` returns 
+0000b870: 6120 6e65 7720 524e 4720 6b65 792c 2077  a new RNG key, w
+0000b880: 6869 6c65 2073 7469 6c6c 2067 7561 7261  hile still guara
+0000b890: 6e74 6565 696e 6720 6675 6c6c 0a20 2020  nteeing full.   
+0000b8a0: 2072 6570 726f 6475 6369 6269 6c69 7479   reproducibility
+0000b8b0: 2e0a 0a20 2020 2054 4f44 4f3a 204c 696e  ...    TODO: Lin
+0000b8c0: 6b20 746f 2046 6c61 7820 524e 4720 6465  k to Flax RNG de
+0000b8d0: 7369 676e 206e 6f74 652e 0a0a 2020 2020  sign note...    
+0000b8e0: 4172 6773 3a0a 2020 2020 2020 6e61 6d65  Args:.      name
+0000b8f0: 3a20 5468 6520 524e 4720 7365 7175 656e  : The RNG sequen
+0000b900: 6365 206e 616d 652e 0a20 2020 2052 6574  ce name..    Ret
+0000b910: 7572 6e73 3a0a 2020 2020 2020 5468 6520  urns:.      The 
+0000b920: 6e65 776c 7920 6765 6e65 7261 7465 6420  newly generated 
+0000b930: 524e 4720 6b65 792e 0a20 2020 2022 2222  RNG key..    """
+0000b940: 0a20 2020 2069 6620 7365 6c66 2e73 636f  .    if self.sco
+0000b950: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+0000b960: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000b970: 6f72 2822 4361 6e27 7420 7573 6520 524e  or("Can't use RN
+0000b980: 4773 206f 6e20 756e 626f 756e 6420 6d6f  Gs on unbound mo
+0000b990: 6475 6c65 7322 290a 2020 2020 7265 7475  dules").    retu
+0000b9a0: 726e 2073 656c 662e 7363 6f70 652e 6d61  rn self.scope.ma
+0000b9b0: 6b65 5f72 6e67 286e 616d 6529 0a0a 2020  ke_rng(name)..  
+0000b9c0: 6465 6620 6973 5f69 6e69 7469 616c 697a  def is_initializ
+0000b9d0: 696e 6728 7365 6c66 2920 2d3e 2062 6f6f  ing(self) -> boo
+0000b9e0: 6c3a 0a20 2020 2022 2222 5265 7475 726e  l:.    """Return
+0000b9f0: 7320 5472 7565 2069 6620 7275 6e6e 696e  s True if runnin
+0000ba00: 6720 756e 6465 7220 7365 6c66 2e69 6e69  g under self.ini
+0000ba10: 7428 2e2e 2e29 206f 7220 6e6e 2e69 6e69  t(...) or nn.ini
+0000ba20: 7428 2e2e 2e29 2829 2e0a 0a20 2020 2054  t(...)()...    T
+0000ba30: 6869 7320 6973 2061 2068 656c 7065 7220  his is a helper 
+0000ba40: 6d65 7468 6f64 2074 6f20 6861 6e64 6c65  method to handle
+0000ba50: 2074 6865 2063 6f6d 6d6f 6e20 6361 7365   the common case
+0000ba60: 206f 6620 7369 6d70 6c65 2069 6e69 7469   of simple initi
+0000ba70: 616c 697a 6174 696f 6e0a 2020 2020 7768  alization.    wh
+0000ba80: 6572 6520 7765 2077 6973 6820 746f 2068  ere we wish to h
+0000ba90: 6176 6520 7365 7475 7020 6c6f 6769 6320  ave setup logic 
+0000baa0: 6f63 6375 7220 7768 656e 206f 6e6c 7920  occur when only 
+0000bab0: 6361 6c6c 6564 2075 6e64 6572 0a20 2020  called under.   
+0000bac0: 2060 606d 6f64 756c 652e 696e 6974 6060   ``module.init``
+0000bad0: 206f 7220 6060 6e6e 2e69 6e69 7460 602e   or ``nn.init``.
+0000bae0: 2020 466f 7220 6d6f 7265 2063 6f6d 706c    For more compl
+0000baf0: 6963 6174 6564 206d 756c 7469 2d70 6861  icated multi-pha
+0000bb00: 7365 0a20 2020 2069 6e69 7469 616c 697a  se.    initializ
+0000bb10: 6174 696f 6e20 7363 656e 6172 696f 7320  ation scenarios 
+0000bb20: 6974 2069 7320 6265 7474 6572 2074 6f20  it is better to 
+0000bb30: 7465 7374 2066 6f72 2074 6865 206d 7574  test for the mut
+0000bb40: 6162 696c 6974 7920 6f66 0a20 2020 2070  ability of.    p
+0000bb50: 6172 7469 6375 6c61 7220 7661 7269 6162  articular variab
+0000bb60: 6c65 2063 6f6c 6c65 6374 696f 6e73 206f  le collections o
+0000bb70: 7220 666f 7220 7468 6520 7072 6573 656e  r for the presen
+0000bb80: 6365 206f 6620 7061 7274 6963 756c 6172  ce of particular
+0000bb90: 0a20 2020 2076 6172 6961 626c 6573 2074  .    variables t
+0000bba0: 6861 7420 706f 7465 6e74 6961 6c6c 7920  hat potentially 
+0000bbb0: 6e65 6564 2074 6f20 6265 2069 6e69 7469  need to be initi
+0000bbc0: 616c 697a 6564 2e0a 2020 2020 2222 220a  alized..    """.
+0000bbd0: 2020 2020 6966 2073 656c 662e 7363 6f70      if self.scop
+0000bbe0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+0000bbf0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000bc00: 7228 2243 616e 2774 2063 6865 636b 2069  r("Can't check i
+0000bc10: 6620 7275 6e6e 696e 6720 756e 6465 7220  f running under 
+0000bc20: 696e 6974 2829 206f 6e20 756e 626f 756e  init() on unboun
+0000bc30: 6420 6d6f 6475 6c65 7322 290a 2020 2020  d modules").    
+0000bc40: 7265 7475 726e 2073 656c 662e 7363 6f70  return self.scop
+0000bc50: 652e 6765 745f 666c 6167 2827 696e 6974  e.get_flag('init
+0000bc60: 6961 6c69 7a69 6e67 272c 2046 616c 7365  ializing', False
+0000bc70: 290a 0a20 2064 6566 205f 6d6f 6475 6c65  )..  def _module
+0000bc80: 5f63 6865 636b 7328 7365 6c66 293a 0a20  _checks(self):. 
+0000bc90: 2020 2022 2222 5275 6e20 7374 616e 6461     """Run standa
+0000bca0: 7264 2072 756e 7469 6d65 2063 6865 636b  rd runtime check
+0000bcb0: 732e 2222 220a 0a20 2020 2069 6620 6e6f  s."""..    if no
+0000bcc0: 7420 6973 696e 7374 616e 6365 2873 656c  t isinstance(sel
+0000bcd0: 662c 204d 6f64 756c 6529 3a0a 2020 2020  f, Module):.    
+0000bce0: 2020 7261 6973 6520 6572 726f 7273 2e49    raise errors.I
+0000bcf0: 6e76 616c 6964 496e 7374 616e 6365 4d6f  nvalidInstanceMo
+0000bd00: 6475 6c65 4572 726f 7228 290a 0a20 2020  duleError()..   
+0000bd10: 206f 7665 7272 6964 6465 6e5f 706f 7374   overridden_post
+0000bd20: 5f69 6e69 7420 3d20 7365 6c66 2e5f 5f70  _init = self.__p
+0000bd30: 6f73 745f 696e 6974 5f5f 2021 3d20 4d6f  ost_init__ != Mo
+0000bd40: 6475 6c65 2e5f 5f70 6f73 745f 696e 6974  dule.__post_init
+0000bd50: 5f5f 0a20 2020 2069 6620 6f76 6572 7269  __.    if overri
+0000bd60: 6464 656e 5f70 6f73 745f 696e 6974 2061  dden_post_init a
+0000bd70: 6e64 206e 6f74 2068 6173 6174 7472 2873  nd not hasattr(s
+0000bd80: 656c 662c 2022 5f69 6422 293a 0a20 2020  elf, "_id"):.   
+0000bd90: 2020 2072 6169 7365 2065 7272 6f72 732e     raise errors.
+0000bda0: 496e 636f 7272 6563 7450 6f73 7449 6e69  IncorrectPostIni
+0000bdb0: 744f 7665 7272 6964 6545 7272 6f72 2829  tOverrideError()
+0000bdc0: 0a0a 2020 4074 7261 6365 6261 636b 5f75  ..  @traceback_u
+0000bdd0: 7469 6c2e 6170 695f 626f 756e 6461 7279  til.api_boundary
+0000bde0: 0a20 2064 6566 2062 696e 6428 7365 6c66  .  def bind(self
+0000bdf0: 3a20 4d2c 0a20 2020 2020 2020 2020 2020  : M,.           
+0000be00: 7661 7269 6162 6c65 733a 2056 6172 6961  variables: Varia
+0000be10: 626c 6544 6963 742c 0a20 2020 2020 2020  bleDict,.       
+0000be20: 2020 2020 2a61 7267 732c 0a20 2020 2020      *args,.     
+0000be30: 2020 2020 2020 726e 6773 3a20 4f70 7469        rngs: Opti
+0000be40: 6f6e 616c 5b52 4e47 5365 7175 656e 6365  onal[RNGSequence
+0000be50: 735d 203d 204e 6f6e 652c 0a20 2020 2020  s] = None,.     
+0000be60: 2020 2020 2020 6d75 7461 626c 653a 2043        mutable: C
+0000be70: 6f6c 6c65 6374 696f 6e46 696c 7465 7220  ollectionFilter 
+0000be80: 3d20 4661 6c73 6529 202d 3e20 4d3a 0a20  = False) -> M:. 
+0000be90: 2020 2022 2222 4372 6561 7465 7320 616e     """Creates an
+0000bea0: 2069 6e74 6572 6163 7469 7665 204d 6f64   interactive Mod
+0000beb0: 756c 6520 696e 7374 616e 6365 2062 7920  ule instance by 
+0000bec0: 6269 6e64 696e 6720 7661 7269 6162 6c65  binding variable
+0000bed0: 7320 616e 6420 524e 4773 2e0a 0a20 2020  s and RNGs...   
+0000bee0: 2060 6062 696e 6460 6020 7072 6f76 6964   ``bind`` provid
+0000bef0: 6573 2061 6e20 2269 6e74 6572 6163 7469  es an "interacti
+0000bf00: 7665 2220 696e 7374 616e 6365 206f 6620  ve" instance of 
+0000bf10: 6120 4d6f 6475 6c65 2064 6972 6563 746c  a Module directl
+0000bf20: 7920 7769 7468 6f75 740a 2020 2020 7472  y without.    tr
+0000bf30: 616e 7366 6f72 6d69 6e67 2061 2066 756e  ansforming a fun
+0000bf40: 6374 696f 6e20 7769 7468 2060 6061 7070  ction with ``app
+0000bf50: 6c79 6060 2e20 5468 6973 2069 7320 7061  ly``. This is pa
+0000bf60: 7274 6963 756c 6172 6c79 2075 7365 6675  rticularly usefu
+0000bf70: 6c20 666f 720a 2020 2020 6465 6275 6767  l for.    debugg
+0000bf80: 696e 6720 616e 6420 696e 7465 7261 6374  ing and interact
+0000bf90: 6976 6520 7573 6520 6361 7365 7320 6c69  ive use cases li
+0000bfa0: 6b65 206e 6f74 6562 6f6f 6b73 2077 6865  ke notebooks whe
+0000bfb0: 7265 2061 2066 756e 6374 696f 6e20 776f  re a function wo
+0000bfc0: 756c 640a 2020 2020 6c69 6d69 7420 7468  uld.    limit th
+0000bfd0: 6520 6162 696c 6974 7920 746f 2073 706c  e ability to spl
+0000bfe0: 6974 2075 7020 636f 6465 2069 6e74 6f20  it up code into 
+0000bff0: 6469 6666 6572 656e 7420 6365 6c6c 732e  different cells.
+0000c000: 0a0a 2020 2020 4f6e 6365 2074 6865 2076  ..    Once the v
+0000c010: 6172 6961 626c 6573 2028 616e 6420 6f70  ariables (and op
+0000c020: 7469 6f6e 616c 6c79 2052 4e47 7329 2061  tionally RNGs) a
+0000c030: 7265 2062 6f75 6e64 2074 6f20 6120 6060  re bound to a ``
+0000c040: 4d6f 6475 6c65 6060 2069 740a 2020 2020  Module`` it.    
+0000c050: 6265 636f 6d65 7320 6120 7374 6174 6566  becomes a statef
+0000c060: 756c 206f 626a 6563 742e 204e 6f74 6520  ul object. Note 
+0000c070: 7468 6174 2069 6469 6f6d 6174 6963 204a  that idiomatic J
+0000c080: 4158 2069 7320 6675 6e63 7469 6f6e 616c  AX is functional
+0000c090: 2061 6e64 0a20 2020 2074 6865 7265 666f   and.    therefo
+0000c0a0: 7265 2061 6e20 696e 7465 7261 6374 6976  re an interactiv
+0000c0b0: 6520 696e 7374 616e 6365 2064 6f65 7320  e instance does 
+0000c0c0: 6e6f 7420 6d69 7820 7765 6c6c 2077 6974  not mix well wit
+0000c0d0: 6820 7661 6e69 6c6c 6120 4a41 5820 4150  h vanilla JAX AP
+0000c0e0: 4973 2e0a 2020 2020 6060 6269 6e64 2829  Is..    ``bind()
+0000c0f0: 6060 2073 686f 756c 6420 6f6e 6c79 2062  `` should only b
+0000c100: 6520 7573 6564 2066 6f72 2069 6e74 6572  e used for inter
+0000c110: 6163 7469 7665 2065 7870 6572 696d 656e  active experimen
+0000c120: 7461 7469 6f6e 2c20 616e 6420 696e 2061  tation, and in a
+0000c130: 6c6c 0a20 2020 206f 7468 6572 2063 6173  ll.    other cas
+0000c140: 6573 2077 6520 7374 726f 6e67 6c79 2065  es we strongly e
+0000c150: 6e63 6f75 7261 6765 2075 7365 7273 2074  ncourage users t
+0000c160: 6f20 7573 6520 6060 6170 706c 7928 2960  o use ``apply()`
+0000c170: 6020 696e 7374 6561 642e 0a0a 2020 2020  ` instead...    
+0000c180: 4578 616d 706c 653a 3a0a 0a20 2020 2020  Example::..     
+0000c190: 2069 6d70 6f72 7420 6a61 780a 2020 2020   import jax.    
+0000c1a0: 2020 696d 706f 7274 206a 6178 2e6e 756d    import jax.num
+0000c1b0: 7079 2061 7320 6a6e 700a 2020 2020 2020  py as jnp.      
+0000c1c0: 696d 706f 7274 2066 6c61 782e 6c69 6e65  import flax.line
+0000c1d0: 6e20 6173 206e 6e0a 0a20 2020 2020 2063  n as nn..      c
+0000c1e0: 6c61 7373 2041 7574 6f45 6e63 6f64 6572  lass AutoEncoder
+0000c1f0: 286e 6e2e 4d6f 6475 6c65 293a 0a20 2020  (nn.Module):.   
+0000c200: 2020 2020 2064 6566 2073 6574 7570 2873       def setup(s
+0000c210: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+0000c220: 7365 6c66 2e65 6e63 6f64 6572 203d 206e  self.encoder = n
+0000c230: 6e2e 4465 6e73 6528 3329 0a20 2020 2020  n.Dense(3).     
+0000c240: 2020 2020 2073 656c 662e 6465 636f 6465       self.decode
+0000c250: 7220 3d20 6e6e 2e44 656e 7365 2835 290a  r = nn.Dense(5).
+0000c260: 0a20 2020 2020 2020 2064 6566 205f 5f63  .        def __c
+0000c270: 616c 6c5f 5f28 7365 6c66 2c20 7829 3a0a  all__(self, x):.
+0000c280: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c290: 2073 656c 662e 6465 636f 6465 7228 7365   self.decoder(se
+0000c2a0: 6c66 2e65 6e63 6f64 6572 2878 2929 0a0a  lf.encoder(x))..
+0000c2b0: 2020 2020 2020 7820 3d20 6a6e 702e 6f6e        x = jnp.on
+0000c2c0: 6573 2828 3136 2c20 3929 290a 2020 2020  es((16, 9)).    
+0000c2d0: 2020 6165 203d 2041 7574 6f45 6e63 6f64    ae = AutoEncod
+0000c2e0: 6572 2829 0a20 2020 2020 2076 6172 6961  er().      varia
+0000c2f0: 626c 6573 203d 2061 652e 696e 6974 286a  bles = ae.init(j
+0000c300: 6178 2e72 616e 646f 6d2e 5052 4e47 4b65  ax.random.PRNGKe
+0000c310: 7928 3029 2c20 7829 0a20 2020 2020 206d  y(0), x).      m
+0000c320: 6f64 656c 203d 2061 652e 6269 6e64 2876  odel = ae.bind(v
+0000c330: 6172 6961 626c 6573 290a 2020 2020 2020  ariables).      
+0000c340: 7a20 3d20 6d6f 6465 6c2e 656e 636f 6465  z = model.encode
+0000c350: 7228 7829 0a20 2020 2020 2078 5f72 6563  r(x).      x_rec
+0000c360: 6f6e 7374 7275 6374 6564 203d 206d 6f64  onstructed = mod
+0000c370: 656c 2e64 6563 6f64 6572 287a 290a 0a20  el.decoder(z).. 
+0000c380: 2020 2041 7267 733a 0a20 2020 2020 2076     Args:.      v
+0000c390: 6172 6961 626c 6573 3a20 4120 6469 6374  ariables: A dict
+0000c3a0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+0000c3b0: 6720 7661 7269 6162 6c65 7320 6b65 7965  g variables keye
+0000c3c0: 6420 6279 2076 6172 6961 626c 650a 2020  d by variable.  
+0000c3d0: 2020 2020 2020 636f 6c6c 6563 7469 6f6e        collection
+0000c3e0: 732e 2053 6565 203a 6d6f 643a 6066 6c61  s. See :mod:`fla
+0000c3f0: 782e 636f 7265 2e76 6172 6961 626c 6573  x.core.variables
+0000c400: 6020 666f 7220 6d6f 7265 2064 6574 6169  ` for more detai
+0000c410: 6c73 0a20 2020 2020 2020 2061 626f 7574  ls.        about
+0000c420: 2076 6172 6961 626c 6573 2e0a 2020 2020   variables..    
+0000c430: 2020 2a61 7267 733a 204e 616d 6564 2061    *args: Named a
+0000c440: 7267 756d 656e 7473 2028 6e6f 7420 7573  rguments (not us
+0000c450: 6564 292e 0a20 2020 2020 2072 6e67 733a  ed)..      rngs:
+0000c460: 2061 2064 6963 7420 6f66 2050 524e 474b   a dict of PRNGK
+0000c470: 6579 7320 746f 2069 6e69 7469 616c 697a  eys to initializ
+0000c480: 6520 7468 6520 5052 4e47 2073 6571 7565  e the PRNG seque
+0000c490: 6e63 6573 2e0a 2020 2020 2020 6d75 7461  nces..      muta
+0000c4a0: 626c 653a 2043 616e 2062 6520 626f 6f6c  ble: Can be bool
+0000c4b0: 2c20 7374 722c 206f 7220 6c69 7374 2e20  , str, or list. 
+0000c4c0: 5370 6563 6966 6965 7320 7768 6963 6820  Specifies which 
+0000c4d0: 636f 6c6c 6563 7469 6f6e 7320 7368 6f75  collections shou
+0000c4e0: 6c64 2062 650a 2020 2020 2020 2020 7472  ld be.        tr
+0000c4f0: 6561 7465 6420 6173 206d 7574 6162 6c65  eated as mutable
+0000c500: 3a0a 2020 2020 2020 2020 2020 6060 626f  :.          ``bo
+0000c510: 6f6c 6060 3a20 616c 6c2f 6e6f 2063 6f6c  ol``: all/no col
+0000c520: 6c65 6374 696f 6e73 2061 7265 206d 7574  lections are mut
+0000c530: 6162 6c65 2e0a 2020 2020 2020 2020 2020  able..          
+0000c540: 6060 7374 7260 603a 2054 6865 206e 616d  ``str``: The nam
+0000c550: 6520 6f66 2061 2073 696e 676c 6520 6d75  e of a single mu
+0000c560: 7461 626c 6520 636f 6c6c 6563 7469 6f6e  table collection
+0000c570: 2e0a 2020 2020 2020 2020 2020 6060 6c69  ..          ``li
+0000c580: 7374 6060 3a20 4120 6c69 7374 206f 6620  st``: A list of 
+0000c590: 6e61 6d65 7320 6f66 206d 7574 6162 6c65  names of mutable
+0000c5a0: 2063 6f6c 6c65 6374 696f 6e73 2e0a 0a20   collections... 
+0000c5b0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000c5c0: 2020 4120 636f 7079 206f 6620 7468 6973    A copy of this
+0000c5d0: 2069 6e73 7461 6e63 6520 7769 7468 2062   instance with b
+0000c5e0: 6f75 6e64 2076 6172 6961 626c 6573 2061  ound variables a
+0000c5f0: 6e64 2052 4e47 732e 0a20 2020 2022 2222  nd RNGs..    """
+0000c600: 0a20 2020 204d 6f64 756c 652e 5f6d 6f64  .    Module._mod
+0000c610: 756c 655f 6368 6563 6b73 2873 656c 6629  ule_checks(self)
+0000c620: 0a0a 2020 2020 6465 6c20 6172 6773 0a20  ..    del args. 
+0000c630: 2020 2073 636f 7065 203d 2063 6f72 652e     scope = core.
+0000c640: 6269 6e64 2876 6172 6961 626c 6573 2c20  bind(variables, 
+0000c650: 726e 6773 3d72 6e67 732c 206d 7574 6162  rngs=rngs, mutab
+0000c660: 6c65 3d6d 7574 6162 6c65 290a 2020 2020  le=mutable).    
+0000c670: 7265 7475 726e 2073 656c 662e 636c 6f6e  return self.clon
+0000c680: 6528 7061 7265 6e74 3d73 636f 7065 290a  e(parent=scope).
+0000c690: 0a20 2064 6566 2075 6e62 696e 6428 7365  .  def unbind(se
+0000c6a0: 6c66 3a20 4d29 202d 3e20 5475 706c 655b  lf: M) -> Tuple[
+0000c6b0: 4d2c 2056 6172 6961 626c 6544 6963 745d  M, VariableDict]
+0000c6c0: 3a0a 2020 2020 2222 2252 6574 7572 6e73  :.    """Returns
+0000c6d0: 2061 6e20 756e 626f 756e 6420 636f 7079   an unbound copy
+0000c6e0: 206f 6620 6120 4d6f 6475 6c65 2061 6e64   of a Module and
+0000c6f0: 2069 7473 2076 6172 6961 626c 6573 2e0a   its variables..
+0000c700: 0a20 2020 2060 6075 6e62 696e 6460 6020  .    ``unbind`` 
+0000c710: 6865 6c70 7320 6372 6561 7465 2061 2073  helps create a s
+0000c720: 7461 7465 6c65 7373 2076 6572 7369 6f6e  tateless version
+0000c730: 206f 6620 6120 626f 756e 6420 4d6f 6475   of a bound Modu
+0000c740: 6c65 2e0a 0a20 2020 2041 6e20 6578 616d  le...    An exam
+0000c750: 706c 6520 6f66 2061 2063 6f6d 6d6f 6e20  ple of a common 
+0000c760: 7573 6520 6361 7365 3a20 746f 2065 7874  use case: to ext
+0000c770: 7261 6374 2061 2073 7562 2d4d 6f64 756c  ract a sub-Modul
+0000c780: 6520 6465 6669 6e65 6420 696e 7369 6465  e defined inside
+0000c790: 0a20 2020 2060 6073 6574 7570 2829 6060  .    ``setup()``
+0000c7a0: 2061 6e64 2069 7473 2063 6f72 7265 7370   and its corresp
+0000c7b0: 6f6e 6469 6e67 2076 6172 6961 626c 6573  onding variables
+0000c7c0: 3a20 3129 2074 656d 706f 7261 7269 6c79  : 1) temporarily
+0000c7d0: 2060 6062 696e 6460 6020 7468 6520 7061   ``bind`` the pa
+0000c7e0: 7265 6e74 0a20 2020 204d 6f64 756c 653b  rent.    Module;
+0000c7f0: 2061 6e64 2074 6865 6e20 3229 2060 6075   and then 2) ``u
+0000c800: 6e62 696e 6460 6020 7468 6520 6465 7369  nbind`` the desi
+0000c810: 7265 6420 7375 622d 4d6f 6475 6c65 2e20  red sub-Module. 
+0000c820: 2852 6563 616c 6c20 7468 6174 2060 6073  (Recall that ``s
+0000c830: 6574 7570 2829 6060 0a20 2020 2069 7320  etup()``.    is 
+0000c840: 6f6e 6c79 2063 616c 6c65 6420 7768 656e  only called when
+0000c850: 2074 6865 204d 6f64 756c 6520 6973 2062   the Module is b
+0000c860: 6f75 6e64 2e29 3a3a 0a0a 2020 2020 2020  ound.)::..      
+0000c870: 636c 6173 7320 4175 746f 456e 636f 6465  class AutoEncode
+0000c880: 7228 6e6e 2e4d 6f64 756c 6529 3a0a 2020  r(nn.Module):.  
+0000c890: 2020 2020 2020 6465 6620 7365 7475 7028        def setup(
+0000c8a0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
+0000c8b0: 2073 656c 662e 656e 636f 6465 7220 3d20   self.encoder = 
+0000c8c0: 456e 636f 6465 7228 290a 2020 2020 2020  Encoder().      
+0000c8d0: 2020 2020 7365 6c66 2e64 6563 6f64 6572      self.decoder
+0000c8e0: 203d 2044 6563 6f64 6572 2829 0a0a 2020   = Decoder()..  
+0000c8f0: 2020 2020 2020 6465 6620 5f5f 6361 6c6c        def __call
+0000c900: 5f5f 2873 656c 662c 2078 293a 0a20 2020  __(self, x):.   
+0000c910: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000c920: 6c66 2e64 6563 6f64 6572 2873 656c 662e  lf.decoder(self.
+0000c930: 656e 636f 6465 7228 7829 290a 0a20 2020  encoder(x))..   
+0000c940: 2020 206d 6f64 756c 6520 3d20 4175 746f     module = Auto
+0000c950: 456e 636f 6465 7228 290a 2020 2020 2020  Encoder().      
+0000c960: 7661 7269 6162 6c65 7320 3d20 6d6f 6475  variables = modu
+0000c970: 6c65 2e69 6e69 7428 6a61 782e 7261 6e64  le.init(jax.rand
+0000c980: 6f6d 2e50 524e 474b 6579 2830 292c 206a  om.PRNGKey(0), j
+0000c990: 6e70 2e6f 6e65 7328 2831 2c20 3738 3429  np.ones((1, 784)
+0000c9a0: 2929 0a20 2020 2020 202e 2e2e 0a20 2020  )).      ....   
+0000c9b0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
+0000c9c0: 2045 6e63 6f64 6572 2073 7562 2d4d 6f64   Encoder sub-Mod
+0000c9d0: 756c 6520 616e 6420 6974 7320 7661 7269  ule and its vari
+0000c9e0: 6162 6c65 730a 2020 2020 2020 656e 636f  ables.      enco
+0000c9f0: 6465 722c 2065 6e63 6f64 6572 5f76 6172  der, encoder_var
+0000ca00: 7320 3d20 6d6f 6475 6c65 2e62 696e 6428  s = module.bind(
+0000ca10: 7661 7269 6162 6c65 7329 2e65 6e63 6f64  variables).encod
+0000ca20: 6572 2e75 6e62 696e 6428 290a 0a20 2020  er.unbind()..   
+0000ca30: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000ca40: 4120 7475 706c 6520 7769 7468 2061 6e20  A tuple with an 
+0000ca50: 756e 626f 756e 6420 636f 7079 206f 6620  unbound copy of 
+0000ca60: 7468 6973 204d 6f64 756c 6520 616e 6420  this Module and 
+0000ca70: 6974 7320 7661 7269 6162 6c65 732e 0a20  its variables.. 
+0000ca80: 2020 2022 2222 0a20 2020 204d 6f64 756c     """.    Modul
+0000ca90: 652e 5f6d 6f64 756c 655f 6368 6563 6b73  e._module_checks
+0000caa0: 2873 656c 6629 0a0a 2020 2020 6966 2073  (self)..    if s
+0000cab0: 656c 662e 7363 6f70 6520 6973 204e 6f6e  elf.scope is Non
+0000cac0: 653a 0a20 2020 2020 2072 6169 7365 2065  e:.      raise e
+0000cad0: 7272 6f72 732e 4361 6c6c 556e 6269 6e64  rrors.CallUnbind
+0000cae0: 4f6e 556e 626f 756e 644d 6f64 756c 6545  OnUnboundModuleE
+0000caf0: 7272 6f72 2829 0a0a 2020 2020 7661 7269  rror()..    vari
+0000cb00: 6162 6c65 7320 3d20 7365 6c66 2e76 6172  ables = self.var
+0000cb10: 6961 626c 6573 0a20 2020 206d 6f64 756c  iables.    modul
+0000cb20: 6520 3d20 7365 6c66 2e63 6c6f 6e65 2829  e = self.clone()
+0000cb30: 0a20 2020 2072 6574 7572 6e20 6d6f 6475  .    return modu
+0000cb40: 6c65 2c20 7661 7269 6162 6c65 730a 0a20  le, variables.. 
+0000cb50: 2040 7472 6163 6562 6163 6b5f 7574 696c   @traceback_util
+0000cb60: 2e61 7069 5f62 6f75 6e64 6172 790a 2020  .api_boundary.  
+0000cb70: 6465 6620 6170 706c 7928 7365 6c66 2c0a  def apply(self,.
+0000cb80: 2020 2020 2020 2020 2020 2020 7661 7269              vari
+0000cb90: 6162 6c65 733a 2056 6172 6961 626c 6544  ables: VariableD
+0000cba0: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
+0000cbb0: 202a 6172 6773 2c0a 2020 2020 2020 2020   *args,.        
+0000cbc0: 2020 2020 726e 6773 3a20 4f70 7469 6f6e      rngs: Option
+0000cbd0: 616c 5b52 4e47 5365 7175 656e 6365 735d  al[RNGSequences]
+0000cbe0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000cbf0: 2020 2020 206d 6574 686f 643a 2055 6e69       method: Uni
+0000cc00: 6f6e 5b43 616c 6c61 626c 655b 2e2e 2e2c  on[Callable[...,
+0000cc10: 2041 6e79 5d2c 2073 7472 2c20 4e6f 6e65   Any], str, None
+0000cc20: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000cc30: 2020 2020 2020 6d75 7461 626c 653a 2043        mutable: C
+0000cc40: 6f6c 6c65 6374 696f 6e46 696c 7465 7220  ollectionFilter 
+0000cc50: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+0000cc60: 2020 2020 2063 6170 7475 7265 5f69 6e74       capture_int
+0000cc70: 6572 6d65 6469 6174 6573 3a20 556e 696f  ermediates: Unio
+0000cc80: 6e5b 626f 6f6c 2c20 4361 6c6c 6162 6c65  n[bool, Callable
+0000cc90: 5b5b 274d 6f64 756c 6527 2c20 7374 725d  [['Module', str]
+0000cca0: 2c20 626f 6f6c 5d5d 203d 2046 616c 7365  , bool]] = False
+0000ccb0: 2c0a 2020 2020 2020 2020 2020 2020 2a2a  ,.            **
+0000ccc0: 6b77 6172 6773 2920 2d3e 2055 6e69 6f6e  kwargs) -> Union
+0000ccd0: 5b41 6e79 2c20 5475 706c 655b 416e 792c  [Any, Tuple[Any,
+0000cce0: 2055 6e69 6f6e 5b46 726f 7a65 6e56 6172   Union[FrozenVar
+0000ccf0: 6961 626c 6544 6963 742c 2044 6963 745b  iableDict, Dict[
+0000cd00: 7374 722c 2041 6e79 5d5d 5d5d 3a0a 2020  str, Any]]]]:.  
+0000cd10: 2020 2222 2241 7070 6c69 6573 2061 206d    """Applies a m
+0000cd20: 6f64 756c 6520 6d65 7468 6f64 2074 6f20  odule method to 
+0000cd30: 7661 7269 6162 6c65 7320 616e 6420 7265  variables and re
+0000cd40: 7475 726e 7320 6f75 7470 7574 2061 6e64  turns output and
+0000cd50: 206d 6f64 6966 6965 6420 7661 7269 6162   modified variab
+0000cd60: 6c65 732e 0a0a 2020 2020 4e6f 7465 2074  les...    Note t
+0000cd70: 6861 7420 606d 6574 686f 6460 2073 686f  hat `method` sho
+0000cd80: 756c 6420 6265 2073 6574 2069 6620 6f6e  uld be set if on
+0000cd90: 6520 776f 756c 6420 6c69 6b65 2074 6f20  e would like to 
+0000cda0: 6361 6c6c 2060 6170 706c 7960 206f 6e20  call `apply` on 
+0000cdb0: 610a 2020 2020 6469 6666 6572 656e 7420  a.    different 
+0000cdc0: 636c 6173 7320 6d65 7468 6f64 2074 6861  class method tha
+0000cdd0: 6e20 6060 5f5f 6361 6c6c 5f5f 6060 2e20  n ``__call__``. 
+0000cde0: 466f 7220 696e 7374 616e 6365 2c20 7375  For instance, su
+0000cdf0: 7070 6f73 6520 610a 2020 2020 5472 616e  ppose a.    Tran
+0000ce00: 7366 6f72 6d65 7220 6d6f 6475 6c65 7320  sformer modules 
+0000ce10: 6861 7320 6120 6d65 7468 6f64 2063 616c  has a method cal
+0000ce20: 6c65 6420 6065 6e63 6f64 6560 2c20 7468  led `encode`, th
+0000ce30: 656e 2074 6865 2066 6f6c 6c6f 7769 6e67  en the following
+0000ce40: 2063 616c 6c73 0a20 2020 2060 6170 706c   calls.    `appl
+0000ce50: 7960 206f 6e20 7468 6174 206d 6574 686f  y` on that metho
+0000ce60: 643a 3a0a 0a20 2020 2020 206d 6f64 656c  d::..      model
+0000ce70: 203d 2054 7261 6e73 666f 726d 6572 2829   = Transformer()
+0000ce80: 0a20 2020 2020 2065 6e63 6f64 6564 203d  .      encoded =
+0000ce90: 206d 6f64 656c 2e61 7070 6c79 287b 2770   model.apply({'p
+0000cea0: 6172 616d 7327 3a20 7061 7261 6d73 7d2c  arams': params},
+0000ceb0: 2078 2c20 6d65 7468 6f64 3d54 7261 6e73   x, method=Trans
+0000cec0: 666f 726d 6572 2e65 6e63 6f64 6529 0a0a  former.encode)..
+0000ced0: 2020 2020 4966 2061 2066 756e 6374 696f      If a functio
+0000cee0: 6e20 696e 7374 616e 6365 2069 7320 7072  n instance is pr
+0000cef0: 6f76 6964 6564 2c20 7468 6520 756e 626f  ovided, the unbo
+0000cf00: 756e 6420 6675 6e63 7469 6f6e 2069 7320  und function is 
+0000cf10: 7573 6564 2e20 466f 720a 2020 2020 696e  used. For.    in
+0000cf20: 7374 616e 6365 2c20 7468 6520 6578 616d  stance, the exam
+0000cf30: 706c 6520 6265 6c6f 7720 6973 2065 7175  ple below is equ
+0000cf40: 6976 616c 656e 7420 746f 2074 6865 206f  ivalent to the o
+0000cf50: 6e65 2061 626f 7665 3a3a 0a0a 2020 2020  ne above::..    
+0000cf60: 2020 656e 636f 6465 6420 3d20 6d6f 6465    encoded = mode
+0000cf70: 6c2e 6170 706c 7928 7b27 7061 7261 6d73  l.apply({'params
+0000cf80: 273a 2070 6172 616d 737d 2c20 782c 206d  ': params}, x, m
+0000cf90: 6574 686f 643d 6d6f 6465 6c2e 656e 636f  ethod=model.enco
+0000cfa0: 6465 290a 0a20 2020 2059 6f75 2063 616e  de)..    You can
+0000cfb0: 2061 6c73 6f20 7061 7373 2061 2073 7472   also pass a str
+0000cfc0: 696e 6720 746f 2061 2063 616c 6c61 626c  ing to a callabl
+0000cfd0: 6520 6174 7472 6962 7574 6520 6f66 2074  e attribute of t
+0000cfe0: 6865 206d 6f64 756c 652e 2046 6f72 0a20  he module. For. 
+0000cff0: 2020 2065 7861 6d70 6c65 2c20 7468 6520     example, the 
+0000d000: 7072 6576 696f 7573 2063 616e 2062 6520  previous can be 
+0000d010: 7772 6974 7465 6e20 6173 3a3a 0a0a 2020  written as::..  
+0000d020: 2020 2020 656e 636f 6465 6420 3d20 6d6f      encoded = mo
+0000d030: 6465 6c2e 6170 706c 7928 7b27 7061 7261  del.apply({'para
+0000d040: 6d73 273a 2070 6172 616d 737d 2c20 782c  ms': params}, x,
+0000d050: 206d 6574 686f 643d 2765 6e63 6f64 6527   method='encode'
+0000d060: 290a 0a20 2020 204e 6f74 6520 6060 6d65  )..    Note ``me
+0000d070: 7468 6f64 6060 2063 616e 2061 6c73 6f20  thod`` can also 
+0000d080: 6265 2061 2066 756e 6374 696f 6e20 7468  be a function th
+0000d090: 6174 2069 7320 6e6f 7420 6465 6669 6e65  at is not define
+0000d0a0: 6420 696e 0a20 2020 2060 6054 7261 6e73  d in.    ``Trans
+0000d0b0: 666f 726d 6572 6060 2e20 496e 2074 6861  former``. In tha
+0000d0c0: 7420 6361 7365 2c20 7468 6520 6675 6e63  t case, the func
+0000d0d0: 7469 6f6e 2073 686f 756c 6420 6861 7665  tion should have
+0000d0e0: 2061 7420 6c65 6173 7420 6f6e 650a 2020   at least one.  
+0000d0f0: 2020 6172 6775 6d65 6e74 2072 6570 7265    argument repre
+0000d100: 7365 6e74 696e 6720 616e 2069 6e73 7461  senting an insta
+0000d110: 6e63 6520 6f66 2074 6865 204d 6f64 756c  nce of the Modul
+0000d120: 6520 636c 6173 733a 3a0a 0a20 2020 2020  e class::..     
+0000d130: 2064 6566 206f 7468 6572 5f66 6e28 696e   def other_fn(in
+0000d140: 7374 616e 6365 2c20 2e2e 2e29 3a0a 2020  stance, ...):.  
+0000d150: 2020 2020 2020 696e 7374 616e 6365 2e73        instance.s
+0000d160: 6f6d 655f 6d6f 6475 6c65 5f61 7474 7228  ome_module_attr(
+0000d170: 2e2e 2e29 0a20 2020 2020 2020 202e 2e2e  ...).        ...
+0000d180: 0a0a 2020 2020 2020 6d6f 6465 6c2e 6170  ..      model.ap
+0000d190: 706c 7928 7b27 7061 7261 6d73 273a 2070  ply({'params': p
+0000d1a0: 6172 616d 737d 2c20 782c 206d 6574 686f  arams}, x, metho
+0000d1b0: 643d 6f74 6865 725f 666e 290a 0a20 2020  d=other_fn)..   
+0000d1c0: 2041 7267 733a 0a20 2020 2020 2076 6172   Args:.      var
+0000d1d0: 6961 626c 6573 3a20 4120 6469 6374 696f  iables: A dictio
+0000d1e0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+0000d1f0: 7661 7269 6162 6c65 7320 6b65 7965 6420  variables keyed 
+0000d200: 6279 2076 6172 6961 626c 650a 2020 2020  by variable.    
+0000d210: 2020 2020 636f 6c6c 6563 7469 6f6e 732e      collections.
+0000d220: 2053 6565 203a 6d6f 643a 6066 6c61 782e   See :mod:`flax.
+0000d230: 636f 7265 2e76 6172 6961 626c 6573 6020  core.variables` 
+0000d240: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
+0000d250: 0a20 2020 2020 2020 2061 626f 7574 2076  .        about v
+0000d260: 6172 6961 626c 6573 2e0a 2020 2020 2020  ariables..      
+0000d270: 2a61 7267 733a 204e 616d 6564 2061 7267  *args: Named arg
+0000d280: 756d 656e 7473 2070 6173 7365 6420 746f  uments passed to
+0000d290: 2074 6865 2073 7065 6369 6669 6564 2061   the specified a
+0000d2a0: 7070 6c79 206d 6574 686f 642e 0a20 2020  pply method..   
+0000d2b0: 2020 2072 6e67 733a 2061 2064 6963 7420     rngs: a dict 
+0000d2c0: 6f66 2050 524e 474b 6579 7320 746f 2069  of PRNGKeys to i
+0000d2d0: 6e69 7469 616c 697a 6520 7468 6520 5052  nitialize the PR
+0000d2e0: 4e47 2073 6571 7565 6e63 6573 2e0a 2020  NG sequences..  
+0000d2f0: 2020 2020 2020 5468 6520 2270 6172 616d        The "param
+0000d300: 7322 2050 524e 4720 7365 7175 656e 6365  s" PRNG sequence
+0000d310: 2069 7320 7573 6564 2074 6f20 696e 6974   is used to init
+0000d320: 6961 6c69 7a65 2070 6172 616d 6574 6572  ialize parameter
+0000d330: 732e 0a20 2020 2020 206d 6574 686f 643a  s..      method:
+0000d340: 2041 2066 756e 6374 696f 6e20 746f 2063   A function to c
+0000d350: 616c 6c20 6170 706c 7920 6f6e 2e20 5468  all apply on. Th
+0000d360: 6973 2069 7320 6765 6e65 7261 6c6c 7920  is is generally 
+0000d370: 6120 6675 6e63 7469 6f6e 2069 6e20 7468  a function in th
+0000d380: 650a 2020 2020 2020 2020 6d6f 6475 6c65  e.        module
+0000d390: 2e20 4966 2070 726f 7669 6465 642c 2061  . If provided, a
+0000d3a0: 7070 6c69 6573 2074 6869 7320 6d65 7468  pplies this meth
+0000d3b0: 6f64 2e20 4966 206e 6f74 2070 726f 7669  od. If not provi
+0000d3c0: 6465 642c 2061 7070 6c69 6573 2074 6865  ded, applies the
+0000d3d0: 0a20 2020 2020 2020 2060 605f 5f63 616c  .        ``__cal
+0000d3e0: 6c5f 5f60 6020 6d65 7468 6f64 206f 6620  l__`` method of 
+0000d3f0: 7468 6520 6d6f 6475 6c65 2e20 4120 7374  the module. A st
+0000d400: 7269 6e67 2063 616e 2061 6c73 6f20 6265  ring can also be
+0000d410: 2070 726f 7669 6465 6420 746f 0a20 2020   provided to.   
+0000d420: 2020 2020 2073 7065 6369 6679 2061 206d       specify a m
+0000d430: 6574 686f 6420 6279 206e 616d 652e 0a20  ethod by name.. 
+0000d440: 2020 2020 206d 7574 6162 6c65 3a20 4361       mutable: Ca
+0000d450: 6e20 6265 2062 6f6f 6c2c 2073 7472 2c20  n be bool, str, 
+0000d460: 6f72 206c 6973 742e 2053 7065 6369 6669  or list. Specifi
+0000d470: 6573 2077 6869 6368 2063 6f6c 6c65 6374  es which collect
+0000d480: 696f 6e73 2073 686f 756c 6420 6265 0a20  ions should be. 
+0000d490: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000d4a0: 6561 7465 6420 6173 206d 7574 6162 6c65  eated as mutable
+0000d4b0: 3a20 6060 626f 6f6c 6060 3a20 616c 6c2f  : ``bool``: all/
+0000d4c0: 6e6f 2063 6f6c 6c65 6374 696f 6e73 2061  no collections a
+0000d4d0: 7265 206d 7574 6162 6c65 2e0a 2020 2020  re mutable..    
+0000d4e0: 2020 2020 2020 2020 2020 2060 6073 7472             ``str
+0000d4f0: 6060 3a20 5468 6520 6e61 6d65 206f 6620  ``: The name of 
+0000d500: 6120 7369 6e67 6c65 206d 7574 6162 6c65  a single mutable
+0000d510: 2063 6f6c 6c65 6374 696f 6e2e 2060 606c   collection. ``l
+0000d520: 6973 7460 603a 2041 0a20 2020 2020 2020  ist``: A.       
+0000d530: 2020 2020 2020 2020 6c69 7374 206f 6620          list of 
+0000d540: 6e61 6d65 7320 6f66 206d 7574 6162 6c65  names of mutable
+0000d550: 2063 6f6c 6c65 6374 696f 6e73 2e0a 2020   collections..  
+0000d560: 2020 2020 6361 7074 7572 655f 696e 7465      capture_inte
+0000d570: 726d 6564 6961 7465 733a 2049 6620 6054  rmediates: If `T
+0000d580: 7275 6560 2c20 6361 7074 7572 6573 2069  rue`, captures i
+0000d590: 6e74 6572 6d65 6469 6174 6520 7265 7475  ntermediate retu
+0000d5a0: 726e 2076 616c 7565 730a 2020 2020 2020  rn values.      
+0000d5b0: 2020 6f66 2061 6c6c 204d 6f64 756c 6573    of all Modules
+0000d5c0: 2069 6e73 6964 6520 7468 6520 2269 6e74   inside the "int
+0000d5d0: 6572 6d65 6469 6174 6573 2220 636f 6c6c  ermediates" coll
+0000d5e0: 6563 7469 6f6e 2e20 4279 2064 6566 6175  ection. By defau
+0000d5f0: 6c74 206f 6e6c 790a 2020 2020 2020 2020  lt only.        
+0000d600: 7468 6520 7265 7475 726e 2076 616c 7565  the return value
+0000d610: 7320 6f66 2061 6c6c 2060 605f 5f63 616c  s of all ``__cal
+0000d620: 6c5f 5f60 6020 6d65 7468 6f64 7320 6172  l__`` methods ar
+0000d630: 6520 7374 6f72 6564 2e20 4120 6675 6e63  e stored. A func
+0000d640: 7469 6f6e 2063 616e 0a20 2020 2020 2020  tion can.       
+0000d650: 2062 6520 7061 7373 6564 2074 6f20 6368   be passed to ch
+0000d660: 616e 6765 2074 6865 2066 696c 7465 7220  ange the filter 
+0000d670: 6265 6861 7669 6f72 2e20 5468 6520 6669  behavior. The fi
+0000d680: 6c74 6572 2066 756e 6374 696f 6e20 7461  lter function ta
+0000d690: 6b65 730a 2020 2020 2020 2020 7468 6520  kes.        the 
+0000d6a0: 4d6f 6475 6c65 2069 6e73 7461 6e63 6520  Module instance 
+0000d6b0: 616e 6420 6d65 7468 6f64 206e 616d 6520  and method name 
+0000d6c0: 616e 6420 7265 7475 726e 7320 6120 626f  and returns a bo
+0000d6d0: 6f6c 2069 6e64 6963 6174 696e 670a 2020  ol indicating.  
+0000d6e0: 2020 2020 2020 7768 6574 6865 7220 7468        whether th
+0000d6f0: 6520 6f75 7470 7574 206f 6620 7468 6174  e output of that
+0000d700: 206d 6574 686f 6420 696e 766f 6361 7469   method invocati
+0000d710: 6f6e 2073 686f 756c 6420 6265 2073 746f  on should be sto
+0000d720: 7265 642e 0a20 2020 2020 202a 2a6b 7761  red..      **kwa
+0000d730: 7267 733a 204b 6579 776f 7264 2061 7267  rgs: Keyword arg
+0000d740: 756d 656e 7473 2070 6173 7365 6420 746f  uments passed to
+0000d750: 2074 6865 2073 7065 6369 6669 6564 2061   the specified a
+0000d760: 7070 6c79 206d 6574 686f 642e 0a20 2020  pply method..   
+0000d770: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000d780: 4966 2060 606d 7574 6162 6c65 6060 2069  If ``mutable`` i
+0000d790: 7320 4661 6c73 652c 2072 6574 7572 6e73  s False, returns
+0000d7a0: 206f 7574 7075 742e 2049 6620 616e 7920   output. If any 
+0000d7b0: 636f 6c6c 6563 7469 6f6e 7320 6172 650a  collections are.
+0000d7c0: 2020 2020 2020 6d75 7461 626c 652c 2072        mutable, r
+0000d7d0: 6574 7572 6e73 2060 6028 6f75 7470 7574  eturns ``(output
+0000d7e0: 2c20 7661 7273 2960 602c 2077 6865 7265  , vars)``, where
+0000d7f0: 2060 6076 6172 7360 6020 6172 6520 6973   ``vars`` are is
+0000d800: 2061 2064 6963 740a 2020 2020 2020 6f66   a dict.      of
+0000d810: 2074 6865 206d 6f64 6966 6965 6420 636f   the modified co
+0000d820: 6c6c 6563 7469 6f6e 732e 0a20 2020 2022  llections..    "
+0000d830: 2222 0a20 2020 204d 6f64 756c 652e 5f6d  "".    Module._m
+0000d840: 6f64 756c 655f 6368 6563 6b73 2873 656c  odule_checks(sel
+0000d850: 6629 0a0a 2020 2020 6966 2069 7369 6e73  f)..    if isins
+0000d860: 7461 6e63 6528 6d65 7468 6f64 2c20 7374  tance(method, st
+0000d870: 7229 3a0a 2020 2020 2020 6174 7472 6962  r):.      attrib
+0000d880: 7574 655f 6e61 6d65 203d 206d 6574 686f  ute_name = metho
+0000d890: 640a 2020 2020 2020 6d65 7468 6f64 203d  d.      method =
+0000d8a0: 2067 6574 6174 7472 2873 656c 662c 2061   getattr(self, a
+0000d8b0: 7474 7269 6275 7465 5f6e 616d 6529 0a20  ttribute_name). 
+0000d8c0: 2020 2020 2069 6620 6e6f 7420 6361 6c6c       if not call
+0000d8d0: 6162 6c65 286d 6574 686f 6429 3a0a 2020  able(method):.  
+0000d8e0: 2020 2020 2020 636c 6173 735f 6e61 6d65        class_name
+0000d8f0: 203d 2074 7970 6528 7365 6c66 292e 5f5f   = type(self).__
+0000d900: 6e61 6d65 5f5f 0a20 2020 2020 2020 2072  name__.        r
+0000d910: 6169 7365 2054 7970 6545 7272 6f72 2866  aise TypeError(f
+0000d920: 275c 277b 636c 6173 735f 6e61 6d65 7d2e  '\'{class_name}.
+0000d930: 7b61 7474 7269 6275 7465 5f6e 616d 657d  {attribute_name}
+0000d940: 5c27 206d 7573 7420 6265 2061 2063 616c  \' must be a cal
+0000d950: 6c61 626c 652c 2067 6f74 207b 7479 7065  lable, got {type
+0000d960: 286d 6574 686f 6429 7d2e 2729 0a20 2020  (method)}.').   
+0000d970: 2065 6c69 6620 6d65 7468 6f64 2069 7320   elif method is 
+0000d980: 4e6f 6e65 3a0a 2020 2020 2020 6d65 7468  None:.      meth
+0000d990: 6f64 203d 2073 656c 662e 5f5f 6361 6c6c  od = self.__call
+0000d9a0: 5f5f 0a20 2020 206d 6574 686f 6420 3d20  __.    method = 
+0000d9b0: 5f67 6574 5f75 6e62 6f75 6e64 5f66 6e28  _get_unbound_fn(
+0000d9c0: 6d65 7468 6f64 290a 2020 2020 7265 7475  method).    retu
+0000d9d0: 726e 2061 7070 6c79 280a 2020 2020 2020  rn apply(.      
+0000d9e0: 2020 6d65 7468 6f64 2c20 7365 6c66 2c0a    method, self,.
+0000d9f0: 2020 2020 2020 2020 6d75 7461 626c 653d          mutable=
+0000da00: 6d75 7461 626c 652c 0a20 2020 2020 2020  mutable,.       
+0000da10: 2063 6170 7475 7265 5f69 6e74 6572 6d65   capture_interme
+0000da20: 6469 6174 6573 3d63 6170 7475 7265 5f69  diates=capture_i
+0000da30: 6e74 6572 6d65 6469 6174 6573 2c0a 2020  ntermediates,.  
+0000da40: 2020 2928 7661 7269 6162 6c65 732c 202a    )(variables, *
+0000da50: 6172 6773 2c20 2a2a 6b77 6172 6773 2c20  args, **kwargs, 
+0000da60: 726e 6773 3d72 6e67 7329 0a0a 2020 4074  rngs=rngs)..  @t
+0000da70: 7261 6365 6261 636b 5f75 7469 6c2e 6170  raceback_util.ap
+0000da80: 695f 626f 756e 6461 7279 0a20 2064 6566  i_boundary.  def
+0000da90: 2069 6e69 745f 7769 7468 5f6f 7574 7075   init_with_outpu
+0000daa0: 7428 7365 6c66 2c0a 2020 2020 2020 2020  t(self,.        
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000dac0: 6e67 733a 2055 6e69 6f6e 5b50 524e 474b  ngs: Union[PRNGK
+0000dad0: 6579 2c20 524e 4753 6571 7565 6e63 6573  ey, RNGSequences
+0000dae0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000daf0: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
+0000db00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000db10: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+0000db20: 556e 696f 6e5b 4361 6c6c 6162 6c65 5b2e  Union[Callable[.
+0000db30: 2e2e 2c20 416e 795d 2c20 7374 722c 204e  .., Any], str, N
+0000db40: 6f6e 655d 203d 204e 6f6e 652c 0a20 2020  one] = None,.   
+0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db60: 2020 2020 6d75 7461 626c 653a 2043 6f6c      mutable: Col
+0000db70: 6c65 6374 696f 6e46 696c 7465 7220 3d20  lectionFilter = 
+0000db80: 4465 6e79 4c69 7374 2827 696e 7465 726d  DenyList('interm
+0000db90: 6564 6961 7465 7327 292c 0a20 2020 2020  ediates'),.     
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 6361 7074 7572 655f 696e 7465 726d    capture_interm
+0000dbc0: 6564 6961 7465 733a 2055 6e69 6f6e 5b62  ediates: Union[b
+0000dbd0: 6f6f 6c2c 2043 616c 6c61 626c 655b 5b27  ool, Callable[['
+0000dbe0: 4d6f 6475 6c65 272c 2073 7472 5d2c 2062  Module', str], b
+0000dbf0: 6f6f 6c5d 5d20 3d20 4661 6c73 652c 0a20  ool]] = False,. 
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc10: 2020 2020 2020 2a2a 6b77 6172 6773 2920        **kwargs) 
+0000dc20: 2d3e 2054 7570 6c65 5b41 6e79 2c20 556e  -> Tuple[Any, Un
+0000dc30: 696f 6e5b 4672 6f7a 656e 5661 7269 6162  ion[FrozenVariab
+0000dc40: 6c65 4469 6374 2c20 4469 6374 5b73 7472  leDict, Dict[str
+0000dc50: 2c20 416e 795d 5d5d 3a0a 2020 2020 2222  , Any]]]:.    ""
+0000dc60: 2249 6e69 7469 616c 697a 6573 2061 206d  "Initializes a m
+0000dc70: 6f64 756c 6520 6d65 7468 6f64 2077 6974  odule method wit
+0000dc80: 6820 7661 7269 6162 6c65 7320 616e 6420  h variables and 
+0000dc90: 7265 7475 726e 7320 6f75 7470 7574 2061  returns output a
+0000dca0: 6e64 206d 6f64 6966 6965 6420 7661 7269  nd modified vari
+0000dcb0: 6162 6c65 732e 0a0a 2020 2020 4172 6773  ables...    Args
+0000dcc0: 3a0a 2020 2020 2020 726e 6773 3a20 5468  :.      rngs: Th
+0000dcd0: 6520 726e 6773 2066 6f72 2074 6865 2076  e rngs for the v
+0000dce0: 6172 6961 626c 6520 636f 6c6c 6563 7469  ariable collecti
+0000dcf0: 6f6e 732e 0a20 2020 2020 202a 6172 6773  ons..      *args
+0000dd00: 3a20 4e61 6d65 6420 6172 6775 6d65 6e74  : Named argument
+0000dd10: 7320 7061 7373 6564 2074 6f20 7468 6520  s passed to the 
+0000dd20: 696e 6974 2066 756e 6374 696f 6e2e 0a20  init function.. 
+0000dd30: 2020 2020 206d 6574 686f 643a 2041 6e20       method: An 
+0000dd40: 6f70 7469 6f6e 616c 206d 6574 686f 642e  optional method.
+0000dd50: 2049 6620 7072 6f76 6964 6564 2c20 6170   If provided, ap
+0000dd60: 706c 6965 7320 7468 6973 206d 6574 686f  plies this metho
+0000dd70: 642e 2049 6620 6e6f 740a 2020 2020 2020  d. If not.      
+0000dd80: 2020 7072 6f76 6964 6564 2c20 6170 706c    provided, appl
+0000dd90: 6965 7320 7468 6520 6060 5f5f 6361 6c6c  ies the ``__call
+0000dda0: 5f5f 6060 206d 6574 686f 642e 2041 2073  __`` method. A s
+0000ddb0: 7472 696e 6720 6361 6e20 616c 736f 2062  tring can also b
+0000ddc0: 6527 0a20 2020 2020 2020 2070 726f 7669  e'.        provi
+0000ddd0: 6465 6420 746f 2073 7065 6369 6679 2061  ded to specify a
+0000dde0: 206d 6574 686f 6420 6279 206e 616d 652e   method by name.
+0000ddf0: 0a20 2020 2020 206d 7574 6162 6c65 3a20  .      mutable: 
+0000de00: 4361 6e20 6265 2062 6f6f 6c2c 2073 7472  Can be bool, str
+0000de10: 2c20 6f72 206c 6973 742e 2053 7065 6369  , or list. Speci
+0000de20: 6669 6573 2077 6869 6368 2063 6f6c 6c65  fies which colle
+0000de30: 6374 696f 6e73 2073 686f 756c 6420 6265  ctions should be
+0000de40: 0a20 2020 2020 2020 2074 7265 6174 6564  .        treated
+0000de50: 2061 7320 6d75 7461 626c 653a 2060 6062   as mutable: ``b
+0000de60: 6f6f 6c60 603a 2061 6c6c 2f6e 6f20 636f  ool``: all/no co
+0000de70: 6c6c 6563 7469 6f6e 7320 6172 6520 6d75  llections are mu
+0000de80: 7461 626c 652e 0a20 2020 2020 2020 2060  table..        `
+0000de90: 6073 7472 6060 3a20 5468 6520 6e61 6d65  `str``: The name
+0000dea0: 206f 6620 6120 7369 6e67 6c65 206d 7574   of a single mut
+0000deb0: 6162 6c65 2063 6f6c 6c65 6374 696f 6e2e  able collection.
+0000dec0: 2060 606c 6973 7460 603a 2041 0a20 2020   ``list``: A.   
+0000ded0: 2020 2020 206c 6973 7420 6f66 206e 616d       list of nam
+0000dee0: 6573 206f 6620 6d75 7461 626c 6520 636f  es of mutable co
+0000def0: 6c6c 6563 7469 6f6e 732e 2042 7920 6465  llections. By de
+0000df00: 6661 756c 7420 616c 6c20 636f 6c6c 6563  fault all collec
+0000df10: 7469 6f6e 730a 2020 2020 2020 2020 6578  tions.        ex
+0000df20: 6365 7074 2022 696e 7465 726d 6564 6961  cept "intermedia
+0000df30: 7465 7322 2061 7265 206d 7574 6162 6c65  tes" are mutable
+0000df40: 2e0a 2020 2020 2020 6361 7074 7572 655f  ..      capture_
+0000df50: 696e 7465 726d 6564 6961 7465 733a 2049  intermediates: I
+0000df60: 6620 6054 7275 6560 2c20 6361 7074 7572  f `True`, captur
+0000df70: 6573 2069 6e74 6572 6d65 6469 6174 6520  es intermediate 
+0000df80: 7265 7475 726e 2076 616c 7565 730a 2020  return values.  
+0000df90: 2020 2020 2020 6f66 2061 6c6c 204d 6f64        of all Mod
+0000dfa0: 756c 6573 2069 6e73 6964 6520 7468 6520  ules inside the 
+0000dfb0: 2269 6e74 6572 6d65 6469 6174 6573 2220  "intermediates" 
+0000dfc0: 636f 6c6c 6563 7469 6f6e 2e20 4279 2064  collection. By d
+0000dfd0: 6566 6175 6c74 206f 6e6c 790a 2020 2020  efault only.    
+0000dfe0: 2020 2020 7468 6520 7265 7475 726e 2076      the return v
+0000dff0: 616c 7565 7320 6f66 2061 6c6c 2060 605f  alues of all ``_
+0000e000: 5f63 616c 6c5f 5f60 6020 6d65 7468 6f64  _call__`` method
+0000e010: 7320 6172 6520 7374 6f72 6564 2e20 4120  s are stored. A 
+0000e020: 6675 6e63 7469 6f6e 2063 616e 0a20 2020  function can.   
+0000e030: 2020 2020 2062 6520 7061 7373 6564 2074       be passed t
+0000e040: 6f20 6368 616e 6765 2074 6865 2066 696c  o change the fil
+0000e050: 7465 7220 6265 6861 7669 6f72 2e20 5468  ter behavior. Th
+0000e060: 6520 6669 6c74 6572 2066 756e 6374 696f  e filter functio
+0000e070: 6e20 7461 6b65 730a 2020 2020 2020 2020  n takes.        
+0000e080: 7468 6520 4d6f 6475 6c65 2069 6e73 7461  the Module insta
+0000e090: 6e63 6520 616e 6420 6d65 7468 6f64 206e  nce and method n
+0000e0a0: 616d 6520 616e 6420 7265 7475 726e 7320  ame and returns 
+0000e0b0: 6120 626f 6f6c 2069 6e64 6963 6174 696e  a bool indicatin
+0000e0c0: 670a 2020 2020 2020 2020 7768 6574 6865  g.        whethe
+0000e0d0: 7220 7468 6520 6f75 7470 7574 206f 6620  r the output of 
+0000e0e0: 7468 6174 206d 6574 686f 6420 696e 766f  that method invo
+0000e0f0: 6361 7469 6f6e 2073 686f 756c 6420 6265  cation should be
+0000e100: 2073 746f 7265 642e 0a20 2020 2020 202a   stored..      *
+0000e110: 2a6b 7761 7267 733a 204b 6579 776f 7264  *kwargs: Keyword
+0000e120: 2061 7267 756d 656e 7473 2070 6173 7365   arguments passe
+0000e130: 6420 746f 2074 6865 2069 6e69 7420 6675  d to the init fu
+0000e140: 6e63 7469 6f6e 2e0a 2020 2020 5265 7475  nction..    Retu
+0000e150: 726e 733a 0a20 2020 2020 2060 286f 7574  rns:.      `(out
+0000e160: 7075 742c 2076 6172 7329 6060 2c20 7768  put, vars)``, wh
+0000e170: 6572 6520 6060 7661 7273 6060 2061 7265  ere ``vars`` are
+0000e180: 2069 7320 6120 6469 6374 206f 6620 7468   is a dict of th
+0000e190: 6520 6d6f 6469 6669 6564 0a20 2020 2020  e modified.     
+0000e1a0: 2063 6f6c 6c65 6374 696f 6e73 2e0a 2020   collections..  
+0000e1b0: 2020 2222 220a 2020 2020 4d6f 6475 6c65    """.    Module
+0000e1c0: 2e5f 6d6f 6475 6c65 5f63 6865 636b 7328  ._module_checks(
+0000e1d0: 7365 6c66 290a 0a20 2020 2069 6620 6e6f  self)..    if no
+0000e1e0: 7420 6973 696e 7374 616e 6365 2872 6e67  t isinstance(rng
+0000e1f0: 732c 2064 6963 7429 3a0a 2020 2020 2020  s, dict):.      
+0000e200: 6966 206e 6f74 2063 6f72 652e 7363 6f70  if not core.scop
+0000e210: 652e 5f69 735f 7661 6c69 645f 726e 6728  e._is_valid_rng(
+0000e220: 726e 6773 293a 0a20 2020 2020 2020 2072  rngs):.        r
+0000e230: 6169 7365 2065 7272 6f72 732e 496e 7661  aise errors.Inva
+0000e240: 6c69 6452 6e67 4572 726f 7228 0a20 2020  lidRngError(.   
+0000e250: 2020 2020 2020 2020 2027 524e 4773 2073           'RNGs s
+0000e260: 686f 756c 6420 6265 206f 6620 7368 6170  hould be of shap
+0000e270: 6520 2832 2c29 206f 7220 4b65 7941 7272  e (2,) or KeyArr
+0000e280: 6179 2069 6e20 4d6f 6475 6c65 2027 0a20  ay in Module '. 
+0000e290: 2020 2020 2020 2020 2020 2066 277b 7365             f'{se
+0000e2a0: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
+0000e2b0: 616d 655f 5f7d 2c20 6275 7420 726e 6773  ame__}, but rngs
+0000e2c0: 2061 7265 3a20 7b72 6e67 737d 2729 0a20   are: {rngs}'). 
+0000e2d0: 2020 2020 2072 6e67 7320 3d20 7b27 7061       rngs = {'pa
+0000e2e0: 7261 6d73 273a 2072 6e67 737d 0a0a 2020  rams': rngs}..  
+0000e2f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000e300: 6d65 7468 6f64 2c20 7374 7229 3a0a 2020  method, str):.  
+0000e310: 2020 2020 6174 7472 6962 7574 655f 6e61      attribute_na
+0000e320: 6d65 203d 206d 6574 686f 640a 2020 2020  me = method.    
+0000e330: 2020 6d65 7468 6f64 203d 2067 6574 6174    method = getat
+0000e340: 7472 2873 656c 662c 2061 7474 7269 6275  tr(self, attribu
+0000e350: 7465 5f6e 616d 6529 0a20 2020 2020 2069  te_name).      i
+0000e360: 6620 6e6f 7420 6361 6c6c 6162 6c65 286d  f not callable(m
+0000e370: 6574 686f 6429 3a0a 2020 2020 2020 2020  ethod):.        
+0000e380: 636c 6173 735f 6e61 6d65 203d 2074 7970  class_name = typ
+0000e390: 6528 7365 6c66 292e 5f5f 6e61 6d65 5f5f  e(self).__name__
+0000e3a0: 0a20 2020 2020 2020 2072 6169 7365 2054  .        raise T
+0000e3b0: 7970 6545 7272 6f72 2866 275c 277b 636c  ypeError(f'\'{cl
+0000e3c0: 6173 735f 6e61 6d65 7d2e 7b61 7474 7269  ass_name}.{attri
+0000e3d0: 6275 7465 5f6e 616d 657d 5c27 206d 7573  bute_name}\' mus
+0000e3e0: 7420 6265 2061 2063 616c 6c61 626c 652c  t be a callable,
+0000e3f0: 2067 6f74 207b 7479 7065 286d 6574 686f   got {type(metho
+0000e400: 6429 7d2e 2729 0a20 2020 2065 6c69 6620  d)}.').    elif 
+0000e410: 6d65 7468 6f64 2069 7320 4e6f 6e65 3a0a  method is None:.
+0000e420: 2020 2020 2020 6d65 7468 6f64 203d 2073        method = s
+0000e430: 656c 662e 5f5f 6361 6c6c 5f5f 0a20 2020  elf.__call__.   
+0000e440: 206d 6574 686f 6420 3d20 5f67 6574 5f75   method = _get_u
+0000e450: 6e62 6f75 6e64 5f66 6e28 6d65 7468 6f64  nbound_fn(method
+0000e460: 290a 2020 2020 7265 7475 726e 2069 6e69  ).    return ini
+0000e470: 745f 7769 7468 5f6f 7574 7075 7428 0a20  t_with_output(. 
+0000e480: 2020 2020 2020 206d 6574 686f 642c 0a20         method,. 
+0000e490: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000e4a0: 2020 2020 206d 7574 6162 6c65 3d6d 7574       mutable=mut
+0000e4b0: 6162 6c65 2c0a 2020 2020 2020 2020 6361  able,.        ca
+0000e4c0: 7074 7572 655f 696e 7465 726d 6564 6961  pture_intermedia
+0000e4d0: 7465 733d 6361 7074 7572 655f 696e 7465  tes=capture_inte
+0000e4e0: 726d 6564 6961 7465 730a 2020 2020 2928  rmediates.    )(
+0000e4f0: 726e 6773 2c20 2a61 7267 732c 202a 2a6b  rngs, *args, **k
+0000e500: 7761 7267 7329 0a0a 2020 4074 7261 6365  wargs)..  @trace
+0000e510: 6261 636b 5f75 7469 6c2e 6170 695f 626f  back_util.api_bo
+0000e520: 756e 6461 7279 0a20 2064 6566 2069 6e69  undary.  def ini
+0000e530: 7428 7365 6c66 2c0a 2020 2020 2020 2020  t(self,.        
+0000e540: 2020 2072 6e67 733a 2055 6e69 6f6e 5b50     rngs: Union[P
+0000e550: 524e 474b 6579 2c20 524e 4753 6571 7565  RNGKey, RNGSeque
+0000e560: 6e63 6573 5d2c 0a20 2020 2020 2020 2020  nces],.         
+0000e570: 2020 2a61 7267 732c 0a20 2020 2020 2020    *args,.       
+0000e580: 2020 2020 6d65 7468 6f64 3a20 556e 696f      method: Unio
+0000e590: 6e5b 4361 6c6c 6162 6c65 5b2e 2e2e 2c20  n[Callable[..., 
+0000e5a0: 416e 795d 2c20 7374 722c 204e 6f6e 655d  Any], str, None]
+0000e5b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000e5c0: 2020 2020 6d75 7461 626c 653a 2043 6f6c      mutable: Col
+0000e5d0: 6c65 6374 696f 6e46 696c 7465 7220 3d20  lectionFilter = 
+0000e5e0: 4465 6e79 4c69 7374 2827 696e 7465 726d  DenyList('interm
+0000e5f0: 6564 6961 7465 7327 292c 0a20 2020 2020  ediates'),.     
+0000e600: 2020 2020 2020 6361 7074 7572 655f 696e        capture_in
+0000e610: 7465 726d 6564 6961 7465 733a 2055 6e69  termediates: Uni
+0000e620: 6f6e 5b62 6f6f 6c2c 2043 616c 6c61 626c  on[bool, Callabl
+0000e630: 655b 5b27 4d6f 6475 6c65 272c 2073 7472  e[['Module', str
+0000e640: 5d2c 2062 6f6f 6c5d 5d20 3d20 4661 6c73  ], bool]] = Fals
+0000e650: 652c 0a20 2020 2020 2020 2020 2020 2a2a  e,.           **
+0000e660: 6b77 6172 6773 2920 2d3e 2055 6e69 6f6e  kwargs) -> Union
+0000e670: 5b46 726f 7a65 6e56 6172 6961 626c 6544  [FrozenVariableD
+0000e680: 6963 742c 2044 6963 745b 7374 722c 2041  ict, Dict[str, A
+0000e690: 6e79 5d5d 3a0a 2020 2020 2222 2249 6e69  ny]]:.    """Ini
+0000e6a0: 7469 616c 697a 6573 2061 206d 6f64 756c  tializes a modul
+0000e6b0: 6520 6d65 7468 6f64 2077 6974 6820 7661  e method with va
+0000e6c0: 7269 6162 6c65 7320 616e 6420 7265 7475  riables and retu
+0000e6d0: 726e 7320 6d6f 6469 6669 6564 2076 6172  rns modified var
+0000e6e0: 6961 626c 6573 2e0a 0a20 2020 2060 6069  iables...    ``i
+0000e6f0: 6e69 7460 6020 7461 6b65 7320 6173 2066  nit`` takes as f
+0000e700: 6972 7374 2061 7267 756d 656e 7420 6569  irst argument ei
+0000e710: 7468 6572 2061 2073 696e 676c 6520 6060  ther a single ``
+0000e720: 5052 4e47 4b65 7960 602c 206f 7220 6120  PRNGKey``, or a 
+0000e730: 6469 6374 696f 6e61 7279 206d 6170 7069  dictionary mappi
+0000e740: 6e67 2076 6172 6961 626c 6520 636f 6c6c  ng variable coll
+0000e750: 6563 7469 6f6e 7320 6e61 6d65 7320 746f  ections names to
+0000e760: 2074 6865 6972 2060 6050 524e 474b 6579   their ``PRNGKey
+0000e770: 7360 602c 2061 6e64 2077 696c 6c20 6361  s``, and will ca
+0000e780: 6c6c 2060 606d 6574 686f 6460 6020 2877  ll ``method`` (w
+0000e790: 6869 6368 2069 7320 7468 6520 6d6f 6475  hich is the modu
+0000e7a0: 6c65 2773 2060 605f 5f63 616c 6c5f 5f60  le's ``__call__`
+0000e7b0: 6020 6675 6e63 7469 6f6e 2062 7920 6465  ` function by de
+0000e7c0: 6661 756c 7429 2070 6173 7369 6e67 2060  fault) passing `
+0000e7d0: 602a 6172 6773 6060 2061 6e64 2060 602a  `*args`` and ``*
+0000e7e0: 2a6b 7761 7267 7360 602c 2061 6e64 2072  *kwargs``, and r
+0000e7f0: 6574 7572 6e73 0a20 2020 2061 2064 6963  eturns.    a dic
+0000e800: 7469 6f6e 6172 7920 6f66 2069 6e69 7469  tionary of initi
+0000e810: 616c 697a 6564 2076 6172 6961 626c 6573  alized variables
+0000e820: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a3a  ...    Example::
+0000e830: 0a0a 2020 2020 2020 3e3e 3e20 696d 706f  ..      >>> impo
+0000e840: 7274 2066 6c61 782e 6c69 6e65 6e20 6173  rt flax.linen as
+0000e850: 206e 6e0a 2020 2020 2020 3e3e 3e20 696d   nn.      >>> im
+0000e860: 706f 7274 206a 6178 2e6e 756d 7079 2061  port jax.numpy a
+0000e870: 7320 6a6e 700a 2020 2020 2020 3e3e 3e20  s jnp.      >>> 
+0000e880: 696d 706f 7274 206a 6178 0a20 2020 2020  import jax.     
+0000e890: 202e 2e2e 0a20 2020 2020 203e 3e3e 2063   ....      >>> c
+0000e8a0: 6c61 7373 2046 6f6f 286e 6e2e 4d6f 6475  lass Foo(nn.Modu
+0000e8b0: 6c65 293a 0a20 2020 2020 202e 2e2e 2020  le):.      ...  
+0000e8c0: 2040 6e6e 2e63 6f6d 7061 6374 0a20 2020   @nn.compact.   
+0000e8d0: 2020 202e 2e2e 2020 2064 6566 205f 5f63     ...   def __c
+0000e8e0: 616c 6c5f 5f28 7365 6c66 2c20 782c 2074  all__(self, x, t
+0000e8f0: 7261 696e 293a 0a20 2020 2020 202e 2e2e  rain):.      ...
+0000e900: 2020 2020 2078 203d 206e 6e2e 4465 6e73       x = nn.Dens
+0000e910: 6528 3136 2928 7829 0a20 2020 2020 202e  e(16)(x).      .
+0000e920: 2e2e 2020 2020 2078 203d 206e 6e2e 4261  ..     x = nn.Ba
+0000e930: 7463 684e 6f72 6d28 7573 655f 7275 6e6e  tchNorm(use_runn
+0000e940: 696e 675f 6176 6572 6167 653d 6e6f 7420  ing_average=not 
+0000e950: 7472 6169 6e29 2878 290a 2020 2020 2020  train)(x).      
+0000e960: 2e2e 2e20 2020 2020 7820 3d20 6e6e 2e72  ...     x = nn.r
+0000e970: 656c 7528 7829 0a20 2020 2020 202e 2e2e  elu(x).      ...
+0000e980: 2020 2020 2072 6574 7572 6e20 6e6e 2e44       return nn.D
+0000e990: 656e 7365 2831 2928 7829 0a20 2020 2020  ense(1)(x).     
+0000e9a0: 202e 2e2e 0a20 2020 2020 203e 3e3e 206d   ....      >>> m
+0000e9b0: 6f64 756c 6520 3d20 466f 6f28 290a 2020  odule = Foo().  
+0000e9c0: 2020 2020 3e3e 3e20 6b65 7920 3d20 6a61      >>> key = ja
+0000e9d0: 782e 7261 6e64 6f6d 2e50 524e 474b 6579  x.random.PRNGKey
+0000e9e0: 2830 290a 2020 2020 2020 3e3e 3e20 7661  (0).      >>> va
+0000e9f0: 7269 6162 6c65 7320 3d20 6d6f 6475 6c65  riables = module
+0000ea00: 2e69 6e69 7428 6b65 792c 206a 6e70 2e65  .init(key, jnp.e
+0000ea10: 6d70 7479 2828 312c 2037 2929 2c20 7472  mpty((1, 7)), tr
+0000ea20: 6169 6e3d 4661 6c73 6529 0a0a 2020 2020  ain=False)..    
+0000ea30: 4966 2079 6f75 2070 6173 7320 6120 7369  If you pass a si
+0000ea40: 6e67 6c65 2060 6050 524e 474b 6579 6060  ngle ``PRNGKey``
+0000ea50: 2c20 466c 6178 2077 696c 6c20 7573 6520  , Flax will use 
+0000ea60: 6974 2074 6f20 6665 6564 2074 6865 2060  it to feed the `
+0000ea70: 6027 7061 7261 6d73 2760 6020 524e 4720  `'params'`` RNG 
+0000ea80: 7374 7265 616d 2e0a 2020 2020 4966 2079  stream..    If y
+0000ea90: 6f75 2077 616e 7420 746f 2075 7365 2061  ou want to use a
+0000eaa0: 2064 6966 6665 7265 6e74 2052 4e47 2073   different RNG s
+0000eab0: 7472 6561 6d20 6f72 206e 6565 6420 746f  tream or need to
+0000eac0: 2075 7365 206d 756c 7469 706c 6520 7374   use multiple st
+0000ead0: 7265 616d 732c 2079 6f75 206d 7573 7420  reams, you must 
+0000eae0: 7061 7373 2061 0a20 2020 2064 6963 7469  pass a.    dicti
+0000eaf0: 6f6e 6172 7920 6d61 7070 696e 6720 6561  onary mapping ea
+0000eb00: 6368 2052 4e47 2073 7472 6561 6d20 6e61  ch RNG stream na
+0000eb10: 6d65 2074 6f20 6974 7320 636f 7272 6573  me to its corres
+0000eb20: 706f 6e64 696e 6720 6060 5052 4e47 4b65  ponding ``PRNGKe
+0000eb30: 7960 6020 746f 2060 6069 6e69 7460 602e  y`` to ``init``.
+0000eb40: 0a0a 2020 2020 4578 616d 706c 653a 3a0a  ..    Example::.
+0000eb50: 0a20 2020 2020 203e 3e3e 2063 6c61 7373  .      >>> class
+0000eb60: 2046 6f6f 286e 6e2e 4d6f 6475 6c65 293a   Foo(nn.Module):
+0000eb70: 0a20 2020 2020 202e 2e2e 2020 2040 6e6e  .      ...   @nn
+0000eb80: 2e63 6f6d 7061 6374 0a20 2020 2020 202e  .compact.      .
+0000eb90: 2e2e 2020 2064 6566 205f 5f63 616c 6c5f  ..   def __call_
+0000eba0: 5f28 7365 6c66 2c20 782c 2074 7261 696e  _(self, x, train
+0000ebb0: 293a 0a20 2020 2020 202e 2e2e 2020 2020  ):.      ...    
+0000ebc0: 2078 203d 206e 6e2e 4465 6e73 6528 3136   x = nn.Dense(16
+0000ebd0: 2928 7829 0a20 2020 2020 202e 2e2e 2020  )(x).      ...  
+0000ebe0: 2020 2078 203d 206e 6e2e 4261 7463 684e     x = nn.BatchN
+0000ebf0: 6f72 6d28 7573 655f 7275 6e6e 696e 675f  orm(use_running_
+0000ec00: 6176 6572 6167 653d 6e6f 7420 7472 6169  average=not trai
+0000ec10: 6e29 2878 290a 2020 2020 2020 2e2e 2e20  n)(x).      ... 
+0000ec20: 2020 2020 7820 3d20 6e6e 2e72 656c 7528      x = nn.relu(
+0000ec30: 7829 0a20 2020 2020 202e 2e2e 0a20 2020  x).      ....   
+0000ec40: 2020 202e 2e2e 2020 2020 2023 2041 6464     ...     # Add
+0000ec50: 2067 6175 7373 6961 6e20 6e6f 6973 650a   gaussian noise.
+0000ec60: 2020 2020 2020 2e2e 2e20 2020 2020 6e6f        ...     no
+0000ec70: 6973 655f 6b65 7920 3d20 7365 6c66 2e6d  ise_key = self.m
+0000ec80: 616b 655f 726e 6728 276e 6f69 7365 2729  ake_rng('noise')
+0000ec90: 0a20 2020 2020 202e 2e2e 2020 2020 2078  .      ...     x
+0000eca0: 203d 2078 202b 206a 6178 2e72 616e 646f   = x + jax.rando
+0000ecb0: 6d2e 6e6f 726d 616c 286e 6f69 7365 5f6b  m.normal(noise_k
+0000ecc0: 6579 2c20 782e 7368 6170 6529 0a20 2020  ey, x.shape).   
+0000ecd0: 2020 202e 2e2e 0a20 2020 2020 202e 2e2e     ....      ...
+0000ece0: 2020 2020 2072 6574 7572 6e20 6e6e 2e44       return nn.D
+0000ecf0: 656e 7365 2831 2928 7829 0a20 2020 2020  ense(1)(x).     
+0000ed00: 202e 2e2e 0a20 2020 2020 203e 3e3e 206d   ....      >>> m
+0000ed10: 6f64 756c 6520 3d20 466f 6f28 290a 2020  odule = Foo().  
+0000ed20: 2020 2020 3e3e 3e20 726e 6773 203d 207b      >>> rngs = {
+0000ed30: 2770 6172 616d 7327 3a20 6a61 782e 7261  'params': jax.ra
+0000ed40: 6e64 6f6d 2e50 524e 474b 6579 2830 292c  ndom.PRNGKey(0),
+0000ed50: 2027 6e6f 6973 6527 3a20 6a61 782e 7261   'noise': jax.ra
+0000ed60: 6e64 6f6d 2e50 524e 474b 6579 2831 297d  ndom.PRNGKey(1)}
+0000ed70: 0a20 2020 2020 203e 3e3e 2076 6172 6961  .      >>> varia
+0000ed80: 626c 6573 203d 206d 6f64 756c 652e 696e  bles = module.in
+0000ed90: 6974 2872 6e67 732c 206a 6e70 2e65 6d70  it(rngs, jnp.emp
+0000eda0: 7479 2828 312c 2037 2929 2c20 7472 6169  ty((1, 7)), trai
+0000edb0: 6e3d 4661 6c73 6529 0a0a 2020 2020 4a69  n=False)..    Ji
+0000edc0: 7474 696e 6720 6069 6e69 7460 2069 6e69  tting `init` ini
+0000edd0: 7469 616c 697a 6573 2061 206d 6f64 656c  tializes a model
+0000ede0: 206c 617a 696c 7920 7573 696e 6720 6f6e   lazily using on
+0000edf0: 6c79 2074 6865 2073 6861 7065 7320 6f66  ly the shapes of
+0000ee00: 2074 6865 0a20 2020 2070 726f 7669 6465   the.    provide
+0000ee10: 6420 6172 6775 6d65 6e74 732c 2061 6e64  d arguments, and
+0000ee20: 2061 766f 6964 7320 636f 6d70 7574 696e   avoids computin
+0000ee30: 6720 7468 6520 666f 7277 6172 6420 7061  g the forward pa
+0000ee40: 7373 2077 6974 6820 6163 7475 616c 0a20  ss with actual. 
+0000ee50: 2020 2076 616c 7565 732e 2045 7861 6d70     values. Examp
+0000ee60: 6c65 3a3a 0a0a 2020 2020 2020 3e3e 3e20  le::..      >>> 
+0000ee70: 6d6f 6475 6c65 203d 206e 6e2e 4465 6e73  module = nn.Dens
+0000ee80: 6528 3129 0a20 2020 2020 203e 3e3e 2069  e(1).      >>> i
+0000ee90: 6e69 745f 6a69 7420 3d20 6a61 782e 6a69  nit_jit = jax.ji
+0000eea0: 7428 6d6f 6475 6c65 2e69 6e69 7429 0a20  t(module.init). 
+0000eeb0: 2020 2020 203e 3e3e 2076 6172 6961 626c       >>> variabl
+0000eec0: 6573 203d 2069 6e69 745f 6a69 7428 6a61  es = init_jit(ja
+0000eed0: 782e 7261 6e64 6f6d 2e50 524e 474b 6579  x.random.PRNGKey
+0000eee0: 2830 292c 206a 6e70 2e65 6d70 7479 2828  (0), jnp.empty((
+0000eef0: 312c 2037 2929 290a 0a20 2020 2060 6069  1, 7)))..    ``i
+0000ef00: 6e69 7460 6020 6973 2061 206c 6967 6874  nit`` is a light
+0000ef10: 2077 7261 7070 6572 206f 7665 7220 6060   wrapper over ``
+0000ef20: 6170 706c 7960 602c 2073 6f20 6f74 6865  apply``, so othe
+0000ef30: 7220 6060 6170 706c 7960 6020 6172 6775  r ``apply`` argu
+0000ef40: 6d65 6e74 7320 6c69 6b65 0a20 2020 2060  ments like.    `
+0000ef50: 606d 6574 686f 6460 602c 2060 606d 7574  `method``, ``mut
+0000ef60: 6162 6c65 6060 2c20 616e 6420 6060 6361  able``, and ``ca
+0000ef70: 7074 7572 655f 696e 7465 726d 6564 6961  pture_intermedia
+0000ef80: 7465 7360 6020 6172 6520 616c 736f 2061  tes`` are also a
+0000ef90: 7661 696c 6162 6c65 2e0a 0a20 2020 2041  vailable...    A
+0000efa0: 7267 733a 0a20 2020 2020 2072 6e67 733a  rgs:.      rngs:
+0000efb0: 2054 6865 2072 6e67 7320 666f 7220 7468   The rngs for th
+0000efc0: 6520 7661 7269 6162 6c65 2063 6f6c 6c65  e variable colle
+0000efd0: 6374 696f 6e73 2e0a 2020 2020 2020 2a61  ctions..      *a
+0000efe0: 7267 733a 204e 616d 6564 2061 7267 756d  rgs: Named argum
+0000eff0: 656e 7473 2070 6173 7365 6420 746f 2074  ents passed to t
+0000f000: 6865 2069 6e69 7420 6675 6e63 7469 6f6e  he init function
+0000f010: 2e0a 2020 2020 2020 6d65 7468 6f64 3a20  ..      method: 
+0000f020: 416e 206f 7074 696f 6e61 6c20 6d65 7468  An optional meth
+0000f030: 6f64 2e20 4966 2070 726f 7669 6465 642c  od. If provided,
+0000f040: 2061 7070 6c69 6573 2074 6869 7320 6d65   applies this me
+0000f050: 7468 6f64 2e20 4966 206e 6f74 0a20 2020  thod. If not.   
+0000f060: 2020 2020 2070 726f 7669 6465 642c 2061       provided, a
+0000f070: 7070 6c69 6573 2074 6865 2060 605f 5f63  pplies the ``__c
+0000f080: 616c 6c5f 5f60 6020 6d65 7468 6f64 2e20  all__`` method. 
+0000f090: 4120 7374 7269 6e67 2063 616e 2061 6c73  A string can als
+0000f0a0: 6f20 6265 0a20 2020 2020 2020 2070 726f  o be.        pro
+0000f0b0: 7669 6465 6420 746f 2073 7065 6369 6679  vided to specify
+0000f0c0: 2061 206d 6574 686f 6420 6279 206e 616d   a method by nam
+0000f0d0: 652e 0a20 2020 2020 206d 7574 6162 6c65  e..      mutable
+0000f0e0: 3a20 4361 6e20 6265 2062 6f6f 6c2c 2073  : Can be bool, s
+0000f0f0: 7472 2c20 6f72 206c 6973 742e 2053 7065  tr, or list. Spe
+0000f100: 6369 6669 6573 2077 6869 6368 2063 6f6c  cifies which col
+0000f110: 6c65 6374 696f 6e73 2073 686f 756c 6420  lections should 
+0000f120: 6265 0a20 2020 2020 2020 2074 7265 6174  be.        treat
+0000f130: 6564 2061 7320 6d75 7461 626c 653a 2060  ed as mutable: `
+0000f140: 6062 6f6f 6c60 603a 2061 6c6c 2f6e 6f20  `bool``: all/no 
+0000f150: 636f 6c6c 6563 7469 6f6e 7320 6172 6520  collections are 
+0000f160: 6d75 7461 626c 652e 0a20 2020 2020 2020  mutable..       
+0000f170: 2060 6073 7472 6060 3a20 5468 6520 6e61   ``str``: The na
+0000f180: 6d65 206f 6620 6120 7369 6e67 6c65 206d  me of a single m
+0000f190: 7574 6162 6c65 2063 6f6c 6c65 6374 696f  utable collectio
+0000f1a0: 6e2e 2060 606c 6973 7460 603a 2041 0a20  n. ``list``: A. 
+0000f1b0: 2020 2020 2020 206c 6973 7420 6f66 206e         list of n
+0000f1c0: 616d 6573 206f 6620 6d75 7461 626c 6520  ames of mutable 
+0000f1d0: 636f 6c6c 6563 7469 6f6e 732e 2042 7920  collections. By 
+0000f1e0: 6465 6661 756c 7420 616c 6c20 636f 6c6c  default all coll
+0000f1f0: 6563 7469 6f6e 730a 2020 2020 2020 2020  ections.        
+0000f200: 6578 6365 7074 2022 696e 7465 726d 6564  except "intermed
+0000f210: 6961 7465 7322 2061 7265 206d 7574 6162  iates" are mutab
+0000f220: 6c65 2e0a 2020 2020 2020 6361 7074 7572  le..      captur
+0000f230: 655f 696e 7465 726d 6564 6961 7465 733a  e_intermediates:
+0000f240: 2049 6620 6054 7275 6560 2c20 6361 7074   If `True`, capt
+0000f250: 7572 6573 2069 6e74 6572 6d65 6469 6174  ures intermediat
+0000f260: 6520 7265 7475 726e 2076 616c 7565 730a  e return values.
+0000f270: 2020 2020 2020 2020 6f66 2061 6c6c 204d          of all M
+0000f280: 6f64 756c 6573 2069 6e73 6964 6520 7468  odules inside th
+0000f290: 6520 2269 6e74 6572 6d65 6469 6174 6573  e "intermediates
+0000f2a0: 2220 636f 6c6c 6563 7469 6f6e 2e20 4279  " collection. By
+0000f2b0: 2064 6566 6175 6c74 206f 6e6c 790a 2020   default only.  
+0000f2c0: 2020 2020 2020 7468 6520 7265 7475 726e        the return
+0000f2d0: 2076 616c 7565 7320 6f66 2061 6c6c 2060   values of all `
+0000f2e0: 605f 5f63 616c 6c5f 5f60 6020 6d65 7468  `__call__`` meth
+0000f2f0: 6f64 7320 6172 6520 7374 6f72 6564 2e20  ods are stored. 
+0000f300: 4120 6675 6e63 7469 6f6e 2063 616e 0a20  A function can. 
+0000f310: 2020 2020 2020 2062 6520 7061 7373 6564         be passed
+0000f320: 2074 6f20 6368 616e 6765 2074 6865 2066   to change the f
+0000f330: 696c 7465 7220 6265 6861 7669 6f72 2e20  ilter behavior. 
+0000f340: 5468 6520 6669 6c74 6572 2066 756e 6374  The filter funct
+0000f350: 696f 6e20 7461 6b65 730a 2020 2020 2020  ion takes.      
+0000f360: 2020 7468 6520 4d6f 6475 6c65 2069 6e73    the Module ins
+0000f370: 7461 6e63 6520 616e 6420 6d65 7468 6f64  tance and method
+0000f380: 206e 616d 6520 616e 6420 7265 7475 726e   name and return
+0000f390: 7320 6120 626f 6f6c 2069 6e64 6963 6174  s a bool indicat
+0000f3a0: 696e 670a 2020 2020 2020 2020 7768 6574  ing.        whet
+0000f3b0: 6865 7220 7468 6520 6f75 7470 7574 206f  her the output o
+0000f3c0: 6620 7468 6174 206d 6574 686f 6420 696e  f that method in
+0000f3d0: 766f 6361 7469 6f6e 2073 686f 756c 6420  vocation should 
+0000f3e0: 6265 2073 746f 7265 642e 0a20 2020 2020  be stored..     
+0000f3f0: 202a 2a6b 7761 7267 733a 204b 6579 776f   **kwargs: Keywo
+0000f400: 7264 2061 7267 756d 656e 7473 2070 6173  rd arguments pas
+0000f410: 7365 6420 746f 2074 6865 2069 6e69 7420  sed to the init 
+0000f420: 6675 6e63 7469 6f6e 2e0a 2020 2020 5265  function..    Re
+0000f430: 7475 726e 733a 0a20 2020 2020 2054 6865  turns:.      The
+0000f440: 2069 6e69 7469 616c 697a 6564 2076 6172   initialized var
+0000f450: 6961 626c 6520 6469 6374 2e0a 2020 2020  iable dict..    
+0000f460: 2222 220a 2020 2020 4d6f 6475 6c65 2e5f  """.    Module._
+0000f470: 6d6f 6475 6c65 5f63 6865 636b 7328 7365  module_checks(se
+0000f480: 6c66 290a 0a20 2020 205f 2c20 765f 6f75  lf)..    _, v_ou
+0000f490: 7420 3d20 7365 6c66 2e69 6e69 745f 7769  t = self.init_wi
+0000f4a0: 7468 5f6f 7574 7075 7428 0a20 2020 2020  th_output(.     
+0000f4b0: 2020 2072 6e67 732c 0a20 2020 2020 2020     rngs,.       
+0000f4c0: 202a 6172 6773 2c0a 2020 2020 2020 2020   *args,.        
+0000f4d0: 6d65 7468 6f64 3d6d 6574 686f 642c 0a20  method=method,. 
+0000f4e0: 2020 2020 2020 206d 7574 6162 6c65 3d6d         mutable=m
+0000f4f0: 7574 6162 6c65 2c0a 2020 2020 2020 2020  utable,.        
+0000f500: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
+0000f510: 6961 7465 733d 6361 7074 7572 655f 696e  iates=capture_in
+0000f520: 7465 726d 6564 6961 7465 732c 0a20 2020  termediates,.   
+0000f530: 2020 2020 202a 2a6b 7761 7267 7329 0a20       **kwargs). 
+0000f540: 2020 2072 6574 7572 6e20 765f 6f75 740a     return v_out.
+0000f550: 0a20 2040 7472 6163 6562 6163 6b5f 7574  .  @traceback_ut
+0000f560: 696c 2e61 7069 5f62 6f75 6e64 6172 790a  il.api_boundary.
+0000f570: 2020 6465 6620 6c61 7a79 5f69 6e69 7428    def lazy_init(
+0000f580: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+0000f590: 2072 6e67 733a 2055 6e69 6f6e 5b50 524e   rngs: Union[PRN
+0000f5a0: 474b 6579 2c20 524e 4753 6571 7565 6e63  GKey, RNGSequenc
+0000f5b0: 6573 5d2c 0a20 2020 2020 2020 2020 2020  es],.           
+0000f5c0: 2a61 7267 732c 0a20 2020 2020 2020 2020  *args,.         
+0000f5d0: 2020 6d65 7468 6f64 3a20 4f70 7469 6f6e    method: Option
+0000f5e0: 616c 5b43 616c 6c61 626c 655b 2e2e 2e2c  al[Callable[...,
+0000f5f0: 2041 6e79 5d5d 203d 204e 6f6e 652c 0a20   Any]] = None,. 
+0000f600: 2020 2020 2020 2020 2020 6d75 7461 626c            mutabl
+0000f610: 653a 2043 6f6c 6c65 6374 696f 6e46 696c  e: CollectionFil
+0000f620: 7465 7220 3d20 4465 6e79 4c69 7374 2827  ter = DenyList('
+0000f630: 696e 7465 726d 6564 6961 7465 7327 292c  intermediates'),
+0000f640: 0a20 2020 2020 2020 2020 2020 2a2a 6b77  .           **kw
+0000f650: 6172 6773 2920 2d3e 2046 726f 7a65 6e56  args) -> FrozenV
+0000f660: 6172 6961 626c 6544 6963 743a 0a20 2020  ariableDict:.   
+0000f670: 2022 2222 496e 6974 6961 6c69 7a65 7320   """Initializes 
+0000f680: 6120 6d6f 6475 6c65 2077 6974 686f 7574  a module without
+0000f690: 2063 6f6d 7075 7469 6e67 206f 6e20 616e   computing on an
+0000f6a0: 2061 6374 7561 6c20 696e 7075 742e 0a0a   actual input...
+0000f6b0: 2020 2020 6c61 7a79 5f69 6e69 7420 7769      lazy_init wi
+0000f6c0: 6c6c 2069 6e69 7469 616c 697a 6520 7468  ll initialize th
+0000f6d0: 6520 7661 7269 6162 6c65 7320 7769 7468  e variables with
+0000f6e0: 6f75 7420 646f 696e 6720 756e 6e65 6365  out doing unnece
+0000f6f0: 7373 6172 7920 636f 6d70 7574 652e 0a20  ssary compute.. 
+0000f700: 2020 2054 6865 2069 6e70 7574 2064 6174     The input dat
+0000f710: 6120 7368 6f75 6c64 2062 6520 7061 7373  a should be pass
+0000f720: 6564 2061 7320 6120 6060 6a61 782e 5368  ed as a ``jax.Sh
+0000f730: 6170 6544 7479 7065 5374 7275 6374 6060  apeDtypeStruct``
+0000f740: 2077 6869 6368 2073 7065 6369 6669 6573   which specifies
+0000f750: 0a20 2020 2074 6865 2073 6861 7065 2061  .    the shape a
+0000f760: 6e64 2064 7479 7065 206f 6620 7468 6520  nd dtype of the 
+0000f770: 696e 7075 7420 6275 7420 6e6f 2063 6f6e  input but no con
+0000f780: 6372 6574 6520 6461 7461 2e0a 0a20 2020  crete data...   
+0000f790: 2045 7861 6d70 6c65 3a3a 0a0a 2020 2020   Example::..    
+0000f7a0: 2020 6d6f 6465 6c20 3d20 6e6e 2e44 656e    model = nn.Den
+0000f7b0: 7365 2866 6561 7475 7265 733d 3235 3629  se(features=256)
+0000f7c0: 0a20 2020 2020 2076 6172 6961 626c 6573  .      variables
+0000f7d0: 203d 206d 6f64 656c 2e6c 617a 795f 696e   = model.lazy_in
+0000f7e0: 6974 2872 6e67 2c20 6a61 782e 5368 6170  it(rng, jax.Shap
+0000f7f0: 6544 7479 7065 5374 7275 6374 2828 312c  eDtypeStruct((1,
+0000f800: 2031 3238 292c 206a 6e70 2e66 6c6f 6174   128), jnp.float
+0000f810: 3332 2929 0a0a 2020 2020 5468 6520 6172  32))..    The ar
+0000f820: 6773 2061 6e64 206b 7761 7267 7320 6172  gs and kwargs ar
+0000f830: 6773 2070 6173 7365 6420 746f 2060 606c  gs passed to ``l
+0000f840: 617a 795f 696e 6974 6060 2063 616e 2062  azy_init`` can b
+0000f850: 6520 6120 6d69 7820 6f66 0a20 2020 2063  e a mix of.    c
+0000f860: 6f6e 6372 6574 6520 286a 6178 2061 7272  oncrete (jax arr
+0000f870: 6179 732c 2073 6361 6c61 7273 2c20 626f  ays, scalars, bo
+0000f880: 6f6c 7329 2061 6e64 2061 6273 7472 6163  ols) and abstrac
+0000f890: 7420 2853 6861 7065 4474 7970 6553 7472  t (ShapeDtypeStr
+0000f8a0: 7563 7429 2076 616c 7565 732e 0a20 2020  uct) values..   
+0000f8b0: 2043 6f6e 6372 6574 6520 7661 6c75 6573   Concrete values
+0000f8c0: 2061 7265 206f 6e6c 7920 6e65 6365 7373   are only necess
+0000f8d0: 6172 7920 666f 7220 6172 6775 6d65 6e74  ary for argument
+0000f8e0: 7320 7468 6174 2061 6666 6563 740a 2020  s that affect.  
+0000f8f0: 2020 7468 6520 696e 6974 6961 6c69 7a61    the initializa
+0000f900: 7469 6f6e 206f 6620 7661 7269 6162 6c65  tion of variable
+0000f910: 732e 2046 6f72 2065 7861 6d70 6c65 2c20  s. For example, 
+0000f920: 7468 6520 6d6f 6465 6c20 6d69 6768 7420  the model might 
+0000f930: 6578 7065 6374 0a20 2020 2061 206b 6579  expect.    a key
+0000f940: 776f 7264 2061 7267 2074 6861 7420 656e  word arg that en
+0000f950: 6162 6c65 732f 6469 7361 626c 6573 2061  ables/disables a
+0000f960: 2073 7562 7061 7274 206f 6620 7468 6520   subpart of the 
+0000f970: 6d6f 6465 6c2e 0a20 2020 2049 6e20 7468  model..    In th
+0000f980: 6973 2063 6173 652c 2061 6e20 6578 706c  is case, an expl
+0000f990: 6963 6974 2076 616c 7565 2028 5472 7565  icit value (True
+0000f9a0: 2f46 6c61 7365 2920 7368 6f75 6c64 2062  /Flase) should b
+0000f9b0: 6520 7061 7373 6564 206f 7468 6572 7769  e passed otherwi
+0000f9c0: 7365 0a20 2020 2060 606c 617a 795f 696e  se.    ``lazy_in
+0000f9d0: 6974 6060 2063 616e 6e6f 7420 696e 6665  it`` cannot infe
+0000f9e0: 7220 7768 6963 6820 7661 7269 6162 6c65  r which variable
+0000f9f0: 7320 7368 6f75 6c64 2062 6520 696e 6974  s should be init
+0000fa00: 6961 6c69 7a65 642e 0a0a 2020 2020 4172  ialized...    Ar
+0000fa10: 6773 3a0a 2020 2020 2020 726e 6773 3a20  gs:.      rngs: 
+0000fa20: 5468 6520 726e 6773 2066 6f72 2074 6865  The rngs for the
+0000fa30: 2076 6172 6961 626c 6520 636f 6c6c 6563   variable collec
+0000fa40: 7469 6f6e 732e 0a20 2020 2020 202a 6172  tions..      *ar
+0000fa50: 6773 3a20 6172 6775 6d65 6e74 7320 7061  gs: arguments pa
+0000fa60: 7373 6564 2074 6f20 7468 6520 696e 6974  ssed to the init
+0000fa70: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
+0000fa80: 206d 6574 686f 643a 2041 6e20 6f70 7469   method: An opti
+0000fa90: 6f6e 616c 206d 6574 686f 642e 2049 6620  onal method. If 
+0000faa0: 7072 6f76 6964 6564 2c20 6170 706c 6965  provided, applie
+0000fab0: 7320 7468 6973 206d 6574 686f 642e 2049  s this method. I
+0000fac0: 6620 6e6f 740a 2020 2020 2020 2020 7072  f not.        pr
+0000fad0: 6f76 6964 6564 2c20 6170 706c 6965 7320  ovided, applies 
+0000fae0: 7468 6520 6060 5f5f 6361 6c6c 5f5f 6060  the ``__call__``
+0000faf0: 206d 6574 686f 642e 0a20 2020 2020 206d   method..      m
+0000fb00: 7574 6162 6c65 3a20 4361 6e20 6265 2062  utable: Can be b
+0000fb10: 6f6f 6c2c 2073 7472 2c20 6f72 206c 6973  ool, str, or lis
+0000fb20: 742e 2053 7065 6369 6669 6573 2077 6869  t. Specifies whi
+0000fb30: 6368 2063 6f6c 6c65 6374 696f 6e73 2073  ch collections s
+0000fb40: 686f 756c 6420 6265 0a20 2020 2020 2020  hould be.       
+0000fb50: 2074 7265 6174 6564 2061 7320 6d75 7461   treated as muta
+0000fb60: 626c 653a 2060 6062 6f6f 6c60 603a 2061  ble: ``bool``: a
+0000fb70: 6c6c 2f6e 6f20 636f 6c6c 6563 7469 6f6e  ll/no collection
+0000fb80: 7320 6172 6520 6d75 7461 626c 652e 0a20  s are mutable.. 
+0000fb90: 2020 2020 2020 2060 6073 7472 6060 3a20         ``str``: 
+0000fba0: 5468 6520 6e61 6d65 206f 6620 6120 7369  The name of a si
+0000fbb0: 6e67 6c65 206d 7574 6162 6c65 2063 6f6c  ngle mutable col
+0000fbc0: 6c65 6374 696f 6e2e 2060 606c 6973 7460  lection. ``list`
+0000fbd0: 603a 2041 0a20 2020 2020 2020 206c 6973  `: A.        lis
+0000fbe0: 7420 6f66 206e 616d 6573 206f 6620 6d75  t of names of mu
+0000fbf0: 7461 626c 6520 636f 6c6c 6563 7469 6f6e  table collection
+0000fc00: 732e 2042 7920 6465 6661 756c 7420 616c  s. By default al
+0000fc10: 6c20 636f 6c6c 6563 7469 6f6e 730a 2020  l collections.  
+0000fc20: 2020 2020 2020 6578 6365 7074 2022 696e        except "in
+0000fc30: 7465 726d 6564 6961 7465 7322 2061 7265  termediates" are
+0000fc40: 206d 7574 6162 6c65 2e0a 2020 2020 2020   mutable..      
+0000fc50: 2a2a 6b77 6172 6773 3a20 4b65 7977 6f72  **kwargs: Keywor
+0000fc60: 6420 6172 6775 6d65 6e74 7320 7061 7373  d arguments pass
+0000fc70: 6564 2074 6f20 7468 6520 696e 6974 2066  ed to the init f
+0000fc80: 756e 6374 696f 6e2e 0a20 2020 2052 6574  unction..    Ret
+0000fc90: 7572 6e73 3a0a 2020 2020 2020 5468 6520  urns:.      The 
+0000fca0: 696e 6974 6961 6c69 7a65 6420 7661 7269  initialized vari
+0000fcb0: 6162 6c65 2064 6963 742e 0a20 2020 2022  able dict..    "
+0000fcc0: 2222 0a20 2020 204d 6f64 756c 652e 5f6d  "".    Module._m
+0000fcd0: 6f64 756c 655f 6368 6563 6b73 2873 656c  odule_checks(sel
+0000fce0: 6629 0a20 2020 2064 6566 206c 617a 795f  f).    def lazy_
+0000fcf0: 7772 6170 7065 7228 726e 6773 2c20 2a61  wrapper(rngs, *a
+0000fd00: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+0000fd10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000fd20: 662e 696e 6974 2872 6e67 732c 202a 6172  f.init(rngs, *ar
+0000fd30: 6773 2c20 6d65 7468 6f64 3d6d 6574 686f  gs, method=metho
+0000fd40: 642c 206d 7574 6162 6c65 3d6d 7574 6162  d, mutable=mutab
+0000fd50: 6c65 2c20 2a2a 6b77 6172 6773 290a 2020  le, **kwargs).  
+0000fd60: 2020 7265 7475 726e 2070 6172 7469 616c    return partial
+0000fd70: 5f65 7661 6c2e 6c61 7a79 5f69 6e69 7428  _eval.lazy_init(
+0000fd80: 6c61 7a79 5f77 7261 7070 6572 2928 726e  lazy_wrapper)(rn
+0000fd90: 6773 2c20 2a61 7267 732c 202a 2a6b 7761  gs, *args, **kwa
+0000fda0: 7267 7329 0a0a 2020 4070 726f 7065 7274  rgs)..  @propert
+0000fdb0: 790a 2020 6465 6620 7661 7269 6162 6c65  y.  def variable
+0000fdc0: 7328 7365 6c66 2920 2d3e 2056 6172 6961  s(self) -> Varia
+0000fdd0: 626c 6544 6963 743a 0a20 2020 2022 2222  bleDict:.    """
+0000fde0: 5265 7475 726e 7320 7468 6520 7661 7269  Returns the vari
+0000fdf0: 6162 6c65 7320 696e 2074 6869 7320 6d6f  ables in this mo
+0000fe00: 6475 6c65 2e22 2222 0a20 2020 2069 6620  dule.""".    if 
+0000fe10: 7365 6c66 2e73 636f 7065 2069 7320 4e6f  self.scope is No
+0000fe20: 6e65 3a0a 2020 2020 2020 7261 6973 6520  ne:.      raise 
+0000fe30: 5661 6c75 6545 7272 6f72 2822 4361 6e27  ValueError("Can'
+0000fe40: 7420 6163 6365 7373 2076 6172 6961 626c  t access variabl
+0000fe50: 6573 206f 6e20 756e 626f 756e 6420 6d6f  es on unbound mo
+0000fe60: 6475 6c65 7322 290a 2020 2020 7265 7475  dules").    retu
+0000fe70: 726e 2073 656c 662e 7363 6f70 652e 7661  rn self.scope.va
+0000fe80: 7269 6162 6c65 7328 290a 0a20 2064 6566  riables()..  def
+0000fe90: 2067 6574 5f76 6172 6961 626c 6528 7365   get_variable(se
+0000fea0: 6c66 2c20 636f 6c3a 2073 7472 2c20 6e61  lf, col: str, na
+0000feb0: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
+0000fec0: 3a20 4f70 7469 6f6e 616c 5b54 5d20 3d20  : Optional[T] = 
+0000fed0: 4e6f 6e65 2920 2d3e 2054 3a0a 2020 2020  None) -> T:.    
+0000fee0: 2222 2252 6574 7269 6576 6573 2074 6865  """Retrieves the
+0000fef0: 2076 616c 7565 206f 6620 6120 5661 7269   value of a Vari
+0000ff00: 6162 6c65 2e0a 0a20 2020 2041 7267 733a  able...    Args:
+0000ff10: 0a20 2020 2020 2063 6f6c 3a20 7468 6520  .      col: the 
+0000ff20: 7661 7269 6162 6c65 2063 6f6c 6c65 6374  variable collect
+0000ff30: 696f 6e2e 0a20 2020 2020 206e 616d 653a  ion..      name:
+0000ff40: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+0000ff50: 2076 6172 6961 626c 652e 0a20 2020 2020   variable..     
+0000ff60: 2064 6566 6175 6c74 3a20 7468 6520 6465   default: the de
+0000ff70: 6661 756c 7420 7661 6c75 6520 746f 2072  fault value to r
+0000ff80: 6574 7572 6e20 6966 2074 6865 2076 6172  eturn if the var
+0000ff90: 6961 626c 6520 646f 6573 206e 6f74 2065  iable does not e
+0000ffa0: 7869 7374 2069 6e0a 2020 2020 2020 2020  xist in.        
+0000ffb0: 7468 6973 2073 636f 7065 2e0a 0a20 2020  this scope...   
+0000ffc0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000ffd0: 5468 6520 7661 6c75 6520 6f66 2074 6865  The value of the
+0000ffe0: 2069 6e70 7574 2076 6172 6961 626c 652c   input variable,
+0000fff0: 206f 6620 7468 6520 6465 6661 756c 7420   of the default 
+00010000: 7661 6c75 6520 6966 2074 6865 2076 6172  value if the var
+00010010: 6961 626c 650a 2020 2020 2020 646f 6573  iable.      does
+00010020: 6e27 7420 6578 6973 7420 696e 2074 6869  n't exist in thi
+00010030: 7320 7363 6f70 652e 0a20 2020 2022 2222  s scope..    """
+00010040: 0a20 2020 2069 6620 7365 6c66 2e73 636f  .    if self.sco
+00010050: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+00010060: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00010070: 6f72 2822 4361 6e27 7420 6163 6365 7373  or("Can't access
+00010080: 2076 6172 6961 626c 6573 206f 6e20 756e   variables on un
+00010090: 626f 756e 6420 6d6f 6475 6c65 7322 290a  bound modules").
+000100a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000100b0: 7363 6f70 652e 6765 745f 7661 7269 6162  scope.get_variab
+000100c0: 6c65 2863 6f6c 2c20 6e61 6d65 2c20 6465  le(col, name, de
+000100d0: 6661 756c 7429 0a0a 2020 6465 6620 7075  fault)..  def pu
+000100e0: 745f 7661 7269 6162 6c65 2873 656c 662c  t_variable(self,
+000100f0: 2063 6f6c 3a20 7374 722c 206e 616d 653a   col: str, name:
+00010100: 2073 7472 2c20 7661 6c75 653a 2041 6e79   str, value: Any
+00010110: 293a 0a20 2020 2022 2222 5570 6461 7465  ):.    """Update
+00010120: 7320 7468 6520 7661 6c75 6520 6f66 2074  s the value of t
+00010130: 6865 2067 6976 656e 2076 6172 6961 626c  he given variabl
+00010140: 6520 6966 2069 7420 6973 206d 7574 6162  e if it is mutab
+00010150: 6c65 2c20 6f72 2061 6e20 6572 726f 7220  le, or an error 
+00010160: 6f74 6865 7277 6973 652e 0a0a 2020 2020  otherwise...    
+00010170: 4172 6773 3a0a 2020 2020 2020 636f 6c3a  Args:.      col:
+00010180: 2074 6865 2076 6172 6961 626c 6520 636f   the variable co
+00010190: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
+000101a0: 6e61 6d65 3a20 7468 6520 6e61 6d65 206f  name: the name o
+000101b0: 6620 7468 6520 7661 7269 6162 6c65 2e0a  f the variable..
+000101c0: 2020 2020 2020 7661 6c75 653a 2074 6865        value: the
+000101d0: 206e 6577 2076 616c 7565 206f 6620 7468   new value of th
+000101e0: 6520 7661 7269 6162 6c65 2e0a 2020 2020  e variable..    
+000101f0: 2222 220a 2020 2020 6966 2073 656c 662e  """.    if self.
+00010200: 7363 6f70 6520 6973 204e 6f6e 653a 0a20  scope is None:. 
+00010210: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00010220: 4572 726f 7228 2243 616e 2774 2061 6363  Error("Can't acc
+00010230: 6573 7320 7661 7269 6162 6c65 7320 6f6e  ess variables on
+00010240: 2075 6e62 6f75 6e64 206d 6f64 756c 6573   unbound modules
+00010250: 2229 0a20 2020 2073 656c 662e 7363 6f70  ").    self.scop
+00010260: 652e 7075 745f 7661 7269 6162 6c65 2863  e.put_variable(c
+00010270: 6f6c 2c20 6e61 6d65 2c20 7661 6c75 6529  ol, name, value)
+00010280: 0a0a 2020 406f 7665 726c 6f61 640a 2020  ..  @overload.  
+00010290: 6465 6620 736f 7728 7365 6c66 2c20 636f  def sow(self, co
+000102a0: 6c3a 2073 7472 2c20 6e61 6d65 3a20 7374  l: str, name: st
+000102b0: 722c 2076 616c 7565 3a20 416e 7929 202d  r, value: Any) -
+000102c0: 3e20 626f 6f6c 3a0a 2020 2020 2e2e 2e0a  > bool:.    ....
+000102d0: 0a20 2040 6f76 6572 6c6f 6164 0a20 2064  .  @overload.  d
+000102e0: 6566 2073 6f77 2873 656c 662c 2063 6f6c  ef sow(self, col
+000102f0: 3a20 7374 722c 206e 616d 653a 2073 7472  : str, name: str
+00010300: 2c20 7661 6c75 653a 2054 2c0a 2020 2020  , value: T,.    
+00010310: 2020 2020 2020 7265 6475 6365 5f66 6e3a        reduce_fn:
+00010320: 2043 616c 6c61 626c 655b 5b4b 2c20 545d   Callable[[K, T]
+00010330: 2c20 4b5d 203d 2074 7570 6c65 5f72 6564  , K] = tuple_red
+00010340: 7563 652c 0a20 2020 2020 2020 2020 2069  uce,.          i
+00010350: 6e69 745f 666e 3a20 4361 6c6c 6162 6c65  nit_fn: Callable
+00010360: 5b5b 5d2c 204b 5d20 3d20 7475 706c 655f  [[], K] = tuple_
+00010370: 696e 6974 2920 2d3e 2062 6f6f 6c3a 2023  init) -> bool: #
+00010380: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
+00010390: 2020 2e2e 2e0a 0a20 2064 6566 2073 6f77    .....  def sow
+000103a0: 2873 656c 662c 2063 6f6c 3a20 7374 722c  (self, col: str,
+000103b0: 206e 616d 653a 2073 7472 2c20 7661 6c75   name: str, valu
+000103c0: 653a 2054 2c0a 2020 2020 2020 2020 2020  e: T,.          
+000103d0: 7265 6475 6365 5f66 6e3a 2043 616c 6c61  reduce_fn: Calla
+000103e0: 626c 655b 5b4b 2c20 545d 2c20 4b5d 203d  ble[[K, T], K] =
+000103f0: 2074 7570 6c65 5f72 6564 7563 652c 0a20   tuple_reduce,. 
+00010400: 2020 2020 2020 2020 2069 6e69 745f 666e           init_fn
+00010410: 3a20 4361 6c6c 6162 6c65 5b5b 5d2c 204b  : Callable[[], K
+00010420: 5d20 3d20 7475 706c 655f 696e 6974 2920  ] = tuple_init) 
+00010430: 2d3e 2062 6f6f 6c3a 2023 2074 7970 653a  -> bool: # type:
+00010440: 2069 676e 6f72 650a 2020 2020 2222 2253   ignore.    """S
+00010450: 746f 7265 7320 6120 7661 6c75 6520 696e  tores a value in
+00010460: 2061 2063 6f6c 6c65 6374 696f 6e2e 0a0a   a collection...
+00010470: 2020 2020 436f 6c6c 6563 7469 6f6e 7320      Collections 
+00010480: 6361 6e20 6265 2075 7365 6420 746f 2063  can be used to c
+00010490: 6f6c 6c65 6374 2069 6e74 6572 6d65 6469  ollect intermedi
+000104a0: 6174 6520 7661 6c75 6573 2077 6974 686f  ate values witho
+000104b0: 7574 0a20 2020 2074 6865 206f 7665 7268  ut.    the overh
+000104c0: 6561 6420 6f66 2065 7870 6c69 6369 746c  ead of explicitl
+000104d0: 7920 7061 7373 696e 6720 6120 636f 6e74  y passing a cont
+000104e0: 6169 6e65 7220 7468 726f 7567 6820 6561  ainer through ea
+000104f0: 6368 204d 6f64 756c 6520 6361 6c6c 2e0a  ch Module call..
+00010500: 0a20 2020 2049 6620 7468 6520 7461 7267  .    If the targ
+00010510: 6574 2063 6f6c 6c65 6374 696f 6e20 6973  et collection is
+00010520: 206e 6f74 206d 7574 6162 6c65 2060 736f   not mutable `so
+00010530: 7760 2062 6568 6176 6573 206c 696b 6520  w` behaves like 
+00010540: 6120 6e6f 2d6f 700a 2020 2020 616e 6420  a no-op.    and 
+00010550: 7265 7475 726e 7320 6046 616c 7365 602e  returns `False`.
+00010560: 0a0a 2020 2020 4578 616d 706c 653a 3a0a  ..    Example::.
+00010570: 0a20 2020 2020 2069 6d70 6f72 7420 6a61  .      import ja
+00010580: 780a 2020 2020 2020 696d 706f 7274 206a  x.      import j
+00010590: 6178 2e6e 756d 7079 2061 7320 6a6e 700a  ax.numpy as jnp.
+000105a0: 2020 2020 2020 696d 706f 7274 2066 6c61        import fla
+000105b0: 782e 6c69 6e65 6e20 6173 206e 6e0a 0a20  x.linen as nn.. 
+000105c0: 2020 2020 2063 6c61 7373 2046 6f6f 286e       class Foo(n
+000105d0: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2020  n.Module):.     
+000105e0: 2020 2040 6e6e 2e63 6f6d 7061 6374 0a20     @nn.compact. 
+000105f0: 2020 2020 2020 2064 6566 205f 5f63 616c         def __cal
+00010600: 6c5f 5f28 7365 6c66 2c20 7829 3a0a 2020  l__(self, x):.  
+00010610: 2020 2020 2020 2020 6820 3d20 6e6e 2e44          h = nn.D
+00010620: 656e 7365 2834 2928 7829 0a20 2020 2020  ense(4)(x).     
+00010630: 2020 2020 2073 656c 662e 736f 7728 2769       self.sow('i
+00010640: 6e74 6572 6d65 6469 6174 6573 272c 2027  ntermediates', '
+00010650: 6827 2c20 6829 0a20 2020 2020 2020 2020  h', h).         
+00010660: 2072 6574 7572 6e20 6e6e 2e44 656e 7365   return nn.Dense
+00010670: 2832 2928 6829 0a0a 2020 2020 2020 7820  (2)(h)..      x 
+00010680: 3d20 6a6e 702e 6f6e 6573 2828 3136 2c20  = jnp.ones((16, 
+00010690: 3929 290a 2020 2020 2020 6d6f 6465 6c20  9)).      model 
+000106a0: 3d20 466f 6f28 290a 2020 2020 2020 7661  = Foo().      va
+000106b0: 7269 6162 6c65 7320 3d20 6d6f 6465 6c2e  riables = model.
+000106c0: 696e 6974 286a 6178 2e72 616e 646f 6d2e  init(jax.random.
+000106d0: 5052 4e47 4b65 7928 3029 2c20 7829 0a20  PRNGKey(0), x). 
+000106e0: 2020 2020 2079 2c20 7374 6174 6520 3d20       y, state = 
+000106f0: 6d6f 6465 6c2e 6170 706c 7928 7661 7269  model.apply(vari
+00010700: 6162 6c65 732c 2078 2c20 6d75 7461 626c  ables, x, mutabl
+00010710: 653d 5b27 696e 7465 726d 6564 6961 7465  e=['intermediate
+00010720: 7327 5d29 0a20 2020 2020 2070 7269 6e74  s']).      print
+00010730: 2873 7461 7465 5b27 696e 7465 726d 6564  (state['intermed
+00010740: 6961 7465 7327 5d29 2020 2320 7b27 6827  iates'])  # {'h'
+00010750: 3a20 282e 2e2e 2c29 7d0a 0a20 2020 2042  : (...,)}..    B
+00010760: 7920 6465 6661 756c 7420 7468 6520 7661  y default the va
+00010770: 6c75 6573 2061 7265 2073 746f 7265 6420  lues are stored 
+00010780: 696e 2061 2074 7570 6c65 2061 6e64 2065  in a tuple and e
+00010790: 6163 6820 7374 6f72 6564 2076 616c 7565  ach stored value
+000107a0: 0a20 2020 2069 7320 6170 7065 6e64 6564  .    is appended
+000107b0: 2061 7420 7468 6520 656e 642e 2054 6869   at the end. Thi
+000107c0: 7320 7761 7920 616c 6c20 696e 7465 726d  s way all interm
+000107d0: 6564 6961 7465 7320 6361 6e20 6265 2074  ediates can be t
+000107e0: 7261 636b 6564 2077 6865 6e0a 2020 2020  racked when.    
+000107f0: 7468 6520 7361 6d65 206d 6f64 756c 6520  the same module 
+00010800: 6973 2063 616c 6c65 6420 6d75 6c74 6970  is called multip
+00010810: 6c65 2074 696d 6573 2e20 416c 7465 726e  le times. Altern
+00010820: 6174 6976 656c 792c 2061 2063 7573 746f  atively, a custo
+00010830: 6d0a 2020 2020 696e 6974 2f72 6564 7563  m.    init/reduc
+00010840: 6520 6675 6e63 7469 6f6e 2063 616e 2062  e function can b
+00010850: 6520 7061 7373 6564 3a3a 0a0a 2020 2020  e passed::..    
+00010860: 2020 636c 6173 7320 466f 6f32 286e 6e2e    class Foo2(nn.
+00010870: 4d6f 6475 6c65 293a 0a20 2020 2020 2020  Module):.       
+00010880: 2040 6e6e 2e63 6f6d 7061 6374 0a20 2020   @nn.compact.   
+00010890: 2020 2020 2064 6566 205f 5f63 616c 6c5f       def __call_
+000108a0: 5f28 7365 6c66 2c20 7829 3a0a 2020 2020  _(self, x):.    
+000108b0: 2020 2020 2020 696e 6974 5f66 6e20 3d20        init_fn = 
+000108c0: 6c61 6d62 6461 3a20 300a 2020 2020 2020  lambda: 0.      
+000108d0: 2020 2020 7265 6475 6365 5f66 6e20 3d20      reduce_fn = 
+000108e0: 6c61 6d62 6461 2061 2c20 623a 2061 202b  lambda a, b: a +
+000108f0: 2062 0a20 2020 2020 2020 2020 2073 656c   b.          sel
+00010900: 662e 736f 7728 2769 6e74 6572 6d65 6469  f.sow('intermedi
+00010910: 6174 6573 272c 2027 6827 2c20 782c 0a20  ates', 'h', x,. 
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 696e 6974 5f66 6e3d 696e 6974 5f66    init_fn=init_f
+00010940: 6e2c 2072 6564 7563 655f 666e 3d72 6564  n, reduce_fn=red
+00010950: 7563 655f 666e 290a 2020 2020 2020 2020  uce_fn).        
+00010960: 2020 7365 6c66 2e73 6f77 2827 696e 7465    self.sow('inte
+00010970: 726d 6564 6961 7465 7327 2c20 2768 272c  rmediates', 'h',
+00010980: 2078 202a 2032 2c0a 2020 2020 2020 2020   x * 2,.        
+00010990: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
+000109a0: 666e 3d69 6e69 745f 666e 2c20 7265 6475  fn=init_fn, redu
+000109b0: 6365 5f66 6e3d 7265 6475 6365 5f66 6e29  ce_fn=reduce_fn)
+000109c0: 0a20 2020 2020 2020 2020 2072 6574 7572  .          retur
+000109d0: 6e20 780a 0a20 2020 2020 206d 6f64 656c  n x..      model
+000109e0: 203d 2046 6f6f 3228 290a 2020 2020 2020   = Foo2().      
+000109f0: 7661 7269 6162 6c65 7320 3d20 6d6f 6465  variables = mode
+00010a00: 6c2e 696e 6974 286a 6178 2e72 616e 646f  l.init(jax.rando
+00010a10: 6d2e 5052 4e47 4b65 7928 3029 2c20 7829  m.PRNGKey(0), x)
+00010a20: 0a20 2020 2020 2079 2c20 7374 6174 6520  .      y, state 
+00010a30: 3d20 6d6f 6465 6c2e 6170 706c 7928 7661  = model.apply(va
+00010a40: 7269 6162 6c65 732c 206a 6e70 2e6f 6e65  riables, jnp.one
+00010a50: 7328 2831 2c20 3129 292c 206d 7574 6162  s((1, 1)), mutab
+00010a60: 6c65 3d5b 2769 6e74 6572 6d65 6469 6174  le=['intermediat
+00010a70: 6573 275d 290a 2020 2020 2020 7072 696e  es']).      prin
+00010a80: 7428 7374 6174 655b 2769 6e74 6572 6d65  t(state['interme
+00010a90: 6469 6174 6573 275d 2920 2023 203d 3d3e  diates'])  # ==>
+00010aa0: 207b 2768 273a 205b 5b33 2e5d 5d7d 0a0a   {'h': [[3.]]}..
+00010ab0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00010ac0: 636f 6c3a 2054 6865 206e 616d 6520 6f66  col: The name of
+00010ad0: 2074 6865 2076 6172 6961 626c 6520 636f   the variable co
+00010ae0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
+00010af0: 6e61 6d65 3a20 5468 6520 6e61 6d65 206f  name: The name o
+00010b00: 6620 7468 6520 7661 7269 6162 6c65 2e0a  f the variable..
+00010b10: 2020 2020 2020 7661 6c75 653a 2054 6865        value: The
+00010b20: 2076 616c 7565 206f 6620 7468 6520 7661   value of the va
+00010b30: 7269 6162 6c65 2e0a 2020 2020 2020 7265  riable..      re
+00010b40: 6475 6365 5f66 6e3a 2054 6865 2066 756e  duce_fn: The fun
+00010b50: 6374 696f 6e20 7573 6564 2074 6f20 636f  ction used to co
+00010b60: 6d62 696e 6520 7468 6520 6578 6973 7469  mbine the existi
+00010b70: 6e67 2076 616c 7565 2077 6974 680a 2020  ng value with.  
+00010b80: 2020 2020 2020 7468 6520 6e65 7720 7661        the new va
+00010b90: 6c75 652e 2054 6865 2064 6566 6175 6c74  lue. The default
+00010ba0: 2069 7320 746f 2061 7070 656e 6420 7468   is to append th
+00010bb0: 6520 7661 6c75 6520 746f 2061 2074 7570  e value to a tup
+00010bc0: 6c65 2e0a 2020 2020 2020 696e 6974 5f66  le..      init_f
+00010bd0: 6e3a 2046 6f72 2074 6865 2066 6972 7374  n: For the first
+00010be0: 2076 616c 7565 2073 746f 7265 642c 2060   value stored, `
+00010bf0: 7265 6475 6365 5f66 6e60 2077 696c 6c20  reduce_fn` will 
+00010c00: 6265 2070 6173 7365 640a 2020 2020 2020  be passed.      
+00010c10: 2020 7468 6520 7265 7375 6c74 206f 6620    the result of 
+00010c20: 6069 6e69 745f 666e 6020 746f 6765 7468  `init_fn` togeth
+00010c30: 6572 2077 6974 6820 7468 6520 7661 6c75  er with the valu
+00010c40: 6520 746f 2062 6520 7374 6f72 6564 2e0a  e to be stored..
+00010c50: 2020 2020 2020 2020 5468 6520 6465 6661          The defa
+00010c60: 756c 7420 6973 2061 6e20 656d 7074 7920  ult is an empty 
+00010c70: 7475 706c 652e 0a0a 2020 2020 5265 7475  tuple...    Retu
+00010c80: 726e 733a 0a20 2020 2020 2060 5472 7565  rns:.      `True
+00010c90: 6020 6966 2074 6865 2076 616c 7565 2068  ` if the value h
+00010ca0: 6173 2062 6565 6e20 7374 6f72 6564 2073  as been stored s
+00010cb0: 7563 6365 7373 6675 6c6c 792c 2060 4661  uccessfully, `Fa
+00010cc0: 6c73 6560 206f 7468 6572 7769 7365 2e0a  lse` otherwise..
+00010cd0: 2020 2020 2222 220a 2020 2020 6966 2073      """.    if s
+00010ce0: 656c 662e 7363 6f70 6520 6973 204e 6f6e  elf.scope is Non
+00010cf0: 653a 0a20 2020 2020 2072 6169 7365 2056  e:.      raise V
+00010d00: 616c 7565 4572 726f 7228 2243 616e 2774  alueError("Can't
+00010d10: 2073 746f 7265 2076 6172 6961 626c 6573   store variables
+00010d20: 206f 6e20 756e 626f 756e 6420 6d6f 6475   on unbound modu
+00010d30: 6c65 7322 290a 2020 2020 6966 206e 6f74  les").    if not
+00010d40: 2073 656c 662e 7363 6f70 652e 6973 5f6d   self.scope.is_m
+00010d50: 7574 6162 6c65 5f63 6f6c 6c65 6374 696f  utable_collectio
+00010d60: 6e28 636f 6c29 3a0a 2020 2020 2020 7265  n(col):.      re
+00010d70: 7475 726e 2046 616c 7365 0a20 2020 2069  turn False.    i
+00010d80: 6620 7365 6c66 2e73 636f 7065 2e68 6173  f self.scope.has
+00010d90: 5f76 6172 6961 626c 6528 636f 6c2c 206e  _variable(col, n
+00010da0: 616d 6529 3a0a 2020 2020 2020 7873 203d  ame):.      xs =
+00010db0: 2073 656c 662e 7363 6f70 652e 6765 745f   self.scope.get_
+00010dc0: 7661 7269 6162 6c65 2863 6f6c 2c20 6e61  variable(col, na
+00010dd0: 6d65 290a 2020 2020 656c 7365 3a0a 2020  me).    else:.  
+00010de0: 2020 2020 7365 6c66 2e73 636f 7065 2e72      self.scope.r
+00010df0: 6573 6572 7665 286e 616d 6529 0a20 2020  eserve(name).   
+00010e00: 2020 2073 656c 662e 5f73 7461 7465 2e63     self._state.c
+00010e10: 6869 6c64 7265 6e5b 6e61 6d65 5d20 3d20  hildren[name] = 
+00010e20: 636f 6c0a 2020 2020 2020 7873 203d 2069  col.      xs = i
+00010e30: 6e69 745f 666e 2829 0a20 2020 2078 7320  nit_fn().    xs 
+00010e40: 3d20 7265 6475 6365 5f66 6e28 7873 2c20  = reduce_fn(xs, 
+00010e50: 7661 6c75 6529 0a20 2020 2073 656c 662e  value).    self.
+00010e60: 7363 6f70 652e 7075 745f 7661 7269 6162  scope.put_variab
+00010e70: 6c65 2863 6f6c 2c20 6e61 6d65 2c20 7873  le(col, name, xs
+00010e80: 290a 2020 2020 7265 7475 726e 2054 7275  ).    return Tru
+00010e90: 650a 0a20 2064 6566 2070 6572 7475 7262  e..  def perturb
+00010ea0: 2873 656c 662c 206e 616d 653a 2073 7472  (self, name: str
+00010eb0: 2c20 7661 6c75 653a 2054 2c20 636f 6c6c  , value: T, coll
+00010ec0: 6563 7469 6f6e 3a20 7374 7220 3d20 2770  ection: str = 'p
+00010ed0: 6572 7475 7262 6174 696f 6e73 2729 202d  erturbations') -
+00010ee0: 3e20 543a 0a20 2020 2022 2222 4164 6420  > T:.    """Add 
+00010ef0: 616e 207a 6572 6f2d 7661 6c75 6520 7661  an zero-value va
+00010f00: 7269 6162 6c65 2028 2770 6572 7475 7262  riable ('perturb
+00010f10: 6174 696f 6e27 2920 746f 2074 6865 2069  ation') to the i
+00010f20: 6e74 6572 6d65 6469 6174 6520 7661 6c75  ntermediate valu
+00010f30: 652e 0a0a 2020 2020 5468 6520 6772 6164  e...    The grad
+00010f40: 6965 6e74 206f 6620 6076 616c 7565 6020  ient of `value` 
+00010f50: 776f 756c 6420 6265 2074 6865 2073 616d  would be the sam
+00010f60: 6520 6173 2074 6865 2067 7261 6469 656e  e as the gradien
+00010f70: 7420 6f66 2074 6869 730a 2020 2020 7065  t of this.    pe
+00010f80: 7274 7572 6261 7469 6f6e 2076 6172 6961  rturbation varia
+00010f90: 626c 652e 2054 6865 7265 666f 7265 2c20  ble. Therefore, 
+00010fa0: 6966 2079 6f75 2064 6566 696e 6520 796f  if you define yo
+00010fb0: 7572 206c 6f73 7320 6675 6e63 7469 6f6e  ur loss function
+00010fc0: 2077 6974 680a 2020 2020 626f 7468 2070   with.    both p
+00010fd0: 6172 616d 7320 616e 6420 7065 7274 7572  arams and pertur
+00010fe0: 6261 7469 6f6e 7320 6173 2073 7461 6e64  bations as stand
+00010ff0: 616c 6f6e 6520 6172 6775 6d65 6e74 732c  alone arguments,
+00011000: 2079 6f75 2063 616e 2067 6574 2074 6865   you can get the
+00011010: 0a20 2020 2069 6e74 6572 6d65 6469 6174  .    intermediat
+00011020: 6520 6772 6164 6965 6e74 7320 6f66 2060  e gradients of `
+00011030: 7661 6c75 6560 2062 7920 7275 6e6e 696e  value` by runnin
+00011040: 6720 606a 6178 2e67 7261 6460 206f 6e20  g `jax.grad` on 
+00011050: 7468 6520 7065 7274 7572 6261 7469 6f6e  the perturbation
+00011060: 0a20 2020 2061 7267 756d 656e 742e 0a0a  .    argument...
+00011070: 2020 2020 4e6f 7465 3a20 7468 6973 2069      Note: this i
+00011080: 7320 616e 2065 7870 6572 696d 656e 7461  s an experimenta
+00011090: 6c20 4150 4920 616e 6420 6d61 7920 6265  l API and may be
+000110a0: 2074 7765 616b 6564 206c 6174 6572 2066   tweaked later f
+000110b0: 6f72 2062 6574 7465 720a 2020 2020 7065  or better.    pe
+000110c0: 7266 6f72 6d61 6e63 6520 616e 6420 7573  rformance and us
+000110d0: 6162 696c 6974 792e 0a20 2020 2041 7420  ability..    At 
+000110e0: 6974 7320 6375 7272 656e 7420 7374 6167  its current stag
+000110f0: 652c 2069 7420 6372 6561 7465 7320 6578  e, it creates ex
+00011100: 7472 6120 6475 6d6d 7920 7661 7269 6162  tra dummy variab
+00011110: 6c65 7320 7468 6174 206f 6363 7570 6965  les that occupie
+00011120: 7320 6578 7472 610a 2020 2020 6d65 6d6f  s extra.    memo
+00011130: 7279 2073 7061 6365 2e20 5573 6520 6974  ry space. Use it
+00011140: 206f 6e6c 7920 746f 2064 6562 7567 2067   only to debug g
+00011150: 7261 6469 656e 7473 2069 6e20 7472 6169  radients in trai
+00011160: 6e69 6e67 2e0a 0a20 2020 2045 7861 6d70  ning...    Examp
+00011170: 6c65 3a3a 0a0a 2020 2020 2020 696d 706f  le::..      impo
+00011180: 7274 206a 6178 0a20 2020 2020 2069 6d70  rt jax.      imp
+00011190: 6f72 7420 6a61 782e 6e75 6d70 7920 6173  ort jax.numpy as
+000111a0: 206a 6e70 0a20 2020 2020 2069 6d70 6f72   jnp.      impor
+000111b0: 7420 666c 6178 2e6c 696e 656e 2061 7320  t flax.linen as 
+000111c0: 6e6e 0a0a 2020 2020 2020 636c 6173 7320  nn..      class 
+000111d0: 466f 6f28 6e6e 2e4d 6f64 756c 6529 3a0a  Foo(nn.Module):.
+000111e0: 2020 2020 2020 2020 2020 406e 6e2e 636f            @nn.co
+000111f0: 6d70 6163 740a 2020 2020 2020 2020 2020  mpact.          
+00011200: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
+00011210: 662c 2078 293a 0a20 2020 2020 2020 2020  f, x):.         
+00011220: 2020 2020 2078 203d 206e 6e2e 4465 6e73       x = nn.Dens
+00011230: 6528 3329 2878 290a 2020 2020 2020 2020  e(3)(x).        
+00011240: 2020 2020 2020 7820 3d20 7365 6c66 2e70        x = self.p
+00011250: 6572 7475 7262 2827 6465 6e73 6533 272c  erturb('dense3',
+00011260: 2078 290a 2020 2020 2020 2020 2020 2020   x).            
+00011270: 2020 7265 7475 726e 206e 6e2e 4465 6e73    return nn.Dens
+00011280: 6528 3229 2878 290a 0a20 2020 2020 2064  e(2)(x)..      d
+00011290: 6566 206c 6f73 7328 7061 7261 6d73 2c20  ef loss(params, 
+000112a0: 7065 7274 7572 6261 7469 6f6e 732c 2069  perturbations, i
+000112b0: 6e70 7574 732c 2074 6172 6765 7473 293a  nputs, targets):
+000112c0: 0a20 2020 2020 2020 2076 6172 6961 626c  .        variabl
+000112d0: 6573 203d 207b 2770 6172 616d 7327 3a20  es = {'params': 
+000112e0: 7061 7261 6d73 2c20 2770 6572 7475 7262  params, 'perturb
+000112f0: 6174 696f 6e73 273a 2070 6572 7475 7262  ations': perturb
+00011300: 6174 696f 6e73 7d0a 2020 2020 2020 2020  ations}.        
+00011310: 7072 6564 7320 3d20 6d6f 6465 6c2e 6170  preds = model.ap
+00011320: 706c 7928 7661 7269 6162 6c65 732c 2069  ply(variables, i
+00011330: 6e70 7574 7329 0a20 2020 2020 2020 2072  nputs).        r
+00011340: 6574 7572 6e20 6a6e 702e 7371 7561 7265  eturn jnp.square
+00011350: 2870 7265 6473 202d 2074 6172 6765 7473  (preds - targets
+00011360: 292e 6d65 616e 2829 0a0a 2020 2020 2020  ).mean()..      
+00011370: 7820 3d20 6a6e 702e 6f6e 6573 2828 322c  x = jnp.ones((2,
+00011380: 2039 2929 0a20 2020 2020 2079 203d 206a   9)).      y = j
+00011390: 6e70 2e6f 6e65 7328 2832 2c20 3229 290a  np.ones((2, 2)).
+000113a0: 2020 2020 2020 6d6f 6465 6c20 3d20 466f        model = Fo
+000113b0: 6f28 290a 2020 2020 2020 7661 7269 6162  o().      variab
+000113c0: 6c65 7320 3d20 6d6f 6465 6c2e 696e 6974  les = model.init
+000113d0: 286a 6178 2e72 616e 646f 6d2e 5052 4e47  (jax.random.PRNG
+000113e0: 4b65 7928 3029 2c20 7829 0a20 2020 2020  Key(0), x).     
+000113f0: 2069 6e74 6d5f 6772 6164 7320 3d20 6a61   intm_grads = ja
+00011400: 782e 6772 6164 286c 6f73 732c 2061 7267  x.grad(loss, arg
+00011410: 6e75 6d73 3d31 2928 7661 7269 6162 6c65  nums=1)(variable
+00011420: 735b 2770 6172 616d 7327 5d2c 2076 6172  s['params'], var
+00011430: 6961 626c 6573 5b27 7065 7274 7572 6261  iables['perturba
+00011440: 7469 6f6e 7327 5d2c 2078 2c20 7929 0a20  tions'], x, y). 
+00011450: 2020 2020 2070 7269 6e74 2869 6e74 6d5f       print(intm_
+00011460: 6772 6164 735b 2764 656e 7365 3327 5d29  grads['dense3'])
+00011470: 2023 203d 3d3e 205b 5b2d 312e 3435 3639   # ==> [[-1.4569
+00011480: 3234 2020 202d 302e 3434 3333 3235 3337  24   -0.44332537
+00011490: 2020 302e 3032 3432 3238 3437 5d0a 2020    0.02422847].  
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 2320 2020 2020 205b 2d31 2e34 3536 3932  #      [-1.45692
+000114d0: 3420 2020 2d30 2e34 3433 3332 3533 3720  4   -0.44332537 
+000114e0: 2030 2e30 3234 3232 3834 375d 5d0a 0a20   0.02422847]].. 
+000114f0: 2020 2049 6620 7065 7274 7572 6261 7469     If perturbati
+00011500: 6f6e 7320 6172 6520 6e6f 7420 7061 7373  ons are not pass
+00011510: 6564 2074 6f20 6061 7070 6c79 602c 2060  ed to `apply`, `
+00011520: 7065 7274 7572 6260 2062 6568 6176 6573  perturb` behaves
+00011530: 206c 696b 6520 6120 6e6f 2d6f 700a 2020   like a no-op.  
+00011540: 2020 736f 2079 6f75 2063 616e 2065 6173    so you can eas
+00011550: 696c 7920 6469 7361 626c 6520 7468 6520  ily disable the 
+00011560: 6265 6861 7669 6f72 2077 6865 6e20 6e6f  behavior when no
+00011570: 7420 6e65 6564 6564 3a3a 0a0a 2020 2020  t needed::..    
+00011580: 2020 6d6f 6465 6c2e 6170 706c 7928 7b27    model.apply({'
+00011590: 7061 7261 6d73 273a 2070 6172 616d 732c  params': params,
+000115a0: 2027 7065 7274 7572 6261 7469 6f6e 7327   'perturbations'
+000115b0: 3a20 7065 7274 7572 6261 7469 6f6e 737d  : perturbations}
+000115c0: 2c20 7829 2023 2077 6f72 6b73 2061 7320  , x) # works as 
+000115d0: 6578 7065 6374 6564 0a20 2020 2020 206d  expected.      m
+000115e0: 6f64 656c 2e61 7070 6c79 287b 2770 6172  odel.apply({'par
+000115f0: 616d 7327 3a20 7061 7261 6d73 7d2c 2078  ams': params}, x
+00011600: 2920 2320 6265 6861 7665 7320 6c69 6b65  ) # behaves like
+00011610: 2061 206e 6f2d 6f70 0a0a 2020 2020 2222   a no-op..    ""
+00011620: 220a 2020 2020 6465 6620 5f72 6f6f 745f  ".    def _root_
+00011630: 6861 735f 636f 6c6c 6563 7469 6f6e 2829  has_collection()
+00011640: 3a0a 2020 2020 2020 2222 2252 6574 7572  :.      """Retur
+00011650: 6e73 2054 7275 6520 6966 2074 6865 2072  ns True if the r
+00011660: 6f6f 7420 7363 6f70 6520 6861 7320 7468  oot scope has th
+00011670: 6520 636f 6c6c 6563 7469 6f6e 2e22 2222  e collection."""
+00011680: 0a20 2020 2020 2061 7373 6572 7420 7365  .      assert se
+00011690: 6c66 2e73 636f 7065 2069 7320 6e6f 7420  lf.scope is not 
+000116a0: 4e6f 6e65 0a20 2020 2020 2072 6574 7572  None.      retur
+000116b0: 6e20 636f 6c6c 6563 7469 6f6e 2069 6e20  n collection in 
+000116c0: 7365 6c66 2e73 636f 7065 2e72 6f6f 742e  self.scope.root.
+000116d0: 5f76 6172 6961 626c 6573 0a20 2020 2023  _variables.    #
+000116e0: 2077 6520 7769 6c6c 206f 6e6c 7920 6164   we will only ad
+000116f0: 6420 7468 6520 7065 7274 7572 6261 7469  d the perturbati
+00011700: 6f6e 2076 6172 6961 626c 6520 6966 2074  on variable if t
+00011710: 6865 2063 6f6c 6c65 6374 696f 6e20 6973  he collection is
+00011720: 206d 7574 6162 6c65 0a20 2020 2023 2028   mutable.    # (
+00011730: 652e 672e 2064 7572 696e 6720 6069 6e69  e.g. during `ini
+00011740: 7460 2920 6f72 2069 6620 7468 6520 636f  t`) or if the co
+00011750: 6c6c 6563 7469 6f6e 2077 6173 2070 6173  llection was pas
+00011760: 7365 6420 746f 2060 6170 706c 7960 2028  sed to `apply` (
+00011770: 636f 6e74 6169 6e65 6420 696e 0a20 2020  contained in.   
+00011780: 2023 2074 6865 2072 6f6f 7420 7363 6f70   # the root scop
+00011790: 6529 2e0a 2020 2020 6966 2073 656c 662e  e)..    if self.
+000117a0: 6973 5f6d 7574 6162 6c65 5f63 6f6c 6c65  is_mutable_colle
+000117b0: 6374 696f 6e28 636f 6c6c 6563 7469 6f6e  ction(collection
+000117c0: 2920 6f72 205f 726f 6f74 5f68 6173 5f63  ) or _root_has_c
+000117d0: 6f6c 6c65 6374 696f 6e28 293a 0a20 2020  ollection():.   
+000117e0: 2020 2076 616c 7565 202b 3d20 7365 6c66     value += self
+000117f0: 2e76 6172 6961 626c 6528 636f 6c6c 6563  .variable(collec
+00011800: 7469 6f6e 2c20 6e61 6d65 2c20 6c61 6d62  tion, name, lamb
+00011810: 6461 3a20 6a6e 702e 7a65 726f 735f 6c69  da: jnp.zeros_li
+00011820: 6b65 2876 616c 7565 2929 2e76 616c 7565  ke(value)).value
+00011830: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+00011840: 2020 2020 7265 7475 726e 2076 616c 7565      return value
+00011850: 0a0a 2020 6465 6620 7461 6275 6c61 7465  ..  def tabulate
+00011860: 280a 2020 2020 7365 6c66 2c0a 2020 2020  (.    self,.    
+00011870: 726e 6773 3a20 556e 696f 6e5b 5052 4e47  rngs: Union[PRNG
+00011880: 4b65 792c 2052 4e47 5365 7175 656e 6365  Key, RNGSequence
+00011890: 735d 2c0a 2020 2020 2a61 7267 732c 0a20  s],.    *args,. 
+000118a0: 2020 2064 6570 7468 3a20 4f70 7469 6f6e     depth: Option
+000118b0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+000118c0: 2020 2020 7368 6f77 5f72 6570 6561 7465      show_repeate
+000118d0: 643a 2062 6f6f 6c20 3d20 4661 6c73 652c  d: bool = False,
+000118e0: 0a20 2020 206d 7574 6162 6c65 3a20 436f  .    mutable: Co
+000118f0: 6c6c 6563 7469 6f6e 4669 6c74 6572 203d  llectionFilter =
+00011900: 2054 7275 652c 0a20 2020 2063 6f6e 736f   True,.    conso
+00011910: 6c65 5f6b 7761 7267 733a 204f 7074 696f  le_kwargs: Optio
+00011920: 6e61 6c5b 4d61 7070 696e 675b 7374 722c  nal[Mapping[str,
+00011930: 2041 6e79 5d5d 203d 204e 6f6e 652c 0a20   Any]] = None,. 
+00011940: 2020 202a 2a6b 7761 7267 7329 202d 3e20     **kwargs) -> 
+00011950: 7374 723a 0a20 2020 2022 2222 4372 6561  str:.    """Crea
+00011960: 7465 7320 6120 7375 6d6d 6172 7920 6f66  tes a summary of
+00011970: 2074 6865 204d 6f64 756c 6520 7265 7072   the Module repr
+00011980: 6573 656e 7465 6420 6173 2061 2074 6162  esented as a tab
+00011990: 6c65 2e0a 0a20 2020 2054 6869 7320 6d65  le...    This me
+000119a0: 7468 6f64 2068 6173 2074 6865 2073 616d  thod has the sam
+000119b0: 6520 7369 676e 6174 7572 6520 616e 6420  e signature and 
+000119c0: 696e 7465 726e 616c 6c79 2063 616c 6c73  internally calls
+000119d0: 2060 4d6f 6475 6c65 2e69 6e69 7460 2c0a   `Module.init`,.
+000119e0: 2020 2020 6275 7420 696e 7374 6561 6420      but instead 
+000119f0: 6f66 2072 6574 7572 6e69 6e67 2074 6865  of returning the
+00011a00: 2076 6172 6961 626c 6573 2c20 6974 2072   variables, it r
+00011a10: 6574 7572 6e73 2074 6865 2073 7472 696e  eturns the strin
+00011a20: 6720 7375 6d6d 6172 697a 696e 670a 2020  g summarizing.  
+00011a30: 2020 7468 6520 4d6f 6475 6c65 2069 6e20    the Module in 
+00011a40: 6120 7461 626c 652e 2060 7461 6275 6c61  a table. `tabula
+00011a50: 7465 6020 7573 6573 2060 6a61 782e 6576  te` uses `jax.ev
+00011a60: 616c 5f73 6861 7065 6020 746f 2072 756e  al_shape` to run
+00011a70: 2074 6865 2066 6f72 7761 7264 0a20 2020   the forward.   
+00011a80: 2063 6f6d 7075 7461 7469 6f6e 2077 6974   computation wit
+00011a90: 686f 7574 2063 6f6e 7375 6d69 6e67 2061  hout consuming a
+00011aa0: 6e79 2046 4c4f 5073 206f 7220 616c 6c6f  ny FLOPs or allo
+00011ab0: 6361 7469 6e67 206d 656d 6f72 792e 0a0a  cating memory...
+00011ac0: 2020 2020 4164 6469 7469 6f6e 616c 2061      Additional a
+00011ad0: 7267 756d 656e 7473 2063 616e 2062 6520  rguments can be 
+00011ae0: 7061 7373 6564 2069 6e74 6f20 7468 6520  passed into the 
+00011af0: 6063 6f6e 736f 6c65 5f6b 7761 7267 7360  `console_kwargs`
+00011b00: 2061 7267 756d 656e 742c 2066 6f72 2065   argument, for e
+00011b10: 7861 6d70 6c65 2c0a 2020 2020 607b 2777  xample,.    `{'w
+00011b20: 6964 7468 273a 2031 3230 7d60 2e20 466f  idth': 120}`. Fo
+00011b30: 7220 6120 6675 6c6c 206c 6973 7420 6f66  r a full list of
+00011b40: 2060 636f 6e73 6f6c 655f 6b77 6172 6773   `console_kwargs
+00011b50: 6020 6172 6775 6d65 6e74 732c 2073 6565  ` arguments, see
+00011b60: 3a0a 2020 2020 6874 7470 733a 2f2f 7269  :.    https://ri
+00011b70: 6368 2e72 6561 6474 6865 646f 6373 2e69  ch.readthedocs.i
+00011b80: 6f2f 656e 2f73 7461 626c 652f 7265 6665  o/en/stable/refe
+00011b90: 7265 6e63 652f 636f 6e73 6f6c 652e 6874  rence/console.ht
+00011ba0: 6d6c 2372 6963 682e 636f 6e73 6f6c 652e  ml#rich.console.
+00011bb0: 436f 6e73 6f6c 650a 0a20 2020 2045 7861  Console..    Exa
+00011bc0: 6d70 6c65 3a3a 0a0a 2020 2020 2020 696d  mple::..      im
+00011bd0: 706f 7274 206a 6178 0a20 2020 2020 2069  port jax.      i
+00011be0: 6d70 6f72 7420 6a61 782e 6e75 6d70 7920  mport jax.numpy 
+00011bf0: 6173 206a 6e70 0a20 2020 2020 2069 6d70  as jnp.      imp
+00011c00: 6f72 7420 666c 6178 2e6c 696e 656e 2061  ort flax.linen a
+00011c10: 7320 6e6e 0a0a 2020 2020 2020 636c 6173  s nn..      clas
+00011c20: 7320 466f 6f28 6e6e 2e4d 6f64 756c 6529  s Foo(nn.Module)
+00011c30: 3a0a 2020 2020 2020 2020 2020 406e 6e2e  :.          @nn.
+00011c40: 636f 6d70 6163 740a 2020 2020 2020 2020  compact.        
+00011c50: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+00011c60: 656c 662c 2078 293a 0a20 2020 2020 2020  elf, x):.       
+00011c70: 2020 2020 2020 2068 203d 206e 6e2e 4465         h = nn.De
+00011c80: 6e73 6528 3429 2878 290a 2020 2020 2020  nse(4)(x).      
+00011c90: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00011ca0: 6e2e 4465 6e73 6528 3229 2868 290a 0a20  n.Dense(2)(h).. 
+00011cb0: 2020 2020 2078 203d 206a 6e70 2e6f 6e65       x = jnp.one
+00011cc0: 7328 2831 362c 2039 2929 0a0a 2020 2020  s((16, 9))..    
+00011cd0: 2020 7072 696e 7428 466f 6f28 292e 7461    print(Foo().ta
+00011ce0: 6275 6c61 7465 286a 6178 2e72 616e 646f  bulate(jax.rando
+00011cf0: 6d2e 5052 4e47 4b65 7928 3029 2c20 7829  m.PRNGKey(0), x)
+00011d00: 290a 0a0a 2020 2020 5468 6973 2067 6976  )...    This giv
+00011d10: 6573 2074 6865 2066 6f6c 6c6f 7769 6e67  es the following
+00011d20: 206f 7574 7075 743a 3a0a 0a20 2020 2020   output::..     
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d50: 2046 6f6f 2053 756d 6d61 7279 0a20 2020   Foo Summary.   
+00011d60: 2020 20e2 948f e294 81e2 9481 e294 81e2     .............
+00011d70: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00011d80: 81e2 94b3 e294 81e2 9481 e294 81e2 9481  ................
+00011d90: e294 81e2 9481 e294 81e2 9481 e294 b3e2  ................
+00011da0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00011db0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00011dc0: e294 81e2 9481 e294 81e2 9481 e294 b3e2  ................
+00011dd0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00011de0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00011df0: e294 81e2 9481 e294 81e2 9481 e294 b3e2  ................
+00011e00: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00011e10: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00011e20: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00011e30: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00011e40: 81e2 9493 0a20 2020 2020 20e2 9483 2070  .....      ... p
+00011e50: 6174 6820 2020 20e2 9483 206d 6f64 756c  ath    ... modul
+00011e60: 6520 e294 8320 696e 7075 7473 2020 2020  e ... inputs    
+00011e70: 2020 2020 e294 8320 6f75 7470 7574 7320      ... outputs 
+00011e80: 2020 2020 2020 e294 8320 7061 7261 6d73        ... params
+00011e90: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
+00011ea0: 9483 0a20 2020 2020 20e2 94a1 e294 81e2  ...      .......
+00011eb0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00011ec0: 81e2 9481 e294 81e2 9587 e294 81e2 9481  ................
+00011ed0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00011ee0: 9481 e295 87e2 9481 e294 81e2 9481 e294  ................
+00011ef0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00011f00: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00011f10: 9481 e295 87e2 9481 e294 81e2 9481 e294  ................
+00011f20: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00011f30: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00011f40: 9481 e295 87e2 9481 e294 81e2 9481 e294  ................
+00011f50: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00011f60: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00011f70: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00011f80: 81e2 9481 e294 81e2 94a9 0a20 2020 2020  ...........     
+00011f90: 20e2 9482 2020 2020 2020 2020 20e2 9482   ...         ...
+00011fa0: 2046 6f6f 2020 2020 e294 8220 666c 6f61   Foo    ... floa
+00011fb0: 7433 325b 3136 2c39 5d20 e294 8220 666c  t32[16,9] ... fl
+00011fc0: 6f61 7433 325b 3136 2c32 5d20 e294 8220  oat32[16,2] ... 
+00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fe0: 2020 2020 20e2 9482 0a20 2020 2020 20e2       ....      .
+00011ff0: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
+00012000: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+00012010: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012020: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
 00012030: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012040: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00012050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012050: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
 00012060: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012070: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00012080: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012080: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
 00012090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000120a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000120b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000120c0: a40a 2020 2020 2020 e294 8220 4465 6e73  ..      ... Dens
-000120d0: 655f 3120 e294 8220 4465 6e73 6520 20e2  e_1 ... Dense  .
-000120e0: 9482 2066 6c6f 6174 3332 5b31 362c 345d  .. float32[16,4]
-000120f0: 20e2 9482 2066 6c6f 6174 3332 5b31 362c   ... float32[16,
-00012100: 325d 20e2 9482 2062 6961 733a 2066 6c6f  2] ... bias: flo
-00012110: 6174 3332 5b32 5d20 2020 2020 e294 820a  at32[2]     ....
-00012120: 2020 2020 2020 e294 8220 2020 2020 2020        ...       
-00012130: 2020 e294 8220 2020 2020 2020 20e2 9482    ...        ...
-00012140: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00012150: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00012160: 20e2 9482 206b 6572 6e65 6c3a 2066 6c6f   ... kernel: flo
-00012170: 6174 3332 5b34 2c32 5d20 e294 820a 2020  at32[4,2] ....  
-00012180: 2020 2020 e294 8220 2020 2020 2020 2020      ...         
-00012190: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
-000121a0: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-000121b0: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-000121c0: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-000121d0: 2020 2020 2020 2020 e294 820a 2020 2020          ....    
-000121e0: 2020 e294 8220 2020 2020 2020 2020 e294    ...         ..
-000121f0: 8220 2020 2020 2020 20e2 9482 2020 2020  .        ...    
-00012200: 2020 2020 2020 2020 2020 20e2 9482 2020             ...  
-00012210: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00012220: 2031 3020 2834 3020 4229 2020 2020 2020   10 (40 B)      
-00012230: 2020 2020 2020 e294 820a 2020 2020 2020        ....      
-00012240: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
-00012250: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012260: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012270: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00012280: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000120c0: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
+000120d0: 0a20 2020 2020 20e2 9482 2044 656e 7365  .      ... Dense
+000120e0: 5f30 20e2 9482 2044 656e 7365 2020 e294  _0 ... Dense  ..
+000120f0: 8220 666c 6f61 7433 325b 3136 2c39 5d20  . float32[16,9] 
+00012100: e294 8220 666c 6f61 7433 325b 3136 2c34  ... float32[16,4
+00012110: 5d20 e294 8220 6269 6173 3a20 666c 6f61  ] ... bias: floa
+00012120: 7433 325b 345d 2020 2020 20e2 9482 0a20  t32[4]     .... 
+00012130: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
+00012140: 20e2 9482 2020 2020 2020 2020 e294 8220   ...        ... 
+00012150: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+00012160: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00012170: e294 8220 6b65 726e 656c 3a20 666c 6f61  ... kernel: floa
+00012180: 7433 325b 392c 345d 20e2 9482 0a20 2020  t32[9,4] ....   
+00012190: 2020 20e2 9482 2020 2020 2020 2020 20e2     ...         .
+000121a0: 9482 2020 2020 2020 2020 e294 8220 2020  ..        ...   
+000121b0: 2020 2020 2020 2020 2020 2020 e294 8220              ... 
+000121c0: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+000121d0: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+000121e0: 2020 2020 2020 20e2 9482 0a20 2020 2020         ....     
+000121f0: 20e2 9482 2020 2020 2020 2020 20e2 9482   ...         ...
+00012200: 2020 2020 2020 2020 e294 8220 2020 2020          ...     
+00012210: 2020 2020 2020 2020 2020 e294 8220 2020            ...   
+00012220: 2020 2020 2020 2020 2020 2020 e294 8220              ... 
+00012230: 3430 2028 3136 3020 4229 2020 2020 2020  40 (160 B)      
+00012240: 2020 2020 20e2 9482 0a20 2020 2020 20e2       ....      .
+00012250: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
+00012260: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+00012270: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012280: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
 00012290: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000122a0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-000122b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000122a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000122b0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
 000122c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000122d0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-000122e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000122d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000122e0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
 000122f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00012300: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00012310: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012320: a40a 2020 2020 2020 e294 8220 2020 2020  ..      ...     
-00012330: 2020 2020 e294 8220 2020 2020 2020 20e2      ...        .
-00012340: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00012350: 20e2 9482 2020 2020 2020 2020 2054 6f74   ...         Tot
-00012360: 616c 20e2 9482 2035 3020 2832 3030 2042  al ... 50 (200 B
-00012370: 2920 2020 2020 2020 2020 2020 e294 820a  )           ....
-00012380: 2020 2020 2020 e294 94e2 9480 e294 80e2        ..........
-00012390: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000123a0: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-000123b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000123c0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-000123d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000123e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000123f0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012400: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012410: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012420: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012430: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012440: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012450: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012460: 80e2 9480 e294 980a 0a20 2020 2020 2020  .........       
-00012470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012480: 2020 2020 2054 6f74 616c 2050 6172 616d       Total Param
-00012490: 6574 6572 733a 2035 3020 2832 3030 2042  eters: 50 (200 B
-000124a0: 290a 0a20 2020 202a 2a4e 6f74 652a 2a3a  )..    **Note**:
-000124b0: 2072 6f77 7320 6f72 6465 7220 696e 2074   rows order in t
-000124c0: 6865 2074 6162 6c65 2064 6f65 7320 6e6f  he table does no
-000124d0: 7420 7265 7072 6573 656e 7420 6578 6563  t represent exec
-000124e0: 7574 696f 6e20 6f72 6465 722c 0a20 2020  ution order,.   
-000124f0: 2069 6e73 7465 6164 2069 7420 616c 6967   instead it alig
-00012500: 6e73 2077 6974 6820 7468 6520 6f72 6465  ns with the orde
-00012510: 7220 6f66 206b 6579 7320 696e 2060 7661  r of keys in `va
-00012520: 7269 6162 6c65 7360 2077 6869 6368 2061  riables` which a
-00012530: 7265 2073 6f72 7465 640a 2020 2020 616c  re sorted.    al
-00012540: 7068 6162 6574 6963 616c 6c79 2e0a 0a20  phabetically... 
-00012550: 2020 2041 7267 733a 0a20 2020 2020 2072     Args:.      r
-00012560: 6e67 733a 2054 6865 2072 6e67 7320 666f  ngs: The rngs fo
-00012570: 7220 7468 6520 7661 7269 6162 6c65 2063  r the variable c
-00012580: 6f6c 6c65 6374 696f 6e73 2061 7320 7061  ollections as pa
-00012590: 7373 6564 2074 6f20 604d 6f64 756c 652e  ssed to `Module.
-000125a0: 696e 6974 602e 0a20 2020 2020 202a 6172  init`..      *ar
-000125b0: 6773 3a20 5468 6520 6172 6775 6d65 6e74  gs: The argument
-000125c0: 7320 746f 2074 6865 2066 6f72 7761 7264  s to the forward
-000125d0: 2063 6f6d 7075 7461 7469 6f6e 2e0a 2020   computation..  
-000125e0: 2020 2020 6465 7074 683a 2063 6f6e 7472      depth: contr
-000125f0: 6f6c 7320 686f 7720 6d61 6e79 2073 7562  ols how many sub
-00012600: 6d6f 6475 6c65 2064 6565 7020 7468 6520  module deep the 
-00012610: 7375 6d6d 6172 7920 6361 6e20 676f 2e20  summary can go. 
-00012620: 4279 2064 6566 6175 6c74 2069 7473 0a20  By default its. 
-00012630: 2020 2020 2020 2060 4e6f 6e65 6020 7768         `None` wh
-00012640: 6963 6820 6d65 616e 7320 6e6f 206c 696d  ich means no lim
-00012650: 6974 2e20 4966 2061 2073 7562 6d6f 6475  it. If a submodu
-00012660: 6c65 2069 7320 6e6f 7420 7368 6f77 6e20  le is not shown 
-00012670: 6265 6361 7573 6520 6f66 2074 6865 0a20  because of the. 
-00012680: 2020 2020 2020 2064 6570 7468 206c 696d         depth lim
-00012690: 6974 2c20 6974 7320 7061 7261 6d65 7465  it, its paramete
-000126a0: 7220 636f 756e 7420 616e 6420 6279 7465  r count and byte
-000126b0: 7320 7769 6c6c 2062 6520 6164 6465 6420  s will be added 
-000126c0: 746f 2074 6865 2072 6f77 206f 6620 6974  to the row of it
-000126d0: 730a 2020 2020 2020 2020 6669 7273 7420  s.        first 
-000126e0: 7368 6f77 6e20 616e 6365 7374 6f72 2073  shown ancestor s
-000126f0: 7563 6820 7468 6174 2074 6865 2073 756d  uch that the sum
-00012700: 206f 6620 616c 6c20 726f 7773 2061 6c77   of all rows alw
-00012710: 6179 7320 6164 6473 2075 7020 746f 2074  ays adds up to t
-00012720: 6865 0a20 2020 2020 2020 2074 6f74 616c  he.        total
-00012730: 206e 756d 6265 7220 6f66 2070 6172 616d   number of param
-00012740: 6574 6572 7320 6f66 2074 6865 204d 6f64  eters of the Mod
-00012750: 756c 652e 0a20 2020 2020 2073 686f 775f  ule..      show_
-00012760: 7265 7065 6174 6564 3a20 4966 2060 5472  repeated: If `Tr
-00012770: 7565 602c 2072 6570 6561 7465 6420 6361  ue`, repeated ca
-00012780: 6c6c 7320 746f 2074 6865 2073 616d 6520  lls to the same 
-00012790: 6d6f 6475 6c65 2077 696c 6c20 6265 2073  module will be s
-000127a0: 686f 776e 0a20 2020 2020 2020 2069 6e20  hown.        in 
-000127b0: 7468 6520 7461 626c 652c 206f 7468 6572  the table, other
-000127c0: 7769 7365 206f 6e6c 7920 7468 6520 6669  wise only the fi
-000127d0: 7273 7420 6361 6c6c 2077 696c 6c20 6265  rst call will be
-000127e0: 2073 686f 776e 2e20 4465 6661 756c 7420   shown. Default 
-000127f0: 6973 0a20 2020 2020 2020 2060 4661 6c73  is.        `Fals
-00012800: 6560 2e0a 2020 2020 2020 6d75 7461 626c  e`..      mutabl
-00012810: 653a 2043 616e 2062 6520 626f 6f6c 2c20  e: Can be bool, 
-00012820: 7374 722c 206f 7220 6c69 7374 2e20 5370  str, or list. Sp
-00012830: 6563 6966 6965 7320 7768 6963 6820 636f  ecifies which co
-00012840: 6c6c 6563 7469 6f6e 7320 7368 6f75 6c64  llections should
-00012850: 2062 650a 2020 2020 2020 2020 7472 6561   be.        trea
-00012860: 7465 6420 6173 206d 7574 6162 6c65 3a20  ted as mutable: 
-00012870: 6060 626f 6f6c 6060 3a20 616c 6c2f 6e6f  ``bool``: all/no
-00012880: 2063 6f6c 6c65 6374 696f 6e73 2061 7265   collections are
-00012890: 206d 7574 6162 6c65 2e20 6060 7374 7260   mutable. ``str`
-000128a0: 603a 2054 6865 0a20 2020 2020 2020 206e  `: The.        n
-000128b0: 616d 6520 6f66 2061 2073 696e 676c 6520  ame of a single 
-000128c0: 6d75 7461 626c 6520 636f 6c6c 6563 7469  mutable collecti
-000128d0: 6f6e 2e20 6060 6c69 7374 6060 3a20 4120  on. ``list``: A 
-000128e0: 6c69 7374 206f 6620 6e61 6d65 7320 6f66  list of names of
-000128f0: 206d 7574 6162 6c65 0a20 2020 2020 2020   mutable.       
-00012900: 2063 6f6c 6c65 6374 696f 6e73 2e20 4279   collections. By
-00012910: 2064 6566 6175 6c74 2061 6c6c 2063 6f6c   default all col
-00012920: 6c65 6374 696f 6e73 2065 7863 6570 7420  lections except 
-00012930: 2769 6e74 6572 6d65 6469 6174 6573 2720  'intermediates' 
-00012940: 6172 650a 2020 2020 2020 2020 6d75 7461  are.        muta
-00012950: 626c 652e 0a20 2020 2020 2063 6f6e 736f  ble..      conso
-00012960: 6c65 5f6b 7761 7267 733a 2041 6e20 6f70  le_kwargs: An op
-00012970: 7469 6f6e 616c 2064 6963 7469 6f6e 6172  tional dictionar
-00012980: 7920 7769 7468 2061 6464 6974 696f 6e61  y with additiona
-00012990: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-000129a0: 6e74 7320 7468 6174 0a20 2020 2020 2020  nts that.       
-000129b0: 2061 7265 2070 6173 7365 6420 746f 2060   are passed to `
-000129c0: 7269 6368 2e63 6f6e 736f 6c65 2e43 6f6e  rich.console.Con
-000129d0: 736f 6c65 6020 7768 656e 2072 656e 6465  sole` when rende
-000129e0: 7269 6e67 2074 6865 2074 6162 6c65 2e20  ring the table. 
-000129f0: 4465 6661 756c 7420 6172 6775 6d65 6e74  Default argument
-00012a00: 730a 2020 2020 2020 2020 6172 6520 607b  s.        are `{
-00012a10: 2766 6f72 6365 5f74 6572 6d69 6e61 6c27  'force_terminal'
-00012a20: 3a20 5472 7565 2c20 2766 6f72 6365 5f6a  : True, 'force_j
-00012a30: 7570 7974 6572 273a 2046 616c 7365 7d60  upyter': False}`
-00012a40: 2e0a 2020 2020 2020 2a2a 6b77 6172 6773  ..      **kwargs
-00012a50: 3a20 6b65 7977 6f72 6420 6172 6775 6d65  : keyword argume
-00012a60: 6e74 7320 746f 2070 6173 7320 746f 2074  nts to pass to t
-00012a70: 6865 2066 6f72 7761 7264 2063 6f6d 7075  he forward compu
-00012a80: 7461 7469 6f6e 2e0a 0a20 2020 2052 6574  tation...    Ret
-00012a90: 7572 6e73 3a0a 2020 2020 2020 4120 7374  urns:.      A st
-00012aa0: 7269 6e67 2073 756d 6d61 7269 7a69 6e67  ring summarizing
-00012ab0: 2074 6865 204d 6f64 756c 652e 0a20 2020   the Module..   
-00012ac0: 2022 2222 0a20 2020 2066 726f 6d20 666c   """.    from fl
-00012ad0: 6178 2e6c 696e 656e 2069 6d70 6f72 7420  ax.linen import 
-00012ae0: 7375 6d6d 6172 790a 0a20 2020 2074 6162  summary..    tab
-00012af0: 756c 6174 655f 666e 203d 2073 756d 6d61  ulate_fn = summa
-00012b00: 7279 2e74 6162 756c 6174 6528 7365 6c66  ry.tabulate(self
-00012b10: 2c20 726e 6773 2c20 6465 7074 683d 6465  , rngs, depth=de
-00012b20: 7074 682c 0a20 2020 2020 2020 2020 2020  pth,.           
-00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b40: 2020 2020 2020 2020 7368 6f77 5f72 6570          show_rep
-00012b50: 6561 7465 643d 7368 6f77 5f72 6570 6561  eated=show_repea
-00012b60: 7465 642c 206d 7574 6162 6c65 3d6d 7574  ted, mutable=mut
-00012b70: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
-00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b90: 2020 2020 2020 2020 2063 6f6e 736f 6c65           console
-00012ba0: 5f6b 7761 7267 733d 636f 6e73 6f6c 655f  _kwargs=console_
-00012bb0: 6b77 6172 6773 290a 2020 2020 7265 7475  kwargs).    retu
-00012bc0: 726e 2074 6162 756c 6174 655f 666e 282a  rn tabulate_fn(*
-00012bd0: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
-00012be0: 0a0a 5f50 6172 656e 7454 7970 6520 3d20  .._ParentType = 
-00012bf0: 556e 696f 6e5b 5479 7065 5b4d 6f64 756c  Union[Type[Modul
-00012c00: 655d 2c20 5479 7065 5b53 636f 7065 5d2c  e], Type[Scope],
-00012c10: 2054 7970 655b 5f53 656e 7469 6e65 6c5d   Type[_Sentinel]
-00012c20: 2c20 4e6f 6e65 5d0a 0a64 6566 206d 6572  , None]..def mer
-00012c30: 6765 5f70 6172 616d 286e 616d 653a 2073  ge_param(name: s
-00012c40: 7472 2c20 613a 204f 7074 696f 6e61 6c5b  tr, a: Optional[
-00012c50: 545d 2c20 623a 204f 7074 696f 6e61 6c5b  T], b: Optional[
-00012c60: 545d 2920 2d3e 2054 3a0a 2020 2222 224d  T]) -> T:.  """M
-00012c70: 6572 6765 7320 636f 6e73 7472 7563 7469  erges constructi
-00012c80: 6f6e 2d20 616e 6420 6361 6c6c 2d74 696d  on- and call-tim
-00012c90: 6520 6172 6775 6d65 6e74 2e0a 0a20 2054  e argument...  T
-00012ca0: 6869 7320 6973 2061 2075 7469 6c69 7479  his is a utility
-00012cb0: 2066 6f72 2073 7570 706f 7274 696e 6720   for supporting 
-00012cc0: 6120 7061 7474 6572 6e20 7768 6572 6520  a pattern where 
-00012cd0: 6120 4d6f 6475 6c65 2068 7970 6572 7061  a Module hyperpa
-00012ce0: 7261 6d65 7465 720a 2020 6361 6e20 6265  rameter.  can be
-00012cf0: 2070 6173 7365 6420 6569 7468 6572 2074   passed either t
-00012d00: 6f20 6060 5f5f 696e 6974 5f5f 6060 206f  o ``__init__`` o
-00012d10: 7220 6060 5f5f 6361 6c6c 5f5f 6060 2c20  r ``__call__``, 
-00012d20: 616e 6420 7468 6520 7661 6c75 6520 7468  and the value th
-00012d30: 6174 2069 730a 2020 6e6f 7420 604e 6f6e  at is.  not `Non
-00012d40: 6560 2077 696c 6c20 6265 2075 7365 642e  e` will be used.
-00012d50: 0a0a 2020 4578 616d 706c 653a 3a0a 0a20  ..  Example::.. 
-00012d60: 2020 2063 6c61 7373 2046 6f6f 286e 6e2e     class Foo(nn.
-00012d70: 4d6f 6475 6c65 293a 0a20 2020 2020 2074  Module):.      t
-00012d80: 7261 696e 3a20 4f70 7469 6f6e 616c 5b62  rain: Optional[b
-00012d90: 6f6f 6c5d 203d 204e 6f6e 650a 0a20 2020  ool] = None..   
-00012da0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-00012db0: 7365 6c66 2c20 7472 6169 6e3a 204f 7074  self, train: Opt
-00012dc0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00012dd0: 6e65 293a 0a20 2020 2020 2020 2074 7261  ne):.        tra
-00012de0: 696e 203d 206e 6e2e 6d65 7267 655f 7061  in = nn.merge_pa
-00012df0: 7261 6d28 2774 7261 696e 272c 2073 656c  ram('train', sel
-00012e00: 662e 7472 6169 6e2c 2074 7261 696e 290a  f.train, train).
-00012e10: 0a20 2041 6e20 6572 726f 7220 6973 2074  .  An error is t
-00012e20: 6872 6f77 6e20 7768 656e 2062 6f74 6820  hrown when both 
-00012e30: 6172 6775 6d65 6e74 7320 6172 6520 604e  arguments are `N
-00012e40: 6f6e 6560 206f 7220 626f 7468 2076 616c  one` or both val
-00012e50: 7565 7320 6172 6520 6e6f 740a 2020 604e  ues are not.  `N
-00012e60: 6f6e 6560 2e0a 0a20 2041 7267 733a 0a20  one`...  Args:. 
-00012e70: 2020 206e 616d 653a 2074 6865 206e 616d     name: the nam
-00012e80: 6520 6f66 2074 6865 2070 6172 616d 6574  e of the paramet
-00012e90: 6572 2e20 5573 6564 2066 6f72 2065 7272  er. Used for err
-00012ea0: 6f72 206d 6573 7361 6765 732e 0a20 2020  or messages..   
-00012eb0: 2061 3a20 6f70 7469 6f6e 2061 0a20 2020   a: option a.   
-00012ec0: 2062 3a20 6f70 7469 6f6e 2062 0a20 2052   b: option b.  R
-00012ed0: 6574 7572 6e73 3a0a 2020 2020 6120 6f72  eturns:.    a or
-00012ee0: 2062 2077 6869 6368 6576 6572 2069 7320   b whichever is 
-00012ef0: 6e6f 7420 604e 6f6e 6560 2e0a 0a20 2022  not `None`...  "
-00012f00: 2222 0a20 2069 6620 6120 6973 204e 6f6e  "".  if a is Non
-00012f10: 6520 616e 6420 6220 6973 204e 6f6e 653a  e and b is None:
-00012f20: 0a20 2020 2072 6169 7365 2056 616c 7565  .    raise Value
-00012f30: 4572 726f 7228 6627 5061 7261 6d65 7465  Error(f'Paramete
-00012f40: 7220 227b 6e61 6d65 7d22 206d 7573 7420  r "{name}" must 
-00012f50: 6265 2070 6173 7365 6420 746f 2074 6865  be passed to the
-00012f60: 2063 6f6e 7374 7275 6374 6f72 206f 7220   constructor or 
-00012f70: 6174 2063 616c 6c20 7469 6d65 2e27 290a  at call time.').
-00012f80: 2020 6966 2061 2069 7320 6e6f 7420 4e6f    if a is not No
-00012f90: 6e65 2061 6e64 2062 2069 7320 6e6f 7420  ne and b is not 
-00012fa0: 4e6f 6e65 3a0a 2020 2020 7261 6973 6520  None:.    raise 
-00012fb0: 5661 6c75 6545 7272 6f72 2866 2750 6172  ValueError(f'Par
-00012fc0: 616d 6574 6572 2022 7b6e 616d 657d 2220  ameter "{name}" 
-00012fd0: 7761 7320 7061 7373 6564 2074 6f20 7468  was passed to th
-00012fe0: 6520 636f 6e73 7472 7563 746f 7220 616e  e constructor an
-00012ff0: 6420 6174 2063 616c 6c20 7469 6d65 2e27  d at call time.'
-00013000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013010: 2020 2020 2020 2720 5368 6f75 6c64 2062        ' Should b
-00013020: 6520 7061 7373 6564 206a 7573 7420 6f6e  e passed just on
-00013030: 6365 2e27 290a 2020 6966 2061 2069 7320  ce.').  if a is 
-00013040: 4e6f 6e65 3a0a 2020 2020 6173 7365 7274  None:.    assert
-00013050: 2062 2069 7320 6e6f 7420 4e6f 6e65 0a20   b is not None. 
-00013060: 2020 2072 6574 7572 6e20 620a 2020 7265     return b.  re
-00013070: 7475 726e 2061 0a0a 0a40 7472 6163 6562  turn a...@traceb
-00013080: 6163 6b5f 7574 696c 2e61 7069 5f62 6f75  ack_util.api_bou
-00013090: 6e64 6172 790a 6465 6620 6170 706c 7928  ndary.def apply(
-000130a0: 666e 3a20 4361 6c6c 6162 6c65 5b2e 2e2e  fn: Callable[...
-000130b0: 2c20 416e 795d 2c20 6d6f 6475 6c65 3a20  , Any], module: 
-000130c0: 4d6f 6475 6c65 2c0a 2020 2020 2020 2020  Module,.        
-000130d0: 2020 6d75 7461 626c 653a 2043 6f6c 6c65    mutable: Colle
-000130e0: 6374 696f 6e46 696c 7465 7220 3d20 4661  ctionFilter = Fa
-000130f0: 6c73 652c 0a20 2020 2020 2020 2020 2063  lse,.          c
-00013100: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
-00013110: 6174 6573 3a20 556e 696f 6e5b 626f 6f6c  ates: Union[bool
-00013120: 2c20 4361 6c6c 6162 6c65 5b5b 4d6f 6475  , Callable[[Modu
-00013130: 6c65 2c20 7374 725d 2c20 626f 6f6c 5d5d  le, str], bool]]
-00013140: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00013150: 2020 2020 2920 2d3e 2043 616c 6c61 626c      ) -> Callabl
-00013160: 655b 2e2e 2e2c 2041 6e79 5d3a 0a20 2022  e[..., Any]:.  "
-00013170: 2222 4372 6561 7465 7320 616e 2061 7070  ""Creates an app
-00013180: 6c79 2066 756e 6374 696f 6e20 746f 2063  ly function to c
-00013190: 616c 6c20 6060 666e 6060 2077 6974 6820  all ``fn`` with 
-000131a0: 6120 626f 756e 6420 6d6f 6475 6c65 2e0a  a bound module..
-000131b0: 0a20 2055 6e6c 696b 6520 6060 4d6f 6475  .  Unlike ``Modu
-000131c0: 6c65 2e61 7070 6c79 6060 2074 6869 7320  le.apply`` this 
-000131d0: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-000131e0: 2061 206e 6577 2066 756e 6374 696f 6e20   a new function 
-000131f0: 7769 7468 2074 6865 2073 6967 6e61 7475  with the signatu
-00013200: 7265 0a20 2060 6028 7661 7269 6162 6c65  re.  ``(variable
-00013210: 732c 202a 6172 6773 2c20 726e 6773 3d4e  s, *args, rngs=N
-00013220: 6f6e 652c 202a 2a6b 7761 7267 7329 202d  one, **kwargs) -
-00013230: 3e20 5460 6020 7768 6572 6520 6054 6020  > T`` where `T` 
-00013240: 6973 2074 6865 2072 6574 7572 6e20 7479  is the return ty
-00013250: 7065 0a20 206f 6620 6060 666e 6060 2e20  pe.  of ``fn``. 
-00013260: 4966 2060 606d 7574 6162 6c65 6060 2069  If ``mutable`` i
-00013270: 7320 6e6f 7420 6060 4661 6c73 6560 6020  s not ``False`` 
-00013280: 7468 6520 7265 7475 726e 2074 7970 6520  the return type 
-00013290: 6973 2061 2074 7570 6c65 2077 6865 7265  is a tuple where
-000132a0: 2074 6865 0a20 2073 6563 6f6e 6420 6974   the.  second it
-000132b0: 656d 2069 7320 6120 6060 4672 6f7a 656e  em is a ``Frozen
-000132c0: 4469 6374 6060 2077 6974 6820 7468 6520  Dict`` with the 
-000132d0: 6d75 7461 7465 6420 7661 7269 6162 6c65  mutated variable
-000132e0: 732e 0a0a 2020 5468 6520 6170 706c 7920  s...  The apply 
-000132f0: 6675 6e63 7469 6f6e 2074 6861 7420 6973  function that is
-00013300: 2072 6574 7572 6e65 6420 6361 6e20 6265   returned can be
-00013310: 2064 6972 6563 746c 7920 636f 6d70 6f73   directly compos
-00013320: 6564 2077 6974 680a 2020 4a41 5820 7472  ed with.  JAX tr
-00013330: 616e 7366 6f72 6d61 7469 6f6e 7320 6c69  ansformations li
-00013340: 6b65 2060 606a 6178 2e6a 6974 6060 3a3a  ke ``jax.jit``::
-00013350: 0a0a 2020 2020 6465 6620 6628 666f 6f2c  ..    def f(foo,
-00013360: 2078 293a 0a20 2020 2020 207a 203d 2066   x):.      z = f
-00013370: 6f6f 2e65 6e63 6f64 6528 7829 0a20 2020  oo.encode(x).   
-00013380: 2020 2079 203d 2066 6f6f 2e64 6563 6f64     y = foo.decod
-00013390: 6528 7a29 0a20 2020 2020 2023 202e 2e2e  e(z).      # ...
-000133a0: 0a20 2020 2020 2072 6574 7572 6e20 790a  .      return y.
-000133b0: 0a20 2020 2066 6f6f 203d 2046 6f6f 2829  .    foo = Foo()
-000133c0: 0a20 2020 2066 5f6a 6974 7465 6420 3d20  .    f_jitted = 
-000133d0: 6a61 782e 6a69 7428 6e6e 2e61 7070 6c79  jax.jit(nn.apply
-000133e0: 2866 2c20 666f 6f29 290a 2020 2020 665f  (f, foo)).    f_
-000133f0: 6a69 7474 6564 2876 6172 6961 626c 6573  jitted(variables
-00013400: 2c20 7829 0a0a 2020 4172 6773 3a0a 2020  , x)..  Args:.  
-00013410: 2020 666e 3a20 5468 6520 6675 6e63 7469    fn: The functi
-00013420: 6f6e 2074 6861 7420 7368 6f75 6c64 2062  on that should b
-00013430: 6520 6170 706c 6965 642e 2054 6865 2066  e applied. The f
-00013440: 6972 7374 2061 7267 756d 656e 7420 7061  irst argument pa
-00013450: 7373 6564 2077 696c 6c0a 2020 2020 2020  ssed will.      
-00013460: 6265 2061 6e20 6d6f 6475 6c65 2069 6e73  be an module ins
-00013470: 7461 6e63 6520 6f66 2074 6865 2060 606d  tance of the ``m
-00013480: 6f64 756c 6560 6020 7769 7468 2076 6172  odule`` with var
-00013490: 6961 626c 6573 2061 6e64 2052 4e47 7320  iables and RNGs 
-000134a0: 626f 756e 640a 2020 2020 2020 746f 2069  bound.      to i
-000134b0: 742e 0a20 2020 206d 6f64 756c 653a 2054  t..    module: T
-000134c0: 6865 2060 604d 6f64 756c 6560 6020 7468  he ``Module`` th
-000134d0: 6174 2077 696c 6c20 6265 2075 7365 6420  at will be used 
-000134e0: 746f 2062 696e 6420 7661 7269 6162 6c65  to bind variable
-000134f0: 7320 616e 6420 524e 4773 2074 6f2e 0a20  s and RNGs to.. 
-00013500: 2020 2020 2054 6865 2060 604d 6f64 756c       The ``Modul
-00013510: 6560 6020 7061 7373 6564 2061 7320 7468  e`` passed as th
-00013520: 6520 6669 7273 7420 6172 6775 6d65 6e74  e first argument
-00013530: 2074 6f20 6060 666e 6060 2077 696c 6c20   to ``fn`` will 
-00013540: 6265 2061 2063 6c6f 6e65 0a20 2020 2020  be a clone.     
-00013550: 206f 6620 6d6f 6475 6c65 2e0a 2020 2020   of module..    
-00013560: 6d75 7461 626c 653a 2043 616e 2062 6520  mutable: Can be 
-00013570: 626f 6f6c 2c20 7374 722c 206f 7220 6c69  bool, str, or li
-00013580: 7374 2e20 5370 6563 6966 6965 7320 7768  st. Specifies wh
-00013590: 6963 6820 636f 6c6c 6563 7469 6f6e 7320  ich collections 
-000135a0: 7368 6f75 6c64 2062 650a 2020 2020 2020  should be.      
-000135b0: 7472 6561 7465 6420 6173 206d 7574 6162  treated as mutab
-000135c0: 6c65 3a20 6060 626f 6f6c 6060 3a20 616c  le: ``bool``: al
-000135d0: 6c2f 6e6f 2063 6f6c 6c65 6374 696f 6e73  l/no collections
-000135e0: 2061 7265 206d 7574 6162 6c65 2e0a 2020   are mutable..  
-000135f0: 2020 2020 6060 7374 7260 603a 2054 6865      ``str``: The
-00013600: 206e 616d 6520 6f66 2061 2073 696e 676c   name of a singl
-00013610: 6520 6d75 7461 626c 6520 636f 6c6c 6563  e mutable collec
-00013620: 7469 6f6e 2e20 6060 6c69 7374 6060 3a20  tion. ``list``: 
-00013630: 410a 2020 2020 2020 6c69 7374 206f 6620  A.      list of 
-00013640: 6e61 6d65 7320 6f66 206d 7574 6162 6c65  names of mutable
-00013650: 2063 6f6c 6c65 6374 696f 6e73 2e0a 2020   collections..  
-00013660: 2020 6361 7074 7572 655f 696e 7465 726d    capture_interm
-00013670: 6564 6961 7465 733a 2049 6620 6054 7275  ediates: If `Tru
-00013680: 6560 2c20 6361 7074 7572 6573 2069 6e74  e`, captures int
-00013690: 6572 6d65 6469 6174 6520 7265 7475 726e  ermediate return
-000136a0: 2076 616c 7565 730a 2020 2020 2020 6f66   values.      of
-000136b0: 2061 6c6c 204d 6f64 756c 6573 2069 6e73   all Modules ins
-000136c0: 6964 6520 7468 6520 2269 6e74 6572 6d65  ide the "interme
-000136d0: 6469 6174 6573 2220 636f 6c6c 6563 7469  diates" collecti
-000136e0: 6f6e 2e20 4279 2064 6566 6175 6c74 206f  on. By default o
-000136f0: 6e6c 790a 2020 2020 2020 7468 6520 7265  nly.      the re
-00013700: 7475 726e 2076 616c 7565 7320 6f66 2061  turn values of a
-00013710: 6c6c 2060 5f5f 6361 6c6c 5f5f 6020 6d65  ll `__call__` me
-00013720: 7468 6f64 7320 6172 6520 7374 6f72 6564  thods are stored
-00013730: 2e20 4120 6675 6e63 7469 6f6e 2063 616e  . A function can
-00013740: 0a20 2020 2020 2062 6520 7061 7373 6564  .      be passed
-00013750: 2074 6f20 6368 616e 6765 2074 6865 2066   to change the f
-00013760: 696c 7465 7220 6265 6861 7669 6f72 2e20  ilter behavior. 
-00013770: 5468 6520 6669 6c74 6572 2066 756e 6374  The filter funct
-00013780: 696f 6e20 7461 6b65 730a 2020 2020 2020  ion takes.      
-00013790: 7468 6520 4d6f 6475 6c65 2069 6e73 7461  the Module insta
-000137a0: 6e63 6520 616e 6420 6d65 7468 6f64 206e  nce and method n
-000137b0: 616d 6520 616e 6420 7265 7475 726e 7320  ame and returns 
-000137c0: 6120 626f 6f6c 2069 6e64 6963 6174 696e  a bool indicatin
-000137d0: 670a 2020 2020 2020 7768 6574 6865 7220  g.      whether 
-000137e0: 7468 6520 6f75 7470 7574 206f 6620 7468  the output of th
-000137f0: 6174 206d 6574 686f 6420 696e 766f 6361  at method invoca
-00013800: 7469 6f6e 2073 686f 756c 6420 6265 2073  tion should be s
-00013810: 746f 7265 642e 0a20 2052 6574 7572 6e73  tored..  Returns
-00013820: 3a0a 2020 2020 5468 6520 6170 706c 7920  :.    The apply 
-00013830: 6675 6e63 7469 6f6e 2077 7261 7070 696e  function wrappin
-00013840: 6720 6060 666e 6060 2e0a 2020 2222 220a  g ``fn``..  """.
-00013850: 2020 4066 756e 6374 6f6f 6c73 2e77 7261    @functools.wra
-00013860: 7073 2866 6e29 0a20 2064 6566 2073 636f  ps(fn).  def sco
-00013870: 7065 5f66 6e28 7363 6f70 652c 202a 6172  pe_fn(scope, *ar
-00013880: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
-00013890: 2020 205f 636f 6e74 6578 742e 6361 7074     _context.capt
-000138a0: 7572 655f 7374 6163 6b2e 6170 7065 6e64  ure_stack.append
-000138b0: 2863 6170 7475 7265 5f69 6e74 6572 6d65  (capture_interme
-000138c0: 6469 6174 6573 290a 2020 2020 7472 793a  diates).    try:
-000138d0: 0a20 2020 2020 2072 6574 7572 6e20 666e  .      return fn
-000138e0: 286d 6f64 756c 652e 636c 6f6e 6528 7061  (module.clone(pa
-000138f0: 7265 6e74 3d73 636f 7065 292c 202a 6172  rent=scope), *ar
-00013900: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
-00013910: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
-00013920: 205f 636f 6e74 6578 742e 6361 7074 7572   _context.captur
-00013930: 655f 7374 6163 6b2e 706f 7028 290a 0a20  e_stack.pop().. 
-00013940: 2069 6620 6361 7074 7572 655f 696e 7465   if capture_inte
-00013950: 726d 6564 6961 7465 7320 6973 2054 7275  rmediates is Tru
-00013960: 653a 2020 2320 7079 6c69 6e74 3a20 6469  e:  # pylint: di
-00013970: 7361 626c 653d 672d 626f 6f6c 2d69 642d  sable=g-bool-id-
-00013980: 636f 6d70 6172 6973 6f6e 0a20 2020 2063  comparison.    c
-00013990: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
-000139a0: 6174 6573 203d 2063 6170 7475 7265 5f63  ates = capture_c
-000139b0: 616c 6c5f 696e 7465 726d 6564 6961 7465  all_intermediate
-000139c0: 730a 2020 6966 2063 6170 7475 7265 5f69  s.  if capture_i
-000139d0: 6e74 6572 6d65 6469 6174 6573 3a0a 2020  ntermediates:.  
-000139e0: 2020 6d75 7461 626c 6520 3d20 756e 696f    mutable = unio
-000139f0: 6e5f 6669 6c74 6572 7328 6d75 7461 626c  n_filters(mutabl
-00013a00: 652c 2027 696e 7465 726d 6564 6961 7465  e, 'intermediate
-00013a10: 7327 290a 2020 7265 7475 726e 2063 6f72  s').  return cor
-00013a20: 652e 6170 706c 7928 7363 6f70 655f 666e  e.apply(scope_fn
-00013a30: 2c20 6d75 7461 626c 653d 6d75 7461 626c  , mutable=mutabl
-00013a40: 6529 0a0a 0a40 7472 6163 6562 6163 6b5f  e)...@traceback_
-00013a50: 7574 696c 2e61 7069 5f62 6f75 6e64 6172  util.api_boundar
-00013a60: 790a 6465 6620 696e 6974 5f77 6974 685f  y.def init_with_
-00013a70: 6f75 7470 7574 2866 6e3a 2043 616c 6c61  output(fn: Calla
-00013a80: 626c 655b 2e2e 2e2c 2041 6e79 5d2c 206d  ble[..., Any], m
-00013a90: 6f64 756c 653a 204d 6f64 756c 652c 0a20  odule: Module,. 
-00013aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ab0: 2020 2020 6d75 7461 626c 653a 2043 6f6c      mutable: Col
-00013ac0: 6c65 6374 696f 6e46 696c 7465 7220 3d20  lectionFilter = 
-00013ad0: 4465 6e79 4c69 7374 2827 696e 7465 726d  DenyList('interm
-00013ae0: 6564 6961 7465 7327 292c 0a20 2020 2020  ediates'),.     
-00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b00: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
-00013b10: 6961 7465 733a 2055 6e69 6f6e 5b62 6f6f  iates: Union[boo
-00013b20: 6c2c 2043 616c 6c61 626c 655b 5b4d 6f64  l, Callable[[Mod
-00013b30: 756c 652c 2073 7472 5d2c 2062 6f6f 6c5d  ule, str], bool]
-00013b40: 5d20 3d20 4661 6c73 652c 0a20 2020 2020  ] = False,.     
-00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b60: 2920 2d3e 2043 616c 6c61 626c 655b 2e2e  ) -> Callable[..
-00013b70: 2e2c 2054 7570 6c65 5b41 6e79 2c20 556e  ., Tuple[Any, Un
-00013b80: 696f 6e5b 4672 6f7a 656e 5661 7269 6162  ion[FrozenVariab
-00013b90: 6c65 4469 6374 2c20 4469 6374 5b73 7472  leDict, Dict[str
-00013ba0: 2c20 416e 795d 5d5d 5d3a 0a20 2022 2222  , Any]]]]:.  """
-00013bb0: 4372 6561 7465 7320 616e 2069 6e69 7420  Creates an init 
-00013bc0: 6675 6e63 7469 6f6e 2074 6f20 6361 6c6c  function to call
-00013bd0: 2060 6066 6e60 6020 7769 7468 2061 2062   ``fn`` with a b
-00013be0: 6f75 6e64 206d 6f64 756c 6520 7468 6174  ound module that
-00013bf0: 2061 6c73 6f20 7265 7475 726e 7320 7468   also returns th
-00013c00: 6520 6675 6e63 7469 6f6e 206f 7574 7075  e function outpu
-00013c10: 7473 2e0a 0a20 2055 6e6c 696b 6520 6060  ts...  Unlike ``
-00013c20: 4d6f 6475 6c65 2e69 6e69 745f 7769 7468  Module.init_with
-00013c30: 5f6f 7574 7075 7460 6020 7468 6973 2066  _output`` this f
-00013c40: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
-00013c50: 6120 6e65 7720 6675 6e63 7469 6f6e 2077  a new function w
-00013c60: 6974 6820 7468 6520 7369 676e 6174 7572  ith the signatur
-00013c70: 650a 2020 6060 2872 6e67 732c 202a 6172  e.  ``(rngs, *ar
-00013c80: 6773 2c20 2a2a 6b77 6172 6773 2920 2d3e  gs, **kwargs) ->
-00013c90: 2028 542c 2076 6172 6961 626c 6573 2960   (T, variables)`
-00013ca0: 6020 7768 6572 6520 6054 6020 6973 2074  ` where `T` is t
-00013cb0: 6865 2072 6574 7572 6e20 7479 7065 206f  he return type o
-00013cc0: 6620 6060 666e 6060 2e0a 2020 5468 6520  f ``fn``..  The 
-00013cd0: 726e 6773 2063 616e 2062 6520 6120 6469  rngs can be a di
-00013ce0: 6374 206f 6620 5052 4e47 4b65 7973 206f  ct of PRNGKeys o
-00013cf0: 7220 6120 7369 6e67 6c65 2060 6060 5052  r a single ```PR
-00013d00: 4e47 4b65 7960 6020 7768 6963 6820 6973  NGKey`` which is
-00013d10: 0a20 2065 7175 6976 616c 656e 7420 746f  .  equivalent to
-00013d20: 2070 6173 7369 6e67 2061 2064 6963 7420   passing a dict 
-00013d30: 7769 7468 206f 6e65 2050 524e 474b 6579  with one PRNGKey
-00013d40: 2077 6974 6820 7468 6520 6e61 6d65 2022   with the name "
-00013d50: 7061 7261 6d73 222e 0a0a 2020 5468 6520  params"...  The 
-00013d60: 696e 6974 2066 756e 6374 696f 6e20 7468  init function th
-00013d70: 6174 2069 7320 7265 7475 726e 6564 2063  at is returned c
-00013d80: 616e 2062 6520 6469 7265 6374 6c79 2063  an be directly c
-00013d90: 6f6d 706f 7365 6420 7769 7468 0a20 204a  omposed with.  J
-00013da0: 4158 2074 7261 6e73 666f 726d 6174 696f  AX transformatio
-00013db0: 6e73 206c 696b 6520 6060 6a61 782e 6a69  ns like ``jax.ji
-00013dc0: 7460 603a 3a0a 0a20 2020 2064 6566 2066  t``::..    def f
-00013dd0: 2866 6f6f 2c20 7829 3a0a 2020 2020 2020  (foo, x):.      
-00013de0: 7a20 3d20 666f 6f2e 656e 636f 6465 2878  z = foo.encode(x
-00013df0: 290a 2020 2020 2020 7920 3d20 666f 6f2e  ).      y = foo.
-00013e00: 6465 636f 6465 287a 290a 2020 2020 2020  decode(z).      
-00013e10: 2320 2e2e 2e0a 2020 2020 2020 7265 7475  # ....      retu
-00013e20: 726e 2079 0a0a 2020 2020 666f 6f20 3d20  rn y..    foo = 
-00013e30: 466f 6f28 290a 2020 2020 665f 6a69 7474  Foo().    f_jitt
-00013e40: 6564 203d 206a 6178 2e6a 6974 286e 6e2e  ed = jax.jit(nn.
-00013e50: 696e 6974 5f77 6974 685f 6f75 7470 7574  init_with_output
-00013e60: 2866 2c20 666f 6f29 290a 2020 2020 792c  (f, foo)).    y,
-00013e70: 2076 6172 6961 626c 6573 203d 2066 5f6a   variables = f_j
-00013e80: 6974 7465 6428 726e 672c 2078 290a 0a20  itted(rng, x).. 
-00013e90: 2041 7267 733a 0a20 2020 2066 6e3a 2054   Args:.    fn: T
-00013ea0: 6865 2066 756e 6374 696f 6e20 7468 6174  he function that
-00013eb0: 2073 686f 756c 6420 6265 2061 7070 6c69   should be appli
-00013ec0: 6564 2e20 5468 6520 6669 7273 7420 6172  ed. The first ar
-00013ed0: 6775 6d65 6e74 2070 6173 7365 6420 7769  gument passed wi
-00013ee0: 6c6c 0a20 2020 2020 2062 6520 616e 206d  ll.      be an m
-00013ef0: 6f64 756c 6520 696e 7374 616e 6365 206f  odule instance o
-00013f00: 6620 7468 6520 6060 6d6f 6475 6c65 6060  f the ``module``
-00013f10: 2077 6974 6820 7661 7269 6162 6c65 7320   with variables 
-00013f20: 616e 6420 524e 4773 2062 6f75 6e64 0a20  and RNGs bound. 
-00013f30: 2020 2020 2074 6f20 6974 2e0a 2020 2020       to it..    
-00013f40: 6d6f 6475 6c65 3a20 5468 6520 6060 4d6f  module: The ``Mo
-00013f50: 6475 6c65 6060 2074 6861 7420 7769 6c6c  dule`` that will
-00013f60: 2062 6520 7573 6564 2074 6f20 6269 6e64   be used to bind
-00013f70: 2076 6172 6961 626c 6573 2061 6e64 2052   variables and R
-00013f80: 4e47 7320 746f 2e0a 2020 2020 2020 5468  NGs to..      Th
-00013f90: 6520 6060 4d6f 6475 6c65 6060 2070 6173  e ``Module`` pas
-00013fa0: 7365 6420 6173 2074 6865 2066 6972 7374  sed as the first
-00013fb0: 2061 7267 756d 656e 7420 746f 2060 6066   argument to ``f
-00013fc0: 6e60 6020 7769 6c6c 2062 6520 6120 636c  n`` will be a cl
-00013fd0: 6f6e 650a 2020 2020 2020 6f66 206d 6f64  one.      of mod
-00013fe0: 756c 652e 0a20 2020 206d 7574 6162 6c65  ule..    mutable
-00013ff0: 3a20 4361 6e20 6265 2062 6f6f 6c2c 2073  : Can be bool, s
-00014000: 7472 2c20 6f72 206c 6973 742e 2053 7065  tr, or list. Spe
-00014010: 6369 6669 6573 2077 6869 6368 2063 6f6c  cifies which col
-00014020: 6c65 6374 696f 6e73 2073 686f 756c 6420  lections should 
-00014030: 6265 0a20 2020 2020 2074 7265 6174 6564  be.      treated
-00014040: 2061 7320 6d75 7461 626c 653a 2060 6062   as mutable: ``b
-00014050: 6f6f 6c60 603a 2061 6c6c 2f6e 6f20 636f  ool``: all/no co
-00014060: 6c6c 6563 7469 6f6e 7320 6172 6520 6d75  llections are mu
-00014070: 7461 626c 652e 0a20 2020 2020 2060 6073  table..      ``s
-00014080: 7472 6060 3a20 5468 6520 6e61 6d65 206f  tr``: The name o
-00014090: 6620 6120 7369 6e67 6c65 206d 7574 6162  f a single mutab
-000140a0: 6c65 2063 6f6c 6c65 6374 696f 6e2e 2060  le collection. `
-000140b0: 606c 6973 7460 603a 2041 0a20 2020 2020  `list``: A.     
-000140c0: 206c 6973 7420 6f66 206e 616d 6573 206f   list of names o
-000140d0: 6620 6d75 7461 626c 6520 636f 6c6c 6563  f mutable collec
-000140e0: 7469 6f6e 732e 2042 7920 6465 6661 756c  tions. By defaul
-000140f0: 7420 616c 6c20 636f 6c6c 6563 7469 6f6e  t all collection
-00014100: 730a 2020 2020 2020 6578 6365 7074 2022  s.      except "
-00014110: 696e 7465 726d 6564 6961 7465 7322 2061  intermediates" a
-00014120: 7265 206d 7574 6162 6c65 2e0a 2020 2020  re mutable..    
-00014130: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
-00014140: 6961 7465 733a 2049 6620 6054 7275 6560  iates: If `True`
-00014150: 2c20 6361 7074 7572 6573 2069 6e74 6572  , captures inter
-00014160: 6d65 6469 6174 6520 7265 7475 726e 2076  mediate return v
-00014170: 616c 7565 730a 2020 2020 2020 6f66 2061  alues.      of a
-00014180: 6c6c 204d 6f64 756c 6573 2069 6e73 6964  ll Modules insid
-00014190: 6520 7468 6520 2269 6e74 6572 6d65 6469  e the "intermedi
-000141a0: 6174 6573 2220 636f 6c6c 6563 7469 6f6e  ates" collection
-000141b0: 2e20 4279 2064 6566 6175 6c74 206f 6e6c  . By default onl
-000141c0: 790a 2020 2020 2020 7468 6520 7265 7475  y.      the retu
-000141d0: 726e 2076 616c 7565 7320 6f66 2061 6c6c  rn values of all
-000141e0: 2060 5f5f 6361 6c6c 5f5f 6020 6d65 7468   `__call__` meth
-000141f0: 6f64 7320 6172 6520 7374 6f72 6564 2e20  ods are stored. 
-00014200: 4120 6675 6e63 7469 6f6e 2063 616e 0a20  A function can. 
-00014210: 2020 2020 2062 6520 7061 7373 6564 2074       be passed t
-00014220: 6f20 6368 616e 6765 2074 6865 2066 696c  o change the fil
-00014230: 7465 7220 6265 6861 7669 6f72 2e20 5468  ter behavior. Th
-00014240: 6520 6669 6c74 6572 2066 756e 6374 696f  e filter functio
-00014250: 6e20 7461 6b65 730a 2020 2020 2020 7468  n takes.      th
-00014260: 6520 4d6f 6475 6c65 2069 6e73 7461 6e63  e Module instanc
-00014270: 6520 616e 6420 6d65 7468 6f64 206e 616d  e and method nam
-00014280: 6520 616e 6420 7265 7475 726e 7320 6120  e and returns a 
-00014290: 626f 6f6c 2069 6e64 6963 6174 696e 670a  bool indicating.
-000142a0: 2020 2020 2020 7768 6574 6865 7220 7468        whether th
-000142b0: 6520 6f75 7470 7574 206f 6620 7468 6174  e output of that
-000142c0: 206d 6574 686f 6420 696e 766f 6361 7469   method invocati
-000142d0: 6f6e 2073 686f 756c 6420 6265 2073 746f  on should be sto
-000142e0: 7265 642e 0a20 2052 6574 7572 6e73 3a0a  red..  Returns:.
-000142f0: 2020 2020 5468 6520 696e 6974 2066 756e      The init fun
-00014300: 6374 696f 6e20 7772 6170 7069 6e67 2060  ction wrapping `
-00014310: 6066 6e60 602e 0a20 2022 2222 0a20 2040  `fn``..  """.  @
-00014320: 6675 6e63 746f 6f6c 732e 7772 6170 7328  functools.wraps(
-00014330: 666e 290a 2020 6465 6620 7363 6f70 655f  fn).  def scope_
-00014340: 666e 2873 636f 7065 2c20 2a61 7267 732c  fn(scope, *args,
-00014350: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00014360: 5f63 6f6e 7465 7874 2e63 6170 7475 7265  _context.capture
-00014370: 5f73 7461 636b 2e61 7070 656e 6428 6361  _stack.append(ca
-00014380: 7074 7572 655f 696e 7465 726d 6564 6961  pture_intermedia
-00014390: 7465 7329 0a20 2020 2074 7279 3a0a 2020  tes).    try:.  
-000143a0: 2020 2020 7265 7475 726e 2066 6e28 6d6f      return fn(mo
-000143b0: 6475 6c65 2e63 6c6f 6e65 2870 6172 656e  dule.clone(paren
-000143c0: 743d 7363 6f70 6529 2c20 2a61 7267 732c  t=scope), *args,
-000143d0: 202a 2a6b 7761 7267 7329 0a20 2020 2066   **kwargs).    f
-000143e0: 696e 616c 6c79 3a0a 2020 2020 2020 5f63  inally:.      _c
-000143f0: 6f6e 7465 7874 2e63 6170 7475 7265 5f73  ontext.capture_s
-00014400: 7461 636b 2e70 6f70 2829 0a0a 2020 6966  tack.pop()..  if
-00014410: 2063 6170 7475 7265 5f69 6e74 6572 6d65   capture_interme
-00014420: 6469 6174 6573 2069 7320 5472 7565 3a20  diates is True: 
-00014430: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-00014440: 6c65 3d67 2d62 6f6f 6c2d 6964 2d63 6f6d  le=g-bool-id-com
-00014450: 7061 7269 736f 6e0a 2020 2020 6361 7074  parison.    capt
-00014460: 7572 655f 696e 7465 726d 6564 6961 7465  ure_intermediate
-00014470: 7320 3d20 6361 7074 7572 655f 6361 6c6c  s = capture_call
-00014480: 5f69 6e74 6572 6d65 6469 6174 6573 0a20  _intermediates. 
-00014490: 2069 6620 6361 7074 7572 655f 696e 7465   if capture_inte
-000144a0: 726d 6564 6961 7465 733a 0a20 2020 206d  rmediates:.    m
-000144b0: 7574 6162 6c65 203d 2075 6e69 6f6e 5f66  utable = union_f
-000144c0: 696c 7465 7273 286d 7574 6162 6c65 2c20  ilters(mutable, 
-000144d0: 2769 6e74 6572 6d65 6469 6174 6573 2729  'intermediates')
-000144e0: 0a20 2072 6574 7572 6e20 636f 7265 2e69  .  return core.i
-000144f0: 6e69 7428 7363 6f70 655f 666e 2c20 6d75  nit(scope_fn, mu
-00014500: 7461 626c 653d 6d75 7461 626c 6529 0a0a  table=mutable)..
-00014510: 0a40 7472 6163 6562 6163 6b5f 7574 696c  .@traceback_util
-00014520: 2e61 7069 5f62 6f75 6e64 6172 790a 6465  .api_boundary.de
-00014530: 6620 696e 6974 2866 6e3a 2043 616c 6c61  f init(fn: Calla
-00014540: 626c 655b 2e2e 2e2c 2041 6e79 5d2c 206d  ble[..., Any], m
-00014550: 6f64 756c 653a 204d 6f64 756c 652c 0a20  odule: Module,. 
-00014560: 2020 2020 2020 2020 6d75 7461 626c 653a          mutable:
-00014570: 2043 6f6c 6c65 6374 696f 6e46 696c 7465   CollectionFilte
-00014580: 7220 3d20 4465 6e79 4c69 7374 2827 696e  r = DenyList('in
-00014590: 7465 726d 6564 6961 7465 7327 292c 0a20  termediates'),. 
-000145a0: 2020 2020 2020 2020 6361 7074 7572 655f          capture_
-000145b0: 696e 7465 726d 6564 6961 7465 733a 2055  intermediates: U
-000145c0: 6e69 6f6e 5b62 6f6f 6c2c 2043 616c 6c61  nion[bool, Calla
-000145d0: 626c 655b 5b4d 6f64 756c 652c 2073 7472  ble[[Module, str
-000145e0: 5d2c 2062 6f6f 6c5d 5d20 3d20 4661 6c73  ], bool]] = Fals
-000145f0: 652c 0a20 2020 2020 2020 2020 2920 2d3e  e,.         ) ->
-00014600: 2043 616c 6c61 626c 655b 2e2e 2e2c 2055   Callable[..., U
-00014610: 6e69 6f6e 5b46 726f 7a65 6e56 6172 6961  nion[FrozenVaria
-00014620: 626c 6544 6963 742c 2044 6963 745b 7374  bleDict, Dict[st
-00014630: 722c 2041 6e79 5d5d 5d3a 0a20 2022 2222  r, Any]]]:.  """
-00014640: 4372 6561 7465 7320 616e 2069 6e69 7420  Creates an init 
-00014650: 6675 6e63 7469 6f6e 2074 6f20 6361 6c6c  function to call
-00014660: 2060 6066 6e60 6020 7769 7468 2061 2062   ``fn`` with a b
-00014670: 6f75 6e64 206d 6f64 756c 652e 0a0a 2020  ound module...  
-00014680: 556e 6c69 6b65 2060 604d 6f64 756c 652e  Unlike ``Module.
-00014690: 696e 6974 6060 2074 6869 7320 6675 6e63  init`` this func
-000146a0: 7469 6f6e 2072 6574 7572 6e73 2061 206e  tion returns a n
-000146b0: 6577 2066 756e 6374 696f 6e20 7769 7468  ew function with
-000146c0: 2074 6865 2073 6967 6e61 7475 7265 0a20   the signature. 
-000146d0: 2060 6028 726e 6773 2c20 2a61 7267 732c   ``(rngs, *args,
-000146e0: 202a 2a6b 7761 7267 7329 202d 3e20 7661   **kwargs) -> va
-000146f0: 7269 6162 6c65 7360 602e 0a20 2054 6865  riables``..  The
-00014700: 2072 6e67 7320 6361 6e20 6265 2061 2064   rngs can be a d
-00014710: 6963 7420 6f66 2050 524e 474b 6579 7320  ict of PRNGKeys 
-00014720: 6f72 2061 2073 696e 676c 6520 6060 6050  or a single ```P
-00014730: 524e 474b 6579 6060 2077 6869 6368 2069  RNGKey`` which i
-00014740: 730a 2020 6571 7569 7661 6c65 6e74 2074  s.  equivalent t
-00014750: 6f20 7061 7373 696e 6720 6120 6469 6374  o passing a dict
-00014760: 2077 6974 6820 6f6e 6520 5052 4e47 4b65   with one PRNGKe
-00014770: 7920 7769 7468 2074 6865 206e 616d 6520  y with the name 
-00014780: 2270 6172 616d 7322 2e0a 0a20 2054 6865  "params"...  The
-00014790: 2069 6e69 7420 6675 6e63 7469 6f6e 2074   init function t
-000147a0: 6861 7420 6973 2072 6574 7572 6e65 6420  hat is returned 
-000147b0: 6361 6e20 6265 2064 6972 6563 746c 7920  can be directly 
-000147c0: 636f 6d70 6f73 6564 2077 6974 680a 2020  composed with.  
-000147d0: 4a41 5820 7472 616e 7366 6f72 6d61 7469  JAX transformati
-000147e0: 6f6e 7320 6c69 6b65 2060 606a 6178 2e6a  ons like ``jax.j
-000147f0: 6974 6060 3a3a 0a0a 2020 2020 6465 6620  it``::..    def 
-00014800: 6628 666f 6f2c 2078 293a 0a20 2020 2020  f(foo, x):.     
-00014810: 207a 203d 2066 6f6f 2e65 6e63 6f64 6528   z = foo.encode(
-00014820: 7829 0a20 2020 2020 2079 203d 2066 6f6f  x).      y = foo
-00014830: 2e64 6563 6f64 6528 7a29 0a20 2020 2020  .decode(z).     
-00014840: 2023 202e 2e2e 0a20 2020 2020 2072 6574   # ....      ret
-00014850: 7572 6e20 790a 0a20 2020 2066 6f6f 203d  urn y..    foo =
-00014860: 2046 6f6f 2829 0a20 2020 2066 5f6a 6974   Foo().    f_jit
-00014870: 7465 6420 3d20 6a61 782e 6a69 7428 6e6e  ted = jax.jit(nn
-00014880: 2e69 6e69 7428 662c 2066 6f6f 2929 0a20  .init(f, foo)). 
-00014890: 2020 2076 6172 6961 626c 6573 203d 2066     variables = f
-000148a0: 5f6a 6974 7465 6428 726e 672c 2078 290a  _jitted(rng, x).
-000148b0: 0a20 2041 7267 733a 0a20 2020 2066 6e3a  .  Args:.    fn:
-000148c0: 2054 6865 2066 756e 6374 696f 6e20 7468   The function th
-000148d0: 6174 2073 686f 756c 6420 6265 2061 7070  at should be app
-000148e0: 6c69 6564 2e20 5468 6520 6669 7273 7420  lied. The first 
-000148f0: 6172 6775 6d65 6e74 2070 6173 7365 6420  argument passed 
-00014900: 7769 6c6c 0a20 2020 2020 2062 6520 616e  will.      be an
-00014910: 206d 6f64 756c 6520 696e 7374 616e 6365   module instance
-00014920: 206f 6620 7468 6520 6060 6d6f 6475 6c65   of the ``module
-00014930: 6060 2077 6974 6820 7661 7269 6162 6c65  `` with variable
-00014940: 7320 616e 6420 524e 4773 2062 6f75 6e64  s and RNGs bound
-00014950: 0a20 2020 2020 2074 6f20 6974 2e0a 2020  .      to it..  
-00014960: 2020 6d6f 6475 6c65 3a20 5468 6520 6060    module: The ``
-00014970: 4d6f 6475 6c65 6060 2074 6861 7420 7769  Module`` that wi
-00014980: 6c6c 2062 6520 7573 6564 2074 6f20 6269  ll be used to bi
-00014990: 6e64 2076 6172 6961 626c 6573 2061 6e64  nd variables and
-000149a0: 2052 4e47 7320 746f 2e0a 2020 2020 2020   RNGs to..      
-000149b0: 5468 6520 6060 4d6f 6475 6c65 6060 2070  The ``Module`` p
-000149c0: 6173 7365 6420 6173 2074 6865 2066 6972  assed as the fir
-000149d0: 7374 2061 7267 756d 656e 7420 746f 2060  st argument to `
-000149e0: 6066 6e60 6020 7769 6c6c 2062 6520 6120  `fn`` will be a 
-000149f0: 636c 6f6e 650a 2020 2020 2020 6f66 206d  clone.      of m
-00014a00: 6f64 756c 652e 0a20 2020 206d 7574 6162  odule..    mutab
-00014a10: 6c65 3a20 4361 6e20 6265 2062 6f6f 6c2c  le: Can be bool,
-00014a20: 2073 7472 2c20 6f72 206c 6973 742e 2053   str, or list. S
-00014a30: 7065 6369 6669 6573 2077 6869 6368 2063  pecifies which c
-00014a40: 6f6c 6c65 6374 696f 6e73 2073 686f 756c  ollections shoul
-00014a50: 6420 6265 0a20 2020 2020 2074 7265 6174  d be.      treat
-00014a60: 6564 2061 7320 6d75 7461 626c 653a 2060  ed as mutable: `
-00014a70: 6062 6f6f 6c60 603a 2061 6c6c 2f6e 6f20  `bool``: all/no 
-00014a80: 636f 6c6c 6563 7469 6f6e 7320 6172 6520  collections are 
-00014a90: 6d75 7461 626c 652e 0a20 2020 2020 2060  mutable..      `
-00014aa0: 6073 7472 6060 3a20 5468 6520 6e61 6d65  `str``: The name
-00014ab0: 206f 6620 6120 7369 6e67 6c65 206d 7574   of a single mut
-00014ac0: 6162 6c65 2063 6f6c 6c65 6374 696f 6e2e  able collection.
-00014ad0: 2060 606c 6973 7460 603a 2041 0a20 2020   ``list``: A.   
-00014ae0: 2020 206c 6973 7420 6f66 206e 616d 6573     list of names
-00014af0: 206f 6620 6d75 7461 626c 6520 636f 6c6c   of mutable coll
-00014b00: 6563 7469 6f6e 732e 2042 7920 6465 6661  ections. By defa
-00014b10: 756c 7420 616c 6c20 636f 6c6c 6563 7469  ult all collecti
-00014b20: 6f6e 730a 2020 2020 2020 6578 6365 7074  ons.      except
-00014b30: 2022 696e 7465 726d 6564 6961 7465 7322   "intermediates"
-00014b40: 2061 7265 206d 7574 6162 6c65 2e0a 2020   are mutable..  
-00014b50: 2020 6361 7074 7572 655f 696e 7465 726d    capture_interm
-00014b60: 6564 6961 7465 733a 2049 6620 6054 7275  ediates: If `Tru
-00014b70: 6560 2c20 6361 7074 7572 6573 2069 6e74  e`, captures int
-00014b80: 6572 6d65 6469 6174 6520 7265 7475 726e  ermediate return
-00014b90: 2076 616c 7565 730a 2020 2020 2020 6f66   values.      of
-00014ba0: 2061 6c6c 204d 6f64 756c 6573 2069 6e73   all Modules ins
-00014bb0: 6964 6520 7468 6520 2269 6e74 6572 6d65  ide the "interme
-00014bc0: 6469 6174 6573 2220 636f 6c6c 6563 7469  diates" collecti
-00014bd0: 6f6e 2e20 4279 2064 6566 6175 6c74 206f  on. By default o
-00014be0: 6e6c 790a 2020 2020 2020 7468 6520 7265  nly.      the re
-00014bf0: 7475 726e 2076 616c 7565 7320 6f66 2061  turn values of a
-00014c00: 6c6c 2060 5f5f 6361 6c6c 5f5f 6020 6d65  ll `__call__` me
-00014c10: 7468 6f64 7320 6172 6520 7374 6f72 6564  thods are stored
-00014c20: 2e20 4120 6675 6e63 7469 6f6e 2063 616e  . A function can
-00014c30: 0a20 2020 2020 2062 6520 7061 7373 6564  .      be passed
-00014c40: 2074 6f20 6368 616e 6765 2074 6865 2066   to change the f
-00014c50: 696c 7465 7220 6265 6861 7669 6f72 2e20  ilter behavior. 
-00014c60: 5468 6520 6669 6c74 6572 2066 756e 6374  The filter funct
-00014c70: 696f 6e20 7461 6b65 730a 2020 2020 2020  ion takes.      
-00014c80: 7468 6520 4d6f 6475 6c65 2069 6e73 7461  the Module insta
-00014c90: 6e63 6520 616e 6420 6d65 7468 6f64 206e  nce and method n
-00014ca0: 616d 6520 616e 6420 7265 7475 726e 7320  ame and returns 
-00014cb0: 6120 626f 6f6c 2069 6e64 6963 6174 696e  a bool indicatin
-00014cc0: 670a 2020 2020 2020 7768 6574 6865 7220  g.      whether 
-00014cd0: 7468 6520 6f75 7470 7574 206f 6620 7468  the output of th
-00014ce0: 6174 206d 6574 686f 6420 696e 766f 6361  at method invoca
-00014cf0: 7469 6f6e 2073 686f 756c 6420 6265 2073  tion should be s
-00014d00: 746f 7265 642e 0a20 2052 6574 7572 6e73  tored..  Returns
-00014d10: 3a0a 2020 2020 5468 6520 696e 6974 2066  :.    The init f
-00014d20: 756e 6374 696f 6e20 7772 6170 7069 6e67  unction wrapping
-00014d30: 2060 6066 6e60 602e 0a20 2022 2222 0a20   ``fn``..  """. 
-00014d40: 2069 6e69 745f 666e 203d 2069 6e69 745f   init_fn = init_
-00014d50: 7769 7468 5f6f 7574 7075 7428 666e 2c20  with_output(fn, 
-00014d60: 6d6f 6475 6c65 2c20 6d75 7461 626c 652c  module, mutable,
-00014d70: 2063 6170 7475 7265 5f69 6e74 6572 6d65   capture_interme
-00014d80: 6469 6174 6573 290a 2020 4066 756e 6374  diates).  @funct
-00014d90: 6f6f 6c73 2e77 7261 7073 2869 6e69 745f  ools.wraps(init_
-00014da0: 666e 290a 2020 6465 6620 696e 6974 5f77  fn).  def init_w
-00014db0: 7261 7070 6572 282a 6172 6773 2c20 2a2a  rapper(*args, **
-00014dc0: 6b77 6172 6773 293a 0a20 2020 2072 6574  kwargs):.    ret
-00014dd0: 7572 6e20 696e 6974 5f66 6e28 2a61 7267  urn init_fn(*arg
-00014de0: 732c 202a 2a6b 7761 7267 7329 5b31 5d0a  s, **kwargs)[1].
-00014df0: 2020 7265 7475 726e 2069 6e69 745f 7772    return init_wr
-00014e00: 6170 7065 720a                           apper.
+00012320: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
+00012330: 0a20 2020 2020 20e2 9482 2044 656e 7365  .      ... Dense
+00012340: 5f31 20e2 9482 2044 656e 7365 2020 e294  _1 ... Dense  ..
+00012350: 8220 666c 6f61 7433 325b 3136 2c34 5d20  . float32[16,4] 
+00012360: e294 8220 666c 6f61 7433 325b 3136 2c32  ... float32[16,2
+00012370: 5d20 e294 8220 6269 6173 3a20 666c 6f61  ] ... bias: floa
+00012380: 7433 325b 325d 2020 2020 20e2 9482 0a20  t32[2]     .... 
+00012390: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
+000123a0: 20e2 9482 2020 2020 2020 2020 e294 8220   ...        ... 
+000123b0: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+000123c0: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+000123d0: e294 8220 6b65 726e 656c 3a20 666c 6f61  ... kernel: floa
+000123e0: 7433 325b 342c 325d 20e2 9482 0a20 2020  t32[4,2] ....   
+000123f0: 2020 20e2 9482 2020 2020 2020 2020 20e2     ...         .
+00012400: 9482 2020 2020 2020 2020 e294 8220 2020  ..        ...   
+00012410: 2020 2020 2020 2020 2020 2020 e294 8220              ... 
+00012420: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+00012430: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00012440: 2020 2020 2020 20e2 9482 0a20 2020 2020         ....     
+00012450: 20e2 9482 2020 2020 2020 2020 20e2 9482   ...         ...
+00012460: 2020 2020 2020 2020 e294 8220 2020 2020          ...     
+00012470: 2020 2020 2020 2020 2020 e294 8220 2020            ...   
+00012480: 2020 2020 2020 2020 2020 2020 e294 8220              ... 
+00012490: 3130 2028 3430 2042 2920 2020 2020 2020  10 (40 B)       
+000124a0: 2020 2020 20e2 9482 0a20 2020 2020 20e2       ....      .
+000124b0: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
+000124c0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+000124d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000124e0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+000124f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012500: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012510: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+00012520: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012530: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012540: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+00012550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012580: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
+00012590: 0a20 2020 2020 20e2 9482 2020 2020 2020  .      ...      
+000125a0: 2020 20e2 9482 2020 2020 2020 2020 e294     ...        ..
+000125b0: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+000125c0: e294 8220 2020 2020 2020 2020 546f 7461  ...         Tota
+000125d0: 6c20 e294 8220 3530 2028 3230 3020 4229  l ... 50 (200 B)
+000125e0: 2020 2020 2020 2020 2020 20e2 9482 0a20             .... 
+000125f0: 2020 2020 20e2 9494 e294 80e2 9480 e294       ...........
+00012600: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012610: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+00012620: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012630: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012640: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012650: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012660: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012690: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000126a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000126b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000126c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000126d0: e294 80e2 9498 0a0a 2020 2020 2020 2020  ........        
+000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126f0: 2020 2020 546f 7461 6c20 5061 7261 6d65      Total Parame
+00012700: 7465 7273 3a20 3530 2028 3230 3020 4229  ters: 50 (200 B)
+00012710: 0a0a 2020 2020 2a2a 4e6f 7465 2a2a 3a20  ..    **Note**: 
+00012720: 726f 7773 206f 7264 6572 2069 6e20 7468  rows order in th
+00012730: 6520 7461 626c 6520 646f 6573 206e 6f74  e table does not
+00012740: 2072 6570 7265 7365 6e74 2065 7865 6375   represent execu
+00012750: 7469 6f6e 206f 7264 6572 2c0a 2020 2020  tion order,.    
+00012760: 696e 7374 6561 6420 6974 2061 6c69 676e  instead it align
+00012770: 7320 7769 7468 2074 6865 206f 7264 6572  s with the order
+00012780: 206f 6620 6b65 7973 2069 6e20 6076 6172   of keys in `var
+00012790: 6961 626c 6573 6020 7768 6963 6820 6172  iables` which ar
+000127a0: 6520 736f 7274 6564 0a20 2020 2061 6c70  e sorted.    alp
+000127b0: 6861 6265 7469 6361 6c6c 792e 0a0a 2020  habetically...  
+000127c0: 2020 4172 6773 3a0a 2020 2020 2020 726e    Args:.      rn
+000127d0: 6773 3a20 5468 6520 726e 6773 2066 6f72  gs: The rngs for
+000127e0: 2074 6865 2076 6172 6961 626c 6520 636f   the variable co
+000127f0: 6c6c 6563 7469 6f6e 7320 6173 2070 6173  llections as pas
+00012800: 7365 6420 746f 2060 4d6f 6475 6c65 2e69  sed to `Module.i
+00012810: 6e69 7460 2e0a 2020 2020 2020 2a61 7267  nit`..      *arg
+00012820: 733a 2054 6865 2061 7267 756d 656e 7473  s: The arguments
+00012830: 2074 6f20 7468 6520 666f 7277 6172 6420   to the forward 
+00012840: 636f 6d70 7574 6174 696f 6e2e 0a20 2020  computation..   
+00012850: 2020 2064 6570 7468 3a20 636f 6e74 726f     depth: contro
+00012860: 6c73 2068 6f77 206d 616e 7920 7375 626d  ls how many subm
+00012870: 6f64 756c 6520 6465 6570 2074 6865 2073  odule deep the s
+00012880: 756d 6d61 7279 2063 616e 2067 6f2e 2042  ummary can go. B
+00012890: 7920 6465 6661 756c 7420 6974 730a 2020  y default its.  
+000128a0: 2020 2020 2020 604e 6f6e 6560 2077 6869        `None` whi
+000128b0: 6368 206d 6561 6e73 206e 6f20 6c69 6d69  ch means no limi
+000128c0: 742e 2049 6620 6120 7375 626d 6f64 756c  t. If a submodul
+000128d0: 6520 6973 206e 6f74 2073 686f 776e 2062  e is not shown b
+000128e0: 6563 6175 7365 206f 6620 7468 650a 2020  ecause of the.  
+000128f0: 2020 2020 2020 6465 7074 6820 6c69 6d69        depth limi
+00012900: 742c 2069 7473 2070 6172 616d 6574 6572  t, its parameter
+00012910: 2063 6f75 6e74 2061 6e64 2062 7974 6573   count and bytes
+00012920: 2077 696c 6c20 6265 2061 6464 6564 2074   will be added t
+00012930: 6f20 7468 6520 726f 7720 6f66 2069 7473  o the row of its
+00012940: 0a20 2020 2020 2020 2066 6972 7374 2073  .        first s
+00012950: 686f 776e 2061 6e63 6573 746f 7220 7375  hown ancestor su
+00012960: 6368 2074 6861 7420 7468 6520 7375 6d20  ch that the sum 
+00012970: 6f66 2061 6c6c 2072 6f77 7320 616c 7761  of all rows alwa
+00012980: 7973 2061 6464 7320 7570 2074 6f20 7468  ys adds up to th
+00012990: 650a 2020 2020 2020 2020 746f 7461 6c20  e.        total 
+000129a0: 6e75 6d62 6572 206f 6620 7061 7261 6d65  number of parame
+000129b0: 7465 7273 206f 6620 7468 6520 4d6f 6475  ters of the Modu
+000129c0: 6c65 2e0a 2020 2020 2020 7368 6f77 5f72  le..      show_r
+000129d0: 6570 6561 7465 643a 2049 6620 6054 7275  epeated: If `Tru
+000129e0: 6560 2c20 7265 7065 6174 6564 2063 616c  e`, repeated cal
+000129f0: 6c73 2074 6f20 7468 6520 7361 6d65 206d  ls to the same m
+00012a00: 6f64 756c 6520 7769 6c6c 2062 6520 7368  odule will be sh
+00012a10: 6f77 6e0a 2020 2020 2020 2020 696e 2074  own.        in t
+00012a20: 6865 2074 6162 6c65 2c20 6f74 6865 7277  he table, otherw
+00012a30: 6973 6520 6f6e 6c79 2074 6865 2066 6972  ise only the fir
+00012a40: 7374 2063 616c 6c20 7769 6c6c 2062 6520  st call will be 
+00012a50: 7368 6f77 6e2e 2044 6566 6175 6c74 2069  shown. Default i
+00012a60: 730a 2020 2020 2020 2020 6046 616c 7365  s.        `False
+00012a70: 602e 0a20 2020 2020 206d 7574 6162 6c65  `..      mutable
+00012a80: 3a20 4361 6e20 6265 2062 6f6f 6c2c 2073  : Can be bool, s
+00012a90: 7472 2c20 6f72 206c 6973 742e 2053 7065  tr, or list. Spe
+00012aa0: 6369 6669 6573 2077 6869 6368 2063 6f6c  cifies which col
+00012ab0: 6c65 6374 696f 6e73 2073 686f 756c 6420  lections should 
+00012ac0: 6265 0a20 2020 2020 2020 2074 7265 6174  be.        treat
+00012ad0: 6564 2061 7320 6d75 7461 626c 653a 2060  ed as mutable: `
+00012ae0: 6062 6f6f 6c60 603a 2061 6c6c 2f6e 6f20  `bool``: all/no 
+00012af0: 636f 6c6c 6563 7469 6f6e 7320 6172 6520  collections are 
+00012b00: 6d75 7461 626c 652e 2060 6073 7472 6060  mutable. ``str``
+00012b10: 3a20 5468 650a 2020 2020 2020 2020 6e61  : The.        na
+00012b20: 6d65 206f 6620 6120 7369 6e67 6c65 206d  me of a single m
+00012b30: 7574 6162 6c65 2063 6f6c 6c65 6374 696f  utable collectio
+00012b40: 6e2e 2060 606c 6973 7460 603a 2041 206c  n. ``list``: A l
+00012b50: 6973 7420 6f66 206e 616d 6573 206f 6620  ist of names of 
+00012b60: 6d75 7461 626c 650a 2020 2020 2020 2020  mutable.        
+00012b70: 636f 6c6c 6563 7469 6f6e 732e 2042 7920  collections. By 
+00012b80: 6465 6661 756c 7420 616c 6c20 636f 6c6c  default all coll
+00012b90: 6563 7469 6f6e 7320 6578 6365 7074 2027  ections except '
+00012ba0: 696e 7465 726d 6564 6961 7465 7327 2061  intermediates' a
+00012bb0: 7265 0a20 2020 2020 2020 206d 7574 6162  re.        mutab
+00012bc0: 6c65 2e0a 2020 2020 2020 636f 6e73 6f6c  le..      consol
+00012bd0: 655f 6b77 6172 6773 3a20 416e 206f 7074  e_kwargs: An opt
+00012be0: 696f 6e61 6c20 6469 6374 696f 6e61 7279  ional dictionary
+00012bf0: 2077 6974 6820 6164 6469 7469 6f6e 616c   with additional
+00012c00: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00012c10: 7473 2074 6861 740a 2020 2020 2020 2020  ts that.        
+00012c20: 6172 6520 7061 7373 6564 2074 6f20 6072  are passed to `r
+00012c30: 6963 682e 636f 6e73 6f6c 652e 436f 6e73  ich.console.Cons
+00012c40: 6f6c 6560 2077 6865 6e20 7265 6e64 6572  ole` when render
+00012c50: 696e 6720 7468 6520 7461 626c 652e 2044  ing the table. D
+00012c60: 6566 6175 6c74 2061 7267 756d 656e 7473  efault arguments
+00012c70: 0a20 2020 2020 2020 2061 7265 2060 7b27  .        are `{'
+00012c80: 666f 7263 655f 7465 726d 696e 616c 273a  force_terminal':
+00012c90: 2054 7275 652c 2027 666f 7263 655f 6a75   True, 'force_ju
+00012ca0: 7079 7465 7227 3a20 4661 6c73 657d 602e  pyter': False}`.
+00012cb0: 0a20 2020 2020 202a 2a6b 7761 7267 733a  .      **kwargs:
+00012cc0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00012cd0: 7473 2074 6f20 7061 7373 2074 6f20 7468  ts to pass to th
+00012ce0: 6520 666f 7277 6172 6420 636f 6d70 7574  e forward comput
+00012cf0: 6174 696f 6e2e 0a0a 2020 2020 5265 7475  ation...    Retu
+00012d00: 726e 733a 0a20 2020 2020 2041 2073 7472  rns:.      A str
+00012d10: 696e 6720 7375 6d6d 6172 697a 696e 6720  ing summarizing 
+00012d20: 7468 6520 4d6f 6475 6c65 2e0a 2020 2020  the Module..    
+00012d30: 2222 220a 2020 2020 6672 6f6d 2066 6c61  """.    from fla
+00012d40: 782e 6c69 6e65 6e20 696d 706f 7274 2073  x.linen import s
+00012d50: 756d 6d61 7279 0a0a 2020 2020 7461 6275  ummary..    tabu
+00012d60: 6c61 7465 5f66 6e20 3d20 7375 6d6d 6172  late_fn = summar
+00012d70: 792e 7461 6275 6c61 7465 2873 656c 662c  y.tabulate(self,
+00012d80: 2072 6e67 732c 2064 6570 7468 3d64 6570   rngs, depth=dep
+00012d90: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012db0: 2020 2020 2020 2073 686f 775f 7265 7065         show_repe
+00012dc0: 6174 6564 3d73 686f 775f 7265 7065 6174  ated=show_repeat
+00012dd0: 6564 2c20 6d75 7461 626c 653d 6d75 7461  ed, mutable=muta
+00012de0: 626c 652c 0a20 2020 2020 2020 2020 2020  ble,.           
+00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e00: 2020 2020 2020 2020 636f 6e73 6f6c 655f          console_
+00012e10: 6b77 6172 6773 3d63 6f6e 736f 6c65 5f6b  kwargs=console_k
+00012e20: 7761 7267 7329 0a20 2020 2072 6574 7572  wargs).    retur
+00012e30: 6e20 7461 6275 6c61 7465 5f66 6e28 2a61  n tabulate_fn(*a
+00012e40: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
+00012e50: 0a5f 5061 7265 6e74 5479 7065 203d 2055  ._ParentType = U
+00012e60: 6e69 6f6e 5b54 7970 655b 4d6f 6475 6c65  nion[Type[Module
+00012e70: 5d2c 2054 7970 655b 5363 6f70 655d 2c20  ], Type[Scope], 
+00012e80: 5479 7065 5b5f 5365 6e74 696e 656c 5d2c  Type[_Sentinel],
+00012e90: 204e 6f6e 655d 0a0a 6465 6620 6d65 7267   None]..def merg
+00012ea0: 655f 7061 7261 6d28 6e61 6d65 3a20 7374  e_param(name: st
+00012eb0: 722c 2061 3a20 4f70 7469 6f6e 616c 5b54  r, a: Optional[T
+00012ec0: 5d2c 2062 3a20 4f70 7469 6f6e 616c 5b54  ], b: Optional[T
+00012ed0: 5d29 202d 3e20 543a 0a20 2022 2222 4d65  ]) -> T:.  """Me
+00012ee0: 7267 6573 2063 6f6e 7374 7275 6374 696f  rges constructio
+00012ef0: 6e2d 2061 6e64 2063 616c 6c2d 7469 6d65  n- and call-time
+00012f00: 2061 7267 756d 656e 742e 0a0a 2020 5468   argument...  Th
+00012f10: 6973 2069 7320 6120 7574 696c 6974 7920  is is a utility 
+00012f20: 666f 7220 7375 7070 6f72 7469 6e67 2061  for supporting a
+00012f30: 2070 6174 7465 726e 2077 6865 7265 2061   pattern where a
+00012f40: 204d 6f64 756c 6520 6879 7065 7270 6172   Module hyperpar
+00012f50: 616d 6574 6572 0a20 2063 616e 2062 6520  ameter.  can be 
+00012f60: 7061 7373 6564 2065 6974 6865 7220 746f  passed either to
+00012f70: 2060 605f 5f69 6e69 745f 5f60 6020 6f72   ``__init__`` or
+00012f80: 2060 605f 5f63 616c 6c5f 5f60 602c 2061   ``__call__``, a
+00012f90: 6e64 2074 6865 2076 616c 7565 2074 6861  nd the value tha
+00012fa0: 7420 6973 0a20 206e 6f74 2060 4e6f 6e65  t is.  not `None
+00012fb0: 6020 7769 6c6c 2062 6520 7573 6564 2e0a  ` will be used..
+00012fc0: 0a20 2045 7861 6d70 6c65 3a3a 0a0a 2020  .  Example::..  
+00012fd0: 2020 636c 6173 7320 466f 6f28 6e6e 2e4d    class Foo(nn.M
+00012fe0: 6f64 756c 6529 3a0a 2020 2020 2020 7472  odule):.      tr
+00012ff0: 6169 6e3a 204f 7074 696f 6e61 6c5b 626f  ain: Optional[bo
+00013000: 6f6c 5d20 3d20 4e6f 6e65 0a0a 2020 2020  ol] = None..    
+00013010: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+00013020: 656c 662c 2074 7261 696e 3a20 4f70 7469  elf, train: Opti
+00013030: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+00013040: 6529 3a0a 2020 2020 2020 2020 7472 6169  e):.        trai
+00013050: 6e20 3d20 6e6e 2e6d 6572 6765 5f70 6172  n = nn.merge_par
+00013060: 616d 2827 7472 6169 6e27 2c20 7365 6c66  am('train', self
+00013070: 2e74 7261 696e 2c20 7472 6169 6e29 0a0a  .train, train)..
+00013080: 2020 416e 2065 7272 6f72 2069 7320 7468    An error is th
+00013090: 726f 776e 2077 6865 6e20 626f 7468 2061  rown when both a
+000130a0: 7267 756d 656e 7473 2061 7265 2060 4e6f  rguments are `No
+000130b0: 6e65 6020 6f72 2062 6f74 6820 7661 6c75  ne` or both valu
+000130c0: 6573 2061 7265 206e 6f74 0a20 2060 4e6f  es are not.  `No
+000130d0: 6e65 602e 0a0a 2020 4172 6773 3a0a 2020  ne`...  Args:.  
+000130e0: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
+000130f0: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
+00013100: 722e 2055 7365 6420 666f 7220 6572 726f  r. Used for erro
+00013110: 7220 6d65 7373 6167 6573 2e0a 2020 2020  r messages..    
+00013120: 613a 206f 7074 696f 6e20 610a 2020 2020  a: option a.    
+00013130: 623a 206f 7074 696f 6e20 620a 2020 5265  b: option b.  Re
+00013140: 7475 726e 733a 0a20 2020 2061 206f 7220  turns:.    a or 
+00013150: 6220 7768 6963 6865 7665 7220 6973 206e  b whichever is n
+00013160: 6f74 2060 4e6f 6e65 602e 0a0a 2020 2222  ot `None`...  ""
+00013170: 220a 2020 6966 2061 2069 7320 4e6f 6e65  ".  if a is None
+00013180: 2061 6e64 2062 2069 7320 4e6f 6e65 3a0a   and b is None:.
+00013190: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000131a0: 7272 6f72 2866 2750 6172 616d 6574 6572  rror(f'Parameter
+000131b0: 2022 7b6e 616d 657d 2220 6d75 7374 2062   "{name}" must b
+000131c0: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
+000131d0: 636f 6e73 7472 7563 746f 7220 6f72 2061  constructor or a
+000131e0: 7420 6361 6c6c 2074 696d 652e 2729 0a20  t call time.'). 
+000131f0: 2069 6620 6120 6973 206e 6f74 204e 6f6e   if a is not Non
+00013200: 6520 616e 6420 6220 6973 206e 6f74 204e  e and b is not N
+00013210: 6f6e 653a 0a20 2020 2072 6169 7365 2056  one:.    raise V
+00013220: 616c 7565 4572 726f 7228 6627 5061 7261  alueError(f'Para
+00013230: 6d65 7465 7220 227b 6e61 6d65 7d22 2077  meter "{name}" w
+00013240: 6173 2070 6173 7365 6420 746f 2074 6865  as passed to the
+00013250: 2063 6f6e 7374 7275 6374 6f72 2061 6e64   constructor and
+00013260: 2061 7420 6361 6c6c 2074 696d 652e 270a   at call time.'.
+00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013280: 2020 2020 2027 2053 686f 756c 6420 6265       ' Should be
+00013290: 2070 6173 7365 6420 6a75 7374 206f 6e63   passed just onc
+000132a0: 652e 2729 0a20 2069 6620 6120 6973 204e  e.').  if a is N
+000132b0: 6f6e 653a 0a20 2020 2061 7373 6572 7420  one:.    assert 
+000132c0: 6220 6973 206e 6f74 204e 6f6e 650a 2020  b is not None.  
+000132d0: 2020 7265 7475 726e 2062 0a20 2072 6574    return b.  ret
+000132e0: 7572 6e20 610a 0a0a 4074 7261 6365 6261  urn a...@traceba
+000132f0: 636b 5f75 7469 6c2e 6170 695f 626f 756e  ck_util.api_boun
+00013300: 6461 7279 0a64 6566 2061 7070 6c79 2866  dary.def apply(f
+00013310: 6e3a 2043 616c 6c61 626c 655b 2e2e 2e2c  n: Callable[...,
+00013320: 2041 6e79 5d2c 206d 6f64 756c 653a 204d   Any], module: M
+00013330: 6f64 756c 652c 0a20 2020 2020 2020 2020  odule,.         
+00013340: 206d 7574 6162 6c65 3a20 436f 6c6c 6563   mutable: Collec
+00013350: 7469 6f6e 4669 6c74 6572 203d 2046 616c  tionFilter = Fal
+00013360: 7365 2c0a 2020 2020 2020 2020 2020 6361  se,.          ca
+00013370: 7074 7572 655f 696e 7465 726d 6564 6961  pture_intermedia
+00013380: 7465 733a 2055 6e69 6f6e 5b62 6f6f 6c2c  tes: Union[bool,
+00013390: 2043 616c 6c61 626c 655b 5b4d 6f64 756c   Callable[[Modul
+000133a0: 652c 2073 7472 5d2c 2062 6f6f 6c5d 5d20  e, str], bool]] 
+000133b0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+000133c0: 2020 2029 202d 3e20 4361 6c6c 6162 6c65     ) -> Callable
+000133d0: 5b2e 2e2e 2c20 416e 795d 3a0a 2020 2222  [..., Any]:.  ""
+000133e0: 2243 7265 6174 6573 2061 6e20 6170 706c  "Creates an appl
+000133f0: 7920 6675 6e63 7469 6f6e 2074 6f20 6361  y function to ca
+00013400: 6c6c 2060 6066 6e60 6020 7769 7468 2061  ll ``fn`` with a
+00013410: 2062 6f75 6e64 206d 6f64 756c 652e 0a0a   bound module...
+00013420: 2020 556e 6c69 6b65 2060 604d 6f64 756c    Unlike ``Modul
+00013430: 652e 6170 706c 7960 6020 7468 6973 2066  e.apply`` this f
+00013440: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
+00013450: 6120 6e65 7720 6675 6e63 7469 6f6e 2077  a new function w
+00013460: 6974 6820 7468 6520 7369 676e 6174 7572  ith the signatur
+00013470: 650a 2020 6060 2876 6172 6961 626c 6573  e.  ``(variables
+00013480: 2c20 2a61 7267 732c 2072 6e67 733d 4e6f  , *args, rngs=No
+00013490: 6e65 2c20 2a2a 6b77 6172 6773 2920 2d3e  ne, **kwargs) ->
+000134a0: 2054 6060 2077 6865 7265 2060 5460 2069   T`` where `T` i
+000134b0: 7320 7468 6520 7265 7475 726e 2074 7970  s the return typ
+000134c0: 650a 2020 6f66 2060 6066 6e60 602e 2049  e.  of ``fn``. I
+000134d0: 6620 6060 6d75 7461 626c 6560 6020 6973  f ``mutable`` is
+000134e0: 206e 6f74 2060 6046 616c 7365 6060 2074   not ``False`` t
+000134f0: 6865 2072 6574 7572 6e20 7479 7065 2069  he return type i
+00013500: 7320 6120 7475 706c 6520 7768 6572 6520  s a tuple where 
+00013510: 7468 650a 2020 7365 636f 6e64 2069 7465  the.  second ite
+00013520: 6d20 6973 2061 2060 6046 726f 7a65 6e44  m is a ``FrozenD
+00013530: 6963 7460 6020 7769 7468 2074 6865 206d  ict`` with the m
+00013540: 7574 6174 6564 2076 6172 6961 626c 6573  utated variables
+00013550: 2e0a 0a20 2054 6865 2061 7070 6c79 2066  ...  The apply f
+00013560: 756e 6374 696f 6e20 7468 6174 2069 7320  unction that is 
+00013570: 7265 7475 726e 6564 2063 616e 2062 6520  returned can be 
+00013580: 6469 7265 6374 6c79 2063 6f6d 706f 7365  directly compose
+00013590: 6420 7769 7468 0a20 204a 4158 2074 7261  d with.  JAX tra
+000135a0: 6e73 666f 726d 6174 696f 6e73 206c 696b  nsformations lik
+000135b0: 6520 6060 6a61 782e 6a69 7460 603a 3a0a  e ``jax.jit``::.
+000135c0: 0a20 2020 2064 6566 2066 2866 6f6f 2c20  .    def f(foo, 
+000135d0: 7829 3a0a 2020 2020 2020 7a20 3d20 666f  x):.      z = fo
+000135e0: 6f2e 656e 636f 6465 2878 290a 2020 2020  o.encode(x).    
+000135f0: 2020 7920 3d20 666f 6f2e 6465 636f 6465    y = foo.decode
+00013600: 287a 290a 2020 2020 2020 2320 2e2e 2e0a  (z).      # ....
+00013610: 2020 2020 2020 7265 7475 726e 2079 0a0a        return y..
+00013620: 2020 2020 666f 6f20 3d20 466f 6f28 290a      foo = Foo().
+00013630: 2020 2020 665f 6a69 7474 6564 203d 206a      f_jitted = j
+00013640: 6178 2e6a 6974 286e 6e2e 6170 706c 7928  ax.jit(nn.apply(
+00013650: 662c 2066 6f6f 2929 0a20 2020 2066 5f6a  f, foo)).    f_j
+00013660: 6974 7465 6428 7661 7269 6162 6c65 732c  itted(variables,
+00013670: 2078 290a 0a20 2041 7267 733a 0a20 2020   x)..  Args:.   
+00013680: 2066 6e3a 2054 6865 2066 756e 6374 696f   fn: The functio
+00013690: 6e20 7468 6174 2073 686f 756c 6420 6265  n that should be
+000136a0: 2061 7070 6c69 6564 2e20 5468 6520 6669   applied. The fi
+000136b0: 7273 7420 6172 6775 6d65 6e74 2070 6173  rst argument pas
+000136c0: 7365 6420 7769 6c6c 0a20 2020 2020 2062  sed will.      b
+000136d0: 6520 616e 206d 6f64 756c 6520 696e 7374  e an module inst
+000136e0: 616e 6365 206f 6620 7468 6520 6060 6d6f  ance of the ``mo
+000136f0: 6475 6c65 6060 2077 6974 6820 7661 7269  dule`` with vari
+00013700: 6162 6c65 7320 616e 6420 524e 4773 2062  ables and RNGs b
+00013710: 6f75 6e64 0a20 2020 2020 2074 6f20 6974  ound.      to it
+00013720: 2e0a 2020 2020 6d6f 6475 6c65 3a20 5468  ..    module: Th
+00013730: 6520 6060 4d6f 6475 6c65 6060 2074 6861  e ``Module`` tha
+00013740: 7420 7769 6c6c 2062 6520 7573 6564 2074  t will be used t
+00013750: 6f20 6269 6e64 2076 6172 6961 626c 6573  o bind variables
+00013760: 2061 6e64 2052 4e47 7320 746f 2e0a 2020   and RNGs to..  
+00013770: 2020 2020 5468 6520 6060 4d6f 6475 6c65      The ``Module
+00013780: 6060 2070 6173 7365 6420 6173 2074 6865  `` passed as the
+00013790: 2066 6972 7374 2061 7267 756d 656e 7420   first argument 
+000137a0: 746f 2060 6066 6e60 6020 7769 6c6c 2062  to ``fn`` will b
+000137b0: 6520 6120 636c 6f6e 650a 2020 2020 2020  e a clone.      
+000137c0: 6f66 206d 6f64 756c 652e 0a20 2020 206d  of module..    m
+000137d0: 7574 6162 6c65 3a20 4361 6e20 6265 2062  utable: Can be b
+000137e0: 6f6f 6c2c 2073 7472 2c20 6f72 206c 6973  ool, str, or lis
+000137f0: 742e 2053 7065 6369 6669 6573 2077 6869  t. Specifies whi
+00013800: 6368 2063 6f6c 6c65 6374 696f 6e73 2073  ch collections s
+00013810: 686f 756c 6420 6265 0a20 2020 2020 2074  hould be.      t
+00013820: 7265 6174 6564 2061 7320 6d75 7461 626c  reated as mutabl
+00013830: 653a 2060 6062 6f6f 6c60 603a 2061 6c6c  e: ``bool``: all
+00013840: 2f6e 6f20 636f 6c6c 6563 7469 6f6e 7320  /no collections 
+00013850: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
+00013860: 2020 2060 6073 7472 6060 3a20 5468 6520     ``str``: The 
+00013870: 6e61 6d65 206f 6620 6120 7369 6e67 6c65  name of a single
+00013880: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
+00013890: 696f 6e2e 2060 606c 6973 7460 603a 2041  ion. ``list``: A
+000138a0: 0a20 2020 2020 206c 6973 7420 6f66 206e  .      list of n
+000138b0: 616d 6573 206f 6620 6d75 7461 626c 6520  ames of mutable 
+000138c0: 636f 6c6c 6563 7469 6f6e 732e 0a20 2020  collections..   
+000138d0: 2063 6170 7475 7265 5f69 6e74 6572 6d65   capture_interme
+000138e0: 6469 6174 6573 3a20 4966 2060 5472 7565  diates: If `True
+000138f0: 602c 2063 6170 7475 7265 7320 696e 7465  `, captures inte
+00013900: 726d 6564 6961 7465 2072 6574 7572 6e20  rmediate return 
+00013910: 7661 6c75 6573 0a20 2020 2020 206f 6620  values.      of 
+00013920: 616c 6c20 4d6f 6475 6c65 7320 696e 7369  all Modules insi
+00013930: 6465 2074 6865 2022 696e 7465 726d 6564  de the "intermed
+00013940: 6961 7465 7322 2063 6f6c 6c65 6374 696f  iates" collectio
+00013950: 6e2e 2042 7920 6465 6661 756c 7420 6f6e  n. By default on
+00013960: 6c79 0a20 2020 2020 2074 6865 2072 6574  ly.      the ret
+00013970: 7572 6e20 7661 6c75 6573 206f 6620 616c  urn values of al
+00013980: 6c20 605f 5f63 616c 6c5f 5f60 206d 6574  l `__call__` met
+00013990: 686f 6473 2061 7265 2073 746f 7265 642e  hods are stored.
+000139a0: 2041 2066 756e 6374 696f 6e20 6361 6e0a   A function can.
+000139b0: 2020 2020 2020 6265 2070 6173 7365 6420        be passed 
+000139c0: 746f 2063 6861 6e67 6520 7468 6520 6669  to change the fi
+000139d0: 6c74 6572 2062 6568 6176 696f 722e 2054  lter behavior. T
+000139e0: 6865 2066 696c 7465 7220 6675 6e63 7469  he filter functi
+000139f0: 6f6e 2074 616b 6573 0a20 2020 2020 2074  on takes.      t
+00013a00: 6865 204d 6f64 756c 6520 696e 7374 616e  he Module instan
+00013a10: 6365 2061 6e64 206d 6574 686f 6420 6e61  ce and method na
+00013a20: 6d65 2061 6e64 2072 6574 7572 6e73 2061  me and returns a
+00013a30: 2062 6f6f 6c20 696e 6469 6361 7469 6e67   bool indicating
+00013a40: 0a20 2020 2020 2077 6865 7468 6572 2074  .      whether t
+00013a50: 6865 206f 7574 7075 7420 6f66 2074 6861  he output of tha
+00013a60: 7420 6d65 7468 6f64 2069 6e76 6f63 6174  t method invocat
+00013a70: 696f 6e20 7368 6f75 6c64 2062 6520 7374  ion should be st
+00013a80: 6f72 6564 2e0a 2020 5265 7475 726e 733a  ored..  Returns:
+00013a90: 0a20 2020 2054 6865 2061 7070 6c79 2066  .    The apply f
+00013aa0: 756e 6374 696f 6e20 7772 6170 7069 6e67  unction wrapping
+00013ab0: 2060 6066 6e60 602e 0a20 2022 2222 0a20   ``fn``..  """. 
+00013ac0: 2040 6675 6e63 746f 6f6c 732e 7772 6170   @functools.wrap
+00013ad0: 7328 666e 290a 2020 6465 6620 7363 6f70  s(fn).  def scop
+00013ae0: 655f 666e 2873 636f 7065 2c20 2a61 7267  e_fn(scope, *arg
+00013af0: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
+00013b00: 2020 5f63 6f6e 7465 7874 2e63 6170 7475    _context.captu
+00013b10: 7265 5f73 7461 636b 2e61 7070 656e 6428  re_stack.append(
+00013b20: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
+00013b30: 6961 7465 7329 0a20 2020 2074 7279 3a0a  iates).    try:.
+00013b40: 2020 2020 2020 7265 7475 726e 2066 6e28        return fn(
+00013b50: 6d6f 6475 6c65 2e63 6c6f 6e65 2870 6172  module.clone(par
+00013b60: 656e 743d 7363 6f70 6529 2c20 2a61 7267  ent=scope), *arg
+00013b70: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
+00013b80: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
+00013b90: 5f63 6f6e 7465 7874 2e63 6170 7475 7265  _context.capture
+00013ba0: 5f73 7461 636b 2e70 6f70 2829 0a0a 2020  _stack.pop()..  
+00013bb0: 6966 2063 6170 7475 7265 5f69 6e74 6572  if capture_inter
+00013bc0: 6d65 6469 6174 6573 2069 7320 5472 7565  mediates is True
+00013bd0: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00013be0: 6162 6c65 3d67 2d62 6f6f 6c2d 6964 2d63  able=g-bool-id-c
+00013bf0: 6f6d 7061 7269 736f 6e0a 2020 2020 6361  omparison.    ca
+00013c00: 7074 7572 655f 696e 7465 726d 6564 6961  pture_intermedia
+00013c10: 7465 7320 3d20 6361 7074 7572 655f 6361  tes = capture_ca
+00013c20: 6c6c 5f69 6e74 6572 6d65 6469 6174 6573  ll_intermediates
+00013c30: 0a20 2069 6620 6361 7074 7572 655f 696e  .  if capture_in
+00013c40: 7465 726d 6564 6961 7465 733a 0a20 2020  termediates:.   
+00013c50: 206d 7574 6162 6c65 203d 2075 6e69 6f6e   mutable = union
+00013c60: 5f66 696c 7465 7273 286d 7574 6162 6c65  _filters(mutable
+00013c70: 2c20 2769 6e74 6572 6d65 6469 6174 6573  , 'intermediates
+00013c80: 2729 0a20 2072 6574 7572 6e20 636f 7265  ').  return core
+00013c90: 2e61 7070 6c79 2873 636f 7065 5f66 6e2c  .apply(scope_fn,
+00013ca0: 206d 7574 6162 6c65 3d6d 7574 6162 6c65   mutable=mutable
+00013cb0: 290a 0a0a 4074 7261 6365 6261 636b 5f75  )...@traceback_u
+00013cc0: 7469 6c2e 6170 695f 626f 756e 6461 7279  til.api_boundary
+00013cd0: 0a64 6566 2069 6e69 745f 7769 7468 5f6f  .def init_with_o
+00013ce0: 7574 7075 7428 666e 3a20 4361 6c6c 6162  utput(fn: Callab
+00013cf0: 6c65 5b2e 2e2e 2c20 416e 795d 2c20 6d6f  le[..., Any], mo
+00013d00: 6475 6c65 3a20 4d6f 6475 6c65 2c0a 2020  dule: Module,.  
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d20: 2020 206d 7574 6162 6c65 3a20 436f 6c6c     mutable: Coll
+00013d30: 6563 7469 6f6e 4669 6c74 6572 203d 2044  ectionFilter = D
+00013d40: 656e 794c 6973 7428 2769 6e74 6572 6d65  enyList('interme
+00013d50: 6469 6174 6573 2729 2c0a 2020 2020 2020  diates'),.      
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013d70: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
+00013d80: 6174 6573 3a20 556e 696f 6e5b 626f 6f6c  ates: Union[bool
+00013d90: 2c20 4361 6c6c 6162 6c65 5b5b 4d6f 6475  , Callable[[Modu
+00013da0: 6c65 2c20 7374 725d 2c20 626f 6f6c 5d5d  le, str], bool]]
+00013db0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+00013dc0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00013dd0: 202d 3e20 4361 6c6c 6162 6c65 5b2e 2e2e   -> Callable[...
+00013de0: 2c20 5475 706c 655b 416e 792c 2055 6e69  , Tuple[Any, Uni
+00013df0: 6f6e 5b46 726f 7a65 6e56 6172 6961 626c  on[FrozenVariabl
+00013e00: 6544 6963 742c 2044 6963 745b 7374 722c  eDict, Dict[str,
+00013e10: 2041 6e79 5d5d 5d5d 3a0a 2020 2222 2243   Any]]]]:.  """C
+00013e20: 7265 6174 6573 2061 6e20 696e 6974 2066  reates an init f
+00013e30: 756e 6374 696f 6e20 746f 2063 616c 6c20  unction to call 
+00013e40: 6060 666e 6060 2077 6974 6820 6120 626f  ``fn`` with a bo
+00013e50: 756e 6420 6d6f 6475 6c65 2074 6861 7420  und module that 
+00013e60: 616c 736f 2072 6574 7572 6e73 2074 6865  also returns the
+00013e70: 2066 756e 6374 696f 6e20 6f75 7470 7574   function output
+00013e80: 732e 0a0a 2020 556e 6c69 6b65 2060 604d  s...  Unlike ``M
+00013e90: 6f64 756c 652e 696e 6974 5f77 6974 685f  odule.init_with_
+00013ea0: 6f75 7470 7574 6060 2074 6869 7320 6675  output`` this fu
+00013eb0: 6e63 7469 6f6e 2072 6574 7572 6e73 2061  nction returns a
+00013ec0: 206e 6577 2066 756e 6374 696f 6e20 7769   new function wi
+00013ed0: 7468 2074 6865 2073 6967 6e61 7475 7265  th the signature
+00013ee0: 0a20 2060 6028 726e 6773 2c20 2a61 7267  .  ``(rngs, *arg
+00013ef0: 732c 202a 2a6b 7761 7267 7329 202d 3e20  s, **kwargs) -> 
+00013f00: 2854 2c20 7661 7269 6162 6c65 7329 6060  (T, variables)``
+00013f10: 2077 6865 7265 2060 5460 2069 7320 7468   where `T` is th
+00013f20: 6520 7265 7475 726e 2074 7970 6520 6f66  e return type of
+00013f30: 2060 6066 6e60 602e 0a20 2054 6865 2072   ``fn``..  The r
+00013f40: 6e67 7320 6361 6e20 6265 2061 2064 6963  ngs can be a dic
+00013f50: 7420 6f66 2050 524e 474b 6579 7320 6f72  t of PRNGKeys or
+00013f60: 2061 2073 696e 676c 6520 6060 6050 524e   a single ```PRN
+00013f70: 474b 6579 6060 2077 6869 6368 2069 730a  GKey`` which is.
+00013f80: 2020 6571 7569 7661 6c65 6e74 2074 6f20    equivalent to 
+00013f90: 7061 7373 696e 6720 6120 6469 6374 2077  passing a dict w
+00013fa0: 6974 6820 6f6e 6520 5052 4e47 4b65 7920  ith one PRNGKey 
+00013fb0: 7769 7468 2074 6865 206e 616d 6520 2270  with the name "p
+00013fc0: 6172 616d 7322 2e0a 0a20 2054 6865 2069  arams"...  The i
+00013fd0: 6e69 7420 6675 6e63 7469 6f6e 2074 6861  nit function tha
+00013fe0: 7420 6973 2072 6574 7572 6e65 6420 6361  t is returned ca
+00013ff0: 6e20 6265 2064 6972 6563 746c 7920 636f  n be directly co
+00014000: 6d70 6f73 6564 2077 6974 680a 2020 4a41  mposed with.  JA
+00014010: 5820 7472 616e 7366 6f72 6d61 7469 6f6e  X transformation
+00014020: 7320 6c69 6b65 2060 606a 6178 2e6a 6974  s like ``jax.jit
+00014030: 6060 3a3a 0a0a 2020 2020 6465 6620 6628  ``::..    def f(
+00014040: 666f 6f2c 2078 293a 0a20 2020 2020 207a  foo, x):.      z
+00014050: 203d 2066 6f6f 2e65 6e63 6f64 6528 7829   = foo.encode(x)
+00014060: 0a20 2020 2020 2079 203d 2066 6f6f 2e64  .      y = foo.d
+00014070: 6563 6f64 6528 7a29 0a20 2020 2020 2023  ecode(z).      #
+00014080: 202e 2e2e 0a20 2020 2020 2072 6574 7572   ....      retur
+00014090: 6e20 790a 0a20 2020 2066 6f6f 203d 2046  n y..    foo = F
+000140a0: 6f6f 2829 0a20 2020 2066 5f6a 6974 7465  oo().    f_jitte
+000140b0: 6420 3d20 6a61 782e 6a69 7428 6e6e 2e69  d = jax.jit(nn.i
+000140c0: 6e69 745f 7769 7468 5f6f 7574 7075 7428  nit_with_output(
+000140d0: 662c 2066 6f6f 2929 0a20 2020 2079 2c20  f, foo)).    y, 
+000140e0: 7661 7269 6162 6c65 7320 3d20 665f 6a69  variables = f_ji
+000140f0: 7474 6564 2872 6e67 2c20 7829 0a0a 2020  tted(rng, x)..  
+00014100: 4172 6773 3a0a 2020 2020 666e 3a20 5468  Args:.    fn: Th
+00014110: 6520 6675 6e63 7469 6f6e 2074 6861 7420  e function that 
+00014120: 7368 6f75 6c64 2062 6520 6170 706c 6965  should be applie
+00014130: 642e 2054 6865 2066 6972 7374 2061 7267  d. The first arg
+00014140: 756d 656e 7420 7061 7373 6564 2077 696c  ument passed wil
+00014150: 6c0a 2020 2020 2020 6265 2061 6e20 6d6f  l.      be an mo
+00014160: 6475 6c65 2069 6e73 7461 6e63 6520 6f66  dule instance of
+00014170: 2074 6865 2060 606d 6f64 756c 6560 6020   the ``module`` 
+00014180: 7769 7468 2076 6172 6961 626c 6573 2061  with variables a
+00014190: 6e64 2052 4e47 7320 626f 756e 640a 2020  nd RNGs bound.  
+000141a0: 2020 2020 746f 2069 742e 0a20 2020 206d      to it..    m
+000141b0: 6f64 756c 653a 2054 6865 2060 604d 6f64  odule: The ``Mod
+000141c0: 756c 6560 6020 7468 6174 2077 696c 6c20  ule`` that will 
+000141d0: 6265 2075 7365 6420 746f 2062 696e 6420  be used to bind 
+000141e0: 7661 7269 6162 6c65 7320 616e 6420 524e  variables and RN
+000141f0: 4773 2074 6f2e 0a20 2020 2020 2054 6865  Gs to..      The
+00014200: 2060 604d 6f64 756c 6560 6020 7061 7373   ``Module`` pass
+00014210: 6564 2061 7320 7468 6520 6669 7273 7420  ed as the first 
+00014220: 6172 6775 6d65 6e74 2074 6f20 6060 666e  argument to ``fn
+00014230: 6060 2077 696c 6c20 6265 2061 2063 6c6f  `` will be a clo
+00014240: 6e65 0a20 2020 2020 206f 6620 6d6f 6475  ne.      of modu
+00014250: 6c65 2e0a 2020 2020 6d75 7461 626c 653a  le..    mutable:
+00014260: 2043 616e 2062 6520 626f 6f6c 2c20 7374   Can be bool, st
+00014270: 722c 206f 7220 6c69 7374 2e20 5370 6563  r, or list. Spec
+00014280: 6966 6965 7320 7768 6963 6820 636f 6c6c  ifies which coll
+00014290: 6563 7469 6f6e 7320 7368 6f75 6c64 2062  ections should b
+000142a0: 650a 2020 2020 2020 7472 6561 7465 6420  e.      treated 
+000142b0: 6173 206d 7574 6162 6c65 3a20 6060 626f  as mutable: ``bo
+000142c0: 6f6c 6060 3a20 616c 6c2f 6e6f 2063 6f6c  ol``: all/no col
+000142d0: 6c65 6374 696f 6e73 2061 7265 206d 7574  lections are mut
+000142e0: 6162 6c65 2e0a 2020 2020 2020 6060 7374  able..      ``st
+000142f0: 7260 603a 2054 6865 206e 616d 6520 6f66  r``: The name of
+00014300: 2061 2073 696e 676c 6520 6d75 7461 626c   a single mutabl
+00014310: 6520 636f 6c6c 6563 7469 6f6e 2e20 6060  e collection. ``
+00014320: 6c69 7374 6060 3a20 410a 2020 2020 2020  list``: A.      
+00014330: 6c69 7374 206f 6620 6e61 6d65 7320 6f66  list of names of
+00014340: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
+00014350: 696f 6e73 2e20 4279 2064 6566 6175 6c74  ions. By default
+00014360: 2061 6c6c 2063 6f6c 6c65 6374 696f 6e73   all collections
+00014370: 0a20 2020 2020 2065 7863 6570 7420 2269  .      except "i
+00014380: 6e74 6572 6d65 6469 6174 6573 2220 6172  ntermediates" ar
+00014390: 6520 6d75 7461 626c 652e 0a20 2020 2063  e mutable..    c
+000143a0: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
+000143b0: 6174 6573 3a20 4966 2060 5472 7565 602c  ates: If `True`,
+000143c0: 2063 6170 7475 7265 7320 696e 7465 726d   captures interm
+000143d0: 6564 6961 7465 2072 6574 7572 6e20 7661  ediate return va
+000143e0: 6c75 6573 0a20 2020 2020 206f 6620 616c  lues.      of al
+000143f0: 6c20 4d6f 6475 6c65 7320 696e 7369 6465  l Modules inside
+00014400: 2074 6865 2022 696e 7465 726d 6564 6961   the "intermedia
+00014410: 7465 7322 2063 6f6c 6c65 6374 696f 6e2e  tes" collection.
+00014420: 2042 7920 6465 6661 756c 7420 6f6e 6c79   By default only
+00014430: 0a20 2020 2020 2074 6865 2072 6574 7572  .      the retur
+00014440: 6e20 7661 6c75 6573 206f 6620 616c 6c20  n values of all 
+00014450: 605f 5f63 616c 6c5f 5f60 206d 6574 686f  `__call__` metho
+00014460: 6473 2061 7265 2073 746f 7265 642e 2041  ds are stored. A
+00014470: 2066 756e 6374 696f 6e20 6361 6e0a 2020   function can.  
+00014480: 2020 2020 6265 2070 6173 7365 6420 746f      be passed to
+00014490: 2063 6861 6e67 6520 7468 6520 6669 6c74   change the filt
+000144a0: 6572 2062 6568 6176 696f 722e 2054 6865  er behavior. The
+000144b0: 2066 696c 7465 7220 6675 6e63 7469 6f6e   filter function
+000144c0: 2074 616b 6573 0a20 2020 2020 2074 6865   takes.      the
+000144d0: 204d 6f64 756c 6520 696e 7374 616e 6365   Module instance
+000144e0: 2061 6e64 206d 6574 686f 6420 6e61 6d65   and method name
+000144f0: 2061 6e64 2072 6574 7572 6e73 2061 2062   and returns a b
+00014500: 6f6f 6c20 696e 6469 6361 7469 6e67 0a20  ool indicating. 
+00014510: 2020 2020 2077 6865 7468 6572 2074 6865       whether the
+00014520: 206f 7574 7075 7420 6f66 2074 6861 7420   output of that 
+00014530: 6d65 7468 6f64 2069 6e76 6f63 6174 696f  method invocatio
+00014540: 6e20 7368 6f75 6c64 2062 6520 7374 6f72  n should be stor
+00014550: 6564 2e0a 2020 5265 7475 726e 733a 0a20  ed..  Returns:. 
+00014560: 2020 2054 6865 2069 6e69 7420 6675 6e63     The init func
+00014570: 7469 6f6e 2077 7261 7070 696e 6720 6060  tion wrapping ``
+00014580: 666e 6060 2e0a 2020 2222 220a 2020 4066  fn``..  """.  @f
+00014590: 756e 6374 6f6f 6c73 2e77 7261 7073 2866  unctools.wraps(f
+000145a0: 6e29 0a20 2064 6566 2073 636f 7065 5f66  n).  def scope_f
+000145b0: 6e28 7363 6f70 652c 202a 6172 6773 2c20  n(scope, *args, 
+000145c0: 2a2a 6b77 6172 6773 293a 0a20 2020 205f  **kwargs):.    _
+000145d0: 636f 6e74 6578 742e 6361 7074 7572 655f  context.capture_
+000145e0: 7374 6163 6b2e 6170 7065 6e64 2863 6170  stack.append(cap
+000145f0: 7475 7265 5f69 6e74 6572 6d65 6469 6174  ture_intermediat
+00014600: 6573 290a 2020 2020 7472 793a 0a20 2020  es).    try:.   
+00014610: 2020 2072 6574 7572 6e20 666e 286d 6f64     return fn(mod
+00014620: 756c 652e 636c 6f6e 6528 7061 7265 6e74  ule.clone(parent
+00014630: 3d73 636f 7065 292c 202a 6172 6773 2c20  =scope), *args, 
+00014640: 2a2a 6b77 6172 6773 290a 2020 2020 6669  **kwargs).    fi
+00014650: 6e61 6c6c 793a 0a20 2020 2020 205f 636f  nally:.      _co
+00014660: 6e74 6578 742e 6361 7074 7572 655f 7374  ntext.capture_st
+00014670: 6163 6b2e 706f 7028 290a 0a20 2069 6620  ack.pop()..  if 
+00014680: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
+00014690: 6961 7465 7320 6973 2054 7275 653a 2020  iates is True:  
+000146a0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+000146b0: 653d 672d 626f 6f6c 2d69 642d 636f 6d70  e=g-bool-id-comp
+000146c0: 6172 6973 6f6e 0a20 2020 2063 6170 7475  arison.    captu
+000146d0: 7265 5f69 6e74 6572 6d65 6469 6174 6573  re_intermediates
+000146e0: 203d 2063 6170 7475 7265 5f63 616c 6c5f   = capture_call_
+000146f0: 696e 7465 726d 6564 6961 7465 730a 2020  intermediates.  
+00014700: 6966 2063 6170 7475 7265 5f69 6e74 6572  if capture_inter
+00014710: 6d65 6469 6174 6573 3a0a 2020 2020 6d75  mediates:.    mu
+00014720: 7461 626c 6520 3d20 756e 696f 6e5f 6669  table = union_fi
+00014730: 6c74 6572 7328 6d75 7461 626c 652c 2027  lters(mutable, '
+00014740: 696e 7465 726d 6564 6961 7465 7327 290a  intermediates').
+00014750: 2020 7265 7475 726e 2063 6f72 652e 696e    return core.in
+00014760: 6974 2873 636f 7065 5f66 6e2c 206d 7574  it(scope_fn, mut
+00014770: 6162 6c65 3d6d 7574 6162 6c65 290a 0a0a  able=mutable)...
+00014780: 4074 7261 6365 6261 636b 5f75 7469 6c2e  @traceback_util.
+00014790: 6170 695f 626f 756e 6461 7279 0a64 6566  api_boundary.def
+000147a0: 2069 6e69 7428 666e 3a20 4361 6c6c 6162   init(fn: Callab
+000147b0: 6c65 5b2e 2e2e 2c20 416e 795d 2c20 6d6f  le[..., Any], mo
+000147c0: 6475 6c65 3a20 4d6f 6475 6c65 2c0a 2020  dule: Module,.  
+000147d0: 2020 2020 2020 206d 7574 6162 6c65 3a20         mutable: 
+000147e0: 436f 6c6c 6563 7469 6f6e 4669 6c74 6572  CollectionFilter
+000147f0: 203d 2044 656e 794c 6973 7428 2769 6e74   = DenyList('int
+00014800: 6572 6d65 6469 6174 6573 2729 2c0a 2020  ermediates'),.  
+00014810: 2020 2020 2020 2063 6170 7475 7265 5f69         capture_i
+00014820: 6e74 6572 6d65 6469 6174 6573 3a20 556e  ntermediates: Un
+00014830: 696f 6e5b 626f 6f6c 2c20 4361 6c6c 6162  ion[bool, Callab
+00014840: 6c65 5b5b 4d6f 6475 6c65 2c20 7374 725d  le[[Module, str]
+00014850: 2c20 626f 6f6c 5d5d 203d 2046 616c 7365  , bool]] = False
+00014860: 2c0a 2020 2020 2020 2020 2029 202d 3e20  ,.         ) -> 
+00014870: 4361 6c6c 6162 6c65 5b2e 2e2e 2c20 556e  Callable[..., Un
+00014880: 696f 6e5b 4672 6f7a 656e 5661 7269 6162  ion[FrozenVariab
+00014890: 6c65 4469 6374 2c20 4469 6374 5b73 7472  leDict, Dict[str
+000148a0: 2c20 416e 795d 5d5d 3a0a 2020 2222 2243  , Any]]]:.  """C
+000148b0: 7265 6174 6573 2061 6e20 696e 6974 2066  reates an init f
+000148c0: 756e 6374 696f 6e20 746f 2063 616c 6c20  unction to call 
+000148d0: 6060 666e 6060 2077 6974 6820 6120 626f  ``fn`` with a bo
+000148e0: 756e 6420 6d6f 6475 6c65 2e0a 0a20 2055  und module...  U
+000148f0: 6e6c 696b 6520 6060 4d6f 6475 6c65 2e69  nlike ``Module.i
+00014900: 6e69 7460 6020 7468 6973 2066 756e 6374  nit`` this funct
+00014910: 696f 6e20 7265 7475 726e 7320 6120 6e65  ion returns a ne
+00014920: 7720 6675 6e63 7469 6f6e 2077 6974 6820  w function with 
+00014930: 7468 6520 7369 676e 6174 7572 650a 2020  the signature.  
+00014940: 6060 2872 6e67 732c 202a 6172 6773 2c20  ``(rngs, *args, 
+00014950: 2a2a 6b77 6172 6773 2920 2d3e 2076 6172  **kwargs) -> var
+00014960: 6961 626c 6573 6060 2e0a 2020 5468 6520  iables``..  The 
+00014970: 726e 6773 2063 616e 2062 6520 6120 6469  rngs can be a di
+00014980: 6374 206f 6620 5052 4e47 4b65 7973 206f  ct of PRNGKeys o
+00014990: 7220 6120 7369 6e67 6c65 2060 6060 5052  r a single ```PR
+000149a0: 4e47 4b65 7960 6020 7768 6963 6820 6973  NGKey`` which is
+000149b0: 0a20 2065 7175 6976 616c 656e 7420 746f  .  equivalent to
+000149c0: 2070 6173 7369 6e67 2061 2064 6963 7420   passing a dict 
+000149d0: 7769 7468 206f 6e65 2050 524e 474b 6579  with one PRNGKey
+000149e0: 2077 6974 6820 7468 6520 6e61 6d65 2022   with the name "
+000149f0: 7061 7261 6d73 222e 0a0a 2020 5468 6520  params"...  The 
+00014a00: 696e 6974 2066 756e 6374 696f 6e20 7468  init function th
+00014a10: 6174 2069 7320 7265 7475 726e 6564 2063  at is returned c
+00014a20: 616e 2062 6520 6469 7265 6374 6c79 2063  an be directly c
+00014a30: 6f6d 706f 7365 6420 7769 7468 0a20 204a  omposed with.  J
+00014a40: 4158 2074 7261 6e73 666f 726d 6174 696f  AX transformatio
+00014a50: 6e73 206c 696b 6520 6060 6a61 782e 6a69  ns like ``jax.ji
+00014a60: 7460 603a 3a0a 0a20 2020 2064 6566 2066  t``::..    def f
+00014a70: 2866 6f6f 2c20 7829 3a0a 2020 2020 2020  (foo, x):.      
+00014a80: 7a20 3d20 666f 6f2e 656e 636f 6465 2878  z = foo.encode(x
+00014a90: 290a 2020 2020 2020 7920 3d20 666f 6f2e  ).      y = foo.
+00014aa0: 6465 636f 6465 287a 290a 2020 2020 2020  decode(z).      
+00014ab0: 2320 2e2e 2e0a 2020 2020 2020 7265 7475  # ....      retu
+00014ac0: 726e 2079 0a0a 2020 2020 666f 6f20 3d20  rn y..    foo = 
+00014ad0: 466f 6f28 290a 2020 2020 665f 6a69 7474  Foo().    f_jitt
+00014ae0: 6564 203d 206a 6178 2e6a 6974 286e 6e2e  ed = jax.jit(nn.
+00014af0: 696e 6974 2866 2c20 666f 6f29 290a 2020  init(f, foo)).  
+00014b00: 2020 7661 7269 6162 6c65 7320 3d20 665f    variables = f_
+00014b10: 6a69 7474 6564 2872 6e67 2c20 7829 0a0a  jitted(rng, x)..
+00014b20: 2020 4172 6773 3a0a 2020 2020 666e 3a20    Args:.    fn: 
+00014b30: 5468 6520 6675 6e63 7469 6f6e 2074 6861  The function tha
+00014b40: 7420 7368 6f75 6c64 2062 6520 6170 706c  t should be appl
+00014b50: 6965 642e 2054 6865 2066 6972 7374 2061  ied. The first a
+00014b60: 7267 756d 656e 7420 7061 7373 6564 2077  rgument passed w
+00014b70: 696c 6c0a 2020 2020 2020 6265 2061 6e20  ill.      be an 
+00014b80: 6d6f 6475 6c65 2069 6e73 7461 6e63 6520  module instance 
+00014b90: 6f66 2074 6865 2060 606d 6f64 756c 6560  of the ``module`
+00014ba0: 6020 7769 7468 2076 6172 6961 626c 6573  ` with variables
+00014bb0: 2061 6e64 2052 4e47 7320 626f 756e 640a   and RNGs bound.
+00014bc0: 2020 2020 2020 746f 2069 742e 0a20 2020        to it..   
+00014bd0: 206d 6f64 756c 653a 2054 6865 2060 604d   module: The ``M
+00014be0: 6f64 756c 6560 6020 7468 6174 2077 696c  odule`` that wil
+00014bf0: 6c20 6265 2075 7365 6420 746f 2062 696e  l be used to bin
+00014c00: 6420 7661 7269 6162 6c65 7320 616e 6420  d variables and 
+00014c10: 524e 4773 2074 6f2e 0a20 2020 2020 2054  RNGs to..      T
+00014c20: 6865 2060 604d 6f64 756c 6560 6020 7061  he ``Module`` pa
+00014c30: 7373 6564 2061 7320 7468 6520 6669 7273  ssed as the firs
+00014c40: 7420 6172 6775 6d65 6e74 2074 6f20 6060  t argument to ``
+00014c50: 666e 6060 2077 696c 6c20 6265 2061 2063  fn`` will be a c
+00014c60: 6c6f 6e65 0a20 2020 2020 206f 6620 6d6f  lone.      of mo
+00014c70: 6475 6c65 2e0a 2020 2020 6d75 7461 626c  dule..    mutabl
+00014c80: 653a 2043 616e 2062 6520 626f 6f6c 2c20  e: Can be bool, 
+00014c90: 7374 722c 206f 7220 6c69 7374 2e20 5370  str, or list. Sp
+00014ca0: 6563 6966 6965 7320 7768 6963 6820 636f  ecifies which co
+00014cb0: 6c6c 6563 7469 6f6e 7320 7368 6f75 6c64  llections should
+00014cc0: 2062 650a 2020 2020 2020 7472 6561 7465   be.      treate
+00014cd0: 6420 6173 206d 7574 6162 6c65 3a20 6060  d as mutable: ``
+00014ce0: 626f 6f6c 6060 3a20 616c 6c2f 6e6f 2063  bool``: all/no c
+00014cf0: 6f6c 6c65 6374 696f 6e73 2061 7265 206d  ollections are m
+00014d00: 7574 6162 6c65 2e0a 2020 2020 2020 6060  utable..      ``
+00014d10: 7374 7260 603a 2054 6865 206e 616d 6520  str``: The name 
+00014d20: 6f66 2061 2073 696e 676c 6520 6d75 7461  of a single muta
+00014d30: 626c 6520 636f 6c6c 6563 7469 6f6e 2e20  ble collection. 
+00014d40: 6060 6c69 7374 6060 3a20 410a 2020 2020  ``list``: A.    
+00014d50: 2020 6c69 7374 206f 6620 6e61 6d65 7320    list of names 
+00014d60: 6f66 206d 7574 6162 6c65 2063 6f6c 6c65  of mutable colle
+00014d70: 6374 696f 6e73 2e20 4279 2064 6566 6175  ctions. By defau
+00014d80: 6c74 2061 6c6c 2063 6f6c 6c65 6374 696f  lt all collectio
+00014d90: 6e73 0a20 2020 2020 2065 7863 6570 7420  ns.      except 
+00014da0: 2269 6e74 6572 6d65 6469 6174 6573 2220  "intermediates" 
+00014db0: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
+00014dc0: 2063 6170 7475 7265 5f69 6e74 6572 6d65   capture_interme
+00014dd0: 6469 6174 6573 3a20 4966 2060 5472 7565  diates: If `True
+00014de0: 602c 2063 6170 7475 7265 7320 696e 7465  `, captures inte
+00014df0: 726d 6564 6961 7465 2072 6574 7572 6e20  rmediate return 
+00014e00: 7661 6c75 6573 0a20 2020 2020 206f 6620  values.      of 
+00014e10: 616c 6c20 4d6f 6475 6c65 7320 696e 7369  all Modules insi
+00014e20: 6465 2074 6865 2022 696e 7465 726d 6564  de the "intermed
+00014e30: 6961 7465 7322 2063 6f6c 6c65 6374 696f  iates" collectio
+00014e40: 6e2e 2042 7920 6465 6661 756c 7420 6f6e  n. By default on
+00014e50: 6c79 0a20 2020 2020 2074 6865 2072 6574  ly.      the ret
+00014e60: 7572 6e20 7661 6c75 6573 206f 6620 616c  urn values of al
+00014e70: 6c20 605f 5f63 616c 6c5f 5f60 206d 6574  l `__call__` met
+00014e80: 686f 6473 2061 7265 2073 746f 7265 642e  hods are stored.
+00014e90: 2041 2066 756e 6374 696f 6e20 6361 6e0a   A function can.
+00014ea0: 2020 2020 2020 6265 2070 6173 7365 6420        be passed 
+00014eb0: 746f 2063 6861 6e67 6520 7468 6520 6669  to change the fi
+00014ec0: 6c74 6572 2062 6568 6176 696f 722e 2054  lter behavior. T
+00014ed0: 6865 2066 696c 7465 7220 6675 6e63 7469  he filter functi
+00014ee0: 6f6e 2074 616b 6573 0a20 2020 2020 2074  on takes.      t
+00014ef0: 6865 204d 6f64 756c 6520 696e 7374 616e  he Module instan
+00014f00: 6365 2061 6e64 206d 6574 686f 6420 6e61  ce and method na
+00014f10: 6d65 2061 6e64 2072 6574 7572 6e73 2061  me and returns a
+00014f20: 2062 6f6f 6c20 696e 6469 6361 7469 6e67   bool indicating
+00014f30: 0a20 2020 2020 2077 6865 7468 6572 2074  .      whether t
+00014f40: 6865 206f 7574 7075 7420 6f66 2074 6861  he output of tha
+00014f50: 7420 6d65 7468 6f64 2069 6e76 6f63 6174  t method invocat
+00014f60: 696f 6e20 7368 6f75 6c64 2062 6520 7374  ion should be st
+00014f70: 6f72 6564 2e0a 2020 5265 7475 726e 733a  ored..  Returns:
+00014f80: 0a20 2020 2054 6865 2069 6e69 7420 6675  .    The init fu
+00014f90: 6e63 7469 6f6e 2077 7261 7070 696e 6720  nction wrapping 
+00014fa0: 6060 666e 6060 2e0a 2020 2222 220a 2020  ``fn``..  """.  
+00014fb0: 696e 6974 5f66 6e20 3d20 696e 6974 5f77  init_fn = init_w
+00014fc0: 6974 685f 6f75 7470 7574 2866 6e2c 206d  ith_output(fn, m
+00014fd0: 6f64 756c 652c 206d 7574 6162 6c65 2c20  odule, mutable, 
+00014fe0: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
+00014ff0: 6961 7465 7329 0a20 2040 6675 6e63 746f  iates).  @functo
+00015000: 6f6c 732e 7772 6170 7328 696e 6974 5f66  ols.wraps(init_f
+00015010: 6e29 0a20 2064 6566 2069 6e69 745f 7772  n).  def init_wr
+00015020: 6170 7065 7228 2a61 7267 732c 202a 2a6b  apper(*args, **k
+00015030: 7761 7267 7329 3a0a 2020 2020 7265 7475  wargs):.    retu
+00015040: 726e 2069 6e69 745f 666e 282a 6172 6773  rn init_fn(*args
+00015050: 2c20 2a2a 6b77 6172 6773 295b 315d 0a20  , **kwargs)[1]. 
+00015060: 2072 6574 7572 6e20 696e 6974 5f77 7261   return init_wra
+00015070: 7070 6572 0a                             pper.
```

### Comparing `flax-0.6.8/flax/linen/normalization.py` & `flax-0.6.9/flax/linen/normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/partitioning.py` & `flax-0.6.9/flax/linen/partitioning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/pooling.py` & `flax-0.6.9/flax/linen/pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/recurrent.py` & `flax-0.6.9/flax/linen/recurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/spmd.py` & `flax-0.6.9/flax/linen/spmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -185,14 +185,27 @@
   return jax.tree_map(
       lambda x: logical_to_mesh_axes(x, rules),
       tree,
       is_leaf=lambda x: isinstance(x, jax.sharding.PartitionSpec),
   )
 
 
+def logical_to_mesh_sharding(
+    tree: Any,
+    mesh: jax.sharding.Mesh,
+    rules: Optional[LogicalRules] = None,
+) -> Any:
+  """Convert pytrees of logical PartitionSpecs to shardings."""
+  return jax.tree_map(
+      lambda x: jax.sharding.NamedSharding(mesh, x),
+      logical_to_mesh(tree, rules),
+      is_leaf=lambda x: isinstance(x, jax.sharding.PartitionSpec),
+  )
+
+
 def _global_mesh_defined() -> bool:
   """Checks if global xmap/pjit mesh resource environment is defined."""
   maps_env = maps.thread_resources.env
   return maps_env.physical_mesh.devices.shape != ()  # pylint: disable=g-explicit-bool-comparison
 
 
 class RulesFallback(enum.Enum):
```

### Comparing `flax-0.6.8/flax/linen/stochastic.py` & `flax-0.6.9/flax/linen/stochastic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/summary.py` & `flax-0.6.9/flax/linen/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/linen/transforms.py` & `flax-0.6.9/flax/linen/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/metrics/__init__.py` & `flax-0.6.9/flax/metrics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/metrics/tensorboard.py` & `flax-0.6.9/flax/metrics/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/serialization.py` & `flax-0.6.9/flax/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/struct.py` & `flax-0.6.9/flax/struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/testing/__init__.py` & `flax-0.6.9/flax/testing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/testing/benchmark.py` & `flax-0.6.9/flax/testing/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/traceback_util.py` & `flax-0.6.9/flax/traceback_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/training/__init__.py` & `flax-0.6.9/flax/training/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/training/checkpoints.py` & `flax-0.6.9/flax/training/checkpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -35,15 +35,15 @@
 from flax import io
 from flax import serialization
 from flax import traverse_util
 from flax.training import orbax_utils
 import jax
 from jax import monitoring
 from jax import process_index
-from jax import sharding
+from jax import tree_util as jtu
 from jax.experimental.multihost_utils import sync_global_devices
 import orbax.checkpoint as orbax
 
 _READ_CHECKPOINT_EVENT: str = '/jax/checkpoint/read/durations_sec'
 _WRITE_CHECKPOINT_EVENT: str = '/jax/checkpoint/write/durations_sec'
 _IMPORT_GDAM_SUCCESSFUL = False
 try:
@@ -544,28 +544,44 @@
   if async_manager:
     async_manager.wait_previous_save()
 
   ckpt_path, ckpt_tmp_path, base_path = _get_checkpoint_paths(
       ckpt_dir, step, prefix)
 
   if config.flax_use_orbax_checkpointing or orbax_checkpointer:
+    logging.info(
+        'Using Orbax as backend to save Flax checkpoints. For potential'
+        ' troubleshooting see:'
+        ' https://flax.readthedocs.io/en/latest/guides/use_checkpointing.html#orbax-as-backend-troubleshooting'
+    )
     if jax.process_count() > 1:
       logging.warning(
-          'Multiple JAX processes detected when saving checkpoint. Please '
-          'note that if `flax.training.checkpoints.save_checkpoint` is only '
-          'called on one process (aka. guarded by a check '
-          '`jax.process_count() == 0`), the other devices will hang.'
+          'Multiple JAX processes detected when calling single-process'
+          ' `save_checkpoint`. Your devices will HANG if this function is only'
+          ' called on process 0! Troubleshoot at:'
+          ' https://flax.readthedocs.io/en/latest/guides/use_checkpointing.html#if-your-devices-hang-when-writing-checkpoints'
       )
+
     # Make sure any previous work is done before making file changes.
     if orbax_checkpointer and isinstance(orbax_checkpointer,
                                          orbax.AsyncCheckpointer):
       orbax_checkpointer.wait_until_finished()
+    # If no checkpointer provided, save synchronously with default setting.
     if not orbax_checkpointer:
-      # If no checkpointer provided, save synchronously with default setting.
       orbax_checkpointer = orbax.Checkpointer(orbax.PyTreeCheckpointHandler())
+    # Check singular target.
+    if jtu.treedef_is_leaf(jtu.tree_structure(target)) and not isinstance(
+        orbax_checkpointer._handler, orbax.ArrayCheckpointHandler  # pylint: disable=protected-access
+    ):
+      raise ValueError(
+          'Orbax backend only accept pytree as save target. To save singular'
+          ' objects like numbers or Numpy arrays, checkout'
+          ' https://flax.readthedocs.io/en/latest/guides/use_checkpointing.html#if-you-don-t-save-pytrees'
+      )
+
     save_args = orbax_utils.save_args_from_target(target)
     orbax_checkpointer.save(
         ckpt_path, target, save_args=save_args, force=overwrite)
     # Do a process check here in case people call this for multihost.
     if process_index() == 0:
       _remove_invalid_ckpts(ckpt_path, base_path, keep, overwrite,
                             keep_every_n_steps, True)
@@ -652,32 +668,48 @@
 
   Returns:
     Filename of saved checkpoint.
   """
   start_time = time.time()
   # Make sure all saves are finished before the logic of checking and removing
   # outdated checkpoints happens.
-  sync_global_devices('starting_save_checkpoint')
+  sync_global_devices('Flax:Checkpoint:StartSave')
   if async_manager:
     async_manager.wait_previous_save()
   if gda_manager:
     gda_manager.wait_until_finished()
-    sync_global_devices('before_save_checkpoint')
+    sync_global_devices('Flax:Checkpoint:WaitLastSaveDone')
 
   ckpt_path, ckpt_tmp_path, base_path = _get_checkpoint_paths(
       ckpt_dir, step, prefix)
 
   if config.flax_use_orbax_checkpointing or orbax_checkpointer:
+    logging.info(
+        'Using Orbax as backend to save Flax checkpoints. For potential'
+        ' troubleshooting see:'
+        ' https://flax.readthedocs.io/en/latest/guides/use_checkpointing.html#orbax-as-backend-troubleshooting'
+    )
     # Make sure any previous work is done before making file changes.
     if orbax_checkpointer and isinstance(orbax_checkpointer,
                                          orbax.AsyncCheckpointer):
       orbax_checkpointer.wait_until_finished()
+
     # If no checkpointer provided, save synchronously with default setting.
     if not orbax_checkpointer:
       orbax_checkpointer = orbax.Checkpointer(orbax.PyTreeCheckpointHandler())
+    # Check singular target.
+    if jtu.treedef_is_leaf(jtu.tree_structure(target)) and not isinstance(
+        orbax_checkpointer._handler, orbax.ArrayCheckpointHandler  # pylint: disable=protected-access
+    ):
+      raise ValueError(
+          'Orbax backend only accept pytree as save target. To save singular'
+          ' objects like numbers or Numpy arrays, checkout'
+          ' https://flax.readthedocs.io/en/latest/guides/use_checkpointing.html#if-you-don-t-save-pytrees'
+      )
+
     if process_index() == 0:
       _remove_invalid_ckpts(ckpt_path, base_path, keep, overwrite,
                             keep_every_n_steps, True)
     save_args = orbax_utils.save_args_from_target(target)
     orbax_checkpointer.save(
         ckpt_path, target, save_args=save_args, force=overwrite)
     end_time = time.time()
@@ -699,15 +731,15 @@
   target = serialization.to_state_dict(target)
   target, mpa_targets = _split_mp_arrays(target)
   target = serialization.msgpack_serialize(target)
   has_mpa = mpa_targets and _IMPORT_GDAM_SUCCESSFUL
 
   if not overwrite:
     _check_overwrite_error(ckpt_tmp_path, ckpt_path, base_path, step) # type: ignore
-    sync_global_devices('check_overwrite_strictly_before_save')
+    sync_global_devices('Flax:Checkpoint:CheckOverwriteBeforeSave')
   # Save the files via I/O sync or async.
   def save_main_ckpt_task():
     jax.monitoring.record_event('/jax/flax/checkpoint/save_main_ckpt_task')
     return _save_main_ckpt_file(target, has_mpa, (ckpt_tmp_path, ckpt_path),
                                 base_path, step, keep, overwrite,
                                 keep_every_n_steps, start_time)
   # Write the main checkpoint file only via process 0, to avoid race condition.
@@ -720,15 +752,15 @@
   if has_mpa:
     if not gda_manager:
       raise errors.MPACheckpointingRequiredError(ckpt_path, step)
     # Creating the directory containing GDAs explicitly. This should happen only
     # on process 0 and before any worker starts to write GDA data.
     if process_index() == 0:
       _make_mpa_dirs(mpa_targets, ckpt_tmp_path)
-    sync_global_devices('Flax:Checkpointing:AfterCreateMPADir')
+    sync_global_devices('Flax:Checkpoint:AfterCreateMPADir')
     _save_mpas(gda_manager, mpa_targets, ckpt_tmp_path, ckpt_path, base_path,
                keep, overwrite, keep_every_n_steps, start_time, async_manager)
 
   end_time = time.time()
   monitoring.record_event_duration_secs(_WRITE_CHECKPOINT_EVENT,
                                         end_time - start_time)
   return ckpt_path
@@ -810,15 +842,16 @@
     ckpt_dir: Union[str, os.PathLike],
     target: Optional[Any],
     step: Optional[Union[int, float]] = None,
     prefix: str = 'checkpoint_',
     parallel: bool = True,
     gda_manager: Optional[Any] = None,
     allow_partial_mpa_restoration: bool = False,
-    orbax_checkpointer: Optional[orbax.Checkpointer] = None) -> PyTree:
+    orbax_checkpointer: Optional[orbax.Checkpointer] = None,
+    orbax_transforms: Optional[Dict] = None) -> PyTree:
   """Restore last/best checkpoint from checkpoints in path.
 
   Sorts the checkpoint files naturally, returning the highest-valued
   file, e.g.:
 
   *  ``ckpt_1, ckpt_2, ckpt_3 --> ckpt_3``
 
@@ -842,14 +875,16 @@
     allow_partial_mpa_restoration: If true, the given `target` doesn't have to
       contain all valid multiprocess arrays. As a result, the restored Pytree
       may have some MPAs not restored correctly. Use this if you cannot provide
       a fully valid ``target`` and don't need all the MPAs in the checkpoint
       to be restored.
     orbax_checkpointer: the `Orbax.Checkpointer` that handles the underlying
       restore, if the given checkpoint is saved with Orbax.
+    orbax_transforms: the Orbax transformations that will be passed into
+      `orbax_checkpointer.restore()` call.
 
   Returns:
     Restored `target` updated from checkpoint file, or if no step specified and
     no checkpoint files present, returns the passed-in `target` unchanged.
     If a file path is specified and is not found, the passed-in `target` will be
     returned. This is to match the behavior of the case where a directory path
     is specified but the directory has not yet been created.
@@ -895,33 +930,39 @@
       if orbax_utils.is_multiprocess_array(x):
         return orbax.ArrayRestoreArgs(
             restore_type=jax.Array,
             sharding=x.sharding,
         )
       return orbax.RestoreArgs()
 
-    restore_args = None
+
+    restore_kwargs = {}
     if target is not None:
-      restore_args = jax.tree_util.tree_map(make_restore_args, target)
+      restore_kwargs['restore_args'] = jax.tree_util.tree_map(
+          make_restore_args, target
+      )
+    if orbax_transforms is not None:
+      restore_kwargs['transforms'] = orbax_transforms
     restored = orbax_checkpointer.restore(
-        ckpt_path, item=target, restore_args=restore_args)
+        ckpt_path, item=target, **restore_kwargs)
     restored = serialization.to_state_dict(restored)
     if target is not None:
       restored = serialization.from_state_dict(target, restored)
     end_time = time.time()
     monitoring.record_event_duration_secs(_READ_CHECKPOINT_EVENT,
                                           end_time - start_time)
     return restored
 
+  ckpt_size = io.getsize(ckpt_path)
   with io.GFile(ckpt_path, 'rb') as fp:
     if parallel and fp.seekable():
       buf_size = 128 << 20  # 128M buffer.
-      num_bufs = fp.size() / buf_size
+      num_bufs = ckpt_size / buf_size
       logging.debug('num_bufs: %d', num_bufs)
-      checkpoint_contents = bytearray(fp.size())
+      checkpoint_contents = bytearray(ckpt_size)
 
       def read_chunk(i):
         # NOTE: We have to re-open the file to read each chunk, otherwise the
         # parallelism has no effect. But we could reuse the file pointers
         # within each thread.
         with io.GFile(ckpt_path, 'rb') as f:
           f.seek(i * buf_size)
```

### Comparing `flax-0.6.8/flax/training/common_utils.py` & `flax-0.6.9/flax/training/common_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/training/dynamic_scale.py` & `flax-0.6.9/flax/training/dynamic_scale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/training/early_stopping.py` & `flax-0.6.9/flax/training/early_stopping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/training/lr_schedule.py` & `flax-0.6.9/flax/training/lr_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/training/orbax_utils.py` & `flax-0.6.9/flax/training/orbax_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utils for Orbax Checkpointing, available even after Flax Checkpointing is deprecated."""
 
 from typing import Any, Optional
+import warnings
 
 import jax
 from jax.sharding import Mesh
 from orbax import checkpoint as orbax
 
 
 PyTree = Any
@@ -33,23 +34,46 @@
 
 def save_args_from_target(target: Any) -> Any:
   return jax.tree_util.tree_map(
       lambda x: orbax.SaveArgs(aggregate=not is_multiprocess_array(x)), target
   )
 
 
-def restore_args_from_target(target: Any, mesh: Optional[Mesh]) -> Any:
-  def find_axes(x):
+def restore_args_from_target(target: Any, mesh: Optional[Mesh] = None) -> Any:
+  """Creates Orbax `restore_args` given a target Pytree.
+
+  Args:
+    target: The Pytree that has the same structure as the checkpoint. The arrays
+      restored from checkpoint will have the same `sharding` as the target
+      Pytree's corresponding arrays.
+    mesh: DEPRECATED ARG. Please simply use your mesh to create the arrays
+      in your `target`, no need to pass it here.
+
+  Returns:
+    A Pytree of Orbax `RestoreArgs` or `ArrayRestoreArgs`
+  """
+  def find_sharding(x):
     if is_multiprocess_array(x):
-      return x.sharding.spec
+      return x.sharding
     return None
+
+  # Simpler case: no multihost arrays
   if not any(
       jax.tree_util.tree_flatten(jax.tree_map(is_multiprocess_array, target))[0]
   ):
     return jax.tree_util.tree_map(lambda x: orbax.RestoreArgs(), target)
-  assert (
-      mesh is not None
-  ), 'Argument `mesh` required because `target` contains multiprocess array.'
-  axes_tree = jax.tree_util.tree_map(find_axes, target)
-  return orbax.checkpoint_utils.restore_args_from_target(
-      mesh, target, axes_tree
-  )
+
+  # Multihost arrays: find sharding from the given target
+  sharding_tree = jax.tree_util.tree_map(find_sharding, target)
+  if mesh is not None:
+    warnings.warn(
+        (
+            'restore_args_from_target(): `mesh` arg is deprecated. Simply'
+            ' calling the function with target pytree should suffice.'
+        ),
+        DeprecationWarning,
+    )
+    axes_tree = jax.tree_util.tree_map(lambda s: s.spec, sharding_tree)
+    return orbax.checkpoint_utils.restore_args_from_target(
+        mesh, target, axes_tree
+    )
+  return orbax.checkpoint_utils.construct_restore_args(target, sharding_tree)
```

### Comparing `flax-0.6.8/flax/training/prefetch_iterator.py` & `flax-0.6.9/flax/training/prefetch_iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/training/train_state.py` & `flax-0.6.9/flax/training/train_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/traverse_util.py` & `flax-0.6.9/flax/traverse_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `flax-0.6.8/flax/version.py` & `flax-0.6.9/flax/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current Flax version at head on Github."""
-__version__ = "0.6.8"
+__version__ = "0.6.9"
```

### Comparing `flax-0.6.8/flax.egg-info/PKG-INFO` & `flax-0.6.9/flax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: flax
-Version: 0.6.8
+Version: 0.6.9
 Summary: Flax: A neural network library for JAX designed for flexibility
-Home-page: https://github.com/google/flax
-Author: Flax team
-Author-email: flax-dev@google.com
+Author-email: Flax team <flax-dev@google.com>
+Project-URL: homepage, https://github.com/google/flax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 Provides-Extra: all
+Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/google/flax/main/images/flax_logo_250px.png" alt="logo"></img>
 </div>
 
@@ -198,29 +197,29 @@
 decoded = model.apply(variables, encoded, method=model.decode)
 ```
 
 ## 🤗 Hugging Face
 
 In-detail examples to train and evaluate a variety of Flax models for
 Natural Language Processing, Computer Vision, and Speech Recognition are
-actively maintained in the [🤗 Transformers repository](https://github.com/huggingface/transformers/tree/master/examples/flax).
+actively maintained in the [🤗 Transformers repository](https://github.com/huggingface/transformers/tree/main/examples/flax).
 
 As of October 2021, the [19 most-used Transformer architectures](https://huggingface.co/transformers/#supported-frameworks) are supported in Flax
 and over 5000 pretrained checkpoints in Flax have been uploaded to the [🤗 Hub](https://huggingface.co/models?library=jax&sort=downloads).
 
 ## Citing Flax
 
 To cite this repository:
 
 ```
 @software{flax2020github,
   author = {Jonathan Heek and Anselm Levskaya and Avital Oliver and Marvin Ritter and Bertrand Rondepierre and Andreas Steiner and Marc van {Z}ee},
   title = {{F}lax: A neural network library and ecosystem for {JAX}},
   url = {http://github.com/google/flax},
-  version = {0.6.8},
+  version = {0.6.9},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, names are in alphabetical order, the version number
 is intended to be that from [flax/version.py](https://github.com/google/flax/blob/main/flax/version.py), and the year corresponds to the project's open-source release.
```

