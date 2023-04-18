# Comparing `tmp/dask-cuda-23.6.0a230328.tar.gz` & `tmp/dask-cuda-23.6.0a230417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-23.6.0a230328.tar", last modified: Tue Mar 28 13:57:20 2023, max compression
+gzip compressed data, was "dask-cuda-23.6.0a230417.tar", last modified: Tue Apr 18 05:02:15 2023, max compression
```

## Comparing `dask-cuda-23.6.0a230328.tar` & `dask-cuda-23.6.0a230417.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1974 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)     1522 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/dask_cuda/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.239824 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6350 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12437 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8598 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10752 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    25569 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15828 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8589 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)    11043 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.239824 dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20062 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17302 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    15517 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    12036 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    15675 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18492 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     9408 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    29112 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.239824 dask-cuda-23.6.0a230328/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1974 2023-03-28 13:57:20.000000 dask-cuda-23.6.0a230328/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-03-28 13:57:20.000000 dask-cuda-23.6.0a230328/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 13:57:20.000000 dask-cuda-23.6.0a230328/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-03-28 13:57:20.000000 dask-cuda-23.6.0a230328/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-03-28 13:57:20.000000 dask-cuda-23.6.0a230328/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-03-28 13:57:20.000000 dask-cuda-23.6.0a230328/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.235824 dask-cuda-23.6.0a230328/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/rtd/
--rw-r--r--   0 root         (0) root         (0)     6223 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/rtd/conf.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-28 13:57:20.243824 dask-cuda-23.6.0a230328/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      953 2023-03-28 13:57:12.000000 dask-cuda-23.6.0a230328/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/dask_cuda/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.019385 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10752 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15828 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8589 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)    11043 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.019385 dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.019385 dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20062 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17302 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29880 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    15517 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    12036 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    15675 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18492 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23464 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     9408 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    29112 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.019385 dask-cuda-23.6.0a230417/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-18 05:02:15.000000 dask-cuda-23.6.0a230417/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-04-18 05:02:15.000000 dask-cuda-23.6.0a230417/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 05:02:15.000000 dask-cuda-23.6.0a230417/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-04-18 05:02:15.000000 dask-cuda-23.6.0a230417/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      209 2023-04-18 05:02:15.000000 dask-cuda-23.6.0a230417/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-18 05:02:15.000000 dask-cuda-23.6.0a230417/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.015385 dask-cuda-23.6.0a230417/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/rtd/
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/rtd/conf.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 05:02:15.023385 dask-cuda-23.6.0a230417/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      953 2023-04-18 05:02:07.000000 dask-cuda-23.6.0a230417/setup.py
```

### Comparing `dask-cuda-23.6.0a230328/LICENSE` & `dask-cuda-23.6.0a230417/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/PKG-INFO` & `dask-cuda-23.6.0a230417/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.6.0a230328
+Version: 23.6.0a230417
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.6.0a230328/README.md` & `dask-cuda-23.6.0a230417/README.md`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/__init__.py` & `dask-cuda-23.6.0a230417/dask_cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/benchmarks/common.py` & `dask-cuda-23.6.0a230417/dask_cuda/benchmarks/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         args.rmm_pool_size,
         args.disable_rmm_pool,
         args.enable_rmm_async,
         args.enable_rmm_managed,
         args.rmm_release_threshold,
         args.rmm_log_directory,
         args.enable_rmm_statistics,
+        args.enable_rmm_track_allocations,
     )
     address_to_index, results, message_data = gather_bench_results(client, args, config)
     p2p_bw = peer_to_peer_bandwidths(message_data, address_to_index)
     config.pretty_print_results(args, address_to_index, p2p_bw, results)
     if args.output_basename:
         df, p2p_bw = config.create_tidy_results(args, p2p_bw, results)
         df["num_workers"] = len(address_to_index)
```

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-23.6.0a230417/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/benchmarks/utils.py` & `dask-cuda-23.6.0a230417/dask_cuda/benchmarks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,25 @@
         "--enable-rmm-statistics",
         action="store_true",
         help="Use RMM's StatisticsResourceAdaptor to gather allocation statistics. "
         "This enables spilling implementations such as JIT-Unspill to provides more "
         "information on out-of-memory errors",
     )
     cluster_args.add_argument(
+        "--enable-rmm-track-allocations",
+        action="store_true",
+        help="When enabled, wraps the memory resource used by each worker with a "
+        "``rmm.mr.TrackingResourceAdaptor``, which tracks the amount of memory "
+        "allocated."
+        "NOTE: This option enables additional diagnostics to be collected and "
+        "reported by the Dask dashboard. However, there is significant overhead "
+        "associated with this and it should only be used for debugging and memory "
+        "profiling.",
+    )
+    cluster_args.add_argument(
         "--enable-tcp-over-ucx",
         default=None,
         action="store_true",
         dest="enable_tcp_over_ucx",
         help="Enable TCP over UCX.",
     )
     cluster_args.add_argument(
@@ -206,14 +217,21 @@
         type=str,
         dest="scheduler_file",
         help="Read cluster configuration from specified file. "
         "If provided, worker configuration options provided to this script are ignored "
         "since the workers are assumed to be started separately. Similarly the other "
         "cluster configuration options have no effect.",
     )
+    group.add_argument(
+        "--dashboard-address",
+        default=None,
+        type=str,
+        help="Address on which to listen for diagnostics dashboard, ignored if "
+        "either ``--scheduler-address`` or ``--scheduler-file`` is specified.",
+    )
     cluster_args.add_argument(
         "--shutdown-external-cluster-on-exit",
         default=False,
         action="store_true",
         dest="shutdown_cluster",
         help="If connecting to an external cluster, should we shut down the cluster "
         "when the benchmark exits?",
@@ -313,15 +331,19 @@
     if args.multi_node is True:
         Cluster = SSHCluster
         cluster_args = [args.hosts.split(",")]
         scheduler_addr = args.protocol + "://" + cluster_args[0][0] + ":8786"
 
         cluster_kwargs = {
             "connect_options": {"known_hosts": None},
-            "scheduler_options": {"protocol": args.protocol, "port": 8786},
+            "scheduler_options": {
+                "protocol": args.protocol,
+                "port": 8786,
+                "dashboard_address": args.dashboard_address,
+            },
             "worker_class": "dask_cuda.CUDAWorker",
             "worker_options": {
                 "protocol": args.protocol,
                 "nthreads": args.threads_per_worker,
                 "interface": args.interface,
                 "device_memory_limit": args.device_memory_limit,
             },
@@ -330,14 +352,15 @@
         }
     else:
         Cluster = LocalCUDACluster
         scheduler_addr = None
         cluster_args = []
         cluster_kwargs = {
             "protocol": args.protocol,
+            "dashboard_address": args.dashboard_address,
             "n_workers": len(args.devs.split(",")),
             "threads_per_worker": args.threads_per_worker,
             "CUDA_VISIBLE_DEVICES": args.devs,
             "interface": args.interface,
             "device_memory_limit": args.device_memory_limit,
             **ucx_options,
         }
@@ -366,14 +389,15 @@
     pool_size=None,
     disable_pool=False,
     rmm_async=False,
     rmm_managed=False,
     release_threshold=None,
     log_directory=None,
     statistics=False,
+    rmm_track_allocations=False,
 ):
     import cupy
 
     import rmm
     from rmm.allocators.cupy import rmm_cupy_allocator
 
     from dask_cuda.utils import get_rmm_log_file_name
@@ -395,50 +419,57 @@
             log_file_name=get_rmm_log_file_name(dask_worker, logging, log_directory),
         )
     cupy.cuda.set_allocator(rmm_cupy_allocator)
     if statistics:
         rmm.mr.set_current_device_resource(
             rmm.mr.StatisticsResourceAdaptor(rmm.mr.get_current_device_resource())
         )
+    if rmm_track_allocations:
+        rmm.mr.set_current_device_resource(
+            rmm.mr.TrackingResourceAdaptor(rmm.mr.get_current_device_resource())
+        )
 
 
 def setup_memory_pools(
     client,
     is_gpu,
     pool_size,
     disable_pool,
     rmm_async,
     rmm_managed,
     release_threshold,
     log_directory,
     statistics,
+    rmm_track_allocations,
 ):
     if not is_gpu:
         return
     client.run(
         setup_memory_pool,
         pool_size=pool_size,
         disable_pool=disable_pool,
         rmm_async=rmm_async,
         rmm_managed=rmm_managed,
         release_threshold=release_threshold,
         log_directory=log_directory,
         statistics=statistics,
+        rmm_track_allocations=rmm_track_allocations,
     )
     # Create an RMM pool on the scheduler due to occasional deserialization
     # of CUDA objects. May cause issues with InfiniBand otherwise.
     client.run_on_scheduler(
         setup_memory_pool,
         pool_size=1e9,
         disable_pool=disable_pool,
         rmm_async=rmm_async,
         rmm_managed=rmm_managed,
         release_threshold=release_threshold,
         log_directory=log_directory,
         statistics=statistics,
+        rmm_track_allocations=rmm_track_allocations,
     )
 
 
 def save_benchmark_data(
     basename,
     address_to_index: Mapping[str, int],
     timing_data: pd.DataFrame,
```

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/cli.py` & `dask-cuda-23.6.0a230417/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/cuda_worker.py` & `dask-cuda-23.6.0a230417/dask_cuda/cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/device_host_file.py` & `dask-cuda-23.6.0a230417/dask_cuda/device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/disk_io.py` & `dask-cuda-23.6.0a230417/dask_cuda/disk_io.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/comms.py` & `dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-23.6.0a230417/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/get_device_memory_objects.py` & `dask-cuda-23.6.0a230417/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/initialize.py` & `dask-cuda-23.6.0a230417/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/is_device_object.py` & `dask-cuda-23.6.0a230417/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/is_spillable_object.py` & `dask-cuda-23.6.0a230417/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/local_cuda_cluster.py` & `dask-cuda-23.6.0a230417/dask_cuda/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/proxify_device_objects.py` & `dask-cuda-23.6.0a230417/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/proxify_host_file.py` & `dask-cuda-23.6.0a230417/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/proxy_object.py` & `dask-cuda-23.6.0a230417/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_dgx.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_explicit_comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_gds.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_initialize.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_proxy.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_spill.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_spill.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_utils.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-23.6.0a230417/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/utils.py` & `dask-cuda-23.6.0a230417/dask_cuda/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda/worker_spec.py` & `dask-cuda-23.6.0a230417/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-23.6.0a230417/dask_cuda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.6.0a230328
+Version: 23.6.0a230417
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.6.0a230328/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-23.6.0a230417/dask_cuda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/examples/ucx/client_initialize.py` & `dask-cuda-23.6.0a230417/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/examples/ucx/local_cuda_cluster.py` & `dask-cuda-23.6.0a230417/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/pyproject.toml` & `dask-cuda-23.6.0a230417/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "NVIDIA Corporation" },
 ]
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 dependencies = [
-    "dask >=2023.1.1",
-    "distributed >=2023.1.1",
+    "dask ==2023.3.2",
+    "distributed ==2023.3.2.1",
     "pynvml >=11.0.0,<11.5",
     "numpy >=1.21",
     "numba >=0.54",
     "pandas >=1.3,<1.6.0dev0",
     "zict >=0.1.3",
 ]
 classifiers = [
```

### Comparing `dask-cuda-23.6.0a230328/rtd/conf.py` & `dask-cuda-23.6.0a230417/rtd/conf.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230328/setup.py` & `dask-cuda-23.6.0a230417/setup.py`

 * *Files identical despite different names*

