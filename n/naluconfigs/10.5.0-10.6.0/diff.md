# Comparing `tmp/naluconfigs-10.5.0.tar.gz` & `tmp/naluconfigs-10.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-10.5.0.tar", last modified: Thu Apr  6 19:59:39 2023, max compression
+gzip compressed data, was "naluconfigs-10.6.0.tar", last modified: Tue Apr 18 01:20:27 2023, max compression
```

## Comparing `naluconfigs-10.5.0.tar` & `naluconfigs-10.6.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.703084 naluconfigs-10.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-06 19:59:39.703084 naluconfigs-10.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 19:59:39.703084 naluconfigs-10.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.695083 naluconfigs-10.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.695083 naluconfigs-10.5.0/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.695083 naluconfigs-10.5.0/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.699083 naluconfigs-10.5.0/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.703084 naluconfigs-10.5.0/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25656 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25960 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    67433 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21959 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18598 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.695083 naluconfigs-10.5.0/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-06 19:59:39.000000 naluconfigs-10.5.0/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-06 19:59:39.000000 naluconfigs-10.5.0/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:59:39.000000 naluconfigs-10.5.0/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-06 19:59:39.000000 naluconfigs-10.5.0/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 19:59:39.000000 naluconfigs-10.5.0/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:59:39.703084 naluconfigs-10.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-06 19:59:24.000000 naluconfigs-10.5.0/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.083176 naluconfigs-10.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-18 01:20:27.083176 naluconfigs-10.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:20:27.083176 naluconfigs-10.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.075176 naluconfigs-10.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.079176 naluconfigs-10.6.0/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.075176 naluconfigs-10.6.0/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.079176 naluconfigs-10.6.0/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.083176 naluconfigs-10.6.0/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25656 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25960 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    67433 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21959 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18598 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.079176 naluconfigs-10.6.0/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-18 01:20:27.000000 naluconfigs-10.6.0/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-18 01:20:27.000000 naluconfigs-10.6.0/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:20:27.000000 naluconfigs-10.6.0/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 01:20:27.000000 naluconfigs-10.6.0/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 01:20:27.000000 naluconfigs-10.6.0/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:20:27.083176 naluconfigs-10.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-18 01:20:10.000000 naluconfigs-10.6.0/tests/test_range_keys.py
```

### Comparing `naluconfigs-10.5.0/PKG-INFO` & `naluconfigs-10.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 10.5.0
+Version: 10.6.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-10.5.0/README.md` & `naluconfigs-10.6.0/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/pyproject.toml` & `naluconfigs-10.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/setup.py` & `naluconfigs-10.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/__init__.py` & `naluconfigs-10.6.0/src/naluconfigs/__init__.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-10.6.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files 0% similar despite different names*

```diff
@@ -46,19 +46,26 @@
       2: 3
       3: 7
   headers: 3
   new_firmware: True
   numregs: 64
   pedestals_blocks: 16
   peripherals:
-    current:
+    current_1v2:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
+      r_sense: 0.05
+    current_2v5:
+      chan: 1
+      addr: 0xD0
+      bits: 16
+      gain: 8
+      r_sense: 0.05
     vadjn:
       chan: 0
       addr: 0xD8
       bits: 16
       gain: 1
     vadjp:
       chan: 1
```

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/upac96.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/upaci.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-10.6.0/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/exceptions.py` & `naluconfigs-10.6.0/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs/postprocess.py` & `naluconfigs-10.6.0/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-10.6.0/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 10.5.0
+Version: 10.6.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-10.5.0/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-10.6.0/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/tests/test_hex_addr_converter.py` & `naluconfigs-10.6.0/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/tests/test_i2c_registers.py` & `naluconfigs-10.6.0/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/tests/test_post_processing.py` & `naluconfigs-10.6.0/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.5.0/tests/test_range_keys.py` & `naluconfigs-10.6.0/tests/test_range_keys.py`

 * *Files identical despite different names*

