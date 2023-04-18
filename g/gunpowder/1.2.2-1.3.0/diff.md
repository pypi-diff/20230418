# Comparing `tmp/gunpowder-1.2.2.tar.gz` & `tmp/gunpowder-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gunpowder-1.2.2.tar", last modified: Tue Oct  5 01:35:55 2021, max compression
+gzip compressed data, was "gunpowder-1.3.0.tar", last modified: Tue Apr 18 17:37:06 2023, max compression
```

## Comparing `gunpowder-1.2.2.tar` & `gunpowder-1.3.0.tar`

### file list

```diff
@@ -1,111 +1,124 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/
--rw-rw-r--   0 jan       (1000) jan       (1000)      315 2021-10-05 01:35:55.273517 gunpowder-1.2.2/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     1343 2020-11-30 17:43:54.000000 gunpowder-1.2.2/README.md
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.269517 gunpowder-1.2.2/gunpowder/
--rw-rw-r--   0 jan       (1000) jan       (1000)      647 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6221 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/array.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3348 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/array_spec.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6504 2021-10-05 01:21:06.000000 gunpowder-1.2.2/gunpowder/batch.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4482 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/batch_request.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      672 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/build.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      355 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/compat.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.269517 gunpowder-1.2.2/gunpowder/contrib/
--rw-rw-r--   0 jan       (1000) jan       (1000)       61 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/contrib/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.269517 gunpowder-1.2.2/gunpowder/contrib/nodes/
--rw-rw-r--   0 jan       (1000) jan       (1000)      558 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    10657 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/add_blobs_from_points.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7352 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/add_boundary_distance_gradients.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5101 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5318 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    16279 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/add_vector_map.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     8923 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/dvid_partner_annotation_source.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5813 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/hdf5_points_source.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2773 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/prepare_malis.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      918 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/contrib/nodes/zero_out_const_sections.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5033 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/coordinate.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.269517 gunpowder-1.2.2/gunpowder/ext/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1346 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/ext/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      322 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/ext/zarr_file.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      377 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/freezable.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    20473 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/graph.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2018 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/graph_spec.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3252 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/morphology.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      386 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/ndarray.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/gunpowder/nodes/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1622 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    10021 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/add_affinities.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5731 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/balance_labels.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     8438 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/batch_filter.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12631 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/batch_provider.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2648 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/crop.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4301 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/csv_points_source.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4464 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/daisy_request_blocks.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12750 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/defect_augment.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2058 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/downsample.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     8781 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/dvid_source.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    23905 2021-10-05 00:48:40.000000 gunpowder-1.2.2/gunpowder/nodes/elastic_augment.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3615 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/exclude_labels.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7364 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/generic_predict.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7351 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/generic_train.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3308 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/grow_boundary.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1629 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/hdf5_source.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1610 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/hdf5_write.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7216 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/hdf5like_source_base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7771 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/hdf5like_write_base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3168 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/intensity_augment.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      688 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/intensity_scale_shift.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6847 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/klb_source.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2432 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/merge_provider.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1974 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/noise_augment.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2415 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/normalize.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4136 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/pad.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4232 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/precache.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3857 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/print_profiling_stats.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    16715 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/random_location.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2356 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/random_provider.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    15368 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/rasterize_graph.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4164 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/reject.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      868 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/renumber_connected_components.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    14255 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/scan.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    11408 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/shift_augment.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    11509 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/simple_augment.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     8095 2021-10-05 01:15:08.000000 gunpowder-1.2.2/gunpowder/nodes/snapshot.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6046 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/specified_location.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1780 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/squeeze.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1554 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/stack.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1704 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/unsqueeze.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2802 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/upsample.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2353 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/nodes/zarr_source.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2708 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/nodes/zarr_write.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6704 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/pipeline.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4669 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/producer_pool.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3892 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/profiling.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7497 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/provider_spec.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12185 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/roi.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/gunpowder/tensorflow/
--rw-rw-r--   0 jan       (1000) jan       (1000)       99 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/tensorflow/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1707 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/tensorflow/local_server.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/gunpowder/tensorflow/nodes/
--rw-rw-r--   0 jan       (1000) jan       (1000)       94 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/tensorflow/nodes/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    13143 2021-10-05 01:21:06.000000 gunpowder-1.2.2/gunpowder/tensorflow/nodes/predict.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12979 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/tensorflow/nodes/train.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/gunpowder/torch/
--rw-rw-r--   0 jan       (1000) jan       (1000)       61 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/torch/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/gunpowder/torch/nodes/
--rw-rw-r--   0 jan       (1000) jan       (1000)      126 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/torch/nodes/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5677 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/torch/nodes/predict.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    13087 2020-11-30 17:43:54.000000 gunpowder-1.2.2/gunpowder/torch/nodes/train.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      537 2021-10-05 01:23:01.000000 gunpowder-1.2.2/gunpowder/version_info.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/gunpowder/zoo/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/zoo/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.273517 gunpowder-1.2.2/gunpowder/zoo/tensorflow/
--rw-rw-r--   0 jan       (1000) jan       (1000)       34 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/zoo/tensorflow/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6760 2020-07-15 15:59:45.000000 gunpowder-1.2.2/gunpowder/zoo/tensorflow/unet.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-10-05 01:35:55.269517 gunpowder-1.2.2/gunpowder.egg-info/
--rw-rw-r--   0 jan       (1000) jan       (1000)      315 2021-10-05 01:35:55.000000 gunpowder-1.2.2/gunpowder.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     3059 2021-10-05 01:35:55.000000 gunpowder-1.2.2/gunpowder.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2021-10-05 01:35:55.000000 gunpowder-1.2.2/gunpowder.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)      126 2021-10-05 01:35:55.000000 gunpowder-1.2.2/gunpowder.egg-info/requires.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       10 2021-10-05 01:35:55.000000 gunpowder-1.2.2/gunpowder.egg-info/top_level.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       38 2021-10-05 01:35:55.273517 gunpowder-1.2.2/setup.cfg
--rw-rw-r--   0 jan       (1000) jan       (1000)     1528 2021-10-05 01:15:08.000000 gunpowder-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 17:36:53.000000 gunpowder-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-18 17:37:06.136411 gunpowder-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-18 17:36:53.000000 gunpowder-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.116410 gunpowder-1.3.0/gunpowder/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/array_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.120411 gunpowder-1.3.0/gunpowder/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.120411 gunpowder-1.3.0/gunpowder/contrib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/add_blobs_from_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/add_boundary_distance_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/add_vector_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/dvid_partner_annotation_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/hdf5_points_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/prepare_malis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/contrib/nodes/zero_out_const_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.120411 gunpowder-1.3.0/gunpowder/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/ext/zarr_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/freezable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20695 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.120411 gunpowder-1.3.0/gunpowder/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/jax/generic_jax_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.124410 gunpowder-1.3.0/gunpowder/jax/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/jax/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/jax/nodes/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/jax/nodes/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/gunpowder/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/add_affinities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/balance_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/batch_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/batch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/csv_points_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/daisy_request_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/defect_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/deform_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/dvid_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24005 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/elastic_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/exclude_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/generic_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/generic_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/graph_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/grow_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/hdf5_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/hdf5_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/hdf5like_source_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/hdf5like_write_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/intensity_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/intensity_scale_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/iterate_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/klb_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/merge_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/noise_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/precache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/print_profiling_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/random_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/random_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/rasterize_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/renumber_connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/shift_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/simple_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/specified_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/zarr_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/nodes/zarr_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/producer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/provider_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/gunpowder/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/tensorflow/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/gunpowder/tensorflow/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/tensorflow/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/tensorflow/nodes/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/tensorflow/nodes/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/gunpowder/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/gunpowder/torch/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/torch/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/torch/nodes/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/torch/nodes/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/gunpowder/zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.136411 gunpowder-1.3.0/gunpowder/zoo/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/zoo/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-18 17:36:53.000000 gunpowder-1.3.0/gunpowder/zoo/tensorflow/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:06.120411 gunpowder-1.3.0/gunpowder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-18 17:37:06.000000 gunpowder-1.3.0/gunpowder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-18 17:37:06.000000 gunpowder-1.3.0/gunpowder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:37:06.000000 gunpowder-1.3.0/gunpowder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-18 17:37:06.000000 gunpowder-1.3.0/gunpowder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 17:37:06.000000 gunpowder-1.3.0/gunpowder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-18 17:36:53.000000 gunpowder-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:37:06.136411 gunpowder-1.3.0/setup.cfg
```

### Comparing `gunpowder-1.2.2/gunpowder/__init__.py` & `gunpowder-1.3.0/gunpowder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import absolute_import
 
-from . import nodes
 from .nodes import *
 
 from .array import Array, ArrayKey, ArrayKeys
 from .array_spec import ArraySpec
 from .batch import Batch
 from .batch_request import BatchRequest
 from .build import build
@@ -15,8 +14,9 @@
 from .producer_pool import ProducerPool
 from .provider_spec import ProviderSpec
 from .roi import Roi
 from .version_info import _version as version
 import gunpowder.contrib
 import gunpowder.tensorflow
 import gunpowder.torch
+import gunpowder.jax
 import gunpowder.zoo
```

### Comparing `gunpowder-1.2.2/gunpowder/array.py` & `gunpowder-1.3.0/gunpowder/array.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from gunpowder.roi import Roi
 import logging
 import numpy as np
 import copy
 
 logger = logging.getLogger(__name__)
 
+
 class Array(Freezable):
-    '''A numpy array with a specification describing the data.
+    """A numpy array with a specification describing the data.
 
     Args:
 
         data (array-like):
 
             The data to be stored in the array. Will be converted to a numpy
             array, if necessary.
@@ -21,67 +22,72 @@
         spec (:class:`ArraySpec`, optional):
 
             A spec describing the data.
 
         attrs (``dict``, optional):
 
             Optional attributes to describe this array.
-    '''
+    """
 
     def __init__(self, data, spec=None, attrs=None):
-
         self.spec = deepcopy(spec)
         self.data = np.asarray(data)
         self.attrs = attrs
 
         if attrs is None:
             self.attrs = {}
 
-        if (
-                spec is not None and
-                spec.roi is not None and
-                spec.voxel_size is not None):
-
+        if spec is not None and spec.roi is not None and spec.voxel_size is not None:
             for d in range(len(spec.voxel_size)):
-                assert spec.voxel_size[d]*data.shape[-spec.roi.dims()+d] == spec.roi.get_shape()[d], \
-                        "ROI %s does not align with voxel size %s * data shape %s"%(spec.roi, spec.voxel_size, data.shape)
-                if spec.roi.get_offset()[d] is not None:
-                    assert spec.roi.get_offset()[d] % spec.voxel_size[d] == 0,\
-                            "ROI offset %s must be a multiple of voxel size %s"\
-                            % (spec.roi.get_offset(), spec.voxel_size)
+                assert (
+                    spec.voxel_size[d] * data.shape[-spec.roi.dims + d]
+                    == spec.roi.shape[d]
+                ), "ROI %s does not align with voxel size %s * data shape %s" % (
+                    spec.roi,
+                    spec.voxel_size,
+                    data.shape,
+                )
+                if spec.roi.offset[d] is not None:
+                    assert (
+                        spec.roi.offset[d] % spec.voxel_size[d] == 0
+                    ), "ROI offset %s must be a multiple of voxel size %s" % (
+                        spec.roi.offset,
+                        spec.voxel_size,
+                    )
 
         if spec.dtype is not None:
-            assert data.dtype == spec.dtype, \
-                "data dtype %s does not match spec dtype %s" % (data.dtype, spec.dtype)
+            assert (
+                data.dtype == spec.dtype
+            ), "data dtype %s does not match spec dtype %s" % (data.dtype, spec.dtype)
 
         self.freeze()
 
     def crop(self, roi, copy=True):
-        '''Create a cropped copy of this Array.
+        """Create a cropped copy of this Array.
 
         Args:
 
             roi (:class:`Roi`):
 
                 ROI in world units to crop to.
 
             copy (``bool``):
 
                 Make a copy of the data.
-        '''
+        """
 
-        assert self.spec.roi.contains(roi), (
-            "Requested crop ROI (%s) doesn't fit in array (%s)" %
-            (roi, self.spec.roi))
+        assert self.spec.roi.contains(
+            roi
+        ), "Requested crop ROI (%s) doesn't fit in array (%s)" % (roi, self.spec.roi)
 
         if self.spec.roi == roi and not copy:
             return self
 
         voxel_size = self.spec.voxel_size
-        data_roi = (roi - self.spec.roi.get_offset())/voxel_size
+        data_roi = (roi - self.spec.roi.offset) / voxel_size
         slices = data_roi.get_bounding_box()
 
         while len(slices) < len(self.data.shape):
             slices = (slice(None),) + slices
 
         data = self.data[slices]
         if copy:
@@ -89,36 +95,38 @@
 
         spec = deepcopy(self.spec)
         attrs = deepcopy(self.attrs)
         spec.roi = deepcopy(roi)
         return Array(data, spec, attrs)
 
     def merge(self, array, copy_from_self=False, copy=False):
-        '''Merge this array with another one. The resulting array will have the
+        """Merge this array with another one. The resulting array will have the
         size of the larger one, with values replaced from ``array``.
 
         This only works if one of the two arrays is contained in the other. In
         this case, ``array`` will overwrite values in ``self`` (unless
         ``copy_from_self`` is set to ``True``).
 
         A copy will only be made if necessary or ``copy`` is set to ``True``.
-        '''
+        """
         # It is unclear how to merge arrays in all cases. Consider a 10x10 array,
         # you crop out a 5x5 area, do a shift augment, and attempt to merge.
         # What does that mean? specs have changed. It should be a new key.
         raise NotImplementedError("Merge function should not be used!")
 
         self_roi = self.spec.roi
         array_roi = array.spec.roi
 
-        assert self_roi.contains(array_roi) or array_roi.contains(self_roi), \
-            "Can not merge arrays that are not contained in each other."
-
-        assert self.spec.voxel_size == array.spec.voxel_size, \
-            "Can not merge arrays with different voxel sizes."
+        assert self_roi.contains(array_roi) or array_roi.contains(
+            self_roi
+        ), "Can not merge arrays that are not contained in each other."
+
+        assert (
+            self.spec.voxel_size == array.spec.voxel_size
+        ), "Can not merge arrays with different voxel sizes."
 
         # make sure self contains array
         if not self_roi.contains(array_roi):
             return array.merge(self, not copy_from_self, copy)
 
         # -> here we know that self contains array
 
@@ -132,69 +140,71 @@
         if self_roi == array_roi:
             return array if not copy else deepcopy(array)
 
         # part of self have to be replaced, a copy is needed
         merged = deepcopy(self)
 
         voxel_size = self.spec.voxel_size
-        data_roi = (array_roi - self_roi.get_offset())/voxel_size
+        data_roi = (array_roi - self_roi.offset) / voxel_size
         slices = data_roi.get_bounding_box()
 
         while len(slices) < len(self.data.shape):
             slices = (slice(None),) + slices
 
         merged.data[slices] = array.data
 
         return merged
 
     def __repr__(self):
         return str(self.spec)
 
     def copy(self):
-        '''Create a copy of this array.'''
+        """Create a copy of this array."""
         return copy.deepcopy(self)
 
 
 class ArrayKey(Freezable):
-    '''A key to identify arrays in requests, batches, and across nodes.
+    """A key to identify arrays in requests, batches, and across nodes.
 
     Used as key in :class:`BatchRequest` and :class:`Batch` to retrieve array
     specs or arrays.
 
     Args:
 
         identifier (``string``):
 
             A unique, human readable identifier for this array key. Will be
             used in log messages and to look up arrays in requests and batches.
             Should be upper case (like ``RAW``, ``GT_LABELS``). The identifier
             is unique: Two array keys with the same identifier will refer to
             the same array.
-    '''
+    """
 
     def __init__(self, identifier):
         self.identifier = identifier
         self.hash = hash(identifier)
         self.freeze()
         logger.debug("Registering array key %s", self)
         setattr(ArrayKeys, self.identifier, self)
 
     def __eq__(self, other):
-        return hasattr(other, 'identifier') and self.identifier == other.identifier
+        return hasattr(other, "identifier") and self.identifier == other.identifier
 
     def __hash__(self):
         return self.hash
 
     def __repr__(self):
         return self.identifier
 
+
 class ArrayKeys:
-    '''Convenience access to all created :class:``ArrayKey``s. A key generated
+    """Convenience access to all created :class:``ArrayKey``s. A key generated
     with::
 
         raw = ArrayKey('RAW')
 
     can be retrieved as::
 
         ArrayKeys.RAW
-    '''
+    """
+
     pass
```

### Comparing `gunpowder-1.2.2/gunpowder/array_spec.py` & `gunpowder-1.3.0/gunpowder/array_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 from .coordinate import Coordinate
 from .freezable import Freezable
 
+
 class ArraySpec(Freezable):
-    '''Contains meta-information about an array. This is used by
+    """Contains meta-information about an array. This is used by
     :class:`BatchProviders<BatchProvider>` to communicate the arrays they
     offer, as well as by :class:`Arrays<Array>` to describe the data they
     contain.
 
     Attributes:
 
         roi (:class:`Roi`):
@@ -30,42 +31,40 @@
             If set, this array does not represent spatial data (e.g., a list of
             labels for samples in a batch). ``roi`` and ``voxel_size`` have to
             be ``None``. No consistency checks will be performed.
 
         dtype (``np.dtype``):
 
             The data type of the array.
-    '''
+    """
 
     def __init__(
-            self,
-            roi=None,
-            voxel_size=None,
-            interpolatable=None,
-            nonspatial=False,
-            dtype=None,
-            placeholder=False):
-
+        self,
+        roi=None,
+        voxel_size=None,
+        interpolatable=None,
+        nonspatial=False,
+        dtype=None,
+        placeholder=False,
+    ):
         self.roi = roi
         self.voxel_size = None if voxel_size is None else Coordinate(voxel_size)
         self.interpolatable = interpolatable
         self.nonspatial = nonspatial
         self.dtype = dtype
         self.placeholder = placeholder
 
         if nonspatial:
             assert roi is None, "Non-spatial arrays can not have a ROI"
-            assert voxel_size is None, "Non-spatial arrays can not " \
-                "have a voxel size"
+            assert voxel_size is None, "Non-spatial arrays can not " "have a voxel size"
 
         self.freeze()
 
     def update_with(self, spec):
-        if self.roi is not None and \
-           spec.roi is not None:
+        if self.roi is not None and spec.roi is not None:
             self.roi = self.roi.union(spec.roi)
         elif spec.roi is not None:
             self.roi = spec.roi
 
         if spec.voxel_size is not None:
             self.voxel_size = spec.voxel_size
 
@@ -78,25 +77,23 @@
         if spec.dtype is not None:
             self.dtype = spec.dtype
 
         if spec.placeholder is not None:
             self.placeholder = spec.placeholder
 
     def copy(self):
-        '''Create a copy of this spec.'''
+        """Create a copy of this spec."""
         return copy.deepcopy(self)
 
     def __eq__(self, other):
-
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return NotImplemented
 
     def __ne__(self, other):
-
         if isinstance(other, self.__class__):
             return not self.__eq__(other)
         return NotImplemented
 
     def __repr__(self):
         r = ""
         r += "ROI: " + str(self.roi) + ", "
```

### Comparing `gunpowder-1.2.2/gunpowder/batch.py` & `gunpowder-1.3.0/gunpowder/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from .freezable import Freezable
 from .profiling import ProfilingStats
 from .array import Array, ArrayKey
 from .graph import Graph, GraphKey
 
 logger = logging.getLogger(__name__)
 
+
 class Batch(Freezable):
-    '''Contains the requested batch as a collection of :class:`Arrays<Array>`
+    """Contains the requested batch as a collection of :class:`Arrays<Array>`
     and :class:`Graph` that is passed through the pipeline from sources to
     sinks.
 
     This collection mimics a dictionary. Items can be added with::
 
         batch = Batch()
         batch[array_key] = Array(...)
@@ -38,107 +39,106 @@
         arrays (dict from :class:`ArrayKey` to :class:`Array`):
 
             Contains all arrays that have been requested for this batch.
 
         graphs (dict from :class:`GraphKey` to :class:`Graph`):
 
             Contains all graphs that have been requested for this batch.
-    '''
+    """
 
-    __next_id = multiprocessing.Value('L')
+    __next_id = multiprocessing.Value("L")
 
     @staticmethod
     def get_next_id():
         with Batch.__next_id.get_lock():
             next_id = Batch.__next_id.value
             Batch.__next_id.value += 1
         return next_id
 
     def __init__(self):
-
         self.id = Batch.get_next_id()
         self.profiling_stats = ProfilingStats()
         self.arrays = {}
         self.graphs = {}
         self.affinity_neighborhood = None
         self.loss = None
         self.iteration = None
 
         self.freeze()
 
     def __setitem__(self, key, value):
-
         if isinstance(value, Array):
-            assert isinstance(key, ArrayKey), (
-                "Only a ArrayKey is allowed as key for an Array value.")
+            assert isinstance(
+                key, ArrayKey
+            ), "Only a ArrayKey is allowed as key for an Array value."
             self.arrays[key] = value
 
         elif isinstance(value, Graph):
             assert isinstance(
                 key, GraphKey
             ), f"Only a GraphKey is allowed as key for Graph value."
             self.graphs[key] = value
 
         else:
             raise RuntimeError(
-                "Only Array or Graph can be set in a %s."%type(self).__name__)
+                "Only Array or Graph can be set in a %s." % type(self).__name__
+            )
 
     def __getitem__(self, key):
-
         if isinstance(key, ArrayKey):
             return self.arrays[key]
 
         elif isinstance(key, GraphKey):
             return self.graphs[key]
 
         else:
             raise RuntimeError(
                 "Only ArrayKey or GraphKey can be used as keys in a "
-                "%s."%type(self).__name__)
+                "%s." % type(self).__name__
+            )
 
     def __len__(self):
-
         return len(self.arrays) + len(self.graphs)
 
     def __contains__(self, key):
-
         if isinstance(key, ArrayKey):
             return key in self.arrays
 
         elif isinstance(key, GraphKey):
             return key in self.graphs
 
         else:
             raise RuntimeError(
                 "Only ArrayKey or GraphKey can be used as keys in a "
-                "%s. Key %s is a %s"%(type(self).__name__, key, type(key).__name__))
+                "%s. Key %s is a %s" % (type(self).__name__, key, type(key).__name__)
+            )
 
     def __delitem__(self, key):
-
         if isinstance(key, ArrayKey):
             del self.arrays[key]
 
         elif isinstance(key, GraphKey):
             del self.graphs[key]
 
         else:
             raise RuntimeError(
                 "Only ArrayKey or GraphKey can be used as keys in a "
-                "%s."%type(self).__name__)
+                "%s." % type(self).__name__
+            )
 
     def items(self):
-        '''Provides a generator iterating over key/value pairs.'''
+        """Provides a generator iterating over key/value pairs."""
 
-        for (k, v) in self.arrays.items():
+        for k, v in self.arrays.items():
             yield k, v
-        for (k, v) in self.graphs.items():
+        for k, v in self.graphs.items():
             yield k, v
 
     def get_total_roi(self):
-        '''Get the union of all the array ROIs in the batch.'''
+        """Get the union of all the array ROIs in the batch."""
 
         total_roi = None
 
         for _, array in self.arrays.items():
             if not array.spec.nonspatial:
                 if total_roi is None:
                     total_roi = array.spec.roi
@@ -150,23 +150,22 @@
                 total_roi = graph.spec.roi
             else:
                 total_roi = total_roi.union(graph.spec.roi)
 
         return total_roi
 
     def __repr__(self):
-
         r = "\n"
         for collection_type in [self.arrays, self.graphs]:
-            for (key, obj) in collection_type.items():
-                r += "\t%s: %s\n"%(key, obj.spec)
+            for key, obj in collection_type.items():
+                r += "\t%s: %s\n" % (key, obj.spec)
         return r
 
     def crop(self, request, copy=False):
-        '''Crop batch to meet the given request.'''
+        """Crop batch to meet the given request."""
 
         cropped = Batch()
         cropped.profiling_stats = self.profiling_stats
         cropped.loss = self.loss
         cropped.iteration = self.iteration
 
         for key, val in request.items():
@@ -178,27 +177,27 @@
                     cropped[key] = self[key].crop(val.roi)
                 else:
                     cropped[key] = self[key].crop(val.roi, copy)
 
         return cropped
 
     def merge(self, batch, merge_profiling_stats=True):
-        '''Merge this batch (``a``) with another batch (``b``).
+        """Merge this batch (``a``) with another batch (``b``).
 
         This creates a new batch ``c`` containing arrays and graphs from
         both batches ``a`` and ``b``:
 
             * Arrays or Graphs that exist in either ``a`` or ``b`` will be
               referenced in ``c`` (not copied).
 
             * Arrays or Graphs that exist in both batches will keep only
               a reference to the version in ``b`` in ``c``.
 
         All other cases will lead to an exception.
-        '''
+        """
 
         merged = shallow_copy(self)
 
         for key, val in batch.items():
             # TODO: What is the goal of `val.spec.roi is None`? Why should that
             # mean that the key in merged gets overwritten?
             if key not in merged or val.spec.roi is None:
```

### Comparing `gunpowder-1.2.2/gunpowder/batch_request.py` & `gunpowder-1.3.0/gunpowder/batch_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,32 +75,32 @@
 
     def copy(self):
         """Create a copy of this request."""
         return copy.deepcopy(self)
 
     @property
     def random_seed(self):
-        return self._random_seed % (2 ** 32)
+        return self._random_seed % (2**32)
 
     def _update_random_seed(self):
         self._random_seed = hash((self._random_seed + 1) ** 2)
 
     def __center_rois(self):
         """Ensure that all ROIs are centered around the same location."""
 
         total_roi = self.get_total_roi()
         if total_roi is None:
             return
 
-        center = total_roi.get_center()
+        center = total_roi.center
 
         for specs_type in [self.array_specs, self.graph_specs]:
             for key in specs_type:
                 roi = specs_type[key].roi
-                specs_type[key].roi = roi.shift(center - roi.get_center())
+                specs_type[key].roi = roi.shift(center - roi.center)
 
     def update_with(self, request):
         """Update current request with another"""
 
         assert isinstance(request, BatchRequest)
 
         merged = self.copy()
```

### Comparing `gunpowder-1.2.2/gunpowder/build.py` & `gunpowder-1.3.0/gunpowder/build.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
-class build(object):
 
+class build(object):
     def __init__(self, pipeline):
         self.pipeline = pipeline
 
     def __enter__(self):
         try:
             self.pipeline.setup()
         except:
-            logger.error("something went wrong during the setup of the pipeline, calling tear down")
+            logger.error(
+                "something went wrong during the setup of the pipeline, calling tear down"
+            )
             self.pipeline.internal_teardown()
             logger.debug("tear down completed")
             raise
         return self.pipeline
 
     def __exit__(self, type, value, traceback):
         logger.debug("leaving context, tearing down pipeline")
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/__init__.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/add_blobs_from_points.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/add_blobs_from_points.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import numpy as np
 
 from gunpowder.array import Array
 from gunpowder.nodes.batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
+
 class AddBlobsFromPoints(BatchFilter):
-    '''Add an array with blobs at locations given by a specified points
+    """Add an array with blobs at locations given by a specified points
     collection. The blobs are also restricted to stay within the same class in
     the restrictive_mask array that corresponds to the center voxel of the
     blob.
 
     Args:
 
         blob_settings(dict):
@@ -54,211 +55,225 @@
                   'output_array_dtype': 'int64',
                   'radius': 60,
                   'output_voxel_size': voxel_size,
                   'restrictive_mask_key': ArrayTypes.GT_LABELS,
                   'max_desired_overlap': 0.05
                 }
               }
-    '''
+    """
 
     def __init__(self, blob_settings):
-
         self.blob_settings = blob_settings
 
         for points_key, settings in self.blob_settings.items():
-            blob_settings[points_key]['blob_placer'] = BlobPlacer(
-                radius=settings['radius'],
-                voxel_size=settings['output_voxel_size'],
-                dtype=settings['output_array_dtype']
-                )
+            blob_settings[points_key]["blob_placer"] = BlobPlacer(
+                radius=settings["radius"],
+                voxel_size=settings["output_voxel_size"],
+                dtype=settings["output_array_dtype"],
+            )
 
     def setup(self):
         for blob_name, settings in self.blob_settings.items():
             self.provides(
-                settings['output_array_key'],
-                self.spec[settings['restrictive_mask_key']]
-                )
+                settings["output_array_key"],
+                self.spec[settings["restrictive_mask_key"]],
+            )
 
     def prepare(self, request):
-
         for blob_name, settings in self.blob_settings.items():
-            array_key = settings['output_array_key']
+            array_key = settings["output_array_key"]
             if array_key in request:
-
-                points_key = settings['points_key']
+                points_key = settings["points_key"]
                 request_roi = request[array_key].roi
 
-
                 # If point is not already requested, add to request
                 if points_key not in request.points_specs:
-                    request.add(points_key, request_roi.get_shape())
+                    request.add(points_key, request_roi.shape)
                 else:
-                    request[points_key].roi =\
-                     request[points_key].roi.union(request_roi)
+                    request[points_key].roi = request[points_key].roi.union(request_roi)
 
                 # Get correct size for restrictive_mask_key
-                restrictive_mask_key = settings['restrictive_mask_key']
+                restrictive_mask_key = settings["restrictive_mask_key"]
                 if restrictive_mask_key not in request.array_specs:
-                    request.add(restrictive_mask_key, request_roi.get_shape())
+                    request.add(restrictive_mask_key, request_roi.shape)
                 else:
-                    request[restrictive_mask_key].roi =\
-                     request[restrictive_mask_key].roi.union(request_roi)
+                    request[restrictive_mask_key].roi = request[
+                        restrictive_mask_key
+                    ].roi.union(request_roi)
             else:
                 # do nothing if no blobs of this type were requested
-                logger.warning('%s output array type for %s never requested. \
-                    Deleting entry...'%(settings['output_array_key'], blob_name))
+                logger.warning(
+                    "%s output array type for %s never requested. \
+                    Deleting entry..."
+                    % (settings["output_array_key"], blob_name)
+                )
                 del self.blob_settings[blob_name]
 
-
     def process(self, batch, request):
-
         # check arrays and gather all IDs and synapse IDs
         all_points = {}
         all_synapse_ids = {}
 
         for blob_name, settings in self.blob_settings.items():
             # Unpack settings
-            points_key = settings['points_key']
-            restrictive_mask_key = settings['restrictive_mask_key']
-
+            points_key = settings["points_key"]
+            restrictive_mask_key = settings["restrictive_mask_key"]
 
             # Make sure both the necesary point types and arrays are present
-            assert points_key in batch.points, "Upstream does not provide required point type\
-            : %s"%points_key
+            assert points_key in batch.points, (
+                "Upstream does not provide required point type\
+            : %s"
+                % points_key
+            )
 
-            assert restrictive_mask_key in batch.arrays, "Upstream does not provide required \
-            array type: %s"%restrictive_mask_key
+            assert restrictive_mask_key in batch.arrays, (
+                "Upstream does not provide required \
+            array type: %s"
+                % restrictive_mask_key
+            )
 
             # Get point data
             points = batch.points[points_key]
 
             # If point doesn't have it's corresponding partner, delete it
-            if 'partner_points' in settings.keys() and settings['partner_points'] is not None:
-                partner_points = batch.points[settings['partner_points']]
+            if (
+                "partner_points" in settings.keys()
+                and settings["partner_points"] is not None
+            ):
+                partner_points = batch.points[settings["partner_points"]]
                 synapse_ids = []
                 for point_id, point in points.data.items():
                     # pdb.set_trace()
                     if not point.partner_ids[0] in partner_points.data.keys():
-                        logger.warning('Point %s has no partner. Deleting...'%point_id)
+                        logger.warning(
+                            "Point %s has no partner. Deleting..." % point_id
+                        )
                         del points.data[point_id]
                     else:
                         synapse_ids.append(point.synapse_id)
 
             all_synapse_ids[points_key] = synapse_ids
             all_points[points_key] = points
 
         for blob_name, settings in self.blob_settings.items():
-
             # Unpack settings
-            points_key = settings['points_key']
-            array_key = settings['output_array_key']
-            voxel_size = settings['output_voxel_size']
-            restrictive_mask_key = settings['restrictive_mask_key']
-            restrictive_mask = batch.arrays[restrictive_mask_key].crop(request[array_key].roi)
+            points_key = settings["points_key"]
+            array_key = settings["output_array_key"]
+            voxel_size = settings["output_voxel_size"]
+            restrictive_mask_key = settings["restrictive_mask_key"]
+            restrictive_mask = batch.arrays[restrictive_mask_key].crop(
+                request[array_key].roi
+            )
 
-            id_mapper = settings['id_mapper']
-            dtype = settings['output_array_dtype']
+            id_mapper = settings["id_mapper"]
+            dtype = settings["output_array_dtype"]
 
             if id_mapper is not None:
                 id_mapper.make_map(all_points)
 
             # Initialize output array
-            shape_array = np.asarray(request[array_key].roi.get_shape())/voxel_size
+            shape_array = np.asarray(request[array_key].roi.shape) / voxel_size
             blob_map = np.zeros(shape_array, dtype=dtype)
 
             # Get point data
             points = batch.points[points_key]
 
-
-            offset = np.asarray(points.spec.roi.get_offset())
+            offset = np.asarray(points.spec.roi.offset)
             for point_id, point_data in points.data.items():
-                voxel_location = np.round(((point_data.location - offset)/(voxel_size))).astype('int32')
+                voxel_location = np.round(
+                    ((point_data.location - offset) / (voxel_size))
+                ).astype("int32")
 
                 synapse_id = point_data.synapse_id
                 # if mapping exists, do it
                 if id_mapper is not None:
                     synapse_id = id_mapper(synapse_id)
 
-                settings['blob_placer'].place(blob_map, voxel_location,
-                    synapse_id, restrictive_mask.data)
-
+                settings["blob_placer"].place(
+                    blob_map, voxel_location, synapse_id, restrictive_mask.data
+                )
 
             # Provide array
             batch.arrays[array_key] = Array(blob_map, spec=request[array_key].copy())
             batch.arrays[array_key].spec.dtype = dtype
 
             # add id_mapping to attributes
             if id_mapper is not None:
                 id_map_list = np.array(list(id_mapper.get_map().items()))
-                batch.arrays[array_key].attrs['id_mapping'] = id_map_list
+                batch.arrays[array_key].attrs["id_mapping"] = id_map_list
 
-            batch.arrays[array_key].attrs['point_ids'] = points.data.keys()
-            batch.arrays[array_key].attrs['synapse_ids'] = all_synapse_ids[points_key]
+            batch.arrays[array_key].attrs["point_ids"] = points.data.keys()
+            batch.arrays[array_key].attrs["synapse_ids"] = all_synapse_ids[points_key]
 
             # Crop all other requests
         for array_key, array in request.array_specs.items():
             batch.arrays[array_key] = batch.arrays[array_key].crop(array.roi)
 
         for points_key, points in request.points_specs.items():
             batch.points[points_key] = batch.points[points_key].spec.roi = points.roi
 
-class BlobPlacer:
-    ''' Places synapse array blobs from location data.
-        Args:
-            radius: int - that desired radius of synaptic blobs
-            voxel_size: array, list, tuple - voxel size in physical
-        '''
 
-    def __init__(self, radius, voxel_size, dtype='uint64'):
+class BlobPlacer:
+    """Places synapse array blobs from location data.
+    Args:
+        radius: int - that desired radius of synaptic blobs
+        voxel_size: array, list, tuple - voxel size in physical
+    """
 
+    def __init__(self, radius, voxel_size, dtype="uint64"):
         self.voxel_size = voxel_size
         if isinstance(self.voxel_size, (list, tuple)):
             self.voxel_size = np.asarray(self.voxel_size)
 
-        self.radius = (radius/self.voxel_size)
-        self.sphere_map = np.zeros(self.radius*2, dtype=dtype)
-        self.center = (np.asarray(self.sphere_map.shape))/2
-
-        ranges = [range(0, self.radius[0]*2),
-                  range(0, self.radius[1]*2),
-                  range(0, self.radius[2]*2)]
+        self.radius = radius / self.voxel_size
+        self.sphere_map = np.zeros(self.radius * 2, dtype=dtype)
+        self.center = (np.asarray(self.sphere_map.shape)) / 2
+
+        ranges = [
+            range(0, self.radius[0] * 2),
+            range(0, self.radius[1] * 2),
+            range(0, self.radius[2] * 2),
+        ]
 
         for index in np.asarray(list(itertools.product(*ranges))):
             # if distance less than r, place a 1
-            if np.linalg.norm((self.center - index)*self.voxel_size) <= radius:
+            if np.linalg.norm((self.center - index) * self.voxel_size) <= radius:
                 self.sphere_map[tuple(index)] = 1
 
         self.sphere_voxel_array = np.sum(self.sphere_map, axis=(0, 1, 2))
 
     def place(self, matrix, location, marker, mask):
-        ''' Places synapse
+        """Places synapse
         Args:
             matrix: 4D np array - 1st dim are for layers to avoid overlap
             (3 should be more than enough)
             location: np array - location where to place synaptic blob within given matrix
             marker: int - the ID used to mark this paricular synapse in the matrix
             mask:   3D np array - when placing a blob, will sample mask at
         center location and only place blob in interection where mask has
         the same ID. Usually used to restrict synaptic blobs inside their
         respective cells (using segmentation)
-        '''
+        """
         # Calculate cube circumscribing the sphere to place
         start = location - self.radius
         end = location + self.radius
 
         # check if sphere fits in matrix
         if np.all(start >= 0) and np.all(np.asarray(matrix.shape) - end >= 0):
-
             # calculate actual synapse shape from intersection between sphere and restrictive mask
             restricting_label = mask[location[0], location[1], location[2]]
 
-            restricting_mask = \
-            mask[start[0]:end[0], start[1]:end[1], start[2]:end[2]] == restricting_label
+            restricting_mask = (
+                mask[start[0] : end[0], start[1] : end[1], start[2] : end[2]]
+                == restricting_label
+            )
 
-            shape = (self.sphere_map*restricting_mask)
+            shape = self.sphere_map * restricting_mask
 
             # place shape in chosen layer
-            matrix[start[0]:end[0], start[1]:end[1], start[2]:end[2]] += shape*marker
+            matrix[start[0] : end[0], start[1] : end[1], start[2] : end[2]] += (
+                shape * marker
+            )
             return matrix, True
 
-        logger.warning('Location %s out of bounds'%(location))
+        logger.warning("Location %s out of bounds" % (location))
         return matrix, False
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/add_boundary_distance_gradients.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/add_boundary_distance_gradients.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from gunpowder.batch_request import BatchRequest
 from gunpowder.nodes.batch_filter import BatchFilter
 from numpy.lib.stride_tricks import as_strided
 from scipy.ndimage.morphology import distance_transform_edt
 
 logger = logging.getLogger(__name__)
 
+
 class AddBoundaryDistanceGradients(BatchFilter):
-    '''Add an array with vectors pointing away from the closest boundary.
+    """Add an array with vectors pointing away from the closest boundary.
 
     The vectors are the spacial gradients of the distance transform, i.e., the
     distance to the boundary between labels or the background label (0).
 
     Args:
 
         label_array_key(:class:``ArrayKey``): The array to read the labels
@@ -35,86 +36,82 @@
 
         scale(string, optional): ``None`` or ``exp``. If ``exp``, distance
             gradients will be scaled by ``beta*e**(-d*alpha)``, where ``d`` is
             the distance to the boundary.
 
         scale_args(tuple, optional): For ``exp`` a tuple with the values of
             ``alpha`` and ``beta``.
-    '''
+    """
 
     def __init__(
-            self,
-            label_array_key,
-            gradient_array_key,
-            distance_array_key=None,
-            boundary_array_key=None,
-            normalize=None,
-            scale=None,
-            scale_args=None):
-
+        self,
+        label_array_key,
+        gradient_array_key,
+        distance_array_key=None,
+        boundary_array_key=None,
+        normalize=None,
+        scale=None,
+        scale_args=None,
+    ):
         self.label_array_key = label_array_key
         self.gradient_array_key = gradient_array_key
         self.distance_array_key = distance_array_key
         self.boundary_array_key = boundary_array_key
         self.normalize = normalize
         self.scale = scale
         self.scale_args = scale_args
 
     def setup(self):
-
         assert self.label_array_key in self.spec, (
             "Upstream does not provide %s needed by "
-            "AddBoundaryDistanceGradients"%self.label_array_key)
+            "AddBoundaryDistanceGradients" % self.label_array_key
+        )
 
         spec = self.spec[self.label_array_key].copy()
         spec.dtype = np.float32
         self.provides(self.gradient_array_key, spec)
         if self.distance_array_key is not None:
             self.provides(self.distance_array_key, spec)
         if self.boundary_array_key is not None:
             spec.voxel_size /= 2
             self.provides(self.boundary_array_key, spec)
         self.enable_autoskip()
 
     def prepare(self, request):
-
         deps = BatchRequest()
         deps[self.label_array_key] = request[self.gradient_array_key]
 
         return deps
 
     def process(self, batch, request):
-
         if not self.gradient_array_key in request:
             return
 
         labels = batch.arrays[self.label_array_key].data
         voxel_size = self.spec[self.label_array_key].voxel_size
 
         # get boundaries between label regions
         boundaries = self.__find_boundaries(labels)
 
         # mark boundaries with 0 (not 1)
         boundaries = 1.0 - boundaries
 
         if np.sum(boundaries == 0) == 0:
-
             # no boundary -- no distance to compute
             distances = np.zeros(labels.shape, dtype=np.float32)
 
         else:
-
             # get distances (voxel_size/2 because image is doubled)
             distances = distance_transform_edt(
-                boundaries,
-                sampling=tuple(float(v)/2 for v in voxel_size))
+                boundaries, sampling=tuple(float(v) / 2 for v in voxel_size)
+            )
             distances = distances.astype(np.float32)
 
             # restore original shape
-            downsample = (slice(None, None, 2),)*len(voxel_size)
+            downsample = (slice(None, None, 2),) * len(voxel_size)
             distances = distances[downsample]
 
             # set distances in background to 0
             distances[labels == 0] = 0
 
         gradients = np.asarray(np.gradient(distances, *voxel_size))
 
@@ -128,89 +125,79 @@
         if self.scale is not None:
             self.__scale(gradients, distances, self.scale, self.scale_args)
 
         spec = self.spec[self.gradient_array_key].copy()
         spec.roi = request[self.gradient_array_key].roi
         batch.arrays[self.gradient_array_key] = Array(gradients, spec)
 
-        if (
-                self.distance_array_key is not None and
-                self.distance_array_key in request):
+        if self.distance_array_key is not None and self.distance_array_key in request:
             batch.arrays[self.distance_array_key] = Array(distances, spec)
 
-        if (
-                self.boundary_array_key is not None and
-                self.boundary_array_key in request):
-
+        if self.boundary_array_key is not None and self.boundary_array_key in request:
             # add one more face at each dimension, as boundary map has shape
             # 2*s - 1 of original shape s
             grown = np.ones(tuple(s + 1 for s in boundaries.shape))
             grown[tuple(slice(0, s) for s in boundaries.shape)] = boundaries
-            spec.voxel_size = voxel_size/2
+            spec.voxel_size = voxel_size / 2
             logger.debug("voxel size of boundary array: %s", spec.voxel_size)
             batch.arrays[self.boundary_array_key] = Array(grown, spec)
 
     def __find_boundaries(self, labels):
-
         # labels: 1 1 1 1 0 0 2 2 2 2 3 3       n
         # shift :   1 1 1 1 0 0 2 2 2 2 3       n - 1
         # diff  :   0 0 0 1 0 1 0 0 0 1 0       n - 1
         # bound.: 00000001000100000001000      2n - 1
 
         logger.debug("computing boundaries for %s", labels.shape)
 
         dims = len(labels.shape)
         in_shape = labels.shape
-        out_shape = tuple(2*s - 1 for s in in_shape)
+        out_shape = tuple(2 * s - 1 for s in in_shape)
         out_slices = tuple(slice(0, s) for s in out_shape)
 
-        boundaries = np.zeros(out_shape, dtype=np.bool)
+        boundaries = np.zeros(out_shape, dtype=bool)
 
         logger.debug("boundaries shape is %s", boundaries.shape)
 
         for d in range(dims):
-
             logger.debug("processing dimension %d", d)
 
-            shift_p = [slice(None)]*dims
+            shift_p = [slice(None)] * dims
             shift_p[d] = slice(1, in_shape[d])
 
-            shift_n = [slice(None)]*dims
+            shift_n = [slice(None)] * dims
             shift_n[d] = slice(0, in_shape[d] - 1)
 
             diff = (labels[tuple(shift_p)] - labels[tuple(shift_n)]) != 0
 
             logger.debug("diff shape is %s", diff.shape)
 
-            target = [slice(None, None, 2)]*dims
+            target = [slice(None, None, 2)] * dims
             target[d] = slice(1, out_shape[d], 2)
 
             logger.debug("target slices are %s", target)
 
             boundaries[tuple(target)] = diff
 
         return boundaries
 
     def __normalize(self, gradients, norm):
-
         dims = gradients.shape[0]
 
-        if norm == 'l1':
+        if norm == "l1":
             factors = sum([np.abs(gradients[d]) for d in range(dims)])
-        elif norm == 'l2':
-            factors = np.sqrt(
-                    sum([np.square(gradients[d]) for d in range(dims)]))
+        elif norm == "l2":
+            factors = np.sqrt(sum([np.square(gradients[d]) for d in range(dims)]))
         else:
-            raise RuntimeError('norm %s not supported'%norm)
+            raise RuntimeError("norm %s not supported" % norm)
 
         factors[factors < 1e-5] = 1
         gradients /= factors
 
     def __scale(self, gradients, distances, scale, scale_args):
-
         dims = gradients.shape[0]
 
-        if scale == 'exp':
+        if scale == "exp":
             alpha, beta = self.scale_args
-            factors = np.exp(-distances*alpha)*beta
+            factors = np.exp(-distances * alpha) * beta
 
         gradients *= factors
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from gunpowder.nodes.batch_filter import BatchFilter
 from gunpowder.array import Array, ArrayKeys
 from gunpowder.nodes.rasterize_graph import RasterizationSettings
 from gunpowder.morphology import enlarge_binary_map
 
 logger = logging.getLogger(__name__)
 
+
 class AddGtMaskExclusiveZone(BatchFilter):
-    ''' Create ExclusizeZone mask for a binary map in batch and add it as
+    """Create ExclusizeZone mask for a binary map in batch and add it as
     array to batch.
 
     An ExclusiveZone mask is a bianry mask [0,1] where locations which lie
     within a given distance to the ON (=1) regions (surrounding the ON regions)
     of the given binary map are set to 0, whereas all the others are set to 1.
 
     Args:
@@ -25,94 +26,102 @@
             binary mask (values of dict).
 
         gaussian_sigma_for_zone(float, optional): Defines extend of exclusive
             zone around ON region in binary map. Defaults to 1.
 
         rasterization_setting(:class:``RasterizationSettings``, optional): Which
             rasterization setting to use.
-    '''
+    """
 
     def __init__(
-            self,
-            EZ_masks_to_binary_map,
-            gaussian_sigma_for_zone=1,
-            rasterization_setting=None):
-
+        self,
+        EZ_masks_to_binary_map,
+        gaussian_sigma_for_zone=1,
+        rasterization_setting=None,
+    ):
         self.EZ_masks_to_binary_map = EZ_masks_to_binary_map
         self.gaussian_sigma_for_zone = gaussian_sigma_for_zone
         if rasterization_setting is None:
             self.rasterization_setting = RasterizationSettings()
         else:
             self.rasterization_setting = rasterization_setting
         self.skip_next = False
 
-
     def setup(self):
-
         self.upstream_spec = self.get_upstream_provider().get_spec()
         self.spec = copy.deepcopy(self.upstream_spec)
 
         for EZ_mask_type, binary_map_type in self.EZ_masks_to_binary_map.items():
             if binary_map_type in self.upstream_spec.arrays:
                 self.spec.arrays[EZ_mask_type] = self.spec.arrays[binary_map_type]
 
-
     def get_spec(self):
         return self.spec
 
-
     def prepare(self, request):
-
         self.EZ_masks_to_create = []
         for EZ_mask_type, binary_map_type in self.EZ_masks_to_binary_map.items():
             # do nothing if binary mask to create EZ mask around is not requested as well
             if EZ_mask_type in request.arrays:
                 # assert that binary mask for which EZ mask is created for is requested
-                assert binary_map_type in request.arrays, \
-                    "ExclusiveZone Mask for {}, can only be created if {} also requested.".format(EZ_mask_type, binary_map_type)
+                assert (
+                    binary_map_type in request.arrays
+                ), "ExclusiveZone Mask for {}, can only be created if {} also requested.".format(
+                    EZ_mask_type, binary_map_type
+                )
                 # assert that ROI of EZ lies within ROI of binary mask
-                assert request.arrays[binary_map_type].contains(request.arrays[EZ_mask_type]),\
-                    "EZ mask for {} requested for ROI outside of source's ({}) ROI.".format(EZ_mask_type,binary_map_type)
+                assert request.arrays[binary_map_type].contains(
+                    request.arrays[EZ_mask_type]
+                ), "EZ mask for {} requested for ROI outside of source's ({}) ROI.".format(
+                    EZ_mask_type, binary_map_type
+                )
 
                 self.EZ_masks_to_create.append(EZ_mask_type)
                 del request.arrays[EZ_mask_type]
 
         if len(self.EZ_masks_to_create) == 0:
             logger.warn("no ExclusiveZone Masks requested, will do nothing")
             self.skip_next = True
 
-
     def process(self, batch, request):
-
         # do nothing if no gt binary maps were requested
         if self.skip_next:
             self.skip_next = False
             return
 
         for EZ_mask_type in self.EZ_masks_to_create:
             binary_map_type = self.EZ_masks_to_binary_map[EZ_mask_type]
             binary_map = batch.arrays[binary_map_type].data
             resolution = batch.arrays[binary_map_type].resolution
-            EZ_mask = self.__get_exclusivezone_mask(binary_map, shape_EZ_mask=request.arrays[EZ_mask_type].get_shape(),
-                                                    resolution=resolution)
-
-            batch.arrays[EZ_mask_type] = Array(data= EZ_mask,
-                                                 roi=request.arrays[EZ_mask_type],
-                                                 resolution=resolution)
+            EZ_mask = self.__get_exclusivezone_mask(
+                binary_map,
+                shape_EZ_mask=request.arrays[EZ_mask_type].get_shape(),
+                resolution=resolution,
+            )
+
+            batch.arrays[EZ_mask_type] = Array(
+                data=EZ_mask, roi=request.arrays[EZ_mask_type], resolution=resolution
+            )
 
     def __get_exclusivezone_mask(self, binary_map, shape_EZ_mask, resolution=None):
-        ''' Exclusive zone surrounds every synapse. Created by enlarging the ON regions of given binary map
-        with different gaussian filter, make it binary and subtract the original binary map from it '''
+        """Exclusive zone surrounds every synapse. Created by enlarging the ON regions of given binary map
+        with different gaussian filter, make it binary and subtract the original binary map from it
+        """
 
         shape_diff = np.asarray(binary_map.shape - np.asarray(shape_EZ_mask))
-        slices = [slice(diff, shape - diff) for diff, shape in zip(shape_diff, binary_map.shape)]
+        slices = [
+            slice(diff, shape - diff)
+            for diff, shape in zip(shape_diff, binary_map.shape)
+        ]
         relevant_binary_map = binary_map[slices]
 
-
-        BM_enlarged_binary = enlarge_binary_map(relevant_binary_map,
-                                                marker_size_voxel=self.rasterization_setting.marker_size_voxel,
-                                                voxel_size=resolution,
-                                                marker_size_physical=self.rasterization_setting.marker_size_physical)
-
-
-        exclusive_zone = np.ones_like(BM_enlarged_binary) - (BM_enlarged_binary - relevant_binary_map)
+        BM_enlarged_binary = enlarge_binary_map(
+            relevant_binary_map,
+            marker_size_voxel=self.rasterization_setting.marker_size_voxel,
+            voxel_size=resolution,
+            marker_size_physical=self.rasterization_setting.marker_size_physical,
+        )
+
+        exclusive_zone = np.ones_like(BM_enlarged_binary) - (
+            BM_enlarged_binary - relevant_binary_map
+        )
         return exclusive_zone
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,142 +4,154 @@
 import pdb
 
 from gunpowder.array import Array
 from gunpowder.nodes.batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
-class AddNonsymmetricAffinities(BatchFilter):
-
 
+class AddNonsymmetricAffinities(BatchFilter):
     def __init__(
-            self,
-            affinity_vectors,
-            array_key_1,
-            array_key_2,
-            affinity_array_key_1,
-            affinity_array_key_2):
-
+        self,
+        affinity_vectors,
+        array_key_1,
+        array_key_2,
+        affinity_array_key_1,
+        affinity_array_key_2,
+    ):
         self.array_key_1 = array_key_1
         self.array_key_2 = array_key_2
         self.affinity_array_key_1 = affinity_array_key_1
         self.affinity_array_key_2 = affinity_array_key_2
         self.affinity_vectors = affinity_vectors
 
     def setup(self):
-        assert self.array_key_1 in self.spec, "Upstream does not provide %s needed by \
-        AddNonsymmetricAffinities"%self.array_key_1
-        assert self.array_key_2 in self.spec, "Upstream does not provide %s needed by \
-        AddNonsymmetricAffinities"%self.array_key_2
+        assert self.array_key_1 in self.spec, (
+            "Upstream does not provide %s needed by \
+        AddNonsymmetricAffinities"
+            % self.array_key_1
+        )
+        assert self.array_key_2 in self.spec, (
+            "Upstream does not provide %s needed by \
+        AddNonsymmetricAffinities"
+            % self.array_key_2
+        )
 
         voxel_size = self.spec[self.array_key_1].voxel_size
 
         self.upstream_spec = self.get_upstream_provider().spec
         self.upstream_roi = self.upstream_spec.get_total_roi()
 
-
         # get maximum offset in each dimension
         self.padding = np.max(np.abs(self.affinity_vectors), axis=0)
         self.padding = tuple(round_to_voxel_size(self.padding, voxel_size))
 
-        logger.debug("padding neg: %s" %np.asarray(self.padding))
+        logger.debug("padding neg: %s" % np.asarray(self.padding))
 
         spec = self.spec[self.array_key_1].copy()
         # if spec.roi is not None:
 
         self.provides(self.affinity_array_key_1, spec)
         self.provides(self.affinity_array_key_2, spec)
         self.enable_autoskip()
 
     def prepare(self, request):
-
         array_1_roi = request[self.array_key_1].roi
-        logger.debug("downstream %s request: "%self.array_key_1 + str(array_1_roi))
+        logger.debug("downstream %s request: " % self.array_key_1 + str(array_1_roi))
 
         array_2_roi = request[self.array_key_2].roi
-        logger.debug("downstream %s request: "%self.array_key_2 + str(array_2_roi))
+        logger.debug("downstream %s request: " % self.array_key_2 + str(array_2_roi))
 
         # grow labels ROI to accomodate padding TODO: vol 2
         array_1_roi = array_1_roi.grow(self.padding, self.padding)
         array_2_roi = array_2_roi.grow(self.padding, self.padding)
 
         request[self.array_key_1].roi = array_1_roi
         request[self.array_key_2].roi = array_2_roi
 
-        logger.debug("upstream %s request: "%self.array_key_1 + str(array_1_roi))
-        logger.debug("upstream %s request: "%self.array_key_2 + str(array_2_roi))
+        logger.debug("upstream %s request: " % self.array_key_1 + str(array_1_roi))
+        logger.debug("upstream %s request: " % self.array_key_2 + str(array_2_roi))
 
         # pdb.set_trace()
 
     def process(self, batch, request):
-
         full_vol1 = batch.arrays[self.array_key_1]
         full_vol2 = batch.arrays[self.array_key_2]
 
         # Both full_vol1 should match
-        assert full_vol1.spec.dtype == full_vol2.spec.dtype,\
-        "data type of array 1(%s) and array 2(%s) should match"%\
-        (full_vol1.spec.dtype, full_vol2.spec.dtype)
-
-        assert full_vol1.spec.voxel_size == full_vol2.spec.voxel_size,\
-        "data type of array 1(%s) and array 2(%s) should match"%\
-        (full_vol1.spec.voxel_size,full_vol2.spec.voxel_size)
+        assert (
+            full_vol1.spec.dtype == full_vol2.spec.dtype
+        ), "data type of array 1(%s) and array 2(%s) should match" % (
+            full_vol1.spec.dtype,
+            full_vol2.spec.dtype,
+        )
+
+        assert (
+            full_vol1.spec.voxel_size == full_vol2.spec.voxel_size
+        ), "data type of array 1(%s) and array 2(%s) should match" % (
+            full_vol1.spec.voxel_size,
+            full_vol2.spec.voxel_size,
+        )
 
         logger.debug("computing ground-truth affinities from labels")
 
         # Calculate affinities 1: from vol2 onto vol1
 
         # Initialize affinity map
         request_vol = request[self.affinity_array_key_1]
         affinity_map = np.zeros(
-            (len(self.affinity_vectors),) +
-            tuple(request_vol.roi.get_shape()/request_vol.voxel_size), dtype=full_vol1.spec.dtype)
+            (len(self.affinity_vectors),)
+            + tuple(request_vol.roi.shape / request_vol.voxel_size),
+            dtype=full_vol1.spec.dtype,
+        )
 
         # calculate affinities
         vol1 = full_vol1.crop(request_vol.roi)
         for i, vector in enumerate(self.affinity_vectors):
             vol2 = full_vol2.crop(request_vol.roi.shift(tuple(-vector)))
-            affinity_map[i,:,:,:] = np.bitwise_and(vol1.data, vol2.data)
+            affinity_map[i, :, :, :] = np.bitwise_and(vol1.data, vol2.data)
 
-
-        batch.arrays[self.affinity_array_key_1] = Array(affinity_map,
-            spec=request[self.affinity_array_key_1].copy())
-
-        batch.arrays[self.affinity_array_key_1].attrs['affinity_vectors'] =\
-         self.affinity_vectors
+        batch.arrays[self.affinity_array_key_1] = Array(
+            affinity_map, spec=request[self.affinity_array_key_1].copy()
+        )
+
+        batch.arrays[self.affinity_array_key_1].attrs[
+            "affinity_vectors"
+        ] = self.affinity_vectors
 
         # Calculate affinities 2: from vol1 onto vol2
 
         # Initialize affinity map
         request_vol = request[self.affinity_array_key_2]
         affinity_map = np.zeros(
-            (len(self.affinity_vectors),) +
-            tuple(request_vol.roi.get_shape()/request_vol.voxel_size), dtype=full_vol1.spec.dtype)
+            (len(self.affinity_vectors),)
+            + tuple(request_vol.roi.shape / request_vol.voxel_size),
+            dtype=full_vol1.spec.dtype,
+        )
 
         # calculate affinities
         vol2 = full_vol2.crop(request_vol.roi)
         for i, vector in enumerate(self.affinity_vectors):
             vol1 = full_vol1.crop(request_vol.roi.shift(tuple(vector)))
-            affinity_map[i,:,:,:] = np.bitwise_and(vol1.data, vol2.data)
-
-
-        batch.arrays[self.affinity_array_key_2] = Array(affinity_map,
-            spec=request[self.affinity_array_key_2].copy())
-
-        batch.arrays[self.affinity_array_key_2].attrs['affinity_vectors'] =\
-         self.affinity_vectors
-
+            affinity_map[i, :, :, :] = np.bitwise_and(vol1.data, vol2.data)
 
+        batch.arrays[self.affinity_array_key_2] = Array(
+            affinity_map, spec=request[self.affinity_array_key_2].copy()
+        )
+
+        batch.arrays[self.affinity_array_key_2].attrs[
+            "affinity_vectors"
+        ] = self.affinity_vectors
 
         # Crop all other requests
         for array_key, array in request.array_specs.items():
             batch.arrays[array_key] = batch.arrays[array_key].crop(array.roi)
 
         for points_key, points in request.points_specs.items():
             recropped = batch.points[points_key].spec.roi = points.roi
             batch.points[points_key] = recropped
 
 
 def round_to_voxel_size(shape, voxel_size):
     voxel_size = np.asarray(voxel_size, dtype=float)
-    shape = np.ceil(shape/voxel_size)*voxel_size
-    return np.array(shape, dtype='int32')
+    shape = np.ceil(shape / voxel_size) * voxel_size
+    return np.array(shape, dtype="int32")
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/add_vector_map.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/add_vector_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,50 +20,50 @@
         src_and_trg_points,
         voxel_sizes,
         radius_phys,
         partner_criterion,
         stayinside_array_keys=None,
         pad_for_partners=(0, 0, 0),
     ):
-        """ Creates a vector map of shape [dim_vector, [shape_of_array]] (e.g. [3, 50,50,50] for an array of
+        """Creates a vector map of shape [dim_vector, [shape_of_array]] (e.g. [3, 50,50,50] for an array of
             shape (50,50,50)) where every voxel which is close to a any source point location has a vector which points to
             one of the source point location's target location.
-            Close to a point location in src_point includes all voxels which 
+            Close to a point location in src_point includes all voxels which
                 1) lie within distance radius_phys of the considered src point location
                 2) (if stayinside_array_keys is not None), lie within the same segment as the src location in the
                     mask provided in stayinside_array_keys.
             The partner_criterion decides to which target location of the source point location that the vector of a
             voxel points (the different criterions are described below).
-        
+
         Args:
             src_and_trg_points (dict):      Dictionary from :class:``ArrayKey`` of the vector map to be created
                                             to a tuple (:class:``GraphKey`` of the source points, :class:``GraphKey``
                                             of the target points) which define the source and target points.
             voxel_sizes (dict):             Dictionary from
                                             :class:``ArrayKey`` of the vector
                                             map to be created to a
                                             :class:`Coordinate` for the voxel
                                             size of the array.
-            stayinside_array_keys (dict):  Dictionary from :class:``ArrayKey`` of the vector map to be created to 
-                                            :class:``ArrayKey`` of the stayinside_array. 
+            stayinside_array_keys (dict):  Dictionary from :class:``ArrayKey`` of the vector map to be created to
+                                            :class:``ArrayKey`` of the stayinside_array.
                                             The stayinside_array is assumed to contain discrete objects labeled with
                                             different object ids. The object id at the specific source location is used
-                                            to restrict the region where vectors are created around a source location. 
+                                            to restrict the region where vectors are created around a source location.
                                             Voxels that are located outside of this object are set to zero.
-                                            If stayinside_array_keys is None, all the voxels within distance 
+                                            If stayinside_array_keys is None, all the voxels within distance
                                             radius_phys to the source location receive a vector.
             pad_for_partners (tuple):       n-dim tuple which defines padding of trg_points request in all dimensions
                                             (in world units).
-                                            This might be used s.t. also partner locations which lie within the padded 
+                                            This might be used s.t. also partner locations which lie within the padded
                                             region, hence slightly outside of the vector map's roi, are considered.
             radius_phys (int):              Radius (in world units) to restrict region where vectors are created around
                                             a source location.
             partner_criterion(str):         'min_distance' or 'all'
                                             'min_distance': the vectors of all the voxels around a source location
-                                            point to the same target location, namely the location which has the 
+                                            point to the same target location, namely the location which has the
                                             minimal distance to the considered source location.
                                             'all': all partner locations of a given source location are considered.
                                             The region around a source location is split up into (num_partners)-subregions
                                             where each voxel points to the target location for which this subregion
                                             is the closest.
         """
 
@@ -71,15 +71,14 @@
         self.voxel_sizes = voxel_sizes
         self.array_keys_to_stayinside_array_keys = stayinside_array_keys
         self.pad_for_partners = pad_for_partners
         self.radius_phys = radius_phys
         self.partner_criterion = partner_criterion
 
     def setup(self):
-
         for (
             array_key,
             (src_points_key, trg_points_key),
         ) in self.array_to_src_trg_points.items():
             for points_key in [src_points_key, trg_points_key]:
                 assert (
                     points_key in self.spec
@@ -100,15 +99,14 @@
                     dtype=np.float32,
                 ),
             )
 
         self.enable_autoskip()
 
     def prepare(self, request):
-
         deps = BatchRequest()
 
         for (
             array_key,
             (src_points_key, trg_points_key),
         ) in self.array_to_src_trg_points.items():
             if array_key in request:
@@ -125,55 +123,49 @@
         ) in self.array_keys_to_stayinside_array_keys.items():
             if array_key in request:
                 deps[stayinside_array_key] = copy.deepcopy(request[array_key])
 
         return deps
 
     def process(self, batch, request):
-
         # create vector map and add it to batch
         for (
             array_key,
             (src_points_key, trg_points_key),
         ) in self.array_to_src_trg_points.items():
             if array_key in request:
                 vector_map = self.__get_vector_map(
                     batch=batch, request=request, vector_map_array_key=array_key
                 )
                 spec = self.spec[array_key].copy()
                 spec.roi = request[array_key].roi
                 batch.arrays[array_key] = Array(data=vector_map, spec=spec)
 
     def __get_vector_map(self, batch, request, vector_map_array_key):
-
         src_points_key, trg_points_key = self.array_to_src_trg_points[
             vector_map_array_key
         ]
-        dim_vectors = len(request[vector_map_array_key].roi.get_shape())
+        dim_vectors = len(request[vector_map_array_key].roi.shape)
         voxel_size_vm = self.voxel_sizes[vector_map_array_key]
-        offset_vector_map_phys = request[vector_map_array_key].roi.get_offset()
+        offset_vector_map_phys = request[vector_map_array_key].roi.offset
         vector_map_total = np.zeros(
-            (dim_vectors,)
-            + (request[vector_map_array_key].roi.get_shape() // voxel_size_vm),
+            (dim_vectors,) + (request[vector_map_array_key].roi.shape // voxel_size_vm),
             dtype=np.float32,
         )
 
         if batch.graphs[src_points_key].num_vertices() == 0:
             return vector_map_total
 
         for node in batch.graphs[src_points_key].nodes:
-
             if request[vector_map_array_key].roi.contains(Coordinate(node.location)):
-
                 # get all partner locations which should be considered
                 relevant_partner_loc = self.__get_relevant_partner_locations(
                     batch, node, trg_points_key
                 )
                 if len(relevant_partner_loc) > 0:
-
                     # get locations where to set vectors around source location
                     # (look only at region close to src location (to avoid np.nonzero() over entire array))
                     mask = self.__get_mask(
                         batch, request, vector_map_array_key, node.location
                     )
                     offset_vx_considered_mask = [
                         (
@@ -290,20 +282,20 @@
                 distance = np.linalg.norm(partner_loc - node.location)
                 if distance < min_distance:
                     min_distance = distance.copy()
                     stored_pos = partner_loc.copy()
             return [stored_pos]
 
     def __get_mask(self, batch, request, vector_map_array_key, src_location):
-        """ create binary mask encoding where to place vectors for in region around considered src_location """
+        """create binary mask encoding where to place vectors for in region around considered src_location"""
 
         voxel_size = self.voxel_sizes[vector_map_array_key]
 
-        offset_bm_phys = request[vector_map_array_key].roi.get_offset()
-        shape_bm_array_vx = request[vector_map_array_key].roi.get_shape() // voxel_size
+        offset_bm_phys = request[vector_map_array_key].roi.offset
+        shape_bm_array_vx = request[vector_map_array_key].roi.shape // voxel_size
         binary_map = np.zeros(shape_bm_array_vx, dtype="uint8")
 
         if self.array_keys_to_stayinside_array_keys is None:
             mask = np.ones_like(binary_map)
         else:
             stayinside_array_key = self.array_keys_to_stayinside_array_keys[
                 vector_map_array_key
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/dvid_partner_annotation_source.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/dvid_partner_annotation_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,194 +10,247 @@
 from gunpowder.graph_spec import GraphSpec
 from gunpowder.profiling import Timing
 
 from gunpowder.graph import Node
 
 logger = logging.getLogger(__name__)
 
+
 class DvidPartnerAnnoationSourceReadException(Exception):
     pass
 
+
 class MaskNotProvidedException(Exception):
     pass
 
 
 # TODO: This seems broken. There is code involving a voxel size, but points
 # don't have voxel sizes
 class DvidPartnerAnnotationSource(BatchProvider):
-    '''
-        :param hostname: hostname for DVID server
-        :type hostname: str
-
-        :param port: port for DVID server
-        :type port: int
-
-        :param uuid: UUID of node on DVID server
-        :type uuid: str
-
-        :param datasets: dict {GraphKey: DVID data instance}
-    '''
-
-    def __init__(
-            self,
-            hostname,
-            port,
-            uuid,
-            datasets=None,
-            rois=None):
+    """
+    :param hostname: hostname for DVID server
+    :type hostname: str
+
+    :param port: port for DVID server
+    :type port: int
+
+    :param uuid: UUID of node on DVID server
+    :type uuid: str
 
+    :param datasets: dict {GraphKey: DVID data instance}
+    """
+
+    def __init__(self, hostname, port, uuid, datasets=None, rois=None):
         self.hostname = hostname
         self.port = port
         self.url = "http://{}:{}".format(self.hostname, self.port)
         self.uuid = uuid
 
         self.datasets = datasets if datasets is not None else {}
         self.rois = rois if rois is not None else {}
 
         self.node_service = None
         self.dims = 0
 
     def setup(self):
-
         for points_key, points_name in self.datasets.items():
-            self.provides(
-                points_key,
-                GraphSpec(roi=self.points_rois[points_key]))
+            self.provides(points_key, GraphSpec(roi=self.points_rois[points_key]))
 
         logger.info("DvidPartnerAnnotationSource.spec:\n{}".format(self.spec))
 
     def provide(self, request):
-
         timing = Timing(self)
         timing.start()
 
         batch = Batch()
 
         # if pre and postsynaptic locations requested, their id : SynapseLocation dictionaries should be created
         # together s.t. the ids are unique and allow to find partner locations
         if GraphKey.PRESYN in request.points or GraphKey.POSTSYN in request.points:
             try:  # either both have the same roi, or only one of them is requested
-                assert request.points[GraphKey.PRESYN] == request.points[GraphKey.POSTSYN]
+                assert (
+                    request.points[GraphKey.PRESYN] == request.points[GraphKey.POSTSYN]
+                )
             except AssertionError:
-                assert GraphKey.PRESYN not in request.points or GraphKey.POSTSYN not in request.points
+                assert (
+                    GraphKey.PRESYN not in request.points
+                    or GraphKey.POSTSYN not in request.points
+                )
             if GraphKey.PRESYN in request.points:
-                presyn_points, postsyn_points = self.__read_syn_points(roi=request.points[GraphKey.PRESYN])
+                presyn_points, postsyn_points = self.__read_syn_points(
+                    roi=request.points[GraphKey.PRESYN]
+                )
             elif GraphKey.POSTSYN in request.points:
-                presyn_points, postsyn_points = self.__read_syn_points(roi=request.points[GraphKey.POSTSYN])
+                presyn_points, postsyn_points = self.__read_syn_points(
+                    roi=request.points[GraphKey.POSTSYN]
+                )
 
-        for (points_key, roi) in request.points.items():
+        for points_key, roi in request.points.items():
             # check if requested points can be provided
             if points_key not in self.spec:
-                raise RuntimeError("Asked for %s which this source does not provide"%points_key)
+                raise RuntimeError(
+                    "Asked for %s which this source does not provide" % points_key
+                )
             # check if request roi lies within provided roi
             if not self.spec[points_key].roi.contains(roi):
-                raise RuntimeError("%s's ROI %s outside of my ROI %s"%(points_key,roi,self.spec[points_key].roi))
+                raise RuntimeError(
+                    "%s's ROI %s outside of my ROI %s"
+                    % (points_key, roi, self.spec[points_key].roi)
+                )
+
+            logger.debug("Reading %s in %s..." % (points_key, roi))
+            id_to_point = {
+                GraphKey.PRESYN: presyn_points,
+                GraphKey.POSTSYN: postsyn_points,
+            }[points_key]
 
-            logger.debug("Reading %s in %s..."%(points_key, roi))
-            id_to_point = {GraphKey.PRESYN: presyn_points,
-                           GraphKey.POSTSYN: postsyn_points}[points_key]
-
-            batch.points[points_key] = Graph(
-                data=id_to_point,
-                spec=GraphSpec(roi=roi))
+            batch.points[points_key] = Graph(data=id_to_point, spec=GraphSpec(roi=roi))
 
         logger.debug("done")
 
         timing.stop()
         batch.profiling_stats.add(timing)
 
         return batch
 
-    def __load_json_annotations(self, array_shape_voxel, array_offset_voxel, array_name):
-        url = "http://" + str(self.hostname) + ":" + str(self.port)+"/api/node/" + str(self.uuid) + '/' + \
-              str(array_name) + "/elements/{}_{}_{}/{}_{}_{}".format(array_shape_voxel[2], array_shape_voxel[1], array_shape_voxel[0],
-                                                   array_offset_voxel[2], array_offset_voxel[1], array_offset_voxel[0])
+    def __load_json_annotations(
+        self, array_shape_voxel, array_offset_voxel, array_name
+    ):
+        url = (
+            "http://"
+            + str(self.hostname)
+            + ":"
+            + str(self.port)
+            + "/api/node/"
+            + str(self.uuid)
+            + "/"
+            + str(array_name)
+            + "/elements/{}_{}_{}/{}_{}_{}".format(
+                array_shape_voxel[2],
+                array_shape_voxel[1],
+                array_shape_voxel[0],
+                array_offset_voxel[2],
+                array_offset_voxel[1],
+                array_offset_voxel[0],
+            )
+        )
         annotations_file = requests.get(url)
         json_annotations = annotations_file.json()
         if json_annotations is None:
             json_annotations = []  # create empty_dummy_json_annotations
             # raise Exception ('No synapses found in region defined by array_offset {} and array_shape {}'.format(array_offset, array_shape))
         return json_annotations
 
     def __read_syn_points(self, roi):
-        """ read json file from dvid source, in json format to create for every location given """
+        """read json file from dvid source, in json format to create for every location given"""
 
         if GraphKey.PRESYN in self.points_voxel_size:
             voxel_size = self.points_voxel_size[GraphKey.PRESYN]
         elif GraphKey.POSTSYN in self.points_voxel_size:
             voxel_size = self.points_voxel_size[GraphKey.POSTSYN]
 
-        syn_file_json = self.__load_json_annotations(array_shape_voxel  = roi.get_shape() // voxel_size,
-                                                     array_offset_voxel = roi.get_offset() // voxel_size,
-                                                     array_name    = self.datasets[GraphKey.PRESYN])
+        syn_file_json = self.__load_json_annotations(
+            array_shape_voxel=roi.shape // voxel_size,
+            array_offset_voxel=roi.offset // voxel_size,
+            array_name=self.datasets[GraphKey.PRESYN],
+        )
 
         presyn_points_dict, postsyn_points_dict = {}, {}
         location_to_location_id_dict, location_id_to_partner_locations = {}, {}
         for node_nr, node in enumerate(syn_file_json):
             # collect information
-            kind        = str(node['Kind'])
-            location    = np.asarray((node['Pos'][2], node['Pos'][1], node['Pos'][0])) * voxel_size
+            kind = str(node["Kind"])
+            location = (
+                np.asarray((node["Pos"][2], node["Pos"][1], node["Pos"][0]))
+                * voxel_size
+            )
             location_id = int(node_nr)
             # some synapses are wrongly annotated in dvid source, have 'Tag': null ???, they are skipped
             try:
-                syn_id = int(node['Tags'][0][3:])
+                syn_id = int(node["Tags"][0][3:])
             except:
                 continue
             location_to_location_id_dict[str(location)] = location_id
 
             partner_locations = []
             try:
-                for relation in node['Rels']:
-                    partner_locations.append((np.asarray([relation['To'][2], relation['To'][1], relation['To'][0]]))*voxel_size)
+                for relation in node["Rels"]:
+                    partner_locations.append(
+                        (
+                            np.asarray(
+                                [
+                                    relation["To"][2],
+                                    relation["To"][1],
+                                    relation["To"][0],
+                                ]
+                            )
+                        )
+                        * voxel_size
+                    )
             except:
                 partner_locations = []
             location_id_to_partner_locations[int(node_nr)] = partner_locations
 
             # check if property given, not always given
             props = {}
-            if 'conf' in node['Prop']:
-                props['conf'] = float(node['Prop']['conf'])
-            if 'agent' in node['Prop']:
-                props['agent']  = str(node['Prop']['agent'])
-            if 'flagged' in node['Prop']:
-                str_value_flagged = str(node['Prop']['flagged'])
-                props['flagged']  = bool(distutils.util.strtobool(str_value_flagged))
-            if 'multi' in node['Prop']:
-                str_value_multi = str(node['Prop']['multi'])
-                props['multi']  = bool(distutils.util.strtobool(str_value_multi))
+            if "conf" in node["Prop"]:
+                props["conf"] = float(node["Prop"]["conf"])
+            if "agent" in node["Prop"]:
+                props["agent"] = str(node["Prop"]["agent"])
+            if "flagged" in node["Prop"]:
+                str_value_flagged = str(node["Prop"]["flagged"])
+                props["flagged"] = bool(distutils.util.strtobool(str_value_flagged))
+            if "multi" in node["Prop"]:
+                str_value_multi = str(node["Prop"]["multi"])
+                props["multi"] = bool(distutils.util.strtobool(str_value_multi))
 
             # create synPoint with information collected so far (partner_ids not completed yet)
-            if kind == 'PreSyn':
-                syn_point = Node(location=location, location_id=location_id,
-                                     synapse_id=syn_id, partner_ids=[], props=props)
+            if kind == "PreSyn":
+                syn_point = Node(
+                    location=location,
+                    location_id=location_id,
+                    synapse_id=syn_id,
+                    partner_ids=[],
+                    props=props,
+                )
                 presyn_points_dict[int(node_nr)] = deepcopy(syn_point)
-            elif kind == 'PostSyn':
-                syn_(location=location, location_id=location_id,
-                                     synapse_id=syn_id, partner_ids=[], props=props)
+            elif kind == "PostSyn":
+                syn_(
+                    location=location,
+                    location_id=location_id,
+                    synapse_id=syn_id,
+                    partner_ids=[],
+                    props=props,
+                )
                 postsyn_points_dict[int(node_nr)] = deepcopy(syn_point)
 
         # add partner ids
-        last_node_nr = len(syn_file_json)-1
+        last_node_nr = len(syn_file_json) - 1
         for current_syn_point_id in location_id_to_partner_locations.keys():
             all_partner_ids = []
             for partner_loc in location_id_to_partner_locations[current_syn_point_id]:
                 if location_to_location_id_dict.has_key(str(partner_loc)):
-                    all_partner_ids.append(int(location_to_location_id_dict[str(partner_loc)]))
+                    all_partner_ids.append(
+                        int(location_to_location_id_dict[str(partner_loc)])
+                    )
                 else:
                     last_node_nr = last_node_nr + 1
                     assert not location_to_location_id_dict.has_key(str(partner_loc))
                     all_partner_ids.append(int(last_node_nr))
 
             if current_syn_point_id in presyn_points_dict:
                 presyn_points_dict[current_syn_point_id].partner_ids = all_partner_ids
             elif current_syn_point_id in postsyn_points_dict:
                 postsyn_points_dict[current_syn_point_id].partner_ids = all_partner_ids
             else:
                 raise Exception("current syn_point id not found in any dictionary")
 
         return presyn_points_dict, postsyn_points_dict
 
-
     def __repr__(self):
         return "DvidPartnerAnnoationSource(hostname={}, port={}, uuid={}, raw_array_name={}, gt_array_name={}".format(
-            self.hostname, self.port, self.uuid, self.array_names[ArrayKeys.RAW],
-            self.array_names[ArrayKeys.GT_LABELS])
+            self.hostname,
+            self.port,
+            self.uuid,
+            self.array_names[ArrayKeys.RAW],
+            self.array_names[ArrayKeys.GT_LABELS],
+        )
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/hdf5_points_source.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/hdf5_points_source.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,142 +9,154 @@
 from gunpowder.graph_spec import GraphSpec
 from gunpowder.profiling import Timing
 from gunpowder.roi import Roi
 from gunpowder.nodes.batch_provider import BatchProvider
 
 logger = logging.getLogger(__name__)
 
+
 class Hdf5PointsSource(BatchProvider):
-    '''An HDF5 data source for :class:``Graph``. Currently only supports a
+    """An HDF5 data source for :class:``Graph``. Currently only supports a
     specific case where graphs represent pre- and post-synaptic markers.
 
     Args:
 
         filename (string): The HDF5 file.
 
         datasets (dict): Dictionary of :class:``GraphKey`` -> dataset names
             that this source offers.
 
         rois (dict): Dictionary of :class:``GraphKey`` -> :class:``Roi`` to
             set the ROI for each point set provided by this source.
 
-    '''
-
-    def __init__(
-            self,
-            filename,
-            datasets,
-            rois):
+    """
 
+    def __init__(self, filename, datasets, rois):
         self.filename = filename
         self.datasets = datasets
         self.rois = rois
 
         self.ndims = None
 
     def setup(self):
+        hdf_file = h5py.File(self.filename, "r")
 
-        hdf_file = h5py.File(self.filename, 'r')
-
-        for (points_key, ds_name) in self.datasets.items():
-
+        for points_key, ds_name in self.datasets.items():
             if ds_name not in hdf_file:
-                raise RuntimeError("%s not in %s"%(ds_name, self.filename))
+                raise RuntimeError("%s not in %s" % (ds_name, self.filename))
 
             spec = PointsSpec()
             spec.roi = self.rois[points_key]
 
             self.provides(points_key, spec)
 
         hdf_file.close()
 
     def provide(self, request):
-
         timing = Timing(self)
         timing.start()
 
         batch = Batch()
 
-        with h5py.File(self.filename, 'r') as hdf_file:
-
+        with h5py.File(self.filename, "r") as hdf_file:
             # if pre and postsynaptic locations required, their id
             # SynapseLocation dictionaries should be created together s.t. ids
             # are unique and allow to find partner locations
-            if PointsKeys.PRESYN in request.points_specs or PointsKeys.POSTSYN in request.points_specs:
-                assert request.points_specs[PointsKeys.PRESYN].roi == request.points_specs[PointsKeys.POSTSYN].roi
+            if (
+                PointsKeys.PRESYN in request.points_specs
+                or PointsKeys.POSTSYN in request.points_specs
+            ):
+                assert (
+                    request.points_specs[PointsKeys.PRESYN].roi
+                    == request.points_specs[PointsKeys.POSTSYN].roi
+                )
                 # Cremi specific, ROI offset corresponds to offset present in the
                 # synapse location relative to the raw data.
-                dataset_offset = self.spec[PointsKeys.PRESYN].roi.get_offset()
+                dataset_offset = self.spec[PointsKeys.PRESYN].roi.offset
                 presyn_points, postsyn_points = self.__get_syn_points(
                     roi=request.points_specs[PointsKeys.PRESYN].roi,
                     syn_file=hdf_file,
-                    dataset_offset=dataset_offset)
-
-            for (points_key, request_spec) in request.points_specs.items():
+                    dataset_offset=dataset_offset,
+                )
 
+            for points_key, request_spec in request.points_specs.items():
                 logger.debug("Reading %s in %s...", points_key, request_spec.roi)
                 id_to_point = {
                     PointsKeys.PRESYN: presyn_points,
-                    PointsKeys.POSTSYN: postsyn_points}[points_key]
+                    PointsKeys.POSTSYN: postsyn_points,
+                }[points_key]
 
                 points_spec = self.spec[points_key].copy()
                 points_spec.roi = request_spec.roi
                 batch.points[points_key] = Points(data=id_to_point, spec=points_spec)
 
         logger.debug("done")
 
         timing.stop()
         batch.profiling_stats.add(timing)
 
         return batch
 
     def __get_syn_points(self, roi, syn_file, dataset_offset=None):
         presyn_points_dict, postsyn_points_dict = {}, {}
-        presyn_node_ids  = syn_file['annotations/presynaptic_site/partners'][:, 0].tolist()
-        postsyn_node_ids = syn_file['annotations/presynaptic_site/partners'][:, 1].tolist()
+        presyn_node_ids = syn_file["annotations/presynaptic_site/partners"][
+            :, 0
+        ].tolist()
+        postsyn_node_ids = syn_file["annotations/presynaptic_site/partners"][
+            :, 1
+        ].tolist()
 
-        for node_nr, node_id in enumerate(syn_file['annotations/ids']):
-            location = syn_file['annotations/locations'][node_nr]
+        for node_nr, node_id in enumerate(syn_file["annotations/ids"]):
+            location = syn_file["annotations/locations"][node_nr]
             if dataset_offset is not None:
-                logging.debug('adding global offset to points %i %i %i' %(dataset_offset[0],
-                                                                          dataset_offset[1], dataset_offset[2]))
+                logging.debug(
+                    "adding global offset to points %i %i %i"
+                    % (dataset_offset[0], dataset_offset[1], dataset_offset[2])
+                )
                 location += dataset_offset
 
-
             # cremi synapse locations are in physical space
             if roi.contains(Coordinate(location)):
                 if node_id in presyn_node_ids:
-                    kind = 'PreSyn'
-                    assert syn_file['annotations/types'][node_nr] == 'presynaptic_site'
+                    kind = "PreSyn"
+                    assert syn_file["annotations/types"][node_nr] == "presynaptic_site"
                     syn_id = int(np.where(presyn_node_ids == node_id)[0])
                     partner_node_id = postsyn_node_ids[syn_id]
                 elif node_id in postsyn_node_ids:
-                    kind = 'PostSyn'
-                    assert syn_file['annotations/types'][node_nr] == 'postsynaptic_site'
+                    kind = "PostSyn"
+                    assert syn_file["annotations/types"][node_nr] == "postsynaptic_site"
                     syn_id = int(np.where(postsyn_node_ids == node_id)[0])
                     partner_node_id = presyn_node_ids[syn_id]
                 else:
-                    raise Exception('Node id neither pre- no post-synaptic')
+                    raise Exception("Node id neither pre- no post-synaptic")
 
                 partners_ids = [int(partner_node_id)]
-                location_id  = int(node_id)
+                location_id = int(node_id)
 
                 props = {}
-                if node_id in syn_file['annotations/comments/target_ids']:
-                    props = {'unsure': True}
+                if node_id in syn_file["annotations/comments/target_ids"]:
+                    props = {"unsure": True}
 
                 # create synpaseLocation & add to dict
-                if kind == 'PreSyn':
-                    syn_point = PreSynPoint(location=location, location_id=location_id,
-                                         synapse_id=syn_id, partner_ids=partners_ids, props=props)
+                if kind == "PreSyn":
+                    syn_point = PreSynPoint(
+                        location=location,
+                        location_id=location_id,
+                        synapse_id=syn_id,
+                        partner_ids=partners_ids,
+                        props=props,
+                    )
                     presyn_points_dict[int(node_id)] = copy.deepcopy(syn_point)
-                elif kind == 'PostSyn':
-                    syn_point = PostSynPoint(location=location, location_id=location_id,
-                                         synapse_id=syn_id, partner_ids=partners_ids, props=props)
+                elif kind == "PostSyn":
+                    syn_point = PostSynPoint(
+                        location=location,
+                        location_id=location_id,
+                        synapse_id=syn_id,
+                        partner_ids=partners_ids,
+                        props=props,
+                    )
                     postsyn_points_dict[int(node_id)] = copy.deepcopy(syn_point)
 
         return presyn_points_dict, postsyn_points_dict
 
-
     def __repr__(self):
-
         return self.filename
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/prepare_malis.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/prepare_malis.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,73 +4,64 @@
 
 from gunpowder.array import Array
 from gunpowder.batch_request import BatchRequest
 from gunpowder.nodes.batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
+
 class PrepareMalis(BatchFilter):
-    ''' Creates a component label array needed for two-phase malis training.
+    """Creates a component label array needed for two-phase malis training.
 
     Args:
 
         labels_array_key(:class:`ArrayKey`): The label array to use.
 
         malis_comp_array_key(:class:`ArrayKey`): The malis component array
             to generate.
 
         ignore_array_key(:class:`ArrayKey`, optional): An ignore mask to
             use.
-    '''
-
-    def __init__(
-            self,
-            labels_array_key,
-            malis_comp_array_key,
-            ignore_array_key=None):
+    """
 
+    def __init__(self, labels_array_key, malis_comp_array_key, ignore_array_key=None):
         self.labels_array_key = labels_array_key
         self.malis_comp_array_key = malis_comp_array_key
         self.ignore_array_key = ignore_array_key
 
     def setup(self):
-
         spec = self.spec[self.labels_array_key].copy()
         self.provides(self.malis_comp_array_key, spec)
         self.enable_autoskip()
 
     def prepare(self, request):
         deps = BatchRequest()
         deps[self.labels_array_key] = copy.deepcopy(request[self.labels_array_key])
         if self.ignore_array_key is not None:
             deps[self.ignore_array_key] = copy.deepcopy(request[self.labels_array_key])
         return deps
 
     def process(self, batch, request):
-
         gt_labels = batch.arrays[self.labels_array_key]
         next_id = gt_labels.data.max() + 1
 
         gt_pos_pass = gt_labels.data
 
         if self.ignore_array_key is not None:
-
             gt_neg_pass = np.array(gt_labels.data)
-            gt_neg_pass[
-                batch.arrays[self.ignore_array_key].data == 0] = next_id
+            gt_neg_pass[batch.arrays[self.ignore_array_key].data == 0] = next_id
 
         else:
-
             gt_neg_pass = gt_pos_pass
 
         spec = self.spec[self.malis_comp_array_key].copy()
         spec.roi = request[self.labels_array_key].roi
         batch.arrays[self.malis_comp_array_key] = Array(
-            np.array([gt_neg_pass, gt_pos_pass]),
-            spec)
+            np.array([gt_neg_pass, gt_pos_pass]), spec
+        )
 
         # Why don't we update gt_affinities in the same way?
         # -> not needed
         #
         # GT affinities are all 0 in the masked area (because masked area is
         # assumed to be set to background in batch.gt).
         #
```

### Comparing `gunpowder-1.2.2/gunpowder/contrib/nodes/zero_out_const_sections.py` & `gunpowder-1.3.0/gunpowder/contrib/nodes/zero_out_const_sections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from gunpowder.nodes.batch_filter import BatchFilter
 
+
 class ZeroOutConstSections(BatchFilter):
-    '''Every z-section that has constant values only will be set to 0.
+    """Every z-section that has constant values only will be set to 0.
 
     This is to handle blank (missing) sections in a less invasive way: Instead
     of leaving them at -1 (which is "black", the lowest possible input to the
     CNN), 0 ("gray") might be easier to ignore.
 
     For that you should call this filter after you are done with all other
     intensity manipulations.
-    '''
+    """
 
     def __init__(self, intensities):
         self.intensities = intensities
 
     def process(self, batch, request):
-
-        assert batch.get_total_roi().dims() == 3, "This filter only works on 3D data."
+        assert batch.get_total_roi().dims == 3, "This filter only works on 3D data."
 
         raw = batch.arrays[self.intensities]
 
-        for z in range((raw.spec.roi/self.spec[self.intensities].voxel_size).get_shape()[0]):
+        for z in range(
+            (raw.spec.roi / self.spec[self.intensities].voxel_size).get_shape()[0]
+        ):
             if raw.data[z].min() == raw.data[z].max():
                 raw.data[z] = 0
```

### Comparing `gunpowder-1.2.2/gunpowder/ext/__init__.py` & `gunpowder-1.3.0/gunpowder/ext/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,58 +13,79 @@
         self.__traceback_str = traceback.format_tb(sys.exc_info()[2])
         errtype, value = sys.exc_info()[:2]
         self.__exception = errtype(value)
 
     def __getattr__(self, item):
         raise self.__exception
 
+
 try:
     import dvision
 except ImportError as e:
-    dvision = NoSuchModule('dvision')
+    dvision = NoSuchModule("dvision")
 
 try:
     import h5py
 except ImportError as e:
-    h5py = NoSuchModule('h5py')
+    h5py = NoSuchModule("h5py")
 
 try:
     import pyklb
 except ImportError as e:
-    pyklb = NoSuchModule('pyklb')
+    pyklb = NoSuchModule("pyklb")
 
 try:
     import tensorflow
 except ImportError as e:
-    tensorflow = NoSuchModule('tensorflow')
+    tensorflow = NoSuchModule("tensorflow")
 
 try:
     import torch
 except ImportError as e:
-    torch = NoSuchModule('torch')
+    torch = NoSuchModule("torch")
 
 try:
     import tensorboardX
 except ImportError as e:
-    tensorboardX = NoSuchModule('tensorboardX')
+    tensorboardX = NoSuchModule("tensorboardX")
 
 try:
     import malis
 except ImportError as e:
-    malis = NoSuchModule('malis')
+    malis = NoSuchModule("malis")
 
 try:
     import augment
 except ImportError as e:
-    augment = NoSuchModule('augment')
+    augment = NoSuchModule("augment")
 
 try:
     import zarr
     from .zarr_file import ZarrFile
 except ImportError as e:
-    zarr = NoSuchModule('zarr')
+    zarr = NoSuchModule("zarr")
     ZarrFile = None
 
 try:
     import daisy
 except ImportError as e:
-    daisy = NoSuchModule('daisy')
+    daisy = NoSuchModule("daisy")
+
+try:
+    import jax
+except ImportError as e:
+    jax = NoSuchModule("jax")
+
+try:
+    import jax.numpy as jnp
+except ImportError as e:
+    jnp = NoSuchModule("jnp")
+
+try:
+    import haiku
+except ImportError as e:
+    haiku = NoSuchModule("haiku")
+
+try:
+    import optax
+except ImportError as e:
+    optax = NoSuchModule("optax")
```

### Comparing `gunpowder-1.2.2/gunpowder/graph.py` & `gunpowder-1.3.0/gunpowder/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,15 @@
         return self.attrs
 
     @classmethod
     def from_attrs(cls, attrs: Dict[str, Any]):
         node_id = attrs["id"]
         location = attrs["location"]
         temporary = attrs.get("temporary", False)
-        return cls(
-            id=node_id, location=location, temporary=temporary, attrs=attrs
-        )
+        return cls(id=node_id, location=location, temporary=temporary, attrs=attrs)
 
     def __str__(self):
         return f"Node({self.temporary}) ({self.id}) at ({self.location})"
 
     def __repr__(self):
         return str(self)
 
@@ -236,14 +234,16 @@
         graph.add_nodes_from(vs)
         graph.add_edges_from([(e.u, e.v, e.all) for e in edges])
         return graph
 
     @property
     def nodes(self):
         for node_id, node_attrs in self.__graph.nodes.items():
+            if "id" not in node_attrs:
+                node_attrs["id"] = node_id
             v = Node.from_attrs(node_attrs)
             if not np.issubdtype(v.location.dtype, self.spec.dtype):
                 raise Exception(
                     f"expected location to have dtype {self.spec.dtype} but it had {v.location.dtype}"
                 )
             yield v
 
@@ -490,27 +490,27 @@
 
         # `offset` can be 0 on some but not all axes leaving a 0 in the denominator.
         # `inside` can be on the bounding box, leaving a 0 in the numerator.
         # `x/0` throws a division warning, `0/0` throws an invalid warning (both are fine here)
         with np.errstate(divide="ignore", invalid="ignore"):
             bb_x = np.asarray(
                 [
-                    (np.asarray(bb.get_begin()) - inside) / offset,
-                    (np.asarray(bb.get_end()) - inside) / offset,
+                    (np.asarray(bb.begin) - inside) / offset,
+                    (np.asarray(bb.end) - inside) / offset,
                 ],
                 dtype=self.spec.dtype,
             )
 
         with np.errstate(invalid="ignore"):
             s = np.min(bb_x[np.logical_and((bb_x >= 0), (bb_x <= 1))])
 
         new_location = inside + s * distance * direction
-        upper = np.array(bb.get_end(), dtype=self.spec.dtype)
+        upper = np.array(bb.end, dtype=self.spec.dtype)
         new_location = np.clip(
-            new_location, bb.get_begin(), upper - upper * np.finfo(self.spec.dtype).eps
+            new_location, bb.begin, upper - upper * np.finfo(self.spec.dtype).eps
         )
         return new_location
 
     def merge(self, other, copy_from_self=False, copy=False):
         """
         Merge this graph with another. The resulting graph will have the Roi
         of the larger one.
@@ -570,15 +570,18 @@
         this Graph.
         """
         return deepcopy(self.__graph)
 
     @classmethod
     def from_nx_graph(cls, graph, spec):
         """
-        Create a gunpowder graph from a networkx graph
+        Create a gunpowder graph from a networkx graph.
+        The network graph is expected to have a "location"
+        attribute for each node. If it is a subclass of a networkx
+        graph with extra functionality, this may not work.
         """
         if spec.directed is None:
             spec.directed = graph.is_directed()
         g = cls([], [], spec)
         g.__graph = graph
         return g
```

### Comparing `gunpowder-1.2.2/gunpowder/graph_spec.py` & `gunpowder-1.3.0/gunpowder/graph_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,23 @@
         dtype (``dtype``, optional):
 
             The data type of the "location" attribute.
             Currently only supports np.float32.
     """
 
     def __init__(self, roi=None, directed=None, dtype=np.float32, placeholder=False):
-
         self.roi = roi
         self.directed = directed
         self.dtype = dtype
         self.placeholder = placeholder
 
         self.freeze()
 
     def update_with(self, spec):
-        if self.roi is not None and \
-           spec.roi is not None:
+        if self.roi is not None and spec.roi is not None:
             self.roi = self.roi.union(spec.roi)
         elif spec.roi is not None:
             self.roi = spec.roi
 
         if spec.directed is not None:
             self.directed = spec.directed
 
@@ -52,21 +50,19 @@
             self.placeholder = spec.placeholder
 
     def copy(self):
         """Create a copy of this spec."""
         return copy.deepcopy(self)
 
     def __eq__(self, other):
-
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return NotImplemented
 
     def __ne__(self, other):
-
         if isinstance(other, self.__class__):
             return not self.__eq__(other)
         return NotImplemented
 
     def __repr__(self):
         r = ""
         r += "ROI: " + str(self.roi) + ", "
```

### Comparing `gunpowder-1.2.2/gunpowder/morphology.py` & `gunpowder-1.3.0/gunpowder/morphology.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import numpy as np
 from scipy.ndimage.morphology import distance_transform_edt
 
 
 def enlarge_binary_map(
-    binary_map,
-    radius,
-    voxel_size,
-    ring_fraction=None,
-    in_place=False):
-    '''Enlarge existing regions in a binary map.
+    binary_map, radius, voxel_size, ring_fraction=None, in_place=False
+):
+    """Enlarge existing regions in a binary map.
 
     Args:
 
         binary_map (numpy array):
 
             A matrix with zeros, in which regions to be enlarged are indicated
             with a 1 (regions can already represent larger areas).
@@ -36,28 +33,28 @@
             If set to ``True``, argument ``binary_map`` will be modified
             directly.
 
     Returns:
 
         A matrix with 0s and 1s of same dimension as input binary_map with
         enlarged regions (indicated with 1), unless ``in_place`` is set.
-    '''
+    """
 
     if len(np.unique(binary_map)) == 1:
         # Check whether there are regions at all. If there is no region (or
         # everything is full), return the same map.
         return binary_map
 
     if voxel_size is None:
-        voxel_size = (1,)*binary_map.shape[0]
+        voxel_size = (1,) * binary_map.shape[0]
 
     voxel_size = np.asarray(voxel_size).astype(np.float32)
 
     # normalize, such that radius == 1 in all dimensions
-    voxel_size = voxel_size/radius
+    voxel_size = voxel_size / radius
 
     if in_place:
         np.logical_not(binary_map, out=binary_map)
     else:
         binary_map = np.logical_not(binary_map)
     edtmap = distance_transform_edt(binary_map, sampling=voxel_size)
 
@@ -74,15 +71,15 @@
     if in_place:
         return None
 
     return binary_map
 
 
 def create_ball_kernel(radius, voxel_size):
-    '''Generates a ball-shaped structuring element.
+    """Generates a ball-shaped structuring element.
 
     Args:
 
         radius (``ndarray`` of ``float``):
 
             The radius of the ball-shaped structuring element in world-units.
 
@@ -92,21 +89,21 @@
 
     Returns:
 
         The structuring element where elements of the neighborhood are 1 and 0
         otherwise. The shape of the returned array depends on radius and
         voxel_size. For instance voxel_size = [2, 1, 1], radius = 5 produces an
         array of shape (7, 11, 11)
-    '''
+    """
     voxel_size = np.asarray(voxel_size)
 
     # Calculate shape for new kernel, make it sufficiently large (--> ceil)
-    radius_voxel = np.ceil(radius/voxel_size).astype(np.int)
-    kernel_shape = np.array(radius_voxel)*2 + 1
+    radius_voxel = np.ceil(radius / voxel_size).astype(int)
+    kernel_shape = np.array(radius_voxel) * 2 + 1
 
     kernel = np.zeros(kernel_shape, dtype=np.uint8)
-    middle_point = kernel_shape//2
+    middle_point = kernel_shape // 2
     kernel[tuple(middle_point)] = 1
 
     enlarge_binary_map(kernel, radius, voxel_size, in_place=True)
 
     return kernel
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/__init__.py` & `gunpowder-1.3.0/gunpowder/nodes/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from __future__ import absolute_import
 
 from .add_affinities import AddAffinities
+from .astype import AsType
 from .balance_labels import BalanceLabels
 from .batch_filter import BatchFilter
 from .batch_provider import BatchProvider
 from .crop import Crop
 from .csv_points_source import CsvPointsSource
 from .daisy_request_blocks import DaisyRequestBlocks
 from .defect_augment import DefectAugment
 from .downsample import DownSample
 from .dvid_source import DvidSource
+from .deform_augment import DeformAugment
 from .elastic_augment import ElasticAugment
 from .exclude_labels import ExcludeLabels
+from .graph_source import GraphSource
 from .grow_boundary import GrowBoundary
 from .hdf5_source import Hdf5Source
 from .hdf5_write import Hdf5Write
 from .intensity_augment import IntensityAugment
 from .intensity_scale_shift import IntensityScaleShift
+from .iterate_locations import IterateLocations
 from .klb_source import KlbSource
 from .merge_provider import MergeProvider
 from .noise_augment import NoiseAugment
 from .normalize import Normalize
 from .pad import Pad
 from .precache import PreCache
 from .print_profiling_stats import PrintProfilingStats
 from .random_location import RandomLocation
 from .random_provider import RandomProvider
 from .rasterize_graph import RasterizationSettings, RasterizeGraph
 from .reject import Reject
 from .renumber_connected_components import RenumberConnectedComponents
+from .resample import Resample
 from .scan import Scan
 from .shift_augment import ShiftAugment
 from .simple_augment import SimpleAugment
 from .snapshot import Snapshot
 from .specified_location import SpecifiedLocation
 from .squeeze import Squeeze
 from .stack import Stack
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/balance_labels.py` & `gunpowder-1.3.0/gunpowder/nodes/balance_labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from .batch_filter import BatchFilter
 from gunpowder.array import Array
 from gunpowder.batch_request import BatchRequest
+from gunpowder.batch import Batch
 from collections.abc import Iterable
 import itertools
 import logging
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
 
 class BalanceLabels(BatchFilter):
-    '''Creates a scale array to balance the loss between class labels.
+    """Creates a scale array to balance the loss between class labels.
 
     Note that this only balances loss weights per-batch and does not accumulate
     statistics about class balance across batches.
 
     Args:
 
         labels (:class:`ArrayKey`):
@@ -56,114 +57,124 @@
 
         clipmax (``float``, optional):
 
             Clip class fraction to clipmax when calculating class weights.
             Defaults to 0.95. Set to None, if you do not want to clip max
             values.
 
-    '''
-
-    def __init__(self, labels, scales, mask=None, slab=None, num_classes=2,
-                 clipmin=0.05, clipmax=0.95):
+    """
 
+    def __init__(
+        self,
+        labels,
+        scales,
+        mask=None,
+        slab=None,
+        num_classes=2,
+        clipmin=0.05,
+        clipmax=0.95,
+    ):
         self.labels = labels
         self.scales = scales
         if mask is None:
             self.masks = []
         elif not isinstance(mask, Iterable):
             self.masks = [mask]
         else:
             self.masks = mask
 
         self.slab = slab
         self.num_classes = num_classes
         self.clipmin = clipmin
         self.clipmax = clipmax
 
-
     def setup(self):
-
         assert self.labels in self.spec, (
-            "Asked to balance labels %s, which are not provided."%self.labels)
+            "Asked to balance labels %s, which are not provided." % self.labels
+        )
 
         for mask in self.masks:
             assert mask in self.spec, (
                 "Asked to apply mask %s to balance labels, but mask is not "
-                "provided."%mask)
+                "provided." % mask
+            )
 
         spec = self.spec[self.labels].copy()
         spec.dtype = np.float32
         self.provides(self.scales, spec)
         self.enable_autoskip()
 
     def prepare(self, request):
-
         deps = BatchRequest()
         deps[self.labels] = request[self.scales]
         for mask in self.masks:
             deps[mask] = request[self.scales]
         return deps
 
     def process(self, batch, request):
-
         labels = batch.arrays[self.labels]
 
         assert len(np.unique(labels.data)) <= self.num_classes, (
-            "Found more unique labels than classes in %s."%self.labels)
+            "Found more unique labels than classes in %s." % self.labels
+        )
         assert 0 <= np.min(labels.data) < self.num_classes, (
-            "Labels %s are not in [0, num_classes)."%self.labels)
+            "Labels %s are not in [0, num_classes)." % self.labels
+        )
         assert 0 <= np.max(labels.data) < self.num_classes, (
-            "Labels %s are not in [0, num_classes)."%self.labels)
+            "Labels %s are not in [0, num_classes)." % self.labels
+        )
 
         # initialize error scale with 1s
         error_scale = np.ones(labels.data.shape, dtype=np.float32)
 
         # set error_scale to 0 in masked-out areas
         for key in self.masks:
             mask = batch.arrays[key]
-            assert labels.data.shape == mask.data.shape, (
-                "Shape of mask %s %s does not match %s %s"%(
-                    mask,
-                    mask.data.shape,
-                    self.labels,
-                    labels.data.shape))
+            assert (
+                labels.data.shape == mask.data.shape
+            ), "Shape of mask %s %s does not match %s %s" % (
+                mask,
+                mask.data.shape,
+                self.labels,
+                labels.data.shape,
+            )
             error_scale *= mask.data
 
         if not self.slab:
             slab = error_scale.shape
         else:
             # slab with -1 replaced by shape
             slab = tuple(
-                m if s == -1 else s
-                for m, s in zip(error_scale.shape, self.slab))
+                m if s == -1 else s for m, s in zip(error_scale.shape, self.slab)
+            )
 
-        slab_ranges = (
-            range(0, m, s)
-            for m, s in zip(error_scale.shape, slab))
+        slab_ranges = (range(0, m, s) for m, s in zip(error_scale.shape, slab))
 
         for start in itertools.product(*slab_ranges):
             slices = tuple(
-                slice(start[d], start[d] + slab[d])
-                for d in range(len(slab)))
-            self.__balance(
-                labels.data[slices],
-                error_scale[slices])
+                slice(start[d], start[d] + slab[d]) for d in range(len(slab))
+            )
+            self.__balance(labels.data[slices], error_scale[slices])
 
         spec = self.spec[self.scales].copy()
         spec.roi = labels.spec.roi
-        batch.arrays[self.scales] = Array(error_scale, spec)
 
-    def __balance(self, labels, scale):
+        outputs = Batch()
+        outputs[self.scales] = Array(error_scale, spec)
+        return outputs
 
+    def __balance(self, labels, scale):
         labels = labels.astype(np.int64)
 
         # in the masked-in area, compute the fraction of per-class samples
         masked_in = scale.sum()
         classes, counts = np.unique(labels[np.nonzero(scale)], return_counts=True)
-        fracs = counts.astype(float) / masked_in if masked_in > 0 else np.zeros(counts.size)
+        fracs = (
+            counts.astype(float) / masked_in if masked_in > 0 else np.zeros(counts.size)
+        )
         if self.clipmin is not None or self.clipmax is not None:
             np.clip(fracs, self.clipmin, self.clipmax, fracs)
 
         # compute the class weights
         w_sparse = 1.0 / float(self.num_classes) / fracs
         w = np.zeros(self.num_classes)
         w[classes] = w_sparse
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/batch_filter.py` & `gunpowder-1.3.0/gunpowder/nodes/batch_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 from gunpowder.batch_request import BatchRequest
 from gunpowder.profiling import Timing
 
 logger = logging.getLogger(__name__)
 
 
 class BatchFilterError(Exception):
-
     def __init__(self, batch_filter, msg):
         self.batch_filter = batch_filter
         self.msg = msg
 
     def __str__(self):
-
         return f"Error in {self.batch_filter.name()}: {self.msg}"
 
 
 class BatchFilter(BatchProvider):
     """Convenience wrapper for :class:`BatchProviders<BatchProvider>` with
     exactly one input provider.
 
@@ -28,40 +26,41 @@
     :func:`provides` and :func:`updates` in :func:`setup`.
 
     Subclasses need to implement at least :func:`process` to modify a passed
     batch (downstream). Optionally, the following methods can be implemented:
 
         :func:`setup`
 
-            Initialize this filter. Called after setup of the DAG. All upstream 
+            Initialize this filter. Called after setup of the DAG. All upstream
             providers will be set up already.
 
         :func:`teardown`
 
             Destruct this filter, free resources, stop worker processes.
 
         :func:`prepare`
 
-            Prepare for a batch request. Always called before each 
+            Prepare for a batch request. Always called before each
             :func:`process`. Used to communicate dependencies.
     """
 
     @property
     def remove_placeholders(self):
-        if not hasattr(self, '_remove_placeholders'):
+        if not hasattr(self, "_remove_placeholders"):
             return False
         return self._remove_placeholders
 
     def get_upstream_provider(self):
         if len(self.get_upstream_providers()) != 1:
             raise BatchFilterError(
                 self,
                 "BatchFilters need to have exactly one upstream provider, "
                 f"this one has {len(self.get_upstream_providers())}: "
-                f"({[b.name() for b in self.get_upstream_providers()]}")
+                f"({[b.name() for b in self.get_upstream_providers()]}",
+            )
         return self.get_upstream_providers()[0]
 
     def updates(self, key, spec):
         """Update an output provided by this :class:`BatchFilter`.
 
         Implementations should call this in their :func:`setup` method, which
         will be called when the pipeline is build.
@@ -78,15 +77,16 @@
         """
 
         if key not in self.spec:
             raise BatchFilterError(
                 self,
                 f"BatchFilter {self} is trying to change the spec for {key}, "
                 f"but {key} is not provided upstream. Upstream offers: "
-                f"{self.get_upstream_provider().spec}")
+                f"{self.get_upstream_provider().spec}",
+            )
         self.spec[key] = copy.deepcopy(spec)
         self.updated_items.append(key)
 
         logger.debug("%s updates %s with %s" % (self.name(), key, spec))
 
     def enable_autoskip(self, skip=True):
         """Enable automatic skipping of this :class:`BatchFilter`, based on
@@ -107,15 +107,14 @@
         if not hasattr(self, "_spec") or self._spec is None:
             if len(self.get_upstream_providers()) != 0:
                 self._spec = copy.deepcopy(self.get_upstream_provider().spec)
             else:
                 self._spec = None
 
     def internal_teardown(self):
-
         logger.debug("Resetting spec of %s", self.name())
         self._spec = None
         self._updated_items = []
 
         self.teardown()
 
     @property
@@ -129,22 +128,20 @@
         if not hasattr(self, "_updated_items"):
             self._updated_items = []
 
         return self._updated_items
 
     @property
     def autoskip_enabled(self):
-
         if not hasattr(self, "_autoskip_enabled"):
             self._autoskip_enabled = False
 
         return self._autoskip_enabled
 
     def provide(self, request):
-
         skip = self.__can_skip(request)
 
         timing_prepare = Timing(self, "prepare")
         timing_prepare.start()
 
         downstream_request = request.copy()
 
@@ -155,15 +152,16 @@
             elif dependencies is None:
                 upstream_request = request.copy()
             else:
                 raise BatchFilterError(
                     self,
                     f"This BatchFilter returned a {type(dependencies)}! "
                     "Supported return types are: `BatchRequest` containing your exact "
-                    "dependencies or `None`, indicating a dependency on the full request.")
+                    "dependencies or `None`, indicating a dependency on the full request.",
+                )
             self.remove_provided(upstream_request)
         else:
             upstream_request = request.copy()
         self.remove_provided(upstream_request)
 
         timing_prepare.stop()
 
@@ -245,10 +243,8 @@
                 The batch received from upstream to be modified by this node.
 
             request (:class:`BatchRequest`):
 
                 The request this node received. The updated batch should meet
                 this request.
         """
-        raise BatchFilterError(
-            self,
-            "does not implement 'process'")
+        raise BatchFilterError(self, "does not implement 'process'")
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/batch_provider.py` & `gunpowder-1.3.0/gunpowder/nodes/batch_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,172 +11,173 @@
 from gunpowder.graph import GraphKey
 from gunpowder.graph_spec import GraphSpec
 
 logger = logging.getLogger(__name__)
 
 
 class BatchRequestError(Exception):
-
     def __init__(self, provider, request, batch):
         self.provider = provider
         self.request = request
         self.batch = batch
 
     def __str__(self):
-
-        return \
-            f"Exception in {self.provider.name()} while processing request" \
-            f"{self.request} \n" \
-            "Batch returned so far:\n" \
+        return (
+            f"Exception in {self.provider.name()} while processing request"
+            f"{self.request} \n"
+            "Batch returned so far:\n"
             f"{self.batch}"
+        )
+
 
 class BatchProvider(object):
-    '''Superclass for all nodes in a `gunpowder` graph.
+    """Superclass for all nodes in a `gunpowder` graph.
 
     A :class:`BatchProvider` provides :class:`Batches<Batch>` containing
     :class:`Arrays<Array>` and/or :class:`Graph`. The available data is
     specified in a :class:`ProviderSpec` instance, accessible via :attr:`spec`.
 
     To create a new node, subclass this class and implement (at least)
     :func:`setup` and :func:`provide`.
 
     A :class:`BatchProvider` can be linked to any number of other
     :class:`BatchProviders<BatchProvider>` upstream. If your node accepts
     exactly one upstream provider, consider subclassing :class:`BatchFilter`
     instead.
-    '''
+    """
 
     def add_upstream_provider(self, provider):
         self.get_upstream_providers().append(provider)
         return provider
 
     def remove_upstream_providers(self):
         self.upstream_providers = []
 
     def get_upstream_providers(self):
-        if not hasattr(self, 'upstream_providers'):
+        if not hasattr(self, "upstream_providers"):
             self.upstream_providers = []
         return self.upstream_providers
 
     @property
     def remove_placeholders(self):
-        if not hasattr(self, '_remove_placeholders'):
+        if not hasattr(self, "_remove_placeholders"):
             return True
         return self._remove_placeholders
 
     def setup(self):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         Called during initialization of the DAG. Callees can assume that all
         upstream providers are set up already.
 
         In setup, call :func:`provides` to announce the arrays and points
         provided by this node.
-        '''
-        raise NotImplementedError("Class %s does not implement 'setup'"%self.name())
+        """
+        raise NotImplementedError("Class %s does not implement 'setup'" % self.name())
 
     def teardown(self):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         Called during destruction of the DAG. Subclasses should use this to
         stop worker processes, if they used some.
-        '''
+        """
         pass
 
     def provides(self, key, spec):
-        '''Introduce a new output provided by this :class:`BatchProvider`.
+        """Introduce a new output provided by this :class:`BatchProvider`.
 
         Implementations should call this in their :func:`setup` method, which
         will be called when the pipeline is build.
 
         Args:
 
             key (:class:`ArrayKey` or :class:`GraphKey`):
 
                 The array or point set key provided.
 
             spec (:class:`ArraySpec` or :class:`GraphSpec`):
 
                 The spec of the array or point set provided.
-        '''
+        """
 
         logger.debug("Current spec of %s:\n%s", self.name(), self.spec)
 
         if self.spec is None:
             self._spec = ProviderSpec()
 
-        assert key not in self.spec, (
-            "Node %s is trying to add spec for %s, but is already "
-            "provided."%(type(self).__name__, key))
+        assert (
+            key not in self.spec
+        ), "Node %s is trying to add spec for %s, but is already " "provided." % (
+            type(self).__name__,
+            key,
+        )
 
         self.spec[key] = copy.deepcopy(spec)
         self.provided_items.append(key)
 
         logger.debug("%s provides %s with spec %s", self.name(), key, spec)
 
     def _init_spec(self):
-        if not hasattr(self, '_spec'):
+        if not hasattr(self, "_spec"):
             self._spec = None
 
     def internal_teardown(self):
-
         logger.debug("Resetting spec of %s", self.name())
         self._spec = None
         self._provided_items = []
 
         self.teardown()
 
     @property
     def spec(self):
-        '''Get the :class:`ProviderSpec` of this :class:`BatchProvider`.
+        """Get the :class:`ProviderSpec` of this :class:`BatchProvider`.
 
         Note that the spec is only available after the pipeline has been build.
         Before that, it is ``None``.
-        '''
+        """
         self._init_spec()
         return self._spec
 
     @property
     def provided_items(self):
-        '''Get a list of the keys provided by this :class:`BatchProvider`.
+        """Get a list of the keys provided by this :class:`BatchProvider`.
 
         This list is only available after the pipeline has been build. Before
         that, it is empty.
-        '''
+        """
 
-        if not hasattr(self, '_provided_items'):
+        if not hasattr(self, "_provided_items"):
             self._provided_items = []
 
         return self._provided_items
 
     def remove_provided(self, request):
-        '''Remove keys from `request` that are provided by this
+        """Remove keys from `request` that are provided by this
         :class:`BatchProvider`.
-        '''
+        """
 
         for key in self.provided_items:
             if key in request:
                 del request[key]
 
     def request_batch(self, request):
-        '''Request a batch from this provider.
+        """Request a batch from this provider.
 
         Args:
 
             request (:class:`BatchRequest`):
 
                 A request containing (possibly partial)
                 :class:`ArraySpecs<ArraySpec>` and
                 :class:`GraphSpecs<GraphSpec>`.
-        '''
+        """
 
         batch = None
 
         try:
-
             request._update_random_seed()
 
             self.set_seeds(request)
 
             logger.debug("%s got request %s", self.name(), request)
 
             self.check_request_consistency(request)
@@ -191,167 +192,207 @@
             self.check_batch_consistency(batch, request)
 
             self.remove_unneeded(batch, request)
 
             logger.debug("%s provides %s", self.name(), batch)
 
         except Exception as e:
-
             raise BatchRequestError(self, request, batch) from e
 
         return batch
 
     def set_seeds(self, request):
         seed = request.random_seed
         random.seed(seed)
         # augment uses numpy for its randomness
         np.random.seed(seed)
 
     def check_request_consistency(self, request):
-
-        for (key, request_spec) in request.items():
-
-            assert key in self.spec, "%s: Asked for %s which this node does not provide"%(self.name(), key)
+        for key, request_spec in request.items():
             assert (
-                isinstance(request_spec, ArraySpec) or
-                isinstance(request_spec, GraphSpec) or
-                isinstance(request_spec, GraphSpec)), ("spec for %s is of type"
-                                                        "%s"%(
-                                                            key,
-                                                            type(request_spec)))
+                key in self.spec
+            ), "%s: Asked for %s which this node does not provide" % (self.name(), key)
+            assert (
+                isinstance(request_spec, ArraySpec)
+                or isinstance(request_spec, GraphSpec)
+                or isinstance(request_spec, GraphSpec)
+            ), "spec for %s is of type" "%s" % (key, type(request_spec))
 
             provided_spec = self.spec[key]
 
             provided_roi = provided_spec.roi
             request_roi = request_spec.roi
 
             if provided_roi is not None:
-                assert provided_roi.contains(request_roi), "%s: %s's ROI %s outside of my ROI %s"%(self.name(), key, request_roi, provided_roi)
+                assert provided_roi.contains(
+                    request_roi
+                ), "%s: %s's ROI %s outside of my ROI %s" % (
+                    self.name(),
+                    key,
+                    request_roi,
+                    provided_roi,
+                )
 
             if isinstance(key, ArrayKey):
-
                 if request_spec.voxel_size is not None:
-                    assert provided_spec.voxel_size == request_spec.voxel_size, "%s: voxel size %s requested for %s, but this node provides %s"%(
+                    assert provided_spec.voxel_size == request_spec.voxel_size, (
+                        "%s: voxel size %s requested for %s, but this node provides %s"
+                        % (
                             self.name(),
                             request_spec.voxel_size,
                             key,
-                            provided_spec.voxel_size)
+                            provided_spec.voxel_size,
+                        )
+                    )
 
-                if (
-                        request_roi is not None and
-                        provided_spec.voxel_size is not None):
-
-                    for d in range(request_roi.dims()):
-                        assert request_roi.get_shape()[d]%provided_spec.voxel_size[d] == 0, \
-                                "in request %s, dimension %d of request %s is not a multiple of voxel_size %d"%(
-                                        request,
-                                        d,
-                                        key,
-                                        provided_spec.voxel_size[d])
+                if request_roi is not None and provided_spec.voxel_size is not None:
+                    for d in range(request_roi.dims):
+                        assert (
+                            request_roi.shape[d] % provided_spec.voxel_size[d] == 0
+                        ), (
+                            "in request %s, dimension %d of request %s is not a multiple of voxel_size %d"
+                            % (request, d, key, provided_spec.voxel_size[d])
+                        )
 
             if isinstance(key, GraphKey):
-
                 if request_spec.directed is not None:
                     assert request_spec.directed == provided_spec.directed, (
                         f"asked for {key}:  directed={request_spec.directed} but "
                         f"{self.name()} provides directed={provided_spec.directed}"
                     )
-    def check_batch_consistency(self, batch, request):
-
-        for (array_key, request_spec) in request.array_specs.items():
 
-            assert array_key in batch.arrays, "%s requested, but %s did not provide it."%(array_key,self.name())
+    def check_batch_consistency(self, batch, request):
+        for array_key, request_spec in request.array_specs.items():
+            assert (
+                array_key in batch.arrays
+            ), "%s requested, but %s did not provide it." % (array_key, self.name())
             array = batch.arrays[array_key]
-            assert array.spec.roi == request_spec.roi, "%s ROI %s requested, but ROI %s provided by %s."%(
-                    array_key,
-                    request_spec.roi,
-                    array.spec.roi,
-                    self.name()
+            assert (
+                array.spec.roi == request_spec.roi
+            ), "%s ROI %s requested, but ROI %s provided by %s." % (
+                array_key,
+                request_spec.roi,
+                array.spec.roi,
+                self.name(),
             )
-            assert array.spec.voxel_size == self.spec[array_key].voxel_size, (
-                "voxel size of %s announced, but %s "
-                "delivered for %s"%(
-                    self.spec[array_key].voxel_size,
-                    array.spec.voxel_size,
-                    array_key))
-            # ensure that the spatial dimensions are the same (other dimensions 
+            assert (
+                array.spec.voxel_size == self.spec[array_key].voxel_size
+            ), "voxel size of %s announced, but %s " "delivered for %s" % (
+                self.spec[array_key].voxel_size,
+                array.spec.voxel_size,
+                array_key,
+            )
+            # ensure that the spatial dimensions are the same (other dimensions
             # on top are okay, e.g., for affinities)
             if request_spec.roi is not None:
-                dims = request_spec.roi.dims()
+                dims = request_spec.roi.dims
                 data_shape = Coordinate(array.data.shape[-dims:])
                 voxel_size = self.spec[array_key].voxel_size
-                assert data_shape == request_spec.roi.get_shape()/voxel_size, "%s ROI %s requested, but size of array is %s*%s=%s provided by %s."%(
+                assert data_shape == request_spec.roi.shape / voxel_size, (
+                    "%s ROI %s requested, but size of array is %s*%s=%s provided by %s."
+                    % (
                         array_key,
                         request_spec.roi,
                         data_shape,
                         voxel_size,
-                        data_shape*voxel_size,
-                        self.name()
+                        data_shape * voxel_size,
+                        self.name(),
+                    )
                 )
             if request_spec.dtype is not None:
-                assert batch[array_key].data.dtype == request_spec.dtype, \
-                    "dtype of array %s (%s) does not match requested dtype %s by %s" % (
-                        array_key,
-                        batch[array_key].data.dtype,
-                        request_spec.dtype,
-                        self.name())
-
-        for (graph_key, request_spec) in request.graph_specs.items():
+                assert (
+                    batch[array_key].data.dtype == request_spec.dtype
+                ), "dtype of array %s (%s) does not match requested dtype %s by %s" % (
+                    array_key,
+                    batch[array_key].data.dtype,
+                    request_spec.dtype,
+                    self.name(),
+                )
 
-            assert graph_key in batch.graphs, "%s requested, but %s did not provide it."%(graph_key,self.name())
+        for graph_key, request_spec in request.graph_specs.items():
+            assert (
+                graph_key in batch.graphs
+            ), "%s requested, but %s did not provide it." % (graph_key, self.name())
             graph = batch.graphs[graph_key]
-            assert graph.spec.roi == request_spec.roi, "%s ROI %s requested, but ROI %s provided by %s."%(
-                                            graph_key,
-                                            request_spec.roi,
-                                            graph.spec.roi,
-                                            self.name())
+            assert (
+                graph.spec.roi == request_spec.roi
+            ), "%s ROI %s requested, but ROI %s provided by %s." % (
+                graph_key,
+                request_spec.roi,
+                graph.spec.roi,
+                self.name(),
+            )
 
             if request_spec.directed is not None:
                 assert request_spec.directed == graph.directed, (
                     f"Recieved {graph_key}:  directed={graph.directed} but "
                     f"{self.name()} should provide directed={request_spec.directed}"
                 )
 
             for node in graph.nodes:
                 contained = graph.spec.roi.contains(node.location)
                 dangling = not contained and all(
-                    [
-                        graph.spec.roi.contains(v.location)
-                        for v in graph.neighbors(node)
-                    ]
+                    [graph.spec.roi.contains(v.location) for v in graph.neighbors(node)]
                 )
                 assert contained or dangling, (
                     f"graph {graph_key} provided by {self.name()} with ROI {graph.spec.roi} "
                     f"contain point at {node.location} which is neither contained nor "
                     f"'dangling'"
                 )
 
     def remove_unneeded(self, batch, request):
-
         batch_keys = set(list(batch.arrays.keys()) + list(batch.graphs.keys()))
         for key in batch_keys:
             if key not in request:
                 del batch[key]
 
     def enable_placeholders(self):
         self._remove_placeholders = False
 
     def provide(self, request):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         This function takes a :class:`BatchRequest` and should return the
         corresponding :class:`Batch`.
 
         Args:
 
             request(:class:`BatchRequest`):
 
                 The request to process.
-        '''
-        raise NotImplementedError("Class %s does not implement 'provide'"%self.name())
+        """
+        raise NotImplementedError("Class %s does not implement 'provide'" % self.name())
 
     def name(self):
         return type(self).__name__
 
     def __repr__(self):
-
         return self.name() + ", providing: " + str(self.spec)
+
+    def __add__(self, other):
+        """Support ``self + other`` operator. Return a :class:`Pipeline`."""
+        from gunpowder import Pipeline
+
+        if isinstance(other, BatchProvider):
+            other = Pipeline(other)
+
+        if not isinstance(other, Pipeline):
+            raise RuntimeError(
+                f"Don't know how to add {type(other)} to BatchProvider "
+                f"{self.name()}"
+            )
+
+        return Pipeline(self) + other
+
+    def __radd__(self, other):
+        """Support ``other + self`` operator. Return a :class:`Pipeline`."""
+        from gunpowder import Pipeline
+
+        if isinstance(other, BatchProvider):
+            return Pipeline(other) + Pipeline(self)
+
+        if isinstance(other, tuple):
+            return other + Pipeline(self)
+
+        raise RuntimeError(
+            f"Don't know how to radd {type(other)} to BatchProvider" f"{self.name()}"
+        )
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/crop.py` & `gunpowder-1.3.0/gunpowder/nodes/crop.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import logging
 
 from .batch_filter import BatchFilter
 from gunpowder.coordinate import Coordinate
 
 logger = logging.getLogger(__name__)
 
+
 class Crop(BatchFilter):
-    '''Limits provided ROIs by either giving a new :class:`Roi` or crop
+    """Limits provided ROIs by either giving a new :class:`Roi` or crop
     fractions from either face of the provided ROI.
 
     Args:
 
         key (:class:`ArrayKey` or :class:`GraphKey`):
 
             The key of the array or points set to modify.
@@ -23,67 +24,60 @@
         fraction_negative (``tuple`` of ``float``):
 
             Relative crop starting from the negative end of the provided ROI.
 
         fraction_positive (``tuple`` of ``float``):
 
             Relative crop starting from the positive end of the provided ROI.
-    '''
-
-    def __init__(
-            self,
-            key,
-            roi=None,
-            fraction_negative=None,
-            fraction_positive=None):
+    """
 
+    def __init__(self, key, roi=None, fraction_negative=None, fraction_positive=None):
         if roi is not None and (
-                fraction_positive is not None or
-                fraction_negative is not None):
+            fraction_positive is not None or fraction_negative is not None
+        ):
             raise RuntimeError(
-                "'roi' and 'fraction_...' arguments can not be given together")
+                "'roi' and 'fraction_...' arguments can not be given together"
+            )
 
         if (roi, fraction_positive, fraction_negative) == (None, None, None):
-            raise RuntimeError(
-                "One of 'roi' and 'fraction_...' has to be given")
+            raise RuntimeError("One of 'roi' and 'fraction_...' has to be given")
 
         if fraction_negative is not None and fraction_positive is None:
-            fraction_positive = (0.0,)*len(fraction_negative)
+            fraction_positive = (0.0,) * len(fraction_negative)
         if fraction_positive is not None and fraction_negative is None:
-            fraction_negative = (0.0,)*len(fraction_positive)
+            fraction_negative = (0.0,) * len(fraction_positive)
 
         self.key = key
         self.roi = roi
         self.fraction_negative = fraction_negative
         self.fraction_positive = fraction_positive
 
     def setup(self):
-
         spec = self.spec[self.key]
 
         if self.roi is not None:
-
-            assert spec.roi.contains(self.roi), (
-                "Crop ROI is not contained in upstream ROI.")
+            assert spec.roi.contains(
+                self.roi
+            ), "Crop ROI is not contained in upstream ROI."
 
             cropped_roi = self.roi
 
         else:
-
             total_fraction = tuple(
-                n + p
-                for n, p in zip(self.fraction_negative, self.fraction_positive)
+                n + p for n, p in zip(self.fraction_negative, self.fraction_positive)
             )
             if max(total_fraction) >= 1:
                 raise RuntimeError("Sum of crop fractions exeeds 1")
 
-            crop_positive = spec.roi.get_shape()*self.fraction_positive
-            crop_negative = spec.roi.get_shape()*self.fraction_negative
-            cropped_roi = spec.roi.grow(
-                -crop_positive,
-                -crop_negative)
+            crop_positive = Coordinate(
+                a * b for a, b in zip(spec.roi.shape, self.fraction_positive)
+            )
+            crop_negative = Coordinate(
+                a * b for a, b in zip(spec.roi.shape, self.fraction_negative)
+            )
+            cropped_roi = spec.roi.grow(-crop_positive, -crop_negative)
 
         spec.roi = cropped_roi
         self.updates(self.key, spec)
 
     def process(self, batch, request):
         pass
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/csv_points_source.py` & `gunpowder-1.3.0/gunpowder/nodes/csv_points_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from gunpowder.graph import Node, Graph
 from gunpowder.graph_spec import GraphSpec
 from gunpowder.profiling import Timing
 from gunpowder.roi import Roi
 
 logger = logging.getLogger(__name__)
 
+
 class CsvPointsSource(BatchProvider):
-    '''Read a set of points from a comma-separated-values text file. Each line
+    """Read a set of points from a comma-separated-values text file. Each line
     in the file represents one point, e.g. z y x (id)
 
     Args:
 
         filename (``string``):
 
             The file to read from.
@@ -42,96 +43,87 @@
             location of the point. If positive, only the first ``ndims`` are used.
             If negative, all but the last ``-ndims`` are used.
 
          id_dim (``int``):
 
             Each line may optionally contain an id for each point. This parameter
             specifies its location, has to come after the position values.
-    '''
-
-    def __init__(self, filename, points, points_spec=None, scale=None,
-                 ndims=None, id_dim=None):
+    """
 
+    def __init__(
+        self, filename, points, points_spec=None, scale=None, ndims=None, id_dim=None
+    ):
         self.filename = filename
         self.points = points
         self.points_spec = points_spec
         self.scale = scale
         self.ndims = ndims
         self.id_dim = id_dim
         self.data = None
 
     def setup(self):
-
         self._parse_csv()
 
         if self.points_spec is not None:
-
             self.provides(self.points, self.points_spec)
             return
 
-        min_bb = Coordinate(np.floor(np.amin(self.data[:,:self.ndims], 0)))
-        max_bb = Coordinate(np.ceil(np.amax(self.data[:,:self.ndims], 0)) + 1)
+        min_bb = Coordinate(np.floor(np.amin(self.data[:, : self.ndims], 0)))
+        max_bb = Coordinate(np.ceil(np.amax(self.data[:, : self.ndims], 0)) + 1)
 
         roi = Roi(min_bb, max_bb - min_bb)
 
         self.provides(self.points, GraphSpec(roi=roi))
 
     def provide(self, request):
-
         timing = Timing(self)
         timing.start()
 
-        min_bb = request[self.points].roi.get_begin()
-        max_bb = request[self.points].roi.get_end()
+        min_bb = request[self.points].roi.begin
+        max_bb = request[self.points].roi.end
 
-        logger.debug(
-            "CSV points source got request for %s",
-            request[self.points].roi)
+        logger.debug("CSV points source got request for %s", request[self.points].roi)
 
-        point_filter = np.ones((self.data.shape[0],), dtype=np.bool)
+        point_filter = np.ones((self.data.shape[0],), dtype=bool)
         for d in range(self.ndims):
-            point_filter = np.logical_and(point_filter, self.data[:,d] >= min_bb[d])
-            point_filter = np.logical_and(point_filter, self.data[:,d] < max_bb[d])
+            point_filter = np.logical_and(point_filter, self.data[:, d] >= min_bb[d])
+            point_filter = np.logical_and(point_filter, self.data[:, d] < max_bb[d])
 
         points_data = self._get_points(point_filter)
         points_spec = GraphSpec(roi=request[self.points].roi.copy())
 
         batch = Batch()
         batch.graphs[self.points] = Graph(points_data, [], points_spec)
 
         timing.stop()
         batch.profiling_stats.add(timing)
 
         return batch
 
     def _get_points(self, point_filter):
-
-        filtered = self.data[point_filter][:,:self.ndims]
+        filtered = self.data[point_filter][:, : self.ndims]
 
         if self.id_dim is not None:
-            ids = self.data[point_filter][:,self.id_dim]
+            ids = self.data[point_filter][:, self.id_dim]
         else:
             ids = np.arange(len(self.data))[point_filter]
 
-        return [
-            Node(id=i, location=p)
-            for i, p in zip(ids, filtered)
-        ]
+        return [Node(id=i, location=p) for i, p in zip(ids, filtered)]
 
     def _parse_csv(self):
-        '''Read one point per line. If ``ndims`` is None, all values in one line
+        """Read one point per line. If ``ndims`` is None, all values in one line
         are considered as the location of the point. If positive, only the
         first ``ndims`` are used. If negative, all but the last ``-ndims`` are
         used.
-        '''
+        """
 
         with open(self.filename, "r") as f:
             self.data = np.array(
                 [[float(t.strip(",")) for t in line.split()] for line in f],
                 dtype=np.float32,
             )
 
         if self.ndims is None:
             self.ndims = self.data.shape[1]
 
         if self.scale is not None:
-            self.data[:,:self.ndims] *= self.scale
+            self.data[:, : self.ndims] *= self.scale
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/daisy_request_blocks.py` & `gunpowder-1.3.0/gunpowder/nodes/daisy_request_blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import multiprocessing
 import time
 
 logger = logging.getLogger(__name__)
 
 
 class DaisyRequestBlocks(BatchFilter):
-    '''Iteratively requests batches similar to ``reference`` from upstream
+    """Iteratively requests batches similar to ``reference`` from upstream
     providers, with their ROIs set to blocks distributed by ``daisy``.
 
     The ROIs of the array or point specs in the reference can be set to either
     the block's ``read_roi`` or ``write_roi``, see parameter ``roi_map``.
 
     The batch request to this node has to be empty, as there is no guarantee
     that this node will get to process all chunks required to fulfill a
@@ -46,94 +46,80 @@
             time.time()`` and ``duration = time.time() - start``, right before
             and after a block gets processed.
 
             This callback can be used to log blocks that have successfully
             finished processing, which can be used in ``check_function`` of
             ``daisy.run_blockwise`` to skip already processed blocks in
             repeated runs.
-    '''
-
-    def __init__(
-            self,
-            reference,
-            roi_map,
-            num_workers=1,
-            block_done_callback=None):
+    """
 
+    def __init__(self, reference, roi_map, num_workers=1, block_done_callback=None):
         self.reference = reference
         self.roi_map = roi_map
         self.num_workers = num_workers
         self.block_done_callback = block_done_callback
 
         if num_workers > 1:
             self.request_queue = multiprocessing.Queue(maxsize=0)
 
     def provide(self, request):
-
-        empty_request = (len(request) == 0)
+        empty_request = len(request) == 0
         if not empty_request:
-            raise RuntimeError(
-                "requests made to DaisyRequestBlocks have to be empty")
+            raise RuntimeError("requests made to DaisyRequestBlocks have to be empty")
 
         if self.num_workers > 1:
-
             self.workers = [
                 multiprocessing.Process(target=self.__get_chunks)
                 for _ in range(self.num_workers)
             ]
 
             for worker in self.workers:
                 worker.start()
 
             for worker in self.workers:
                 worker.join()
 
         else:
-
             self.__get_chunks()
 
         return Batch()
 
     def __get_chunks(self):
-
         daisy_client = daisy.Client()
 
         while True:
-
-            block = daisy_client.acquire_block()
-
-            if block is None:
-                return
-
-            logger.info("Processing block %s", block)
-            start = time.time()
-
-            chunk_request = self.reference.copy()
-
-            for key, reference_spec in self.reference.items():
-
-                roi_type = self.roi_map.get(key, None)
-
-                if roi_type is None:
-                    raise RuntimeError(
-                        "roi_map does not map item %s to either 'read_roi' "
-                        "or 'write_roi'" % key)
-
-                if roi_type == 'read_roi':
-                    chunk_request[key].roi = Roi(
-                        block.read_roi.get_offset(),
-                        block.read_roi.get_shape())
-                elif roi_type == 'write_roi':
-                    chunk_request[key].roi = Roi(
-                        block.write_roi.get_offset(),
-                        block.write_roi.get_shape())
-                else:
-                    raise RuntimeError(
-                        "%s is not a vaid ROI type (read_roi or write_roi)")
-
-            self.get_upstream_provider().request_batch(chunk_request)
-
-            end = time.time()
-            if self.block_done_callback:
-                self.block_done_callback(block, start, end - start)
-
-            daisy_client.release_block(block, ret=0)
+            with daisy_client.acquire_block() as block:
+                if block is None:
+                    return
+
+                logger.info("Processing block %s", block)
+                start = time.time()
+
+                chunk_request = self.reference.copy()
+
+                for key, reference_spec in self.reference.items():
+                    roi_type = self.roi_map.get(key, None)
+
+                    if roi_type is None:
+                        raise RuntimeError(
+                            "roi_map does not map item %s to either 'read_roi' "
+                            "or 'write_roi'" % key
+                        )
+
+                    if roi_type == "read_roi":
+                        chunk_request[key].roi = Roi(
+                            block.read_roi.offset, block.read_roi.shape
+                        )
+                    elif roi_type == "write_roi":
+                        chunk_request[key].roi = Roi(
+                            block.write_roi.offset, block.write_roi.shape
+                        )
+                    else:
+                        raise RuntimeError(
+                            "%s is not a vaid ROI type (read_roi or write_roi)"
+                        )
+
+                self.get_upstream_provider().request_batch(chunk_request)
+
+                end = time.time()
+                if self.block_done_callback:
+                    self.block_done_callback(block, start, end - start)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/defect_augment.py` & `gunpowder-1.3.0/gunpowder/nodes/defect_augment.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 from gunpowder.batch_request import BatchRequest
 from gunpowder.coordinate import Coordinate
 from .batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
+
 class DefectAugment(BatchFilter):
-    '''Augment intensity arrays section-wise with artifacts like missing
+    """Augment intensity arrays section-wise with artifacts like missing
     sections, low-contrast sections, by blending in artifacts drawn from a
     separate source, or by deforming a section.
 
     Args:
 
         intensities (:class:`ArrayKey`):
 
@@ -62,48 +63,47 @@
             ``prob_deform`` > 0. The deformation models a fold by shifting the
             section contents towards a randomly oriented line in the section.
             The line itself will be drawn with a value of 0.
 
         axis (``int``, optional):
 
             Along which axis sections are cut.
-    '''
+    """
 
     def __init__(
-            self,
-            intensities,
-            prob_missing=0.05,
-            prob_low_contrast=0.05,
-            prob_artifact=0.0,
-            prob_deform=0.0,
-            contrast_scale=0.1,
-            artifact_source=None,
-            artifacts=None,
-            artifacts_mask=None,
-            deformation_strength=20,
-            axis=0):
+        self,
+        intensities,
+        prob_missing=0.05,
+        prob_low_contrast=0.05,
+        prob_artifact=0.0,
+        prob_deform=0.0,
+        contrast_scale=0.1,
+        artifact_source=None,
+        artifacts=None,
+        artifacts_mask=None,
+        deformation_strength=20,
+        axis=0,
+    ):
         self.intensities = intensities
         self.prob_missing = prob_missing
         self.prob_low_contrast = prob_low_contrast
         self.prob_artifact = prob_artifact
         self.prob_deform = prob_deform
         self.contrast_scale = contrast_scale
         self.artifact_source = artifact_source
         self.artifacts = artifacts
         self.artifacts_mask = artifacts_mask
         self.deformation_strength = deformation_strength
         self.axis = axis
 
     def setup(self):
-
         if self.artifact_source is not None:
             self.artifact_source.setup()
 
     def teardown(self):
-
         if self.artifact_source is not None:
             self.artifact_source.teardown()
 
     # send roi request to data-source upstream
     def prepare(self, request):
         random.seed(request.random_seed)
         deps = BatchRequest()
@@ -124,190 +124,206 @@
         logger.debug("downstream request ROI is %s" % roi)
         raw_voxel_size = self.spec[self.intensities].voxel_size
 
         # store the mapping slice to augmentation type in a dict
         self.slice_to_augmentation = {}
         # store the transformations for deform slice
         self.deform_slice_transformations = {}
-        for c in range((roi / raw_voxel_size).get_shape()[self.axis]):
+        for c in range((roi / raw_voxel_size).shape[self.axis]):
             r = random.random()
 
             if r < prob_missing_threshold:
                 logger.debug("Zero-out " + str(c))
-                self.slice_to_augmentation[c] = 'zero_out'
+                self.slice_to_augmentation[c] = "zero_out"
 
             elif r < prob_low_contrast_threshold:
                 logger.debug("Lower contrast " + str(c))
-                self.slice_to_augmentation[c] = 'lower_contrast'
+                self.slice_to_augmentation[c] = "lower_contrast"
 
             elif r < prob_artifact_threshold:
                 logger.debug("Add artifact " + str(c))
-                self.slice_to_augmentation[c] = 'artifact'
+                self.slice_to_augmentation[c] = "artifact"
 
             elif r < prob_deform_slice:
                 logger.debug("Add deformed slice " + str(c))
-                self.slice_to_augmentation[c] = 'deformed_slice'
+                self.slice_to_augmentation[c] = "deformed_slice"
                 # get the shape of a single slice
-                slice_shape = (roi / raw_voxel_size).get_shape()
-                slice_shape = slice_shape[:self.axis] + slice_shape[self.axis+1:]
-                self.deform_slice_transformations[c] = self.__prepare_deform_slice(slice_shape)
+                slice_shape = (roi / raw_voxel_size).shape
+                slice_shape = slice_shape[: self.axis] + slice_shape[self.axis + 1 :]
+                self.deform_slice_transformations[c] = self.__prepare_deform_slice(
+                    slice_shape
+                )
 
         # prepare transformation and
         # request bigger upstream roi for deformed slice
-        if 'deformed_slice' in self.slice_to_augmentation.values():
-
+        if "deformed_slice" in self.slice_to_augmentation.values():
             # create roi sufficiently large to feed deformation
             logger.debug("before growth: %s" % spec.roi)
             growth = Coordinate(
-                tuple(0 if d == self.axis else raw_voxel_size[d] * self.deformation_strength
-                      for d in range(spec.roi.dims()))
+                tuple(
+                    0
+                    if d == self.axis
+                    else raw_voxel_size[d] * self.deformation_strength
+                    for d in range(spec.roi.dims)
+                )
             )
             logger.debug("growing request by %s" % str(growth))
             source_roi = roi.grow(growth, growth)
 
             # update request ROI to get all voxels necessary to perfrom
             # transformation
             spec.roi = source_roi
             logger.debug("upstream request roi is %s" % spec.roi)
 
         deps[self.intensities] = spec
 
     def process(self, batch, request):
-
-        assert batch.get_total_roi().dims() == 3, "defectaugment works on 3d batches only"
+        assert batch.get_total_roi().dims == 3, "defectaugment works on 3d batches only"
 
         raw = batch.arrays[self.intensities]
         raw_voxel_size = self.spec[self.intensities].voxel_size
 
         for c, augmentation_type in self.slice_to_augmentation.items():
-
             section_selector = tuple(
-                slice(None if d != self.axis else c, None if d != self.axis else c+1)
-                for d in range(raw.spec.roi.dims())
+                slice(None if d != self.axis else c, None if d != self.axis else c + 1)
+                for d in range(raw.spec.roi.dims)
             )
 
-            if augmentation_type == 'zero_out':
+            if augmentation_type == "zero_out":
                 raw.data[section_selector] = 0
 
-            elif augmentation_type == 'low_contrast':
+            elif augmentation_type == "low_contrast":
                 section = raw.data[section_selector]
 
                 mean = section.mean()
                 section -= mean
                 section *= self.contrast_scale
                 section += mean
 
                 raw.data[section_selector] = section
 
-            elif augmentation_type == 'artifact':
-
+            elif augmentation_type == "artifact":
                 section = raw.data[section_selector]
 
-                alpha_voxel_size = self.artifact_source.spec[self.artifacts_mask].voxel_size
-
-                assert raw_voxel_size == alpha_voxel_size, ("Can only alpha blend RAW with "
-                                                            "ALPHA_MASK if both have the same "
-                                                            "voxel size")
+                alpha_voxel_size = self.artifact_source.spec[
+                    self.artifacts_mask
+                ].voxel_size
+
+                assert raw_voxel_size == alpha_voxel_size, (
+                    "Can only alpha blend RAW with "
+                    "ALPHA_MASK if both have the same "
+                    "voxel size"
+                )
 
                 artifact_request = BatchRequest()
-                artifact_request.add(self.artifacts, Coordinate(section.shape) * raw_voxel_size, voxel_size=raw_voxel_size)
-                artifact_request.add(self.artifacts_mask, Coordinate(section.shape) * alpha_voxel_size, voxel_size=raw_voxel_size)
+                artifact_request.add(
+                    self.artifacts,
+                    Coordinate(section.shape) * raw_voxel_size,
+                    voxel_size=raw_voxel_size,
+                )
+                artifact_request.add(
+                    self.artifacts_mask,
+                    Coordinate(section.shape) * alpha_voxel_size,
+                    voxel_size=raw_voxel_size,
+                )
                 logger.debug("Requesting artifact batch %s", artifact_request)
 
                 artifact_batch = self.artifact_source.request_batch(artifact_request)
                 artifact_alpha = artifact_batch.arrays[self.artifacts_mask].data
-                artifact_raw   = artifact_batch.arrays[self.artifacts].data
+                artifact_raw = artifact_batch.arrays[self.artifacts].data
 
                 assert artifact_alpha.dtype == np.float32
                 assert artifact_alpha.min() >= 0.0
                 assert artifact_alpha.max() <= 1.0
 
-                raw.data[section_selector] = section*(1.0 - artifact_alpha) + artifact_raw*artifact_alpha
-
-            elif augmentation_type == 'deformed_slice':
+                raw.data[section_selector] = (
+                    section * (1.0 - artifact_alpha) + artifact_raw * artifact_alpha
+                )
 
+            elif augmentation_type == "deformed_slice":
                 section = raw.data[section_selector].squeeze()
 
                 # set interpolation to cubic, spec interploatable is true, else to 0
                 interpolation = 3 if self.spec[self.intensities].interpolatable else 0
 
                 # load the deformation fields that were prepared for this slice
                 flow_x, flow_y, line_mask = self.deform_slice_transformations[c]
 
                 # apply the deformation fields
                 shape = section.shape
                 section = map_coordinates(
-                    section, (flow_y, flow_x), mode='constant', order=interpolation
+                    section, (flow_y, flow_x), mode="constant", order=interpolation
                 ).reshape(shape)
 
                 # things can get smaller than 0 at the boundary, so we clip
-                section = np.clip(section, 0., 1.)
+                section = np.clip(section, 0.0, 1.0)
 
                 # zero-out data below the line mask
-                section[line_mask] = 0.
+                section[line_mask] = 0.0
 
                 raw.data[section_selector] = section
 
         # in case we needed to change the ROI due to a deformation augment,
         # restore original ROI and crop the array data
-        if 'deformed_slice' in self.slice_to_augmentation.values():
+        if "deformed_slice" in self.slice_to_augmentation.values():
             old_roi = request[self.intensities].roi
             logger.debug("resetting roi to %s" % old_roi)
             crop = tuple(
-                slice(None) if d == self.axis else slice(self.deformation_strength, -self.deformation_strength)
-                for d in range(raw.spec.roi.dims())
+                slice(None)
+                if d == self.axis
+                else slice(self.deformation_strength, -self.deformation_strength)
+                for d in range(raw.spec.roi.dims)
             )
             raw.data = raw.data[crop]
             raw.spec.roi = old_roi
 
     def __prepare_deform_slice(self, slice_shape):
-
         # grow slice shape by 2 x deformation strength
         grow_by = 2 * self.deformation_strength
         shape = (slice_shape[0] + grow_by, slice_shape[1] + grow_by)
 
         # randomly choose fixed x or fixed y with p = 1/2
-        fixed_x = random.random() < .5
+        fixed_x = random.random() < 0.5
         if fixed_x:
             x0, y0 = 0, np.random.randint(1, shape[1] - 2)
             x1, y1 = shape[0] - 1, np.random.randint(1, shape[1] - 2)
         else:
             x0, y0 = np.random.randint(1, shape[0] - 2), 0
             x1, y1 = np.random.randint(1, shape[0] - 2), shape[1] - 1
 
         ## generate the mask of the line that should be blacked out
-        line_mask = np.zeros(shape, dtype='bool')
+        line_mask = np.zeros(shape, dtype="bool")
         rr, cc = line(x0, y0, x1, y1)
         line_mask[rr, cc] = 1
 
         # generate vectorfield pointing towards the line to compress the image
         # first we get the unit vector representing the line
-        line_vector = np.array([x1 - x0, y1 - y0], dtype='float32')
+        line_vector = np.array([x1 - x0, y1 - y0], dtype="float32")
         line_vector /= np.linalg.norm(line_vector)
         # next, we generate the normal to the line
         normal_vector = np.zeros_like(line_vector)
-        normal_vector[0] = - line_vector[1]
+        normal_vector[0] = -line_vector[1]
         normal_vector[1] = line_vector[0]
 
         # make meshgrid
         x, y = np.meshgrid(np.arange(shape[1]), np.arange(shape[0]))
         # generate the vector field
         flow_x, flow_y = np.zeros(shape), np.zeros(shape)
 
         # find the 2 components where coordinates are bigger / smaller than the line
         # to apply normal vector in the correct direction
-        components, n_components = label(np.logical_not(line_mask).view('uint8'))
+        components, n_components = label(np.logical_not(line_mask).view("uint8"))
         assert n_components == 2, "%i" % n_components
         neg_val = components[0, 0] if fixed_x else components[-1, -1]
         pos_val = components[-1, -1] if fixed_x else components[0, 0]
 
         flow_x[components == pos_val] = self.deformation_strength * normal_vector[1]
         flow_y[components == pos_val] = self.deformation_strength * normal_vector[0]
-        flow_x[components == neg_val] = - self.deformation_strength * normal_vector[1]
-        flow_y[components == neg_val] = - self.deformation_strength * normal_vector[0]
+        flow_x[components == neg_val] = -self.deformation_strength * normal_vector[1]
+        flow_y[components == neg_val] = -self.deformation_strength * normal_vector[0]
 
         # generate the flow fields
         flow_x, flow_y = (x + flow_x).reshape(-1, 1), (y + flow_y).reshape(-1, 1)
 
         # dilate the line mask
         line_mask = binary_dilation(line_mask, iterations=10)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/downsample.py` & `gunpowder-1.3.0/gunpowder/nodes/downsample.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 from .batch_filter import BatchFilter
 from gunpowder.array import ArrayKey, Array
 from gunpowder.batch_request import BatchRequest
 from gunpowder.batch import Batch
 import logging
 import numbers
+from funlib.geometry import Coordinate
 
 logger = logging.getLogger(__name__)
 
+
 class DownSample(BatchFilter):
-    '''Downsample arrays in a batch by given factors.
+    """Downsample arrays in a batch by given factors.
 
     Args:
 
         source (:class:`ArrayKey`):
 
             The key of the array to downsample.
 
         factor (``int`` or ``tuple`` of ``int``):
 
             The factor to downsample with.
 
         target (:class:`ArrayKey`):
 
             The key of the array to store the downsampled ``source``.
-    '''
+    """
 
     def __init__(self, source, factor, target):
-
         assert isinstance(source, ArrayKey)
         assert isinstance(target, ArrayKey)
-        assert (
-            isinstance(factor, numbers.Number) or isinstance(factor, tuple)), (
-            "Scaling factor should be a number or a tuple of numbers.")
+        assert isinstance(factor, numbers.Number) or isinstance(
+            factor, tuple
+        ), "Scaling factor should be a number or a tuple of numbers."
 
         self.source = source
-        self.factor = factor
+        self.factor = (
+            factor if isinstance(factor, numbers.Number) else Coordinate(factor)
+        )
         self.target = target
 
     def setup(self):
-
         spec = self.spec[self.source].copy()
         spec.voxel_size *= self.factor
         self.provides(self.target, spec)
         self.enable_autoskip()
 
     def prepare(self, request):
-
         deps = BatchRequest()
         deps[self.source] = request[self.target]
         return deps
 
     def process(self, batch, request):
         outputs = Batch()
+        data = batch.arrays[self.source].data
+
+        channel_dims = len(data.shape) - batch.arrays[self.source].spec.roi.dims
 
         # downsample
         if isinstance(self.factor, tuple):
-            slices = tuple(
-                slice(None, None, k)
-                for k in self.factor)
+            slices = tuple(slice(None, None) for _ in range(channel_dims)) + tuple(
+                slice(None, None, k) for k in self.factor
+            )
         else:
-            slices = tuple(
+            slices = tuple(slice(None, None) for _ in range(channel_dims)) + tuple(
                 slice(None, None, self.factor)
-                for i in range(batch[self.source].spec.roi.dims()))
+                for i in range(batch[self.source].spec.roi.dims)
+            )
 
         logger.debug("downsampling %s with %s", self.source, slices)
 
-        data = batch.arrays[self.source].data[slices]
+        data = data[slices]
 
         # create output array
         spec = self.spec[self.target].copy()
         spec.roi = request[self.target].roi
         outputs.arrays[self.target] = Array(data, spec)
-        
+
         return outputs
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/dvid_source.py` & `gunpowder-1.3.0/gunpowder/nodes/dvid_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from gunpowder.roi import Roi
 from gunpowder.array import Array
 from gunpowder.array_spec import ArraySpec
 from .batch_provider import BatchProvider
 
 logger = logging.getLogger(__name__)
 
+
 class DvidSource(BatchProvider):
-    '''A DVID array source.
+    """A DVID array source.
 
     Provides arrays from DVID servers for each array key given.
 
     Args:
 
         hostname (``string``):
 
@@ -43,212 +44,194 @@
 
         array_specs (``dict``, :class:`ArrayKey` -> :class:`ArraySpec`, optional):
 
             An optional dictionary of array keys to specs to overwrite the
             array specs automatically determined from the DVID server. This is
             useful to set ``voxel_size``, for example. Only fields that are not
             ``None`` in the given :class:`ArraySpec` will be used.
-    '''
-
-    def __init__(
-            self,
-            hostname,
-            port,
-            uuid,
-            datasets,
-            masks=None,
-            array_specs=None):
+    """
 
+    def __init__(self, hostname, port, uuid, datasets, masks=None, array_specs=None):
         self.hostname = hostname
         self.port = port
         self.url = "http://{}:{}".format(self.hostname, self.port)
         self.uuid = uuid
 
         self.datasets = datasets
         self.masks = masks if masks is not None else {}
 
         self.array_specs = array_specs if array_specs is not None else {}
 
         self.ndims = None
 
     def setup(self):
-
         for array_key, _ in self.datasets.items():
             spec = self.__get_spec(array_key)
             self.provides(array_key, spec)
 
         for array_key, _ in self.masks.items():
             spec = self.__get_mask_spec(array_key)
             self.provides(array_key, spec)
 
         logger.info("DvidSource.spec:\n%s", self.spec)
 
     def provide(self, request):
-
         timing = Timing(self)
         timing.start()
 
         batch = Batch()
 
-        for (array_key, request_spec) in request.array_specs.items():
-
+        for array_key, request_spec in request.array_specs.items():
             logger.debug("Reading %s in %s...", array_key, request_spec.roi)
 
             voxel_size = self.spec[array_key].voxel_size
 
             # scale request roi to voxel units
-            dataset_roi = request_spec.roi/voxel_size
+            dataset_roi = request_spec.roi / voxel_size
 
             # shift request roi into dataset
-            dataset_roi = dataset_roi - self.spec[array_key].roi.get_offset()/voxel_size
+            dataset_roi = dataset_roi - self.spec[array_key].roi.offset / voxel_size
 
             # create array spec
             array_spec = self.spec[array_key].copy()
             array_spec.roi = request_spec.roi
 
             # read the data
             if array_key in self.datasets:
                 data = self.__read_array(self.datasets[array_key], dataset_roi)
             elif array_key in self.masks:
                 data = self.__read_mask(self.masks[array_key], dataset_roi)
             else:
-                assert False, ("Encountered a request for %s that is neither a volume "
-                               "nor a mask."%array_key)
+                assert False, (
+                    "Encountered a request for %s that is neither a volume "
+                    "nor a mask." % array_key
+                )
 
             # add array to batch
             batch.arrays[array_key] = Array(data, array_spec)
 
         logger.debug("done")
 
         timing.stop()
         batch.profiling_stats.add(timing)
 
         return batch
 
     def __get_info(self, array_key):
-
         if array_key in self.datasets:
-
             data = dvision.DVIDDataInstance(
-                self.hostname,
-                self.port,
-                self.uuid,
-                self.datasets[array_key])
+                self.hostname, self.port, self.uuid, self.datasets[array_key]
+            )
 
         elif array_key in self.masks:
-
             data = dvision.DVIDRegionOfInterest(
-                self.hostname,
-                self.port,
-                self.uuid,
-                self.masks[array_key])
+                self.hostname, self.port, self.uuid, self.masks[array_key]
+            )
 
         else:
-
-            assert False, ("Encountered a request that is neither a volume "
-                           "nor a mask.")
+            assert False, (
+                "Encountered a request that is neither a volume " "nor a mask."
+            )
 
         return data.info
 
     def __get_spec(self, array_key):
-
         info = self.__get_info(array_key)
 
-        roi_min = info['Extended']['MinPoint']
+        roi_min = info["Extended"]["MinPoint"]
         if roi_min is not None:
             roi_min = Coordinate(roi_min[::-1])
-        roi_max = info['Extended']['MaxPoint']
+        roi_max = info["Extended"]["MaxPoint"]
         if roi_max is not None:
             roi_max = Coordinate(roi_max[::-1])
 
-        data_roi = Roi(
-            offset=roi_min,
-            shape=(roi_max - roi_min))
-        data_dims = Coordinate(data_roi.get_shape())
+        data_roi = Roi(offset=roi_min, shape=(roi_max - roi_min))
+        data_dims = Coordinate(data_roi.shape)
 
         if self.ndims is None:
             self.ndims = len(data_dims)
         else:
             assert self.ndims == len(data_dims)
 
         if array_key in self.array_specs:
             spec = self.array_specs[array_key].copy()
         else:
             spec = ArraySpec()
 
         if spec.voxel_size is None:
-            spec.voxel_size = Coordinate(info['Extended']['VoxelSize'])
+            spec.voxel_size = Coordinate(info["Extended"]["VoxelSize"])
 
         if spec.roi is None:
-            spec.roi = data_roi*spec.voxel_size
+            spec.roi = data_roi * spec.voxel_size
 
         data_dtype = dvision.DVIDDataInstance(
-            self.hostname,
-            self.port,
-            self.uuid,
-            self.datasets[array_key]).dtype
+            self.hostname, self.port, self.uuid, self.datasets[array_key]
+        ).dtype
 
         if spec.dtype is not None:
-            assert spec.dtype == data_dtype, ("dtype %s provided in array_specs for %s, "
-                                              "but differs from instance %s dtype %s"%
-                                              (self.array_specs[array_key].dtype,
-                                               array_key,
-                                               self.datasets[array_key],
-                                               data_dtype))
+            assert spec.dtype == data_dtype, (
+                "dtype %s provided in array_specs for %s, "
+                "but differs from instance %s dtype %s"
+                % (
+                    self.array_specs[array_key].dtype,
+                    array_key,
+                    self.datasets[array_key],
+                    data_dtype,
+                )
+            )
         else:
             spec.dtype = data_dtype
 
         if spec.interpolatable is None:
-
             spec.interpolatable = spec.dtype in [
-                np.float,
                 np.float32,
                 np.float64,
                 np.float128,
-                np.uint8 # assuming this is not used for labels
+                np.uint8,  # assuming this is not used for labels
             ]
-            logger.warning("WARNING: You didn't set 'interpolatable' for %s. "
-                           "Based on the dtype %s, it has been set to %s. "
-                           "This might not be what you want.",
-                           array_key, spec.dtype, spec.interpolatable)
+            logger.warning(
+                "WARNING: You didn't set 'interpolatable' for %s. "
+                "Based on the dtype %s, it has been set to %s. "
+                "This might not be what you want.",
+                array_key,
+                spec.dtype,
+                spec.interpolatable,
+            )
 
         return spec
 
     def __get_mask_spec(self, mask_key):
-
         # create initial array spec
 
         if mask_key in self.array_specs:
             spec = self.array_specs[mask_key].copy()
         else:
             spec = ArraySpec()
 
         # get voxel size
 
         if spec.voxel_size is None:
-
             voxel_size = None
             for array_key in self.datasets:
                 if voxel_size is None:
                     voxel_size = self.spec[array_key].voxel_size
                 else:
                     assert voxel_size == self.spec[array_key].voxel_size, (
                         "No voxel size was given for mask %s, and the voxel "
                         "sizes of the volumes %s are not all the same. I don't "
-                        "know what voxel size to use to create the mask."%(
-                            mask_key, self.datasets.keys()))
+                        "know what voxel size to use to create the mask."
+                        % (mask_key, self.datasets.keys())
+                    )
 
             spec.voxel_size = voxel_size
 
         # get ROI
 
         if spec.roi is None:
-
             for array_key in self.datasets:
-
                 roi = self.spec[array_key].roi
 
                 if spec.roi is None:
                     spec.roi = roi.copy()
                 else:
                     spec.roi = roi.union(spec.roi)
 
@@ -256,39 +239,34 @@
 
         if spec.interpolatable is None:
             spec.interpolatable = False
 
         # set datatype
 
         if spec.dtype is not None and spec.dtype != np.uint8:
-            logger.warn("Ignoring dtype in array_spec for %s, only np.uint8 "
-                        "is allowed for masks.", mask_key)
+            logger.warn(
+                "Ignoring dtype in array_spec for %s, only np.uint8 "
+                "is allowed for masks.",
+                mask_key,
+            )
         spec.dtype = np.uint8
 
         return spec
 
     def __read_array(self, instance, roi):
-
         data_instance = dvision.DVIDDataInstance(
-            self.hostname,
-            self.port,
-            self.uuid,
-            instance)
+            self.hostname, self.port, self.uuid, instance
+        )
 
         return data_instance[roi.get_bounding_box()]
 
     def __read_mask(self, instance, roi):
-
         dvid_roi = dvision.DVIDRegionOfInterest(
-            self.hostname,
-            self.port,
-            self.uuid,
-            instance)
+            self.hostname, self.port, self.uuid, instance
+        )
 
         return dvid_roi[roi.get_bounding_box()]
 
     def __repr__(self):
-
         return "DvidSource(hostname={}, port={}, uuid={}".format(
-            self.hostname,
-            self.port,
-            self.uuid)
+            self.hostname, self.port, self.uuid
+        )
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/elastic_augment.py` & `gunpowder-1.3.0/gunpowder/nodes/elastic_augment.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 from .batch_filter import BatchFilter
 from gunpowder.batch_request import BatchRequest
 from gunpowder.coordinate import Coordinate
 from gunpowder.ext import augment
 from gunpowder.roi import Roi
 from gunpowder.array import ArrayKey
 
+import warnings
+
 logger = logging.getLogger(__name__)
 
 
 class ElasticAugment(BatchFilter):
-    """Elasticly deform a batch. Requests larger batches upstream to avoid data 
+    """(DEPRICATED) Elasticly deform a batch. Requests larger batches upstream to avoid data
     loss due to rotation and jitter.
 
     Args:
 
         control_point_spacing (``tuple`` of ``int``):
 
             Distance between control points for the elastic deformation, in
@@ -98,14 +100,18 @@
         prob_shift=0,
         max_misalign=0,
         subsample=1,
         spatial_dims=3,
         use_fast_points_transform=False,
         recompute_missing_points=True,
     ):
+        warnings.warn(
+            "ElasticAugment is deprecated, please use the DeformAugment",
+            DeprecationWarning,
+        )
 
         self.control_point_spacing = control_point_spacing
         self.jitter_sigma = jitter_sigma
         self.rotation_start = rotation_interval[0]
         self.rotation_max_amount = rotation_interval[1] - rotation_interval[0]
         self.scale_min = scale_interval[0]
         self.scale_max = scale_interval[1]
@@ -131,18 +137,18 @@
         logger.debug("total ROI is %s" % total_roi)
 
         # First, get the total ROI of the request in spatial dimensions only.
         # Channels and time don't matter. This is our master ROI.
 
         # get master ROI
         master_roi = Roi(
-            total_roi.get_begin()[-self.spatial_dims :],
-            total_roi.get_shape()[-self.spatial_dims :],
+            total_roi.begin[-self.spatial_dims :],
+            total_roi.shape[-self.spatial_dims :],
         )
-        self.spatial_dims = master_roi.dims()
+        self.spatial_dims = master_roi.dims
         logger.debug("master ROI is %s" % master_roi)
 
         # make sure the master ROI aligns with the voxel size
         master_roi = master_roi.snap_to_grid(self.voxel_size, mode="grow")
         logger.debug("master ROI aligned with voxel size is %s" % master_roi)
 
         # get master roi in voxels
@@ -151,36 +157,35 @@
 
         # Second, create a master transformation. This is a transformation that
         # covers all voxels of the all requested ROIs. The master transformation
         # is zero-based.
 
         # create a transformation with the size of the master ROI in voxels
         self.master_transformation = self.__create_transformation(
-            master_roi_voxels.get_shape()
+            master_roi_voxels.shape
         )
 
         # Third, crop out parts of the master transformation for each of the
         # smaller requested ROIs. Since these ROIs now have to align with the
         # voxel size (which for points does not have to be the case), we also
         # remember these smaller ROIs as target_rois in global world units.
 
         # crop the parts corresponding to the requested ROIs
         self.transformations = {}
         self.target_rois = {}
         deps = BatchRequest()
         for key, spec in request.items():
-
             spec = spec.copy()
 
             if spec.roi is None:
                 continue
 
             target_roi = Roi(
-                spec.roi.get_begin()[-self.spatial_dims :],
-                spec.roi.get_shape()[-self.spatial_dims :],
+                spec.roi.begin[-self.spatial_dims :],
+                spec.roi.shape[-self.spatial_dims :],
             )
             logger.debug("downstream request spatial ROI for %s is %s", key, target_roi)
 
             # make sure the target ROI aligns with the voxel grid (which might
             # not be the case for points)
             target_roi = target_roi.snap_to_grid(self.voxel_size, mode="grow")
             logger.debug(
@@ -195,15 +200,15 @@
             self.target_rois[key] = target_roi
 
             # get ROI in voxels
             target_roi_voxels = target_roi / self.voxel_size
 
             # get ROI relative to master ROI
             target_roi_in_master_roi_voxels = (
-                target_roi_voxels - master_roi_voxels.get_begin()
+                target_roi_voxels - master_roi_voxels.begin
             )
 
             # crop out relevant part of transformation for this request
             transformation = np.copy(
                 self.master_transformation[
                     (slice(None),) + target_roi_in_master_roi_voxels.get_bounding_box()
                 ]
@@ -213,65 +218,63 @@
             # get ROI of all voxels necessary to perfrom transformation
             #
             # for that we follow the same transformations to get from the
             # request ROI to the target ROI in master ROI in voxels, just in
             # reverse
             source_roi_in_master_roi_voxels = self.__get_source_roi(transformation)
             source_roi_voxels = (
-                source_roi_in_master_roi_voxels + master_roi_voxels.get_begin()
+                source_roi_in_master_roi_voxels + master_roi_voxels.begin
             )
             source_roi = source_roi_voxels * self.voxel_size
 
             # transformation is still defined on voxels relative to master ROI
             # in voxels (i.e., lowest source coordinate could be 5, but data
             # array we get later starts at 0).
             #
             # shift transformation to be indexed relative to beginning of
             # source_roi_voxels
             self.__shift_transformation(
-                -source_roi_in_master_roi_voxels.get_begin(), transformation
+                -source_roi_in_master_roi_voxels.begin, transformation
             )
 
             # update upstream request
             spec.roi = Roi(
-                spec.roi.get_begin()[: -self.spatial_dims]
-                + source_roi.get_begin()[-self.spatial_dims :],
-                spec.roi.get_shape()[: -self.spatial_dims]
-                + source_roi.get_shape()[-self.spatial_dims :],
+                spec.roi.begin[: -self.spatial_dims]
+                + source_roi.begin[-self.spatial_dims :],
+                spec.roi.shape[: -self.spatial_dims]
+                + source_roi.shape[-self.spatial_dims :],
             )
 
             deps[key] = spec
 
             logger.debug("upstream request roi for %s = %s" % (key, spec.roi))
 
         return deps
 
     def process(self, batch, request):
-
-        for (array_key, array) in batch.arrays.items():
-
+        for array_key, array in batch.arrays.items():
             if array_key not in self.target_rois:
                 continue
 
             # for arrays, the target ROI and the requested ROI should be the
             # same in spatial coordinates
             assert (
-                self.target_rois[array_key].get_begin()
-                == request[array_key].roi.get_begin()[-self.spatial_dims :]
+                self.target_rois[array_key].begin
+                == request[array_key].roi.begin[-self.spatial_dims :]
             ), "Target roi offset {} does not match request roi offset {}".format(
-                self.target_rois[array_key].get_begin(),
-                request[array_key].roi.get_begin()[-self.spatial_dims :],
+                self.target_rois[array_key].begin,
+                request[array_key].roi.begin[-self.spatial_dims :],
             )
 
             assert (
-                self.target_rois[array_key].get_shape()
-                == request[array_key].roi.get_shape()[-self.spatial_dims :]
+                self.target_rois[array_key].shape
+                == request[array_key].roi.shape[-self.spatial_dims :]
             ), "Target roi offset {} does not match request roi offset {}".format(
-                self.target_rois[array_key].get_shape(),
-                request[array_key].roi.get_shape()[-self.spatial_dims :],
+                self.target_rois[array_key].shape,
+                request[array_key].roi.shape[-self.spatial_dims :],
             )
 
             # reshape array data into (channels,) + spatial dims
             shape = array.data.shape
             channel_shape = shape[: -self.spatial_dims]
             data = array.data.reshape((-1,) + shape[-self.spatial_dims :])
 
@@ -283,22 +286,23 @@
                         self.transformations[array_key],
                         interpolate=self.spec[array_key].interpolatable,
                     )
                     for c in range(data.shape[0])
                 ]
             )
 
-            data_roi = request[array_key].roi/self.spec[array_key].voxel_size
-            array.data = data.reshape(channel_shape + data_roi.get_shape()[-self.spatial_dims:])
+            data_roi = request[array_key].roi / self.spec[array_key].voxel_size
+            array.data = data.reshape(
+                channel_shape + data_roi.shape[-self.spatial_dims :]
+            )
 
             # restore original ROIs
             array.spec.roi = request[array_key].roi
 
-        for (graph_key, graph) in batch.graphs.items():
-
+        for graph_key, graph in batch.graphs.items():
             nodes = list(graph.nodes)
 
             if self.use_fast_points_transform:
                 missed_nodes = self.__fast_point_projection(
                     self.transformations[graph_key],
                     nodes,
                     graph.spec.roi,
@@ -311,15 +315,15 @@
             else:
                 missed_nodes = nodes
 
             for node in missed_nodes:
                 # logger.debug("projecting %s", node.location)
 
                 # get location relative to beginning of upstream ROI
-                location = node.location - graph.spec.roi.get_begin()
+                location = node.location - graph.spec.roi.begin
                 logger.debug("relative to upstream ROI: %s", location)
 
                 # get spatial coordinates of node in voxels
                 location_voxels = location[-self.spatial_dims :] / self.voxel_size
 
                 # get projected location in transformation data space, this
                 # yields voxel coordinates relative to target ROI
@@ -336,22 +340,22 @@
                     graph.remove_node(node, retain_connectivity=True)
                     continue
 
                 # convert to world units (now in float again)
                 projected = projected_voxels * np.array(self.voxel_size)
 
                 logger.debug(
-                    "projected in world units, relative to target ROI: %s",
-                    projected)
+                    "projected in world units, relative to target ROI: %s", projected
+                )
 
                 # get global coordinates
-                projected += np.array(self.target_rois[graph_key].get_begin())
+                projected += np.array(self.target_rois[graph_key].begin)
 
                 # update spatial coordinates of node location
-                node.location[-self.spatial_dims:] = projected
+                node.location[-self.spatial_dims :] = projected
 
                 logger.debug("final location: %s", node.location)
 
                 # finally, it can happen that a node no longer is contained in
                 # the requested ROI (because larger ROIs than necessary have
                 # been requested upstream)
                 if not request[graph_key].roi.contains(node.location):
@@ -359,38 +363,41 @@
                     graph.remove_node(node, retain_connectivity=True)
                     continue
 
             # restore original ROIs
             graph.spec.roi = request[graph_key].roi
 
     def __get_common_voxel_size(self, request):
-
         voxel_size = None
         prev = None
         for array_key in request.array_specs.keys():
             if voxel_size is None:
-                voxel_size = self.spec[array_key].voxel_size[-self.spatial_dims:]
+                voxel_size = self.spec[array_key].voxel_size[-self.spatial_dims :]
             elif self.spec[array_key].voxel_size is not None:
-                assert voxel_size == self.spec[array_key].voxel_size[-self.spatial_dims:], \
-                        "ElasticAugment can only be used with arrays of same voxel sizes, " \
-                        "but %s has %s, and %s has %s."%(
-                                array_key, self.spec[array_key].voxel_size,
-                                prev, self.spec[prev].voxel_size)
+                assert (
+                    voxel_size == self.spec[array_key].voxel_size[-self.spatial_dims :]
+                ), (
+                    "ElasticAugment can only be used with arrays of same voxel sizes, "
+                    "but %s has %s, and %s has %s."
+                    % (
+                        array_key,
+                        self.spec[array_key].voxel_size,
+                        prev,
+                        self.spec[prev].voxel_size,
+                    )
+                )
             prev = array_key
 
         if voxel_size is None:
             raise RuntimeError("voxel size must not be None")
 
-        return voxel_size
+        return Coordinate(voxel_size)
 
     def __create_transformation(self, target_shape):
-
-        scale = self.scale_min + random.random()*(
-            self.scale_max - self.scale_min
-        )
+        scale = self.scale_min + random.random() * (self.scale_max - self.scale_min)
 
         transformation = augment.create_identity_transformation(
             target_shape, subsample=self.subsample, scale=scale
         )
         if sum(self.jitter_sigma) > 0:
             transformation += augment.create_elastic_transformation(
                 target_shape,
@@ -410,35 +417,31 @@
             )
 
         if self.prob_slip + self.prob_shift > 0:
             self.__misalign(transformation)
 
         return transformation
 
-    def __fast_point_projection(
-        self, transformation, nodes, source_roi, target_roi
-    ):
+    def __fast_point_projection(self, transformation, nodes, source_roi, target_roi):
         if len(nodes) < 1:
             return []
         # rasterize the points into an array
         ids, locs = zip(
             *[
                 (
                     node.id,
-                    (np.floor(node.location).astype(int) - source_roi.get_begin())
+                    (np.floor(node.location).astype(int) - source_roi.begin)
                     // self.voxel_size,
                 )
                 for node in nodes
                 if source_roi.contains(node.location)
             ]
         )
         ids, locs = np.array(ids), tuple(zip(*locs))
-        points_array = np.zeros(
-            source_roi.get_shape() / self.voxel_size, dtype=np.int64
-        )
+        points_array = np.zeros(source_roi.shape / self.voxel_size, dtype=np.int64)
         points_array[locs] = ids
 
         # reshape array data into (channels,) + spatial dims
         shape = points_array.shape
         data = points_array.reshape((-1,) + shape[-self.spatial_dims :])
 
         # apply transformation on each channel
@@ -450,19 +453,18 @@
                 for c in range(data.shape[0])
             ]
         )
 
         missing_points = []
         projected_locs = ndimage.measurements.center_of_mass(data > 0, data, ids)
         projected_locs = [
-            np.array(loc[-self.spatial_dims :]) * self.voxel_size
-            + target_roi.get_begin()
+            np.array(loc[-self.spatial_dims :]) * self.voxel_size + target_roi.begin
             for loc in projected_locs
         ]
-        node_dict = {node.id:node for node in nodes}
+        node_dict = {node.id: node for node in nodes}
         for point_id, proj_loc in zip(ids, projected_locs):
             point = node_dict.pop(point_id)
             if not any([np.isnan(x) for x in proj_loc]):
                 assert (
                     len(proj_loc) == self.spatial_dims
                 ), "projected location has wrong number of dimensions: {}, expected: {}".format(
                     len(proj_loc), self.spatial_dims
@@ -503,27 +505,27 @@
 
         logger.debug("projecting %s onto grid", location)
         logger.debug("grid shape: %s", transformation.shape[1:])
         logger.debug("grid projection: %s", center_grid)
         logger.debug("dist shape: %s", dist.shape)
         logger.debug("dist.argmin(): %s", dist.argmin())
         logger.debug("dist[argmin]: %s", dist[center_grid])
-        logger.debug("transform[argmin]: %s",
-                     transformation[(slice(None),) + center_grid])
+        logger.debug(
+            "transform[argmin]: %s", transformation[(slice(None),) + center_grid]
+        )
         logger.debug("min dist: %s", dist.min())
         logger.debug("center source: %s", center_source)
 
         # inspect grid edges incident to center_grid
         for d in range(dims):
-
             # nothing to do for dimensions without spatial extent
             if transformation.shape[1 + d] == 1:
                 continue
 
-            dim_vector = tuple(1 if dd == d else 0 for dd in range(dims))
+            dim_vector = Coordinate(1 if dd == d else 0 for dd in range(dims))
             pos_grid = center_grid + dim_vector
             neg_grid = center_grid - dim_vector
             logger.debug("interpolating along %s", dim_vector)
 
             pos_u = -1
             neg_u = -1
 
@@ -558,15 +560,14 @@
     def __source_at(self, transformation, index):
         """Read the source point of a transformation at index."""
 
         slices = (slice(None),) + tuple(slice(i, i + 1) for i in index)
         return transformation[slices].flatten()
 
     def __get_source_roi(self, transformation):
-
         dims = transformation.shape[0]
 
         # get bounding box of needed data for transformation
         bb_min = Coordinate(
             int(math.floor(transformation[d].min())) for d in range(dims)
         )
         bb_max = Coordinate(
@@ -575,37 +576,32 @@
 
         # create roi sufficiently large to feed transformation
         source_roi = Roi(bb_min, bb_max - bb_min)
 
         return source_roi
 
     def __shift_transformation(self, shift, transformation):
-
         for d in range(transformation.shape[0]):
             transformation[d] += shift[d]
 
     def __misalign(self, transformation):
-
         assert (
             transformation.shape[0] == 3
         ), "misalign can only be applied to 3D volumes"
 
         num_sections = transformation[0].shape[0]
 
         shifts = [Coordinate((0, 0, 0))] * num_sections
         for z in range(num_sections):
-
             r = random.random()
 
             if r <= self.prob_slip:
-
                 shifts[z] = self.__random_offset()
 
             elif r <= self.prob_slip + self.prob_shift:
-
                 offset = self.__random_offset()
                 for zp in range(z, num_sections):
                     shifts[zp] += offset
 
         logger.debug("misaligning sections with " + str(shifts))
 
         dims = 3
@@ -623,15 +619,14 @@
             "min/max of transformation after misalignment: "
             + str(bb_min)
             + "/"
             + str(bb_max)
         )
 
     def __random_offset(self):
-
         return Coordinate(
             (0,)
             + tuple(
                 self.max_misalign - random.randint(0, 2 * int(self.max_misalign))
                 for d in range(2)
             )
         )
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/exclude_labels.py` & `gunpowder-1.3.0/gunpowder/nodes/exclude_labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from scipy.ndimage.morphology import distance_transform_edt
 
 from .batch_filter import BatchFilter
 from gunpowder.array import Array
 
 logger = logging.getLogger(__name__)
 
+
 class ExcludeLabels(BatchFilter):
-    '''Excludes several labels from the ground-truth.
+    """Excludes several labels from the ground-truth.
 
     The labels will be replaced by background_value. An optional ignore mask
     will be created and set to 0 for the excluded locations that are further
     than a threshold away from not excluded locations.
 
     Args:
 
@@ -31,76 +32,73 @@
         ignore_mask_erode (``float``, optional):
 
             By how much (in world units) to erode the ignore mask.
 
         background_value (``int``, optional):
 
             Value to replace excluded IDs, defaults to 0.
-    '''
+    """
 
     def __init__(
-            self,
-            labels,
-            exclude,
-            ignore_mask=None,
-            ignore_mask_erode=0,
-            background_value=0):
-
+        self, labels, exclude, ignore_mask=None, ignore_mask_erode=0, background_value=0
+    ):
         self.labels = labels
         self.exclude = set(exclude)
         self.ignore_mask = ignore_mask
         self.ignore_mask_erode = ignore_mask_erode
         self.background_value = background_value
 
     def setup(self):
-
-        assert self.labels in self.spec, "ExcludeLabels can only be used if GT_LABELS is provided upstream."
+        assert (
+            self.labels in self.spec
+        ), "ExcludeLabels can only be used if GT_LABELS is provided upstream."
         if self.ignore_mask:
             self.provides(self.ignore_mask, self.spec[self.labels])
 
     def process(self, batch, request):
-
         gt = batch.arrays[self.labels]
 
         # 0 marks included regions (to be used directly with distance transform
         # later)
         include_mask = np.ones(gt.data.shape)
 
         gt_labels = np.unique(gt.data)
         logger.debug("batch contains GT labels: " + str(gt_labels))
         for label in gt_labels:
             if label in self.exclude:
                 logger.debug("excluding label " + str(label))
-                gt.data[gt.data==label] = self.background_value
+                gt.data[gt.data == label] = self.background_value
             else:
-                include_mask[gt.data==label] = 0
+                include_mask[gt.data == label] = 0
 
         # if no ignore mask is provided or requested, we are done
         if not self.ignore_mask or not self.ignore_mask in request:
             return
 
         voxel_size = self.spec[self.labels].voxel_size
         distance_to_include = distance_transform_edt(include_mask, sampling=voxel_size)
         logger.debug("max distance to foreground is " + str(distance_to_include.max()))
 
         # 1 marks included regions, plus a context area around them
-        include_mask = distance_to_include<self.ignore_mask_erode
+        include_mask = distance_to_include < self.ignore_mask_erode
 
         # include mask was computed on labels ROI, we need to copy it to
         # the requested ignore_mask ROI
         gt_ignore_roi = request[self.ignore_mask].roi
 
         intersection = gt.spec.roi.intersect(gt_ignore_roi)
-        intersection_in_gt = intersection - gt.spec.roi.get_offset()
-        intersection_in_gt_ignore = intersection - gt_ignore_roi.get_offset()
+        intersection_in_gt = intersection - gt.spec.roi.offset
+        intersection_in_gt_ignore = intersection - gt_ignore_roi.offset
 
         # to voxel coordinates
         intersection_in_gt //= voxel_size
         intersection_in_gt_ignore //= voxel_size
 
-        gt_ignore = np.zeros((gt_ignore_roi//voxel_size).get_shape(), dtype=np.uint8)
-        gt_ignore[intersection_in_gt_ignore.get_bounding_box()] = include_mask[intersection_in_gt.get_bounding_box()]
+        gt_ignore = np.zeros((gt_ignore_roi // voxel_size).get_shape(), dtype=np.uint8)
+        gt_ignore[intersection_in_gt_ignore.get_bounding_box()] = include_mask[
+            intersection_in_gt.get_bounding_box()
+        ]
 
         spec = self.spec[self.labels].copy()
         spec.roi = gt_ignore_roi
         spec.dtype = np.uint8
         batch.arrays[self.ignore_mask] = Array(gt_ignore, spec)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/generic_predict.py` & `gunpowder-1.3.0/gunpowder/nodes/generic_predict.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 import time
 
 from gunpowder.nodes.batch_filter import BatchFilter
 from gunpowder.producer_pool import ProducerPool, WorkersDied, NoResult
 from gunpowder.array import ArrayKey
 from gunpowder.array_spec import ArraySpec
 from gunpowder.batch_request import BatchRequest
+from queue import Full
 
 logger = logging.getLogger(__name__)
 
+
 class PredictProcessDied(Exception):
     pass
 
+
 class GenericPredict(BatchFilter):
-    '''Generic predict node to add predictions of a trained network to each each
+    """Generic predict node to add predictions of a trained network to each each
     batch that passes through. This node alone does nothing and should be
     subclassed for concrete implementations.
 
     Args:
 
         inputs (dict): Dictionary from names of input layers in the network to
             :class:``ArrayKey`` or batch attribute name as string.
@@ -32,66 +35,56 @@
             generated arrays (``outputs`` and ``gradients``). This is useful
             to set the ``voxel_size``, for example, if they differ from the
             voxel size of the input arrays. Only fields that are not ``None``
             in the given :class:`ArraySpec` will be used.
 
         spawn_subprocess (bool, optional): Whether to run ``predict`` in a
             separate process. Default is false.
-    '''
-
-    def __init__(
-            self,
-            inputs,
-            outputs,
-            array_specs=None,
-            spawn_subprocess=False):
+    """
 
+    def __init__(self, inputs, outputs, array_specs=None, spawn_subprocess=False):
         self.initialized = False
         self.inputs = inputs
         self.outputs = outputs
         self.array_specs = {} if array_specs is None else array_specs
         self.spawn_subprocess = spawn_subprocess
         self.timer_start = None
 
     def setup(self):
-
         # get common voxel size of inputs, or None if they differ
         common_voxel_size = None
         for key in self.inputs.values():
-
             if not isinstance(key, ArrayKey):
                 continue
 
             voxel_size = self.spec[key].voxel_size
 
             if common_voxel_size is None:
                 common_voxel_size = voxel_size
             elif common_voxel_size != voxel_size:
                 common_voxel_size = None
                 break
 
         # announce provided outputs
         for key in self.outputs.values():
-
             if key in self.array_specs:
                 spec = self.array_specs[key].copy()
             else:
                 spec = ArraySpec()
 
             if spec.voxel_size is None and not spec.nonspatial:
-
                 assert common_voxel_size is not None, (
                     "There is no common voxel size of the inputs, and no "
                     "ArraySpec has been given for %s that defines "
-                    "voxel_size."%key)
+                    "voxel_size." % key
+                )
 
                 spec.voxel_size = common_voxel_size
 
             if spec.interpolatable is None:
-
                 # default for predictions
                 spec.interpolatable = False
 
             self.provides(key, spec)
 
         if self.spawn_subprocess:
             # start prediction as a producer pool, so that we can gracefully
@@ -101,112 +94,103 @@
             self.batch_in_lock = multiprocessing.Lock()
             self.batch_out_lock = multiprocessing.Lock()
             self.worker.start()
 
     def teardown(self):
         if self.spawn_subprocess:
             # signal "stop"
-            self.batch_in.put((None, None))
+            try:
+                self.batch_in.put((None, None), timeout=2)
+            except Full:
+                # worker process might be stopped already
+                pass
             try:
                 self.worker.get(timeout=2)
             except NoResult:
                 pass
             self.worker.stop()
         else:
             self.stop()
 
     def prepare(self, request):
-
         if not self.initialized and not self.spawn_subprocess:
             self.start()
             self.initialized = True
 
         deps = BatchRequest()
         for key in self.inputs.values():
             deps[key] = request[key]
         return deps
 
-
     def process(self, batch, request):
-
         if self.spawn_subprocess:
-
             start = time.time()
             self.batch_in_lock.acquire()
-            logger.debug(
-                "waited for batch in lock for %.3fs", time.time() - start)
+            logger.debug("waited for batch in lock for %.3fs", time.time() - start)
             start = time.time()
             self.batch_in.put((batch, request))
-            logger.debug(
-                "queued batch for %.3fs", time.time() - start)
+            logger.debug("queued batch for %.3fs", time.time() - start)
 
             start = time.time()
             with self.batch_out_lock:
-                logger.debug(
-                    "waited for batch out lock for %.3fs", time.time() - start)
+                logger.debug("waited for batch out lock for %.3fs", time.time() - start)
 
                 start = time.time()
                 self.batch_in_lock.release()
-                logger.debug(
-                    "released batch in lock for %.3fs", time.time() - start)
+                logger.debug("released batch in lock for %.3fs", time.time() - start)
                 try:
                     start = time.time()
                     out = self.worker.get()
-                    logger.debug(
-                        "retreived batch for %.3fs", time.time() - start)
+                    logger.debug("retreived batch for %.3fs", time.time() - start)
                 except WorkersDied:
                     raise PredictProcessDied()
 
             for array_key in self.outputs.values():
                 if array_key in request:
                     batch.arrays[array_key] = out.arrays[array_key]
 
         else:
-
             self.predict(batch, request)
 
     def start(self):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         This method will be called before the first call to :fun:`predict`,
         from the same process that :fun:`predict` will be called from. Use
         this to initialize your model and hardware.
-        '''
+        """
         pass
 
     def predict(self, batch, request):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         In this method, an implementation should predict arrays on the given
         batch. Output arrays should be created according to the given request
-        and added to ``batch``.'''
-        raise NotImplementedError("Class %s does not implement 'predict'"%self.name())
+        and added to ``batch``."""
+        raise NotImplementedError("Class %s does not implement 'predict'" % self.name())
 
     def stop(self):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         This method will be called after the last call to :fun:`predict`,
         from the same process that :fun:`predict` will be called from. Use
         this to tear down your model and free training hardware.
-        '''
+        """
         pass
 
     def __produce_predict_batch(self):
-        '''Process one batch.'''
+        """Process one batch."""
 
         if not self.initialized:
-
             self.start()
             self.initialized = True
 
+        self.time_out = 0
         if self.timer_start is not None:
             self.time_out = time.time() - self.timer_start
-            logger.debug(
-                "batch in: %.3fs, predict: %.3fs, batch out: %.3fs",
-                self.time_in, self.time_predict, self.time_out)
 
         self.timer_start = time.time()
         batch, request = self.batch_in.get()
         self.time_in = time.time() - self.timer_start
 
         # stop signal
         if batch is None:
@@ -214,9 +198,15 @@
             return None
 
         self.timer_start = time.time()
         self.predict(batch, request)
         self.time_predict = time.time() - self.timer_start
         self.timer_start = time.time()
 
-        return batch
+        logger.debug(
+            "batch in: %.3fs, predict: %.3fs, batch out: %.3fs",
+            self.time_in,
+            self.time_predict,
+            self.time_out,
+        )
 
+        return batch
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/generic_train.py` & `gunpowder-1.3.0/gunpowder/nodes/generic_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from gunpowder.producer_pool import ProducerPool, WorkersDied, NoResult
 from gunpowder.array import ArrayKey
 from gunpowder.array_spec import ArraySpec
 from gunpowder.batch_request import BatchRequest
 
 logger = logging.getLogger(__name__)
 
+
 class TrainProcessDied(Exception):
     pass
 
+
 class GenericTrain(BatchFilter):
-    '''Generic train node to perform one training iteration for each batch that
+    """Generic train node to perform one training iteration for each batch that
     passes through. This node alone does nothing and should be subclassed for
     concrete implementations.
 
     Args:
 
         inputs (dict): Dictionary from names of input layers in the network to
             :class:``ArrayKey`` or batch attribute name as string.
@@ -39,70 +41,65 @@
             generated arrays (``outputs`` and ``gradients``). This is useful
             to set the ``voxel_size``, for example, if they differ from the
             voxel size of the input arrays. Only fields that are not ``None``
             in the given :class:`ArraySpec` will be used.
 
         spawn_subprocess (bool, optional): Whether to run the ``train_step`` in
             a separate process. Default is false.
-    '''
+    """
 
     def __init__(
-            self,
-            inputs,
-            outputs,
-            gradients,
-            array_specs=None,
-            spawn_subprocess=False):
-
+        self, inputs, outputs, gradients, array_specs=None, spawn_subprocess=False
+    ):
         self.initialized = False
 
         self.inputs = inputs
         self.outputs = outputs
         self.gradients = gradients
         self.array_specs = {} if array_specs is None else array_specs
         self.spawn_subprocess = spawn_subprocess
 
-        self.provided_arrays = list(self.outputs.values()) + list(self.gradients.values())
+        self.provided_arrays = list(self.outputs.values()) + list(
+            self.gradients.values()
+        )
 
     def setup(self):
-
         # get common voxel size of inputs, or None if they differ
         common_voxel_size = None
         for key in self.inputs.values():
-
             if not isinstance(key, ArrayKey):
                 continue
+            if self.spec[key].nonspatial:
+                continue
 
             voxel_size = self.spec[key].voxel_size
 
             if common_voxel_size is None:
                 common_voxel_size = voxel_size
             elif common_voxel_size != voxel_size:
                 common_voxel_size = None
                 break
 
         # announce provided outputs
         for key in self.provided_arrays:
-
             if key in self.array_specs:
                 spec = self.array_specs[key].copy()
             else:
                 spec = ArraySpec()
 
             if spec.voxel_size is None and not spec.nonspatial:
-
                 assert common_voxel_size is not None, (
                     "There is no common voxel size of the inputs, and no "
                     "ArraySpec has been given for %s that defines "
-                    "voxel_size."%key)
+                    "voxel_size." % key
+                )
 
                 spec.voxel_size = common_voxel_size
 
             if spec.interpolatable is None:
-
                 # default for predictions
                 spec.interpolatable = False
 
             self.provides(key, spec)
 
         if self.spawn_subprocess:
             # start training as a producer pool, so that we can gracefully exit if
@@ -129,19 +126,17 @@
             except NoResult:
                 pass
             self.worker.stop()
         else:
             self.stop()
 
     def process(self, batch, request):
-
         start = time.time()
 
         if self.spawn_subprocess:
-
             self.batch_in.put((batch, request))
 
             try:
                 out = self.worker.get()
             except WorkersDied:
                 raise TrainProcessDied()
 
@@ -149,77 +144,78 @@
                 if array_key in request:
                     batch.arrays[array_key] = out.arrays[array_key]
 
             batch.loss = out.loss
             batch.iteration = out.iteration
 
         else:
-
             self.train_step(batch, request)
 
         time_of_iteration = time.time() - start
 
         logger.info(
             "Train process: iteration=%d loss=%f time=%f",
-            batch.iteration, batch.loss, time_of_iteration)
+            batch.iteration,
+            batch.loss,
+            time_of_iteration,
+        )
 
     def start(self):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         This method will be called before the first call to :fun:`train_step`,
         from the same process that :fun:`train_step` will be called from. Use
         this to initialize you solver and training hardware.
-        '''
+        """
         pass
 
     def train_step(self, batch, request):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         In this method, an implementation should perform one training iteration
         on the given batch. ``batch.loss`` and ``batch.iteration`` should be
         set. Output arrays should be created according to the given request
-        and added to ``batch``.'''
-        raise NotImplementedError("Class %s does not implement 'train_step'"%self.name())
+        and added to ``batch``."""
+        raise NotImplementedError(
+            "Class %s does not implement 'train_step'" % self.name()
+        )
 
     def stop(self):
-        '''To be implemented in subclasses.
+        """To be implemented in subclasses.
 
         This method will be called after the last call to :fun:`train_step`,
         from the same process that :fun:`train_step` will be called from. Use
         this to tear down you solver and free training hardware.
-        '''
+        """
         pass
 
     def _checkpoint_name(self, basename, iteration):
-        return basename + '_checkpoint_' + '%i' % iteration
+        return basename + "_checkpoint_" + "%i" % iteration
 
     def _get_latest_checkpoint(self, basename):
-
         def atoi(text):
             return int(text) if text.isdigit() else text
 
         def natural_keys(text):
-            return [ atoi(c) for c in re.split(r'(\d+)', text) ]
+            return [atoi(c) for c in re.split(r"(\d+)", text)]
 
-        checkpoints = glob.glob(basename + '_checkpoint_*')
+        checkpoints = glob.glob(basename + "_checkpoint_*")
         checkpoints.sort(key=natural_keys)
 
         if len(checkpoints) > 0:
-
             checkpoint = checkpoints[-1]
-            iteration = int(checkpoint.split('_')[-1])
+            iteration = int(checkpoint.split("_")[-1])
             return checkpoint, iteration
 
         return None, 0
 
     def __produce_train_batch(self):
-        '''Process one train batch.'''
+        """Process one train batch."""
 
         if not self.initialized:
-
             self.start()
             self.initialized = True
 
         batch, request = self.batch_in.get()
 
         # stop signal
         if batch is None:
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/grow_boundary.py` & `gunpowder-1.3.0/gunpowder/nodes/grow_boundary.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 from scipy import ndimage
 
 from .batch_filter import BatchFilter
 from gunpowder.array import Array
 
+
 class GrowBoundary(BatchFilter):
-    '''Grow a boundary between regions in a label array. Does not grow at the
+    """Grow a boundary between regions in a label array. Does not grow at the
     border of the batch or an optionally provided mask.
 
     Args:
 
         labels (:class:`ArrayKey`):
 
             The array containing labels.
@@ -26,68 +27,78 @@
         background (``int``, optional):
 
             The label to assign to the boundary voxels.
 
         only_xy (``bool``, optional):
 
             Do not grow a boundary in the z direction.
-    '''
+    """
 
     def __init__(self, labels, mask=None, steps=1, background=0, only_xy=False):
         self.labels = labels
         self.mask = mask
         self.steps = steps
         self.background = background
         self.only_xy = only_xy
 
     def process(self, batch, request):
-
         gt = batch.arrays[self.labels]
         gt_mask = None if not self.mask else batch.arrays[self.mask]
 
         if gt_mask is not None:
-
             # grow only in area where mask and gt are defined
             crop = gt_mask.spec.roi.intersect(gt.spec.roi)
 
             if crop is None:
-                raise RuntimeError("GT_LABELS %s and GT_MASK %s ROIs don't intersect."%(gt.spec.roi,gt_mask.spec.roi))
+                raise RuntimeError(
+                    "GT_LABELS %s and GT_MASK %s ROIs don't intersect."
+                    % (gt.spec.roi, gt_mask.spec.roi)
+                )
             voxel_size = self.spec[self.labels].voxel_size
-            crop_in_gt = (crop.shift(-gt.spec.roi.get_offset())/voxel_size).get_bounding_box()
-            crop_in_gt_mask = (crop.shift(-gt_mask.spec.roi.get_offset())/voxel_size).get_bounding_box()
-
-            self.__grow(gt.data[crop_in_gt], gt_mask.data[crop_in_gt_mask], self.only_xy)
+            crop_in_gt = (
+                crop.shift(-gt.spec.roi.offset) / voxel_size
+            ).get_bounding_box()
+            crop_in_gt_mask = (
+                crop.shift(-gt_mask.spec.roi.offset) / voxel_size
+            ).get_bounding_box()
+
+            self.__grow(
+                gt.data[crop_in_gt], gt_mask.data[crop_in_gt_mask], self.only_xy
+            )
 
         else:
-
             self.__grow(gt.data, only_xy=self.only_xy)
 
     def __grow(self, gt, gt_mask=None, only_xy=False):
         if gt_mask is not None:
-            assert gt.shape == gt_mask.shape, "GT_LABELS and GT_MASK do not have the same size."
+            assert (
+                gt.shape == gt_mask.shape
+            ), "GT_LABELS and GT_MASK do not have the same size."
 
         if only_xy:
             assert len(gt.shape) == 3
             for z in range(gt.shape[0]):
                 self.__grow(gt[z], None if gt_mask is None else gt_mask[z])
             return
 
         # get all foreground voxels by erosion of each component
-        foreground = np.zeros(shape=gt.shape, dtype=np.bool)
+        foreground = np.zeros(shape=gt.shape, dtype=bool)
         masked = None
         if gt_mask is not None:
             masked = np.equal(gt_mask, 0)
         for label in np.unique(gt):
             if label == self.background:
                 continue
-            label_mask = gt==label
+            label_mask = gt == label
             # Assume that masked out values are the same as the label we are
             # eroding in this iteration. This ensures that at the boundary to
             # a masked region the value blob is not shrinking.
             if masked is not None:
                 label_mask = np.logical_or(label_mask, masked)
-            eroded_label_mask = ndimage.binary_erosion(label_mask, iterations=self.steps, border_value=1)
+            eroded_label_mask = ndimage.binary_erosion(
+                label_mask, iterations=self.steps, border_value=1
+            )
             foreground = np.logical_or(eroded_label_mask, foreground)
 
         # label new background
         background = np.logical_not(foreground)
         gt[background] = self.background
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/hdf5_source.py` & `gunpowder-1.3.0/gunpowder/nodes/hdf5_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from gunpowder.ext import h5py
 from .hdf5like_source_base import Hdf5LikeSource
 
+
 class Hdf5Source(Hdf5LikeSource):
-    '''An HDF5 data source.
+    """An HDF5 data source.
 
     Provides arrays from HDF5 datasets. If the attribute ``resolution`` is set
     in a HDF5 dataset, it will be used as the array's ``voxel_size``. If the
     attribute ``offset`` is set in a dataset, it will be used as the offset of
     the :class:`Roi` for this array. It is assumed that the offset is given in
     world units.
 
@@ -30,10 +31,11 @@
         channels_first (``bool``, optional):
 
             Specifies the ordering of the dimensions of the HDF5-like data source.
             If channels_first is set (default), then the input shape is expected
             to be (channels, spatial dimensions). This is recommended because of
             better performance. If channels_first is set to false, then the input
             data is read in channels_last manner and converted to channels_first.
-    '''
+    """
+
     def _open_file(self, filename):
-        return h5py.File(filename, 'r')
+        return h5py.File(filename, "r")
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/hdf5_write.py` & `gunpowder-1.3.0/gunpowder/nodes/hdf5_write.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .hdf5like_write_base import Hdf5LikeWrite
 from gunpowder.ext import h5py
 import os
 
+
 class Hdf5Write(Hdf5LikeWrite):
-    '''Assemble arrays of passing batches in one HDF5 file. This is useful to
+    """Assemble arrays of passing batches in one HDF5 file. This is useful to
     store chunks produced by :class:`Scan` on disk without keeping the larger
     array in memory. The ROIs of the passing arrays will be used to determine
     the position where to store the data in the dataset.
 
     Args:
 
         dataset_names (``dict``, :class:`ArrayKey` -> ``string``):
@@ -32,14 +33,14 @@
             compression level.
 
         dataset_dtypes (``dict``, :class:`ArrayKey` -> data type):
 
             A dictionary from array keys to datatype (eg. ``np.int8``). If
             given, arrays are stored using this type. The original arrays
             within the pipeline remain unchanged.
-        '''
+    """
 
     def _open_file(self, filename):
         if os.path.exists(filename):
-            return h5py.File(filename, 'r+')
+            return h5py.File(filename, "r+")
         else:
-            return h5py.File(filename, 'w')
+            return h5py.File(filename, "w")
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/hdf5like_source_base.py` & `gunpowder-1.3.0/gunpowder/nodes/hdf5like_source_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import logging
-import numpy as np
-
 from gunpowder.batch import Batch
 from gunpowder.coordinate import Coordinate
 from gunpowder.profiling import Timing
 from gunpowder.roi import Roi
 from gunpowder.array import Array
 from gunpowder.array_spec import ArraySpec
 from .batch_provider import BatchProvider
 
+import logging
+import numpy as np
+import warnings
+
 logger = logging.getLogger(__name__)
 
 
 class Hdf5LikeSource(BatchProvider):
-    '''An HDF5-like data source.
+    """An HDF5-like data source.
 
     Provides arrays from datasets accessed with an h5py-like API for each array
     key given. If the attribute ``resolution`` is set in a dataset, it will be
     used as the array's ``voxel_size``. If the attribute ``offset`` is set in a
     dataset, it will be used as the offset of the :class:`Roi` for this array.
     It is assumed that the offset is given in world units.
 
@@ -41,21 +42,21 @@
         channels_first (``bool``, optional):
 
             Specifies the ordering of the dimensions of the HDF5-like data source.
             If channels_first is set (default), then the input shape is expected
             to be (channels, spatial dimensions). This is recommended due to
             better performance. If channels_first is set to false, then the input
             data is read in channels_last manner and converted to channels_first.
-    '''
-    def __init__(
-            self,
-            filename,
-            datasets,
-            array_specs=None,
-            channels_first=True):
+    """
+
+    def __init__(self, filename, datasets, array_specs=None, channels_first=True):
+        warnings.warn(
+            "HDF5LikeSource is depricated and will soon be removed in v2.0",
+            DeprecationWarning,
+        )
 
         self.filename = filename
         self.datasets = datasets
 
         if array_specs is None:
             self.array_specs = {}
         else:
@@ -63,140 +64,146 @@
 
         self.channels_first = channels_first
 
         # number of spatial dimensions
         self.ndims = None
 
     def _open_file(self, filename):
-        raise NotImplementedError('Only implemented in subclasses')
+        raise NotImplementedError("Only implemented in subclasses")
 
     def setup(self):
         with self._open_file(self.filename) as data_file:
-            for (array_key, ds_name) in self.datasets.items():
-
+            for array_key, ds_name in self.datasets.items():
                 if ds_name not in data_file:
                     raise RuntimeError("%s not in %s" % (ds_name, self.filename))
 
                 spec = self.__read_spec(array_key, data_file, ds_name)
 
                 self.provides(array_key, spec)
 
     def provide(self, request):
-
         timing = Timing(self)
         timing.start()
 
         batch = Batch()
 
         with self._open_file(self.filename) as data_file:
-            for (array_key, request_spec) in request.array_specs.items():
+            for array_key, request_spec in request.array_specs.items():
                 logger.debug("Reading %s in %s...", array_key, request_spec.roi)
 
                 voxel_size = self.spec[array_key].voxel_size
 
                 # scale request roi to voxel units
                 dataset_roi = request_spec.roi / voxel_size
 
                 # shift request roi into dataset
-                dataset_roi = dataset_roi - self.spec[array_key].roi.get_offset() / voxel_size
+                dataset_roi = dataset_roi - self.spec[array_key].roi.offset / voxel_size
 
                 # create array spec
                 array_spec = self.spec[array_key].copy()
                 array_spec.roi = request_spec.roi
 
                 # add array to batch
                 batch.arrays[array_key] = Array(
                     self.__read(data_file, self.datasets[array_key], dataset_roi),
-                    array_spec)
+                    array_spec,
+                )
 
         logger.debug("done")
 
         timing.stop()
         batch.profiling_stats.add(timing)
 
         return batch
 
     def _get_voxel_size(self, dataset):
         try:
-            return Coordinate(dataset.attrs['resolution'])
+            return Coordinate(dataset.attrs["resolution"])
         except Exception:  # todo: make specific when z5py supports it
             return None
 
     def _get_offset(self, dataset):
         try:
-            return Coordinate(dataset.attrs['offset'])
+            return Coordinate(dataset.attrs["offset"])
         except Exception:  # todo: make specific when z5py supports it
             return None
 
     def __read_spec(self, array_key, data_file, ds_name):
-
         dataset = data_file[ds_name]
 
         if array_key in self.array_specs:
             spec = self.array_specs[array_key].copy()
         else:
             spec = ArraySpec()
 
         if spec.voxel_size is None:
             voxel_size = self._get_voxel_size(dataset)
             if voxel_size is None:
-                voxel_size = Coordinate((1,)*len(dataset.shape))
-                logger.warning("WARNING: File %s does not contain resolution information "
-                               "for %s (dataset %s), voxel size has been set to %s. This "
-                               "might not be what you want.",
-                               self.filename, array_key, ds_name, spec.voxel_size)
+                voxel_size = Coordinate((1,) * len(dataset.shape))
+                logger.warning(
+                    "WARNING: File %s does not contain resolution information "
+                    "for %s (dataset %s), voxel size has been set to %s. This "
+                    "might not be what you want.",
+                    self.filename,
+                    array_key,
+                    ds_name,
+                    spec.voxel_size,
+                )
             spec.voxel_size = voxel_size
 
         self.ndims = len(spec.voxel_size)
 
         if spec.roi is None:
             offset = self._get_offset(dataset)
             if offset is None:
-                offset = Coordinate((0,)*self.ndims)
+                offset = Coordinate((0,) * self.ndims)
 
             if self.channels_first:
-                shape = Coordinate(dataset.shape[-self.ndims:])
+                shape = Coordinate(dataset.shape[-self.ndims :])
             else:
-                shape = Coordinate(dataset.shape[:self.ndims])
+                shape = Coordinate(dataset.shape[: self.ndims])
 
-            spec.roi = Roi(offset, shape*spec.voxel_size)
+            spec.roi = Roi(offset, shape * spec.voxel_size)
 
         if spec.dtype is not None:
-            assert spec.dtype == dataset.dtype, ("dtype %s provided in array_specs for %s, "
-                                                 "but differs from dataset %s dtype %s" %
-                                                 (self.array_specs[array_key].dtype,
-                                                  array_key, ds_name, dataset.dtype))
+            assert spec.dtype == dataset.dtype, (
+                "dtype %s provided in array_specs for %s, "
+                "but differs from dataset %s dtype %s"
+                % (self.array_specs[array_key].dtype, array_key, ds_name, dataset.dtype)
+            )
         else:
             spec.dtype = dataset.dtype
 
         if spec.interpolatable is None:
             spec.interpolatable = spec.dtype in [
-                np.float,
                 np.float32,
                 np.float64,
                 np.float128,
-                np.uint8  # assuming this is not used for labels
+                np.uint8,  # assuming this is not used for labels
             ]
-            logger.warning("WARNING: You didn't set 'interpolatable' for %s "
-                           "(dataset %s). Based on the dtype %s, it has been "
-                           "set to %s. This might not be what you want.",
-                           array_key, ds_name, spec.dtype,
-                           spec.interpolatable)
+            logger.warning(
+                "WARNING: You didn't set 'interpolatable' for %s "
+                "(dataset %s). Based on the dtype %s, it has been "
+                "set to %s. This might not be what you want.",
+                array_key,
+                ds_name,
+                spec.dtype,
+                spec.interpolatable,
+            )
 
         return spec
 
     def __read(self, data_file, ds_name, roi):
-
         c = len(data_file[ds_name].shape) - self.ndims
 
         if self.channels_first:
             array = np.asarray(data_file[ds_name][(slice(None),) * c + roi.to_slices()])
         else:
             array = np.asarray(data_file[ds_name][roi.to_slices() + (slice(None),) * c])
-            array = np.transpose(array,
-                                 axes=[i + self.ndims for i in range(c)] + list(range(self.ndims)))
+            array = np.transpose(
+                array, axes=[i + self.ndims for i in range(c)] + list(range(self.ndims))
+            )
 
         return array
 
     def name(self):
-
         return super().name() + f"[{self.filename}]"
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/hdf5like_write_base.py` & `gunpowder-1.3.0/gunpowder/nodes/hdf5like_write_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from .batch_filter import BatchFilter
 from gunpowder.batch_request import BatchRequest
 from gunpowder.coordinate import Coordinate
 from gunpowder.roi import Roi
 import logging
 import os
+import warnings
 
 logger = logging.getLogger(__name__)
 
+
 class Hdf5LikeWrite(BatchFilter):
-    '''Assemble arrays of passing batches in one HDF5-like container. This is
+    """Assemble arrays of passing batches in one HDF5-like container. This is
     useful to store chunks produced by :class:`Scan` on disk without keeping
     the larger array in memory. The ROIs of the passing arrays will be used to
     determine the position where to store the data in the dataset.
 
     Args:
 
         dataset_names (``dict``, :class:`ArrayKey` -> ``string``):
@@ -37,23 +39,28 @@
             compression level.
 
         dataset_dtypes (``dict``, :class:`ArrayKey` -> data type):
 
             A dictionary from array keys to datatype (eg. ``np.int8``). If
             given, arrays are stored using this type. The original arrays
             within the pipeline remain unchanged.
-        '''
+    """
 
     def __init__(
-            self,
-            dataset_names,
-            output_dir='.',
-            output_filename='output.hdf',
-            compression_type=None,
-            dataset_dtypes=None):
+        self,
+        dataset_names,
+        output_dir=".",
+        output_filename="output.hdf",
+        compression_type=None,
+        dataset_dtypes=None,
+    ):
+        warnings.warn(
+            "HDF5LikeWrite is depricated and will soon be removed in v2.0",
+            DeprecationWarning,
+        )
 
         self.dataset_names = dataset_names
         self.output_dir = output_dir
         self.output_filename = output_filename
         self.compression_type = compression_type
         if dataset_dtypes is None:
             self.dataset_dtypes = {}
@@ -70,142 +77,147 @@
     def prepare(self, request):
         deps = BatchRequest()
         for key in self.dataset_names.keys():
             deps[key] = request[key]
         return deps
 
     def _open_file(self, filename):
-        raise NotImplementedError('Only implemented in subclasses')
+        raise NotImplementedError("Only implemented in subclasses")
 
     def _get_voxel_size(self, dataset):
-        return Coordinate(dataset.attrs['resolution'])
+        return Coordinate(dataset.attrs["resolution"])
 
     def _get_offset(self, dataset):
-        return Coordinate(dataset.attrs['offset'])
+        return Coordinate(dataset.attrs["offset"])
 
     def _set_voxel_size(self, dataset, voxel_size):
-        dataset.attrs['resolution'] = voxel_size
+        dataset.attrs["resolution"] = voxel_size
 
     def _set_offset(self, dataset, offset):
-        dataset.attrs['offset'] = offset
+        dataset.attrs["offset"] = offset
 
     def init_datasets(self, batch):
-
         filename = os.path.join(self.output_dir, self.output_filename)
         logger.debug("Initializing container %s", filename)
 
         try:
             os.makedirs(self.output_dir)
         except:
             pass
 
-        for (array_key, dataset_name) in self.dataset_names.items():
-
+        for array_key, dataset_name in self.dataset_names.items():
             logger.debug("Initializing dataset for %s", array_key)
 
             assert array_key in self.spec, (
-                "Asked to store %s, but is not provided upstream."%array_key)
+                "Asked to store %s, but is not provided upstream." % array_key
+            )
             assert array_key in batch.arrays, (
-                "Asked to store %s, but is not part of batch."%array_key)
+                "Asked to store %s, but is not part of batch." % array_key
+            )
 
             array = batch.arrays[array_key]
-            dims = array.spec.roi.dims()
+            dims = array.spec.roi.dims
             batch_shape = array.data.shape
 
             with self._open_file(filename) as data_file:
-
                 # if a dataset already exists, read its meta-information (if
                 # present)
                 if dataset_name in data_file:
-
-                    offset = self._get_offset(data_file[dataset_name]) or Coordinate((0,)*dims)
+                    offset = self._get_offset(data_file[dataset_name]) or Coordinate(
+                        (0,) * dims
+                    )
 
                 else:
-
                     provided_roi = self.spec[array_key].roi
 
                     if provided_roi is None:
                         raise RuntimeError(
                             "Dataset %s does not exist in %s, and no ROI is "
                             "provided for %s. I don't know how to initialize "
-                            "the dataset."%(dataset_name, filename, array_key))
+                            "the dataset." % (dataset_name, filename, array_key)
+                        )
 
-                    offset = provided_roi.get_offset()
+                    offset = provided_roi.offset
                     voxel_size = array.spec.voxel_size
-                    data_shape = provided_roi.get_shape()//voxel_size
+                    data_shape = provided_roi.shape // voxel_size
 
                     logger.debug("Shape in voxels: %s", data_shape)
                     # add channel dimensions (if present)
                     data_shape = batch_shape[:-dims] + data_shape
                     logger.debug("Shape with channel dimensions: %s", data_shape)
 
                     if array_key in self.dataset_dtypes:
                         dtype = self.dataset_dtypes[array_key]
                     else:
                         dtype = batch.arrays[array_key].data.dtype
 
                     logger.debug(
                         "create_dataset: %s, %s, %s, %s, offset=%s, resolution=%s",
-                        dataset_name, data_shape, self.compression_type, dtype,
-                        offset, voxel_size)
+                        dataset_name,
+                        data_shape,
+                        self.compression_type,
+                        dtype,
+                        offset,
+                        voxel_size,
+                    )
 
                     dataset = data_file.create_dataset(
-                            name=dataset_name,
-                            shape=data_shape,
-                            compression=self.compression_type,
-                            dtype=dtype)
+                        name=dataset_name,
+                        shape=data_shape,
+                        compression=self.compression_type,
+                        dtype=dtype,
+                    )
 
                     self._set_offset(dataset, offset)
                     self._set_voxel_size(dataset, voxel_size)
 
                 logger.debug(
                     "%s (%s in %s) has offset %s",
                     array_key,
                     dataset_name,
                     filename,
-                    offset)
+                    offset,
+                )
                 self.dataset_offsets[array_key] = offset
 
     def process(self, batch, request):
-
         filename = os.path.join(self.output_dir, self.output_filename)
 
         if not self.dataset_offsets:
             self.init_datasets(batch)
 
         with self._open_file(filename) as data_file:
-
-            for (array_key, dataset_name) in self.dataset_names.items():
-
+            for array_key, dataset_name in self.dataset_names.items():
                 dataset = data_file[dataset_name]
 
                 array_roi = batch.arrays[array_key].spec.roi
                 voxel_size = self.spec[array_key].voxel_size
-                dims = array_roi.dims()
-                channel_slices = (slice(None),)*max(0, len(dataset.shape) - dims)
+                dims = array_roi.dims
+                channel_slices = (slice(None),) * max(0, len(dataset.shape) - dims)
 
                 dataset_roi = Roi(
                     self.dataset_offsets[array_key],
-                    Coordinate(dataset.shape[-dims:])*voxel_size)
+                    Coordinate(dataset.shape[-dims:]) * voxel_size,
+                )
                 common_roi = array_roi.intersect(dataset_roi)
 
-                if common_roi.empty():
+                if common_roi.empty:
                     logger.warn(
                         "array %s with ROI %s lies outside of dataset ROI %s, "
-                        "skipping writing"%(
-                            array_key,
-                            array_roi,
-                            dataset_roi))
+                        "skipping writing" % (array_key, array_roi, dataset_roi)
+                    )
                     continue
 
-                dataset_voxel_roi = (common_roi - self.dataset_offsets[array_key])//voxel_size
+                dataset_voxel_roi = (
+                    common_roi - self.dataset_offsets[array_key]
+                ) // voxel_size
                 dataset_voxel_slices = dataset_voxel_roi.to_slices()
-                array_voxel_roi = (common_roi - array_roi.get_offset())//voxel_size
+                array_voxel_roi = (common_roi - array_roi.offset) // voxel_size
                 array_voxel_slices = array_voxel_roi.to_slices()
 
                 logger.debug(
-                    "writing %s to voxel coordinates %s"%(
-                        array_key,
-                        dataset_voxel_roi))
+                    "writing %s to voxel coordinates %s"
+                    % (array_key, dataset_voxel_roi)
+                )
 
                 data = batch.arrays[array_key].data[channel_slices + array_voxel_slices]
                 dataset[channel_slices + dataset_voxel_slices] = data
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/intensity_augment.py` & `gunpowder-1.3.0/gunpowder/nodes/intensity_augment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 
 from gunpowder.batch_request import BatchRequest
 
 from .batch_filter import BatchFilter
 
+
 class IntensityAugment(BatchFilter):
-    '''Randomly scale and shift the values of an intensity array.
+    """Randomly scale and shift the values of an intensity array.
 
     Args:
 
         array (:class:`ArrayKey`):
 
             The intensity array to modify.
 
@@ -29,17 +30,26 @@
             Perform the augmentation z-section wise. Requires 3D arrays and
             assumes that z is the first dimension.
 
         clip (``bool``):
 
             Set to False if modified values should not be clipped to [0, 1]
             Disables range check!
-    '''
+    """
 
-    def __init__(self, array, scale_min, scale_max, shift_min, shift_max, z_section_wise=False, clip=True):
+    def __init__(
+        self,
+        array,
+        scale_min,
+        scale_max,
+        shift_min,
+        shift_max,
+        z_section_wise=False,
+        clip=True,
+    ):
         self.array = array
         self.scale_min = scale_min
         self.scale_max = scale_max
         self.shift_min = shift_min
         self.shift_max = shift_max
         self.z_section_wise = z_section_wise
         self.clip = clip
@@ -53,35 +63,43 @@
         # TODO: write a test for this node
         np.random.seed(request.random_seed)
         deps = BatchRequest()
         deps[self.array] = request[self.array].copy()
         return deps
 
     def process(self, batch, request):
-
         raw = batch.arrays[self.array]
 
-        assert not self.z_section_wise or raw.spec.roi.dims() == 3, "If you specify 'z_section_wise', I expect 3D data."
-        assert raw.data.dtype == np.float32 or raw.data.dtype == np.float64, "Intensity augmentation requires float types for the raw array (not " + str(raw.data.dtype) + "). Consider using Normalize before."
+        assert (
+            not self.z_section_wise or raw.spec.roi.dims == 3
+        ), "If you specify 'z_section_wise', I expect 3D data."
+        assert raw.data.dtype == np.float32 or raw.data.dtype == np.float64, (
+            "Intensity augmentation requires float types for the raw array (not "
+            + str(raw.data.dtype)
+            + "). Consider using Normalize before."
+        )
         if self.clip:
-            assert raw.data.min() >= 0 and raw.data.max() <= 1, "Intensity augmentation expects raw values in [0,1]. Consider using Normalize before."
+            assert (
+                raw.data.min() >= 0 and raw.data.max() <= 1
+            ), "Intensity augmentation expects raw values in [0,1]. Consider using Normalize before."
 
         if self.z_section_wise:
-            for z in range((raw.spec.roi/self.spec[self.array].voxel_size).get_shape()[0]):
+            for z in range((raw.spec.roi / self.spec[self.array].voxel_size).shape[0]):
                 raw.data[z] = self.__augment(
-                        raw.data[z],
-                        np.random.uniform(low=self.scale_min, high=self.scale_max),
-                        np.random.uniform(low=self.shift_min, high=self.shift_max))
+                    raw.data[z],
+                    np.random.uniform(low=self.scale_min, high=self.scale_max),
+                    np.random.uniform(low=self.shift_min, high=self.shift_max),
+                )
         else:
             raw.data = self.__augment(
-                    raw.data,
-                    np.random.uniform(low=self.scale_min, high=self.scale_max),
-                    np.random.uniform(low=self.shift_min, high=self.shift_max))
+                raw.data,
+                np.random.uniform(low=self.scale_min, high=self.scale_max),
+                np.random.uniform(low=self.shift_min, high=self.shift_max),
+            )
 
         # clip values, we might have pushed them out of [0,1]
         if self.clip:
-            raw.data[raw.data>1] = 1
-            raw.data[raw.data<0] = 0
+            raw.data[raw.data > 1] = 1
+            raw.data[raw.data < 0] = 0
 
     def __augment(self, a, scale, shift):
-
-        return a.mean() + (a-a.mean())*scale + shift
+        return a.mean() + (a - a.mean()) * scale + shift
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/intensity_scale_shift.py` & `gunpowder-1.3.0/gunpowder/nodes/intensity_scale_shift.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from .batch_filter import BatchFilter
 
+
 class IntensityScaleShift(BatchFilter):
-    '''Scales the intensities of a batch by ``scale``, then adds ``shift``.
+    """Scales the intensities of a batch by ``scale``, then adds ``shift``.
 
     Args:
 
         array (:class:`ArrayKey`):
 
             The key of the array to modify.
 
         scale (``float``):
         shift (``float``):
 
             The shift and scale to apply to ``array``.
-    '''
+    """
 
     def __init__(self, array, scale, shift):
         self.array = array
         self.scale = scale
         self.shift = shift
 
     def process(self, batch, request):
-
         if self.array not in batch.arrays:
             return
 
         raw = batch.arrays[self.array]
-        raw.data = raw.data*self.scale + self.shift
+        raw.data = raw.data * self.scale + self.shift
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/klb_source.py` & `gunpowder-1.3.0/gunpowder/nodes/klb_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from gunpowder.roi import Roi
 from gunpowder.array import Array
 from gunpowder.array_spec import ArraySpec
 from .batch_provider import BatchProvider
 
 logger = logging.getLogger(__name__)
 
+
 class KlbSource(BatchProvider):
-    '''A `KLB <https://bitbucket.org/fernandoamat/keller-lab-block-filetype>`_
+    """A `KLB <https://bitbucket.org/fernandoamat/keller-lab-block-filetype>`_
     data source.
 
     Provides a single array from the given KLB dataset.
 
     Args:
 
         filename (``string``):
@@ -46,92 +47,83 @@
 
             An optional integer to pass to pyklb reader indicating the number
             of threads to use when reading klb files. Entering None causes
             uses the pyklb default, which now is based on the number of cores
             in the machine. This pyklb default is bad for jobs on the cluster that
             are limited to the number of cores requested, and 1 is recommended.
 
-    '''
-
-    def __init__(
-            self,
-            filename,
-            array,
-            array_spec=None,
-            num_threads=1):
+    """
 
+    def __init__(self, filename, array, array_spec=None, num_threads=1):
         self.filename = filename
         self.array = array
         self.array_spec = array_spec
         self.num_threads = num_threads
 
         self.files = None
         self.ndims = None
 
     def setup(self):
-
         self.files = glob.glob(self.filename)
         self.files.sort()
 
         logger.info("Reading KLB headers of %d files...", len(self.files))
-        headers = [ pyklb.readheader(f) for f in self.files ]
+        headers = [pyklb.readheader(f) for f in self.files]
         spec = self.__read_spec(headers)
 
         self.provides(self.array, spec)
 
     def provide(self, request):
-
         timing = Timing(self)
         timing.start()
 
         batch = Batch()
 
         request_spec = request[self.array]
 
         logger.debug("Reading %s in %s...", self.array, request_spec.roi)
 
         voxel_size = self.spec[self.array].voxel_size
 
         # scale request roi to voxel units
-        dataset_roi = request_spec.roi/voxel_size
+        dataset_roi = request_spec.roi / voxel_size
 
         # shift request roi into dataset
-        dataset_roi = dataset_roi - self.spec[self.array].roi.get_offset()/voxel_size
+        dataset_roi = dataset_roi - self.spec[self.array].roi.offset / voxel_size
 
         # create array spec
         array_spec = self.spec[self.array].copy()
         array_spec.roi = request_spec.roi
 
         # add array to batch
-        batch.arrays[self.array] = Array(
-            self.__read(dataset_roi),
-            array_spec)
+        batch.arrays[self.array] = Array(self.__read(dataset_roi), array_spec)
 
         logger.debug("done")
 
         timing.stop()
         batch.profiling_stats.add(timing)
 
         return batch
 
     def __read_spec(self, headers):
-
         num_files = len(headers)
         assert num_files > 0
         common_header = headers[0]
         for header in headers:
-            for attr in ['imagesize_tczyx', 'pixelspacing_tczyx']:
+            for attr in ["imagesize_tczyx", "pixelspacing_tczyx"]:
                 assert (common_header[attr] == header[attr]).all(), (
-                    "Headers of provided KLB files differ in attribute %s"%attr)
-            assert common_header['datatype'] == header['datatype'], (
-                "Headers of provided KLB files differ in attribute datatype")
-
-        size = Coordinate(common_header['imagesize_tczyx'])
-        voxel_size = Coordinate(common_header['pixelspacing_tczyx'])
-        dtype = common_header['datatype']
+                    "Headers of provided KLB files differ in attribute %s" % attr
+                )
+            assert (
+                common_header["datatype"] == header["datatype"]
+            ), "Headers of provided KLB files differ in attribute datatype"
+
+        size = Coordinate(common_header["imagesize_tczyx"])
+        voxel_size = Coordinate(common_header["pixelspacing_tczyx"])
+        dtype = common_header["datatype"]
 
         # strip leading 1 dimensions
         while size[0] == 1 and len(size) > 1:
             size = size[1:]
             voxel_size = voxel_size[1:]
 
         # append num_files dimension
@@ -147,75 +139,65 @@
         else:
             spec = ArraySpec()
 
         if spec.voxel_size is None:
             spec.voxel_size = Coordinate(voxel_size)
 
         if spec.roi is None:
-            offset = Coordinate((0,)*self.ndims)
-            spec.roi = Roi(offset, dims*spec.voxel_size)
+            offset = Coordinate((0,) * self.ndims)
+            spec.roi = Roi(offset, dims * spec.voxel_size)
 
         if spec.dtype is not None:
             assert spec.dtype == dtype, (
                 "dtype %s provided in array_specs for %s, but differs from "
-                "dataset dtype %s"%(
-                    self.array_specs[self.array].dtype, self.array,
-                    dataset.dtype))
+                "dataset dtype %s"
+                % (self.array_specs[self.array].dtype, self.array, dataset.dtype)
+            )
         else:
             spec.dtype = dtype
 
         if spec.interpolatable is None:
-
             spec.interpolatable = spec.dtype in [
-                np.float,
                 np.float32,
                 np.float64,
                 np.float128,
-                np.uint8 # assuming this is not used for labels
+                np.uint8,  # assuming this is not used for labels
             ]
-            logger.warning("WARNING: You didn't set 'interpolatable' for %s. "
-                           "Based on the dtype %s, it has been set to %s. "
-                           "This might not be what you want.",
-                           self.array, spec.dtype, spec.interpolatable)
+            logger.warning(
+                "WARNING: You didn't set 'interpolatable' for %s. "
+                "Based on the dtype %s, it has been set to %s. "
+                "This might not be what you want.",
+                self.array,
+                spec.dtype,
+                spec.interpolatable,
+            )
 
         return spec
 
     def __read(self, roi):
-
         if len(self.files) == 1:
-
             return self.__read_file(self.files[0], roi)
 
         else:
+            file_indices = range(roi.begin[0], roi.end[0])
 
-            file_indices = range(
-                roi.get_begin()[0],
-                roi.get_end()[0])
-
-            file_roi = Roi(
-                roi.get_begin()[1:],
-                roi.get_shape()[1:])
-
-            return np.array([
-                    self.__read_file(self.files[i], file_roi)
-                    for i in file_indices
-                ])
+            file_roi = Roi(roi.begin[1:], roi.shape[1:])
 
-    def __read_file(self, filename, roi):
+            return np.array(
+                [self.__read_file(self.files[i], file_roi) for i in file_indices]
+            )
 
+    def __read_file(self, filename, roi):
         # pyklb reads max-inclusive, gunpowder rois are max exclusive ->
         # subtract (1, 1, ...) from max coordinate
         if self.num_threads:
             return pyklb.readroi(
                 filename,
-                roi.get_begin(),
-                roi.get_end() - (1,)*roi.dims(),
-                numthreads=self.num_threads)
+                roi.begin,
+                roi.end - (1,) * roi.dims,
+                numthreads=self.num_threads,
+            )
         else:
-            return pyklb.readroi(
-                filename,
-                roi.get_begin(),
-                roi.get_end() - (1,)*roi.dims())
+            return pyklb.readroi(filename, roi.begin, roi.end - (1,) * roi.dims)
 
     def __repr__(self):
-
         return self.filename
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/merge_provider.py` & `gunpowder-1.3.0/gunpowder/nodes/merge_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,61 +4,63 @@
 
 from .batch_provider import BatchProvider
 
 import random
 
 
 class MergeProvider(BatchProvider):
-    '''Merges different providers::
+    """Merges different providers::
 
-        (a + b + c) + MergeProvider()
+        (a, b, c) + MergeProvider()
 
     will create a provider that combines the arrays and points offered by
     ``a``, ``b``, and ``c``. Array and point keys of ``a``, ``b``, and ``c`` should be
     the disjoint.
-    '''
+    """
+
     def __init__(self):
         self.key_to_provider = {}
 
     def setup(self):
         self.enable_placeholders()
-        assert len(self.get_upstream_providers()) > 0, "at least one batch provider needs to be added to the MergeProvider"
+        assert (
+            len(self.get_upstream_providers()) > 0
+        ), "at least one batch provider needs to be added to the MergeProvider"
         # Only allow merging if no two upstream_providers have the same
         # array/points keys
-        error_message = "Key {} provided by more than one upstream provider. Node MergeProvider only allows to merge " \
-                        "providers with different keys."
+        error_message = (
+            "Key {} provided by more than one upstream provider. Node MergeProvider only allows to merge "
+            "providers with different keys."
+        )
         for provider in self.get_upstream_providers():
             for key, spec in provider.spec.items():
-                assert self.spec is None or key not in self.spec, error_message.format(key)
+                assert self.spec is None or key not in self.spec, error_message.format(
+                    key
+                )
                 self.provides(key, spec)
                 self.key_to_provider[key] = provider
 
     def provide(self, request):
-
         # create upstream requests
         upstream_requests = {}
         for key, spec in request.items():
-
             provider = self.key_to_provider[key]
             if provider not in upstream_requests:
                 # use new random seeds per upstream request.
                 # seeds picked by random should be deterministic since
                 # the provided request already has a random seed.
                 seed = random.randint(0, 2**32)
                 upstream_requests[provider] = BatchRequest(random_seed=seed)
 
             upstream_requests[provider][key] = spec
 
         # execute requests, merge batches
         merged_batch = Batch()
         for provider, upstream_request in upstream_requests.items():
-
             batch = provider.request_batch(upstream_request)
             for key, array in batch.arrays.items():
                 merged_batch.arrays[key] = array
             for key, graph in batch.graphs.items():
                 merged_batch.graphs[key] = graph
             merged_batch.profiling_stats.merge_with(batch.profiling_stats)
 
         return merged_batch
-
-
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/noise_augment.py` & `gunpowder-1.3.0/gunpowder/nodes/noise_augment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import skimage
 
 from gunpowder.batch_request import BatchRequest
 
 from .batch_filter import BatchFilter
 
+
 class NoiseAugment(BatchFilter):
-    '''Add random noise to an array. Uses the scikit-image function skimage.util.random_noise.
+    """Add random noise to an array. Uses the scikit-image function skimage.util.random_noise.
     See scikit-image documentation for more information on arguments and additional kwargs.
 
     Args:
 
         array (:class:`ArrayKey`):
 
             The intensity array to modify. Should be of type float and within range [-1, 1] or [0, 1].
@@ -23,17 +24,17 @@
 
             Optionally set a random seed, see scikit-image documentation.
 
         clip (``bool``):
 
             Whether to preserve the image range (either [-1, 1] or [0, 1]) by clipping values in the end, see
             scikit-image documentation
-    '''
+    """
 
-    def __init__(self, array, mode='gaussian', seed=None, clip=True, **kwargs):
+    def __init__(self, array, mode="gaussian", seed=None, clip=True, **kwargs):
         self.array = array
         self.mode = mode
         self.seed = seed
         self.clip = clip
         self.kwargs = kwargs
 
     def setup(self):
@@ -42,18 +43,21 @@
 
     def prepare(self, request):
         deps = BatchRequest()
         deps[self.array] = request[self.array].copy()
         return deps
 
     def process(self, batch, request):
-
         raw = batch.arrays[self.array]
 
-        assert raw.data.dtype == np.float32 or raw.data.dtype == np.float64, "Noise augmentation requires float types for the raw array (not " + str(raw.data.dtype) + "). Consider using Normalize before."
-        assert raw.data.min() >= -1 and raw.data.max() <= 1, "Noise augmentation expects raw values in [-1,1] or [0,1]. Consider using Normalize before."
+        assert raw.data.dtype == np.float32 or raw.data.dtype == np.float64, (
+            "Noise augmentation requires float types for the raw array (not "
+            + str(raw.data.dtype)
+            + "). Consider using Normalize before."
+        )
+        if self.clip:
+            assert (
+                raw.data.min() >= -1 and raw.data.max() <= 1
+            ), "Noise augmentation expects raw values in [-1,1] or [0,1]. Consider using Normalize before."
         raw.data = skimage.util.random_noise(
-            raw.data,
-            mode=self.mode,
-            seed=self.seed,
-            clip=self.clip,
-            **self.kwargs).astype(raw.data.dtype)
+            raw.data, mode=self.mode, seed=self.seed, clip=self.clip, **self.kwargs
+        ).astype(raw.data.dtype)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/normalize.py` & `gunpowder-1.3.0/gunpowder/nodes/normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 from gunpowder.batch_request import BatchRequest
 
 from .batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
+
 class Normalize(BatchFilter):
-    '''Normalize the values of an array to be floats between 0 and 1, based on
+    """Normalize the values of an array to be floats between 0 and 1, based on
     the type of the array.
 
     Args:
 
         array (:class:`ArrayKey`):
 
             The key of the array to modify.
@@ -23,18 +24,17 @@
             The factor to use. If not given, a factor is chosen based on the
             ``dtype`` of the array (e.g., ``np.uint8`` would result in a factor
             of ``1.0/255``).
 
         dtype (data-type, optional):
 
             The datatype of the normalized array. Defaults to ``np.float32``.
-    '''
+    """
 
     def __init__(self, array, factor=None, dtype=np.float32):
-
         self.array = array
         self.factor = factor
         self.dtype = dtype
 
     def setup(self):
         self.enable_autoskip()
         array_spec = copy.deepcopy(self.spec[self.array])
@@ -44,36 +44,41 @@
     def prepare(self, request):
         deps = BatchRequest()
         deps[self.array] = request[self.array]
         deps[self.array].dtype = None
         return deps
 
     def process(self, batch, request):
-
         if self.array not in batch.arrays:
             return
 
         factor = self.factor
         array = batch.arrays[self.array]
         array.spec.dtype = self.dtype
 
         if factor is None:
-
-            logger.debug("automatically normalizing %s with dtype=%s",
-                    self.array, array.data.dtype)
+            logger.debug(
+                "automatically normalizing %s with dtype=%s",
+                self.array,
+                array.data.dtype,
+            )
 
             if array.data.dtype == np.uint8:
-                factor = 1.0/255
+                factor = 1.0 / 255
             elif array.data.dtype == np.uint16:
-                factor = 1.0/(256*256-1)
+                factor = 1.0 / (256 * 256 - 1)
             elif array.data.dtype == np.float32:
                 assert array.data.min() >= 0 and array.data.max() <= 1, (
-                        "Values are float but not in [0,1], I don't know how "
-                        "to normalize. Please provide a factor.")
+                    "Values are float but not in [0,1], I don't know how "
+                    "to normalize. Please provide a factor."
+                )
                 factor = 1.0
             else:
-                raise RuntimeError("Automatic normalization for " +
-                        str(array.data.dtype) + " not implemented, please "
-                        "provide a factor.")
+                raise RuntimeError(
+                    "Automatic normalization for "
+                    + str(array.data.dtype)
+                    + " not implemented, please "
+                    "provide a factor."
+                )
 
         logger.debug("scaling %s with %f", self.array, factor)
-        array.data = array.data.astype(self.dtype)*factor
+        array.data = array.data.astype(self.dtype) * factor
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/pad.py` & `gunpowder-1.3.0/gunpowder/nodes/pad.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import logging
 import numpy as np
 
 from .batch_filter import BatchFilter
 from gunpowder.array import ArrayKey
 from gunpowder.roi import Roi
+from gunpowder.coordinate import Coordinate
 from gunpowder.batch_request import BatchRequest
 
 logger = logging.getLogger(__name__)
 
+
 class Pad(BatchFilter):
-    '''Add a constant intensity padding around arrays of another batch 
-    provider. This is useful if your requested batches can be larger than what 
+    """Add a constant intensity padding around arrays of another batch
+    provider. This is useful if your requested batches can be larger than what
     your source provides.
 
     Args:
 
         key (:class:`ArrayKey` or :class:`GraphKey`):
 
             The array or points set to pad.
@@ -25,111 +27,110 @@
             a coordinate, this amount will be added to the ROI in the positive
             and negative direction.
 
         value (scalar or ``None``):
 
             The value to report inside the padding. If not given, 0 is used.
             Only used for :class:`Array<Arrays>`.
-    '''
+    """
 
     def __init__(self, key, size, value=None):
-
         self.key = key
         self.size = size
         self.value = value
 
     def setup(self):
         self.enable_autoskip()
 
         assert self.key in self.spec, (
-            "Asked to pad %s, but is not provided upstream."%self.key)
+            "Asked to pad %s, but is not provided upstream." % self.key
+        )
         assert self.spec[self.key].roi is not None, (
             "Asked to pad %s, but upstream provider doesn't have a ROI for "
-            "it."%self.key)
+            "it." % self.key
+        )
 
         spec = self.spec[self.key].copy()
         if self.size is not None:
             spec.roi = spec.roi.grow(self.size, self.size)
         else:
-            spec.roi.set_shape(None)
+            spec.roi.shape = Coordinate((None,) * spec.roi.dims)
         self.updates(self.key, spec)
 
     def prepare(self, request):
-
         upstream_spec = self.get_upstream_provider().spec
 
-        logger.debug("request: %s"%request)
-        logger.debug("upstream spec: %s"%upstream_spec)
+        logger.debug("request: %s" % request)
+        logger.debug("upstream spec: %s" % upstream_spec)
 
         # TODO: remove this?
         if self.key not in request:
             return
 
         roi = request[self.key].roi.copy()
 
         # change request to fit into upstream spec
         request[self.key].roi = roi.intersect(upstream_spec[self.key].roi)
 
-        if request[self.key].roi.empty():
-
+        if request[self.key].roi.empty:
             logger.warning(
-                "Requested %s ROI %s lies entirely outside of upstream "
-                "ROI %s.", self.key, roi, upstream_spec[self.key].roi)
+                "Requested %s ROI %s lies entirely outside of upstream " "ROI %s.",
+                self.key,
+                roi,
+                upstream_spec[self.key].roi,
+            )
 
             # ensure a valid request by asking for empty ROI
             request[self.key].roi = Roi(
-                    upstream_spec[self.key].roi.get_offset(),
-                    (0,)*upstream_spec[self.key].roi.dims()
+                upstream_spec[self.key].roi.offset,
+                (0,) * upstream_spec[self.key].roi.dims,
             )
 
-        logger.debug("new request: %s"%request)
+        logger.debug("new request: %s" % request)
 
         deps = BatchRequest()
         deps[self.key] = request[self.key]
         return deps
 
     def process(self, batch, request):
-
         if self.key not in request:
             return
 
         # restore requested batch size and ROI
         if isinstance(self.key, ArrayKey):
-
             array = batch.arrays[self.key]
             array.data = self.__expand(
-                    array.data,
-                    array.spec.roi/array.spec.voxel_size,
-                    request[self.key].roi/array.spec.voxel_size,
-                    self.value if self.value else 0
+                array.data,
+                array.spec.roi / array.spec.voxel_size,
+                request[self.key].roi / array.spec.voxel_size,
+                self.value if self.value else 0,
             )
             array.spec.roi = request[self.key].roi
 
         else:
-
             points = batch.graphs[self.key]
             points.spec.roi = request[self.key].roi
 
     def __expand(self, a, from_roi, to_roi, value):
-        '''from_roi and to_roi should be in voxels.'''
+        """from_roi and to_roi should be in voxels."""
 
         logger.debug(
-            "expanding array of shape %s from %s to %s",
-            str(a.shape), from_roi, to_roi)
+            "expanding array of shape %s from %s to %s", str(a.shape), from_roi, to_roi
+        )
 
-        num_channels = len(a.shape) - from_roi.dims()
+        num_channels = len(a.shape) - from_roi.dims
         channel_shapes = a.shape[:num_channels]
 
-        b = np.zeros(channel_shapes + to_roi.get_shape(), dtype=a.dtype)
+        b = np.zeros(channel_shapes + to_roi.shape, dtype=a.dtype)
         if value != 0:
             b[:] = value
 
-        shift = tuple(-x for x in to_roi.get_offset())
+        shift = -to_roi.offset
         logger.debug("shifting 'from' by " + str(shift))
         a_in_b = from_roi.shift(shift).to_slices()
 
         logger.debug("target shape is " + str(b.shape))
         logger.debug("target slice is " + str(a_in_b))
 
-        b[(slice(None),)*num_channels + a_in_b] = a
+        b[(slice(None),) * num_channels + a_in_b] = a
 
         return b
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/precache.py` & `gunpowder-1.3.0/gunpowder/nodes/precache.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 
 logger = logging.getLogger(__name__)
 
 
 class WorkersDiedException(Exception):
     pass
 
+
 class PreCache(BatchFilter):
-    '''Pre-cache repeated equal batch requests. For the first of a series of
+    """Pre-cache repeated equal batch requests. For the first of a series of
     equal batch request, a set of workers is spawned to pre-cache the batches
     in parallel processes. This way, subsequent requests can be served quickly.
 
     A note on changing the requests sent to `PreCache`.
     Given requests A and B, if requests are sent in the sequence:
     A, ..., A, B, A, ..., A, B, A, ...
     Precache will build a Queue of batches that satisfy A, and handle requests
@@ -42,63 +43,67 @@
         cache_size (``int``):
 
             How many batches to hold at most in the cache.
 
         num_workers (``int``):
 
             How many processes to spawn to fill the cache.
-    '''
+    """
 
     def __init__(self, cache_size=50, num_workers=20):
-
         self.current_request = None
         self.workers = None
         self.cache_size = cache_size
         self.num_workers = num_workers
 
         # keep track of recent requests
-        self.last_5 = deque([None,] * 5, maxlen=5)
+        self.last_5 = deque(
+            [
+                None,
+            ]
+            * 5,
+            maxlen=5,
+        )
 
     def teardown(self):
-
         if self.workers is not None:
             self.workers.stop()
 
     def provide(self, request):
-
         timing = Timing(self)
         timing.start()
 
         # update recent requests
         self.last_5.popleft()
         self.last_5.append(request)
 
         if request != self.current_request:
-
             current_count = sum(
                 [
                     recent_request == self.current_request
                     for recent_request in self.last_5
                 ]
             )
             new_count = sum(
                 [recent_request == request for recent_request in self.last_5]
             )
             if new_count > current_count or self.current_request is None:
-
                 if self.workers is not None:
                     logger.info("new request received, stopping current workers...")
                     self.workers.stop()
 
                 self.current_request = copy.deepcopy(request)
 
-                logger.info("starting new set of workers (%s, cache size %s)...",
-                            self.num_workers, self.cache_size)
+                logger.info(
+                    "starting new set of workers (%s, cache size %s)...",
+                    self.num_workers,
+                    self.cache_size,
+                )
                 self.workers = ProducerPool(
-                    [lambda i=i: self.__run_worker(i) for i in range(self.num_workers)],
+                    [self._run_worker for _ in range(self.num_workers)],
                     queue_size=self.cache_size,
                 )
                 self.workers.start()
 
                 logger.debug("getting batch from queue...")
                 batch = self.workers.get()
 
@@ -117,14 +122,14 @@
             batch = self.workers.get()
 
             timing.stop()
             batch.profiling_stats.add(timing)
 
         return batch
 
-    def __run_worker(self, i):
+    def _run_worker(self):
         request = copy.deepcopy(self.current_request)
         # Note that using a precache node breaks determinism in batches recieved since we do not
         # keep a mapping of the order in which random seeds were used, and the order in which
         # the corresponding batch gets returned.
         request._random_seed = random.randint(0, 2**32)
         return self.get_upstream_provider().request_batch(request)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/print_profiling_stats.py` & `gunpowder-1.3.0/gunpowder/nodes/print_profiling_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 import logging
 
 from .batch_filter import BatchFilter
 from gunpowder.profiling import Timing, TimingSummary, ProfilingStats
 
 logger = logging.getLogger(__name__)
 
+
 class PrintProfilingStats(BatchFilter):
-    '''Print profiling information about nodes upstream of this node in the DAG.
+    """Print profiling information about nodes upstream of this node in the DAG.
 
-    The output also includes a ``TOTAL`` section, which shows the wall-time 
-    spent in the upstream and downstream passes. For the downstream pass, this 
-    information is not available in the first iteration, since the request-batch 
+    The output also includes a ``TOTAL`` section, which shows the wall-time
+    spent in the upstream and downstream passes. For the downstream pass, this
+    information is not available in the first iteration, since the request-batch
     cycle is not completed, yet.
 
     Args:
 
         every (``int``):
 
             Collect statistics about that many batch requests and show min,
             max, mean, and median runtimes.
-    '''
+    """
 
     def __init__(self, every=1):
-
         self.every = every
         self.n = 0
         self.accumulated_stats = ProfilingStats()
         self.__upstream_timing = Timing(self)
         self.__upstream_timing_summary = TimingSummary()
         self.__downstream_timing = Timing(self)
         self.__downstream_timing_summary = TimingSummary()
 
     def prepare(self, request):
-
         self.__downstream_timing.stop()
-        # skip the first one, where we don't know how much time we spent 
+        # skip the first one, where we don't know how much time we spent
         # downstream
         if self.__downstream_timing.elapsed() > 0:
             self.__downstream_timing_summary.add(self.__downstream_timing)
             self.__downstream_timing = Timing(self)
 
         self.__upstream_timing.start()
 
         deps = request
         return deps
 
     def process(self, batch, request):
-
         self.__upstream_timing.stop()
         self.__upstream_timing_summary.add(self.__upstream_timing)
         self.__upstream_timing = Timing(self)
 
         self.__downstream_timing.start()
 
         self.n += 1
-        print_stats = self.n%self.every == 0
+        print_stats = self.n % self.every == 0
 
         self.accumulated_stats.merge_with(batch.profiling_stats)
 
         if not print_stats:
             return
 
         stats = "\n"
@@ -74,38 +72,41 @@
         stats += "MEDIAN".ljust(10)
         stats += "\n"
 
         summaries = list(self.accumulated_stats.get_timing_summaries().items())
         summaries.sort()
 
         for (node_name, method_name), summary in summaries:
-
             if summary.counts() > 0:
                 stats += node_name[:19].ljust(20)
-                stats += method_name[:19].ljust(10) if method_name is not None else ' '*10
-                stats += ("%d"%summary.counts())[:9].ljust(10)
-                stats += ("%.2f"%summary.min())[:9].ljust(10)
-                stats += ("%.2f"%summary.max())[:9].ljust(10)
-                stats += ("%.2f"%summary.mean())[:9].ljust(10)
-                stats += ("%.2f"%summary.median())[:9].ljust(10)
+                stats += (
+                    method_name[:19].ljust(10) if method_name is not None else " " * 10
+                )
+                stats += ("%d" % summary.counts())[:9].ljust(10)
+                stats += ("%.2f" % summary.min())[:9].ljust(10)
+                stats += ("%.2f" % summary.max())[:9].ljust(10)
+                stats += ("%.2f" % summary.mean())[:9].ljust(10)
+                stats += ("%.2f" % summary.median())[:9].ljust(10)
                 stats += "\n"
 
         stats += "\n"
         stats += "TOTAL"
         stats += "\n"
 
-        for phase, summary in zip(['upstream', 'downstream'], [self.__upstream_timing_summary, self.__downstream_timing_summary]):
-
+        for phase, summary in zip(
+            ["upstream", "downstream"],
+            [self.__upstream_timing_summary, self.__downstream_timing_summary],
+        ):
             if summary.counts() > 0:
                 stats += phase[:19].ljust(30)
-                stats += ("%d"%summary.counts())[:9].ljust(10)
-                stats += ("%.2f"%summary.min())[:9].ljust(10)
-                stats += ("%.2f"%summary.max())[:9].ljust(10)
-                stats += ("%.2f"%summary.mean())[:9].ljust(10)
-                stats += ("%.2f"%summary.median())[:9].ljust(10)
+                stats += ("%d" % summary.counts())[:9].ljust(10)
+                stats += ("%.2f" % summary.min())[:9].ljust(10)
+                stats += ("%.2f" % summary.max())[:9].ljust(10)
+                stats += ("%.2f" % summary.mean())[:9].ljust(10)
+                stats += ("%.2f" % summary.median())[:9].ljust(10)
                 stats += "\n"
 
         stats += "\n"
 
         logger.info(stats)
 
         # reset summaries
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/random_location.py` & `gunpowder-1.3.0/gunpowder/nodes/random_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 import numpy as np
 from scipy.spatial import cKDTree
 from skimage.transform import integral_image, integrate
 from gunpowder.batch_request import BatchRequest
 from gunpowder.coordinate import Coordinate
 from gunpowder.roi import Roi
+from gunpowder.array import Array
+from gunpowder.array_spec import ArraySpec
 from .batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
 
 class RandomLocation(BatchFilter):
     """Choses a batch at a random location in the bounding box of the upstream
@@ -53,61 +55,68 @@
             ``ensure_nonempty`` will contain at least one point.
 
         p_nonempty (``float``, optional):
 
             If ``ensure_nonempty`` is set, it defines the probability that a
             request for ``ensure_nonempty`` will contain at least one point.
             Default value is 1.0.
-            
+
         ensure_centered (``bool``, optional):
 
             if ``ensure_nonempty`` is set, ``ensure_centered`` guarantees
             that the center voxel of the roi contains a point.
 
         point_balance_radius (``int``):
 
             if ``ensure_nonempty`` is set, ``point_balance_radius`` defines
             a radius s.t. for every point `p` in ``ensure_nonempty``, the
             probability of picking p is inversely related to the number of
             other points within a distance of ``point_balance_radius`` to p.
             This helps avoid oversampling of dense regions of the graph, and
-            undersampling of sparse regions. 
+            undersampling of sparse regions.
+
+        random_shift_key (``ArrayKey`` optional):
+
+            if ``random_shift_key`` is not None, this node will populate
+            that key with a nonspatial array containing the random shift
+            used for each request. This can be useful for snapshot iterations
+            if you want to figure out where that snapshot came from.
     """
 
     def __init__(
         self,
         min_masked=0,
         mask=None,
         ensure_nonempty=None,
         p_nonempty=1.0,
         ensure_centered=None,
         point_balance_radius=1,
+        random_shift_key=None,
     ):
-
         self.min_masked = min_masked
         self.mask = mask
         self.mask_spec = None
         self.mask_integral = None
         self.ensure_nonempty = ensure_nonempty
         self.points = None
         self.p_nonempty = p_nonempty
         self.upstream_spec = None
         self.random_shift = None
         self.ensure_centered = ensure_centered
         self.point_balance_radius = point_balance_radius
+        self.random_shift_key = random_shift_key
 
     def setup(self):
-
         upstream = self.get_upstream_provider()
         self.upstream_spec = upstream.spec
 
         if self.mask and self.min_masked > 0:
-
             assert self.mask in self.upstream_spec, (
-                "Upstream provider does not have %s"%self.mask)
+                "Upstream provider does not have %s" % self.mask
+            )
             self.mask_spec = self.upstream_spec.array_specs[self.mask]
 
             logger.info("requesting complete mask...")
 
             mask_request = BatchRequest({self.mask: self.mask_spec})
             mask_batch = upstream.request_batch(mask_request)
 
@@ -119,23 +128,24 @@
             if mask_data.size < 2**32:
                 mask_integral_dtype = np.uint32
             if mask_data.size < 2**16:
                 mask_integral_dtype = np.uint16
             logger.debug("chose %s as integral array dtype", mask_integral_dtype)
 
             self.mask_integral = np.array(mask_data > 0, dtype=mask_integral_dtype)
-            self.mask_integral = integral_image(self.mask_integral).astype(mask_integral_dtype)
+            self.mask_integral = integral_image(self.mask_integral).astype(
+                mask_integral_dtype
+            )
 
         if self.ensure_nonempty:
-
             assert self.ensure_nonempty in self.upstream_spec, (
-                "Upstream provider does not have %s"%self.ensure_nonempty)
+                "Upstream provider does not have %s" % self.ensure_nonempty
+            )
             graph_spec = self.upstream_spec.graph_specs[self.ensure_nonempty]
 
-
             logger.info("requesting all %s points...", self.ensure_nonempty)
 
             nonempty_request = BatchRequest({self.ensure_nonempty: graph_spec})
             nonempty_batch = upstream.request_batch(nonempty_request)
 
             self.points = cKDTree(
                 [p.location for p in nonempty_batch[self.ensure_nonempty].nodes]
@@ -150,206 +160,196 @@
 
             logger.debug("retrieved %d points", len(self.points.data))
 
         # clear bounding boxes of all provided arrays and points --
         # RandomLocation does not have limits (offsets are ignored)
         for key, spec in self.spec.items():
             if spec.roi is not None:
-                spec.roi.set_shape(None)
+                spec.roi.shape = Coordinate((None,) * spec.roi.dims)
                 self.updates(key, spec)
 
+        # provide randomness if asked for
+        if self.random_shift_key is not None:
+            self.provides(self.random_shift_key, ArraySpec(nonspatial=True))
+
     def prepare(self, request):
         seed(request.random_seed)
 
         logger.debug("request: %s", request.array_specs)
         logger.debug("my spec: %s", self.spec)
 
         if request.array_specs.keys():
-            lcm_voxel_size = self.spec.get_lcm_voxel_size(
-                request.array_specs.keys())
+            lcm_voxel_size = self.spec.get_lcm_voxel_size(request.array_specs.keys())
         else:
-            lcm_voxel_size = Coordinate((1,)*request.get_total_roi().dims())
+            lcm_voxel_size = Coordinate((1,) * request.get_total_roi().dims)
 
         shift_roi = self.__get_possible_shifts(request, lcm_voxel_size)
 
         if request.array_specs.keys():
-
-            shift_roi = shift_roi.snap_to_grid(lcm_voxel_size, mode='shrink')
-            lcm_shift_roi = shift_roi/lcm_voxel_size
+            shift_roi = shift_roi.snap_to_grid(lcm_voxel_size, mode="shrink")
+            lcm_shift_roi = shift_roi / lcm_voxel_size
             logger.debug(
                 "restricting random locations to multiples of voxel size %s",
-                lcm_voxel_size)
+                lcm_voxel_size,
+            )
 
         else:
-
             lcm_shift_roi = shift_roi
 
-        assert not lcm_shift_roi.unbounded(), (
+        assert not lcm_shift_roi.unbounded, (
             "Can not pick a random location, intersection of upstream ROIs is "
-            "unbounded.")
-        assert not lcm_shift_roi.empty(), (
-            "Can not satisfy batch request, no location covers all requested "
-            "ROIs.")
+            "unbounded."
+        )
+        assert not lcm_shift_roi.empty, (
+            "Can not satisfy batch request, no location covers all requested " "ROIs."
+        )
 
         random_shift = self.__select_random_shift(
-            request,
-            lcm_shift_roi,
-            lcm_voxel_size)
+            request, lcm_shift_roi, lcm_voxel_size
+        )
 
         self.random_shift = random_shift
         self.__shift_request(request, random_shift)
 
         return request
 
     def process(self, batch, request):
+        if self.random_shift_key is not None:
+            batch[self.random_shift_key] = Array(
+                np.array(self.random_shift),
+                ArraySpec(nonspatial=True),
+            )
 
         # reset ROIs to request
-        for (array_key, spec) in request.array_specs.items():
+        for array_key, spec in request.array_specs.items():
             batch.arrays[array_key].spec.roi = spec.roi
-        for (graph_key, spec) in request.graph_specs.items():
+        for graph_key, spec in request.graph_specs.items():
             batch.graphs[graph_key].spec.roi = spec.roi
 
         # change shift point locations to lie within roi
         for graph_key in request.graph_specs.keys():
             batch.graphs[graph_key].shift(-self.random_shift)
 
     def accepts(self, request):
-        '''Should return True if the randomly chosen location is acceptable
+        """Should return True if the randomly chosen location is acceptable
         (besided meeting other criteria like ``min_masked`` and/or
         ``ensure_nonempty``). Subclasses can overwrite this method to implement
-        additional tests for acceptable locations.'''
+        additional tests for acceptable locations."""
 
         return True
 
     def __get_possible_shifts(self, request, voxel_size):
-
         total_shift_roi = None
 
         for key, spec in request.items():
-
             if spec.roi is None:
                 continue
 
             request_roi = spec.roi
             provided_roi = self.upstream_spec[key].roi
 
-            shift_roi = provided_roi.shift(
-                -request_roi.get_begin()
-            ).grow(
-                (0,)*request_roi.dims(),
-                -(request_roi.get_shape() - voxel_size)
+            shift_roi = provided_roi.shift(-request_roi.begin).grow(
+                (0,) * request_roi.dims, -(request_roi.shape - voxel_size)
             )
 
             if total_shift_roi is None:
                 total_shift_roi = shift_roi
             else:
                 if shift_roi != total_shift_roi:
                     total_shift_roi = total_shift_roi.intersect(shift_roi)
 
         logger.debug("valid shifts for request in " + str(total_shift_roi))
 
         return total_shift_roi
 
     def __select_random_shift(self, request, lcm_shift_roi, lcm_voxel_size):
-
-        ensure_points = (
-            self.ensure_nonempty is not None
-            and
-            random() <= self.p_nonempty)
+        ensure_points = self.ensure_nonempty is not None and random() <= self.p_nonempty
 
         while True:
-
             if ensure_points:
                 random_shift = self.__select_random_location_with_points(
-                    request,
-                    lcm_shift_roi,
-                    lcm_voxel_size)
+                    request, lcm_shift_roi, lcm_voxel_size
+                )
             else:
                 random_shift = self.__select_random_location(
-                    lcm_shift_roi,
-                    lcm_voxel_size)
+                    lcm_shift_roi, lcm_voxel_size
+                )
 
             logger.debug("random shift: " + str(random_shift))
 
             if not self.__is_min_masked(random_shift, request):
-                logger.debug(
-                    "random location does not meet 'min_masked' criterium")
+                logger.debug("random location does not meet 'min_masked' criterium")
                 continue
 
             if not self.__accepts(random_shift, request):
-                logger.debug(
-                    "random location does not meet user-provided criterium")
+                logger.debug("random location does not meet user-provided criterium")
                 continue
 
             return random_shift
 
     def __is_min_masked(self, random_shift, request):
-
         if not self.mask or self.min_masked == 0:
             return True
 
         # get randomly chosen mask ROI
         request_mask_roi = request.array_specs[self.mask].roi
         request_mask_roi = request_mask_roi.shift(random_shift)
 
         # get coordinates inside mask array
         mask_voxel_size = self.spec[self.mask].voxel_size
-        request_mask_roi_in_array = request_mask_roi/mask_voxel_size
-        request_mask_roi_in_array -= self.mask_spec.roi.get_offset()/mask_voxel_size
+        request_mask_roi_in_array = request_mask_roi / mask_voxel_size
+        request_mask_roi_in_array -= self.mask_spec.roi.offset / mask_voxel_size
 
         # get number of masked-in voxels
         num_masked_in = integrate(
             self.mask_integral,
-            [request_mask_roi_in_array.get_begin()],
-            [request_mask_roi_in_array.get_end()-(1,)*self.mask_integral.ndim]
+            [request_mask_roi_in_array.begin],
+            [
+                request_mask_roi_in_array.end
+                - Coordinate((1,) * self.mask_integral.ndim)
+            ],
         )[0]
 
-        mask_ratio = float(num_masked_in)/request_mask_roi_in_array.size()
+        mask_ratio = float(num_masked_in) / request_mask_roi_in_array.size
         logger.debug("mask ratio is %f", mask_ratio)
 
         return mask_ratio >= self.min_masked
 
     def __accepts(self, random_shift, request):
-
         # create a shifted copy of the request
         shifted_request = request.copy()
         self.__shift_request(shifted_request, random_shift)
 
         return self.accepts(shifted_request)
 
     def __shift_request(self, request, shift):
-
         # shift request ROIs
         for specs_type in [request.array_specs, request.graph_specs]:
-            for (key, spec) in specs_type.items():
+            for key, spec in specs_type.items():
                 if spec.roi is None:
                     continue
                 roi = spec.roi.shift(shift)
                 specs_type[key].roi = roi
 
     def __select_random_location_with_points(
-            self,
-            request,
-            lcm_shift_roi,
-            lcm_voxel_size):
-
+        self, request, lcm_shift_roi, lcm_voxel_size
+    ):
         request_points = request.graph_specs.get(self.ensure_nonempty)
         if request_points is None:
             total_roi = request.get_total_roi()
             logger.warning(
                 f"Requesting non empty {self.ensure_nonempty}, however {self.ensure_nonempty} "
                 f"has not been requested. Falling back on using the total roi of the "
                 f"request {total_roi} for {self.ensure_nonempty}."
             )
             request_points_roi = total_roi
         else:
             request_points_roi = request_points.roi
 
         while True:
-
             # How to pick shifts that ensure that a randomly chosen point is
             # contained in the request ROI:
             #
             #
             # request          point
             # [---------)      .
             # 0        +10     17
@@ -376,22 +376,20 @@
 
             # pick a random point
             point = choices(self.points.data, cum_weights=self.cumulative_weights)[0]
 
             logger.debug("select random point at %s", point)
 
             # get the lcm voxel that contains this point
-            lcm_location = Coordinate(point/lcm_voxel_size)
-            logger.debug(
-                "belongs to lcm voxel %s",
-                lcm_location)
+            lcm_location = Coordinate(point / lcm_voxel_size)
+            logger.debug("belongs to lcm voxel %s", lcm_location)
 
             # get the request ROI's shape in lcm
-            lcm_roi_begin = request_points_roi.get_begin()/lcm_voxel_size
-            lcm_roi_shape = request_points_roi.get_shape()/lcm_voxel_size
+            lcm_roi_begin = request_points_roi.begin / lcm_voxel_size
+            lcm_roi_shape = request_points_roi.shape / lcm_voxel_size
             logger.debug("Point request ROI: %s", request_points_roi)
             logger.debug("Point request lcm ROI shape: %s", lcm_roi_shape)
 
             # get all possible starting points of lcm_roi_shape that contain
             # lcm_location
             if self.ensure_centered:
                 lcm_shift_roi_begin = (
@@ -399,64 +397,70 @@
                     - lcm_roi_begin
                     - lcm_roi_shape / 2
                     + Coordinate((1,) * len(lcm_location))
                 )
                 lcm_shift_roi_shape = Coordinate((1,) * len(lcm_location))
             else:
                 lcm_shift_roi_begin = (
-                    lcm_location - lcm_roi_begin - lcm_roi_shape +
-                    Coordinate((1,)*len(lcm_location))
+                    lcm_location
+                    - lcm_roi_begin
+                    - lcm_roi_shape
+                    + Coordinate((1,) * len(lcm_location))
                 )
                 lcm_shift_roi_shape = lcm_roi_shape
             lcm_point_shift_roi = Roi(lcm_shift_roi_begin, lcm_shift_roi_shape)
 
             logger.debug("lcm point shift roi: %s", lcm_point_shift_roi)
 
             # intersect with total shift ROI
             if not lcm_point_shift_roi.intersects(lcm_shift_roi):
                 logger.debug(
                     "reject random shift, random point %s shift ROI %s does "
-                    "not intersect total shift ROI %s", point,
-                    lcm_point_shift_roi, lcm_shift_roi)
+                    "not intersect total shift ROI %s",
+                    point,
+                    lcm_point_shift_roi,
+                    lcm_shift_roi,
+                )
                 continue
             lcm_point_shift_roi = lcm_point_shift_roi.intersect(lcm_shift_roi)
 
             # select a random shift from all possible shifts
             random_shift = self.__select_random_location(
-                lcm_point_shift_roi,
-                lcm_voxel_size)
+                lcm_point_shift_roi, lcm_voxel_size
+            )
             logger.debug("random shift: %s", random_shift)
 
             # count all points inside the shifted ROI
-            points = self.__get_points_in_roi(
-                request_points_roi.shift(random_shift))
-            assert point in points, (
-                "Requested batch to contain point %s, but got points "
-                "%s"%(point, points))
+            points = self.__get_points_in_roi(request_points_roi.shift(random_shift))
+            assert (
+                point in points
+            ), "Requested batch to contain point %s, but got points " "%s" % (
+                point,
+                points,
+            )
             num_points = len(points)
 
             return random_shift
 
     def __select_random_location(self, lcm_shift_roi, lcm_voxel_size):
-
         # select a random point inside ROI
         random_shift = Coordinate(
             randint(begin, end - 1)
-            for begin, end in zip(lcm_shift_roi.get_begin(), lcm_shift_roi.get_end()))
+            for begin, end in zip(lcm_shift_roi.begin, lcm_shift_roi.end)
+        )
 
         random_shift *= lcm_voxel_size
 
         return random_shift
 
     def __get_points_in_roi(self, roi):
-
         points = []
 
-        center = roi.get_center()
-        radius = math.ceil(float(max(roi.get_shape()))/2)
+        center = roi.center
+        radius = math.ceil(float(max(roi.shape)) / 2)
         candidates = self.points.query_ball_point(center, radius, p=np.inf)
 
         for i in candidates:
             if roi.contains(self.points.data[i]):
                 points.append(self.points.data[i])
 
         return np.array(points)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/random_provider.py` & `gunpowder-1.3.0/gunpowder/nodes/random_provider.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,89 @@
 import copy
 import numpy as np
 
+from gunpowder.array import Array
+from gunpowder.array_spec import ArraySpec
+
 from .batch_provider import BatchProvider
 
 
 class RandomProvider(BatchProvider):
-    '''Randomly selects one of the upstream providers::
+    """Randomly selects one of the upstream providers::
 
         (a + b + c) + RandomProvider()
 
     will create a provider that randomly relays requests to providers ``a``,
     ``b``, or ``c``. Array and point keys of ``a``, ``b``, and ``c`` should be
     the same.
 
     Args:
-        probabilities (1-D array-like, optional): An optional list of
+        probabilities (1-D array-like, optional):
+
+            An optional list of
             probabilities for choosing upstream providers, given in the
             same order. Probabilities do not need to be normalized. Default
             is ``None``, corresponding to equal probabilities.
-    '''
 
-    def __init__(self, probabilities=None):
+        random_provider_key (``ArrayKey``):
+
+            If provided, this node will store the index of the chosen random
+            provider in a nonspatial array.
+    """
+
+    def __init__(self, probabilities=None, random_provider_key=None):
         self.probabilities = probabilities
+        self.random_provider_key = random_provider_key
 
         # automatically normalize probabilities to sum to 1
         if self.probabilities is not None:
-            self.probabilities = [float(x)/np.sum(probabilities) for x in
-                                  self.probabilities]
+            self.probabilities = [
+                float(x) / np.sum(probabilities) for x in self.probabilities
+            ]
 
     def setup(self):
         self.enable_placeholders()
-        assert len(self.get_upstream_providers()) > 0,\
-            "at least one batch provider must be added to the RandomProvider"
+        assert (
+            len(self.get_upstream_providers()) > 0
+        ), "at least one batch provider must be added to the RandomProvider"
         if self.probabilities is not None:
-            assert len(self.get_upstream_providers()) == len(
-                self.probabilities), "if probabilities are specified, they " \
-                                     "need to be given for each batch " \
-                                     "provider added to the RandomProvider"
+            assert len(self.get_upstream_providers()) == len(self.probabilities), (
+                "if probabilities are specified, they "
+                "need to be given for each batch "
+                "provider added to the RandomProvider"
+            )
 
         common_spec = None
 
         # advertise outputs only if all upstream providers have them
         for provider in self.get_upstream_providers():
-
             if common_spec is None:
                 common_spec = copy.deepcopy(provider.spec)
             else:
                 for key, spec in list(common_spec.items()):
                     if key not in provider.spec:
                         del common_spec[key]
 
         for key, spec in common_spec.items():
             self.provides(key, spec)
 
+        if self.random_provider_key is not None:
+            self.provides(self.random_provider_key, ArraySpec(nonspatial=True))
 
     def provide(self, request):
         # Random seed is set in provide rather than prepare since this node
         # is not a batch filter
         np.random.seed(request.random_seed)
-        return np.random.choice(self.get_upstream_providers(),
-                                p=self.probabilities).request_batch(request)
+
+        if self.random_provider_key is not None:
+            del request[self.random_provider_key]
+
+        i = np.random.choice(
+            range(len(self.get_upstream_providers())), p=self.probabilities
+        )
+        provider = self.get_upstream_providers()[i]
+        batch = provider.request_batch(request)
+        if self.random_provider_key is not None:
+            batch[self.random_provider_key] = Array(
+                np.array(i), ArraySpec(nonspatial=True)
+            )
+        return batch
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/rasterize_graph.py` & `gunpowder-1.3.0/gunpowder/nodes/rasterize_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 from gunpowder.ndarray import replace
 from gunpowder.graph import GraphKey
 from gunpowder.graph_spec import GraphSpec
 from gunpowder.roi import Roi
 
 logger = logging.getLogger(__name__)
 
+
 class RasterizationSettings(Freezable):
-    '''Data structure to store parameters for rasterization of graph.
+    """Data structure to store parameters for rasterization of graph.
 
     Args:
 
         radius (``float`` or ``tuple`` of ``float``):
 
             The radius (for balls or tubes) or sigma (for peaks) in world units.
 
@@ -69,38 +70,37 @@
             Default is True.
 
         color_attr (``str``, optional)
 
             Which graph attribute to use for coloring nodes and edges. One
             useful example might be `component` which would color your graph
             based on the component labels.
-            Notes: 
+            Notes:
             - Only available in "ball" mode
             - Nodes and Edges missing the attribute will be skipped.
             - color_attr must be populated for nodes and edges upstream of this node
-    '''
-    def __init__(
-            self,
-            radius,
-            mode='ball',
-            mask=None,
-            inner_radius_fraction=None,
-            fg_value=1,
-            bg_value=0,
-            edges=True,
-            color_attr=None,
-            ):
+    """
 
+    def __init__(
+        self,
+        radius,
+        mode="ball",
+        mask=None,
+        inner_radius_fraction=None,
+        fg_value=1,
+        bg_value=0,
+        edges=True,
+        color_attr=None,
+    ):
         radius = np.array([radius]).flatten().astype(np.float64)
 
         if inner_radius_fraction is not None:
             assert (
-                inner_radius_fraction > 0.0 and
-                inner_radius_fraction < 1.0), (
-                    "Inner radius fraction has to be between (excluding) 0 and 1")
+                inner_radius_fraction > 0.0 and inner_radius_fraction < 1.0
+            ), "Inner radius fraction has to be between (excluding) 0 and 1"
             inner_radius_fraction = 1.0 - inner_radius_fraction
 
         self.radius = radius
         self.mode = mode
         self.mask = mask
         self.inner_radius_fraction = inner_radius_fraction
         self.fg_value = fg_value
@@ -127,286 +127,273 @@
             voxel size.
 
         settings (:class:`RasterizationSettings`, optional):
             Which settings to use to rasterize the graph.
     """
 
     def __init__(self, graph, array, array_spec=None, settings=None):
-
         self.graph = graph
         self.array = array
         if array_spec is None:
             self.array_spec = ArraySpec()
         else:
             self.array_spec = array_spec
         if settings is None:
             self.settings = RasterizationSettings(1)
         else:
             self.settings = settings
 
     def setup(self):
-
         graph_roi = self.spec[self.graph].roi
 
         if self.array_spec.voxel_size is None:
-            self.array_spec.voxel_size = Coordinate((1,)*graph_roi.dims())
+            self.array_spec.voxel_size = Coordinate((1,) * graph_roi.dims)
 
         if self.array_spec.dtype is None:
-            if self.settings.mode == 'ball':
+            if self.settings.mode == "ball":
                 self.array_spec.dtype = np.uint8
             else:
                 self.array_spec.dtype = np.float32
 
         self.array_spec.roi = graph_roi.copy()
-        self.provides(
-            self.array,
-            self.array_spec)
+        self.provides(self.array, self.array_spec)
 
         self.enable_autoskip()
 
     def prepare(self, request):
-
-        if self.settings.mode == 'ball':
-            context = np.ceil(self.settings.radius).astype(np.int)
-        elif self.settings.mode == 'peak':
-            context = np.ceil(2*self.settings.radius).astype(np.int)
+        if self.settings.mode == "ball":
+            context = np.ceil(self.settings.radius).astype(int)
+        elif self.settings.mode == "peak":
+            context = np.ceil(2 * self.settings.radius).astype(int)
         else:
-            raise RuntimeError('unknown raster mode %s'%self.settings.mode)
+            raise RuntimeError("unknown raster mode %s" % self.settings.mode)
 
-        dims = self.array_spec.roi.dims()
+        dims = self.array_spec.roi.dims
         if len(context) == 1:
             context = context.repeat(dims)
 
         # request graph in a larger area to get rasterization from outside
         # graph
         graph_roi = request[self.array].roi.grow(
-                Coordinate(context),
-                Coordinate(context))
+            Coordinate(context), Coordinate(context)
+        )
 
         # however, restrict the request to the graph actually provided
         graph_roi = graph_roi.intersect(self.spec[self.graph].roi)
 
         deps = BatchRequest()
         deps[self.graph] = GraphSpec(roi=graph_roi)
 
         if self.settings.mask is not None:
-
             mask_voxel_size = self.spec[self.settings.mask].voxel_size
-            assert self.spec[self.array].voxel_size == mask_voxel_size, (
-                "Voxel size of mask and rasterized volume need to be equal")
+            assert (
+                self.spec[self.array].voxel_size == mask_voxel_size
+            ), "Voxel size of mask and rasterized volume need to be equal"
 
             new_mask_roi = graph_roi.snap_to_grid(mask_voxel_size)
             deps[self.settings.mask] = ArraySpec(roi=new_mask_roi)
 
         return deps
 
     def process(self, batch, request):
-
         graph = batch.graphs[self.graph]
         mask = self.settings.mask
         voxel_size = self.spec[self.array].voxel_size
 
         # get roi used for creating the new array (graph_roi does not
         # necessarily align with voxel size)
         enlarged_vol_roi = graph.spec.roi.snap_to_grid(voxel_size)
-        offset = enlarged_vol_roi.get_begin() / voxel_size
-        shape = enlarged_vol_roi.get_shape() / voxel_size
+        offset = enlarged_vol_roi.begin / voxel_size
+        shape = enlarged_vol_roi.shape / voxel_size
         data_roi = Roi(offset, shape)
 
         logger.debug("Graph in %s", graph.spec.roi)
         for node in graph.nodes:
             logger.debug("%d, %s", node.id, node.location)
         logger.debug("Data roi in voxels: %s", data_roi)
-        logger.debug("Data roi in world units: %s", data_roi*voxel_size)
+        logger.debug("Data roi in world units: %s", data_roi * voxel_size)
 
         if graph.num_vertices == 0:
             # If there are no nodes at all, just create an empty matrix.
             rasterized_graph_data = np.zeros(
-                data_roi.get_shape(), dtype=self.spec[self.array].dtype
+                data_roi.shape, dtype=self.spec[self.array].dtype
             )
         elif mask is not None:
-
             mask_array = batch.arrays[mask].crop(enlarged_vol_roi)
             # get those component labels in the mask, that contain graph
             labels = []
             for i, point in graph.data.items():
                 v = Coordinate(point.location / voxel_size)
-                v -= data_roi.get_begin()
+                v -= data_roi.begin
                 labels.append(mask_array.data[v])
             # Make list unique
             labels = list(set(labels))
 
             # zero label should be ignored
             if 0 in labels:
                 labels.remove(0)
 
             if len(labels) == 0:
-                logger.debug("Graph and provided object mask do not overlap. No graph to rasterize.")
-                rasterized_graph_data = np.zeros(data_roi.get_shape(),
-                                                  dtype=self.spec[self.array].dtype)
+                logger.debug(
+                    "Graph and provided object mask do not overlap. No graph to rasterize."
+                )
+                rasterized_graph_data = np.zeros(
+                    data_roi.shape, dtype=self.spec[self.array].dtype
+                )
             else:
                 # create data for the whole graph ROI, "or"ed together over
                 # individual object masks
                 rasterized_graph_data = np.sum(
                     [
                         self.__rasterize(
                             graph,
                             data_roi,
                             voxel_size,
                             self.spec[self.array].dtype,
                             self.settings,
-                            Array(data=mask_array.data==label, spec=mask_array.spec))
-
+                            Array(data=mask_array.data == label, spec=mask_array.spec),
+                        )
                         for label in labels
                     ],
-                    axis=0)
+                    axis=0,
+                )
 
         else:
-
             # create data for the whole graph ROI without mask
             rasterized_graph_data = self.__rasterize(
-                graph,
-                data_roi,
-                voxel_size,
-                self.spec[self.array].dtype,
-                self.settings)
+                graph, data_roi, voxel_size, self.spec[self.array].dtype, self.settings
+            )
 
         # fix bg/fg labelling if requested
-        if (self.settings.bg_value != 0 or
-            self.settings.fg_value != 1):
-
+        if self.settings.bg_value != 0 or self.settings.fg_value != 1:
             replaced = replace(
                 rasterized_graph_data,
                 [0, 1],
-                [self.settings.bg_value, self.settings.fg_value])
+                [self.settings.bg_value, self.settings.fg_value],
+            )
             rasterized_graph_data = replaced.astype(self.spec[self.array].dtype)
 
         # create array and crop it to requested roi
         spec = self.spec[self.array].copy()
-        spec.roi = data_roi*voxel_size
-        rasterized_points = Array(
-            data=rasterized_graph_data,
-            spec=spec)
+        spec.roi = data_roi * voxel_size
+        rasterized_points = Array(data=rasterized_graph_data, spec=spec)
         batch[self.array] = rasterized_points.crop(request[self.array].roi)
 
-    def __rasterize(self, graph, data_roi, voxel_size, dtype, settings, mask_array=None):
-        '''Rasterize 'graph' into an array with the given 'voxel_size'''
+    def __rasterize(
+        self, graph, data_roi, voxel_size, dtype, settings, mask_array=None
+    ):
+        """Rasterize 'graph' into an array with the given 'voxel_size"""
 
         mask = mask_array.data if mask_array is not None else None
 
         logger.debug("Rasterizing graph in %s", graph.spec.roi)
 
         # prepare output array
-        rasterized_graph = np.zeros(data_roi.get_shape(), dtype=dtype)
+        rasterized_graph = np.zeros(data_roi.shape, dtype=dtype)
 
         # Fast rasterization currently only implemented for mode ball without
         # inner radius set
         use_fast_rasterization = (
             settings.mode == "ball"
             and settings.inner_radius_fraction is None
             and len(list(graph.edges)) == 0
         )
 
         if use_fast_rasterization:
-
             dims = len(rasterized_graph.shape)
 
             # get structuring element for mode ball
             ball_kernel = create_ball_kernel(settings.radius, voxel_size)
-            radius_voxel = Coordinate(np.array(ball_kernel.shape)/2)
+            radius_voxel = Coordinate(np.array(ball_kernel.shape) / 2)
             data_roi_base = Roi(
-                    offset=Coordinate((0,)*dims),
-                    shape=Coordinate(rasterized_graph.shape))
+                offset=Coordinate((0,) * dims), shape=Coordinate(rasterized_graph.shape)
+            )
             kernel_roi_base = Roi(
-                    offset=Coordinate((0,)*dims),
-                    shape=Coordinate(ball_kernel.shape))
+                offset=Coordinate((0,) * dims), shape=Coordinate(ball_kernel.shape)
+            )
 
         # Rasterize volume either with single voxel or with defined struct elememt
         for node in graph.nodes:
-
             # get the voxel coordinate, 'Coordinate' ensures integer
-            v = Coordinate(node.location/voxel_size)
+            v = Coordinate(node.location / voxel_size)
 
             # get the voxel coordinate relative to output array start
-            v -= data_roi.get_begin()
+            v -= data_roi.begin
 
             # skip graph outside of mask
             if mask is not None and not mask[v]:
                 continue
 
             logger.debug(
                 "Rasterizing node %s at %s",
                 node.location,
-                node.location/voxel_size - data_roi.get_begin())
+                node.location / voxel_size - data_roi.begin,
+            )
 
             if use_fast_rasterization:
-
                 # Calculate where to crop the kernel mask and the rasterized array
                 shifted_kernel = kernel_roi_base.shift(v - radius_voxel)
                 shifted_data = data_roi_base.shift(-(v - radius_voxel))
                 arr_crop = data_roi_base.intersect(shifted_kernel)
                 kernel_crop = kernel_roi_base.intersect(shifted_data)
                 arr_crop_ind = arr_crop.get_bounding_box()
                 kernel_crop_ind = kernel_crop.get_bounding_box()
 
                 rasterized_graph[arr_crop_ind] = np.logical_or(
                     ball_kernel[kernel_crop_ind], rasterized_graph[arr_crop_ind]
                 )
 
             else:
-
                 if settings.color_attr is not None:
                     c = graph.nodes[node].get(settings.color_attr)
                     if c is None:
                         logger.debug(f"Skipping node: {node}")
                         continue
                     elif np.isclose(c, 1) and not np.isclose(settings.fg_value, 1):
                         logger.warning(
                             f"Node {node} is being colored with color {c} according to "
                             f"attribute {settings.color_attr} "
                             f"but color 1 will be replaced with fg_value: {settings.fg_value}"
-                            )
+                        )
                 else:
                     c = 1
                 rasterized_graph[v] = c
         if settings.edges:
             for e in graph.edges:
                 if settings.color_attr is not None:
                     c = graph.edges[e].get(settings.color_attr)
                     if c is None:
                         continue
                     elif np.isclose(c, 1) and not np.isclose(settings.fg_value, 1):
                         logger.warning(
                             f"Edge {e} is being colored with color {c} according to "
                             f"attribute {settings.color_attr} "
                             f"but color 1 will be replaced with fg_value: {settings.fg_value}"
-                            )
+                        )
 
                 u = graph.node(e.u)
                 v = graph.node(e.v)
                 u_coord = Coordinate(u.location / voxel_size)
                 v_coord = Coordinate(v.location / voxel_size)
                 line = draw.line_nd(u_coord, v_coord, endpoint=True)
                 rasterized_graph[line] = 1
 
         # grow graph
         if not use_fast_rasterization:
-
             if settings.mode == "ball":
-
                 enlarge_binary_map(
                     rasterized_graph,
                     settings.radius,
                     voxel_size,
                     settings.inner_radius_fraction,
-                    in_place=True)
+                    in_place=True,
+                )
 
             else:
-
-                sigmas = settings.radius/voxel_size
+                sigmas = settings.radius / voxel_size
 
                 gaussian_filter(
                     rasterized_graph, sigmas, output=rasterized_graph, mode="constant"
                 )
 
                 # renormalize to have 1 be the highest value
                 max_value = np.max(rasterized_graph)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/reject.py` & `gunpowder-1.3.0/gunpowder/nodes/reject.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from .batch_filter import BatchFilter
 from gunpowder.profiling import Timing
 
 logger = logging.getLogger(__name__)
 
 
 class Reject(BatchFilter):
-    '''Reject batches based on the masked-in vs. masked-out ratio.
+    """Reject batches based on the masked-in vs. masked-out ratio.
+
+    If a pipeline also contains a :class:`RandomLocation` node,
+    :class:`Reject` needs to be placed downstream of it.
 
     Args:
 
         mask (:class:`ArrayKey`, optional):
 
             The mask to use, if any.
 
@@ -26,103 +29,106 @@
             Ensures there is at least one point in the batch.
 
         reject_probability (``float``, optional):
 
             The probability by which a batch that is not valid (less than
             min_masked) is actually rejected. Defaults to 1., i.e. strict
             rejection.
-    '''
+    """
 
     def __init__(
-            self,
-            mask=None,
-            min_masked=0.5,
-            ensure_nonempty=None,
-            reject_probability=1.):
-
+        self, mask=None, min_masked=0.5, ensure_nonempty=None, reject_probability=1.0
+    ):
         self.mask = mask
         self.min_masked = min_masked
         self.ensure_nonempty = ensure_nonempty
         self.reject_probability = reject_probability
 
     def setup(self):
         if self.mask:
             assert self.mask in self.spec, (
-                "Reject can only be used if %s is provided" % self.mask)
+                "Reject can only be used if %s is provided" % self.mask
+            )
         if self.ensure_nonempty:
             assert self.ensure_nonempty in self.spec, (
-                "Reject can only be used if %s is provided" %
-                self.ensure_nonempty)
+                "Reject can only be used if %s is provided" % self.ensure_nonempty
+            )
         self.upstream_provider = self.get_upstream_provider()
 
     def provide(self, request):
         random.seed(request.random_seed)
 
         report_next_timeout = 10
         num_rejected = 0
 
         timing = Timing(self)
         timing.start()
         if self.mask:
             assert self.mask in request, (
-                "Reject can only be used if %s is provided" % self.mask)
+                "Reject can only be used if %s is provided" % self.mask
+            )
         if self.ensure_nonempty:
             assert self.ensure_nonempty in request, (
-                "Reject can only be used if %s is provided" %
-                self.ensure_nonempty)
+                "Reject can only be used if %s is provided" % self.ensure_nonempty
+            )
 
         have_good_batch = False
         while not have_good_batch:
-
             batch = self.upstream_provider.request_batch(request)
 
             if self.mask:
                 mask_ratio = batch.arrays[self.mask].data.mean()
             else:
                 mask_ratio = None
 
             if self.ensure_nonempty:
-                num_points = len(
-                    list(batch.points[self.ensure_nonempty].nodes))
+                num_points = len(list(batch.graphs[self.ensure_nonempty].nodes))
             else:
                 num_points = None
 
             have_min_mask = mask_ratio is None or mask_ratio > self.min_masked
             have_points = num_points is None or num_points > 0
 
             have_good_batch = have_min_mask and have_points
 
-            if not have_good_batch and self.reject_probability < 1.:
+            if not have_good_batch and self.reject_probability < 1.0:
                 have_good_batch = random.random() > self.reject_probability
 
             if not have_good_batch:
                 if self.mask:
                     logger.debug(
                         "reject batch with mask ratio %f at %s",
-                        mask_ratio, batch.arrays[self.mask].spec.roi)
+                        mask_ratio,
+                        batch.arrays[self.mask].spec.roi,
+                    )
                 if self.ensure_nonempty:
                     logger.debug(
                         "reject batch with empty points in %s",
-                        batch.points[self.ensure_nonempty].spec.roi)
+                        batch.graphs[self.ensure_nonempty].spec.roi,
+                    )
                 num_rejected += 1
 
                 if timing.elapsed() > report_next_timeout:
-
                     logger.warning(
-                        "rejected %d batches, been waiting for a good one "
-                        "since %ds", num_rejected, report_next_timeout)
+                        "rejected %d batches, been waiting for a good one " "since %ds",
+                        num_rejected,
+                        report_next_timeout,
+                    )
                     report_next_timeout *= 2
 
             else:
                 if self.mask:
                     logger.debug(
                         "accepted batch with mask ratio %f at %s",
-                        mask_ratio, batch.arrays[self.mask].spec.roi)
+                        mask_ratio,
+                        batch.arrays[self.mask].spec.roi,
+                    )
                 if self.ensure_nonempty:
                     logger.debug(
                         "accepted batch with nonempty points in %s",
-                        self.ensure_nonempty)
+                        self.ensure_nonempty,
+                    )
 
         timing.stop()
         batch.profiling_stats.add(timing)
 
         return batch
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/scan.py` & `gunpowder-1.3.0/gunpowder/nodes/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from gunpowder.roi import Roi
 from .batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
 
 class Scan(BatchFilter):
-    '''Iteratively requests batches of size ``reference`` from upstream
+    """Iteratively requests batches of size ``reference`` from upstream
     providers in a scanning fashion, until all requested ROIs are covered. If
     the batch request to this node is empty, it will scan the complete upstream
     ROIs (and return nothing). Otherwise, it scans only the requested ROIs and
     returns a batch assembled of the smaller requests. In either case, the
     upstream requests will be contained in the downstream requested ROI or
     upstream ROIs.
 
@@ -36,151 +36,136 @@
 
             If set to >1, upstream requests are made in parallel with that
             number of workers.
 
         cache_size (``int``, optional):
 
             If multiple workers are used, how many batches to hold at most.
-    '''
+    """
 
     def __init__(self, reference, num_workers=1, cache_size=50):
-
         self.reference = reference.copy()
         self.num_workers = num_workers
         self.cache_size = cache_size
         self.workers = None
         self.batch = None
 
     def setup(self):
-
         if self.num_workers > 1:
             self.request_queue = multiprocessing.Queue(maxsize=0)
             self.workers = ProducerPool(
-                [self.__worker_get_chunk for _ in range(self.num_workers)],
-                queue_size=self.cache_size)
+                [self._worker_get_chunk for _ in range(self.num_workers)],
+                queue_size=self.cache_size,
+            )
             self.workers.start()
 
     def teardown(self):
-
         if self.num_workers > 1:
             self.workers.stop()
 
     def provide(self, request):
-
-        empty_request = (len(request) == 0)
+        empty_request = len(request) == 0
         if empty_request:
             scan_spec = self.spec
         else:
             scan_spec = request
 
-        stride = self.__get_stride()
-        shift_roi = self.__get_shift_roi(scan_spec)
+        stride = self._get_stride()
+        shift_roi = self._get_shift_roi(scan_spec)
 
-        shifts = self.__enumerate_shifts(shift_roi, stride)
+        shifts = self._enumerate_shifts(shift_roi, stride)
         num_chunks = len(shifts)
 
         logger.info("scanning over %d chunks", num_chunks)
 
         # the batch to return
         self.batch = Batch()
 
         if self.num_workers > 1:
-
             for shift in shifts:
-                shifted_reference = self.__shift_request(self.reference, shift)
+                shifted_reference = self._shift_request(self.reference, shift)
                 self.request_queue.put(shifted_reference)
 
             for i in tqdm.tqdm(range(num_chunks)):
-
                 chunk = self.workers.get()
 
                 if not empty_request:
-                    self.__add_to_batch(request, chunk)
+                    self._add_to_batch(request, chunk)
 
                 logger.debug("processed chunk %d/%d", i + 1, num_chunks)
 
         else:
-
-            for i, shift in tqdm.tqdm(enumerate(shifts)):
-
-                shifted_reference = self.__shift_request(self.reference, shift)
-                chunk = self.__get_chunk(shifted_reference)
+            for i, shift in enumerate(tqdm.tqdm(shifts)):
+                shifted_reference = self._shift_request(self.reference, shift)
+                chunk = self._get_chunk(shifted_reference)
 
                 if not empty_request:
-                    self.__add_to_batch(request, chunk)
+                    self._add_to_batch(request, chunk)
 
                 logger.debug("processed chunk %d/%d", i + 1, num_chunks)
 
         batch = self.batch
         self.batch = None
 
         logger.debug("returning batch %s", batch)
 
         return batch
 
-    def __get_stride(self):
-        '''Get the maximal amount by which ``reference`` can be moved, such
-        that it tiles the space.'''
+    def _get_stride(self):
+        """Get the maximal amount by which ``reference`` can be moved, such
+        that it tiles the space."""
 
         stride = None
 
         # get the least common multiple of all voxel sizes, we have to stride
         # at least that far
-        lcm_voxel_size = self.spec.get_lcm_voxel_size(
-            self.reference.array_specs.keys())
+        lcm_voxel_size = self.spec.get_lcm_voxel_size(self.reference.array_specs.keys())
 
         # that's just the minimal size in each dimension
         for key, reference_spec in self.reference.items():
-
-            shape = reference_spec.roi.get_shape()
+            shape = reference_spec.roi.shape
 
             for d in range(len(lcm_voxel_size)):
-                assert shape[d] >= lcm_voxel_size[d], ("Shape of reference "
-                                                       "ROI %s for %s is "
-                                                       "smaller than least "
-                                                       "common multiple of "
-                                                       "voxel size "
-                                                       "%s"%(reference_spec.roi,
-                                                             key,
-                                                             lcm_voxel_size))
+                assert shape[d] >= lcm_voxel_size[d], (
+                    "Shape of reference "
+                    "ROI %s for %s is "
+                    "smaller than least "
+                    "common multiple of "
+                    "voxel size "
+                    "%s" % (reference_spec.roi, key, lcm_voxel_size)
+                )
 
             if stride is None:
                 stride = shape
             else:
-                stride = Coordinate((
-                    min(a, b)
-                    for a, b in zip(stride, shape)))
+                stride = Coordinate((min(a, b) for a, b in zip(stride, shape)))
 
         return stride
 
-    def __get_shift_roi(self, spec):
-        '''Get the minimal and maximal shift (as a ROI) to apply to
+    def _get_shift_roi(self, spec):
+        """Get the minimal and maximal shift (as a ROI) to apply to
         ``self.reference``, such that it is still fully contained in ``spec``.
-        '''
+        """
 
         total_shift_roi = None
 
         # get individual shift ROIs and intersect them
         for key, reference_spec in self.reference.items():
-
-            logger.debug(
-                "getting shift roi for %s with spec %s",
-                key,
-                reference_spec)
+            logger.debug("getting shift roi for %s with spec %s", key, reference_spec)
 
             if key not in spec:
                 logger.debug("skipping, %s not in upstream spec", key)
                 continue
             if spec[key].roi is None:
                 logger.debug("skipping, %s has not ROI", key)
                 continue
 
             logger.debug("upstream ROI is %s", spec[key].roi)
 
-            for r, s in zip(reference_spec.roi.get_shape(), spec[key].roi.get_shape()):
+            for r, s in zip(reference_spec.roi.shape, spec[key].roi.shape):
                 assert s is None or r <= s, (
                     "reference %s with ROI %s does not fit into provided "
                     "upstream %s" % (key, reference_spec.roi, spec[key].roi)
                 )
 
             # we have a reference ROI
             #
@@ -206,191 +191,192 @@
             #              [-------) [8]
             #              13      21
             #
             # 1. the starting point is beginning of spec - beginning of reference
             # 2. the length is length of spec - length of reference + 1
 
             # 1. get the starting point of the shift ROI
-            shift_begin = (
-                spec[key].roi.get_begin() -
-                reference_spec.roi.get_begin())
+            shift_begin = spec[key].roi.begin - reference_spec.roi.begin
 
             # 2. get the shape of the shift ROI
-            shift_shape = (
-                spec[key].roi.get_shape() -
-                reference_spec.roi.get_shape() +
-                (1,)*reference_spec.roi.dims())
+            shift_shape = spec[key].roi.shape - reference_spec.roi.shape + 1
 
             # create a ROI...
             shift_roi = Roi(shift_begin, shift_shape)
 
             logger.debug("shift ROI for %s is %s", key, shift_roi)
 
             # ...and intersect it with previous shift ROIs
             if total_shift_roi is None:
                 total_shift_roi = shift_roi
             else:
                 total_shift_roi = total_shift_roi.intersect(shift_roi)
-                if total_shift_roi.empty():
-                    raise RuntimeError("There is no location where the ROIs "
-                                       "the reference %s are contained in the "
-                                       "request/upstream ROIs "
-                                       "%s."%(self.reference, spec))
+                if total_shift_roi.empty:
+                    raise RuntimeError(
+                        "There is no location where the ROIs "
+                        "the reference %s are contained in the "
+                        "request/upstream ROIs "
+                        "%s." % (self.reference, spec)
+                    )
 
-            logger.debug("intersected with total shift ROI this yields %s",
-                    total_shift_roi)
+            logger.debug(
+                "intersected with total shift ROI this yields %s", total_shift_roi
+            )
 
         if total_shift_roi is None:
-            raise RuntimeError("None of the upstream ROIs are bounded (all "
-                               "ROIs are None). Scan needs at least one "
-                               "bounded upstream ROI.")
+            raise RuntimeError(
+                "None of the upstream ROIs are bounded (all "
+                "ROIs are None). Scan needs at least one "
+                "bounded upstream ROI."
+            )
 
         return total_shift_roi
 
-    def __enumerate_shifts(self, shift_roi, stride):
-        '''Produces a sequence of shift coordinates starting at the beginning
+    def _enumerate_shifts(self, shift_roi, stride):
+        """Produces a sequence of shift coordinates starting at the beginning
         of ``shift_roi``, progressing with ``stride``. The maximum shift
         coordinate in any dimension will be the last point inside the shift roi
-        in this dimension.'''
+        in this dimension."""
 
-        min_shift = shift_roi.get_offset()
-        max_shift = max(min_shift,
-                        Coordinate(m - 1 for m in shift_roi.get_end()))
+        min_shift = shift_roi.offset
+        max_shift = max(min_shift, Coordinate(m - 1 for m in shift_roi.end))
 
         shift = np.array(min_shift)
         shifts = []
 
         dims = len(min_shift)
 
-        logger.debug(
-            "enumerating possible shifts of %s in %s", stride, shift_roi)
+        logger.debug("enumerating possible shifts of %s in %s", stride, shift_roi)
 
         while True:
-
             logger.debug("adding %s", shift)
             shifts.append(Coordinate(shift))
 
             if (shift == max_shift).all():
                 break
 
             # count up dimensions
             for d in range(dims):
-
                 if shift[d] >= max_shift[d]:
                     if d == dims - 1:
                         break
                     shift[d] = min_shift[d]
                 else:
                     shift[d] += stride[d]
                     # snap to last possible shift, don't overshoot
                     if shift[d] > max_shift[d]:
                         shift[d] = max_shift[d]
                     break
 
         return shifts
 
-    def __shift_request(self, request, shift):
-
+    def _shift_request(self, request, shift):
         shifted = request.copy()
         for _, spec in shifted.items():
             spec.roi = spec.roi.shift(shift)
 
         return shifted
 
-    def __worker_get_chunk(self):
-
+    def _worker_get_chunk(self):
         request = self.request_queue.get()
-        return self.__get_chunk(request)
-
-    def __get_chunk(self, request):
+        return self._get_chunk(request)
 
+    def _get_chunk(self, request):
         return self.get_upstream_provider().request_batch(request)
 
-    def __add_to_batch(self, spec, chunk):
-
+    def _add_to_batch(self, spec, chunk):
         if self.batch.get_total_roi() is None:
-            self.batch = self.__setup_batch(spec, chunk)
+            self.batch = self._setup_batch(spec, chunk)
         self.batch.profiling_stats.merge_with(chunk.profiling_stats)
 
-        for (array_key, array) in chunk.arrays.items():
+        for array_key, array in chunk.arrays.items():
             if array_key not in spec:
                 continue
-            self.__fill(self.batch.arrays[array_key].data, array.data,
-                        spec.array_specs[array_key].roi, array.spec.roi,
-                        self.spec[array_key].voxel_size)
+            self._fill(
+                self.batch.arrays[array_key].data,
+                array.data,
+                spec.array_specs[array_key].roi,
+                array.spec.roi,
+                self.spec[array_key].voxel_size,
+            )
 
-        for (graph_key, graphs) in chunk.graphs.items():
+        for graph_key, graphs in chunk.graphs.items():
             if graph_key not in spec:
                 continue
-            self.__fill_points(self.batch.graphs[graph_key], graphs,
-                               spec.graph_specs[graph_key].roi, graphs.spec.roi)
-
-    def __setup_batch(self, batch_spec, chunk):
-        '''Allocate a batch matching the sizes of ``batch_spec``, using
-        ``chunk`` as template.'''
+            self._fill_points(
+                self.batch.graphs[graph_key],
+                graphs,
+                spec.graph_specs[graph_key].roi,
+                graphs.spec.roi,
+            )
+
+    def _setup_batch(self, batch_spec, chunk):
+        """Allocate a batch matching the sizes of ``batch_spec``, using
+        ``chunk`` as template."""
 
         batch = Batch()
 
-        for (array_key, spec) in batch_spec.array_specs.items():
+        for array_key, spec in batch_spec.array_specs.items():
             roi = spec.roi
             voxel_size = self.spec[array_key].voxel_size
 
             # get the 'non-spatial' shape of the chunk-batch
             # and append the shape of the request to it
             array = chunk.arrays[array_key]
-            shape = array.data.shape[:-roi.dims()]
-            shape += (roi.get_shape() // voxel_size)
+            shape = array.data.shape[: -roi.dims]
+            shape += roi.shape // voxel_size
 
             spec = self.spec[array_key].copy()
             spec.roi = roi
             logger.info("allocating array of shape %s for %s", shape, array_key)
-            batch.arrays[array_key] = Array(data=np.zeros(shape, dtype=spec.dtype),
-                                                spec=spec)
+            batch.arrays[array_key] = Array(
+                data=np.zeros(shape, dtype=spec.dtype), spec=spec
+            )
 
-        for (graph_key, spec) in batch_spec.graph_specs.items():
+        for graph_key, spec in batch_spec.graph_specs.items():
             roi = spec.roi
             spec = self.spec[graph_key].copy()
             spec.roi = roi
             batch.graphs[graph_key] = Graph(nodes=[], edges=[], spec=spec)
 
         logger.debug("setup batch to fill %s", batch)
 
         return batch
 
-    def __fill(self, a, b, roi_a, roi_b, voxel_size):
+    def _fill(self, a, b, roi_a, roi_b, voxel_size):
         logger.debug("filling " + str(roi_b) + " into " + str(roi_a))
 
         roi_a = roi_a // voxel_size
         roi_b = roi_b // voxel_size
 
         common_roi = roi_a.intersect(roi_b)
-        if common_roi.empty():
+        if common_roi.empty:
             return
 
-        common_in_a_roi = common_roi - roi_a.get_offset()
-        common_in_b_roi = common_roi - roi_b.get_offset()
+        common_in_a_roi = common_roi - roi_a.offset
+        common_in_b_roi = common_roi - roi_b.offset
 
         slices_a = common_in_a_roi.get_bounding_box()
         slices_b = common_in_b_roi.get_bounding_box()
 
         if len(a.shape) > len(slices_a):
-            slices_a = (slice(None),)*(len(a.shape) - len(slices_a)) + slices_a
-            slices_b = (slice(None),)*(len(b.shape) - len(slices_b)) + slices_b
+            slices_a = (slice(None),) * (len(a.shape) - len(slices_a)) + slices_a
+            slices_b = (slice(None),) * (len(b.shape) - len(slices_b)) + slices_b
 
         a[slices_a] = b[slices_b]
 
-    def __fill_points(self, a, b, roi_a, roi_b):
+    def _fill_points(self, a, b, roi_a, roi_b):
         """
         Take points from b and add them to a.
         Nodes marked temporary must be ignored. Temporary nodes are nodes
         that were created during processing. Since it is impossible to know
         in general, that a node created during processing of a subgraph was
         not assigned an id that is already used by the full graph, we cannot
         include temporary nodes and assume there will not be ambiguous node
-        id's that correspond to multiple distinct nodes. 
+        id's that correspond to multiple distinct nodes.
         """
         logger.debug("filling points of " + str(roi_b) + " into points of" + str(roi_a))
 
         common_roi = roi_a.intersect(roi_b)
         if common_roi is None:
             return
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/shift_augment.py` & `gunpowder-1.3.0/gunpowder/nodes/shift_augment.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,29 @@
 
 from .batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
 
 class ShiftAugment(BatchFilter):
-    def __init__(
-            self,
-            prob_slip=0,
-            prob_shift=0,
-            sigma=0,
-            shift_axis=0):
-
+    def __init__(self, prob_slip=0, prob_shift=0, sigma=0, shift_axis=0):
         self.prob_slip = prob_slip
         self.prob_shift = prob_shift
         self.sigma = sigma
         self.shift_axis = shift_axis
 
         self.ndim = None
         self.shift_sigmas = None
         self.shift_array = None
         self.lcm_voxel_size = None
 
     def prepare(self, request):
         random.seed(request.random_seed)
-        
-        self.ndim = request.get_total_roi().dims()
+
+        self.ndim = request.get_total_roi().dims
         assert self.shift_axis in range(self.ndim)
 
         try:
             self.shift_sigmas = tuple(self.sigma)
         except TypeError:
             self.shift_sigmas = [float(self.sigma)] * self.ndim
             self.shift_sigmas[self.shift_axis] = 0.0
@@ -49,170 +43,218 @@
         for sigma in self.shift_sigmas:
             if sigma != 0.0:
                 has_nonzero = True
                 break
         assert has_nonzero
 
         if not request.array_specs:
-            raise ValueError("Request passed to Jitter node must contain at least one array key. " +
-                             "Check to make sure that Jitter node is not upstream of a RandomLocation node " +
-                             "with an ensure_nonempty argument.")
-
-        self.lcm_voxel_size = self.spec.get_lcm_voxel_size(array_keys=request.array_specs.keys())
+            raise ValueError(
+                "Request passed to Jitter node must contain at least one array key. "
+                + "Check to make sure that Jitter node is not upstream of a RandomLocation node "
+                + "with an ensure_nonempty argument."
+            )
+
+        self.lcm_voxel_size = self.spec.get_lcm_voxel_size(
+            array_keys=request.array_specs.keys()
+        )
         assert self.lcm_voxel_size
 
-        roi_shape = request.get_total_roi().get_shape()
-        assert roi_shape // self.lcm_voxel_size * self.lcm_voxel_size == roi_shape, \
-            "total roi shape {} must be divisible by least common voxel size {}".format(roi_shape, self.lcm_voxel_size)
+        roi_shape = request.get_total_roi().shape
+        assert (
+            roi_shape // self.lcm_voxel_size * self.lcm_voxel_size == roi_shape
+        ), "total roi shape {} must be divisible by least common voxel size {}".format(
+            roi_shape, self.lcm_voxel_size
+        )
         roi_shape_adjusted = roi_shape // self.lcm_voxel_size
         shift_axis_len = roi_shape_adjusted[self.shift_axis]
 
-        self.shift_array = self.construct_global_shift_array(shift_axis_len,
-                                                             self.shift_sigmas,
-                                                             self.prob_slip,
-                                                             self.prob_shift,
-                                                             self.lcm_voxel_size)
+        self.shift_array = self.construct_global_shift_array(
+            shift_axis_len,
+            self.shift_sigmas,
+            self.prob_slip,
+            self.prob_shift,
+            self.lcm_voxel_size,
+        )
 
         for key, spec in request.items():
-            sub_shift_array = self.get_sub_shift_array(request.get_total_roi(), spec.roi,
-                                                       self.shift_array, self.shift_axis, self.lcm_voxel_size)
+            sub_shift_array = self.get_sub_shift_array(
+                request.get_total_roi(),
+                spec.roi,
+                self.shift_array,
+                self.shift_axis,
+                self.lcm_voxel_size,
+            )
             updated_roi = self.compute_upstream_roi(spec.roi, sub_shift_array)
-            spec.roi.set_offset(updated_roi.get_offset())
-            spec.roi.set_shape(updated_roi.get_shape())
+            spec.roi.offset = updated_roi.offset
+            spec.roi.shape = updated_roi.shape
             request[key] = spec
 
         deps = request
         return deps
 
     def process(self, batch, request):
         for array_key, array in batch.arrays.items():
-            sub_shift_array = self.get_sub_shift_array(request.get_total_roi(), array.spec.roi,
-                                                       self.shift_array, self.shift_axis, self.lcm_voxel_size)
-            array.data = self.shift_and_crop(array.data,
-                                             request[array_key].roi.get_shape(),
-                                             sub_shift_array,
-                                             array.spec.voxel_size)
+            sub_shift_array = self.get_sub_shift_array(
+                request.get_total_roi(),
+                array.spec.roi,
+                self.shift_array,
+                self.shift_axis,
+                self.lcm_voxel_size,
+            )
+            array.data = self.shift_and_crop(
+                array.data,
+                request[array_key].roi.shape,
+                sub_shift_array,
+                array.spec.voxel_size,
+            )
             array.spec.roi = request[array_key].roi
-            assert request[array_key].roi.get_shape() == Coordinate(array.data.shape) * self.lcm_voxel_size, \
-                'request roi shape {} is not the same as generated array shape {}'.format(
-                    request[array_key].roi.get_shape(), array.data.shape)
+            assert (
+                request[array_key].roi.shape
+                == Coordinate(array.data.shape) * self.lcm_voxel_size
+            ), "request roi shape {} is not the same as generated array shape {}".format(
+                request[array_key].roi.shape, array.data.shape
+            )
             batch[array_key] = array
 
         for points_key, points in batch.graphs.items():
-            sub_shift_array = self.get_sub_shift_array(request.get_total_roi(), points.spec.roi,
-                                                       self.shift_array, self.shift_axis, self.lcm_voxel_size)
-            points = self.shift_points(points,
-                                       request[points_key].roi,
-                                       sub_shift_array,
-                                       self.shift_axis,
-                                       self.lcm_voxel_size)
+            sub_shift_array = self.get_sub_shift_array(
+                request.get_total_roi(),
+                points.spec.roi,
+                self.shift_array,
+                self.shift_axis,
+                self.lcm_voxel_size,
+            )
+            points = self.shift_points(
+                points,
+                request[points_key].roi,
+                sub_shift_array,
+                self.shift_axis,
+                self.lcm_voxel_size,
+            )
             batch[points_key] = points
 
     def shift_and_crop(self, arr, roi_shape, sub_shift_array, voxel_size):
-        """ Shift an array received from upstream and crop it to the target downstream region
+        """Shift an array received from upstream and crop it to the target downstream region
 
         :param arr: an array of upstream data to be shifted and cropped
         :param roi_shape: the shape of the downstream ROI
         :param sub_shift_array: the cropped section of the global shift array that applies to this specific request
         :param voxel_size: the voxel sizes of the data in the array
         :return: an array of shape roi_shape that contains the array to be passed downstream
         """
 
         array_shift_axis_len = arr.shape[self.shift_axis]
         sub_shift_array_len = len(sub_shift_array)
-        assert array_shift_axis_len % sub_shift_array_len == 0, \
-            "array shift axis length {} is not divisible by the sub_shift_array length {}".format(
-                arr.shape[self.shift_axis], sub_shift_array.shape[0])
+        assert (
+            array_shift_axis_len % sub_shift_array_len == 0
+        ), "array shift axis length {} is not divisible by the sub_shift_array length {}".format(
+            arr.shape[self.shift_axis], sub_shift_array.shape[0]
+        )
 
         voxel_ratio = array_shift_axis_len // sub_shift_array_len
 
         # assumption: each sub shift array element divides evenly by the voxel size
         rescaled_sub_shift_array = sub_shift_array // np.array(voxel_size, dtype=int)
 
         max_shift = rescaled_sub_shift_array.max(axis=0)
         batch = arr.copy()
         batch_view = np.moveaxis(batch, self.shift_axis, 0)
         for index, plane in enumerate(batch_view):
             adjusted_index = index // voxel_ratio
             shift = rescaled_sub_shift_array[adjusted_index, :] - max_shift
             shift = np.delete(shift, self.shift_axis, axis=0)
-            assert(len(shift) == plane.ndim)
+            assert len(shift) == plane.ndim
             plane = np.roll(plane, shift, axis=tuple(range(len(shift))))
             batch_view[index] = plane
 
         adjusted_roi_shape = Coordinate(roi_shape) // Coordinate(voxel_size)
 
         sl = tuple(slice(0, adjusted_roi_shape[index]) for index in range(self.ndim))
         return batch[sl]
 
     @staticmethod
     def shift_points(points, request_roi, sub_shift_array, shift_axis, lcm_voxel_size):
-        """ Shift a set of points received from upstream and crop out those not the the target downstream region
+        """Shift a set of points received from upstream and crop out those not the the target downstream region
 
         :param points: the points from upstream
         :param request_roi: the downstream ROI
         :param sub_shift_array: the cropped section of the global shift array that applies to this specific request
         :param shift_axis: the axis to perform the shift along
         :param lcm_voxel_size: the least common voxel size for the arrays in the request
         :return a Graph object with the updated point locations and ROI
         """
 
         nodes = list(points.nodes)
         spec = points.spec
-        shift_axis_start_pos = spec.roi.get_offset()[shift_axis]
+        shift_axis_start_pos = spec.roi.offset[shift_axis]
 
         for node in nodes:
             loc = node.location
             shift_axis_position = loc[shift_axis]
-            shift_array_index = int((shift_axis_position - shift_axis_start_pos) // lcm_voxel_size[shift_axis])
-            assert(shift_array_index >= 0)
+            shift_array_index = int(
+                (shift_axis_position - shift_axis_start_pos)
+                // lcm_voxel_size[shift_axis]
+            )
+            assert shift_array_index >= 0
             shift = Coordinate(sub_shift_array[shift_array_index])
             loc += shift
             if not request_roi.contains(loc):
                 points.remove_node(node)
 
         points.spec.roi = request_roi
         return points
 
     @staticmethod
-    def get_sub_shift_array(total_roi, item_roi, shift_array, shift_axis, lcm_voxel_size):
-        """ Slices the global shift array to return the sub-shift array to shift an item in the request
+    def get_sub_shift_array(
+        total_roi, item_roi, shift_array, shift_axis, lcm_voxel_size
+    ):
+        """Slices the global shift array to return the sub-shift array to shift an item in the request
 
         :param total_roi: the total roi of the request
         :param item_roi: the roi of the item (array or points) being shifted
         :param shift_array: the shift array for the total_roi
         :param shift_axis: the axis along which we are shifting
         :param lcm_voxel_size: the least common voxel size for the arrays in the request
         :return: the portion of the global shift array that should be used to shift the item
         """
-        item_offset_from_total = item_roi.get_offset() - total_roi.get_offset()
-        offset_in_shift_axis = item_offset_from_total[shift_axis] // lcm_voxel_size[shift_axis]
-        len_in_shift_axis = item_roi.get_shape()[shift_axis] // lcm_voxel_size[shift_axis]
-        return shift_array[offset_in_shift_axis: offset_in_shift_axis + len_in_shift_axis]
+        item_offset_from_total = item_roi.offset - total_roi.offset
+        offset_in_shift_axis = (
+            item_offset_from_total[shift_axis] // lcm_voxel_size[shift_axis]
+        )
+        len_in_shift_axis = item_roi.shape[shift_axis] // lcm_voxel_size[shift_axis]
+        return shift_array[
+            offset_in_shift_axis : offset_in_shift_axis + len_in_shift_axis
+        ]
 
     @staticmethod
-    def construct_global_shift_array(shift_axis_len, shift_sigmas, prob_slip, prob_shift, lcm_voxel_size):
-        """ Sets the attribute variable self.shift_array
+    def construct_global_shift_array(
+        shift_axis_len, shift_sigmas, prob_slip, prob_shift, lcm_voxel_size
+    ):
+        """Sets the attribute variable self.shift_array
 
         :param shift_axis_len: the length of the shift axis
         :param shift_sigmas: the sigma to generate the normal distribution of shift amounts in each direction
         :param prob_slip: the probability of the slice shifting independently of all other slices
         :param prob_shift: the probability of the slice and all following slices shifting
         :param lcm_voxel_size: the least common voxel size of all the arrays in the request
         :return: the shift_array for the total_roi
         """
         # each row is one slice along shift axis
         shift_array = np.zeros(shape=(shift_axis_len, len(shift_sigmas)), dtype=int)
         base_shift = np.zeros(shape=len(shift_sigmas), dtype=int)
-        assert(prob_slip + prob_shift <= 1)
+        assert prob_slip + prob_shift <= 1
 
         for shift_axis_position in range(shift_axis_len):
             r = random.random()
-            slip = np.array([np.random.normal(scale=sigma / lcm_voxel_size[dimension])
-                             for dimension, sigma in enumerate(shift_sigmas)])
+            slip = np.array(
+                [
+                    np.random.normal(scale=sigma / lcm_voxel_size[dimension])
+                    for dimension, sigma in enumerate(shift_sigmas)
+                ]
+            )
             slip = np.rint(slip).astype(int)
             slip = slip * np.array(lcm_voxel_size, dtype=int)
 
             if r <= prob_slip:
                 shift_array[shift_axis_position] = base_shift + slip
             elif r <= prob_slip + prob_shift:
                 base_shift += slip
@@ -220,21 +262,21 @@
             else:
                 shift_array[shift_axis_position] = base_shift
 
         return shift_array
 
     @staticmethod
     def compute_upstream_roi(request_roi, sub_shift_array):
-        """ Compute the ROI to pass upstream for a specific item (array or points) in a request
+        """Compute the ROI to pass upstream for a specific item (array or points) in a request
 
         :param request_roi: the downstream ROI passed to the Jitter node
         :param sub_shift_array: the portion of the global shift array that should be used to shift the item
         :return: the expanded ROI to pass upstream
         """
 
         max_shift = Coordinate(sub_shift_array.max(axis=0))
         min_shift = Coordinate(sub_shift_array.min(axis=0))
 
-        downstream_offset = request_roi.get_offset()
+        downstream_offset = request_roi.offset
         upstream_offset = downstream_offset - max_shift
-        upstream_shape = request_roi.get_shape() + max_shift - min_shift
+        upstream_shape = request_roi.shape + max_shift - min_shift
         return Roi(offset=upstream_offset, shape=upstream_shape)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/simple_augment.py` & `gunpowder-1.3.0/gunpowder/nodes/simple_augment.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,24 @@
     def __init__(
         self,
         mirror_only=None,
         transpose_only=None,
         mirror_probs=None,
         transpose_probs=None,
     ):
-
         self.mirror_only = mirror_only
         self.mirror_probs = mirror_probs
         self.transpose_only = transpose_only
         self.transpose_probs = transpose_probs
         self.mirror_mask = None
         self.dims = None
         self.transpose_dims = None
 
     def setup(self):
-
-        self.dims = self.spec.get_total_roi().dims()
+        self.dims = self.spec.get_total_roi().dims
 
         # mirror_mask and transpose_dims refer to the indices of the spatial
         # dimensions only, starting counting at 0 for the first spatial
         # dimension
 
         if self.mirror_only is None:
             self.mirror_mask = [True] * self.dims
@@ -141,22 +139,21 @@
         self.__mirror_request(request, self.mirror)
 
         logger.debug("upstream request = %s", request)
 
         return request
 
     def process(self, batch, request):
-
         # mirror and transpose ROIs of arrays & points in batch
         total_roi = batch.get_total_roi().copy()
         requested_keys = request.array_specs.keys()
         lcm_voxel_size = self.spec.get_lcm_voxel_size(requested_keys)
 
         for collection_type in [batch.arrays, batch.graphs]:
-            for (key, collector) in collection_type.items():
+            for key, collector in collection_type.items():
                 if key not in request:
                     continue
                 if collector.spec.roi is None:
                     continue
                 logger.debug("total ROI = %s", batch.get_total_roi())
                 logger.debug("upstream %s ROI = %s", key, collector.spec.roi)
                 self.__mirror_roi(collector.spec.roi, total_roi, self.mirror)
@@ -164,16 +161,15 @@
                 self.__transpose_roi(
                     collector.spec.roi, total_roi, self.transpose, lcm_voxel_size
                 )
                 logger.debug("transposed %s ROI = %s", key, collector.spec.roi)
 
         mirror = tuple(slice(None, None, -1 if m else 1) for m in self.mirror)
         # arrays
-        for (array_key, array) in batch.arrays.items():
-
+        for array_key, array in batch.arrays.items():
             if array_key not in request:
                 continue
 
             if array.spec.nonspatial:
                 continue
 
             num_channels = len(array.data.shape) - self.dims
@@ -183,32 +179,30 @@
 
             transpose = [t + num_channels for t in self.transpose]
             array.data = array.data = array.data.transpose(
                 list(range(num_channels)) + transpose
             )
 
         # graphs
-        total_roi_offset = total_roi.get_offset()
-        total_roi_center = total_roi.get_center()
+        total_roi_offset = total_roi.offset
+        total_roi_center = total_roi.center
         if lcm_voxel_size is not None:
             nearest_voxel_shift = Coordinate(
                 (d % v) for d, v in zip(total_roi_center, lcm_voxel_size)
             )
             total_roi_center = total_roi_center - nearest_voxel_shift
-        total_roi_end = total_roi.get_end()
+        total_roi_end = total_roi.end
         logger.debug("augmenting in %s and center %s", total_roi, total_roi_center)
 
-        for (graph_key, graph) in batch.graphs.items():
-
+        for graph_key, graph in batch.graphs.items():
             if graph_key not in request:
                 continue
 
             logger.debug("converting nodes in graph %s", graph_key)
             for node in list(graph.nodes):
-
                 logger.debug("old location: %s, %s", node.id, node.location)
 
                 # mirror
                 location_in_total_offset = np.asarray(node.location) - total_roi_offset
                 node.location = np.asarray(
                     [
                         total_roi_end[dim] - location_in_total_offset[dim]
@@ -235,68 +229,65 @@
 
                 # due to the mirroring, points at the lower boundary of the ROI
                 # could fall on the upper one, which excludes them from the ROI
                 if not graph.spec.roi.contains(node.location):
                     graph.remove_node(node)
 
     def __mirror_request(self, request, mirror):
-
         total_roi = request.get_total_roi().copy()
         for key, spec in request.items():
             if spec.roi is not None:
                 self.__mirror_roi(spec.roi, total_roi, mirror)
 
     def __transpose_request(self, request, transpose):
         total_roi = request.get_total_roi().copy()
         requested_keys = request.array_specs.keys()
         lcm_voxel_size = self.spec.get_lcm_voxel_size(requested_keys)
         for key, spec in request.items():
             if spec.roi is not None:
                 self.__transpose_roi(spec.roi, total_roi, transpose, lcm_voxel_size)
 
     def __mirror_roi(self, roi, total_roi, mirror):
+        total_roi_offset = total_roi.offset
+        total_roi_shape = total_roi.shape
 
-        total_roi_offset = total_roi.get_offset()
-        total_roi_shape = total_roi.get_shape()
-
-        roi_offset = roi.get_offset()
-        roi_shape = roi.get_shape()
+        roi_offset = roi.offset
+        roi_shape = roi.shape
 
         roi_in_total_offset = roi_offset - total_roi_offset
         end_of_roi_in_total = roi_in_total_offset + roi_shape
         roi_in_total_offset_mirrored = total_roi_shape - end_of_roi_in_total
         roi_offset = Coordinate(
             total_roi_offset[d] + roi_in_total_offset_mirrored[d]
             if mirror[d]
             else roi_offset[d]
             for d in range(self.dims)
         )
 
-        roi.set_offset(roi_offset)
+        roi.offset = roi_offset
 
     def __transpose_roi(self, roi, total_roi, transpose, lcm_voxel_size):
-
         logger.debug("original roi = %s", roi)
 
-        center = total_roi.get_center()
+        center = total_roi.center
         if lcm_voxel_size is not None:
             nearest_voxel_shift = Coordinate(
                 (d % v) for d, v in zip(center, lcm_voxel_size)
             )
             center = center - nearest_voxel_shift
         logger.debug("center = %s", center)
 
         # Get distance from center, then transpose
-        dist_to_center = center - roi.get_offset()
+        dist_to_center = center - roi.offset
         dist_to_center = Coordinate(
             dist_to_center[transpose[d]] for d in range(self.dims)
         )
         logger.debug("dist_to_center = %s", dist_to_center)
 
         # Using the tranposed distance to center, get the correct offset.
         new_offset = center - dist_to_center
         logger.debug("new_offset = %s", new_offset)
 
-        shape = tuple(roi.get_shape()[transpose[d]] for d in range(self.dims))
-        roi.set_offset(new_offset)
-        roi.set_shape(shape)
+        shape = tuple(roi.shape[transpose[d]] for d in range(self.dims))
+        roi.offset = new_offset
+        roi.shape = shape
         logger.debug("tranposed roi = %s", roi)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/snapshot.py` & `gunpowder-1.3.0/gunpowder/nodes/snapshot.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Snapshot(BatchFilter):
     """Save a passing batch in an HDF file.
 
+    The default behaviour is to periodically save a snapshot after
+    ``every`` iterations.
+
+    Data-dependent criteria for saving can be implemented by subclassing and
+    overwriting :func:`write_if`. This method is applied as an additional
+    filter to the batches picked for periodic saving. It should return ``True``
+    if a batch meets the criteria for saving.
+
     Args:
 
         dataset_names (``dict``, :class:`ArrayKey` -> ``string``):
 
             A dictionary from array keys to names of the datasets to store them
             in.
 
@@ -56,15 +64,15 @@
             A dictionary from array keys to datatype (eg. ``np.int8``). If
             given, arrays are stored using this type. The original arrays
             within the pipeline remain unchanged.
 
         store_value_range (``bool``):
 
             If set to ``True``, store range of values in data set attributes.
-        """
+    """
 
     def __init__(
         self,
         dataset_names,
         output_dir="snapshots",
         output_filename="{id}.zarr",
         every=1,
@@ -86,29 +94,48 @@
         if dataset_dtypes is None:
             self.dataset_dtypes = {}
         else:
             self.dataset_dtypes = dataset_dtypes
 
         self.mode = "w"
 
-    def setup(self):
+    def write_if(self, batch):
+        """To be implemented in subclasses.
+
+        This function is run in :func:`process` and acts as a data-dependent
+        filter for saving snapshots.
 
+        Args:
+
+            batch (:class:`Batch`):
+
+                The batch received from upstream.
+
+        Returns:
+
+            ``True`` if ``batch`` should be written to snapshot, ``False``
+            otherwise.
+        """
+
+        return True
+
+    def setup(self):
         for key, _ in self.additional_request.items():
             assert key in self.dataset_names, (
-                "%s requested but not in dataset_names"% key)
+                "%s requested but not in dataset_names" % key
+            )
 
         for array_key in self.additional_request.array_specs.keys():
             spec = self.spec[array_key]
             self.updates(array_key, spec)
         for graph_key in self.additional_request.graph_specs.keys():
             spec = self.spec[graph_key]
             self.updates(graph_key, spec)
 
     def prepare(self, request):
-
         deps = BatchRequest()
         for key, spec in request.items():
             if key in self.dataset_names:
                 deps[key] = spec
 
         self.record_snapshot = self.n % self.every == 0
 
@@ -118,24 +145,23 @@
                 if array_key not in deps:
                     deps[array_key] = spec
             for graph_key, spec in self.additional_request.graph_specs.items():
                 if graph_key not in deps:
                     deps[graph_key] = spec
 
             for key in self.dataset_names.keys():
-                assert key in deps, (
-                    "%s wanted for %s, but not in request." %
-                    (key, self.name()))
+                assert key in deps, "%s wanted for %s, but not in request." % (
+                    key,
+                    self.name(),
+                )
 
         return deps
 
     def process(self, batch, request):
-
-        if self.record_snapshot:
-
+        if self.record_snapshot and self.write_if(batch):
             try:
                 os.makedirs(self.output_dir)
             except:
                 pass
 
             snapshot_name = os.path.join(
                 self.output_dir,
@@ -149,16 +175,15 @@
             elif snapshot_name.endswith(".zarr"):
                 open_func = ZarrFile
             else:
                 logger.warning("ambiguous file type")
                 open_func = h5py.File
 
             with open_func(snapshot_name, self.mode) as f:
-                for (array_key, array) in batch.arrays.items():
-
+                for array_key, array in batch.arrays.items():
                     if array_key not in self.dataset_names:
                         continue
 
                     ds_name = self.dataset_names[array_key]
 
                     if array_key in self.dataset_dtypes:
                         dtype = self.dataset_dtypes[array_key]
@@ -173,28 +198,28 @@
                             name=ds_name,
                             data=array.data,
                             compression=self.compression_type,
                         )
 
                     if not array.spec.nonspatial:
                         if array.spec.roi is not None:
-                            dataset.attrs["offset"] = array.spec.roi.get_offset()
+                            dataset.attrs["offset"] = array.spec.roi.offset
                         dataset.attrs["resolution"] = self.spec[array_key].voxel_size
 
                     if self.store_value_range:
                         dataset.attrs["value_range"] = (
                             np.asscalar(array.data.min()),
                             np.asscalar(array.data.max()),
                         )
 
                     # if array has attributes, add them to the dataset
                     for attribute_name, attribute in array.attrs.items():
                         dataset.attrs[attribute_name] = attribute
 
-                for (graph_key, graph) in batch.graphs.items():
+                for graph_key, graph in batch.graphs.items():
                     if graph_key not in self.dataset_names:
                         continue
 
                     ds_name = self.dataset_names[graph_key]
 
                     node_ids = []
                     locations = []
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/specified_location.py` & `gunpowder-1.3.0/gunpowder/nodes/specified_location.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from gunpowder.coordinate import Coordinate
 from gunpowder.batch_request import BatchRequest
 
 from .batch_filter import BatchFilter
 
 logger = logging.getLogger(__name__)
 
+
 class SpecifiedLocation(BatchFilter):
-    '''Choses a batch at a location from the list provided at init, making sure
+    """Choses a batch at a location from the list provided at init, making sure
     it is in the bounding box of the upstream provider.
 
     Locations should be given in world units.
 
     Locations will be chosen in order or at random from the list depending on the
     ``choose_randomly`` parameter.
 
@@ -41,80 +42,83 @@
 
         jitter (``tuple`` of int):
 
             How far to allow the point to shift in each direction.
             Default is None, which places the point in the center.
             Chooses uniformly from [loc - jitter, loc + jitter] in each
             direction.
-    '''
-
-    def __init__(self, locations, choose_randomly=False, extra_data=None,
-                 jitter=None):
+    """
 
+    def __init__(self, locations, choose_randomly=False, extra_data=None, jitter=None):
         self.coordinates = locations
         self.choose_randomly = choose_randomly
         self.jitter = jitter
         self.loc_i = -1
         self.upstream_spec = None
         self.specified_shift = None
 
         if extra_data is not None:
-            assert len(extra_data) == len(locations),\
-                "extra_data (%d) should match the length of specified locations (%d)"%(len(extra_data),\
-                len(locations))
+            assert len(extra_data) == len(locations), (
+                "extra_data (%d) should match the length of specified locations (%d)"
+                % (len(extra_data), len(locations))
+            )
 
         self.extra_data = extra_data
 
     def setup(self):
-
         self.upstream_spec = self.get_upstream_provider().spec
 
         # clear bounding boxes of all provided arrays and points --
         # SpecifiedLocation does know its locations at setup (checks on the fly)
         for key, spec in self.spec.items():
-            spec.roi.set_shape(None)
+            spec.roi.shape = (None,) * spec.roi.dims
             self.updates(key, spec)
 
     def prepare(self, request):
         seed(request.random_seed)
         np.random.seed(request.random_seed)
-        lcm_voxel_size = self.spec.get_lcm_voxel_size(
-            request.array_specs.keys())
+        lcm_voxel_size = self.spec.get_lcm_voxel_size(request.array_specs.keys())
 
         # shift to center
         total_roi = request.get_total_roi()
-        request_center = total_roi.get_shape()/2 + total_roi.get_offset()
+        request_center = total_roi.shape / 2 + total_roi.offset
 
         self.specified_shift = self._get_next_shift(request_center, lcm_voxel_size)
         while not self.__check_shift(request):
-            logger.warning("Location %s (shift %s) skipped"
-                           % (self.coordinates[self.loc_i], self.specified_shift))
+            logger.warning(
+                "Location %s (shift %s) skipped"
+                % (self.coordinates[self.loc_i], self.specified_shift)
+            )
             self.specified_shift = self._get_next_shift(request_center, lcm_voxel_size)
 
         # Set shift for all requests
         for specs_type in [request.array_specs, request.graph_specs]:
-            for (key, spec) in specs_type.items():
+            for key, spec in specs_type.items():
                 roi = spec.roi.shift(self.specified_shift)
                 specs_type[key].roi = roi
 
-        logger.debug("{}'th ({}) shift selected: {}".format(
-            self.loc_i, self.coordinates[self.loc_i], self.specified_shift))
+        logger.debug(
+            "{}'th ({}) shift selected: {}".format(
+                self.loc_i, self.coordinates[self.loc_i], self.specified_shift
+            )
+        )
 
         deps = request
         return deps
 
     def process(self, batch, request):
         # reset ROIs to request
-        for (array_key, spec) in request.array_specs.items():
+        for array_key, spec in request.array_specs.items():
             batch.arrays[array_key].spec.roi = spec.roi
             if self.extra_data is not None:
-                batch.arrays[array_key].attrs['specified_location_extra_data'] =\
-                 self.extra_data[self.loc_i]
+                batch.arrays[array_key].attrs[
+                    "specified_location_extra_data"
+                ] = self.extra_data[self.loc_i]
 
-        for (graph_key, spec) in request.graph_specs.items():
+        for graph_key, spec in request.graph_specs.items():
             batch.points[graph_key].spec.roi = spec.roi
 
         # change shift point locations to lie within roi
         for graph_key in request.graph_specs.keys():
             batch.points[graph_key].shift(-self.specified_shift)
 
     def _get_next_shift(self, center_shift, voxel_size):
@@ -122,36 +126,41 @@
 
         if self.choose_randomly:
             self.loc_i = randrange(len(self.coordinates))
         else:
             self.loc_i += 1
             if self.loc_i >= len(self.coordinates):
                 self.loc_i = 0
-                logger.warning('Ran out of specified locations, looping list')
+                logger.warning("Ran out of specified locations, looping list")
         next_shift = Coordinate(self.coordinates[self.loc_i]) - center_shift
 
         if self.jitter is not None:
             rnd = []
             for i in range(len(self.jitter)):
-                rnd.append(np.random.randint(-self.jitter[i],
-                                              self.jitter[i]+1))
+                rnd.append(np.random.randint(-self.jitter[i], self.jitter[i] + 1))
             next_shift += Coordinate(rnd)
         logger.debug("Shift before rounding: %s" % str(next_shift))
         # make sure shift is a multiple of voxel size (round to nearest)
-        next_shift = Coordinate([int(vs * round(float(shift)/vs)) for vs, shift in zip(voxel_size, next_shift)])
+        next_shift = Coordinate(
+            [
+                int(vs * round(float(shift) / vs))
+                for vs, shift in zip(voxel_size, next_shift)
+            ]
+        )
         logger.debug("Shift after rounding: %s" % str(next_shift))
         return next_shift
 
     def __check_shift(self, request):
         for key, spec in request.items():
             request_roi = spec.roi
             if key in self.upstream_spec:
                 provided_roi = self.upstream_spec[key].roi
             else:
-                raise Exception(
-                    "Requested %s, but upstream does not provide it."%key)
+                raise Exception("Requested %s, but upstream does not provide it." % key)
             shifted_roi = request_roi.shift(self.specified_shift)
             if not provided_roi.contains(shifted_roi):
-                logger.warning("Provided roi %s for key %s does not contain shifted roi %s"
-                             % (provided_roi, key, shifted_roi))
+                logger.warning(
+                    "Provided roi %s for key %s does not contain shifted roi %s"
+                    % (provided_roi, key, shifted_roi)
+                )
                 return False
         return True
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/squeeze.py` & `gunpowder-1.3.0/gunpowder/nodes/squeeze.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,24 @@
             if array in request:
                 deps[array] = request[array].copy()
         return deps
 
     def process(self, batch, request):
         outputs = Batch()
         for array in self.arrays:
-
             if array in batch:
                 if not batch[array].spec.nonspatial:
-                    spatial_dims = request[array].roi.dims()
+                    spatial_dims = request[array].roi.dims
                     if self.axis >= batch[array].data.ndim - spatial_dims:
-                        raise ValueError((
-                            f"Squeeze.axis={self.axis} not permitted. "
-                            "Squeeze only supported for "
-                            "non-spatial dimensions of Array."
-                        ))
+                        raise ValueError(
+                            (
+                                f"Squeeze.axis={self.axis} not permitted. "
+                                "Squeeze only supported for "
+                                "non-spatial dimensions of Array."
+                            )
+                        )
 
-                outputs[array] = copy.deepcopy(batch[array])
+                outputs[array] = batch[array]
                 outputs[array].data = np.squeeze(batch[array].data, self.axis)
-                logger.debug(f'{array} shape: {outputs[array].data.shape}')
+                logger.debug(f"{array} shape: {outputs[array].data.shape}")
 
         return outputs
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/stack.py` & `gunpowder-1.3.0/gunpowder/nodes/stack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 from .batch_filter import BatchFilter
 from gunpowder.array import Array
 from gunpowder.batch import Batch
 from gunpowder.profiling import Timing
 import numpy as np
 
+
 class Stack(BatchFilter):
-    '''Request several batches and stack them together, introducing a new
+    """Request several batches and stack them together, introducing a new
     dimension for each array. This is useful to create batches with several
     samples and only makes sense if there is a source of randomness upstream.
 
     This node stacks only arrays, not points. The resulting batch will have the
     same point sets as found in the first batch requested upstream.
 
     Args:
 
         num_repetitions (``int``):
 
             How many upstream batches to stack.
-    '''
+    """
 
     def __init__(self, num_repetitions):
-
         self.num_repetitions = num_repetitions
 
     def provide(self, request):
-
         batches = [
             self.get_upstream_provider().request_batch(request)
             for _ in range(self.num_repetitions)
         ]
 
         timing = Timing(self)
         timing.start()
 
         batch = Batch()
         for b in batches:
             batch.profiling_stats.merge_with(b.profiling_stats)
 
         for key, spec in request.array_specs.items():
-
             data = np.stack([b[key].data for b in batches])
-            batch[key] = Array(
-                data,
-                batches[0][key].spec.copy())
+            batch[key] = Array(data, batches[0][key].spec.copy())
 
         # copy points of first batch requested
         for key, spec in request.points_specs.items():
             batch[key] = batches[0][key]
 
         timing.stop()
         batch.profiling_stats.add(timing)
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/unsqueeze.py` & `gunpowder-1.3.0/gunpowder/nodes/unsqueeze.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,18 +38,20 @@
         return deps
 
     def process(self, batch, request):
         outputs = Batch()
         for array in self.arrays:
             if array in batch:
                 if not batch[array].spec.nonspatial:
-                    spatial_dims = request[array].roi.dims()
+                    spatial_dims = request[array].roi.dims
                     if self.axis > batch[array].data.ndim - spatial_dims:
-                        raise ValueError((
-                            f"Unsqueeze.axis={self.axis} not permitted. "
-                            "Unsqueeze only supported for "
-                            "non-spatial dimensions of Array."
-                        ))
+                        raise ValueError(
+                            (
+                                f"Unsqueeze.axis={self.axis} not permitted. "
+                                "Unsqueeze only supported for "
+                                "non-spatial dimensions of Array."
+                            )
+                        )
 
-                outputs[array] = copy.deepcopy(batch[array])
+                outputs[array] = batch[array]
                 outputs[array].data = np.expand_dims(batch[array].data, self.axis)
         return outputs
```

### Comparing `gunpowder-1.2.2/gunpowder/nodes/upsample.py` & `gunpowder-1.3.0/gunpowder/nodes/upsample.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,69 +6,74 @@
 from gunpowder.batch import Batch
 import logging
 import numbers
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
+
 class UpSample(BatchFilter):
-    '''Upsample arrays in a batch by given factors.
+    """Upsample arrays in a batch by given factors.
 
     Args:
 
         source (:class:`ArrayKey`):
 
             The key of the array to upsample.
 
-        factor (``int`` or ``tuple`` of ``int``):
+        factor (``int`` or ``Coordinate``):
 
             The factor to upsample with.
 
         target (:class:`ArrayKey`):
 
             The key of the array to store the upsampled ``source``.
-    '''
+    """
 
     def __init__(self, source, factor, target):
-
         assert isinstance(source, ArrayKey)
         assert isinstance(target, ArrayKey)
-        assert (
-            isinstance(factor, numbers.Number) or isinstance(factor, tuple)), (
-            "Scaling factor should be a number or a tuple of numbers.")
+        assert isinstance(factor, numbers.Number) or isinstance(
+            factor, Coordinate
+        ), "Scaling factor should be a number or a Coordinate."
 
         self.source = source
         self.factor = factor
         self.target = target
 
     def setup(self):
-
         spec = self.spec[self.source].copy()
 
-        if not isinstance(self.factor, tuple):
-            self.factor = (self.factor,)*spec.roi.dims()
+        if not isinstance(self.factor, Coordinate):
+            self.factor = Coordinate((self.factor,) * spec.roi.dims)
 
-        assert spec.voxel_size % self.factor == (0,)*len(spec.voxel_size), \
-            "voxel size of upsampled volume is not integer: %s/%s = %s" % (
-                spec.voxel_size,
-                self.factor,
-                tuple(v/f for v, f in zip(spec.voxel_size, self.factor)))
+        assert spec.voxel_size % self.factor == (0,) * len(
+            spec.voxel_size
+        ), "voxel size of upsampled volume is not integer: %s/%s = %s" % (
+            spec.voxel_size,
+            self.factor,
+            tuple(v / f for v, f in zip(spec.voxel_size, self.factor)),
+        )
         spec.voxel_size /= self.factor
         self.provides(self.target, spec)
 
     def prepare(self, request):
         deps = BatchRequest()
 
         if self.target not in request:
             return
 
         logger.debug("preparing upsampling of " + str(self.source))
 
-        request_roi = request[self.target].roi
-        logger.debug("request ROI is %s"%request_roi)
+        upstream_voxel_size = self.spec[self.source].voxel_size
+
+        request_roi = request[self.target].roi.snap_to_grid(
+            upstream_voxel_size, mode="grow"
+        )
+        logger.debug("request ROI is %s" % request_roi)
 
         # add or merge to batch request
         deps[self.source] = ArraySpec(roi=request_roi)
 
         return deps
 
     def process(self, batch, request):
@@ -82,18 +87,18 @@
 
         assert input_roi.contains(request_roi)
 
         # upsample
 
         logger.debug("upsampling %s with %s", self.source, self.factor)
 
-        crop = batch.arrays[self.source].crop(request_roi)
+        crop = batch.arrays[self.source]
         data = crop.data
 
         for d, f in enumerate(self.factor):
-            data = np.repeat(data, f, axis=d)
+            data = np.repeat(data, f, axis=-self.factor.dims + d)
 
         # create output array
         spec = self.spec[self.target].copy()
-        spec.roi = request_roi
-        outputs.arrays[self.target] = Array(data, spec)
+        spec.roi = input_roi
+        outputs.arrays[self.target] = Array(data, spec).crop(request_roi)
         return outputs
```

### Comparing `gunpowder-1.2.2/gunpowder/producer_pool.py` & `gunpowder-1.3.0/gunpowder/producer_pool.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,156 +9,161 @@
 import time
 import traceback
 
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
+
 class NoResult(Exception):
     pass
 
+
 class ParentDied(Exception):
     pass
 
+
 class WorkersDied(Exception):
     pass
 
-class ProducerPool(object):
 
+class ProducerPool(object):
     def __init__(self, callables, queue_size=10):
-        self.__watch_dog = multiprocessing.Process(target=self.__run_watch_dog, args=(callables,))
+        self.__watch_dog = multiprocessing.Process(
+            target=self._run_watch_dog, args=(callables,)
+        )
         self.__stop = multiprocessing.Event()
         self.__result_queue = multiprocessing.Queue(queue_size)
 
     def __del__(self):
         self.stop()
 
     def start(self):
-        '''Start the pool of producers.'''
+        """Start the pool of producers."""
 
         if self.__watch_dog is None:
             raise RuntimeError("can't start a ProducerPool a second time")
 
         if self.__watch_dog.is_alive():
             logger.warning("trying to start workers, but they are already running")
             return
 
         self.__stop.clear()
         self.__watch_dog.start()
 
     def get(self, timeout=0):
-        '''Return the next result from the producer pool.
+        """Return the next result from the producer pool.
 
-        If timeout is set and there is not result after the given number of 
+        If timeout is set and there is not result after the given number of
         seconds, exception NoResult is raised.
-        '''
+        """
 
         block = False
         if timeout == 0:
             timeout = 1
             block = True
 
         item = None
         while item == None:
-
             try:
                 item = self.__result_queue.get(timeout=timeout)
             except Queue.Empty:
                 if not block:
                     raise NoResult()
 
         if isinstance(item, Exception):
             raise item
         return item
 
     def stop(self):
-        '''Stop the pool of producers.
+        """Stop the pool of producers.
 
-        Items currently being produced will not be waited for and be discarded.'''
+        Items currently being produced will not be waited for and be discarded."""
 
         if self.__watch_dog is None:
             return
 
         self.__stop.set()
-        self.__watch_dog.join()
+        if self.__watch_dog._popen is not None:
+            self.__watch_dog.join()
         self.__watch_dog = None
 
-    def __run_watch_dog(self, callables):
-
+    def _run_watch_dog(self, callables):
         parent_pid = os.getppid()
 
         logger.debug("watchdog started with PID " + str(os.getpid()))
         logger.debug("parent PID " + str(parent_pid))
 
-        workers = [ multiprocessing.Process(target=self.__run_worker, args=(c,)) for c in callables ]
+        workers = [
+            multiprocessing.Process(target=self._run_worker, args=(c,))
+            for c in callables
+        ]
 
         try:
-
-            logger.debug("starting %d workers"%len(workers))
+            logger.debug("starting %d workers" % len(workers))
             for worker in workers:
                 worker.start()
 
             while not self.__stop.wait(1):
                 if os.getppid() != parent_pid:
                     logger.error("parent of producer pool died, shutting down")
                     self.__result_queue.put(ParentDied())
                     break
-                if not self.__all_workers_alive(workers):
+                if not self._all_workers_alive(workers):
                     logger.error("at least one of my workers died, shutting down")
                     self.__result_queue.put(WorkersDied())
                     break
         except:
             pass
 
         finally:
-
             logger.info("terminating workers...")
             for worker in workers:
                 worker.terminate()
 
             logger.info("joining workers...")
             for worker in workers:
                 worker.join()
 
             logger.info("done")
 
-    def __run_worker(self, target):
-
+    def _run_worker(self, target):
         parent_pid = os.getppid()
 
         logger.debug("worker started with PID " + str(os.getpid()))
         logger.debug("parent PID " + str(parent_pid))
 
         result = None
         np.random.seed(None)
         while True:
-
             if os.getppid() != parent_pid:
-                logger.debug("worker %d: watch-dog died, stopping"%os.getpid())
+                logger.debug("worker %d: watch-dog died, stopping" % os.getpid())
                 break
 
             if result is None:
-
                 try:
                     result = target()
                 except Exception as e:
                     logger.error(e, exc_info=True)
                     result = e
                     traceback.print_exc()
-                    # don't stop on normal exceptions -- place them in result queue 
+                    # don't stop on normal exceptions -- place them in result queue
                     # and let them be handled by caller
                 except:
                     logger.error("received error: " + str(sys.exc_info()[0]))
                     # this is most likely a keyboard interrupt, stop process
                     break
 
             try:
                 self.__result_queue.put(result, timeout=1)
                 result = None
             except Queue.Full:
-                logger.debug("worker %d: result queue is full, waiting to place my result"%os.getpid())
+                logger.debug(
+                    "worker %d: result queue is full, waiting to place my result"
+                    % os.getpid()
+                )
 
         logger.debug("worker with PID " + str(os.getpid()) + " exiting")
         os._exit(1)
 
-    def __all_workers_alive(self, workers):
-        return all([ worker.is_alive() for worker in workers ])
+    def _all_workers_alive(self, workers):
+        return all([worker.is_alive() for worker in workers])
```

### Comparing `gunpowder-1.2.2/gunpowder/profiling.py` & `gunpowder-1.3.0/gunpowder/profiling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import numpy as np
 import time
 
 from .freezable import Freezable
 
-class Timing(Freezable):
 
+class Timing(Freezable):
     def __init__(self, node, method_name=None):
         self.__name = type(node).__name__
         self.__method_name = method_name
         self.__start = 0
         self.__first_start = 0
         self.__last_stop = 0
         self.__time = 0
@@ -20,51 +20,52 @@
         if self.__first_start == 0:
             self.__first_start = self.__start
 
     def stop(self):
         if self.__start == 0:
             return
         t = time.time()
-        self.__time += (t - self.__start)
+        self.__time += t - self.__start
         self.__start = 0
         self.__last_stop = t
 
     def elapsed(self):
-        '''Accumulated time elapsed between calls to start() and stop().'''
+        """Accumulated time elapsed between calls to start() and stop()."""
 
         if self.__start == 0:
             return self.__time
 
         return self.__time + (time.time() - self.__start)
 
     def span(self):
-        '''Timestamps of the first call to start() and last call to stop().'''
+        """Timestamps of the first call to start() and last call to stop()."""
         return self.__first_start, self.__last_stop
 
     def get_node_name(self):
         return self.__name
 
     def get_method_name(self):
         return self.__method_name
 
+
 class TimingSummary(Freezable):
-    '''Holds repeated Timings of the same node/method to be queried for statistics.'''
+    """Holds repeated Timings of the same node/method to be queried for statistics."""
 
     def __init__(self):
         self.timings = []
         self.times = []
         self.freeze()
 
     def add(self, timing):
-        '''Add a Timing to this summary.'''
+        """Add a Timing to this summary."""
         self.timings.append(timing)
         self.times.append(timing.elapsed())
 
     def merge(self, other):
-        '''Merge another summary into this one.'''
+        """Merge another summary into this one."""
         for timing in other.timings:
             self.add(timing)
 
     def counts(self):
         return len(self.times)
 
     def min(self):
@@ -75,61 +76,67 @@
 
     def mean(self):
         return np.mean(self.times)
 
     def median(self):
         return np.median(self.times)
 
-class ProfilingStats(Freezable):
 
+class ProfilingStats(Freezable):
     def __init__(self):
         self.__summaries = {}
         self.freeze()
 
     def add(self, timing):
-        '''Add a Timing instance. Timings are grouped by their class and method names.'''
+        """Add a Timing instance. Timings are grouped by their class and method names."""
 
         node_name = timing.get_node_name()
         method_name = timing.get_method_name()
         id = (node_name, method_name)
 
         if id not in self.__summaries:
             self.__summaries[id] = TimingSummary()
         self.__summaries[id].add(copy.deepcopy(timing))
 
     def merge_with(self, other):
-        '''Combine statitics of two ProfilingStats.'''
+        """Combine statitics of two ProfilingStats."""
 
         for id, summary in other.__summaries.items():
             if id in self.__summaries:
                 self.__summaries[id].merge(copy.deepcopy(summary))
             else:
                 self.__summaries[id] = copy.deepcopy(summary)
 
     def get_timing_summaries(self):
-        '''Get a dictionary (node_name,method_name) -> TimingSummary.'''
+        """Get a dictionary (node_name,method_name) -> TimingSummary."""
         return self.__summaries
 
     def get_timing_summary(self, node_name, method_name=None):
-        '''Get a :class:`TimingSummary` for the given node and method name.'''
+        """Get a :class:`TimingSummary` for the given node and method name."""
 
         if (node_name, method_name) not in self.__summaries:
-            raise RuntimeError("No timing summary for node %s, method %s"%(node_name,method_name))
+            raise RuntimeError(
+                "No timing summary for node %s, method %s" % (node_name, method_name)
+            )
 
-        return self.__summaries[(node_name,method_name)]
+        return self.__summaries[(node_name, method_name)]
 
     def span(self):
-        '''Timestamps of the first call to start() and last call to stop() over 
-        all Timings added.'''
+        """Timestamps of the first call to start() and last call to stop() over
+        all Timings added."""
 
-        spans = [t.span() for (_, summary) in self.__summaries.items() for t in summary.timings]
+        spans = [
+            t.span()
+            for (_, summary) in self.__summaries.items()
+            for t in summary.timings
+        ]
         first_start = min([span[0] for span in spans])
         last_stop = max([span[1] for span in spans])
 
         return first_start, last_stop
 
     def span_time(self):
-        '''Time between the first call to start() and last call to stop() over 
-        any timing.'''
+        """Time between the first call to start() and last call to stop() over
+        any timing."""
 
         start, stop = self.span()
         return stop - start
```

### Comparing `gunpowder-1.2.2/gunpowder/provider_spec.py` & `gunpowder-1.3.0/gunpowder/provider_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 
 
 import logging
 import warnings
 
 logger = logging.getLogger(__file__)
 
+
 class ProviderSpec(Freezable):
-    '''A collection of (possibly partial) :class:`ArraySpecs<ArraySpec>` and
+    """A collection of (possibly partial) :class:`ArraySpecs<ArraySpec>` and
     :class:`GraphSpecs<GraphSpec>` describing a
     :class:`BatchProvider's<BatchProvider>` offered arrays and graphs.
 
     This collection mimics a dictionary. Specs can be added with::
 
         provider_spec = ProviderSpec()
         provider_spec[array_key] = ArraySpec(...)
@@ -57,18 +58,17 @@
         array_specs (``dict``, :class:`ArrayKey` -> :class:`ArraySpec`):
 
             Contains all array specs contained in this provider spec.
 
         graph_specs (``dict``, :class:`GraphKey` -> :class:`GraphSpec`):
 
             Contains all graph specs contained in this provider spec.
-    '''
+    """
 
     def __init__(self, array_specs=None, graph_specs=None, points_specs=None):
-
         self.array_specs = {}
         self.graph_specs = {}
         self.freeze()
 
         # use __setitem__ instead of copying the dicts, this ensures type tests
         # are run
         if array_specs is not None:
@@ -86,128 +86,129 @@
         # Alias to graphs
         warnings.warn(
             "points_specs are depricated. Please use graph_specs", DeprecationWarning
         )
         return self.graph_specs
 
     def __setitem__(self, key, spec):
-
-        assert isinstance(key, ArrayKey) or isinstance(key, GraphKey), \
-            f"Only ArrayKey or GraphKey (not {type(key).__name__} are " \
+        assert isinstance(key, ArrayKey) or isinstance(key, GraphKey), (
+            f"Only ArrayKey or GraphKey (not {type(key).__name__} are "
             "allowed as key for ProviderSpec, "
+        )
 
         if isinstance(key, ArrayKey):
-
             if isinstance(spec, Roi):
                 spec = ArraySpec(roi=spec)
 
-            assert isinstance(spec, ArraySpec), \
-                f"Only ArraySpec (not {type(spec).__name__}) can be set for " \
-                "ArrayKey"
+            assert isinstance(spec, ArraySpec), (
+                f"Only ArraySpec (not {type(spec).__name__}) can be set for " "ArrayKey"
+            )
 
             self.array_specs[key] = spec.copy()
 
         else:
-
             if isinstance(spec, Roi):
                 spec = GraphSpec(roi=spec)
 
-            assert isinstance(spec, GraphSpec), \
-                f"Only GraphSpec (not {type(spec).__name__}) can be set for " \
-                "GraphKey"
+            assert isinstance(spec, GraphSpec), (
+                f"Only GraphSpec (not {type(spec).__name__}) can be set for " "GraphKey"
+            )
 
             self.graph_specs[key] = spec.copy()
 
     def __getitem__(self, key):
-
         if isinstance(key, ArrayKey):
             return self.array_specs[key]
 
         elif isinstance(key, GraphKey):
             return self.graph_specs[key]
         else:
             raise RuntimeError(
                 "Only ArrayKey or GraphKey can be used as keys in a "
-                "%s."%type(self).__name__)
+                "%s." % type(self).__name__
+            )
 
     def __len__(self):
-
         return len(self.array_specs) + len(self.graph_specs)
 
     def __contains__(self, key):
-
         if isinstance(key, ArrayKey):
             return key in self.array_specs
 
         elif isinstance(key, GraphKey):
             return key in self.graph_specs
 
         else:
             raise RuntimeError(
                 "Only ArrayKey or GraphKey, can be used as keys in a "
-                "%s. Key %s is a %s"%(type(self).__name__, key, type(key).__name__))
+                "%s. Key %s is a %s" % (type(self).__name__, key, type(key).__name__)
+            )
 
     def __delitem__(self, key):
-
         if isinstance(key, ArrayKey):
             del self.array_specs[key]
 
         elif isinstance(key, GraphKey):
             del self.graph_specs[key]
 
         else:
             raise RuntimeError(
                 "Only ArrayKey or GraphKey can be used as keys in a "
-                "%s."%type(self).__name__)
+                "%s." % type(self).__name__
+            )
 
     def remove_placeholders(self):
-        self.array_specs = {k: v for k, v in self.array_specs.items() if not v.placeholder}
-        self.graph_specs = {k: v for k, v in self.graph_specs.items() if not v.placeholder}
+        self.array_specs = {
+            k: v for k, v in self.array_specs.items() if not v.placeholder
+        }
+        self.graph_specs = {
+            k: v for k, v in self.graph_specs.items() if not v.placeholder
+        }
 
     def items(self):
-        '''Provides a generator iterating over key/value pairs.'''
+        """Provides a generator iterating over key/value pairs."""
 
-        for (k, v) in self.array_specs.items():
+        for k, v in self.array_specs.items():
             yield k, v
-        for (k, v) in self.graph_specs.items():
+        for k, v in self.graph_specs.items():
             yield k, v
 
     def get_total_roi(self):
-        '''Get the union of all the ROIs.'''
+        """Get the union of all the ROIs."""
 
         total_roi = None
         for specs_type in [self.array_specs, self.graph_specs]:
-            for (_, spec) in specs_type.items():
+            for _, spec in specs_type.items():
                 if total_roi is None:
                     total_roi = spec.roi
                 elif spec.roi is not None:
                     total_roi = total_roi.union(spec.roi)
         return total_roi
 
     def get_common_roi(self):
-        '''Get the intersection of all the requested ROIs.'''
+        """Get the intersection of all the requested ROIs."""
 
         common_roi = None
         for specs_type in [self.array_specs, self.graph_specs]:
-            for (_, spec) in specs_type.items():
+            for _, spec in specs_type.items():
                 if common_roi is None:
                     common_roi = spec.roi
                 else:
                     common_roi = common_roi.intersect(spec.roi)
 
         return common_roi
 
     def get_lcm_voxel_size(self, array_keys=None):
-        '''Get the least common multiple of the voxel sizes in this spec.
+        """Get the least common multiple of the voxel sizes in this spec.
 
         Args:
 
             array_keys (list of :class:`ArrayKey`, optional): If given,
                 consider only the given array types.
-        '''
+        """
 
         if array_keys is None:
             array_keys = self.array_specs.keys()
 
         if not array_keys:
             return None
 
@@ -216,32 +217,32 @@
             voxel_size = self.array_specs[key].voxel_size
             if voxel_size is None:
                 continue
             if lcm_voxel_size is None:
                 lcm_voxel_size = voxel_size
             else:
                 lcm_voxel_size = Coordinate(
-                    (a * b // math.gcd(a, b)
-                     for a, b in zip(lcm_voxel_size, voxel_size)))
+                    (
+                        a * b // math.gcd(a, b)
+                        for a, b in zip(lcm_voxel_size, voxel_size)
+                    )
+                )
 
         return lcm_voxel_size
 
     def __eq__(self, other):
-
         if isinstance(other, self.__class__):
             other_dict = copy.deepcopy(other.__dict__)
             self_dict = copy.deepcopy(self.__dict__)
             return self_dict == other_dict
         return NotImplemented
 
     def __ne__(self, other):
-
         if isinstance(other, self.__class__):
             return not self.__eq__(other)
         return NotImplemented
 
     def __repr__(self):
-
         r = "\n"
-        for (key, spec) in self.items():
-            r += "\t%s: %s\n"%(key, spec)
+        for key, spec in self.items():
+            r += "\t%s: %s\n" % (key, spec)
         return r
```

### Comparing `gunpowder-1.2.2/gunpowder/tensorflow/local_server.py` & `gunpowder-1.3.0/gunpowder/tensorflow/local_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 import multiprocessing
 import ctypes
 from gunpowder.ext import tensorflow as tf
 from gunpowder.freezable import Freezable
 
 logger = logging.getLogger(__name__)
 
+
 class LocalServer(Freezable):
-    '''Wrapper around ``tf.train.Server`` to create a local server on-demand.
+    """Wrapper around ``tf.train.Server`` to create a local server on-demand.
 
     This class is necessary because tensorflow's GPU support should not be
     initialized before forking processes (the CUDA driver needs to be
     initialized in each process separately, not in the main process and then
     forked). Creating a ``tf.train.Server`` initializes GPU support, however.
     With this wrapper, server creating can be delayed until a GPU process
     creates a ``tf.Session``::
 
         session = tf.Session(target=LocalServer.get_target())
-    '''
+    """
 
-    __target = multiprocessing.Array(ctypes.c_char, b' '*256)
+    __target = multiprocessing.Array(ctypes.c_char, b" " * 256)
     __server = None
 
     @staticmethod
     def get_target():
-        '''Get the target string of this tensorflow server to connect a
+        """Get the target string of this tensorflow server to connect a
         ``tf.Session()``. This will start the server, if it is not running
         already.
-        '''
+        """
 
         with LocalServer.__target.get_lock():
-
             target = LocalServer.__target.value
 
-            if target == b' '*256:
+            if target == b" " * 256:
                 logger.info("Creating local tensorflow server")
                 LocalServer.__server = tf.train.Server.create_local_server()
                 target = LocalServer.__server.target
                 if not isinstance(target, bytes):
-                    target = target.encode('ascii')
+                    target = target.encode("ascii")
                 logger.info("Server running at %s", target)
             else:
                 logger.info("Server already running at %s", target)
 
             LocalServer.__target.value = target
 
         return target
```

### Comparing `gunpowder-1.2.2/gunpowder/tensorflow/nodes/predict.py` & `gunpowder-1.3.0/gunpowder/tensorflow/nodes/predict.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from gunpowder.ext import tensorflow as tf
 from gunpowder.nodes.generic_predict import GenericPredict
 from gunpowder.tensorflow.local_server import LocalServer
 from operator import mul
 
 logger = logging.getLogger(__name__)
 
+
 class Predict(GenericPredict):
-    '''Tensorflow implementation of :class:`gunpowder.nodes.Predict`.
+    """Tensorflow implementation of :class:`gunpowder.nodes.Predict`.
 
     Args:
 
         checkpoint (``string``):
 
             Basename of a tensorflow checkpoint storing the tensorflow graph
             and associated tensor values and metadata, as created by
@@ -54,89 +55,76 @@
             Skip prediction, if all inputs are empty (contain only 0). In this
             case, outputs are simply set to 0.
 
         max_shared_memory (``int``, optional):
 
             The maximal amount of shared memory in bytes to allocate to send
             batches to the GPU processes. Defaults to 1GB.
-    '''
+    """
 
     def __init__(
-            self,
-            checkpoint,
-            inputs,
-            outputs,
-            array_specs=None,
-            graph=None,
-            skip_empty=False,
-            max_shared_memory=1024*1024*1024):
-
-        super(Predict, self).__init__(
-            inputs,
-            outputs,
-            array_specs)
+        self,
+        checkpoint,
+        inputs,
+        outputs,
+        array_specs=None,
+        graph=None,
+        skip_empty=False,
+        max_shared_memory=1024 * 1024 * 1024,
+    ):
+        super(Predict, self).__init__(inputs, outputs, array_specs)
 
         self.checkpoint = checkpoint
         self.meta_graph = graph
         self.session = None
         self.graph = None
         self.skip_empty = skip_empty
 
         self.manager = mp.Manager()
         self.max_shared_memory = max_shared_memory
         self.shared_input_array_config = self.manager.dict()
         self.shared_output_array_config = self.manager.dict()
         self.shared_input_arrays = {}
         self.shared_output_arrays = {}
-        self.shared_input_memory = mp.RawArray(
-            ctypes.c_float,
-            self.max_shared_memory)
-        self.shared_output_memory = mp.RawArray(
-            ctypes.c_float,
-            self.max_shared_memory)
+        self.shared_input_memory = mp.RawArray(ctypes.c_float, self.max_shared_memory)
+        self.shared_output_memory = mp.RawArray(ctypes.c_float, self.max_shared_memory)
 
         self.send_lock = mp.Lock()
         self.receive_lock = mp.Lock()
         self.predict_process_initialized = mp.Event()
         self.worker_sent_inputs = mp.Event()
         self.predict_received_inputs = mp.Event()
         self.predict_sent_outputs = mp.Event()
 
         self.predict_process = mp.Process(target=self.__predict)
-        self.predict_process_crashed = mp.Value('i', False)
+        self.predict_process_crashed = mp.Value("i", False)
         self.predict_process.start()
         self.predict_process_initialized.wait()
 
     def predict(self, batch, request):
-
         if not self.shared_output_arrays:
             self.__init_shared_output_arrays()
 
         if self.skip_empty:
-
             can_skip = True
             for array_key in self.inputs.values():
                 if batch[array_key].data.any():
                     can_skip = False
                     break
 
             if can_skip:
-
-                logger.info("Skipping batch %i (all inputs are 0)"%batch.id)
+                logger.info("Skipping batch %i (all inputs are 0)" % batch.id)
 
                 for name, array_key in self.outputs.items():
-
                     shape = self.shared_output_arrays[name].shape
                     dtype = self.shared_output_arrays[name].dtype
 
                     spec = self.spec[array_key].copy()
                     spec.roi = request[array_key].roi.copy()
-                    batch.arrays[array_key] = Array(
-                        np.zeros(shape, dtype=dtype),
-                        spec)
+                    batch.arrays[array_key] = Array(np.zeros(shape, dtype=dtype), spec)
 
                 return
 
         logger.debug("predicting in batch %i", batch.id)
 
         output_tensors = self.__collect_outputs(request)
         input_data = self.__collect_provided_inputs(batch)
@@ -166,233 +154,215 @@
         output_data = self.__read_outputs_from_shared(output_tensors)
 
         self.receive_lock.release()
 
         for array_key in output_tensors:
             spec = self.spec[array_key].copy()
             spec.roi = request[array_key].roi
-            batch.arrays[array_key] = Array(
-                output_data[array_key],
-                spec)
+            batch.arrays[array_key] = Array(output_data[array_key], spec)
 
         logger.debug("predicted in batch %i", batch.id)
 
     def __predict(self):
-        '''The background predict process.'''
+        """The background predict process."""
 
         try:
             # TODO: is the server still needed?
             target = LocalServer.get_target()
             logger.info("Initializing tf session, connecting to %s...", target)
 
             self.graph = tf.Graph()
-            self.session = tf.Session(
-                target=target,
-                graph=self.graph)
+            self.session = tf.Session(target=target, graph=self.graph)
 
             with self.graph.as_default():
                 self.__read_checkpoint()
 
             if not self.shared_output_arrays:
                 if not self.shared_output_array_config:
                     self.__create_shared_output_array_config()
                 self.__init_shared_output_arrays()
 
             # from now on it is save to access the shared array configuration
             self.predict_process_initialized.set()
 
             # loop predict
             while True:
-
                 # wait for inputs
                 self.worker_sent_inputs.wait()
                 self.worker_sent_inputs.clear()
 
                 if not self.shared_input_arrays:
                     self.__init_shared_input_arrays()
 
                 # read inputs
                 input_data = self.__read_inputs_from_shared()
                 self.predict_received_inputs.set()
 
                 # compute outputs
                 output_data = self.session.run(
-                    {t: t for t in self.outputs.keys()},
-                    feed_dict=input_data)
+                    {t: t for t in self.outputs.keys()}, feed_dict=input_data
+                )
 
                 # write outputs
                 self.__write_outputs_to_shared(output_data)
                 self.predict_sent_outputs.set()
 
         except Exception as e:
-
             self.predict_process_crashed.value = True
 
             # release locks and events
             self.predict_process_initialized.set()
             self.worker_sent_inputs.clear()
             self.predict_received_inputs.set()
             self.predict_sent_outputs.set()
             raise e
 
     def teardown(self):
-
         self.predict_process.terminate()
         self.predict_process.join()
 
     def __check_background_process(self, locks=[]):
-
         if self.predict_process_crashed.value:
             # release all locks before raising exception
             for l in locks:
                 l.release()
             raise RuntimeError("Background process died.")
 
     def __read_checkpoint(self):
-
         # read the graph associated to the checkpoint
         if self.meta_graph is None:
-            meta_graph_file = self.checkpoint + '.meta'
+            meta_graph_file = self.checkpoint + ".meta"
         # read alternative, custom graph
         else:
             meta_graph_file = self.meta_graph
 
         logger.info(
             "Reading graph from %s and weights from %s...",
-            meta_graph_file, self.checkpoint)
+            meta_graph_file,
+            self.checkpoint,
+        )
 
-        saver = tf.train.import_meta_graph(
-                meta_graph_file,
-                clear_devices=True)
+        saver = tf.train.import_meta_graph(meta_graph_file, clear_devices=True)
 
         # restore variables from checkpoint
         saver.restore(self.session, self.checkpoint)
 
     def __collect_outputs(self, request=None):
-        '''Get a dict:
+        """Get a dict:
 
             array key: tensor name
 
         If request is not None, return only outputs that are in request.
-        '''
+        """
 
         array_outputs = {}
 
         for tensor_name, array_key in self.outputs.items():
             if request is None or array_key in request:
                 array_outputs[array_key] = tensor_name
 
         return array_outputs
 
     def __collect_provided_inputs(self, batch):
-        '''Get a dict:
+        """Get a dict:
 
-            tensor name: ndarray
-        '''
+        tensor name: ndarray
+        """
 
         inputs = {}
 
         for input_name, input_key in self.inputs.items():
             if isinstance(input_key, ArrayKey):
                 if input_key in batch.arrays:
                     inputs[input_name] = batch.arrays[input_key].data
                 else:
-                    logger.warn("batch does not contain %s, input %s will not "
-                                "be set", input_key, input_name)
+                    logger.warn(
+                        "batch does not contain %s, input %s will not " "be set",
+                        input_key,
+                        input_name,
+                    )
             elif isinstance(input_key, np.ndarray):
                 inputs[input_name] = input_key
             elif isinstance(input_key, str):
                 inputs[input_name] = getattr(batch, input_key)
             else:
                 raise Exception(
                     "Unknown network input key {}, can't be given to "
-                    "network".format(input_key))
+                    "network".format(input_key)
+                )
 
         return inputs
 
     def __create_shared_input_array_config(self, batch, request):
-        '''Store the shared array config in a shared dictionary. Should be run
-        once by the first worker to submit a batch.'''
+        """Store the shared array config in a shared dictionary. Should be run
+        once by the first worker to submit a batch."""
 
         begin = 0
         for name, array_key in self.inputs.items():
-
             shape = batch[array_key].data.shape
             size = reduce(mul, shape, 1)
             dtype = batch[array_key].data.dtype
 
-            self.shared_input_array_config[name] = (
-                begin,
-                size,
-                shape,
-                dtype)
-
-            begin += size*np.dtype(dtype).itemsize
-            assert begin <= self.max_shared_memory, (
-                "The input arrays exceed the max_shared_memory")
+            self.shared_input_array_config[name] = (begin, size, shape, dtype)
+
+            begin += size * np.dtype(dtype).itemsize
+            assert (
+                begin <= self.max_shared_memory
+            ), "The input arrays exceed the max_shared_memory"
 
     def __create_shared_output_array_config(self):
-        '''To be called by predict process.'''
+        """To be called by predict process."""
 
         begin = 0
         for name, array_key in self.outputs.items():
-
             tensor = self.graph.get_tensor_by_name(name)
             shape = tensor.get_shape().as_list()
             size = reduce(mul, shape, 1)
             dtype = tensor.dtype.as_numpy_dtype
 
-            self.shared_output_array_config[name] = (
-                begin,
-                size,
-                tuple(shape),
-                dtype)
-
-            begin += size*np.dtype(dtype).itemsize
-            assert begin <= self.max_shared_memory, (
-                "The output arrays exceed the max_shared_memory")
+            self.shared_output_array_config[name] = (begin, size, tuple(shape), dtype)
+
+            begin += size * np.dtype(dtype).itemsize
+            assert (
+                begin <= self.max_shared_memory
+            ), "The output arrays exceed the max_shared_memory"
 
     def __init_shared_input_arrays(self):
-        '''Assign the shared memory to numpy arrays.'''
+        """Assign the shared memory to numpy arrays."""
 
         for name, (begin, size, shape, dtype) in self.shared_input_array_config.items():
-
             self.shared_input_arrays[name] = np.frombuffer(
-                self.shared_input_memory,
-                dtype=dtype,
-                offset=begin,
-                count=size).reshape(shape)
+                self.shared_input_memory, dtype=dtype, offset=begin, count=size
+            ).reshape(shape)
 
     def __init_shared_output_arrays(self):
-        '''Assign the shared memory to numpy arrays.'''
-
-        for name, (begin, size, shape, dtype) in self.shared_output_array_config.items():
+        """Assign the shared memory to numpy arrays."""
 
+        for name, (
+            begin,
+            size,
+            shape,
+            dtype,
+        ) in self.shared_output_array_config.items():
             self.shared_output_arrays[name] = np.frombuffer(
-                self.shared_output_memory,
-                dtype=dtype,
-                offset=begin,
-                count=size).reshape(shape)
+                self.shared_output_memory, dtype=dtype, offset=begin, count=size
+            ).reshape(shape)
 
     def __write_inputs_to_shared(self, input_data):
-
         for tensor_name, data in input_data.items():
             self.shared_input_arrays[tensor_name][:] = data
 
     def __read_inputs_from_shared(self):
-
         return {
             tensor_name: self.shared_input_arrays[tensor_name].copy()
             for tensor_name in self.inputs.keys()
         }
 
     def __write_outputs_to_shared(self, output_data):
-
         for tensor_name, data in output_data.items():
             self.shared_output_arrays[tensor_name][:] = data
 
     def __read_outputs_from_shared(self, output_tensors):
-
         return {
-                array_key: self.shared_output_arrays[tensor_name].copy()
-                for array_key, tensor_name in output_tensors.items()
+            array_key: self.shared_output_arrays[tensor_name].copy()
+            for array_key, tensor_name in output_tensors.items()
         }
```

### Comparing `gunpowder-1.2.2/gunpowder/tensorflow/nodes/train.py` & `gunpowder-1.3.0/gunpowder/tensorflow/nodes/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from gunpowder.array import ArrayKey, Array
 from gunpowder.ext import tensorflow as tf
 from gunpowder.nodes.generic_train import GenericTrain
 from gunpowder.tensorflow.local_server import LocalServer
 
 logger = logging.getLogger(__name__)
 
+
 class Train(GenericTrain):
-    '''Tensorflow implementation of :class:`gunpowder.nodes.Train`.
+    """Tensorflow implementation of :class:`gunpowder.nodes.Train`.
 
     Args:
 
         graph (``string``):
 
             Filename of a tensorflow meta-graph storing the tensorflow graph
             containing an optimizer. A meta-graph file can be created by
@@ -99,36 +100,33 @@
         log_dir (``string``, optional):
 
             Directory for saving tensorboard summaries.
 
         log_every (``int``, optional):
 
             After how many iterations to write out tensorboard summaries.
-    '''
+    """
 
     def __init__(
-            self,
-            graph,
-            optimizer,
-            loss,
-            inputs,
-            outputs,
-            gradients,
-            summary=None,
-            array_specs=None,
-            save_every=2000,
-            log_dir='./',
-            log_every=1):
-
+        self,
+        graph,
+        optimizer,
+        loss,
+        inputs,
+        outputs,
+        gradients,
+        summary=None,
+        array_specs=None,
+        save_every=2000,
+        log_dir="./",
+        log_every=1,
+    ):
         super(Train, self).__init__(
-            inputs,
-            outputs,
-            gradients,
-            array_specs,
-            spawn_subprocess=False)
+            inputs, outputs, gradients, array_specs, spawn_subprocess=False
+        )
         self.meta_graph_filename = graph
         self.optimizer_func = None
         self.optimizer_loss_names = None
         self.optimizer = None
         self.loss = None
         self.summary = summary
         self.session = None
@@ -139,139 +137,120 @@
         self.save_every = save_every
         self.iteration = None
         self.iteration_increment = None
         self.summary_saver = None
         self.log_dir = log_dir
         self.log_every = log_every
         # Check if optimizer is a str in python 2/3 compatible way.
-        if isinstance(optimizer, ("".__class__, u"".__class__)):
+        if isinstance(optimizer, ("".__class__, "".__class__)):
             self.optimizer_loss_names = (optimizer, loss)
         else:
             self.optimizer_func = optimizer
 
         # at least for some versions of tensorflow, the checkpoint name has to
         # start with a . if it is a relative path
         if not os.path.isabs(self.meta_graph_filename):
-            self.meta_graph_filename = os.path.join('.', self.meta_graph_filename)
+            self.meta_graph_filename = os.path.join(".", self.meta_graph_filename)
 
     def start(self):
-
         target = LocalServer.get_target()
         logger.info("Initializing tf session, connecting to %s...", target)
 
         self.graph = tf.Graph()
-        self.session = tf.Session(
-            target=target,
-            graph=self.graph)
+        self.session = tf.Session(target=target, graph=self.graph)
 
         with self.graph.as_default():
             self.__read_meta_graph()
 
         if self.summary is not None:
             self.summary_saver = tf.summary.FileWriter(self.log_dir, self.graph)
 
         if self.optimizer_func is None:
-
             # get actual operations/tensors from names
-            self.optimizer = self.graph.get_operation_by_name(self.optimizer_loss_names[0])
+            self.optimizer = self.graph.get_operation_by_name(
+                self.optimizer_loss_names[0]
+            )
             self.loss = self.graph.get_tensor_by_name(self.optimizer_loss_names[1])
 
         # add symbolic gradients
         for tensor_name in self.gradients:
             tensor = self.graph.get_tensor_by_name(tensor_name)
-            self.tf_gradient[tensor_name] = tf.gradients(
-                self.loss,
-                [tensor])[0]
+            self.tf_gradient[tensor_name] = tf.gradients(self.loss, [tensor])[0]
 
     def train_step(self, batch, request):
-
         array_outputs = self.__collect_requested_outputs(request)
         inputs = self.__collect_provided_inputs(batch)
 
         to_compute = {
-            'optimizer': self.optimizer,
-            'loss': self.loss,
-            'iteration': self.iteration_increment}
+            "optimizer": self.optimizer,
+            "loss": self.loss,
+            "iteration": self.iteration_increment,
+        }
         to_compute.update(array_outputs)
 
         # compute outputs, gradients, and update variables
         if isinstance(self.summary, str):
             to_compute["summaries"] = self.summary
         elif isinstance(self.summary, dict):
             for k, (v, f) in self.summary.items():
-                if int(self.current_step+1) % f == 0:
+                if int(self.current_step + 1) % f == 0:
                     to_compute[k] = v
         outputs = self.session.run(to_compute, feed_dict=inputs)
 
         for array_key in array_outputs:
             spec = self.spec[array_key].copy()
             spec.roi = request[array_key].roi
-            batch.arrays[array_key] = Array(
-                outputs[array_key],
-                spec)
+            batch.arrays[array_key] = Array(outputs[array_key], spec)
 
-        batch.loss = outputs['loss']
-        batch.iteration = outputs['iteration'][0]
+        batch.loss = outputs["loss"]
+        batch.iteration = outputs["iteration"][0]
         self.current_step = batch.iteration
         if self.summary is not None:
-            if isinstance(self.summary, str) and \
-               (batch.iteration % self.log_every == 0 or batch.iteration == 1):
-                self.summary_saver.add_summary(
-                            outputs['summaries'], batch.iteration)
+            if isinstance(self.summary, str) and (
+                batch.iteration % self.log_every == 0 or batch.iteration == 1
+            ):
+                self.summary_saver.add_summary(outputs["summaries"], batch.iteration)
             else:
                 for k, (_, f) in self.summary.items():
                     if int(self.current_step) % f == 0:
-                        self.summary_saver.add_summary(
-                            outputs[k], batch.iteration)
-
-        if batch.iteration%self.save_every == 0:
+                        self.summary_saver.add_summary(outputs[k], batch.iteration)
 
+        if batch.iteration % self.save_every == 0:
             checkpoint_name = (
-                self.meta_graph_filename +
-                '_checkpoint_%i'%batch.iteration)
+                self.meta_graph_filename + "_checkpoint_%i" % batch.iteration
+            )
 
-            logger.info(
-                "Creating checkpoint %s",
-                checkpoint_name)
-
-            self.full_saver.save(
-                self.session,
-                checkpoint_name)
+            logger.info("Creating checkpoint %s", checkpoint_name)
 
-    def stop(self):
+            self.full_saver.save(self.session, checkpoint_name)
 
+    def stop(self):
         if self.session is not None:
-
             self.optimizer = None
             self.loss = None
             if self.summary is not None:
                 self.summary_saver.close()
             self.session.close()
             self.graph = None
             self.session = None
 
     def __read_meta_graph(self):
-
         logger.info("Reading meta-graph...")
 
         # read the original meta-graph
         tf.train.import_meta_graph(
-            self.meta_graph_filename + '.meta',
-            clear_devices=True)
+            self.meta_graph_filename + ".meta", clear_devices=True
+        )
 
         # add custom gunpowder variables
-        with tf.variable_scope('gunpowder'):
+        with tf.variable_scope("gunpowder"):
             self.iteration = tf.get_variable(
-                'iteration',
-                shape=1,
-                initializer=tf.zeros_initializer,
-                trainable=False)
-            self.iteration_increment = tf.assign(
-                self.iteration,
-                self.iteration + 1)
+                "iteration", shape=1, initializer=tf.zeros_initializer, trainable=False
+            )
+            self.iteration_increment = tf.assign(self.iteration, self.iteration + 1)
 
         # Until now, only variables have been added to the graph that are part
         # of every checkpoint. We create a 'basic_saver' for only those
         # variables.
         self.basic_saver = tf.train.Saver(max_to_keep=None)
 
         # Add custom optimizer and loss, if requested. This potentially adds
@@ -285,85 +264,80 @@
         self.full_saver = tf.train.Saver(max_to_keep=None)
 
         # find most recent checkpoint
         checkpoint_dir = os.path.dirname(self.meta_graph_filename)
         checkpoint = tf.train.latest_checkpoint(checkpoint_dir)
 
         if checkpoint:
-
             try:
                 # Try to restore the graph, including the custom optimizer
                 # state (if a custom optimizer was used).
                 self.__restore_graph(checkpoint, restore_full=True)
 
             except tf.errors.NotFoundError:
-
                 # If that failed, we just transitioned from an earlier training
                 # without the custom optimizer. In this case, restore only the
                 # variables of the original meta-graph and 'gunpowder'
                 # variables. Custom optimizer variables will be default
                 # initialized.
-                logger.info("Checkpoint did not contain custom optimizer "
-                            "variables")
+                logger.info("Checkpoint did not contain custom optimizer " "variables")
                 self.__restore_graph(checkpoint, restore_full=False)
         else:
-
             logger.info("No checkpoint found")
 
             # initialize all variables
             self.session.run(tf.global_variables_initializer())
 
     def __restore_graph(self, checkpoint, restore_full):
-
         logger.info("Restoring model from %s", checkpoint)
 
         if restore_full:
-
             logger.info("...using a saver for all variables")
             self.full_saver.restore(self.session, checkpoint)
 
         else:
-
             # initialize all variables, such that non-basic variables are
             # initialized
             self.session.run(tf.global_variables_initializer())
 
             logger.info("...using a saver for basic variables only")
             self.basic_saver.restore(self.session, checkpoint)
 
         self.current_step = self.session.run(self.iteration)
 
     def __collect_requested_outputs(self, request):
-
         array_outputs = {}
 
         for output_name, array_key in self.outputs.items():
             if array_key in request:
                 array_outputs[array_key] = output_name
 
         for output_name, array_key in self.gradients.items():
             if array_key in request:
                 array_outputs[array_key] = self.tf_gradient[output_name]
 
         return array_outputs
 
     def __collect_provided_inputs(self, batch):
-
         inputs = {}
 
         for input_name, input_key in self.inputs.items():
             if isinstance(input_key, ArrayKey):
                 if input_key in batch.arrays:
                     inputs[input_name] = batch.arrays[input_key].data
                 else:
-                    logger.warn("batch does not contain %s, input %s will not "
-                                "be set", input_key, input_name)
+                    logger.warn(
+                        "batch does not contain %s, input %s will not " "be set",
+                        input_key,
+                        input_name,
+                    )
             elif isinstance(input_key, np.ndarray):
                 inputs[input_name] = input_key
             elif isinstance(input_key, str):
                 inputs[input_name] = getattr(batch, input_key)
             else:
                 raise Exception(
                     "Unknown network input key {}, can't be given to "
-                    "network".format(input_key))
+                    "network".format(input_key)
+                )
 
         return inputs
```

### Comparing `gunpowder-1.2.2/gunpowder/torch/nodes/predict.py` & `gunpowder-1.3.0/gunpowder/torch/nodes/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,44 +59,38 @@
         self,
         model,
         inputs: Dict[str, ArrayKey],
         outputs: Dict[Union[str, int], ArrayKey],
         array_specs: Dict[ArrayKey, ArraySpec] = None,
         checkpoint: str = None,
         device="cuda",
-        spawn_subprocess=False
+        spawn_subprocess=False,
     ):
-
         self.array_specs = array_specs if array_specs is not None else {}
 
         if model.training:
             logger.warning(
                 "Model is in training mode during prediction. "
                 "Consider using model.eval()"
             )
 
         super(Predict, self).__init__(
-            inputs,
-            outputs,
-            array_specs,
-            spawn_subprocess=spawn_subprocess)
+            inputs, outputs, array_specs, spawn_subprocess=spawn_subprocess
+        )
 
         self.device_string = device
         self.device = None  # to be set in start()
         self.model = model
         self.checkpoint = checkpoint
 
         self.intermediate_layers = {}
         self.register_hooks()
 
     def start(self):
-
-        self.use_cuda = (
-            torch.cuda.is_available() and
-            self.device_string == "cuda")
+        self.use_cuda = torch.cuda.is_available() and self.device_string == "cuda"
         logger.info(f"Predicting on {'gpu' if self.use_cuda else 'cpu'}")
         self.device = torch.device("cuda" if self.use_cuda else "cpu")
 
         try:
             self.model = self.model.to(self.device)
         except RuntimeError as e:
             raise RuntimeError(
```

### Comparing `gunpowder-1.2.2/gunpowder/torch/nodes/train.py` & `gunpowder-1.3.0/gunpowder/torch/nodes/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             Directory for saving tensorboard summaries.
 
         log_every (``int``, optional):
 
             After how many iterations to write out tensorboard summaries.
 
         spawn_subprocess (``bool``, optional):
-        
+
             Whether to run the ``train_step`` in a separate process. Default is false.
     """
 
     def __init__(
         self,
         model,
         loss,
@@ -92,15 +92,14 @@
         array_specs: Optional[Dict[ArrayKey, ArraySpec]] = None,
         checkpoint_basename: str = "model",
         save_every: int = 2000,
         log_dir: str = None,
         log_every: int = 1,
         spawn_subprocess: bool = False,
     ):
-
         if not model.training:
             logger.warning(
                 "Model is in evaluation mode during training. "
                 "Consider using model.train()"
             )
 
         # not yet implemented
@@ -156,15 +155,14 @@
             else:
                 raise RuntimeError(
                     "only ints and strings are supported as gradients keys"
                 )
             tensor.retain_grad()
 
     def start(self):
-
         self.use_cuda = torch.cuda.is_available()
         self.device = torch.device("cuda" if self.use_cuda else "cpu")
 
         try:
             self.model = self.model.to(self.device)
         except RuntimeError as e:
             raise RuntimeError(
@@ -176,30 +174,27 @@
             self.loss = self.loss.to(self.device)
 
         checkpoint, self.iteration = self._get_latest_checkpoint(
             self.checkpoint_basename
         )
 
         if checkpoint is not None:
-
             logger.info("Resuming training from iteration %d", self.iteration)
             logger.info("Loading %s", checkpoint)
 
             checkpoint = torch.load(checkpoint, map_location=self.device)
             self.model.load_state_dict(checkpoint["model_state_dict"])
             self.optimizer.load_state_dict(checkpoint["optimizer_state_dict"])
 
         else:
-
             logger.info("Starting training from scratch")
 
         logger.info("Using device %s", self.device)
 
     def train_step(self, batch, request):
-
         inputs = self.__collect_provided_inputs(batch)
         requested_outputs = self.__collect_requested_outputs(request)
 
         # keys are argument names of model forward pass
         device_inputs = {
             k: torch.as_tensor(v, device=self.device) for k, v in inputs.items()
         }
@@ -246,21 +241,20 @@
                 device_loss_kwargs[k] = device_loss_inputs.pop(k)
         assert (
             len(device_loss_inputs) == 0
         ), f"Not all loss inputs could be interpreted. Failed keys: {device_loss_inputs.keys()}"
 
         self.retain_gradients(request, outputs)
 
-        logger.debug(
-            "model outputs: %s",
-            {k: v.shape for k, v in outputs.items()})
+        logger.debug("model outputs: %s", {k: v.shape for k, v in outputs.items()})
         logger.debug(
             "loss inputs: %s %s",
             [v.shape for v in device_loss_args],
-            {k: v.shape for k, v in device_loss_kwargs.items()})
+            {k: v.shape for k, v in device_loss_kwargs.items()},
+        )
         loss = self.loss(*device_loss_args, **device_loss_kwargs)
         loss.backward()
         self.optimizer.step()
 
         # add requested model outputs to batch
         for array_key, array_name in requested_outputs.items():
             spec = self.spec[array_key].copy()
@@ -278,31 +272,28 @@
                 tensor = getattr(self.model, array_name)
             else:
                 raise RuntimeError(
                     "only ints and strings are supported as gradients keys"
                 )
             spec = self.spec[array_key].copy()
             spec.roi = request[array_key].roi
-            batch.arrays[array_key] = Array(
-                tensor.grad.cpu().detach().numpy(), spec
-            )
+            batch.arrays[array_key] = Array(tensor.grad.cpu().detach().numpy(), spec)
 
         for array_key, array_name in requested_outputs.items():
             spec = self.spec[array_key].copy()
             spec.roi = request[array_key].roi
             batch.arrays[array_key] = Array(
                 outputs[array_name].cpu().detach().numpy(), spec
             )
 
         batch.loss = loss.cpu().detach().numpy()
         self.iteration += 1
         batch.iteration = self.iteration
 
         if batch.iteration % self.save_every == 0:
-
             checkpoint_name = self._checkpoint_name(
                 self.checkpoint_basename, batch.iteration
             )
 
             logger.info("Creating checkpoint %s", checkpoint_name)
 
             torch.save(
@@ -313,37 +304,33 @@
                 checkpoint_name,
             )
 
         if self.summary_writer and batch.iteration % self.log_every == 0:
             self.summary_writer.add_scalar("loss", batch.loss, batch.iteration)
 
     def __collect_requested_outputs(self, request):
-
         array_outputs = {}
 
         for output_name, array_key in self.outputs.items():
             if array_key in request:
                 array_outputs[array_key] = output_name
 
         return array_outputs
 
     def __collect_provided_inputs(self, batch):
-
         return self.__collect_provided_arrays(
             {k: v for k, v in self.inputs.items() if k not in self.loss_inputs}, batch
         )
 
     def __collect_provided_loss_inputs(self, batch):
-
         return self.__collect_provided_arrays(
             self.loss_inputs, batch, expect_missing_arrays=True
         )
 
     def __collect_provided_arrays(self, reference, batch, expect_missing_arrays=False):
-
         arrays = {}
 
         for array_name, array_key in reference.items():
             if isinstance(array_key, ArrayKey):
                 msg = f"batch does not contain {array_key}, array {array_name} will not be set"
                 if array_key in batch.arrays:
                     arrays[array_name] = batch.arrays[array_key].data
```

### Comparing `gunpowder-1.2.2/gunpowder/version_info.py` & `gunpowder-1.3.0/gunpowder/version_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-__major__   = 1
-__minor__   = 2
-__patch__   = 2
-__tag__     = ''
-__version__ = '{}.{}.{}{}'.format(__major__, __minor__, __patch__, __tag__).strip('.')
+__major__ = 1
+__minor__ = 3
+__patch__ = 0
+__tag__ = ""
+__version__ = "{}.{}.{}{}".format(__major__, __minor__, __patch__, __tag__).strip(".")
 
-class _Version(object):
 
+class _Version(object):
     def major(self):
         return __major__
 
     def minor(self):
         return __minor__
 
     def patch(self):
@@ -20,11 +20,12 @@
 
     def version(self):
         return __version__
 
     def __str__(self):
         return self.version()
 
+
 _version = _Version()
 
 if __name__ == "__main__":
     print(_version)
```

### Comparing `gunpowder-1.2.2/gunpowder/zoo/tensorflow/unet.py` & `gunpowder-1.3.0/gunpowder/zoo/tensorflow/unet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import tensorflow as tf
 
+
 def conv_pass(
-        fmaps_in,
-        kernel_size,
-        num_fmaps,
-        num_repetitions,
-        activation='relu',
-        name='conv_pass'):
-    '''Create a convolution pass::
+    fmaps_in,
+    kernel_size,
+    num_fmaps,
+    num_repetitions,
+    activation="relu",
+    name="conv_pass",
+):
+    """Create a convolution pass::
 
         f_in --> f_1 --> ... --> f_n
 
     where each ``-->`` is a convolution followed by a (non-linear) activation
     function and ``n`` ``num_repetitions``. Each convolution will decrease the
     size of the feature maps by ``kernel_size-1``.
 
@@ -35,105 +37,108 @@
             How many convolutions to apply.
 
         activation:
 
             Which activation to use after a convolution. Accepts the name of any
             tensorflow activation function (e.g., ``relu`` for ``tf.nn.relu``).
 
-    '''
+    """
 
     fmaps = fmaps_in
     if activation is not None:
         activation = getattr(tf.nn, activation)
 
     conv_layer = getattr(
-        tf.layers,
-        {2: 'conv2d', 3: 'conv3d'}[fmaps_in.get_shape().ndims - 2])
+        tf.layers, {2: "conv2d", 3: "conv3d"}[fmaps_in.get_shape().ndims - 2]
+    )
 
     for i in range(num_repetitions):
         fmaps = conv_layer(
             inputs=fmaps,
             filters=num_fmaps,
             kernel_size=kernel_size,
-            padding='valid',
-            data_format='channels_first',
+            padding="valid",
+            data_format="channels_first",
             activation=activation,
-            name=name + '_%i'%i)
+            name=name + "_%i" % i,
+        )
 
     return fmaps
 
-def downsample(fmaps_in, factors, name='down'):
 
+def downsample(fmaps_in, factors, name="down"):
     pooling_layer = getattr(
         tf.layers,
-        {2: 'max_pooling2d', 3: 'max_pooling3d'}[fmaps_in.get_shape().ndims - 2])
+        {2: "max_pooling2d", 3: "max_pooling3d"}[fmaps_in.get_shape().ndims - 2],
+    )
 
     fmaps = pooling_layer(
         fmaps_in,
         pool_size=factors,
         strides=factors,
-        padding='valid',
-        data_format='channels_first',
-        name=name)
+        padding="valid",
+        data_format="channels_first",
+        name=name,
+    )
 
     return fmaps
 
-def upsample(fmaps_in, factors, num_fmaps, activation='relu', name='up'):
 
+def upsample(fmaps_in, factors, num_fmaps, activation="relu", name="up"):
     if activation is not None:
         activation = getattr(tf.nn, activation)
 
     conv_trans_layer = getattr(
         tf.layers,
-        {2: 'conv2d_transpose', 3: 'conv3d_transpose'}[fmaps_in.get_shape().ndims - 2])
+        {2: "conv2d_transpose", 3: "conv3d_transpose"}[fmaps_in.get_shape().ndims - 2],
+    )
 
     fmaps = conv_trans_layer(
         fmaps_in,
         filters=num_fmaps,
         kernel_size=factors,
         strides=factors,
-        padding='valid',
-        data_format='channels_first',
+        padding="valid",
+        data_format="channels_first",
         activation=activation,
-        name=name)
+        name=name,
+    )
 
     return fmaps
 
+
 def crop_spatial(fmaps_in, shape):
-    '''Crop only the spacial dimensions to match shape.
+    """Crop only the spacial dimensions to match shape.
 
     Args:
 
         fmaps_in:
 
             The input tensor.
 
         shape:
 
             A list (not a tensor) with the requested shape [_, _, z, y, x] or
             [_, _, y, x].
-    '''
+    """
 
     in_shape = fmaps_in.get_shape().as_list()
 
     offset = [0, 0] + [(in_shape[i] - shape[i]) // 2 for i in range(2, len(shape))]
     size = in_shape[0:2] + shape[2:]
 
     fmaps = tf.slice(fmaps_in, offset, size)
 
     return fmaps
 
+
 def unet(
-        fmaps_in,
-        num_fmaps,
-        fmap_inc_factor,
-        downsample_factors,
-        activation='relu',
-        layer=0):
-    '''Create a 2D or 3D U-Net::
+    fmaps_in, num_fmaps, fmap_inc_factor, downsample_factors, activation="relu", layer=0
+):
+    """Create a 2D or 3D U-Net::
 
         f_in --> f_left --------------------------->> f_right--> f_out
                     |                                   ^
                     v                                   |
                  g_in --> g_left ------->> g_right --> g_out
                              |               ^
                              v               |
@@ -175,60 +180,62 @@
 
             Which activation to use after a convolution. Accepts the name of any
             tensorflow activation function (e.g., ``relu`` for ``tf.nn.relu``).
 
         layer:
 
             Used internally to build the U-Net recursively.
-    '''
+    """
 
-    prefix = "    "*layer
-    print(prefix + "Creating U-Net layer %i"%layer)
+    prefix = "    " * layer
+    print(prefix + "Creating U-Net layer %i" % layer)
     print(prefix + "f_in: " + str(fmaps_in.shape))
 
     # convolve
     f_left = conv_pass(
         fmaps_in,
         kernel_size=3,
         num_fmaps=num_fmaps,
         num_repetitions=2,
         activation=activation,
-        name='unet_layer_%i_left'%layer)
+        name="unet_layer_%i_left" % layer,
+    )
 
     # last layer does not recurse
-    bottom_layer = (layer == len(downsample_factors))
+    bottom_layer = layer == len(downsample_factors)
     if bottom_layer:
         print(prefix + "bottom layer")
         print(prefix + "f_out: " + str(f_left.shape))
         return f_left
 
     # downsample
     g_in = downsample(
-        f_left,
-        downsample_factors[layer],
-        'unet_down_%i_to_%i'%(layer, layer + 1))
+        f_left, downsample_factors[layer], "unet_down_%i_to_%i" % (layer, layer + 1)
+    )
 
     # recursive U-net
     g_out = unet(
         g_in,
-        num_fmaps=num_fmaps*fmap_inc_factor,
+        num_fmaps=num_fmaps * fmap_inc_factor,
         fmap_inc_factor=fmap_inc_factor,
         downsample_factors=downsample_factors,
         activation=activation,
-        layer=layer+1)
+        layer=layer + 1,
+    )
 
     print(prefix + "g_out: " + str(g_out.shape))
 
     # upsample
     g_out_upsampled = upsample(
         g_out,
         downsample_factors[layer],
         num_fmaps,
         activation=activation,
-        name='unet_up_%i_to_%i'%(layer + 1, layer))
+        name="unet_up_%i_to_%i" % (layer + 1, layer),
+    )
 
     print(prefix + "g_out_upsampled: " + str(g_out_upsampled.shape))
 
     # copy-crop
     f_left_cropped = crop_spatial(f_left, g_out_upsampled.get_shape().as_list())
 
     print(prefix + "f_left_cropped: " + str(f_left_cropped.shape))
@@ -240,12 +247,13 @@
 
     # convolve
     f_out = conv_pass(
         f_right,
         kernel_size=3,
         num_fmaps=num_fmaps,
         num_repetitions=2,
-        name='unet_layer_%i_right'%layer)
+        name="unet_layer_%i_right" % layer,
+    )
 
     print(prefix + "f_out: " + str(f_out.shape))
 
     return f_out
```

### Comparing `gunpowder-1.2.2/gunpowder.egg-info/SOURCES.txt` & `gunpowder-1.3.0/gunpowder.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+LICENSE
 README.md
-setup.py
+pyproject.toml
 gunpowder/__init__.py
 gunpowder/array.py
 gunpowder/array_spec.py
 gunpowder/batch.py
 gunpowder/batch_request.py
 gunpowder/build.py
 gunpowder/compat.py
@@ -33,48 +34,58 @@
 gunpowder/contrib/nodes/add_vector_map.py
 gunpowder/contrib/nodes/dvid_partner_annotation_source.py
 gunpowder/contrib/nodes/hdf5_points_source.py
 gunpowder/contrib/nodes/prepare_malis.py
 gunpowder/contrib/nodes/zero_out_const_sections.py
 gunpowder/ext/__init__.py
 gunpowder/ext/zarr_file.py
+gunpowder/jax/__init__.py
+gunpowder/jax/generic_jax_model.py
+gunpowder/jax/nodes/__init__.py
+gunpowder/jax/nodes/predict.py
+gunpowder/jax/nodes/train.py
 gunpowder/nodes/__init__.py
 gunpowder/nodes/add_affinities.py
+gunpowder/nodes/astype.py
 gunpowder/nodes/balance_labels.py
 gunpowder/nodes/batch_filter.py
 gunpowder/nodes/batch_provider.py
 gunpowder/nodes/crop.py
 gunpowder/nodes/csv_points_source.py
 gunpowder/nodes/daisy_request_blocks.py
 gunpowder/nodes/defect_augment.py
+gunpowder/nodes/deform_augment.py
 gunpowder/nodes/downsample.py
 gunpowder/nodes/dvid_source.py
 gunpowder/nodes/elastic_augment.py
 gunpowder/nodes/exclude_labels.py
 gunpowder/nodes/generic_predict.py
 gunpowder/nodes/generic_train.py
+gunpowder/nodes/graph_source.py
 gunpowder/nodes/grow_boundary.py
 gunpowder/nodes/hdf5_source.py
 gunpowder/nodes/hdf5_write.py
 gunpowder/nodes/hdf5like_source_base.py
 gunpowder/nodes/hdf5like_write_base.py
 gunpowder/nodes/intensity_augment.py
 gunpowder/nodes/intensity_scale_shift.py
+gunpowder/nodes/iterate_locations.py
 gunpowder/nodes/klb_source.py
 gunpowder/nodes/merge_provider.py
 gunpowder/nodes/noise_augment.py
 gunpowder/nodes/normalize.py
 gunpowder/nodes/pad.py
 gunpowder/nodes/precache.py
 gunpowder/nodes/print_profiling_stats.py
 gunpowder/nodes/random_location.py
 gunpowder/nodes/random_provider.py
 gunpowder/nodes/rasterize_graph.py
 gunpowder/nodes/reject.py
 gunpowder/nodes/renumber_connected_components.py
+gunpowder/nodes/resample.py
 gunpowder/nodes/scan.py
 gunpowder/nodes/shift_augment.py
 gunpowder/nodes/simple_augment.py
 gunpowder/nodes/snapshot.py
 gunpowder/nodes/specified_location.py
 gunpowder/nodes/squeeze.py
 gunpowder/nodes/stack.py
```

