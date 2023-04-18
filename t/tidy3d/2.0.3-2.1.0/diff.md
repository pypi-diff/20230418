# Comparing `tmp/tidy3d-2.0.3.tar.gz` & `tmp/tidy3d-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.0.3.tar", last modified: Tue Apr 11 13:11:50 2023, max compression
+gzip compressed data, was "tidy3d-2.1.0.tar", last modified: Tue Apr 18 20:46:11 2023, max compression
```

## Comparing `tidy3d-2.0.3.tar` & `tidy3d-2.1.0.tar`

### file list

```diff
@@ -1,189 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.249168 tidy3d-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-11 13:11:30.000000 tidy3d-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-11 13:11:30.000000 tidy3d-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-11 13:11:50.249168 tidy3d-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-11 13:11:30.000000 tidy3d-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-11 13:11:30.000000 tidy3d-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 13:11:30.000000 tidy3d-2.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:11:50.249168 tidy3d-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-11 13:11:30.000000 tidy3d-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.233167 tidy3d-2.0.3/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    22157 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    49798 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_plugins/test_resonance_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.237167 tidy3d-2.0.3/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23162 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    69858 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    27869 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146855 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47455 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)    57298 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   115895 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.245167 tidy3d-2.0.3/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/plugins/smatrix/smatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.249168 tidy3d-2.0.3/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.249168 tidy3d-2.0.3/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21550 2023-04-11 13:11:30.000000 tidy3d-2.0.3/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:11:50.241167 tidy3d-2.0.3/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 13:11:50.000000 tidy3d-2.0.3/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.198248 tidy3d-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-18 20:45:52.000000 tidy3d-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-18 20:45:52.000000 tidy3d-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-18 20:46:11.198248 tidy3d-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-18 20:45:52.000000 tidy3d-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 20:45:52.000000 tidy3d-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.174246 tidy3d-2.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:46:11.198248 tidy3d-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-18 20:45:52.000000 tidy3d-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.174246 tidy3d-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.174246 tidy3d-2.1.0/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22157 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49798 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25771 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.182247 tidy3d-2.1.0/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.182247 tidy3d-2.1.0/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23162 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77646 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27869 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146855 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47455 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57298 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115895 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/dispersion/fit_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.194247 tidy3d-2.1.0/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.194247 tidy3d-2.1.0/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.194247 tidy3d-2.1.0/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.198248 tidy3d-2.1.0/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19165 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.182247 tidy3d-2.1.0/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.0.3/LICENSE` & `tidy3d-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/PKG-INFO` & `tidy3d-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.0.3
+Version: 2.1.0
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,14 +56,22 @@
 ```
 pip install --user tidy3d
 tidy3d configure --apikey=XXX
 ```
 
 Where `XXX` is your API key, which can be copied from your [account page](https://tidy3d.simulation.cloud/account) in the web interface.
 
+In a hosted jupyter notebook environment (eg google colab), it may be more convenient to install and configure via the following lines at the top of the notebook.
+
+```
+!pip install tidy3d
+import tidy3d.web as web
+web.configure("XXX")
+```
+
 If those commands did not work, advanced installation instructions are below, which should help solve the issue.
 
 ### Advanced Installation Instructions
 
 Some users might require more a specialized installation, which we cover below.
 
 #### Using pip (recommended)
```

### Comparing `tidy3d-2.0.3/README.md` & `tidy3d-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,22 @@
 ```
 pip install --user tidy3d
 tidy3d configure --apikey=XXX
 ```
 
 Where `XXX` is your API key, which can be copied from your [account page](https://tidy3d.simulation.cloud/account) in the web interface.
 
+In a hosted jupyter notebook environment (eg google colab), it may be more convenient to install and configure via the following lines at the top of the notebook.
+
+```
+!pip install tidy3d
+import tidy3d.web as web
+web.configure("XXX")
+```
+
 If those commands did not work, advanced installation instructions are below, which should help solve the issue.
 
 ### Advanced Installation Instructions
 
 Some users might require more a specialized installation, which we cover below.
 
 #### Using pip (recommended)
```

### Comparing `tidy3d-2.0.3/setup.py` & `tidy3d-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.1.0/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/_test_local/_test_data_performance.py` & `tidy3d-2.1.0/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/_test_local/_test_fit_web.py` & `tidy3d-2.1.0/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.1.0/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/_test_local/_test_web.py` & `tidy3d-2.1.0/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_IO.py` & `tidy3d-2.1.0/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_apodization.py` & `tidy3d-2.1.0/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_base.py` & `tidy3d-2.1.0/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_boundaries.py` & `tidy3d-2.1.0/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_custom.py` & `tidy3d-2.1.0/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_field_projection.py` & `tidy3d-2.1.0/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_geometry.py` & `tidy3d-2.1.0/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_grid.py` & `tidy3d-2.1.0/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_grid_spec.py` & `tidy3d-2.1.0/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_medium.py` & `tidy3d-2.1.0/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_meshgenerate.py` & `tidy3d-2.1.0/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_mode.py` & `tidy3d-2.1.0/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_monitor.py` & `tidy3d-2.1.0/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_sidewall.py` & `tidy3d-2.1.0/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_simulation.py` & `tidy3d-2.1.0/tests/test_components/test_simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_source.py` & `tidy3d-2.1.0/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_components/test_types.py` & `tidy3d-2.1.0/tests/test_components/test_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,8 +55,8 @@
 def test_hash():
     class MyClass(Tidy3dBaseModel):
 
         a: ArrayLike
         b: constrained_array(ndim=1)
 
     c = MyClass(a=[1.0], b=[2.0, 1.0])
-    hash(c)
+    hash(c.json())
```

### Comparing `tidy3d-2.0.3/tests/test_data/test_data_arrays.py` & `tidy3d-2.1.0/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_data/test_monitor_data.py` & `tidy3d-2.1.0/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_data/test_sim_data.py` & `tidy3d-2.1.0/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_package/test_config.py` & `tidy3d-2.1.0/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_package/test_log.py` & `tidy3d-2.1.0/tests/test_package/test_log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_package/test_make_script.py` & `tidy3d-2.1.0/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_package/test_material_library.py` & `tidy3d-2.1.0/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_package/test_parametric_variants.py` & `tidy3d-2.1.0/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_plugins/test_adjoint.py` & `tidy3d-2.1.0/tests/test_plugins/test_adjoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from tidy3d.plugins.adjoint.components.structure import JaxStructure
 from tidy3d.plugins.adjoint.components.simulation import JaxSimulation
 from tidy3d.plugins.adjoint.components.data.sim_data import JaxSimulationData
 from tidy3d.plugins.adjoint.components.data.monitor_data import JaxModeData, JaxDiffractionData
 from tidy3d.plugins.adjoint.components.data.data_array import JaxDataArray
 from tidy3d.plugins.adjoint.components.data.dataset import JaxPermittivityDataset
 from tidy3d.plugins.adjoint.web import run, run_async
+from tidy3d.plugins.adjoint.components.data.data_array import VALUE_FILTER_THRESHOLD
 
 from ..utils import run_emulated, assert_log_level, log_capture, run_async_emulated
 
 
 EPS = 2.0
 SIZE = (1.0, 2.0, 3.0)
 CENTER = (2.0, -1.0, 1.0)
@@ -769,7 +770,21 @@
     """Test that a custom error is raised if running tidy3d through web.run()"""
 
     sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
     import tidy3d.web as web
 
     with pytest.raises(ValueError):
         web.run(sim, task_name="test")
+
+
+def test_value_filter():
+    """Ensure value filter works as expected."""
+
+    values = np.array([1, 0.5 * VALUE_FILTER_THRESHOLD, 2 * VALUE_FILTER_THRESHOLD, 0])
+    coords = dict(x=list(range(4)))
+    data = JaxDataArray(values=values, coords=coords)
+
+    values_after, _ = data.nonzero_val_coords
+
+    # assert that the terms <= VALUE_FILTER_THRESHOLD should be removed
+    values_expected = np.array([1, 2 * VALUE_FILTER_THRESHOLD])
+    assert np.allclose(np.array(values_after), values_expected)
```

### Comparing `tidy3d-2.0.3/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.1.0/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.1.0/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.1.0/tests/test_plugins/test_mode_solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,30 +40,30 @@
         precision="double",
         track_freq="lowest",
     )
     ms = ModeSolver(
         simulation=simulation,
         plane=PLANE,
         mode_spec=mode_spec,
-        freqs=[td.constants.C_0 / 0.9, td.constants.C_0 / 1.0, td.constants.C_0 / 1.1],
+        freqs=[td.C_0 / 0.9, td.C_0 / 1.0, td.C_0 / 1.1],
     )
     modes = ms.solve()
 
 
 def test_mode_solver_custom_medium():
     """Test mode solver can work with custom medium. Consider a waveguide with varying
     permittivity along x-direction. The value of n_eff at different x position should be
     different.
     """
 
     # waveguide made of custom medium
     x_custom = np.linspace(-0.6, 0.6, 2)
     y_custom = [0]
     z_custom = [0]
-    freq0 = td.constants.C_0 / 1.0
+    freq0 = td.C_0 / 1.0
     n = np.array([1.5, 5])
     n = n[:, None, None, None]
     n_data = ScalarFieldDataArray(n, coords=dict(x=x_custom, y=y_custom, z=z_custom, f=[freq0]))
     mat_custom = td.CustomMedium.from_nk(n_data, interp_method="nearest")
 
     waveguide = td.Structure(geometry=td.Box(size=(100, 0.5, 0.5)), medium=mat_custom)
     simulation = td.Simulation(
@@ -114,17 +114,15 @@
         bend_axis=0,
         angle_theta=np.pi / 3,
         angle_phi=np.pi,
         track_freq="highest",
     )
     # put plane entirely in the symmetry quadrant rather than sitting on its center
     plane = td.Box(center=(0, 0.5, 0), size=(1, 0, 1))
-    ms = ModeSolver(
-        simulation=simulation, plane=plane, mode_spec=mode_spec, freqs=[td.constants.C_0 / 1.0]
-    )
+    ms = ModeSolver(simulation=simulation, plane=plane, mode_spec=mode_spec, freqs=[td.C_0 / 1.0])
     modes = ms.solve()
     # Plot field
     _, ax = plt.subplots(1)
     ms.plot_field("Ex", ax=ax, mode_index=1)
 
     # Create source and monitor
     st = td.GaussianPulse(freq0=1.0, fwidth=1.0)
@@ -145,50 +143,90 @@
         size=(0, SIM_SIZE[1], SIM_SIZE[2]),
         grid_spec=td.GridSpec(wavelength=1.0),
         structures=[WAVEGUIDE],
         run_time=1e-12,
         boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
         sources=[SRC],
     )
-    ms = ModeSolver(
-        simulation=simulation, plane=PLANE, mode_spec=mode_spec, freqs=[td.constants.C_0 / 1.0]
-    )
+    ms = ModeSolver(simulation=simulation, plane=PLANE, mode_spec=mode_spec, freqs=[td.C_0 / 1.0])
     modes = ms.solve()
 
     mode_spec = td.ModeSpec(num_modes=3, filter_pol="te", precision="double", num_pml=(10, 0))
     simulation = td.Simulation(
         size=(SIM_SIZE[0], SIM_SIZE[1], 0),
         grid_spec=td.GridSpec(wavelength=1.0),
         structures=[WAVEGUIDE],
         run_time=1e-12,
         sources=[SRC],
     )
-    ms = ModeSolver(
-        simulation=simulation, plane=PLANE, mode_spec=mode_spec, freqs=[td.constants.C_0 / 1.0]
-    )
+    ms = ModeSolver(simulation=simulation, plane=PLANE, mode_spec=mode_spec, freqs=[td.C_0 / 1.0])
     modes = ms.solve()
 
     # The simulation and the mode plane are both 0D along the same dimension
     simulation = td.Simulation(
         size=PLANE.size,
         grid_spec=td.GridSpec(wavelength=1.0),
         run_time=1e-12,
         boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
         sources=[SRC],
     )
-    ms = ModeSolver(
-        simulation=simulation, plane=PLANE, mode_spec=mode_spec, freqs=[td.constants.C_0 / 1.0]
-    )
+    ms = ModeSolver(simulation=simulation, plane=PLANE, mode_spec=mode_spec, freqs=[td.C_0 / 1.0])
     modes = ms.solve()
 
 
 def test_compute_modes():
     """Test direct call to ``compute_modes`` (used in e.g. gdsfactory)."""
     eps_cross = np.random.rand(10, 10)
     coords = np.arange(11)
     mode_spec = td.ModeSpec(num_modes=3, target_neff=2.0)
     modes = compute_modes(
         eps_cross=[eps_cross] * 3,
         coords=[coords, coords],
-        freq=td.constants.C_0 / 1.0,
+        freq=td.C_0 / 1.0,
+        mode_spec=mode_spec,
+    )
+
+
+def test_group_index():
+    """Test group index calculation"""
+
+    simulation = td.Simulation(
+        size=(5, 5, 1),
+        grid_spec=td.GridSpec(wavelength=1.55),
+        structures=[
+            td.Structure(
+                geometry=td.Box(size=(0.5, 0.22, td.inf)), medium=td.Medium(permittivity=3.48**2)
+            )
+        ],
+        medium=td.Medium(permittivity=1.44**2),
+        run_time=1e-12,
+        boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
+        sources=[SRC],
+    )
+    mode_spec = td.ModeSpec(
+        num_modes=2,
+        target_neff=3.0,
+        precision="double",
+        track_freq="central",
+    )
+
+    # No group index calculation by default
+    ms = ModeSolver(
+        simulation=simulation,
+        plane=td.Box(size=(td.inf, td.inf, 0)),
         mode_spec=mode_spec,
+        freqs=[td.C_0 / 1.54, td.C_0 / 1.55, td.C_0 / 1.56],
     )
+    assert ms.data.n_group is None
+
+    # Group index calculated
+    ms = ModeSolver(
+        simulation=simulation,
+        plane=td.Box(size=(td.inf, td.inf, 0)),
+        mode_spec=mode_spec.copy(update={"group_index_step": True}),
+        freqs=[td.C_0 / 1.54, td.C_0 / 1.55, td.C_0 / 1.56],
+    )
+    modes = ms.solve()
+    assert (modes.n_group.sel(mode_index=0).values > 3.9).all()
+    assert (modes.n_group.sel(mode_index=0).values < 4.2).all()
+    assert (modes.n_group.sel(mode_index=1).values > 3.7).all()
+    assert (modes.n_group.sel(mode_index=1).values < 4.0).all()
```

### Comparing `tidy3d-2.0.3/tests/test_plugins/test_polyslab.py` & `tidy3d-2.1.0/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.1.0/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_web/test_auth.py` & `tidy3d-2.1.0/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_web/test_cli.py` & `tidy3d-2.1.0/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_web/test_material_fitter.py` & `tidy3d-2.1.0/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.1.0/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.1.0/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.1.0/tests/test_web/test_tidy3d_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/test_web/test_webapi.py` & `tidy3d-2.1.0/tests/test_web/test_webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tests/utils.py` & `tidy3d-2.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/__init__.py` & `tidy3d-2.1.0/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/__main__.py` & `tidy3d-2.1.0/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/apodization.py` & `tidy3d-2.1.0/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/base.py` & `tidy3d-2.1.0/tidy3d/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/boundary.py` & `tidy3d-2.1.0/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/data/data_array.py` & `tidy3d-2.1.0/tidy3d/components/data/data_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,30 @@
     >>> td = TimeDataArray((1+1j) * np.random.random((3,)), coords=dict(t=t))
     """
 
     __slots__ = ()
     _dims = "t"
 
 
+class MixedModeDataArray(DataArray):
+    """Scalar property associated with mode pairs
+
+    Example
+    -------
+    >>> f = [1e14, 2e14, 3e14]
+    >>> mode_index_0 = np.arange(4)
+    >>> mode_index_1 = np.arange(2)
+    >>> coords = dict(f=f, mode_index_0=mode_index_0, mode_index_1=mode_index_1)
+    >>> data = MixedModeDataArray((1+1j) * np.random.random((3, 4, 2)), coords=coords)
+    """
+
+    __slots__ = ()
+    _dims = ("f", "mode_index_0", "mode_index_1")
+
+
 class ScalarFieldDataArray(DataArray):
     """Spatial distribution in the frequency-domain.
 
     Example
     -------
     >>> x = [1,2]
     >>> y = [2,3,4]
```

### Comparing `tidy3d-2.0.3/tidy3d/components/data/dataset.py` & `tidy3d-2.1.0/tidy3d/components/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,20 @@
 
     n_complex: ModeIndexDataArray = pd.Field(
         ...,
         title="Propagation Index",
         description="Complex-valued effective propagation constants associated with the mode.",
     )
 
+    n_group: ModeIndexDataArray = pd.Field(
+        None,
+        title="Group Index",
+        description="Index associated with group velocity of the mode.",
+    )
+
     @property
     def field_components(self) -> Dict[str, DataArray]:
         """Maps the field components to thier associated data."""
         # pylint:disable=no-member
         return {field: getattr(self, field) for field in ["Ex", "Ey", "Ez", "Hx", "Hy", "Hz"]}
 
     @property
```

### Comparing `tidy3d-2.0.3/tidy3d/components/data/monitor_data.py` & `tidy3d-2.1.0/tidy3d/components/data/monitor_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from typing import Union, Tuple, Callable, Dict, List
 import warnings
 
 import xarray as xr
 import numpy as np
 import pydantic as pd
 
-from .data_array import FluxTimeDataArray, FluxDataArray, ModeIndexDataArray, ModeAmpsDataArray
+from .data_array import FluxTimeDataArray, FluxDataArray
+from .data_array import MixedModeDataArray, ModeIndexDataArray, ModeAmpsDataArray
 from .data_array import FieldProjectionAngleDataArray, FieldProjectionCartesianDataArray
 from .data_array import FieldProjectionKSpaceDataArray
 from .data_array import DataArray, DiffractionDataArray
 from .data_array import ScalarFieldDataArray, ScalarFieldTimeDataArray
 from .data_array import FreqDataArray, TimeDataArray, FreqModeDataArray
 from .dataset import Dataset, AbstractFieldDataset, ElectromagneticFieldDataset
 from .dataset import FieldDataset, FieldTimeDataset, ModeSolverDataset, PermittivityDataset
 from ..base import TYPE_TAG_STR, cached_property
-from ..types import Coordinate, Symmetry, ArrayFloat1D, Size, Numpy, TrackFreq
+from ..types import Coordinate, Symmetry, ArrayFloat1D, ArrayFloat2D, Size, Numpy, TrackFreq
 from ..grid.grid import Grid, Coords
 from ..validators import enforce_monitor_fields_present, required_if_symmetry_present
 from ..monitor import MonitorType, FieldMonitor, FieldTimeMonitor, ModeSolverMonitor
 from ..monitor import ModeMonitor, FluxMonitor, FluxTimeMonitor, PermittivityMonitor
 from ..monitor import FieldProjectionAngleMonitor, FieldProjectionCartesianMonitor
 from ..monitor import FieldProjectionKSpaceMonitor, FieldProjectionSurface
 from ..monitor import DiffractionMonitor
@@ -190,71 +191,63 @@
             raise DataError("Data must be 2D to get tangential dimensions.")
         tangential_dims = ["x", "y", "z"]
         tangential_dims.pop(self.monitor.zero_dims[0])
 
         return tangential_dims
 
     @property
-    def _tangential_fields(self) -> Dict[str, DataArray]:
-        """For a 2D monitor data, return a dictionary with only the tangential field components,
-        oriented such that the third component would be the normal axis. This just means that the
-        H field gets an extra minus sign if the normal axis is ``"y"``. Raise if any of the
-        tangential field components is missing.
-
-        Note
-        ----
-            The finite grid correction factors are applied and symmetry is expanded.
-        """
-
-        tan_dims = self._tangential_dims
-        normal_dim = "xyz"[self.monitor.size.index(0)]
-        field_components = ["E" + dim for dim in tan_dims] + ["H" + dim for dim in tan_dims]
-        fields_expanded = self.symmetry_expanded_copy.field_components
-        tan_fields = {}
-        for field in field_components:
-            if field not in self.field_components:
-                raise DataError(f"Tangential field component {field} is missing in data.")
-            tan_fields[field] = fields_expanded[field]
-            if field[0] == "E":
-                tan_fields[field] *= self.grid_primal_correction
-            elif field[0] == "H":
-                tan_fields[field] *= self.grid_dual_correction
-                if normal_dim == "y":
-                    tan_fields[field] *= -1
-            tan_fields[field] = tan_fields[field].squeeze(dim=normal_dim, drop=True)
-        return tan_fields
+    def _grid_corrected_fields(self) -> Dict[str, DataArray]:
+        """Dictionary of field components with finite grid correction factors applied and symmetry
+        expanded."""
+        if len(self.monitor.zero_dims) != 1:
+            raise DataError("Data must be 2D to apply grid corrections.")
+        normal_dim = "xyz"[self.monitor.zero_dims[0]]
+        fields = {}
+        for field_name, field in self.symmetry_expanded_copy.field_components.items():
+            eig_val = self.symmetry_eigenvalues[field_name](normal_dim)
+            if eig_val < 0:
+                fields[field_name] = field * self.grid_dual_correction
+            else:
+                fields[field_name] = field * self.grid_primal_correction
+            fields[field_name] = fields[field_name].squeeze(dim=normal_dim, drop=True)
+        return fields
 
     @property
     def _plane_grid_boundaries(self) -> Tuple[Coords1D, Coords1D]:
         """For a 2D monitor data, return the boundaries of the in-plane grid to be used to compute
         differential area and to colocate fields to grid centers if needed."""
         if np.any(np.array(self.monitor.interval_space) > 1):
             raise Tidy3dNotImplementedError(
                 "Cannot determine grid boundaries corresponding to "
                 "down-sampled monitor data ('interval_space' > 1 along a direction)."
             )
         dim1, dim2 = self._tangential_dims
-        tan_fields = self._tangential_fields
 
         # In-plane grid bounds inferred from the field data
         if self.monitor.colocate:
             # Should be equivalent to sim.discretize(self.monitor, extend=True)
             # Take ``unique`` to handle 0D cases along a given dimension
             plane_bounds1 = np.unique(self.grid_expanded.boundaries.to_dict[dim1])
             plane_bounds2 = np.unique(self.grid_expanded.boundaries.to_dict[dim2])
         else:
             # Last pixel missing compared to sim.discretize(self.monitor, extend=True).
             # This is because we cannot colocate the fields to the center of that pixel.
             # However, the monitor should be completely outside of this last pixel.
-            plane_bounds1 = tan_fields["E" + dim2].coords[dim1].values
-            plane_bounds2 = tan_fields["E" + dim1].coords[dim2].values
+            fields = self.symmetry_expanded_copy.field_components
+            plane_bounds1 = fields["E" + dim2].coords[dim1].values
+            plane_bounds2 = fields["E" + dim1].coords[dim2].values
 
         return plane_bounds1, plane_bounds2
 
     @property
+    def _plane_grid_centers(self) -> Tuple[Coords1D, Coords1D]:
+        """For 2D monitor data, return the centers of the in-plane grid"""
+        return [(bs[1:] + bs[:-1]) / 2 for bs in self._plane_grid_boundaries]
+
+    @property
     def _diff_area(self) -> xr.DataArray:
         """For a 2D monitor data, return the area of each cell in the plane, for use in numerical
         integrations."""
         bounds = [bs.copy() for bs in self._plane_grid_boundaries]
 
         # Fix the grid boundaries to match the analytic monitor boundaries.
         _, plane_inds = self.monitor.pop_axis([0, 1, 2], self.monitor.size.index(0.0))
@@ -274,41 +267,97 @@
         bounds[1][np.argwhere(bounds[1] < mnt_bounds[1, 0])] = mnt_bounds[1, 0]
         bounds[1][np.argwhere(bounds[1] > mnt_bounds[1, 1])] = mnt_bounds[1, 1]
 
         sizes_dim0 = bounds[0][1:] - bounds[0][:-1] if bounds[0].size > 1 else [1.0]
         sizes_dim1 = bounds[1][1:] - bounds[1][:-1] if bounds[1].size > 1 else [1.0]
         return xr.DataArray(np.outer(sizes_dim0, sizes_dim1), dims=self._tangential_dims)
 
+    def _tangential_corrected(self, fields: Dict[str, DataArray]) -> Dict[str, DataArray]:
+        """For a 2D monitor data, extract the tangential components from fields and orient them
+        such that the third component would be the normal axis. This just means that the H field
+        gets an extra minus sign if the normal axis is ``"y"``. Raise if any of the tangential
+        field components is missing.
+        """
+        # Tangential field components
+        tan_dims = self._tangential_dims
+        components = [fname + dim for fname in "EH" for dim in tan_dims]
+
+        normal_dim = "xyz"[self.monitor.size.index(0)]
+
+        tan_fields = {}
+        for component in components:
+            if component not in fields:
+                raise DataError(f"Tangential field component '{component}' missing in field data.")
+
+            if normal_dim == "y" and component[0] == "H":
+                tan_fields[component] = -fields[component]
+            else:
+                tan_fields[component] = fields[component]
+
+        return tan_fields
+
     @property
-    def _centered_tangential_fields(self) -> Dict[str, DataArray]:
-        """For a 2D monitor data, get the tangential E and H fields colocated to the cell centers in
-        the 2D plane grid."""
+    def _tangential_fields(self) -> Dict[str, DataArray]:
+        """For a 2D monitor data, get the tangential E and H fields in the 2D plane grid.  Fields
+        are oriented such that the third component would be the normal axis. This just means that
+        the H field gets an extra minus sign if the normal axis is ``"y"``.
 
-        # Tangential directions and fields
-        tan_dims = self._tangential_dims
-        tan_fields = self._tangential_fields
+        Note
+        ----
+            The finite grid correction factors are applied and symmetry is expanded.
+        """
+        return self._tangential_corrected(self._grid_corrected_fields)
 
-        if self.monitor.colocate:
-            # Already colocated
-            return tan_fields
+    @property
+    def _centered_fields(self) -> Dict[str, DataArray]:
+        """For a 2D monitor data, get all E and H fields colocated to the cell centers in the 2D
+        plane grid.
+
+        Note
+        ----
+            The finite grid correction factors are applied and symmetry is expanded.
+        """
 
-        # Colocate to plane center coordinates
-        bounds = self._plane_grid_boundaries
-        centers = [(bs[1:] + bs[:-1]) / 2 for bs in bounds]
+        field_components = self._grid_corrected_fields
+        if self.monitor.colocate:
+            return field_components
 
-        # Interpolate tangential field components to cell centers
+        # Interpolate field components to cell centers
         interp_dict = {}
-        for dim, cents in zip(tan_dims, centers):
+        for dim, cents in zip(self._tangential_dims, self._plane_grid_centers):
             if cents.size > 0:
                 interp_dict[dim] = cents
-        centered_fields = {key: val.interp(**interp_dict) for key, val in tan_fields.items()}
+
+        centered_fields = {key: val.interp(**interp_dict) for key, val in field_components.items()}
 
         return centered_fields
 
     @property
+    def _centered_tangential_fields(self) -> Dict[str, DataArray]:
+        """For a 2D monitor data, get the tangential E and H fields colocated to the cell centers in
+        the 2D plane grid.  Fields are oriented such that the third component would be the normal
+        axis. This just means that the H field gets an extra minus sign if the normal axis is
+        ``"y"``. Raise if any of the tangential field components is missing.
+
+        Note
+        ----
+            The finite grid correction factors are applied and symmetry is expanded.
+        """
+        return self._tangential_corrected(self._centered_fields)
+
+    @property
+    def intensity(self) -> ScalarFieldDataArray:
+        """Return the sum of the squared absolute electric field components."""
+        fields = self._centered_fields
+        components = ("Ex", "Ey", "Ez")
+        if any(cmp not in fields for cmp in components):
+            raise KeyError("Can't compute intensity, all E field components must be present.")
+        return sum(fields[cmp].abs ** 2 for cmp in components)
+
+    @property
     def poynting(self) -> ScalarFieldDataArray:
         """Time-averaged Poynting vector for frequency-domain data associated to a 2D monitor,
         projected to the direction normal to the monitor plane."""
 
         # Tangential fields are ordered as E1, E2, H1, H2
         tan_fields = self._centered_tangential_fields
         dim1, dim2 = self._tangential_dims
@@ -321,14 +370,28 @@
     def flux(self) -> FluxDataArray:
         """Flux for data corresponding to a 2D monitor."""
 
         # Compute flux by integrating Poynting vector in-plane
         d_area = self._diff_area
         return FluxDataArray((self.poynting * d_area).sum(dim=d_area.dims))
 
+    @cached_property
+    def mode_area(self) -> FreqModeDataArray:
+        """Effective mode area corresponding to a 2D monitor.
+
+        Effective mode area is calculated as: (∫|E|²dA)² / (∫|E|⁴dA)
+        """
+        intensity = self.intensity
+        # integrate over the plane
+        d_area = self._diff_area
+        num = (intensity * d_area).sum(dim=d_area.dims) ** 2
+        den = (intensity**2 * d_area).sum(dim=d_area.dims)
+
+        return FreqModeDataArray(num / den)
+
     def dot(
         self, field_data: Union[FieldData, ModeSolverData], conjugate: bool = True
     ) -> ModeAmpsDataArray:
         """Dot product (modal overlap) with another :class:`.FieldData` object. Both datasets have
         to be frequency-domain data associated with a 2D monitor. Along the tangential directions,
         the datasets have to have the same discretization. Along the normal direction, the monitor
         position may differ and is ignored. Other coordinates (``frequency``, ``mode_index``) have
@@ -375,14 +438,127 @@
         h_self_x_e_other -= fields_self["H" + dim2] * fields_other["E" + dim1]
 
         # Integrate over plane
         d_area = self._diff_area
         integrand = (e_self_x_h_other - h_self_x_e_other) * d_area
         return ModeAmpsDataArray(0.25 * integrand.sum(dim=d_area.dims))
 
+    def _interpolated_tangential_fields(self, centers: ArrayFloat2D) -> Dict[str, DataArray]:
+        """For 2D monitors, interpolate this fields to given centers in the tangential plane.
+
+        Parameters
+        ----------
+        centers : ArrayFloat2D
+            Interpolation centers in the monitor's tangential plane.
+
+        Return
+        ------
+            Dictionary with interpolated fields.
+        """
+        fields = self._tangential_fields
+
+        interp_dict = {}
+        for dim, cents in zip(self._tangential_dims, centers):
+            if cents.size > 0:
+                interp_dict[dim] = cents
+
+        kwargs = {"bounds_error": False, "fill_value": 0.0}
+        for component, field in fields.items():
+            fields[component] = field.interp(kwargs=kwargs, **interp_dict)
+
+        return fields
+
+    # pylint: disable=too-many-locals
+    def outer_dot(
+        self, field_data: Union[FieldData, ModeSolverData], conjugate: bool = True
+    ) -> MixedModeDataArray:
+        """Dot product (modal overlap) with another :class:`.FieldData` object.
+
+        The tangential fields from ``field_data`` are interpolated to this object's grid, so the
+        data arrays don't need to have the same discretization.  The calculation is performed for
+        all common frequencies between data arrays.  In the output, ``mode_index_0`` and
+        ``mode_index_1`` are the mode indices from this object and ``field_data``, respectively.
+
+        Parameters
+        ----------
+        field_data : :class:`ElectromagneticFieldData`
+            A data instance to compute the dot product with.
+        conjugate : bool = True
+            If ``True`` (default), the dot product is defined as ``1 / 4`` times the integral of
+            ``E_self* x H_other - H_self* x E_other``, where ``x`` is the cross product and ``*`` is
+            complex conjugation. If ``False``, the complex conjugation is skipped.
+
+        Returns
+        -------
+        :class:`.MixedModeDataArray`
+            Dataset with the complex-valued modal overlaps between the two mode data.
+
+        See also
+        --------
+        :member:`dot`
+        """
+
+        tan_dims = self._tangential_dims
+
+        # pylint: disable=protected-access
+        if not all(a == b for a, b in zip(tan_dims, field_data._tangential_dims)):
+            raise DataError("Tangential dimentions must match between the two monitors.")
+
+        # Tangential fields for current
+        fields_self = self._centered_tangential_fields
+        if conjugate:
+            fields_self = {component: field.conj() for component, field in fields_self.items()}
+
+        # Tangential fields for other data
+        # pylint:disable=protected-access
+        fields_other = field_data._interpolated_tangential_fields(self._plane_grid_centers)
+
+        # Tangential field component names
+        dim1, dim2 = tan_dims
+        e_1 = "E" + dim1
+        e_2 = "E" + dim2
+        h_1 = "H" + dim1
+        h_2 = "H" + dim2
+
+        # Prepare array with proper dimensions for the dot product data
+        arrays = (fields_self[e_1], fields_other[e_1])
+        coords = (arrays[0].coords, arrays[1].coords)
+        # Common frequencies to both data arrays
+        f = np.array(sorted(set(coords[0]["f"].values).intersection(coords[1]["f"].values)))
+        mode_index_0 = coords[0]["mode_index"].values
+        mode_index_1 = coords[1]["mode_index"].values
+        dtype = np.promote_types(arrays[0].dtype, arrays[1].dtype)
+        dot = np.empty((f.size, mode_index_0.size, mode_index_1.size), dtype=dtype)
+
+        # Calculate overlap for each common frequency and each mode pair
+        for i, freq in enumerate(f):
+            for mi0 in mode_index_0:
+                e_self_1 = fields_self[e_1].sel(f=freq, mode_index=mi0, drop=True)
+                e_self_2 = fields_self[e_2].sel(f=freq, mode_index=mi0, drop=True)
+                h_self_1 = fields_self[h_1].sel(f=freq, mode_index=mi0, drop=True)
+                h_self_2 = fields_self[h_2].sel(f=freq, mode_index=mi0, drop=True)
+
+                for mi1 in mode_index_1:
+                    e_other_1 = fields_other[e_1].sel(f=freq, mode_index=mi1, drop=True)
+                    e_other_2 = fields_other[e_2].sel(f=freq, mode_index=mi1, drop=True)
+                    h_other_1 = fields_other[h_1].sel(f=freq, mode_index=mi1, drop=True)
+                    h_other_2 = fields_other[h_2].sel(f=freq, mode_index=mi1, drop=True)
+
+                    # Cross products of fields
+                    e_self_x_h_other = e_self_1 * h_other_2 - e_self_2 * h_other_1
+                    h_self_x_e_other = h_self_1 * e_other_2 - h_self_2 * e_other_1
+
+                    # Integrate over plane
+                    d_area = self._diff_area
+                    integrand = (e_self_x_h_other - h_self_x_e_other) * d_area
+                    dot[i, mi0, mi1] = 0.25 * integrand.sum(dim=d_area.dims)
+
+        coords = {"f": f, "mode_index_0": mode_index_0, "mode_index_1": mode_index_1}
+        return MixedModeDataArray(dot, coords=coords)
+
     @property
     def time_reversed_copy(self) -> FieldData:
         """Make a copy of the data with time-reversed fields."""
 
         # Time reversal for frequency-domain fields; overwritten in :class:`FieldTimeData`.
         new_data = {}
         for comp, field in self.field_components.items():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tidy3d-2.0.3/tidy3d/components/data/sim_data.py` & `tidy3d-2.1.0/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/field_projection.py` & `tidy3d-2.1.0/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/geometry.py` & `tidy3d-2.1.0/tidy3d/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/grid/grid.py` & `tidy3d-2.1.0/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.1.0/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/grid/mesher.py` & `tidy3d-2.1.0/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/medium.py` & `tidy3d-2.1.0/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/mode.py` & `tidy3d-2.1.0/tidy3d/components/mode.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 import pydantic as pd
 import numpy as np
 
 from ..constants import MICROMETER, RADIAN, GLANCING_CUTOFF
 from .base import Tidy3dBaseModel
 from .types import Axis2D, Literal, TrackFreq
-from ..exceptions import SetupError
+from ..log import log
+from ..exceptions import SetupError, ValidationError
+
+
+GROUP_INDEX_STEP = 0.005
 
 
 class ModeSpec(Tidy3dBaseModel):
     """Stores specifications for the mode solver to find an electromagntic mode.
     Note, the planar axes are found by popping the injection axis from {x,y,z}.
     For example, if injection axis is y, the planar axes are ordered {x,z}.
 
@@ -96,14 +100,23 @@
         title="Mode Tracking Frequency",
         description="Parameter that turns on/off mode tracking based on their similarity. "
         "Can take values ``'lowest'``, ``'central'``, or ``'highest'``, which correspond to "
         "mode tracking based on the lowest, central, or highest frequency. "
         "If ``None`` no mode tracking is performed.",
     )
 
+    group_index_step: Union[bool, pd.PositiveFloat] = pd.Field(
+        False,
+        title="Frequency step for group index computation",
+        description="Control the computation of the group index alongside the effective index. If "
+        "set to a positive value, it sets the fractional frequency step used in the numerical "
+        "differentiation of the effective index to compute the group index. If set to `True`, the "
+        f"default of {GROUP_INDEX_STEP} is used.",
+    )
+
     @pd.validator("bend_axis", always=True)
     def bend_axis_given(cls, val, values):
         """check that ``bend_axis`` is provided if ``bend_radius`` is not ``None``"""
         if val is None and values.get("bend_radius") is not None:
             raise SetupError("bend_axis must also be defined if bend_radius is defined.")
         return val
 
@@ -112,7 +125,32 @@
         """Warn if close to glancing incidence."""
         if np.abs(np.pi / 2 - val) < GLANCING_CUTOFF:
             raise SetupError(
                 "Mode propagation axis too close to glancing angle for accurate injection. "
                 "For best results, switch the injection axis."
             )
         return val
+
+    @pd.validator("group_index_step")
+    def assign_default_on_true(cls, val):
+        """Assing the default fractional frequency step value if not provided."""
+        if val is True:
+            return GROUP_INDEX_STEP
+        if val >= 1:
+            raise ValidationError("Parameter 'group_index_step' must be less than 1.")
+        return val
+
+    @pd.root_validator()
+    def check_precision(cls, values):
+        """Verify critical ModeSpec settings for group index calculation."""
+        if values["group_index_step"] > 0:
+            if values["track_freq"] is None:
+                log.warning(
+                    "Group index calculation without mode tracking can lead to incorrect results "
+                    "around mode crossings. Consider setting 'track_freq' to 'central'."
+                )
+            if values["precision"] != "double":
+                log.warning(
+                    "Group index calculation should be performed with double precision for better "
+                    "accuracy. Consider setting 'precision' to 'double'."
+                )
+        return values
```

### Comparing `tidy3d-2.0.3/tidy3d/components/monitor.py` & `tidy3d-2.1.0/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/simulation.py` & `tidy3d-2.1.0/tidy3d/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/source.py` & `tidy3d-2.1.0/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/structure.py` & `tidy3d-2.1.0/tidy3d/components/structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .validators import validate_name_str
 from .geometry import GeometryType
 from .medium import MediumType, CustomMedium, Medium2D
 from .types import Ax, TYPE_TAG_STR
 from .viz import add_ax_if_none, equal_aspect
 from .grid.grid import Coords
 from ..constants import MICROMETER
+from ..exceptions import SetupError
 
 
 class AbstractStructure(Tidy3dBaseModel):
     """
     A basic structure object.
     """
 
@@ -94,17 +95,21 @@
         if isinstance(self.medium, CustomMedium):
             return self.medium.eps_diagonal_on_grid(frequency=frequency, coords=coords)
         return self.medium.eps_diagonal(frequency=frequency)
 
     @pydantic.validator("medium", always=True)
     def _check_2d_geometry(cls, val, values):
         """Medium2D is only consistent with certain geometry types"""
-        geom = values["geometry"]
         if isinstance(val, Medium2D):
             # validate that the geometry is actually 2d
+            geom = values.get("geometry")
+            if not geom:
+                raise SetupError(
+                    "Can't validate 2D structure because its geometry did not pass validation."
+                )
             _ = geom._normal_2dmaterial  # pylint: disable=protected-access
         return val
 
 
 class MeshOverrideStructure(AbstractStructure):
     """Defines an object that is only used in the process of generating the mesh.
     A :class:`MeshOverrideStructure` is a combination of geometry :class:`Geometry`,
```

### Comparing `tidy3d-2.0.3/tidy3d/components/types.py` & `tidy3d-2.1.0/tidy3d/components/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,23 +30,14 @@
 def _totuple(arr: np.ndarray) -> tuple:
     """Convert a numpy array to a nested tuple."""
     if arr.ndim > 1:
         return tuple(_totuple(val) for val in arr)
     return tuple(arr)
 
 
-class TidyNDArray(np.ndarray):
-    """subclass of np.ndarray with a hash."""
-
-    def __hash__(self) -> int:
-        """Hash the nested tuple version of the data."""
-        tuple_val = _totuple(self)
-        return hash(tuple_val)
-
-
 # generic numpy array
 Numpy = np.ndarray
 
 
 class ArrayLike:
     """Type that stores a numpy array."""
 
@@ -70,15 +61,15 @@
         arr_imag = np.array(val["imag"])
         return arr_real + 1j * arr_imag
 
     @classmethod
     def convert_to_numpy(cls, val):
         """Convert the value to np.ndarray and provide some casting."""
         arr_numpy = np.array(val, ndmin=1, dtype=cls.dtype, copy=True)
-        arr_tidy3d = TidyNDArray(shape=arr_numpy.shape, dtype=arr_numpy.dtype)
+        arr_tidy3d = np.ndarray(shape=arr_numpy.shape, dtype=arr_numpy.dtype)
         arr_tidy3d[:] = arr_numpy
         return arr_tidy3d
 
     @classmethod
     def check_dims(cls, val):
         """Make sure the number of dimensions is correct."""
         if cls.ndim and val.ndim != cls.ndim:
```

### Comparing `tidy3d-2.0.3/tidy3d/components/validators.py` & `tidy3d-2.1.0/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/components/viz.py` & `tidy3d-2.1.0/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/config.py` & `tidy3d-2.1.0/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/constants.py` & `tidy3d-2.1.0/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/exceptions.py` & `tidy3d-2.1.0/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/log.py` & `tidy3d-2.1.0/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/material_library/material_library.py` & `tidy3d-2.1.0/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/material_library/material_reference.py` & `tidy3d-2.1.0/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.1.0/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 import numpy as np
 import jax.numpy as jnp
 from jax.tree_util import register_pytree_node_class
 from .....components.base import Tidy3dBaseModel, cached_property
 from .....exceptions import DataError, Tidy3dKeyError, AdjointError
 
 
+# condition setting when to set value in DataArray to zero:
+# if abs(val) <= VALUE_FILTER_THRESHOLD * max(abs(val))
+VALUE_FILTER_THRESHOLD = 1e-6
+
+
 @register_pytree_node_class
 class JaxDataArray(Tidy3dBaseModel):
     """A :class:`.DataArray`-like class that only wraps xarray for jax compability."""
 
     values: Any = pd.Field(
         ...,
         title="Values",
@@ -163,16 +168,23 @@
         raise NotImplementedError("Interpolation is not currently supported in the 'output_data'.")
 
     @cached_property
     def nonzero_val_coords(self) -> Tuple[List[complex], Dict[str, Any]]:
         """The value and coordinate associated with the only non-zero element of ``self.values``."""
 
         values = np.nan_to_num(self.as_ndarray)
-        nonzero_inds = np.nonzero(values)
-        nonzero_values = values[nonzero_inds].tolist()
+
+        # filter out values that are very small relative to maximum
+        values_filtered = values.copy()
+        max_value = np.max(np.abs(values_filtered))
+        val_cutoff = VALUE_FILTER_THRESHOLD * max_value
+        values_filtered[np.abs(values_filtered) <= val_cutoff] = 0.0
+
+        nonzero_inds = np.nonzero(values_filtered)
+        nonzero_values = values_filtered[nonzero_inds].tolist()
 
         nonzero_coords = {}
         for nz_inds, (coord_name, coord_list) in zip(nonzero_inds, self.coords.items()):
             coord_array = np.array(coord_list)
             nonzero_coords[coord_name] = coord_array[nz_inds].tolist()
 
         return nonzero_values, nonzero_coords
```

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.1.0/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.1.0/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/dispersion/fit_web.py` & `tidy3d-2.1.0/tidy3d/plugins/dispersion/fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.1.0/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.1.0/tidy3d/plugins/mode/mode_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,24 +112,80 @@
         Returns
         -------
         ModeSolverData
             :class:`.ModeSolverData` object containing the effective index and mode fields.
         """
         return self.data
 
+    # pylint: disable=too-many-locals
+    def _get_data_with_group_index(self) -> ModeSolverData:
+        """:class:`.ModeSolverData` with fields, effective and group indices on unexpanded grid.
+
+        Returns
+        -------
+        ModeSolverData
+            :class:`.ModeSolverData` object containing the effective and group indices, and mode
+            fields.
+        """
+
+        # insert extra frequency steps into original array
+        f_step = self.mode_spec.group_index_step
+        fractional_steps = (1 - f_step, 1, 1 + f_step)
+        freqs = np.outer(self.freqs, fractional_steps).flatten()
+
+        # create a copy with the required frequencies for numerical differentiation
+        mode_spec = self.mode_spec.copy(update={"group_index_step": False})
+        mode_solver = self.copy(update={"freqs": freqs, "mode_spec": mode_spec})
+        mode_solver_data = mode_solver.data_raw
+
+        # calculate group index
+        num_freqs = freqs.size
+        original_slice = slice(1, num_freqs, 3)
+        n_center = mode_solver_data.n_eff.isel(f=original_slice).values
+        n_backward = mode_solver_data.n_eff.isel(f=slice(0, num_freqs, 3)).values
+        n_forward = mode_solver_data.n_eff.isel(f=slice(2, num_freqs, 3)).values
+
+        n_group_data = n_center + (n_forward - n_backward) / (2 * f_step)
+        n_group = ModeIndexDataArray(
+            n_group_data,
+            coords={
+                "f": list(self.freqs),
+                "mode_index": np.arange(self.mode_spec.num_modes),
+            },
+            attrs={"long name": "Group index"},
+        )
+
+        # remove data corresponding to frequencies used only for group index calculation
+        update_dict = {
+            "n_complex": mode_solver_data.n_complex.isel(f=original_slice),
+            "n_group": n_group,
+        }
+
+        for key, field in mode_solver_data.field_components.items():
+            update_dict[key] = field.isel(f=original_slice)
+
+        # pylint: disable=protected-access
+        for key, data in mode_solver_data._grid_correction_dict.items():
+            update_dict[key] = data.isel(f=original_slice)
+
+        return mode_solver_data.copy(update=update_dict)
+
     @cached_property
     def data_raw(self) -> ModeSolverData:
         """:class:`.ModeSolverData` containing the field and effective index on unexpanded grid.
 
         Returns
         -------
         ModeSolverData
             :class:`.ModeSolverData` object containing the effective index and mode fields.
         """
 
+        if self.mode_spec.group_index_step > 0:
+            return self._get_data_with_group_index()
+
         _, _solver_coords = self.plane.pop_axis(
             self._solver_grid.boundaries.to_list, axis=self.normal_axis
         )
 
         # Compute and store the modes at all frequencies
         n_complex, fields = self._solve_all_freqs(
             coords=_solver_coords, symmetry=self.solver_symmetry
@@ -265,15 +321,16 @@
                 freq=freq, coords=coords, symmetry=symmetry
             )
             fields.append(fields_freq)
             n_complex.append(n_freq)
 
         return n_complex, fields
 
-    def _solve_single_freq(  # pylint:disable=too-many-locals
+    # pylint:disable=too-many-locals
+    def _solve_single_freq(
         self,
         freq: float,
         coords: Tuple[ArrayFloat1D, ArrayFloat1D],
         symmetry: Tuple[Symmetry, Symmetry],
     ) -> Tuple[float, Dict[str, ArrayComplex4D]]:
         """Call the mode solver at a single frequency.
         The fields are rotated from propagation coordinates back to global coordinates.
@@ -486,15 +543,16 @@
             size=self.plane.size,
             center=self.plane.center,
             mode_spec=self.mode_spec,
             freqs=self.freqs,
             name=name,
         )
 
-    def plot_field(  # pylint:disable=too-many-arguments
+    # pylint:disable=too-many-arguments
+    def plot_field(
         self,
         field_name: str,
         val: Literal["real", "imag", "abs"] = "real",
         eps_alpha: float = 0.2,
         robust: bool = True,
         vmin: float = None,
         vmax: float = None,
```

### Comparing `tidy3d-2.0.3/tidy3d/plugins/mode/solver.py` & `tidy3d-2.1.0/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.1.0/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.1.0/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.1.0/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.1.0/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/updater.py` & `tidy3d-2.1.0/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/asynchronous.py` & `tidy3d-2.1.0/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/auth.py` & `tidy3d-2.1.0/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/cacert.pem` & `tidy3d-2.1.0/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/cli/app.py` & `tidy3d-2.1.0/tidy3d/web/cli/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,26 @@
     """
 
 
 @click.command()
 @click.option("--apikey", prompt=False)
 def configure(apikey):
     """Click command to configure the api key.
+
+    Parameters
+    ----------
+    apikey : str
+        User input api key.
+    """
+    configure_fn(apikey)
+
+
+def configure_fn(apikey: str) -> None:
+    """Python function that tries to set configuration based on a provided API key.
+
     Parameters
     ----------
     apikey : str
         User input api key.
     """
 
     def auth(req):
```

### Comparing `tidy3d-2.0.3/tidy3d/web/cli/migrate.py` & `tidy3d-2.1.0/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/config.py` & `tidy3d-2.1.0/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/container.py` & `tidy3d-2.1.0/tidy3d/web/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pydantic as pd
 
 from . import webapi as web
 from .task import TaskId, TaskInfo, RunInfo, TaskName
 from ..components.simulation import Simulation
 from ..components.base import Tidy3dBaseModel
 from ..components.data.sim_data import SimulationData
+from ..log import log
 
 from ..exceptions import DataError
 
 
 DEFAULT_DATA_PATH = "simulation_data.hdf5"
 DEFAULT_DATA_DIR = "."
 
@@ -199,14 +200,15 @@
         True, title="Verbose", description="Whether to print info messages and progressbars."
     )
 
     def load_sim_data(self, task_name: str) -> SimulationData:
         """Load a :class:`.SimulationData` from file by task name."""
         task_data_path = self.task_paths[task_name]
         task_id = self.task_ids[task_name]
+        web.get_info(task_id)
         return web.load(
             task_id=task_id,
             path=task_data_path,
             replace_existing=False,
             verbose=self.verbose,
         )
 
@@ -379,27 +381,34 @@
 
         Note
         ----
         To loop through the data of completed simulations, can call :meth:`Batch.items`.
         """
 
         def pbar_description(task_name: str, status: str) -> str:
-            return f"{task_name}: status = {status}"
+            """Make a progressbar description based on the status."""
+            description = f"{task_name}: status = {status}"
+
+            # if something went wrong, make it red
+            if "error" in status or "diverge" in status:
+                description = f"[red]{description}"
+
+            return description
 
         run_statuses = [
             "draft",
             "queued",
             "preprocess",
             "queued_solver",
             "running",
             "postprocess",
             "visualize",
             "success",
         ]
-        end_statuses = ("success", "error", "diverged", "deleted", "draft")
+        end_statuses = ("success", "error", "errored", "diverged", "diverge", "deleted", "draft")
 
         if self.verbose:
             console = Console()
             console.log("Started working on Batch.")
 
             with Progress(console=console) as progress:
 
@@ -412,30 +421,36 @@
                     pbar_tasks[task_name] = pbar
 
                 while any(job.status not in end_statuses for job in self.jobs.values()):
                     for task_name, job in self.jobs.items():
                         pbar = pbar_tasks[task_name]
                         status = job.status
                         description = pbar_description(task_name, status)
-                        completed = run_statuses.index(status)
+
+                        # if a problem occured, update progressbar completion to 100%
+                        if status not in run_statuses:
+                            completed = run_statuses.index("success")
+                        else:
+                            completed = run_statuses.index(status)
+
                         progress.update(pbar, description=description, completed=completed)
                     time.sleep(web.REFRESH_TIME)
 
-                # set all to 100% completed
+                # set all to 100% completed (if error or diverge, will be red)
                 for task_name, job in self.jobs.items():
                     pbar = pbar_tasks[task_name]
                     status = job.status
                     description = pbar_description(task_name, status)
-                    if status == "success":
-                        progress.update(
-                            pbar,
-                            description=description,
-                            completed=len(run_statuses) - 1,
-                            refresh=True,
-                        )
+
+                    progress.update(
+                        pbar,
+                        description=description,
+                        completed=len(run_statuses) - 1,
+                        refresh=True,
+                    )
 
                 console.log("Batch complete.")
 
         else:
             while any(job.status not in end_statuses for job in self.jobs.values()):
                 time.sleep(web.REFRESH_TIME)
 
@@ -489,16 +504,21 @@
         The data for each task will be named as ``{path_dir}/{task_name}.hdf5``.
         The :class:`Batch` hdf5 file will be automatically saved as ``{path_dir}/batch.hdf5``,
         allowing one to load this :class:`Batch` later using ``batch = Batch.from_file()``.
         """
 
         self.to_file(self._batch_path(path_dir=path_dir))
 
-        for job in self.jobs.values():
+        for task_name, job in self.jobs.items():
             job_path = self._job_data_path(task_id=job.task_id, path_dir=path_dir)
+
+            if "error" in job.status:
+                log.warning(f"Not downloading '{task_name}' as the task errored.")
+                continue
+
             job.download(path=job_path)
 
     def load(self, path_dir: str = DEFAULT_DATA_DIR) -> BatchData:
         """Download results and load them into :class:`.BatchData` object.
 
         Parameters
         ----------
@@ -518,14 +538,19 @@
 
         if self.jobs is None:
             raise DataError("Can't load batch results, hasn't been uploaded.")
 
         task_paths = {}
         task_ids = {}
         for task_name, job in self.jobs.items():
+
+            if "error" in job.status:
+                log.warning(f"Not loading '{task_name}' as the task errored.")
+                continue
+
             task_paths[task_name] = self._job_data_path(task_id=job.task_id, path_dir=path_dir)
             task_ids[task_name] = self.jobs[task_name].task_id
 
         return BatchData(task_paths=task_paths, task_ids=task_ids, verbose=self.verbose)
 
     def delete(self):
         """Delete server-side data associated with each task in the batch."""
```

### Comparing `tidy3d-2.0.3/tidy3d/web/environment.py` & `tidy3d-2.1.0/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/http_management.py` & `tidy3d-2.1.0/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/httputils.py` & `tidy3d-2.1.0/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/material_fitter.py` & `tidy3d-2.1.0/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/material_libray.py` & `tidy3d-2.1.0/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/s3utils.py` & `tidy3d-2.1.0/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/simulation_task.py` & `tidy3d-2.1.0/tidy3d/web/simulation_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/task.py` & `tidy3d-2.1.0/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/types.py` & `tidy3d-2.1.0/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.0.3/tidy3d/web/webapi.py` & `tidy3d-2.1.0/tidy3d/web/webapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,16 @@
     simulation.validate_pre_upload()
     log.debug("Creating task.")
 
     task = SimulationTask.create(simulation, task_name, folder_name, callback_url)
     if verbose:
         console = Console()
         console.log(f"Created task '{task_name}' with task_id '{task.task_id}'.")
+        url = f"https://tidy3d.simulation.cloud/workbench?taskId={task.task_id}"
+        console.log(f"View task using web UI at [link={url}]'{url}'[/link].")
     task.upload_simulation(verbose=verbose, progress_callback=progress_callback)
 
     # log the url for the task in the web UI
     log.debug(
         f"{Env.current.website_endpoint}/folders/{task.folder.folder_id}/tasks/{task.task_id}"
     )
     return task.task_id
```

### Comparing `tidy3d-2.0.3/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.1.0/tidy3d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.0.3
+Version: 2.1.0
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,14 +56,22 @@
 ```
 pip install --user tidy3d
 tidy3d configure --apikey=XXX
 ```
 
 Where `XXX` is your API key, which can be copied from your [account page](https://tidy3d.simulation.cloud/account) in the web interface.
 
+In a hosted jupyter notebook environment (eg google colab), it may be more convenient to install and configure via the following lines at the top of the notebook.
+
+```
+!pip install tidy3d
+import tidy3d.web as web
+web.configure("XXX")
+```
+
 If those commands did not work, advanced installation instructions are below, which should help solve the issue.
 
 ### Advanced Installation Instructions
 
 Some users might require more a specialized installation, which we cover below.
 
 #### Using pip (recommended)
```

### Comparing `tidy3d-2.0.3/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.1.0/tidy3d.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 tests/test_plugins/__init__.py
 tests/test_plugins/test_adjoint.py
 tests/test_plugins/test_component_modeler.py
 tests/test_plugins/test_dispersion_fitter.py
 tests/test_plugins/test_mode_solver.py
 tests/test_plugins/test_polyslab.py
 tests/test_plugins/test_resonance_finder.py
+tests/test_plugins/test_waveguide.py
 tests/test_web/__init__.py
 tests/test_web/mock_web.py
 tests/test_web/test_auth.py
 tests/test_web/test_cli.py
 tests/test_web/test_material_fitter.py
 tests/test_web/test_task.py
 tests/test_web/test_tidy3d_folder.py
@@ -134,14 +135,16 @@
 tidy3d/plugins/mode/transforms.py
 tidy3d/plugins/polyslab/__init__.py
 tidy3d/plugins/polyslab/polyslab.py
 tidy3d/plugins/resonance/__init__.py
 tidy3d/plugins/resonance/resonance.py
 tidy3d/plugins/smatrix/__init__.py
 tidy3d/plugins/smatrix/smatrix.py
+tidy3d/plugins/waveguide/__init__.py
+tidy3d/plugins/waveguide/rectangular_dielectric.py
 tidy3d/web/__init__.py
 tidy3d/web/asynchronous.py
 tidy3d/web/auth.py
 tidy3d/web/cacert.pem
 tidy3d/web/cache.py
 tidy3d/web/config.py
 tidy3d/web/container.py
```

### Comparing `tidy3d-2.0.3/tidy3d.egg-info/requires.txt` & `tidy3d-2.1.0/tidy3d.egg-info/requires.txt`

 * *Files identical despite different names*

