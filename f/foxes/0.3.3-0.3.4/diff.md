# Comparing `tmp/foxes-0.3.3.tar.gz` & `tmp/foxes-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.3.3.tar", last modified: Wed Mar 15 10:39:30 2023, max compression
+gzip compressed data, was "foxes-0.3.4.tar", last modified: Tue Apr 18 09:48:26 2023, max compression
```

## Comparing `foxes-0.3.3.tar` & `foxes-0.3.4.tar`

### file list

```diff
@@ -1,253 +1,259 @@
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.931264 foxes-0.3.3/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1071 2022-11-21 08:01:11.000000 foxes-0.3.3/LICENSE
--rw-r--r--   0 jonas     (1000) jonas     (1000)    40774 2022-11-21 08:01:11.000000 foxes-0.3.3/Logo_FOXES.svg
--rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2022-12-20 07:43:15.000000 foxes-0.3.3/MANIFEST.in
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6579 2023-03-15 10:39:30.931264 foxes-0.3.3/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5753 2023-03-14 07:02:54.000000 foxes-0.3.3/README.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-03-14 07:11:40.000000 foxes-0.3.3/foxes/VERSION
--rw-r--r--   0 jonas     (1000) jonas     (1000)      712 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/algorithms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      131 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/algorithms/downwind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       53 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/algorithms/downwind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17373 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/algorithms/downwind/downwind.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/algorithms/downwind/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      242 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/algorithms/downwind/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2292 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/downwind/models/calc_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3339 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4368 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1876 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1436 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/algorithms/iterative/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/iterative/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2056 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/iterative/iterative.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/algorithms/iterative/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      161 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/iterative/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5083 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/iterative/models/convergence.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3297 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4084 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/algorithms/iterative/models/loop_runner.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)       70 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/constants.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      762 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14868 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/core/algorithm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2815 2023-02-13 07:42:18.000000 foxes-0.3.3/foxes/core/data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7861 2023-03-03 07:14:48.000000 foxes-0.3.3/foxes/core/data_calc_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12080 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/core/farm_controller.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7098 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/core/farm_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      246 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/core/farm_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5439 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/core/model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5062 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/core/partial_wakes_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6952 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/core/point_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12685 2023-02-13 07:43:05.000000 foxes-0.3.3/foxes/core/rotor_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8006 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/core/states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2929 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/core/turbine.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1058 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/core/turbine_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      926 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/core/turbine_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1619 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/core/vertical_profile.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6499 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/core/wake_frame.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2901 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/core/wake_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2540 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/core/wake_superposition.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1636 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/core/wind_farm.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/data/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      120 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/data/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/data/farms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/farms/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1872 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/farms/test_farm_67.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2921 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/data/parse.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/data/power_ct_curves/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      410 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      300 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      851 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      401 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/power_ct_curves/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes/data/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)   427815 2022-11-29 07:36:46.000000 foxes-0.3.3/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/states/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)   126124 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/states/abl_states_6000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    29085 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/data/states/timeseries_3000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    78694 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/states/timeseries_8000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4943 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/states/wind_rose_bremen.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10990 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/states/wind_rotation.nc
--rw-r--r--   0 jonas     (1000) jonas     (1000)      519 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/data/static_data.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/input/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       47 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/input/farm_layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      181 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/farm_layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2997 2022-12-20 07:58:50.000000 foxes-0.3.3/foxes/input/farm_layout/add_from_csv.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1561 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/farm_layout/add_from_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1619 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/farm_layout/add_from_json.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1444 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/farm_layout/add_grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1175 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/farm_layout/add_row.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/input/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      244 2023-02-27 10:01:22.000000 foxes-0.3.3/foxes/input/states/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/input/states/create/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       81 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/states/create/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3248 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/input/states/create/random_abl_states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    16412 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/input/states/field_data_nc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12359 2023-03-14 06:54:40.000000 foxes-0.3.3/foxes/input/states/multi_height.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4362 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/input/states/scan_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5734 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/input/states/single.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10477 2023-03-14 06:54:40.000000 foxes-0.3.3/foxes/input/states/states_table.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      349 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/farm_controllers/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       39 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/farm_controllers/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      211 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/farm_controllers/basic.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/farm_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       44 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/farm_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3347 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/models/farm_models/turbine2farm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12536 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/model_book.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/partial_wakes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/partial_wakes/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10395 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/partial_wakes/axiwake.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10687 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/partial_wakes/distsliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2571 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/partial_wakes/grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7406 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/partial_wakes/mapped.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6098 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/partial_wakes/rotor_points.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9581 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/partial_wakes/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/point_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      108 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/models/point_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4468 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/point_models/set_uniform_data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1372 2022-12-20 07:58:50.000000 foxes-0.3.3/foxes/models/point_models/tke2ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1935 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/point_models/wake_deltas.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/rotor_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       60 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/rotor_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5582 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/rotor_models/centre.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4843 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/rotor_models/grid.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/turbine_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      348 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/models/turbine_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2533 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/models/turbine_models/calculator.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2511 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/models/turbine_models/kTI_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5390 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/models/turbine_models/power_mask.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7409 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/turbine_models/sector_management.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3393 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/turbine_models/set_XYHD.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3879 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/turbine_models/set_farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5120 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/turbine_models/table_factors.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2060 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/turbine_models/thrust2ct.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1580 2022-12-20 07:58:50.000000 foxes-0.3.3/foxes/models/turbine_models/yaw2yawm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1551 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/turbine_models/yawm2yaw.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/turbine_types/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7386 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/turbine_types/PCt_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8599 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/turbine_types/PCt_two_files.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/models/turbine_types/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1284 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/turbine_types/null_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11131 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/turbine_types/wsrho2PCt_two_files.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/vertical_profiles/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       59 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/vertical_profiles/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/vertical_profiles/abl_log/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      244 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/vertical_profiles/abl_log/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1082 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1161 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1173 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2495 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1151 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/vertical_profiles/abl_log/sheared_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/vertical_profiles/uniform.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/wake_frames/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      137 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_frames/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4646 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_frames/farm_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3740 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_frames/rotor_wd.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11929 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/models/wake_frames/streamlines.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8001 2023-03-09 13:41:59.000000 foxes-0.3.3/foxes/models/wake_frames/yawed_wakes.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/wake_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      207 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/wake_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2672 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/wake_models/axisymmetric.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6535 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_models/dist_sliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2637 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/models/wake_models/gaussian.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/wake_models/ti/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       82 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/wake_models/ti/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8169 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5947 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_models/ti/iec_ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5038 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/wake_models/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/wake_models/wind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      178 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_models/wind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5278 2023-02-06 08:55:24.000000 foxes-0.3.3/foxes/models/wake_models/wind/bastankhah.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4768 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/models/wake_models/wind/jensen.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14461 2023-03-09 13:41:59.000000 foxes-0.3.3/foxes/models/wake_models/wind/porte_agel.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11735 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_models/wind/turbopark.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/models/wake_superpositions/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      159 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/wake_superpositions/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5889 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/models/wake_superpositions/linear.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6678 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_superpositions/max.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6470 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/models/wake_superpositions/quadratic.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4758 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/models/wake_superpositions/ti_superp.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/opt/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      139 2023-02-09 13:42:08.000000 foxes-0.3.3/foxes/opt/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/opt/constraints/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      114 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/opt/constraints/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5879 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/constraints/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7391 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/constraints/min_dist.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/opt/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2023-03-08 13:05:43.000000 foxes-0.3.3/foxes/opt/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1889 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/opt/core/farm_constraint.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1888 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/opt/core/farm_objective.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9490 2023-03-09 13:41:59.000000 foxes-0.3.3/foxes/opt/core/farm_opt_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7652 2023-03-08 13:11:48.000000 foxes-0.3.3/foxes/opt/core/farm_vars_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5570 2023-02-13 07:43:05.000000 foxes-0.3.3/foxes/opt/core/pop_states.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/opt/objectives/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      109 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/objectives/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8779 2023-03-09 13:41:59.000000 foxes-0.3.3/foxes/opt/objectives/farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3909 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/opt/objectives/max_n_turbines.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/opt/problems/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       61 2023-03-09 13:41:59.000000 foxes-0.3.3/foxes/opt/problems/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/opt/problems/layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      180 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5753 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/farm_layout.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      333 2023-03-08 12:08:09.000000 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7680 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8069 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7446 2023-03-08 12:08:09.000000 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9661 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    13910 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5984 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11665 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/reggrids_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10479 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/opt/problems/layout/regular_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    18815 2023-03-09 13:41:59.000000 foxes-0.3.3/foxes/opt/problems/opt_farm_vars.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/output/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      355 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/output/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10501 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/output/farm_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    15170 2023-03-14 06:54:40.000000 foxes-0.3.3/foxes/output/farm_results_eval.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    45206 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/output/flow_plots_2d.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2189 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/output/output.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2581 2022-12-20 07:58:50.000000 foxes-0.3.3/foxes/output/results_writer.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9970 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/output/rose_plot.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2347 2023-03-08 12:08:09.000000 foxes-0.3.3/foxes/output/state_turbine_map.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5452 2023-03-01 14:50:54.000000 foxes-0.3.3/foxes/output/turbine_type_curves.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/utils/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      453 2023-03-14 13:40:43.000000 foxes-0.3.3/foxes/utils/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.921264 foxes-0.3.3/foxes/utils/abl/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       88 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/utils/abl/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1278 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/abl/neutral.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      444 2023-01-27 13:11:08.000000 foxes-0.3.3/foxes/utils/abl/sheared.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1728 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/abl/stable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1530 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/abl/unstable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3313 2022-12-02 07:34:54.000000 foxes-0.3.3/foxes/utils/cubic_roots.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5141 2022-12-20 07:43:15.000000 foxes-0.3.3/foxes/utils/data_book.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      793 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/dict.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.931264 foxes-0.3.3/foxes/utils/geom2d/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      179 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/geom2d/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    18793 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/utils/geom2d/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4451 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/geom2d/circle.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1627 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/geom2d/example_intersection.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1751 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/geom2d/example_union.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6091 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/geom2d/half_plane.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5467 2023-03-14 13:15:51.000000 foxes-0.3.3/foxes/utils/geom2d/polygon.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7770 2023-03-15 07:55:36.000000 foxes-0.3.3/foxes/utils/geopandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4623 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/utils/pandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      350 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/utils/plotly_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5767 2023-03-03 07:14:48.000000 foxes-0.3.3/foxes/utils/runners.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      362 2023-03-08 12:07:41.000000 foxes-0.3.3/foxes/utils/subclasses.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2761 2022-11-21 08:01:11.000000 foxes-0.3.3/foxes/utils/two_circles.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2746 2022-12-20 07:58:50.000000 foxes-0.3.3/foxes/utils/wind_dir.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1268 2023-03-09 13:41:59.000000 foxes-0.3.3/foxes/variables.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-03-15 10:39:30.911264 foxes-0.3.3/foxes.egg-info/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6579 2023-03-15 10:39:30.000000 foxes-0.3.3/foxes.egg-info/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7491 2023-03-15 10:39:30.000000 foxes-0.3.3/foxes.egg-info/SOURCES.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-03-15 10:39:30.000000 foxes-0.3.3/foxes.egg-info/dependency_links.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)      189 2023-03-15 10:39:30.000000 foxes-0.3.3/foxes.egg-info/requires.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-03-15 10:39:30.000000 foxes-0.3.3/foxes.egg-info/top_level.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-03-15 10:39:30.000000 foxes-0.3.3/foxes.egg-info/zip-safe
--rw-r--r--   0 jonas     (1000) jonas     (1000)      185 2022-11-21 08:01:11.000000 foxes-0.3.3/pyproject.toml
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1132 2023-03-15 10:39:30.931264 foxes-0.3.3/setup.cfg
--rw-r--r--   0 jonas     (1000) jonas     (1000)       69 2022-11-21 08:01:11.000000 foxes-0.3.3/setup.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1071 2022-11-29 14:27:28.000000 foxes-0.3.4/LICENSE
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    40774 2022-11-29 14:27:28.000000 foxes-0.3.4/Logo_FOXES.svg
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      215 2023-03-07 14:47:39.000000 foxes-0.3.4/MANIFEST.in
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6589 2023-04-18 09:48:26.916066 foxes-0.3.4/PKG-INFO
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5769 2023-04-18 09:34:13.000000 foxes-0.3.4/README.md
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        6 2023-03-15 10:46:27.000000 foxes-0.3.4/foxes/VERSION
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      712 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      131 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/downwind/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       53 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/algorithms/downwind/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    17373 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/downwind.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/downwind/models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      242 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/algorithms/downwind/models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2292 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/calc_order.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3339 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4368 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1876 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1436 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/iterative/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       55 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2056 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/iterative.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/iterative/models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      161 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5083 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/convergence.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3297 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4084 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/loop_runner.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      201 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/constants.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/core/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      762 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    15807 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/core/algorithm.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2815 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/data.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7874 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/core/data_calc_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12080 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/farm_controller.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7098 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/farm_data_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      246 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/farm_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5439 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5062 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/partial_wakes_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6952 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/point_data_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12685 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/rotor_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8006 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/states.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2929 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/turbine.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1058 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/turbine_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1359 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/core/turbine_type.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1619 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/vertical_profile.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6499 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/wake_frame.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2901 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/wake_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2540 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/wake_superposition.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1636 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/wind_farm.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      120 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/farms/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/farms/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1872 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/farms/test_farm_67.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2921 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/data/parse.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/power_ct_curves/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      410 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      300 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      851 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      401 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/states/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)   427815 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)   126124 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/abl_states_6000.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    29085 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/timeseries_3000.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    78694 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/timeseries_8000.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4943 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/wind_rose_bremen.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10990 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/wind_rotation.nc
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      519 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/static_data.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       68 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/farm_layout/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      218 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/farm_layout/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3135 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_csv.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      550 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_df.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1561 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_file.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1619 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_json.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1444 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_grid.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1175 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_row.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/states/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      244 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/states/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/states/create/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       81 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/states/create/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3248 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/states/create/random_abl_states.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    15880 2023-04-13 06:31:59.000000 foxes-0.3.4/foxes/input/states/field_data_nc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12359 2023-03-14 07:04:35.000000 foxes-0.3.4/foxes/input/states/multi_height.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4362 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/input/states/scan_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5734 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/input/states/single.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10477 2023-03-14 07:04:35.000000 foxes-0.3.4/foxes/input/states/states_table.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/windio/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       29 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/windio/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8809 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/windio/windio.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      349 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/farm_controllers/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       39 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/farm_controllers/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      211 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/farm_controllers/basic.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/farm_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       44 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/farm_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3347 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/farm_models/turbine2farm.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12536 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/model_book.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/partial_wakes/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      212 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/partial_wakes/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10395 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/axiwake.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10687 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/distsliced.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2571 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/partial_wakes/grid.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7406 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/mapped.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6098 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/rotor_points.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     9581 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/top_hat.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/point_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      108 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/point_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4468 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/point_models/set_uniform_data.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1372 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/point_models/tke2ti.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1935 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/point_models/wake_deltas.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/rotor_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       60 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/rotor_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5582 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/rotor_models/centre.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4843 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/rotor_models/grid.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/turbine_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      348 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2533 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/calculator.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2511 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/kTI_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5390 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/power_mask.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7409 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/sector_management.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3393 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/turbine_models/set_XYHD.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3879 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/set_farm_vars.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5120 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/table_factors.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2060 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/turbine_models/thrust2ct.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1580 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/yaw2yawm.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1551 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/yawm2yaw.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/turbine_types/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1422 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/CpCt_file.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2056 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/CpCt_from_two.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7686 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/PCt_file.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8877 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/PCt_from_two.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      221 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1284 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/turbine_types/null_type.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11131 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_types/wsrho2PCt_two_files.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/vertical_profiles/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       59 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      244 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1082 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1161 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1173 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2495 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1151 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/sheared_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      375 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/uniform.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_frames/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      137 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4646 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/farm_order.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3740 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/rotor_wd.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11929 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/streamlines.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8001 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/yawed_wakes.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      207 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2672 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/axisymmetric.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6535 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/dist_sliced.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2637 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/gaussian.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_models/ti/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       82 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/ti/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8169 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5947 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/ti/iec_ti.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5038 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/top_hat.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_models/wind/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      178 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5278 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/bastankhah.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4768 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/jensen.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    14461 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/porte_agel.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11735 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/turbopark.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_superpositions/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      159 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_superpositions/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5889 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_superpositions/linear.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6678 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_superpositions/max.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6470 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_superpositions/quadratic.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4758 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_superpositions/ti_superp.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/opt/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      139 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/opt/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/constraints/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      114 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/opt/constraints/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5879 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/constraints/area_geometry.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7391 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/constraints/min_dist.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/core/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      212 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1889 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_constraint.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1888 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_objective.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     9490 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_opt_problem.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7652 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_vars_problem.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5570 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/pop_states.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/objectives/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      109 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/objectives/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8779 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/objectives/farm_vars.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3909 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/objectives/max_n_turbines.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/problems/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       61 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/problems/layout/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      180 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5753 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/farm_layout.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      333 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7680 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8069 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7446 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     9661 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    13910 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5984 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11665 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/reggrids_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10479 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/regular_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    18815 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/opt_farm_vars.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/output/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      355 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/output/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10501 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/farm_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    15715 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/output/farm_results_eval.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    45206 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/flow_plots_2d.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2189 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/output.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2581 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/results_writer.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     9970 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/rose_plot.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2347 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/state_turbine_map.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5452 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/turbine_type_curves.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/utils/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      453 2023-03-15 10:38:11.000000 foxes-0.3.4/foxes/utils/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/utils/abl/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       88 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/abl/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1278 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/abl/neutral.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      444 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/abl/sheared.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1728 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/abl/stable.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1530 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/abl/unstable.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3313 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/cubic_roots.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5141 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/data_book.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      793 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/dict.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/utils/geom2d/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      179 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    18793 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/geom2d/area_geometry.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4451 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/circle.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1627 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/example_intersection.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1751 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/example_union.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6091 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/half_plane.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5467 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/polygon.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7770 2023-03-15 10:38:11.000000 foxes-0.3.4/foxes/utils/geopandas_helpers.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4623 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/pandas_helpers.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      350 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/plotly_helpers.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5802 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/utils/runners.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      362 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/subclasses.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2761 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/two_circles.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2746 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/wind_dir.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1268 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/variables.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes.egg-info/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6589 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/PKG-INFO
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7673 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        1 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      194 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/requires.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        6 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/top_level.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        1 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/zip-safe
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      185 2022-11-29 14:27:28.000000 foxes-0.3.4/pyproject.toml
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1130 2023-04-18 09:48:26.916066 foxes-0.3.4/setup.cfg
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       69 2022-11-29 14:27:28.000000 foxes-0.3.4/setup.py
```

### Comparing `foxes-0.3.3/LICENSE` & `foxes-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/Logo_FOXES.svg` & `foxes-0.3.4/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/PKG-INFO` & `foxes-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.3.3
+Version: 0.3.4
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
 Keywords: Wind farm,Wake modelling,Wind farm optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: scripts
 License-File: LICENSE
 
 # Welcome to foxes
@@ -51,14 +51,15 @@
 
 The supported Python versions are: 
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
+- `Python 3.11`
 
 ## Installation via conda
 
 ### Virtual Python environment
 
 First create a new `conda` environment, for example called `foxes`, by
```

### Comparing `foxes-0.3.3/README.md` & `foxes-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 The supported Python versions are: 
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
+- `Python 3.11`
 
 ## Installation via conda
 
 ### Virtual Python environment
 
 First create a new `conda` environment, for example called `foxes`, by
```

### Comparing `foxes-0.3.3/foxes/__init__.py` & `foxes-0.3.4/foxes/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/downwind/downwind.py` & `foxes-0.3.4/foxes/algorithms/downwind/downwind.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/downwind/models/calc_order.py` & `foxes-0.3.4/foxes/algorithms/downwind/models/calc_order.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.3.4/foxes/algorithms/downwind/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.3.4/foxes/algorithms/downwind/models/point_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/iterative/iterative.py` & `foxes-0.3.4/foxes/algorithms/iterative/iterative.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.3.4/foxes/algorithms/iterative/models/convergence.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.3.4/foxes/algorithms/iterative/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/algorithms/iterative/models/loop_runner.py` & `foxes-0.3.4/foxes/algorithms/iterative/models/loop_runner.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/__init__.py` & `foxes-0.3.4/foxes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/algorithm.py` & `foxes-0.3.4/foxes/core/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import xarray as xr
 
 from .model import Model
 from .farm_data_model import FarmDataModelList
 from .point_data_model import PointDataModelList
 from .farm_controller import FarmController
 from foxes.data import StaticData
-from foxes.utils import Dict
+from foxes.utils import Dict, all_subclasses
 import foxes.variables as FV
 
-
 class Algorithm(Model):
     """
     Abstract base class for algorithms.
 
     Algorithms collect required objects for running
     calculations, and contain the calculation functions
     which are meant to be called from top level code.
@@ -395,7 +394,41 @@
             Clear idata memory, including keep_models entries
 
         """
         if clear_mem:
             self._idata_mem = Dict()
         if self.initialized:
             super().finalize(self, self.verbosity)
+
+    @classmethod
+    def new(cls, algo_type, *args, **kwargs):
+        """
+        Run-time algorithm factory.
+
+        Parameters
+        ----------
+        algo_type : str
+            The selected derived class name
+        args : tuple, optional
+            Additional parameters for the constructor
+        kwargs : dict, optional
+            Additional parameters for the constructor
+
+        """
+
+        if algo_type is None:
+            return None
+
+        allc = all_subclasses(cls)
+        found = algo_type in [scls.__name__ for scls in allc]
+
+        if found:
+            for scls in allc:
+                if scls.__name__ == algo_type:
+                    return scls(*args, **kwargs)
+
+        else:
+            estr = "Algorithm type '{}' is not defined, available types are \n {}".format(
+                algo_type, sorted([i.__name__ for i in allc])
+            )
+            raise KeyError(estr)
+
```

### Comparing `foxes-0.3.3/foxes/core/data.py` & `foxes-0.3.4/foxes/core/data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/data_calc_model.py` & `foxes-0.3.4/foxes/core/data_calc_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import numpy as np
 import xarray as xr
 from abc import abstractmethod
 from dask.distributed import progress
+from dask.diagnostics import ProgressBar
 
 from .model import Model
 from .data import Data
+from foxes.utils.runners import DaskRunner
 import foxes.variables as FV
 import foxes.constants as FC
 
 
+
 class DataCalcModel(Model):
     """
     Abstract base class for models with
     that run calculation on xarray Dataset
     data.
 
     The calculations are run via xarray's
@@ -243,19 +246,15 @@
             dask="parallelized",
             dask_gufunc_kwargs=dargs,
             kwargs=wargs,
         )
 
         # reorganize results Dataset:
         results = (
-            results.assign_coords({FV.VARS: out_vars}).to_dataset(dim=FV.VARS).persist()
+            results.assign_coords({FV.VARS: out_vars}).to_dataset(dim=FV.VARS)
         )
 
-        # try to show progress bar:
-        if algo.verbosity > 0:
-            try:
-                progress(results)
-            except ValueError:
-                pass
+        if DaskRunner.is_distributed() and len(ProgressBar.active):
+            progress(results.persist())
 
         # update data by calculation results:
         return results.compute()
```

### Comparing `foxes-0.3.3/foxes/core/farm_controller.py` & `foxes-0.3.4/foxes/core/farm_controller.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/farm_data_model.py` & `foxes-0.3.4/foxes/core/farm_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/model.py` & `foxes-0.3.4/foxes/core/model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/partial_wakes_model.py` & `foxes-0.3.4/foxes/core/partial_wakes_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/point_data_model.py` & `foxes-0.3.4/foxes/core/point_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/rotor_model.py` & `foxes-0.3.4/foxes/core/rotor_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/states.py` & `foxes-0.3.4/foxes/core/states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/turbine.py` & `foxes-0.3.4/foxes/core/turbine.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/turbine_model.py` & `foxes-0.3.4/foxes/core/turbine_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/turbine_type.py` & `foxes-0.3.4/foxes/core/turbine_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .turbine_model import TurbineModel
-
+import foxes.constants as FC
 
 class TurbineType(TurbineModel):
     """
     Abstract base class for turbine type models.
 
     Rotor diameter and hub height can be overwritten
     by individual settings in the Turbine object.
@@ -14,28 +14,44 @@
         The model name
     D : float, optional
         The rotor diameter
     H : float, optional
         The hub height
     P_nominal : float, optional
         The nominal power in kW
+    P_unit : str
+        The unit of power, choices:
+        W, kW, MW, GW
 
     Attributes
     ----------
     name : str
         The model name
     D : float
         The rotor diameter
     H : float
         The hub height
     P_nominal : float
         The nominal power in kW
+    P_unit : str
+        The unit of power
 
     """
 
-    def __init__(self, name=None, D=None, H=None, P_nominal=None):
+    def __init__(
+            self, 
+            name=None, 
+            D=None, 
+            H=None, 
+            P_nominal=None,
+            P_unit="kW"
+        ):
         super().__init__()
 
         self.name = name if name is not None else type(self).__name__
         self.D = D
         self.H = H
         self.P_nominal = P_nominal
+        self.P_unit = P_unit
+
+        if P_unit not in FC.P_UNITS:
+            raise KeyError(f"Turbine type '{self.name}': Unkown P_unit '{P_unit}', expecting {list(FC.P_UNITS.keys())}")
```

### Comparing `foxes-0.3.3/foxes/core/vertical_profile.py` & `foxes-0.3.4/foxes/core/vertical_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/wake_frame.py` & `foxes-0.3.4/foxes/core/wake_frame.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/wake_model.py` & `foxes-0.3.4/foxes/core/wake_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/wake_superposition.py` & `foxes-0.3.4/foxes/core/wake_superposition.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/core/wind_farm.py` & `foxes-0.3.4/foxes/core/wind_farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/farms/test_farm_67.csv` & `foxes-0.3.4/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/parse.py` & `foxes-0.3.4/foxes/data/parse.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.3.4/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.3.4/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.3.4/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.3.4/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.3.4/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.3.4/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/states/wind_rotation.nc` & `foxes-0.3.4/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/data/static_data.py` & `foxes-0.3.4/foxes/data/static_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/farm_layout/add_from_csv.py` & `foxes-0.3.4/foxes/input/farm_layout/add_from_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 
 from foxes.core import Turbine
 
 
 def add_from_csv(
     farm,
-    file_path,
+    data_source,
     col_index=None,
     col_name=None,
     col_x="x",
     col_y="y",
     col_H=None,
     col_D=None,
     col_id=None,
@@ -26,16 +26,16 @@
 
     Additional turbine_parameters are forwarded to the WindFarm.add_turbine().
 
     Parameters
     ----------
     farm : foxes.WindFarm
         The wind farm
-    file_path : str
-        The input csv file
+    data_source : str or pandas.DataFrame
+        The input csv file or data source
     col_index : str, optional
         The index column, or None
     col_name : str, optional
         The name column, or None
     col_x : str, optional
         The x column
     col_y : str, optional
@@ -61,17 +61,20 @@
     turbine_base_name_count_shift : bool, optional
         Start turbine names by 1 instead of 0
     verbosity : int
         The verbosity level, 0 = silent
 
     """
 
-    if verbosity:
-        print("Reading file", file_path)
-    data = pd.read_csv(file_path, index_col=col_index)
+    if isinstance(data_source, pd.DataFrame):
+        data = data_source
+    else:
+        if verbosity:
+            print("Reading file", data_source)
+        data = pd.read_csv(data_source, index_col=col_index)
 
     tmodels = turbine_parameters.pop("turbine_models", [])
     H = turbine_parameters.pop("H", None)
     D = turbine_parameters.pop("D", None)
 
     for i in data.index:
```

### Comparing `foxes-0.3.3/foxes/input/farm_layout/add_from_file.py` & `foxes-0.3.4/foxes/input/farm_layout/add_from_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/farm_layout/add_from_json.py` & `foxes-0.3.4/foxes/input/farm_layout/add_from_json.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/farm_layout/add_grid.py` & `foxes-0.3.4/foxes/input/farm_layout/add_grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/farm_layout/add_row.py` & `foxes-0.3.4/foxes/input/farm_layout/add_row.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/states/create/random_abl_states.py` & `foxes-0.3.4/foxes/input/states/create/random_abl_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/states/field_data_nc.py` & `foxes-0.3.4/foxes/input/states/field_data_nc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
+from pathlib import Path
 from scipy.interpolate import RegularGridInterpolator
+from copy import deepcopy
 
 from foxes.core import States
 from foxes.utils import wd2uv, uv2wd
-from foxes.data import STATES
+from foxes.data import STATES, StaticData
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class FieldDataNC(States):
     """
     Heterogeneous ambient states on a regular
@@ -45,14 +47,16 @@
         Flag for raising errors if bounds are exceeded
     fill_value : number, optional
         Fill value in case of exceeding bounds, if no bounds error
     time_format : str
         The datetime parsing format string
     sel : dict, optional
         Subset selection via xr.Dataset.sel()
+    verbosity : int
+        Verbosity level for pre_load file reading
 
     Attributes
     ----------
     data_source : str or xarray.Dataset
         The data or the file search pattern, should end with
         suffix '.nc'. One or many files.
     ovars : list of str
@@ -99,14 +103,15 @@
         h_coord="height",
         pre_load=True,
         weight_ncvar=None,
         bounds_error=True,
         fill_value=None,
         time_format="%Y-%m-%d_%H:%M:%S",
         sel=None,
+        verbosity=1
     ):
         super().__init__()
 
         self.data_source = data_source
         self.states_coord = states_coord
         self.ovars = output_vars
         self.fixed_vars = fixed_vars
@@ -122,20 +127,83 @@
 
         self.var2ncvar = {
             v: var2ncvar.get(v, v) for v in output_vars if v not in fixed_vars
         }
 
         self._inds = None
         self._N = None
+        self._weights = None
+
+        # pre-load file reading, usually prior to DaskRunner:
+        if not isinstance(self.data_source, xr.Dataset):
+
+            if "*" in str(self.data_source):
+                pass
+            else:
+                self.data_source = StaticData().get_file_path(STATES, self.data_source, check_raw=True)
+            if verbosity:
+                if pre_load:
+                    print(f"States '{self.name}': Reading data from '{self.data_source}'")
+                else:
+                    print(f"States '{self.name}': Reading index from '{self.data_source}'")
+
+            with xr.open_mfdataset(
+                str(self.data_source),
+                parallel=False,
+                concat_dim=self.states_coord,
+                combine="nested",
+                data_vars="minimal",
+                coords="minimal",
+                compat="override",
+            ) as ds:
+                
+                dss = ds if self.sel is None else ds.sel(self.sel)
+                if pre_load:
+                    self.data_source = dss.load()
+                else:
+                    self.data_source = dss
+                self._get_inds(dss)
+
+    def _get_inds(self, ds):
+        """
+        Helper function for index and weights 
+        reading
+        """
+        for c in [self.states_coord, self.x_coord, self.y_coord, self.h_coord]:
+            if not c in ds:
+                raise KeyError(
+                    f"States '{self.name}': Missing coordinate '{c}' in data"
+                )
 
+        self._inds = ds[self.states_coord].to_numpy()
+        if self.time_format is not None:
+            self._inds = pd.to_datetime(
+                self._inds, format=self.time_format
+            ).to_numpy()
+        self._N = len(self._inds)
+
+        if self.weight_ncvar is not None:
+            self._weights = ds[self.weight_ncvar].to_numpy()
+
+        for v in self.ovars:
+            if v in self.var2ncvar:
+                ncv = self.var2ncvar[v]
+                if not ncv in ds:
+                    raise KeyError(
+                        f"States '{self.name}': nc variable '{ncv}' not found in data, found: {sorted(list(ds.keys()))}"
+                    )
+            elif v not in self.fixed_vars:
+                raise ValueError(
+                    f"States '{self.name}': Variable '{v}' neither found in var2ncvar not in fixed_vars"
+                )  
+                
     def _get_data(self, ds, verbosity):
         """
         Helper function for data extraction
         """
-
         x = ds[self.x_coord].to_numpy()
         y = ds[self.y_coord].to_numpy()
         h = ds[self.h_coord].to_numpy()
         n_x = len(x)
         n_y = len(y)
         n_h = len(h)
         n_sts = ds.sizes[self.states_coord]
@@ -168,15 +236,14 @@
                 data[..., self._dkys[v]] = np.swapaxes(ds[ncv].to_numpy(), 2, 3)
         for v in vars_sh:
             ncv = self.var2ncvar[v]
             data[..., self._dkys[v]] = ds[ncv].to_numpy()[:, :, None, None]
         for v in vars_s:
             ncv = self.var2ncvar[v]
             data[..., self._dkys[v]] = ds[ncv].to_numpy()[:, None, None, None]
-
         if FV.WD in self.fixed_vars:
             data[..., self._dkys[FV.WD]] = np.full(
                 (n_sts, n_h, n_y, n_x), self.fixed_vars[FV.WD], dtype=FC.DTYPE
             )
 
         if verbosity > 1:
             print(f"\n{self.name}: Data ranges")
@@ -185,87 +252,14 @@
                 nn = np.sum(np.isnan(d))
                 print(
                     f"  {v}: {np.nanmin(d)} --> {np.nanmax(d)}, nans: {nn} ({100*nn/len(d.flat):.2f}%)"
                 )
 
         return data
 
-    def _read_nc(self, algo, pattern, verbosity):
-
-        def extract_data(ds):
-
-            if self.sel is not None:
-                ds = ds.sel(self.sel)
-
-            for c in [self.states_coord, self.x_coord, self.y_coord, self.h_coord]:
-                if not c in ds:
-                    raise KeyError(
-                        f"States '{self.name}': Missing coordinate '{c}' in data"
-                    )
-
-            self._inds = ds[self.states_coord].to_numpy()
-            if self.time_format is not None:
-                self._inds = pd.to_datetime(
-                    self._inds, format=self.time_format
-                ).to_numpy()
-            self._N = len(self._inds)
-
-            if self.weight_ncvar is not None:
-                self._weights = ds[self.weight_ncvar].to_numpy()
-            else:
-                self._weights = np.full(
-                    (self._N, algo.n_turbines), 1.0 / self._N, dtype=FC.DTYPE
-                )
-
-            for v in self.ovars:
-                if v in self.var2ncvar:
-                    ncv = self.var2ncvar[v]
-                    if not ncv in ds:
-                        raise KeyError(
-                            f"States '{self.name}': nc variable '{ncv}' not found in data, found: {sorted(list(ds.keys()))}"
-                        )
-                elif v not in self.fixed_vars:
-                    raise ValueError(
-                        f"States '{self.name}': Variable '{v}' neither found in var2ncvar not in fixed_vars"
-                    )  
-
-            if self.pre_load:
-
-                self.X = self.var(FV.X)
-                self.Y = self.var(FV.Y)
-                self.H = self.var(FV.H)
-                self.VARS = self.var("vars")
-                self.DATA = self.var("data")
-
-                h = ds[self.h_coord].to_numpy()
-                y = ds[self.y_coord].to_numpy()
-                x = ds[self.x_coord].to_numpy()
-                v = list(self._dkys.keys())
-
-                coos = (FV.STATE, self.H, self.Y, self.X, self.VARS)
-                data = self._get_data(ds, verbosity)
-                data = (coos, data)
-
-                return h, y, x, v, data
-
-        if isinstance(self.data_source, xr.Dataset):
-            return extract_data(self.data_source)
-        else:
-            with xr.open_mfdataset(
-                pattern,
-                parallel=True,
-                concat_dim=self.states_coord,
-                combine="nested",
-                data_vars="minimal",
-                coords="minimal",
-                compat="override",
-            ) as ds:
-                out = extract_data(ds)
-            return out
-
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
@@ -283,14 +277,15 @@
         -------
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
+        
         if (FV.WS in self.ovars and FV.WD not in self.ovars) or (
             FV.WS not in self.ovars and FV.WD in self.ovars
         ):
             raise KeyError(
                 f"States '{self.name}': Missing '{FV.WS}' or '{FV.WD}' in output variables {self.ovars}"
             )
 
@@ -300,39 +295,40 @@
             self._dkys[FV.WD] = 0
         if FV.WS in self.var2ncvar:
             self._dkys[FV.WS] = 1
         for v in self.var2ncvar:
             if v not in self._dkys:
                 self._dkys[v] = len(self._dkys)
         self._n_dvars = len(self._dkys)
-        self._weights = None
 
-        if isinstance(self.data_source, xr.Dataset):
-            r = self._read_nc(algo, None, verbosity)
-        else:
-            if verbosity:
-                print(f"States '{self.name}': Reading files {self.data_source}")
-            try:
-                r = self._read_nc(algo, self.data_source, verbosity)
-            except OSError:
-                if verbosity:
-                    print(
-                        f"States '{self.name}': Reading static data '{self.data_source}' from context '{STATES}'"
-                    )
-                fpath = algo.dbook.get_file_path(STATES, self.data_source, check_raw=False)
-                if verbosity:
-                    print(f"Path: {fpath}")
-                r = self._read_nc(algo, fpath, verbosity)
+        if self._weights is None:
+            self._weights = np.full(
+                (self._N, algo.n_turbines), 1.0 / self._N, dtype=FC.DTYPE
+            )
 
         idata = super().initialize(algo, verbosity)
         self._update_idata(algo, idata)
 
         if self.pre_load:
 
-            h, y, x, v, data = r
+            self.X = self.var(FV.X)
+            self.Y = self.var(FV.Y)
+            self.H = self.var(FV.H)
+            self.VARS = self.var("vars")
+            self.DATA = self.var("data")
+
+            ds = self.data_source
+
+            h = ds[self.h_coord].to_numpy()
+            y = ds[self.y_coord].to_numpy()
+            x = ds[self.x_coord].to_numpy()
+            v = list(self._dkys.keys())
+            coos = (FV.STATE, self.H, self.Y, self.X, self.VARS)
+            data = self._get_data(ds, verbosity)
+            data = (coos, data)
 
             idata["coords"][self.H] = h
             idata["coords"][self.Y] = y
             idata["coords"][self.X] = x
             idata["coords"][self.VARS] = v
             idata["data_vars"][self.DATA] = data
         
@@ -433,32 +429,21 @@
             h = mdata[self.H]
             data = mdata[self.DATA].copy()
 
         # read data for this chunk:
         else:
             i0 = np.where(self._inds == mdata[FV.STATE][0])[0][0]
             s = slice(i0, i0 + n_states)
-            ds = (
-                xr.open_mfdataset(
-                    self.data_source,
-                    parallel=False,
-                    concat_dim=self.states_coord,
-                    combine="nested",
-                    data_vars="minimal",
-                    coords="minimal",
-                    compat="override",
-                )
-                .isel({self.states_coord: s})
-                .load()
-            )
+            ds = self.data_source.isel({self.states_coord: s}).load()
 
             x = ds[self.x_coord].to_numpy()
             y = ds[self.y_coord].to_numpy()
             h = ds[self.h_coord].to_numpy()
             data = self._get_data(ds, verbosity=0)
+
             del ds
 
         # translate WS, WD into U, V:
         if FV.WD in self.ovars and FV.WS in self.ovars:
             wd = data[..., self._dkys[FV.WD]]
             ws = (
                 data[..., self._dkys[FV.WS]]
```

### Comparing `foxes-0.3.3/foxes/input/states/multi_height.py` & `foxes-0.3.4/foxes/input/states/multi_height.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/states/scan_ws.py` & `foxes-0.3.4/foxes/input/states/scan_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/states/single.py` & `foxes-0.3.4/foxes/input/states/single.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/input/states/states_table.py` & `foxes-0.3.4/foxes/input/states/states_table.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/farm_models/turbine2farm.py` & `foxes-0.3.4/foxes/models/farm_models/turbine2farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/model_book.py` & `foxes-0.3.4/foxes/models/model_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/partial_wakes/axiwake.py` & `foxes-0.3.4/foxes/models/partial_wakes/axiwake.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/partial_wakes/distsliced.py` & `foxes-0.3.4/foxes/models/partial_wakes/distsliced.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/partial_wakes/grid.py` & `foxes-0.3.4/foxes/models/partial_wakes/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/partial_wakes/mapped.py` & `foxes-0.3.4/foxes/models/partial_wakes/mapped.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.3.4/foxes/models/partial_wakes/rotor_points.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/partial_wakes/top_hat.py` & `foxes-0.3.4/foxes/models/partial_wakes/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/point_models/set_uniform_data.py` & `foxes-0.3.4/foxes/models/point_models/set_uniform_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/point_models/tke2ti.py` & `foxes-0.3.4/foxes/models/point_models/tke2ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/point_models/wake_deltas.py` & `foxes-0.3.4/foxes/models/point_models/wake_deltas.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/rotor_models/centre.py` & `foxes-0.3.4/foxes/models/rotor_models/centre.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/rotor_models/grid.py` & `foxes-0.3.4/foxes/models/rotor_models/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/calculator.py` & `foxes-0.3.4/foxes/models/turbine_models/calculator.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/kTI_model.py` & `foxes-0.3.4/foxes/models/turbine_models/kTI_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/power_mask.py` & `foxes-0.3.4/foxes/models/turbine_models/power_mask.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/sector_management.py` & `foxes-0.3.4/foxes/models/turbine_models/sector_management.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/set_XYHD.py` & `foxes-0.3.4/foxes/models/turbine_models/set_XYHD.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.3.4/foxes/models/turbine_models/set_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/table_factors.py` & `foxes-0.3.4/foxes/models/turbine_models/table_factors.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.3.4/foxes/models/turbine_models/thrust2ct.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/yaw2yawm.py` & `foxes-0.3.4/foxes/models/turbine_models/yaw2yawm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_models/yawm2yaw.py` & `foxes-0.3.4/foxes/models/turbine_models/yawm2yaw.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_types/PCt_file.py` & `foxes-0.3.4/foxes/models/turbine_types/PCt_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import pandas as pd
 from pathlib import Path
 
 from foxes.core import TurbineType
 from foxes.utils import PandasFileHelper
 from foxes.data import PCTCURVE, parse_Pct_file_name
 import foxes.variables as FV
-
+import foxes.constants as FC
 
 class PCtFile(TurbineType):
     """
     Calculate power and ct by interpolating
-    from power-ct-curve data file.
+    from power-ct-curve data file (or pandas DataFrame).
 
     Parameters
     ----------
     data_source : str or pandas.DataFrame
         The file path, static name, or data
     col_ws : str
         The wind speed column
@@ -151,14 +151,19 @@
             data = PandasFileHelper.read_file(fpath, **self.rpars)
 
         data = data.set_index(self.col_ws).sort_index()
         self.data_ws = data.index.to_numpy()
         self.data_P = data[self.col_P].to_numpy()
         self.data_ct = data[self.col_ct].to_numpy()
 
+        if self.P_nominal is None:
+            self.P_nominal = np.max(self.data_P) / FC.P_UNITS[self.P_unit]
+            if verbosity > 0:
+                print(f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}")
+
         return super().initialize(algo, verbosity)
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
```

### Comparing `foxes-0.3.3/foxes/models/turbine_types/PCt_two_files.py` & `foxes-0.3.4/foxes/models/turbine_types/PCt_from_two.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pandas as pd
 
 from foxes.core import TurbineType
 from foxes.utils import PandasFileHelper
 from foxes.data import PCTCURVE, parse_Pct_two_files
 import foxes.variables as FV
+import foxes.constants as FC
 
-
-class PCtTwoFiles(TurbineType):
+class PCtFromTwo(TurbineType):
     """
     Calculate power and ct by interpolating
     from power curve and ct curve data files.
 
     Parameters
     ----------
     data_source_P : str or pandas.DataFrame
@@ -179,14 +179,19 @@
             )
             self._data_ct = PandasFileHelper.read_file(fpath, **self.rpars_ct)
 
         self._data_ct = self._data_ct.set_index(self.col_ws_ct_file).sort_index()
         self._data_ws_ct = self._data_ct.index.to_numpy()
         self._data_ct = self._data_ct[self.col_ct].to_numpy()
 
+        if self.P_nominal is None:
+            self.P_nominal = np.max(self._data_P) / FC.P_UNITS[self.P_unit]
+            if verbosity > 0:
+                print(f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}")
+
         return super().initialize(algo, verbosity)
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
```

### Comparing `foxes-0.3.3/foxes/models/turbine_types/null_type.py` & `foxes-0.3.4/foxes/models/turbine_types/null_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/turbine_types/wsrho2PCt_two_files.py` & `foxes-0.3.4/foxes/models/turbine_types/wsrho2PCt_two_files.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py` & `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py` & `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py` & `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/vertical_profiles/abl_log/abl_log_ws.py` & `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/vertical_profiles/abl_log/sheared_ws.py` & `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/sheared_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_frames/farm_order.py` & `foxes-0.3.4/foxes/models/wake_frames/farm_order.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.3.4/foxes/models/wake_frames/rotor_wd.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_frames/streamlines.py` & `foxes-0.3.4/foxes/models/wake_frames/streamlines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_frames/yawed_wakes.py` & `foxes-0.3.4/foxes/models/wake_frames/yawed_wakes.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/axisymmetric.py` & `foxes-0.3.4/foxes/models/wake_models/axisymmetric.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/dist_sliced.py` & `foxes-0.3.4/foxes/models/wake_models/dist_sliced.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/gaussian.py` & `foxes-0.3.4/foxes/models/wake_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/ti/crespo_hernandez.py` & `foxes-0.3.4/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.3.4/foxes/models/wake_models/ti/iec_ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/top_hat.py` & `foxes-0.3.4/foxes/models/wake_models/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/wind/bastankhah.py` & `foxes-0.3.4/foxes/models/wake_models/wind/bastankhah.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/wind/jensen.py` & `foxes-0.3.4/foxes/models/wake_models/wind/jensen.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/wind/porte_agel.py` & `foxes-0.3.4/foxes/models/wake_models/wind/porte_agel.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.3.4/foxes/models/wake_models/wind/turbopark.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_superpositions/linear.py` & `foxes-0.3.4/foxes/models/wake_superpositions/linear.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_superpositions/max.py` & `foxes-0.3.4/foxes/models/wake_superpositions/max.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_superpositions/quadratic.py` & `foxes-0.3.4/foxes/models/wake_superpositions/quadratic.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/models/wake_superpositions/ti_superp.py` & `foxes-0.3.4/foxes/models/wake_superpositions/ti_superp.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/constraints/area_geometry.py` & `foxes-0.3.4/foxes/opt/constraints/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/constraints/min_dist.py` & `foxes-0.3.4/foxes/opt/constraints/min_dist.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/core/farm_constraint.py` & `foxes-0.3.4/foxes/opt/core/farm_constraint.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/core/farm_objective.py` & `foxes-0.3.4/foxes/opt/core/farm_objective.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/core/farm_opt_problem.py` & `foxes-0.3.4/foxes/opt/core/farm_opt_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/core/farm_vars_problem.py` & `foxes-0.3.4/foxes/opt/core/farm_vars_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/core/pop_states.py` & `foxes-0.3.4/foxes/opt/core/pop_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/objectives/farm_vars.py` & `foxes-0.3.4/foxes/opt/objectives/farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/objectives/max_n_turbines.py` & `foxes-0.3.4/foxes/opt/objectives/max_n_turbines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/farm_layout.py` & `foxes-0.3.4/foxes/opt/problems/layout/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/constraints.py` & `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/constraints.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/geom_layouts/objectives.py` & `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/objectives.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.3.4/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.3.4/foxes/opt/problems/layout/regular_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.3.4/foxes/opt/problems/opt_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/output/farm_layout.py` & `foxes-0.3.4/foxes/output/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/output/farm_results_eval.py` & `foxes-0.3.4/foxes/output/farm_results_eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -355,50 +355,64 @@
         """
         v = FV.P if not ambient else FV.AMB_P
         cdata = self.reduce_all(states_op={v: "mean"}, turbines_op={v: "sum"})
         return cdata[v]
 
     def calc_turbine_yield(
         self,
+        algo=None,
         annual=False,
         ambient=False,
         hours=None,
         delta_t=None,
-        P_unit_W=1e3,
+        P_unit_W=None,
     ):
         """
         Calculates the yield per turbine
 
         Parameters
         ----------
+        algo : foxes.core.Algorithm, optional
+            The algorithm, for P_nominal lookup
         annual : bool, optional
             Flag for returing annual results, by default False
         ambient : bool, optional
             Flag for ambient power, by default False
         hours : int, optional
             The duration time in hours, if not timeseries states
         delta_t : np.datetime64, optional
             The time delta step in case of time series data,
             by default automatically determined
         P_unit_W : float
-            The power unit in Watts, 1000 for kW
+            The power unit in Watts, 1000 for kW. Looked up
+            in algorithm if not given
 
         Returns
         -------
         pandas.DataFrame
             A dataframe of yield values by turbine in GWh
 
         """
         if ambient:
             var_in = FV.AMB_P
             var_out = FV.AMB_YLD
         else:
             var_in = FV.P
             var_out = FV.YLD
 
+        if algo is not None and P_unit_W is None:
+            P_unit_W = np.array(
+                [FC.P_UNITS[t.P_unit] for t in algo.farm_controller.turbine_types],
+                dtype=FC.DTYPE,
+            )[:, None]
+        elif algo is None and P_unit_W is not None:
+            pass
+        else:
+            raise KeyError("Expecting either 'algo' or 'P_unit_W'")
+        
         # compute yield per turbine
         if np.issubdtype(self.results[FV.STATE].dtype, np.datetime64):
             if hours is not None:
                 raise KeyError("Unexpected parameter 'hours' for timeseries data")
             times = self.results[FV.STATE].to_numpy()
             if delta_t is None:
                 delta_t = times[-1] - times[-2]
```

### Comparing `foxes-0.3.3/foxes/output/flow_plots_2d.py` & `foxes-0.3.4/foxes/output/flow_plots_2d.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/output/output.py` & `foxes-0.3.4/foxes/output/output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/output/results_writer.py` & `foxes-0.3.4/foxes/output/results_writer.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/output/rose_plot.py` & `foxes-0.3.4/foxes/output/rose_plot.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/output/state_turbine_map.py` & `foxes-0.3.4/foxes/output/state_turbine_map.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/output/turbine_type_curves.py` & `foxes-0.3.4/foxes/output/turbine_type_curves.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/abl/neutral.py` & `foxes-0.3.4/foxes/utils/abl/neutral.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/abl/stable.py` & `foxes-0.3.4/foxes/utils/abl/stable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/abl/unstable.py` & `foxes-0.3.4/foxes/utils/abl/unstable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/cubic_roots.py` & `foxes-0.3.4/foxes/utils/cubic_roots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/data_book.py` & `foxes-0.3.4/foxes/utils/data_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/dict.py` & `foxes-0.3.4/foxes/utils/dict.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/geom2d/area_geometry.py` & `foxes-0.3.4/foxes/utils/geom2d/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/geom2d/circle.py` & `foxes-0.3.4/foxes/utils/geom2d/circle.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/geom2d/example_intersection.py` & `foxes-0.3.4/foxes/utils/geom2d/example_intersection.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/geom2d/example_union.py` & `foxes-0.3.4/foxes/utils/geom2d/example_union.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/geom2d/half_plane.py` & `foxes-0.3.4/foxes/utils/geom2d/half_plane.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/geom2d/polygon.py` & `foxes-0.3.4/foxes/utils/geom2d/polygon.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/geopandas_helpers.py` & `foxes-0.3.4/foxes/utils/geopandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/pandas_helpers.py` & `foxes-0.3.4/foxes/utils/pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/runners.py` & `foxes-0.3.4/foxes/utils/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod, ABCMeta
 from copy import deepcopy
 import dask
-from dask.diagnostics import ProgressBar
 from dask.distributed import Client, LocalCluster
-
+from dask.distributed import get_client
+from dask.diagnostics import ProgressBar
 
 class Runner(metaclass=ABCMeta):
     """
     Abstract base class for runners.
     """
 
     def __init__(self):
@@ -165,32 +165,36 @@
         if scheduler is None and (
             n_workers is not None
             or threads_per_worker is not None
             or cluster_args is not None
         ):
             self.scheduler = "distributed"
 
+    @classmethod
+    def is_distributed(cls):
+        try:
+            get_client()
+            return True
+        except ValueError:
+            return False
+    
     def initialize(self):
         """
         Initialize the runner
         """
         if self.scheduler == "distributed":
 
             self.print("Launching dask cluster..")
 
             self._cluster = LocalCluster(**self.cluster_args)
             self._client = Client(self._cluster, **self.client_args)
 
             self.print(self._cluster)
             self.print(f"Dashboard: {self._client.dashboard_link}\n")
 
-        else:
-            self._config0 = deepcopy(dask.config.config)
-            dask.config.config["scheduler"] = self.scheduler
-
         super().initialize()
 
     def print(self, *args, **kwargs):
         """
         Prints if verbosity is not zero
         """
         if self.verbosity > 0:
@@ -228,12 +232,11 @@
         Finallize the runner
         """
         if self.scheduler == "distributed":
 
             self.print("\n\nShutting down dask cluster")
             self._client.close()
             self._cluster.close()
-
-        else:
-            dask.config.config["scheduler"] = self._config0
+        
+        dask.config.refresh()
 
         super().finalize()
```

### Comparing `foxes-0.3.3/foxes/utils/two_circles.py` & `foxes-0.3.4/foxes/utils/two_circles.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/utils/wind_dir.py` & `foxes-0.3.4/foxes/utils/wind_dir.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes/variables.py` & `foxes-0.3.4/foxes/variables.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.3/foxes.egg-info/PKG-INFO` & `foxes-0.3.4/foxes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.3.3
+Version: 0.3.4
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
 Keywords: Wind farm,Wake modelling,Wind farm optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: scripts
 License-File: LICENSE
 
 # Welcome to foxes
@@ -51,14 +51,15 @@
 
 The supported Python versions are: 
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
+- `Python 3.11`
 
 ## Installation via conda
 
 ### Virtual Python environment
 
 First create a new `conda` environment, for example called `foxes`, by
```

### Comparing `foxes-0.3.3/foxes.egg-info/SOURCES.txt` & `foxes-0.3.4/foxes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,26 +66,29 @@
 foxes/data/states/timeseries_3000.csv.gz
 foxes/data/states/timeseries_8000.csv.gz
 foxes/data/states/wind_rose_bremen.csv
 foxes/data/states/wind_rotation.nc
 foxes/input/__init__.py
 foxes/input/farm_layout/__init__.py
 foxes/input/farm_layout/add_from_csv.py
+foxes/input/farm_layout/add_from_df.py
 foxes/input/farm_layout/add_from_file.py
 foxes/input/farm_layout/add_from_json.py
 foxes/input/farm_layout/add_grid.py
 foxes/input/farm_layout/add_row.py
 foxes/input/states/__init__.py
 foxes/input/states/field_data_nc.py
 foxes/input/states/multi_height.py
 foxes/input/states/scan_ws.py
 foxes/input/states/single.py
 foxes/input/states/states_table.py
 foxes/input/states/create/__init__.py
 foxes/input/states/create/random_abl_states.py
+foxes/input/windio/__init__.py
+foxes/input/windio/windio.py
 foxes/models/__init__.py
 foxes/models/model_book.py
 foxes/models/farm_controllers/__init__.py
 foxes/models/farm_controllers/basic.py
 foxes/models/farm_models/__init__.py
 foxes/models/farm_models/turbine2farm.py
 foxes/models/partial_wakes/__init__.py
@@ -109,16 +112,18 @@
 foxes/models/turbine_models/sector_management.py
 foxes/models/turbine_models/set_XYHD.py
 foxes/models/turbine_models/set_farm_vars.py
 foxes/models/turbine_models/table_factors.py
 foxes/models/turbine_models/thrust2ct.py
 foxes/models/turbine_models/yaw2yawm.py
 foxes/models/turbine_models/yawm2yaw.py
+foxes/models/turbine_types/CpCt_file.py
+foxes/models/turbine_types/CpCt_from_two.py
 foxes/models/turbine_types/PCt_file.py
-foxes/models/turbine_types/PCt_two_files.py
+foxes/models/turbine_types/PCt_from_two.py
 foxes/models/turbine_types/__init__.py
 foxes/models/turbine_types/null_type.py
 foxes/models/turbine_types/wsrho2PCt_two_files.py
 foxes/models/vertical_profiles/__init__.py
 foxes/models/vertical_profiles/uniform.py
 foxes/models/vertical_profiles/abl_log/__init__.py
 foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py
```

### Comparing `foxes-0.3.3/setup.cfg` & `foxes-0.3.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 
 [options]
 zip_safe = True
 include_package_data = True
 package_dir = 
 packages = find:
 python_requires = 
-	>=3.7, <3.11
+	>=3.7
 install_requires = 
 	matplotlib
 	numpy
 	xarray
 	dask[distributed]
 	scipy
 	netcdf4
 	plotly
 	kaleido
 	iwopy>=0.1.4
-	pymoo
+	pymoo>=0.6
 
 [options.extras_require]
 test = 
 	flake8
 	pytest
 doc = 
 	sphinx
```

