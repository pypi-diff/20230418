# Comparing `tmp/PyFstat-1.9.0.tar.gz` & `tmp/PyFstat-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyFstat-1.9.0.tar", last modified: Fri Oct 30 19:46:33 2020, max compression
+gzip compressed data, was "PyFstat-2.0.0.tar", last modified: Tue Apr 18 15:22:12 2023, max compression
```

## Comparing `PyFstat-1.9.0.tar` & `PyFstat-2.0.0.tar`

### file list

```diff
@@ -1,78 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.748659 PyFstat-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)       33 2020-10-30 19:42:11.000000 PyFstat-1.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.736658 PyFstat-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.740658 PyFstat-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1462 2020-10-30 19:42:11.000000 PyFstat-1.9.0/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2253 2020-10-30 19:42:11.000000 PyFstat-1.9.0/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1607 2020-10-30 19:42:11.000000 PyFstat-1.9.0/.github/workflows/run_examples.yml
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-10-30 19:42:11.000000 PyFstat-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      177 2020-10-30 19:42:11.000000 PyFstat-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      944 2020-10-30 19:42:11.000000 PyFstat-1.9.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (116)     7618 2020-10-30 19:42:11.000000 PyFstat-1.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)      777 2020-10-30 19:42:11.000000 PyFstat-1.9.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)     1081 2020-10-30 19:42:11.000000 PyFstat-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      104 2020-10-30 19:42:11.000000 PyFstat-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    17739 2020-10-30 19:46:33.748659 PyFstat-1.9.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/PyFstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    17739 2020-10-30 19:46:33.000000 PyFstat-1.9.0/PyFstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2623 2020-10-30 19:46:33.000000 PyFstat-1.9.0/PyFstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-30 19:46:33.000000 PyFstat-1.9.0/PyFstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      108 2020-10-30 19:46:33.000000 PyFstat-1.9.0/PyFstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-10-30 19:46:33.000000 PyFstat-1.9.0/PyFstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    14264 2020-10-30 19:42:11.000000 PyFstat-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)      633 2020-10-30 19:42:11.000000 PyFstat-1.9.0/bin/check_if_virtual_environment.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      742 2020-10-30 19:42:11.000000 PyFstat-1.9.0/bin/get-and-export-ephemeris.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      717 2020-10-30 19:42:11.000000 PyFstat-1.9.0/bin/setup-dev-tools.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/examples/binary_examples/
--rw-r--r--   0 runner    (1001) docker     (116)     8971 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/binary_examples/PyFstat_example_binary_mcmc_vs_grid_comparison.py
--rw-r--r--   0 runner    (1001) docker     (116)     3414 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/binary_examples/PyFstat_example_semi_coherent_binary_search_using_MCMC.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/examples/followup_examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2602 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/followup_examples/PyFstat_example_semi_coherent_directed_follow_up.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/examples/glitch_examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2572 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_MCMC_search_on_1_glitch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2607 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_grid_search_on_1_glitch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1897 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_make_data_for_search_on_1_glitch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1304 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_standard_directed_MCMC_search_on_1_glitch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/examples/grid_examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2057 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/grid_examples/PyFstat_example_grid_search_F0.py
--rw-r--r--   0 runner    (1001) docker     (116)     1974 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/grid_examples/PyFstat_example_grid_search_F0F1.py
--rw-r--r--   0 runner    (1001) docker     (116)     2647 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/grid_examples/PyFstat_example_grid_search_F0F1F2.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/examples/mcmc_examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2314 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/mcmc_examples/PyFstat_example_MCMC_search_using_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/mcmc_examples/PyFstat_example_fully_coherent_MCMC_search.py
--rw-r--r--   0 runner    (1001) docker     (116)     2680 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/mcmc_examples/PyFstat_example_semi_coherent_MCMC_search.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.744659 PyFstat-1.9.0/examples/mcmc_vs_grid_simple_example/
--rw-r--r--   0 runner    (1001) docker     (116)    11521 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/mcmc_vs_grid_simple_example/PyFstat_example_simple_mcmc_vs_grid_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.748659 PyFstat-1.9.0/examples/other_examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2966 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/other_examples/PyFstat_example_InjectionParametersGenerator.py
--rw-r--r--   0 runner    (1001) docker     (116)     3045 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/other_examples/PyFstat_example_injecting_into_noise_sfts.py
--rw-r--r--   0 runner    (1001) docker     (116)     1182 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/other_examples/PyFstat_example_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (116)     2435 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/other_examples/PyFstat_example_twoF_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (116)     2612 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/run_all_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.748659 PyFstat-1.9.0/examples/transient_examples/
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/transient_examples/PyFstat_example_long_transient_MCMC_search.py
--rw-r--r--   0 runner    (1001) docker     (116)      799 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/transient_examples/PyFstat_example_make_data_for_long_transient_search.py
--rw-r--r--   0 runner    (1001) docker     (116)      840 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/transient_examples/PyFstat_example_make_data_for_short_transient_search.py
--rw-r--r--   0 runner    (1001) docker     (116)     1874 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/transient_examples/PyFstat_example_short_transient_MCMC_search.py
--rw-r--r--   0 runner    (1001) docker     (116)     1885 2020-10-30 19:42:11.000000 PyFstat-1.9.0/examples/transient_examples/PyFstat_example_short_transient_grid_search.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.748659 PyFstat-1.9.0/pyfstat/
--rw-r--r--   0 runner    (1001) docker     (116)      830 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      498 2020-10-30 19:46:33.748659 PyFstat-1.9.0/pyfstat/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    68931 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/core.py
--rw-r--r--   0 runner    (1001) docker     (116)    62555 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/grid_based_searches.py
--rw-r--r--   0 runner    (1001) docker     (116)    29366 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    45752 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/make_sfts.py
--rw-r--r--   0 runner    (1001) docker     (116)   129956 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/mcmc_based_searches.py
--rw-r--r--   0 runner    (1001) docker     (116)     8757 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/optimal_setup_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 19:46:33.748659 PyFstat-1.9.0/pyfstat/pyCUDAkernels/
--rw-r--r--   0 runner    (1001) docker     (116)     4443 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/pyCUDAkernels/cudaTransientFstatExpWindow.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4237 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/pyCUDAkernels/cudaTransientFstatRectWindow.cu
--rw-r--r--   0 runner    (1001) docker     (116)    18532 2020-10-30 19:42:11.000000 PyFstat-1.9.0/pyfstat/tcw_fstat_map_funcs.py
--rw-r--r--   0 runner    (1001) docker     (116)       37 2020-10-30 19:42:11.000000 PyFstat-1.9.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      108 2020-10-30 19:42:11.000000 PyFstat-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      381 2020-10-30 19:46:33.748659 PyFstat-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2020-10-30 19:42:11.000000 PyFstat-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)    62151 2020-10-30 19:42:11.000000 PyFstat-1.9.0/tests.py
--rw-r--r--   0 runner    (1001) docker     (116)    69057 2020-10-30 19:42:11.000000 PyFstat-1.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.947201 PyFstat-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    23890 2023-04-18 15:15:40.000000 PyFstat-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-18 15:15:40.000000 PyFstat-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 15:15:40.000000 PyFstat-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-04-18 15:22:12.947201 PyFstat-2.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/PyFstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-04-18 15:22:12.000000 PyFstat-2.0.0/PyFstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-18 15:22:12.000000 PyFstat-2.0.0/PyFstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:22:12.000000 PyFstat-2.0.0/PyFstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-18 15:22:12.000000 PyFstat-2.0.0/PyFstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 15:22:12.000000 PyFstat-2.0.0/PyFstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-04-18 15:15:40.000000 PyFstat-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/binary_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/binary_examples/PyFstat_example_binary_mcmc_vs_grid_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/binary_examples/PyFstat_example_semi_coherent_binary_search_using_MCMC.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/followup_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/followup_examples/PyFstat_example_semi_coherent_directed_follow_up.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/glitch_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_MCMC_search_on_1_glitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_grid_search_on_1_glitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_make_data_for_search_on_1_glitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_standard_directed_MCMC_search_on_1_glitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/grid_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/grid_examples/PyFstat_example_grid_search_F0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/grid_examples/PyFstat_example_grid_search_F0F1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/grid_examples/PyFstat_example_grid_search_F0F1F2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/grid_examples/PyFstat_example_grid_search_with_BSGL.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/mcmc_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/mcmc_examples/PyFstat_example_MCMC_search_using_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/mcmc_examples/PyFstat_example_fully_coherent_MCMC_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/mcmc_examples/PyFstat_example_fully_coherent_MCMC_search_with_BSGL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/mcmc_examples/PyFstat_example_semi_coherent_MCMC_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/mcmc_vs_grid_simple_example/
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/mcmc_vs_grid_simple_example/PyFstat_example_simple_mcmc_vs_grid_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/other_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/other_examples/PyFstat_example_InjectionParametersGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/other_examples/PyFstat_example_injecting_into_noise_sfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/other_examples/PyFstat_example_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/other_examples/PyFstat_example_twoF_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/run_all_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/transient_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/transient_examples/PyFstat_example_long_transient_MCMC_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/transient_examples/PyFstat_example_make_data_for_long_transient_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/transient_examples/PyFstat_example_make_data_for_short_transient_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/transient_examples/PyFstat_example_short_transient_MCMC_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/transient_examples/PyFstat_example_short_transient_grid_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.943201 PyFstat-2.0.0/examples/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-18 15:15:40.000000 PyFstat-2.0.0/examples/tutorials/tutorial_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.947201 PyFstat-2.0.0/pyfstat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 15:22:12.947201 PyFstat-2.0.0/pyfstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92525 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47491 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/grid_based_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/gridcorner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/injection_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64197 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/make_sfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137781 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/mcmc_based_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/optimal_setup_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.947201 PyFstat-2.0.0/pyfstat/pyCUDAkernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/pyCUDAkernels/cudaTransientFstatExpWindow.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/pyCUDAkernels/cudaTransientFstatRectWindow.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31939 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/tcw_fstat_map_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.947201 PyFstat-2.0.0/pyfstat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/converting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/gsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/runlalsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-18 15:15:40.000000 PyFstat-2.0.0/pyfstat/utils/sft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-18 15:22:12.947201 PyFstat-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-18 15:15:40.000000 PyFstat-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:22:12.947201 PyFstat-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/commons_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_grid_based_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_injection_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29443 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_make_sfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_mcmc_based_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-18 15:15:40.000000 PyFstat-2.0.0/tests/test_tcw_fstat_map_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69057 2023-04-18 15:15:40.000000 PyFstat-2.0.0/versioneer.py
```

### Comparing `PyFstat-1.9.0/LICENSE` & `PyFstat-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFstat-1.9.0/PKG-INFO` & `PyFstat-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,131 @@
 Metadata-Version: 2.1
 Name: PyFstat
-Version: 1.9.0
+Version: 2.0.0
 Summary: a python package for gravitational wave analysis with the F-statistic
 Home-page: https://github.com/PyFstat/PyFstat
 Author: Gregory Ashton, David Keitel, Reinhard Prix, Rodrigo Tenorio
 Author-email: gregory.ashton@ligo.org
 Maintainer: David Keitel
 Maintainer-email: david.keitel@ligo.org
 License: MIT
+Project-URL: Changelog, https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://pyfstat.readthedocs.io/
+Project-URL: Issue tracker, https://github.com/PyFstat/PyFstat/issues
 Description: # PyFstat
         
         This is a python package providing an interface to perform F-statistic based
-        continuous gravitational wave (CW) searches.
+        continuous gravitational wave (CW) searches,
+        built on top of the [LALSuite library](https://doi.org/10.7935/GT1W-FZ16).
         
         Getting started:
         * This README provides information on
-        installation,
-        [contributing](#contributors) to 
+        [installing](#installation),
+        [contributing](#contributors) to
         and [citing](#citing-this-work) PyFstat.
-        * Additional usage documentation will be added to the
-        [project wiki](https://github.com/PyFstat/PyFstat/wiki) (work in progress).
-        * We also have a number of
-        [examples](https://github.com/PyFstat/PyFstat/tree/master/examples),
-        demonstrating different use cases.
-        * New contributors are encouraged to have a look into
-        [how to set up a development environment](#contributing-to-pyfstat)
+        * PyFstat usage and its API are documented at [pyfstat.readthedocs.io](https://pyfstat.readthedocs.io/).
+        * We also have a number of [tutorials](https://github.com/PyFstat/PyFstat/tree/master/examples/tutorials) and
+        [examples](https://github.com/PyFstat/PyFstat/tree/master/examples), demonstrating different use cases.
+        You can run them locally, or online as jupyter notebooks with
+        [binder](https://mybinder.org/v2/gh/PyFstat/PyFstat/master).
+        * The [project wiki](https://github.com/PyFstat/PyFstat/wiki) is mainly used for developer information.
+        * A [changelog](https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md)
+        is also available.
+        * PyFstat >=2.0.0 requires a recent LALSuite (>=7.13) / lalpulsar (>=6.0)
+        including the [SFTv3 specification](https://dcc.ligo.org/T040164-v2/public).
+        If you need to work with older versions, the last PyFstat release supporting those was `1.19.1`.
         
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967045.svg)](https://doi.org/10.5281/zenodo.3967045)
         [![PyPI version](https://badge.fury.io/py/PyFstat.svg)](https://badge.fury.io/py/PyFstat)
-        ![Integration Tests](https://github.com/PyFstat/PyFstat/workflows/Integration%20Tests/badge.svg)
-        ![Docker](https://github.com/PyFstat/PyFstat/workflows/Docker/badge.svg)
-        
-        A [changelog](https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md)
-        is also available (only maintained from v1.2 onwards).
+        [![Conda version](https://anaconda.org/conda-forge/pyfstat/badges/version.svg)](https://anaconda.org/conda-forge/pyfstat)
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967045.svg)](https://doi.org/10.5281/zenodo.3967045)
+        [![ASCL](https://img.shields.io/badge/ascl-2102.027-blue.svg?colorB=262255)](https://ascl.net/2102.027)
+        [![JOSS](https://joss.theoj.org/papers/10.21105/joss.03000/status.svg)](https://doi.org/10.21105/joss.03000)
+        [![Docker](https://github.com/PyFstat/PyFstat/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/PyFstat/PyFstat/actions/workflows/docker-publish.yml)
+        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PyFstat/PyFstat/master)
+        [![Integration Tests](https://github.com/PyFstat/PyFstat/actions/workflows/integration.yml/badge.svg)](https://github.com/PyFstat/PyFstat/actions/workflows/integration.yml)
+        [![codecov](https://codecov.io/gh/PyFstat/PyFstat/branch/master/graph/badge.svg?token=P0W8MIIUGD)](https://codecov.io/gh/PyFstat/PyFstat)
+        [![Documentation Status](https://readthedocs.org/projects/pyfstat/badge/?version=latest)](https://pyfstat.readthedocs.io/en/latest/?badge=latest)
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         ## Installation
         
         PyFstat releases can be installed in a variety of ways, including
+        [`pip install` from PyPI](#pip-install-from-PyPi),
+        [conda](#conda-installation),
         [Docker/Singularity images](#docker-container),
-        [`pip install` from PyPi](#pip-install-from-PyPi),
         and [from source releases on Zenodo](#install-pyfstat-from-source-zenodo-or-git-clone).
         Latest development versions can
         [also be installed with pip](#pip-install-from-github)
         or [from a local git clone](#install-pyfstat-from-source-zenodo-or-git-clone).
         
-        If you don't have a recent `python` installation (`3.6+`) on your system or
-        prefer `conda` environments over system-wide installation / venvs, please
-        start with the [conda installation](#conda-installation) section.
+        If you don't have a recent `python` installation (`3.8+`) on your system,
+        then `Docker` or `conda` are the easiest paths.
         
         In either case, be sure to also check out the notes on
-        [dependencies](#dependencies),
-        [ephemerides files](#ephemerides-installation)
+        [dependencies](#dependencies)
         and [citing this work](#citing-this-work).
         
-        ### Docker container
-        Ready-to-use PyFstat containers are available at the [Packages](https://github.com/PyFstat/PyFstat/packages)
-        page. A git-hub account together with a personal access token is required. [Go to the wiki page](https://github.com/PyFstat/PyFstat/wiki/Containers) to learn how to pull them from the git-hub
-        registry using Docker or Singularity.
-        
-        ### pip install from PyPi
+        If you run into problems with ephemerides files, check the wiki page on
+        [ephemerides installation](https://github.com/PyFstat/PyFstat/wiki/ephemerides-installation).
         
-        PyPi releases are available from https://pypi.org/project/PyFstat/.
+        ### pip install from PyPI
         
-        Note that the PyFstat installation will fail at the
-        [LALSuite](https://pypi.org/project/lalsuite/) dependency stage
-        if your `pip` is too old (e.g. 18.1); to be on the safe side, before starting do
-        ```
-        pip install --upgrade pip
-        ```
+        PyPI releases are available from https://pypi.org/project/PyFstat/.
         
-        Then, a simple
+        A simple
         ```
         pip install pyfstat
         ```
-        should give you the latest release version with all dependencies.
+        should give you the latest release version with all dependencies;
+        recent releases now also include a sufficient minimal set of ephemerides files.
         
         If you are not installing into a [venv](https://docs.python.org/3/library/venv.html)
-        or [conda environment](#conda-installation),
+        or [conda environment](#conda-installation)
+        (you really should!),
         on many systems you may need to use the `--user` flag.
         
+        Note that the PyFstat installation will fail at the
+        LALSuite dependency stage
+        if your `pip` is too old (e.g. 18.1); to fix this, do
+        ```
+        pip install --upgrade pip setuptools
+        ```
+        
         ### conda installation
         
-        `PyFstat` requires `python3.6+`.
-        While many systems come with a system-wide python installation,
-        it may not be sufficiently recent for this package;
-        anyway, it can often be easier to manage a user-specific python installation
-        (this way one does not require root access to install or remove modules).
-        One method to do this is to use the `conda` system, either through
-        the stripped down [`Miniconda`](https://conda.pydata.org/miniconda.html)
-        installation, or the full-featured
-        [`Anaconda`](https://www.anaconda.com/products/individual#Downloads)
-        (these are essentially the
-        same, but the `Anaconda` version installs a variety of useful packages such as
-        `numpy` and `scipy` by default).
-        The fastest/easiest method is to follow your OS instructions
-        [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/)
-        which will install `Miniconda`.
-        
-        After you have installed a version of `conda` and
-        [set up an environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), 
-        `pip` can also be used to install modules into this environment.
-        (There is no direct `conda` release of `PyFstat` at the moment.)
-        This can be installed with
-        ```
-        conda install pip
-        ```
-        and then you can continue with the `pip` instructions,
-        either [a release version from PyPi](#pip-install-from-PyPi)
-        as described above
-        or [the latest development version directly from github](#pip-install-from-github)
-        as described below.
-        
-        A simple way to get started with an otherwise clean environment
-        is to use a minimal .yml recipe file
-        [as explained here](https://github.com/PyFstat/PyFstat/wiki/conda-environments).
-        
-        Alternatively, you may consider starting from an
-        [`igwn` environment](https://computing.docs.ligo.org/conda/),
-        which contains most packages relevant to gravitational waves,
-        instead of doing it from scratch,
-        and just adding `PyFstat` to it through pip as described above.
-        But be advised that the downloads for the `igwn` environments are huge.
+        See [this wiki page](https://github.com/PyFstat/PyFstat/wiki/conda-environments)
+        for further instructions on installing conda itself,
+        installing PyFstat into an existing environment,
+        or for .yml recipes to set up a PyFstat-specific environment
+        both for normal users and for developers.
+        
+        If getting PyFstat from conda-forge, it already includes the required ephemerides files.
+        
+        ### Docker container
+        
+        Ready-to-use PyFstat containers are available at the [Packages](https://github.com/PyFstat/PyFstat/packages)
+        page. A GitHub account together with a personal access token is required.
+        [Go to the wiki page](https://github.com/PyFstat/PyFstat/wiki/Containers)
+        to learn how to pull them from the GitHub registry using `Docker` or `Singularity`.
         
         ### pip install from github
         
         Development versions of PyFstat can also be easily installed by
         pointing pip directly to this git repository,
         which will give you the latest version of the master branch:
         ```
         pip install git+https://github.com/PyFstat/PyFstat
         ```
         or, if you have an ssh key installed in github:
         ```
         pip install git+ssh://git@github.com/PyFstat/PyFstat
         ```
         
-        
-        ### Dependencies
-        
-        PyFstat uses the following external python modules,
-        which should all be pulled in automatically if you use `pip`:
-        
-        * [numpy](https://www.numpy.org/)
-        * [matplotlib](https://matplotlib.org/)
-        * [scipy](https://www.scipy.org/)
-        * [ptemcee](https://github.com/willvousden/ptemcee)
-        * [corner](https://pypi.python.org/pypi/corner/)
-        * [dill](https://pypi.python.org/pypi/dill)
-        * [tqdm](https://pypi.python.org/pypi/tqdm)
-        * [bashplotlib](https://github.com/glamp/bashplotlib)
-        * [peakutils](https://pypi.python.org/pypi/PeakUtils)
-        * [pathos](https://pypi.python.org/pypi/pathos)
-        * [lalsuite](https://pypi.org/project/lalsuite/)
-        * [versioneer](https://pypi.org/project/versioneer/)
-        
-        In case the automatic install doesn't properly pull in all dependencies,
-        to install all of these modules manually, you can also run
-        ```
-        pip install -r /PATH/TO/THIS/DIRECTORY/requirements.txt
-        ```
-        For a general introduction to installing modules, see
-        [here](https://docs.python.org/3/installing/index.html).
-        
-        *Optional dependencies*:
-        * [pycuda](https://pypi.org/project/pycuda/),
-          required for the `tCWFstatMapVersion=pycuda`
-          option of the `TransientGridSearch` class.
-          (Note: `pip install pycuda` requires a working `nvcc` compiler in your path.)
-        * [pytest](https://docs.pytest.org) for running the test suite locally
-          (`python -m pytest tests.py`)
-        * Developers are also highly encouraged to use
-          the [flake8](https://flake8.pycqa.org/en/latest/) linter
-          and [black](https://black.readthedocs.io) style checker
-          locally,
-          as these checks are required to pass by the online integration pipeline.
-        * Some optional plotting methods depend on two additional packages,
-          and some of the [examples](./examples) require these to run:
-         [gridcorner](https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner) 
-          and [chainconsumer](https://github.com/Samreay/ChainConsumer);
-        for `pip` users this is most conveniently installed by
-        ```
-        pip install git+https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner
-        pip install chainconsumer
-        ```
-        * If you prefer to make your own LALSuite installation
-        [from source](https://git.ligo.org/lscsoft/lalsuite/),
-        make sure it is **swig-enabled** and contains at least the `lalpulsar` and `lalapps` packages.
-        A minimal configuration line to use would be e.g.:
-        ```
-        ./configure --prefix=${HOME}/lalsuite-install --disable-all-lal --enable-lalpulsar --enable-lalapps --enable-swig
-        ```
-        
+        This should pull in all dependencies in the same way as installing from PyPI,
+        and recent lalsuite dependencies will include ephemerides files too.
         
         ### install PyFstat from source (Zenodo or git clone)
         
         You can download a source release tarball from [Zenodo](https://doi.org/10.5281/zenodo.3967045)
         and extract to an arbitrary temporary directory.
         Alternatively, clone this repository:
         
@@ -224,133 +154,224 @@
         was successful, run
         ```
         python -c 'import pyfstat'
         ```
         if no error message is output, then you have installed `pyfstat`. Note that
         the module will be installed to whichever python executable you call it from.
         
-        ### Ephemerides installation
+        This should pull in all dependencies in the same way as installing from PyPI,
+        and recent lalsuite dependencies will include ephemerides files too.
         
-        PyFstat requires paths to earth and sun ephemerides files
-        in order to use the `lalpulsar.ComputeFstat` module and various `lalapps` tools.
+        ### Dependencies
         
-        If you have done `pip install lalsuite`
-        (or it got pulled in automatically as a dependency),
-        you need to manually download at least these two files:
-        *  [earth00-40-DE405.dat.gz](https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/earth00-40-DE405.dat.gz)
-        *  [sun00-40-DE405.dat.gz](https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/sun00-40-DE405.dat.gz)
-        
-        (Other ephemerides versions exist, but these two files should be sufficient for most applications.)
-        You then need to tell PyFstat where to find these files,
-        by either setting an environment variable `$LALPULSAR_DATADIR`
-        or by creating a `~/.pyfstat.conf` file as described further below.
-        If you are working with a virtual environment,
-        you should be able to get a full working ephemerides installation with these commands:
-        ```
-        mkdir $VIRTUAL_ENV/share/lalpulsar
-        wget https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/earth00-40-DE405.dat.gz -P $VIRTUAL_ENV/share/lalpulsar
-        wget https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/sun00-40-DE405.dat.gz -P $VIRTUAL_ENV/share/lalpulsar
-        echo 'export LALPULSAR_DATADIR=$VIRTUAL_ENV/share/lalpulsar' >> ${VIRTUAL_ENV}/bin/activate
-        deactivate
-        source path/to/venv/bin/activate
-        ```
-        An executable version of this snippet is readily accessible by **sourcing** `bin/get-and-export-ephemeris.sh`. 
-        Mind that this script does **not** include an `export` command anywhere, so you will have to source it every time
-        in order to properly set `LALPULSAR_DATADIR` variable.
-        
-        If instead you have built and installed lalsuite from source,
-        and set your path up properly through something like
-        `source $MYLALPATH/etc/lalsuite-user-env.sh`,
-        then the ephemerides path should be automatically picked up from
-        the `$LALPULSAR_DATADIR` environment variable.
-        Similarly, if you have installed lalsuite from conda-forge,
-        it should come with ephemerides included and properly set up.
-        
-        Alternatively, you can place a file
-        `~/.pyfstat.conf` into your home directory which looks like
+        PyFstat uses the following external python modules,
+        which should all be pulled in automatically if you use `pip`:
+        
+        * [corner](https://pypi.python.org/pypi/corner/)
+        * [dill](https://pypi.python.org/pypi/dill)
+        * [lalsuite](https://pypi.org/project/lalsuite/)
+        * [matplotlib](https://matplotlib.org/)
+        * [numpy](https://www.numpy.org/)
+        * [pathos](https://pypi.python.org/pypi/pathos)
+        * [ptemcee](https://github.com/willvousden/ptemcee)
+        * [scipy](https://www.scipy.org/)
+        * [tqdm](https://pypi.python.org/pypi/tqdm)
+        * [versioneer](https://pypi.org/project/versioneer/)
         
+        For a general introduction to installing modules, see
+        [here](https://docs.python.org/3/installing/index.html).
+        
+        NOTE: currently we have pinned to
+        `numpy<1.24.0` (due to an incompatibility with ptemcee).
+        
+        NOTE: We require a recent LALSuite (>=7.13) / lalpulsar (>=6.0).
+        If you need to work with older versions,
+        the last PyFstat release supporting those was `1.19.1`.
+        
+        ### Optional dependencies
+        
+        PyFstat manages optional dependencies through setuptool's `extras_require`.
+        
+        Available sets of optional dependencies are:
+        
+        * `chainconsumer` ([Samreay/Chainconsumer](https://github.com/Samreay/ChainConsumer)): Required to run some optional
+        plotting methods and some of the [example scripts](./examples).
+        * `dev`: Collects `docs`, `style`, `test` and `wheel`.
+        * `docs`: Required dependencies to build the documentation.
+        * `pycuda` ([PyPI](https://pypi.org/project/pycuda/)): Required for the `tCWFstatMapVersion=pycuda`
+          option of the `TransientGridSearch` class. (Note: Installing `pycuda` requires a working
+          `nvcc` compiler in your path.)
+        * `style`: Includes the `flake8` linter ([flake8.pycqa](https://flake8.pycqa.org/en/latest)),
+          `black` style checker ([black.readthedocs](https://black.readthedocs.io)),
+          and `isort` for import ordering ([pycqa.github.io](https://pycqa.github.io/isort/)).
+          These checks are required to pass by the online integration pipeline.
+        * `test`: For running the test suite locally using [pytest](https://docs.pytest.org) and some of its addons
+          (`python -m pytest tests/`).
+        * `wheel`: Includes `wheel` and `check-wheel-contents`.
+        
+        Installation can be done by adding one or more of the aforementioned tags to the installation command.
+        
+        For example, installing PyFstat including `chainconsumer`, `pycuda` and `style` dependencies would look like
+        (mind the lack of whitespaces!)
         ```
-        earth_ephem = '/home/<USER>/lalsuite-install/share/lalpulsar/earth00-19-DE405.dat.gz'
-        sun_ephem = '/home/<USER>/lalsuite-install/share/lalpulsar/sun00-19-DE405.dat.gz'
+        pip install pyfstat[chainconsumer,pycuda,style]
         ```
-        Paths set in this way will take precedence over the environment variable.
+        This command accepts the "development mode" tag `-e`.
         
-        Finally, you can manually specify ephemerides files when initialising
-        each PyFstat search (as one of the arguments).
+        Note that LALSuite is a default requirement, not an optional one,
+        but its installation from PyPI can be disabled
+        by setting the `NO_LALSUITE_FROM_PYPI` environment variable,
+        e.g. for a development install from a local git clone:
+        ```
+        NO_LALSUITE_FROM_PYPI=1 pip install -e .
+        ```
+        This can be useful to avoid duplication when in a conda environment
+        or installing LALSuite from source.
+        
+        ### Using LALSuite built from source
+        
+        Instructions to use a custom local LALSuite installation can be found in [here on the wiki](https://github.com/PyFstat/PyFstat/wiki/Using-LALSuite-built-from-source).
         
         ## Contributing to PyFstat
+        
         This project is open to development, please feel free to contact us
         for advice or just jump in and submit an
         [issue](https://github.com/PyFstat/PyFstat/issues/new/choose) or
         [pull request](https://github.com/PyFstat/PyFstat/compare).
         
         Here's what you need to know:
-        * The github automated tests currently run on `python` [3.6,3.7,3.8] and new PRs need to pass all these.
-        * The automated test also runs
-          the [black](https://black.readthedocs.io) style checker
-          and the [flake8](https://flake8.pycqa.org/en/latest/) linter.
-          If at all possible, please run these two tools locally before pushing changes / submitting PRs:
+        * As a developer, you should install directly from a git clone,
+          with either `pip install -e .[dev]` into some environment
+          or creating a development-enabled conda environment directly from the
+          `pyfstat-dev.yml` file
+          as explained on [this wiki page](https://github.com/PyFstat/PyFstat/wiki/conda-environments).
+          Please also run, just once after installing:
+          ```
+          pre-commit install
+          ```
+        
+          This sets up everything for automated code quality tests (see below)
+          to be checked for you at every commit.
+        * The github automated tests currently run on `python` [3.8,3.9,3.10,3.11]
+          and new PRs need to pass all these.
+        * You can also run the full test suite locally via `pytest tests/`,
+          or run individual tests as explained
+          [on this page](https://docs.pytest.org/en/6.2.x/usage.html#specifying-tests-selecting-tests).
+        * The automated test on github also runs
+          the [black](https://black.readthedocs.io) style checker,
+          the [flake8](https://flake8.pycqa.org/en/latest/) linter,
+          and the [isort](https://pycqa.github.io/isort/) import ordering helper.
+        * If you have installed the dev dependencies correctly via pip or conda,
+          and ran `pre-commit install` once,
+          then you're ready to let the `pre-commit` tool do all of this automatically for you
+          every time you do `git commit`.
+          For anything that would fail on the github integration tests,
+          it will then either automatically reformat your code to match our style
+          or print warnings for things to fix.
+          The first time it will take a while for setup,
+          later it should be faster.
+        * If for some reason you can't use `pre-commit`,
+          you can still manually run these tools before pushing changes / submitting PRs:
+          `isort .` to sort package imports,
           `flake8 --count --statistics .` to find common coding errors and then fix them manually,
-          and then
           `black --check --diff .` to show the required style changes, or `black .` to automatically apply them.
-        * `bin/setup-dev-tools.sh` gets your virtual environment ready for you. After making sure you are 
-        using a virtual environment (venv or conda),
-        it installs `black`, `flake8`, `pre-commit`, `pytest`, `wheel` via `pip` and uses `pre-commit` to run
-        the `black` and `flake8` using a pre-commit hook. In this way, you will be prompted a warning whenever you
-        forget to run `black` or `flake8` before doing your commit :wink:.
         
         ## Contributors
         
         Maintainers:
         * Greg Ashton
         * David Keitel
         
-        Other contributors:
+        Active contributors:
         * Reinhard Prix
         * Rodrigo Tenorio
+        
+        Other contributors:
         * Karl Wette
         * Sylvia Zhu
+        * Dan Foreman-Mackey (`pyfstat.gridcorner` is based on DFM's [corner.py](https://github.com/dfm/corner.py))
         
         
         ## Citing this work
         
-        If you use `PyFstat` in a publication we would appreciate if you cite both a DOI for the software itself (see below)
-        and the original paper introducing the code: Ashton&Prix 2018 [[inspire](https://inspirehep.net/literature/1655200)] [[ADS](https://ui.adsabs.harvard.edu/abs/2018PhRvD..97j3020A/)].
-        If you use the transient module, please also cite: Keitel&Ashton 2018 [[inspire](https://inspirehep.net/literature/1673205)] [[ADS](https://ui.adsabs.harvard.edu/abs/2018CQGra..35t5003K/)].
+        If you use `PyFstat` in a publication we would appreciate if you cite both a release DOI for the software itself (see below)
+        and one or more of the following scientific papers:
+        * The recent JOSS (Journal of Open Source Software) paper summarising the package:
+        [Keitel, Tenorio, Ashton & Prix 2021](https://doi.org/10.21105/joss.03000)
+        ([inspire:1842895](https://inspirehep.net/literature/1842895)
+        / [ADS:2021arXiv210110915K](https://ui.adsabs.harvard.edu/abs/2021arXiv210110915K/)).
+        * The original paper introducing the package and the MCMC functionality:
+        [Ashton&Prix 2018](https://doi.org/10.1103/PhysRevD.97.103020)
+        ([inspire:1655200](https://inspirehep.net/literature/1655200)
+        / [ADS:2018PhRvD..97j3020A](https://ui.adsabs.harvard.edu/abs/2018PhRvD..97j3020A/)).
+        * The methods paper introducing a Bayes factor to evaluate the multi-stage follow-up:
+        [Tenorio, Keitel, Sintes 2021](https://doi.org/10.1103/PhysRevD.104.084012)
+        ([inspire:1865975](https://inspirehep.net/literature/1865975)
+        / [ADS:2021PhRvD.104h4012T](https://ui.adsabs.harvard.edu/abs/2021PhRvD.104h4012T/))
+        * For transient searches:
+        [Keitel&Ashton 2018](https://doi.org/10.1088/1361-6382/aade34)
+        ([inspire:1673205](https://inspirehep.net/literature/1673205)
+        / [ADS:2018CQGra..35t5003K](https://ui.adsabs.harvard.edu/abs/2018CQGra..35t5003K/)).
+        * For glitch-robust searches:
+        [Ashton, Prix & Jones 2018](https://doi.org/10.1103/PhysRevD.98.063011)
+        ([inspire:1672396](https://inspirehep.net/literature/1672396)
+        / [ADS:2018PhRvD..98f3011A](https://ui.adsabs.harvard.edu/abs/2018PhRvD..98f3011A/)
         
-        If you'd like to cite the `PyFstat` package in general,
-        or versions from 1.5.x upwards,
+        If you'd additionally like to cite the `PyFstat` package in general,
         please refer to the [version-independent Zenodo listing](https://doi.org/10.5281/zenodo.3967045)
         or use directly the following BibTeX entry:
         ```
         @misc{pyfstat,
           author       = {Ashton, Gregory and
                           Keitel, David and
                           Prix, Reinhard
                           and Tenorio, Rodrigo},
-          title        = {PyFstat},
+          title        = {{PyFstat}},
           month        = jul,
           year         = 2020,
           publisher    = {Zenodo},
           doi          = {10.5281/zenodo.3967045},
           url          = {https://doi.org/10.5281/zenodo.3967045},
           note         = {\url{https://doi.org/10.5281/zenodo.3967045}}
         }
         ```
-        You can also obtain DOIs for individual versioned releases
+        You can also obtain DOIs for individual versioned releases (from 1.5.x upward)
         from the right sidebar at [Zenodo](https://doi.org/10.5281/zenodo.3967045).
         
         Alternatively, if you've used PyFstat up to version 1.4.x in your works,
-        the DOIs for those version can be found from the sidebar at
+        the DOIs for those versions can be found from the sidebar at
         [this older Zenodo record](https://doi.org/10.5281/zenodo.1243930)
         and please amend the BibTeX entry accordingly.
         
+        
+        PyFstat uses the [`ptemcee` sampler](https://github.com/willvousden/ptemcee), which can be
+        cited as
+        [Vousden, Far & Mandel 2015](https://doi.org/10.1093/mnras/stv2422)
+        ([ADS:2016MNRAS.455.1919V](https://ui.adsabs.harvard.edu/abs/2016MNRAS.455.1919V/abstract))
+        and [Foreman-Mackey, Hogg, Lang, and Goodman 2012](https://doi.org/10.1086/670067)
+        ([2013PASP..125..306F](https://ui.adsabs.harvard.edu/abs/2013PASP..125..306F/abstract)).
+        
+        PyFstat also makes generous use of functionality from the LALSuite library
+        and it will usually be appropriate to also cite that project
+        (see [this recommended bibtex entry](https://git.ligo.org/lscsoft/lalsuite/#acknowledgment))
+        and also [Wette 2020](https://doi.org/10.1016/j.softx.2020.100634)
+        ([inspire:1837108](https://inspirehep.net/literature/1837108)
+        / [ADS:2020SoftX..1200634W](https://ui.adsabs.harvard.edu/abs/2020SoftX..1200634W/))
+        for the C-to-python [SWIG](http://www.swig.org) bindings.
+        
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: chainconsumer
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: pycuda
+Provides-Extra: style
+Provides-Extra: test
+Provides-Extra: wheel
```

### Comparing `PyFstat-1.9.0/PyFstat.egg-info/PKG-INFO` & `PyFstat-2.0.0/PyFstat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,131 @@
 Metadata-Version: 2.1
 Name: PyFstat
-Version: 1.9.0
+Version: 2.0.0
 Summary: a python package for gravitational wave analysis with the F-statistic
 Home-page: https://github.com/PyFstat/PyFstat
 Author: Gregory Ashton, David Keitel, Reinhard Prix, Rodrigo Tenorio
 Author-email: gregory.ashton@ligo.org
 Maintainer: David Keitel
 Maintainer-email: david.keitel@ligo.org
 License: MIT
+Project-URL: Changelog, https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://pyfstat.readthedocs.io/
+Project-URL: Issue tracker, https://github.com/PyFstat/PyFstat/issues
 Description: # PyFstat
         
         This is a python package providing an interface to perform F-statistic based
-        continuous gravitational wave (CW) searches.
+        continuous gravitational wave (CW) searches,
+        built on top of the [LALSuite library](https://doi.org/10.7935/GT1W-FZ16).
         
         Getting started:
         * This README provides information on
-        installation,
-        [contributing](#contributors) to 
+        [installing](#installation),
+        [contributing](#contributors) to
         and [citing](#citing-this-work) PyFstat.
-        * Additional usage documentation will be added to the
-        [project wiki](https://github.com/PyFstat/PyFstat/wiki) (work in progress).
-        * We also have a number of
-        [examples](https://github.com/PyFstat/PyFstat/tree/master/examples),
-        demonstrating different use cases.
-        * New contributors are encouraged to have a look into
-        [how to set up a development environment](#contributing-to-pyfstat)
+        * PyFstat usage and its API are documented at [pyfstat.readthedocs.io](https://pyfstat.readthedocs.io/).
+        * We also have a number of [tutorials](https://github.com/PyFstat/PyFstat/tree/master/examples/tutorials) and
+        [examples](https://github.com/PyFstat/PyFstat/tree/master/examples), demonstrating different use cases.
+        You can run them locally, or online as jupyter notebooks with
+        [binder](https://mybinder.org/v2/gh/PyFstat/PyFstat/master).
+        * The [project wiki](https://github.com/PyFstat/PyFstat/wiki) is mainly used for developer information.
+        * A [changelog](https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md)
+        is also available.
+        * PyFstat >=2.0.0 requires a recent LALSuite (>=7.13) / lalpulsar (>=6.0)
+        including the [SFTv3 specification](https://dcc.ligo.org/T040164-v2/public).
+        If you need to work with older versions, the last PyFstat release supporting those was `1.19.1`.
         
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967045.svg)](https://doi.org/10.5281/zenodo.3967045)
         [![PyPI version](https://badge.fury.io/py/PyFstat.svg)](https://badge.fury.io/py/PyFstat)
-        ![Integration Tests](https://github.com/PyFstat/PyFstat/workflows/Integration%20Tests/badge.svg)
-        ![Docker](https://github.com/PyFstat/PyFstat/workflows/Docker/badge.svg)
-        
-        A [changelog](https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md)
-        is also available (only maintained from v1.2 onwards).
+        [![Conda version](https://anaconda.org/conda-forge/pyfstat/badges/version.svg)](https://anaconda.org/conda-forge/pyfstat)
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967045.svg)](https://doi.org/10.5281/zenodo.3967045)
+        [![ASCL](https://img.shields.io/badge/ascl-2102.027-blue.svg?colorB=262255)](https://ascl.net/2102.027)
+        [![JOSS](https://joss.theoj.org/papers/10.21105/joss.03000/status.svg)](https://doi.org/10.21105/joss.03000)
+        [![Docker](https://github.com/PyFstat/PyFstat/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/PyFstat/PyFstat/actions/workflows/docker-publish.yml)
+        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PyFstat/PyFstat/master)
+        [![Integration Tests](https://github.com/PyFstat/PyFstat/actions/workflows/integration.yml/badge.svg)](https://github.com/PyFstat/PyFstat/actions/workflows/integration.yml)
+        [![codecov](https://codecov.io/gh/PyFstat/PyFstat/branch/master/graph/badge.svg?token=P0W8MIIUGD)](https://codecov.io/gh/PyFstat/PyFstat)
+        [![Documentation Status](https://readthedocs.org/projects/pyfstat/badge/?version=latest)](https://pyfstat.readthedocs.io/en/latest/?badge=latest)
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         ## Installation
         
         PyFstat releases can be installed in a variety of ways, including
+        [`pip install` from PyPI](#pip-install-from-PyPi),
+        [conda](#conda-installation),
         [Docker/Singularity images](#docker-container),
-        [`pip install` from PyPi](#pip-install-from-PyPi),
         and [from source releases on Zenodo](#install-pyfstat-from-source-zenodo-or-git-clone).
         Latest development versions can
         [also be installed with pip](#pip-install-from-github)
         or [from a local git clone](#install-pyfstat-from-source-zenodo-or-git-clone).
         
-        If you don't have a recent `python` installation (`3.6+`) on your system or
-        prefer `conda` environments over system-wide installation / venvs, please
-        start with the [conda installation](#conda-installation) section.
+        If you don't have a recent `python` installation (`3.8+`) on your system,
+        then `Docker` or `conda` are the easiest paths.
         
         In either case, be sure to also check out the notes on
-        [dependencies](#dependencies),
-        [ephemerides files](#ephemerides-installation)
+        [dependencies](#dependencies)
         and [citing this work](#citing-this-work).
         
-        ### Docker container
-        Ready-to-use PyFstat containers are available at the [Packages](https://github.com/PyFstat/PyFstat/packages)
-        page. A git-hub account together with a personal access token is required. [Go to the wiki page](https://github.com/PyFstat/PyFstat/wiki/Containers) to learn how to pull them from the git-hub
-        registry using Docker or Singularity.
-        
-        ### pip install from PyPi
+        If you run into problems with ephemerides files, check the wiki page on
+        [ephemerides installation](https://github.com/PyFstat/PyFstat/wiki/ephemerides-installation).
         
-        PyPi releases are available from https://pypi.org/project/PyFstat/.
+        ### pip install from PyPI
         
-        Note that the PyFstat installation will fail at the
-        [LALSuite](https://pypi.org/project/lalsuite/) dependency stage
-        if your `pip` is too old (e.g. 18.1); to be on the safe side, before starting do
-        ```
-        pip install --upgrade pip
-        ```
+        PyPI releases are available from https://pypi.org/project/PyFstat/.
         
-        Then, a simple
+        A simple
         ```
         pip install pyfstat
         ```
-        should give you the latest release version with all dependencies.
+        should give you the latest release version with all dependencies;
+        recent releases now also include a sufficient minimal set of ephemerides files.
         
         If you are not installing into a [venv](https://docs.python.org/3/library/venv.html)
-        or [conda environment](#conda-installation),
+        or [conda environment](#conda-installation)
+        (you really should!),
         on many systems you may need to use the `--user` flag.
         
+        Note that the PyFstat installation will fail at the
+        LALSuite dependency stage
+        if your `pip` is too old (e.g. 18.1); to fix this, do
+        ```
+        pip install --upgrade pip setuptools
+        ```
+        
         ### conda installation
         
-        `PyFstat` requires `python3.6+`.
-        While many systems come with a system-wide python installation,
-        it may not be sufficiently recent for this package;
-        anyway, it can often be easier to manage a user-specific python installation
-        (this way one does not require root access to install or remove modules).
-        One method to do this is to use the `conda` system, either through
-        the stripped down [`Miniconda`](https://conda.pydata.org/miniconda.html)
-        installation, or the full-featured
-        [`Anaconda`](https://www.anaconda.com/products/individual#Downloads)
-        (these are essentially the
-        same, but the `Anaconda` version installs a variety of useful packages such as
-        `numpy` and `scipy` by default).
-        The fastest/easiest method is to follow your OS instructions
-        [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/)
-        which will install `Miniconda`.
-        
-        After you have installed a version of `conda` and
-        [set up an environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), 
-        `pip` can also be used to install modules into this environment.
-        (There is no direct `conda` release of `PyFstat` at the moment.)
-        This can be installed with
-        ```
-        conda install pip
-        ```
-        and then you can continue with the `pip` instructions,
-        either [a release version from PyPi](#pip-install-from-PyPi)
-        as described above
-        or [the latest development version directly from github](#pip-install-from-github)
-        as described below.
-        
-        A simple way to get started with an otherwise clean environment
-        is to use a minimal .yml recipe file
-        [as explained here](https://github.com/PyFstat/PyFstat/wiki/conda-environments).
-        
-        Alternatively, you may consider starting from an
-        [`igwn` environment](https://computing.docs.ligo.org/conda/),
-        which contains most packages relevant to gravitational waves,
-        instead of doing it from scratch,
-        and just adding `PyFstat` to it through pip as described above.
-        But be advised that the downloads for the `igwn` environments are huge.
+        See [this wiki page](https://github.com/PyFstat/PyFstat/wiki/conda-environments)
+        for further instructions on installing conda itself,
+        installing PyFstat into an existing environment,
+        or for .yml recipes to set up a PyFstat-specific environment
+        both for normal users and for developers.
+        
+        If getting PyFstat from conda-forge, it already includes the required ephemerides files.
+        
+        ### Docker container
+        
+        Ready-to-use PyFstat containers are available at the [Packages](https://github.com/PyFstat/PyFstat/packages)
+        page. A GitHub account together with a personal access token is required.
+        [Go to the wiki page](https://github.com/PyFstat/PyFstat/wiki/Containers)
+        to learn how to pull them from the GitHub registry using `Docker` or `Singularity`.
         
         ### pip install from github
         
         Development versions of PyFstat can also be easily installed by
         pointing pip directly to this git repository,
         which will give you the latest version of the master branch:
         ```
         pip install git+https://github.com/PyFstat/PyFstat
         ```
         or, if you have an ssh key installed in github:
         ```
         pip install git+ssh://git@github.com/PyFstat/PyFstat
         ```
         
-        
-        ### Dependencies
-        
-        PyFstat uses the following external python modules,
-        which should all be pulled in automatically if you use `pip`:
-        
-        * [numpy](https://www.numpy.org/)
-        * [matplotlib](https://matplotlib.org/)
-        * [scipy](https://www.scipy.org/)
-        * [ptemcee](https://github.com/willvousden/ptemcee)
-        * [corner](https://pypi.python.org/pypi/corner/)
-        * [dill](https://pypi.python.org/pypi/dill)
-        * [tqdm](https://pypi.python.org/pypi/tqdm)
-        * [bashplotlib](https://github.com/glamp/bashplotlib)
-        * [peakutils](https://pypi.python.org/pypi/PeakUtils)
-        * [pathos](https://pypi.python.org/pypi/pathos)
-        * [lalsuite](https://pypi.org/project/lalsuite/)
-        * [versioneer](https://pypi.org/project/versioneer/)
-        
-        In case the automatic install doesn't properly pull in all dependencies,
-        to install all of these modules manually, you can also run
-        ```
-        pip install -r /PATH/TO/THIS/DIRECTORY/requirements.txt
-        ```
-        For a general introduction to installing modules, see
-        [here](https://docs.python.org/3/installing/index.html).
-        
-        *Optional dependencies*:
-        * [pycuda](https://pypi.org/project/pycuda/),
-          required for the `tCWFstatMapVersion=pycuda`
-          option of the `TransientGridSearch` class.
-          (Note: `pip install pycuda` requires a working `nvcc` compiler in your path.)
-        * [pytest](https://docs.pytest.org) for running the test suite locally
-          (`python -m pytest tests.py`)
-        * Developers are also highly encouraged to use
-          the [flake8](https://flake8.pycqa.org/en/latest/) linter
-          and [black](https://black.readthedocs.io) style checker
-          locally,
-          as these checks are required to pass by the online integration pipeline.
-        * Some optional plotting methods depend on two additional packages,
-          and some of the [examples](./examples) require these to run:
-         [gridcorner](https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner) 
-          and [chainconsumer](https://github.com/Samreay/ChainConsumer);
-        for `pip` users this is most conveniently installed by
-        ```
-        pip install git+https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner
-        pip install chainconsumer
-        ```
-        * If you prefer to make your own LALSuite installation
-        [from source](https://git.ligo.org/lscsoft/lalsuite/),
-        make sure it is **swig-enabled** and contains at least the `lalpulsar` and `lalapps` packages.
-        A minimal configuration line to use would be e.g.:
-        ```
-        ./configure --prefix=${HOME}/lalsuite-install --disable-all-lal --enable-lalpulsar --enable-lalapps --enable-swig
-        ```
-        
+        This should pull in all dependencies in the same way as installing from PyPI,
+        and recent lalsuite dependencies will include ephemerides files too.
         
         ### install PyFstat from source (Zenodo or git clone)
         
         You can download a source release tarball from [Zenodo](https://doi.org/10.5281/zenodo.3967045)
         and extract to an arbitrary temporary directory.
         Alternatively, clone this repository:
         
@@ -224,133 +154,224 @@
         was successful, run
         ```
         python -c 'import pyfstat'
         ```
         if no error message is output, then you have installed `pyfstat`. Note that
         the module will be installed to whichever python executable you call it from.
         
-        ### Ephemerides installation
+        This should pull in all dependencies in the same way as installing from PyPI,
+        and recent lalsuite dependencies will include ephemerides files too.
         
-        PyFstat requires paths to earth and sun ephemerides files
-        in order to use the `lalpulsar.ComputeFstat` module and various `lalapps` tools.
+        ### Dependencies
         
-        If you have done `pip install lalsuite`
-        (or it got pulled in automatically as a dependency),
-        you need to manually download at least these two files:
-        *  [earth00-40-DE405.dat.gz](https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/earth00-40-DE405.dat.gz)
-        *  [sun00-40-DE405.dat.gz](https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/sun00-40-DE405.dat.gz)
-        
-        (Other ephemerides versions exist, but these two files should be sufficient for most applications.)
-        You then need to tell PyFstat where to find these files,
-        by either setting an environment variable `$LALPULSAR_DATADIR`
-        or by creating a `~/.pyfstat.conf` file as described further below.
-        If you are working with a virtual environment,
-        you should be able to get a full working ephemerides installation with these commands:
-        ```
-        mkdir $VIRTUAL_ENV/share/lalpulsar
-        wget https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/earth00-40-DE405.dat.gz -P $VIRTUAL_ENV/share/lalpulsar
-        wget https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/sun00-40-DE405.dat.gz -P $VIRTUAL_ENV/share/lalpulsar
-        echo 'export LALPULSAR_DATADIR=$VIRTUAL_ENV/share/lalpulsar' >> ${VIRTUAL_ENV}/bin/activate
-        deactivate
-        source path/to/venv/bin/activate
-        ```
-        An executable version of this snippet is readily accessible by **sourcing** `bin/get-and-export-ephemeris.sh`. 
-        Mind that this script does **not** include an `export` command anywhere, so you will have to source it every time
-        in order to properly set `LALPULSAR_DATADIR` variable.
-        
-        If instead you have built and installed lalsuite from source,
-        and set your path up properly through something like
-        `source $MYLALPATH/etc/lalsuite-user-env.sh`,
-        then the ephemerides path should be automatically picked up from
-        the `$LALPULSAR_DATADIR` environment variable.
-        Similarly, if you have installed lalsuite from conda-forge,
-        it should come with ephemerides included and properly set up.
-        
-        Alternatively, you can place a file
-        `~/.pyfstat.conf` into your home directory which looks like
+        PyFstat uses the following external python modules,
+        which should all be pulled in automatically if you use `pip`:
+        
+        * [corner](https://pypi.python.org/pypi/corner/)
+        * [dill](https://pypi.python.org/pypi/dill)
+        * [lalsuite](https://pypi.org/project/lalsuite/)
+        * [matplotlib](https://matplotlib.org/)
+        * [numpy](https://www.numpy.org/)
+        * [pathos](https://pypi.python.org/pypi/pathos)
+        * [ptemcee](https://github.com/willvousden/ptemcee)
+        * [scipy](https://www.scipy.org/)
+        * [tqdm](https://pypi.python.org/pypi/tqdm)
+        * [versioneer](https://pypi.org/project/versioneer/)
         
+        For a general introduction to installing modules, see
+        [here](https://docs.python.org/3/installing/index.html).
+        
+        NOTE: currently we have pinned to
+        `numpy<1.24.0` (due to an incompatibility with ptemcee).
+        
+        NOTE: We require a recent LALSuite (>=7.13) / lalpulsar (>=6.0).
+        If you need to work with older versions,
+        the last PyFstat release supporting those was `1.19.1`.
+        
+        ### Optional dependencies
+        
+        PyFstat manages optional dependencies through setuptool's `extras_require`.
+        
+        Available sets of optional dependencies are:
+        
+        * `chainconsumer` ([Samreay/Chainconsumer](https://github.com/Samreay/ChainConsumer)): Required to run some optional
+        plotting methods and some of the [example scripts](./examples).
+        * `dev`: Collects `docs`, `style`, `test` and `wheel`.
+        * `docs`: Required dependencies to build the documentation.
+        * `pycuda` ([PyPI](https://pypi.org/project/pycuda/)): Required for the `tCWFstatMapVersion=pycuda`
+          option of the `TransientGridSearch` class. (Note: Installing `pycuda` requires a working
+          `nvcc` compiler in your path.)
+        * `style`: Includes the `flake8` linter ([flake8.pycqa](https://flake8.pycqa.org/en/latest)),
+          `black` style checker ([black.readthedocs](https://black.readthedocs.io)),
+          and `isort` for import ordering ([pycqa.github.io](https://pycqa.github.io/isort/)).
+          These checks are required to pass by the online integration pipeline.
+        * `test`: For running the test suite locally using [pytest](https://docs.pytest.org) and some of its addons
+          (`python -m pytest tests/`).
+        * `wheel`: Includes `wheel` and `check-wheel-contents`.
+        
+        Installation can be done by adding one or more of the aforementioned tags to the installation command.
+        
+        For example, installing PyFstat including `chainconsumer`, `pycuda` and `style` dependencies would look like
+        (mind the lack of whitespaces!)
         ```
-        earth_ephem = '/home/<USER>/lalsuite-install/share/lalpulsar/earth00-19-DE405.dat.gz'
-        sun_ephem = '/home/<USER>/lalsuite-install/share/lalpulsar/sun00-19-DE405.dat.gz'
+        pip install pyfstat[chainconsumer,pycuda,style]
         ```
-        Paths set in this way will take precedence over the environment variable.
+        This command accepts the "development mode" tag `-e`.
         
-        Finally, you can manually specify ephemerides files when initialising
-        each PyFstat search (as one of the arguments).
+        Note that LALSuite is a default requirement, not an optional one,
+        but its installation from PyPI can be disabled
+        by setting the `NO_LALSUITE_FROM_PYPI` environment variable,
+        e.g. for a development install from a local git clone:
+        ```
+        NO_LALSUITE_FROM_PYPI=1 pip install -e .
+        ```
+        This can be useful to avoid duplication when in a conda environment
+        or installing LALSuite from source.
+        
+        ### Using LALSuite built from source
+        
+        Instructions to use a custom local LALSuite installation can be found in [here on the wiki](https://github.com/PyFstat/PyFstat/wiki/Using-LALSuite-built-from-source).
         
         ## Contributing to PyFstat
+        
         This project is open to development, please feel free to contact us
         for advice or just jump in and submit an
         [issue](https://github.com/PyFstat/PyFstat/issues/new/choose) or
         [pull request](https://github.com/PyFstat/PyFstat/compare).
         
         Here's what you need to know:
-        * The github automated tests currently run on `python` [3.6,3.7,3.8] and new PRs need to pass all these.
-        * The automated test also runs
-          the [black](https://black.readthedocs.io) style checker
-          and the [flake8](https://flake8.pycqa.org/en/latest/) linter.
-          If at all possible, please run these two tools locally before pushing changes / submitting PRs:
+        * As a developer, you should install directly from a git clone,
+          with either `pip install -e .[dev]` into some environment
+          or creating a development-enabled conda environment directly from the
+          `pyfstat-dev.yml` file
+          as explained on [this wiki page](https://github.com/PyFstat/PyFstat/wiki/conda-environments).
+          Please also run, just once after installing:
+          ```
+          pre-commit install
+          ```
+        
+          This sets up everything for automated code quality tests (see below)
+          to be checked for you at every commit.
+        * The github automated tests currently run on `python` [3.8,3.9,3.10,3.11]
+          and new PRs need to pass all these.
+        * You can also run the full test suite locally via `pytest tests/`,
+          or run individual tests as explained
+          [on this page](https://docs.pytest.org/en/6.2.x/usage.html#specifying-tests-selecting-tests).
+        * The automated test on github also runs
+          the [black](https://black.readthedocs.io) style checker,
+          the [flake8](https://flake8.pycqa.org/en/latest/) linter,
+          and the [isort](https://pycqa.github.io/isort/) import ordering helper.
+        * If you have installed the dev dependencies correctly via pip or conda,
+          and ran `pre-commit install` once,
+          then you're ready to let the `pre-commit` tool do all of this automatically for you
+          every time you do `git commit`.
+          For anything that would fail on the github integration tests,
+          it will then either automatically reformat your code to match our style
+          or print warnings for things to fix.
+          The first time it will take a while for setup,
+          later it should be faster.
+        * If for some reason you can't use `pre-commit`,
+          you can still manually run these tools before pushing changes / submitting PRs:
+          `isort .` to sort package imports,
           `flake8 --count --statistics .` to find common coding errors and then fix them manually,
-          and then
           `black --check --diff .` to show the required style changes, or `black .` to automatically apply them.
-        * `bin/setup-dev-tools.sh` gets your virtual environment ready for you. After making sure you are 
-        using a virtual environment (venv or conda),
-        it installs `black`, `flake8`, `pre-commit`, `pytest`, `wheel` via `pip` and uses `pre-commit` to run
-        the `black` and `flake8` using a pre-commit hook. In this way, you will be prompted a warning whenever you
-        forget to run `black` or `flake8` before doing your commit :wink:.
         
         ## Contributors
         
         Maintainers:
         * Greg Ashton
         * David Keitel
         
-        Other contributors:
+        Active contributors:
         * Reinhard Prix
         * Rodrigo Tenorio
+        
+        Other contributors:
         * Karl Wette
         * Sylvia Zhu
+        * Dan Foreman-Mackey (`pyfstat.gridcorner` is based on DFM's [corner.py](https://github.com/dfm/corner.py))
         
         
         ## Citing this work
         
-        If you use `PyFstat` in a publication we would appreciate if you cite both a DOI for the software itself (see below)
-        and the original paper introducing the code: Ashton&Prix 2018 [[inspire](https://inspirehep.net/literature/1655200)] [[ADS](https://ui.adsabs.harvard.edu/abs/2018PhRvD..97j3020A/)].
-        If you use the transient module, please also cite: Keitel&Ashton 2018 [[inspire](https://inspirehep.net/literature/1673205)] [[ADS](https://ui.adsabs.harvard.edu/abs/2018CQGra..35t5003K/)].
+        If you use `PyFstat` in a publication we would appreciate if you cite both a release DOI for the software itself (see below)
+        and one or more of the following scientific papers:
+        * The recent JOSS (Journal of Open Source Software) paper summarising the package:
+        [Keitel, Tenorio, Ashton & Prix 2021](https://doi.org/10.21105/joss.03000)
+        ([inspire:1842895](https://inspirehep.net/literature/1842895)
+        / [ADS:2021arXiv210110915K](https://ui.adsabs.harvard.edu/abs/2021arXiv210110915K/)).
+        * The original paper introducing the package and the MCMC functionality:
+        [Ashton&Prix 2018](https://doi.org/10.1103/PhysRevD.97.103020)
+        ([inspire:1655200](https://inspirehep.net/literature/1655200)
+        / [ADS:2018PhRvD..97j3020A](https://ui.adsabs.harvard.edu/abs/2018PhRvD..97j3020A/)).
+        * The methods paper introducing a Bayes factor to evaluate the multi-stage follow-up:
+        [Tenorio, Keitel, Sintes 2021](https://doi.org/10.1103/PhysRevD.104.084012)
+        ([inspire:1865975](https://inspirehep.net/literature/1865975)
+        / [ADS:2021PhRvD.104h4012T](https://ui.adsabs.harvard.edu/abs/2021PhRvD.104h4012T/))
+        * For transient searches:
+        [Keitel&Ashton 2018](https://doi.org/10.1088/1361-6382/aade34)
+        ([inspire:1673205](https://inspirehep.net/literature/1673205)
+        / [ADS:2018CQGra..35t5003K](https://ui.adsabs.harvard.edu/abs/2018CQGra..35t5003K/)).
+        * For glitch-robust searches:
+        [Ashton, Prix & Jones 2018](https://doi.org/10.1103/PhysRevD.98.063011)
+        ([inspire:1672396](https://inspirehep.net/literature/1672396)
+        / [ADS:2018PhRvD..98f3011A](https://ui.adsabs.harvard.edu/abs/2018PhRvD..98f3011A/)
         
-        If you'd like to cite the `PyFstat` package in general,
-        or versions from 1.5.x upwards,
+        If you'd additionally like to cite the `PyFstat` package in general,
         please refer to the [version-independent Zenodo listing](https://doi.org/10.5281/zenodo.3967045)
         or use directly the following BibTeX entry:
         ```
         @misc{pyfstat,
           author       = {Ashton, Gregory and
                           Keitel, David and
                           Prix, Reinhard
                           and Tenorio, Rodrigo},
-          title        = {PyFstat},
+          title        = {{PyFstat}},
           month        = jul,
           year         = 2020,
           publisher    = {Zenodo},
           doi          = {10.5281/zenodo.3967045},
           url          = {https://doi.org/10.5281/zenodo.3967045},
           note         = {\url{https://doi.org/10.5281/zenodo.3967045}}
         }
         ```
-        You can also obtain DOIs for individual versioned releases
+        You can also obtain DOIs for individual versioned releases (from 1.5.x upward)
         from the right sidebar at [Zenodo](https://doi.org/10.5281/zenodo.3967045).
         
         Alternatively, if you've used PyFstat up to version 1.4.x in your works,
-        the DOIs for those version can be found from the sidebar at
+        the DOIs for those versions can be found from the sidebar at
         [this older Zenodo record](https://doi.org/10.5281/zenodo.1243930)
         and please amend the BibTeX entry accordingly.
         
+        
+        PyFstat uses the [`ptemcee` sampler](https://github.com/willvousden/ptemcee), which can be
+        cited as
+        [Vousden, Far & Mandel 2015](https://doi.org/10.1093/mnras/stv2422)
+        ([ADS:2016MNRAS.455.1919V](https://ui.adsabs.harvard.edu/abs/2016MNRAS.455.1919V/abstract))
+        and [Foreman-Mackey, Hogg, Lang, and Goodman 2012](https://doi.org/10.1086/670067)
+        ([2013PASP..125..306F](https://ui.adsabs.harvard.edu/abs/2013PASP..125..306F/abstract)).
+        
+        PyFstat also makes generous use of functionality from the LALSuite library
+        and it will usually be appropriate to also cite that project
+        (see [this recommended bibtex entry](https://git.ligo.org/lscsoft/lalsuite/#acknowledgment))
+        and also [Wette 2020](https://doi.org/10.1016/j.softx.2020.100634)
+        ([inspire:1837108](https://inspirehep.net/literature/1837108)
+        / [ADS:2020SoftX..1200634W](https://ui.adsabs.harvard.edu/abs/2020SoftX..1200634W/))
+        for the C-to-python [SWIG](http://www.swig.org) bindings.
+        
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: chainconsumer
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: pycuda
+Provides-Extra: style
+Provides-Extra: test
+Provides-Extra: wheel
```

### Comparing `PyFstat-1.9.0/PyFstat.egg-info/SOURCES.txt` & `PyFstat-2.0.0/PyFstat.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,74 @@
-.gitattributes
-.gitignore
-.pre-commit-config.yaml
-.zenodo.json
 CHANGELOG.md
-Dockerfile
 LICENSE
 MANIFEST.in
 README.md
-requirements-dev.txt
-requirements.txt
 setup.cfg
 setup.py
-tests.py
 versioneer.py
-.github/workflows/docker-publish.yml
-.github/workflows/integration.yml
-.github/workflows/run_examples.yml
 PyFstat.egg-info/PKG-INFO
 PyFstat.egg-info/SOURCES.txt
 PyFstat.egg-info/dependency_links.txt
 PyFstat.egg-info/requires.txt
 PyFstat.egg-info/top_level.txt
-bin/check_if_virtual_environment.py
-bin/get-and-export-ephemeris.sh
-bin/setup-dev-tools.sh
 examples/run_all_examples.py
 examples/binary_examples/PyFstat_example_binary_mcmc_vs_grid_comparison.py
 examples/binary_examples/PyFstat_example_semi_coherent_binary_search_using_MCMC.py
 examples/followup_examples/PyFstat_example_semi_coherent_directed_follow_up.py
 examples/glitch_examples/PyFstat_example_glitch_robust_directed_MCMC_search_on_1_glitch.py
 examples/glitch_examples/PyFstat_example_glitch_robust_directed_grid_search_on_1_glitch.py
 examples/glitch_examples/PyFstat_example_make_data_for_search_on_1_glitch.py
 examples/glitch_examples/PyFstat_example_standard_directed_MCMC_search_on_1_glitch.py
 examples/grid_examples/PyFstat_example_grid_search_F0.py
 examples/grid_examples/PyFstat_example_grid_search_F0F1.py
 examples/grid_examples/PyFstat_example_grid_search_F0F1F2.py
+examples/grid_examples/PyFstat_example_grid_search_with_BSGL.py
 examples/mcmc_examples/PyFstat_example_MCMC_search_using_initialisation.py
 examples/mcmc_examples/PyFstat_example_fully_coherent_MCMC_search.py
+examples/mcmc_examples/PyFstat_example_fully_coherent_MCMC_search_with_BSGL.py
 examples/mcmc_examples/PyFstat_example_semi_coherent_MCMC_search.py
 examples/mcmc_vs_grid_simple_example/PyFstat_example_simple_mcmc_vs_grid_comparison.py
 examples/other_examples/PyFstat_example_InjectionParametersGenerator.py
 examples/other_examples/PyFstat_example_injecting_into_noise_sfts.py
-examples/other_examples/PyFstat_example_sliding_window.py
+examples/other_examples/PyFstat_example_spectrogram.py
 examples/other_examples/PyFstat_example_twoF_cumulative.py
 examples/transient_examples/PyFstat_example_long_transient_MCMC_search.py
 examples/transient_examples/PyFstat_example_make_data_for_long_transient_search.py
 examples/transient_examples/PyFstat_example_make_data_for_short_transient_search.py
 examples/transient_examples/PyFstat_example_short_transient_MCMC_search.py
 examples/transient_examples/PyFstat_example_short_transient_grid_search.py
+examples/tutorials/tutorial_utils.py
 pyfstat/__init__.py
 pyfstat/_version.py
 pyfstat/core.py
 pyfstat/grid_based_searches.py
-pyfstat/helper_functions.py
+pyfstat/gridcorner.py
+pyfstat/injection_parameters.py
+pyfstat/logging.py
 pyfstat/make_sfts.py
 pyfstat/mcmc_based_searches.py
 pyfstat/optimal_setup_functions.py
+pyfstat/snr.py
 pyfstat/tcw_fstat_map_funcs.py
 pyfstat/pyCUDAkernels/cudaTransientFstatExpWindow.cu
-pyfstat/pyCUDAkernels/cudaTransientFstatRectWindow.cu
+pyfstat/pyCUDAkernels/cudaTransientFstatRectWindow.cu
+pyfstat/utils/__init__.py
+pyfstat/utils/atoms.py
+pyfstat/utils/cli.py
+pyfstat/utils/converting.py
+pyfstat/utils/ephemeris.py
+pyfstat/utils/formatting.py
+pyfstat/utils/gsl.py
+pyfstat/utils/importing.py
+pyfstat/utils/io.py
+pyfstat/utils/predict.py
+pyfstat/utils/runlalsuite.py
+pyfstat/utils/sft.py
+tests/commons_for_tests.py
+tests/test_core.py
+tests/test_grid_based_searches.py
+tests/test_injection_parameters.py
+tests/test_logging.py
+tests/test_make_sfts.py
+tests/test_mcmc_based_searches.py
+tests/test_snr.py
+tests/test_tcw_fstat_map_funcs.py
```

### Comparing `PyFstat-1.9.0/README.md` & `PyFstat-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,118 @@
 # PyFstat
 
 This is a python package providing an interface to perform F-statistic based
-continuous gravitational wave (CW) searches.
+continuous gravitational wave (CW) searches,
+built on top of the [LALSuite library](https://doi.org/10.7935/GT1W-FZ16).
 
 Getting started:
 * This README provides information on
-installation,
-[contributing](#contributors) to 
+[installing](#installation),
+[contributing](#contributors) to
 and [citing](#citing-this-work) PyFstat.
-* Additional usage documentation will be added to the
-[project wiki](https://github.com/PyFstat/PyFstat/wiki) (work in progress).
-* We also have a number of
-[examples](https://github.com/PyFstat/PyFstat/tree/master/examples),
-demonstrating different use cases.
-* New contributors are encouraged to have a look into
-[how to set up a development environment](#contributing-to-pyfstat)
+* PyFstat usage and its API are documented at [pyfstat.readthedocs.io](https://pyfstat.readthedocs.io/).
+* We also have a number of [tutorials](https://github.com/PyFstat/PyFstat/tree/master/examples/tutorials) and
+[examples](https://github.com/PyFstat/PyFstat/tree/master/examples), demonstrating different use cases.
+You can run them locally, or online as jupyter notebooks with
+[binder](https://mybinder.org/v2/gh/PyFstat/PyFstat/master).
+* The [project wiki](https://github.com/PyFstat/PyFstat/wiki) is mainly used for developer information.
+* A [changelog](https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md)
+is also available.
+* PyFstat >=2.0.0 requires a recent LALSuite (>=7.13) / lalpulsar (>=6.0)
+including the [SFTv3 specification](https://dcc.ligo.org/T040164-v2/public).
+If you need to work with older versions, the last PyFstat release supporting those was `1.19.1`.
 
-
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967045.svg)](https://doi.org/10.5281/zenodo.3967045)
 [![PyPI version](https://badge.fury.io/py/PyFstat.svg)](https://badge.fury.io/py/PyFstat)
-![Integration Tests](https://github.com/PyFstat/PyFstat/workflows/Integration%20Tests/badge.svg)
-![Docker](https://github.com/PyFstat/PyFstat/workflows/Docker/badge.svg)
-
-A [changelog](https://github.com/PyFstat/PyFstat/blob/master/CHANGELOG.md)
-is also available (only maintained from v1.2 onwards).
+[![Conda version](https://anaconda.org/conda-forge/pyfstat/badges/version.svg)](https://anaconda.org/conda-forge/pyfstat)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967045.svg)](https://doi.org/10.5281/zenodo.3967045)
+[![ASCL](https://img.shields.io/badge/ascl-2102.027-blue.svg?colorB=262255)](https://ascl.net/2102.027)
+[![JOSS](https://joss.theoj.org/papers/10.21105/joss.03000/status.svg)](https://doi.org/10.21105/joss.03000)
+[![Docker](https://github.com/PyFstat/PyFstat/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/PyFstat/PyFstat/actions/workflows/docker-publish.yml)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PyFstat/PyFstat/master)
+[![Integration Tests](https://github.com/PyFstat/PyFstat/actions/workflows/integration.yml/badge.svg)](https://github.com/PyFstat/PyFstat/actions/workflows/integration.yml)
+[![codecov](https://codecov.io/gh/PyFstat/PyFstat/branch/master/graph/badge.svg?token=P0W8MIIUGD)](https://codecov.io/gh/PyFstat/PyFstat)
+[![Documentation Status](https://readthedocs.org/projects/pyfstat/badge/?version=latest)](https://pyfstat.readthedocs.io/en/latest/?badge=latest)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Installation
 
 PyFstat releases can be installed in a variety of ways, including
+[`pip install` from PyPI](#pip-install-from-PyPi),
+[conda](#conda-installation),
 [Docker/Singularity images](#docker-container),
-[`pip install` from PyPi](#pip-install-from-PyPi),
 and [from source releases on Zenodo](#install-pyfstat-from-source-zenodo-or-git-clone).
 Latest development versions can
 [also be installed with pip](#pip-install-from-github)
 or [from a local git clone](#install-pyfstat-from-source-zenodo-or-git-clone).
 
-If you don't have a recent `python` installation (`3.6+`) on your system or
-prefer `conda` environments over system-wide installation / venvs, please
-start with the [conda installation](#conda-installation) section.
+If you don't have a recent `python` installation (`3.8+`) on your system,
+then `Docker` or `conda` are the easiest paths.
 
 In either case, be sure to also check out the notes on
-[dependencies](#dependencies),
-[ephemerides files](#ephemerides-installation)
+[dependencies](#dependencies)
 and [citing this work](#citing-this-work).
 
-### Docker container
-Ready-to-use PyFstat containers are available at the [Packages](https://github.com/PyFstat/PyFstat/packages)
-page. A git-hub account together with a personal access token is required. [Go to the wiki page](https://github.com/PyFstat/PyFstat/wiki/Containers) to learn how to pull them from the git-hub
-registry using Docker or Singularity.
-
-### pip install from PyPi
+If you run into problems with ephemerides files, check the wiki page on
+[ephemerides installation](https://github.com/PyFstat/PyFstat/wiki/ephemerides-installation).
 
-PyPi releases are available from https://pypi.org/project/PyFstat/.
+### pip install from PyPI
 
-Note that the PyFstat installation will fail at the
-[LALSuite](https://pypi.org/project/lalsuite/) dependency stage
-if your `pip` is too old (e.g. 18.1); to be on the safe side, before starting do
-```
-pip install --upgrade pip
-```
+PyPI releases are available from https://pypi.org/project/PyFstat/.
 
-Then, a simple
+A simple
 ```
 pip install pyfstat
 ```
-should give you the latest release version with all dependencies.
+should give you the latest release version with all dependencies;
+recent releases now also include a sufficient minimal set of ephemerides files.
 
 If you are not installing into a [venv](https://docs.python.org/3/library/venv.html)
-or [conda environment](#conda-installation),
+or [conda environment](#conda-installation)
+(you really should!),
 on many systems you may need to use the `--user` flag.
 
+Note that the PyFstat installation will fail at the
+LALSuite dependency stage
+if your `pip` is too old (e.g. 18.1); to fix this, do
+```
+pip install --upgrade pip setuptools
+```
+
 ### conda installation
 
-`PyFstat` requires `python3.6+`.
-While many systems come with a system-wide python installation,
-it may not be sufficiently recent for this package;
-anyway, it can often be easier to manage a user-specific python installation
-(this way one does not require root access to install or remove modules).
-One method to do this is to use the `conda` system, either through
-the stripped down [`Miniconda`](https://conda.pydata.org/miniconda.html)
-installation, or the full-featured
-[`Anaconda`](https://www.anaconda.com/products/individual#Downloads)
-(these are essentially the
-same, but the `Anaconda` version installs a variety of useful packages such as
-`numpy` and `scipy` by default).
-The fastest/easiest method is to follow your OS instructions
-[here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/)
-which will install `Miniconda`.
-
-After you have installed a version of `conda` and
-[set up an environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), 
-`pip` can also be used to install modules into this environment.
-(There is no direct `conda` release of `PyFstat` at the moment.)
-This can be installed with
-```
-conda install pip
-```
-and then you can continue with the `pip` instructions,
-either [a release version from PyPi](#pip-install-from-PyPi)
-as described above
-or [the latest development version directly from github](#pip-install-from-github)
-as described below.
-
-A simple way to get started with an otherwise clean environment
-is to use a minimal .yml recipe file
-[as explained here](https://github.com/PyFstat/PyFstat/wiki/conda-environments).
-
-Alternatively, you may consider starting from an
-[`igwn` environment](https://computing.docs.ligo.org/conda/),
-which contains most packages relevant to gravitational waves,
-instead of doing it from scratch,
-and just adding `PyFstat` to it through pip as described above.
-But be advised that the downloads for the `igwn` environments are huge.
+See [this wiki page](https://github.com/PyFstat/PyFstat/wiki/conda-environments)
+for further instructions on installing conda itself,
+installing PyFstat into an existing environment,
+or for .yml recipes to set up a PyFstat-specific environment
+both for normal users and for developers.
+
+If getting PyFstat from conda-forge, it already includes the required ephemerides files.
+
+### Docker container
+
+Ready-to-use PyFstat containers are available at the [Packages](https://github.com/PyFstat/PyFstat/packages)
+page. A GitHub account together with a personal access token is required.
+[Go to the wiki page](https://github.com/PyFstat/PyFstat/wiki/Containers)
+to learn how to pull them from the GitHub registry using `Docker` or `Singularity`.
 
 ### pip install from github
 
 Development versions of PyFstat can also be easily installed by
 pointing pip directly to this git repository,
 which will give you the latest version of the master branch:
 ```
 pip install git+https://github.com/PyFstat/PyFstat
 ```
 or, if you have an ssh key installed in github:
 ```
 pip install git+ssh://git@github.com/PyFstat/PyFstat
 ```
 
-
-### Dependencies
-
-PyFstat uses the following external python modules,
-which should all be pulled in automatically if you use `pip`:
-
-* [numpy](https://www.numpy.org/)
-* [matplotlib](https://matplotlib.org/)
-* [scipy](https://www.scipy.org/)
-* [ptemcee](https://github.com/willvousden/ptemcee)
-* [corner](https://pypi.python.org/pypi/corner/)
-* [dill](https://pypi.python.org/pypi/dill)
-* [tqdm](https://pypi.python.org/pypi/tqdm)
-* [bashplotlib](https://github.com/glamp/bashplotlib)
-* [peakutils](https://pypi.python.org/pypi/PeakUtils)
-* [pathos](https://pypi.python.org/pypi/pathos)
-* [lalsuite](https://pypi.org/project/lalsuite/)
-* [versioneer](https://pypi.org/project/versioneer/)
-
-In case the automatic install doesn't properly pull in all dependencies,
-to install all of these modules manually, you can also run
-```
-pip install -r /PATH/TO/THIS/DIRECTORY/requirements.txt
-```
-For a general introduction to installing modules, see
-[here](https://docs.python.org/3/installing/index.html).
-
-*Optional dependencies*:
-* [pycuda](https://pypi.org/project/pycuda/),
-  required for the `tCWFstatMapVersion=pycuda`
-  option of the `TransientGridSearch` class.
-  (Note: `pip install pycuda` requires a working `nvcc` compiler in your path.)
-* [pytest](https://docs.pytest.org) for running the test suite locally
-  (`python -m pytest tests.py`)
-* Developers are also highly encouraged to use
-  the [flake8](https://flake8.pycqa.org/en/latest/) linter
-  and [black](https://black.readthedocs.io) style checker
-  locally,
-  as these checks are required to pass by the online integration pipeline.
-* Some optional plotting methods depend on two additional packages,
-  and some of the [examples](./examples) require these to run:
- [gridcorner](https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner) 
-  and [chainconsumer](https://github.com/Samreay/ChainConsumer);
-for `pip` users this is most conveniently installed by
-```
-pip install git+https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner
-pip install chainconsumer
-```
-* If you prefer to make your own LALSuite installation
-[from source](https://git.ligo.org/lscsoft/lalsuite/),
-make sure it is **swig-enabled** and contains at least the `lalpulsar` and `lalapps` packages.
-A minimal configuration line to use would be e.g.:
-```
-./configure --prefix=${HOME}/lalsuite-install --disable-all-lal --enable-lalpulsar --enable-lalapps --enable-swig
-```
-
+This should pull in all dependencies in the same way as installing from PyPI,
+and recent lalsuite dependencies will include ephemerides files too.
 
 ### install PyFstat from source (Zenodo or git clone)
 
 You can download a source release tarball from [Zenodo](https://doi.org/10.5281/zenodo.3967045)
 and extract to an arbitrary temporary directory.
 Alternatively, clone this repository:
 
@@ -214,122 +141,206 @@
 was successful, run
 ```
 python -c 'import pyfstat'
 ```
 if no error message is output, then you have installed `pyfstat`. Note that
 the module will be installed to whichever python executable you call it from.
 
-### Ephemerides installation
+This should pull in all dependencies in the same way as installing from PyPI,
+and recent lalsuite dependencies will include ephemerides files too.
 
-PyFstat requires paths to earth and sun ephemerides files
-in order to use the `lalpulsar.ComputeFstat` module and various `lalapps` tools.
+### Dependencies
 
-If you have done `pip install lalsuite`
-(or it got pulled in automatically as a dependency),
-you need to manually download at least these two files:
-*  [earth00-40-DE405.dat.gz](https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/earth00-40-DE405.dat.gz)
-*  [sun00-40-DE405.dat.gz](https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/sun00-40-DE405.dat.gz)
-
-(Other ephemerides versions exist, but these two files should be sufficient for most applications.)
-You then need to tell PyFstat where to find these files,
-by either setting an environment variable `$LALPULSAR_DATADIR`
-or by creating a `~/.pyfstat.conf` file as described further below.
-If you are working with a virtual environment,
-you should be able to get a full working ephemerides installation with these commands:
-```
-mkdir $VIRTUAL_ENV/share/lalpulsar
-wget https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/earth00-40-DE405.dat.gz -P $VIRTUAL_ENV/share/lalpulsar
-wget https://git.ligo.org/lscsoft/lalsuite/raw/master/lalpulsar/lib/sun00-40-DE405.dat.gz -P $VIRTUAL_ENV/share/lalpulsar
-echo 'export LALPULSAR_DATADIR=$VIRTUAL_ENV/share/lalpulsar' >> ${VIRTUAL_ENV}/bin/activate
-deactivate
-source path/to/venv/bin/activate
-```
-An executable version of this snippet is readily accessible by **sourcing** `bin/get-and-export-ephemeris.sh`. 
-Mind that this script does **not** include an `export` command anywhere, so you will have to source it every time
-in order to properly set `LALPULSAR_DATADIR` variable.
-
-If instead you have built and installed lalsuite from source,
-and set your path up properly through something like
-`source $MYLALPATH/etc/lalsuite-user-env.sh`,
-then the ephemerides path should be automatically picked up from
-the `$LALPULSAR_DATADIR` environment variable.
-Similarly, if you have installed lalsuite from conda-forge,
-it should come with ephemerides included and properly set up.
-
-Alternatively, you can place a file
-`~/.pyfstat.conf` into your home directory which looks like
+PyFstat uses the following external python modules,
+which should all be pulled in automatically if you use `pip`:
+
+* [corner](https://pypi.python.org/pypi/corner/)
+* [dill](https://pypi.python.org/pypi/dill)
+* [lalsuite](https://pypi.org/project/lalsuite/)
+* [matplotlib](https://matplotlib.org/)
+* [numpy](https://www.numpy.org/)
+* [pathos](https://pypi.python.org/pypi/pathos)
+* [ptemcee](https://github.com/willvousden/ptemcee)
+* [scipy](https://www.scipy.org/)
+* [tqdm](https://pypi.python.org/pypi/tqdm)
+* [versioneer](https://pypi.org/project/versioneer/)
 
+For a general introduction to installing modules, see
+[here](https://docs.python.org/3/installing/index.html).
+
+NOTE: currently we have pinned to
+`numpy<1.24.0` (due to an incompatibility with ptemcee).
+
+NOTE: We require a recent LALSuite (>=7.13) / lalpulsar (>=6.0).
+If you need to work with older versions,
+the last PyFstat release supporting those was `1.19.1`.
+
+### Optional dependencies
+
+PyFstat manages optional dependencies through setuptool's `extras_require`.
+
+Available sets of optional dependencies are:
+
+* `chainconsumer` ([Samreay/Chainconsumer](https://github.com/Samreay/ChainConsumer)): Required to run some optional
+plotting methods and some of the [example scripts](./examples).
+* `dev`: Collects `docs`, `style`, `test` and `wheel`.
+* `docs`: Required dependencies to build the documentation.
+* `pycuda` ([PyPI](https://pypi.org/project/pycuda/)): Required for the `tCWFstatMapVersion=pycuda`
+  option of the `TransientGridSearch` class. (Note: Installing `pycuda` requires a working
+  `nvcc` compiler in your path.)
+* `style`: Includes the `flake8` linter ([flake8.pycqa](https://flake8.pycqa.org/en/latest)),
+  `black` style checker ([black.readthedocs](https://black.readthedocs.io)),
+  and `isort` for import ordering ([pycqa.github.io](https://pycqa.github.io/isort/)).
+  These checks are required to pass by the online integration pipeline.
+* `test`: For running the test suite locally using [pytest](https://docs.pytest.org) and some of its addons
+  (`python -m pytest tests/`).
+* `wheel`: Includes `wheel` and `check-wheel-contents`.
+
+Installation can be done by adding one or more of the aforementioned tags to the installation command.
+
+For example, installing PyFstat including `chainconsumer`, `pycuda` and `style` dependencies would look like
+(mind the lack of whitespaces!)
 ```
-earth_ephem = '/home/<USER>/lalsuite-install/share/lalpulsar/earth00-19-DE405.dat.gz'
-sun_ephem = '/home/<USER>/lalsuite-install/share/lalpulsar/sun00-19-DE405.dat.gz'
+pip install pyfstat[chainconsumer,pycuda,style]
 ```
-Paths set in this way will take precedence over the environment variable.
+This command accepts the "development mode" tag `-e`.
 
-Finally, you can manually specify ephemerides files when initialising
-each PyFstat search (as one of the arguments).
+Note that LALSuite is a default requirement, not an optional one,
+but its installation from PyPI can be disabled
+by setting the `NO_LALSUITE_FROM_PYPI` environment variable,
+e.g. for a development install from a local git clone:
+```
+NO_LALSUITE_FROM_PYPI=1 pip install -e .
+```
+This can be useful to avoid duplication when in a conda environment
+or installing LALSuite from source.
+
+### Using LALSuite built from source
+
+Instructions to use a custom local LALSuite installation can be found in [here on the wiki](https://github.com/PyFstat/PyFstat/wiki/Using-LALSuite-built-from-source).
 
 ## Contributing to PyFstat
+
 This project is open to development, please feel free to contact us
 for advice or just jump in and submit an
 [issue](https://github.com/PyFstat/PyFstat/issues/new/choose) or
 [pull request](https://github.com/PyFstat/PyFstat/compare).
 
 Here's what you need to know:
-* The github automated tests currently run on `python` [3.6,3.7,3.8] and new PRs need to pass all these.
-* The automated test also runs
-  the [black](https://black.readthedocs.io) style checker
-  and the [flake8](https://flake8.pycqa.org/en/latest/) linter.
-  If at all possible, please run these two tools locally before pushing changes / submitting PRs:
+* As a developer, you should install directly from a git clone,
+  with either `pip install -e .[dev]` into some environment
+  or creating a development-enabled conda environment directly from the
+  `pyfstat-dev.yml` file
+  as explained on [this wiki page](https://github.com/PyFstat/PyFstat/wiki/conda-environments).
+  Please also run, just once after installing:
+  ```
+  pre-commit install
+  ```
+
+  This sets up everything for automated code quality tests (see below)
+  to be checked for you at every commit.
+* The github automated tests currently run on `python` [3.8,3.9,3.10,3.11]
+  and new PRs need to pass all these.
+* You can also run the full test suite locally via `pytest tests/`,
+  or run individual tests as explained
+  [on this page](https://docs.pytest.org/en/6.2.x/usage.html#specifying-tests-selecting-tests).
+* The automated test on github also runs
+  the [black](https://black.readthedocs.io) style checker,
+  the [flake8](https://flake8.pycqa.org/en/latest/) linter,
+  and the [isort](https://pycqa.github.io/isort/) import ordering helper.
+* If you have installed the dev dependencies correctly via pip or conda,
+  and ran `pre-commit install` once,
+  then you're ready to let the `pre-commit` tool do all of this automatically for you
+  every time you do `git commit`.
+  For anything that would fail on the github integration tests,
+  it will then either automatically reformat your code to match our style
+  or print warnings for things to fix.
+  The first time it will take a while for setup,
+  later it should be faster.
+* If for some reason you can't use `pre-commit`,
+  you can still manually run these tools before pushing changes / submitting PRs:
+  `isort .` to sort package imports,
   `flake8 --count --statistics .` to find common coding errors and then fix them manually,
-  and then
   `black --check --diff .` to show the required style changes, or `black .` to automatically apply them.
-* `bin/setup-dev-tools.sh` gets your virtual environment ready for you. After making sure you are 
-using a virtual environment (venv or conda),
-it installs `black`, `flake8`, `pre-commit`, `pytest`, `wheel` via `pip` and uses `pre-commit` to run
-the `black` and `flake8` using a pre-commit hook. In this way, you will be prompted a warning whenever you
-forget to run `black` or `flake8` before doing your commit :wink:.
 
 ## Contributors
 
 Maintainers:
 * Greg Ashton
 * David Keitel
 
-Other contributors:
+Active contributors:
 * Reinhard Prix
 * Rodrigo Tenorio
+
+Other contributors:
 * Karl Wette
 * Sylvia Zhu
+* Dan Foreman-Mackey (`pyfstat.gridcorner` is based on DFM's [corner.py](https://github.com/dfm/corner.py))
 
 
 ## Citing this work
 
-If you use `PyFstat` in a publication we would appreciate if you cite both a DOI for the software itself (see below)
-and the original paper introducing the code: Ashton&Prix 2018 [[inspire](https://inspirehep.net/literature/1655200)] [[ADS](https://ui.adsabs.harvard.edu/abs/2018PhRvD..97j3020A/)].
-If you use the transient module, please also cite: Keitel&Ashton 2018 [[inspire](https://inspirehep.net/literature/1673205)] [[ADS](https://ui.adsabs.harvard.edu/abs/2018CQGra..35t5003K/)].
+If you use `PyFstat` in a publication we would appreciate if you cite both a release DOI for the software itself (see below)
+and one or more of the following scientific papers:
+* The recent JOSS (Journal of Open Source Software) paper summarising the package:
+[Keitel, Tenorio, Ashton & Prix 2021](https://doi.org/10.21105/joss.03000)
+([inspire:1842895](https://inspirehep.net/literature/1842895)
+/ [ADS:2021arXiv210110915K](https://ui.adsabs.harvard.edu/abs/2021arXiv210110915K/)).
+* The original paper introducing the package and the MCMC functionality:
+[Ashton&Prix 2018](https://doi.org/10.1103/PhysRevD.97.103020)
+([inspire:1655200](https://inspirehep.net/literature/1655200)
+/ [ADS:2018PhRvD..97j3020A](https://ui.adsabs.harvard.edu/abs/2018PhRvD..97j3020A/)).
+* The methods paper introducing a Bayes factor to evaluate the multi-stage follow-up:
+[Tenorio, Keitel, Sintes 2021](https://doi.org/10.1103/PhysRevD.104.084012)
+([inspire:1865975](https://inspirehep.net/literature/1865975)
+/ [ADS:2021PhRvD.104h4012T](https://ui.adsabs.harvard.edu/abs/2021PhRvD.104h4012T/))
+* For transient searches:
+[Keitel&Ashton 2018](https://doi.org/10.1088/1361-6382/aade34)
+([inspire:1673205](https://inspirehep.net/literature/1673205)
+/ [ADS:2018CQGra..35t5003K](https://ui.adsabs.harvard.edu/abs/2018CQGra..35t5003K/)).
+* For glitch-robust searches:
+[Ashton, Prix & Jones 2018](https://doi.org/10.1103/PhysRevD.98.063011)
+([inspire:1672396](https://inspirehep.net/literature/1672396)
+/ [ADS:2018PhRvD..98f3011A](https://ui.adsabs.harvard.edu/abs/2018PhRvD..98f3011A/)
 
-If you'd like to cite the `PyFstat` package in general,
-or versions from 1.5.x upwards,
+If you'd additionally like to cite the `PyFstat` package in general,
 please refer to the [version-independent Zenodo listing](https://doi.org/10.5281/zenodo.3967045)
 or use directly the following BibTeX entry:
 ```
 @misc{pyfstat,
   author       = {Ashton, Gregory and
                   Keitel, David and
                   Prix, Reinhard
                   and Tenorio, Rodrigo},
-  title        = {PyFstat},
+  title        = {{PyFstat}},
   month        = jul,
   year         = 2020,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.3967045},
   url          = {https://doi.org/10.5281/zenodo.3967045},
   note         = {\url{https://doi.org/10.5281/zenodo.3967045}}
 }
 ```
-You can also obtain DOIs for individual versioned releases
+You can also obtain DOIs for individual versioned releases (from 1.5.x upward)
 from the right sidebar at [Zenodo](https://doi.org/10.5281/zenodo.3967045).
 
 Alternatively, if you've used PyFstat up to version 1.4.x in your works,
-the DOIs for those version can be found from the sidebar at
+the DOIs for those versions can be found from the sidebar at
 [this older Zenodo record](https://doi.org/10.5281/zenodo.1243930)
 and please amend the BibTeX entry accordingly.
+
+
+PyFstat uses the [`ptemcee` sampler](https://github.com/willvousden/ptemcee), which can be
+cited as
+[Vousden, Far & Mandel 2015](https://doi.org/10.1093/mnras/stv2422)
+([ADS:2016MNRAS.455.1919V](https://ui.adsabs.harvard.edu/abs/2016MNRAS.455.1919V/abstract))
+and [Foreman-Mackey, Hogg, Lang, and Goodman 2012](https://doi.org/10.1086/670067)
+([2013PASP..125..306F](https://ui.adsabs.harvard.edu/abs/2013PASP..125..306F/abstract)).
+
+PyFstat also makes generous use of functionality from the LALSuite library
+and it will usually be appropriate to also cite that project
+(see [this recommended bibtex entry](https://git.ligo.org/lscsoft/lalsuite/#acknowledgment))
+and also [Wette 2020](https://doi.org/10.1016/j.softx.2020.100634)
+([inspire:1837108](https://inspirehep.net/literature/1837108)
+/ [ADS:2020SoftX..1200634W](https://ui.adsabs.harvard.edu/abs/2020SoftX..1200634W/))
+for the C-to-python [SWIG](http://www.swig.org) bindings.
```

### Comparing `PyFstat-1.9.0/examples/binary_examples/PyFstat_example_binary_mcmc_vs_grid_comparison.py` & `PyFstat-2.0.0/examples/binary_examples/PyFstat_example_binary_mcmc_vs_grid_comparison.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,31 @@
-#!/usr/bin/env python
+"""
+Binary CW example: Comparison between MCMC and grid search
+==========================================================
+
+Comparison of the semicoherent F-statistic MCMC search algorithm
+to a simple grid search accross the parameter space corresponding
+to a CW source in a binary system.
+"""
 
-import pyfstat
 import os
-import numpy as np
+
 import matplotlib.pyplot as plt
+import numpy as np
+
+import pyfstat
 
 # Set to false to include eccentricity
 circular_orbit = False
 
-label = os.path.splitext(os.path.basename(__file__))[0] + (
-    "_circular_orbit" if circular_orbit else ""
+label = "PyFstatExampleBinaryMCMCvsGridComparison" + (
+    "CircularOrbit" if circular_orbit else ""
 )
 outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 # Parameters to generate a data set
 data_parameters = {
     "sqrtSX": 1e-22,
     "tstart": 1000000000,
     "duration": 90 * 86400,
     "detectors": "H1,L1",
@@ -40,25 +50,25 @@
     "argp": 0.0 if circular_orbit else 0.54,
     "ecc": 0.0 if circular_orbit else 0.7,
     "h0": data_parameters["sqrtSX"] / depth,
     "cosi": 1.0,
 }
 
 
-print("Generating SFTs with injected signal...")
+logger.info("Generating SFTs with injected signal...")
 writer = pyfstat.BinaryModulatedWriter(
-    label="simulated_signal",
+    label=label + "SimulatedSignal",
     outdir=outdir,
     **data_parameters,
     **signal_parameters,
 )
 writer.make_data()
-print("")
+logger.info("")
 
-print("Performing Grid Search...")
+logger.info("Performing Grid Search...")
 
 # Create ad-hoc grid and compute Fstatistic around injection point
 # There's no class supporting a binary search in the same way as
 # grid_based_searches.GridSearch, so we do it by hand constructing
 # a grid and using core.ComputeFstat.
 half_points_per_dimension = 2
 search_keys = ["period", "asini", "tp", "argp", "ecc"]
@@ -82,53 +92,51 @@
     ]
 )
 grid_points = np.hstack(
     [grid_arrays[i].reshape(-1, 1) for i in range(len(grid_arrays))]
 )
 
 compute_f_stat = pyfstat.ComputeFstat(
-    sftfilepattern=os.path.join(outdir, "*simulated_signal*sft"),
+    sftfilepattern=writer.sftfilepath,
     tref=signal_parameters["tref"],
     binary=True,
     minCoverFreq=-0.5,
     maxCoverFreq=-0.5,
 )
 twoF_values = np.zeros(grid_points.shape[0])
 for ind in range(grid_points.shape[0]):
     point = grid_points[ind]
     twoF_values[ind] = compute_f_stat.get_fullycoherent_twoF(
-        tstart=data_parameters["tstart"],
-        tend=tend,
         F0=signal_parameters["F0"],
         F1=signal_parameters["F1"],
         F2=signal_parameters["F2"],
         Alpha=signal_parameters["Alpha"],
         Delta=signal_parameters["Delta"],
         period=point[0],
         asini=point[1],
         tp=point[2],
         argp=point[3],
         ecc=point[4],
     )
-print(f"2Fstat computed on {grid_points.shape[0]} points")
-print("")
-print("Plotting results...")
+logger.info(f"2Fstat computed on {grid_points.shape[0]} points")
+logger.info("")
+logger.info("Plotting results...")
 dim = len(search_keys)
 fig, ax = plt.subplots(dim, 1, figsize=(10, 10))
 for ind in range(dim):
     a = ax.ravel()[ind]
     a.grid()
     a.set(xlabel=search_keys_label[ind], ylabel=r"$2 \mathcal{F}$", yscale="log")
     a.plot(grid_points[:, ind], twoF_values, "o")
     a.axvline(signal_parameters[search_keys[ind]], label="Injection", color="orange")
 plt.tight_layout()
 fig.savefig(os.path.join(outdir, "grid_twoF_per_dimension.png"))
 
 
-print("Performing MCMCSearch...")
+logger.info("Performing MCMCSearch...")
 # Fixed points in frequency and sky parameters
 theta_prior = {
     "F0": signal_parameters["F0"],
     "F1": signal_parameters["F1"],
     "F2": signal_parameters["F2"],
     "Alpha": signal_parameters["Alpha"],
     "Delta": signal_parameters["Delta"],
@@ -153,17 +161,17 @@
 # ptemcee sampler settings - in a real application we might want higher values
 ntemps = 2
 log10beta_min = -1
 nwalkers = 100
 nsteps = [100, 100]  # [burnin,production]
 
 mcmcsearch = pyfstat.MCMCSearch(
-    label="mcmc_search",
+    label=label + "MCMCSearch",
     outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*simulated_signal*sft"),
+    sftfilepattern=writer.sftfilepath,
     theta_prior=theta_prior,
     tref=signal_parameters["tref"],
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
     log10beta_min=log10beta_min,
     binary=True,
@@ -173,33 +181,33 @@
     plot_walkers=True,
     walker_plot_args={"plot_det_stat": True, "injection_parameters": signal_parameters},
 )
 mcmcsearch.print_summary()
 
 # call some built-in plotting methods
 # these can all highlight the injection parameters, too
-print("Making MCMCSearch {:s} corner plot...".format("-".join(search_keys)))
+logger.info("Making MCMCSearch {:s} corner plot...".format("-".join(search_keys)))
 mcmcsearch.plot_corner(truths=signal_parameters)
-print("Making MCMCSearch prior-posterior comparison plot...")
+logger.info("Making MCMCSearch prior-posterior comparison plot...")
 mcmcsearch.plot_prior_posterior(injection_parameters=signal_parameters)
-print("")
+logger.info("")
 
-print("*" * 20)
-print("Quantitative comparisons:")
-print("*" * 20)
+logger.info("*" * 20)
+logger.info("Quantitative comparisons:")
+logger.info("*" * 20)
 
 # some informative command-line output comparing search results and injection
 # get max twoF and binary Doppler parameters
 max_grid_index = np.argmax(twoF_values)
 max_grid_2F = twoF_values[max_grid_index]
 max_grid_parameters = grid_points[max_grid_index]
 
 # same for MCMCSearch, here twoF is separate, and non-sampled parameters are not included either
 max_dict_mcmc, max_2F_mcmc = mcmcsearch.get_max_twoF()
-print(
+logger.info(
     "Grid Search:\n\tmax2F={:.4f}\n\tOffsets from injection parameters (relative error): {:s}.".format(
         max_grid_2F,
         ", ".join(
             [
                 "\n\t\t{1:s}: {0:.4e} ({2:.4f}%)".format(
                     max_grid_parameters[search_keys.index(key)]
                     - signal_parameters[key],
@@ -212,15 +220,15 @@
                     / signal_parameters[key],
                 )
                 for key in search_keys
             ]
         ),
     )
 )
-print(
+logger.info(
     "Max 2F candidate from MCMC Search:\n\tmax2F={:.4f}"
     "\n\tOffsets from injection parameters (relative error): {:s}.".format(
         max_2F_mcmc,
         ", ".join(
             [
                 "\n\t\t{1:s}: {0:.4e} ({2:.4f}%)".format(
                     max_dict_mcmc[key] - signal_parameters[key],
@@ -232,15 +240,15 @@
                 for key in search_keys
             ]
         ),
     )
 )
 # get additional point and interval estimators
 stats_dict_mcmc = mcmcsearch.get_summary_stats()
-print(
+logger.info(
     "Mean from MCMCSearch:\n\tOffset from injection parameters (relative error): {:s}"
     "\n\tExpressed as fractions of 2sigma intervals: {:s}.".format(
         ", ".join(
             [
                 "\n\t\t{1:s}: {0:.4e} ({2:.4f}%)".format(
                     stats_dict_mcmc[key]["mean"] - signal_parameters[key],
                     key,
@@ -260,15 +268,15 @@
                     key,
                 )
                 for key in search_keys
             ]
         ),
     )
 )
-print(
+logger.info(
     "Median from MCMCSearch:\n\tOffset from injection parameters (relative error): {:s},"
     "\n\tExpressed as fractions of 90% confidence intervals: {:s}.".format(
         ", ".join(
             [
                 "\n\t\t{1:s}: {0:.4e} ({2:.4f}%)".format(
                     stats_dict_mcmc[key]["median"] - signal_parameters[key],
                     key,
```

### Comparing `PyFstat-1.9.0/examples/binary_examples/PyFstat_example_semi_coherent_binary_search_using_MCMC.py` & `PyFstat-2.0.0/examples/binary_examples/PyFstat_example_semi_coherent_binary_search_using_MCMC.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-import pyfstat
-import numpy as np
+"""
+Binary CW example: Semicoherent MCMC search
+==========================================================
+
+MCMC search of a CW signal produced by a source in a binary
+system using the semicoherent F-statistic.
+"""
+
 import os
 
+import numpy as np
+
+import pyfstat
+
 # If False, sky priors are used
 directed_search = True
 # If False, ecc and argp priors are used
 known_eccentricity = True
 
-label = os.path.splitext(os.path.basename(__file__))[0]
+label = "PyFstatExampleSemiCoherentBinarySearchUsingMCMC"
 outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 # Properties of the GW data
 data_parameters = {
     "sqrtSX": 1e-23,
     "tstart": 1000000000,
     "duration": 10 * 86400,
     "detectors": "H1",
@@ -108,15 +119,15 @@
 nwalkers = 150
 nsteps = [100, 200]
 
 mcmc = pyfstat.MCMCSemiCoherentSearch(
     label=label,
     outdir=outdir,
     nsegs=10,
-    sftfilepattern=os.path.join(outdir, "*{}*sft".format(label)),
+    sftfilepattern=data.sftfilepath,
     theta_prior=theta_prior,
     tref=signal_parameters["tref"],
     minStartTime=data_parameters["tstart"],
     maxStartTime=tend,
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
```

### Comparing `PyFstat-1.9.0/examples/followup_examples/PyFstat_example_semi_coherent_directed_follow_up.py` & `PyFstat-2.0.0/examples/followup_examples/PyFstat_example_semi_coherent_directed_follow_up.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,24 @@
-import pyfstat
-import numpy as np
-import matplotlib.pyplot as plt
+"""
+Follow up example
+=================
+
+Multi-stage MCMC follow up of a CW signal produced by an isolated
+source using a ladder of coherent times.
+"""
 import os
 
-label = os.path.splitext(os.path.basename(__file__))[0]
+import matplotlib.pyplot as plt
+import numpy as np
+
+import pyfstat
+
+label = "PyFstatExampleSemiCoherentDirectedFollowup"
 outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 # Properties of the GW data
 data_parameters = {
     "sqrtSX": 1e-23,
     "tstart": 1000000000,
     "duration": 100 * 86400,
     "detectors": "H1",
@@ -30,17 +40,17 @@
 }
 
 data = pyfstat.Writer(
     label=label, outdir=outdir, **data_parameters, **signal_parameters
 )
 data.make_data()
 
-# The predicted twoF, given by lalapps_predictFstat can be accessed by
+# The predicted twoF (expectation over noise realizations) can be accessed by
 twoF = data.predict_fstat()
-print("Predicted twoF value: {}\n".format(twoF))
+logger.info("Predicted twoF value: {}\n".format(twoF))
 
 # Search
 VF0 = VF1 = 1e5
 DeltaF0 = np.sqrt(VF0) * np.sqrt(3) / (np.pi * data_parameters["duration"])
 DeltaF1 = np.sqrt(VF1) * np.sqrt(180) / (np.pi * data_parameters["duration"] ** 2)
 theta_prior = {
     "F0": {
@@ -62,15 +72,15 @@
 log10beta_min = -0.5
 nwalkers = 100
 nsteps = [100, 100]
 
 mcmc = pyfstat.MCMCFollowUpSearch(
     label=label,
     outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*{}*sft".format(label)),
+    sftfilepattern=data.sftfilepath,
     theta_prior=theta_prior,
     tref=mid_time,
     minStartTime=data_parameters["tstart"],
     maxStartTime=tend,
     nwalkers=nwalkers,
     nsteps=nsteps,
     ntemps=ntemps,
```

### Comparing `PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_MCMC_search_on_1_glitch.py` & `PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_MCMC_search_on_1_glitch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-import numpy as np
-import pyfstat
-import gridcorner
+"""
+Glitch robust MCMC search
+=========================
+
+MCMC search employing a signal hypothesis allowing for a glitch to
+be present in the data. The setup corresponds to a targeted search,
+and the simulated signal contains a single glitch.
+"""
+
+import os
 import time
+
+import numpy as np
 from PyFstat_example_make_data_for_search_on_1_glitch import (
-    tstart,
-    duration,
-    tref,
     F0,
     F1,
     F2,
     Alpha,
     Delta,
     delta_F0,
     dtglitch,
+    duration,
     outdir,
+    tref,
+    tstart,
 )
-import os
 
-label = "semicoherent_glitch_robust_directed_MCMC_search_on_1_glitch"
+import pyfstat
+
+label = "PyFstatExampleGlitchRobustDirectedMCMCSearchOn1Glitch"
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 Nstar = 1000
 F0_width = np.sqrt(Nstar) * np.sqrt(12) / (np.pi * duration)
-F1_width = np.sqrt(Nstar) * np.sqrt(180) / (np.pi * duration ** 2)
+F1_width = np.sqrt(Nstar) * np.sqrt(180) / (np.pi * duration**2)
 
 theta_prior = {
     "F0": {"type": "unif", "lower": F0 - F0_width / 2.0, "upper": F0 + F0_width / 2.0},
     "F1": {"type": "unif", "lower": F1 - F1_width / 2.0, "upper": F1 + F1_width / 2.0},
     "F2": F2,
     "delta_F0": {"type": "unif", "lower": 0, "upper": 1e-5},
     "delta_F1": 0,
@@ -42,15 +53,15 @@
 log10beta_min = -0.5
 nwalkers = 100
 nsteps = [250, 250]
 
 mcmc = pyfstat.MCMCGlitchSearch(
     label=label,
     outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*1_glitch*sft"),
+    sftfilepattern=os.path.join(outdir, "*1glitch*sft"),
     theta_prior=theta_prior,
     tref=tref,
     minStartTime=tstart,
     maxStartTime=tstart + duration,
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
@@ -75,21 +86,20 @@
 ] = "$t^\\mathrm{g}-t^\\mathrm{g}_\\mathrm{s}$\n[d]"
 
 t1 = time.time()
 mcmc.run(save_loudest=False)  # uses CFSv2 which doesn't support glitch parameters
 dT = time.time() - t1
 mcmc.print_summary()
 
-fig_and_axes = gridcorner._get_fig_and_axes(4, 2, 0.05)
+logger.info("Making corner plot...")
 mcmc.plot_corner(
     label_offset=0.25,
     truths={"F0": F0, "F1": F1, "delta_F0": delta_F0, "tglitch": tstart + dtglitch},
-    fig_and_axes=fig_and_axes,
-    quantiles=(0.16, 0.84),
+    quantiles=(0.16, 0.5, 0.84),
     hist_kwargs=dict(lw=1.5, zorder=-1),
     truth_color="C3",
 )
 
-mcmc.plot_cumulative_max()
+mcmc.plot_cumulative_max(savefig=True)
 
-print(("Prior widths =", F0_width, F1_width))
-print(("Actual run time = {}".format(dT)))
+logger.info(f"Prior widths = {F0_width}, {F1_width}")
+logger.info(f"Actual run time = {dT} s")
```

### Comparing `PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_grid_search_on_1_glitch.py` & `PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_glitch_robust_directed_grid_search_on_1_glitch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-import pyfstat
+"""
+Glitch robust grid search
+=========================
+
+Grid search employing a signal hypothesis allowing for a glitch to
+be present in the data. The setup corresponds to a targeted search,
+and the simulated signal contains a single glitch.
+"""
+
+import os
+import time
+
 import numpy as np
 from PyFstat_example_make_data_for_search_on_1_glitch import (
-    tstart,
-    duration,
-    tref,
     F0,
     F1,
     F2,
     Alpha,
     Delta,
     delta_F0,
-    outdir,
     dtglitch,
+    duration,
+    outdir,
+    tref,
+    tstart,
 )
-import time
-import os
 
-try:
-    from gridcorner import gridcorner
-except ImportError:
-    raise ImportError(
-        "Python module 'gridcorner' not found, please install from "
-        "https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner"
-    )
+import pyfstat
 
-label = "semicoherent_glitch_robust_directed_grid_search_on_1_glitch"
+label = "PyFstatExampleGlitchRobustDirectedGridSearchOn1Glitch"
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 Nstar = 1000
 F0_width = np.sqrt(Nstar) * np.sqrt(12) / (np.pi * duration)
-F1_width = np.sqrt(Nstar) * np.sqrt(180) / (np.pi * duration ** 2)
+F1_width = np.sqrt(Nstar) * np.sqrt(180) / (np.pi * duration**2)
 N = 20
 F0s = [F0 - F0_width / 2.0, F0 + F0_width / 2.0, F0_width / N]
 F1s = [F1 - F1_width / 2.0, F1 + F1_width / 2.0, F1_width / N]
 F2s = [F2]
 Alphas = [Alpha]
 Deltas = [Delta]
 
@@ -42,15 +46,15 @@
 delta_F1s = [0]
 
 
 t1 = time.time()
 search = pyfstat.GridGlitchSearch(
     label,
     outdir,
-    os.path.join(outdir, "*1_glitch*sft"),
+    os.path.join(outdir, "*1glitch*sft"),
     F0s=F0s,
     F1s=F1s,
     F2s=F2s,
     Alphas=Alphas,
     Deltas=Deltas,
     tref=tref,
     minStartTime=tstart,
@@ -58,41 +62,42 @@
     tglitchs=tglitchs,
     delta_F0s=delta_F0s,
     delta_F1s=delta_F1s,
 )
 search.run()
 dT = time.time() - t1
 
-F0_vals = np.unique(search.data[:, 0]) - F0
-F1_vals = np.unique(search.data[:, 1]) - F1
-delta_F0s_vals = np.unique(search.data[:, 5]) - delta_F0
-tglitch_vals = np.unique(search.data[:, 7])
+F0_vals = np.unique(search.data["F0"]) - F0
+F1_vals = np.unique(search.data["F1"]) - F1
+delta_F0s_vals = np.unique(search.data["delta_F0"]) - delta_F0
+tglitch_vals = np.unique(search.data["tglitch"])
 tglitch_vals_days = (tglitch_vals - tstart) / 86400.0 - dtglitch / 86400.0
 
-twoF = search.data[:, -1].reshape(
+logger.info("Making gridcorner plot...")
+twoF = search.data["twoF"].reshape(
     (len(F0_vals), len(F1_vals), len(delta_F0s_vals), len(tglitch_vals))
 )
 xyz = [F0_vals * 1e6, F1_vals * 1e12, delta_F0s_vals * 1e6, tglitch_vals_days]
 labels = [
     "$f - f_\\mathrm{s}$\n[$\\mu$Hz]",
     "$\\dot{f} - \\dot{f}_\\mathrm{s}$\n[$p$Hz/s]",
     "$\\delta f-\\delta f_\\mathrm{s}$\n[$\\mu$Hz]",
     "$t^\\mathrm{g} - t^\\mathrm{g}_\\mathrm{s}$\n[d]",
     "$t^\\mathrm{g} - t^\\mathrm{g}_\\mathrm{s}$\n[d]",
     "$\\widehat{2\\mathcal{F}}$",
 ]
-fig, axes = gridcorner(
+fig, axes = pyfstat.gridcorner(
     twoF,
     xyz,
     projection="log_mean",
     labels=labels,
     showDvals=False,
     lines=[0, 0, 0, 0],
     label_offset=0.25,
     max_n_ticks=4,
 )
 fig.savefig("{}/{}_projection_matrix.png".format(outdir, label), bbox_inches="tight")
 
 
-print(("Prior widths =", F0_width, F1_width))
-print(("Actual run time = {}".format(dT)))
-print(("Actual number of grid points = {}".format(search.data.shape[0])))
+logger.info(f"Prior widths = {F0_width}, {F1_width}")
+logger.info(f"Actual run time = {dT} s")
+logger.info(f"Actual number of grid points = {search.data.shape[0]}")
```

### Comparing `PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_make_data_for_search_on_1_glitch.py` & `PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_make_data_for_search_on_1_glitch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,22 @@
-from pyfstat import Writer, GlitchWriter
-import numpy as np
+"""
+Glitch examples: Make data
+==========================
+
+Generate the data to run examples on glitch-robust searches.
+"""
+
 import os
 
-outdir = os.path.join("PyFstat_example_data", "PyFstat_example_glitch_robust_search")
+import numpy as np
+
+from pyfstat import GlitchWriter, Writer
+
+label = "PyFstatExampleGlitchRobustSearch"
+outdir = os.path.join("PyFstat_example_data", label)
 
 # First, we generate data with a reasonably strong smooth signal
 
 # Define parameters of the Crab pulsar as an example
 F0 = 30.0
 F1 = -1e-10
 F2 = 0
@@ -22,15 +32,15 @@
 tstart = 1000000000
 duration = 50 * 86400
 tend = tstart + duration
 tref = tstart + 0.5 * duration
 IFO = "H1"
 
 data = Writer(
-    label="0_glitch",
+    label=label + "0glitch",
     outdir=outdir,
     tref=tref,
     tstart=tstart,
     F0=F0,
     F1=F1,
     F2=F2,
     duration=duration,
@@ -45,15 +55,15 @@
 
 # Next, taking the same signal parameters, we include a glitch half way through
 dtglitch = duration / 2.0
 delta_F0 = 5e-6
 delta_F1 = 0
 
 glitch_data = GlitchWriter(
-    label="1_glitch",
+    label=label + "1glitch",
     outdir=outdir,
     tref=tref,
     tstart=tstart,
     F0=F0,
     F1=F1,
     F2=F2,
     duration=duration,
@@ -74,15 +84,15 @@
 dtglitch_2 = [duration / 4.0, 4 * duration / 5.0]
 delta_phi_2 = [0, 0]
 delta_F0_2 = [4e-6, 3e-7]
 delta_F1_2 = [0, 0]
 delta_F2_2 = [0, 0]
 
 two_glitch_data = GlitchWriter(
-    label="2_glitch",
+    label=label + "2glitch",
     outdir=outdir,
     tref=tref,
     tstart=tstart,
     F0=F0,
     F1=F1,
     F2=F2,
     duration=duration,
```

### Comparing `PyFstat-1.9.0/examples/glitch_examples/PyFstat_example_standard_directed_MCMC_search_on_1_glitch.py` & `PyFstat-2.0.0/examples/glitch_examples/PyFstat_example_standard_directed_MCMC_search_on_1_glitch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,39 @@
+"""
+MCMC search on data presenting a glitch
+=======================================
+
+Executes a directed MCMC semicoherent F-statistic search on data
+presenting a glitch. This is intended to show the impact of
+glitches on vanilla CW searches.
+"""
+
+import os
+
 import numpy as np
-import pyfstat
 from PyFstat_example_make_data_for_search_on_1_glitch import (
-    tstart,
-    duration,
-    tref,
     F0,
     F1,
     F2,
     Alpha,
     Delta,
+    duration,
     outdir,
+    tref,
+    tstart,
 )
-import os
 
-label = "standard_directed_MCMC_search_on_1_glitch"
+import pyfstat
+
+label = "PyFstatExampleStandardDirectedMCMCSearchOn1Glitch"
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 Nstar = 10000
 F0_width = np.sqrt(Nstar) * np.sqrt(12) / (np.pi * duration)
-F1_width = np.sqrt(Nstar) * np.sqrt(180) / (np.pi * duration ** 2)
+F1_width = np.sqrt(Nstar) * np.sqrt(180) / (np.pi * duration**2)
 
 theta_prior = {
     "F0": {"type": "unif", "lower": F0 - F0_width / 2.0, "upper": F0 + F0_width / 2.0},
     "F1": {"type": "unif", "lower": F1 - F1_width / 2.0, "upper": F1 + F1_width / 2.0},
     "F2": F2,
     "Alpha": Alpha,
     "Delta": Delta,
@@ -31,15 +43,15 @@
 log10beta_min = -0.5
 nwalkers = 100
 nsteps = [500, 2000]
 
 mcmc = pyfstat.MCMCSearch(
     label=label,
     outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*1_glitch*sft"),
+    sftfilepattern=os.path.join(outdir, "*1glitch*sft"),
     theta_prior=theta_prior,
     tref=tref,
     minStartTime=tstart,
     maxStartTime=tstart + duration,
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
@@ -50,8 +62,8 @@
 mcmc.transform_dictionary["F1"] = dict(
     subtractor=F1, symbol="$\\dot{f}-\\dot{f}^\\mathrm{s}$"
 )
 
 mcmc.run()
 mcmc.print_summary()
 mcmc.plot_corner()
-mcmc.plot_cumulative_max()
+mcmc.plot_cumulative_max(savefig=True)
```

### Comparing `PyFstat-1.9.0/examples/mcmc_examples/PyFstat_example_MCMC_search_using_initialisation.py` & `PyFstat-2.0.0/examples/mcmc_examples/PyFstat_example_MCMC_search_using_initialisation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,24 @@
-import pyfstat
-import numpy as np
+"""
+MCMC search: Semicoherent F-statistic with initialisation
+=========================================================
+
+Directed MCMC search for an isolated CW signal using the
+fully-coherent F-statistic. Prior to the burn-in stage, walkers
+are initialized with a certain scattering factor.
+"""
 import os
 
-label = os.path.splitext(os.path.basename(__file__))[0]
+import numpy as np
+
+import pyfstat
+
+label = "PyFstatExampleMCMCSearchUsingInitialisation"
 outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 # Properties of the GW data
 data_parameters = {
     "sqrtSX": 1e-23,
     "tstart": 1000000000,
     "duration": 100 * 86400,
     "detectors": "H1",
@@ -29,23 +40,23 @@
 }
 
 data = pyfstat.Writer(
     label=label, outdir=outdir, **data_parameters, **signal_parameters
 )
 data.make_data()
 
-# The predicted twoF, given by lalapps_predictFstat can be accessed by
+# The predicted twoF (expectation over noise realizations) can be accessed by
 twoF = data.predict_fstat()
-print("Predicted twoF value: {}\n".format(twoF))
+logger.info("Predicted twoF value: {}\n".format(twoF))
 
 DeltaF0 = 1e-7
 DeltaF1 = 1e-13
 VF0 = (np.pi * data_parameters["duration"] * DeltaF0) ** 2 / 3.0
 VF1 = (np.pi * data_parameters["duration"] ** 2 * DeltaF1) ** 2 * 4 / 45.0
-print("\nV={:1.2e}, VF0={:1.2e}, VF1={:1.2e}\n".format(VF0 * VF1, VF0, VF1))
+logger.info("\nV={:1.2e}, VF0={:1.2e}, VF1={:1.2e}\n".format(VF0 * VF1, VF0, VF1))
 
 theta_prior = {
     "F0": {
         "type": "unif",
         "lower": signal_parameters["F0"] - DeltaF0 / 2.0,
         "upper": signal_parameters["F0"] + DeltaF0 / 2.0,
     },
@@ -62,15 +73,15 @@
 log10beta_min = -1
 nwalkers = 100
 nsteps = [100, 100]
 
 mcmc = pyfstat.MCMCSearch(
     label=label,
     outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*{}*sft".format(label)),
+    sftfilepattern=data.sftfilepath,
     theta_prior=theta_prior,
     tref=mid_time,
     minStartTime=data_parameters["tstart"],
     maxStartTime=tend,
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
```

### Comparing `PyFstat-1.9.0/examples/mcmc_examples/PyFstat_example_fully_coherent_MCMC_search.py` & `PyFstat-2.0.0/examples/mcmc_examples/PyFstat_example_fully_coherent_MCMC_search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,25 @@
-import pyfstat
-import numpy as np
+"""
+MCMC search: Fully coherent F-statistic
+=======================================
+
+Directed MCMC search for an isolated CW signal using the
+fully coherent F-statistic.
+"""
+
 import os
 
-label = os.path.splitext(os.path.basename(__file__))[0]
+import numpy as np
+
+import pyfstat
+from pyfstat.utils import get_predict_fstat_parameters_from_dict
+
+label = "PyFstatExampleFullyCoherentMCMCSearch"
 outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 # Properties of the GW data
 data_parameters = {
     "sqrtSX": 1e-23,
     "tstart": 1000000000,
     "duration": 100 * 86400,
     "detectors": "H1",
@@ -29,23 +41,23 @@
 }
 
 data = pyfstat.Writer(
     label=label, outdir=outdir, **data_parameters, **signal_parameters
 )
 data.make_data()
 
-# The predicted twoF, given by lalapps_predictFstat can be accessed by
+# The predicted twoF (expectation over noise realizations) can be accessed by
 twoF = data.predict_fstat()
-print("Predicted twoF value: {}\n".format(twoF))
+logger.info("Predicted twoF value: {}\n".format(twoF))
 
 DeltaF0 = 1e-7
 DeltaF1 = 1e-13
 VF0 = (np.pi * data_parameters["duration"] * DeltaF0) ** 2 / 3.0
 VF1 = (np.pi * data_parameters["duration"] ** 2 * DeltaF1) ** 2 * 4 / 45.0
-print("\nV={:1.2e}, VF0={:1.2e}, VF1={:1.2e}\n".format(VF0 * VF1, VF0, VF1))
+logger.info("\nV={:1.2e}, VF0={:1.2e}, VF1={:1.2e}\n".format(VF0 * VF1, VF0, VF1))
 
 theta_prior = {
     "F0": {
         "type": "unif",
         "lower": signal_parameters["F0"] - DeltaF0 / 2.0,
         "upper": signal_parameters["F0"] + DeltaF0 / 2.0,
     },
@@ -62,15 +74,15 @@
 log10beta_min = -0.5
 nwalkers = 100
 nsteps = [300, 300]
 
 mcmc = pyfstat.MCMCSearch(
     label=label,
     outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*{}*sft".format(label)),
+    sftfilepattern=data.sftfilepath,
     theta_prior=theta_prior,
     tref=mid_time,
     minStartTime=data_parameters["tstart"],
     maxStartTime=tend,
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
@@ -84,7 +96,20 @@
 )
 mcmc.run(
     walker_plot_args={"plot_det_stat": True, "injection_parameters": signal_parameters}
 )
 mcmc.print_summary()
 mcmc.plot_corner(add_prior=True, truths=signal_parameters)
 mcmc.plot_prior_posterior(injection_parameters=signal_parameters)
+
+mcmc.generate_loudest()
+
+# plot cumulative 2F, first building a dict as required for PredictFStat
+d, maxtwoF = mcmc.get_max_twoF()
+for key, val in mcmc.theta_prior.items():
+    if key not in d:
+        d[key] = val
+d["h0"] = data.h0
+d["cosi"] = data.cosi
+d["psi"] = data.psi
+PFS_input = get_predict_fstat_parameters_from_dict(d)
+mcmc.plot_cumulative_max(PFS_input=PFS_input)
```

### Comparing `PyFstat-1.9.0/examples/mcmc_examples/PyFstat_example_semi_coherent_MCMC_search.py` & `PyFstat-2.0.0/examples/mcmc_examples/PyFstat_example_semi_coherent_MCMC_search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-import pyfstat
-import numpy as np
+"""
+MCMC search: Semicoherent F-statistic
+=======================================
+
+Directed MCMC search for an isolated CW signal using the
+semicoherent F-statistic.
+"""
 import os
 
-label = os.path.splitext(os.path.basename(__file__))[0]
+import numpy as np
+
+import pyfstat
+
+label = "PyFstatExampleSemiCoherentMCMCSearch"
 outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 # Properties of the GW data
 data_parameters = {
     "sqrtSX": 1e-23,
     "tstart": 1000000000,
     "duration": 100 * 86400,
     "detectors": "H1",
@@ -29,23 +39,23 @@
 }
 
 data = pyfstat.Writer(
     label=label, outdir=outdir, **data_parameters, **signal_parameters
 )
 data.make_data()
 
-# The predicted twoF, given by lalapps_predictFstat can be accessed by
+# The predicted twoF (expectation over noise realizations) can be accessed by
 twoF = data.predict_fstat()
-print("Predicted twoF value: {}\n".format(twoF))
+logger.info("Predicted twoF value: {}\n".format(twoF))
 
 DeltaF0 = 1e-7
 DeltaF1 = 1e-13
 VF0 = (np.pi * data_parameters["duration"] * DeltaF0) ** 2 / 3.0
 VF1 = (np.pi * data_parameters["duration"] ** 2 * DeltaF1) ** 2 * 4 / 45.0
-print("\nV={:1.2e}, VF0={:1.2e}, VF1={:1.2e}\n".format(VF0 * VF1, VF0, VF1))
+logger.info("\nV={:1.2e}, VF0={:1.2e}, VF1={:1.2e}\n".format(VF0 * VF1, VF0, VF1))
 
 theta_prior = {
     "F0": {
         "type": "unif",
         "lower": signal_parameters["F0"] - DeltaF0 / 2.0,
         "upper": signal_parameters["F0"] + DeltaF0 / 2.0,
     },
@@ -63,15 +73,15 @@
 nwalkers = 100
 nsteps = [300, 300]
 
 mcmc = pyfstat.MCMCSemiCoherentSearch(
     label=label,
     outdir=outdir,
     nsegs=10,
-    sftfilepattern=os.path.join(outdir, "*{}*sft".format(label)),
+    sftfilepattern=data.sftfilepath,
     theta_prior=theta_prior,
     tref=mid_time,
     minStartTime=data_parameters["tstart"],
     maxStartTime=tend,
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
```

### Comparing `PyFstat-1.9.0/examples/mcmc_vs_grid_simple_example/PyFstat_example_simple_mcmc_vs_grid_comparison.py` & `PyFstat-2.0.0/examples/mcmc_vs_grid_simple_example/PyFstat_example_simple_mcmc_vs_grid_comparison.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-#!/usr/bin/env python
+"""
+MCMC search v.s. grid search
+============================
+
+An example to compare MCMCSearch and GridSearch on the same data.
+"""
 
-import pyfstat
 import os
-import numpy as np
+
 import matplotlib.pyplot as plt
+import numpy as np
 
-try:
-    from gridcorner import gridcorner
-except ImportError:
-    raise ImportError(
-        "Python module 'gridcorner' not found, please install from "
-        "https://gitlab.aei.uni-hannover.de/GregAshton/gridcorner"
-    )
+import pyfstat
 
 # flip this switch for a more expensive 4D (F0,F1,Alpha,Delta) run
 # instead of just (F0,F1)
 # (still only a few minutes on current laptops)
 sky = False
 
-outdir = os.path.join(
-    "PyFstat_example_data", "PyFstat_example_simple_mcmc_vs_grid_F0F1"
-)
+label = "PyFstatExampleSimpleMCMCvsGridComparison"
+outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 if sky:
     outdir += "AlphaDelta"
 
 # parameters for the data set to generate
 tstart = 1000000000
 duration = 30 * 86400
 Tsft = 1800
@@ -39,278 +38,27 @@
     "F2": 0,
     "Alpha": 0.5,
     "Delta": 1,
     "h0": 0.05 * sqrtSX,
     "cosi": 1.0,
 }
 
-# latex-formated plotting labels
+# latex-formatted plotting labels
 labels = {
     "F0": "$f$ [Hz]",
     "F1": "$\\dot{f}$ [Hz/s]",
     "2F": "$2\\mathcal{F}$",
     "Alpha": "$\\alpha$",
     "Delta": "$\\delta$",
 }
 labels["max2F"] = "$\\max\\,$" + labels["2F"]
 
-print("Generating SFTs with injected signal...")
-writer = pyfstat.Writer(
-    label="simulated_signal",
-    outdir=outdir,
-    tstart=tstart,
-    duration=duration,
-    detectors=detectors,
-    sqrtSX=sqrtSX,
-    Tsft=Tsft,
-    **inj,
-    Band=1,  # default band estimation would be too narrow for a wide grid/prior
-)
-writer.make_data()
-print("")
-
-
-# set up square search grid with fixed (F0,F1) mismatch
-# and (optionally) some ad-hoc sky coverage
-m = 0.001
-dF0 = np.sqrt(12 * m) / (np.pi * duration)
-dF1 = np.sqrt(180 * m) / (np.pi * duration ** 2)
-DeltaF0 = 500 * dF0
-DeltaF1 = 200 * dF1
-if sky:
-    # cover less range to keep runtime down
-    DeltaF0 /= 10
-    DeltaF1 /= 10
-F0s = [inj["F0"] - DeltaF0 / 2.0, inj["F0"] + DeltaF0 / 2.0, dF0]
-F1s = [inj["F1"] - DeltaF1 / 2.0, inj["F1"] + DeltaF1 / 2.0, dF1]
-F2s = [inj["F2"]]
-search_keys = ["F0", "F1"]  # only the ones that aren't 0-width
-if sky:
-    dSky = 0.01  # rather coarse to keep runtime down
-    DeltaSky = 10 * dSky
-    Alphas = [inj["Alpha"] - DeltaSky / 2.0, inj["Alpha"] + DeltaSky / 2.0, dSky]
-    Deltas = [inj["Delta"] - DeltaSky / 2.0, inj["Delta"] + DeltaSky / 2.0, dSky]
-    search_keys += ["Alpha", "Delta"]
-else:
-    Alphas = [inj["Alpha"]]
-    Deltas = [inj["Delta"]]
-search_keys_label = "".join(search_keys)
-
-print("Performing GridSearch...")
-gridsearch = pyfstat.GridSearch(
-    label="grid_search_" + search_keys_label,
-    outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*simulated_signal*sft"),
-    F0s=F0s,
-    F1s=F1s,
-    F2s=F2s,
-    Alphas=Alphas,
-    Deltas=Deltas,
-    tref=inj["tref"],
-    BSGL=False,
-)
-gridsearch.run()
-gridsearch.print_max_twoF()
-gridsearch.save_array_to_disk(gridsearch.data)
-
-# do some plots of the GridSearch results
-if not sky:  # this plotter can't currently deal with too large result arrays
-    print("Plotting 1D 2F distributions...")
-    for key in search_keys:
-        gridsearch.plot_1D(xkey=key, xlabel=labels[key], ylabel=labels["2F"])
-
-print("Making GridSearch {:s} corner plot...".format("-".join(search_keys)))
-vals = [
-    np.unique(gridsearch.data[:, gridsearch.keys.index(key)]) - inj[key]
-    for key in search_keys
-]
-twoF = gridsearch.data[:, -1].reshape([len(kval) for kval in vals])
-corner_labels = [
-    "$f - f_0$ [Hz]",
-    "$\\dot{f} - \\dot{f}_0$ [Hz/s]",
-]
-if sky:
-    corner_labels.append("$\\alpha - \\alpha_0$")
-    corner_labels.append("$\\delta - \\delta_0$")
-corner_labels.append(labels["2F"])
-gridcorner_fig, gridcorner_axes = gridcorner(
-    twoF, vals, projection="log_mean", labels=corner_labels, whspace=0.1, factor=1.8
-)
-gridcorner_fig.savefig(os.path.join(outdir, gridsearch.label + "_corner.png"))
-plt.close(gridcorner_fig)
-print("")
-
-
-print("Performing MCMCSearch...")
-# set up priors in F0 and F1 (over)covering the grid ranges
-if sky:  # MCMC will still be fast in 4D with wider range than grid
-    DeltaF0 *= 50
-    DeltaF1 *= 50
-theta_prior = {
-    "F0": {
-        "type": "unif",
-        "lower": inj["F0"] - DeltaF0 / 2.0,
-        "upper": inj["F0"] + DeltaF0 / 2.0,
-    },
-    "F1": {
-        "type": "unif",
-        "lower": inj["F1"] - DeltaF1 / 2.0,
-        "upper": inj["F1"] + DeltaF1 / 2.0,
-    },
-    "F2": inj["F2"],
-}
-if sky:
-    # also implicitly covering twice the grid range here
-    theta_prior["Alpha"] = {
-        "type": "unif",
-        "lower": inj["Alpha"] - DeltaSky,
-        "upper": inj["Alpha"] + DeltaSky,
-    }
-    theta_prior["Delta"] = {
-        "type": "unif",
-        "lower": inj["Delta"] - DeltaSky,
-        "upper": inj["Delta"] + DeltaSky,
-    }
-else:
-    theta_prior["Alpha"] = inj["Alpha"]
-    theta_prior["Delta"] = inj["Delta"]
-# ptemcee sampler settings - in a real application we might want higher values
-ntemps = 2
-log10beta_min = -1
-nwalkers = 100
-nsteps = [200, 200]  # [burnin,production]
-
-mcmcsearch = pyfstat.MCMCSearch(
-    label="mcmc_search_" + search_keys_label,
-    outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*simulated_signal*sft"),
-    theta_prior=theta_prior,
-    tref=inj["tref"],
-    nsteps=nsteps,
-    nwalkers=nwalkers,
-    ntemps=ntemps,
-    log10beta_min=log10beta_min,
-)
-# walker plot is generated during main run of the search class
-mcmcsearch.run(walker_plot_args={"plot_det_stat": True, "injection_parameters": inj})
-mcmcsearch.print_summary()
-
-# call some built-in plotting methods
-# these can all highlight the injection parameters, too
-print("Making MCMCSearch {:s} corner plot...".format("-".join(search_keys)))
-mcmcsearch.plot_corner(truths=inj)
-print("Making MCMCSearch prior-posterior comparison plot...")
-mcmcsearch.plot_prior_posterior(injection_parameters=inj)
-print("")
-
-
-# NOTE: everything below here is just custom commandline output and plotting
-# for this particular example, which uses the PyFstat outputs,
-# but isn't very instructive if you just want to learn the main usage of the package.
-
-
-# some informative command-line output comparing search results and injection
-# get max of GridSearch, contains twoF and all Doppler parameters in the dict
-max_dict_grid = gridsearch.get_max_twoF()
-# same for MCMCSearch, here twoF is separate, and non-sampled parameters are not included either
-max_dict_mcmc, max_2F_mcmc = mcmcsearch.get_max_twoF()
-print(
-    "max2F={:.4f} from GridSearch, offsets from injection: {:s}.".format(
-        max_dict_grid["twoF"],
-        ", ".join(
-            [
-                "{:.4e} in {:s}".format(max_dict_grid[key] - inj[key], key)
-                for key in search_keys
-            ]
-        ),
-    )
-)
-print(
-    "max2F={:.4f} from MCMCSearch, offsets from injection: {:s}.".format(
-        max_2F_mcmc,
-        ", ".join(
-            [
-                "{:.4e} in {:s}".format(max_dict_mcmc[key] - inj[key], key)
-                for key in search_keys
-            ]
-        ),
-    )
-)
-# get additional point and interval estimators
-stats_dict_mcmc = mcmcsearch.get_summary_stats()
-print(
-    "mean   from MCMCSearch: offset from injection by      {:s},"
-    " or in fractions of 2sigma intervals: {:s}.".format(
-        ", ".join(
-            [
-                "{:.4e} in {:s}".format(stats_dict_mcmc[key]["mean"] - inj[key], key)
-                for key in search_keys
-            ]
-        ),
-        ", ".join(
-            [
-                "{:.2f}% in {:s}".format(
-                    100
-                    * np.abs(stats_dict_mcmc[key]["mean"] - inj[key])
-                    / (2 * stats_dict_mcmc[key]["std"]),
-                    key,
-                )
-                for key in search_keys
-            ]
-        ),
-    )
-)
-print(
-    "median from MCMCSearch: offset from injection by      {:s},"
-    " or in fractions of 90% confidence intervals: {:s}.".format(
-        ", ".join(
-            [
-                "{:.4e} in {:s}".format(stats_dict_mcmc[key]["median"] - inj[key], key)
-                for key in search_keys
-            ]
-        ),
-        ", ".join(
-            [
-                "{:.2f}% in {:s}".format(
-                    100
-                    * np.abs(stats_dict_mcmc[key]["median"] - inj[key])
-                    / (
-                        stats_dict_mcmc[key]["upper90"]
-                        - stats_dict_mcmc[key]["lower90"]
-                    ),
-                    key,
-                )
-                for key in search_keys
-            ]
-        ),
-    )
-)
-print()
-
-# do additional custom plotting
-print("Loading grid and MCMC search results for custom comparison plots...")
-gridfile = os.path.join(outdir, gridsearch.label + "_NA_GridSearch.txt")
-if not os.path.isfile(gridfile):
-    raise RuntimeError("Please first run PyFstat_example_simple_grid_search.py !")
-grid_res = pyfstat.helper_functions.read_txt_file_with_header(gridfile)
-mcmc_file = os.path.join(outdir, mcmcsearch.label + "_samples.dat")
-if not os.path.isfile(mcmc_file):
-    raise RuntimeError("Please first run PyFstat_example_simple_mcmc_search.py !")
-mcmc_res = pyfstat.helper_functions.read_txt_file_with_header(mcmc_file)
-
-zoom = {
-    "F0": [inj["F0"] - 10 * dF0, inj["F0"] + 10 * dF0],
-    "F1": [inj["F1"] - 5 * dF1, inj["F1"] + 5 * dF1],
-}
-
-# we'll use two local plotting functions to avoid code duplication in the sky case
-print("Creating MCMC-grid comparison plots...")
-
 
 def plot_grid_vs_samples(grid_res, mcmc_res, xkey, ykey):
+    """local plotting function to avoid code duplication in the 4D case"""
     plt.plot(grid_res[xkey], grid_res[ykey], ".", label="grid")
     plt.plot(mcmc_res[xkey], mcmc_res[ykey], ".", label="mcmc")
     plt.plot(inj[xkey], inj[ykey], "*k", label="injection")
     grid_maxidx = np.argmax(grid_res["twoF"])
     mcmc_maxidx = np.argmax(mcmc_res["twoF"])
     plt.plot(
         grid_res[xkey][grid_maxidx],
@@ -333,14 +81,15 @@
         plt.xlim(zoom[xkey])
         plt.ylim(zoom[ykey])
         plt.savefig(plotfilename_base + "_zoom.png")
     plt.close()
 
 
 def plot_2F_scatter(res, label, xkey, ykey):
+    """local plotting function to avoid code duplication in the 4D case"""
     markersize = 3 if label == "grid" else 1
     sc = plt.scatter(res[xkey], res[ykey], c=res["twoF"], s=markersize)
     cb = plt.colorbar(sc)
     plt.xlabel(labels[xkey])
     plt.ylabel(labels[ykey])
     cb.set_label(labels["2F"])
     plt.title(label)
@@ -358,15 +107,267 @@
     )
     plt.xlim([min(res[xkey]), max(res[xkey])])
     plt.ylim([min(res[ykey]), max(res[ykey])])
     plt.savefig(plotfilename_base + ".png")
     plt.close()
 
 
-# do the actual comparison plots
-plot_grid_vs_samples(grid_res, mcmc_res, "F0", "F1")
-plot_2F_scatter(grid_res, "grid", "F0", "F1")
-plot_2F_scatter(mcmc_res, "mcmc", "F0", "F1")
-if sky:
-    plot_grid_vs_samples(grid_res, mcmc_res, "Alpha", "Delta")
-    plot_2F_scatter(grid_res, "grid", "Alpha", "Delta")
-    plot_2F_scatter(mcmc_res, "mcmc", "Alpha", "Delta")
+if __name__ == "__main__":
+    logger.info("Generating SFTs with injected signal...")
+    writer = pyfstat.Writer(
+        label=label + "SimulatedSignal",
+        outdir=outdir,
+        tstart=tstart,
+        duration=duration,
+        detectors=detectors,
+        sqrtSX=sqrtSX,
+        Tsft=Tsft,
+        **inj,
+        Band=1,  # default band estimation would be too narrow for a wide grid/prior
+    )
+    writer.make_data()
+
+    # set up square search grid with fixed (F0,F1) mismatch
+    # and (optionally) some ad-hoc sky coverage
+    m = 0.001
+    dF0 = np.sqrt(12 * m) / (np.pi * duration)
+    dF1 = np.sqrt(180 * m) / (np.pi * duration**2)
+    DeltaF0 = 500 * dF0
+    DeltaF1 = 200 * dF1
+    if sky:
+        # cover less range to keep runtime down
+        DeltaF0 /= 10
+        DeltaF1 /= 10
+    F0s = [inj["F0"] - DeltaF0 / 2.0, inj["F0"] + DeltaF0 / 2.0, dF0]
+    F1s = [inj["F1"] - DeltaF1 / 2.0, inj["F1"] + DeltaF1 / 2.0, dF1]
+    F2s = [inj["F2"]]
+    search_keys = ["F0", "F1"]  # only the ones that aren't 0-width
+    if sky:
+        dSky = 0.01  # rather coarse to keep runtime down
+        DeltaSky = 10 * dSky
+        Alphas = [inj["Alpha"] - DeltaSky / 2.0, inj["Alpha"] + DeltaSky / 2.0, dSky]
+        Deltas = [inj["Delta"] - DeltaSky / 2.0, inj["Delta"] + DeltaSky / 2.0, dSky]
+        search_keys += ["Alpha", "Delta"]
+    else:
+        Alphas = [inj["Alpha"]]
+        Deltas = [inj["Delta"]]
+    search_keys_label = "".join(search_keys)
+
+    logger.info("Performing GridSearch...")
+    gridsearch = pyfstat.GridSearch(
+        label="GridSearch" + search_keys_label,
+        outdir=outdir,
+        sftfilepattern=writer.sftfilepath,
+        F0s=F0s,
+        F1s=F1s,
+        F2s=F2s,
+        Alphas=Alphas,
+        Deltas=Deltas,
+        tref=inj["tref"],
+    )
+    gridsearch.run()
+    gridsearch.print_max_twoF()
+    gridsearch.generate_loudest()
+
+    # do some plots of the GridSearch results
+    if not sky:  # this plotter can't currently deal with too large result arrays
+        logger.info("Plotting 1D 2F distributions...")
+        for key in search_keys:
+            gridsearch.plot_1D(xkey=key, xlabel=labels[key], ylabel=labels["2F"])
+
+    logger.info("Making GridSearch {:s} corner plot...".format("-".join(search_keys)))
+    vals = [np.unique(gridsearch.data[key]) - inj[key] for key in search_keys]
+    twoF = gridsearch.data["twoF"].reshape([len(kval) for kval in vals])
+    corner_labels = [
+        "$f - f_0$ [Hz]",
+        "$\\dot{f} - \\dot{f}_0$ [Hz/s]",
+    ]
+    if sky:
+        corner_labels.append("$\\alpha - \\alpha_0$")
+        corner_labels.append("$\\delta - \\delta_0$")
+    corner_labels.append(labels["2F"])
+    gridcorner_fig, gridcorner_axes = pyfstat.gridcorner(
+        twoF, vals, projection="log_mean", labels=corner_labels, whspace=0.1, factor=1.8
+    )
+    gridcorner_fig.savefig(os.path.join(outdir, gridsearch.label + "_corner.png"))
+    plt.close(gridcorner_fig)
+
+    logger.info("Performing MCMCSearch...")
+    # set up priors in F0 and F1 (over)covering the grid ranges
+    if sky:  # MCMC will still be fast in 4D with wider range than grid
+        DeltaF0 *= 50
+        DeltaF1 *= 50
+    theta_prior = {
+        "F0": {
+            "type": "unif",
+            "lower": inj["F0"] - DeltaF0 / 2.0,
+            "upper": inj["F0"] + DeltaF0 / 2.0,
+        },
+        "F1": {
+            "type": "unif",
+            "lower": inj["F1"] - DeltaF1 / 2.0,
+            "upper": inj["F1"] + DeltaF1 / 2.0,
+        },
+        "F2": inj["F2"],
+    }
+    if sky:
+        # also implicitly covering twice the grid range here
+        theta_prior["Alpha"] = {
+            "type": "unif",
+            "lower": inj["Alpha"] - DeltaSky,
+            "upper": inj["Alpha"] + DeltaSky,
+        }
+        theta_prior["Delta"] = {
+            "type": "unif",
+            "lower": inj["Delta"] - DeltaSky,
+            "upper": inj["Delta"] + DeltaSky,
+        }
+    else:
+        theta_prior["Alpha"] = inj["Alpha"]
+        theta_prior["Delta"] = inj["Delta"]
+    # ptemcee sampler settings - in a real application we might want higher values
+    ntemps = 2
+    log10beta_min = -1
+    nwalkers = 100
+    nsteps = [200, 200]  # [burnin,production]
+
+    mcmcsearch = pyfstat.MCMCSearch(
+        label="MCMCSearch" + search_keys_label,
+        outdir=outdir,
+        sftfilepattern=writer.sftfilepath,
+        theta_prior=theta_prior,
+        tref=inj["tref"],
+        nsteps=nsteps,
+        nwalkers=nwalkers,
+        ntemps=ntemps,
+        log10beta_min=log10beta_min,
+    )
+    # walker plot is generated during main run of the search class
+    mcmcsearch.run(
+        walker_plot_args={"plot_det_stat": True, "injection_parameters": inj}
+    )
+    mcmcsearch.print_summary()
+
+    # call some built-in plotting methods
+    # these can all highlight the injection parameters, too
+    logger.info("Making MCMCSearch {:s} corner plot...".format("-".join(search_keys)))
+    mcmcsearch.plot_corner(truths=inj)
+    logger.info("Making MCMCSearch prior-posterior comparison plot...")
+    mcmcsearch.plot_prior_posterior(injection_parameters=inj)
+
+    # NOTE: everything below here is just custom commandline output and plotting
+    # for this particular example, which uses the PyFstat outputs,
+    # but isn't very instructive if you just want to learn the main usage of the package.
+
+    # some informative command-line output comparing search results and injection
+    # get max of GridSearch, contains twoF and all Doppler parameters in the dict
+    max_dict_grid = gridsearch.get_max_twoF()
+    # same for MCMCSearch, here twoF is separate, and non-sampled parameters are not included either
+    max_dict_mcmc, max_2F_mcmc = mcmcsearch.get_max_twoF()
+    logger.info(
+        "max2F={:.4f} from GridSearch, offsets from injection: {:s}.".format(
+            max_dict_grid["twoF"],
+            ", ".join(
+                [
+                    "{:.4e} in {:s}".format(max_dict_grid[key] - inj[key], key)
+                    for key in search_keys
+                ]
+            ),
+        )
+    )
+    logger.info(
+        "max2F={:.4f} from MCMCSearch, offsets from injection: {:s}.".format(
+            max_2F_mcmc,
+            ", ".join(
+                [
+                    "{:.4e} in {:s}".format(max_dict_mcmc[key] - inj[key], key)
+                    for key in search_keys
+                ]
+            ),
+        )
+    )
+    # get additional point and interval estimators
+    stats_dict_mcmc = mcmcsearch.get_summary_stats()
+    logger.info(
+        "mean   from MCMCSearch: offset from injection by      {:s},"
+        " or in fractions of 2sigma intervals: {:s}.".format(
+            ", ".join(
+                [
+                    "{:.4e} in {:s}".format(
+                        stats_dict_mcmc[key]["mean"] - inj[key], key
+                    )
+                    for key in search_keys
+                ]
+            ),
+            ", ".join(
+                [
+                    "{:.2f}% in {:s}".format(
+                        100
+                        * np.abs(stats_dict_mcmc[key]["mean"] - inj[key])
+                        / (2 * stats_dict_mcmc[key]["std"]),
+                        key,
+                    )
+                    for key in search_keys
+                ]
+            ),
+        )
+    )
+    logger.info(
+        "median from MCMCSearch: offset from injection by      {:s},"
+        " or in fractions of 90% confidence intervals: {:s}.".format(
+            ", ".join(
+                [
+                    "{:.4e} in {:s}".format(
+                        stats_dict_mcmc[key]["median"] - inj[key], key
+                    )
+                    for key in search_keys
+                ]
+            ),
+            ", ".join(
+                [
+                    "{:.2f}% in {:s}".format(
+                        100
+                        * np.abs(stats_dict_mcmc[key]["median"] - inj[key])
+                        / (
+                            stats_dict_mcmc[key]["upper90"]
+                            - stats_dict_mcmc[key]["lower90"]
+                        ),
+                        key,
+                    )
+                    for key in search_keys
+                ]
+            ),
+        )
+    )
+
+    # do additional custom plotting
+    logger.info("Loading grid and MCMC search results for custom comparison plots...")
+    gridfile = os.path.join(outdir, gridsearch.label + "_NA_GridSearch.txt")
+    if not os.path.isfile(gridfile):
+        raise RuntimeError(
+            "Failed to load GridSearch results from file '{:s}',"
+            " something must have gone wrong!".format(gridfile)
+        )
+    grid_res = pyfstat.utils.read_txt_file_with_header(gridfile)
+    mcmc_file = os.path.join(outdir, mcmcsearch.label + "_samples.dat")
+    if not os.path.isfile(mcmc_file):
+        raise RuntimeError(
+            "Failed to load MCMCSearch results from file '{:s}',"
+            " something must have gone wrong!".format(mcmc_file)
+        )
+    mcmc_res = pyfstat.utils.read_txt_file_with_header(mcmc_file)
+
+    zoom = {
+        "F0": [inj["F0"] - 10 * dF0, inj["F0"] + 10 * dF0],
+        "F1": [inj["F1"] - 5 * dF1, inj["F1"] + 5 * dF1],
+    }
+
+    # we'll use the two local plotting functions defined above
+    # to avoid code duplication in the sky case
+    logger.info("Creating MCMC-grid comparison plots...")
+    plot_grid_vs_samples(grid_res, mcmc_res, "F0", "F1")
+    plot_2F_scatter(grid_res, "grid", "F0", "F1")
+    plot_2F_scatter(mcmc_res, "mcmc", "F0", "F1")
+    if sky:
+        plot_grid_vs_samples(grid_res, mcmc_res, "Alpha", "Delta")
+        plot_2F_scatter(grid_res, "grid", "Alpha", "Delta")
+        plot_2F_scatter(mcmc_res, "mcmc", "Alpha", "Delta")
```

### Comparing `PyFstat-1.9.0/examples/other_examples/PyFstat_example_twoF_cumulative.py` & `PyFstat-2.0.0/examples/other_examples/PyFstat_example_twoF_cumulative.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+"""
+Cumulative coherent 2F
+======================
+
+Compute the cumulative coherent F-statistic of a signal candidate.
+"""
+
+
 import os
+
 import numpy as np
-import pyfstat
 
-from pyfstat.helper_functions import get_predict_fstat_parameters_from_dict
+import pyfstat
+from pyfstat.utils import get_predict_fstat_parameters_from_dict
 
-label = os.path.splitext(os.path.basename(__file__))[0]
+label = "PyFstatExampleTwoFCumulative"
 outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(label=label, outdir=outdir)
 
 # Properties of the GW data
 gw_data = {
     "sqrtSX": 1e-23,
     "tstart": 1000000000,
     "duration": 100 * 86400,
     "detectors": "H1,L1",
@@ -51,17 +61,17 @@
     tref=tref,
     **gw_data,
     **phase_parameters,
     **amplitude_parameters,
 )
 data.make_data()
 
-# The predicted twoF, given by lalapps_predictFstat can be accessed by
+# The predicted twoF (expectation over noise realizations) can be accessed by
 twoF = data.predict_fstat()
-print("Predicted twoF value: {}\n".format(twoF))
+logger.info("Predicted twoF value: {}\n".format(twoF))
 
 # Create a search object for each of the possible SFT combinations
 # (H1 only, L1 only, H1 + L1).
 ifo_constraints = ["L1", "H1", None]
 compute_fstat_per_ifo = [
     pyfstat.ComputeFstat(
         sftfilepattern=os.path.join(
```

### Comparing `PyFstat-1.9.0/examples/transient_examples/PyFstat_example_long_transient_MCMC_search.py` & `PyFstat-2.0.0/examples/transient_examples/PyFstat_example_short_transient_MCMC_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,104 @@
-#!/usr/bin/env python
+"""
+Short transient MCMC search
+===========================
+
+MCMC search for a Short transient CW signal.
+"""
 
-import pyfstat
 import os
+
 import numpy as np
+import PyFstat_example_make_data_for_short_transient_search as data
+
+import pyfstat
+from pyfstat.utils import get_predict_fstat_parameters_from_dict
 
-outdir = os.path.join("PyFstat_example_data", "PyFstat_example_long_transient_search")
-if not os.path.isdir(outdir) or not np.any(
-    [f.endswith(".sft") for f in os.listdir(outdir)]
-):
-    raise RuntimeError(
-        "Please first run PyFstat_example_make_data_for_long_transient_search.py !"
-    )
-
-tstart = 1000000000
-duration = 200 * 86400
-
-inj = {
-    "tref": tstart,
-    "F0": 30.0,
-    "F1": -1e-10,
-    "F2": 0,
-    "Alpha": 0.5,
-    "Delta": 1,
-    "transient_tstart": tstart + 0.25 * duration,
-    "transient_duration": 0.5 * duration,
-}
-
-DeltaF0 = 6e-7
-DeltaF1 = 1e-13
-
-# to make the search cheaper, we exactly target the transientStartTime
-# to the injected value and only search over TransientTau
-theta_prior = {
-    "F0": {
-        "type": "unif",
-        "lower": inj["F0"] - DeltaF0 / 2.0,
-        "upper": inj["F0"] + DeltaF0 / 2.0,
-    },
-    "F1": {
-        "type": "unif",
-        "lower": inj["F1"] - DeltaF1 / 2.0,
-        "upper": inj["F1"] + DeltaF1 / 2.0,
-    },
-    "F2": inj["F2"],
-    "Alpha": inj["Alpha"],
-    "Delta": inj["Delta"],
-    "transient_tstart": tstart + 0.25 * duration,
-    "transient_duration": {
-        "type": "halfnorm",
-        "loc": 0.001 * duration,
-        "scale": 0.5 * duration,
-    },
-}
+if __name__ == "__main__":
+    label = "PyFstatExampleShortTransientMCMCSearch"
+    logger = pyfstat.set_up_logger(label=label, outdir=data.outdir)
+
+    if not os.path.isdir(data.outdir) or not np.any(
+        [f.endswith(".sft") for f in os.listdir(data.outdir)]
+    ):
+        raise RuntimeError(
+            "Please first run PyFstat_example_make_data_for_short_transient_search.py !"
+        )
+
+    inj = {
+        "tref": data.tstart,
+        "F0": data.F0,
+        "F1": data.F1,
+        "F2": data.F2,
+        "Alpha": data.Alpha,
+        "Delta": data.Delta,
+        "transient_tstart": data.transient_tstart,
+        "transient_duration": data.transient_duration,
+    }
+
+    DeltaF0 = 1e-2
+    DeltaF1 = 1e-9
+
+    theta_prior = {
+        "F0": {
+            "type": "unif",
+            "lower": inj["F0"] - DeltaF0 / 2.0,
+            "upper": inj["F0"] + DeltaF0 / 2.0,
+        },
+        "F1": {
+            "type": "unif",
+            "lower": inj["F1"] - DeltaF1 / 2.0,
+            "upper": inj["F1"] + DeltaF1 / 2.0,
+        },
+        "F2": inj["F2"],
+        "Alpha": inj["Alpha"],
+        "Delta": inj["Delta"],
+        "transient_tstart": {
+            "type": "unif",
+            "lower": data.tstart,
+            "upper": data.tstart + data.duration - 2 * data.Tsft,
+        },
+        "transient_duration": {
+            "type": "unif",
+            "lower": 2 * data.Tsft,
+            "upper": data.duration - 2 * data.Tsft,
+        },
+    }
 
 ntemps = 2
 log10beta_min = -1
 nwalkers = 100
-nsteps = [100, 100]
+nsteps = [200, 200]
+
+BSGL = False
+transientWindowType = "rect"
 
 mcmc = pyfstat.MCMCTransientSearch(
-    label="transient_search",
-    outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*simulated_transient_signal*sft"),
+    label=label + ("BSGL" if BSGL else ""),
+    outdir=data.outdir,
+    sftfilepattern=os.path.join(data.outdir, f"*{data.label}*sft"),
     theta_prior=theta_prior,
     tref=inj["tref"],
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
     log10beta_min=log10beta_min,
-    transientWindowType="rect",
+    transientWindowType=transientWindowType,
+    BSGL=BSGL,
 )
 mcmc.run(walker_plot_args={"plot_det_stat": True, "injection_parameters": inj})
 mcmc.print_summary()
 mcmc.plot_corner(add_prior=True, truths=inj)
 mcmc.plot_prior_posterior(injection_parameters=inj)
+
+# plot cumulative 2F, first building a dict as required for PredictFStat
+d, maxtwoF = mcmc.get_max_twoF()
+for key, val in mcmc.theta_prior.items():
+    if key not in d:
+        d[key] = val
+d["h0"] = data.h0
+d["cosi"] = data.cosi
+d["psi"] = data.psi
+PFS_input = get_predict_fstat_parameters_from_dict(
+    d, transientWindowType=transientWindowType
+)
+mcmc.plot_cumulative_max(PFS_input=PFS_input)
```

### Comparing `PyFstat-1.9.0/examples/transient_examples/PyFstat_example_make_data_for_short_transient_search.py` & `PyFstat-2.0.0/examples/transient_examples/PyFstat_example_make_data_for_long_transient_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,62 @@
-#!/usr/bin/env python
+"""
+Long transient search examples: Make data
+=========================================
+
+An example to generate data with a long transient signal.
+
+This can be run either stand-alone (will just generate SFT files and nothing else);
+or it is also being imported from
+PyFstat_example_long_transient_MCMC_search.py
+"""
 
-import pyfstat
 import os
 
-outdir = os.path.join("PyFstat_example_data", "PyFstat_example_short_transient_search")
+import pyfstat
+
+label = "PyFstatExampleLongTransientSearch"
+outdir = os.path.join("PyFstat_example_data", label)
+logger = pyfstat.set_up_logger(outdir=outdir, label=label)
 
 F0 = 30.0
 F1 = -1e-10
 F2 = 0
 Alpha = 0.5
 Delta = 1
 
 tstart = 1000000000
-duration = 2 * 86400
+duration = 200 * 86400
 
 transient_tstart = tstart + 0.25 * duration
 transient_duration = 0.5 * duration
+transientWindowType = "rect"
 tref = tstart
 
 h0 = 1e-23
 cosi = 0
+psi = 0
+phi = 0
 sqrtSX = 1e-22
 detectors = "H1,L1"
 
-Tsft = 1800
-
-transient = pyfstat.Writer(
-    label="simulated_transient_signal",
-    outdir=outdir,
-    tref=tref,
-    tstart=tstart,
-    duration=duration,
-    F0=F0,
-    F1=F1,
-    F2=F2,
-    Alpha=Alpha,
-    Delta=Delta,
-    h0=h0,
-    cosi=cosi,
-    detectors=detectors,
-    sqrtSX=sqrtSX,
-    transientStartTime=transient_tstart,
-    transientTau=transient_duration,
-    transientWindowType="rect",
-    Tsft=Tsft,
-    Band=0.1,
-)
-transient.make_data()
+if __name__ == "__main__":
+    transient = pyfstat.Writer(
+        label=label,
+        outdir=outdir,
+        tref=tref,
+        tstart=tstart,
+        duration=duration,
+        F0=F0,
+        F1=F1,
+        F2=F2,
+        Alpha=Alpha,
+        Delta=Delta,
+        h0=h0,
+        cosi=cosi,
+        detectors=detectors,
+        sqrtSX=sqrtSX,
+        transientStartTime=transient_tstart,
+        transientTau=transient_duration,
+        transientWindowType=transientWindowType,
+    )
+    transient.make_data()
+    logger.info(f"Predicted 2F from injection Writer: {transient.predict_fstat()}")
```

### Comparing `PyFstat-1.9.0/examples/transient_examples/PyFstat_example_short_transient_MCMC_search.py` & `PyFstat-2.0.0/examples/transient_examples/PyFstat_example_long_transient_MCMC_search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,111 @@
-#!/usr/bin/env python
-
-import pyfstat
+"""
+Long transient MCMC search
+==========================
+
+MCMC search for a long transient CW signal.
+
+By default, the standard persistent-CW 2F-statistic
+and the transient max2F statistic are compared.
+
+You can turn on either `BSGL = True` or `BtSG = True` (not both!)
+to test alternative statistics.
+"""
 import os
+
 import numpy as np
+import PyFstat_example_make_data_for_long_transient_search as data
 
-outdir = os.path.join("PyFstat_example_data", "PyFstat_example_short_transient_search")
-if not os.path.isdir(outdir) or not np.any(
-    [f.endswith(".sft") for f in os.listdir(outdir)]
+import pyfstat
+from pyfstat.utils import get_predict_fstat_parameters_from_dict
+
+if not os.path.isdir(data.outdir) or not np.any(
+    [f.endswith(".sft") for f in os.listdir(data.outdir)]
 ):
     raise RuntimeError(
-        "Please first run PyFstat_example_make_data_for_short_transient_search.py !"
+        "Please first run PyFstat_example_make_data_for_long_transient_search.py !"
     )
 
-tstart = 1000000000
-duration = 2 * 86400
-Tsft = 1800
+label = "PyFstatExampleLongTransientMCMCSearch"
+logger = pyfstat.set_up_logger(label=label, outdir=data.outdir)
+
+tstart = data.tstart
+duration = data.duration
 
 inj = {
-    "tref": tstart,
-    "F0": 30.0,
-    "F1": -1e-10,
-    "F2": 0,
-    "Alpha": 0.5,
-    "Delta": 1,
-    "transient_tstart": tstart + 0.25 * duration,
-    "transient_duration": 0.5 * duration,
+    "tref": data.tstart,
+    "F0": data.F0,
+    "F1": data.F1,
+    "F2": data.F2,
+    "Alpha": data.Alpha,
+    "Delta": data.Delta,
+    "transient_tstart": data.transient_tstart,
+    "transient_duration": data.transient_duration,
 }
 
-DeltaF0 = 1e-2
-DeltaF1 = 1e-9
+DeltaF0 = 6e-7
+DeltaF1 = 1e-13
 
+# to make the search cheaper, we exactly target the transientStartTime
+# to the injected value and only search over TransientTau
 theta_prior = {
     "F0": {
         "type": "unif",
         "lower": inj["F0"] - DeltaF0 / 2.0,
         "upper": inj["F0"] + DeltaF0 / 2.0,
     },
     "F1": {
         "type": "unif",
         "lower": inj["F1"] - DeltaF1 / 2.0,
         "upper": inj["F1"] + DeltaF1 / 2.0,
     },
     "F2": inj["F2"],
     "Alpha": inj["Alpha"],
     "Delta": inj["Delta"],
-    "transient_tstart": {
-        "type": "unif",
-        "lower": tstart,
-        "upper": tstart + duration - 2 * Tsft,
-    },
+    "transient_tstart": tstart + 0.25 * duration,
     "transient_duration": {
-        "type": "unif",
-        "lower": 2 * Tsft,
-        "upper": duration - 2 * Tsft,
+        "type": "halfnorm",
+        "loc": 0.001 * duration,
+        "scale": 0.5 * duration,
     },
 }
 
 ntemps = 2
 log10beta_min = -1
 nwalkers = 100
 nsteps = [100, 100]
 
+transientWindowType = "rect"
+BSGL = False
+BtSG = False
+
 mcmc = pyfstat.MCMCTransientSearch(
-    label="transient_search",
-    outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*simulated_transient_signal*sft"),
+    label=label + ("BSGL" if BSGL else "") + ("BtSG" if BtSG else ""),
+    outdir=data.outdir,
+    sftfilepattern=os.path.join(data.outdir, f"*{data.label}*sft"),
     theta_prior=theta_prior,
     tref=inj["tref"],
     nsteps=nsteps,
     nwalkers=nwalkers,
     ntemps=ntemps,
     log10beta_min=log10beta_min,
-    transientWindowType="rect",
+    transientWindowType=transientWindowType,
+    BSGL=BSGL,
+    BtSG=BtSG,
 )
 mcmc.run(walker_plot_args={"plot_det_stat": True, "injection_parameters": inj})
 mcmc.print_summary()
 mcmc.plot_corner(add_prior=True, truths=inj)
 mcmc.plot_prior_posterior(injection_parameters=inj)
+
+# plot cumulative 2F, first building a dict as required for PredictFStat
+d, maxtwoF = mcmc.get_max_twoF()
+for key, val in mcmc.theta_prior.items():
+    if key not in d:
+        d[key] = val
+d["h0"] = data.h0
+d["cosi"] = data.cosi
+d["psi"] = data.psi
+PFS_input = get_predict_fstat_parameters_from_dict(
+    d, transientWindowType=transientWindowType
+)
+mcmc.plot_cumulative_max(PFS_input=PFS_input)
```

### Comparing `PyFstat-1.9.0/examples/transient_examples/PyFstat_example_short_transient_grid_search.py` & `PyFstat-2.0.0/examples/transient_examples/PyFstat_example_short_transient_grid_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,93 @@
-#!/usr/bin/env python
+"""
+Short transient grid search
+===========================
+
+An example grid-based search for a short transient signal.
+By default, the standard persistent-CW 2F-statistic
+and the transient max2F statistic are compared.
+
+You can turn on either `BSGL = True` or `BtSG = True` (not both!)
+to test alternative statistics.
+
+This is also ready to use on a GPU,
+if you have one available and `pycuda` installed.
+Just change to `tCWFstatMapVersion = "pycuda"`.
+"""
 
-import pyfstat
 import os
+
 import numpy as np
+import PyFstat_example_make_data_for_short_transient_search as data
 
-outdir = os.path.join("PyFstat_example_data", "PyFstat_example_short_transient_search")
-if not os.path.isdir(outdir) or not np.any(
-    [f.endswith(".sft") for f in os.listdir(outdir)]
-):
-    raise RuntimeError(
-        "Please first run PyFstat_example_make_data_for_short_transient_search.py !"
-    )
+import pyfstat
 
-F0 = 30.0
-F1 = -1e-10
-F2 = 0
-Alpha = 0.5
-Delta = 1
-
-minStartTime = 1000000000
-maxStartTime = minStartTime + 2 * 86400
-Tspan = maxStartTime - minStartTime
-tref = minStartTime
-
-Tsft = 1800
-
-m = 0.001
-dF0 = np.sqrt(12 * m) / (np.pi * Tspan)
-DeltaF0 = 100 * dF0
-F0s = [F0 - DeltaF0 / 2.0, F0 + DeltaF0 / 2.0, dF0]
-F1s = [F1]
-F2s = [F2]
-Alphas = [Alpha]
-Deltas = [Delta]
-
-print("Standard CW search:")
-search1 = pyfstat.GridSearch(
-    label="CW",
-    outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*simulated_transient_signal*sft"),
-    F0s=F0s,
-    F1s=F1s,
-    F2s=F2s,
-    Alphas=Alphas,
-    Deltas=Deltas,
-    tref=tref,
-    minStartTime=minStartTime,
-    maxStartTime=maxStartTime,
-    BSGL=False,
-)
-search1.run()
-search1.print_max_twoF()
-search1.save_array_to_disk(search1.data)
-
-search1.plot_1D(xkey="F0", xlabel="freq [Hz]", ylabel="$2\\mathcal{F}$")
-
-print("with t0,tau bands:")
-search2 = pyfstat.TransientGridSearch(
-    label="tCW",
-    outdir=outdir,
-    sftfilepattern=os.path.join(outdir, "*simulated_transient_signal*sft"),
-    F0s=F0s,
-    F1s=F1s,
-    F2s=F2s,
-    Alphas=Alphas,
-    Deltas=Deltas,
-    tref=tref,
-    minStartTime=minStartTime,
-    maxStartTime=maxStartTime,
-    transientWindowType="rect",
-    t0Band=Tspan - 2 * Tsft,
-    tauBand=Tspan,
-    BSGL=False,
-    outputTransientFstatMap=True,
-    tCWFstatMapVersion="lal",
-)
-search2.run()
-search2.print_max_twoF()
-search2.save_array_to_disk(search2.data)
+tCWFstatMapVersion = "lal"
 
-search2.plot_1D(xkey="F0", xlabel="freq [Hz]", ylabel="$2\\mathcal{F}$")
+if __name__ == "__main__":
+    label = "PyFstatExampleShortTransientGridSearch"
+    logger = pyfstat.set_up_logger(label=label, outdir=data.outdir)
+    if not os.path.isdir(data.outdir) or not np.any(
+        [f.endswith(".sft") for f in os.listdir(data.outdir)]
+    ):
+        raise RuntimeError(
+            "Please first run PyFstat_example_make_data_for_short_transient_search.py !"
+        )
+
+    maxStartTime = data.tstart + data.duration
+
+    m = 0.001
+    dF0 = np.sqrt(12 * m) / (np.pi * data.duration)
+    DeltaF0 = 100 * dF0
+    F0s = [data.F0 - DeltaF0 / 2.0, data.F0 + DeltaF0 / 2.0, dF0]
+    F1s = [data.F1]
+    F2s = [data.F2]
+    Alphas = [data.Alpha]
+    Deltas = [data.Delta]
+
+    BSGL = False
+    BtSG = False
+
+    logger.info("Standard CW search:")
+    search1 = pyfstat.GridSearch(
+        label=label + f"CW{'BSGL' if BSGL else ''}",
+        outdir=data.outdir,
+        sftfilepattern=os.path.join(data.outdir, f"*{data.label}*sft"),
+        F0s=F0s,
+        F1s=F1s,
+        F2s=F2s,
+        Alphas=Alphas,
+        Deltas=Deltas,
+        tref=data.tref,
+        BSGL=BSGL,
+    )
+    search1.run()
+    search1.print_max_twoF()
+    search1.plot_1D(
+        xkey="F0", xlabel="freq [Hz]", ylabel=search1.tex_labels[search1.detstat]
+    )
+
+    logger.info("with t0,tau bands:")
+    label = f"tCW{'_BSGL' if BSGL else ''}{'_BtSG' if BtSG else ''}_FstatMap_{tCWFstatMapVersion}"
+    search2 = pyfstat.TransientGridSearch(
+        label=label,
+        outdir=data.outdir,
+        sftfilepattern=os.path.join(data.outdir, f"*{data.label}*sft"),
+        F0s=F0s,
+        F1s=F1s,
+        F2s=F2s,
+        Alphas=Alphas,
+        Deltas=Deltas,
+        tref=data.tref,
+        transientWindowType="rect",
+        t0Band=data.duration - 2 * data.Tsft,
+        tauBand=data.duration,
+        outputTransientFstatMap=True,
+        tCWFstatMapVersion=tCWFstatMapVersion,
+        BSGL=BSGL,
+        BtSG=BtSG,
+    )
+    search2.run()
+    search2.print_max_twoF()
+    search2.plot_1D(
+        xkey="F0", xlabel="freq [Hz]", ylabel=search2.tex_labels[search2.detstat]
+    )
```

### Comparing `PyFstat-1.9.0/pyfstat/core.py` & `PyFstat-2.0.0/pyfstat/make_sfts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1771 +1,1757 @@
-""" The core tools used in pyfstat """
+"""PyFstat tools to generate and manipulate data in the form of SFTs."""
 
 
-import os
-import logging
-import copy
-from pprint import pformat
-
 import glob
-import numpy as np
-import scipy.special
-import scipy.optimize
-from datetime import datetime
-import getpass
-import socket
+import logging
+import os
+import pkgutil
 
 import lal
 import lalpulsar
-import pyfstat.helper_functions as helper_functions
-import pyfstat.tcw_fstat_map_funcs as tcw
-
-# workaround for matplotlib on X-less remote logins
-if "DISPLAY" in os.environ:
-    import matplotlib.pyplot as plt
-else:
-    logging.info(
-        'No $DISPLAY environment variable found, so importing \
-                  matplotlib.pyplot with non-interactive "Agg" backend.'
-    )
-    import matplotlib
-
-    matplotlib.use("Agg")
-    import matplotlib.pyplot as plt
-
-helper_functions.set_up_matplotlib_defaults()
-args, tqdm = helper_functions.set_up_command_line_arguments()
-detector_colors = {"h1": "C0", "l1": "C1"}
-
-
-class BaseSearchClass:
-    """ The base search class providing parent methods to other searches """
-
-    def __new__(cls, *args, **kwargs):
-        logging.info(f"Creating {cls.__name__} object...")
-        instance = super().__new__(cls)
-        return instance
-
-    def _add_log_file(self, header=None):
-        """ Log output to a file, requires class to have outdir and label """
-        header = [] if header is None else header
-        logfilename = os.path.join(self.outdir, self.label + ".log")
-        with open(logfilename, "w") as fp:
-            for hline in header:
-                fp.write("# {:s}\n".format(hline))
-        fh = logging.FileHandler(logfilename)
-        fh.setLevel(logging.INFO)
-        fh.setFormatter(
-            logging.Formatter(
-                "%(asctime)s %(levelname)-8s: %(message)s", datefmt="%y-%m-%d %H:%M"
-            )
-        )
-        logging.getLogger().addHandler(fh)
-
-    def _get_list_of_matching_sfts(self):
-        """ Returns a list of sfts matching the attribute sftfilepattern """
-        sftfilepatternlist = np.atleast_1d(self.sftfilepattern.split(";"))
-        matches = [glob.glob(p) for p in sftfilepatternlist]
-        matches = [item for sublist in matches for item in sublist]
-        if len(matches) > 0:
-            return matches
-        else:
-            raise IOError("No sfts found matching {}".format(self.sftfilepattern))
-
-    def set_ephemeris_files(self, earth_ephem=None, sun_ephem=None):
-        """Set the ephemeris files to use for the Earth and Sun
-
-        Parameters
-        ----------
-        earth_ephem, sun_ephem: str
-            Paths of the two files containing positions of Earth and Sun,
-            respectively at evenly spaced times, as passed to CreateFstatInput
-
-        Note: If not manually set, default values from get_ephemeris_files()
-              are used (looking in ~/.pyfstat or $LALPULSAR_DATADIR)
+import numpy as np
+from tqdm import tqdm, trange
 
-        """
+import pyfstat.utils as utils
+from pyfstat.core import BaseSearchClass, SearchForSignalWithJumps
 
-        earth_ephem_default, sun_ephem_default = helper_functions.get_ephemeris_files()
+logger = logging.getLogger(__name__)
 
-        if earth_ephem is None:
-            self.earth_ephem = earth_ephem_default
-        else:
-            self.earth_ephem = earth_ephem
-        if sun_ephem is None:
-            self.sun_ephem = sun_ephem_default
-        else:
-            self.sun_ephem = sun_ephem
 
-    def _set_init_params_dict(self, argsdict):
-        argsdict.pop("self")
-        self.init_params_dict = argsdict
-
-    def pprint_init_params_dict(self):
-        """
-        Pretty-print a parameters dictionary for output file headers.
-
-        Returns a list of lines to be printed,
-        including opening/closing "{" and "}",
-        consistent indentation,
-        as well as end-of-line commas,
-        but no comment markers at start of lines.
-        """
-        pretty_init_parameters = pformat(
-            self.init_params_dict, indent=2, width=74
-        ).split("\n")
-        pretty_init_parameters = (
-            ["{"]
-            + [pretty_init_parameters[0].replace("{", " ")]
-            + pretty_init_parameters[1:-2]
-            + [pretty_init_parameters[-1].rstrip("}")]
-            + ["}"]
-        )
-        return pretty_init_parameters
+class Writer(BaseSearchClass):
+    """The main class for generating data in the form of SFTs.
 
-    def get_output_file_header(self):
-        header = [
-            "date: {}".format(str(datetime.now())),
-            "user: {}".format(getpass.getuser()),
-            "hostname: {}".format(socket.gethostname()),
-            "PyFstat: {}".format(helper_functions.get_version_string()),
-        ]
-        lalVCSinfo = lal.VCSInfoString(lalpulsar.PulsarVCSInfoList, 0, "")
-        header += filter(None, lalVCSinfo.split("\n"))
-        header += [
-            "search: {}".format(type(self).__name__),
-            "parameters: ",
-        ]
-        header += self.pprint_init_params_dict()
-        return header
+    Short Fourier Transforms (SFTs) are a standard data format used in LALSuite,
+    containing the Fourier transform of strain data over a duration Tsft.
 
-    def read_par(
-        self, filename=None, label=None, outdir=None, suffix="par", raise_error=True
-    ):
-        params_dict = helper_functions.read_par(
-            filename=filename,
-            label=label or getattr(self, "label", None),
-            outdir=outdir or getattr(self, "outdir", None),
-            suffix=suffix,
-            raise_error=raise_error,
-        )
-        return params_dict
+    SFT data can be generated from scratch, including Gaussian noise and/or
+    simulated CW signals or transient signals.
+    Existing SFTs (real data or previously simulated) can also be reused through
+    the `noiseSFTs` option, allowing to 'inject' additional signals into them.
 
-    @staticmethod
-    def translate_keys_to_lal(dictionary):
-        """Convert input keys into lal input keys
-
-        Input keys are F0, F1, F2, ..., while LAL functions
-        prefer to use Freq, f1dot, f2dot, ....
-
-        Since lal keys are only used to call for lal routines,
-        it makes sense to have this function defined this way
-        so it can be called on the fly.
-
-        Parameters
-        ----------
-        dictionary: dict
-            Dictionary to translate. A copy will be made (an returned)
-            before translation takes place.
-
-        Returns
-        -------
-        translated_dict: dict
-            Copy of "dictionary" with new keys according to lal.
-        """
-
-        translation = {
-            "F0": "Freq",
-            "F1": "f1dot",
-            "F2": "f2dot",
-            "phi": "phi0",
-            "tref": "refTime",
-            "asini": "orbitasini",
-            "period": "orbitPeriod",
-            "tp": "orbitTp",
-            "argp": "orbitArgp",
-            "ecc": "orbitEcc",
-            "transient_tstart": "transient-t0Epoch",
-            "transient_duration": "transient-tau",
-        }
+    This class currently relies on the `Makefakedata_v5` executable
+    which will be run in a subprocess.
+    See `lalpulsar_Makefakedata_v5 --help`
+    for more detailed help with some of the parameters.
+    """
 
-        keys_to_translate = [key for key in dictionary.keys() if key in translation]
+    mfd = "lalpulsar_Makefakedata_v5"
+    """The executable; can be overridden by child classes."""
 
-        translated_dict = dictionary.copy()
-        for key in keys_to_translate:
-            translated_dict[translation[key]] = translated_dict.pop(key)
-        return translated_dict
+    signal_parameter_labels = [
+        "tref",
+        "F0",
+        "F1",
+        "F2",
+        "Alpha",
+        "Delta",
+        "h0",
+        "cosi",
+        "psi",
+        "phi",
+        "transientWindowType",
+        "transientStartTime",
+        "transientTau",
+    ]
+    """Default convention of labels for the various signal parameters."""
+
+    gps_time_and_string_formats_as_LAL = {
+        "refTime": ":10.9f",
+        "transientWindowType": ":s",
+        "transientStartTime": ":10.0f",
+        "transientTau": ":10.0f",
+    }
+    """Dictionary to ensure proper format handling for some special parameters.
 
+    GPS times should NOT be parsed using scientific notation.
+    LAL routines would silently parse them wrongly.
+    """
 
-class ComputeFstat(BaseSearchClass):
-    """ Base class providing interface to `lalpulsar.ComputeFstat` """
+    required_signal_parameters = [
+        # leaving out "F1","F2","psi","phi","tref" as they have defaults
+        "F0",
+        "Alpha",
+        "Delta",
+        "cosi",
+    ]
+    """List of parameters required for a successful execution of Makefakedata_v5.
+    The rest of available parameters are not required as they have default values
+    silently given by Makefakedata_v5
+    """
 
-    @helper_functions.initializer
+    @utils.initializer
     def __init__(
         self,
-        tref,
-        sftfilepattern=None,
-        minStartTime=None,
-        maxStartTime=None,
+        label="PyFstat",
+        tstart=None,
+        duration=None,
+        tref=None,
+        F0=None,
+        F1=0,
+        F2=0,
+        Alpha=None,
+        Delta=None,
+        h0=None,
+        cosi=None,
+        psi=0.0,
+        phi=0,
         Tsft=1800,
-        binary=False,
-        BSGL=False,
-        transientWindowType=None,
-        t0Band=None,
-        tauBand=None,
-        tauMin=None,
-        dt0=None,
-        dtau=None,
+        outdir=".",
+        sqrtSX=None,
+        noiseSFTs=None,
+        SFTWindowType=None,
+        SFTWindowParam=None,
+        SFTWindowBeta=None,
+        Band=None,
         detectors=None,
-        minCoverFreq=None,
-        maxCoverFreq=None,
-        search_ranges=None,
-        injectSources=None,
-        injectSqrtSX=None,
-        assumeSqrtSX=None,
-        SSBprec=None,
-        RngMedWindow=None,
-        tCWFstatMapVersion="lal",
-        cudaDeviceName=None,
-        computeAtoms=False,
         earth_ephem=None,
         sun_ephem=None,
+        transientWindowType="none",
+        transientStartTime=None,
+        transientTau=None,
+        randSeed=None,
+        timestamps=None,
     ):
         """
         Parameters
         ----------
-        tref : int
-            GPS seconds of the reference time.
-        sftfilepattern : str
-            Pattern to match SFTs using wildcards (*?) and ranges [0-9];
-            mutiple patterns can be given separated by colons.
-        minStartTime, maxStartTime : int
-            Only use SFTs with timestamps starting from this range,
-            following the XLALCWGPSinRange convention:
-            half-open intervals [minStartTime,maxStartTime]
-        binary : bool
-            If true, search of binary parameters.
-        BSGL : bool
-            If true, compute the BSGL rather than the twoF value.
-        transientWindowType: str
-            If 'rect' or 'exp',
-            allow for the Fstat to be computed over a transient range.
-            ('none' instead of None explicitly calls the transient-window
-            function, but with the full range, for debugging)
-            (if not None, will also force atoms regardless of computeAtoms option)
-        t0Band, tauBand: int
-            if >0, search t0 in (minStartTime,minStartTime+t0Band)
-                   and tau in (tauMin,2*Tsft+tauBand).
-            if =0, only compute CW Fstat with t0=minStartTime,
-                   tau=maxStartTime-minStartTime.
-        tauMin: int
-            defaults to 2*Tsft
-        dt0, dtau: int
-            grid resolutions in transient start-time and duration,
-            both default to Tsft
-        detectors : str
-            Two-character references to the detectors for which to use data.
-            Specify None for no constraint.
-            For multiple detectors, separate by comma.
-        minCoverFreq, maxCoverFreq : float
-            The min and max cover frequency passed to CreateFstatInput.
-            For negative values, these will be used as offsets from the min/max
-            frequency contained in the sftfilepattern.
-            If either is None, search_ranges is used to estimate them.
-            If the automatic estimation fails and you do not have a good idea
-            what to set these two options to, setting both to -0.5 will
-            reproduce the default behaviour of PyFstat <=1.4 and may be a
-            reasonably safe fallback in many cases.
-        search_ranges: dict
-            Dictionary of ranges in all search parameters,
-            only used to estimate frequency band passed to CreateFstatInput,
-            if minCoverFreq, maxCoverFreq are not specified (=='None').
-            For actually running searches,
-            grids/points will have to be passed separately to the .run() method.
-            The entry for each parameter must be a list of length 1, 2 or 3:
-            [single_value], [min,max] or [min,max,step].
-        injectSources : dict or str
-            Either a dictionary of the values to inject, or a string pointing
-            to the .cff file to inject
-        injectSqrtSX : float or list or str
-            Single-sided PSD values for generating fake Gaussian noise on the fly.
-            Single float or str value: use same for all IFOs.
-            List or comma-separated string: must match len(detectors)
-            and/or the data in sftfilepattern.
-            Detectors will be paired to list elements following alphabetical order.
-        assumeSqrtSX : float or list or str
-            Don't estimate noise-floors but assume this (stationary) single-sided PSD.
-            Single float or str value: use same for all IFOs.
-            List or comma-separated string: must match len(detectors)
-            and/or the data in sftfilepattern.
+        label: string
+            A human-readable label to be used in naming the output files.
+            NOTE: to agree with the v3 SFT naming specification
+            ( https://dcc.ligo.org/T040164-v2/public )
+            label can only contain ASCII alphanumeric characters
+            in their "description" field,
+            i.e. no underscores, hyphens etc.
+            Also, internally
+            a "channel"/"frame" name is constructed as `IFO:label`,
+            which may not exceed 64 characters,
+            so a label may only be 60 characters long.
+        tstart: int
+            Starting GPS epoch of the data set.
+            If `noiseSFT` are given, this is used as a LALPulsar
+            `SFTConstraint <https://lscsoft.docs.ligo.org/lalsuite/lalpulsar/struct_s_f_t_constraints.html>`_.
+            NOTE: mutually exclusive with `timestamps`.
+        duration: int
+            Duration (in GPS seconds) of the total data set.
+            If `noiseSFT` are given, this is used as a LALPulsar
+            `SFTConstraint <https://lscsoft.docs.ligo.org/lalsuite/lalpulsar/struct_s_f_t_constraints.html>`_.
+            NOTE: mutually exclusive with `timestamps`.
+        tref: float or None
+            Reference time for simulated signals.
+            Default is `None`, which sets the reference time to `tstart`.
+        F0: float or None
+            Frequency of a signal to inject.
+            Also used (if `Band` is not `None`) as center of frequency band.
+            Also needed when noise-only (`h0=None` or `h0==0`)
+            but no `noiseSFTs` given,
+            in which case it is also used as center of frequency band.
+        F1, F2, Alpha, Delta, h0, cosi, psi, phi: float or None
+            Additional frequency evolution and amplitude parameters for a signal.
+            If `h0=None` or `h0=0`, these are all ignored.
+            If `h0>0`, then at least `[Alpha,Delta,cosi]` need to be set explicitly.
+        Tsft: int
+            The SFT duration in seconds.
+            Will be ignored if `noiseSFTs` are given.
+        outdir: str
+            The directory where files are written to.
+            Default: current working directory.
+        sqrtSX: float or list or str or None
+            Single-sided PSD values for generating fake Gaussian noise.
+            Single float or str value: use same for all detectors.
+            List or comma-separated string: must match len(detectors).
             Detectors will be paired to list elements following alphabetical order.
-            If working with signal-only data, please set assumeSqrtSX=1 .
-        SSBprec : int
-            Flag to set the SSB calculation: 0=Newtonian, 1=relativistic,
-            2=relativisitic optimised, 3=DMoff, 4=NO_SPIN
-        RngMedWindow : int
-           Running-Median window size (number of bins)
-        tCWFstatMapVersion: str
-            Choose between standard 'lal' implementation,
-            'pycuda' for gpu, and some others for devel/debug.
-        cudaDeviceName: str
-            GPU name to be matched against drv.Device output.
-        computeAtoms: bool
-            request atoms calculations regardless of transientWindowType
-        earth_ephem: str
-            Earth ephemeris file path
-            if None, will check standard sources as per
-            helper_functions.get_ephemeris_files()
-        sun_ephem: str
-            Sun ephemeris file path
-            if None, will check standard sources as per
-            helper_functions.get_ephemeris_files()
+        noiseSFTs: str or None
+            Existing SFT files on top of which signals will be injected.
+            If not `None`, additional constraints can be applied
+            using the arguments `tstart` and `duration`.
+            NOTE: mutually exclusive with `timestamps`.
+        SFTWindowType: str or None
+            LAL name of the windowing function to apply to the data.
+        SFTWindowParam: float
+            Optional parameter for some windowing functions.
+        SFTWindowBeta: float
+            Defunct alias to `SFTWindowParam`.
+            Will be removed in a future release.
+        Band: float or None
+            If float, and `F0` is also not `None`, then output SFTs cover
+            `[F0-Band/2,F0+Band/2]`.
+            If `None` and `noiseSFTs` given, use their bandwidth.
+            If `None` and no `noiseSFTs` given,
+            a minimal covering band for a perfectly-matched
+            single-template ComputeFstat analysis is estimated.
+        detectors: str or None
+            Comma-separated list of detectors to generate data for.
+            May be required depending on `timestamps`; see its documentation.
+        earth_ephem, sun_ephem: str or None
+            Paths of the two files containing positions of Earth and Sun.
+            If None, will check standard sources as per
+            utils.get_ephemeris_files().
+        transientWindowType: str
+            If `none`, a fully persistent CW signal is simulated.
+            If `rect` or `exp`, a transient signal with the corresponding
+            amplitude evolution is simulated.
+        transientStartTime: int or None
+            Start time for a transient signal.
+        transientTau: int or None
+            Duration (`rect` case) or decay time (`exp` case) of a transient signal.
+        randSeed: int or None
+            Optionally fix the random seed of Gaussian noise generation
+            for reproducibility.
+        timestamps: str or dict
+            Dictionary of timestamps (each key must refer to a detector),
+            a single list of timestamps
+            (will be replicated for all detectors; `detectors` must be set),
+            or comma-separated list of per-detector timestamps files
+            (simple text files,
+            comments must use `%`,
+            the first column is interpreted as SFT start times
+            and additional columns are ignored;
+            `detectors` must be set,
+            and the length and order must match).
+            Timestamps must be integers;
+            otherwise, will be implicitly cast by this method and MFDv5.
+            NOTE: mutually exclusive with [`tstart`, `duration`]
+            and with `noiseSFTs`.
         """
 
-        self._set_init_params_dict(locals())
         self.set_ephemeris_files(earth_ephem, sun_ephem)
-        self.init_computefstatistic()
-        self.output_file_header = self.get_output_file_header()
-
-    def _get_SFTCatalog(self):
-        """Load the SFTCatalog
-
-        If sftfilepattern is specified, load the data. If not, attempt to
-        create data on the fly.
-
-        """
-        if hasattr(self, "SFTCatalog"):
-            return
-        if self.sftfilepattern is None:
-            for k in ["minStartTime", "maxStartTime", "detectors"]:
-                if getattr(self, k) is None:
-                    raise ValueError(
-                        "If sftfilepattern==None, you must provide" " '{}'.".format(k)
-                    )
-            C1 = getattr(self, "injectSources", None) is None
-            C2 = getattr(self, "injectSqrtSX", None) is None
-            C3 = getattr(self, "Tsft", None) is None
-            if (C1 and C2) or C3:
-                raise ValueError(
-                    "If sftfilepattern==None, you must specify Tsft and"
-                    " either one of injectSources or injectSqrtSX."
-                )
-            SFTCatalog = lalpulsar.SFTCatalog()
-            Toverlap = 0
-            self.detector_names = self.detectors.split(",")
-            detNames = lal.CreateStringVector(*[d for d in self.detector_names])
-            # MakeMultiTimestamps follows the same [minStartTime,maxStartTime)
-            # convention as the SFT library, so we can pass Tspan like this
-            Tspan = self.maxStartTime - self.minStartTime
-            multiTimestamps = lalpulsar.MakeMultiTimestamps(
-                self.minStartTime, Tspan, self.Tsft, Toverlap, detNames.length
-            )
-            SFTCatalog = lalpulsar.MultiAddToFakeSFTCatalog(
-                SFTCatalog, detNames, multiTimestamps
-            )
-            self.SFTCatalog = SFTCatalog
-            return
-
-        logging.info("Initialising SFTCatalog")
-        constraints = lalpulsar.SFTConstraints()
-        constr_str = []
-        if self.detectors:
-            if "," in self.detectors:
-                logging.warning(
-                    "Multiple-detector constraints not available,"
-                    " using all available data."
-                )
-            else:
-                constraints.detector = self.detectors
-                constr_str.append("detector=" + constraints.detector)
-        if self.minStartTime:
-            constraints.minStartTime = lal.LIGOTimeGPS(self.minStartTime)
-            constr_str.append("minStartTime={}".format(self.minStartTime))
-        if self.maxStartTime:
-            constraints.maxStartTime = lal.LIGOTimeGPS(self.maxStartTime)
-            constr_str.append("maxStartTime={}".format(self.maxStartTime))
-        logging.info(
-            "Loading data matching SFT file name pattern '{}'"
-            " with constraints {}.".format(self.sftfilepattern, ", ".join(constr_str))
-        )
-        self.SFTCatalog = lalpulsar.SFTdataFind(self.sftfilepattern, constraints)
-        Tsft_from_catalog = int(1.0 / self.SFTCatalog.data[0].header.deltaF)
-        if Tsft_from_catalog != self.Tsft:
-            logging.info(
-                "Overwriting pre-set Tsft={:d} with {:d} obtained from SFTs.".format(
-                    self.Tsft, Tsft_from_catalog
-                )
-            )
-        self.Tsft = Tsft_from_catalog
-
-        # NOTE: in multi-IFO case, this will be a joint list of timestamps
-        # over all IFOs, probably sorted and not cleaned for uniqueness.
-        SFT_timestamps = [d.header.epoch for d in self.SFTCatalog.data]
-        self.SFT_timestamps = [float(s) for s in SFT_timestamps]
-        if len(SFT_timestamps) == 0:
-            raise ValueError("Failed to load any data")
-        if args.quite is False and args.no_interactive is False:
-            try:
-                from bashplotlib.histogram import plot_hist
+        self._basic_setup()
+        self._parse_args_consistent_with_mfd()
+        self.calculate_fmin_Band()
+
+    def _get_sft_constraints_from_tstart_duration(self):
+        """
+        Use start and duration to set up a lalpulsar.SFTConstraints
+        object. This method is only used if noiseSFTs is not None.
+        """
+        SFTConstraint = lalpulsar.SFTConstraints()
+
+        if self.tstart is None:
+            SFTConstraint.minStartTime = None
+            SFTConstraint.maxStartTime = None
+        elif self.duration is None:
+            SFTConstraint.maxStartTime = None
+        else:
+            SFTConstraint.minStartTime = lal.LIGOTimeGPS(self.tstart)
+            SFTConstraint.maxStartTime = SFTConstraint.minStartTime + self.duration
 
-                print("Data timestamps histogram:")
-                plot_hist(SFT_timestamps, height=5, bincount=50)
-            except ImportError:
-                pass
-
-        cl_tconv1 = "lalapps_tconvert {}".format(int(SFT_timestamps[0]))
-        output = helper_functions.run_commandline(cl_tconv1, log_level=logging.DEBUG)
-        tconvert1 = output.rstrip("\n")
-        cl_tconv2 = "lalapps_tconvert {}".format(int(SFT_timestamps[-1]))
-        output = helper_functions.run_commandline(cl_tconv2, log_level=logging.DEBUG)
-        tconvert2 = output.rstrip("\n")
-        logging.info(
-            "Data contains SFT timestamps from {} ({}) to (including) {} ({})".format(
-                int(SFT_timestamps[0]), tconvert1, int(SFT_timestamps[-1]), tconvert2
-            )
-        )
+        SFTConstraint.timestamps = None  # FIXME: not currently supported
 
-        if self.minStartTime is None:
-            self.minStartTime = int(SFT_timestamps[0])
-        if self.maxStartTime is None:
-            # XLALCWGPSinRange() convention: half-open intervals,
-            # maxStartTime must always be > last actual SFT timestamp
-            self.maxStartTime = int(SFT_timestamps[-1]) + self.Tsft
-
-        self.detector_names = list(set([d.header.name for d in self.SFTCatalog.data]))
-        if len(self.detector_names) == 0:
-            raise ValueError("No data loaded.")
-        logging.info(
-            "Loaded {} SFTs from detectors {}".format(
-                len(SFT_timestamps), self.detector_names
+        logger.info(
+            "SFT Constraints: [minStartTime:{}, maxStartTime:{}]".format(
+                SFTConstraint.minStartTime,
+                SFTConstraint.maxStartTime,
             )
         )
 
-    def init_computefstatistic(self):
-        """ Initialisation step of run_computefstatistic for a single point or search range """
+        return SFTConstraint
 
-        self._get_SFTCatalog()
+    def _get_setup_from_tstart_duration(self):
+        """
+        Default behavior: If no noiseSFTs are given, use the input parameters (tstart,
+        duration, detectors and Tsft) to make fake data.
+        """
+        self.tstart = int(self.tstart)
+        self.duration = int(self.duration)
 
-        logging.info("Initialising ephems")
-        ephems = lalpulsar.InitBarycenter(self.earth_ephem, self.sun_ephem)
+        IFOs = self.detectors.split(",")
+        # when duration is not a multiple of Tsft, to match MFDv5
+        # we need to round the number *up*
+        # and also include the overlapping bit at the end in the duration
+        numSFTs = int(np.ceil(float(self.duration) / self.Tsft))  # per IFO
+        effective_duration = numSFTs * self.Tsft
 
-        logging.info("Initialising Fstat arguments")
-        dFreq = 0
-        self.whatToCompute = lalpulsar.FSTATQ_2F
-        if self.transientWindowType or self.computeAtoms:
-            self.whatToCompute += lalpulsar.FSTATQ_ATOMS_PER_DET
-
-        FstatOAs = lalpulsar.FstatOptionalArgs()
-        FstatOAs.randSeed = lalpulsar.FstatOptionalArgsDefaults.randSeed
-        if self.SSBprec:
-            logging.info("Using SSBprec={}".format(self.SSBprec))
-            FstatOAs.SSBprec = self.SSBprec
-        else:
-            FstatOAs.SSBprec = lalpulsar.FstatOptionalArgsDefaults.SSBprec
-        FstatOAs.Dterms = lalpulsar.FstatOptionalArgsDefaults.Dterms
-        if self.RngMedWindow:
-            FstatOAs.runningMedianWindow = self.RngMedWindow
-        else:
-            FstatOAs.runningMedianWindow = (
-                lalpulsar.FstatOptionalArgsDefaults.runningMedianWindow
+        self.sftfilenames = [
+            utils.get_official_sft_filename(
+                dets,
+                numSFTs,
+                self.Tsft,
+                self.tstart,
+                effective_duration,
+                self.label,
             )
-        FstatOAs.FstatMethod = lalpulsar.FstatOptionalArgsDefaults.FstatMethod
-        if self.assumeSqrtSX is None:
-            FstatOAs.assumeSqrtSX = lalpulsar.FstatOptionalArgsDefaults.assumeSqrtSX
-        else:
-            mnf = lalpulsar.MultiNoiseFloor()
-            assumeSqrtSX = helper_functions.parse_list_of_numbers(self.assumeSqrtSX)
-            mnf.sqrtSn[: len(assumeSqrtSX)] = assumeSqrtSX
-            mnf.length = len(assumeSqrtSX)
-            FstatOAs.assumeSqrtSX = mnf
-        FstatOAs.prevInput = lalpulsar.FstatOptionalArgsDefaults.prevInput
-        FstatOAs.collectTiming = lalpulsar.FstatOptionalArgsDefaults.collectTiming
-
-        if hasattr(self, "injectSources") and type(self.injectSources) == dict:
-            logging.info("Injecting source with params: {}".format(self.injectSources))
-            PPV = lalpulsar.CreatePulsarParamsVector(1)
-            PP = PPV.data[0]
-            h0 = self.injectSources["h0"]
-            cosi = self.injectSources["cosi"]
-            use_aPlus = "aPlus" in dir(PP.Amp)
-            print("use_aPlus = {}".format(use_aPlus))
-            if use_aPlus:  # lalsuite interface changed in aff93c45
-                PP.Amp.aPlus = 0.5 * h0 * (1.0 + cosi ** 2)
-                PP.Amp.aCross = h0 * cosi
-            else:
-                PP.Amp.h0 = h0
-                PP.Amp.cosi = cosi
+            for ind, dets in enumerate(IFOs)
+        ]
 
-            PP.Amp.phi0 = self.injectSources["phi"]
-            PP.Amp.psi = self.injectSources["psi"]
-            PP.Doppler.Alpha = self.injectSources["Alpha"]
-            PP.Doppler.Delta = self.injectSources["Delta"]
-            if "fkdot" in self.injectSources:
-                PP.Doppler.fkdot = np.array(self.injectSources["fkdot"])
-            else:
-                PP.Doppler.fkdot = np.zeros(lalpulsar.PULSAR_MAX_SPINS)
-                for i, key in enumerate(["F0", "F1", "F2"]):
-                    PP.Doppler.fkdot[i] = self.injectSources[key]
-            PP.Doppler.refTime = self.tref
-            if "t0" not in self.injectSources:
-                PP.Transient.type = lalpulsar.TRANSIENT_NONE
-            FstatOAs.injectSources = PPV
-        elif hasattr(self, "injectSources") and type(self.injectSources) == str:
-            logging.info(
-                "Injecting source from param file: {}".format(self.injectSources)
-            )
-            PPV = lalpulsar.PulsarParamsFromFile(self.injectSources, self.tref)
-            FstatOAs.injectSources = PPV
-        else:
-            FstatOAs.injectSources = lalpulsar.FstatOptionalArgsDefaults.injectSources
-        if hasattr(self, "injectSqrtSX") and self.injectSqrtSX is not None:
-            self.injectSqrtSX = helper_functions.parse_list_of_numbers(
-                self.injectSqrtSX
+    def _get_setup_from_noiseSFTs(self):
+        """
+        If noiseSFTs are given, use them to obtain relevant data parameters (tstart,
+        duration, detectors and Tsft). The corresponding input values will be used to
+        set up a lalpulsar.SFTConstraints object to be imposed to the SFTs. Keep in
+        mind that Tsft will also be checked to be consistent accross all SFTs (this is
+        not implemented through SFTConstraints but through a simple list check).
+        """
+        SFTConstraint = self._get_sft_constraints_from_tstart_duration()
+        noise_multi_sft_catalog = lalpulsar.GetMultiSFTCatalogView(
+            lalpulsar.SFTdataFind(self.noiseSFTs, SFTConstraint)
+        )
+        if noise_multi_sft_catalog.length == 0:
+            raise IOError("Got empty SFT catalog.")
+
+        # Information to be extracted from the SFTs themselves
+        IFOs = []
+        tstart = []
+        tend = []
+        Tsft = []
+        self.sftfilenames = []  # This refers to the MFD output!
+
+        for ifo_catalog in noise_multi_sft_catalog.data:
+            ifo_name = lalpulsar.ListIFOsInCatalog(ifo_catalog).data[0]
+
+            time_stamps = lalpulsar.TimestampsFromSFTCatalog(ifo_catalog)
+            this_Tsft = int(round(1.0 / ifo_catalog.data[0].header.deltaF))
+            this_start_time = time_stamps.data[0].gpsSeconds
+            this_end_time = time_stamps.data[-1].gpsSeconds + this_Tsft
+
+            self.sftfilenames.append(
+                utils.get_official_sft_filename(
+                    ifo_name,
+                    time_stamps.length,  # ifo_catalog.length fails for NB case
+                    this_Tsft,
+                    this_start_time,
+                    this_end_time - this_start_time,
+                    self.label,
+                )
+            )
+
+            IFOs.append(ifo_name)
+            tstart.append(this_start_time)
+            tend.append(this_end_time)
+            Tsft.append(this_Tsft)
+
+        # Get the "overall" values of the search
+        Tsft = np.unique(Tsft)
+        if len(Tsft) != 1:
+            raise ValueError(f"SFTs contain different basetimes: {Tsft}")
+        if Tsft[0] != self.Tsft:
+            logger.warning(
+                f"Overwriting self.Tsft={self.Tsft}"
+                f" with value {Tsft[0]} read from noiseSFTs."
+            )
+        self.Tsft = Tsft[0]
+        self.tstart = min(tstart)
+        self.duration = max(tend) - self.tstart
+        self.detectors = ",".join(IFOs)
+
+    def _get_setup_from_timestamps(self):
+        """
+        If timestamps are given, use them to obtain relevant data parameters
+        (tstart, duration; but not detectors and Tsft as in the noiseSFTs case).
+
+        We ignore any extra columns (e.g. nanoseconds, end times)
+        after the first (SFT start times)
+        and implicitly assume that all SFTs are the same length.
+        """
+        self._parse_timestamps()
+        IFOs = self.detectors.split(",")
+        # at this point, it's definitely a comma-separated string
+        tsfiles = self.timestamps.split(",")
+        if len(IFOs) != len(tsfiles):
+            raise ValueError(
+                f"Length of detectors=='{self.detectors}'"
+                f" does not match that of timestamps=='{self.timestamps}'"
+                f" ({len(IFOs)}!={len(tsfiles)})"
+            )
+        tstart = []
+        tend = []
+        self.sftfilenames = []  # This refers to the MFD output!
+        for X, IFO in enumerate(IFOs):
+            tsX = np.genfromtxt(tsfiles[X], comments="%")
+            if tsX.ndim > 1:
+                logger.warning(
+                    f"Timestamps file {tsfiles[X]} has more than 1 column,"
+                    " we will ignore the rest."
+                )
+                tsX = tsX[:, 0]
+            if not tsX[0].is_integer() or not tsX[-1].is_integer():
+                logger.warning(
+                    "Detected non-integer timestamps in timestamp file."
+                    " We will floor start and end times to the nearest integer"
+                    " for the SFT name,"
+                    " and let lalpulsar_Makefakedata_v5 handle the rest."
+                )
+
+            this_start_time = int(tsX[0])
+            this_end_time = int(tsX[-1]) + self.Tsft
+            tstart.append(this_start_time)
+            tend.append(this_end_time)
+            self.sftfilenames.append(
+                utils.get_official_sft_filename(
+                    IFO,
+                    len(tsX),
+                    self.Tsft,
+                    this_start_time,
+                    this_end_time - this_start_time,
+                    self.label,
+                )
+            )
+        self.tstart = min(tstart)
+        self.duration = max(tend) - self.tstart
+
+    def _parse_timestamps(self):
+        """
+        Timestamps can be given either as a timestamp file or as an actual list
+        of timestamps. The former case ignores this function, whereas the second
+        one requires us to actually construct the timestamps file.
+        """
+        if self.detectors is None and not isinstance(self.timestamps, dict):
+            raise ValueError(
+                "Detector names must be given either as a key in"
+                " a `timestamps` dict or explicitly via `detectors`."
             )
-            if len(self.injectSqrtSX) != len(self.detector_names):
+
+        if isinstance(self.timestamps, str):
+            numTS = len(self.timestamps.split(","))
+            numDets = len(self.detectors.split(","))
+            if not numTS == numDets:
                 raise ValueError(
-                    "injectSqrtSX must be of same length as detector_names ({}!={})".format(
-                        len(self.injectSqrtSX), len(self.detector_names)
-                    )
+                    "Inconsistent length of comma-separated"
+                    f" `timestamps` and `detectors`: {numTS}!={numDets}"
                 )
-            FstatOAs.injectSqrtSX = lalpulsar.MultiNoiseFloor()
-            FstatOAs.injectSqrtSX.length = len(self.injectSqrtSX)
-            FstatOAs.injectSqrtSX.sqrtSn[
-                : FstatOAs.injectSqrtSX.length
-            ] = self.injectSqrtSX
-        else:
-            FstatOAs.injectSqrtSX = lalpulsar.FstatOptionalArgsDefaults.injectSqrtSX
-        self._set_min_max_cover_freqs()
-
-        logging.info("Initialising FstatInput")
-        self.FstatInput = lalpulsar.CreateFstatInput(
-            self.SFTCatalog,
-            self.minCoverFreq,
-            self.maxCoverFreq,
-            dFreq,
-            ephems,
-            FstatOAs,
-        )
+            return
 
-        logging.info("Initialising PulsarDoplerParams")
-        PulsarDopplerParams = lalpulsar.PulsarDopplerParams()
-        PulsarDopplerParams.refTime = self.tref
-        PulsarDopplerParams.Alpha = 1
-        PulsarDopplerParams.Delta = 1
-        PulsarDopplerParams.fkdot = np.array([0, 0, 0, 0, 0, 0, 0])
-        self.PulsarDopplerParams = PulsarDopplerParams
-
-        logging.info("Initialising FstatResults")
-        self.FstatResults = lalpulsar.FstatResults()
-
-        if self.BSGL:
-            if len(self.detector_names) < 2:
-                raise ValueError("Can't use BSGL with single detectors data")
+        if isinstance(self.timestamps, dict):
+            # Each key should correspond to `detectors` if given;
+            # otherwise, construct detectors from the given keys.
+            ifos = list(self.timestamps.keys())
+            input_timestamps = self.timestamps.values()
+
+            if self.detectors is not None:
+                ifos_in_detectors = self.detectors.split(",")
+                if np.setdiff1d(ifos, ifos_in_detectors).size:
+                    raise ValueError(
+                        f"Detector names in timestamps dictionary ({ifos}) "
+                        f"are inconsistent with detector names given via keyword ({ifos_in_detectors})."
+                    )
             else:
-                logging.info("Initialising BSGL")
+                self.detectors = ",".join(ifos)
+        else:
+            # Otherwise, assume it's a single list of timestamps,
+            # and replicate it for each detector.
+            ifos = self.detectors.split(",")
+            input_timestamps = [self.timestamps for i in ifos]
+
+        # If this point was reached, it means we should create timestamps files.
+        timestamp_files = []
+        for ind, ts in enumerate(input_timestamps):
+            output_file = os.path.join(
+                self.outdir, f"{self.label}_timestamps_{ifos[ind]}.csv"
+            )
+            np.savetxt(output_file, ts.reshape(-1, 1), fmt="%d")
+            timestamp_files.append(output_file)
+        self.timestamps = ",".join(timestamp_files)
 
-            # Tuning parameters - to be reviewed
-            numDetectors = 2
-            if hasattr(self, "nsegs"):
-                p_val_threshold = 1e-6
-                Fstar0s = np.linspace(0, 1000, 10000)
-                p_vals = scipy.special.gammaincc(2 * self.nsegs, Fstar0s)
-                Fstar0 = Fstar0s[np.argmin(np.abs(p_vals - p_val_threshold))]
-                if Fstar0 == Fstar0s[-1]:
-                    raise ValueError("Max Fstar0 exceeded")
-            else:
-                Fstar0 = 15.0
-            logging.info("Using Fstar0 of {:1.2f}".format(Fstar0))
-            oLGX = np.zeros(10)
-            oLGX[:numDetectors] = 1.0 / numDetectors
-            self.BSGLSetup = lalpulsar.CreateBSGLSetup(
-                numDetectors, Fstar0, oLGX, True, 1
-            )
-            self.twoFX = np.zeros(10)
-            self.whatToCompute += lalpulsar.FSTATQ_2F_PER_DET
-
-        if self.transientWindowType:
-            logging.info("Initialising transient parameters")
-            self.windowRange = lalpulsar.transientWindowRange_t()
-            transientWindowTypes = {
-                "none": lalpulsar.TRANSIENT_NONE,
-                "rect": lalpulsar.TRANSIENT_RECTANGULAR,
-                "exp": lalpulsar.TRANSIENT_EXPONENTIAL,
-            }
-            if self.transientWindowType in transientWindowTypes:
-                self.windowRange.type = transientWindowTypes[self.transientWindowType]
-            else:
-                raise ValueError(
-                    "Unknown window-type ({}) passed as input, [{}] allows.".format(
-                        self.transientWindowType, ", ".join(transientWindowTypes)
-                    )
-                )
+    def _basic_setup(self):
+        """Basic parameters handling, path setup etc."""
 
-            # default spacing
-            self.windowRange.dt0 = self.Tsft
-            self.windowRange.dtau = self.Tsft
-
-            # special treatment of window_type = none
-            # ==> replace by rectangular window spanning all the data
-            if self.windowRange.type == lalpulsar.TRANSIENT_NONE:
-                self.windowRange.t0 = int(self.minStartTime)
-                self.windowRange.t0Band = 0
-                self.windowRange.tau = int(self.maxStartTime - self.minStartTime)
-                self.windowRange.tauBand = 0
-            else:  # user-set bands and spacings
-                if getattr(self, "t0Band", None) is None:
-                    self.windowRange.t0Band = 0
-                else:
-                    if not isinstance(self.t0Band, int):
-                        logging.warn(
-                            "Casting non-integer t0Band={} to int...".format(
-                                self.t0Band
-                            )
-                        )
-                        self.t0Band = int(self.t0Band)
-                    self.windowRange.t0Band = self.t0Band
-                    if self.dt0:
-                        self.windowRange.dt0 = self.dt0
-                if getattr(self, "tauBand", None) is None:
-                    self.windowRange.tauBand = 0
-                else:
-                    if not isinstance(self.tauBand, int):
-                        logging.warn(
-                            "Casting non-integer tauBand={} to int...".format(
-                                self.tauBand
-                            )
-                        )
-                        self.tauBand = int(self.tauBand)
-                    self.windowRange.tauBand = self.tauBand
-                    if self.dtau:
-                        self.windowRange.dtau = self.dtau
-                    if self.tauMin is None:
-                        self.windowRange.tau = int(2 * self.Tsft)
-                    else:
-                        if not isinstance(self.tauMin, int):
-                            logging.warn(
-                                "Casting non-integer tauMin={} to int...".format(
-                                    self.tauMin
-                                )
-                            )
-                            self.tauMin = int(self.tauMin)
-                        self.windowRange.tau = self.tauMin
-
-            logging.info("Initialising transient FstatMap features...")
-            (
-                self.tCWFstatMapFeatures,
-                self.gpu_context,
-            ) = tcw.init_transient_fstat_map_features(
-                self.tCWFstatMapVersion == "pycuda", self.cudaDeviceName
-            )
-
-    def _set_min_max_cover_freqs(self):
-        # decide on which minCoverFreq and maxCoverFreq to use:
-        # either from direct user input, estimate_min_max_CoverFreq(), or SFTs
-        if self.sftfilepattern is not None:
-            minFreq_SFTs, maxFreq_SFTs = self._get_min_max_freq_from_SFTCatalog()
-        if (self.minCoverFreq is None) != (self.maxCoverFreq is None):
+        if not self.label.isalnum():
+            raise ValueError(
+                f"Label '{self.label}' is not alphanumeric,"
+                " which is incompatible with the SFTv3 naming specification"
+                " ( https://dcc.ligo.org/T040164-v2/public )."
+                " Please avoid underscores, hyphens etc."
+            )
+        if len(self.label) > 60:
             raise ValueError(
-                "Please use either both or none of [minCoverFreq,maxCoverFreq]."
+                f"Label {self.label} is too long to comply with SFT naming rules"
+                f" ({len(self.label)}>60)."
             )
-        elif (
-            self.minCoverFreq is None
-            and self.maxCoverFreq is None
-            and self.search_ranges is None
+
+        os.makedirs(self.outdir, exist_ok=True)
+        self.config_file_name = os.path.join(self.outdir, self.label + ".cff")
+        self.theta = np.array([self.phi, self.F0, self.F1, self.F2])
+
+        if self.h0 and np.any(
+            [getattr(self, k, None) is None for k in self.required_signal_parameters]
         ):
             raise ValueError(
-                "Please use either search_ranges or both of [minCoverFreq,maxCoverFreq]."
+                "If h0>0, also need all of ({:s})".format(
+                    ",".join(self.required_signal_parameters)
+                )
             )
-        elif self.minCoverFreq is None or self.maxCoverFreq is None:
-            logging.info(
-                "[minCoverFreq,maxCoverFreq] not provided, trying to estimate"
-                " from search ranges."
-            )
-            self.estimate_min_max_CoverFreq()
-        elif (self.minCoverFreq < 0.0) or (self.maxCoverFreq < 0.0):
-            if self.sftfilepattern is None:
+
+        incompatible_with_TS = ["tstart", "duration", "noiseSFTs"]
+        TS_required_options = ["Tsft"]
+        no_noiseSFTs_options = ["tstart", "duration", "Tsft", "detectors"]
+
+        if getattr(self, "timestamps", None) is not None:
+            if np.any(
+                [getattr(self, k, None) is not None for k in incompatible_with_TS]
+            ):
                 raise ValueError(
-                    "If sftfilepattern==None, cannot use negative values for"
-                    " minCoverFreq or maxCoverFreq (interpreted as offsets from"
-                    " min/max SFT frequency)."
-                    " Please use actual frequency values for both,"
-                    " or set both to None (automated estimation)."
-                )
-            if self.minCoverFreq < 0.0:
-                logging.info(
-                    "minCoverFreq={:f} provided, using as offset from min(SFTs).".format(
-                        self.minCoverFreq
-                    )
+                    "timestamps option is incompatible with"
+                    f" ({','.join(incompatible_with_TS)})."
                 )
-                # to set *above* min, since minCoverFreq is negative: subtract it
-                self.minCoverFreq = minFreq_SFTs - self.minCoverFreq
-            if self.maxCoverFreq < 0.0:
-                logging.info(
-                    "maxCoverFreq={:f} provided, using as offset from max(SFTs).".format(
-                        self.maxCoverFreq
-                    )
+            if np.any([getattr(self, k, None) is None for k in TS_required_options]):
+                raise ValueError(
+                    "With timestamps option, need also all of"
+                    f" ({','.join(TS_required_options)})."
                 )
-                # to set *below* max, since minCoverFreq is negative: add it
-                self.maxCoverFreq = maxFreq_SFTs + self.maxCoverFreq
-        if (self.sftfilepattern is not None) and (
-            (self.minCoverFreq < minFreq_SFTs) or (self.maxCoverFreq > maxFreq_SFTs)
-        ):
+            self._get_setup_from_timestamps()
+        elif self.noiseSFTs is not None:
+            logger.info(
+                "noiseSFTs is not None: Inferring tstart, duration, Tsft. "
+                "Input tstart and duration will be treated as SFT constraints "
+                "using lalpulsar.SFTConstraints; Tsft will be checked for "
+                "internal consistency accross input SFTs."
+            )
+            self._get_setup_from_noiseSFTs()
+        elif np.any([getattr(self, k, None) is None for k in no_noiseSFTs_options]):
             raise ValueError(
-                "[minCoverFreq,maxCoverFreq]=[{:f},{:f}] Hz incompatible with"
-                " SFT files content [{:f},{:f}] Hz".format(
-                    self.minCoverFreq, self.maxCoverFreq, minFreq_SFTs, maxFreq_SFTs
+                "Need either noiseSFTs, timestamps or all of ({:s}).".format(
+                    ",".join(no_noiseSFTs_options)
                 )
             )
-        logging.info(
-            "Using minCoverFreq={} and maxCoverFreq={}.".format(
-                self.minCoverFreq, self.maxCoverFreq
-            )
-        )
+        else:
+            self._get_setup_from_tstart_duration()
 
-    def _get_min_max_freq_from_SFTCatalog(self):
-        fAs = [d.header.f0 for d in self.SFTCatalog.data]
-        minFreq_SFTs = np.min(fAs)
-        fBs = [
-            d.header.f0 + (d.numBins - 1) * d.header.deltaF
-            for d in self.SFTCatalog.data
-        ]
-        maxFreq_SFTs = np.max(fBs)
-        return minFreq_SFTs, maxFreq_SFTs
+        self.sftfilenames = [os.path.join(self.outdir, fn) for fn in self.sftfilenames]
+        self.sftfilepath = ";".join(self.sftfilenames)
+
+        if self.tref is None:
+            self.tref = self.tstart
 
-    def estimate_min_max_CoverFreq(self):
-        # extract spanned spin-range at reference-time from the template-bank
-        # input self.search_ranges must be a dictionary of lists per search parameter
-        # which can be either [single_value], [min,max] or [min,max,step].
-        if type(self.search_ranges) is not dict:
-            raise ValueError("Need a dictionary for search_ranges!")
-        range_keys = list(self.search_ranges.keys())
-        required_keys = ["Alpha", "Delta", "F0"]
-        if len(np.setdiff1d(required_keys, range_keys)) > 0:
+        if getattr(self, "SFTWindowBeta", None):
             raise ValueError(
-                "Required keys not found in search_ranges: {}".format(
-                    np.setdiff1d(required_keys, range_keys)
-                )
+                "Option 'SFTWindowBeta' is defunct, please use 'SFTWindowParam'."
             )
-        for key in range_keys:
-            if (
-                type(self.search_ranges[key]) is not list
-                or len(self.search_ranges[key]) == 0
-                or len(self.search_ranges[key]) > 3
-            ):
+        if getattr(self, "SFTWindowType", None):
+            try:
+                lal.CheckNamedWindow(
+                    self.SFTWindowType, self.SFTWindowParam is not None
+                )
+            except RuntimeError:
                 raise ValueError(
-                    "search_ranges entry for {:s}"
-                    " is not a list of a known format"
-                    " (either [single_value], [min,max]"
-                    " or [min,max,step]): {}".format(key, self.search_ranges[key])
-                )
-        # start by constructing a DopplerRegion structure
-        # which will be needed to conservatively account for sky-position dependent
-        # Doppler shifts of the frequency range to be covered
-        searchRegion = lalpulsar.DopplerRegion()
-        # sky region
-        Alpha = self.search_ranges["Alpha"][0]
-        AlphaBand = (
-            self.search_ranges["Alpha"][1] - Alpha
-            if len(self.search_ranges["Alpha"]) >= 2
-            else 0.0
-        )
-        Delta = self.search_ranges["Delta"][0]
-        DeltaBand = (
-            self.search_ranges["Delta"][1] - Delta
-            if len(self.search_ranges["Delta"]) >= 2
-            else 0.0
-        )
-        searchRegion.skyRegionString = lalpulsar.SkySquare2String(
-            Alpha,
-            Delta,
-            AlphaBand,
-            DeltaBand,
-        )
-        searchRegion.refTime = self.tref
-        # frequency and spindowns
-        searchRegion.fkdot = np.zeros(lalpulsar.PULSAR_MAX_SPINS)
-        searchRegion.fkdotBand = np.zeros(lalpulsar.PULSAR_MAX_SPINS)
-        for k in range(3):
-            Fk = "F{:d}".format(k)
-            if Fk in range_keys:
-                searchRegion.fkdot[k] = self.search_ranges[Fk][0]
-                searchRegion.fkdotBand[k] = (
-                    self.search_ranges[Fk][1] - self.search_ranges[Fk][0]
-                    if len(self.search_ranges[Fk]) >= 2
-                    else 0.0
-                )
-        # now construct DopplerFullScan from searchRegion
-        scanInit = lalpulsar.DopplerFullScanInit()
-        scanInit.searchRegion = searchRegion
-        scanInit.stepSizes = lalpulsar.PulsarDopplerParams()
-        scanInit.stepSizes.refTime = self.tref
-        scanInit.stepSizes.Alpha = (
-            self.search_ranges["Alpha"][-1]
-            if len(self.search_ranges["Alpha"]) == 3
-            else 0.001  # fallback, irrelevant for band estimate but must be > 0
-        )
-        scanInit.stepSizes.Delta = (
-            self.search_ranges["Delta"][-1]
-            if len(self.search_ranges["Delta"]) == 3
-            else 0.001  # fallback, irrelevant for band estimate but must be > 0
-        )
-        scanInit.stepSizes.fkdot = np.zeros(lalpulsar.PULSAR_MAX_SPINS)
-        for k in range(3):
-            if Fk in range_keys:
-                Fk = "F{:d}".format(k)
-                scanInit.stepSizes.fkdot[k] = (
-                    self.search_ranges[Fk][-1]
-                    if len(self.search_ranges[Fk]) == 3
-                    else 0.0
-                )
-        scanInit.startTime = self.minStartTime
-        scanInit.Tspan = float(self.maxStartTime - self.minStartTime)
-        scanState = lalpulsar.InitDopplerFullScan(scanInit)
-        # now obtain the PulsarSpinRange extended over all relevant Doppler shifts
-        spinRangeRef = lalpulsar.PulsarSpinRange()
-        lalpulsar.GetDopplerSpinRange(spinRangeRef, scanState)
-        # optional: binary parameters
-        if "asini" in range_keys:
-            if len(self.search_ranges["asini"]) >= 2:
-                maxOrbitAsini = self.search_ranges["asini"][1]
-            else:
-                maxOrbitAsini = self.search_ranges["asini"][0]
-        else:
-            maxOrbitAsini = 0.0
-        if "period" in range_keys:
-            minOrbitPeriod = self.search_ranges["period"][0]
-        else:
-            minOrbitPeriod = 0.0
-        if "ecc" in range_keys:
-            if len(self.search_ranges["ecc"]) >= 2:
-                maxOrbitEcc = self.search_ranges["ecc"][1]
-            else:
-                maxOrbitEcc = self.search_ranges["ecc"][0]
-        else:
-            maxOrbitEcc = 0.0
-        # finally call the wrapped lalpulsar estimation function with the
-        # extended PulsarSpinRange and optional binary parameters
-        self.minCoverFreq, self.maxCoverFreq = helper_functions.get_covering_band(
-            tref=self.tref,
-            tstart=self.minStartTime,
-            tend=self.maxStartTime,
-            F0=spinRangeRef.fkdot[0],
-            F1=spinRangeRef.fkdot[1],
-            F2=spinRangeRef.fkdot[2],
-            F0band=spinRangeRef.fkdotBand[0],
-            F1band=spinRangeRef.fkdotBand[1],
-            F2band=spinRangeRef.fkdotBand[2],
-            maxOrbitAsini=maxOrbitAsini,
-            minOrbitPeriod=minOrbitPeriod,
-            maxOrbitEcc=maxOrbitEcc,
-        )
-
-    def get_fullycoherent_twoF(
-        self,
-        tstart,
-        tend,
-        F0,
-        F1,
-        F2,
-        Alpha,
-        Delta,
-        asini=None,
-        period=None,
-        ecc=None,
-        tp=None,
-        argp=None,
-    ):
-        """ Returns twoF or ln(BSGL) fully-coherently at a single point """
-        self.PulsarDopplerParams.fkdot = np.array([F0, F1, F2, 0, 0, 0, 0])
-        self.PulsarDopplerParams.Alpha = float(Alpha)
-        self.PulsarDopplerParams.Delta = float(Delta)
-        if self.binary:
-            self.PulsarDopplerParams.asini = float(asini)
-            self.PulsarDopplerParams.period = float(period)
-            self.PulsarDopplerParams.ecc = float(ecc)
-            self.PulsarDopplerParams.tp = float(tp)
-            self.PulsarDopplerParams.argp = float(argp)
-
-        lalpulsar.ComputeFstat(
-            self.FstatResults,
-            self.FstatInput,
-            self.PulsarDopplerParams,
-            1,
-            self.whatToCompute,
+                    "XLAL error on checking SFT window options."
+                    f" Likely either SFTWindowType={self.SFTWindowType} is not a recognised window name,"
+                    " or it requires also setting an SFTWindowParam."
+                )
+
+    @property
+    def tend(self):
+        """`
+        Defined as `self.start + self.duration`.
+
+        If stored as an attribute, there would be the risk of it going out of
+        sync with the other two values.
+        """
+        return self.tstart + self.duration
+
+    def _parse_args_consistent_with_mfd(self):
+        """Internal method to ensure parameters are handled consistently with MFD."""
+        self.signal_parameters = self.translate_keys_to_lal(
+            {
+                key: self.__dict__[key]
+                for key in self.signal_parameter_labels
+                if self.__dict__.get(key, None) is not None
+            }
         )
 
-        if not self.transientWindowType:
-            if self.BSGL is False:
-                return self.FstatResults.twoF[0]
-
-            twoF = np.float(self.FstatResults.twoF[0])
-            self.twoFX[0] = self.FstatResults.twoFPerDet(0)
-            self.twoFX[1] = self.FstatResults.twoFPerDet(1)
-            log10_BSGL = lalpulsar.ComputeBSGL(twoF, self.twoFX, self.BSGLSetup)
-            return log10_BSGL / np.log10(np.exp(1))
-
-        self.windowRange.t0 = int(tstart)  # TYPE UINT4
-        if self.windowRange.tauBand == 0:
-            # true single-template search also in transient params:
-            # actual (t0,tau) window was set with tstart, tend before
-            self.windowRange.tau = int(tend - tstart)  # TYPE UINT4
-
-        self.FstatMap, self.timingFstatMap = tcw.call_compute_transient_fstat_map(
-            self.tCWFstatMapVersion,
-            self.tCWFstatMapFeatures,
-            self.FstatResults.multiFatoms[0],
-            self.windowRange,
-        )
-        if self.tCWFstatMapVersion == "lal":
-            F_mn = self.FstatMap.F_mn.data
-        else:
-            F_mn = self.FstatMap.F_mn
+        self.signal_formats = {
+            key: self.gps_time_and_string_formats_as_LAL.get(key, ":1.18e")
+            for key in self.signal_parameters
+        }
 
-        twoF = 2 * np.max(F_mn)
-        if self.BSGL is False:
-            if np.isnan(twoF):
-                return 0
-            else:
-                return twoF
+    def calculate_fmin_Band(self):
+        """Set fmin and Band for the output SFTs to cover.
 
-        FstatResults_single = copy.copy(self.FstatResults)
-        FstatResults_single.numDetectors = 1
-        FstatResults_single.data = self.FstatResults.multiFatoms[0].data[0]
-        FS0 = lalpulsar.ComputeTransientFstatMap(
-            FstatResults_single.multiFatoms[0], self.windowRange, False
-        )
-        FstatResults_single.data = self.FstatResults.multiFatoms[0].data[1]
-        FS1 = lalpulsar.ComputeTransientFstatMap(
-            FstatResults_single.multiFatoms[0], self.windowRange, False
+        Either uses the user-provided `Band` and puts `F0` in the middle;
+        does nothing to later reuse the full bandwidth of `noiseSFTs`
+        (only if using MFDv5);
+        or if `F0!=None`, `noiseSFTs=None` and `Band=None`
+        it estimates a minimal band for just the injected signal:
+        F-stat covering band plus extra bins for demod default parameters.
+        This way a perfectly matched single-template `ComputeFstat` analysis
+        should run through perfectly on the returned SFTs.
+        For any wider-band or mismatched search, one needs to set `Band` manually.
+        If using MFDv4, at least `F0` is required even if `noiseSFTs!=None`.
+        """
+        if self.F0 is None and self.Band is not None:
+            raise ValueError("Band option can only be set if F0 is also given.")
+        elif self.F0 is not None and self.Band is not None:
+            self.fmin = self.F0 - 0.5 * self.Band
+        elif self.noiseSFTs and not self.mfd.endswith("v4"):
+            logger.info("Generating SFTs with full bandwidth from noiseSFTs.")
+        elif self.F0 is None:
+            err_msg = "Need F0 and Band,"
+            if not self.mfd.endswith("v4"):
+                err_msg += " or noiseSFTs,"
+            err_msg += " or at least F0 to auto-estimate bandwidth around it."
+            if self.mfd.endswith("v4"):
+                err_msg += (
+                    f" Since we are using {self.mfd}, we need this even with noiseSFTs."
+                )
+            raise ValueError(err_msg)
+        else:
+            extraBins = (
+                # matching extraBinsFull in XLALCreateFstatInput():
+                # https://lscsoft.docs.ligo.org/lalsuite/lalpulsar/_compute_fstat_8c_source.html#l00490
+                lalpulsar.FstatOptionalArgsDefaults.Dterms
+                + int(lalpulsar.FstatOptionalArgsDefaults.runningMedianWindow / 2)
+                + 1
+            )
+            logger.info(
+                "Estimating required SFT frequency range from properties"
+                " of signal to inject plus {:d} extra bins either side"
+                " (corresponding to default F-statistic settings).".format(extraBins)
+            )
+            minCoverFreq, maxCoverFreq = utils.get_covering_band(
+                tref=self.tref,
+                tstart=self.tstart,
+                tend=self.tend,
+                F0=self.F0,
+                F1=self.F1,
+                F2=self.F2,
+                F0band=0.0,
+                F1band=0.0,
+                F2band=0.0,
+                maxOrbitAsini=getattr(self, "asini", 0.0),
+                minOrbitPeriod=getattr(self, "period", 0.0),
+                maxOrbitEcc=getattr(self, "ecc", 0.0),
+            )
+            self.fmin = minCoverFreq - extraBins / self.Tsft
+            self.Band = maxCoverFreq - minCoverFreq + 2 * extraBins / self.Tsft
+        if hasattr(self, "fmin"):
+            logger.info(
+                "Generating SFTs with fmin={}, Band={}".format(self.fmin, self.Band)
+            )
+
+    def _get_single_config_line(self, i):
+        """Formatting for signal injection parameters."""
+        config_line = "[TS{}]\n".format(i)
+        config_line += "\n".join(
+            [
+                "{} = {{{}}}".format(key, self.signal_formats[key]).format(
+                    self.signal_parameters[key]
+                )
+                for key in self.signal_parameters.keys()
+            ]
         )
+        config_line += "\n"
 
-        # for now, use the Doppler parameter with
-        # multi-detector F maximised over t0,tau
-        # to return BSGL
-        # FIXME: should we instead compute BSGL over the whole F_mn
-        # and return the maximum of that?
-        idx_maxTwoF = np.argmax(F_mn)
-
-        self.twoFX[0] = 2 * FS0.F_mn.data[idx_maxTwoF]
-        self.twoFX[1] = 2 * FS1.F_mn.data[idx_maxTwoF]
-        log10_BSGL = lalpulsar.ComputeBSGL(twoF, self.twoFX, self.BSGLSetup)
-
-        return log10_BSGL / np.log10(np.exp(1))
-
-    def _set_up_cumulative_times(self, tstart, tend, num_segments):
-        """Construct time arrays to be used in cumulative twoF computations.
-
-        This allows calculate_twoF_cumulative and predict_twoF_cumulative to use
-        the same convention (although the number of segments on use is generally
-        different due to the computing time required by predict_twoF_cumulative).
+        return config_line
 
-        First segment is hardcoded to spann 2 * self.Tsft. Last segment embraces
-        the whole data stream.
+    def make_cff(self, verbose=False):
+        """Generates a .cff file including signal injection parameters.
+
+        This will be saved to `self.config_file_name`.
 
         Parameters
         ----------
-        tstart, tend: int or None
-            GPS times to restrict the range of data used;
-            if None: falls back to self.minStartTime and self.maxStartTime;
-            if outside those: auto-truncated
-        num_segments: int
-            Number of segments to split [tstart,tend] into
-        """
-        tstart = max(tstart, self.minStartTime) if tstart else self.minStartTime
-        tend = min(tend, self.maxStartTime) if tend else self.maxStartTime
-        min_duration = 2 * self.Tsft
-        max_duration = tend - tstart
-        cumulative_durations = np.linspace(min_duration, max_duration, num_segments)
+        verbose: boolean
+            If true, increase logging verbosity.
+        """
 
-        return tstart, tend, cumulative_durations
+        content = self._get_single_config_line(0)
 
-    def calculate_twoF_cumulative(
-        self,
-        F0,
-        F1,
-        F2,
-        Alpha,
-        Delta,
-        asini=None,
-        period=None,
-        ecc=None,
-        tp=None,
-        argp=None,
-        tstart=None,
-        tend=None,
-        num_segments=1000,
-    ):
-        """Calculate the cumulative twoF over subsets of the observation span.
+        if verbose:
+            logger.info("Injection parameters:")
+            logger.info(content.rstrip("\n"))
 
-        This means that we consider sub-"segments" of the [tstart,tend] interval,
-        each starting at the overall tstart and with increasing durations,
-        and compute the 2F for each of these, which for a true CW signal should
-        increase roughly with duration towards the full value.
+        if self._check_if_cff_file_needs_rewriting(content):
+            logger.info("Writing config file: {:s}".format(self.config_file_name))
+            config_file = open(self.config_file_name, "w+")
+            config_file.write(content)
+            config_file.close()
 
-        Parameters
-        ----------
-        F0, F1, F2, Alpha, Delta: float
-            Parameters at which to compute the cumulative twoF
-        asini, period, ecc, tp, argp: float, optional
-            Optional: Binary parameters at which to compute the cumulative 2F
-        tstart, tend: int or None
-            GPS times to restrict the range of data used;
-            if None: falls back to self.minStartTime and self.maxStartTime;
-            if outside those: auto-truncated
-        num_segments: int
-            Number of segments to split [tstart,tend] into
+    def check_cached_data_okay_to_use(self, cl_mfd):
+        """Check if SFT files already exist that can be re-used.
 
-        Returns
-        -------
-        cumulative_durations : ndarray of shape (num_segments,)
-            Offsets of each segment's tend from the overall tstart.
-        twoFs : ndarray of shape (num_segments,)
-            Values of twoF computed over
-            [[tstart,tstart+duration] for duration in cumulative_durations].
+        This does not check the actual data contents of the SFTs,
+        but only the following criteria:
+
+         * filename
+
+         * if injecting a signal, that the .cff file is older than the SFTs
+           (but its contents should have been checked separately)
 
+         * that the commandline stored in the (first) SFT header matches
+
+        Parameters
+        ----------
+        cl_mfd: str
+            The commandline we'd execute if not finding matching files.
         """
 
-        reset_old_window = None
-        if not self.transientWindowType:
-            reset_old_window = self.transientWindowType
-            self.transientWindowType = "rect"
-            self.init_computefstatistic()
+        need_new = "Will create new SFT file(s)."
 
-        tstart, tend, cumulative_durations = self._set_up_cumulative_times(
-            tstart, tend, num_segments
-        )
+        logger.info("Checking if we can re-use existing SFT data file(s)...")
+        for sftfile in self.sftfilenames:
+            if os.path.isfile(sftfile) is False:
+                logger.info(
+                    "...no SFT file matching '{}' found. {}".format(sftfile, need_new)
+                )
+                return False
+        logger.info("...OK: file(s) found matching '{}'.".format(sftfile))
+
+        if os.path.isfile(self.config_file_name):
+            if np.any(
+                [
+                    os.path.getmtime(sftfile) < os.path.getmtime(self.config_file_name)
+                    for sftfile in self.sftfilenames
+                ]
+            ):
+                logger.info(
+                    (
+                        "...the config file '{}' has been modified since"
+                        " creation of the SFT file(s) '{}'. {}"
+                    ).format(self.config_file_name, self.sftfilepath, need_new)
+                )
+                return False
+            else:
+                logger.info(
+                    "...OK: The config file '{}' is older than the SFT file(s)"
+                    " '{}'.".format(self.config_file_name, self.sftfilepath)
+                )
+                # NOTE: at this point we assume it's safe to re-use, since
+                # _check_if_cff_file_needs_rewriting()
+                # should have already been called before
+        elif "injectionSources" in cl_mfd:
+            raise RuntimeError(
+                "Commandline requires file '{}' but it is missing.".format(
+                    self.config_file_name
+                )
+            )
 
-        twoFs = [
-            self.get_fullycoherent_twoF(
-                tstart=tstart,
-                tend=tstart + duration,
-                F0=F0,
-                F1=F1,
-                F2=F2,
-                Alpha=Alpha,
-                Delta=Delta,
-                asini=asini,
-                period=period,
-                ecc=ecc,
-                tp=tp,
-                argp=argp,
+        logger.info("...checking new commandline against existing SFT header(s)...")
+        # here we check one SFT header from each SFT file,
+        # assuming that any concatenated file has been sanely constructed with
+        # matching CLs
+        for sftfile in self.sftfilenames:
+            catalog = lalpulsar.SFTdataFind(sftfile, None)
+            cl_old = utils.get_commandline_from_SFTDescriptor(catalog.data[0])
+            if len(cl_old) == 0:
+                logger.info(
+                    "......could not obtain comparison commandline from first SFT"
+                    " header in old file '{}'. {}".format(sftfile, need_new)
+                )
+                return False
+            if not utils.match_commandlines(cl_old, cl_mfd):
+                logger.info(
+                    "......commandlines unmatched for first SFT in old"
+                    " file '{}':".format(sftfile)
+                )
+                logger.info(cl_old)
+                logger.info(cl_mfd)
+                logger.info(need_new)
+                return False
+        logger.info("......OK: Commandline matched with old SFT header(s).")
+        logger.info(
+            "...all data consistency checks passed: Looks like existing"
+            " SFT data matches current options, will re-use it!"
+        )
+        return True
+
+    def _check_if_cff_file_needs_rewriting(self, content):
+        """Check if the .cff file has changed.
+
+        Returns True if the file should be overwritten - where possible avoid
+        overwriting to allow cached data to be used
+        """
+        logger.info("Checking if we can re-use injection config file...")
+        if os.path.isfile(self.config_file_name) is False:
+            logger.info("...no config file {} found.".format(self.config_file_name))
+            return True
+        else:
+            logger.info(
+                "...OK: config file {} already exists.".format(self.config_file_name)
             )
-            for duration in cumulative_durations
-        ]
 
-        if reset_old_window is not None:
-            self.transientWindowType = reset_old_window
-            self.init_computefstatistic()
+        with open(self.config_file_name, "r") as f:
+            file_content = f.read()
+            if file_content == content:
+                logger.info(
+                    "...OK: file contents match, no update of {} required.".format(
+                        self.config_file_name
+                    )
+                )
+                return False
+            else:
+                logger.info(
+                    "...file contents unmatched, updating {}.".format(
+                        self.config_file_name
+                    )
+                )
+                return True
 
-        return tstart, cumulative_durations, np.array(twoFs)
+    def make_data(self, verbose=False):
+        """A convenience wrapper to generate a cff file and then SFTs."""
+        if self.h0:
+            self.make_cff(verbose)
+        else:
+            logger.info("Got h0=0, not writing an injection .cff file.")
+        self.run_makefakedata()
 
-    def predict_twoF_cumulative(
-        self,
-        F0,
-        Alpha,
-        Delta,
-        h0,
-        cosi,
-        psi,
-        tstart=None,
-        tend=None,
-        num_segments=10,
-        **predict_fstat_kwargs,
-    ):
-        """Calculate expected 2F, with uncertainty, over subsets of the observation span.
+    def run_makefakedata(self):
+        """Generate the SFT data calling Makefakedata_v5 executable.
 
-        This yields the expected behaviour that calculate_twoF_cumulative() can
-        be compared against: 2F for CW signals increases with duration
-        as we take longer and longer subsets of the total observation span.
+        This first builds the full commandline,
+        then calls `check_cached_data_okay_to_use()`
+        to see if equivalent data files already exist,
+        and else runs the actual generation code.
+        """
+        cl_mfd = self._build_MFD_command_line()
+
+        check_ok = self.check_cached_data_okay_to_use(cl_mfd)
+        if check_ok is False:
+            utils.run_commandline(cl_mfd)
+            if not np.all([os.path.isfile(f) for f in self.sftfilenames]):
+                raise IOError(
+                    f"It seems we successfully ran {self.mfd},"
+                    f" but did not get the expected SFT file path(s): {self.sftfilepath}."
+                    f" What we have in the output directory '{self.outdir}' is:"
+                    f" {os.listdir(self.outdir)}"
+                )
+            logger.info(f"Successfully wrote SFTs to: {self.sftfilepath}")
+            logger.info("Now validating each SFT file...")
+            for sft in self.sftfilenames:
+                lalpulsar.ValidateSFTFile(sft)
+
+    def _build_MFD_command_line(self):
+        cl_mfd = [self.mfd]
+        cl_mfd.append("--outSingleSFT=TRUE")
+        cl_mfd.append('--outSFTdir="{}"'.format(self.outdir))
+        cl_mfd.append('--outLabel="{}"'.format(self.label))
+
+        if self.noiseSFTs is not None:
+            if self.sqrtSX and np.any(
+                [s > 0 for s in utils.parse_list_of_numbers(self.sqrtSX)]
+            ):
+                logger.warning(
+                    "In addition to using noiseSFTs, you are adding "
+                    "Gaussian noise with sqrtSX={} "
+                    "Please, make sure this is what you intend to do.".format(
+                        self.sqrtSX
+                    )
+                )
+            cl_mfd.append('--noiseSFTs="{}"'.format(self.noiseSFTs))
+        else:
+            cl_mfd.append(
+                "--IFOs={}".format(
+                    ",".join(['"{}"'.format(d) for d in self.detectors.split(",")])
+                )
+            )
+        if self.sqrtSX:
+            cl_mfd.append('--sqrtSX="{}"'.format(self.sqrtSX))
+
+        if self.SFTWindowType is not None:
+            cl_mfd.append('--SFTWindowType="{}"'.format(self.SFTWindowType))
+            cl_mfd.append("--SFTWindowParam={}".format(self.SFTWindowParam))
+        if getattr(self, "timestamps", None) is not None:
+            cl_mfd.append("--timestampsFiles={}".format(self.timestamps))
+        else:
+            cl_mfd.append("--startTime={}".format(self.tstart))
+            cl_mfd.append("--duration={}".format(self.duration))
+        if hasattr(self, "fmin") and self.fmin:
+            cl_mfd.append("--fmin={:.16g}".format(self.fmin))
+        if hasattr(self, "Band") and self.Band:
+            cl_mfd.append("--Band={:.16g}".format(self.Band))
+        cl_mfd.append("--Tsft={}".format(self.Tsft))
+        if self.h0:
+            cl_mfd.append('--injectionSources="{}"'.format(self.config_file_name))
+        earth_ephem = getattr(self, "earth_ephem", None)
+        sun_ephem = getattr(self, "sun_ephem", None)
+        if earth_ephem is not None:
+            cl_mfd.append('--ephemEarth="{}"'.format(earth_ephem))
+        if sun_ephem is not None:
+            cl_mfd.append('--ephemSun="{}"'.format(sun_ephem))
+        if self.randSeed:
+            cl_mfd.append("--randSeed={}".format(self.randSeed))
 
-        Parameters
-        ----------
-        F0, Alpha, Delta, h0, cosi, psi: float
-            Parameters at which to compute the cumulative predicted twoF
-        tstart, tend: int or None
-            GPS times to restrict the range of data used;
-            if None: falls back to self.minStartTime and self.maxStartTime;
-            if outside those: auto-truncated
-        num_segments: int
-            Number of segments to split [tstart,tend] into
-        predict_fstat_kwargs:
-            Other kwargs to be passed to helper_functions.predict_fstat.
+        return " ".join(cl_mfd)
 
-        Returns
-        -------
-        cumulative_durations : ndarray of shape (num_segments,)
-            Offsets of each segment's tend from the overall tstart.
-        pfs : ndarray of size (num_segments,)
-            Predicted 2F for each segment.
-        pfs_sigma : ndarray of size (num_segments,)
-            Standard deviations of predicted 2F.
+    def predict_fstat(self, assumeSqrtSX=None):
+        """Predict the expected F-statistic value for the injection parameters.
+
+        Through utils.predict_fstat(), this wraps
+        the PredictFstat executable.
 
+        Parameters
+        ----------
+        assumeSqrtSX: float, str or None
+            If None, PSD is estimated from self.sftfilepath.
+            Else, assume this stationary per-detector noise-floor instead.
+            Single float or str value: use same for all IFOs.
+            Comma-separated string: must match len(self.detectors)
+            and the data in self.sftfilepath.
+            Detectors will be paired to list elements following alphabetical order.
         """
-        tstart, tend, cumulative_durations = self._set_up_cumulative_times(
-            tstart, tend, num_segments
+        twoF_expected, twoF_sigma = utils.predict_fstat(
+            h0=self.h0,
+            cosi=self.cosi,
+            psi=self.psi,
+            Alpha=self.Alpha,
+            Delta=self.Delta,
+            F0=self.F0,
+            sftfilepattern=self.sftfilepath,
+            minStartTime=self.tstart,
+            duration=self.duration,
+            IFOs=self.detectors,
+            assumeSqrtSX=(assumeSqrtSX or self.sqrtSX),
+            tempory_filename=os.path.join(self.outdir, self.label + ".tmp"),
+            earth_ephem=self.earth_ephem,
+            sun_ephem=self.sun_ephem,
+            transientWindowType=self.transientWindowType,
+            transientStartTime=self.transientStartTime,
+            transientTau=self.transientTau,
         )
-        out = [
-            helper_functions.predict_fstat(
-                minStartTime=tstart,
-                duration=duration,
-                sftfilepattern=self.sftfilepattern,
-                h0=h0,
-                cosi=cosi,
-                psi=psi,
-                Alpha=Alpha,
-                Delta=Delta,
-                F0=F0,
-                **predict_fstat_kwargs,
-            )
-            for duration in cumulative_durations
-        ]
-        pfs, pfs_sigma = np.array(out).T
-        return tstart, cumulative_durations, pfs, pfs_sigma
+        return twoF_expected
+
 
-    def plot_twoF_cumulative(
+class BinaryModulatedWriter(Writer):
+    """Special Writer variant for simulating a CW signal for a source in a binary system."""
+
+    @utils.initializer
+    def __init__(
         self,
-        CFS_input,
-        PFS_input=None,
+        label="PyFstat",
         tstart=None,
-        tend=None,
-        num_segments_CFS=1000,
-        num_segments_PFS=10,
-        custom_ax_kwargs=None,
-        savefig=False,
-        label=None,
-        outdir=None,
-        **PFS_kwargs,
+        duration=None,
+        tref=None,
+        F0=None,
+        F1=0,
+        F2=0,
+        Alpha=None,
+        Delta=None,
+        tp=0.0,
+        argp=0.0,
+        asini=0.0,
+        ecc=0.0,
+        period=0.0,
+        h0=None,
+        cosi=None,
+        psi=0.0,
+        phi=0,
+        Tsft=1800,
+        outdir=".",
+        sqrtSX=None,
+        noiseSFTs=None,
+        SFTWindowType=None,
+        SFTWindowParam=None,
+        SFTWindowBeta=None,
+        Band=None,
+        detectors=None,
+        earth_ephem=None,
+        sun_ephem=None,
+        transientWindowType="none",
+        transientStartTime=None,
+        transientTau=None,
+        randSeed=None,
+        timestamps=None,
     ):
-        """Plot how 2F accumulates over time, and compare with expectation.
+        """
+        Most parameters are the same as for the basic `Writer` class,
+        only the additional ones are documented here:
 
         Parameters
         ----------
-        CFS_input: dict
-            self.calculate_twoF_cumulative input arguments.
-            (besides [tstart, tend, num_segments]).
-        PFS_input: dict
-            self.predict_twoF_cumulative input arguments
-            (besides [tstart, tend, num_segments]).
-            if None: do not calculate predicted 2F
-        tstart, tend: int or None
-            GPS times to restrict the range of data used;
-            if None: falls back to self.minStartTime and self.maxStartTime;
-            if outside those: auto-truncated
-        num_segments_(CFS|PFS) : int
-            Number of time segments to (compute|predict) twoF.
-        custom_ax_kwargs : dict
-            Optional axis formatting options.
-        savefig : bool
-            If true, save the figure in outdir.
-        label: str
-            Output filename (ignored unless savefig is True).
-        outdir: str
-            Output folder (ignored unless savefig is True).
-
-        Returns
-        -------
-        ax : matplotlib.axes._subplots_AxesSubplot, optional
-            The axes object containing the plot.
+        tp, argp, asini, ecc, period:
+            binary orbit parameters
         """
+        self.signal_parameter_labels = super().signal_parameter_labels + [
+            "tp",
+            "argp",
+            "asini",
+            "ecc",
+            "period",
+        ]
+        self.gps_time_and_string_formats_as_LAL["orbitTp"] = ":10.9f"
 
-        # Compute cumulative twoF
-        actual_tstart_CFS, taus_CFS, twoFs = self.calculate_twoF_cumulative(
+        super().__init__(
+            label=label,
             tstart=tstart,
-            tend=tend,
-            num_segments=num_segments_CFS,
-            **CFS_input,
+            duration=duration,
+            tref=tref,
+            F0=F0,
+            F1=F1,
+            F2=F2,
+            Alpha=Alpha,
+            Delta=Delta,
+            h0=h0,
+            cosi=cosi,
+            psi=psi,
+            phi=phi,
+            Tsft=Tsft,
+            outdir=outdir,
+            sqrtSX=sqrtSX,
+            SFTWindowType=SFTWindowType,
+            SFTWindowParam=SFTWindowParam,
+            SFTWindowBeta=SFTWindowBeta,
+            noiseSFTs=noiseSFTs,
+            Band=Band,
+            detectors=detectors,
+            earth_ephem=earth_ephem,
+            sun_ephem=sun_ephem,
+            transientWindowType=transientWindowType,
+            transientStartTime=transientStartTime,
+            transientTau=transientTau,
         )
-        taus_CFS_days = taus_CFS / 86400.0
 
-        # Set up plot-related objects
-        axis_kwargs = {
-            "xlabel": f"Days from $t_\\mathrm{{start}}={actual_tstart_CFS:.0f}$",
-            "ylabel": "$\\log_{10}(\\mathrm{BSGL})_{\\mathrm{cumulative}$"
-            if self.BSGL
-            else "$\\widetilde{2\\mathcal{F}}_{\\mathrm{cumulative}}$",
-            "xlim": (0, taus_CFS_days[-1]),
-        }
-        plot_label = (
-            f"Cumulative 2F {num_segments_CFS:d} segments"
-            f" ({(taus_CFS_days[1] - taus_CFS_days[0]):.2g} days per segment)"
-        )
 
-        if custom_ax_kwargs is not None:
-            for kwarg in "xlabel", "ylabel":
-                if kwarg in custom_ax_kwargs:
-                    logging.warning(
-                        f"Be careful, overwriting {kwarg} {axis_kwargs[kwarg]}"
-                        " with {custom_ax_kwargs[kwarg]}: Check out the units!"
-                    )
-            axis_kwargs.update(custom_ax_kwargs or {})
-            plot_label = custom_ax_kwargs.pop("label", plot_label)
+class LineWriter(Writer):
+    """Inject a simulated line-like detector artifact into SFT data.
 
-        fig, ax = plt.subplots()
-        ax.grid()
-        ax.set(**axis_kwargs)
-
-        ax.plot(taus_CFS_days, twoFs, label=plot_label, color="k")
-
-        # Predict cumulative twoF and plot if required
-        if PFS_input is not None:
-            actual_tstart_PFS, taus_PFS, pfs, pfs_sigma = self.predict_twoF_cumulative(
-                tstart=tstart,
-                tend=tend,
-                num_segments=num_segments_PFS,
-                **PFS_input,
-                **PFS_kwargs,
-            )
-            taus_PFS_days = taus_PFS / 86400.0
-            assert actual_tstart_CFS == actual_tstart_PFS, (
-                "CFS and PFS starting time differs: This shouldn't be the case. "
-                "Did you change conventions?"
-            )
-
-            ax.fill_between(
-                taus_PFS_days,
-                pfs - pfs_sigma,
-                pfs + pfs_sigma,
-                color="cyan",
-                label=(
-                    "Predicted $\\langle 2\\mathcal{F} \\rangle \\pm 1\\sigma$ band"
-                ),
-                zorder=-10,
-                alpha=0.2,
-            )
-
-        ax.legend(loc="best")
-        if savefig:
-            plt.tight_layout()
-            plt.savefig(os.path.join(outdir, label + "_twoFcumulative.png"))
-            plt.close()
-        return ax
-
-    def get_full_CFSv2_output(self, tstart, tend, F0, F1, F2, Alpha, Delta, tref):
-        """ Basic wrapper around CFSv2 to get the full (h0..) output """
-        cl_CFSv2 = "lalapps_ComputeFstatistic_v2 --minStartTime={} --maxStartTime={} --Freq={} --f1dot={} --f2dot={} --Alpha={} --Delta={} --refTime={} --DataFiles='{}' --outputLoudest='{}' --ephemEarth={} --ephemSun={}"
-        LoudestFile = "loudest.temp"
-        helper_functions.run_commandline(
-            cl_CFSv2.format(
-                tstart,
-                tend,
-                F0,
-                F1,
-                F2,
-                Alpha,
-                Delta,
-                tref,
-                self.sftfilepattern,
-                LoudestFile,
-                self.earth_ephem,
-                self.sun_ephem,
-            )
-        )
-        loudest = self.read_par(filename=LoudestFile, raise_error=False)
-        os.remove(LoudestFile)
-        return loudest
-
-    def write_atoms_to_file(self, fnamebase=""):
-        multiFatoms = getattr(self.FstatResults, "multiFatoms", None)
-        if multiFatoms and multiFatoms[0]:
-            dopplerName = lalpulsar.PulsarDopplerParams2String(self.PulsarDopplerParams)
-            # fnameAtoms = os.path.join(self.outdir,'Fstatatoms_%s.dat' % dopplerName)
-            fnameAtoms = fnamebase + "_Fstatatoms_%s.dat" % dopplerName
-            fo = lal.FileOpen(fnameAtoms, "w")
-            for hline in self.output_file_header:
-                lal.FilePuts("# {:s}\n".format(hline), fo)
-            lalpulsar.write_MultiFstatAtoms_to_fp(fo, multiFatoms[0])
-            del fo  # instead of lal.FileClose() which is not SWIG-exported
-        else:
-            raise RuntimeError(
-                "Cannot print atoms vector to file: no FstatResults.multiFatoms, or it is None!"
+    A (transient) line is defined as a constant amplitude and constant excess power artifact in the data.
+
+    In practice, it corresponds to a CW without Doppler or antenna-pattern-induced amplitude modulation.
+
+    NOTE: This functionality is implemented via `Makefakedata_v4`'s `lineFeature` option.
+    This version of MFD only supports one interferometer at a time.
+
+    NOTE: All signal parameters except for `h0`, `Freq`, `phi0` and transient parameters will be ignored.
+    """
+
+    mfd = "lalpulsar_Makefakedata_v4"
+    """The executable (older version that supports the `--lineFeature` option)."""
+
+    required_signal_parameters = [
+        "F0",
+        "phi",
+        "h0",
+    ]
+    """Required parameters for Makefakedata_v4 to success. Any other parameter is
+    silently given a default value by Makefakedata_v4.
+    """
+    signal_parameters_labels = required_signal_parameters + [
+        "transientWindowType",
+        "transientStartTime",
+        "transientTau",
+    ]
+    """Other signal parameters will be removed before passing to Makefakedata_v4."""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        if self.detectors is None:
+            raise ValueError("Makefakedata_v4 requires detector name to be given")
+        elif len(self.detectors.split(",")) > 1:
+            raise NotImplementedError(
+                "Makefakedata_v4 does not support more than one detector at a time. "
+                "Multi-detector behaviour can be reproduced by calling the procedure "
+                "on single-detector SFT sets once at a time."
             )
 
-    def __del__(self):
+    def _parse_args_consistent_with_mfd(self):
         """
-        In pyCuda case without autoinit,
-        we need to make sure the context is removed at the end
+        Adapt input arguments.
+        Take care of minor inconsistencies between MFD_v4 and MFD_v5
         """
-        if hasattr(self, "gpu_context") and self.gpu_context:
-            self.gpu_context.detach()
+        super()._parse_args_consistent_with_mfd()
+
+        # FIXME: There should be a smoother way to translate keys
+        lal_required_signal_parameters = self.translate_keys_to_lal(
+            dict(
+                zip(
+                    self.required_signal_parameters,
+                    [0] * len(self.required_signal_parameters),
+                )
+            )
+        )
 
+        if any(
+            key not in lal_required_signal_parameters for key in self.signal_parameters
+        ):
+            logger.warning(
+                "Injection of line artifacts only uses the following parameters:\n"
+                f"{self.required_signal_parameters}.\n"
+                "Any other parameter will be purged from this class now"
+            )
+            params_to_purge = list(
+                set(self.signal_parameters) - set(lal_required_signal_parameters)
+            )
+            logger.info(
+                "Purging input parameters that are not meaningful for LineWriter: {}".format(
+                    params_to_purge
+                )
+            )
+            for key in params_to_purge:
+                self.signal_parameters.pop(key)
 
-class SemiCoherentSearch(ComputeFstat):
-    """ A semi-coherent search """
+        if "transientTau" in self.signal_parameters:
+            self.signal_parameters["transientTauDays"] = (
+                self.signal_parameters.pop("transientTau") / 86400.0
+            )
+            self.signal_formats["transientTauDays"] = self.signal_formats.pop(
+                "transientTau"
+            )
+
+    def _build_MFD_command_line(self):
+        """Generate the SFT data calling Makefakedata_v4."""
 
-    @helper_functions.initializer
+        cl_mfd = [self.mfd]
+
+        cl_mfd.append("--lineFeature=TRUE")
+        cl_mfd.append("--outSingleSFT=TRUE")
+        cl_mfd.append('--outSFTbname="{}"'.format(self.sftfilenames[0]))
+        cl_mfd.append('--IFO="{}"'.format(self.detectors))
+
+        if self.noiseSFTs is not None and self.SFTWindowType is None:
+            raise ValueError(
+                "SFTWindowType is required when using noiseSFTs. "
+                "Please, make sure you understand the window function used "
+                "to produce noiseSFTs."
+            )
+        elif self.noiseSFTs is not None:
+            if self.sqrtSX and np.any(
+                [s > 0 for s in utils.parse_list_of_numbers(self.sqrtSX)]
+            ):
+                logger.warning(
+                    "In addition to using noiseSFTs, you are adding "
+                    "Gaussian noise with sqrtSX={} "
+                    "Please, make sure this is what you intend to do.".format(
+                        self.sqrtSX
+                    )
+                )
+            cl_mfd.append('--noiseSFTs="{}"'.format(self.noiseSFTs))
+        if self.sqrtSX:
+            cl_mfd.append("--noiseSqrtSh={}".format(self.sqrtSX))
+
+        if self.SFTWindowType is not None:
+            cl_mfd.append('--window="{}"'.format(self.SFTWindowType))
+            cl_mfd.append("--windowParam={}".format(self.SFTWindowParam))
+        cl_mfd.append("--startTime={}".format(self.tstart))
+        cl_mfd.append("--duration={}".format(self.duration))
+        if getattr(self, "fmin", None):
+            cl_mfd.append("--fmin={:.16g}".format(self.fmin))
+        if getattr(self, "Band", None):
+            cl_mfd.append("--Band={:.16g}".format(self.Band))
+        cl_mfd.append("--Tsft={}".format(self.Tsft))
+        if self.h0:
+            cl_mfd.append(
+                " ".join(
+                    f"--{key}={value:.16g}"
+                    for key, value in self.signal_parameters.items()
+                )
+            )
+            cl_mfd.append("--cosi=0")  # Required by MFDv4
+
+        earth_ephem = getattr(self, "earth_ephem", None)
+        sun_ephem = getattr(self, "sun_ephem", None)
+        if earth_ephem is not None:
+            cl_mfd.append('--ephemEarth="{}"'.format(earth_ephem))
+        if sun_ephem is not None:
+            cl_mfd.append('--ephemSun="{}"'.format(sun_ephem))
+        if self.randSeed:
+            cl_mfd.append("--randSeed={}".format(self.randSeed))
+
+        return " ".join(cl_mfd)
+
+
+class GlitchWriter(SearchForSignalWithJumps, Writer):
+    """Special Writer variant for simulating a CW signal containing a timing glitch."""
+
+    @utils.initializer
     def __init__(
         self,
-        label,
-        outdir,
-        tref,
-        nsegs=None,
-        sftfilepattern=None,
-        binary=False,
-        BSGL=False,
-        minStartTime=None,
-        maxStartTime=None,
+        label="PyFstat",
+        tstart=None,
+        duration=None,
+        dtglitch=None,
+        delta_phi=0,
+        delta_F0=0,
+        delta_F1=0,
+        delta_F2=0,
+        tref=None,
+        F0=None,
+        F1=0,
+        F2=0,
+        Alpha=None,
+        Delta=None,
+        h0=None,
+        cosi=None,
+        psi=0.0,
+        phi=0,
         Tsft=1800,
-        minCoverFreq=None,
-        maxCoverFreq=None,
-        search_ranges=None,
+        outdir=".",
+        sqrtSX=None,
+        noiseSFTs=None,
+        SFTWindowType=None,
+        SFTWindowParam=None,
+        SFTWindowBeta=None,
+        Band=None,
         detectors=None,
-        injectSources=None,
-        assumeSqrtSX=None,
-        SSBprec=None,
-        RngMedWindow=None,
         earth_ephem=None,
         sun_ephem=None,
+        transientWindowType="rect",
+        randSeed=None,
+        timestamps=None,
     ):
         """
+        Most parameters are the same as for the basic `Writer` class,
+        only the additional ones are documented here:
+
         Parameters
         ----------
-        label, outdir: str
-            A label and directory to read/write data from/to.
-        tref: int
-            GPS seconds of the reference time.
-        minStartTime, maxStartTime : int
-            Only use SFTs with timestamps starting from this range,
-            following the XLALCWGPSinRange convention:
-            half-open intervals [minStartTime,maxStartTime].
-            Also used to set up segment boundaries, i.e.
-            maxStartTime-minStartTime will be divided by nsegs
-            to obtain the per-segment coherence time Tcoh.
-        nsegs: int
-            The (fixed) number of segments
-        sftfilepattern: str
-            Pattern to match SFTs using wildcards (*?) and ranges [0-9];
-            multiple patterns can be given separated by colons.
-
-        For all other parameters, see pyfstat.ComputeFStat.
+        dtglitch: float or None
+            Time (in GPS seconds) of the glitch after `tstart`.
+            To create data without a glitch, set `dtglitch=None`.
+        delta_phi, delta_F0, delta_F1: float
+            Instantaneous glitch magnitudes in rad, Hz, and Hz/s respectively.
         """
 
-        self.fs_file_name = os.path.join(self.outdir, self.label + "_FS.dat")
         self.set_ephemeris_files(earth_ephem, sun_ephem)
-        self.transientWindowType = None  # will use semicoherentWindowRange instead
-        self.computeAtoms = True  # for semicoh 2F from ComputeTransientFstatMap()
-        self.tCWFstatMapVersion = "lal"
-        self.cudaDeviceName = None
-        self.init_computefstatistic()
-        self.init_semicoherent_parameters()
-
-    def _init_semicoherent_window_range(self):
-        """
-        Use this window to compute the semicoherent Fstat using TransientFstatMaps.
-        This way we are able to decouple the semicoherent computation from the
-        actual usage of a transient window.
-        """
-        self.semicoherentWindowRange = lalpulsar.transientWindowRange_t()
-        self.semicoherentWindowRange.type = lalpulsar.TRANSIENT_RECTANGULAR
-
-        # Range [t0, t0+t0Band] step dt0
-        self.semicoherentWindowRange.t0 = int(self.tboundaries[0])
-        self.semicoherentWindowRange.t0Band = int(
-            self.tboundaries[-1] - self.tboundaries[0] - self.Tcoh
-        )
-        self.semicoherentWindowRange.dt0 = int(self.Tcoh)
+        self._basic_setup()
+        self.calculate_fmin_Band()
 
-        # Range [tau, tau + tauBand] step dtau
-        # Watch out: dtau must be !=0, but tauBand==0 is allowed
-        self.semicoherentWindowRange.tau = int(self.Tcoh)
-        self.semicoherentWindowRange.tauBand = int(0)
-        self.semicoherentWindowRange.dtau = int(1)  # Irrelevant
-
-    def init_semicoherent_parameters(self):
-        logging.info(
-            (
-                "Initialising semicoherent parameters from"
-                " minStartTime={:d} to maxStartTime={:d} in {:d} segments..."
-            ).format(self.minStartTime, self.maxStartTime, self.nsegs)
-        )
-        self.tboundaries = np.linspace(
-            self.minStartTime, self.maxStartTime, self.nsegs + 1
-        )
-        self.Tcoh = self.tboundaries[1] - self.tboundaries[0]
-        logging.info(
-            ("Obtained {:d} segments of length Tcoh={:f}s (={:f}d).").format(
-                self.nsegs, self.Tcoh, self.Tcoh / 86400.0
+        shapes = np.array(
+            [
+                np.shape(x)
+                for x in [self.delta_phi, self.delta_F0, self.delta_F1, self.delta_F2]
+            ]
+        )
+        if not np.all(shapes == shapes[0]):
+            raise ValueError("all delta_* must be the same shape: {}".format(shapes))
+
+        for d in self.delta_phi, self.delta_F0, self.delta_F1, self.delta_F2:
+            if np.size(d) == 1:
+                d = np.atleast_1d(d)
+
+        if self.dtglitch is None:
+            self.tbounds = [self.tstart, self.tend]
+        else:
+            self.dtglitch = np.atleast_1d(self.dtglitch)
+            self.tglitch = self.tstart + self.dtglitch
+            self.tbounds = np.concatenate(([self.tstart], self.tglitch, [self.tend]))
+        logger.info("Using segment boundaries {}".format(self.tbounds))
+
+        tbs = np.array(self.tbounds)
+        self.durations = tbs[1:] - tbs[:-1]
+
+        self.delta_thetas = np.atleast_2d(
+            np.array([delta_phi, delta_F0, delta_F1, delta_F2]).T
+        )
+
+    def _get_base_template(self, i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref):
+        """FIXME: ported over from Writer,
+        should be replaced by a more elegant re-use of _parse_args_consistent_with_mfd
+        """
+        return """[TS{}]
+Alpha = {:1.18e}
+Delta = {:1.18e}
+h0 = {:1.18e}
+cosi = {:1.18e}
+psi = {:1.18e}
+phi0 = {:1.18e}
+Freq = {:1.18e}
+f1dot = {:1.18e}
+f2dot = {:1.18e}
+refTime = {:10.6f}"""
+
+    def _get_single_config_line_cw(
+        self, i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
+    ):
+        template = (
+            self._get_base_template(
+                i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
             )
+            + """\n"""
         )
-        logging.debug("Segment boundaries: {}".format(self.tboundaries))
-        if self.Tcoh < 2 * self.Tsft:
-            raise RuntimeError(
-                "Per-segment coherent time {} may not be < Tsft={}"
-                " to avoid degenerate F-statistic computations".format(
-                    self.Tcoh, self.Tsft
-                )
-            )
-        # FIXME: We can only easily do the next sanity check for a single
-        # detector, since self.SFT_timestamps is a joint list for multi-IFO case
-        # and the lower-level error checking of XLAL is complicated in that case.
-        # But even in the multi-IFO case, if the last segment does not include
-        # enough data, there will still be an error message (just uglier) from
-        # XLALComputeTransientFstatMap()
-        if (
-            (len(self.detector_names) == 1)
-            and hasattr(self, "SFT_timestamps")
-            and (self.tboundaries[-2] > self.SFT_timestamps[-2])
-        ):
-            raise RuntimeError(
-                "Each segment must contain at least 2 SFTs to avoid degenerate"
-                " F-statistic computations, but last segment start time {}"
-                " is after second-to-last SFT timestamp {}.".format(
-                    self.tboundaries[-2], self.SFT_timestamps[-2]
-                )
-            )
-        self._init_semicoherent_window_range()
+        return template.format(i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref)
 
-    def get_semicoherent_det_stat(
+    def _get_single_config_line_tcw(
         self,
+        i,
+        Alpha,
+        Delta,
+        h0,
+        cosi,
+        psi,
+        phi,
         F0,
         F1,
         F2,
-        Alpha,
-        Delta,
-        asini=None,
-        period=None,
-        ecc=None,
-        tp=None,
-        argp=None,
-        record_segments=False,
+        tref,
+        window,
+        transientStartTime,
+        transientTau,
     ):
-        """ Returns twoF or ln(BSGL) semi-coherently at a single point """
-
-        self.PulsarDopplerParams.fkdot = np.array([F0, F1, F2, 0, 0, 0, 0])
-        self.PulsarDopplerParams.Alpha = float(Alpha)
-        self.PulsarDopplerParams.Delta = float(Delta)
-        if self.binary:
-            self.PulsarDopplerParams.asini = float(asini)
-            self.PulsarDopplerParams.period = float(period)
-            self.PulsarDopplerParams.ecc = float(ecc)
-            self.PulsarDopplerParams.tp = float(tp)
-            self.PulsarDopplerParams.argp = float(argp)
-
-        lalpulsar.ComputeFstat(
-            self.FstatResults,
-            self.FstatInput,
-            self.PulsarDopplerParams,
-            1,
-            self.whatToCompute,
+        template = (
+            self._get_base_template(
+                i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
+            )
+            + """
+transientWindowType = {:s}
+transientStartTime = {:10.0f}
+transientTau = {:10.0f}\n"""
+        )
+        return template.format(
+            i,
+            Alpha,
+            Delta,
+            h0,
+            cosi,
+            psi,
+            phi,
+            F0,
+            F1,
+            F2,
+            tref,
+            window,
+            transientStartTime,
+            transientTau,
         )
 
-        twoF_per_segment = self._get_per_segment_twoF()
-        twoF = twoF_per_segment.sum()
-
-        if np.isnan(twoF):
-            logging.debug(
-                "NaNs in per-segment 2F treated as zero"
-                " and semi-coherent 2F re-computed."
+    def _get_single_config_line(
+        self,
+        i,
+        Alpha,
+        Delta,
+        h0,
+        cosi,
+        psi,
+        phi,
+        F0,
+        F1,
+        F2,
+        tref,
+        window,
+        transientStartTime,
+        transientTau,
+    ):
+        if window == "none":
+            return self._get_single_config_line_cw(
+                i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
             )
-            twoF_per_segment = np.nan_to_num(twoF_per_segment, nan=0.0)
-            twoF = twoF_per_segment.sum()
-
-        if record_segments:
-            self.twoF_per_segment = twoF_per_segment
-
-        if self.BSGL is False:
-            return twoF
         else:
-            for X in range(self.FstatResults.numDetectors):
-                FstatResults_single = copy.copy(self.FstatResults)
-                FstatResults_single.numDetectors = 1
-                FstatResults_single.data = self.FstatResults.multiFatoms[0].data[X]
-                FSX = lalpulsar.ComputeTransientFstatMap(
-                    FstatResults_single.multiFatoms[0],
-                    self.semicoherentWindowRange,
-                    False,
-                )
-                twoFX_per_segment = 2 * FSX.F_mn.data[:, 0]
-                self.twoFX[X] = twoFX_per_segment.sum()
-                if np.isnan(self.twoFX[X]):
-                    logging.debug(
-                        "NaNs in per-segment per-detector 2F treated as zero"
-                        " and sum re-computed."
-                    )
-                    twoFX_per_segment = np.nan_to_num(twoFX_per_segment, nan=0.0)
-                    self.twoFX[X] = twoFX_per_segment.sum()
-            log10_BSGL = lalpulsar.ComputeBSGL(twoF, self.twoFX, self.BSGLSetup)
-            ln_BSGL = log10_BSGL * np.log(10.0)
-            if np.isnan(ln_BSGL):
-                logging.debug("NaNs in semi-coherent ln(BSGL) treated as zero")
-                ln_BSGL = 0.0
-            return ln_BSGL
-
-    def _get_per_segment_twoF(self):
-        Fmap = lalpulsar.ComputeTransientFstatMap(
-            self.FstatResults.multiFatoms[0], self.semicoherentWindowRange, False
-        )
-        twoF = 2 * Fmap.F_mn.data[:, 0]
-        return twoF
-
+            return self._get_single_config_line_tcw(
+                i,
+                Alpha,
+                Delta,
+                h0,
+                cosi,
+                psi,
+                phi,
+                F0,
+                F1,
+                F2,
+                tref,
+                window,
+                transientStartTime,
+                transientTau,
+            )
 
-class SearchForSignalWithJumps(BaseSearchClass):
-    """ A class which just adds some useful methods for glitches or timing noise """
+    def make_cff(self, verbose=False):
+        """Generates a .cff file including signal injection parameters, including a glitch.
 
-    def _shift_matrix(self, n, dT):
-        """Generate the shift matrix
+        This will be saved to `self.config_file_name`.
 
         Parameters
         ----------
-        n : int
-            The dimension of the shift-matrix to generate
-        dT : float
-            The time delta of the shift matrix
-
-        Returns
-        -------
-        m : ndarray, shape (n,)
-            The shift matrix.
-
+        verbose: boolean
+            If true, increase logging verbosity.
         """
-        m = np.zeros((n, n))
-        factorial = np.math.factorial
-        for i in range(n):
-            for j in range(n):
-                if i == j:
-                    m[i, j] = 1.0
-                elif i > j:
-                    m[i, j] = 0.0
-                else:
-                    if i == 0:
-                        m[i, j] = 2 * np.pi * float(dT) ** (j - i) / factorial(j - i)
-                    else:
-                        m[i, j] = float(dT) ** (j - i) / factorial(j - i)
-        return m
 
-    def _shift_coefficients(self, theta, dT):
-        """Shift a set of coefficients by dT
+        thetas = self._calculate_thetas(self.theta, self.delta_thetas, self.tbounds)
+
+        content = ""
+        for i, (t, d, ts) in enumerate(zip(thetas, self.durations, self.tbounds[:-1])):
+            line = self._get_single_config_line(
+                i,
+                self.Alpha,
+                self.Delta,
+                self.h0,
+                self.cosi,
+                self.psi,
+                t[0],
+                t[1],
+                t[2],
+                t[3],
+                self.tref,
+                self.transientWindowType,
+                ts,
+                d,
+            )
+
+            content += line
+
+        if verbose:
+            logger.info("Injection parameters:")
+            logger.info(content.rstrip("\n"))
+
+        if self._check_if_cff_file_needs_rewriting(content):
+            logger.info("Writing config file: {:s}".format(self.config_file_name))
+            config_file = open(self.config_file_name, "w+")
+            config_file.write(content)
+            config_file.close()
+
+
+class FrequencyModulatedArtifactWriter(Writer):
+    """Specialized Writer variant to generate SFTs containing simulated instrumental artifacts.
+
+    Contrary to the main `Writer` class, this calls the older
+    `Makefakedata_v4` executable which supports the special `--lineFeature` option.
+    See `lalpulsar_Makefakedata_v4 --help`
+    for more detailed help with some of the parameters.
+    """
 
+    @utils.initializer
+    def __init__(
+        self,
+        label,
+        outdir=".",
+        tstart=700000000,
+        duration=86400,
+        F0=30,
+        F1=0,
+        tref=None,
+        h0=10,
+        Tsft=1800,
+        sqrtSX=0.0,
+        Band=4,
+        Pmod=lal.DAYSID_SI,
+        Pmod_phi=0,
+        Pmod_amp=1,
+        Alpha=None,
+        Delta=None,
+        detectors=None,
+        earth_ephem=None,
+        sun_ephem=None,
+        randSeed=None,
+    ):
+        """
         Parameters
         ----------
-        theta : array-like, shape (n,)
-            Vector of the expansion coefficients to transform starting from the
-            lowest degree e.g [phi, F0, F1,...].
-        dT : float
-            Difference between the two reference times as tref_new - tref_old.
+        label: string
+            A human-readable label to be used in naming the output files.
+        outdir: str
+            The directory where files are written to.
+            Default: current working directory.
+        tstart: int
+            Starting GPS epoch of the data set.
+        duration: int
+            Duration (in GPS seconds) of the total data set.
+        F0: float
+            Frequency of the artifact.
+        F1: float
+            Frequency drift of the artifact.
+        tref: float or None
+            Reference time for simulated signals.
+            Default is `None`, which sets the reference time to `tstart`.
+        h0: float
+            Amplitude of the artifact.
+        Tsft: int
+            The SFT duration in seconds.
+            Will be ignored if `noiseSFTs` are given.
+        sqrtSX: float
+            Background detector noise level.
+        Band: float
+            Output SFTs cover
+            `[F0-Band/2,F0+Band/2]`.
+        Pmod: float
+            Modulation period of the artifact.
+        Pmod_phi, Pmod_amp: float
+            Additional parameters for modulation of the artifact.
+        Alpha, Delta: float or None
+            If not none: add an orbital modulation to the artifact
+            corresponding to a signal from that sky position, in radians.
+        detectors: str or None
+            Comma-separated list of detectors to generate data for.
+        earth_ephem, sun_ephem: str or None
+            Paths of the two files containing positions of Earth and Sun.
+            If None, will check standard sources as per
+            utils.get_ephemeris_files().
+        randSeed: int or None
+            Optionally fix the random seed of Gaussian noise generation
+            for reproducibility.
+        """
+
+        self.phi = 0
+        self.F2 = 0
+
+        self.cosi = 0
+        self.noiseSFTs = None
+
+        if type(self.detectors) is not str or len(self.detectors.split(",")) > 1:
+            raise ValueError("'detectors' must be  a single-IFO string")
+
+        # The _basic_setup() method inherited from Writer
+        # requires additional CW signal parameters if h0>0,
+        # which an artifact doesn't need to have,
+        # hence we temporarily unset it here as a workaround
+        # and restore it after the method call.
+        h0_value = self.h0
+        self.h0 = None
+        self._basic_setup()
+        self.h0 = h0_value
 
-        Returns
-        -------
-        theta_new : ndarray, shape (n,)
-            Vector of the coefficients as evaluated as the new reference time.
-        """
-        n = len(theta)
-        m = self._shift_matrix(n, dT)
-        return np.dot(m, theta)
-
-    def _calculate_thetas(self, theta, delta_thetas, tbounds, theta0_idx=0):
-        """Calculates the set of thetas given delta_thetas, the jumps
-
-        This is used when generating data containing glitches or timing noise.
-        Specifically, the source parameters of the signal are not constant in
-        time, but jump by `delta_theta` at `tbounds`.
+        self.set_ephemeris_files(earth_ephem, sun_ephem)
+        self.tstart = int(tstart)
+        self.duration = int(duration)
+
+        if os.path.isdir(self.outdir) is False:
+            os.makedirs(self.outdir)
+        if tref is None:
+            raise ValueError("Input `tref` not specified")
+
+        self.nsfts = int(np.ceil(self.duration / self.Tsft))
+        self.calculate_fmin_Band()
+
+        self.Fmax = F0
+
+        if Alpha is not None and Delta is not None:
+            self.n = np.array(
+                [
+                    np.cos(Alpha) * np.cos(Delta),
+                    np.sin(Alpha) * np.cos(Delta),
+                    np.sin(Delta),
+                ]
+            )
+
+    def get_frequency(self, t):
+        """Evolve the artifact frequency in time.
+
+        This includes a drift term and optionally,
+        if `Alpha` and `Delta` are not `None`,
+        a simulated orbital modulation.
 
         Parameters
         ----------
-        theta : array_like
-            The source parameters of size (n,).
-        delta_thetas : array_like
-            The jumps in the source parameters of size (m, n) where m is the
-            number of jumps.
-        tbounds : array_like
-            Time boundaries of the jumps of size (m+2,).
-        theta0_idx : int
-            Index of the segment for which the theta are defined.
+        t: float
+            Time stamp to evaluate the frequency at.
 
         Returns
         -------
-        ndarray
-            The set of thetas, shape (m+1, n).
-
+        f: float
+            Frequency at time `t`.
         """
-        thetas = [theta]
-        for i, dt in enumerate(delta_thetas):
-            if i < theta0_idx:
-                pre_theta_at_ith_glitch = self._shift_coefficients(
-                    thetas[0], tbounds[i + 1] - self.tref
-                )
-                post_theta_at_ith_glitch = pre_theta_at_ith_glitch - dt
-                thetas.insert(
-                    0,
-                    self._shift_coefficients(
-                        post_theta_at_ith_glitch, self.tref - tbounds[i + 1]
-                    ),
-                )
-
-            elif i >= theta0_idx:
-                pre_theta_at_ith_glitch = self._shift_coefficients(
-                    thetas[i], tbounds[i + 1] - self.tref
-                )
-                post_theta_at_ith_glitch = pre_theta_at_ith_glitch + dt
-                thetas.append(
-                    self._shift_coefficients(
-                        post_theta_at_ith_glitch, self.tref - tbounds[i + 1]
-                    )
+        DeltaFDrift = self.F1 * (t - self.tref)
+
+        phir = 2 * np.pi * t / self.Pmod + self.Pmod_phi
+
+        if self.Alpha is not None and self.Delta is not None:
+            spin_posvel = lalpulsar.PosVel3D_t()
+            orbit_posvel = lalpulsar.PosVel3D_t()
+            det = lal.CachedDetectors[4]
+            ephems = lalpulsar.InitBarycenter(self.earth_ephem, self.sun_ephem)
+            lalpulsar.DetectorPosVel(
+                spin_posvel,
+                orbit_posvel,
+                lal.LIGOTimeGPS(t),
+                det,
+                ephems,
+                lalpulsar.DETMOTION_ORBIT,
+            )
+            # Pos and vel returned in units of c
+            DeltaFOrbital = np.dot(self.n, orbit_posvel.vel) * self.Fmax
+
+            if self.detectors == "H1":
+                Lambda = lal.LHO_4K_DETECTOR_LATITUDE_RAD
+            elif self.detectors == "L1":
+                Lambda = lal.LLO_4K_DETECTOR_LATITUDE_RAD
+            else:
+                raise ValueError(
+                    "Simulated orbital modulation"
+                    " (triggered by Alpha, Delta parameters)"
+                    " is currently only supported for detectors H1 or L1."
                 )
-        self.thetas_at_tref = thetas
-        return thetas
 
+            DeltaFSpin = (
+                self.Pmod_amp
+                * lal.REARTH_SI
+                / lal.C_SI
+                * 2
+                * np.pi
+                / self.Pmod
+                * (np.cos(self.Delta) * np.cos(Lambda) * np.sin(self.Alpha - phir))
+                * self.Fmax
+            )
+        else:
+            DeltaFOrbital = 0
+            DeltaFSpin = 2 * np.pi * self.Pmod_amp / self.Pmod * np.cos(phir)
 
-class SemiCoherentGlitchSearch(SearchForSignalWithJumps, ComputeFstat):
-    """A semi-coherent glitch search
+        f = self.F0 + DeltaFDrift + DeltaFOrbital + DeltaFSpin
+        return f
 
-    This implements a basic `semi-coherent glitch F-stat in which the data
-    is divided into segments either side of the proposed glitches and the
-    fully-coherent F-stat in each segment is summed to give the semi-coherent
-    F-stat
-    """
+    def get_h0(self, t):
+        """Evaluate the artifact amplitude at a given time.
+
+        NOTE: Here it's actually implemented as a constant!
 
-    @helper_functions.initializer
-    def __init__(
-        self,
-        label,
-        outdir,
-        tref,
-        minStartTime,
-        maxStartTime,
-        Tsft=1800,
-        nglitch=1,
-        sftfilepattern=None,
-        theta0_idx=0,
-        BSGL=False,
-        minCoverFreq=None,
-        maxCoverFreq=None,
-        search_ranges=None,
-        assumeSqrtSX=None,
-        detectors=None,
-        SSBprec=None,
-        RngMedWindow=None,
-        injectSources=None,
-        earth_ephem=None,
-        sun_ephem=None,
-    ):
-        """
         Parameters
         ----------
-        label, outdir: str
-            A label and directory to read/write data from/to.
-        tref, minStartTime, maxStartTime: int
-            GPS seconds of the reference time, and start and end of the data.
-        nglitch: int
-            The (fixed) number of glitches; this can zero, but occasionally
-            this causes issue (in which case just use ComputeFstat).
-        sftfilepattern: str
-            Pattern to match SFTs using wildcards (*?) and ranges [0-9];
-            mutiple patterns can be given separated by colons.
-        theta0_idx, int
-            Index (zero-based) of which segment the theta refers to - uyseful
-            if providing a tight prior on theta to allow the signal to jump
-            too theta (and not just from)
+        t: float
+            Time stamp to evaluate at.
 
-        For all other parameters, see pyfstat.ComputeFStat.
+        Returns
+        -------
+        h0: float
+            Amplitude at time `t`.
         """
+        return self.h0
 
-        self.fs_file_name = os.path.join(self.outdir, self.label + "_FS.dat")
-        self.set_ephemeris_files(earth_ephem, sun_ephem)
-        self.transientWindowType = "rect"
-        self.t0Band = None
-        self.tauBand = None
-        self.tCWFstatMapVersion = "lal"
-        self.cudaDeviceName = None
-        self.binary = False
-        self.init_computefstatistic()
-
-    def get_semicoherent_nglitch_twoF(self, F0, F1, F2, Alpha, Delta, *args):
-        """ Returns the semi-coherent glitch summed twoF """
-
-        args = list(args)
-        tboundaries = [self.minStartTime] + args[-self.nglitch :] + [self.maxStartTime]
-        delta_F0s = args[-3 * self.nglitch : -2 * self.nglitch]
-        delta_F1s = args[-2 * self.nglitch : -self.nglitch]
-        delta_F2 = np.zeros(len(delta_F0s))
-        delta_phi = np.zeros(len(delta_F0s))
-        theta = [0, F0, F1, F2]
-        delta_thetas = np.atleast_2d(
-            np.array([delta_phi, delta_F0s, delta_F1s, delta_F2]).T
-        )
+    def concatenate_sft_files(self):
+        """Merges the individual SFT files via splitSFTs executable."""
 
-        thetas = self._calculate_thetas(
-            theta, delta_thetas, tboundaries, theta0_idx=self.theta0_idx
+        SFTFilename = (
+            f"{self.detectors[0]}-{self.nsfts}_{self.detectors}_{self.Tsft}SFT_mfdv4"
+        )
+        # We don't try to reproduce the NB filename convention exactly,
+        # as there could be always rounding offsets with the number of bins,
+        # instead we use wildcards there.
+        outfreq = int(np.floor(self.fmin))
+        outwidth = int(np.floor(self.Band))
+        SFTFilename += f"_NBF{outfreq:04d}Hz*W{outwidth:04d}Hz*"
+        SFTFilename += f"-{self.tstart}-{self.duration}.sft"
+        SFTFile_fullpath = os.path.join(self.outdir, SFTFilename)
+        if os.path.isfile(SFTFile_fullpath):
+            logger.info(
+                f"Removing previous file(s) {SFTFile_fullpath} (no caching implemented)."
+            )
+            os.remove(SFTFile_fullpath)
+
+        inpattern = os.path.join(self.tmp_outdir, "*sft")
+        cl_splitSFTS = "lalpulsar_splitSFTs"
+        cl_splitSFTS += " -fs {} -fb {} -fe {} -n {} -- {}".format(
+            self.fmin, self.Band, self.fmin + self.Band, self.outdir, inpattern
+        )
+        utils.run_commandline(cl_splitSFTS)
+        utils.run_commandline(f"rm -r {self.tmp_outdir}")
+        outglob = glob.glob(SFTFile_fullpath)
+        if len(outglob) != 1:
+            raise IOError(
+                "Expected to produce exactly 1 merged file"
+                f" matching pattern '{SFTFile_fullpath}',"
+                f" but got {len(outglob)} matches: {outglob}"
+                " Something went wrong!"
+            )
+        self.sftfilepath = outglob[0]
+        logger.info(f"Successfully wrote SFTs to: {self.sftfilepath}")
+
+    def pre_compute_evolution(self):
+        """Precomputes evolution parameters for the artifact.
+
+        This computes midtimes, frequencies, phases and amplitudes
+        over the list of SFT timestamps.
+        """
+        logger.info("Precomputing evolution parameters")
+        self.lineFreqs = []
+        self.linePhis = []
+        self.lineh0s = []
+        self.mid_times = []
+
+        linePhi = 0
+        lineFreq_old = 0
+
+        for i in trange(self.nsfts):
+            mid_time = self.tstart + (i + 0.5) * self.Tsft
+            lineFreq = self.get_frequency(mid_time)
+
+            self.mid_times.append(mid_time)
+            self.lineFreqs.append(lineFreq)
+            self.linePhis.append(
+                linePhi + np.pi * self.Tsft * (lineFreq_old + lineFreq)
+            )
+            self.lineh0s.append(self.get_h0(mid_time))
+
+            lineFreq_old = lineFreq
+
+    def make_ith_sft(self, i):
+        """Call MFDv4 to create a single SFT with evolved artifact parameters."""
+        self.run_makefakedata_v4(
+            self.mid_times[i],
+            self.lineFreqs[i],
+            self.linePhis[i],
+            self.lineh0s[i],
+            self.tmp_outdir,
         )
 
-        twoFSum = 0
-        for i, theta_i_at_tref in enumerate(thetas):
-            ts, te = tboundaries[i], tboundaries[i + 1]
-            if te - ts > 1800:
-                twoFVal = self.get_fullycoherent_twoF(
-                    ts,
-                    te,
-                    theta_i_at_tref[1],
-                    theta_i_at_tref[2],
-                    theta_i_at_tref[3],
-                    Alpha,
-                    Delta,
-                )
-                twoFSum += twoFVal
-
-        if np.isfinite(twoFSum):
-            return twoFSum
-        else:
-            return -np.inf
+    def make_data(self, num_threads=1):
+        """Create a full multi-SFT data set.
 
-    def compute_glitch_fstat_single(
-        self, F0, F1, F2, Alpha, Delta, delta_F0, delta_F1, tglitch
-    ):
-        """Returns the semi-coherent glitch summed twoF for nglitch=1
+        This loops over SFTs and generate them serially or in parallel,
+        then contatenates the results together at the end.
 
-        Note: OBSOLETE, used only for testing
+        Parameters
+        ----------
+        num_processes: int
+            Number threads to use when running in parallel.
+            Verbatim implementation of the former `args.N`.
         """
 
-        theta = [F0, F1, F2]
-        delta_theta = [delta_F0, delta_F1, 0]
-        tref = self.tref
+        self.tmp_outdir = os.path.join(self.outdir, self.label + "_tmp")
+        if os.path.isdir(self.tmp_outdir) is True:
+            raise ValueError(
+                "Temporary directory {} already exists, please rename".format(
+                    self.tmp_outdir
+                )
+            )
+        else:
+            os.makedirs(self.tmp_outdir)
 
-        theta_at_glitch = self._shift_coefficients(theta, tglitch - tref)
-        theta_post_glitch_at_glitch = theta_at_glitch + delta_theta
-        theta_post_glitch = self._shift_coefficients(
-            theta_post_glitch_at_glitch, tref - tglitch
-        )
+        self.pre_compute_evolution()
 
-        twoFsegA = self.get_fullycoherent_twoF(
-            self.minStartTime, tglitch, theta[0], theta[1], theta[2], Alpha, Delta
-        )
+        logger.info("Generating SFTs")
 
-        if tglitch == self.maxStartTime:
-            return twoFsegA
+        if num_threads > 1 and pkgutil.find_loader("pathos") is not None:
+            import pathos.pools
 
-        twoFsegB = self.get_fullycoherent_twoF(
-            tglitch,
-            self.maxStartTime,
-            theta_post_glitch[0],
-            theta_post_glitch[1],
-            theta_post_glitch[2],
-            Alpha,
-            Delta,
-        )
+            logger.info("Using {} threads".format(num_threads))
+            try:
+                with pathos.pools.ProcessPool(num_threads) as p:
+                    list(
+                        tqdm(
+                            p.imap(self.make_ith_sft, list(range(self.nsfts))),
+                            total=self.nsfts,
+                        )
+                    )
+            except KeyboardInterrupt:
+                p.terminate()
+        else:
+            logger.info(
+                "No multiprocessing requested or `pathos` not install, cont."
+                " without multiprocessing"
+            )
+            for i in trange(self.nsfts):
+                self.make_ith_sft(i)
+
+        self.concatenate_sft_files()
+
+    def run_makefakedata_v4(self, mid_time, lineFreq, linePhi, h0, tmp_outdir):
+        """Generate SFT data using the MFDv4 code with the --lineFeature option."""
+        cl_mfd = []
+        cl_mfd.append("lalpulsar_Makefakedata_v4")
+        cl_mfd.append("--outSingleSFT=FALSE")
+        cl_mfd.append('--outSFTbname="{}"'.format(tmp_outdir))
+        cl_mfd.append("--IFO={}".format(self.detectors))
+        cl_mfd.append('--noiseSqrtSh="{}"'.format(self.sqrtSX))
+        cl_mfd.append("--startTime={:0.0f}".format(mid_time - self.Tsft / 2.0))
+        cl_mfd.append("--refTime={:0.0f}".format(mid_time))
+        cl_mfd.append("--duration={}".format(self.Tsft))
+        cl_mfd.append("--fmin={:.16g}".format(self.fmin))
+        cl_mfd.append("--Band={:.16g}".format(self.Band))
+        cl_mfd.append("--Tsft={}".format(self.Tsft))
+        cl_mfd.append("--Freq={}".format(lineFreq))
+        cl_mfd.append("--phi0={}".format(linePhi))
+        cl_mfd.append("--h0={}".format(h0))
+        cl_mfd.append("--cosi={}".format(self.cosi))
+        cl_mfd.append("--lineFeature=TRUE")
+        earth_ephem = getattr(self, "earth_ephem", None)
+        sun_ephem = getattr(self, "sun_ephem", None)
+        if earth_ephem is not None:
+            cl_mfd.append('--ephemEarth="{}"'.format(earth_ephem))
+        if sun_ephem is not None:
+            cl_mfd.append('--ephemSun="{}"'.format(sun_ephem))
+        if self.randSeed:
+            cl_mfd.append("--randSeed={}".format(self.randSeed))
+        cl_mfd = " ".join(cl_mfd)
+        utils.run_commandline(cl_mfd)
 
-        return twoFsegA + twoFsegB
 
+class FrequencyAmplitudeModulatedArtifactWriter(FrequencyModulatedArtifactWriter):
+    """A variant of FrequencyModulatedArtifactWriter with evolving amplitude."""
 
-class DeprecatedClass:
-    def __new__(cls, *args, **kwargs):
-        logging.warning(
-            f"The {cls.__name__} class is no longer maintained"
-            " and will be removed in an upcoming release of PyFstat!"
-            " If you rely on this class and/or are interested in taking over"
-            " maintenance, please report an issue at:"
-            " https://github.com/PyFstat/PyFstat/issues",
-        )
-        return super().__new__(cls, *args, **kwargs)
+    def get_h0(self, t):
+        """Evaluate the artifact amplitude at a given time.
 
+        NOTE: Here it's actually changing over time!
 
-class DefunctClass:
-    last_supported_version = None
-    pr_welcome = True
-
-    def __new__(cls, *args, **kwargs):
-        defunct_message = f"The {cls.__name__} class is no longer included in PyFstat!"
-        if cls.last_supported_version:
-            defunct_message += (
-                f" Last supported version was {cls.last_supported_version}."
-            )
-        if cls.pr_welcome:
-            defunct_message += " Pull requests to reinstate the class are welcome."
-        raise NotImplementedError(defunct_message)
+        Parameters
+        ----------
+        t: float
+            Time stamp to evaluate at.
+
+        Returns
+        -------
+        h0: float
+            Amplitude at time `t`.
+        """
+        return self.h0 * np.sin(2 * np.pi * t / self.Pmod + self.Pmod_phi)
```

### Comparing `PyFstat-1.9.0/pyfstat/helper_functions.py` & `PyFstat-2.0.0/pyfstat/tcw_fstat_map_funcs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,903 +1,901 @@
-"""
-Provides helpful functions to facilitate ease-of-use of pyfstat
+"""Additional helper functions dealing with transient-CW F(t0,tau) maps.
+
+See Prix, Giampanis & Messenger (PRD 84, 023007, 2011):
+https://arxiv.org/abs/1104.1704
+for the algorithm in general
+and Keitel & Ashton (CQG 35, 205003, 2018):
+https://arxiv.org/abs/1805.05652
+for a detailed discussion of the GPU implementation.
 """
 
-import os
-import sys
-import subprocess
-import argparse
+# optional imports
+import importlib as imp
 import logging
-import inspect
-import peakutils
-import shutil
-from functools import wraps
-from scipy.stats.distributions import ncx2
-import numpy as np
-import lal
-import lalpulsar
-from ._version import get_versions
+import os
+from time import time
 
-# workaround for matplotlib on X-less remote logins
-if "DISPLAY" in os.environ:
-    import matplotlib.pyplot as plt
-else:
-    logging.info(
-        'No $DISPLAY environment variable found, so importing \
-                  matplotlib.pyplot with non-interactive "Agg" backend.'
-    )
-    import matplotlib
+import numpy as np
 
-    matplotlib.use("Agg")
-    import matplotlib.pyplot as plt
+logger = logging.getLogger(__name__)
 
 
-def set_up_optional_tqdm():
-    try:
-        from tqdm import tqdm
-    except ImportError:
+def _optional_import(modulename, shorthand=None):
+    """
+    Import a module/submodule only if it's available.
 
-        def tqdm(x, *args, **kwargs):
-            return x
+    using importlib instead of __import__
+    because the latter doesn't handle sub.modules
 
-    return tqdm
+    Also including a special check to fail more gracefully
+    when CUDA_DEVICE is set to too high a number.
+    """
 
+    if shorthand is None:
+        shorthand = modulename
+        shorthandbit = ""
+    else:
+        shorthandbit = " as " + shorthand
 
-def set_up_matplotlib_defaults():
-    plt.switch_backend("Agg")
-    plt.rcParams["text.usetex"] = shutil.which("latex") is not None
-    plt.rcParams["axes.formatter.useoffset"] = False
-
-
-def set_up_command_line_arguments():
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="Increase output verbosity [logging.DEBUG]",
-    )
-    parser.add_argument(
-        "-q",
-        "--quite",
-        action="store_true",
-        help="Decrease output verbosity [logging.WARNING]",
-    )
-    parser.add_argument(
-        "--no-interactive", help="Don't use interactive", action="store_true"
-    )
-    parser.add_argument(
-        "-c",
-        "--clean",
-        action="store_true",
-        help="Force clean data, never use cached data",
-    )
-    fu_parser = parser.add_argument_group(
-        "follow-up options", "Options related to MCMCFollowUpSearch"
-    )
-    fu_parser.add_argument(
-        "-s",
-        "--setup-only",
-        action="store_true",
-        help="Only generate the setup file, don't run",
-    )
-    fu_parser.add_argument(
-        "--no-template-counting",
-        action="store_true",
-        help="No counting of templates, useful if the setup is predefined",
-    )
-    parser.add_argument(
-        "-N",
-        type=int,
-        default=3,
-        metavar="N",
-        help="Number of threads to use when running in parallel",
-    )
-    parser.add_argument("unittest_args", nargs="*")
-    args, unknown = parser.parse_known_args()
-    sys.argv[1:] = args.unittest_args
+    try:
+        globals()[shorthand] = imp.import_module(modulename)
+        logger.debug("Successfully imported module %s%s." % (modulename, shorthandbit))
+        success = True
+    except ImportError:
+        logger.debug("Failed to import module {:s}.".format(modulename))
+        success = False
 
-    if args.quite or args.no_interactive:
+    return success
 
-        def tqdm(x, *args, **kwargs):
-            return x
 
-    else:
-        tqdm = set_up_optional_tqdm()
+class pyTransientFstatMap:
+    """
+    Simplified object class for a F(t0,tau) F-stat map.
 
-    logger = logging.getLogger()
-    stream_handler = logging.StreamHandler()
-    stream_handler.setFormatter(
-        logging.Formatter("%(asctime)s %(levelname)-8s: %(message)s", datefmt="%H:%M")
-    )
+    This is based on LALSuite's transientFstatMap_t type,
+    replacing the gsl matrix with a numpy array.
 
-    if args.quite:
-        logger.setLevel(logging.WARNING)
-        stream_handler.setLevel(logging.WARNING)
-    elif args.verbose:
-        logger.setLevel(logging.DEBUG)
-        stream_handler.setLevel(logging.DEBUG)
-    else:
-        logger.setLevel(logging.INFO)
-        stream_handler.setLevel(logging.INFO)
+    Here, `t0` is a transient start time,
+    `tau` is a transient duration parameter,
+    and `F(t0,tau)` is the F-statistic (not 2F)! evaluated
+    for a signal with those parameters
+    (and an implicit window function, which is not stored inside this object).
 
-    logger.addHandler(stream_handler)
-    return args, tqdm
+    The 'map' covers a range of different `(t0,tau)` pairs.
 
-
-def get_ephemeris_files():
-    """ Returns the earth_ephem and sun_ephem """
-    config_file = os.path.join(os.path.expanduser("~"), ".pyfstat.conf")
-    env_var = "LALPULSAR_DATADIR"
-    please = "Please provide the ephemerides paths when initialising searches."
-    if os.path.isfile(config_file):
-        d = {}
-        with open(config_file, "r") as f:
-            for line in f:
-                k, v = line.split("=")
-                k = k.replace(" ", "")
-                for item in [" ", "'", '"', "\n"]:
-                    v = v.replace(item, "")
-                d[k] = v
-        try:
-            earth_ephem = d["earth_ephem"]
-            sun_ephem = d["sun_ephem"]
-        except KeyError:
-            logging.warning(
-                "No [earth/sun]_ephem found in " + config_file + ". " + please
-            )
-            earth_ephem = None
-            sun_ephem = None
-    elif env_var in list(os.environ.keys()):
-        ephem_version = "DE405"
-        earth_ephem = os.path.join(
-            os.environ[env_var], "earth00-40-{:s}.dat.gz".format(ephem_version)
-        )
-        sun_ephem = os.path.join(
-            os.environ[env_var], "sun00-40-{:s}.dat.gz".format(ephem_version)
-        )
-        if not (os.path.isfile(earth_ephem) and os.path.isfile(sun_ephem)):
-            earth_ephem = os.path.join(
-                os.environ[env_var], "earth00-19-{:s}.dat.gz".format(ephem_version)
-            )
-            sun_ephem = os.path.join(
-                os.environ[env_var], "sun00-19-{:s}.dat.gz".format(ephem_version)
+    Attributes
+    ----------
+    F_mn: np.ndarray
+        2D array of F values (not 2F!),
+        with `m` an index over start-times `t0`,
+        and  `n` an index over duration parameters `tau`,
+        in steps of `dt0`  in `[t0,  t0+t0Band]`,
+        and `dtau` in `[tau, tau+tauBand]`.
+    maxF: float
+        Maximum of F (not 2F!) over the array.
+    t0_ML: float
+        Maximum likelihood estimate of the transient start time `t0`.
+    tau_ML: float
+        Maximum likelihood estimate of the transient duration `tau`.
+    lnBtSG: float
+        Natural log of the marginalised transient Bayes factor.
+        NOTE: This is always initialised as `nan`,
+        and you have to call `get_lnBtSG()` to get its actual value.
+    """
+
+    def __init__(
+        self,
+        N_t0Range=None,
+        N_tauRange=None,
+        transientFstatMap_t=None,
+        from_file=None,
+    ):
+        """
+        The class can be initialized with either
+        a pair of (N_t0Range,N_tauRange),
+        from a lalpulsar object,
+        or reading from a file.
+
+        Parameters
+        ----------
+        N_t0Range: int
+            Number of `t0` values covered.
+        N_tauRange: int
+            Number of `tau` values covered.
+        transientFstatMap_t: lalpulsar.transientFstatMap_t
+            pre-allocated matrix from lalpulsar to initialise from.
+        from_file: str or None
+            Text file,
+            compatible with `lalpulsar.write_transientFstatMap_to_fp()` format,
+            to load and initialise from.
+        """
+        if transientFstatMap_t and from_file:  # pragma: no cover
+            raise ValueError(
+                "Please choose either a transientFstatMap_t or file to init from."
             )
-            if not (os.path.isfile(earth_ephem) and os.path.isfile(sun_ephem)):
-                logging.warning(
-                    "Default [earth/sun]00-[19/40]-" + ephem_version + " ephemerides "
-                    "not found in the " + os.environ[env_var] + " directory. " + please
+        elif transientFstatMap_t:
+            self._init_from_lalpulsar_type(transientFstatMap_t)
+        elif from_file:
+            self.read_from_file(from_file)
+        else:
+            if not N_t0Range or not N_tauRange:
+                raise ValueError(
+                    "Need either a transientFstatMap_t or a pair of (N_t0Range, N_tauRange)!."
                 )
-                earth_ephem = None
-                sun_ephem = None
-    else:
-        logging.warning(
-            "No " + config_file + " file or $" + env_var + " environment "
-            "variable found. " + please
-        )
-        earth_ephem = None
-        sun_ephem = None
-    return earth_ephem, sun_ephem
-
-
-def round_to_n(x, n):
-    if not x:
-        return 0
-    power = -int(np.floor(np.log10(abs(x)))) + (n - 1)
-    factor = 10 ** power
-    return round(x * factor) / factor
-
-
-def texify_float(x, d=2):
-    if x == 0:
-        return 0
-    if type(x) == str:
-        return x
-    x = round_to_n(x, d)
-    if 0.01 < abs(x) < 100:
-        return str(x)
-    else:
-        power = int(np.floor(np.log10(abs(x))))
-        stem = np.round(x / 10 ** power, d)
-        if d == 1:
-            stem = int(stem)
-        return r"${}{{\times}}10^{{{}}}$".format(stem, power)
-
-
-def initializer(func):
-    """ Decorator function to automatically assign the parameters to self """
-    argspec = inspect.getfullargspec(func)
-
-    @wraps(func)
-    def wrapper(self, *args, **kargs):
-        for name, arg in list(zip(argspec.args[1:], args)) + list(kargs.items()):
-            setattr(self, name, arg)
-
-        for name, default in zip(reversed(argspec.args), reversed(argspec.defaults)):
-            if not hasattr(self, name):
-                setattr(self, name, default)
-
-        func(self, *args, **kargs)
-
-    return wrapper
-
-
-def get_peak_values(frequencies, twoF, threshold_2F, F0=None, F0range=None):
-    if F0:
-        cut_idxs = np.abs(frequencies - F0) < F0range
-        frequencies = frequencies[cut_idxs]
-        twoF = twoF[cut_idxs]
-    idxs = peakutils.indexes(twoF, thres=1.0 * threshold_2F / np.max(twoF))
-    F0maxs = frequencies[idxs]
-    twoFmaxs = twoF[idxs]
-    freq_err = frequencies[1] - frequencies[0]
-    return F0maxs, twoFmaxs, freq_err * np.ones(len(idxs))
-
-
-def get_comb_values(F0, frequencies, twoF, period, N=4):
-    if period == "sidereal":
-        period = 23 * 60 * 60 + 56 * 60 + 4.0616
-    elif period == "terrestrial":
-        period = 86400
-    freq_err = frequencies[1] - frequencies[0]
-    comb_frequencies = [n * 1 / period for n in range(-N, N + 1)]
-    comb_idxs = [np.argmin(np.abs(frequencies - F0 - F)) for F in comb_frequencies]
-    return comb_frequencies, twoF[comb_idxs], freq_err * np.ones(len(comb_idxs))
-
-
-def compute_P_twoFstarcheck(twoFstarcheck, twoFcheck, M0, plot=False):
-    """ Returns the unnormalised pdf of twoFstarcheck given twoFcheck """
-    upper = 4 + twoFstarcheck + 0.5 * (2 * (4 * M0 + 2 * twoFcheck))
-    rho2starcheck = np.linspace(1e-1, upper, 500)
-    integrand = ncx2.pdf(twoFstarcheck, 4 * M0, rho2starcheck) * ncx2.pdf(
-        twoFcheck, 4, rho2starcheck
-    )
-    if plot:
-        fig, ax = plt.subplots()
-        ax.plot(rho2starcheck, integrand)
-        fig.savefig("test")
-    return np.trapz(integrand, rho2starcheck)
-
-
-def compute_pstar(twoFcheck_obs, twoFstarcheck_obs, m0, plot=False):
-    M0 = 2 * m0 + 1
-    upper = 4 + twoFcheck_obs + (2 * (4 * M0 + 2 * twoFcheck_obs))
-    twoFstarcheck_vals = np.linspace(1e-1, upper, 500)
-    P_twoFstarcheck = np.array(
-        [
-            compute_P_twoFstarcheck(twoFstarcheck, twoFcheck_obs, M0)
-            for twoFstarcheck in twoFstarcheck_vals
-        ]
-    )
-    C = np.trapz(P_twoFstarcheck, twoFstarcheck_vals)
-    idx = np.argmin(np.abs(twoFstarcheck_vals - twoFstarcheck_obs))
-    if plot:
-        fig, ax = plt.subplots()
-        ax.plot(twoFstarcheck_vals, P_twoFstarcheck)
-        ax.fill_between(twoFstarcheck_vals[: idx + 1], 0, P_twoFstarcheck[: idx + 1])
-        ax.axvline(twoFstarcheck_vals[idx])
-        fig.savefig("test")
-    pstar_l = np.trapz(P_twoFstarcheck[: idx + 1] / C, twoFstarcheck_vals[: idx + 1])
-    return 2 * np.min([pstar_l, 1 - pstar_l])
+            self.F_mn = np.zeros((N_t0Range, N_tauRange), dtype=np.float32)
+            # Initializing maxF to a negative value ensures
+            # that we always update at least once and hence return
+            # sane t0_d_ML, tau_d_ML
+            # even if there is only a single bin where F=0 happens.
+            self.maxF = float(-1.0)
+            self.t0_ML = float(0.0)
+            self.tau_ML = float(0.0)
+        self.lnBtSG = np.nan
+
+    def _init_from_lalpulsar_type(self, transientFstatMap_t):
+        """This essentially just strips out a redundant member level from the lalpulsar structure.
+
+        Parameters
+        ----------
+        transientFstatMap_t: str
+            The lalpulsar structure to extract data from.
+        """
+        self.F_mn = transientFstatMap_t.F_mn.data
+        self.maxF = transientFstatMap_t.maxF
+        self.t0_ML = transientFstatMap_t.t0_ML
+        self.tau_ML = transientFstatMap_t.tau_ML
+
+    def read_from_file(self, file):
+        """Read F_mn map from a text file and set all other fields.
+
+        Apart from optional header lines (`#` comments),
+        the format has to be consistent with lalpulsar.write_transientFstatMap_to_fp()
+        and the `write_F_mn_to_file()` method of this class itself:
+        with the columns `[t0[s], tau[s], 2F]`.
+        NOTE that the file is expected to provide 2F,
+        so the values will be halved to obtain F for storage in this class.
+
+        Parameters
+        ----------
+        file: str
+            Name of the file to load from.
+        """
+        inarray = np.genfromtxt(
+            file,
+            comments="#",
+        )
+        t0s = np.unique(inarray[:, 0])
+        taus = np.unique(inarray[:, 1])
+        self.F_mn = (0.5 * inarray[:, 2]).reshape(len(t0s), len(taus))
+        maxidx = np.argmax(inarray[:, 2])
+        self.t0_ML = inarray[maxidx, 0]
+        self.tau_ML = inarray[maxidx, 1]
+        self.maxF = 0.5 * inarray[maxidx, 2]
+
+    def get_maxF_idx(self):
+        """Gets the 2D-unravelled index pair of the maximum of the F_mn map
+
+        Returns
+        -------
+        idx: tuple
+            The m,n indices of the map entry with maximal F value.
+        """
+        return np.unravel_index(np.argmax(self.F_mn), self.F_mn.shape)
+
+    def get_lnBtSG(self):
+        """Compute (natural log of the) transient-CW Bayes-factor B_tSG = P(x|HyptS)/P(x|HypG).
+
+        Here HypG = Gaussian noise hypothesis, HyptS = transient-CW signal hypothesis.
+
+        B_tSG is marginalized over start-time and timescale of transient CW signal,
+        using given type and parameters of transient window range.
+
+        This is a python port of the `lalpulsar.ComputeTransientBstat` implementation,
+        replacing `for` loops by numpy operations.
+        """
+        # The first 2 lines are equivalent to `logBhat = logsumexp(self.F_mn)`,
+        # but since we have `self.maxF` already precomputed,
+        # doing the manual version of the same stable summation trick is slightly faster.
+        sum_eB = np.sum(np.exp(-(self.maxF - self.F_mn)))
+        logBhat = self.maxF + np.log(sum_eB)  # unnormalized Bhat
+        normBh = 70.0 / np.prod(
+            self.F_mn.shape
+        )  # normalization factor assuming rhohMax=1
+        # NOTE: correct this for different rhohMax by adding "- 4 * log(rhohMax)" to lnBtSG
+        self.lnBtSG = np.log(normBh) + logBhat  # - 4.0 * log ( rhohMax )
+        return self.lnBtSG
+
+    def write_F_mn_to_file(self, tCWfile, windowRange, header=[]):
+        """Format a 2D transient-F-stat matrix over `(t0,tau)` and write as a text file.
+
+        Apart from the optional extra header lines,
+        the format is consistent with lalpulsar.write_transientFstatMap_to_fp(),
+        with the columns `[t0[s], tau[s], 2F]`.
+        NOTE that the output is 2F, not F like stored in this class itself!
+
+        Parameters
+        ----------
+        tCWfile: str
+            Name of the file to write to.
+        windowRange: lalpulsar.transientWindowRange_t
+            A lalpulsar structure containing the transient parameters.
+        header: list
+            A list of additional header lines
+            to print at the start of the file.
+        """
+        with open(tCWfile, "w") as tfp:
+            for hline in header:
+                tfp.write("# {:s}\n".format(hline))
+            tfp.write("# t0[s]     tau[s]     2F\n")
+            for m, F_m in enumerate(self.F_mn):
+                this_t0 = windowRange.t0 + m * windowRange.dt0
+                for n, this_F in enumerate(F_m):
+                    this_tau = windowRange.tau + n * windowRange.dtau
+                    tfp.write(
+                        "  %10d %10d %- 11.8g\n" % (this_t0, this_tau, 2.0 * this_F)
+                    )
 
 
-def run_commandline(cl, log_level=20, raise_error=True, return_output=True):
-    """Run a string cmd as a subprocess, check for errors and return output.
+fstatmap_versions = {
+    "lal": lambda multiFstatAtoms, windowRange, BtSG: lalpulsar_compute_transient_fstat_map(
+        multiFstatAtoms, windowRange, BtSG
+    ),
+    "pycuda": lambda multiFstatAtoms, windowRange, BtSG: pycuda_compute_transient_fstat_map(
+        multiFstatAtoms, windowRange, BtSG
+    ),
+}
+"""Dictionary of the actual callable transient F-stat map functions this module supports.
 
-    Parameters
-    ----------
-    cl: str
-        Command to run
-    log_level: int
-        See https://docs.python.org/library/logging.html#logging-levels
-        default is '20' (INFO)
+Actual runtime availability depends on the corresponding external modules
+being available.
+"""
 
-    """
 
-    logging.log(log_level, "Now executing: " + cl)
-    if "|" in cl:
-        logging.warning(
-            "Pipe ('|') found in commandline, errors may not be" " properly caught!"
-        )
-    try:
-        if return_output:
-            out = subprocess.check_output(
-                cl,  # what to run
-                stderr=subprocess.STDOUT,  # catch errors
-                shell=True,  # proper environment etc
-                universal_newlines=True,  # properly display linebreaks in error/output printing
-            )
-        else:
-            subprocess.check_call(cl, shell=True)
-    except subprocess.CalledProcessError as e:
-        logging.log(40, "Execution failed: {}".format(e))
-        if e.output:
-            logging.log(40, e.output)
-        if raise_error:
-            raise
-        elif return_output:
-            out = 0
-    os.system("\n")
-    if return_output:
-        return out
-
-
-def convert_array_to_gsl_matrix(array):
-    gsl_matrix = lal.gsl_matrix(*array.shape)
-    gsl_matrix.data = array
-    return gsl_matrix
-
-
-def get_sft_array(sftfilepattern, data_duration=None, F0=None, dF0=None):
-    """Return the raw data (absolute value) from a set of SFTs
-
-    FIXME: currently only returns data for first detector
-    """
-
-    if F0 is None and dF0 is None:
-        fMin = -1
-        fMax = -1
-    elif F0 is None or dF0 is None:
-        raise ValueError("Need either none or both of F0, dF0.")
-    else:
-        fMin = F0 - dF0
-        fMax = F0 + dF0
+def _optional_imports_pycuda():
+    """Helper function to check for all all modules we need."""
+    have_pycuda = _optional_import("pycuda")
+    have_pycuda_drv = _optional_import("pycuda.driver", "drv")
+    have_pycuda_gpuarray = _optional_import("pycuda.gpuarray", "gpuarray")
+    have_pycuda_tools = _optional_import("pycuda.tools", "cudatools")
+    have_pycuda_compiler = _optional_import("pycuda.compiler", "cudacomp")
+    return (
+        have_pycuda
+        and have_pycuda_drv
+        and have_pycuda_gpuarray
+        and have_pycuda_tools
+        and have_pycuda_compiler
+    )
 
-    if data_duration is not None:
-        logging.warning(
-            "Option 'data_duration' for get_sft_array()"
-            " is no longer in use and will be removed."
-        )
-
-    SFTCatalog = lalpulsar.SFTdataFind(sftfilepattern, lalpulsar.SFTConstraints())
-    MultiSFTs = lalpulsar.LoadMultiSFTs(SFTCatalog, fMin, fMax)
-    ndet = MultiSFTs.length
-    if ndet > 1:
-        logging.warning(
-            "Loaded SFTs from {:d} detectors, only using the first.".format(ndet)
-        )
-
-    SFTs = MultiSFTs.data[0]
-    times = [sft.epoch.gpsSeconds for sft in SFTs.data]
-    data = [np.abs(sft.data.data) for sft in SFTs.data]
-    data = np.array(data).T
-    nbins, nsfts = data.shape
-
-    sft0 = SFTs.data[0]
-    freqs = np.linspace(sft0.f0, sft0.f0 + (nbins - 1) * sft0.deltaF, nbins)
-
-    return times, freqs, data
-
-
-def get_covering_band(
-    tref,
-    tstart,
-    tend,
-    F0,
-    F1,
-    F2,
-    F0band=0.0,
-    F1band=0.0,
-    F2band=0.0,
-    maxOrbitAsini=0.0,
-    minOrbitPeriod=0.0,
-    maxOrbitEcc=0.0,
-):
-    """Get the covering band using XLALCWSignalCoveringBand
+
+def _get_transient_fstat_map_features():
+    """Helper function to check available features."""
+    features = {}
+    have_lal = _optional_import("lal")
+    have_lalpulsar = _optional_import("lalpulsar")
+    features["lal"] = have_lal and have_lalpulsar
+    features["pycuda"] = _optional_imports_pycuda()
+    return features
+
+
+def init_transient_fstat_map_features(feature="lal", cudaDeviceName=None):
+    """Initialization of available modules (or 'features') for computing transient F-stat maps.
+
+    Currently, two implementations are supported and checked for
+    through the `_optional_import()` method:
+
+    1. `lal`: requires both `lal` and `lalpulsar` packages to be importable.
+
+    2. `pycuda`: requires the `pycuda` package to be importable
+    along with its modules
+    `driver`, `gpuarray`, `tools` and `compiler`.
 
     Parameters
     ----------
-    tref, tstart, tend: int
-        The reference, start, and end times of interest
-    F0, F1, F1: float
-        Minimum frequency and spin-down of signals to be covered
-    F0band, F1band, F1band: float
-        Ranges of frequency and spin-down of signals to be covered
-    maxOrbitAsini: float
-        Largest orbital projected semi-major axis to be covered
-    minOrbitPeriod: float
-        Shortest orbital period to be covered
-    maxOrbitEcc: float
-        Highest orbital eccentricity to be covered
+    feature: str
+        Set the transient F-stat map implementation.
+    cudaDeviceName: str or None
+        Request a CUDA device with this name.
+        Partial matches are allowed.
 
     Returns
     -------
-    F0min, F0max: float
-        Estimates of the minimum and maximum frequencies of the signal during
-        the search
-
-    """
-    tref = lal.LIGOTimeGPS(tref)
-    tstart = lal.LIGOTimeGPS(tstart)
-    tend = lal.LIGOTimeGPS(tend)
-    psr = lalpulsar.PulsarSpinRange()
-    psr.fkdot[0] = F0
-    psr.fkdot[1] = F1
-    psr.fkdot[2] = F2
-    psr.fkdotBand[0] = F0band
-    psr.fkdotBand[1] = F1band
-    psr.fkdotBand[2] = F2band
-    psr.refTime = tref
-    minCoverFreq, maxCoverFreq = lalpulsar.CWSignalCoveringBand(
-        tstart, tend, psr, maxOrbitAsini, minOrbitPeriod, maxOrbitEcc
-    )
-    if (
-        np.isnan(minCoverFreq)
-        or np.isnan(maxCoverFreq)
-        or minCoverFreq <= 0.0
-        or maxCoverFreq <= 0.0
-        or maxCoverFreq < minCoverFreq
-    ):
-        raise RuntimeError(
-            "Got invalid pair minCoverFreq={}, maxCoverFreq={} from"
-            " lalpulsar.CWSignalCoveringBand.".format(minCoverFreq, maxCoverFreq)
+    features: dict
+        A dictionary of available method names, to match `fstatmap_versions`.
+        Each key's value is set to `True` only if
+        all required modules are importable on this system.
+    gpu_context: pycuda.driver.Context or None
+        A CUDA device context object, if assigned.
+    """
+
+    features = _get_transient_fstat_map_features()
+    logger.debug("Got the following features for transient F-stat maps:")
+    logger.debug(features)
+
+    if feature == "pycuda":
+        if not features["pycuda"]:
+            raise RuntimeError("pycuda use was requested, but imports failed.")
+        logger.info("CUDA version: " + ".".join(map(str, drv.get_version())))
+
+        drv.init()
+        logger.debug(
+            "Starting with default pyCUDA context,"
+            " then checking all available devices..."
         )
-    return minCoverFreq, maxCoverFreq
+        try:
+            context0 = pycuda.tools.make_default_context()
+        except pycuda._driver.LogicError as e:
+            if e.message == "cuDeviceGet failed: invalid device ordinal":
+                devn = int(os.environ["CUDA_DEVICE"])
+                raise RuntimeError(
+                    "Requested CUDA device number {} exceeds"
+                    " number of available devices!"
+                    " Please change through environment"
+                    " variable $CUDA_DEVICE.".format(devn)
+                )
+            else:
+                raise pycuda._driver.LogicError(e.message)
 
+        num_gpus = drv.Device.count()
+        logger.info("Found {} CUDA device(s).".format(num_gpus))
 
-def twoFDMoffThreshold(
-    twoFon, knee=400, twoFDMoffthreshold_below_threshold=62, prefactor=0.9, offset=0.5
-):
-    """ Calculation of the 2F_DMoff threshold, see Eq 2 of arXiv:1707.5286 """
-    if twoFon <= knee:
-        return twoFDMoffthreshold_below_threshold
-    else:
-        return 10 ** (prefactor * np.log10(twoFon - offset))
+        devices = []
+        devnames = np.empty(num_gpus, dtype="S32")
+        for n in range(num_gpus):
+            devn = drv.Device(n)
+            devices.append(devn)
+            devnames[n] = devn.name().replace(" ", "-").replace("_", "-")
+            logger.info(
+                "device {}: model: {}, RAM: {}MB".format(
+                    n, devnames[n], devn.total_memory() / (2.0**20)
+                )
+            )
 
+        if "CUDA_DEVICE" in os.environ:
+            devnum0 = int(os.environ["CUDA_DEVICE"])
+        else:
+            devnum0 = 0
 
-def match_commandlines(cl1, cl2, be_strict_about_full_executable_path=False):
-    """ Check if two commandlines match element-by-element, regardless of order """
-    cl1s = cl1.split(" ")
-    cl2s = cl2.split(" ")
-    # first item will be the executable name
-    # by default be generous here and do not worry about full paths
-    if not be_strict_about_full_executable_path:
-        cl1s[0] = os.path.basename(cl1s[0])
-        cl2s[0] = os.path.basename(cl2s[0])
-    unmatched = np.setxor1d(cl1s, cl2s)
-    return len(unmatched) == 0
-
-
-def get_version_string():
-    return get_versions()["version"]
-
-
-def get_doppler_params_output_format(keys):
-    # use same format for writing out search parameters
-    # as write_FstatCandidate_to_fp() function of lalapps_CFSv2
-    fmt = []
-    CFSv2_fmt = "%.16g"
-    doppler_keys = [
-        "F0",
-        "F1",
-        "F2",
-        "Alpha",
-        "Delta",
-        "asini",
-        "period",
-        "ecc",
-        "tp",
-        "argp",
-    ]
+        matchbit = ""
+        if cudaDeviceName:
+            # allow partial matches in device names
+            devmatches = [
+                devidx
+                for devidx, devname in enumerate(devnames)
+                if cudaDeviceName in devname
+            ]
+            if len(devmatches) == 0:
+                context0.detach()
+                raise RuntimeError(
+                    'Requested CUDA device "{}" not found.'
+                    " Available devices: [{}]".format(
+                        cudaDeviceName, ",".join(devnames)
+                    )
+                )
+            else:
+                devnum = devmatches[0]
+                if len(devmatches) > 1:
+                    logger.warning(
+                        'Found {} CUDA devices matching name "{}".'
+                        " Choosing first one with index {}.".format(
+                            len(devmatches), cudaDeviceName, devnum
+                        )
+                    )
+            os.environ["CUDA_DEVICE"] = str(devnum)
+            matchbit = '(matched to user request "{}")'.format(cudaDeviceName)
+        elif "CUDA_DEVICE" in os.environ:
+            devnum = int(os.environ["CUDA_DEVICE"])
+        else:
+            devnum = 0
+        devn = devices[devnum]
+        logger.info(
+            "Choosing CUDA device {},"
+            " of {} devices present: {}{}...".format(
+                devnum, num_gpus, devn.name(), matchbit
+            )
+        )
+        if devnum == devnum0:
+            gpu_context = context0
+        else:
+            context0.pop()
+            gpu_context = pycuda.tools.make_default_context()
+            gpu_context.push()
+
+        _print_GPU_memory_MB("Available")
+    elif feature == "lal":
+        gpu_context = None
+    else:
+        raise ValueError(
+            "Unknown transient F-stat map computation feature" f"'{feature}' requested."
+        )
 
-    for k in keys:
-        if k in doppler_keys:
-            fmt += [CFSv2_fmt]
-    return fmt
-
-
-def read_txt_file_with_header(f, comments="#"):
-    # wrapper to np.genfromtxt with smarter header handling
-    with open(f, "r") as f_opened:
-        Nhead = 0
-        for line in f_opened:
-            if not line.startswith(comments):
-                break
-            Nhead += 1
-    data = np.genfromtxt(f, skip_header=Nhead - 1, names=True, comments=comments)
+    return features, gpu_context
 
-    return data
 
+def call_compute_transient_fstat_map(
+    version, features, multiFstatAtoms=None, windowRange=None, BtSG=False
+):
+    """Call a version of the ComputeTransientFstatMap function.
 
-def get_lalapps_commandline_from_SFTDescriptor(descriptor):
-    """get a lalapps commandline from SFT descriptor "comment" entry
+    This checks if the requested `version` is available,
+    and if so, executes the computation of a transient F-statistic map
+    over the `windowRange`.
 
     Parameters
     ----------
-    descriptor: SFTDescriptor
-        element of a lalpulsar SFTCatalog
+    version: str
+        Name of the method to call
+        (currently supported: 'lal' or 'pycuda').
+    features: dict
+        Dictionary of available features,
+        as obtained from `init_transient_fstat_map_features()`.
+    multiFstatAtoms: lalpulsar.MultiFstatAtomVector or None
+        The time-dependent F-stat atoms previously computed by `ComputeFstat`.
+    windowRange: lalpulsar.transientWindowRange_t or None
+        The structure defining the transient parameters.
+    BtSG: boolean
+        If true, also compute the lnBtSG transient Bayes factor statistic,
+        using the appropriate implementation for each feature,
+        and store it in `FstatMap.lnBtSG`.
 
     Returns
     -------
-    cmd: str
-        a lalapps commandline, or empty string if "lalapps" not found in comment
-    """
-    comment = getattr(descriptor, "comment", None)
-    if comment is None:
-        return ""
-    comment_lines = comment.split("\n")
-    # get the first line with the right substring
-    # (iterate until it's found)
-    return next((line for line in comment_lines if "lalapps" in line), "")
+    FstatMap: pyTransientFstatMap or lalpulsar.transientFstatMap_t
+        The output of the called function,
+        including the evaluated transient F-statistic map
+        over the windowRange.
+    timingFstatMap: float
+        Execution time of the called function.
+    """
+    if version in fstatmap_versions:
+        if features[version]:
+            time0 = time()
+            FstatMap = fstatmap_versions[version](multiFstatAtoms, windowRange, BtSG)
+            timingFstatMap = time() - time0
+        else:
+            raise Exception(
+                "Required module(s) for transient F-stat map"
+                ' method "{}" not available!'.format(version)
+            )
+    else:
+        raise Exception(
+            'Transient F-stat map method "{}"' " not implemented!".format(version)
+        )
+    return FstatMap, timingFstatMap
 
 
-def read_parameters_dict_lines_from_file_header(
-    outfile, comments="#", strip_spaces=True
-):
-    """load a list of pretty-printed parameters dictionary lines from a commented file header
+def lalpulsar_compute_transient_fstat_map(multiFstatAtoms, windowRange, BtSG=False):
+    """Wrapper for the standard lalpulsar function for computing a transient F-statistic map.
 
-    Returns a list of lines from a commented file header
-    that match the pretty-printed parameters dictionary format
-    as generated by BaseSearchClass.get_output_file_header().
-    The opening/closing bracket lines ("{","}") are not included.
-    Newline characters at the end of each line are stripped.
+    See https://lscsoft.docs.ligo.org/lalsuite/lalpulsar/_transient_c_w__utils_8h.html
+    for the wrapped function.
 
     Parameters
     ----------
-    outfile: str
-        name of a PyFstat-produced output file
-    comments: str
-        comment character used to start header lines
-    strip_spaces: bool
-        whether to strip leading/trailing spaces
+    multiFstatAtoms: lalpulsar.MultiFstatAtomVector
+        The time-dependent F-stat atoms previously computed by `ComputeFstat`.
+    windowRange: lalpulsar.transientWindowRange_t
+        The structure defining the transient parameters.
+    BtSG: boolean
+        If true, also compute the lnBtSG transient Bayes factor statistic,
+        using the corresponding lalpulsar function,
+        and store it in `FstatMap.lnBtSG`.
 
     Returns
     -------
-    dict_lines: list
-        a list of unparsed pprinted dictionary entries
+    FstatMap: pyTransientFstatMap
+        The computed results, see the class definition for details.
     """
-    dict_lines = []
-    with open(outfile, "r") as f_opened:
-        in_dict = False
-        for line in f_opened:
-            if not line.startswith(comments):
-                raise IOError(
-                    "Encountered end of {:s}-commented header before finding closing '}}' of parameters dictionary in file '{:s}'.".format(
-                        comments, outfile
-                    )
-                )
-            elif line.startswith(comments + " {"):
-                in_dict = True
-            elif line.startswith(comments + " }"):
-                break
-            elif in_dict:
-                line = line.lstrip(comments).rstrip("\n")
-                if strip_spaces:
-                    line = line.strip(" ")
-                dict_lines.append(line)
-    if len(dict_lines) == 0:
-        raise IOError(
-            "Could not parse non-empty parameters dictionary from file '{:s}'.".format(
-                outfile
-            )
+    FstatMap_lalpulsar = lalpulsar.ComputeTransientFstatMap(
+        multiFstatAtoms=multiFstatAtoms,
+        windowRange=windowRange,
+        useFReg=False,
+    )
+    FstatMap = pyTransientFstatMap(transientFstatMap_t=FstatMap_lalpulsar)
+    if BtSG:
+        FstatMap.lnBtSG = lalpulsar.ComputeTransientBstat(
+            windowRange, FstatMap_lalpulsar
         )
-    return dict_lines
-
+    return FstatMap
 
-def get_parameters_dict_from_file_header(outfile, comments="#", eval_values=False):
-    """load a parameters dict from a commented file header
 
-    Returns a parameters dictionary,
-    as generated by BaseSearchClass.get_output_file_header(),
-    from an output file header.
-    Always returns a proper python dictionary,
-    but the values will be unparsed strings if not requested otherwise.
+def reshape_FstatAtomsVector(atomsVector):
+    """Make a dictionary of ndarrays out of an F-stat atoms 'vector' structure.
 
     Parameters
     ----------
-    outfile: str
-        name of a PyFstat-produced output file
-    comments: str
-        comment character used to start header lines
-    eval_values: bool
-        If False, return dictionary values as strings.
-        If True, evaluate them. DANGER! Only do this if you trust the source.
+    atomsVector: lalpulsar.FstatAtomVector
+        The atoms in a 'vector'-like structure:
+        iterating over timestamps as the higher hierarchical level,
+        with a set of 'atoms' quantities defined at each timestamp.
 
     Returns
     -------
-    params_dict: dictionary
-        a dictionary of parameters
-        (with values either as unparsed strings, or evaluated)
-    """
-    if eval_values:
-        logging.warning(
-            "Will evaluate dictionary values read from file '{:s}'.".format(outfile)
-        )
-    params_dict = {}
-    dict_lines = read_parameters_dict_lines_from_file_header(
-        outfile, comments="#", strip_spaces=True
-    )
-    for line in dict_lines:
-        line_split = line.rstrip(",").split(":")
-        # check for a few possible corrupt formats,
-        # though we can't be exhaustive here...
-        if (
-            (len(line_split) != 2)
-            or np.any([len(s) == 0 for s in line_split])
-            or (line_split[-1] == ",")
-            or (line_split[0][0] != "'")
-            or (line_split[0][-1] != "'")
-        ):
-            raise IOError(
-                "Line '{:s}' is not of the expected format (# 'key': val,').".format(
-                    line
+    atomsDict: dict
+        A dictionary with an entry for each quantity,
+        which then is a 1D ndarray over timestamps for that one quantity.
+    """
+
+    numAtoms = atomsVector.length
+    atomsDict = {}
+    tempDict = {}
+    atom_fields = [
+        ("timestamp", np.uint32),
+        ("a2_alpha", np.float32),
+        ("b2_alpha", np.float32),
+        ("ab_alpha", np.float32),
+        ("Fa_alpha", complex),
+        ("Fb_alpha", complex),
+    ]
+    for dtype in atom_fields:
+        if dtype[1] == complex:
+            for part in "re", "im":
+                atomsDict[dtype[0] + "_" + part] = np.ndarray(
+                    numAtoms, dtype=np.float32
                 )
-            )
-        key = line_split[0].strip("'")
-        val = line_split[1].strip(" ")
-        if eval_values:
-            val = eval(val)  # DANGER
-        params_dict[key] = val
-    return params_dict
+            tempDict[dtype[0]] = np.ndarray(numAtoms, dtype=complex)
+        else:
+            atomsDict[dtype[0]] = np.ndarray(numAtoms, dtype=dtype[1])
+    for n, atom in enumerate(atomsVector.data):
+        for dtype in atom_fields:
+            if dtype[1] == complex:
+                tempDict[dtype[0]][n] = atom.__getattribute__(dtype[0])
+            else:
+                atomsDict[dtype[0]][n] = atom.__getattribute__(dtype[0])
+    for dtype in atom_fields:
+        if dtype[1] == complex:
+            for part in "real", "imag":
+                atomsDict[dtype[0] + "_" + part[:2]] = np.float32(
+                    getattr(tempDict[dtype[0]], part)
+                )
+    return atomsDict
 
 
-def read_par(
-    filename=None,
-    label=None,
-    outdir=None,
-    suffix="par",
-    comments=["%", "#"],
-    raise_error=False,
-):
-    """Read in a .par or .loudest file, returns a dict of the data
+def _get_absolute_kernel_path(kernel):
+    pyfstatdir = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
+    kernelfile = kernel + ".cu"
+    return os.path.join(pyfstatdir, "pyCUDAkernels", kernelfile)
 
-    Parameters
-    ----------
-    filename : str
-        Filename (path) containing rows of `key=val` data to read in.
-    label, outdir, suffix : str, optional
-        If filename is None, form the file to read as `outdir/label.suffix`.
-    comments : str or list of strings, optional
-        Characters denoting that a row is a comment.
-    raise_error : bool, optional
-        If True, raise an error for lines which are not comments, but cannot
-        be read.
-
-    Notes
-    -----
-    This can also be used to read in .loudest files, or any file which has
-    rows of `key=val` data (in which the val can be understood using eval(val)
 
-    Returns
-    -------
-    d: dict
-        The par values as a dict type
+def _print_GPU_memory_MB(key):
+    mem_used_MB = drv.mem_get_info()[0] / (2.0**20)
+    mem_total_MB = drv.mem_get_info()[1] / (2.0**20)
+    logger.debug(
+        "{} GPU memory: {:.4f} / {:.4f} MB free".format(key, mem_used_MB, mem_total_MB)
+    )
 
-    """
-    if filename is None:
-        filename = os.path.join(outdir, "{}.{}".format(label, suffix))
-    if os.path.isfile(filename) is False:
-        raise ValueError("No file {} found".format(filename))
-    d = {}
-    with open(filename, "r") as f:
-        d = get_dictionary_from_lines(f, comments, raise_error)
-    return d
 
+def pycuda_compute_transient_fstat_map(multiFstatAtoms, windowRange, BtSG=False):
+    """GPU version of computing a transient F-statistic map.
+
+    This is based on XLALComputeTransientFstatMap from LALSuite,
+    (C) 2009 Reinhard Prix, licensed under GPL.
+
+    The 'map' consists of F-statistics evaluated over
+    a range of different `(t0,tau)` pairs
+    (transient start-times and duration parameters).
 
-def get_dictionary_from_lines(lines, comments, raise_error):
-    """Return dictionary of key=val pairs for each line in lines
+    This is a high-level wrapper function;
+    the actual CUDA computations are performed in one of the functions
+    `pycuda_compute_transient_fstat_map_rect()`
+    or `pycuda_compute_transient_fstat_map_exp()`,
+    depending on the window functon defined in `windowRange`.
 
     Parameters
     ----------
-    comments : str or list of strings
-        Characters denoting that a row is a comment.
-    raise_error : bool
-        If True, raise an error for lines which are not comments, but cannot
-        be read.
-        Note that CFSv2 "loudest" files contain complex numbers which fill raise
-        an error unless this is set to False.
+    multiFstatAtoms: lalpulsar.MultiFstatAtomVector
+        The time-dependent F-stat atoms previously computed by `ComputeFstat`.
+    windowRange: lalpulsar.transientWindowRange_t
+        The structure defining the transient parameters.
+    BtSG: boolean
+        If true, also compute the lnBtSG transient Bayes factor statistic,
+        using a CPU python port of the corresponding lalpulsar function,
+        and store it in `FstatMap.lnBtSG`.
 
     Returns
     -------
-    d: dict
-        The par values as a dict type
-
+    FstatMap: pyTransientFstatMap
+        The computed results, see the class definition for details.
     """
-    d = {}
-    for line in lines:
-        if line[0] not in comments and len(line.split("=")) == 2:
-            try:
-                key, val = line.rstrip("\n").split("=")
-                key = key.strip()
-                val = val.strip()
-                if (val[0] in ["'", '"']) and (val[-1] in ["'", '"']):
-                    d[key] = val.lstrip('"').lstrip("'").rstrip('"').rstrip("'")
-                else:
-                    try:
-                        d[key] = np.float64(eval(val.rstrip("; ")))
-                    except NameError:
-                        d[key] = val.rstrip("; ")
-                    # FIXME: learn how to deal with complex numbers
-            except SyntaxError:
-                if raise_error:
-                    raise IOError("Line {} not understood".format(line))
-                pass
-    return d
-
-
-def get_predict_fstat_parameters_from_dict(signal_parameters):
-    """
-    Given a dictionary with arbitrary signal parameters,
-    return only those ones required by helper_functions.predict_fstat
-    (Freq, Alpha, Delta, h0, cosi, psi)
 
-    Parameters
-    ----------
-    signal_parameters: dict
-        Dictionary containing at least the signal parameters required by
-        helper_functions.predict_fstat. This dictionary's keys must follow
-        the PyFstat convention (F0 instead of Freq).
-    """
-    predict_fstat_params = {
-        key: signal_parameters[key]
-        for key in ["F0", "Alpha", "Delta", "h0", "cosi", "psi"]
-    }
-    return predict_fstat_params
-
-
-def predict_fstat(
-    h0=None,
-    cosi=None,
-    psi=None,
-    Alpha=None,
-    Delta=None,
-    F0=None,
-    sftfilepattern=None,
-    timestampsFiles=None,
-    minStartTime=None,
-    duration=None,
-    IFOs=None,
-    assumeSqrtSX=None,
-    tempory_filename="fs.tmp",
-    earth_ephem=None,
-    sun_ephem=None,
-    transientWindowType="none",
-    transientStartTime=None,
-    transientTau=None,
-):
-    """Wrapper to lalapps_PredictFstat
+    if windowRange.type >= lalpulsar.TRANSIENT_LAST:
+        raise ValueError(
+            "Unknown window-type ({}) passed as input."
+            " Allowed are [0,{}].".format(
+                windowRange.type, lalpulsar.TRANSIENT_LAST - 1
+            )
+        )
+
+    # internal dict for search/setup parameters
+    tCWparams = {}
+
+    # first combine all multi-atoms
+    # into a single atoms-vector with *unique* timestamps
+    tCWparams["TAtom"] = multiFstatAtoms.data[0].TAtom
+    TAtomHalf = int(tCWparams["TAtom"] / 2)  # integer division
+    atoms = lalpulsar.mergeMultiFstatAtomsBinned(multiFstatAtoms, tCWparams["TAtom"])
+
+    # make a combined input matrix of all atoms vectors, for transfer to GPU
+    tCWparams["numAtoms"] = atoms.length
+    atomsDict = reshape_FstatAtomsVector(atoms)
+    atomsInputMatrix = np.column_stack(
+        (
+            atomsDict["a2_alpha"],
+            atomsDict["b2_alpha"],
+            atomsDict["ab_alpha"],
+            atomsDict["Fa_alpha_re"],
+            atomsDict["Fa_alpha_im"],
+            atomsDict["Fb_alpha_re"],
+            atomsDict["Fb_alpha_im"],
+        )
+    )
+
+    # actual data spans [t0_data, t0_data + tCWparams['numAtoms'] * TAtom]
+    # in steps of TAtom
+    tCWparams["t0_data"] = int(atoms.data[0].timestamp)
+    tCWparams["t1_data"] = int(
+        atoms.data[tCWparams["numAtoms"] - 1].timestamp + tCWparams["TAtom"]
+    )
+
+    logger.debug(
+        "Transient F-stat map:"
+        " t0_data={:d}, t1_data={:d}".format(tCWparams["t0_data"], tCWparams["t1_data"])
+    )
+    logger.debug(
+        "Transient F-stat map:"
+        " numAtoms={:d}, TAtom={:d},"
+        " TAtomHalf={:d}".format(tCWparams["numAtoms"], tCWparams["TAtom"], TAtomHalf)
+    )
+
+    # special treatment of window_type = none
+    # ==> replace by rectangular window spanning all the data
+    if windowRange.type == lalpulsar.TRANSIENT_NONE:
+        windowRange.type = lalpulsar.TRANSIENT_RECTANGULAR
+        windowRange.t0 = tCWparams["t0_data"]
+        windowRange.t0Band = 0
+        windowRange.dt0 = tCWparams["TAtom"]  # irrelevant
+        windowRange.tau = tCWparams["numAtoms"] * tCWparams["TAtom"]
+        windowRange.tauBand = 0
+        windowRange.dtau = tCWparams["TAtom"]  # irrelevant
+
+    """ NOTE: indices {i,j} enumerate *actual* atoms and their timestamps t_i,
+    * while the indices {m,n} enumerate the full grid of values
+    * in [t0_min, t0_max]x[Tcoh_min, Tcoh_max] in steps of deltaT.
+    * This allows us to deal with gaps in the data in a transparent way.
+    *
+    * NOTE2: we operate on the 'binned' atoms returned
+    * from XLALmergeMultiFstatAtomsBinned(),
+    * which means we can safely assume all atoms to be lined up
+    * perfectly on a 'deltaT' binned grid.
+    *
+    * The mapping used will therefore be {i,j} -> {m,n}:
+    *   m = offs_i  / deltaT
+    *   start-time offset from t0_min measured in deltaT
+    *   n = Tcoh_ij / deltaT
+    *   duration Tcoh_ij measured in deltaT,
+    *
+    * where
+    *   offs_i  = t_i - t0_min
+    *   Tcoh_ij = t_j - t_i + deltaT
+    *
+    """
+
+    # We allocate a matrix  {m x n} = t0Range * TcohRange elements
+    # covering the full transient window-range [t0,t0+t0Band]x[tau,tau+tauBand]
+    tCWparams["N_t0Range"] = int(
+        np.floor(1.0 * windowRange.t0Band / windowRange.dt0) + 1
+    )
+    tCWparams["N_tauRange"] = int(
+        np.floor(1.0 * windowRange.tauBand / windowRange.dtau) + 1
+    )
+    FstatMap = pyTransientFstatMap(tCWparams["N_t0Range"], tCWparams["N_tauRange"])
+
+    logger.debug(
+        "Transient F-stat map:"
+        " N_t0Range={:d}, N_tauRange={:d},"
+        " total grid points: {:d}".format(
+            tCWparams["N_t0Range"],
+            tCWparams["N_tauRange"],
+            tCWparams["N_t0Range"] * tCWparams["N_tauRange"],
+        )
+    )
+
+    if windowRange.type == lalpulsar.TRANSIENT_RECTANGULAR:
+        FstatMap.F_mn = pycuda_compute_transient_fstat_map_rect(
+            atomsInputMatrix, windowRange, tCWparams
+        )
+    elif windowRange.type == lalpulsar.TRANSIENT_EXPONENTIAL:
+        FstatMap.F_mn = pycuda_compute_transient_fstat_map_exp(
+            atomsInputMatrix, windowRange, tCWparams
+        )
+    else:
+        raise ValueError(
+            "Invalid transient window type {}"
+            " not in [{}, {}].".format(
+                windowRange.type, lalpulsar.TRANSIENT_NONE, lalpulsar.TRANSIENT_LAST - 1
+            )
+        )
+
+    # out of loop: get max2F and ML estimates over the m x n matrix
+    FstatMap.maxF = FstatMap.F_mn.max()
+    maxidx = np.unravel_index(
+        FstatMap.F_mn.argmax(), (tCWparams["N_t0Range"], tCWparams["N_tauRange"])
+    )
+    FstatMap.t0_ML = windowRange.t0 + maxidx[0] * windowRange.dt0
+    FstatMap.tau_ML = windowRange.tau + maxidx[1] * windowRange.dtau
+
+    logger.debug(
+        "Done computing transient F-stat map."
+        " maxF={:.4f}, t0_ML={}, tau_ML={}".format(
+            FstatMap.maxF, FstatMap.t0_ML, FstatMap.tau_ML
+        )
+    )
+
+    if BtSG:
+        # so far seems there is no need to move this onto the GPU
+        FstatMap.lnBtSG = FstatMap.get_lnBtSG()
+        logger.debug(f"Also computed: lnBtSG={FstatMap.lnBtSG:.4f}")
+
+    return FstatMap
+
+
+def pycuda_compute_transient_fstat_map_rect(atomsInputMatrix, windowRange, tCWparams):
+    """GPU computation of the transient F-stat map for rectangular windows.
+
+    As discussed in Keitel & Ashton (CQG 35, 205003, 2018):
+    https://arxiv.org/abs/1805.05652
+    this version only does GPU parallization for the outer loop,
+    keeping the partial sums of the inner loop local to each individual kernel
+    using the 'memory trick'.
 
     Parameters
     ----------
-    h0, cosi, psi, Alpha, Delta : float
-        Signal properties, see `lalapps_PredictFstat --help` for more info.
-    F0: float or None
-        Only needed for noise floor estimation when given sftfilepattern
-        but assumeSqrtSX is None.
-    sftfilepattern : str or None
-        Pattern matching the sftfiles to use.
-    timestampsFiles : str or None
-        Comma-separated list of per-detector files containing timestamps to use.
-        Only used if no sftfilepattern given.
-    minStartTime, duration : int or None
-        If sftfilepattern given: used as optional constraints.
-        If timestampsFiles given: ignored.
-        If neither given: used as the interval for prediction.
-    IFOs : str or None
-        Comma-separated list of detectors.
-        Ignored if sftfilepattern is given,
-        required if it is not.
-    assumeSqrtSX : float or str
-        Assume stationary per-detector noise-floor instead of estimating from SFTs.
-        Single float or str value: use same for all IFOs.
-        Comma-separated string: must match len(detectors)
-        and/or the data in sftfilepattern.
-        Detectors will be paired to list elements following alphabetical order.
-        Required if sftfilepattern is not given,
-        optional if it is.
-    tempory_filename : str
-        Temporary file used for lalapps_PredictFstat output, will be deleted.
-    earth_ephem, sun_ephem : str or None
-        Ephemerides files, defaults will be used if None.
-    transientWindowType: str
-        Optional parameter for transient signals,
-        see `lalapps_PredictFstat --help`.
-        Default of "none" means a classical Continuous Wave signal.
-    transientStartTime, transientTau: int or None
-        Optional parameters for transient signals,
-        see `lalapps_PredictFstat --help`.
+    atomsInputMatrix: np.ndarray
+        A 2D array of stacked named columns containing the F-stat atoms.
+    windowRange: lalpulsar.transientWindowRange_t
+        The structure defining the transient parameters.
+    tCWparams: dict
+        A dictionary of miscellaneous parameters.
 
     Returns
     -------
-    twoF_expected, twoF_sigma : float
-        The expectation and standard deviation of 2F.
-
-    """
-
-    cl_pfs = []
-    cl_pfs.append("lalapps_PredictFstat")
+    F_mn: np.ndarray
+        A 2D array of the computed transient F-stat map over the
+        `[t0,tau]` range.
+    """
+
+    # gpu data setup and transfer
+    _print_GPU_memory_MB("Initial")
+    input_gpu = gpuarray.to_gpu(atomsInputMatrix)
+    Fmn_gpu = gpuarray.GPUArray(
+        (tCWparams["N_t0Range"], tCWparams["N_tauRange"]), dtype=np.float32
+    )
+    _print_GPU_memory_MB("After input+output allocation:")
+
+    # GPU kernel
+    kernel = "cudaTransientFstatRectWindow"
+    kernelfile = _get_absolute_kernel_path(kernel)
+    partial_Fstat_cuda_code = cudacomp.SourceModule(open(kernelfile, "r").read())
+    partial_Fstat_cuda = partial_Fstat_cuda_code.get_function(kernel)
+    partial_Fstat_cuda.prepare("PIIIIIIIIP")
+
+    # GPU grid setup
+    blockRows = min(1024, tCWparams["N_t0Range"])
+    blockCols = 1
+    gridRows = int(np.ceil(1.0 * tCWparams["N_t0Range"] / blockRows))
+    gridCols = 1
+
+    # running the kernel
+    logger.debug(
+        "Calling pyCUDA kernel with a grid of {}*{}={} blocks"
+        " of {}*{}={} threads each: {} total threads...".format(
+            gridRows,
+            gridCols,
+            gridRows * gridCols,
+            blockRows,
+            blockCols,
+            blockRows * blockCols,
+            gridRows * gridCols * blockRows * blockCols,
+        )
+    )
+    partial_Fstat_cuda.prepared_call(
+        (gridRows, gridCols),
+        (blockRows, blockCols, 1),
+        input_gpu.gpudata,
+        tCWparams["numAtoms"],
+        tCWparams["TAtom"],
+        tCWparams["t0_data"],
+        windowRange.t0,
+        windowRange.dt0,
+        windowRange.tau,
+        windowRange.dtau,
+        tCWparams["N_tauRange"],
+        Fmn_gpu.gpudata,
+    )
+
+    # return results to host
+    F_mn = Fmn_gpu.get()
+
+    _print_GPU_memory_MB("Final")
+
+    return F_mn
+
+
+def pycuda_compute_transient_fstat_map_exp(atomsInputMatrix, windowRange, tCWparams):
+    """GPU computation of the transient F-stat map for exponential windows.
+
+    As discussed in Keitel & Ashton (CQG 35, 205003, 2018):
+    https://arxiv.org/abs/1805.05652
+    this version does full GPU parallization
+    of both the inner and outer loop.
 
-    if h0 is not None:
-        cl_pfs.append("--h0={}".format(h0))
-    if cosi is not None:
-        cl_pfs.append("--cosi={}".format(cosi))
-    # NOTE: as of lalsuite 6.76, [psi,Alpha,Delta] are required even for
-    # noise-only calls, hence we default them to 0 if h0 is None or ==0,
-    # but fail if they're not set with h0>0.
-    # This can likely be simplified after a future lalsuite release.
-    pars = {"psi": psi, "Alpha": Alpha, "Delta": Delta}
-    for par in pars.keys():
-        if pars[par] is None:
-            if h0:
-                raise ValueError(
-                    "For h0>0, {:s} needs to be set explicitly.".format(par)
-                )
-            else:
-                cl_pfs.append("--{:s}=0".format(par))
-        else:
-            cl_pfs.append("--{:s}={}".format(par, pars[par]))
+    Parameters
+    ----------
+    atomsInputMatrix: np.ndarray
+        A 2D array of stacked named columns containing the F-stat atoms.
+    windowRange: lalpulsar.transientWindowRange_t
+        The structure defining the transient parameters.
+    tCWparams: dict
+        A dictionary of miscellaneous parameters.
 
-    if sftfilepattern is None:
-        if IFOs is None or assumeSqrtSX is None:
-            raise ValueError("Without sftfilepattern, need IFOs and assumeSqrtSX!")
-        cl_pfs.append("--IFOs={}".format(IFOs))
-        if timestampsFiles is None:
-            if minStartTime is None or duration is None:
-                raise ValueError(
-                    "Without sftfilepattern, need timestampsFiles or [minStartTime,duration]!"
-                )
-            else:
-                cl_pfs.append("--minStartTime={}".format(minStartTime))
-                cl_pfs.append("--duration={}".format(duration))
-        else:
-            if len(timestampsFiles.split(",")) != len(IFOs.split(",")):
-                # checking this manually here because PFS would segfault
-                raise ValueError("timestampsFiles and IFOs must have same length!")
-            cl_pfs.append("--timestampsFiles={}".format(timestampsFiles))
-    else:
-        cl_pfs.append("--DataFiles='{}'".format(sftfilepattern))
-        if minStartTime is not None:
-            cl_pfs.append("--minStartTime={}".format(minStartTime))
-            if duration is not None:
-                cl_pfs.append("--maxStartTime={}".format(minStartTime + duration))
-        if assumeSqrtSX is None:
-            if F0 is None:
-                raise ValueError(
-                    "With sftfilepattern but without assumeSqrtSX,"
-                    " we need F0 to estimate noise floor."
-                )
-            cl_pfs.append("--Freq={}".format(F0))
-    if assumeSqrtSX is not None:
-        if np.any([s <= 0 for s in parse_list_of_numbers(assumeSqrtSX)]):
-            raise ValueError("assumeSqrtSX must be >0!")
-        cl_pfs.append("--assumeSqrtSX={}".format(assumeSqrtSX))
-
-    cl_pfs.append("--outputFstat={}".format(tempory_filename))
-
-    earth_ephem_default, sun_ephem_default = get_ephemeris_files()
-    if earth_ephem is None:
-        earth_ephem = earth_ephem_default
-    if sun_ephem is None:
-        sun_ephem = sun_ephem_default
-    cl_pfs.append("--ephemEarth='{}'".format(earth_ephem))
-    cl_pfs.append("--ephemSun='{}'".format(sun_ephem))
-
-    if transientWindowType != "none":
-        cl_pfs.append("--transientWindowType='{}'".format(transientWindowType))
-        cl_pfs.append("--transientStartTime='{}'".format(transientStartTime))
-        cl_pfs.append("--transientTau='{}'".format(transientTau))
-
-    cl_pfs = " ".join(cl_pfs)
-    run_commandline(cl_pfs)
-    d = read_par(filename=tempory_filename)
-    twoF_expected = float(d["twoF_expected"])
-    twoF_sigma = float(d["twoF_sigma"])
-    os.remove(tempory_filename)
-    return twoF_expected, twoF_sigma
+    Returns
+    -------
+    F_mn: np.ndarray
+        A 2D array of the computed transient F-stat map over the
+        `[t0,tau]` range.
+    """
+
+    # gpu data setup and transfer
+    _print_GPU_memory_MB("Initial")
+    input_gpu = gpuarray.to_gpu(atomsInputMatrix)
+    Fmn_gpu = gpuarray.GPUArray(
+        (tCWparams["N_t0Range"], tCWparams["N_tauRange"]), dtype=np.float32
+    )
+    _print_GPU_memory_MB("After input+output allocation:")
+
+    # GPU kernel
+    kernel = "cudaTransientFstatExpWindow"
+    kernelfile = _get_absolute_kernel_path(kernel)
+    partial_Fstat_cuda_code = cudacomp.SourceModule(open(kernelfile, "r").read())
+    partial_Fstat_cuda = partial_Fstat_cuda_code.get_function(kernel)
+    partial_Fstat_cuda.prepare("PIIIIIIIIIP")
+
+    # GPU grid setup
+    blockRows = min(32, tCWparams["N_t0Range"])
+    blockCols = min(32, tCWparams["N_tauRange"])
+    gridRows = int(np.ceil(1.0 * tCWparams["N_t0Range"] / blockRows))
+    gridCols = int(np.ceil(1.0 * tCWparams["N_tauRange"] / blockCols))
+
+    # running the kernel
+    logger.debug(
+        "Calling kernel with a grid of {}*{}={} blocks"
+        " of {}*{}={} threads each: {} total threads...".format(
+            gridRows,
+            gridCols,
+            gridRows * gridCols,
+            blockRows,
+            blockCols,
+            blockRows * blockCols,
+            gridRows * gridCols * blockRows * blockCols,
+        )
+    )
+    partial_Fstat_cuda.prepared_call(
+        (gridRows, gridCols),
+        (blockRows, blockCols, 1),
+        input_gpu.gpudata,
+        tCWparams["numAtoms"],
+        tCWparams["TAtom"],
+        tCWparams["t0_data"],
+        windowRange.t0,
+        windowRange.dt0,
+        windowRange.tau,
+        windowRange.dtau,
+        tCWparams["N_t0Range"],
+        tCWparams["N_tauRange"],
+        Fmn_gpu.gpudata,
+    )
 
+    # return results to host
+    F_mn = Fmn_gpu.get()
 
-def parse_list_of_numbers(val):
-    """Convert a number, list of numbers or comma-separated str into a list of numbers.
+    _print_GPU_memory_MB("Final")
 
-    This is useful e.g. for sqrtSX inputs where the user can be expected
-    to try either type of input.
-    """
-    try:
-        out = list(
-            map(float, val.split(",") if hasattr(val, "split") else np.atleast_1d(val))
-        )
-    except Exception as e:
-        raise ValueError(
-            f"Could not parse '{val}' as a number or list of numbers."
-            f" Got exception: {e}."
-        )
-    return out
+    return F_mn
```

### Comparing `PyFstat-1.9.0/pyfstat/make_sfts.py` & `PyFstat-2.0.0/pyfstat/grid_based_searches.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1321 +1,1317 @@
-""" pyfstat tools to generate sfts """
+"""PyFstat search classes using grid-based methods."""
 
 
-import numpy as np
-import functools
+import itertools
 import logging
 import os
-import glob
-import pkgutil
+import re
+from collections import OrderedDict
 
-import lal
-import lalpulsar
+import matplotlib
+import matplotlib.pyplot as plt
+import numpy as np
+from tqdm import tqdm
 
+import pyfstat.utils as utils
 from pyfstat.core import (
     BaseSearchClass,
-    SearchForSignalWithJumps,
-    tqdm,
-    args,
+    ComputeFstat,
+    DefunctClass,
+    SemiCoherentGlitchSearch,
+    SemiCoherentSearch,
 )
-import pyfstat.helper_functions as helper_functions
 
+logger = logging.getLogger(__name__)
 
-class KeyboardInterruptError(Exception):
-    pass
 
+class GridSearch(BaseSearchClass):
+    """A search evaluating the F-statistic over a regular grid in parameter space.
 
-class InjectionParametersGenerator:
-    """
-    Draw injection parameter samples from the specified priors and return
-    them in the proper format.
-    """
+    This implements a simple 'square box' grid
+    with fixed spacing and ranges in each dimension,
+    i.e. for each parameter there's a simple 1D list of grid points
+    and the total grid is just the Cartesian product of these.
 
-    def __init__(self, priors=None, seed=None):
-        """
-        priors: dict
-            Each key refers to one of the signal's parameters (following the PyFstat convention).
-            Priors can be given as values in three formats (by order of evaluation):
-                1) Callable without required arguments
-                    {"ParameterA": np.random.uniform}
-                2) Dict containing numpy.random distribution as key and kwargs in a dict as value
-                    {"ParameterA": {"uniform": {"low": 0, "high":1}}}
-                3) Constant value to be returned as is
-                    {"ParameterA": 1.0}
-        seed:
-            `seed` argument to be feed to numpy.random.default_rng.
-        """
-        self.set_seed(seed)
-        self.set_priors(priors or {})
+    For N parameter space dimensions and a total of M points in the product grid,
+    the basic output is a (N+1,M)-dimensional array with the detection statistic
+    (twoF or log10BSGL) appended.
 
-    def set_priors(self, new_priors):
-        """Set priors to draw parameter space points from """
-        if type(new_priors) is not dict:
-            raise ValueError(
-                "new_priors is not a dict type.\nPlease, check "
-                "this class' docstring to learn about the expected format: "
-                f"{self.__init__.__doc__}"
-            )
-
-        self.priors = {}
-        self._update_priors(new_priors)
-
-    def set_seed(self, seed):
-        self.seed = seed
-        self._rng = np.random.default_rng(self.seed)
-
-    def _update_priors(self, new_priors):
-        for parameter_name, parameter_prior in new_priors.items():
-            if callable(parameter_prior):
-                self.priors[parameter_name] = parameter_prior
-            elif isinstance(parameter_prior, dict):
-                rng_function_name = next(iter(parameter_prior))
-                rng_function = getattr(self._rng, rng_function_name)
-                rng_kwargs = parameter_prior[rng_function_name]
-                self.priors[parameter_name] = functools.partial(
-                    rng_function, **rng_kwargs
-                )
-            else:  # Assume it is something to be returned as is
-                self.priors[parameter_name] = functools.partial(
-                    lambda x: x, parameter_prior
-                )
+    NOTE: if a large number of grid points are used, checks against cached
+    data may be slow as the array is loaded into memory. To avoid this, run
+    with the `clean` option which uses a generator instead.
 
-    def draw(self):
-        injection_parameters = {
-            parameter_name: parameter_prior()
-            for parameter_name, parameter_prior in self.priors.items()
-        }
-        return injection_parameters
-
-    def __call__(self):
-        return self.draw()
-
-
-class AllSkyInjectionParametersGenerator(InjectionParametersGenerator):
-    """Like InjectionParametersGenerator, but with hardcoded priors to perform
-    all sky searches. It assumes 1) PyFstat notation and 2) Equatorial coordinates"""
-
-    def set_priors(self, new_priors):
-        self._check_if_updating_sky_priors(new_priors)
-        super().set_priors({**new_priors, **self.restricted_priors})
-
-    def set_seed(self, seed):
-        super().set_seed(seed)
-        self.restricted_priors = {
-            # This is required because numpy has no arcsin distro
-            "Alpha": lambda: self._rng.uniform(low=0.0, high=2 * np.pi),
-            "Delta": lambda: np.arcsin(self._rng.uniform(low=-1.0, high=1.0)),
-        }
-
-    def _check_if_updating_sky_priors(self, new_priors):
-        if any(
-            restricted_key in new_priors
-            for restricted_key in self.restricted_priors.keys()
-        ):
-            logging.warning(
-                "Ignoring specified sky priors (Alpha, Delta)."
-                "This class is explicitly coded to prevent that from happening. Please, restore "
-                "to InjectionParametersGenerator if that's really what you want to do."
-            )
+    Most parameters are the same as for the `core.ComputeFstat` class,
+    only the additional ones are documented here:
+    """
 
+    tex_labels = {
+        "F0": r"$f$",
+        "F1": r"$\dot{f}$",
+        "F2": r"$\ddot{f}$",
+        "Alpha": r"$\alpha$",
+        "Delta": r"$\delta$",
+        "twoF": r"$\widetilde{2\mathcal{F}}$",
+        "maxTwoF": r"$\max\widetilde{2\mathcal{F}}$",
+        "log10BSGL": r"$\log_{10}\mathcal{B}_{\mathrm{S/GL}}$",
+        "lnBtSG": r"$\ln\mathcal{B}_{\mathrm{tS/G}}$",
+    }
+    """Formatted labels used for plot annotations."""
 
-class Writer(BaseSearchClass):
-    """ Instance object for generating SFTs """
-
-    signal_parameter_labels = [
-        "tref",
-        "F0",
-        "F1",
-        "F2",
-        "Alpha",
-        "Delta",
-        "h0",
-        "cosi",
-        "psi",
-        "phi",
-        "transientWindowType",
-    ]
-    gps_time_and_string_formats_as_LAL = {
-        # GPS times should NOT be parsed using scientific notation
-        # LAL routines silently parse them wrongly
-        "refTime": ":10.9f",
-        "transientWindowType": ":s",
+    tex_labels0 = {
+        "F0": r"$-f_0$",
+        "F1": r"$-\dot{f}_0$",
+        "F2": r"$-\ddot{f}_0$",
+        "Alpha": r"$-\alpha_0$",
+        "Delta": r"$-\delta_0$",
     }
+    """Formatted labels used for annotating central values in plots."""
+
+    fmt_detstat = "%.9g"
+    """Standard output precision for detection statistics."""
 
-    @helper_functions.initializer
+    @utils.initializer
     def __init__(
         self,
-        label="PyFstat",
-        tstart=None,
-        duration=None,
+        label,
+        outdir,
+        sftfilepattern,
+        F0s,
+        F1s,
+        F2s,
+        Alphas,
+        Deltas,
         tref=None,
-        F0=None,
-        F1=0,
-        F2=0,
-        Alpha=None,
-        Delta=None,
-        h0=None,
-        cosi=None,
-        psi=0.0,
-        phi=0,
-        Tsft=1800,
-        outdir=".",
-        sqrtSX=None,
-        noiseSFTs=None,
-        SFTWindowType=None,
-        SFTWindowBeta=0.0,
-        Band=None,
+        minStartTime=None,
+        maxStartTime=None,
+        nsegs=1,
+        BSGL=False,
+        minCoverFreq=None,
+        maxCoverFreq=None,
         detectors=None,
+        SSBprec=None,
+        RngMedWindow=None,
+        injectSources=None,
+        input_arrays=False,
+        assumeSqrtSX=None,
         earth_ephem=None,
         sun_ephem=None,
-        transientWindowType="none",
-        transientStartTime=None,
-        transientTau=None,
-        randSeed=None,
+        clean=False,
     ):
         """
         Parameters
         ----------
-        label: string
-            a human-readable label to be used in naming the output files
-        tstart, duration : int
-            start and duration (in gps seconds) of the total observation span
-        tref: float or None
-            reference time (default is None, which sets the reference time to
-            tstart)
-        F0: float or None
-            frequency of signal to inject,
-            also used (if Band is not None) as center of frequency band;
-            also needed when noise-only (h0==None or ==0)
-            but no noiseSFTs given,
-            then again used as center of frequency band.
-        F1, F2, Alpha, Delta, h0, cosi, psi, phi: float or None
-            frequency evolution and amplitude parameters for injection
-            if h0==None or h0==0, these are all ignored
-            if h0>0, then Alpha, Delta, cosi need to be set explicitly
-        Tsft: int
-            The SFT duration in seconds.
-            Will be ignored if noiseSFTs are given.
-        noiseSFTs: str or None
-            SFT on top of which signals will be injected.
-            If not None, additional constraints can be applied using the arguments
-            tstart and duration.
-        Band: float or None
-            If float, and F0 is also not None, then output SFTs cover
-            [F0-Band/2,F0+Band/2].
-            If None and noiseSFTs given, use their bandwidth.
-            If None and no noiseSFTs given,
-            a minimal covering band for a perfectly-matched
-            single-template ComputeFstat analysis is estimated.
-        see `lalapps_Makefakedata_v5 --help` for help with the other paramaters
-        """
-
-        self.set_ephemeris_files(earth_ephem, sun_ephem)
-        self.basic_setup()
-        self.parse_args_consistent_with_mfd()
-        self.calculate_fmin_Band()
-
-    def _get_sft_constraints_from_tstart_duration(self):
-        """
-        Use start and duration to set up a lalpulsar.SFTConstraints
-        object. This method is only used if noiseSFTs is not None.
-        """
-        SFTConstraint = lalpulsar.SFTConstraints()
-
-        if self.tstart is None:
-            SFTConstraint.minStartTime = None
-            SFTConstraint.maxStartTime = None
-        elif self.duration is None:
-            SFTConstraint.maxStartTime = None
+        label: str
+            Output filenames will be constructed using this label.
+        outdir: str
+            Output directory.
+        F0s, F1s, F2s, Alphas, Deltas: tuple
+            A length 3 tuple describing the grid for each parameter,
+            e.g [F0min, F0max, dF0].
+            Alternatively, for a fixed value simply give [F0].
+            Unless `input_arrays=True`, then these are the exact arrays to search over.
+        nsegs: int
+            Number of segments to split the data set into.
+            If `nsegs=1`, the basic ComputeFstat class is used.
+            If `nsegs>1`, the SemiCoherentSearch class is used.
+        input_arrays: bool
+            If true, use the F0s, F1s, etc as arrays just as they are given
+            (do not interpret as 3-tuples of [min,max,step]).
+        clean: bool
+            If true, ignore existing data and overwrite.
+            Otherwise, re-use existing data if no inconsistencies are found.
+        """
+
+        self._set_init_params_dict(locals())
+        os.makedirs(outdir, exist_ok=True)
+        self.set_out_file()
+        self.search_keys = ["F0", "F1", "F2", "Alpha", "Delta"]
+        for k in self.search_keys:
+            setattr(self, k, np.atleast_1d(getattr(self, k + "s")))
+        if self.BSGL:
+            self.detstat = "log10BSGL"
         else:
-            SFTConstraint.minStartTime = lal.LIGOTimeGPS(self.tstart)
-            SFTConstraint.maxStartTime = SFTConstraint.minStartTime + self.duration
-
-        SFTConstraint.timestamps = None  # FIXME: not currently supported
+            self.detstat = "twoF"
+        self._initiate_search_object()
+        self._set_output_keys()
+        self.output_file_header = self.get_output_file_header()
+
+    def _set_output_keys(self):
+        self.output_keys = self.search_keys.copy()
+        self.output_keys.append("twoF")
+        if self.search.singleFstats:
+            self.output_keys += [f"twoF{IFO}" for IFO in self.search.detector_names]
+        if self.BSGL:
+            self.output_keys.append(self.detstat)
+
+    def _get_search_ranges(self):
+        if (self.minCoverFreq is None) or (self.maxCoverFreq is None):
+            return {key: getattr(self, key + "s") for key in self.search_keys}
+        else:
+            return None
 
-        logging.info(
-            "SFT Constraints: [minStartTime:{}, maxStartTime:{}]".format(
-                SFTConstraint.minStartTime,
-                SFTConstraint.maxStartTime,
+    def _initiate_search_object(self):
+        logger.info("Setting up search object")
+        search_ranges = self._get_search_ranges()
+        if self.nsegs == 1:
+            self.search = ComputeFstat(
+                tref=self.tref,
+                sftfilepattern=self.sftfilepattern,
+                minCoverFreq=self.minCoverFreq,
+                maxCoverFreq=self.maxCoverFreq,
+                search_ranges=search_ranges,
+                detectors=self.detectors,
+                minStartTime=self.minStartTime,
+                maxStartTime=self.maxStartTime,
+                BSGL=self.BSGL,
+                SSBprec=self.SSBprec,
+                RngMedWindow=self.RngMedWindow,
+                injectSources=self.injectSources,
+                assumeSqrtSX=self.assumeSqrtSX,
+                earth_ephem=self.earth_ephem,
+                sun_ephem=self.sun_ephem,
             )
-        )
-
-        return SFTConstraint
+        else:
+            self.search = SemiCoherentSearch(
+                label=self.label,
+                outdir=self.outdir,
+                tref=self.tref,
+                nsegs=self.nsegs,
+                sftfilepattern=self.sftfilepattern,
+                BSGL=self.BSGL,
+                minStartTime=self.minStartTime,
+                maxStartTime=self.maxStartTime,
+                minCoverFreq=self.minCoverFreq,
+                maxCoverFreq=self.maxCoverFreq,
+                search_ranges=search_ranges,
+                detectors=self.detectors,
+                injectSources=self.injectSources,
+            )
+        # make sure to overwrite the min/max starttime in case the user
+        # passed None and they were read from SFTs
+        self.minStartTime = self.search.minStartTime
+        self.maxStartTime = self.search.maxStartTime
+
+    def _get_array_from_tuple(self, x):
+        if len(x) == 1:
+            return np.array(x)
+        elif len(x) == 3 and self.input_arrays is False:
+            # This used to be
+            # return np.arange(x[0], x[1], x[2])
+            # but according to the numpy docs:
+            # "When using a non-integer step, such as 0.1,
+            # the results will often not be consistent.
+            # It is better to use numpy.linspace for these cases."
+            # and indeed it sometimes included the end point, sometimes didn't
+            return np.linspace(
+                x[0], x[1], num=int((x[1] - x[0]) / x[2]) + 1, endpoint=True
+            )
+        else:
+            logger.info("Using tuple of length {:d} as is.".format(len(x)))
+            return np.array(x)
 
-    def _get_setup_from_tstart_duration(self):
-        """
-        Default behavior: If no noiseSFTs are given, use the input parameters (tstart,
-        duration, detectors and Tsft) to make fake data.
-        """
-        self.tstart = int(self.tstart)
-        self.duration = int(self.duration)
+    def _get_input_data_array(self):
+        """Set up an input data array, i.e. the product array over search dimensions.
 
-        IFOs = self.detectors.split(",")
-        # when duration is not a multiple of Tsft, to match MFDv5
-        # we need to round the number *up*
-        # and also include the overlapping bit at the end in the duration
-        numSFTs = int(np.ceil(float(self.duration) / self.Tsft))  # per IFO
-        effective_duration = numSFTs * self.Tsft
-
-        self.sftfilenames = [
-            lalpulsar.OfficialSFTFilename(
-                dets[0],
-                dets[1],
-                numSFTs,
-                self.Tsft,
-                self.tstart,
-                effective_duration,
-                self.label,
+        This is a numpy structured array with named columns
+        and explicit dtype (cannot have named columns without that).
+        (Will also ensure safety when reading/saving data from/to .txt files.)
+        """
+        logger.info("Generating input data array")
+        coord_arrays = []
+        for sl in self.search_keys:
+            coord_arrays.append(
+                self._get_array_from_tuple(np.atleast_1d(getattr(self, sl)))
+            )
+        self.coord_arrays = coord_arrays
+        self.total_iterations = np.prod([len(ca) for ca in coord_arrays])
+
+        if not self.clean:
+            input_data = []
+            for vals in itertools.product(*coord_arrays):
+                input_data.append(vals)
+            input_dtype = np.dtype(
+                {
+                    "names": self.search_keys,
+                    "formats": np.repeat(float, len(self.search_keys)),
+                }
+            )
+            self.input_data = np.array(input_data, dtype=input_dtype)
+
+    def check_old_data_is_okay_to_use(self):
+        """Check if an existing output file matches this search and reuse the results.
+
+        Results will be loaded from old output file,
+        and no new search run, if all of the following checks pass:
+
+        1. Output file with matching name found in `outdir`.
+
+        2. Output file is not older than SFT files matching `sftfilepattern`.
+
+        3. Parameters string in file header matches current search setup.
+
+        4. Data in old file can be loaded successfully,
+           its input parts (i.e. minus the detection statistic columns)
+           matches in dimension with current grid,
+           and the values in those input columns match with the current grid.
+
+        Through `utils.read_txt_file_with_header()`,
+        the existing file is read in with `np.genfromtxt()`.
+        """
+        if self.clean:
+            return False
+        if os.path.isfile(self.out_file) is False:
+            logger.info(
+                "No old output file '{:s}' found, continuing with grid search.".format(
+                    self.out_file
+                )
             )
-            for ind, dets in enumerate(IFOs)
-        ]
-
-    def _gps_to_int(self, tGPS):
-        """Simple LIGOTimeGPS helper, SWIG-LAL does not import this functionality"""
-        return tGPS.gpsSeconds
+            return False
+        if self.sftfilepattern is not None:
+            oldest_sft = min(
+                [os.path.getmtime(f) for f in self._get_list_of_matching_sfts()]
+            )
+            if os.path.getmtime(self.out_file) < oldest_sft:
+                logger.info(
+                    "Search output data outdates sft files,"
+                    + " continuing with grid search."
+                )
+                return False
 
-    def _get_setup_from_noiseSFTs(self):
-        """
-        If noiseSFTs are given, use them to obtain relevant data parameters (tstart,
-        duration, detectors and Tsft). The corresponding input values will be used to
-        set up a lalpulsar.SFTConstraints object to be imposed to the SFTs. Keep in
-        mind that Tsft will also be checked to be consistent accross all SFTs (this is
-        not implemented through SFTConstraints but through a simple list check).
-        """
-        SFTConstraint = self._get_sft_constraints_from_tstart_duration()
-        noise_multi_sft_catalog = lalpulsar.GetMultiSFTCatalogView(
-            lalpulsar.SFTdataFind(self.noiseSFTs, SFTConstraint)
+        logger.info("Checking header of '{:s}'".format(self.out_file))
+        old_params_dict_str_list = utils.read_parameters_dict_lines_from_file_header(
+            self.out_file
         )
-        if noise_multi_sft_catalog.length == 0:
-            raise IOError("Got empty SFT catalog.")
+        new_params_dict_str_list = [
+            line.strip(" ") for line in self.pprint_init_params_dict()[1:-1]
+        ]
+        unmatched = np.setxor1d(old_params_dict_str_list, new_params_dict_str_list)
+        if len(unmatched) > 0:
+            logger.info(
+                "Parameters string in file header does not match"
+                + " current search setup, continuing with grid search."
+            )
+            return False
+        else:
+            logger.info(
+                "Parameters string in file header matches current search setup."
+            )
 
-        # Information to be extracted from the SFTs themselves
-        IFOs = []
-        tstart = []
-        tend = []
-        Tsft = []
-        self.sftfilenames = []  # This refers to the MFD output!
-
-        for ifo_catalog in noise_multi_sft_catalog.data:
-            ifo_name = lalpulsar.ListIFOsInCatalog(ifo_catalog).data[0]
-
-            time_stamps = lalpulsar.TimestampsFromSFTCatalog(ifo_catalog)
-            this_Tsft = int(round(1.0 / ifo_catalog.data[0].header.deltaF))
-            this_start_time = self._gps_to_int(time_stamps.data[0])
-            this_end_time = self._gps_to_int(time_stamps.data[-1]) + this_Tsft
-
-            self.sftfilenames.append(
-                lalpulsar.OfficialSFTFilename(
-                    ifo_name[0],
-                    ifo_name[1],
-                    ifo_catalog.length,
-                    this_Tsft,
-                    this_start_time,
-                    this_end_time - this_start_time,
-                    self.label,
+        logger.info("Loading old data from '{:s}'.".format(self.out_file))
+        old_data = utils.read_txt_file_with_header(self.out_file, names=True)
+        if len(old_data) != len(self.input_data):
+            logger.info(
+                "Old data found in '{:s}', but differs"
+                " in length ({:d} points in file, {:d} points requested);"
+                " continuing with grid search.".format(
+                    self.out_file, np.shape(old_data)[0], np.shape(self.input_data)[0]
                 )
             )
-
-            IFOs.append(ifo_name)
-            tstart.append(this_start_time)
-            tend.append(this_end_time)
-            Tsft.append(this_Tsft)
-
-        # Get the "overall" values of the search
-        Tsft = np.unique(Tsft)
-        if len(Tsft) != 1:
-            raise ValueError(f"SFTs contain different basetimes: {Tsft}")
-        if Tsft[0] != self.Tsft:
-            logging.warning(
-                f"Overwriting self.Tsft={self.Tsft}"
-                f" with value {Tsft[0]} read from noiseSFTs."
-            )
-        self.Tsft = Tsft[0]
-        self.tstart = min(tstart)
-        self.duration = max(tend) - self.tstart
-        self.detectors = ",".join(IFOs)
-
-    def basic_setup(self):
-        os.makedirs(self.outdir, exist_ok=True)
-        self.config_file_name = os.path.join(self.outdir, self.label + ".cff")
-        self.theta = np.array([self.phi, self.F0, self.F1, self.F2])
-
-        required_signal_params = [
-            # leaving out "F1","F2","psi","phi","tref" as they have defaults
-            "F0",
-            "Alpha",
-            "Delta",
-            "cosi",
-        ]
-        if self.h0 and np.any(
-            [getattr(self, k, None) is None for k in required_signal_params]
-        ):
-            raise ValueError(
-                "If h0>0, also need all of ({:s})".format(
-                    ",".join(required_signal_params)
+            return False
+        if len(old_data.dtype) < len(self.input_data.dtype):
+            logger.info(
+                "Old data found in '{:s}', but has less columns ({:d})"
+                " than new input parameters grid ({:d});"
+                " continuing with grid search.".format(
+                    self.out_file, np.shape(old_data)[1], np.shape(self.input_data)[1]
                 )
             )
-
-        no_noiseSFTs_options = ["tstart", "duration", "detectors"]
-        if self.noiseSFTs is not None:
-            logging.warning(
-                "noiseSFTs is not None: Inferring tstart, duration, Tsft. "
-                "Input tstart and duration will be treated as SFT constraints "
-                "using lalpulsar.SFTConstraints; Tsft will be checked for "
-                "internal consistency accross input SFTs."
-            )
-            self._get_setup_from_noiseSFTs()
-        elif np.any([getattr(self, k) is None for k in no_noiseSFTs_options]):
-            raise ValueError(
-                "Need either noiseSFTs or all of ({:s}).".format(
-                    ",".join(no_noiseSFTs_options)
+            return False
+        # not yet explicitly testing the case of
+        # len(old_data.dtype) >= len(self.input_data.dtype)
+        # because output file can have detstat and post-proc quantities
+        # added and hence have different number of dimensions
+        # (this could in principle be cleverly predicted at this point)
+        # and the np.allclose() check should safely catch those situations
+        rtol, atol = self._get_tolerance_from_savetxt_fmt()
+        column_matches = [
+            np.allclose(
+                old_data[key],
+                self.input_data[key],
+                rtol=rtol[key],
+                atol=atol[key],
+            )
+            for key in self.search_keys
+        ]
+        if np.all(column_matches):
+            logger.info(
+                "Old data found in '{:s}' with matching input parameters grid,"
+                " no search performed. Data grid size: {:d}x{:d}".format(
+                    self.out_file, len(old_data), len(old_data.dtype)
                 )
             )
+            return old_data
         else:
-            self._get_setup_from_tstart_duration()
+            logger.info(
+                "Old data found in '{:s}', input parameters grid differs,"
+                "  continuing with grid search.".format(self.out_file)
+            )
+            return False
+        return False
 
-        self.sftfilepath = ";".join(
-            [os.path.join(self.outdir, fn) for fn in self.sftfilenames]
-        )
+    def run(self, return_data=False):
+        """Execute the actual search over the full grid.
+
+        This iterates over all points in the multi-dimensional product grid
+        and the end result is either returned as a numpy array or saved to disk.
 
-        if self.tref is None:
-            self.tref = self.tstart
+        Parameters
+        ----------
+        return_data: boolean
+            If true, the final inputs+outputs data set is returned as a numpy array.
+            If false, it is saved to disk and nothing is returned.
+
+        Returns
+        -------
+        data: np.ndarray
+            The final inputs+outputs data set.
+            Only if `return_data=true`.
+        """
+        self._get_input_data_array()
 
-    def tend(self):
-        return self.tstart + self.duration
+        if self.clean:
+            iterable = itertools.product(*self.coord_arrays)
+        else:
+            old_data = self.check_old_data_is_okay_to_use()
+            iterable = self.input_data
 
-    def parse_args_consistent_with_mfd(self):
-        self.signal_parameters = self.translate_keys_to_lal(
+            if old_data is not False:
+                self.data = old_data
+                return
+
+        logger.info(
+            "Running search over a total of {:d} grid points...".format(
+                np.shape(iterable)[0]
+            )
+        )
+        output_dtype = np.dtype(
             {
-                key: self.__dict__[key]
-                for key in self.signal_parameter_labels
-                if self.__dict__.get(key, None) is not None
+                "names": self.output_keys,
+                "formats": np.repeat(float, len(self.output_keys)),
             }
         )
+        data = np.zeros(len(self.input_data), dtype=output_dtype)
 
-        self.signal_formats = {
-            key: self.gps_time_and_string_formats_as_LAL.get(key, ":1.18e")
-            for key in self.signal_parameters
-        }
-
-        if self.signal_parameters["transientWindowType"] != "none":
-            self.signal_parameters["transientStartTime"] = self.transientStartTime
-            self.signal_formats["transientStartTime"] = ":10.0f"
-            self.signal_parameters["transientTau"] = self.transientTau
-            self.signal_formats["transientTau"] = ":10.0f"
-
-    def calculate_fmin_Band(self):
-        """
-        Set fmin and Band for the output SFTs to cover.
+        for n, vals in enumerate(
+            tqdm(iterable, total=getattr(self, "total_iterations", None))
+        ):
+            thisCand = list(vals)
+            detstat = self.search.get_det_stat(*vals)
+            thisCand.append(self.search.twoF)
+            if self.search.singleFstats:
+                thisCand += list(self.search.twoFX[: self.search.numDetectors])
+            if self.detstat != "twoF":
+                thisCand.append(detstat)
+            for k, key in enumerate(self.output_keys):
+                data[key][n] = thisCand[k]
 
-        Either uses the user-provided Band and puts F0 in the middle,
-        does nothing to later reuse full bandwidth of noiseSFTs,
-        or if F0!=None, noiseSFTs==None and Band==None
-        it estimates a minimal band for just the injected signal:
-        F-stat covering band plus extra bins for demod default parameters.
-        This way a perfectly matched single-template ComputeFstat analysis
-        should run through perfectly on the SFTs.
-        For any wider-band or mismatched search, the set Band manually.
-
-        If you want to use noiseSFTs but auto-estimate a minimal band,
-        call helper_functions.get_covering_band() yourself
-        and pass the results as fmin, Band.
-        """
-        if self.F0 is not None and self.Band is not None:
-            self.fmin = self.F0 - 0.5 * self.Band
-        elif self.noiseSFTs:
-            logging.info("Generating SFTs with full bandwidth from noiseSFTs.")
-        elif self.F0 is None:
-            raise ValueError(
-                "Need F0 and Band, or one of (F0 or noiseSFTs)"
-                " to auto-estimate bandwidth."
-            )
+        if return_data:
+            return data
         else:
-            extraBins = (
-                # matching extraBinsFull in XLALCreateFstatInput():
-                # https://lscsoft.docs.ligo.org/lalsuite/lalpulsar/_compute_fstat_8c_source.html#l00490
-                lalpulsar.FstatOptionalArgsDefaults.Dterms
-                + int(lalpulsar.FstatOptionalArgsDefaults.runningMedianWindow / 2)
-                + 1
-            )
-            logging.info(
-                "Estimating required SFT frequency range from properties"
-                " of signal to inject plus {:d} extra bins either side"
-                " (corresponding to default F-statistic settings).".format(extraBins)
-            )
-            minCoverFreq, maxCoverFreq = helper_functions.get_covering_band(
-                tref=self.tref,
-                tstart=self.tstart,
-                tend=self.tend(),
-                F0=self.F0,
-                F1=self.F1,
-                F2=self.F2,
-                F0band=0.0,
-                F1band=0.0,
-                F2band=0.0,
-                maxOrbitAsini=getattr(self, "asini", 0.0),
-                minOrbitPeriod=getattr(self, "period", 0.0),
-                maxOrbitEcc=getattr(self, "ecc", 0.0),
-            )
-            self.fmin = minCoverFreq - extraBins / self.Tsft
-            self.Band = maxCoverFreq - minCoverFreq + 2 * extraBins / self.Tsft
-        if hasattr(self, "fmin"):
-            logging.info(
-                "Generating SFTs with fmin={}, Band={}".format(self.fmin, self.Band)
-            )
-
-    def get_single_config_line(self, i):
-        config_line = "[TS{}]\n".format(i)
-        config_line += "\n".join(
-            [
-                "{} = {{{}}}".format(key, self.signal_formats[key]).format(
-                    self.signal_parameters[key]
+            self.data = data
+            self.save_array_to_disk()
+
+    def _get_savetxt_fmt_dict(self):
+        """Define the output precision for each parameter and computed quantity."""
+        fmt_dict = utils.get_doppler_params_output_format(self.output_keys)
+        fmt_dict["twoF"] = self.fmt_detstat
+        if self.search.singleFstats:
+            for IFO in self.search.detector_names:
+                fmt_dict[f"twoF{IFO}"] = self.fmt_detstat
+        if self.BSGL:
+            fmt_dict["log10BSGL"] = self.fmt_detstat
+        return fmt_dict
+
+    def _get_savetxt_fmt_list(self):
+        """Returns a list of output format specifiers, ordered like the data.
+
+        This is required because the output of _get_savetxt_fmt_dict()
+        will depend on the order in which those entries have been coded up.
+        """
+        fmt_dict = self._get_savetxt_fmt_dict()
+        fmt_list = [fmt_dict[key] for key in self.output_keys]
+        return fmt_list
+
+    def _get_tolerance_from_savetxt_fmt(self):
+        """Decide appropriate input grid comparison tolerances from fprintf formats."""
+        fmt = self._get_savetxt_fmt_dict()
+        rtol = {}
+        atol = {}
+        for key, f in fmt.items():
+            if f.endswith("d"):
+                rtol[key] = 0
+                atol[key] = 0
+            elif f.endswith("g"):
+                precision = int(re.findall(r"\d+", f)[-1])
+                rtol[key] = 10 ** (1 - precision)
+                atol[key] = 0
+            elif f.endswith("f"):
+                decimals = int(re.findall(r"\d+", f)[-1])
+                rtol[key] = 0
+                atol[key] = 10**-decimals
+            else:
+                raise ValueError(
+                    "Cannot parse fprintf format '{:s}' to obtain recommended tolerance.".format(
+                        f
+                    )
                 )
-                for key in self.signal_parameters.keys()
-            ]
-        )
-        config_line += "\n"
+        return rtol, atol
 
-        return config_line
+    def save_array_to_disk(self):
+        """Save the results array to a txt file.
 
-    def make_cff(self, verbose=False):
-        """
-        Generates a .cff file
+        This includes a header with version and parameters information.
 
-        """
+        It should be flexible enough to be reused by child classes,
+        as long as the `_get_savetxt_fmt_dict() method` is suitably overridden
+        to account for any additional parameters.
+        """
+        logger.info("Saving data to {}".format(self.out_file))
+        header = "\n".join(self.output_file_header)
+        header += "\n" + " ".join(self.output_keys)
+        outfmt = self._get_savetxt_fmt_list()
+        Ncols = len(self.data.dtype)
+        if len(outfmt) != Ncols:
+            raise RuntimeError(
+                "Lengths of data rows ({:d})"
+                " and output format ({:d})"
+                " do not match."
+                " If your search class uses different"
+                " keys than the base GridSearch class,"
+                " override the _get_savetxt_fmt_dict"
+                " method.".format(Ncols, len(outfmt))
+            )
+        np.savetxt(
+            self.out_file,
+            np.nan_to_num(self.data),
+            delimiter=" ",
+            header=header,
+            fmt=outfmt,
+        )
 
-        content = self.get_single_config_line(0)
+    def _convert_F0_to_mismatch(self, F0, F0hat, Tseg):
+        DeltaF0 = F0[1] - F0[0]
+        m_spacing = (np.pi * Tseg * DeltaF0) ** 2 / 12.0
+        N = len(F0)
+        return np.arange(-N * m_spacing / 2.0, N * m_spacing / 2.0, m_spacing)
+
+    def _convert_F1_to_mismatch(self, F1, F1hat, Tseg):
+        DeltaF1 = F1[1] - F1[0]
+        m_spacing = (np.pi * Tseg**2 * DeltaF1) ** 2 / 720.0
+        N = len(F1)
+        return np.arange(-N * m_spacing / 2.0, N * m_spacing / 2.0, m_spacing)
+
+    def _add_mismatch_to_ax(self, ax, x, y, xkey, ykey, xhat, yhat, Tseg):
+        axX = ax.twiny()
+        axX.zorder = -10
+        axY = ax.twinx()
+        axY.zorder = -10
+        if xkey == "F0":
+            m = self._convert_F0_to_mismatch(x, xhat, Tseg)
+            axX.set_xlim(m[0], m[-1])
+        if ykey == "F1":
+            m = self._convert_F1_to_mismatch(y, yhat, Tseg)
+            axY.set_ylim(m[0], m[-1])
 
-        if verbose:
-            logging.info("Injection parameters:")
-            logging.info(content.rstrip("\n"))
-
-        if self.check_if_cff_file_needs_rewriting(content):
-            logging.info("Writing config file: {:s}".format(self.config_file_name))
-            config_file = open(self.config_file_name, "w+")
-            config_file.write(content)
-            config_file.close()
-
-    def check_cached_data_okay_to_use(self, cl_mfd):
-        """Check if SFT files already exist that can be re-used.
-
-        This does not check the actual data contents of the SFTs,
-        but only the following criteria:
-         * filename
-         * if injecting a signal, that the .cff file is older than the SFTs
-           (but its contents should have been checked separately)
-         * that the commandline stored in the (first) SFT header matches
-        """
+    def plot_1D(
+        self,
+        xkey,
+        ax=None,
+        x0=None,
+        xrescale=1,
+        savefig=True,
+        xlabel=None,
+        ylabel=None,
+        agg_chunksize=None,
+    ):
+        """Make a plot of the detection statistic over a single grid dimension.
+
+        Parameters
+        ----------
+        xkey: str
+            The name of the search parameter to plot against.
+        ax: matplotlib.axes._subplots_AxesSubplot or None
+            An optional pre-existing axes set to draw into.
+        x0: float or None
+            Plot x values relative to this central value.
+        xrescale: float
+            Rescale all x values by this factor.
+        savefig : bool
+            If true, save the figure in `self.outdir`.
+            If false, return an axis object without saving to disk.
+        xlabel: str or None
+            Override default text label for the x-axis.
+        ylabel: str or None
+            Override default text label for the y-axis.
+        agg_chunksize: int or None
+            Set this to some high value to work around
+            matplotlib 'Exceeded cell block limit' errors.
+
+        Returns
+        -------
+        ax: matplotlib.axes._subplots_AxesSubplot, optional
+            The axes object containing the plot, only if `savefig=false`.
+        """
+        if agg_chunksize:
+            # FIXME: workaround for matplotlib "Exceeded cell block limit" errors
+            plt.rcParams["agg.path.chunksize"] = agg_chunksize
+        if ax is None:
+            fig, ax = plt.subplots()
+        # x = np.unique(self.data[xkey]) # this doesn't work for multi-dim searches!
+        x = self.data[xkey]
+        if x0:
+            x = x - x0
+        x = x * xrescale
+        z = self.data[self.detstat]
+        ax.plot(x, z)
+        if xlabel:
+            ax.set_xlabel(xlabel)
+        elif x0:
+            ax.set_xlabel(self.tex_labels[xkey] + self.tex_labels0[xkey])
+        else:
+            ax.set_xlabel(self.tex_labels[xkey])
+        if ylabel:
+            ax.set_ylabel(ylabel)
+        else:
+            ax.set_ylabel(self.tex_labels[self.detstat])
+        if savefig:
+            fig.tight_layout()
+            fname = "{}_1D_{}_{}.png".format(self.label, xkey, self.detstat)
+            fig.savefig(os.path.join(self.outdir, fname))
+            plt.close(fig)
+        else:
+            return ax
 
-        need_new = "Will create new SFT file(s)."
+    def plot_2D(
+        self,
+        xkey,
+        ykey,
+        ax=None,
+        savefig=True,
+        vmin=None,
+        vmax=None,
+        add_mismatch=None,
+        xN=None,
+        yN=None,
+        flat_keys=[],
+        rel_flat_idxs=[],
+        flatten_method=np.max,
+        title=None,
+        predicted_twoF=None,
+        cm=None,
+        cbarkwargs={},
+        x0=None,
+        y0=None,
+        colorbar=False,
+        xrescale=1,
+        yrescale=1,
+        xlabel=None,
+        ylabel=None,
+        zlabel=None,
+    ):
+        """Plots the detection statistic over a 2D grid.
 
-        logging.info("Checking if we can re-use existing SFT data file(s)...")
-        sftfiles = self.sftfilepath.split(";")
-        for sftfile in sftfiles:
-            if os.path.isfile(sftfile) is False:
-                logging.info(
-                    "...no SFT file matching '{}' found. {}".format(sftfile, need_new)
-                )
-                return False
-        logging.info("...OK: file(s) found matching '{}'.".format(sftfile))
+        FIXME: this will currently fail if the search went over >2 dimensions.
 
-        if "injectionSources" in cl_mfd:
-            if os.path.isfile(self.config_file_name):
-                if np.any(
-                    [
-                        os.path.getmtime(sftfile)
-                        < os.path.getmtime(self.config_file_name)
-                        for sftfile in sftfiles
-                    ]
-                ):
-                    logging.info(
-                        (
-                            "...the config file '{}' has been modified since"
-                            " creation of the SFT file(s) '{}'. {}"
-                        ).format(self.config_file_name, self.sftfilepath, need_new)
-                    )
-                    return False
-                else:
-                    logging.info(
-                        "...OK: The config file '{}' is older than the SFT file(s)"
-                        " '{}'.".format(self.config_file_name, self.sftfilepath)
-                    )
-                    # NOTE: at this point we assume it's safe to re-use, since
-                    # check_if_cff_file_needs_rewriting()
-                    # should have already been called before
-            else:
-                raise RuntimeError(
-                    "Commandline requires file '{}' but it is missing.".format(
-                        self.config_file_name
-                    )
-                )
+        Parameters
+        ----------
+        xkey: str
+            The name of the first search parameter to plot against.
+        ykey: str
+            The name of the second search parameter to plot against.
+        ax: matplotlib.axes._subplots_AxesSubplot or None
+            An optional pre-existing axes set to draw into.
+        savefig: bool
+            If true, save the figure in `self.outdir`.
+            If false, return an axis object without saving to disk.
+        vmin, vmax: float or None
+            Cutoffs for rescaling the colormap.
+        add_mismatch: tuple or None
+            If given a tuple `(xhat, yhat, Tseg)`,
+            add a secondary axis with the metric mismatch from the
+            point `(xhat, yhat)` with duration `Tseg`.
+        xN, yN: int or  None
+            Number of tick label intervals.
+        flat_keys: list
+            Keys to be used in flattening higher-dimensional arrays.
+        rel_flat_idxs: list
+            Indices to be used in flattening higher-dimensional arrays.
+        flatten_method: numpy function
+            Function to use in flattening the `flat_keys`,
+            default: `np.max`.
+        title: str or None
+            Optional plot title text.
+        predicted_twoF: float or None
+            Expected/predicted value of twoF,
+            used to rescale the z-axis.
+        cm: matplotlib.colors.ListedColormap or None
+            Override standard (viridis) colormap.
+        cbarkwargs: dict
+            Additional arguments for colorbar formatting.
+        x0: float
+            Plot x values relative to this central value.
+        y0: float
+            Plot y values relative to this central value.
+        xrescale: float
+            Rescale all x values by this factor.
+        yrescale: float
+            Rescale all y values by this factor.
+        xlabel: str
+            Override default text label for the x-axis.
+        ylabel: str
+            Override default text label for the y-axis.
+        zlabel: str
+            Override default text label for the z-axis.
+
+        Returns
+        -------
+        ax: matplotlib.axes._subplots_AxesSubplot, optional
+            The axes object containing the plot, only if `savefig=false`.
+        """
+        if ax is None:
+            fig, ax = plt.subplots()
+        flat_idxs = [self.search_keys.index(k) for k in flat_keys]
+
+        x = np.unique(self.data[xkey])
+        if x0:
+            x = x - x0
+        y = np.unique(self.data[ykey])
+        if y0:
+            y = y - y0
+        flat_vals = [np.unique(self.data[:, j]) for j in flat_idxs]
+
+        z = self.data[self.detstat]
+
+        Y, X = np.meshgrid(y, x)
+        shape = [len(x), len(y)] + [len(v) for v in flat_vals]
+        Z = z.reshape(shape)
+
+        if len(rel_flat_idxs) > 0:
+            Z = flatten_method(Z, axis=tuple(rel_flat_idxs))
+
+        if predicted_twoF:
+            Z = (predicted_twoF - Z) / (predicted_twoF + 4)
+            if cm is None:
+                cm = plt.cm.viridis_r
+        else:
+            if cm is None:
+                cm = plt.cm.viridis
 
-        logging.info("...checking new commandline against existing SFT header(s)...")
-        # here we check one SFT header from each SFT file,
-        # assuming that any concatenated file has been sanely constructed with
-        # matching CLs
-        for sftfile in sftfiles:
-            catalog = lalpulsar.SFTdataFind(sftfile, None)
-            cl_old = helper_functions.get_lalapps_commandline_from_SFTDescriptor(
-                catalog.data[0]
-            )
-            if len(cl_old) == 0:
-                logging.info(
-                    "......could not obtain comparison commandline from first SFT"
-                    " header in old file '{}'. {}".format(sftfile, need_new)
-                )
-                return False
-            if not helper_functions.match_commandlines(cl_old, cl_mfd):
-                logging.info(
-                    "......commandlines unmatched for first SFT in old"
-                    " file '{}'. {}".format(sftfile, need_new)
-                )
-                return False
-        logging.info("......OK: Commandline matched with old SFT header(s).")
-        logging.info(
-            "...all data consistency checks passed: Looks like existing"
-            " SFT data matches current options, will re-use it!"
+        pax = ax.pcolormesh(
+            X * xrescale,
+            Y * yrescale,
+            Z,
+            cmap=cm,
+            vmin=vmin,
+            vmax=vmax,
+            shading="auto",
         )
-        return True
+        if colorbar:
+            cb = plt.colorbar(pax, ax=ax, **cbarkwargs)
+            if zlabel:
+                cb.set_label(zlabel)
+            else:
+                cb.set_label(self.tex_labels[self.detstat])
 
-    def check_if_cff_file_needs_rewriting(self, content):
-        """Check if the .cff file has changed
+        if add_mismatch:
+            self.add_mismatch_to_ax(ax, x, y, xkey, ykey, *add_mismatch)
 
-        Returns True if the file should be overwritten - where possible avoid
-        overwriting to allow cached data to be used
-        """
-        logging.info("Checking if we can re-use injection config file...")
-        if os.path.isfile(self.config_file_name) is False:
-            logging.info("...no config file {} found.".format(self.config_file_name))
-            return True
+        if x[-1] > x[0]:
+            ax.set_xlim(x[0] * xrescale, x[-1] * xrescale)
+        if y[-1] > y[0]:
+            ax.set_ylim(y[0] * yrescale, y[-1] * yrescale)
+
+        if xlabel:
+            ax.set_xlabel(xlabel)
+        elif x0:
+            ax.set_xlabel(self.tex_labels[xkey] + self.tex_labels0[xkey])
         else:
-            logging.info(
-                "...OK: config file {} already exists.".format(self.config_file_name)
-            )
-
-        with open(self.config_file_name, "r") as f:
-            file_content = f.read()
-            if file_content == content:
-                logging.info(
-                    "...OK: file contents match, no update of {} required.".format(
-                        self.config_file_name
-                    )
-                )
-                return False
-            else:
-                logging.info(
-                    "...file contents unmatched, updating {}.".format(
-                        self.config_file_name
-                    )
-                )
-                return True
+            ax.set_xlabel(self.tex_labels[xkey])
 
-    def make_data(self, verbose=False):
-        """ A convienience wrapper to generate a cff file then sfts """
-        if self.h0:
-            self.make_cff(verbose)
+        if ylabel:
+            ax.set_ylabel(ylabel)
+        elif y0:
+            ax.set_ylabel(self.tex_labels[ykey] + self.tex_labels0[ykey])
         else:
-            logging.info("Got h0=0, not writing an injection .cff file.")
-        self.run_makefakedata()
+            ax.set_ylabel(self.tex_labels[ykey])
 
-    def run_makefakedata(self):
-        """ Generate the sft data from the configuration file """
+        if title:
+            ax.set_title(title)
 
-        # Remove old data:
-        try:
-            os.unlink(os.path.join(self.outdir, "*" + self.label + "*.sft"))
-        except OSError:
-            pass
-
-        mfd = "lalapps_Makefakedata_v5"
-        cl_mfd = [mfd]
-        cl_mfd.append("--outSingleSFT=TRUE")
-        cl_mfd.append('--outSFTdir="{}"'.format(self.outdir))
-        cl_mfd.append('--outLabel="{}"'.format(self.label))
-
-        if self.noiseSFTs is not None and self.SFTWindowType is None:
-            raise ValueError(
-                "SFTWindowType is required when using noiseSFTs. "
-                "Please, make sure you understand the window function used "
-                "to produce noiseSFTs."
-            )
-        elif self.noiseSFTs is not None:
-            if self.sqrtSX and np.any(
-                [s > 0 for s in helper_functions.parse_list_of_numbers(self.sqrtSX)]
-            ):
-                logging.warning(
-                    "In addition to using noiseSFTs, you are adding "
-                    "Gaussian noise with sqrtSX={} "
-                    "Please, make sure this is what you intend to do.".format(
-                        self.sqrtSX
-                    )
-                )
-            cl_mfd.append('--noiseSFTs="{}"'.format(self.noiseSFTs))
+        if xN:
+            ax.xaxis.set_major_locator(matplotlib.ticker.MaxNLocator(xN))
+        if yN:
+            ax.yaxis.set_major_locator(matplotlib.ticker.MaxNLocator(yN))
+
+        if savefig:
+            fig.tight_layout()
+            fname = "{}_2D_{}_{}_{}.png".format(self.label, xkey, ykey, self.detstat)
+            fig.savefig(os.path.join(self.outdir, fname))
         else:
-            cl_mfd.append(
-                "--IFOs={}".format(
-                    ",".join(['"{}"'.format(d) for d in self.detectors.split(",")])
-                )
-            )
-        if self.sqrtSX:
-            cl_mfd.append('--sqrtSX="{}"'.format(self.sqrtSX))
+            return ax
 
-        if self.SFTWindowType is not None:
-            cl_mfd.append('--SFTWindowType="{}"'.format(self.SFTWindowType))
-            cl_mfd.append("--SFTWindowBeta={}".format(self.SFTWindowBeta))
-        cl_mfd.append("--startTime={}".format(self.tstart))
-        cl_mfd.append("--duration={}".format(self.duration))
-        if hasattr(self, "fmin") and self.fmin:
-            cl_mfd.append("--fmin={:.16g}".format(self.fmin))
-        if hasattr(self, "Band") and self.Band:
-            cl_mfd.append("--Band={:.16g}".format(self.Band))
-        cl_mfd.append("--Tsft={}".format(self.Tsft))
-        if self.h0:
-            cl_mfd.append('--injectionSources="{}"'.format(self.config_file_name))
-        earth_ephem = getattr(self, "earth_ephem", None)
-        sun_ephem = getattr(self, "sun_ephem", None)
-        if earth_ephem is not None:
-            cl_mfd.append('--ephemEarth="{}"'.format(earth_ephem))
-        if sun_ephem is not None:
-            cl_mfd.append('--ephemSun="{}"'.format(sun_ephem))
-        if self.randSeed:
-            cl_mfd.append("--randSeed={}".format(self.randSeed))
-
-        cl_mfd = " ".join(cl_mfd)
-        check_ok = self.check_cached_data_okay_to_use(cl_mfd)
-        if check_ok is False:
-            helper_functions.run_commandline(cl_mfd)
-            if np.all([os.path.isfile(f) for f in self.sftfilepath.split(";")]):
-                logging.info(f"Successfully wrote SFTs to: {self.sftfilepath}")
-            else:
-                raise RuntimeError(
-                    f"It seems we successfully ran {mfd},"
-                    f" but did not get the expected SFT file path(s): {self.sftfilepath}."
-                )
+    def get_max_det_stat(self):
+        """Get the maximum detection statistic over the grid.
+
+        This requires the `run()` method to have been called before.
 
-    def predict_fstat(self, assumeSqrtSX=None):
-        """ Wrapper to lalapps_PredictFstat """
-        twoF_expected, twoF_sigma = helper_functions.predict_fstat(
-            h0=self.h0,
-            cosi=self.cosi,
-            psi=self.psi,
-            Alpha=self.Alpha,
-            Delta=self.Delta,
-            F0=self.F0,
-            sftfilepattern=self.sftfilepath,
-            minStartTime=self.tstart,
-            duration=self.duration,
-            IFOs=self.detectors,
-            assumeSqrtSX=(assumeSqrtSX or self.sqrtSX),
-            tempory_filename=os.path.join(self.outdir, self.label + ".tmp"),
+        Returns
+        -------
+        d: dict
+            Dictionary containing parameters and detection statistic at the maximum.
+        """
+        idx = np.argmax(self.data[self.detstat])
+        d = OrderedDict([(key, self.data[key][idx]) for key in self.output_keys])
+        return d
+
+    def get_max_twoF(self):
+        """Get the maximum twoF over the grid.
+
+        This requires the `run()` method to have been called before.
+
+        Returns
+        -------
+        d: dict
+            Dictionary containing parameters and twoF value at the maximum.
+        """
+        idx = np.argmax(self.data["twoF"])
+        d = OrderedDict([(key, self.data[key][idx]) for key in self.output_keys])
+        return d
+
+    def print_max_twoF(self):
+        """Get and print the maximum twoF point over the grid.
+
+        This prints out the full dictionary from `get_max_twoF()`,
+        i.e. the maximum value and its corresponding parameters.
+        """
+        d = self.get_max_twoF()
+        logger.info("Grid point with max(twoF) for {}:".format(self.label))
+        for k, v in d.items():
+            logger.info("  {}={}".format(k, v))
+
+    def generate_loudest(self):
+        """Use ComputeFstatistic_v2 executable to produce a .loudest file"""
+        max_params = self.get_max_twoF()
+        max_params.pop("twoF")
+        max_params = self.translate_keys_to_lal(max_params)
+        self.loudest_file = utils.generate_loudest_file(
+            max_params=max_params,
+            tref=self.tref,
+            outdir=self.outdir,
+            label=self.label,
+            sftfilepattern=self.sftfilepattern,
+            minStartTime=self.minStartTime,
+            maxStartTime=self.maxStartTime,
+            transientWindowType=getattr(self, "transientWindowType", None),
             earth_ephem=self.earth_ephem,
             sun_ephem=self.sun_ephem,
-            transientWindowType=self.transientWindowType,
-            transientStartTime=self.transientStartTime,
-            transientTau=self.transientTau,
         )
-        return twoF_expected
 
+    def set_out_file(self, extra_label=None):
+        """Set (or reset) the name of the main output file.
 
-class BinaryModulatedWriter(Writer):
-    """ Instance object for generating SFTs containing a continuous wave signal for a source in a binary system """
+        File will always be stored in `self.outdir`
+        and the base of the name be determined from `self.label` and other
+        parts of the search setup,
+        but this method allows to attach an `extra_label` bit if desired.
 
-    @helper_functions.initializer
-    def __init__(
-        self,
-        label="PyFstat",
-        tstart=None,
-        duration=None,
-        tref=None,
-        F0=None,
-        F1=0,
-        F2=0,
-        Alpha=None,
-        Delta=None,
-        tp=0.0,
-        argp=0.0,
-        asini=0.0,
-        ecc=0.0,
-        period=0.0,
-        h0=None,
-        cosi=None,
-        psi=0.0,
-        phi=0,
-        Tsft=1800,
-        outdir=".",
-        sqrtSX=None,
-        noiseSFTs=None,
-        SFTWindowType=None,
-        SFTWindowBeta=0.0,
-        Band=None,
-        detectors=None,
-        earth_ephem=None,
-        sun_ephem=None,
-        transientWindowType="none",
-        transientStartTime=None,
-        transientTau=None,
-        randSeed=None,
-    ):
-        """
         Parameters
-        ----------
-        label: string
-            a human-readable label to be used in naming the output files
-        tstart, duration : int
-            start and duration (in gps seconds) of the total observation span
-        tref: float or None
-            reference time (default is None, which sets the reference time to
-            tstart)
-        F0, F1, F2, Alpha, Delta, tp, argp, asini, ecc, period, h0, cosi, psi, phi: float
-            frequency, sky-position, binary orbit and amplitude parameters
-        Tsft: float
-            the sft duration
-        see `lalapps_Makefakedata_v5 --help` for help with the other paramaters
+        -------
+        extra_label: str
+            Additional text bit to be attached at the end of the filename
+            (but before the extension).
         """
-        self.signal_parameter_labels = super().signal_parameter_labels + [
-            "tp",
-            "argp",
-            "asini",
-            "ecc",
-            "period",
-        ]
-        self.gps_time_and_string_formats_as_LAL["orbitTp"] = ":10.9f"
+        if self.detectors:
+            dets = self.detectors.replace(",", "")
+        else:
+            dets = "NA"
+        if extra_label:
+            self.out_file = os.path.join(
+                self.outdir,
+                "{}_{}_{}_{}.txt".format(
+                    self.label, dets, type(self).__name__, extra_label
+                ),
+            )
+        else:
+            self.out_file = os.path.join(
+                self.outdir,
+                "{}_{}_{}.txt".format(self.label, dets, type(self).__name__),
+            )
 
-        super().__init__(
-            label=label,
-            tstart=tstart,
-            duration=duration,
-            tref=tref,
-            F0=F0,
-            F1=F1,
-            F2=F2,
-            Alpha=Alpha,
-            Delta=Delta,
-            h0=h0,
-            cosi=cosi,
-            psi=psi,
-            phi=phi,
-            Tsft=Tsft,
-            outdir=outdir,
-            sqrtSX=sqrtSX,
-            SFTWindowType=SFTWindowType,
-            SFTWindowBeta=SFTWindowBeta,
-            noiseSFTs=noiseSFTs,
-            Band=Band,
-            detectors=detectors,
-            earth_ephem=earth_ephem,
-            sun_ephem=sun_ephem,
-            transientWindowType=transientWindowType,
-            transientStartTime=transientStartTime,
-            transientTau=transientTau,
-        )
 
+class TransientGridSearch(GridSearch):
+    """A search for transient CW-like signals using the F-statistic.
+
+    This is based on the transient signal model and transient-F-stat algorithm
+    from Prix, Giampanis & Messenger (PRD 84, 023007, 2011):
+    https://arxiv.org/abs/1104.1704
+
+    The frequency evolution parameters are searched over in a grid just like
+    in the normal `GridSearch`, then at each point the time-dependent 'atoms'
+    are used to evaluate partial sums of the F-statistic over a 2D array
+    in transient start times `t0` and duration parameters `tau`.
+
+    The signal templates are modulated by a 'transient window function' which can be
+
+    1. `none` (standard, persistent CW signal)
+
+    2. `rect` (rectangular: constant amplitude within `[t0,t0+tau]`, zero outside)
 
-class GlitchWriter(SearchForSignalWithJumps, Writer):
-    """ Instance object for generating SFTs containing glitch signals """
+    3. `exp` (exponential decay over `[t0,t0+3*tau]`, zero outside)
 
-    @helper_functions.initializer
+    This class currently only supports fully-coherent searches (`nsegs=1` is hardcoded).
+
+    Also see Keitel & Ashton (CQG 35, 205003, 2018):
+    https://arxiv.org/abs/1805.05652
+    for a detailed discussion of the GPU implementation.
+
+    NOTE for GPU users (`tCWFstatMapVersion="pycuda"`):
+    The underlying `ComputeFstat` class tries to
+    conveniently deal with GPU context management behind the scenes.
+    A known problematic case is if you try to instantiate it twice from the same
+    session/script. If you then get some messages like
+    `RuntimeError: make_default_context()`
+    and `invalid device context`,
+    that is because the GPU is still blocked from the first instance when
+    you try to initiate the second.
+    To avoid this problem, use context management::
+
+        with pyfstat.TransientGridSearch(
+            [...],
+            tCWFstatMapVersion="pycuda",
+        ) as search:
+            search.search.run()
+
+    or manually call the `search.search.finalizer_()` method where needed.
+
+    Most parameters are the same as for `GridSearch`
+    and the `core.ComputeFstat` class,
+    only the additional ones are documented here:
+    """
+
+    @utils.initializer
     def __init__(
         self,
-        label="PyFstat",
-        tstart=None,
-        duration=None,
-        dtglitch=None,
-        delta_phi=0,
-        delta_F0=0,
-        delta_F1=0,
-        delta_F2=0,
+        label,
+        outdir,
+        sftfilepattern,
+        F0s,
+        F1s,
+        F2s,
+        Alphas,
+        Deltas,
         tref=None,
-        F0=None,
-        F1=0,
-        F2=0,
-        Alpha=None,
-        Delta=None,
-        h0=None,
-        cosi=None,
-        psi=0.0,
-        phi=0,
-        Tsft=1800,
-        outdir=".",
-        sqrtSX=None,
-        noiseSFTs=None,
-        SFTWindowType=None,
-        SFTWindowBeta=0.0,
-        Band=None,
+        minStartTime=None,
+        maxStartTime=None,
+        BSGL=False,
+        BtSG=False,
+        minCoverFreq=None,
+        maxCoverFreq=None,
         detectors=None,
+        SSBprec=None,
+        RngMedWindow=None,
+        injectSources=None,
+        input_arrays=False,
+        assumeSqrtSX=None,
+        transientWindowType=None,
+        t0Band=None,
+        tauBand=None,
+        tauMin=None,
+        dt0=None,
+        dtau=None,
+        outputTransientFstatMap=False,
+        outputAtoms=False,
+        tCWFstatMapVersion="lal",
+        cudaDeviceName=None,
         earth_ephem=None,
         sun_ephem=None,
-        transientWindowType="rect",
-        randSeed=None,
+        clean=False,
     ):
         """
         Parameters
         ----------
-        label: string
-            a human-readable label to be used in naming the output files
-        tstart, duration : float
-            start and duration (in gps seconds) of the total observation span
-        dtglitch: float
-            time (in gps seconds) of the glitch after tstart. To create data
-            without a glitch, set dtglitch=None
-        delta_phi, delta_F0, delta_F1: float
-            instanteneous glitch magnitudes in rad, Hz, and Hz/s respectively
-        tref: float or None
-            reference time (default is None, which sets the reference time to
-            tstart)
-        F0, F1, F2, Alpha, Delta, h0, cosi, psi, phi: float
-            frequency, sky-position, and amplitude parameters
-        Tsft: float
-            the sft duration
-
-        see `lalapps_Makefakedata_v5 --help` for help with the other paramaters
-        """
-
-        self.set_ephemeris_files(earth_ephem, sun_ephem)
-        self.basic_setup()
-        self.calculate_fmin_Band()
-
-        shapes = np.array(
-            [
-                np.shape(x)
-                for x in [self.delta_phi, self.delta_F0, self.delta_F1, self.delta_F2]
+        transientWindowType: str
+            If `rect` or `exp`,
+            allow for the Fstat to be computed over a transient range.
+            (`none` instead of `None` explicitly calls the transient-window
+            function, but with the full range, for debugging.)
+        t0Band, tauBand: int
+            Search ranges for transient start-time t0 and duration tau.
+            If >0, search `t0` in `(minStartTime,minStartTime+t0Band)`
+            and tau in `(tauMin,2*Tsft+tauBand)`.
+            If =0, only compute the continuous-wave F-stat with `t0=minStartTime`,
+            `tau=maxStartTime-minStartTime`.
+        tauMin: int
+            Minimum transient duration to cover,
+            defaults to `2*Tsft`.
+        dt0: int
+            Grid resolution in transient start-time,
+            defaults to `Tsft`.
+        dtau: int
+            Grid resolution in transient duration,
+            defaults to `Tsft`.
+        outputTransientFstatMap: bool
+            If true, write additional output files for `(t0,tau)` F-stat maps.
+            (One file for each grid point!)
+        outputAtoms: bool
+            If true, write additional output files for the F-stat `atoms`.
+            (One file for each grid point!)
+        tCWFstatMapVersion: str
+            Choose between implementations of the transient F-statistic funcionality:
+            standard `lal` implementation,
+            `pycuda` for GPU version,
+            and some others only for devel/debug.
+        cudaDeviceName: str
+            GPU name to be matched against drv.Device output,
+            only for `tCWFstatMapVersion=pycuda`.
+        """
+
+        self._set_init_params_dict(locals())
+        self.nsegs = 1
+        os.makedirs(outdir, exist_ok=True)
+        self.set_out_file()
+        self.search_keys = ["F0", "F1", "F2", "Alpha", "Delta"]
+        for k in self.search_keys:
+            setattr(self, k, np.atleast_1d(getattr(self, k + "s")))
+        if self.BSGL and self.BtSG:  # pragma: no cover
+            raise ValueError("Please choose only one of [BSGL,BtSG].")
+        elif self.BSGL:
+            self.detstat = "log10BSGL"
+        elif self.BtSG:
+            self.detstat = "lnBtSG"
+        else:
+            self.detstat = "maxTwoF"
+        self._initiate_search_object()
+        self._set_output_keys()
+        self.output_file_header = self.get_output_file_header()
+        if self.outputTransientFstatMap:
+            self.tCWfilebase = os.path.splitext(self.out_file)[0] + "_tCW_"
+            logger.info(
+                "Will save per-Doppler Fstatmap"
+                " results to {}*.dat".format(self.tCWfilebase)
+            )
+
+    def __enter__(self):
+        logger.debug("Entering the TransientGridSearch context...")
+        self.search.__enter__()
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        logger.debug("Leaving the TransientGridSearch context...")
+        self.search.__exit__(*args, **kwargs)
+
+    def _set_output_keys(self):
+        self.output_keys = self.search_keys.copy()
+        self.output_keys.append("twoF")
+        if self.search.singleFstats:
+            self.output_keys += [f"twoF{IFO}" for IFO in self.search.detector_names]
+        if self.transientWindowType:
+            self.output_keys.append("maxTwoF")
+        if hasattr(self.search, "twoFXatMaxTwoF"):
+            self.output_keys += [
+                f"twoF{IFO}atMaxTwoF" for IFO in self.search.detector_names
             ]
+        if self.detstat != "maxTwoF":
+            self.output_keys.append(self.detstat)
+        if self.transientWindowType:
+            # for consistency below, t0/tau must come after detstat
+            # they are not included in self.search_keys because the main Fstat
+            # code does not loop over them
+            self.output_keys += ["t0", "tau"]
+
+    def _initiate_search_object(self):
+        logger.info("Setting up search object")
+        search_ranges = self._get_search_ranges()
+        self.search = ComputeFstat(
+            tref=self.tref,
+            sftfilepattern=self.sftfilepattern,
+            minCoverFreq=self.minCoverFreq,
+            maxCoverFreq=self.maxCoverFreq,
+            search_ranges=search_ranges,
+            detectors=self.detectors,
+            transientWindowType=self.transientWindowType,
+            t0Band=self.t0Band,
+            tauBand=self.tauBand,
+            tauMin=self.tauMin,
+            dt0=self.dt0,
+            dtau=self.dtau,
+            minStartTime=self.minStartTime,
+            maxStartTime=self.maxStartTime,
+            BSGL=self.BSGL,
+            BtSG=self.BtSG,
+            SSBprec=self.SSBprec,
+            RngMedWindow=self.RngMedWindow,
+            injectSources=self.injectSources,
+            assumeSqrtSX=self.assumeSqrtSX,
+            tCWFstatMapVersion=self.tCWFstatMapVersion,
+            cudaDeviceName=self.cudaDeviceName,
+            computeAtoms=self.outputAtoms,
+            earth_ephem=self.earth_ephem,
+            sun_ephem=self.sun_ephem,
         )
-        if not np.all(shapes == shapes[0]):
-            raise ValueError("all delta_* must be the same shape: {}".format(shapes))
-
-        for d in self.delta_phi, self.delta_F0, self.delta_F1, self.delta_F2:
-            if np.size(d) == 1:
-                d = np.atleast_1d(d)
-
-        if self.dtglitch is None:
-            self.tbounds = [self.tstart, self.tend()]
-        else:
-            self.dtglitch = np.atleast_1d(self.dtglitch)
-            self.tglitch = self.tstart + self.dtglitch
-            self.tbounds = np.concatenate(([self.tstart], self.tglitch, [self.tend()]))
-        logging.info("Using segment boundaries {}".format(self.tbounds))
+        # make sure to overwrite the min/max starttime in case the user
+        # passed None and they were read from SFTs
+        self.minStartTime = self.search.minStartTime
+        self.maxStartTime = self.search.maxStartTime
+
+    def run(self, return_data=False):
+        """Execute the actual search over the full grid.
+
+        This iterates over all points in the multi-dimensional product grid
+        and the end result is either returned as a numpy array or saved to disk.
+
+        If the `outputTransientFstatMap` or `outputAtoms` options have been set
+        when initiating the search,
+        additional files are written for each
+        frequency-evolution parameter-space point ('Doppler' point).
 
-        tbs = np.array(self.tbounds)
-        self.durations = tbs[1:] - tbs[:-1]
+        Parameters
+        ----------
+        return_data: boolean
+            If true, the final inputs+outputs data set is returned as a numpy array.
+            If false, it is saved to disk and nothing is returned.
+
+        Returns
+        -------
+        data: np.ndarray
+            The final inputs+outputs data set.
+            Only if `return_data=true`.
+        """
+        self._get_input_data_array()
+        old_data = self.check_old_data_is_okay_to_use()
+        if old_data is not False:
+            self.data = old_data
+            return
 
-        self.delta_thetas = np.atleast_2d(
-            np.array([delta_phi, delta_F0, delta_F1, delta_F2]).T
+        output_dtype = np.dtype(
+            {
+                "names": self.output_keys,
+                "formats": np.repeat(float, len(self.output_keys)),
+            }
         )
-
-    def get_base_template(self, i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref):
-        """FIXME: ported over from Writer,
-        should be replaced by a more elegant re-use of parse_args_consistent_with_mfd
-        """
-        return """[TS{}]
-Alpha = {:1.18e}
-Delta = {:1.18e}
-h0 = {:1.18e}
-cosi = {:1.18e}
-psi = {:1.18e}
-phi0 = {:1.18e}
-Freq = {:1.18e}
-f1dot = {:1.18e}
-f2dot = {:1.18e}
-refTime = {:10.6f}"""
-
-    def get_single_config_line_cw(
-        self, i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
-    ):
-        template = (
-            self.get_base_template(
-                i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
+        data = np.zeros(len(self.input_data), dtype=output_dtype)
+        self.timingFstatMap = 0.0
+        logger.info(
+            "Running search over a total of {:d} grid points...".format(
+                np.shape(self.input_data)[0]
             )
-            + """\n"""
         )
-        return template.format(i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref)
-
-    def get_single_config_line_tcw(
-        self,
-        i,
-        Alpha,
-        Delta,
-        h0,
-        cosi,
-        psi,
-        phi,
-        F0,
-        F1,
-        F2,
-        tref,
-        window,
-        transientStartTime,
-        transientTau,
-    ):
-        template = (
-            self.get_base_template(
-                i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
-            )
-            + """
-transientWindowType = {:s}
-transientStartTime = {:10.0f}
-transientTau = {:10.0f}\n"""
-        )
-        return template.format(
-            i,
-            Alpha,
-            Delta,
-            h0,
-            cosi,
-            psi,
-            phi,
-            F0,
-            F1,
-            F2,
-            tref,
-            window,
-            transientStartTime,
-            transientTau,
+        for n, vals in enumerate(tqdm(self.input_data)):
+            thisCand = list(vals)
+            detstat = self.search.get_det_stat(*vals)
+            windowRange = getattr(self.search, "windowRange", None)
+            self.timingFstatMap += getattr(self.search, "timingFstatMap", 0.0)
+            thisCand.append(self.search.twoF)
+            if self.search.singleFstats:
+                thisCand += list(self.search.twoFX[: self.search.numDetectors])
+            if hasattr(self.search, "maxTwoF"):
+                thisCand.append(self.search.maxTwoF)
+            if hasattr(self.search, "twoFXatMaxTwoF"):
+                thisCand += list(self.search.twoFXatMaxTwoF[: self.search.numDetectors])
+            if self.detstat != "maxTwoF":
+                thisCand.append(detstat)
+            if getattr(self, "transientWindowType", None):
+                if not hasattr(self.search, "FstatMap"):
+                    raise RuntimeError(
+                        "Since transientWindowType!=None, we expected to have a FstatMap."
+                    )
+                if self.outputTransientFstatMap:
+                    tCWfile = self.get_transient_fstat_map_filename(thisCand)
+                    self.search.FstatMap.write_F_mn_to_file(
+                        tCWfile, windowRange, self.output_file_header
+                    )
+                maxidx = self.search.FstatMap.get_maxF_idx()
+                thisCand += [
+                    windowRange.t0 + maxidx[0] * windowRange.dt0,
+                    windowRange.tau + maxidx[1] * windowRange.dtau,
+                ]
+            for k, key in enumerate(self.output_keys):
+                data[key][n] = thisCand[k]
+            if self.outputAtoms:
+                self.search.write_atoms_to_file(os.path.splitext(self.out_file)[0])
+
+        logger.info(
+            "Total time spent computing transient F-stat maps: {:.2f}s".format(
+                self.timingFstatMap
+            )
         )
 
-    def get_single_config_line(
-        self,
-        i,
-        Alpha,
-        Delta,
-        h0,
-        cosi,
-        psi,
-        phi,
-        F0,
-        F1,
-        F2,
-        tref,
-        window,
-        transientStartTime,
-        transientTau,
-    ):
-        if window == "none":
-            return self.get_single_config_line_cw(
-                i, Alpha, Delta, h0, cosi, psi, phi, F0, F1, F2, tref
-            )
+        if return_data:
+            return data
         else:
-            return self.get_single_config_line_tcw(
-                i,
-                Alpha,
-                Delta,
-                h0,
-                cosi,
-                psi,
-                phi,
-                F0,
-                F1,
-                F2,
-                tref,
-                window,
-                transientStartTime,
-                transientTau,
-            )
-
-    def make_cff(self, verbose=False):
-        """
-        Generates an .cff file for a 'glitching' signal
-
-        """
+            self.data = data
+            self.save_array_to_disk()
 
-        thetas = self._calculate_thetas(self.theta, self.delta_thetas, self.tbounds)
+    def get_transient_fstat_map_filename(self, param_point):
+        """Filename convention for given grid point: freq_alpha_delta_f1dot_f2dot
 
-        content = ""
-        for i, (t, d, ts) in enumerate(zip(thetas, self.durations, self.tbounds[:-1])):
-            line = self.get_single_config_line(
-                i,
-                self.Alpha,
-                self.Delta,
-                self.h0,
-                self.cosi,
-                self.psi,
-                t[0],
-                t[1],
-                t[2],
-                t[3],
-                self.tref,
-                self.transientWindowType,
-                ts,
-                d,
-            )
-
-            content += line
-
-        if verbose:
-            logging.info("Injection parameters:")
-            logging.info(content.rstrip("\n"))
-
-        if self.check_if_cff_file_needs_rewriting(content):
-            logging.info("Writing config file: {:s}".format(self.config_file_name))
-            config_file = open(self.config_file_name, "w+")
-            config_file.write(content)
-            config_file.close()
+        Parameters
+        ----------
+        param_point: tuple, dict, list, np.void or np.ndarray
+            A multi-dimensional parameter point.
+            If not a type with named fields (e.g. a plain tuple or list),
+            the order must match that of `self.output_keys`.
+
+        Returns
+        -------
+        f: str
+            The constructed filename.
+        """
+        fmt_keys = ["F0", "Alpha", "Delta", "F1", "F2"]
+        fmt = "{:.16g}_{:.16g}_{:.16g}_{:.16g}_{:.16g}"
+        if isinstance(param_point, tuple) or isinstance(param_point, np.void):
+            param_point = list(param_point)
+        if isinstance(param_point, dict):
+            vals = [param_point[key] for key in fmt_keys]
+        elif isinstance(param_point, list) or isinstance(param_point, np.ndarray):
+            vals = [param_point[self.output_keys.index(key)] for key in fmt_keys]
+        else:
+            raise ValueError("param_point must be a dict, list, tuple or numpy array!")
+        f = self.tCWfilebase + fmt.format(*vals) + ".dat"
+        return f
 
+    def _get_savetxt_fmt_dict(self):
+        """Define the output precision for each parameter and computed quantity."""
+        fmt_dict = utils.get_doppler_params_output_format(self.output_keys)
+        fmt_dict["twoF"] = self.fmt_detstat
+        if self.search.singleFstats:
+            for IFO in self.search.detector_names:
+                fmt_dict[f"twoF{IFO}"] = self.fmt_detstat
+        fmt_dict["maxTwoF"] = self.fmt_detstat
+        if hasattr(self.search, "twoFXatMaxTwoF"):
+            for IFO in self.search.detector_names:
+                fmt_dict[f"twoF{IFO}atMaxTwoF"] = self.fmt_detstat
+        if self.detstat != "maxTwoF":
+            fmt_dict[self.detstat] = self.fmt_detstat
+        fmt_dict["t0"] = "%d"
+        fmt_dict["tau"] = "%d"
+        return fmt_dict
+
+
+class SliceGridSearch(DefunctClass):
+    last_supported_version = "1.9.0"
+
+
+class GridUniformPriorSearch(DefunctClass):
+    last_supported_version = "1.9.0"
+
+
+class GridGlitchSearch(GridSearch):
+    """A grid search using the `SemiCoherentGlitchSearch` class.
+
+    This implements a basic semi-coherent F-stat search in which the data
+    is divided into segments either side of the proposed glitch epochs and the
+    fully-coherent F-stat in each segment is summed to give the semi-coherent
+    F-stat.
 
-class FrequencyModulatedArtifactWriter(Writer):
-    """ Instance object for generating SFTs containing artifacts """
+    This class currently only works for a single glitch in the observing time.
+    """
 
-    @helper_functions.initializer
+    @utils.initializer
     def __init__(
         self,
         label,
-        outdir=".",
-        tstart=700000000,
-        duration=86400,
-        F0=30,
-        F1=0,
+        outdir="data",
+        sftfilepattern=None,
+        F0s=[0],
+        F1s=[0],
+        F2s=[0],
+        delta_F0s=[0],
+        delta_F1s=[0],
+        tglitchs=None,
+        Alphas=[0],
+        Deltas=[0],
         tref=None,
-        h0=10,
-        Tsft=1800,
-        sqrtSX=0.0,
-        Band=4,
-        Pmod=lal.DAYSID_SI,
-        Pmod_phi=0,
-        Pmod_amp=1,
-        Alpha=None,
-        Delta=None,
+        minStartTime=None,
+        maxStartTime=None,
+        minCoverFreq=None,
+        maxCoverFreq=None,
         detectors=None,
         earth_ephem=None,
         sun_ephem=None,
-        randSeed=None,
+        clean=False,
     ):
         """
+        Most parameters are the same as for `GridSearch`
+        and the `core.SemiCoherentGlitchSearch` class,
+        only the additional ones are documented here:
+
         Parameters
         ----------
-        tstart, duration : int
-            start and duration times (in gps seconds) of the total observation
-        Pmod, F0, F1 h0: float
-            Modulation period, freq, freq-drift, and h0 of the artifact
-        Alpha, Delta: float
-            Sky position, in radians, of a signal of which to add the orbital
-            modulation to the artifact, if not `None`.
-        Tsft: float
-            the sft duration
-        sqrtSX: float
-            Background IFO noise
-
-        see `lalapps_Makefakedata_v4 --help` for help with the other paramaters
-        """
-
-        self.phi = 0
-        self.F2 = 0
-
-        self.basic_setup()
-        self.set_ephemeris_files(earth_ephem, sun_ephem)
-        self.tstart = int(tstart)
-        self.duration = int(duration)
-
-        if os.path.isdir(self.outdir) is False:
-            os.makedirs(self.outdir)
-        if tref is None:
-            raise ValueError("Input `tref` not specified")
-
-        self.nsfts = int(np.ceil(self.duration / self.Tsft))
-        self.calculate_fmin_Band()
-
-        self.cosi = 0
-        self.Fmax = F0
-
-        if Alpha is not None and Delta is not None:
-            self.n = np.array(
-                [
-                    np.cos(Alpha) * np.cos(Delta),
-                    np.sin(Alpha) * np.cos(Delta),
-                    np.sin(Delta),
-                ]
-            )
-
-    def get_frequency(self, t):
-        DeltaFDrift = self.F1 * (t - self.tref)
-
-        phir = 2 * np.pi * t / self.Pmod + self.Pmod_phi
-
-        if self.Alpha is not None and self.Delta is not None:
-            spin_posvel = lalpulsar.PosVel3D_t()
-            orbit_posvel = lalpulsar.PosVel3D_t()
-            det = lal.CachedDetectors[4]
-            ephems = lalpulsar.InitBarycenter(self.earth_ephem, self.sun_ephem)
-            lalpulsar.DetectorPosVel(
-                spin_posvel,
-                orbit_posvel,
-                lal.LIGOTimeGPS(t),
-                det,
-                ephems,
-                lalpulsar.DETMOTION_ORBIT,
-            )
-            # Pos and vel returned in units of c
-            DeltaFOrbital = np.dot(self.n, orbit_posvel.vel) * self.Fmax
-
-            if self.detectors == "H1":
-                Lambda = lal.LHO_4K_DETECTOR_LATITUDE_RAD
-            elif self.detectors == "L1":
-                Lambda = lal.LLO_4K_DETECTOR_LATITUDE_RAD
-            else:
-                raise ValueError(
-                    "This class currently only supports detectors H1 or L1."
-                )
-
-            DeltaFSpin = (
-                self.Pmod_amp
-                * lal.REARTH_SI
-                / lal.C_SI
-                * 2
-                * np.pi
-                / self.Pmod
-                * (np.cos(self.Delta) * np.cos(Lambda) * np.sin(self.Alpha - phir))
-                * self.Fmax
-            )
-        else:
-            DeltaFOrbital = 0
-            DeltaFSpin = 2 * np.pi * self.Pmod_amp / self.Pmod * np.cos(phir)
-
-        f = self.F0 + DeltaFDrift + DeltaFOrbital + DeltaFSpin
-        return f
-
-    def get_h0(self, t):
-        return self.h0
-
-    def concatenate_sft_files(self):
-        SFTFilename = lalpulsar.OfficialSFTFilename(
-            self.detectors[0],
-            self.detectors[1],
-            self.nsfts,
-            self.Tsft,
-            int(self.tstart),
-            int(self.duration),
-            self.label,
-        )
-        SFTFile_fullpath = os.path.join(self.outdir, SFTFilename)
-
-        # If the file already exists, simply remove it for now (no caching
-        # implemented)
-        helper_functions.run_commandline(
-            "rm {}".format(SFTFile_fullpath), raise_error=False, log_level=10
+        delta_F0s: tuple
+            A length 3 tuple describing the grid of frequency jumps,
+            or just `[delta_F0]` for a fixed value.
+        delta_F1s: tuple
+            A length 3 tuple describing the grid of spindown parameter jumps,
+            or just `[delta_F1]` for a fixed value.
+        tglitchs: tuple
+            A length 3 tuple describing the grid of glitch epochs,
+            or just `[tglitch]` for a fixed value.
+            These are relative time offsets, referenced to zero at `minStartTime`.
+        """
+
+        self._set_init_params_dict(locals())
+        os.makedirs(outdir, exist_ok=True)
+        self.set_out_file()
+        self.BSGL = False
+        self.input_arrays = False
+        if tglitchs is None:
+            raise ValueError("You must specify `tglitchs`")
+        self.search_keys = [
+            "F0",
+            "F1",
+            "F2",
+            "Alpha",
+            "Delta",
+            "delta_F0",
+            "delta_F1",
+            "tglitch",
+        ]
+        for k in self.search_keys:
+            setattr(self, k, np.atleast_1d(getattr(self, k + "s")))
+        self.detstat = "twoF"
+        self._initiate_search_object()
+        self._set_output_keys()
+        self.output_file_header = self.get_output_file_header()
+
+    def _initiate_search_object(self):
+        logger.info("Setting up search object")
+        search_ranges = self._get_search_ranges()
+        self.search = SemiCoherentGlitchSearch(
+            label=self.label,
+            outdir=self.outdir,
+            sftfilepattern=self.sftfilepattern,
+            tref=self.tref,
+            minStartTime=self.minStartTime,
+            maxStartTime=self.maxStartTime,
+            minCoverFreq=self.minCoverFreq,
+            maxCoverFreq=self.maxCoverFreq,
+            search_ranges=search_ranges,
+            BSGL=self.BSGL,
+            earth_ephem=self.earth_ephem,
+            sun_ephem=self.sun_ephem,
         )
 
-        inpattern = os.path.join(self.tmp_outdir, "*sft")
-        cl_splitSFTS = "lalapps_splitSFTs -fs {} -fb {} -fe {} -o {} -i {}".format(
-            self.fmin, self.Band, self.fmin + self.Band, SFTFile_fullpath, inpattern
-        )
-        helper_functions.run_commandline(cl_splitSFTS)
-        helper_functions.run_commandline("rm {} -r".format(self.tmp_outdir))
-        files = glob.glob(SFTFile_fullpath + "*")
-        if len(files) == 1:
-            fn = files[0]
-            fn_new = fn.split(".")[0] + ".sft"
-            helper_functions.run_commandline("mv {} {}".format(fn, fn_new))
-        else:
-            raise IOError(
-                "Attempted to rename file, but multiple files found: {}".format(files)
-            )
+    def _get_savetxt_fmt_dict(self):
+        """Define the output precision for each parameter and computed quantity."""
+        fmt_dict = utils.get_doppler_params_output_format(self.output_keys)
+        fmt_dict["delta_F0"] = "%.16g"
+        fmt_dict["delta_F1"] = "%.16g"
+        fmt_dict["tglitch"] = "%d"
+        fmt_dict[self.detstat] = self.fmt_detstat
+        return fmt_dict
 
-    def pre_compute_evolution(self):
-        logging.info("Precomputing evolution parameters")
-        self.lineFreqs = []
-        self.linePhis = []
-        self.lineh0s = []
-        self.mid_times = []
-
-        linePhi = 0
-        lineFreq_old = 0
-        for i in tqdm(list(range(self.nsfts))):
-            mid_time = self.tstart + (i + 0.5) * self.Tsft
-            lineFreq = self.get_frequency(mid_time)
-
-            self.mid_times.append(mid_time)
-            self.lineFreqs.append(lineFreq)
-            self.linePhis.append(
-                linePhi + np.pi * self.Tsft * (lineFreq_old + lineFreq)
-            )
-            self.lineh0s.append(self.get_h0(mid_time))
-
-            lineFreq_old = lineFreq
-
-    def make_ith_sft(self, i):
-        try:
-            self.run_makefakedata_v4(
-                self.mid_times[i],
-                self.lineFreqs[i],
-                self.linePhis[i],
-                self.lineh0s[i],
-                self.tmp_outdir,
-            )
-        except KeyboardInterrupt:
-            raise KeyboardInterruptError()
-
-    def make_data(self):
-        self.duration = self.Tsft
-
-        self.tmp_outdir = os.path.join(self.outdir, self.label + "_tmp")
-        if os.path.isdir(self.tmp_outdir) is True:
-            raise ValueError(
-                "Temporary directory {} already exists, please rename".format(
-                    self.tmp_outdir
-                )
-            )
-        else:
-            os.makedirs(self.tmp_outdir)
 
-        self.pre_compute_evolution()
+class SlidingWindow(DefunctClass):
+    last_supported_version = "1.9.0"
 
-        logging.info("Generating SFTs")
 
-        if args.N > 1 and pkgutil.find_loader("pathos") is not None:
-            import pathos.pools
+class FrequencySlidingWindow(DefunctClass):
+    last_supported_version = "1.9.0"
 
-            logging.info("Using {} threads".format(args.N))
-            try:
-                with pathos.pools.ProcessPool(args.N) as p:
-                    list(
-                        tqdm(
-                            p.imap(self.make_ith_sft, list(range(self.nsfts))),
-                            total=self.nsfts,
-                        )
-                    )
-            except KeyboardInterrupt:
-                p.terminate()
-        else:
-            logging.info(
-                "No multiprocessing requested or `pathos` not install, cont."
-                " without multiprocessing"
-            )
-            for i in tqdm(list(range(self.nsfts))):
-                self.make_ith_sft(i)
-
-        self.concatenate_sft_files()
-
-    def run_makefakedata_v4(self, mid_time, lineFreq, linePhi, h0, tmp_outdir):
-        """ Generate the sft data using the --lineFeature option """
-        cl_mfd = []
-        cl_mfd.append("lalapps_Makefakedata_v4")
-        cl_mfd.append("--outSingleSFT=FALSE")
-        cl_mfd.append('--outSFTbname="{}"'.format(tmp_outdir))
-        cl_mfd.append("--IFO={}".format(self.detectors))
-        cl_mfd.append('--noiseSqrtSh="{}"'.format(self.sqrtSX))
-        cl_mfd.append("--startTime={:0.0f}".format(mid_time - self.Tsft / 2.0))
-        cl_mfd.append("--refTime={:0.0f}".format(mid_time))
-        cl_mfd.append("--duration={}".format(self.duration))
-        cl_mfd.append("--fmin={:.16g}".format(self.fmin))
-        cl_mfd.append("--Band={:.16g}".format(self.Band))
-        cl_mfd.append("--Tsft={}".format(self.Tsft))
-        cl_mfd.append("--Freq={}".format(lineFreq))
-        cl_mfd.append("--phi0={}".format(linePhi))
-        cl_mfd.append("--h0={}".format(h0))
-        cl_mfd.append("--cosi={}".format(self.cosi))
-        cl_mfd.append("--lineFeature=TRUE")
-        earth_ephem = getattr(self, "earth_ephem", None)
-        sun_ephem = getattr(self, "sun_ephem", None)
-        if earth_ephem is not None:
-            cl_mfd.append('--ephemEarth="{}"'.format(earth_ephem))
-        if sun_ephem is not None:
-            cl_mfd.append('--ephemSun="{}"'.format(sun_ephem))
-        if self.randSeed:
-            cl_mfd.append("--randSeed={}".format(self.randSeed))
-        cl_mfd = " ".join(cl_mfd)
-        helper_functions.run_commandline(cl_mfd, log_level=10)
 
+class EarthTest(DefunctClass):
+    last_supported_version = "1.9.0"
 
-class FrequencyAmplitudeModulatedArtifactWriter(FrequencyModulatedArtifactWriter):
-    """ Instance object for generating SFTs containing artifacts """
 
-    def get_h0(self, t):
-        return self.h0 * np.sin(2 * np.pi * t / self.Pmod + self.Pmod_phi)
+class DMoff_NO_SPIN(DefunctClass):
+    last_supported_version = "1.9.0"
```

### Comparing `PyFstat-1.9.0/pyfstat/mcmc_based_searches.py` & `PyFstat-2.0.0/pyfstat/mcmc_based_searches.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,138 +1,121 @@
-""" Searches using MCMC-based methods """
+"""PyFstat search & follow-up classes using MCMC-based methods
 
+The general approach is described in
+Ashton & Prix (PRD 97, 103020, 2018):
+https://arxiv.org/abs/1802.05450
+and we use the `ptemcee` sampler
+described in Vousden et al. (MNRAS 455, 1919-1937, 2016):
+https://arxiv.org/abs/1501.05823
+and based on Foreman-Mackey et al. (PASP 125, 306, 2013):
+https://arxiv.org/abs/1202.3665
+
+Defining the prior
+##################
+
+The MCMC based searches (i.e. `pyfstat.MCMC*`) require a prior specification for each model parameter,
+implemented via a `python dictionary <https://docs.python.org/tutorial/datastructures.html#dictionaries>`_.
+This is best explained through a simple example, here is the prior for a *directed* search with a *uniform*
+prior on the frequency and a *normal* prior on the frequency derivative:
+
+.. code-block:: python
+
+    theta_prior = {'F0': {'type': 'unif',
+                          'lower': 29.9,
+                          'upper': 30.1},
+                   'F1': {'type': 'norm',
+                          'loc': 0,
+                          'scale': 1e-10},
+                   'F2': 0,
+                   'Alpha': 2.3,
+                   'Delta': 1.8
+                   }
+
+For the sky positions ``Alpha`` and ``Delta``, we give the fixed values (i.e. they are considered *known* by
+the MCMC simulation), the same is true for ``F2``, the second derivative of the frequency which we fix at ``0``.
+Meanwhile, for the frequency ``F0`` and first frequency derivative ``F1`` we give a dictionary specifying their
+prior distribution. This dictionary must contain three arguments: the ``type`` (in this case either ``unif`` or
+``norm``) which specifies the type of distribution, then two shape arguments. The shape parameters will depend
+on the ``type`` of distribution, but here we use ``lower`` and ``upper``, required for the ``unif`` prior while
+``loc`` and ``scale`` are required for the ``norm`` prior.
+
+Currently, two other types of prior are implemented: ``halfnorm``, ``neghalfnorm`` (both of which require ``loc``
+and ``scale`` shape parameters). Further priors can be added by modifying ``pyfstat.MCMCSearch._generic_lnprior``.
+
+"""
 
-import sys
-import os
 import copy
 import logging
+import os
+import sys
 from collections import OrderedDict
 
-import numpy as np
+import corner
+import dill as pickle
 import matplotlib
 import matplotlib.pyplot as plt
+import numpy as np
 from ptemcee import Sampler as PTSampler
-import corner
-import dill as pickle
 from scipy.stats import lognorm
+from tqdm import tqdm
 
 import pyfstat.core as core
-from pyfstat.core import BaseSearchClass, tqdm, args
 import pyfstat.optimal_setup_functions as optimal_setup_functions
-import pyfstat.helper_functions as helper_functions
+import pyfstat.utils as utils
+from pyfstat.core import BaseSearchClass
 
+logger = logging.getLogger(__name__)
 
-class MCMCSearch(BaseSearchClass):
-    """MCMC search using ComputeFstat
 
-    Parameters
-    ----------
-    theta_prior: dict
-        Dictionary of priors and fixed values for the search parameters.
-        For each parameters (key of the dict), if it is to be held fixed
-        the value should be the constant float, if it is be searched, the
-        value should be a dictionary of the prior.
-    tref, minStartTime, maxStartTime: int
-        GPS seconds of the reference time, start time and end time. While tref
-        is requirede, minStartTime and maxStartTime default to None in which
-        case all available data is used.
-    label, outdir: str
-        A label and output directory (optional, defaults is `'data'`) to
-        name files
-    sftfilepattern: str, optional
-        Pattern to match SFTs using wildcards (*?) and ranges [0-9];
-        mutiple patterns can be given separated by colons.
-    detectors: str, optional
-        Two character reference to the detectors to use, specify None for no
-        contraint and comma separate for multiple references.
-    nsteps: list (2,), optional
-        Number of burn-in and production steps to take, [nburn, nprod]. See
-        `pyfstat.MCMCSearch.setup_initialisation()` for details on adding
-        initialisation steps.
-    nwalkers, ntemps: int, optional
-        The number of walkers and temperates to use in the parallel
-        tempered PTSampler.
-    log10beta_min float < 0, optional
-        The  log_10(beta) value, if given the set of betas passed to PTSampler
-        are generated from `np.logspace(0, log10beta_min, ntemps)` (given
-        in descending order to ptemcee).
-    theta_initial: dict, array, optional
-        A dictionary of distribution about which to distribute the
-        initial walkers about
-    rhohatmax: float, optional
-        Upper bound for the SNR scale parameter (required to normalise the
-        Bayes factor) - this needs to be carefully set when using the
-        evidence.
-    binary: bool, optional
-        If true, search over binary parameters
-    BSGL: bool, optional
-        If true, use the BSGL statistic
-    SSBPrec: int, optional
-        SSBPrec (SSB precision) to use when calling ComputeFstat
-    RngMedWindow: int, optional
-        Running-Median window size (number of bins) for ComputeFstat
-    minCoverFreq, maxCoverFreq: float, optional
-        Minimum and maximum instantaneous frequency which will be covered
-        over the SFT time span as passed to CreateFstatInput
-    injectSources: dict, optional
-        If given, inject these properties into the SFT files before running
-        the search
-    assumeSqrtSX: float or list or str
-        Don't estimate noise-floors, but assume (stationary) per-IFO sqrt{SX}.
-        See `core.ComputeFstat`.
-    transientWindowType: str
-        If 'rect' or 'exp',
-        compute atoms so that a transient (t0,tau) map can later be computed.
-        ('none' instead of None explicitly calls the transient-window function,
-        but with the full range, for debugging)
-        Currently only supported for nsegs=1.
-    tCWFstatMapVersion: str
-        Choose between standard 'lal' implementation,
-        'pycuda' for gpu, and some others for devel/debug.
-
-    Attributes
-    ----------
-    symbol_dictionary: dict
-        Key, val pairs of the parameters (i.e. `F0`, `F1`), to Latex math
-        symbols for plots
-    unit_dictionary: dict
-        Key, val pairs of the parameters (i.e. `F0`, `F1`), and the
-        units (i.e. `Hz`)
-    transform_dictionary: dict
-        Key, val pairs of the parameters (i.e. `F0`, `F1`), where the key is
-        itself a dictionary which can item `multiplier`, `subtractor`, or
-        `unit` by which to transform by and update the units.
+class MCMCSearch(BaseSearchClass):
+    """
+    MCMC search using ComputeFstat.
 
+    Evaluates the coherent F-statistic across a parameter space region
+    corresponding to an isolated/binary-modulated CW signal.
     """
 
     symbol_dictionary = dict(
         F0=r"$f$",
         F1=r"$\dot{f}$",
         F2=r"$\ddot{f}$",
         Alpha=r"$\alpha$",
         Delta=r"$\delta$",
         asini=r"asini",
         period=r"P",
         ecc=r"ecc",
         tp=r"tp",
         argp=r"argp",
     )
+    """
+        Key, val pairs of the parameters (`F0`, `F1`, ...), to LaTeX math
+        symbols for plots
+    """
     unit_dictionary = dict(
         F0=r"Hz",
         F1=r"Hz/s",
         F2=r"Hz/s$^2$",
         Alpha=r"rad",
         Delta=r"rad",
         asini="",
         period=r"s",
         ecc="",
-        tp="",
+        tp=r"s",
         argp="",
     )
+    """
+        Key, val pairs of the parameters (i.e. `F0`, `F1`), and the
+        units (i.e. `Hz`)
+    """
     transform_dictionary = {}
+    """
+        Key, val pairs of the parameters (i.e. `F0`, `F1`), where the key is
+        itself a dictionary which can item `multiplier`, `subtractor`, or
+        `unit` by which to transform by and update the units.
+    """
 
     def __init__(
         self,
         theta_prior,
         tref,
         label,
         outdir="data",
@@ -144,26 +127,103 @@
         nwalkers=100,
         ntemps=1,
         log10beta_min=-5,
         theta_initial=None,
         rhohatmax=1000,
         binary=False,
         BSGL=False,
+        BtSG=False,
         SSBprec=None,
         RngMedWindow=None,
         minCoverFreq=None,
         maxCoverFreq=None,
         injectSources=None,
         assumeSqrtSX=None,
         transientWindowType=None,
         tCWFstatMapVersion="lal",
         earth_ephem=None,
         sun_ephem=None,
+        allowedMismatchFromSFTLength=None,
+        clean=False,
     ):
-
+        """
+        Parameters
+        ----------
+        theta_prior: dict
+            Dictionary of priors and fixed values for the search parameters.
+            For each parameters (key of the dict), if it is to be held fixed
+            the value should be the constant float, if it is be searched, the
+            value should be a dictionary of the prior.
+        tref, minStartTime, maxStartTime: int
+            GPS seconds of the reference time, start time and end time. While tref
+            is requirede, minStartTime and maxStartTime default to None in which
+            case all available data is used.
+        label, outdir: str
+            A label and output directory (optional, default is `data`) to
+            name files
+        sftfilepattern: str, optional
+            Pattern to match SFTs using wildcards (`*?`) and ranges [0-9];
+            mutiple patterns can be given separated by colons.
+        detectors: str, optional
+            Two character reference to the detectors to use, specify None for no
+            contraint and comma separated strings for multiple references.
+        nsteps: list (2,), optional
+            Number of burn-in and production steps to take, [nburn, nprod]. See
+            `pyfstat.MCMCSearch.setup_initialisation()` for details on adding
+            initialisation steps.
+        nwalkers, ntemps: int, optional
+            The number of walkers and temperates to use in the parallel
+            tempered PTSampler.
+        log10beta_min: float < 0, optional
+            The log_10(beta) value. If given, the set of betas passed to PTSampler
+            are generated from `np.logspace(0, log10beta_min, ntemps)` (given
+            in descending order to ptemcee).
+        theta_initial: dict, array, optional
+            A dictionary of distribution about which to distribute the
+            initial walkers about.
+        rhohatmax: float, optional
+            Upper bound for the SNR scale parameter (required to normalise the
+            Bayes factor) - this needs to be carefully set when using the
+            evidence.
+        binary: bool, optional
+            If true, search over binary orbital parameters.
+        BSGL: bool, optional
+            If true, use the BSGL statistic.
+        BtSG: bool, optional
+            If true, use the transient lnBtSG statistic.
+            (Only for transient searches.)
+        SSBPrec: int, optional
+            SSBPrec (SSB precision) to use when calling ComputeFstat. See `core.ComputeFstat`.
+        RngMedWindow: int, optional
+            Running-Median window size (number of bins) for ComputeFstat. See `core.ComputeFstat`.
+        minCoverFreq, maxCoverFreq: float, optional
+            Minimum and maximum instantaneous frequency which will be covered
+            over the SFT time span as passed to CreateFstatInput. See `core.ComputeFstat`.
+        injectSources: dict, optional
+            If given, inject these properties into the SFT files before running
+            the search. See `core.ComputeFstat`.
+        assumeSqrtSX: float or list or str
+            Don't estimate noise-floors, but assume (stationary) per-IFO sqrt{SX}.
+            See `core.ComputeFstat`.
+        transientWindowType: str
+            If 'rect' or 'exp',
+            compute atoms so that a transient (t0,tau) map can later be computed.
+            ('none' instead of None explicitly calls the transient-window function,
+            but with the full range, for debugging). See `core.ComputeFstat`.
+            Currently only supported for nsegs=1.
+        tCWFstatMapVersion: str
+            Choose between standard 'lal' implementation,
+            'pycuda' for gpu, and some others for devel/debug.
+        allowedMismatchFromSFTLength: float
+            Maximum allowed mismatch from SFTs being too long
+            [Default: what's hardcoded in XLALFstatMaximumSFTLength].
+        clean: bool
+            If true, ignore existing data and overwrite.
+            Otherwise, re-use existing data if no inconsistencies are found.
+        """
         self._set_init_params_dict(locals())
         self.theta_prior = theta_prior
         self.tref = tref
         self.label = label
         self.outdir = outdir
         self.minStartTime = minStartTime
         self.maxStartTime = maxStartTime
@@ -173,66 +233,93 @@
         self.nwalkers = nwalkers
         self.ntemps = ntemps
         self.log10beta_min = log10beta_min
         self.theta_initial = theta_initial
         self.rhohatmax = rhohatmax
         self.binary = binary
         self.BSGL = BSGL
+        self.BtSG = BtSG
         self.SSBprec = SSBprec
         self.RngMedWindow = RngMedWindow
         self.minCoverFreq = minCoverFreq
         self.maxCoverFreq = maxCoverFreq
         self.injectSources = injectSources
         self.assumeSqrtSX = assumeSqrtSX
         self.transientWindowType = transientWindowType
         self.tCWFstatMapVersion = tCWFstatMapVersion
         self.set_ephemeris_files(earth_ephem, sun_ephem)
+        self.allowedMismatchFromSFTLength = allowedMismatchFromSFTLength
+        self.clean = clean
 
-        if os.path.isdir(outdir) is False:
-            os.mkdir(outdir)
+        os.makedirs(outdir, exist_ok=True)
         self.output_file_header = self.get_output_file_header()
-        self._add_log_file(self.output_file_header)
-        logging.info("Set-up MCMC search for model {}".format(self.label))
+        logger.info("Set-up MCMC search for model {}".format(self.label))
         if sftfilepattern:
-            logging.info("Using data {}".format(self.sftfilepattern))
+            logger.info("Using data {}".format(self.sftfilepattern))
         else:
-            logging.info("No sftfilepattern given")
+            logger.info("No sftfilepattern given")
         if injectSources:
-            logging.info("Inject sources: {}".format(injectSources))
+            logger.info("Inject sources: {}".format(injectSources))
         self.pickle_path = os.path.join(self.outdir, self.label + "_saved_data.p")
         self._unpack_input_theta()
         self.ndim = len(self.theta_keys)
         if self.log10beta_min:
             self.betas = np.logspace(0, self.log10beta_min, self.ntemps)
         else:
             self.betas = None
 
-        if args.clean and os.path.isfile(self.pickle_path):
+        if self.clean and os.path.isfile(self.pickle_path):
             os.rename(self.pickle_path, self.pickle_path + ".old")
 
         self._set_likelihoodcoef()
         self._log_input()
 
     def _set_likelihoodcoef(self):
-        self.likelihoodcoef = np.log(70.0 / self.rhohatmax ** 4)
+        """Additional constant terms to turn a detection statistic into a likelihood.
+
+        In general, the (log-)likelihood can be obtained from the signal-to-noise
+        (log-)Bayes factor
+        (omitting the overall Gaussian-noise normalization term)
+        but the detection statistic may only be a monotonic function of the
+        Bayes factor, not the full thing.
+        E.g. this is the case for the standard CW F-statistic!
+        """
+        if self.BSGL:
+            # In this case, the corresponding term is already included
+            # in the detection statistic itself.
+            # See Eq. (36) in Keitel et al (PRD 89, 064023, 2014):
+            # https://arxiv.org/abs/1311.5738
+            # where Fstar0 = ln(cstar) = ln(rhohatmax**4/70).
+            # We just need to switch to natural log basis.
+            self.likelihooddetstatmultiplier = np.log(10)
+            self.likelihoodcoef = 0
+        else:
+            # If assuming only Gaussian noise + signal,
+            # the likelihood is essentially the F-statistic,
+            # but with an extra constant term depending on the amplitude prior.
+            # See Eq. (9) of Ashton & Prix (PRD 97, 103020, 2018):
+            # https://arxiv.org/abs/1802.05450
+            # Also need to go from twoF to F.
+            self.likelihooddetstatmultiplier = 0.5
+            self.likelihoodcoef = np.log(70.0 / self.rhohatmax**4)
 
     def _log_input(self):
-        logging.info("theta_prior = {}".format(self.theta_prior))
-        logging.info("nwalkers={}".format(self.nwalkers))
-        logging.info("nsteps = {}".format(self.nsteps))
-        logging.info("ntemps = {}".format(self.ntemps))
-        logging.info("log10beta_min = {}".format(self.log10beta_min))
+        logger.info("theta_prior = {}".format(self.theta_prior))
+        logger.info("nwalkers={}".format(self.nwalkers))
+        logger.info("nsteps = {}".format(self.nsteps))
+        logger.info("ntemps = {}".format(self.ntemps))
+        logger.info("log10beta_min = {}".format(self.log10beta_min))
 
     def _get_search_ranges(self):
-        """ take prior widths as proxy "search ranges" to allow covering band estimate """
+        """take prior widths as proxy "search ranges" to allow covering band estimate"""
         if (self.minCoverFreq is None) or (self.maxCoverFreq is None):
             normal_stds = 3  # this might not always be enough
             prior_bounds, norm_trunc_warn = self._get_prior_bounds(normal_stds)
             if norm_trunc_warn:
-                logging.warning(
+                logger.warning(
                     "Gaussian priors (normal / half-normal) have been truncated"
                     " at {:f} standard deviations for estimating the coverage"
                     " frequency band. If sampling fails at any point, please"
                     " consider manually setting [minCoverFreq,maxCoverFreq] to"
                     " more generous values.".format(normal_stds)
                 )
             # first start with parameters that have non-delta prior ranges
@@ -245,15 +332,15 @@
                 if key not in self.theta_keys:
                     search_ranges[key] = [self.theta_prior[key]]
             return search_ranges
         else:
             return None
 
     def _initiate_search_object(self):
-        logging.info("Setting up search object")
+        logger.info("Setting up search object")
         search_ranges = self._get_search_ranges()
         self.search = core.ComputeFstat(
             tref=self.tref,
             sftfilepattern=self.sftfilepattern,
             minCoverFreq=self.minCoverFreq,
             maxCoverFreq=self.maxCoverFreq,
             search_ranges=search_ranges,
@@ -266,50 +353,55 @@
             injectSources=self.injectSources,
             assumeSqrtSX=self.assumeSqrtSX,
             SSBprec=self.SSBprec,
             RngMedWindow=self.RngMedWindow,
             tCWFstatMapVersion=self.tCWFstatMapVersion,
             earth_ephem=self.earth_ephem,
             sun_ephem=self.sun_ephem,
+            allowedMismatchFromSFTLength=self.allowedMismatchFromSFTLength,
         )
         if self.minStartTime is None:
             self.minStartTime = self.search.minStartTime
         if self.maxStartTime is None:
             self.maxStartTime = self.search.maxStartTime
 
-    def logp(self, theta_vals, theta_prior, theta_keys, search):
+    def _logp(self, theta_vals, theta_prior, theta_keys, search):
         H = [
             self._generic_lnprior(**theta_prior[key])(p)
             for p, key in zip(theta_vals, theta_keys)
         ]
         return np.sum(H)
 
-    def logl(self, theta, search):
+    def _set_point_for_evaluation(self, theta):
+        """Combines fixed and variable parameters to form a valid evaluation point.
+
+        Parameters
+        ----------
+        theta: list or np.ndarray
+            The sampled (variable) parameters.
+        Returns
+        -------
+        p: list
+            The full parameter space point as a list.
+        """
+        p = copy.copy(self.fixed_theta)
         for j, theta_i in enumerate(self.theta_idxs):
-            self.fixed_theta[theta_i] = theta[j]
-        twoF = search.get_fullycoherent_twoF(
-            self.minStartTime, self.maxStartTime, *self.fixed_theta
-        )
-        return twoF / 2.0 + self.likelihoodcoef
+            p[theta_i] = theta[j]
+        return p
 
-    def _unpack_input_theta(self):
-        full_theta_keys = ["F0", "F1", "F2", "Alpha", "Delta"]
-        if self.binary:
-            full_theta_keys += ["asini", "period", "ecc", "tp", "argp"]
-        full_theta_keys_copy = copy.copy(full_theta_keys)
+    def _logl(self, theta, search):
+        in_theta = self._set_point_for_evaluation(theta)
+        detstat = search.get_det_stat(*in_theta)
+        return detstat * self.likelihooddetstatmultiplier + self.likelihoodcoef
 
-        full_theta_symbols = [
-            r"$f$",
-            r"$\dot{f}$",
-            r"$\ddot{f}$",
-            r"$\alpha$",
-            r"$\delta$",
-        ]
+    def _unpack_input_theta(self):
+        self.full_theta_keys = ["F0", "F1", "F2", "Alpha", "Delta"]
         if self.binary:
-            full_theta_symbols += ["asini", "period", "ecc", "tp", "argp"]
+            self.full_theta_keys += ["asini", "period", "ecc", "tp", "argp"]
+        full_theta_keys_copy = copy.copy(self.full_theta_keys)
 
         self.theta_keys = []
         fixed_theta_dict = {}
         for key, val in self.theta_prior.items():
             if type(val) is dict:
                 fixed_theta_dict[key] = 0
                 self.theta_keys.append(key)
@@ -324,62 +416,67 @@
         if len(full_theta_keys_copy) > 0:
             raise ValueError(
                 ("Input dictionary `theta` is missing the" "following keys: {}").format(
                     full_theta_keys_copy
                 )
             )
 
-        self.fixed_theta = [fixed_theta_dict[key] for key in full_theta_keys]
-        self.theta_idxs = [full_theta_keys.index(k) for k in self.theta_keys]
-        self.theta_symbols = [full_theta_symbols[i] for i in self.theta_idxs]
+        self.fixed_theta = [fixed_theta_dict[key] for key in self.full_theta_keys]
+        self.theta_idxs = [self.full_theta_keys.index(k) for k in self.theta_keys]
+        self.theta_symbols = [self.symbol_dictionary[k] for k in self.theta_keys]
 
         idxs = np.argsort(self.theta_idxs)
         self.theta_idxs = [self.theta_idxs[i] for i in idxs]
         self.theta_symbols = [self.theta_symbols[i] for i in idxs]
         self.theta_keys = [self.theta_keys[i] for i in idxs]
 
+        self.output_keys = self.theta_keys.copy()
+        self.output_keys.append("twoF")
+        if self.BSGL:
+            self.output_keys.append("log10BSGL")
+
     def _evaluate_logpost(self, p0vec):
         init_logp = np.array(
             [
-                self.logp(p, self.theta_prior, self.theta_keys, self.search)
+                self._logp(p, self.theta_prior, self.theta_keys, self.search)
                 for p in p0vec
             ]
         )
-        init_logl = np.array([self.logl(p, self.search) for p in p0vec])
+        init_logl = np.array([self._logl(p, self.search) for p in p0vec])
         return init_logl + init_logp
 
     def _check_initial_points(self, p0):
         for nt in range(self.ntemps):
-            logging.info("Checking temperature {} chains".format(nt))
+            logger.info("Checking temperature {} chains".format(nt))
             num = sum(self._evaluate_logpost(p0[nt]) == -np.inf)
             if num > 0:
-                logging.warning(
+                logger.warning(
                     "Of {} initial values, {} are -np.inf due to the prior".format(
                         len(p0[0]), num
                     )
                 )
                 p0 = self._generate_new_p0_to_fix_initial_points(p0, nt)
 
     def _generate_new_p0_to_fix_initial_points(self, p0, nt):
-        logging.info("Attempting to correct intial values")
+        logger.info("Attempting to correct intial values")
         init_logpost = self._evaluate_logpost(p0[nt])
         idxs = np.arange(self.nwalkers)[init_logpost == -np.inf]
         count = 0
         while sum(init_logpost == -np.inf) > 0 and count < 100:
             for j in idxs:
                 p0[nt][j] = p0[nt][np.random.randint(0, self.nwalkers)] * (
                     1 + np.random.normal(0, 1e-10, self.ndim)
                 )
             init_logpost = self._evaluate_logpost(p0[nt])
             count += 1
 
         if sum(init_logpost == -np.inf) > 0:
-            logging.info("Failed to fix initial priors")
+            logger.info("Failed to fix initial priors")
         else:
-            logging.info("Suceeded to fix initial priors")
+            logger.info("Suceeded to fix initial priors")
 
         return p0
 
     def setup_initialisation(self, nburn0, scatter_val=1e-10):
         """Add an initialisation step to the MCMC run
 
         If called prior to `run()`, adds an intial step in which the MCMC
@@ -387,158 +484,163 @@
         continues in the usual manner (i.e. for nburn and nprod steps), but the
         walkers are reset scattered around the maximum likelihood position
         of the initialisation step.
 
         Parameters
         ----------
         nburn0: int
-            Number of initialisation steps to take
+            Number of initialisation steps to take.
         scatter_val: float
             Relative number to scatter walkers around the maximum likelihood
-            position after the initialisation step
-
+            position after the initialisation step. If the maximum likelihood
+            point is located at `p`, the new walkers are randomly drawn from a
+            multivariate gaussian distribution centered at `p` with standard
+            deviation `diag(scatter_val * p)`.
         """
 
-        logging.info(
+        logger.info(
             "Setting up initialisation with nburn0={}, scatter_val={}".format(
                 nburn0, scatter_val
             )
         )
         self.nsteps = [nburn0] + self.nsteps
         self.scatter_val = scatter_val
 
-    #    def setup_burnin_convergence_testing(
-    #            self, n=10, test_type='autocorr', windowed=False, **kwargs):
-    #        """ Set up convergence testing during the MCMC simulation
-    #
-    #        Parameters
-    #        ----------
-    #        n: int
-    #            Number of steps after which to test convergence
-    #        test_type: str ['autocorr', 'GR']
-    #            If 'autocorr' use the exponential autocorrelation time (kwargs
-    #            passed to `get_autocorr_convergence`). If 'GR' use the Gelman-Rubin
-    #            statistic (kwargs passed to `get_GR_convergence`)
-    #        windowed: bool
-    #            If True, only calculate the convergence test in a window of length
-    #            `n`
-    #        **kwargs:
-    #            Passed to either `_test_autocorr_convergence()` or
-    #            `_test_GR_convergence()` depending on `test_type`.
-    #
-    #        """
-    #        logging.info('Setting up convergence testing')
-    #        self.convergence_n = n
-    #        self.convergence_windowed = windowed
-    #        self.convergence_test_type = test_type
-    #        self.convergence_kwargs = kwargs
-    #        self.convergence_diagnostic = []
-    #        self.convergence_diagnosticx = []
-    #        if test_type in ['autocorr']:
-    #            self._get_convergence_test = self._test_autocorr_convergence
-    #        elif test_type in ['GR']:
-    #            self._get_convergence_test = self._test_GR_convergence
-    #        else:
-    #            raise ValueError('test_type {} not understood'.format(test_type))
-    #
-    #
-    #    def _test_autocorr_convergence(self, i, test=True, n_cut=5):
-    #        try:
-    #            acors = np.zeros((self.ntemps, self.ndim))
-    #            for temp in range(self.ntemps):
-    #                if self.convergence_windowed:
-    #                    j = i-self.convergence_n
-    #                else:
-    #                    j = 0
-    #                x = np.mean(self.sampler.chain[temp, :, j:i, :], axis=0)
-    #                acors[temp, :] = emcee.autocorr.exponential_time(x)
-    #            c = np.max(acors, axis=0)
-    #        except emcee.autocorr.AutocorrError:
-    #            logging.info('Failed to calculate exponential autocorrelation')
-    #            c = np.zeros(self.ndim) + np.nan
-    #        except AttributeError:
-    #            logging.info('Unable to calculate exponential autocorrelation')
-    #            c = np.zeros(self.ndim) + np.nan
-    #
-    #        self.convergence_diagnosticx.append(i - self.convergence_n/2.)
-    #        self.convergence_diagnostic.append(list(c))
-    #
-    #        if test:
-    #            return i > n_cut * np.max(c)
-    #
-    #    def _test_GR_convergence(self, i, test=True, R=1.1):
-    #        if self.convergence_windowed:
-    #            s = self.sampler.chain[0, :, i-self.convergence_n+1:i+1, :]
-    #        else:
-    #            s = self.sampler.chain[0, :, :i+1, :]
-    #        N = float(self.convergence_n)
-    #        M = float(self.nwalkers)
-    #        W = np.mean(np.var(s, axis=1), axis=0)
-    #        per_walker_mean = np.mean(s, axis=1)
-    #        mean = np.mean(per_walker_mean, axis=0)
-    #        B = N / (M-1.) * np.sum((per_walker_mean-mean)**2, axis=0)
-    #        Vhat = (N-1)/N * W + (M+1)/(M*N) * B
-    #        c = np.sqrt(Vhat/W)
-    #        self.convergence_diagnostic.append(c)
-    #        self.convergence_diagnosticx.append(i - self.convergence_n/2.)
-    #
-    #        if test and np.max(c) < R:
-    #            return True
-    #        else:
-    #            return False
-    #
-    #    def _test_convergence(self, i, **kwargs):
-    #        if np.mod(i+1, self.convergence_n) == 0:
-    #            return self._get_convergence_test(i, self.sampler, **kwargs)
-    #        else:
-    #            return False
-    #
-    #    def _run_sampler_with_conv_test(self, p0, nprod=0, nburn=0):
-    #        logging.info('Running {} burn-in steps with convergence testing'
-    #                     .format(nburn))
-    #        iterator = tqdm(self.sampler.sample(p0, iterations=nburn), total=nburn)
-    #        for i, output in enumerate(iterator):
-    #            if self._test_convergence(i, self.sampler, test=True,
-    #                                      **self.convergence_kwargs):
-    #                logging.info(
-    #                    'Converged at {} before max number {} of steps reached'
-    #                    .format(i, nburn))
-    #                self.convergence_idx = i
-    #                break
-    #        iterator.close()
-    #        logging.info('Running {} production steps'.format(nprod))
-    #        j = nburn
-    #        iterator = tqdm(self.sampler.sample(output[0], iterations=nprod),
-    #                        total=nprod)
-    #        for result in iterator:
-    #            self._test_convergence(j, self.sampler, test=False,
-    #                                   **self.convergence_kwargs)
-    #            j += 1
-
     def _run_sampler(self, p0, nprod=0, nburn=0, window=50):
         for result in tqdm(
             self.sampler.sample(p0, iterations=nburn + nprod), total=nburn + nprod
         ):
             pass
 
         self.mean_acceptance_fraction = np.mean(
             self.sampler.acceptance_fraction, axis=1
         )
-        logging.info(
+        logger.info(
             "Mean acceptance fraction: {}".format(self.mean_acceptance_fraction)
         )
         if self.ntemps > 1:
             self.tswap_acceptance_fraction = self.sampler.tswap_acceptance_fraction
-            logging.info(
+            logger.info(
                 "Tswap acceptance fraction: {}".format(
                     self.sampler.tswap_acceptance_fraction
                 )
             )
-        self.autocorr_time = self.sampler.get_autocorr_time(window=window)
-        logging.info("Autocorrelation length: {}".format(self.autocorr_time))
+        self.autocorr_time = self._get_autocorr_time(
+            sampler=self.sampler, window=window
+        )
+        logger.info("Autocorrelation length: {}".format(self.autocorr_time))
+
+    def _get_autocorr_time(self, sampler, window=50):
+        """
+        Returns a matrix of autocorrelation lengths for each
+        parameter in each temperature of shape ``(Ntemps, Ndim)``.
+
+        This is copied from sampler.py of ptemcee-1.0.0
+        [(c) Daniel Foreman-Mackey & contributors],
+        to allow us to call the locally fixed _autocorr_function().
+
+        :param window: (optional)
+            The size of the windowing function. This is equivalent to the
+            maximum number of lags to use. (default: 50)
+
+        """
+        acors = np.zeros((sampler.ntemps, sampler.dim))
+
+        for i in range(sampler.ntemps):
+            x = np.mean(sampler._chain[i, :, :, :], axis=0)
+            acors[i, :] = self._autocorr_integrated_time(x=x, window=window)
+        return acors
+
+    def _autocorr_integrated_time(self, x, axis=0, window=50, fast=False):
+        """
+        Estimate the integrated autocorrelation time of a time series.
+
+        See `Sokal's notes <http://www.stat.unc.edu/faculty/cji/Sokal.pdf>`_ on
+        MCMC and sample estimators for autocorrelation times.
+
+        This version of this function is copied from util.py of ptemcee-1.0.0
+        [(c) Daniel Foreman-Mackey & contributors],
+        and fixed up to be compatible with numpy>=1.23.0.
+
+        :param x:
+            The time series. If multidimensional, set the time axis using the
+            ``axis`` keyword argument and the function will be computed for every
+            other axis.
+
+        :param axis: (optional)
+            The time axis of ``x``. Assumed to be the first axis if not specified.
+
+        :param window: (optional)
+            The size of the window to use. (default: 50)
+
+        :param fast: (optional)
+            If ``True``, only use the largest ``2^n`` entries for efficiency.
+            (default: False)
+
+        """
+        # Compute the autocorrelation function.
+        f = self._autocorr_function(x, axis=axis, fast=fast)
+
+        # Special case 1D for simplicity.
+        if len(f.shape) == 1:
+            return 1 + 2 * np.sum(f[1:window])
+
+        # N-dimensional case.
+        m = [
+            slice(None),
+        ] * len(f.shape)
+        m[axis] = slice(1, window)
+        m = tuple(m)  # fix for numpy>=1.23.0
+        tau = 1 + 2 * np.sum(f[m], axis=axis)
+
+        return tau
+
+    def _autocorr_function(self, x, axis=0, fast=False):
+        """
+        Estimate the autocorrelation function of a time series using the FFT.
+
+        This version of this function is copied from util.py of ptemcee-1.0.0
+        [(c) Daniel Foreman-Mackey & contributors],
+        and fixed up to be compatible with numpy>=1.23.0.
+
+        :param x:
+            The time series. If multidimensional, set the time axis using the
+            ``axis`` keyword argument and the function will be computed for every
+            other axis.
+
+        :param axis: (optional)
+            The time axis of ``x``. Assumed to be the first axis if not specified.
+
+        :param fast: (optional)
+            If ``True``, only use the largest ``2^n`` entries for efficiency.
+            (default: False)
+
+        """
+        x = np.atleast_1d(x)
+        m = [
+            slice(None),
+        ] * len(x.shape)
+
+        # For computational efficiency, crop the chain to the largest power of
+        # two if requested.
+        if fast:
+            n = int(2 ** np.floor(np.log2(x.shape[axis])))
+            m[axis] = slice(0, n)
+            x = x
+        else:
+            n = x.shape[axis]
+
+        # Compute the FFT and then (from that) the auto-correlation function.
+        f = np.fft.fft(x - np.mean(x, axis=axis), n=2 * n, axis=axis)
+        m[axis] = slice(0, n)
+        m_tuple = tuple(m)  # fix for numpy>=1.23.0
+        acf = np.fft.ifft(f * np.conjugate(f), axis=axis)[m_tuple].real
+        m[axis] = 0
+        m_tuple = tuple(m)  # fix for numpy>=1.23.0
+        return acf / acf[m_tuple]
 
     def _estimate_run_time(self):
         """Print the estimated run time
 
         Uses timing coefficients based on a Lenovo T460p Intel(R)
         Core(TM) i5-6300HQ CPU @ 2.30GHz.
 
@@ -572,15 +674,15 @@
             time = np.sum(ts)
         else:
             numb_evals = np.sum(self.nsteps) * self.nwalkers * self.ntemps
             time = (tau0S + tau0LD * Nsfts) * numb_evals
             if getattr(self, "nsegs", 1) > 1:
                 time += (tau0C + tau0T * Nsfts) * self.nsegs * numb_evals
 
-        logging.info(
+        logger.info(
             "Estimated run-time = {} s = {:1.0f}:{:1.0f} m".format(
                 time, *divmod(time, 60)
             )
         )
 
     def run(
         self,
@@ -593,89 +695,96 @@
         window=50,
     ):
         """Run the MCMC simulatation
 
         Parameters
         ----------
         proposal_scale_factor: float
-            The proposal scale factor used by the sampler, see Goodman & Weare
-            (2010). If the acceptance fraction is too low, you can raise it by
-            decreasing the a parameter; and if it is too high, you can reduce
-            it by increasing the a parameter [Foreman-Mackay (2013)].
+            The proposal scale factor `a > 1` used by the sampler.
+            See Goodman & Weare (Comm App Math Comp Sci, Vol 5, No. 1, 2010): 10.2140/camcos.2010.5.65.
+            The bigger the value, the wider the range to draw proposals from.
+            If the acceptance fraction is too low, you can raise it by
+            decreasing the `a` parameter; and if it is too high, you can reduce
+            it by increasing the `a` parameter.
+            See Foreman-Mackay et al. (PASP 125 306, 2013): https://arxiv.org/abs/1202.3665.
         save_pickle: bool
             If true, save a pickle file of the full sampler state.
         export_samples: bool
-            If true, save ASCII samples file to disk.
+            If true, save ASCII samples file to disk. See `MCMCSearch.export_samples_to_disk`.
         save_loudest: bool
-            If true, save a CFSv2 .loudest file to disk.
+            If true, save a CFSv2 .loudest file to disk. See `MCMCSearch.generate_loudest`.
         plot_walkers: bool
             If true, save trace plots of the walkers.
         walker_plot_args:
             Dictionary passed as kwargs to _plot_walkers to control the plotting.
-            Also, if both "fig" and "axes" entries are set,
-            the plot is not saved to disk directly,
-            but .walker_fig and .walker_axes properties are returned.
+            Histogram of sampled detection statistic values can be retrieved setting "plot_det_stat" to `True`.
+            Parameters corresponding to an injected signal can be passed through "injection_parameters"
+            as a dictionary containing the parameters of said signal. All parameters being searched for must
+            be present, otherwise this option is ignored.
+            If both "fig" and "axes" entries are set, the plot is not saved to disk
+            directly, but (fig, axes) are returned.
         window: int
             The minimum number of autocorrelation times needed to trust the
             result when estimating the autocorrelation time (see
             ptemcee.Sampler.get_autocorr_time for further details.
 
         """
 
+        self._initiate_search_object()
+
         self.old_data_is_okay_to_use = self._check_old_data_is_okay_to_use()
         if self.old_data_is_okay_to_use is True:
-            logging.warning("Using saved data from {}".format(self.pickle_path))
+            logger.warning("Using saved data from {}".format(self.pickle_path))
             d = self.get_saved_data_dictionary()
             self.samples = d["samples"]
             self.lnprobs = d["lnprobs"]
             self.lnlikes = d["lnlikes"]
             self.all_lnlikelihood = d["all_lnlikelihood"]
             self.chain = d["chain"]
             return
 
-        self._initiate_search_object()
         self._estimate_run_time()
 
         walker_plot_args = walker_plot_args or {}
 
         self.sampler = PTSampler(
             ntemps=self.ntemps,
             nwalkers=self.nwalkers,
             dim=self.ndim,
-            logl=self.logl,
-            logp=self.logp,
+            logl=self._logl,
+            logp=self._logp,
             logpargs=(self.theta_prior, self.theta_keys, self.search),
             loglargs=(self.search,),
             betas=self.betas,
             a=proposal_scale_factor,
         )
 
         p0 = self._generate_initial_p0()
         p0 = self._apply_corrections_to_p0(p0)
         self._check_initial_points(p0)
 
         # Run initialisation steps if required
         ninit_steps = len(self.nsteps) - 2
         for j, n in enumerate(self.nsteps[:-2]):
-            logging.info(
+            logger.info(
                 "Running {}/{} initialisation with {} steps".format(j, ninit_steps, n)
             )
             self._run_sampler(p0, nburn=n, window=window)
             if plot_walkers:
                 try:
                     walker_fig, walker_axes = self._plot_walkers(**walker_plot_args)
                     walker_fig.tight_layout()
                     walker_fig.savefig(
                         os.path.join(
                             self.outdir, "{}_init_{}_walkers.png".format(self.label, j)
                         )
                     )
                     plt.close(walker_fig)
                 except Exception as e:
-                    logging.warning(
+                    logger.warning(
                         "Failed to plot initialisation walkers due to Error {}".format(
                             e
                         )
                     )
 
             p0 = self._get_new_p0()
             p0 = self._apply_corrections_to_p0(p0)
@@ -683,15 +792,15 @@
             self.sampler.reset()
 
         if len(self.nsteps) > 1:
             nburn = self.nsteps[-2]
         else:
             nburn = 0
         nprod = self.nsteps[-1]
-        logging.info("Running final burn and prod with {} steps".format(nburn + nprod))
+        logger.info("Running final burn and prod with {} steps".format(nburn + nprod))
         self._run_sampler(p0, nburn=nburn, nprod=nprod)
 
         samples = self.sampler.chain[0, :, nburn:, :].reshape((-1, self.ndim))
         lnprobs = self.sampler.logprobability[0, :, nburn:].reshape((-1))
         lnlikes = self.sampler.loglikelihood[0, :, nburn:].reshape((-1))
         all_lnlikelihood = self.sampler.loglikelihood[:, :, nburn:]
         self.samples = samples
@@ -709,28 +818,28 @@
         if plot_walkers:
             try:
                 walkers_fig, walkers_axes = self._plot_walkers(
                     nprod=nprod, **walker_plot_args
                 )
                 walkers_fig.tight_layout()
             except Exception as e:
-                logging.warning("Failed to plot walkers due to Error {}".format(e))
+                logger.warning("Failed to plot walkers due to Error {}".format(e))
             if (walker_plot_args.get("fig") is not None) and (
                 walker_plot_args.get("axes") is not None
             ):
                 self.walker_fig = walkers_fig
                 self.walker_axes = walkers_axes
             else:
                 try:
                     walkers_fig.savefig(
                         os.path.join(self.outdir, self.label + "_walkers.png")
                     )
                     plt.close(walkers_fig)
                 except Exception as e:
-                    logging.warning(
+                    logger.warning(
                         "Failed to save walker plots due to Error {}".format(e)
                     )
 
     def _get_rescale_multiplier_for_key(self, key):
         """Get the rescale multiplier from the transform_dictionary
 
         Can either be a float, a string (in which case it is interpretted as
@@ -777,54 +886,55 @@
             else:
                 subtractor = val
         else:
             subtractor = 0
         return subtractor
 
     def _scale_samples(self, samples, theta_keys):
-        """ Scale the samples using the transform_dictionary """
+        """Scale the samples using the transform_dictionary"""
         for key in theta_keys:
             if key in self.transform_dictionary:
                 idx = theta_keys.index(key)
                 s = samples[:, idx]
                 subtractor = self._get_rescale_subtractor_for_key(key)
                 s = s - subtractor
                 multiplier = self._get_rescale_multiplier_for_key(key)
                 s *= multiplier
                 samples[:, idx] = s
 
         return samples
 
     def _get_labels(self, newline_units=False):
-        """ Combine the units, symbols and rescaling to give labels """
+        """Combine the units, symbols and rescaling to give labels"""
 
         labels = []
         for key in self.theta_keys:
-            label = None
-            s = self.symbol_dictionary[key]
-            s.replace("_{glitch}", r"_\mathrm{glitch}")
-            u = self.unit_dictionary[key]
-            if key in self.transform_dictionary:
-                if "symbol" in self.transform_dictionary[key]:
-                    s = self.transform_dictionary[key]["symbol"]
-                if "label" in self.transform_dictionary[key]:
-                    label = self.transform_dictionary[key]["label"]
-                if "unit" in self.transform_dictionary[key]:
-                    u = self.transform_dictionary[key]["unit"]
+            values = self.transform_dictionary.get(key, {})
+            s, label, u = [
+                values.get(slu_key, None) for slu_key in ["symbol", "label", "unit"]
+            ]
+
             if label is None:
-                if newline_units:
-                    label = "{} \n [{}]".format(s, u)
-                else:
-                    label = "{} [{}]".format(s, u)
+                s = s or self.symbol_dictionary[key].replace(
+                    "_{glitch}", r"_\mathrm{glitch}"
+                )
+                u = u or self.unit_dictionary[key]
+                label = (
+                    f"{s}"
+                    + ("\n" if newline_units else " ")
+                    + (f"[{u}]" if u != "" else "")
+                )
+
             labels.append(label)
+
         return labels
 
     def plot_corner(
         self,
-        figsize=(7, 7),
+        figsize=(10, 10),
         add_prior=False,
         nstds=None,
         label_offset=0.4,
         dpi=300,
         rc_context={},
         tglitch_ratio=False,
         fig_and_axes=None,
@@ -840,60 +950,63 @@
         ----------
         figsize: tuple (7, 7)
             Figure size in inches (passed to plt.subplots)
         add_prior: bool, str
             If true, plot the prior as a red line. If 'full' then for uniform
             priors plot the full extent of the prior.
         nstds: float
-            The number of standard deviations to plot centered on the mean
+            The number of standard deviations to plot centered on the median.
+            Standard deviation is computed from the samples using `numpy.std`.
         label_offset: float
-            Offset the labels from the plot: useful to precent overlapping the
-            tick labels with the axis labels
+            Offset the labels from the plot: useful to prevent overlapping the
+            tick labels with the axis labels. This option is passed to `ax.[x|y]axis.set_label_coords`.
         dpi: int
-            Passed to plt.savefig
+            Passed to plt.savefig.
         rc_context: dict
             Dictionary of rc values to set while generating the figure (see
-            matplotlib rc for more details)
+            matplotlib rc for more details).
         tglitch_ratio: bool
             If true, and tglitch is a parameter, plot posteriors as the
             fractional time at which the glitch occurs instead of the actual
-            time
+            time.
         fig_and_axes: tuple
-            fig and axes to plot on, the axes must be of the right shape,
+            (fig, axes) tuple to plot on. The axes must be of the right shape,
             namely (ndim, ndim)
         save_fig: bool
-            If true, save the figure, else return the fig, axes
+            If true, save the figure, else return the fig, axes.
         **kwargs:
-            Passed to corner.corner
+            Passed to corner.corner. Use "truths" to plot the true parameters of a signal.
 
         Returns
         -------
         fig, axes:
-            The matplotlib figure and axes, only returned if save_fig = False
+            The matplotlib figure and axes, only returned if save_fig = False.
 
         """
 
         if "truths" in kwargs:
-
             if not isinstance(kwargs["truths"], dict):
                 raise ValueError("'truths' must be a dictionary.")
 
             missing_keys = set(self.theta_keys) - kwargs["truths"].keys()
             if missing_keys:
-                logging.warning(
+                logger.warning(
                     f"plot_corner(): Missing keys {missing_keys} in 'truths' dictionary,"
                     " argument will be ignored."
                 )
                 kwargs["truths"] = None
             else:
                 kwargs["truths"] = [kwargs["truths"][key] for key in self.theta_keys]
                 kwargs["truths"] = self._scale_samples(
                     np.reshape(kwargs["truths"], (1, -1)), self.theta_keys
                 ).ravel()
 
+                if "truth_color" not in kwargs:
+                    kwargs["truth_color"] = "black"
+
         if self.ndim < 2:
             with plt.rc_context(rc_context):
                 if fig_and_axes is None:
                     fig, ax = plt.subplots(figsize=figsize)
                 else:
                     fig, ax = fig_and_axes
                 ax.hist(self.samples, bins=50, histtype="stepfilled")
@@ -906,15 +1019,15 @@
         with plt.rc_context(rc_context):
             if fig_and_axes is None:
                 fig, axes = plt.subplots(self.ndim, self.ndim, figsize=figsize)
             else:
                 fig, axes = fig_and_axes
 
             samples_plt = copy.copy(self.samples)
-            labels = self._get_labels(newline_units=True)
+            labels = self._get_labels(newline_units=False)
 
             samples_plt = self._scale_samples(samples_plt, self.theta_keys)
 
             if tglitch_ratio:
                 for j, k in enumerate(self.theta_keys):
                     if k == "tglitch":
                         s = samples_plt[:, j]
@@ -942,18 +1055,24 @@
                 samples_plt,
                 labels=labels,
                 fig=fig,
                 bins=50,
                 max_n_ticks=4,
                 plot_contours=True,
                 plot_datapoints=True,
-                # label_kwargs={'fontsize': 12},
+                label_kwargs={"fontsize": 12},
                 data_kwargs={"alpha": 0.1, "ms": 0.5},
                 range=_range,
                 hist_kwargs=hist_kwargs,
+                show_titles=True,
+                fill_contours=True,
+                quantiles=[0.05, 0.5, 0.95]  # [lower, central, upper]
+                if "quantiles" not in kwargs
+                else kwargs.pop("quantiles"),
+                verbose=True if "verbose" not in kwargs else kwargs.pop("verbose"),
                 **kwargs,
             )
 
             axes_list = fig_triangle.get_axes()
             axes = np.array(axes_list).reshape(self.ndim, self.ndim)
             plt.draw()
             for ax in axes[:, 0]:
@@ -961,63 +1080,65 @@
             for ax in axes[-1, :]:
                 ax.xaxis.set_label_coords(0.5, -label_offset)
             for ax in axes_list:
                 ax.set_rasterized(True)
                 ax.set_rasterization_zorder(-10)
 
                 for tick in ax.xaxis.get_major_ticks():
-                    # tick.label.set_fontsize(8)
-                    tick.label.set_rotation("horizontal")
+                    # tick.label1.set_fontsize(8)
+                    tick.label1.set_rotation(30)
                 for tick in ax.yaxis.get_major_ticks():
-                    # tick.label.set_fontsize(8)
-                    tick.label.set_rotation("vertical")
+                    # tick.label1.set_fontsize(8)
+                    tick.label1.set_rotation(30)
 
-            plt.tight_layout(h_pad=0.0, w_pad=0.0)
-            fig.subplots_adjust(hspace=0.05, wspace=0.05)
+            plt.tight_layout()
+            fig.subplots_adjust(hspace=0.1, wspace=0.1)
 
             if add_prior:
                 self._add_prior_to_corner(axes, self.samples, add_prior)
 
             if save_fig:
                 fig_triangle.savefig(
                     os.path.join(self.outdir, self.label + "_corner.png"), dpi=dpi
                 )
                 plt.close(fig_triangle)
             else:
                 return fig, axes
 
     def plot_chainconsumer(self, save_fig=True, label_offset=0.25, dpi=300, **kwargs):
-        """Generate a corner plot of the posterior using chainconsumer
+        """Generate a corner plot of the posterior using the `chaniconsumer` package.
+
+        `chainconsumer` is an optional dependency of PyFstat. See https://samreay.github.io/ChainConsumer/.
+
+        Parameters are akin to the ones described in MCMCSearch.plot_corner.
+        Only the differing parameters are explicitly described.
 
         Parameters
         ----------
-        dpi: int
-            Passed to plt.savefig
         **kwargs:
-            Passed to chainconsumer.plotter.plot
-
+            Passed to chainconsumer.plotter.plot. Use "truths" to plot the true parameters of a signal.
         """
         try:
             import chainconsumer
         except ImportError:
-            logging.warning(
+            logger.warning(
                 "Could not import 'chainconsumer' package, please install it to use this method."
             )
             return
 
         samples_plt = copy.copy(self.samples)
         labels = self._get_labels(newline_units=True)
 
         samples_plt = self._scale_samples(samples_plt, self.theta_keys)
         if "truth" in kwargs:
             if not isinstance(kwargs["truth"], dict):
                 raise ValueError("'truth' must be a dictionary.")
             missing_keys = np.setdiff1d(self.theta_keys, list(kwargs["truth"].keys()))
             if len(missing_keys) > 0:
-                logging.warning(
+                logger.warning(
                     "plot_chainconsumer(): Missing keys {} in 'truth' dictionary,"
                     " argument will be ignored.".format(missing_keys)
                 )
                 kwargs["truth"] = None
             else:
                 parameters_in_order = np.array(
                     [kwargs["truth"][key] for key in self.theta_keys]
@@ -1039,21 +1160,14 @@
             ax.yaxis.set_label_coords(-label_offset, 0.5)
         for ax in axes[-1, :]:
             ax.xaxis.set_label_coords(0.5, -label_offset)
         for ax in axes_list:
             ax.set_rasterized(True)
             ax.set_rasterization_zorder(-10)
 
-            # for tick in ax.xaxis.get_major_ticks():
-            #    #tick.label.set_fontsize(8)
-            #    tick.label.set_rotation('horizontal')
-            # for tick in ax.yaxis.get_major_ticks():
-            #    #tick.label.set_fontsize(8)
-            #    tick.label.set_rotation('vertical')
-
             plt.tight_layout(h_pad=0.0, w_pad=0.0)
             fig.subplots_adjust(hspace=0.05, wspace=0.05)
 
         if save_fig:
             fig.savefig(
                 os.path.join(self.outdir, self.label + "_chainconsumer_corner.png"),
                 dpi=dpi,
@@ -1154,22 +1268,42 @@
     def plot_prior_posterior(
         self,
         normal_stds=2,
         injection_parameters=None,
         fig_and_axes=None,
         save_fig=True,
     ):
-        """ Plot the posterior in the context of the prior """
+        """Plot the prior and posterior probability distributions in the same figure
+
+        Parameters
+        ----------
+        normal_stds: int
+           Bounds of priors in terms of their standard deviation. Only used if
+           `norm`, `halfnorm`, `neghalfnorm` or `lognorm` priors are given, otherwise ignored.
+        injection_parameters: dict
+            Dictionary containing the parameters of a signal. All parameters being searched must be
+            present as dictionary keys, otherwise this option is ignored.
+        fig_and_axes: tuple
+            (fig, axes) tuple to plot on.
+        save_fig: bool
+            If true, save the figure, else return the fig, axes.
+
+        Returns
+        -------
+        (fig, ax): (matplotlib.pyplot.figure, matplotlib.pyplot.axes)
+            If `save_fig` evaluates to `False`, return figure and axes.
+        """
 
         # Check injection parameters first
+        injection_parameters = injection_parameters or {}
         missing_keys = set(self.theta_keys) - injection_parameters.keys()
         if missing_keys:
-            logging.warning(
+            logger.warning(
                 f"plot_prior_posterior(): Missing keys {missing_keys} in 'injection_parameters',"
-                " argument will be ignored."
+                " no injection parameters will be highlighted."
             )
             injection_parameters = None
 
         if fig_and_axes is None:
             fig, axes = plt.subplots(nrows=self.ndim, figsize=(8, 4 * self.ndim))
         else:
             fig, ax = fig_and_axes
@@ -1185,15 +1319,15 @@
             x = np.linspace(prior_bounds[key]["lower"], prior_bounds[key]["upper"], N)
             prior = np.exp([ln_prior_func(xi) for xi in x])  # may not be vectorized
 
             priorln = ax.plot(x, prior, "C3", label="prior")
             ax.set(xlabel=self.theta_symbols[i], yticks=[])
 
             s = self.samples[:, i]
-            while len(s) > 10 ** 4:
+            while len(s) > 10**4:
                 # random downsample to avoid slow calculation of kde
                 s = np.random.choice(s, size=int(len(s) / 2.0))
             kde = gaussian_kde(s)
             ax2 = ax.twinx()
             postln = ax2.plot(x, kde.pdf(x), "k", label="posterior")
             ax2.set(yticks=[], yticklabels=[])
 
@@ -1227,27 +1361,28 @@
 
         For example, one can pass signal arguments to predic_twoF_cumulative through `PFS_kwargs`, or
         set the number of segments using `num_segments_(CFS|PFS)`. The same applies for other options
         such as `tstart`, `tend` or `savefig`. Every single of these arguments will be passed to
         `pyfstat.core.ComputeFstat.plot_twoF_cumulative` as they are, using their default argument
         otherwise.
 
-        Keep in mind that one has to explicitely set `savefig=True` to output the figure!
-
         See `pyfstat.core.ComputeFstat.plot_twoF_cumulative` for a comprehensive list of accepted
         arguments and their default values.
+
+        Unlike the core function, here savefig=True is the default,
+        for consistency with other MCMC plotting functions.
         """
-        logging.info("Getting cumulative 2F")
+        logger.info("Getting cumulative 2F")
         d, maxtwoF = self.get_max_twoF()
         for key, val in self.theta_prior.items():
             if key not in d:
                 d[key] = val
 
-        if hasattr(self, "search") is False:
-            self._initiate_search_object()
+        if kwargs.get("savefig") is None:
+            kwargs["savefig"] = True
 
         self.search.plot_twoF_cumulative(
             CFS_input=d, label=self.label, outdir=self.outdir, **kwargs
         )
 
     def _generic_lnprior(self, **kwargs):
         """Return a lambda function of the pdf
@@ -1289,15 +1424,15 @@
                 return p
 
         def log_of_halfnorm(x, loc, scale):
             if x < loc:
                 return -np.inf
             else:
                 return -0.5 * (
-                    (x - loc) ** 2 / scale ** 2 + np.log(0.5 * np.pi * scale ** 2)
+                    (x - loc) ** 2 / scale**2 + np.log(0.5 * np.pi * scale**2)
                 )
 
         def cauchy(x, x0, gamma):
             return 1.0 / (np.pi * gamma * (1 + ((x - x0) / gamma) ** 2))
 
         def exp(x, x0, gamma):
             if x > x0:
@@ -1323,15 +1458,15 @@
         elif kwargs["type"] == "lognorm":
             # as of scipy 1.4.1 and numpy 1.18.1 the following parametrisation
             # should be consistent with np.random.lognormal in _generate_rv()
             return lambda x: lognorm.pdf(
                 x, s=kwargs["scale"], scale=np.exp(kwargs["loc"])
             )
         else:
-            logging.info("kwargs:", kwargs)
+            logger.info("kwargs:", kwargs)
             raise ValueError("Prior pdf type {:s} unknown.".format(kwargs["type"]))
 
     def _generate_rv(self, **kwargs):
         dist_type = kwargs.pop("type")
         if dist_type == "unif":
             return np.random.uniform(low=kwargs["lower"], high=kwargs["upper"])
         if dist_type == "log10unif":
@@ -1364,22 +1499,22 @@
         axes=None,
         xoffset=0,
         injection_parameters=None,
         plot_det_stat=False,
         context="ggplot",
         labelpad=5,
     ):
-        """ Plot all the chains from a sampler """
+        """Plot all the chains from a sampler"""
         if injection_parameters is not None:
             if not isinstance(injection_parameters, dict):
                 raise ValueError("injection_parameters is not a dictionary")
 
             missing_keys = set(self.theta_keys) - injection_parameters.keys()
             if missing_keys:
-                logging.warning(
+                logger.warning(
                     f"plot_walkers(): Missing keys {missing_keys} in 'injection_parameters',"
                     " argument will be ignored."
                 )
                 injection_parameters = None
             else:
                 scaled_injection_parameters = {
                     key: (
@@ -1406,15 +1541,15 @@
         shape = self.sampler.chain.shape
         if len(shape) == 3:
             nwalkers, nsteps, ndim = shape
             chain = self.sampler.chain[:, :, :].copy()
         if len(shape) == 4:
             ntemps, nwalkers, nsteps, ndim = shape
             if temp < ntemps:
-                logging.info("Plotting temperature {} chains".format(temp))
+                logger.info("Plotting temperature {} chains".format(temp))
             else:
                 raise ValueError(
                     ("Requested temperature {} outside of" "available range").format(
                         temp
                     )
                 )
             chain = self.sampler.chain[temp, :, :, :].copy()
@@ -1499,88 +1634,92 @@
                 if len(axes) == ndim:
                     axes.append(fig.add_subplot(ndim + 1, 1, ndim + 1))
 
                 lnl = self.sampler.loglikelihood[temp, :, :]
                 if burnin_idx and add_det_stat_burnin:
                     burn_in_vals = lnl[:, :burnin_idx].flatten()
                     try:
-                        twoF_burnin = 2 * (
+                        detstat_burnin = (
                             burn_in_vals[~np.isnan(burn_in_vals)] - self.likelihoodcoef
+                        ) / self.likelihooddetstatmultiplier
+                        axes[-1].hist(
+                            detstat_burnin, bins=50, histtype="step", color="C3"
                         )
-                        axes[-1].hist(twoF_burnin, bins=50, histtype="step", color="C3")
                     except ValueError:
-                        logging.info(
-                            "Det. Stat. hist failed, most likely all "
-                            "values where the same"
+                        logger.info(
+                            "Histogram of detection statistic failed, "
+                            "most likely all values were the same."
                         )
                         pass
                 else:
-                    twoF_burnin = []
+                    detstat_burnin = []
                 prod_vals = lnl[:, burnin_idx:].flatten()
                 try:
-                    twoF = 2 * (prod_vals[~np.isnan(prod_vals)] - self.likelihoodcoef)
-                    axes[-1].hist(twoF, bins=50, histtype="step", color="k")
+                    detstat = (
+                        prod_vals[~np.isnan(prod_vals)] - self.likelihoodcoef
+                    ) / self.likelihooddetstatmultiplier
+                    axes[-1].hist(detstat, bins=50, histtype="step", color="k")
                 except ValueError:
-                    logging.info(
-                        "Det. Stat. hist failed, most likely all "
-                        "values where the same"
+                    logger.info(
+                        "Histogram of detection statistic failed, "
+                        "most likely all values were the same."
                     )
                     pass
                 if self.BSGL:
-                    axes[-1].set_xlabel(r"$\mathcal{B}_\mathrm{S/GL}$")
+                    axes[-1].set_xlabel(r"$\log_{10}\mathcal{B}_\mathrm{S/GL}$")
                 else:
                     axes[-1].set_xlabel(r"$\widetilde{2\mathcal{F}}$")
                 axes[-1].set_ylabel(r"$\mathrm{Counts}$")
-                combined_vals = np.append(twoF_burnin, twoF)
+                combined_vals = np.append(detstat_burnin, detstat)
                 if len(combined_vals) > 0:
                     minv = np.min(combined_vals)
                     maxv = np.max(combined_vals)
                     Range = abs(maxv - minv)
                     axes[-1].set_xlim(minv - 0.1 * Range, maxv + 0.1 * Range)
 
                 xfmt = matplotlib.ticker.ScalarFormatter()
                 xfmt.set_powerlimits((-4, 4))
                 axes[-1].xaxis.set_major_formatter(xfmt)
 
         return fig, axes
 
     def _apply_corrections_to_p0(self, p0):
-        """ Apply any correction to the initial p0 values """
+        """Apply any correction to the initial p0 values"""
         return p0
 
     def _generate_scattered_p0(self, p):
-        """ Generate a set of p0s scattered about p """
+        """Generate a set of p0s scattered about p"""
         p0 = [
             [
                 p + self.scatter_val * p * np.random.randn(self.ndim)
                 for i in range(self.nwalkers)
             ]
             for j in range(self.ntemps)
         ]
         return p0
 
     def _generate_initial_p0(self):
-        """ Generate a set of init vals for the walkers """
+        """Generate a set of init vals for the walkers"""
 
         if type(self.theta_initial) == dict:
-            logging.info("Generate initial values from initial dictionary")
+            logger.info("Generate initial values from initial dictionary")
             if hasattr(self, "nglitch") and self.nglitch > 1:
                 raise ValueError("Initial dict not implemented for nglitch>1")
             p0 = [
                 [
                     [
                         self._generate_rv(**self.theta_initial[key])
                         for key in self.theta_keys
                     ]
                     for i in range(self.nwalkers)
                 ]
                 for j in range(self.ntemps)
             ]
         elif self.theta_initial is None:
-            logging.info("Generate initial values from prior dictionary")
+            logger.info("Generate initial values from prior dictionary")
             p0 = [
                 [
                     [
                         self._generate_rv(**self.theta_prior[key])
                         for key in self.theta_keys
                     ]
                     for i in range(self.nwalkers)
@@ -1602,45 +1741,41 @@
         temp_idx = 0
         pF = self.sampler.chain[temp_idx, :, :, :]
         lnl = self.sampler.loglikelihood[temp_idx, :, :]
         lnp = self.sampler.logprobability[temp_idx, :, :]
 
         # General warnings about the state of lnp
         if np.any(np.isnan(lnp)):
-            logging.warning(
+            logger.warning(
                 "Of {} lnprobs {} are nan".format(np.shape(lnp), np.sum(np.isnan(lnp)))
             )
         if np.any(np.isposinf(lnp)):
-            logging.warning(
+            logger.warning(
                 "Of {} lnprobs {} are +np.inf".format(
                     np.shape(lnp), np.sum(np.isposinf(lnp))
                 )
             )
         if np.any(np.isneginf(lnp)):
-            logging.warning(
+            logger.warning(
                 "Of {} lnprobs {} are -np.inf".format(
                     np.shape(lnp), np.sum(np.isneginf(lnp))
                 )
             )
 
         lnp_finite = copy.copy(lnp)
         lnp_finite[np.isinf(lnp)] = np.nan
         idx = np.unravel_index(np.nanargmax(lnp_finite), lnp_finite.shape)
         p = pF[idx]
         p0 = self._generate_scattered_p0(p)
 
-        self.search.BSGL = False
-        twoF = self.logl(p, self.search)
-        self.search.BSGL = self.BSGL
-
-        logging.info(
+        logger.info(
             (
-                "Gen. new p0 from pos {} which had det. stat.={:2.1f},"
-                " twoF={:2.1f} and lnp={:2.1f}"
-            ).format(idx[1], lnl[idx], twoF, lnp_finite[idx])
+                "Gen. new p0 from pos {} which had det. stat.={:2.1f}"
+                " and lnp={:2.1f}"
+            ).format(idx[1], lnl[idx], lnp_finite[idx])
         )
 
         return p0
 
     def _get_data_dictionary_to_save(self):
         d = dict(
             nsteps=self.nsteps,
@@ -1660,40 +1795,46 @@
         d["samples"] = samples
         d["lnprobs"] = lnprobs
         d["lnlikes"] = lnlikes
         d["chain"] = self.sampler.chain
         d["all_lnlikelihood"] = all_lnlikelihood
 
         if os.path.isfile(self.pickle_path):
-            logging.info(
+            logger.info(
                 "Saving backup of {} as {}.old".format(
                     self.pickle_path, self.pickle_path
                 )
             )
             os.rename(self.pickle_path, self.pickle_path + ".old")
         with open(self.pickle_path, "wb") as File:
             pickle.dump(d, File)
 
     def get_saved_data_dictionary(self):
-        """ Returns dictionary of the data saved in the pickle """
+        """Read the data saved in `self.pickel_path` and return it as a dictionary.
+
+        Returns
+        --------
+        d: dict
+            Dictionary containing the data saved in the pickle `self.pickle_path`.
+        """
         with open(self.pickle_path, "rb") as File:
             d = pickle.load(File)
         return d
 
     def _check_old_data_is_okay_to_use(self):
         if os.path.isfile(self.pickle_path) is False:
-            logging.info("No pickled data found")
+            logger.info("No pickled data found")
             return False
 
         if self.sftfilepattern is not None:
             oldest_sft = min(
                 [os.path.getmtime(f) for f in self._get_list_of_matching_sfts()]
             )
             if os.path.getmtime(self.pickle_path) < oldest_sft:
-                logging.info("Pickled data outdates sft files")
+                logger.info("Pickled data outdates sft files")
                 return False
 
         old_d = self.get_saved_data_dictionary().copy()
         new_d = self._get_data_dictionary_to_save().copy()
 
         old_d.pop("samples")
         old_d.pop("lnprobs")
@@ -1713,91 +1854,137 @@
                     mod_keys.append((key, old_d[key], new_d[key]))
             else:
                 raise ValueError("Keys {} not in old dictionary".format(key))
 
         if len(mod_keys) == 0:
             return True
         else:
-            logging.warning("Saved data differs from requested")
-            logging.info("Differences found in following keys:")
+            logger.warning("Saved data differs from requested")
+            logger.info("Differences found in following keys:")
             for key in mod_keys:
                 if len(key) == 3:
                     if np.isscalar(key[1]) or key[0] == "nsteps":
-                        logging.info("    {} : {} -> {}".format(*key))
+                        logger.info("    {} : {} -> {}".format(*key))
                     else:
-                        logging.info("    " + key[0])
+                        logger.info("    " + key[0])
                 else:
-                    logging.info(key)
+                    logger.info(key)
             return False
 
-    def get_savetxt_fmt(self):
-        fmt = helper_functions.get_doppler_params_output_format(self.theta_keys)
-        fmt += ["%.9g"]  # for detection statistic
-        return fmt
+    def _get_savetxt_fmt_dict(self):
+        fmt_dict = utils.get_doppler_params_output_format(self.theta_keys)
+        fmt_dict["twoF"] = "%.9g"
+        if self.BSGL:
+            fmt_dict["log10BSGL"] = "%.9g"
+        return fmt_dict
+
+    def _get_savetxt_gmt_list(self):
+        """Returns a list of output format specifiers, ordered like the samples
+
+        This is required because the output of _get_savetxt_fmt_dict()
+        will depend on the order in which those entries have been coded up.
+        """
+        fmt_dict = self._get_savetxt_fmt_dict()
+        fmt_list = [fmt_dict[key] for key in self.output_keys]
+        return fmt_list
 
     def export_samples_to_disk(self):
+        """
+        Export MCMC samples into a text file using `numpy.savetxt`.
+        """
         self.samples_file = os.path.join(self.outdir, self.label + "_samples.dat")
-        logging.info("Exporting samples to {}".format(self.samples_file))
+        logger.info("Exporting samples to {}".format(self.samples_file))
         header = "\n".join(self.output_file_header)
-        header += "\n" + " ".join(self.theta_keys) + " twoF"
-        outfmt = self.get_savetxt_fmt()
-        twoF = np.atleast_2d(self._get_twoF_from_loglikelihood()).T
-        samples_out = np.concatenate((self.samples, twoF), axis=1)
+        header += "\n" + " ".join(self.output_keys)
+        outfmt = self._get_savetxt_gmt_list()
+        samples_out = copy.copy(self.samples)
+        # For convenience, we always save a twoF column,
+        # even if log10BSGL was used for the likelihood.
+        detstat = np.atleast_2d(self._get_detstat_from_loglikelihood()).T
+        if self.BSGL:
+            twoF = np.zeros_like(detstat)
+            self.search.BSGL = False
+            for idx, samp in enumerate(self.samples):
+                p = self._set_point_for_evaluation(samp)
+                if isinstance(p, dict):
+                    twoF[idx] = self.search.get_det_stat(**p)
+                else:
+                    twoF[idx] = self.search.get_det_stat(*p)
+            self.search.BSGL = self.BSGL
+            samples_out = np.concatenate((samples_out, twoF), axis=1)
+        # TODO: add single-IFO F-stats?
+        samples_out = np.concatenate((samples_out, detstat), axis=1)
         Ncols = np.shape(samples_out)[1]
         if len(outfmt) != Ncols:
             raise RuntimeError(
                 "Lengths of data rows ({:d})"
                 " and output format ({:d})"
                 " do not match."
                 " If your search class uses different"
                 " keys than the base MCMCSearch class,"
-                " override the get_savetxt_fmt"
+                " override the _get_savetxt_fmt_dict"
                 " method.".format(Ncols, len(outfmt))
             )
         np.savetxt(
             self.samples_file,
             samples_out,
             delimiter=" ",
             header=header,
             fmt=outfmt,
         )
 
-    def _get_twoF_from_loglikelihood(self, idx=None):
-        if idx is None:
-            return (self.lnlikes - self.likelihoodcoef) * 2
-        else:
-            return (self.lnlikes[idx] - self.likelihoodcoef) * 2
-
-    def get_max_twoF(self, threshold=0.05):
-        """Returns the max likelihood sample and the corresponding 2F value
-
-        Note: the sample is returned as a dictionary along with an estimate of
-        the standard deviation calculated from the std of all samples with a
-        twoF within `threshold` (relative) to the max twoF
+    def _get_detstat_from_loglikelihood(self, idx=None):
+        """Inverts the extra terms applied in logl()."""
+        return (
+            self.lnlikes[idx if idx is not None else ...] - self.likelihoodcoef
+        ) / self.likelihooddetstatmultiplier
+
+    def get_max_twoF(self):
+        """Get the max. likelihood (loudest) sample and the compute
+        its corresponding detection statistic.
+
+        The employed detection statistic depends on `self.BSGL`
+        (i.e. 2F if `self.BSGL` evaluates to `False`, log10BSGL otherwise).
 
+        Returns
+        -------
+        d: dict
+            Parameters of the loudest sample.
+
+        maxtwoF: float
+            Detection statistic (2F or log10BSGL) corresponding to the loudest sample.
         """
+        if not hasattr(self, "search"):
+            raise RuntimeError(
+                "Object has no self.lnlikes attribute, please execute .run() first."
+            )
         if any(np.isposinf(self.lnlikes)):
-            logging.info("lnlike values contain positive infinite values")
+            logger.info("lnlike values contain positive infinite values")
         if any(np.isneginf(self.lnlikes)):
-            logging.info("lnlike values contain negative infinite values")
+            logger.info("lnlike values contain negative infinite values")
         if any(np.isnan(self.lnlikes)):
-            logging.info("lnlike values contain nan")
+            logger.info("lnlike values contain nan")
         idxs = np.isfinite(self.lnlikes)
         jmax = np.nanargmax(self.lnlikes[idxs])
         d = OrderedDict()
 
         if self.BSGL:
+            # need to recompute twoF at the max likelihood
             if hasattr(self, "search") is False:
                 self._initiate_search_object()
-            p = self.samples[jmax]
+            p = self._set_point_for_evaluation(self.samples[jmax])
             self.search.BSGL = False
-            maxtwoF = self.logl(p, self.search)
+            if isinstance(p, dict):
+                maxtwoF = self.search.get_det_stat(**p)
+            else:
+                maxtwoF = self.search.get_det_stat(*p)
             self.search.BSGL = self.BSGL
         else:
-            maxtwoF = self._get_twoF_from_loglikelihood(jmax)
+            # can just reuse the logl value
+            maxtwoF = self._get_detstat_from_loglikelihood(jmax)
 
         repeats = []
         for i, k in enumerate(self.theta_keys):
             if k in d and k not in repeats:
                 d[k + "_0"] = d[k]  # relabel the old key
                 d.pop(k)
                 repeats.append(k)
@@ -1807,15 +1994,25 @@
                 while k in d:
                     k = k.replace("_{}".format(count - 1), "_{}".format(count))
                     count += 1
             d[k] = self.samples[jmax][i]
         return d, maxtwoF
 
     def get_summary_stats(self):
-        """ Returns a dict of point estimates for all production samples """
+        """Returns a dict of point estimates for all production samples.
+
+        Point estimates are computed on the MCMC samples using `numpy.mean`,
+        `numpy.std` and `numpy.quantiles` with q=[0.005, 0.05, 0.25, 0.5, 0.75, 0.95, 0.995].
+
+        Returns
+        -------
+        d: dict
+            Dictionary containing point estimates corresponding to ["mean", "std", "lower99",
+            "lower90", "lower50", "median", "upper50", "upper90", "upper99"].
+        """
         d = OrderedDict()
         repeats = []  # taken from old get_median_stds(), not sure why necessary
         for s, k in zip(self.samples.T, self.theta_keys):
             if k in d and k not in repeats:
                 d[k + "_0"] = d[k]  # relabel the old key
                 d.pop(k)
                 repeats.append(k)
@@ -1864,35 +2061,41 @@
                 fracs = []
                 for bound in ["lower", "upper"]:
                     bools = np.abs(s - prior[bound]) / prior_range < threshold
                     if np.any(bools):
                         edges.append(bound)
                         fracs.append(str(100 * float(np.sum(bools)) / len(bools)))
                 if len(edges) > 0:
-                    logging.warning(
+                    logger.warning(
                         "{}% of the {} posterior is railing on the {} edges".format(
                             "% & ".join(fracs), k, " & ".join(edges)
                         )
                     )
                     return_flag = True
         return return_flag
 
     def write_par(self, method="median"):
-        """ Writes a .par of the best-fit params with an estimated std """
+        """Writes a .par of the best-fit params with an estimated std
+
+        Parameters
+        ----------
+        method: str
+            How to select the `best-fit` params. Available methods: "median", "mean", "twoFmax".
+        """
 
         if method == "med":
             method = "median"
         if method in ["median", "mean"]:
             summary_stats = self.get_summary_stats()
             filename = os.path.join(self.outdir, self.label + "_" + method + ".par")
-            logging.info("Writing {} using {} parameters.".format(filename, method))
+            logger.info("Writing {} using {} parameters.".format(filename, method))
         elif method == "twoFmax":
             max_twoF_d, max_twoF = self.get_max_twoF()
             filename = os.path.join(self.outdir, self.label + "_max2F.par")
-            logging.info("Writing {} at max twoF = {}.".format(filename, max_twoF))
+            logger.info("Writing {} at max twoF = {}.".format(filename, max_twoF))
         else:
             raise ValueError("Method '{}' not supported.".format(method))
 
         with open(filename, "w+") as f:
             for hline in self.output_file_header:
                 f.write("# {:s}\n".format(hline))
             if method == "twoFmax":
@@ -1909,72 +2112,57 @@
                         )
                     )
             elif method == "twoFmax":
                 for key, val in max_twoF_d.items():
                     f.write("{} = {:1.16e}\n".format(key, val))
 
     def generate_loudest(self):
-        """ Use lalapps_ComputeFstatistic_v2 to produce a .loudest file """
-        logging.info("Running CFSv2 to get .loudest file")
-        self.write_par(method="twoFmax")
-        params = self.read_par(label=self.label + "_max2F")
-        if np.any([key in params for key in ["delta_F0", "delta_F1", "tglitch"]]):
-            raise RuntimeError(
-                "CFSv2 --outputLoudest cannot deal with glitch parameters."
-            )
-        if getattr(self, "transientWindowType", None) is not None:
-            logging.warning(
-                "CFSv2 --outputLoudest always reports the maximum of the"
-                " standard CW 2F-statistic, not the transient max2F."
-            )
+        """Use ComputeFstatistic_v2 executable to produce a .loudest file"""
+        max_params, max_twoF = self.get_max_twoF()
         for key in self.theta_prior:
-            if key not in params:
-                params[key] = self.theta_prior[key]
-        params_sanitised = self.translate_keys_to_lal(params)
+            if key not in max_params:
+                max_params[key] = self.theta_prior[key]
+        max_params = self.translate_keys_to_lal(max_params)
         for key in ["transient-t0Epoch", "transient-t0Offset", "transient-tau"]:
-            if (
-                key in params_sanitised
-                and not int(params_sanitised[key]) == params_sanitised[key]
-            ):
-                rounded = int(round(params_sanitised[key]))
-                logging.warning(
+            if key in max_params and not int(max_params[key]) == max_params[key]:
+                rounded = int(round(max_params[key]))
+                logger.warning(
                     "Rounding {:s}={:f} to {:d} for CFSv2 call.".format(
-                        key, params_sanitised[key], rounded
+                        key, max_params[key], rounded
                     )
                 )
-                params_sanitised[key] = rounded
-        signal_parameter_keys = self.translate_keys_to_lal(self.theta_prior).keys()
-
-        self.loudest_file = os.path.join(self.outdir, self.label + ".loudest")
-        cmd = "lalapps_ComputeFstatistic_v2 "
-        cmd += (
-            '-D "{}" --outputLoudest="{}" --minStartTime={} --maxStartTime={} --refTime={} '
-        ).format(
-            self.sftfilepattern,
-            self.loudest_file,
-            self.minStartTime,
-            self.maxStartTime,
-            self.tref,
+                max_params[key] = rounded
+        signal_parameter_keys = list(
+            self.translate_keys_to_lal(self.theta_prior).keys()
         )
-        cmd += " ".join(
-            [
-                "--{0} {1}".format(key, params_sanitised[key])
-                for key in signal_parameter_keys
-            ]
+        par_keys = list(max_params.keys())
+        pardiff = np.setdiff1d(par_keys, signal_parameter_keys)
+        if len(pardiff) > 0:
+            raise RuntimeError(
+                f"Dictionary for parameters at max2F point {par_keys}"
+                " did include keys"
+                # " (other than refTime)"
+                " not expected from signal parameters being searched over:"
+                f" {pardiff} not in {signal_parameter_keys}."
+            )
+        self.loudest_file = utils.generate_loudest_file(
+            max_params=max_params,
+            tref=self.tref,
+            outdir=self.outdir,
+            label=self.label,
+            sftfilepattern=self.sftfilepattern,
+            minStartTime=self.minStartTime,
+            maxStartTime=self.maxStartTime,
+            transientWindowType=getattr(self, "transientWindowType", None),
+            earth_ephem=self.earth_ephem,
+            sun_ephem=self.sun_ephem,
         )
-        if getattr(self, "transientWindowType", None) is not None:
-            cmd += " --transient-WindowType='{}'".format(self.transientWindowType)
-        if getattr(self, "earth_ephem", None) is not None:
-            cmd += " --ephemEarth='{}'".format(self.earth_ephem)
-        if getattr(self, "sun_ephem", None) is not None:
-            cmd += " --ephemSun='{}'".format(self.sun_ephem)
-        helper_functions.run_commandline(cmd, return_output=False)
 
     def write_prior_table(self):
-        """ Generate a .tex file of the prior """
+        """Generate a .tex file of the prior"""
         with open(os.path.join(self.outdir, self.label + "_prior.tex"), "w") as f:
             f.write(
                 r"\begin{tabular}{c l c} \hline" + "\n"
                 r"Parameter & & &  \\ \hhline{====}"
             )
 
             for key, prior in self.theta_prior.items():
@@ -1992,47 +2180,46 @@
                         a = prior["loc"]
                         b = prior["scale"]
                         line = r"{} & $|\mathcal{{N}}$({}, {})| & {}\\"
 
                     u = self.unit_dictionary[key]
                     s = self.symbol_dictionary[key]
                     f.write("\n")
-                    a = helper_functions.texify_float(a)
-                    b = helper_functions.texify_float(b)
+                    a = utils.texify_float(a)
+                    b = utils.texify_float(b)
                     f.write(" " + line.format(s, a, b, u) + r" \\")
             f.write("\n\\end{tabular}\n")
 
     def print_summary(self):
-        """ Prints a summary of the max twoF found to the terminal """
+        """Prints a summary of the max twoF found to the terminal"""
         max_twoFd, max_twoF = self.get_max_twoF()
         summary_stats = self.get_summary_stats()
-        logging.info("Summary:")
+        logger.info("Summary:")
         if hasattr(self, "theta0_idx"):
-            logging.info("theta0 index: {}".format(self.theta0_idx))
-        logging.info("Max twoF: {} with parameters:".format(max_twoF))
+            logger.info("theta0 index: {}".format(self.theta0_idx))
+        logger.info("Max twoF: {} with parameters:".format(max_twoF))
         for k in np.sort(list(max_twoFd.keys())):
-            logging.info("  {:10s} = {:1.9e}".format(k, max_twoFd[k]))
-        logging.info("Mean +- std for production values:")
+            logger.info("  {:10s} = {:1.9e}".format(k, max_twoFd[k]))
+        logger.info("Mean +- std for production values:")
         for k in np.sort(list(summary_stats.keys())):
-            logging.info(
+            logger.info(
                 "  {:10s} = {:1.9e} +/- {:1.9e}".format(
                     k, summary_stats[k]["mean"], summary_stats[k]["std"]
                 )
             )
-        logging.info("Median and 90% quantiles for production values:")
+        logger.info("Median and 90% quantiles for production values:")
         for k in np.sort(list(summary_stats.keys())):
-            logging.info(
+            logger.info(
                 "  {:10s} = {:1.9e} - {:1.9e} + {:1.9e}".format(
                     k,
                     summary_stats[k]["median"],
                     summary_stats[k]["median"] - summary_stats[k]["lower90"],
                     summary_stats[k]["upper90"] - summary_stats[k]["median"],
                 )
             )
-        logging.info("\n")
 
     def _CF_twoFmax(self, theta, twoFmax, ntrials):
         Fmax = twoFmax / 2.0
         return (
             np.exp(1j * theta * twoFmax)
             * ntrials
             / 2.0
@@ -2076,51 +2263,74 @@
         ntrials: int, array of len Nglitch+1
             The number of trials for each glitch+1
         """
         twoFhats = np.linspace(twoFhat, twoFhatmax, Npoints)
         pdf = self._pdf_twoFhat(twoFhats, self.nglitch, ntrials)
         return np.trapz(pdf, twoFhats)
 
-    def get_p_value(self, delta_F0, time_trials=0):
-        """ Get's the p-value for the maximum twoFhat value """
+    def get_p_value(self, delta_F0=0, time_trials=0):
+        """Gets the p-value for the maximum twoFhat value assuming Gaussian noise
+
+        Parameters
+        ----------
+        delta_F0: float
+            Frequency variation due to a glitch.
+        time_trials: int, optional
+            Number of trials in each glitch + 1.
+        """
         d, max_twoF = self.get_max_twoF()
         if self.nglitch == 1:
             tglitches = [d["tglitch"]]
         else:
             tglitches = [d["tglitch_{}".format(i)] for i in range(self.nglitch)]
         tboundaries = [self.minStartTime] + tglitches + [self.maxStartTime]
         deltaTs = np.diff(tboundaries)
         ntrials = [time_trials + delta_F0 * dT for dT in deltaTs]
         p_val = self._p_val_twoFhat(max_twoF, ntrials)
-        logging.info("p-value = {}".format(p_val))
+        logger.info("p-value = {}".format(p_val))
         return p_val
 
     def compute_evidence(self, make_plots=False, write_to_file=None):
-        """ Computes the evidence/marginal likelihood for the model """
+        """Computes the evidence/marginal likelihood for the model.
+
+        Parameters
+        ----------
+        make_plots: bool
+           Plot the results and save them to os.path.join(self.outdir, self.label + "_beta_lnl.png")
+        write_to_file: str
+           If given, dump evidence and uncertainty estimation to the specified path.
+
+        Returns
+        -------
+        log10evidence: float
+            Estimation of the log10 evidence.
+        log10evidence_err: float
+            Log10 uncertainty of the evidence estimation.
+        """
         betas = self.betas
         mean_lnlikes = np.mean(np.mean(self.all_lnlikelihood, axis=1), axis=1)
 
         mean_lnlikes = mean_lnlikes[::-1]
         betas = betas[::-1]
 
         if any(np.isinf(mean_lnlikes)):
-            logging.warning(
+            logger.warning(
                 "mean_lnlikes contains inf: recalculating without"
                 " the {} infs".format(len(betas[np.isinf(mean_lnlikes)]))
             )
             idxs = np.isinf(mean_lnlikes)
             mean_lnlikes = mean_lnlikes[~idxs]
             betas = betas[~idxs]
 
         log10evidence = np.trapz(mean_lnlikes, betas) / np.log(10)
         z1 = np.trapz(mean_lnlikes, betas)
         z2 = np.trapz(mean_lnlikes[::-1][::2][::-1], betas[::-1][::2][::-1])
         log10evidence_err = np.abs(z1 - z2) / np.log(10)
 
-        logging.info(
+        logger.info(
             "log10 evidence for {} = {} +/- {}".format(
                 self.label, log10evidence, log10evidence_err
             )
         )
 
         if write_to_file:
             EvidenceDict = self.read_evidence_file_to_dict(write_to_file)
@@ -2150,78 +2360,109 @@
             fig.savefig(os.path.join(self.outdir, self.label + "_beta_lnl.png"))
             plt.close(fig)
 
         return log10evidence, log10evidence_err
 
     @staticmethod
     def read_evidence_file_to_dict(evidence_file_name="Evidences.txt"):
+        """Read evidence file and put it into an OrderedDict
+
+        An evidence file contains paris (log10evidence, log10evidence_err) for each
+        considered model. These pairs are prepended by the `self.label` variable.
+
+        Parameters
+        ----------
+        evidence_file_name: str
+            Filename to read.
+
+        Returns
+        -------
+        EvidenceDict: dict
+            Dictionary with the contents of `evidence_file_name`
+        """
         EvidenceDict = OrderedDict()
         if os.path.isfile(evidence_file_name):
             with open(evidence_file_name, "r") as f:
                 for line in f:
                     key, log10evidence, log10evidence_err = line.split(" ")
                     EvidenceDict[key] = [float(log10evidence), float(log10evidence_err)]
         return EvidenceDict
 
     def write_evidence_file_from_dict(self, EvidenceDict, evidence_file_name):
+        """Write evidence dict to a file
+
+        Parameters
+        ----------
+        EvidenceDict: dict
+            Dictionary to dump into a file.
+        evidence_file_name: str
+            File name to dump dict into.
+        """
         with open(evidence_file_name, "w+") as f:
             for key, val in EvidenceDict.items():
                 f.write("{} {} {}\n".format(key, val[0], val[1]))
 
 
 class MCMCGlitchSearch(MCMCSearch):
     """MCMC search using the SemiCoherentGlitchSearch
 
     See parent MCMCSearch for a list of all additional parameters, here we list
     only the additional init parameters of this class.
-
-    Parameters
-    ----------
-    nglitch: int
-        The number of glitches to allow
-    dtglitchmin: int
-        The minimum duration (in seconds) of a segment between two glitches
-        or a glitch and the start/end of the data
-    theta0_idx, int
-        Index (zero-based) of which segment the theta refers to - useful
-        if providing a tight prior on theta to allow the signal to jump
-        too theta (and not just from)
-
     """
 
     symbol_dictionary = dict(
         F0=r"$f$",
         F1=r"$\dot{f}$",
         F2=r"$\ddot{f}$",
         Alpha=r"$\alpha$",
         Delta=r"$\delta$",
+    )
+    """
+        Key, val pairs of the parameters (`F0`, `F1`, ...), to LaTeX math
+        symbols for plots
+    """
+    glitch_symbol_dictionary = dict(
         delta_F0=r"$\delta f$",
         delta_F1=r"$\delta \dot{f}$",
         tglitch=r"$t_\mathrm{glitch}$",
     )
+    """
+        Key, val pairs of glitch parameters (`dF0`, `dF1`, `tglitch`), to LaTeX math
+        symbols for plots. This dictionary included within `self.symbol_dictionary`.
+    """
+    symbol_dictionary.update(glitch_symbol_dictionary)
     unit_dictionary = dict(
         F0=r"Hz",
         F1=r"Hz/s",
         F2=r"Hz/s$^2$",
         Alpha=r"rad",
         Delta=r"rad",
         delta_F0=r"Hz",
         delta_F1=r"Hz/s",
         tglitch=r"s",
     )
+    """
+        Key, val pairs of the parameters (`F0`, `F1`, ..., including glitch parameters),
+        and the units (`Hz`, `Hz/s`, ...).
+    """
     transform_dictionary = dict(
         tglitch={
             "multiplier": 1 / 86400.0,
             "subtractor": "minStartTime",
             "unit": "day",
             "label": r"$t^{g}_0$ \n [d]",
         }
     )
+    """
+        Key, val pairs of the parameters (`F0`, `F1`, ...), where the key is
+        itself a dictionary which can item `multiplier`, `subtractor`, or
+        `unit` by which to transform by and update the units.
+    """
 
-    @helper_functions.initializer
+    @utils.initializer
     def __init__(
         self,
         theta_prior,
         tref,
         label,
         outdir="data",
         minStartTime=None,
@@ -2243,46 +2484,66 @@
         injectSources=None,
         assumeSqrtSX=None,
         dtglitchmin=1 * 86400,
         theta0_idx=0,
         nglitch=1,
         earth_ephem=None,
         sun_ephem=None,
+        allowedMismatchFromSFTLength=None,
+        clean=False,
     ):
-
+        """
+        Parameters
+        ----------
+        nglitch: int
+            The number of glitches to allow
+        dtglitchmin: int
+            The minimum duration (in seconds) of a segment between two glitches
+            or a glitch and the start/end of the data
+        theta0_idx, int
+            Index (zero-based) of which segment the theta refers to - useful
+            if providing a tight prior on theta to allow the signal to jump
+            too theta (and not just from)
+        """
         self._set_init_params_dict(locals())
-        if os.path.isdir(outdir) is False:
-            os.mkdir(outdir)
+        os.makedirs(outdir, exist_ok=True)
         self.output_file_header = self.get_output_file_header()
-        self._add_log_file(self.output_file_header)
-        logging.info(
+        logger.info(
             (
                 "Set-up MCMC glitch search with {} glitches for model {}" " on data {}"
             ).format(self.nglitch, self.label, self.sftfilepattern)
         )
         self.pickle_path = os.path.join(self.outdir, self.label + "_saved_data.p")
         self._unpack_input_theta()
         self.ndim = len(self.theta_keys)
         if self.log10beta_min:
             self.betas = np.logspace(0, self.log10beta_min, self.ntemps)
         else:
             self.betas = None
-        if args.clean and os.path.isfile(self.pickle_path):
+        if self.clean and os.path.isfile(self.pickle_path):
             os.rename(self.pickle_path, self.pickle_path + ".old")
 
         self.old_data_is_okay_to_use = self._check_old_data_is_okay_to_use()
         self._log_input()
         self._set_likelihoodcoef()
         self.set_ephemeris_files(earth_ephem, sun_ephem)
+        self.allowedMismatchFromSFTLength = allowedMismatchFromSFTLength
 
     def _set_likelihoodcoef(self):
-        self.likelihoodcoef = (self.nglitch + 1) * np.log(70.0 / self.rhohatmax ** 4)
+        """Additional constant terms to turn a detection statistic into a likelihood.
+
+        See MCMCSearch._set_likelihoodcoef for the base implementation.
+        This method simply extends it in order to account for the increased number
+        of segments due to the presence of glitches.
+        """
+        super()._set_likelihoodcoef()
+        self.likelihoodcoef *= self.nglitch + 1
 
     def _initiate_search_object(self):
-        logging.info("Setting up search object")
+        logger.info("Setting up search object")
         search_ranges = self._get_search_ranges()
         self.search = core.SemiCoherentGlitchSearch(
             label=self.label,
             outdir=self.outdir,
             sftfilepattern=self.sftfilepattern,
             tref=self.tref,
             minStartTime=self.minStartTime,
@@ -2293,21 +2554,22 @@
             detectors=self.detectors,
             BSGL=self.BSGL,
             nglitch=self.nglitch,
             theta0_idx=self.theta0_idx,
             injectSources=self.injectSources,
             earth_ephem=self.earth_ephem,
             sun_ephem=self.sun_ephem,
+            allowedMismatchFromSFTLength=self.allowedMismatchFromSFTLength,
         )
         if self.minStartTime is None:
             self.minStartTime = self.search.minStartTime
         if self.maxStartTime is None:
             self.maxStartTime = self.search.maxStartTime
 
-    def logp(self, theta_vals, theta_prior, theta_keys, search):
+    def _logp(self, theta_vals, theta_prior, theta_keys, search):
         if self.nglitch > 1:
             ts = (
                 [self.minStartTime]
                 + list(theta_vals[-self.nglitch :])
                 + [self.maxStartTime]
             )
             if np.array_equal(ts, np.sort(ts)) is False:
@@ -2317,28 +2579,28 @@
 
         H = [
             self._generic_lnprior(**theta_prior[key])(p)
             for p, key in zip(theta_vals, theta_keys)
         ]
         return np.sum(H)
 
-    def logl(self, theta, search):
+    def _logl(self, theta, search):
+        in_theta = self._set_point_for_evaluation(theta)
         if self.nglitch > 1:
             ts = (
                 [self.minStartTime] + list(theta[-self.nglitch :]) + [self.maxStartTime]
             )
             if np.array_equal(ts, np.sort(ts)) is False:
                 return -np.inf
-
-        for j, theta_i in enumerate(self.theta_idxs):
-            self.fixed_theta[theta_i] = theta[j]
-        twoF = search.get_semicoherent_nglitch_twoF(*self.fixed_theta)
-        return twoF / 2.0 + self.likelihoodcoef
+        # FIXME: BSGL case?
+        twoF = search.get_semicoherent_nglitch_twoF(*in_theta)
+        return twoF * self.likelihooddetstatmultiplier + self.likelihoodcoef
 
     def _unpack_input_theta(self):
+        base_keys = ["F0", "F1", "F2", "Alpha", "Delta"]
         glitch_keys = ["delta_F0", "delta_F1", "tglitch"]
         full_glitch_keys = list(
             np.array([[gk] * self.nglitch for gk in glitch_keys]).flatten()
         )
 
         if "tglitch_0" in self.theta_prior:
             full_glitch_keys[-self.nglitch :] = [
@@ -2346,27 +2608,24 @@
             ]
             full_glitch_keys[-2 * self.nglitch : -1 * self.nglitch] = [
                 "delta_F1_{}".format(i) for i in range(self.nglitch)
             ]
             full_glitch_keys[-4 * self.nglitch : -2 * self.nglitch] = [
                 "delta_F0_{}".format(i) for i in range(self.nglitch)
             ]
-        full_theta_keys = ["F0", "F1", "F2", "Alpha", "Delta"] + full_glitch_keys
+        full_theta_keys = base_keys + full_glitch_keys
         full_theta_keys_copy = copy.copy(full_theta_keys)
 
-        glitch_symbols = [r"$\delta f$", r"$\delta \dot{f}$", r"$t_{glitch}$"]
         full_glitch_symbols = list(
-            np.array([[gs] * self.nglitch for gs in glitch_symbols]).flatten()
+            np.array(
+                [[gs] * self.nglitch for gs in self.glitch_symbol_dictionary]
+            ).flatten()
         )
         full_theta_symbols = [
-            r"$f$",
-            r"$\dot{f}$",
-            r"$\ddot{f}$",
-            r"$\alpha$",
-            r"$\delta$",
+            self.symbol_dictionary[key] for key in base_keys
         ] + full_glitch_symbols
         self.theta_keys = []
         fixed_theta_dict = {}
         for key, val in self.theta_prior.items():
             if type(val) is dict:
                 fixed_theta_dict[key] = 0
                 if key in glitch_keys:
@@ -2405,14 +2664,19 @@
         # Correct for number of glitches in the idxs
         self.theta_idxs = np.array(self.theta_idxs)
         while np.sum(self.theta_idxs[:-1] == self.theta_idxs[1:]) > 0:
             for i, idx in enumerate(self.theta_idxs):
                 if idx in self.theta_idxs[:i]:
                     self.theta_idxs[i] += 1
 
+        self.output_keys = self.theta_keys.copy()
+        self.output_keys.append("twoF")
+        if self.BSGL:
+            self.output_keys.append("log10BSGL")
+
     def _get_data_dictionary_to_save(self):
         d = dict(
             nsteps=self.nsteps,
             nwalkers=self.nwalkers,
             ntemps=self.ntemps,
             theta_keys=self.theta_keys,
             theta_prior=self.theta_prior,
@@ -2426,16 +2690,28 @@
 
     def _apply_corrections_to_p0(self, p0):
         p0 = np.array(p0)
         if self.nglitch > 1:
             p0[:, :, -self.nglitch :] = np.sort(p0[:, :, -self.nglitch :], axis=2)
         return p0
 
-    def plot_cumulative_max(self):
-        logging.info("Getting cumulative 2F")
+    def plot_cumulative_max(self, savefig=True):
+        """
+        Override MCMCSearch.plot_cumulative_max implementation to deal with the
+        split at glitches.
+
+        Parameters
+        ----------
+        savefig: boolean
+            included for consistency with core plot_twoF_cumulative() function.
+            If true, save the figure in outdir.
+            If false, return an axis object.
+        """
+
+        logger.info("Getting cumulative 2F")
         fig, ax = plt.subplots()
         d, maxtwoF = self.get_max_twoF()
         for key, val in self.theta_prior.items():
             if key not in d:
                 d[key] = val
 
         if self.nglitch > 1:
@@ -2453,15 +2729,15 @@
 
         tboundaries = [self.minStartTime] + tglitches + [self.maxStartTime]
 
         for j in range(self.nglitch + 1):
             ts = tboundaries[j]
             te = tboundaries[j + 1]
             if (te - ts) / 86400 < 5:
-                logging.info("Period too short to perform cumulative search")
+                logger.info("Period too short to perform cumulative search")
                 continue
             if j < self.theta0_idx:
                 summed_deltaF0 = np.sum(delta_F0s[j : self.theta0_idx])
                 F0_j = d["F0"] - summed_deltaF0
                 actual_ts, taus, twoFs = self.search.calculate_twoF_cumulative(
                     F0_j,
                     F1=d["F1"],
@@ -2483,89 +2759,41 @@
                     Delta=d["Delta"],
                     tstart=ts,
                     tend=te,
                 )
             ax.plot(actual_ts + taus, twoFs)
 
         ax.set_xlabel("GPS time")
-        fig.savefig(os.path.join(self.outdir, self.label + "_twoFcumulative.png"))
-        plt.close(fig)
+        if savefig:
+            fig.savefig(os.path.join(self.outdir, self.label + "_twoFcumulative.png"))
+            plt.close(fig)
+        return ax
 
-    def get_savetxt_fmt(self):
-        fmt = helper_functions.get_doppler_params_output_format(
-            [k.split("_")[1] for k in self.theta_keys if k.startswith("delta_F")]
-        )
+    def _get_savetxt_fmt_dict(self):
+        fmt_dict = utils.get_doppler_params_output_format(self.theta_keys)
         if "tglitch" in self.theta_keys:
-            fmt += ["%d"]
-        fmt += helper_functions.get_doppler_params_output_format(self.theta_keys)
-        fmt += ["%.9g"]  # for detection statistic
-        return fmt
+            fmt_dict["tglitch"] = "%d"
+        if "delta_F0" in self.theta_keys:
+            fmt_dict["delta_F0"] = "%.16g"
+        if "delta_F1" in self.theta_keys:
+            fmt_dict["delta_F1"] = "%.16g"
+        fmt_dict["twoF"] = "%.9g"
+        if self.BSGL:
+            fmt_dict["log10BSGL"] = "%.9g"
+        return fmt_dict
 
 
 class MCMCSemiCoherentSearch(MCMCSearch):
-    """MCMC search for a signal using the semi-coherent ComputeFstat
+    """MCMC search for a signal using the semicoherent ComputeFstat.
 
-    Parameters
-    ----------
-    theta_prior: dict
-        Dictionary of priors and fixed values for the search parameters.
-        For each parameters (key of the dict), if it is to be held fixed
-        the value should be the constant float, if it is be searched, the
-        value should be a dictionary of the prior.
-    tref, minStartTime, maxStartTime: int
-        GPS seconds of the reference time, start time and end time. While tref
-        is requirede, minStartTime and maxStartTime default to None in which
-        case all available data is used.
-    label, outdir: str
-        A label and output directory (optional, defaults is `'data'`) to
-        name files
-    sftfilepattern: str, optional
-        Pattern to match SFTs using wildcards (*?) and ranges [0-9];
-        mutiple patterns can be given separated by colons.
-    detectors: str, optional
-        Two character reference to the detectors to use, specify None for no
-        contraint and comma separate for multiple references.
-    nsteps: list (2,), optional
-        Number of burn-in and production steps to take, [nburn, nprod]. See
-        `pyfstat.MCMCSearch.setup_initialisation()` for details on adding
-        initialisation steps.
-    nwalkers, ntemps: int, optional
-        The number of walkers and temperates to use in the parallel
-        tempered PTSampler.
-    log10beta_min float < 0, optional
-        The  log_10(beta) value, if given the set of betas passed to PTSampler
-        are generated from `np.logspace(0, log10beta_min, ntemps)` (given
-        in descending order to ptemcee).
-    theta_initial: dict, array, optional
-        A dictionary of distribution about which to distribute the
-        initial walkers about
-    rhohatmax: float, optional
-        Upper bound for the SNR scale parameter (required to normalise the
-        Bayes factor) - this needs to be carefully set when using the
-        evidence.
-    binary: bool, optional
-        If true, search over binary parameters
-    BSGL: bool, optional
-        If true, use the BSGL statistic
-    SSBPrec: int, optional
-        SSBPrec (SSB precision) to use when calling ComputeFstat
-    RngMedWindow: int, optional
-        Running-Median window size (number of bins) for ComputeFstat
-    minCoverFreq, maxCoverFreq: float, optional
-        Minimum and maximum instantaneous frequency which will be covered
-        over the SFT time span as passed to CreateFstatInput
-    injectSources: dict, optional
-        If given, inject these properties into the SFT files before running
-        the search
-    assumeSqrtSX: float or list or str, optional
-        Don't estimate noise-floors, but assume (stationary) per-IFO sqrt{SX}.
-        See `core.ComputeFstat`.
-    nsegs: int
-        The number of segments
+    Evaluates the semicoherent F-statistic acros a parameter space region
+    corresponding to an isolated/binary-modulated CW signal.
 
+    See MCMCSearch for a list of additional parameters, here we list only the additional
+    init parameters of this class.
     """
 
     def __init__(
         self,
         theta_prior,
         tref,
         label,
@@ -2587,16 +2815,24 @@
         minCoverFreq=None,
         maxCoverFreq=None,
         injectSources=None,
         assumeSqrtSX=None,
         nsegs=None,
         earth_ephem=None,
         sun_ephem=None,
+        allowedMismatchFromSFTLength=None,
+        clean=False,
     ):
-
+        """
+        Parameters
+        ----------
+        nsegs: int
+            The number of segments into which the input datastream will be devided.
+            Coherence time is computed internally as (maxStartTime - minStarTime) / nsegs.
+        """
         self._set_init_params_dict(locals())
         self.theta_prior = theta_prior
         self.tref = tref
         self.label = label
         self.outdir = outdir
         self.minStartTime = minStartTime
         self.maxStartTime = maxStartTime
@@ -2614,43 +2850,50 @@
         self.RngMedWindow = RngMedWindow
         self.minCoverFreq = minCoverFreq
         self.maxCoverFreq = maxCoverFreq
         self.injectSources = injectSources
         self.assumeSqrtSX = assumeSqrtSX
         self.nsegs = nsegs
         self.set_ephemeris_files(earth_ephem, sun_ephem)
+        self.allowedMismatchFromSFTLength = allowedMismatchFromSFTLength
+        self.clean = clean
 
-        if os.path.isdir(outdir) is False:
-            os.mkdir(outdir)
+        os.makedirs(outdir, exist_ok=True)
         self.output_file_header = self.get_output_file_header()
-        self._add_log_file(self.output_file_header)
-        logging.info(
+        logger.info(
             ("Set-up MCMC semi-coherent search for model {} on data" "{}").format(
                 self.label, self.sftfilepattern
             )
         )
         self.pickle_path = os.path.join(self.outdir, self.label + "_saved_data.p")
         self._unpack_input_theta()
         self.ndim = len(self.theta_keys)
         if self.log10beta_min:
             self.betas = np.logspace(0, self.log10beta_min, self.ntemps)
         else:
             self.betas = None
-        if args.clean and os.path.isfile(self.pickle_path):
+        if self.clean and os.path.isfile(self.pickle_path):
             os.rename(self.pickle_path, self.pickle_path + ".old")
 
         self._log_input()
 
         if self.nsegs:
             self._set_likelihoodcoef()
         else:
-            logging.info("Value `nsegs` not yet provided")
+            logger.info("Value `nsegs` not yet provided")
 
     def _set_likelihoodcoef(self):
-        self.likelihoodcoef = self.nsegs * np.log(70.0 / self.rhohatmax ** 4)
+        """Additional constant terms to turn a detection statistic into a likelihood.
+
+        See MCMCSearch._set_likelihoodcoef for the base implementation.
+        This method simply extends it in order to account for the increased number
+        of segments a semicoherent search works with.
+        """
+        super()._set_likelihoodcoef()
+        self.likelihoodcoef *= self.nsegs
 
     def _get_data_dictionary_to_save(self):
         d = dict(
             nsteps=self.nsteps,
             nwalkers=self.nwalkers,
             ntemps=self.ntemps,
             theta_keys=self.theta_keys,
@@ -2660,15 +2903,15 @@
             nsegs=self.nsegs,
             minStartTime=self.minStartTime,
             maxStartTime=self.maxStartTime,
         )
         return d
 
     def _initiate_search_object(self):
-        logging.info("Setting up search object")
+        logger.info("Setting up search object")
         search_ranges = self._get_search_ranges()
         self.search = core.SemiCoherentSearch(
             label=self.label,
             outdir=self.outdir,
             tref=self.tref,
             nsegs=self.nsegs,
             sftfilepattern=self.sftfilepattern,
@@ -2680,105 +2923,39 @@
             maxCoverFreq=self.maxCoverFreq,
             search_ranges=search_ranges,
             detectors=self.detectors,
             injectSources=self.injectSources,
             assumeSqrtSX=self.assumeSqrtSX,
             earth_ephem=self.earth_ephem,
             sun_ephem=self.sun_ephem,
+            allowedMismatchFromSFTLength=self.allowedMismatchFromSFTLength,
         )
         if self.minStartTime is None:
             self.minStartTime = self.search.minStartTime
         if self.maxStartTime is None:
             self.maxStartTime = self.search.maxStartTime
 
-    def logp(self, theta_vals, theta_prior, theta_keys, search):
+    def _logp(self, theta_vals, theta_prior, theta_keys, search):
         H = [
             self._generic_lnprior(**theta_prior[key])(p)
             for p, key in zip(theta_vals, theta_keys)
         ]
         return np.sum(H)
 
-    def logl(self, theta, search):
-        for j, theta_i in enumerate(self.theta_idxs):
-            self.fixed_theta[theta_i] = theta[j]
-        twoF = search.get_semicoherent_det_stat(*self.fixed_theta)
-        return twoF / 2.0 + self.likelihoodcoef
-
-
-class MCMCFollowUpSearch(MCMCSemiCoherentSearch):
-    """A follow up procudure increasing the coherence time in a zoom
-
-    Parameters
-    ----------
-    theta_prior: dict
-        Dictionary of priors and fixed values for the search parameters.
-        For each parameters (key of the dict), if it is to be held fixed
-        the value should be the constant float, if it is be searched, the
-        value should be a dictionary of the prior.
-    tref, minStartTime, maxStartTime: int
-        GPS seconds of the reference time, start time and end time. While tref
-        is requirede, minStartTime and maxStartTime default to None in which
-        case all available data is used.
-    label, outdir: str
-        A label and output directory (optional, defaults is `'data'`) to
-        name files
-    sftfilepattern: str, optional
-        Pattern to match SFTs using wildcards (*?) and ranges [0-9];
-        mutiple patterns can be given separated by colons.
-    detectors: str, optional
-        Two character reference to the detectors to use, specify None for no
-        contraint and comma separate for multiple references.
-    nsteps: list (2,), optional
-        Number of burn-in and production steps to take, [nburn, nprod]. See
-        `pyfstat.MCMCSearch.setup_initialisation()` for details on adding
-        initialisation steps.
-    nwalkers, ntemps: int, optional
-        The number of walkers and temperates to use in the parallel
-        tempered PTSampler.
-    log10beta_min float < 0, optional
-        The  log_10(beta) value, if given the set of betas passed to PTSampler
-        are generated from `np.logspace(0, log10beta_min, ntemps)` (given
-        in descending order to ptemcee).
-    theta_initial: dict, array, optional
-        A dictionary of distribution about which to distribute the
-        initial walkers about
-    rhohatmax: float, optional
-        Upper bound for the SNR scale parameter (required to normalise the
-        Bayes factor) - this needs to be carefully set when using the
-        evidence.
-    binary: bool, optional
-        If true, search over binary parameters
-    BSGL: bool, optional
-        If true, use the BSGL statistic
-    SSBPrec: int, optional
-        SSBPrec (SSB precision) to use when calling ComputeFstat
-    RngMedWindow: int, optional
-        Running-Median window size (number of bins) for ComputeFstat
-    minCoverFreq, maxCoverFreq: float, optional
-        Minimum and maximum instantaneous frequency which will be covered
-        over the SFT time span as passed to CreateFstatInput
-    injectSources: dict, optional
-        If given, inject these properties into the SFT files before running
-        the search
-    assumeSqrtSX: float, optional
-        Don't estimate noise-floors, but assume (stationary) per-IFO sqrt{SX}
-
-    Attributes
-    ----------
-    symbol_dictionary: dict
-        Key, val pairs of the parameters (i.e. `F0`, `F1`), to Latex math
-        symbols for plots
-    unit_dictionary: dict
-        Key, val pairs of the parameters (i.e. `F0`, `F1`), and the
-        units (i.e. `Hz`)
-    transform_dictionary: dict
-        Key, val pairs of the parameters (i.e. `F0`, `F1`), where the key is
-        itself a dictionary which can item `multiplier`, `subtractor`, or
-        `unit` by which to transform by and update the units.
 
+class MCMCFollowUpSearch(MCMCSemiCoherentSearch, core.DeprecatedClass):
+    """Hierarchical follow-up procedure
+
+    Executes MCMC runs with increasing coherence times in order to follow up a parameter space
+    region. The main idea is to use an MCMC run to identify an interesting parameter space region
+    to then zoom-in said region using a finer "effective resolution" by increasing the coherence time.
+    See Ashton & Prix (PRD 97, 103020, 2018): https://arxiv.org/abs/1802.05450
+
+    See MCMCSemiCoherentSearch for a list of additional parameters, here we list only the additional
+    init parameters of this class.
     """
 
     def __init__(
         self,
         theta_prior,
         tref,
         label,
@@ -2799,16 +2976,17 @@
         RngMedWindow=None,
         minCoverFreq=None,
         maxCoverFreq=None,
         injectSources=None,
         assumeSqrtSX=None,
         earth_ephem=None,
         sun_ephem=None,
+        allowedMismatchFromSFTLength=None,
+        clean=False,
     ):
-
         self._set_init_params_dict(locals())
         self.theta_prior = theta_prior
         self.tref = tref
         self.label = label
         self.outdir = outdir
         self.minStartTime = minStartTime
         self.maxStartTime = maxStartTime
@@ -2826,40 +3004,40 @@
         self.RngMedWindow = RngMedWindow
         self.minCoverFreq = minCoverFreq
         self.maxCoverFreq = maxCoverFreq
         self.injectSources = injectSources
         self.assumeSqrtSX = assumeSqrtSX
         self.nsegs = None
         self.set_ephemeris_files(earth_ephem, sun_ephem)
+        self.allowedMismatchFromSFTLength = allowedMismatchFromSFTLength
+        self.clean = clean
 
-        if os.path.isdir(outdir) is False:
-            os.mkdir(outdir)
+        os.makedirs(outdir, exist_ok=True)
         self.output_file_header = self.get_output_file_header()
-        self._add_log_file(self.output_file_header)
-        logging.info(
+        logger.info(
             ("Set-up MCMC semi-coherent search for model {} on data" "{}").format(
                 self.label, self.sftfilepattern
             )
         )
         self.pickle_path = os.path.join(self.outdir, self.label + "_saved_data.p")
         self._unpack_input_theta()
         self.ndim = len(self.theta_keys)
         if self.log10beta_min:
             self.betas = np.logspace(0, self.log10beta_min, self.ntemps)
         else:
             self.betas = None
-        if args.clean and os.path.isfile(self.pickle_path):
+        if self.clean and os.path.isfile(self.pickle_path):
             os.rename(self.pickle_path, self.pickle_path + ".old")
 
         self._log_input()
 
         if self.nsegs:
             self._set_likelihoodcoef()
         else:
-            logging.info("Value `nsegs` not yet provided")
+            logger.info("Value `nsegs` not yet provided")
 
     def _get_data_dictionary_to_save(self):
         d = dict(
             nwalkers=self.nwalkers,
             ntemps=self.ntemps,
             theta_keys=self.theta_keys,
             theta_prior=self.theta_prior,
@@ -2867,94 +3045,231 @@
             BSGL=self.BSGL,
             minStartTime=self.minStartTime,
             maxStartTime=self.maxStartTime,
             run_setup=self.run_setup,
         )
         return d
 
-    def update_search_object(self):
-        logging.info("Update search object")
-        self.search.init_computefstatistic()
+    def run(
+        self,
+        run_setup=None,
+        proposal_scale_factor=2,
+        NstarMax=10,
+        Nsegs0=None,
+        save_pickle=True,
+        export_samples=True,
+        save_loudest=True,
+        plot_walkers=True,
+        walker_plot_args=None,
+        log_table=True,
+        gen_tex_table=True,
+        window=50,
+    ):
+        """Run the follow-up with the given run_setup.
 
-    def get_width_from_prior(self, prior, key):
-        if prior[key]["type"] == "unif":
-            return prior[key]["upper"] - prior[key]["lower"]
-
-    def get_mid_from_prior(self, prior, key):
-        if prior[key]["type"] == "unif":
-            return 0.5 * (prior[key]["upper"] + prior[key]["lower"])
+        See MCMCSearch.run's docstring for a description of the remainder arguments.
 
-    def read_setup_input_file(self, run_setup_input_file):
-        with open(run_setup_input_file, "rb+") as f:
-            d = pickle.load(f)
-        return d
+        Parameters
+        ----------
+        run_setup, log_table, gen_tex_table:
+            See `MCMCFollowUpSearch.init_run_setup`.
+        NstarMax, Nsegs0:
+            See `pyfstat.optimal_setup_functions.get_optimal_setup`.
+        """
 
-    def write_setup_input_file(
-        self,
-        run_setup_input_file,
-        NstarMax,
-        Nsegs0,
-        nsegs_vals,
-        Nstar_vals,
-        theta_prior,
-    ):
-        d = dict(
+        self.nsegs = 1
+        self._set_likelihoodcoef()
+        self._initiate_search_object()
+        run_setup = self.init_run_setup(
+            run_setup,
             NstarMax=NstarMax,
             Nsegs0=Nsegs0,
-            nsegs_vals=nsegs_vals,
-            theta_prior=theta_prior,
-            Nstar_vals=Nstar_vals,
+            log_table=log_table,
+            gen_tex_table=gen_tex_table,
         )
-        with open(run_setup_input_file, "wb+") as f:
-            pickle.dump(d, f)
+        self.run_setup = run_setup
+        self._estimate_run_time()
 
-    def check_old_run_setup(self, old_setup, **kwargs):
-        try:
-            truths = [val == old_setup[key] for key, val in kwargs.items()]
-            if all(truths):
-                return True
+        walker_plot_args = walker_plot_args or {}
+
+        self.old_data_is_okay_to_use = self._check_old_data_is_okay_to_use()
+        if self.old_data_is_okay_to_use is True:
+            logger.warning("Using saved data from {}".format(self.pickle_path))
+            d = self.get_saved_data_dictionary()
+            self.samples = d["samples"]
+            self.lnprobs = d["lnprobs"]
+            self.lnlikes = d["lnlikes"]
+            self.all_lnlikelihood = d["all_lnlikelihood"]
+            self.chain = d["chain"]
+            self.nsegs = run_setup[-1][1]
+            return
+
+        nsteps_total = 0
+        for j, ((nburn, nprod), nseg, reset_p0) in enumerate(run_setup):
+            p0 = self._get_p0_per_stage(reset_p0)
+
+            self.nsegs = nseg
+            self._set_likelihoodcoef()
+            self.search.nsegs = nseg
+            self._update_search_object()
+            self.search.init_semicoherent_parameters()
+            self.sampler = PTSampler(
+                ntemps=self.ntemps,
+                nwalkers=self.nwalkers,
+                dim=self.ndim,
+                logl=self._logl,
+                logp=self._logp,
+                logpargs=(self.theta_prior, self.theta_keys, self.search),
+                loglargs=(self.search,),
+                betas=self.betas,
+                a=proposal_scale_factor,
+            )
+
+            Tcoh = (self.maxStartTime - self.minStartTime) / nseg / 86400.0
+            logger.info(
+                (
+                    "Running {}/{} with {} steps and {} nsegs " "(Tcoh={:1.2f} days)"
+                ).format(j + 1, len(run_setup), (nburn, nprod), nseg, Tcoh)
+            )
+            self._run_sampler(p0, nburn=nburn, nprod=nprod, window=window)
+            logger.info(
+                "Max detection statistic of run was {}".format(
+                    np.max(self.sampler.loglikelihood)
+                )
+            )
+
+            if plot_walkers:
+                try:
+                    walkers_fig, walkers_axes = self._plot_walkers(
+                        nprod=nprod, xoffset=nsteps_total, **walker_plot_args
+                    )
+                    for ax in walkers_axes[: self.ndim]:
+                        ax.axvline(nsteps_total, color="k", ls="--", lw=0.25)
+                except Exception as e:
+                    logger.warning("Failed to plot walkers due to Error {}".format(e))
+
+            nsteps_total += nburn + nprod
+
+        if plot_walkers:
+            nstep_list = np.array(
+                [el[0][0] for el in run_setup] + [run_setup[-1][0][1]]
+            )
+            mids = np.cumsum(nstep_list) - nstep_list / 2
+            mid_labels = ["{:1.0f}".format(i) for i in np.arange(0, len(mids) - 1)]
+            mid_labels += ["Production"]
+            for ax in walkers_axes[: self.ndim]:
+                axy = ax.twiny()
+                axy.tick_params(pad=-10, direction="in", axis="x", which="major")
+                axy.minorticks_off()
+                axy.set_xlim(ax.get_xlim())
+                axy.set_xticks(mids)
+                axy.set_xticklabels(mid_labels)
+
+        samples = self.sampler.chain[0, :, nburn:, :].reshape((-1, self.ndim))
+        lnprobs = self.sampler.logprobability[0, :, nburn:].reshape((-1))
+        lnlikes = self.sampler.loglikelihood[0, :, nburn:].reshape((-1))
+        all_lnlikelihood = self.sampler.loglikelihood
+        self.samples = samples
+        self.lnprobs = lnprobs
+        self.lnlikes = lnlikes
+        self.all_lnlikelihood = all_lnlikelihood
+        if save_pickle:
+            self._pickle_data(samples, lnprobs, lnlikes, all_lnlikelihood)
+        if export_samples:
+            self.export_samples_to_disk()
+        if save_loudest:
+            self.generate_loudest()
+
+        if plot_walkers:
+            try:
+                walkers_fig.tight_layout()
+            except Exception as e:
+                logger.warning(
+                    "Failed to set tight layout for walkers plot due to Error {}".format(
+                        e
+                    )
+                )
+            if (walker_plot_args.get("fig") is not None) and (
+                walker_plot_args.get("axes") is not None
+            ):
+                self.walkers_fig = walkers_fig
+                self.walkers_axes = walkers_axes
             else:
-                logging.info("Old setup doesn't match one of NstarMax, Nsegs0 or prior")
-        except KeyError as e:
-            logging.info("Error found when comparing with old setup: {}".format(e))
-            return False
+                try:
+                    walkers_fig.savefig(
+                        os.path.join(self.outdir, self.label + "_walkers.png")
+                    )
+                    plt.close(walkers_fig)
+                except Exception as e:
+                    logger.warning(
+                        "Failed to save walker plots due to Error {}".format(e)
+                    )
+
+    def _update_search_object(self):
+        logger.info("Update search object")
+        self.search.init_computefstatistic()
 
     def init_run_setup(
         self,
         run_setup=None,
         NstarMax=1000,
         Nsegs0=None,
         log_table=True,
         gen_tex_table=True,
+        setup_only=False,
+        no_template_counting=True,
     ):
+        """
+        Initialize the setup of the follow-up run computing the required quantities fro, NstarMax
+        and Nsegs0.
+
+        Parameters
+        ----------
+        NstarMax, Nsegs0: int
+            Required parameters to create a new follow-up setup.
+            See `pyfstat.optimal_setup_functions.get_optimal_setup`.
+        run_setup: optional
+            If None, a new setup will be created from NstarMax and Nsegs0.
+            Use `MCMCFollowUpSearch.read_setup_input_file` to read a previous
+            setup file.
+        log_table: bool
+            Log follow-up setup using `logger.info` as a table.
+        gen_tex_table: bool
+            Dump follow-up setup into a text file as a tex table.
+            File is constructed as `os.path.join(self.outdir, self.label + "_run_setup.tex")`.
 
+        Returns
+        -------
+        run_setup: list
+           List containing the setup of the follow-up run.
+        """
         if run_setup is None and Nsegs0 is None:
             raise ValueError(
                 "You must either specify the run_setup, or Nsegs0 and NStarMax"
                 " from which the optimal run_setup can be estimated"
             )
         if run_setup is None:
-            logging.info("No run_setup provided")
+            logger.info("No run_setup provided")
 
             run_setup_input_file = os.path.join(
                 self.outdir, self.label + "_run_setup.p"
             )
 
             if os.path.isfile(run_setup_input_file):
-                logging.info(
+                logger.info(
                     "Checking old setup input file {}".format(run_setup_input_file)
                 )
                 old_setup = self.read_setup_input_file(run_setup_input_file)
-                if self.check_old_run_setup(
+                if self._check_old_run_setup(
                     old_setup,
                     NstarMax=NstarMax,
                     Nsegs0=Nsegs0,
                     theta_prior=self.theta_prior,
                 ):
-                    logging.info(
+                    logger.info(
                         "Using old setup with NstarMax={}, Nsegs0={}".format(
                             NstarMax, Nsegs0
                         )
                     )
                     nsegs_vals = old_setup["nsegs_vals"]
                     Nstar_vals = old_setup["Nstar_vals"]
                     generate_setup = False
@@ -2969,62 +3284,62 @@
                     Nsegs0,
                     self.tref,
                     self.minStartTime,
                     self.maxStartTime,
                     self.theta_prior,
                     self.search.detector_names,
                 )
-                self.write_setup_input_file(
+                self._write_setup_input_file(
                     run_setup_input_file,
                     NstarMax,
                     Nsegs0,
                     nsegs_vals,
                     Nstar_vals,
                     self.theta_prior,
                 )
 
             run_setup = [
                 ((self.nsteps[0], 0), nsegs, False) for nsegs in nsegs_vals[:-1]
             ]
             run_setup.append(((self.nsteps[0], self.nsteps[1]), nsegs_vals[-1], False))
 
         else:
-            logging.info("Calculating the number of templates for this setup")
+            logger.info("Calculating the number of templates for this setup")
             Nstar_vals = []
             for i, rs in enumerate(run_setup):
                 rs = list(rs)
                 if len(rs) == 2:
                     rs.append(False)
                 if np.shape(rs[0]) == ():
                     rs[0] = (rs[0], 0)
                 run_setup[i] = rs
 
-                if args.no_template_counting:
+                if no_template_counting:
                     Nstar_vals.append([1, 1, 1])
                 else:
                     Nstar = optimal_setup_functions.get_Nstar_estimate(
                         rs[1],
                         self.tref,
                         self.minStartTime,
                         self.maxStartTime,
                         self.theta_prior,
                         self.search.detector_names,
                     )
                     Nstar_vals.append(Nstar)
 
         if log_table:
-            logging.info("Using run-setup as follows:")
-            logging.info("Stage | nburn | nprod | nsegs | Tcoh d | resetp0 | Nstar")
+            logger.info("Using run-setup as follows:")
+            logger.info("Stage | nburn | nprod | nsegs | Tcoh d | resetp0 | Nstar")
             for i, rs in enumerate(run_setup):
                 Tcoh = (self.maxStartTime - self.minStartTime) / rs[1] / 86400
                 if Nstar_vals[i] is None:
                     vtext = "N/A"
                 else:
                     vtext = "{:0.3e}".format(int(Nstar_vals[i]))
-                logging.info(
+                logger.info(
                     "{} | {} | {} | {} | {} | {} | {}".format(
                         str(i).ljust(5),
                         str(rs[0][0]).ljust(5),
                         str(rs[0][1]).ljust(5),
                         str(rs[1]).ljust(5),
                         "{:6.1f}".format(Tcoh),
                         str(rs[2]).ljust(7),
@@ -3049,317 +3364,203 @@
                         Nstar = "N/A"
                     else:
                         Nstar = Nstar_vals[i]
                     line = line.format(
                         i,
                         rs[1],
                         "{:1.1f}".format(Tcoh),
-                        helper_functions.texify_float(Nstar),
+                        utils.texify_float(Nstar),
                     )
                     f.write(line)
                 f.write(r"\end{tabular}" + "\n")
 
-        if args.setup_only:
-            logging.info("Exit as requested by setup_only flag")
+        if setup_only:
+            logger.info("Exit as requested by setup_only flag")
             sys.exit()
         else:
             return run_setup
 
+    def read_setup_input_file(self, run_setup_input_file):
+        with open(run_setup_input_file, "rb+") as f:
+            d = pickle.load(f)
+        return d
+
+    def _write_setup_input_file(
+        self,
+        run_setup_input_file,
+        NstarMax,
+        Nsegs0,
+        nsegs_vals,
+        Nstar_vals,
+        theta_prior,
+    ):
+        d = dict(
+            NstarMax=NstarMax,
+            Nsegs0=Nsegs0,
+            nsegs_vals=nsegs_vals,
+            theta_prior=theta_prior,
+            Nstar_vals=Nstar_vals,
+        )
+        with open(run_setup_input_file, "wb+") as f:
+            pickle.dump(d, f)
+
+    def _check_old_run_setup(self, old_setup, **kwargs):
+        try:
+            truths = [val == old_setup[key] for key, val in kwargs.items()]
+            if all(truths):
+                return True
+            else:
+                logger.info("Old setup doesn't match one of NstarMax, Nsegs0 or prior")
+        except KeyError as e:
+            logger.info("Error found when comparing with old setup: {}".format(e))
+            return False
+
     def _get_p0_per_stage(self, reset_p0=False):
         """Returns new initial positions for walkers at each stage of the ladder"""
         if not hasattr(self, "sampler"):  # must be stage 0
             p0 = self._generate_initial_p0()
             p0 = self._apply_corrections_to_p0(p0)
         elif reset_p0:
             p0 = self._get_new_p0(self.sampler)
             p0 = self._apply_corrections_to_p0(p0)
             # self._check_initial_points(p0)
         else:
             p0 = self.sampler.chain[:, :, -1, :]
         return p0
 
-    def run(
-        self,
-        run_setup=None,
-        proposal_scale_factor=2,
-        NstarMax=10,
-        Nsegs0=None,
-        save_pickle=True,
-        export_samples=True,
-        save_loudest=True,
-        plot_walkers=True,
-        walker_plot_args=None,
-        log_table=True,
-        gen_tex_table=True,
-        window=50,
-    ):
-        """Run the follow-up with the given run_setup
-
-        Parameters
-        ----------
-        run_setup: list of tuples, optional
-        proposal_scale_factor: float
-            The proposal scale factor used by the sampler, see Goodman & Weare
-            (2010). If the acceptance fraction is too low, you can raise it by
-            decreasing the a parameter; and if it is too high, you can reduce
-            it by increasing the a parameter [Foreman-Mackay (2013)].
-        save_pickle: bool
-            If true, save a pickle file of the full sampler state.
-        export_samples: bool
-            If true, save ASCII samples file to disk.
-        save_loudest: bool
-            If true, save a CFSv2 .loudest file to disk.
-        plot_walkers: bool
-            If true, save trace plots of the walkers.
-        walker_plot_args:
-            Dictionary passed as kwargs to _plot_walkers to control the plotting.
-            Also, if both "fig" and "axes" entries are set,
-            the plot is not saved to disk directly,
-            but .walker_fig and .walker_axes properties are returned.
-        window: int
-            The minimum number of autocorrelation times needed to trust the
-            result when estimating the autocorrelation time (see
-            ptemcee.Sampler.get_autocorr_time for further details.
-        **kwargs:
-            Passed to _plot_walkers to control the figures
-
-        """
-
-        self.nsegs = 1
-        self._set_likelihoodcoef()
-        self._initiate_search_object()
-        run_setup = self.init_run_setup(
-            run_setup,
-            NstarMax=NstarMax,
-            Nsegs0=Nsegs0,
-            log_table=log_table,
-            gen_tex_table=gen_tex_table,
-        )
-        self.run_setup = run_setup
-        self._estimate_run_time()
-
-        walker_plot_args = walker_plot_args or {}
-
-        self.old_data_is_okay_to_use = self._check_old_data_is_okay_to_use()
-        if self.old_data_is_okay_to_use is True:
-            logging.warning("Using saved data from {}".format(self.pickle_path))
-            d = self.get_saved_data_dictionary()
-            self.samples = d["samples"]
-            self.lnprobs = d["lnprobs"]
-            self.lnlikes = d["lnlikes"]
-            self.all_lnlikelihood = d["all_lnlikelihood"]
-            self.chain = d["chain"]
-            self.nsegs = run_setup[-1][1]
-            return
-
-        nsteps_total = 0
-        for j, ((nburn, nprod), nseg, reset_p0) in enumerate(run_setup):
-            p0 = self._get_p0_per_stage(reset_p0)
-
-            self.nsegs = nseg
-            self._set_likelihoodcoef()
-            self.search.nsegs = nseg
-            self.update_search_object()
-            self.search.init_semicoherent_parameters()
-            self.sampler = PTSampler(
-                ntemps=self.ntemps,
-                nwalkers=self.nwalkers,
-                dim=self.ndim,
-                logl=self.logl,
-                logp=self.logp,
-                logpargs=(self.theta_prior, self.theta_keys, self.search),
-                loglargs=(self.search,),
-                betas=self.betas,
-                a=proposal_scale_factor,
-            )
-
-            Tcoh = (self.maxStartTime - self.minStartTime) / nseg / 86400.0
-            logging.info(
-                (
-                    "Running {}/{} with {} steps and {} nsegs " "(Tcoh={:1.2f} days)"
-                ).format(j + 1, len(run_setup), (nburn, nprod), nseg, Tcoh)
-            )
-            self._run_sampler(p0, nburn=nburn, nprod=nprod, window=window)
-            logging.info(
-                "Max detection statistic of run was {}".format(
-                    np.max(self.sampler.loglikelihood)
-                )
-            )
-
-            if plot_walkers:
-                try:
-                    walkers_fig, walkers_axes = self._plot_walkers(
-                        nprod=nprod, xoffset=nsteps_total, **walker_plot_args
-                    )
-                    for ax in walkers_axes[: self.ndim]:
-                        ax.axvline(nsteps_total, color="k", ls="--", lw=0.25)
-                except Exception as e:
-                    logging.warning("Failed to plot walkers due to Error {}".format(e))
-
-            nsteps_total += nburn + nprod
-
-        if plot_walkers:
-            nstep_list = np.array(
-                [el[0][0] for el in run_setup] + [run_setup[-1][0][1]]
-            )
-            mids = np.cumsum(nstep_list) - nstep_list / 2
-            mid_labels = ["{:1.0f}".format(i) for i in np.arange(0, len(mids) - 1)]
-            mid_labels += ["Production"]
-            for ax in walkers_axes[: self.ndim]:
-                axy = ax.twiny()
-                axy.tick_params(pad=-10, direction="in", axis="x", which="major")
-                axy.minorticks_off()
-                axy.set_xlim(ax.get_xlim())
-                axy.set_xticks(mids)
-                axy.set_xticklabels(mid_labels)
-
-        samples = self.sampler.chain[0, :, nburn:, :].reshape((-1, self.ndim))
-        lnprobs = self.sampler.logprobability[0, :, nburn:].reshape((-1))
-        lnlikes = self.sampler.loglikelihood[0, :, nburn:].reshape((-1))
-        all_lnlikelihood = self.sampler.loglikelihood
-        self.samples = samples
-        self.lnprobs = lnprobs
-        self.lnlikes = lnlikes
-        self.all_lnlikelihood = all_lnlikelihood
-        if save_pickle:
-            self._pickle_data(samples, lnprobs, lnlikes, all_lnlikelihood)
-        if export_samples:
-            self.export_samples_to_disk()
-        if save_loudest:
-            self.generate_loudest()
-
-        if plot_walkers:
-            try:
-                walkers_fig.tight_layout()
-            except Exception as e:
-                logging.warning(
-                    "Failed to set tight layout for walkers plot due to Error {}".format(
-                        e
-                    )
-                )
-            if (walker_plot_args.get("fig") is not None) and (
-                walker_plot_args.get("axes") is not None
-            ):
-                self.walkers_fig = walkers_fig
-                self.walkers_axes = walkers_axes
-            else:
-                try:
-                    walkers_fig.savefig(
-                        os.path.join(self.outdir, self.label + "_walkers.png")
-                    )
-                    plt.close(walkers_fig)
-                except Exception as e:
-                    logging.warning(
-                        "Failed to save walker plots due to Error {}".format(e)
-                    )
-
 
 class MCMCTransientSearch(MCMCSearch):
-    """MCMC search for a transient signal using ComputeFstat
-
-    See parent MCMCSearch for a list of all additional parameters, here we list
-    only the additional init parameters of this class.
-
-    """
+    """MCMC search for a transient signal using ComputeFstat"""
 
     symbol_dictionary = dict(
         F0=r"$f$",
         F1=r"$\dot{f}$",
         F2=r"$\ddot{f}$",
         Alpha=r"$\alpha$",
         Delta=r"$\delta$",
         transient_tstart=r"$t_\mathrm{start}$",
         transient_duration=r"$\Delta T$",
     )
+    """
+        Key, val pairs of the parameters (`F0`, `F1`, ...), to LaTeX math
+        symbols for plots
+    """
     unit_dictionary = dict(
         F0=r"Hz",
         F1=r"Hz/s",
         F2=r"Hz/s$^2$",
         Alpha=r"rad",
         Delta=r"rad",
         transient_tstart=r"s",
         transient_duration=r"s",
     )
-
+    """
+        Key, val pairs of the parameters (`F0`, `F1`, ..., including glitch parameters),
+        and the units (`Hz`, `Hz/s`, ...).
+    """
     transform_dictionary = dict(
         transient_duration={
             "multiplier": 1 / 86400.0,
             "unit": "day",
             "symbol": "Transient duration",
         },
         transient_tstart={
             "multiplier": 1 / 86400.0,
             "subtractor": "minStartTime",
             "unit": "day",
             "label": "Transient start-time \n days after minStartTime",
         },
     )
+    """
+        Key, val pairs of the parameters (`F0`, `F1`, ...), where the key is
+        itself a dictionary which can item `multiplier`, `subtractor`, or
+        `unit` by which to transform by and update the units.
+    """
 
     def _initiate_search_object(self):
-        logging.info("Setting up search object")
+        logger.info("Setting up search object")
         if not self.transientWindowType:
             self.transientWindowType = "rect"
         search_ranges = self._get_search_ranges()
         self.search = core.ComputeFstat(
             tref=self.tref,
             sftfilepattern=self.sftfilepattern,
             minCoverFreq=self.minCoverFreq,
             maxCoverFreq=self.maxCoverFreq,
             search_ranges=search_ranges,
             detectors=self.detectors,
             transientWindowType=self.transientWindowType,
             minStartTime=self.minStartTime,
             maxStartTime=self.maxStartTime,
             BSGL=self.BSGL,
+            BtSG=self.BtSG,
             binary=self.binary,
             injectSources=self.injectSources,
             tCWFstatMapVersion=self.tCWFstatMapVersion,
             earth_ephem=self.earth_ephem,
             sun_ephem=self.sun_ephem,
+            allowedMismatchFromSFTLength=self.allowedMismatchFromSFTLength,
         )
         if self.minStartTime is None:
             self.minStartTime = self.search.minStartTime
         if self.maxStartTime is None:
             self.maxStartTime = self.search.maxStartTime
 
-    def logl(self, theta, search):
-        for j, theta_i in enumerate(self.theta_idxs):
-            self.fixed_theta[theta_i] = theta[j]
-        in_theta = copy.copy(self.fixed_theta)
-        in_theta[1] = in_theta[0] + in_theta[1]
-        if in_theta[1] > self.maxStartTime:
+    def _set_point_for_evaluation(self, theta):
+        """Combines fixed and variable parameters to form a valid evaluation point.
+
+        Parameters
+        ----------
+        theta: list or np.ndarray
+            The sampled (variable) parameters.
+        Returns
+        -------
+        p: dict
+            The full parameter space point as a dictionary.
+            (different from base MCMCSearch class!)
+        """
+        p = {
+            key: self.fixed_theta[k]
+            for k, key in enumerate(self.full_theta_keys)
+            if "transient" not in key
+        }
+        p.update(
+            {
+                key: theta[k]
+                for k, key in enumerate(self.theta_keys)
+                if "transient" not in key
+            }
+        )
+        # FIXME: this can be simplified when changing all theta lists to dicts
+        if "transient_tstart" in self.theta_keys:
+            p["tstart"] = theta[self.theta_keys.index("transient_tstart")]
+        else:
+            p["tstart"] = self.fixed_theta[
+                self.full_theta_keys.index("transient_tstart")
+            ]
+        if "transient_duration" in self.theta_keys:
+            tau = theta[self.theta_keys.index("transient_duration")]
+        else:
+            tau = self.fixed_theta[self.full_theta_keys.index("transient_duration")]
+        p["tend"] = p["tstart"] + tau
+        return p
+
+    def _logl(self, theta, search):
+        in_theta = self._set_point_for_evaluation(theta)
+        if in_theta["tend"] > self.maxStartTime:
             return -np.inf
-        twoF = search.get_fullycoherent_twoF(*in_theta)
-        return twoF / 2.0 + self.likelihoodcoef
+        detstat = search.get_det_stat(**in_theta)
+        return detstat * self.likelihooddetstatmultiplier + self.likelihoodcoef
 
     def _unpack_input_theta(self):
-        full_theta_keys = [
-            "transient_tstart",
-            "transient_duration",
-            "F0",
-            "F1",
-            "F2",
-            "Alpha",
-            "Delta",
-        ]
+        self.full_theta_keys = ["F0", "F1", "F2", "Alpha", "Delta"]
         if self.binary:
-            full_theta_keys += ["asini", "period", "ecc", "tp", "argp"]
-        full_theta_keys_copy = copy.copy(full_theta_keys)
-
-        full_theta_symbols = [
-            r"$t_{\rm start}$",
-            r"$\Delta T$",
-            r"$f$",
-            r"$\dot{f}$",
-            r"$\ddot{f}$",
-            r"$\alpha$",
-            r"$\delta$",
-        ]
-        if self.binary:
-            full_theta_symbols += ["asini", "period", "period", "ecc", "tp", "argp"]
+            self.full_theta_keys += ["asini", "period", "ecc", "tp", "argp"]
+        self.full_theta_keys += ["transient_tstart", "transient_duration"]
+        full_theta_keys_copy = copy.copy(self.full_theta_keys)
 
         self.theta_keys = []
         fixed_theta_dict = {}
         for key, val in self.theta_prior.items():
             if type(val) is dict:
                 fixed_theta_dict[key] = 0
                 self.theta_keys.append(key)
@@ -3374,25 +3575,31 @@
         if len(full_theta_keys_copy) > 0:
             raise ValueError(
                 ("Input dictionary `theta` is missing the" "following keys: {}").format(
                     full_theta_keys_copy
                 )
             )
 
-        self.fixed_theta = [fixed_theta_dict[key] for key in full_theta_keys]
-        self.theta_idxs = [full_theta_keys.index(k) for k in self.theta_keys]
-        self.theta_symbols = [full_theta_symbols[i] for i in self.theta_idxs]
+        self.fixed_theta = [fixed_theta_dict[key] for key in self.full_theta_keys]
+        self.theta_idxs = [self.full_theta_keys.index(k) for k in self.theta_keys]
+        self.theta_symbols = [self.symbol_dictionary[k] for k in self.theta_keys]
 
         idxs = np.argsort(self.theta_idxs)
         self.theta_idxs = [self.theta_idxs[i] for i in idxs]
         self.theta_symbols = [self.theta_symbols[i] for i in idxs]
         self.theta_keys = [self.theta_keys[i] for i in idxs]
 
-    def get_savetxt_fmt(self):
-        fmt = []
+        self.output_keys = self.theta_keys.copy()
+        self.output_keys.append("twoF")
+        if self.BSGL:
+            self.output_keys.append("log10BSGL")
+
+    def _get_savetxt_fmt_dict(self):
+        fmt_dict = utils.get_doppler_params_output_format(self.theta_keys)
         if "transient_tstart" in self.theta_keys:
-            fmt += ["%d"]
+            fmt_dict["transient_tstart"] = "%d"
         if "transient_duration" in self.theta_keys:
-            fmt += ["%d"]
-        fmt += helper_functions.get_doppler_params_output_format(self.theta_keys)
-        fmt += ["%.9g"]  # for detection statistic
-        return fmt
+            fmt_dict["transient_duration"] = "%d"
+        fmt_dict["twoF"] = "%.9g"
+        if self.BSGL:
+            fmt_dict["log10BSGL"] = "%.9g"
+        return fmt_dict
```

### Comparing `PyFstat-1.9.0/pyfstat/optimal_setup_functions.py` & `PyFstat-2.0.0/pyfstat/optimal_setup_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 
 Provides functions to aid in calculating the optimal setup for zoom follow up
 
 """
 
 
 import logging
-import numpy as np
-import scipy.optimize
+
 import lal
 import lalpulsar
-import pyfstat.helper_functions as helper_functions
+import numpy as np
+import scipy.optimize
+
+import pyfstat.utils as utils
+
+logger = logging.getLogger(__name__)
 
 
 def get_optimal_setup(
     NstarMax, Nsegs0, tref, minStartTime, maxStartTime, prior, detector_names
 ):
     """Using an optimisation step, calculate the optimal setup ladder
 
@@ -44,36 +48,36 @@
     Returns
     -------
     nsegs, Nstar : list
         Ladder of segment numbers and the corresponding Nstar
 
     """
 
-    logging.info(
+    logger.info(
         "Calculating optimal setup for NstarMax={}, Nsegs0={}".format(NstarMax, Nsegs0)
     )
 
     Nstar_0 = get_Nstar_estimate(
         Nsegs0, tref, minStartTime, maxStartTime, prior, detector_names
     )
-    logging.info("Stage {}, nsegs={}, Nstar={}".format(0, Nsegs0, int(Nstar_0)))
+    logger.info("Stage {}, nsegs={}, Nstar={}".format(0, Nsegs0, int(Nstar_0)))
 
     nsegs_vals = [Nsegs0]
     Nstar_vals = [Nstar_0]
 
     i = 0
     nsegs_i = Nsegs0
     while nsegs_i > 1:
         nsegs_i, Nstar_i = _get_nsegs_ip1(
             nsegs_i, NstarMax, tref, minStartTime, maxStartTime, prior, detector_names
         )
         nsegs_vals.append(nsegs_i)
         Nstar_vals.append(Nstar_i)
         i += 1
-        logging.info("Stage {}, nsegs={}, Nstar={}".format(i, nsegs_i, int(Nstar_i)))
+        logger.info("Stage {}, nsegs={}, Nstar={}".format(i, nsegs_i, int(Nstar_i)))
 
     return nsegs_vals, Nstar_vals
 
 
 def _get_nsegs_ip1(
     nsegs_i, NstarMax, tref, minStartTime, maxStartTime, prior, detector_names
 ):
@@ -124,15 +128,15 @@
         else:
             log10Nstarip1 = np.log10(Nstarip1)
             return np.abs(log10Nstari + log10NstarMax - log10Nstarip1)
 
     res = scipy.optimize.minimize(
         f, 0.4 * nsegs_i, method="Powell", tol=1, options={"maxiter": 10}
     )
-    logging.info("{} with {} evaluations".format(res["message"], res["nfev"]))
+    logger.info("{} with {} evaluations".format(res["message"], res["nfev"]))
     nsegs_ip1 = int(res.x)
     if nsegs_ip1 == 0:
         nsegs_ip1 = 1
     if res.success:
         return (
             nsegs_ip1,
             get_Nstar_estimate(
@@ -218,20 +222,20 @@
     -------
     Nstar: int
         The estimated approximate number of templates to cover the prior
         parameter space at a mismatch of unity, assuming the normalised
         thickness is unity.
 
     """
-    earth_ephem, sun_ephem = helper_functions.get_ephemeris_files()
+    earth_ephem, sun_ephem = utils.get_ephemeris_files()
     in_phys, spindowns, sky, fiducial_freq = _extract_data_from_prior(prior)
     out_rssky = np.zeros(in_phys.shape)
 
-    in_phys = helper_functions.convert_array_to_gsl_matrix(in_phys)
-    out_rssky = helper_functions.convert_array_to_gsl_matrix(out_rssky)
+    in_phys = utils.convert_array_to_gsl_matrix(in_phys)
+    out_rssky = utils.convert_array_to_gsl_matrix(out_rssky)
 
     tboundaries = np.linspace(minStartTime, maxStartTime, nsegs + 1)
 
     ref_time = lal.LIGOTimeGPS(tref)
     segments = lal.SegListCreate()
     for j in range(len(tboundaries) - 1):
         seg = lal.SegCreate(
@@ -253,15 +257,15 @@
             fiducial_freq,
             detectors,
             detector_weights,
             detector_motion,
             ephemeris,
         )
     except RuntimeError as e:
-        logging.warning("Encountered run-time error {}".format(e))
+        logger.warning("Encountered run-time error {}".format(e))
         raise RuntimeError("Calculation of the SSkyMetric failed")
 
     if sky:
         i = 0
     else:
         i = 2
 
@@ -277,13 +281,13 @@
     parallelepiped = (d[i:, 1:].T - d[i:, 0]).T
 
     Nstars = []
     for j in range(1, len(g) + 1):
         dV = np.abs(np.linalg.det(parallelepiped[:j, :j]))
         sqrtdetG = np.sqrt(np.abs(np.linalg.det(g[:j, :j])))
         Nstars.append(sqrtdetG * dV)
-    logging.debug(
+    logger.debug(
         "Nstar for each dimension = {}".format(
             ", ".join(["{:1.1e}".format(n) for n in Nstars])
         )
     )
     return np.max(Nstars)
```

### Comparing `PyFstat-1.9.0/pyfstat/pyCUDAkernels/cudaTransientFstatExpWindow.cu` & `PyFstat-2.0.0/pyfstat/pyCUDAkernels/cudaTransientFstatExpWindow.cu`

 * *Files 11% similar despite different names*

```diff
@@ -97,29 +97,40 @@
       Fa_re += input[i*input_cols+3] * win_i; // Fa_alpha_re
       Fa_im += input[i*input_cols+4] * win_i; // Fa_alpha_im
       Fb_re += input[i*input_cols+5] * win_i; // Fb_alpha_re
       Fb_im += input[i*input_cols+6] * win_i; // Fb_alpha_im
 
     }
 
-    /* get determinant */
-    float Dd = ( Ad * Bd - Cd * Cd );
-    float DdInv = 0.0f;
-    /* safety catch as in XLALWeightMultiAMCoeffs():
-     * make it so that in the end F=0 instead of -nan
+    /* get inverse antenna pattern determinant,
+     * following safety checks from
+     * XLALComputeAntennaPatternSqrtDeterminant()
+     * and estimateAntennaPatternConditionNumber()
      */
-    if ( Dd > 0.0 ) {
-      DdInv  = 1.0 / Dd;
+    float sumAB  = Ad + Bd;
+    float diffAB = Ad - Bd;
+    float disc   = sqrt ( diffAB*diffAB + 4.0 * Cd*Cd );
+    float denom = sumAB - disc;
+    float cond = (denom > 0) ? ((sumAB + disc) / denom) : INFINITY;
+    float DdInv = 0.0f;
+    if ( cond < 1e4 ) {
+      DdInv = 1.0 / ( Ad * Bd - Cd * Cd );
     }
 
-    /* from XLALComputeFstatFromFaFb */
-    float F  = DdInv * (  Bd * ( Fa_re*Fa_re + Fa_im*Fa_im )
-                        + Ad * ( Fb_re*Fb_re + Fb_im*Fb_im )
-                        - 2.0 * Cd * ( Fa_re * Fb_re + Fa_im * Fb_im )
-                       );
+    /* matching compute_fstat_from_fa_fb
+     * including default fallback = 0.5*E[2F] in noise
+     * when DdInv == 0 due to ill-conditionness of M_munu
+     */
+    float F = 2;
+    if ( DdInv > 0 ) {
+      F  = DdInv * (   Bd * ( Fa_re*Fa_re + Fa_im*Fa_im )
+                     + Ad * ( Fb_re*Fb_re + Fb_im*Fb_im )
+                     - 2.0 * Cd * ( Fa_re * Fb_re + Fa_im * Fb_im )
+                   );
+    }
 
     /* store result in Fstat-matrix
      * at unraveled index of element {m,n}
      */
     Fmn[outidx] = F;
 
   } // ( (m < Fmn_rows) && (n < Fmn_cols) )
```

### Comparing `PyFstat-1.9.0/pyfstat/pyCUDAkernels/cudaTransientFstatRectWindow.cu` & `PyFstat-2.0.0/pyfstat/pyCUDAkernels/cudaTransientFstatRectWindow.cu`

 * *Files 10% similar despite different names*

```diff
@@ -86,29 +86,40 @@
         Fa_im += input[i*input_cols+4]; // Fa_alpha_im
         Fb_re += input[i*input_cols+5]; // Fb_alpha_re
         Fb_im += input[i*input_cols+6]; // Fb_alpha_im
         /* keep track of up to where we summed for the next iteration */
         i_t1_last = i_t1 + 1;
       }
 
-      /* get determinant */
-      float Dd = ( Ad * Bd - Cd * Cd );
-      float DdInv = 0.0f;
-      /* safety catch as in XLALWeightMultiAMCoeffs():
-       * make it so that in the end F=0 instead of -nan
+      /* get inverse antenna pattern determinant,
+       * following safety checks from
+       * XLALComputeAntennaPatternSqrtDeterminant()
+       * and estimateAntennaPatternConditionNumber()
        */
-      if ( Dd > 0.0 ) {
-        DdInv  = 1.0 / Dd;
+      float sumAB  = Ad + Bd;
+      float diffAB = Ad - Bd;
+      float disc   = sqrt ( diffAB*diffAB + 4.0 * Cd*Cd );
+      float denom = sumAB - disc;
+      float cond = (denom > 0) ? ((sumAB + disc) / denom) : INFINITY;
+      float DdInv = 0.0f;
+      if ( cond < 1e4 ) {
+        DdInv = 1.0 / ( Ad * Bd - Cd * Cd );
       }
 
-      /* from XLALComputeFstatFromFaFb */
-      float F  = DdInv * (  Bd * ( Fa_re*Fa_re + Fa_im*Fa_im )
-                          + Ad * ( Fb_re*Fb_re + Fb_im*Fb_im )
-                          - 2.0 * Cd * ( Fa_re * Fb_re + Fa_im * Fb_im )
-                         );
+      /* matching compute_fstat_from_fa_fb
+       * including default fallback = 0.5*E[2F] in noise
+       * when DdInv == 0 due to ill-conditionness of M_munu
+       */
+      float F = 2;
+      if ( DdInv > 0 ) {
+        F  = DdInv * (   Bd * ( Fa_re*Fa_re + Fa_im*Fa_im )
+                       + Ad * ( Fb_re*Fb_re + Fb_im*Fb_im )
+                       - 2.0 * Cd * ( Fa_re * Fb_re + Fa_im * Fb_im )
+                     );
+      }
 
       /* store result in Fstat-matrix
        * at unraveled index of element {m,n}
        */
       unsigned int outidx = m * N_tauRange + n;
       Fmn[outidx] = F;
```

### Comparing `PyFstat-1.9.0/versioneer.py` & `PyFstat-2.0.0/versioneer.py`

 * *Files identical despite different names*

