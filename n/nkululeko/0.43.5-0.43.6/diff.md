# Comparing `tmp/nkululeko-0.43.5.tar.gz` & `tmp/nkululeko-0.43.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.43.5.tar", last modified: Tue Apr  4 12:57:14 2023, max compression
+gzip compressed data, was "nkululeko-0.43.6.tar", last modified: Tue Apr 18 14:14:02 2023, max compression
```

## Comparing `nkululeko-0.43.5.tar` & `nkululeko-0.43.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-04 12:57:14.135829 nkululeko-0.43.5/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5114 2023-04-04 12:53:01.000000 nkululeko-0.43.5/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.43.5/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15838 2023-04-04 12:57:14.135829 nkululeko-0.43.5/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10171 2023-04-04 08:11:52.000000 nkululeko-0.43.5/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-04 12:57:14.135829 nkululeko-0.43.5/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.43.5/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.43.5/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.43.5/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.43.5/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.43.5/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-04-04 12:53:38.000000 nkululeko-0.43.5/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.43.5/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1820 2023-03-23 14:42:03.000000 nkululeko-0.43.5/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.43.5/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.43.5/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.43.5/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19786 2023-04-04 12:53:16.000000 nkululeko-0.43.5/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1617 2023-03-13 09:54:10.000000 nkululeko-0.43.5/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3599 2023-03-13 10:45:56.000000 nkululeko-0.43.5/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2536 2023-02-20 12:40:05.000000 nkululeko-0.43.5/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-02-09 11:59:30.000000 nkululeko-0.43.5/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.43.5/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.43.5/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.43.5/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1699 2023-02-15 16:11:36.000000 nkululeko-0.43.5/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2899 2023-02-09 12:01:24.000000 nkululeko-0.43.5/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.43.5/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2985 2023-02-08 10:22:44.000000 nkululeko-0.43.5/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.43.5/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.43.5/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.43.5/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.43.5/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.43.5/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.43.5/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.43.5/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.43.5/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.43.5/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.43.5/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.43.5/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.43.5/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.43.5/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.43.5/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.43.5/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.43.5/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.43.5/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.43.5/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.43.5/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.43.5/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.43.5/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.43.5/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4496 2023-02-28 14:44:32.000000 nkululeko-0.43.5/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.43.5/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.43.5/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10638 2023-02-16 12:26:38.000000 nkululeko-0.43.5/nkululeko/runmanager copy.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.43.5/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.43.5/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.43.5/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.43.5/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7661 2023-02-20 11:54:33.000000 nkululeko-0.43.5/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-04 12:57:14.135829 nkululeko-0.43.5/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15838 2023-04-04 12:57:14.000000 nkululeko-0.43.5/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1538 2023-04-04 12:57:14.000000 nkululeko-0.43.5/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-04-04 12:57:14.000000 nkululeko-0.43.5/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      225 2023-04-04 12:57:14.000000 nkululeko-0.43.5/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-04-04 12:57:14.000000 nkululeko-0.43.5/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.43.5/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      901 2023-04-04 12:57:14.135829 nkululeko-0.43.5/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.43.5/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-18 14:14:02.908260 nkululeko-0.43.6/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5159 2023-04-18 13:31:59.000000 nkululeko-0.43.6/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.43.6/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15883 2023-04-18 14:14:02.908260 nkululeko-0.43.6/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10171 2023-04-04 08:11:52.000000 nkululeko-0.43.6/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-18 14:14:02.908260 nkululeko-0.43.6/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.43.6/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.43.6/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.43.6/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.43.6/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.43.6/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-04-18 13:31:33.000000 nkululeko-0.43.6/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.43.6/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1820 2023-03-23 14:42:03.000000 nkululeko-0.43.6/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.43.6/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.43.6/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.43.6/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19786 2023-04-04 12:53:16.000000 nkululeko-0.43.6/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1617 2023-03-13 09:54:10.000000 nkululeko-0.43.6/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.43.6/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2536 2023-02-20 12:40:05.000000 nkululeko-0.43.6/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-02-09 11:59:30.000000 nkululeko-0.43.6/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.43.6/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.43.6/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.43.6/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1699 2023-02-15 16:11:36.000000 nkululeko-0.43.6/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2899 2023-02-09 12:01:24.000000 nkululeko-0.43.6/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.43.6/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2985 2023-02-08 10:22:44.000000 nkululeko-0.43.6/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.43.6/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.43.6/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.43.6/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.43.6/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.43.6/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.43.6/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.43.6/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.43.6/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.43.6/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.43.6/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.43.6/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.43.6/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.43.6/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.43.6/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.43.6/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.43.6/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.43.6/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.43.6/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.43.6/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.43.6/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.43.6/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.43.6/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4496 2023-02-28 14:44:32.000000 nkululeko-0.43.6/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.43.6/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.43.6/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10638 2023-02-16 12:26:38.000000 nkululeko-0.43.6/nkululeko/runmanager copy.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.43.6/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.43.6/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.43.6/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.43.6/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7661 2023-02-20 11:54:33.000000 nkululeko-0.43.6/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-18 14:14:02.908260 nkululeko-0.43.6/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15883 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1538 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      225 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.43.6/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      901 2023-04-18 14:14:02.908260 nkululeko-0.43.6/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.43.6/setup.py
```

### Comparing `nkululeko-0.43.5/CHANGELOG.md` & `nkululeko-0.43.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.43.6
+--------------
+* small bugs
+
+
 Version 0.43.5
 --------------
 * because of difficulties with numba and audiomentations importing audiomentations only when augmenting
 
 Version 0.43.4
 --------------
 * added error when experiment type and predictor don't match
```

### Comparing `nkululeko-0.43.5/LICENSE` & `nkululeko-0.43.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/PKG-INFO` & `nkululeko-0.43.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.43.5
+Version: 0.43.6
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -206,14 +206,19 @@
 
 ## Licence
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.43.6
+--------------
+* small bugs
+
+
 Version 0.43.5
 --------------
 * because of difficulties with numba and audiomentations importing audiomentations only when augmenting
 
 Version 0.43.4
 --------------
 * added error when experiment type and predictor don't match
```

### Comparing `nkululeko-0.43.5/README.md` & `nkululeko-0.43.6/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/augment.py` & `nkululeko-0.43.6/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/augmenter.py` & `nkululeko-0.43.6/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/cacheddataset.py` & `nkululeko-0.43.6/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/dataset.py` & `nkululeko-0.43.6/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/dataset_csv.py` & `nkululeko-0.43.6/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/dataset_ravdess.py` & `nkululeko-0.43.6/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/demo.py` & `nkululeko-0.43.6/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/demo_predictor.py` & `nkululeko-0.43.6/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/experiment.py` & `nkululeko-0.43.6/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/explore.py` & `nkululeko-0.43.6/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_analyser.py` & `nkululeko-0.43.6/nkululeko/feats_analyser.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,10 +75,12 @@
         df_imp.to_csv(file_name, mode='a')
 
                 # check if feature distributions should be plotted
         plot_feats = self.util.config_val('EXPL', 'feature_distributions', False)
         if plot_feats: 
             if self.util.exp_is_classification():
                 for feature in df_imp.feats:
-                    plots.plot_feature(plot_feats, feature, 'class_label', self.df_labels, self.X)
+                    # plot_feature(self, title, feature, label, df_labels, df_features):
+                    _plots = Plots()
+                    _plots.plot_feature(plot_feats, feature, 'class_label', self.df_labels, self.X)
             else:
                 self.util.debug('can\'t plot feature distributions if not classification')
```

### Comparing `nkululeko-0.43.5/nkululeko/feats_audmodel.py` & `nkululeko-0.43.6/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_import.py` & `nkululeko-0.43.6/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_mld.py` & `nkululeko-0.43.6/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_opensmile.py` & `nkululeko-0.43.6/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_oxbow.py` & `nkululeko-0.43.6/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_praat.py` & `nkululeko-0.43.6/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_trill.py` & `nkululeko-0.43.6/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feats_wav2vec2.py` & `nkululeko-0.43.6/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feature_extractor.py` & `nkululeko-0.43.6/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/featureset.py` & `nkululeko-0.43.6/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/feinberg_praat.py` & `nkululeko-0.43.6/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/filter_data.py` & `nkululeko-0.43.6/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/loss_ccc.py` & `nkululeko-0.43.6/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/loss_softf1loss.py` & `nkululeko-0.43.6/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model.py` & `nkululeko-0.43.6/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model_cnn.py` & `nkululeko-0.43.6/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model_gmm.py` & `nkululeko-0.43.6/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model_knn.py` & `nkululeko-0.43.6/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model_knn_reg.py` & `nkululeko-0.43.6/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model_mlp.py` & `nkululeko-0.43.6/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model_mlp_regression.py` & `nkululeko-0.43.6/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/model_svm.py` & `nkululeko-0.43.6/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/modelrunner.py` & `nkululeko-0.43.6/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/nkululeko.py` & `nkululeko-0.43.6/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/plots.py` & `nkululeko-0.43.6/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/reporter.py` & `nkululeko-0.43.6/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/runmanager copy.py` & `nkululeko-0.43.6/nkululeko/runmanager copy.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/runmanager.py` & `nkululeko-0.43.6/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/scaler.py` & `nkululeko-0.43.6/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/test.py` & `nkululeko-0.43.6/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/test_predictor.py` & `nkululeko-0.43.6/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko/util.py` & `nkululeko-0.43.6/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.43.6/nkululeko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.43.5
+Version: 0.43.6
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -206,14 +206,19 @@
 
 ## Licence
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.43.6
+--------------
+* small bugs
+
+
 Version 0.43.5
 --------------
 * because of difficulties with numba and audiomentations importing audiomentations only when augmenting
 
 Version 0.43.4
 --------------
 * added error when experiment type and predictor don't match
```

### Comparing `nkululeko-0.43.5/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.43.6/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.5/setup.cfg` & `nkululeko-0.43.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nkululeko
-version = 0.43.5
+version = 0.43.6
 author = Felix Burkhardt
 author_email = fxburk@gmail.com
 description = Machine learning audio prediction experiments based on templates
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers =
```

