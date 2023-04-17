# Comparing `tmp/PyTDC-0.3.9.tar.gz` & `tmp/PyTDC-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTDC-0.3.9.tar", last modified: Fri Jan 27 06:15:25 2023, max compression
+gzip compressed data, was "PyTDC-0.4.0.tar", last modified: Mon Apr 17 23:34:18 2023, max compression
```

## Comparing `PyTDC-0.3.9.tar` & `PyTDC-0.4.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.117985 PyTDC-0.3.9/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1069 2023-01-26 22:40:19.000000 PyTDC-0.3.9/LICENSE
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      102 2023-01-26 22:40:19.000000 PyTDC-0.3.9/MANIFEST.in
--rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-01-27 06:15:25.118085 PyTDC-0.3.9/PKG-INFO
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.109991 PyTDC-0.3.9/PyTDC.egg-info/
--rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-01-27 06:15:24.000000 PyTDC-0.3.9/PyTDC.egg-info/PKG-INFO
--rw-r--r--   0 kexinhuang   (502) staff       (20)     2170 2023-01-27 06:15:25.000000 PyTDC-0.3.9/PyTDC.egg-info/SOURCES.txt
--rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-01-27 06:15:24.000000 PyTDC-0.3.9/PyTDC.egg-info/dependency_links.txt
--rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-01-27 06:15:24.000000 PyTDC-0.3.9/PyTDC.egg-info/not-zip-safe
--rw-r--r--   0 kexinhuang   (502) staff       (20)       70 2023-01-27 06:15:25.000000 PyTDC-0.3.9/PyTDC.egg-info/requires.txt
--rw-r--r--   0 kexinhuang   (502) staff       (20)        4 2023-01-27 06:15:25.000000 PyTDC-0.3.9/PyTDC.egg-info/top_level.txt
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    17381 2023-01-26 22:40:19.000000 PyTDC-0.3.9/README.md
--rw-rw-r--   0 kexinhuang   (502) staff       (20)       70 2023-01-26 22:40:19.000000 PyTDC-0.3.9/requirements.txt
--rw-rw-r--   0 kexinhuang   (502) staff       (20)       79 2023-01-27 06:15:25.118364 PyTDC-0.3.9/setup.cfg
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1141 2023-01-26 22:40:19.000000 PyTDC-0.3.9/setup.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.110916 PyTDC-0.3.9/tdc/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      148 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     8277 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/base_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    21837 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/benchmark_deprecated.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.111584 PyTDC-0.3.9/tdc/benchmark_group/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      162 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/benchmark_group/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      449 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/benchmark_group/admet_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    10178 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/benchmark_group/base_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    15827 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/benchmark_group/docking_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      441 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/benchmark_group/drugcombo_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      453 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/benchmark_group/dti_dg_group.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.111887 PyTDC-0.3.9/tdc/chem_utils/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1021 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    13620 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/evaluator.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.112553 PyTDC-0.3.9/tdc/chem_utils/featurize/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/featurize/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    28488 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/featurize/_smartsPatts.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    23518 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/featurize/_smiles2pubchem.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    21707 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/featurize/_xyz2mol.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    27045 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/featurize/molconvert.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.113085 PyTDC-0.3.9/tdc/chem_utils/oracle/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/oracle/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1121 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/oracle/docking.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     6080 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/oracle/filter.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    59584 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/chem_utils/oracle/oracle.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    15901 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/evaluator.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.114026 PyTDC-0.3.9/tdc/generation/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      112 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3750 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/bi_generation_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     9843 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/generation_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      817 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/ligandmolgen.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      993 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/molgen.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1147 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/reaction.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     2508 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/retrosyn.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     5776 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/generation/sbdd.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    27239 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/metadata.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.115567 PyTDC-0.3.9/tdc/multi_pred/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      348 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1492 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/antibodyaff.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    13146 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/bi_pred_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1404 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/catalyst.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1985 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/ddi.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1944 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/drugres.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1239 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/drugsyn.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3034 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/dti.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1457 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/gda.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1502 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/mti.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     4028 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/multi_pred_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1545 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/peptidemhc.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     2008 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/ppi.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1253 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/tcr_epi.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1164 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/multi_pred/test_multi_pred.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    25879 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/oracles.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.115772 PyTDC-0.3.9/tdc/resource/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)       29 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/resource/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1321 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/resource/primekg.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.117000 PyTDC-0.3.9/tdc/single_pred/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      287 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     4106 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/adme.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1561 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/crispr_outcome.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     5632 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/develop.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1555 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/epitope.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1474 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/hts.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1560 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/paratope.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1588 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/qm.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     6783 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/single_pred_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1485 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/test_single_pred.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1518 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/tox.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1584 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/single_pred/yields.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     2449 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/tdc_hf.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-01-27 06:15:25.117876 PyTDC-0.3.9/tdc/utils/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1072 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     8168 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/label.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    19104 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/label_name_list.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    36203 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/load.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3398 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/misc.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3054 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/query.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3563 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/retrieve.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    12788 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/utils/split.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      535 2023-01-26 22:40:19.000000 PyTDC-0.3.9/tdc/version.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.132928 PyTDC-0.4.0/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1069 2023-04-15 16:25:42.000000 PyTDC-0.4.0/LICENSE
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      102 2023-04-15 16:25:42.000000 PyTDC-0.4.0/MANIFEST.in
+-rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-04-17 23:34:18.133002 PyTDC-0.4.0/PKG-INFO
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.125131 PyTDC-0.4.0/PyTDC.egg-info/
+-rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-04-17 23:34:17.000000 PyTDC-0.4.0/PyTDC.egg-info/PKG-INFO
+-rw-r--r--   0 kexinhuang   (502) staff       (20)     2170 2023-04-17 23:34:18.000000 PyTDC-0.4.0/PyTDC.egg-info/SOURCES.txt
+-rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-04-17 23:34:17.000000 PyTDC-0.4.0/PyTDC.egg-info/dependency_links.txt
+-rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-04-17 23:34:17.000000 PyTDC-0.4.0/PyTDC.egg-info/not-zip-safe
+-rw-r--r--   0 kexinhuang   (502) staff       (20)       98 2023-04-17 23:34:18.000000 PyTDC-0.4.0/PyTDC.egg-info/requires.txt
+-rw-r--r--   0 kexinhuang   (502) staff       (20)        4 2023-04-17 23:34:18.000000 PyTDC-0.4.0/PyTDC.egg-info/top_level.txt
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    17381 2023-04-15 16:25:42.000000 PyTDC-0.4.0/README.md
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)       98 2023-04-15 16:25:42.000000 PyTDC-0.4.0/requirements.txt
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)       79 2023-04-17 23:34:18.133275 PyTDC-0.4.0/setup.cfg
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1141 2023-04-15 16:25:42.000000 PyTDC-0.4.0/setup.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.126037 PyTDC-0.4.0/tdc/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      147 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     8277 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/base_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    21837 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_deprecated.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.126673 PyTDC-0.4.0/tdc/benchmark_group/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      162 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      449 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/admet_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    10178 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/base_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    15827 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/docking_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      441 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/drugcombo_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      453 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/dti_dg_group.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.126881 PyTDC-0.4.0/tdc/chem_utils/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1021 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    13620 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/evaluator.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.127450 PyTDC-0.4.0/tdc/chem_utils/featurize/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    28488 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/_smartsPatts.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    23693 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/_smiles2pubchem.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    21707 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/_xyz2mol.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    27045 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/molconvert.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.127860 PyTDC-0.4.0/tdc/chem_utils/oracle/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1121 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/docking.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     6080 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/filter.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    59584 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/oracle.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    15901 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/evaluator.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.128712 PyTDC-0.4.0/tdc/generation/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      112 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3750 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/bi_generation_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     9843 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/generation_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      817 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/ligandmolgen.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      993 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/molgen.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1147 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/reaction.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     2508 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/retrosyn.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     5776 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/sbdd.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    27239 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/metadata.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.130224 PyTDC-0.4.0/tdc/multi_pred/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      348 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1492 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/antibodyaff.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    13146 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/bi_pred_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1404 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/catalyst.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1985 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/ddi.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1944 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/drugres.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1239 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/drugsyn.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3034 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/dti.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1457 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/gda.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1502 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/mti.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     4028 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/multi_pred_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1545 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/peptidemhc.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     2008 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/ppi.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1253 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/tcr_epi.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1164 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/test_multi_pred.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    25879 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/oracles.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.130453 PyTDC-0.4.0/tdc/resource/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)       29 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/resource/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1321 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/resource/primekg.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.131871 PyTDC-0.4.0/tdc/single_pred/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      287 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     4106 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/adme.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1561 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/crispr_outcome.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     5632 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/develop.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1555 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/epitope.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1474 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/hts.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1560 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/paratope.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1588 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/qm.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     6783 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/single_pred_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1485 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/test_single_pred.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1518 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/tox.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1584 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/yields.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3327 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/tdc_hf.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.132826 PyTDC-0.4.0/tdc/utils/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1072 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     8168 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/label.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    19104 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/label_name_list.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    36203 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/load.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3398 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/misc.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3054 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/query.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3563 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/retrieve.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    12788 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/split.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      535 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/version.py
```

### Comparing `PyTDC-0.3.9/LICENSE` & `PyTDC-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/PKG-INFO` & `PyTDC-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.3.9
+Version: 0.4.0
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: kexinhuang@hsph.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTDC-0.3.9/PyTDC.egg-info/PKG-INFO` & `PyTDC-0.4.0/PyTDC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.3.9
+Version: 0.4.0
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: kexinhuang@hsph.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTDC-0.3.9/PyTDC.egg-info/SOURCES.txt` & `PyTDC-0.4.0/PyTDC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/README.md` & `PyTDC-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/setup.py` & `PyTDC-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/base_dataset.py` & `PyTDC-0.4.0/tdc/base_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/benchmark_deprecated.py` & `PyTDC-0.4.0/tdc/benchmark_deprecated.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/benchmark_group/base_group.py` & `PyTDC-0.4.0/tdc/benchmark_group/base_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/benchmark_group/docking_group.py` & `PyTDC-0.4.0/tdc/benchmark_group/docking_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/__init__.py` & `PyTDC-0.4.0/tdc/chem_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/evaluator.py` & `PyTDC-0.4.0/tdc/chem_utils/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/featurize/_smartsPatts.py` & `PyTDC-0.4.0/tdc/chem_utils/featurize/_smartsPatts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/featurize/_smiles2pubchem.py` & `PyTDC-0.4.0/tdc/chem_utils/featurize/_smiles2pubchem.py`

 * *Files 1% similar despite different names*

```diff
@@ -932,14 +932,20 @@
             AllBits[index2 + 115 + 148] = 1
     res2 = calcPubChemFingerPart2(mol)
     for index3, item3 in enumerate(res2):
         if item3 == 1:
             AllBits[index3 + 115] = 1
     return np.array(AllBits)
 
+def canonicalize(smiles):
+    mol = Chem.MolFromSmiles(smiles)
+    if mol is not None:
+        return Chem.MolToSmiles(mol, isomericSmiles=True)
+    else:
+        return None
 
 def smiles2pubchem(s):
     s = canonicalize(s)
     try:
         features = calcPubChemFingerAll(s)
     except:
         print(
```

### Comparing `PyTDC-0.3.9/tdc/chem_utils/featurize/_xyz2mol.py` & `PyTDC-0.4.0/tdc/chem_utils/featurize/_xyz2mol.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/featurize/molconvert.py` & `PyTDC-0.4.0/tdc/chem_utils/featurize/molconvert.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/oracle/docking.py` & `PyTDC-0.4.0/tdc/chem_utils/oracle/docking.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/oracle/filter.py` & `PyTDC-0.4.0/tdc/chem_utils/oracle/filter.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/chem_utils/oracle/oracle.py` & `PyTDC-0.4.0/tdc/chem_utils/oracle/oracle.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/evaluator.py` & `PyTDC-0.4.0/tdc/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/generation/bi_generation_dataset.py` & `PyTDC-0.4.0/tdc/generation/bi_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/generation/generation_dataset.py` & `PyTDC-0.4.0/tdc/generation/generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/generation/ligandmolgen.py` & `PyTDC-0.4.0/tdc/generation/ligandmolgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/generation/molgen.py` & `PyTDC-0.4.0/tdc/generation/molgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/generation/reaction.py` & `PyTDC-0.4.0/tdc/generation/reaction.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/generation/retrosyn.py` & `PyTDC-0.4.0/tdc/generation/retrosyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/generation/sbdd.py` & `PyTDC-0.4.0/tdc/generation/sbdd.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/metadata.py` & `PyTDC-0.4.0/tdc/metadata.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/antibodyaff.py` & `PyTDC-0.4.0/tdc/multi_pred/antibodyaff.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/bi_pred_dataset.py` & `PyTDC-0.4.0/tdc/multi_pred/bi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/catalyst.py` & `PyTDC-0.4.0/tdc/multi_pred/catalyst.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/ddi.py` & `PyTDC-0.4.0/tdc/multi_pred/ddi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/drugres.py` & `PyTDC-0.4.0/tdc/multi_pred/drugres.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/drugsyn.py` & `PyTDC-0.4.0/tdc/multi_pred/drugsyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/dti.py` & `PyTDC-0.4.0/tdc/multi_pred/dti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/gda.py` & `PyTDC-0.4.0/tdc/multi_pred/gda.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/mti.py` & `PyTDC-0.4.0/tdc/multi_pred/mti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/multi_pred_dataset.py` & `PyTDC-0.4.0/tdc/multi_pred/multi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/peptidemhc.py` & `PyTDC-0.4.0/tdc/multi_pred/peptidemhc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/ppi.py` & `PyTDC-0.4.0/tdc/multi_pred/ppi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/tcr_epi.py` & `PyTDC-0.4.0/tdc/multi_pred/tcr_epi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/multi_pred/test_multi_pred.py` & `PyTDC-0.4.0/tdc/multi_pred/test_multi_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/oracles.py` & `PyTDC-0.4.0/tdc/oracles.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/resource/primekg.py` & `PyTDC-0.4.0/tdc/resource/primekg.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/adme.py` & `PyTDC-0.4.0/tdc/single_pred/adme.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/crispr_outcome.py` & `PyTDC-0.4.0/tdc/single_pred/crispr_outcome.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/develop.py` & `PyTDC-0.4.0/tdc/single_pred/develop.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/epitope.py` & `PyTDC-0.4.0/tdc/single_pred/epitope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/hts.py` & `PyTDC-0.4.0/tdc/single_pred/hts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/paratope.py` & `PyTDC-0.4.0/tdc/single_pred/paratope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/qm.py` & `PyTDC-0.4.0/tdc/single_pred/qm.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/single_pred_dataset.py` & `PyTDC-0.4.0/tdc/single_pred/single_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/test_single_pred.py` & `PyTDC-0.4.0/tdc/single_pred/test_single_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/tox.py` & `PyTDC-0.4.0/tdc/single_pred/tox.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/single_pred/yields.py` & `PyTDC-0.4.0/tdc/single_pred/yields.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/__init__.py` & `PyTDC-0.4.0/tdc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/label.py` & `PyTDC-0.4.0/tdc/utils/label.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/label_name_list.py` & `PyTDC-0.4.0/tdc/utils/label_name_list.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/load.py` & `PyTDC-0.4.0/tdc/utils/load.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/misc.py` & `PyTDC-0.4.0/tdc/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/query.py` & `PyTDC-0.4.0/tdc/utils/query.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/retrieve.py` & `PyTDC-0.4.0/tdc/utils/retrieve.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/utils/split.py` & `PyTDC-0.4.0/tdc/utils/split.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.3.9/tdc/version.py` & `PyTDC-0.4.0/tdc/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.3.9"  # pragma: no cover
+__version__ = "0.4.0"  # pragma: no cover
```

