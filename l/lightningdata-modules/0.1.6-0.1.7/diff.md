# Comparing `tmp/lightningdata-modules-0.1.6.tar.gz` & `tmp/lightningdata-modules-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightningdata-modules-0.1.6.tar", last modified: Mon Apr 17 14:07:53 2023, max compression
+gzip compressed data, was "lightningdata-modules-0.1.7.tar", last modified: Tue Apr 18 12:42:42 2023, max compression
```

## Comparing `lightningdata-modules-0.1.6.tar` & `lightningdata-modules-0.1.7.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.321437 lightningdata-modules-0.1.6/
--rw-rw-rw-   0        0        0     2430 2023-04-17 14:07:53.320446 lightningdata-modules-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1761 2022-11-09 12:29:04.000000 lightningdata-modules-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.511141 lightningdata-modules-0.1.6/lightningdata/
--rw-rw-rw-   0        0        0     1461 2023-04-17 07:40:15.000000 lightningdata-modules-0.1.6/lightningdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.540141 lightningdata-modules-0.1.6/lightningdata/common/
--rw-rw-rw-   0        0        0        0 2022-02-02 14:20:15.000000 lightningdata-modules-0.1.6/lightningdata/common/__init__.py
--rw-rw-rw-   0        0        0      550 2023-04-17 07:36:40.000000 lightningdata-modules-0.1.6/lightningdata/common/config.py
--rw-rw-rw-   0        0        0     4883 2023-04-17 14:03:41.000000 lightningdata-modules-0.1.6/lightningdata/common/folder2lmdb.py
--rw-rw-rw-   0        0        0     8727 2022-02-14 12:32:07.000000 lightningdata-modules-0.1.6/lightningdata/common/pre_process.py
--rw-rw-rw-   0        0        0     2395 2022-02-15 15:32:32.000000 lightningdata-modules-0.1.6/lightningdata/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.542141 lightningdata-modules-0.1.6/lightningdata/modules/
--rw-rw-rw-   0        0        0        0 2022-02-11 08:08:08.000000 lightningdata-modules-0.1.6/lightningdata/modules/__init__.py
--rw-rw-rw-   0        0        0     2241 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/modules/datamodule_base.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.577140 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/
--rw-rw-rw-   0        0        0        0 2022-02-09 11:07:33.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/__init__.py
--rw-rw-rw-   0        0        0     1346 2022-02-21 13:22:43.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/digit5_datamodule.py
--rw-rw-rw-   0        0        0     8573 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainAdaptation_base.py
--rw-rw-rw-   0        0        0     1394 2022-02-21 13:23:46.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainNet_datamodule.py
--rw-rw-rw-   0        0        0     1363 2022-02-21 13:23:46.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/office31_datamodule.py
--rw-rw-rw-   0        0        0     1405 2022-02-21 13:22:15.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/officeHome_datamodule.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.596144 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/
--rw-rw-rw-   0        0        0        0 2022-02-10 14:34:26.000000 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/__init__.py
--rw-rw-rw-   0        0        0     1048 2022-02-11 09:46:51.000000 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/emnist_datamodule.py
--rw-rw-rw-   0        0        0     3966 2022-11-09 12:58:43.000000 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/federatedLearning_base.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.621142 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/
--rw-rw-rw-   0        0        0        0 2022-04-12 08:56:02.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/__init__.py
--rw-rw-rw-   0        0        0     3378 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/metaLearning_base.py
--rw-rw-rw-   0        0        0     2181 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py
--rw-rw-rw-   0        0        0     2156 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/omiglot_datamodule.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.623145 lightningdata-modules-0.1.6/lightningdata/thirdparty/
--rw-rw-rw-   0        0        0        0 2022-11-09 14:16:25.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.643143 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/
--rw-rw-rw-   0        0        0      352 2022-11-09 14:09:26.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.812422 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/
--rw-rw-rw-   0        0        0     1620 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/__init__.py
--rw-rw-rw-   0        0        0    19222 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/bach.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.847442 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/
--rw-rw-rw-   0        0        0      195 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/__init__.py
--rw-rw-rw-   0        0        0     6861 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py
--rw-rw-rw-   0        0        0     5332 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py
--rw-rw-rw-   0        0        0     5708 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py
--rw-rw-rw-   0        0        0    10048 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cub.py
--rw-rw-rw-   0        0        0    10334 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py
--rw-rw-rw-   0        0        0    14448 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers.py
--rw-rw-rw-   0        0        0     6522 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py
--rw-rw-rw-   0        0        0    11646 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/letter.py
--rw-rw-rw-   0        0        0     9242 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py
--rw-rw-rw-   0        0        0    11285 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/omniglot.py
--rw-rw-rw-   0        0        0    14763 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py
--rw-rw-rw-   0        0        0    14686 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py
--rw-rw-rw-   0        0        0    14786 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py
--rw-rw-rw-   0        0        0    10004 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py
--rw-rw-rw-   0        0        0    21872 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tcga.py
--rw-rw-rw-   0        0        0    10696 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py
--rw-rw-rw-   0        0        0    10345 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py
--rw-rw-rw-   0        0        0     1975 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.976430 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/
--rw-rw-rw-   0        0        0     1100 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/__init__.py
--rw-rw-rw-   0        0        0     2576 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/activation.py
--rw-rw-rw-   0        0        0     2301 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/batchnorm.py
--rw-rw-rw-   0        0        0      736 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/container.py
--rw-rw-rw-   0        0        0     1149 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/conv.py
--rw-rw-rw-   0        0        0      786 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/linear.py
--rw-rw-rw-   0        0        0     2437 2022-11-09 13:14:11.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/module.py
--rw-rw-rw-   0        0        0      555 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/normalization.py
--rw-rw-rw-   0        0        0     2091 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/parallel.py
--rw-rw-rw-   0        0        0     1084 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/sparse.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.041447 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/
--rw-rw-rw-   0        0        0      345 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/__init__.py
--rw-rw-rw-   0        0        0     5592 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/harmonic.py
--rw-rw-rw-   0        0        0     4121 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/helpers.py
--rw-rw-rw-   0        0        0     4744 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid.py
--rw-rw-rw-   0        0        0     6312 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.127425 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/
--rw-rw-rw-   0        0        0      556 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/__init__.py
--rw-rw-rw-   0        0        0     2589 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/augmentations.py
--rw-rw-rw-   0        0        0     2748 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/categorical.py
--rw-rw-rw-   0        0        0    16328 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/splitters.py
--rw-rw-rw-   0        0        0      555 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py
--rw-rw-rw-   0        0        0     1325 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py
--rw-rw-rw-   0        0        0     1139 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.214445 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/
--rw-rw-rw-   0        0        0      843 2022-11-09 14:09:46.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.294468 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/
--rw-rw-rw-   0        0        0      818 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/__init__.py
--rw-rw-rw-   0        0        0     2651 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py
--rw-rw-rw-   0        0        0    13806 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataset.py
--rw-rw-rw-   0        0        0     2113 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/sampler.py
--rw-rw-rw-   0        0        0     2190 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/task.py
--rw-rw-rw-   0        0        0     3129 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py
--rw-rw-rw-   0        0        0     2330 2022-11-09 14:09:55.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/gradient_based.py
--rw-rw-rw-   0        0        0     7624 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/matching.py
--rw-rw-rw-   0        0        0     4277 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/metrics.py
--rw-rw-rw-   0        0        0     2832 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/prototype.py
--rw-rw-rw-   0        0        0     4966 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/r2d2.py
--rw-rw-rw-   0        0        0       17 2022-11-09 13:14:09.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/version.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.318441 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/
--rw-rw-rw-   0        0        0     2430 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4581 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 14:07:53.321437 lightningdata-modules-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1175 2023-04-17 14:07:24.000000 lightningdata-modules-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:42.345223 lightningdata-modules-0.1.7/
+-rw-rw-rw-   0        0        0     2430 2023-04-18 12:42:42.344233 lightningdata-modules-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1761 2022-11-09 12:29:04.000000 lightningdata-modules-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.584223 lightningdata-modules-0.1.7/lightningdata/
+-rw-rw-rw-   0        0        0     1461 2023-04-17 07:40:15.000000 lightningdata-modules-0.1.7/lightningdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.604233 lightningdata-modules-0.1.7/lightningdata/common/
+-rw-rw-rw-   0        0        0        0 2022-02-02 14:20:15.000000 lightningdata-modules-0.1.7/lightningdata/common/__init__.py
+-rw-rw-rw-   0        0        0      550 2023-04-17 07:36:40.000000 lightningdata-modules-0.1.7/lightningdata/common/config.py
+-rw-rw-rw-   0        0        0     4976 2023-04-18 12:22:44.000000 lightningdata-modules-0.1.7/lightningdata/common/folder2lmdb.py
+-rw-rw-rw-   0        0        0     8727 2022-02-14 12:32:07.000000 lightningdata-modules-0.1.7/lightningdata/common/pre_process.py
+-rw-rw-rw-   0        0        0     2395 2022-02-15 15:32:32.000000 lightningdata-modules-0.1.7/lightningdata/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.607223 lightningdata-modules-0.1.7/lightningdata/modules/
+-rw-rw-rw-   0        0        0        0 2022-02-11 08:08:08.000000 lightningdata-modules-0.1.7/lightningdata/modules/__init__.py
+-rw-rw-rw-   0        0        0     2241 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/modules/datamodule_base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.636225 lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/
+-rw-rw-rw-   0        0        0        0 2022-02-09 11:07:33.000000 lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/__init__.py
+-rw-rw-rw-   0        0        0     1346 2022-02-21 13:22:43.000000 lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/digit5_datamodule.py
+-rw-rw-rw-   0        0        0     8577 2023-04-18 12:36:07.000000 lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/domainAdaptation_base.py
+-rw-rw-rw-   0        0        0     1394 2022-02-21 13:23:46.000000 lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/domainNet_datamodule.py
+-rw-rw-rw-   0        0        0     1363 2023-04-18 12:39:48.000000 lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/office31_datamodule.py
+-rw-rw-rw-   0        0        0     1405 2022-02-21 13:22:15.000000 lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/officeHome_datamodule.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.654235 lightningdata-modules-0.1.7/lightningdata/modules/federated_learning/
+-rw-rw-rw-   0        0        0        0 2022-02-10 14:34:26.000000 lightningdata-modules-0.1.7/lightningdata/modules/federated_learning/__init__.py
+-rw-rw-rw-   0        0        0     1048 2022-02-11 09:46:51.000000 lightningdata-modules-0.1.7/lightningdata/modules/federated_learning/emnist_datamodule.py
+-rw-rw-rw-   0        0        0     3966 2022-11-09 12:58:43.000000 lightningdata-modules-0.1.7/lightningdata/modules/federated_learning/federatedLearning_base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.679233 lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/
+-rw-rw-rw-   0        0        0        0 2022-04-12 08:56:02.000000 lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/__init__.py
+-rw-rw-rw-   0        0        0     3378 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/metaLearning_base.py
+-rw-rw-rw-   0        0        0     2181 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py
+-rw-rw-rw-   0        0        0     2156 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/omiglot_datamodule.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.681233 lightningdata-modules-0.1.7/lightningdata/thirdparty/
+-rw-rw-rw-   0        0        0        0 2022-11-09 14:16:25.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.701238 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/
+-rw-rw-rw-   0        0        0      352 2022-11-09 14:09:26.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.865237 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/
+-rw-rw-rw-   0        0        0     1620 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/__init__.py
+-rw-rw-rw-   0        0        0    19222 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/bach.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:41.898235 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/
+-rw-rw-rw-   0        0        0      195 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/__init__.py
+-rw-rw-rw-   0        0        0     6861 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py
+-rw-rw-rw-   0        0        0     5332 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py
+-rw-rw-rw-   0        0        0     5708 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py
+-rw-rw-rw-   0        0        0    10048 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cub.py
+-rw-rw-rw-   0        0        0    10334 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py
+-rw-rw-rw-   0        0        0    14448 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/helpers.py
+-rw-rw-rw-   0        0        0     6522 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py
+-rw-rw-rw-   0        0        0    11646 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/letter.py
+-rw-rw-rw-   0        0        0     9242 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py
+-rw-rw-rw-   0        0        0    11285 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/omniglot.py
+-rw-rw-rw-   0        0        0    14763 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py
+-rw-rw-rw-   0        0        0    14686 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py
+-rw-rw-rw-   0        0        0    14786 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py
+-rw-rw-rw-   0        0        0    10004 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py
+-rw-rw-rw-   0        0        0    21872 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/tcga.py
+-rw-rw-rw-   0        0        0    10696 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py
+-rw-rw-rw-   0        0        0    10345 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py
+-rw-rw-rw-   0        0        0     1975 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:42.019225 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/
+-rw-rw-rw-   0        0        0     1100 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/__init__.py
+-rw-rw-rw-   0        0        0     2576 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/activation.py
+-rw-rw-rw-   0        0        0     2301 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/batchnorm.py
+-rw-rw-rw-   0        0        0      736 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/container.py
+-rw-rw-rw-   0        0        0     1149 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/conv.py
+-rw-rw-rw-   0        0        0      786 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/linear.py
+-rw-rw-rw-   0        0        0     2437 2022-11-09 13:14:11.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/module.py
+-rw-rw-rw-   0        0        0      555 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/normalization.py
+-rw-rw-rw-   0        0        0     2091 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/parallel.py
+-rw-rw-rw-   0        0        0     1084 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/sparse.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:42.080237 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/
+-rw-rw-rw-   0        0        0      345 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/__init__.py
+-rw-rw-rw-   0        0        0     5592 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/harmonic.py
+-rw-rw-rw-   0        0        0     4121 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/helpers.py
+-rw-rw-rw-   0        0        0     4744 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/sinusoid.py
+-rw-rw-rw-   0        0        0     6312 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:42.164215 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/
+-rw-rw-rw-   0        0        0      556 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2589 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/augmentations.py
+-rw-rw-rw-   0        0        0     2748 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/categorical.py
+-rw-rw-rw-   0        0        0    16328 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/splitters.py
+-rw-rw-rw-   0        0        0      555 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py
+-rw-rw-rw-   0        0        0     1325 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py
+-rw-rw-rw-   0        0        0     1139 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:42.247214 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/
+-rw-rw-rw-   0        0        0      843 2022-11-09 14:09:46.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:42.319224 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/
+-rw-rw-rw-   0        0        0      818 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/__init__.py
+-rw-rw-rw-   0        0        0     2651 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py
+-rw-rw-rw-   0        0        0    13806 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/dataset.py
+-rw-rw-rw-   0        0        0     2113 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/sampler.py
+-rw-rw-rw-   0        0        0     2190 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/task.py
+-rw-rw-rw-   0        0        0     3129 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py
+-rw-rw-rw-   0        0        0     2330 2022-11-09 14:09:55.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/gradient_based.py
+-rw-rw-rw-   0        0        0     7624 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/matching.py
+-rw-rw-rw-   0        0        0     4277 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/metrics.py
+-rw-rw-rw-   0        0        0     2832 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/prototype.py
+-rw-rw-rw-   0        0        0     4966 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/r2d2.py
+-rw-rw-rw-   0        0        0       17 2022-11-09 13:14:09.000000 lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:42:42.342224 lightningdata-modules-0.1.7/lightningdata_modules.egg-info/
+-rw-rw-rw-   0        0        0     2430 2023-04-18 12:42:41.000000 lightningdata-modules-0.1.7/lightningdata_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4581 2023-04-18 12:42:41.000000 lightningdata-modules-0.1.7/lightningdata_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 12:42:41.000000 lightningdata-modules-0.1.7/lightningdata_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-04-18 12:42:41.000000 lightningdata-modules-0.1.7/lightningdata_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 12:42:41.000000 lightningdata-modules-0.1.7/lightningdata_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 12:42:42.345223 lightningdata-modules-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-04-18 12:39:24.000000 lightningdata-modules-0.1.7/setup.py
```

### Comparing `lightningdata-modules-0.1.6/PKG-INFO` & `lightningdata-modules-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningdata-modules
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pre-packages Pytorch-Lightning datasets
 Home-page: https://github.com/ManuelRoeder/lightningdata-modules
 Author: Manuel Roeder
 Author-email: manuel.roeder@web.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lightningdata-modules-0.1.6/README.md` & `lightningdata-modules-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/__init__.py` & `lightningdata-modules-0.1.7/lightningdata/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/common/config.py` & `lightningdata-modules-0.1.7/lightningdata/common/config.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/common/folder2lmdb.py` & `lightningdata-modules-0.1.7/lightningdata/common/folder2lmdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,20 @@
             self.open_lmdb()
 
         img, target = None, None
         byteflow = self.txn.get(self.keys[index])
         unpacked = pickle.loads(byteflow)
 
         # load image
-        imgbuf = unpacked[0]
+        if type(unpacked[0]) is tuple:
+            imgbuf = unpacked[0][0]
+        else:
+            imgbuf = unpacked[0]
         buf = six.BytesIO()
-        buf.write(imgbuf[0])
+        buf.write(imgbuf)
         buf.seek(0)
         img = Image.open(buf)
 
         # load label
         target = unpacked[1]
 
         if self.transform is not None:
```

### Comparing `lightningdata-modules-0.1.6/lightningdata/common/pre_process.py` & `lightningdata-modules-0.1.7/lightningdata/common/pre_process.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/common/utils.py` & `lightningdata-modules-0.1.7/lightningdata/common/utils.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/datamodule_base.py` & `lightningdata-modules-0.1.7/lightningdata/modules/datamodule_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/digit5_datamodule.py` & `lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/digit5_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainAdaptation_base.py` & `lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/domainAdaptation_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,23 +40,23 @@
 
     def get_train_transform(self):
         if self.train_transform:
             print("Using user-defined training data augmentation")
             return self.train_transform
         else:
             print("Using default training data augmentation")
-            return self._default_train_transforms
+            return self._default_train_transforms()
 
     def get_test_transform(self):
         if self.test_transform:
             print("Using user-defined test data augmentation")
             return self.test_transform
         else:
             print("Using default test data augmentation")
-            return self._default_test_transforms
+            return self._default_test_transforms()
 
     def __prepare_dataset(self, root: str, remote_folder: str, ds_name: str, domain: str, split: bool) -> bool:
         print("Domain " + domain + " available")
         dataset_path = os.path.join(root, ds_name)
         # collect the subsets
         subsets = []
         if split:
```

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainNet_datamodule.py` & `lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/domainNet_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/office31_datamodule.py` & `lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/office31_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/officeHome_datamodule.py` & `lightningdata-modules-0.1.7/lightningdata/modules/domain_adaptation/officeHome_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/emnist_datamodule.py` & `lightningdata-modules-0.1.7/lightningdata/modules/federated_learning/emnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/federatedLearning_base.py` & `lightningdata-modules-0.1.7/lightningdata/modules/federated_learning/federatedLearning_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/metaLearning_base.py` & `lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/metaLearning_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py` & `lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/omiglot_datamodule.py` & `lightningdata-modules-0.1.7/lightningdata/modules/meta_learning/omiglot_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/__init__.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/bach.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/bach.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cub.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/cub.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/helpers.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/letter.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/letter.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/omniglot.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/omniglot.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tcga.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/tcga.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/utils.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/__init__.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/activation.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/activation.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/batchnorm.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/container.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/container.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/conv.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/conv.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/linear.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/linear.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/module.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/module.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/normalization.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/parallel.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/parallel.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/sparse.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/harmonic.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/harmonic.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/helpers.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/helpers.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/sinusoid.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/__init__.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/augmentations.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/augmentations.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/categorical.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/categorical.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/splitters.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/splitters.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/utils.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/__init__.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/__init__.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataset.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/sampler.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/sampler.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/task.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/task.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/gradient_based.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/gradient_based.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/matching.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/matching.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/metrics.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/prototype.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/prototype.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/r2d2.py` & `lightningdata-modules-0.1.7/lightningdata/thirdparty/torchmeta/utils/r2d2.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/lightningdata_modules.egg-info/PKG-INFO` & `lightningdata-modules-0.1.7/lightningdata_modules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningdata-modules
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pre-packages Pytorch-Lightning datasets
 Home-page: https://github.com/ManuelRoeder/lightningdata-modules
 Author: Manuel Roeder
 Author-email: manuel.roeder@web.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lightningdata-modules-0.1.6/lightningdata_modules.egg-info/SOURCES.txt` & `lightningdata-modules-0.1.7/lightningdata_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.6/setup.py` & `lightningdata-modules-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 required_packages = [
     "getfilelistpy", "lmdb", "matplotlib", "numpy", "Pillow", "pytorch_lightning", "setuptools",
     "six", "torch", "torchvision", "py7zr"
 ]
 
 setup(
     name="lightningdata-modules",
-    version="0.1.6",
+    version="0.1.7",
     description="Pre-packages Pytorch-Lightning datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ManuelRoeder/lightningdata-modules",
     author="Manuel Roeder",
     author_email="manuel.roeder@web.de",
     license="MIT",
```

