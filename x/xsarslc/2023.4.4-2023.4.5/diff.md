# Comparing `tmp/xsarslc-2023.4.4.tar.gz` & `tmp/xsarslc-2023.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsarslc-2023.4.4.tar", last modified: Tue Apr  4 12:07:09 2023, max compression
+gzip compressed data, was "xsarslc-2023.4.5.tar", last modified: Wed Apr  5 11:10:57 2023, max compression
```

## Comparing `xsarslc-2023.4.4.tar` & `xsarslc-2023.4.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.076468 xsarslc-2023.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.064468 xsarslc-2023.4.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.064468 xsarslc-2023.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-04 12:07:09.076468 xsarslc-2023.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.068468 xsarslc-2023.4.4/auxdata/
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/auxdata/S1B_IRs_IW3_VV.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.060468 xsarslc-2023.4.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.068468 xsarslc-2023.4.4/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.068468 xsarslc-2023.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/ATBD.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/ATBD_L1BSLC.tex
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.060468 xsarslc-2023.4.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.068468 xsarslc-2023.4.4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/_static/css/xsarslc.css
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/crossspectra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/cutoff.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.068468 xsarslc-2023.4.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/examples/default_impulseResponse_files_IW.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/examples/xspec_WV_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.072468 xsarslc-2023.4.4/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/figures/NIRAN_NRCS_VH.png
--rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/figures/NIRAN_NRCS_vv.png
--rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/figures/S1_azimuth_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/figures/S1_azimuth_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/figures/S1_range_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/figures/S1_range_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/figures/index
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/normalizedvariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/docs/sigma0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 12:07:09.076468 xsarslc-2023.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.072468 xsarslc-2023.4.4/xsarslc/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/get_config_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/get_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.076468 xsarslc-2023.4.4/xsarslc/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/processing/HR_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/processing/deramping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/processing/impulseResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/processing/interburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/processing/intraburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/processing/xspectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.076468 xsarslc-2023.4.4/xsarslc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-04-04 12:06:49.000000 xsarslc-2023.4.4/xsarslc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:07:09.072468 xsarslc-2023.4.4/xsarslc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-04 12:07:09.000000 xsarslc-2023.4.4/xsarslc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-04 12:07:09.000000 xsarslc-2023.4.4/xsarslc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:07:09.000000 xsarslc-2023.4.4/xsarslc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 12:07:09.000000 xsarslc-2023.4.4/xsarslc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-04 12:07:09.000000 xsarslc-2023.4.4/xsarslc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 12:07:09.000000 xsarslc-2023.4.4/xsarslc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.128500 xsarslc-2023.4.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.128500 xsarslc-2023.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.132500 xsarslc-2023.4.5/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VV.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.124500 xsarslc-2023.4.5/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.132500 xsarslc-2023.4.5/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.136500 xsarslc-2023.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/ATBD.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/ATBD_L1BSLC.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.124500 xsarslc-2023.4.5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.136500 xsarslc-2023.4.5/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/_static/css/xsarslc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/crossspectra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/cutoff.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.136500 xsarslc-2023.4.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/default_impulseResponse_files_IW.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/xspec_WV_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.140501 xsarslc-2023.4.5/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_VH.png
+-rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_vv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_range_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_range_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/index
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/normalizedvariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/sigma0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.140501 xsarslc-2023.4.5/xsarslc/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/get_config_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/get_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/xsarslc/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/HR_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/deramping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/impulseResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/interburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/intraburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/xspectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/xsarslc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/xsarslc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/top_level.txt
```

### Comparing `xsarslc-2023.4.4/.github/workflows/publish.yml` & `xsarslc-2023.4.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/.gitignore` & `xsarslc-2023.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/.pre-commit-config.yaml` & `xsarslc-2023.4.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/LICENSE` & `xsarslc-2023.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/PKG-INFO` & `xsarslc-2023.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.4.4
+Version: 2023.4.5
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_HH.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_HV.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_VH.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW1_VV.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW2_VH.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW2_VV.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_HH.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_HV.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_VH.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1A_IRs_IW3_VV.nc` & `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_HH.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_HV.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_VH.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW1_VV.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_HH.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_HV.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_VH.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW2_VV.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW3_VH.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/auxdata/S1B_IRs_IW3_VV.nc` & `xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/ATBD.rst` & `xsarslc-2023.4.5/docs/ATBD.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/ATBD_L1BSLC.tex` & `xsarslc-2023.4.5/docs/ATBD_L1BSLC.tex`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/Makefile` & `xsarslc-2023.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/basic_api.rst` & `xsarslc-2023.4.5/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/conf.py` & `xsarslc-2023.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/crossspectra.rst` & `xsarslc-2023.4.5/docs/crossspectra.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/cutoff.rst` & `xsarslc-2023.4.5/docs/cutoff.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/examples/default_impulseResponse_files_IW.ipynb` & `xsarslc-2023.4.5/docs/examples/default_impulseResponse_files_IW.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.4.5/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.4.5/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/examples/xspec_IW_intra_and_inter_burst.ipynb` & `xsarslc-2023.4.5/docs/examples/xspec_IW_intra_and_inter_burst.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/examples/xspec_WV_example.ipynb` & `xsarslc-2023.4.5/docs/examples/xspec_WV_example.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/figures/NIRAN_NRCS_VH.png` & `xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_VH.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/figures/NIRAN_NRCS_vv.png` & `xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_vv.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/figures/S1_azimuth_IR_IW_VV.png` & `xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/figures/S1_azimuth_IR_WV_VV.png` & `xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/figures/S1_range_IR_IW_VV.png` & `xsarslc-2023.4.5/docs/figures/S1_range_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/figures/S1_range_IR_WV_VV.png` & `xsarslc-2023.4.5/docs/figures/S1_range_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/index.rst` & `xsarslc-2023.4.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/installing.rst` & `xsarslc-2023.4.5/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/normalizedvariance.rst` & `xsarslc-2023.4.5/docs/normalizedvariance.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/oceanspectrumSAR.png` & `xsarslc-2023.4.5/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/docs/sigma0.rst` & `xsarslc-2023.4.5/docs/sigma0.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/pyproject.toml` & `xsarslc-2023.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/burst.py` & `xsarslc-2023.4.5/xsarslc/burst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/config.yml` & `xsarslc-2023.4.5/xsarslc/config.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/get_config_infos.py` & `xsarslc-2023.4.5/xsarslc/get_config_infos.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/get_test_files.py` & `xsarslc-2023.4.5/xsarslc/get_test_files.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/interface.py` & `xsarslc-2023.4.5/xsarslc/interface.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/processing/HR_tiles.py` & `xsarslc-2023.4.5/xsarslc/processing/HR_tiles.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/processing/deramping.py` & `xsarslc-2023.4.5/xsarslc/processing/deramping.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/processing/impulseResponse.py` & `xsarslc-2023.4.5/xsarslc/processing/impulseResponse.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/processing/interburst.py` & `xsarslc-2023.4.5/xsarslc/processing/interburst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/processing/intraburst.py` & `xsarslc-2023.4.5/xsarslc/processing/intraburst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/processing/xspectra.py` & `xsarslc-2023.4.5/xsarslc/processing/xspectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     if 'spatial_ref' in inter_xs:
         inter_xs = inter_xs.drop('spatial_ref')
     if isinstance(inter_xs, xr.Dataset):
         if 'multidataset' in inter_xs.attrs:
             inter_xs.attrs.update({'multidataset': str(inter_xs.multidataset)})
             # inter_xs.attrs.update({'start_date': str(inter_xs.start_date)})
             # inter_xs.attrs.update({'stop_date': str(inter_xs.stop_date)})
-        inter_xs.attrs.update({'footprint': str(inter_xs.footprint)})
+        if 'footprint' in inter_xs.attrs:
+            inter_xs.attrs.update({'footprint': str(inter_xs.footprint)})
         # inter_xs.attrs.pop('pixel_line_m')
         # inter_xs.attrs.pop('pixel_sample_m')
     if not inter_xs and not intra_xs:
         dt = None
     else:
         dt_dict = {}
         if inter_xs:
```

### Comparing `xsarslc-2023.4.4/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py` & `xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py` & `xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc/tools.py` & `xsarslc-2023.4.5/xsarslc/tools.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.4/xsarslc.egg-info/PKG-INFO` & `xsarslc-2023.4.5/xsarslc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.4.4
+Version: 2023.4.5
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.4.4/xsarslc.egg-info/SOURCES.txt` & `xsarslc-2023.4.5/xsarslc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

