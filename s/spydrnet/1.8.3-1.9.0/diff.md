# Comparing `tmp/spydrnet-1.8.3.tar.gz` & `tmp/spydrnet-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spydrnet-1.8.3.tar", last modified: Tue Jul 20 16:54:02 2021, max compression
+gzip compressed data, was "dist/spydrnet-1.9.0.tar", last modified: Thu Nov 18 01:46:17 2021, max compression
```

## Comparing `spydrnet-1.8.3.tar` & `spydrnet-1.9.0.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7843 2021-07-20 16:54:02.000000 spydrnet-1.8.3/PKG-INFO
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1532 2021-07-02 19:59:19.000000 spydrnet-1.8.3/LICENSE
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet.egg-info/
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       46 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet.egg-info/requires.txt
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7843 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet.egg-info/PKG-INFO
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        1 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet.egg-info/not-zip-safe
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        9 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet.egg-info/top_level.txt
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        1 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet.egg-info/dependency_links.txt
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     9281 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet.egg-info/SOURCES.txt
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6168 2021-07-02 19:59:19.000000 spydrnet-1.8.3/README.rst
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1985 2021-07-02 19:59:19.000000 spydrnet-1.8.3/setup.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       38 2021-07-20 16:54:02.000000 spydrnet-1.8.3/setup.cfg
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      787 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/tests/test_example_netlist_functionality.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8816 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/tests/test_flatten.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    13166 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/tests/test_clone.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4362 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/tests/test_uniquify.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      675 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/tests/test_util.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)       73 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/tests/test_verilog_to_edif.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/ir/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/ir/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      654 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_print.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8064 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_shortcuts.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1685 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_cable.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1188 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_outerpin.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5880 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_instance.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2680 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_library.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      546 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_pin.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6911 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_definition.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)       87 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1240 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_bundle.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3222 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_netlist.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4888 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_wire.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      517 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_innerpin.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1615 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_element.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4103 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/tests/test_port.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/ir/views/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/ir/views/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1618 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/tests/test_outerpinsview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2703 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/tests/test_listview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2472 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/tests/test_dictview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3364 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/tests/test_setview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2110 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/listview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      805 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/outerpinsview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3344 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/setview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1296 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/views/dictview.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    10620 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/netlist.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1889 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/innerpin.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3089 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/outerpin.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3881 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/first_class_element.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8302 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/ir/instance.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     7480 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/cable.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     9659 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/port.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4373 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/bundle.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      527 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    18971 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/definition.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      755 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/pin.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      153 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/element.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8050 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/library.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6597 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/ir/wire.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/composers/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/composers/verilog/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/composers/verilog/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/verilog/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3650 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/verilog/tests/test_composer.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    22477 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/composers/verilog/tests/test_composer_unit.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/verilog/__init__.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    21565 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/composers/verilog/composer.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      724 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/__init__.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/composers/edif/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/composers/edif/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2987 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/edif/tests/test_edifify_names.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/edif/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2573 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/edif/tests/test_topological_sort.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/edif/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    20346 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/edif/composer.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5786 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/composers/edif/edifify_names.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/support_files/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5539 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/b13.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      672 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/namespace.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1640 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/basic_clock_crossing.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1786 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/unique_different_modules.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2088 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer2.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      859 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/AND_gate.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2385 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/lfsr_zybo.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1291 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/passthrough_test.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1227 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/carrychain.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      149 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/Readme.md
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3196 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/lfsr_kc705.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1461 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/three_layer_hierarchy.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1240 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/TMR_hierarchy.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1131 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/ports_diff_modules.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4459 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/adder.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3650 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/4bitadder.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      851 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/toggle.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      774 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/inverter.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1512 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/fourBitCounter.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1831 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/bram.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1832 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/basic_synchronizer.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2148 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/synchronizer_test.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1613 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/hierarchical_luts.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1473 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/n_bit_counter.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      785 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/unused_blackbox.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6503 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/register_file.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1285 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/multi_port.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2040 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/netlist_with_large_integer.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1938 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/port_test.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1623 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/fourBitCounterWithAnd.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2087 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3448 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/unique_challenge.edf.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2940 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/one_counter.edf.zip
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5692 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/three_stage_synchronizer2.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2252 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/unused_blackbox.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2658 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/three_layer_hierarchy.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2533 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/TMR_hierarchy.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6094 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/synchronizer_test.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5684 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/three_stage_synchronizer.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5035 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/basic_clock_crossing.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6041 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/one_counter.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8492 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/float_demo.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2988 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/port_test.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2671 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/carrychain.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6538 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/lfsr_kc705.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3419 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/hierarchical_luts.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2493 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/ports_diff_modules.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5461 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/basic_synchronizer.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3566 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/unique_challenge.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4722 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/adder.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2986 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/multi_port.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      719 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/namespace.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5012 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/netlist_with_large_integer.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2588 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/passthrough_test.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2243 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/inverter.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5494 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/lfsr_zybo.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5186 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/fourBitCounterWithAnd.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5122 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/fourBitCounter.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     7205 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/register_file.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8529 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/b13.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3134 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/unique_different_modules.v.zip
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1554 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/support_files/convert.tcl
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/parsers/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/parsers/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      176 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/tests/test_parsers.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/tests/__init__.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/tests/
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1293 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_verilog_tokens.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    54042 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_verilogParser.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1309 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_tokenizer.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3421 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_token_factory.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3947 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/verilog_token_factory.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3065 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/tokenizer.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    51317 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/parser.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/__init__.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3707 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/parsers/verilog/verilog_tokens.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2412 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/parsers/__init__.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/parsers/primatives/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)   218735 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/primatives/parsetab.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/primatives/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4672 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/primatives/parse_primatives.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/parsers/edif/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/parsers/edif/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/edif/tests/__init__.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2918 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/parsers/edif/tests/test_edif_parser.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/edif/tests/test_edif_construction.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4702 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/edif/tests/test_tokenizer.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5962 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/edif/tokenizer.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    43226 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/parsers/edif/parser.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/edif/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2300 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/parsers/edif/edif_tokens.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/global_state/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/global_state/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6291 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/global_state/tests/test_global_callback.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/global_state/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3136 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/global_state/tests/test_global_service.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/global_state/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1796 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/global_state/global_service.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    10261 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/global_state/global_callback.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4166 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/release.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/shortcuts/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3115 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/shortcuts/getter.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/shortcuts/__init__.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/util/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5216 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_pins.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/util/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1054 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_patterns.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8186 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_hierarchical_reference.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     9159 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_hwires.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4667 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_instances.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6342 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_wires.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     5258 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_hinstances.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     9198 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_hports.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6059 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_cables.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8511 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_definitions.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2836 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_pins.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    10346 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_hcables.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4045 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_ports.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     7834 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_libraries.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     2971 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_netlists.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     9212 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/tests/test_get_hpins.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      677 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/patterns.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    10298 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_definitions.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    15967 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/hierarchical_reference.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      706 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    10030 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_instances.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    10527 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_hports.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     7177 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_ports.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    11013 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_libraries.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    11275 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_hpins.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    16923 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_hwires.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     9271 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_wires.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     6562 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_netlists.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    16240 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_hcables.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8622 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_hinstances.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     7298 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/library.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      198 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/selection.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    11852 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/util/get_cables.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1648 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/__init__.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/callback/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/callback/__init__.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    16801 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/callback/callback_listener.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/plugins/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/plugins/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/plugins/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      555 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/plugins/tests/test_namespace_manager.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/plugins/tests/test_hierarchical_reference_manager.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      104 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/plugins/__init__.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/plugins/namespace_manager/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/plugins/namespace_manager/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     8652 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/plugins/namespace_manager/tests/test_edif_namespace.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/plugins/namespace_manager/tests/__init__.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4308 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/plugins/namespace_manager/default_namespace.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    10838 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/plugins/namespace_manager/__init__.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7684 2021-07-20 16:50:55.000000 spydrnet-1.8.3/spydrnet/plugins/namespace_manager/edif_namespace.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3013 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/uniquify.py
--rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       32 2021-07-20 16:54:01.000000 spydrnet-1.8.3/spydrnet/VERSION
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     1193 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/clone.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/compare/
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/compare/tests/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/compare/tests/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      222 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/compare/tests/test_composers.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     3884 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/compare/tests/test_compare_netlists.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/compare/__init__.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)    15363 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/compare/compare_netlists.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)     4302 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/flatten.py
-drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 16:54:02.000000 spydrnet-1.8.3/spydrnet/testing/
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)      706 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/testing/test.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/testing/utils.py
--rw-r--r--   0 jacobb00  (1000) jacobb00  (1000)       74 2021-07-02 19:59:19.000000 spydrnet-1.8.3/spydrnet/testing/__init__.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7862 2021-11-18 01:46:17.000000 spydrnet-1.9.0/PKG-INFO
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1532 2021-07-20 20:08:18.000000 spydrnet-1.9.0/LICENSE
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet.egg-info/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       46 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet.egg-info/requires.txt
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7862 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet.egg-info/PKG-INFO
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        1 2021-07-20 16:54:02.000000 spydrnet-1.9.0/spydrnet.egg-info/not-zip-safe
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        9 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet.egg-info/top_level.txt
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        1 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     9281 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6187 2021-11-18 01:42:39.000000 spydrnet-1.9.0/README.rst
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1985 2021-07-20 20:08:18.000000 spydrnet-1.9.0/setup.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       38 2021-11-18 01:46:17.000000 spydrnet-1.9.0/setup.cfg
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      787 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/tests/test_example_netlist_functionality.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8816 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/tests/test_flatten.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    13166 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/tests/test_clone.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4347 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/tests/test_uniquify.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      675 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/tests/test_util.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       73 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/tests/test_verilog_to_edif.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/ir/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/ir/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      654 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_print.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8064 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_shortcuts.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1868 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_cable.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1188 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_outerpin.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8118 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_instance.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3048 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_library.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      665 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_pin.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7850 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_definition.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       87 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1240 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_bundle.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4153 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_netlist.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6167 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_wire.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      517 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_innerpin.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1615 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_element.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4229 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/tests/test_port.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/ir/views/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/ir/views/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1618 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/tests/test_outerpinsview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2703 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/tests/test_listview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2472 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/tests/test_dictview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3364 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/tests/test_setview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2110 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/listview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      805 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/outerpinsview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3344 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/setview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1296 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/views/dictview.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    11168 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/netlist.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1889 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/innerpin.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3089 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/outerpin.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3881 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/first_class_element.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8781 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/instance.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7480 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/cable.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     9659 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/port.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4373 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/bundle.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      527 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    19242 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/definition.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      755 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/pin.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      153 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/element.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8050 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/ir/library.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7061 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/ir/wire.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/composers/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/composers/verilog/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/composers/verilog/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/verilog/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5633 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/composers/verilog/tests/test_composer.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    22360 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/composers/verilog/tests/test_composer_unit.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/verilog/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    22131 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/composers/verilog/composer.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      796 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/composers/__init__.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/composers/edif/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/composers/edif/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2987 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/edif/tests/test_edifify_names.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/edif/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2573 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/edif/tests/test_topological_sort.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/edif/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    20346 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/edif/composer.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5786 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/composers/edif/edifify_names.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/support_files/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5539 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/b13.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      672 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/namespace.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1640 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/basic_clock_crossing.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1786 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/unique_different_modules.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2088 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer2.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      859 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/AND_gate.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2385 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/lfsr_zybo.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1291 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/passthrough_test.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1227 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/carrychain.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1151 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/Readme.md
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3196 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/lfsr_kc705.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1461 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/three_layer_hierarchy.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1240 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/TMR_hierarchy.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1131 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/ports_diff_modules.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4459 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/adder.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3650 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/4bitadder.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      851 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/toggle.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      774 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/inverter.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1512 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/fourBitCounter.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1831 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/bram.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1832 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/basic_synchronizer.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2148 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/synchronizer_test.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1613 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/hierarchical_luts.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1473 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/n_bit_counter.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      785 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/unused_blackbox.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6503 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/register_file.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1285 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/multi_port.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2040 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/netlist_with_large_integer.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1938 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/port_test.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1623 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/fourBitCounterWithAnd.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2087 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3448 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/unique_challenge.edf.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2940 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/one_counter.edf.zip
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5692 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/three_stage_synchronizer2.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2252 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/unused_blackbox.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2658 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/three_layer_hierarchy.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2533 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/TMR_hierarchy.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6094 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/synchronizer_test.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5684 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/three_stage_synchronizer.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5035 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/basic_clock_crossing.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6041 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/one_counter.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8492 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/float_demo.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2988 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/port_test.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2671 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/carrychain.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6538 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/lfsr_kc705.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3419 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/hierarchical_luts.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2493 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/ports_diff_modules.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5461 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/basic_synchronizer.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3566 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/unique_challenge.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4722 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/adder.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2986 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/multi_port.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      719 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/namespace.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5012 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/netlist_with_large_integer.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2588 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/passthrough_test.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2243 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/inverter.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5494 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/lfsr_zybo.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5186 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/fourBitCounterWithAnd.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5122 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/fourBitCounter.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7205 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/register_file.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8529 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/b13.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3134 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/unique_different_modules.v.zip
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1554 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/support_files/convert.tcl
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/parsers/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/parsers/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      176 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/tests/test_parsers.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/tests/__init__.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1293 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_verilog_tokens.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    54042 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_verilogParser.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1309 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_tokenizer.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3575 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_token_factory.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3947 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/verilog_token_factory.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3283 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/tokenizer.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    51279 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/parser.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3707 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/verilog/verilog_tokens.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2412 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/__init__.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/parsers/primatives/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)   218735 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/primatives/parsetab.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/primatives/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4684 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/parsers/primatives/parse_primatives.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/parsers/edif/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/parsers/edif/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/edif/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2918 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/edif/tests/test_edif_parser.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/edif/tests/test_edif_construction.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4702 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/edif/tests/test_tokenizer.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5964 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/parsers/edif/tokenizer.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    43226 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/edif/parser.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/edif/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2300 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/parsers/edif/edif_tokens.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/global_state/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/global_state/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6291 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/global_state/tests/test_global_callback.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/global_state/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3136 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/global_state/tests/test_global_service.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/global_state/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1796 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/global_state/global_service.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    10261 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/global_state/global_callback.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4166 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/release.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/shortcuts/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3115 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/shortcuts/getter.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/shortcuts/__init__.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/util/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5216 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_pins.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/util/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1054 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_patterns.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8186 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_hierarchical_reference.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     9159 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_hwires.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4667 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_instances.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6342 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_wires.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     5258 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_hinstances.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     9198 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_hports.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6059 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_cables.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8511 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_definitions.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2836 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_pins.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    10346 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_hcables.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4045 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_ports.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7834 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_libraries.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     2971 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_netlists.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     9212 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/tests/test_get_hpins.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      677 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/patterns.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    10298 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_definitions.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    15967 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/hierarchical_reference.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      706 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    10030 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_instances.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    10527 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_hports.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7177 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_ports.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    11013 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_libraries.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    11275 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_hpins.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    16923 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_hwires.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     9271 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_wires.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     6562 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_netlists.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    16240 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_hcables.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8622 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_hinstances.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7298 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/library.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      198 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/selection.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    11852 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/util/get_cables.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1648 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/__init__.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/callback/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/callback/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    16801 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/callback/callback_listener.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/plugins/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/plugins/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      555 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/tests/test_namespace_manager.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/tests/test_hierarchical_reference_manager.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      104 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/__init__.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/plugins/namespace_manager/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/plugins/namespace_manager/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     8652 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/namespace_manager/tests/test_edif_namespace.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/namespace_manager/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4308 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/namespace_manager/default_namespace.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    10838 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/namespace_manager/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     7684 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/plugins/namespace_manager/edif_namespace.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3006 2021-11-18 01:42:39.000000 spydrnet-1.9.0/spydrnet/uniquify.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       32 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/VERSION
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     1193 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/clone.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/compare/
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/compare/tests/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/compare/tests/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      222 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/compare/tests/test_composers.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     3884 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/compare/tests/test_compare_netlists.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/compare/__init__.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)    15363 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/compare/compare_netlists.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)     4302 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/flatten.py
+drwxrwxr-x   0 jacobb00  (1000) jacobb00  (1000)        0 2021-11-18 01:46:17.000000 spydrnet-1.9.0/spydrnet/testing/
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)      706 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/testing/test.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)        0 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/testing/utils.py
+-rw-rw-r--   0 jacobb00  (1000) jacobb00  (1000)       74 2021-07-20 20:08:18.000000 spydrnet-1.9.0/spydrnet/testing/__init__.py
```

### Comparing `spydrnet-1.8.3/PKG-INFO` & `spydrnet-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spydrnet
-Version: 1.8.3
+Version: 1.9.0
 Summary: Python package for analyzing and transforming netlists
 Home-page: https://byuccl.github.io/spydrnet
 Author: Andrew Keller
 Author-email: andrewmkeller@byu.edu
 Maintainer: SpyDrNet Developers
 Maintainer-email: spydrnet-discuss@googlegroups.com
 License: BSD
@@ -44,28 +44,28 @@
 
 .. image:: https://img.shields.io/pypi/v/spydrnet.svg
    :target: https://pypi.org/project/spydrnet/
    
 .. image:: https://img.shields.io/pypi/pyversions/spydrnet.svg
    :target: https://pypi.org/project/spydrnet/
 
-.. image:: https://travis-ci.com/byuccl/spydrnet.svg?branch=master
-   :target: https://travis-ci.com/byuccl/spydrnet
+.. image:: https://app.travis-ci.com/byuccl/spydrnet.svg?branch=master
+   :target: https://app.travis-ci.com/github/byuccl/spydrnet
 
 A flexible framework for analyzing and transforming `netlists <https://en.wikipedia.org/wiki/Netlist>`_. Built to fill an important gap in FPGA research and reliability. Currently available as a pure Python package.
 
 - **Website and Documentation:** https://byuccl.github.io/spydrnet
 - **Mailing List:** https://groups.google.com/forum/#!forum/spydrnet-discuss
 - **Source:** https://github.com/byuccl/spydrnet
 - **Bug Reports:** https://github.com/byuccl/spydrnet/issues
 
 Simple Examples
 ---------------
 
-SpyDrNet can be used to create netlists from scratch. Because it is a low-level framework, manual netlist creation can be tedious (much like writting a high level application in assembly). To assist in rapid productivity, parsers and composers are provided for common netlist formats. Currently only `EDIF <https://en.wikipedia.org/wiki/EDIF>`_ is supported, but the roadmap includes structural Verilog, structural VHDL, Verilog Quartus Mapping Files (`Intel's VQM <https://www.intel.com/content/www/us/en/programmable/quartushelp/17.0/mapIdTopics/mwh1465406414431.htm>`_), and JSON.
+SpyDrNet can be used to create netlists from scratch. Because it is a low-level framework, manual netlist creation can be tedious (much like writting a high level application in assembly). To assist in rapid productivity, parsers and composers are provided for common netlist formats. Currently `EDIF <https://en.wikipedia.org/wiki/EDIF>`_ and structural Verilog are supported, but the roadmap also includes structural VHDL, Verilog Quartus Mapping Files (`Intel's VQM <https://www.intel.com/content/www/us/en/programmable/quartushelp/17.0/mapIdTopics/mwh1465406414431.htm>`_), and JSON.
 
 **Loading Example Netlists**
 
 Several example netlists are included with the package to introduce the framework, its features, and functionality. To list and load these netlists, modify the following example: 
 
 .. code:: python
```

### Comparing `spydrnet-1.8.3/LICENSE` & `spydrnet-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet.egg-info/PKG-INFO` & `spydrnet-1.9.0/spydrnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spydrnet
-Version: 1.8.3
+Version: 1.9.0
 Summary: Python package for analyzing and transforming netlists
 Home-page: https://byuccl.github.io/spydrnet
 Author: Andrew Keller
 Author-email: andrewmkeller@byu.edu
 Maintainer: SpyDrNet Developers
 Maintainer-email: spydrnet-discuss@googlegroups.com
 License: BSD
@@ -44,28 +44,28 @@
 
 .. image:: https://img.shields.io/pypi/v/spydrnet.svg
    :target: https://pypi.org/project/spydrnet/
    
 .. image:: https://img.shields.io/pypi/pyversions/spydrnet.svg
    :target: https://pypi.org/project/spydrnet/
 
-.. image:: https://travis-ci.com/byuccl/spydrnet.svg?branch=master
-   :target: https://travis-ci.com/byuccl/spydrnet
+.. image:: https://app.travis-ci.com/byuccl/spydrnet.svg?branch=master
+   :target: https://app.travis-ci.com/github/byuccl/spydrnet
 
 A flexible framework for analyzing and transforming `netlists <https://en.wikipedia.org/wiki/Netlist>`_. Built to fill an important gap in FPGA research and reliability. Currently available as a pure Python package.
 
 - **Website and Documentation:** https://byuccl.github.io/spydrnet
 - **Mailing List:** https://groups.google.com/forum/#!forum/spydrnet-discuss
 - **Source:** https://github.com/byuccl/spydrnet
 - **Bug Reports:** https://github.com/byuccl/spydrnet/issues
 
 Simple Examples
 ---------------
 
-SpyDrNet can be used to create netlists from scratch. Because it is a low-level framework, manual netlist creation can be tedious (much like writting a high level application in assembly). To assist in rapid productivity, parsers and composers are provided for common netlist formats. Currently only `EDIF <https://en.wikipedia.org/wiki/EDIF>`_ is supported, but the roadmap includes structural Verilog, structural VHDL, Verilog Quartus Mapping Files (`Intel's VQM <https://www.intel.com/content/www/us/en/programmable/quartushelp/17.0/mapIdTopics/mwh1465406414431.htm>`_), and JSON.
+SpyDrNet can be used to create netlists from scratch. Because it is a low-level framework, manual netlist creation can be tedious (much like writting a high level application in assembly). To assist in rapid productivity, parsers and composers are provided for common netlist formats. Currently `EDIF <https://en.wikipedia.org/wiki/EDIF>`_ and structural Verilog are supported, but the roadmap also includes structural VHDL, Verilog Quartus Mapping Files (`Intel's VQM <https://www.intel.com/content/www/us/en/programmable/quartushelp/17.0/mapIdTopics/mwh1465406414431.htm>`_), and JSON.
 
 **Loading Example Netlists**
 
 Several example netlists are included with the package to introduce the framework, its features, and functionality. To list and load these netlists, modify the following example: 
 
 .. code:: python
```

### Comparing `spydrnet-1.8.3/spydrnet.egg-info/SOURCES.txt` & `spydrnet-1.9.0/spydrnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/README.rst` & `spydrnet-1.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 .. image:: https://img.shields.io/pypi/v/spydrnet.svg
    :target: https://pypi.org/project/spydrnet/
    
 .. image:: https://img.shields.io/pypi/pyversions/spydrnet.svg
    :target: https://pypi.org/project/spydrnet/
 
-.. image:: https://travis-ci.com/byuccl/spydrnet.svg?branch=master
-   :target: https://travis-ci.com/byuccl/spydrnet
+.. image:: https://app.travis-ci.com/byuccl/spydrnet.svg?branch=master
+   :target: https://app.travis-ci.com/github/byuccl/spydrnet
 
 A flexible framework for analyzing and transforming `netlists <https://en.wikipedia.org/wiki/Netlist>`_. Built to fill an important gap in FPGA research and reliability. Currently available as a pure Python package.
 
 - **Website and Documentation:** https://byuccl.github.io/spydrnet
 - **Mailing List:** https://groups.google.com/forum/#!forum/spydrnet-discuss
 - **Source:** https://github.com/byuccl/spydrnet
 - **Bug Reports:** https://github.com/byuccl/spydrnet/issues
 
 Simple Examples
 ---------------
 
-SpyDrNet can be used to create netlists from scratch. Because it is a low-level framework, manual netlist creation can be tedious (much like writting a high level application in assembly). To assist in rapid productivity, parsers and composers are provided for common netlist formats. Currently only `EDIF <https://en.wikipedia.org/wiki/EDIF>`_ is supported, but the roadmap includes structural Verilog, structural VHDL, Verilog Quartus Mapping Files (`Intel's VQM <https://www.intel.com/content/www/us/en/programmable/quartushelp/17.0/mapIdTopics/mwh1465406414431.htm>`_), and JSON.
+SpyDrNet can be used to create netlists from scratch. Because it is a low-level framework, manual netlist creation can be tedious (much like writting a high level application in assembly). To assist in rapid productivity, parsers and composers are provided for common netlist formats. Currently `EDIF <https://en.wikipedia.org/wiki/EDIF>`_ and structural Verilog are supported, but the roadmap also includes structural VHDL, Verilog Quartus Mapping Files (`Intel's VQM <https://www.intel.com/content/www/us/en/programmable/quartushelp/17.0/mapIdTopics/mwh1465406414431.htm>`_), and JSON.
 
 **Loading Example Netlists**
 
 Several example netlists are included with the package to introduce the framework, its features, and functionality. To list and load these netlists, modify the following example: 
 
 .. code:: python
```

### Comparing `spydrnet-1.8.3/setup.py` & `spydrnet-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/tests/test_example_netlist_functionality.py` & `spydrnet-1.9.0/spydrnet/tests/test_example_netlist_functionality.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/tests/test_flatten.py` & `spydrnet-1.9.0/spydrnet/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/tests/test_clone.py` & `spydrnet-1.9.0/spydrnet/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/tests/test_uniquify.py` & `spydrnet-1.9.0/spydrnet/tests/test_uniquify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 
 import unittest
-import spydrnet as sdn
-from spydrnet import Netlist, Instance, Definition
+from spydrnet import Netlist, Instance
 from spydrnet.uniquify import uniquify
 
 class TestUniquify(unittest.TestCase):
     def create_netlist(self):
         nl = Netlist()
         lib = nl.create_library()
         d1 = lib.create_definition()
         d2 = lib.create_definition()
-        d3 = lib.create_definition()
+        d3 = lib.create_definition(name='instance_name')
         i11 = d1.create_child()
         i12 = d1.create_child()
         i13 = d1.create_child()
         i24 = d2.create_child()
         i25 = d2.create_child()
         i26 = d2.create_child()
         i27 = d2.create_child()
```

### Comparing `spydrnet-1.8.3/spydrnet/tests/test_util.py` & `spydrnet-1.9.0/spydrnet/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_print.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_shortcuts.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_cable.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_cable.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,8 +43,14 @@
     def test_remove_wire_from(self):
         wire_included = self.cable.create_wire()
         wire = self.cable.create_wire()
         self.cable.remove_wires_from({wire})
         self.assertFalse(wire in self.cable.wires)
         self.assertIsNone(wire.cable)
         self.assertTrue(wire_included in self.cable.wires)
-        self.assertEqual(wire_included.cable, self.cable)
+        self.assertEqual(wire_included.cable, self.cable)
+
+    def test_scalar_false(self):
+        cable = sdn.Cable()
+        cable.create_wire()
+        cable.create_wire()
+        self.assertTrue('is_scalar: False;' in cable.__str__())
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_outerpin.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_outerpin.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_library.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_library.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,8 +54,18 @@
     def test_remove_definitions_from(self):
         definition_included = self.library.create_definition()
         definition = self.library.create_definition()
         self.library.remove_definitions_from({definition})
         self.assertFalse(definition in self.library.definitions)
         self.assertIsNone(definition.library)
         self.assertTrue(definition_included in self.library.definitions)
-        self.assertEqual(definition_included.library, self.library)
+        self.assertEqual(definition_included.library, self.library)
+
+    def test_no_parent_netlist(self):
+        library = sdn.Library()
+        self.assertTrue('parent netlist undefined' in library.__str__())
+
+    def test_no_parent_netlist_name(self):
+        netlist = sdn.Netlist()
+        library = sdn.Library()
+        netlist.add_library(library)
+        self.assertTrue('parent netlist.name undefined' in library.__str__())
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_pin.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_pin.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,8 +15,12 @@
         self.assertNotEqual(self.pin, pin2)
 
     def test_wire(self):
         self.assertIsNone(self.pin.wire)
 
     @unittest.expectedFailure
     def test_wire_set(self):
-        self.pin.wire = None
+        self.pin.wire = None
+
+    def test_no_wire(self):
+        pin = Pin()
+        self.assertTrue('Wire connected undefined' in pin.__str__())
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_definition.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,17 @@
         port1 = self.definition.create_port()
         port2 = self.definition.create_port()
         self.assertEqual(self.definition.ports, [port1, port2])
         self.definition.ports = [port2, port1]
         self.assertEqual(self.definition.ports, [port2, port1])
 
     def test_create_port(self):
-        port = self.definition.create_port()
+        port = self.definition.create_port("Port1", pins=2)
+        self.assertEqual(port.name, "Port1")
+        self.assertEqual(len(port.pins), 2)
         self.assertTrue(port in self.definition.ports)
         self.assertEqual(port.definition, self.definition)
 
     def test_add_port(self):
         port = sdn.Port()
         self.definition.add_port(port, position=0)
         self.assertTrue(port in self.definition.ports)
@@ -40,14 +42,23 @@
 
     def test_remove_port(self):
         port = self.definition.create_port()
         self.definition.remove_port(port)
         self.assertFalse(port in self.definition.ports)
         self.assertIsNone(port.definition)
 
+    def test_remove_multiple_ports(self):
+        port = self.definition.create_port()
+        port_2 = self.definition.create_port()
+        self.definition.remove_ports_from([port,port_2])
+        self.assertFalse(port in self.definition.ports)
+        self.assertFalse(port_2 in self.definition.ports)
+        self.assertIsNone(port.definition)
+        self.assertIsNone(port_2.definition)
+
     @unittest.expectedFailure
     def test_remove_ports_from_outside_definition(self):
         port = sdn.Port()
         self.definition.remove_ports_from((port,))
 
     def test_remove_ports_from(self):
         port_included = self.definition.create_port()
@@ -68,15 +79,17 @@
         cable1 = self.definition.create_cable()
         cable2 = self.definition.create_cable()
         self.assertEqual(self.definition.cables, [cable1, cable2])
         self.definition.cables = [cable2, cable1]
         self.assertEqual(self.definition.cables, [cable2, cable1])
 
     def test_create_cable(self):
-        cable = self.definition.create_cable()
+        cable = self.definition.create_cable("cable1", wires=2)
+        self.assertEqual(cable.name, "cable1")
+        self.assertEqual(len(cable.wires), 2)
         self.assertTrue(cable in self.definition.cables)
         self.assertEqual(self.definition, cable.definition)
 
     def test_add_cable(self):
         cable = sdn.Cable()
         self.definition.add_cable(cable, position=0)
         self.assertTrue(cable in self.definition.cables)
@@ -156,8 +169,16 @@
         self.definition.create_cable()
         self.assertFalse(self.definition.is_leaf()), "Definition with a cable is considered a leaf cell"
         self.definition.remove_cables_from(self.definition.cables)
         self.definition.create_child()
         self.assertFalse(self.definition.is_leaf()), "Definition with a child instance is considered a leaf cell"
         self.definition.create_cable()
         self.assertFalse(self.definition.is_leaf()), "Definition with a cable and child instance is considered a leaf" \
-                                                     " cell"
+                                                     " cell"
+
+    def test_library_name(self):
+        definition = sdn.Definition()
+        library = sdn.Library()
+        library.add_definition(definition)
+        self.assertTrue('Library.name undefined' in definition.__str__())
+        library.name = 'library'
+        self.assertTrue('Library.name \'library\'' in definition.__str__())
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_bundle.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_netlist.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_netlist.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import spydrnet as sdn
 from spydrnet.ir.first_class_element import FirstClassElement
-
+from spydrnet.uniquify import uniquify
 
 class TestNetlist(unittest.TestCase):
     def setUp(self):
         self.netlist = sdn.Netlist()
 
     def test_constructor(self):
         self.assertIsInstance(self.netlist, FirstClassElement, "Netlist is not an element.")
@@ -71,8 +71,31 @@
         self.assertIsNone(library.netlist)
         library_included = self.netlist.create_library()
         library = self.netlist.create_library()
         self.netlist.remove_libraries_from({library})
         self.assertFalse(library in self.netlist)
         self.assertIsNone(library.netlist)
         self.assertTrue(library_included in self.netlist.libraries)
-        self.assertEqual(library_included.netlist, self.netlist)
+        self.assertEqual(library_included.netlist, self.netlist)
+
+    def test_top_instance_name(self):
+        netlist = sdn.load_example_netlist_by_name('toggle')
+        self.assertTrue('top_instance.name \'toggle\'' in netlist.__str__())
+
+    def test_set_top_instance_using_instance(self):
+        netlist = sdn.Netlist()
+        instance = sdn.Instance()
+        netlist.set_top_instance(instance)
+        self.assertTrue(netlist.top_instance is instance)
+
+    def test_set_top_instance_using_definition(self):
+        netlist = sdn.Netlist()
+        definition = sdn.Definition()
+        netlist.set_top_instance(definition)
+        self.assertTrue(netlist.top_instance.reference is definition)
+
+    def test_is_unique(self):
+        example_name = 'unique_challenge'
+        netlist = sdn.load_example_netlist_by_name(example_name)
+        self.assertFalse(netlist.is_unique())
+        uniquify(netlist)
+        self.assertTrue(netlist.is_unique())
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_innerpin.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_innerpin.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_element.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/tests/test_port.py` & `spydrnet-1.9.0/spydrnet/ir/tests/test_port.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         for direction in directions:
             self.port.direction = direction
             self.assertEqual(self.port.direction.name.lower(), direction.lower())
         for direction in sdn.Port.Direction:
             self.port.direction = direction
             self.assertEqual(self.port.direction, direction)
 
+    def test_direction_2(self):
+        port = sdn.Port(direction=sdn.IN)
+        self.assertTrue(port.direction is sdn.IN)
+
     @unittest.expectedFailure
     def test_direction_set_bad_type(self):
         self.port.direction = list()
 
     def test_initialize_pins(self):
         self.port.create_pins(2)
         self.assertEqual(len(self.port.pins), 2)
@@ -108,8 +112,8 @@
         self.port.is_array = True
         self.port.remove_pins_from(self.port.pins)
         self.assertTrue(self.port.is_array)
 
     @unittest.expectedFailure
     def test_is_array_clear_on_array_bundle(self):
         self.port.create_pins(2)
-        self.port.is_array = False
+        self.port.is_array = False
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/tests/test_outerpinsview.py` & `spydrnet-1.9.0/spydrnet/ir/views/tests/test_outerpinsview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/tests/test_listview.py` & `spydrnet-1.9.0/spydrnet/ir/views/tests/test_listview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/tests/test_dictview.py` & `spydrnet-1.9.0/spydrnet/ir/views/tests/test_dictview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/tests/test_setview.py` & `spydrnet-1.9.0/spydrnet/ir/views/tests/test_setview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/listview.py` & `spydrnet-1.9.0/spydrnet/ir/views/listview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/outerpinsview.py` & `spydrnet-1.9.0/spydrnet/ir/views/outerpinsview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/setview.py` & `spydrnet-1.9.0/spydrnet/ir/views/setview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/views/dictview.py` & `spydrnet-1.9.0/spydrnet/ir/views/dictview.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/netlist.py` & `spydrnet-1.9.0/spydrnet/ir/netlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,21 +119,25 @@
         creates a new instance with that definition and set it as the top instance.
         """
         assert instance is None or isinstance(instance, Instance) or isinstance(
             instance, Definition), "Must specify an instance"
         global_callback._call_netlist_top_instance(self, instance)
         # TODO: should We have a DRC that makes sure the instance is of a definition contained in netlist? I think no
         #  but I am open to hear other points of veiw.
-
+        if self.top_instance:
+            self.top_instance.is_top_instance = False
         if isinstance(instance, Definition):
             top = Instance()
             top.reference = instance
+            top.is_top_instance = True
             self.top_instance = top
         else:
             self._top_instance = instance
+            if instance:
+                instance.is_top_instance = True
 
     def set_top_instance(self, instance, instance_name='instance'):
         """Sets the top instance of the design.
 
         The instance must not be null and should probably come from this netlist
 
         Parameters
@@ -296,7 +300,18 @@
             rep += 'top_instance undefined'
         elif self.top_instance.name is None:
             rep += 'top_instance.name undefined'
         else:
             rep += 'top_instance.name \'' + self.top_instance.name + '\''
         rep += '>'
         return rep
+
+    def is_unique(self):
+        """
+        checks whether all of the instances in the netlist are unique or not
+        """
+        for instance in self.get_instances():
+            if len(instance.reference.references) == 1 or instance.reference.is_leaf():
+                continue
+            else:
+                return False
+        return True
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/innerpin.py` & `spydrnet-1.9.0/spydrnet/ir/innerpin.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/outerpin.py` & `spydrnet-1.9.0/spydrnet/ir/outerpin.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/first_class_element.py` & `spydrnet-1.9.0/spydrnet/ir/first_class_element.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/instance.py` & `spydrnet-1.9.0/spydrnet/ir/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,29 +17,30 @@
     :ivar parent: the parent of the object. Parent is the definition that instances another definition.
     :ivar child: the instance itself is the child of the parent.
     :ivar reference: the item of the object. Reference is the definition of the instance.
 
     For example, when writing definition 1, we instance definition 2. Definition 1 is the parent, the instance is the child, and definition 2 is the instance's reference.
 
     """
-    __slots__ = ['_parent', '_reference', '_pins']
+    __slots__ = ['_parent', '_reference', '_pins','_is_top_instance']
 
     def __init__(self, name=None, properties=None):
         """Creates an empty object of type instance.
 
         parameters
         ----------
 
         name - (str) the name of this instance
         properties - (dict) the dictionary which holds the properties
         """
         super().__init__()
         self._parent = None
         self._reference = None
         self._pins = OrderedDict()
+        self._is_top_instance = False
         _call_create_instance(self)
         if name != None:
             self.name = name
         if properties != None:
             assert isinstance(
                 properties, dict), "properties must be a dictionary"
             for key in properties:
@@ -183,14 +184,23 @@
         """
         if self._reference is None:
             return False
         elif len(self._reference._children) > 0 or len(self._reference._cables) > 0:
             return False
         return True
 
+    def is_unique(self):
+        """
+        Check to see if the instance is unique
+        """
+        if len(self.reference.references) == 1 or self.reference.is_leaf():
+            return True
+        else:
+            return False
+
     def __str__(self):
         """Re-define the print function so it is easier to read"""
         rep = super().__str__()
         rep = rep[:-1] + '; '
         if self.parent is None:
             rep += 'parent definition undefined'
         elif self.parent.name is None:
@@ -204,7 +214,15 @@
             rep += 'reference definition undefined'
         elif self.reference.name is None:
             rep += 'reference definition.name undefined'
         else:
             rep += 'reference definition.name \'' + self.reference.name + '\''
         rep += '>'
         return rep
+
+    @property
+    def is_top_instance(self):
+        return self._is_top_instance
+
+    @is_top_instance.setter
+    def is_top_instance(self,value):
+        self._is_top_instance = value
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/cable.py` & `spydrnet-1.9.0/spydrnet/ir/cable.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/port.py` & `spydrnet-1.9.0/spydrnet/ir/port.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/bundle.py` & `spydrnet-1.9.0/spydrnet/ir/bundle.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/__init__.py` & `spydrnet-1.9.0/spydrnet/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/definition.py` & `spydrnet-1.9.0/spydrnet/ir/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,31 +138,33 @@
         Leaf cells are cells with no children instances or no
         children cables. Blackbox cells are considered leaf cells as well as direct pass through cells with cables only
         """
         if len(self._children) > 0 or len(self._cables) > 0:
             return False
         return True
 
-    def create_port(self, name=None, properties=None, is_downto=None, is_scalar=None, lower_index=None, direction=None):
+    def create_port(self, name=None, properties=None, is_downto=None, is_scalar=None, lower_index=None, direction=None, pins=None):
         """Create a port, add it to the definition, and return that port.
 
         parameters
         ----------
 
         name - (str) the name of this instance
         properties - (dict) the dictionary which holds the properties
         id_downto - (bool) set the downto status. Downto is False if the right index is higher than the left one, True otherwise
         is_scalar - (bool) set the scalar status. Return True if the item is a scalar False otherwise.
         lower_index - (int) get the value of the lower index of the array.
         direction - (Enum) Define the possible directions for a given port. (UNDEFINED, INOUT, IN, OUT)
-
+        pins - (int) Create number of pins in the newly created port
         """
         port = Port(name, properties, is_downto,
                     is_scalar, lower_index, direction)
         self.add_port(port)
+        if pins:
+            port.create_pins(pins)
         return port
 
     def add_port(self, port, position=None):
         """Add a preexisting port to the definition.
 
         This port must not be a member of any definition
 
@@ -336,28 +338,31 @@
     def _remove_child(self, child):
         """
         Internal function for dissociating a child instance from the definition.
         """
         global_callback._call_definition_remove_child(self, child)
         child._parent = None
 
-    def create_cable(self, name=None, properties=None, is_downto=None, is_scalar=None, lower_index=None):
+    def create_cable(self, name=None, properties=None, is_downto=None, is_scalar=None, lower_index=None, wires=None):
         """Create a cable, add it to the definition, and return the cable.
 
         parameters
         ----------
 
         name - (str) the name of this instance
         properties - (dict) the dictionary which holds the properties
         id_downto - (bool) set the downto status. Downto is False if the right index is higher than the left one, True otherwise
         is_scalar - (bool) set the scalar status. Return True if the item is a scalar False otherwise.
         lower_index - (int) get the value of the lower index of the array.
+        wires - (int) Create number of wires in the newly created cable
         """
         cable = Cable(name, properties, is_downto, is_scalar, lower_index)
         self.add_cable(cable)
+        if wires:
+            cable.create_wires(wires)
         return cable
 
     def add_cable(self, cable, position=None):
         """Add a cable to the definition.
 
         The cable must not already be a member of another definition.
```

### Comparing `spydrnet-1.8.3/spydrnet/ir/pin.py` & `spydrnet-1.9.0/spydrnet/ir/pin.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/library.py` & `spydrnet-1.9.0/spydrnet/ir/library.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/ir/wire.py` & `spydrnet-1.9.0/spydrnet/ir/wire.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from copy import copy, deepcopy, error
+import spydrnet as sdn
 from spydrnet.ir.element import Element
 from spydrnet.ir.outerpin import OuterPin
 from spydrnet.ir.views.listview import ListView
 from spydrnet.global_state import global_callback
-from copy import copy, deepcopy, error
 
 
 class Wire(Element):
     """
     Represents a wire object
     """
     __slots__ = ['_cable', '_pins', '__weakref__']
@@ -148,15 +149,15 @@
         memo[self] = c
         c._cable = None
         # shallow copy the list so that it retains its pin references
         c._pins = copy(self._pins)
         return c
 
     def clone(self):
-        """clone wire in an api safe way. 
+        """clone wire in an api safe way.
 
         The following properties can be expected from the returned element:
          * The wire is not connected to any pins.
          * The wire is orphaned from any cable.
          * No pins are connected to the wire
          """
         c = self._clone(dict())
@@ -165,20 +166,34 @@
 
     def index(self):
         """if this wire is in a cable, returns the index number of the wire in the parent cable"""
 
         assert self.cable is not None, "the wire does not belong to a cable"
 
         return self.cable.wires.index(self)
-    
+
     def __str__(self):
         """Re-define the print function so it is easier to read"""
         rep = str(type(self))
         rep = rep[:-1] + '; '
         if self.cable is None:
             rep += 'Not contained by any Cable'
         elif self.cable.name is None:
             rep += 'Contained by Cable whose name is undefined'
         else:
-            rep += 'Cotained by Cable.name \'' + str(self.cable) + '\''
+            rep += 'Contained by Cable.name \'' + str(self.cable.name) + '\' ' + str(self.cable)
         rep += '>'
         return rep
+
+    def get_driver(self):
+        '''
+        returns the driver(s) of the wire
+        '''
+        drivers = []
+        for pin in self._pins:
+            if pin.__class__ is sdn.InnerPin:
+                if pin.port.direction is sdn.IN:
+                    drivers.append(pin)
+            else:
+                if pin.inner_pin.port.direction is sdn.OUT:
+                    drivers.append(pin)
+        return drivers
```

### Comparing `spydrnet-1.8.3/spydrnet/composers/verilog/tests/test_composer_unit.py` & `spydrnet-1.9.0/spydrnet/composers/verilog/tests/test_composer_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #Copyright 2021
 #Author Dallin Skouson
 #see the license for details
 #
 #Tests the verilog composers functions and output
 
+from collections import OrderedDict
 import unittest
 from unittest.case import expectedFailure
 import spydrnet as sdn
 from spydrnet.composers.verilog.composer import Composer
+from collections import OrderedDict
 
 class TestVerilogComposerUnit(unittest.TestCase):
-    
+
     class TestFile:
         '''represents a file (has a write function for the composer)
         can be used as a drop in replacement for the composer file.write function
         saves all written stuff to a string'''
         def __init__(self):
             self.written = ""
 
         def write(self, text):
             self.written += text
-        
+
         def clear(self):
             self.written = ""
 
         def compare(self, text, should_match = True):
             self.written = self.written.lstrip()
             if (text == self.written) == should_match:
                 return True
@@ -41,15 +43,15 @@
                 return False
 
 
     def initialize_tests(self):
         composer = Composer()
         composer.file = self.TestFile()
         return composer
-    
+
     def initialize_netlist(self):
         netlist = sdn.Netlist()
         netlist.name = "test_netlist"
         return netlist
 
     def initialize_library(self):
         netlist = self.initialize_netlist()
@@ -60,15 +62,15 @@
     def initialize_definition(self):
         library = self.initialize_library()
         definition = library.create_definition()
         definition.name = "test_definition"
         return definition
 
     def initialize_instance_parameters(self, instance):
-        instance["VERILOG.Parameters"] = dict()
+        instance["VERILOG.Parameters"] = OrderedDict()
         instance["VERILOG.Parameters"]["key"] = "value"
         instance["VERILOG.Parameters"]["key2"] = "value2"
 
         expected1 = ".key(value)"
         expected2 = ".key2(value2)"
 
         return expected1, expected2
@@ -78,21 +80,21 @@
         instance.reference = ref_def
         ref_def.name = "reference_definition"
 
         single_bit_port = ref_def.create_port()
         single_bit_port.create_pin()
         single_bit_port.is_downto = True
         single_bit_port.name = "single_bit_port"
-        
+
         single_bit_cable = definition.create_cable()
         single_bit_cable.name = "single_bit_cable"
         single_bit_cable.is_downto = True
         single_bit_cable.create_wire()
 
-        
+
         multi_bit_port = ref_def.create_port()
         multi_bit_port.is_downto = True
         multi_bit_port.create_pins(4)
         multi_bit_port.name = "multi_bit_port"
 
         multi_bit_port_offset = ref_def.create_port()
         multi_bit_port_offset.lower_index = 4
@@ -105,43 +107,43 @@
         partial_port.is_downto = True
         partial_port.name = "partial_port"
 
         multi_bit_cable = definition.create_cable()
         multi_bit_cable.create_wires(4)
         multi_bit_cable.name = "multi_bit_cable"
         multi_bit_cable.is_downto = True
-        
+
 
         concatenated_port = ref_def.create_port()
         concatenated_port.create_pins(4)
         concatenated_port.name = "concatenated_port"
 
         ccs = []
         for i in range(4):
             cable = definition.create_cable()
             cable.create_wire()
             cable.is_downto = True
             cable.name = "cc_" + str(i)
             ccs.append(cable)
-    
+
 
         single_bit_cable.wires[0].connect_pin(instance.pins[single_bit_port.pins[0]])
 
         for i in range(4):
             multi_bit_cable.wires[i].connect_pin(instance.pins[multi_bit_port.pins[i]])
             multi_bit_cable.wires[i].connect_pin(instance.pins[multi_bit_port_offset.pins[i]])
             ccs[i].wires[0].connect_pin(instance.pins[concatenated_port.pins[i]])
 
         for i in range(2):
             multi_bit_cable.wires[i].connect_pin(instance.pins[partial_port.pins[i]])
 
         single_bit_expected = "." + single_bit_port.name + "(" + single_bit_cable.name + ")"
-        
+
         multi_bit_expected = "." + multi_bit_port.name + "(" + multi_bit_cable.name + ")"
-        
+
         offset_expected = "." + multi_bit_port_offset.name + "(" + multi_bit_cable.name + ")"
 
         partial_expected = "." + partial_port.name + "(" + multi_bit_cable.name + "[1:0])"
 
         concatenated_expected = "." + concatenated_port.name + "({" + ccs[0].name + ', ' + ccs[1].name + ', ' + ccs[2].name + ', ' + ccs[3].name + "})"
 
         return single_bit_port, single_bit_expected, \
@@ -156,21 +158,21 @@
         netlist.name = "Netlist_name"
         composer._write_header(netlist)
         assert composer.file.compare("//Generated from netlist by SpyDrNet\n//netlist name: Netlist_name\n")
 
     def test_write_brackets_single_bit(self):
         #def _write_brackets(self, bundle, low_index, high_index):
         composer = self.initialize_tests()
-        
+
         port = sdn.Port()
         cable = sdn.Cable()
 
         cable_name = "my_cable"
         port_name = "my_port"
-        
+
         port.name = port_name
         cable.name = cable_name
 
         port.create_pin()
         cable.create_wire()
 
         composer._write_brackets(port, None, None)
@@ -195,25 +197,25 @@
         composer._write_brackets(cable, None, 0)
         assert composer.file.compare("")
         composer.file.clear()
         composer._write_brackets(cable, 0, 0)
         assert composer.file.compare("")
         composer.file.clear()
         #none of these should write because they are all single bit.
-    
+
     def test_write_brackets_single_bit_offset(self):
         #def _write_brackets(self, bundle, low_index, high_index):
         composer = self.initialize_tests()
-        
+
         port = sdn.Port()
         cable = sdn.Cable()
 
         cable_name = "my_cable"
         port_name = "my_port"
-        
+
         port.name = port_name
         cable.name = cable_name
 
         port.create_pin()
         cable.create_wire()
 
         port.lower_index = 4
@@ -241,24 +243,24 @@
         composer._write_brackets(cable, None, 4)
         assert composer.file.compare("")
         composer.file.clear()
         composer._write_brackets(cable, 4, 4)
         assert composer.file.compare("")
         composer.file.clear()
         #none of these should write because they are all single bit.
-        
+
     def test_write_brackets_multi_bit(self):
         composer = self.initialize_tests()
-        
+
         port = sdn.Port()
         cable = sdn.Cable()
 
         cable_name = "my_cable"
         port_name = "my_port"
-        
+
         port.name = port_name
         cable.name = cable_name
 
         port.create_pins(4) #input [3:0] my_input;
         port.is_downto = True
         cable.create_wires(4) #wire [3:0] my_wire;
         cable.is_downto = True
@@ -296,25 +298,25 @@
         composer.file.clear()
         composer._write_brackets(cable, 0, 3)
         assert composer.file.compare("")
         composer.file.clear()
         composer._write_brackets(cable, 1, 2)
         assert composer.file.compare("[2:1]")
         composer.file.clear()
-        
+
 
     def test_write_brackets_multi_bit_offset(self):
         composer = self.initialize_tests()
-        
+
         port = sdn.Port()
         cable = sdn.Cable()
 
         cable_name = "my_cable"
         port_name = "my_port"
-        
+
         port.name = port_name
         cable.name = cable_name
 
         port.create_pins(4) #input [3:0] my_input;
         port.is_downto = True
         port.lower_index = 4
         cable.create_wires(4) #wire [3:0] my_wire;
@@ -359,15 +361,15 @@
         assert composer.file.compare("[6:5]")
         composer.file.clear()
 
     def test_write_brackets_fail(self):
         pass #we should add some tests to test out of bounds on the brackets.
 
     def test_write_brackets_defining(self):
-        
+
         composer = self.initialize_tests()
 
         def initialize_bundle(bundle, offset, width):
             if isinstance(bundle, sdn.Port):
                 bundle.create_pins(width)
             else: #it's a cable
                 bundle.create_wires(width)
@@ -387,39 +389,39 @@
         composer._write_brackets_defining(b2)
         assert composer.file.compare("[4:4]")
         composer.file.clear()
 
         composer._write_brackets_defining(b3)
         assert composer.file.compare("[3:0]")
         composer.file.clear()
-        
+
         composer._write_brackets_defining(b4)
         assert composer.file.compare("[7:4]")
         composer.file.clear()
 
     def test_write_name(self):
         composer = self.initialize_tests()
         o = sdn.Cable() #Type of this shouldn't really matter
         valid_names = ["basic_name", "\\escaped ", "\\fads#@%!$!@#%$[0:4320] "]
         for n in valid_names:
             o.name = n
             composer._write_name(o)
             assert composer.file.compare(n)
             composer.file.clear()
-    
+
     @unittest.expectedFailure
     def test_write_none_name(self):
         composer = self.initialize_tests()
-        o = sdn.Cable() 
+        o = sdn.Cable()
         composer._write_name(o)
 
     @unittest.expectedFailure
     def test_write_invalid_name(self):
         composer = self.initialize_tests()
-        o = sdn.Cable() 
+        o = sdn.Cable()
         o.name = "\\escaped_no_space"
         composer._write_name(o)
 
     def test_write_instance_port(self):
         composer = self.initialize_tests()
         definition = self.initialize_definition()
         instance = definition.create_child()
@@ -431,19 +433,19 @@
             partial_port, partial_expected, \
             concatenated_port, concatenated_expected\
             = self.initialize_instance_port_connections(instance, definition)
 
         composer._write_instance_port(instance, single_bit_port)
         assert composer.file.compare(single_bit_expected)
         composer.file.clear()
-        
+
         composer._write_instance_port(instance, multi_bit_port)
         assert composer.file.compare(multi_bit_expected)
         composer.file.clear()
-        
+
         composer._write_instance_port(instance, multi_bit_port_offset)
         assert composer.file.compare(offset_expected)
         composer.file.clear()
 
         composer._write_instance_port(instance, partial_port)
         assert composer.file.compare(partial_expected)
         composer.file.clear()
@@ -525,16 +527,15 @@
 
         expected = instance.reference.name + " " + parameters_expected + "    " + instance.name + port_expected + "\n"
         assert composer.file.compare(expected)
 
     def test_write_module_header(self):
         composer = self.initialize_tests()
         definition = self.initialize_definition()
-        
-        definition["VERILOG.Parameters"] = dict()
+        definition["VERILOG.Parameters"] = OrderedDict()
 
         definition["VERILOG.Parameters"]["key"] = "value"
         definition["VERILOG.Parameters"]["no_default"] = None
 
         port = definition.create_port()
         port.name = "my_port"
         port.create_pin()
@@ -600,29 +601,29 @@
     def test_write_module_ports_header_and_body_disconnect(self):
         composer = self.initialize_tests()
         definition = self.initialize_definition()
 
         port_disconnect = definition.create_port("disconnected")
         port_disconnect.direction = sdn.Port.Direction.INOUT
         port_disconnect.create_pin()
-    
+
         composer._write_module_header_port(port_disconnect)
         assert composer.file.compare(port_disconnect.name)
         composer.file.clear()
         composer._write_module_body_port(port_disconnect)
         assert composer.file.compare("inout " + port_disconnect.name + ';\n')
         composer.file.clear()
 
     def test_write_module_body_cables(self):
         composer = self.initialize_tests()
         definition = self.initialize_definition()
 
         cable = definition.create_cable(name = "test_cable", is_downto = True)
         cable.create_wires(4)
-        
+
         composer._write_module_body_cable(cable)
         assert composer.file.compare("wire [3:0]" + cable.name + ";\n")
 
 
     def test_assignment_single_bit(self):
         pass
```

### Comparing `spydrnet-1.8.3/spydrnet/composers/verilog/composer.py` & `spydrnet-1.9.0/spydrnet/composers/verilog/composer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,34 @@
 from spydrnet.ir.port import Port
 from spydrnet.ir.cable import Cable
 import spydrnet.parsers.verilog.verilog_tokens as vt
 
 
 class Composer:
 
-    def __init__(self):
+    def __init__(self, definition_list=None, write_blackbox=False):
+        """ Write a verilog netlist from SDN netlist
+
+        parameters
+        ----------
+
+        definition_list - (list[str]) list of defintions to write
+        write_blackbox - (bool) Skips writing black boxes/verilog primitives
+        """
         self.file = None
         self.direction_string_map = dict()
         self.direction_string_map[Port.Direction.IN] = "input"
         self.direction_string_map[Port.Direction.OUT] = "output"
         self.direction_string_map[Port.Direction.INOUT] = "inout"
         self.direction_string_map[Port.Direction.UNDEFINED] = "/* undefined port direction */ inout"
         self.written = set()
         self.indent_count = 4  # set the indentation level for various components
+        self.write_blackbox = write_blackbox
+        self.definition_list = definition_list
+
 
     def run(self, ir, file_out="out.v"):
         self._open_file(file_out)
         self._compose(ir)
 
     def _open_file(self, file_name):
         f = open(file_name, "w")
@@ -90,17 +101,22 @@
         '''write out a bundle name and indicies. in name indicies order.
         useful for cable and port instances'''
         self._write_name(bundle)
         self._write_brackets(bundle, low, high)
 
     def _write_module(self, definition):
         '''write the constraints then the module header then the module body'''
+        if self.definition_list:
+            if not (definition.name in self.definition_list):
+                return
         if definition.library.name == "SDN_VERILOG_ASSIGNMENT":
             return  # don't write assignment definitions
         if definition.library.name == "SDN.verilog_primitives":
+            if not self.write_blackbox:
+                return
             self.file.write(vt.CELL_DEFINE)
             self.file.write(vt.NEW_LINE)
         self._write_star_constraints(definition)
         self._write_module_header(definition)
         self._write_module_body(definition)
         self.file.write(vt.END_MODULE)
         if definition.library.name == "SDN.verilog_primitives":
```

### Comparing `spydrnet-1.8.3/spydrnet/composers/__init__.py` & `spydrnet-1.9.0/spydrnet/composers/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 
 
-def compose(netlist, filename):
+def compose(netlist, filename, definition_list=[], write_blackbox=True):
     """To compose a file into a netlist format"""
     extension = os.path.splitext(filename)[1]
     extension_lower = extension.lower()
     if extension_lower in {".edf", ".edif"}:
         from spydrnet.composers.edif.composer import ComposeEdif
         composer = ComposeEdif()
         if netlist.name is None:
             raise Exception("netlist.name undefined")
         composer.run(netlist, filename)
     elif extension_lower in [".v", ".vh"]:
         from spydrnet.composers.verilog.composer import Composer
-        composer = Composer()
+        composer = Composer(definition_list, write_blackbox)
         composer.run(netlist, file_out=filename)
     else:
         raise RuntimeError("Extension {} not recognized.".format(extension))
```

### Comparing `spydrnet-1.8.3/spydrnet/composers/edif/tests/test_edifify_names.py` & `spydrnet-1.9.0/spydrnet/composers/edif/tests/test_edifify_names.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/composers/edif/tests/test_topological_sort.py` & `spydrnet-1.9.0/spydrnet/composers/edif/tests/test_topological_sort.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/composers/edif/composer.py` & `spydrnet-1.9.0/spydrnet/composers/edif/composer.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/composers/edif/edifify_names.py` & `spydrnet-1.9.0/spydrnet/composers/edif/edifify_names.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/b13.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/b13.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/namespace.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/namespace.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/basic_clock_crossing.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/basic_clock_crossing.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/unique_different_modules.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/unique_different_modules.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer2.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer2.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/AND_gate.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/AND_gate.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/lfsr_zybo.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/lfsr_zybo.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/passthrough_test.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/passthrough_test.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/carrychain.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/carrychain.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/lfsr_kc705.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/lfsr_kc705.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/three_layer_hierarchy.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/three_layer_hierarchy.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/TMR_hierarchy.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/TMR_hierarchy.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/ports_diff_modules.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/ports_diff_modules.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/adder.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/adder.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/4bitadder.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/4bitadder.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/toggle.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/toggle.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/inverter.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/inverter.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/fourBitCounter.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/fourBitCounter.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/bram.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/bram.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/basic_synchronizer.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/basic_synchronizer.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/synchronizer_test.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/synchronizer_test.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/hierarchical_luts.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/hierarchical_luts.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/n_bit_counter.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/n_bit_counter.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/unused_blackbox.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/unused_blackbox.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/register_file.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/register_file.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/multi_port.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/multi_port.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/netlist_with_large_integer.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/netlist_with_large_integer.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/port_test.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/port_test.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/fourBitCounterWithAnd.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/fourBitCounterWithAnd.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/three_stage_synchronizer.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/unique_challenge.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/unique_challenge.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/EDIF_netlists/one_counter.edf.zip` & `spydrnet-1.9.0/spydrnet/support_files/EDIF_netlists/one_counter.edf.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/three_stage_synchronizer2.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/three_stage_synchronizer2.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/unused_blackbox.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/unused_blackbox.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/three_layer_hierarchy.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/three_layer_hierarchy.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/TMR_hierarchy.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/TMR_hierarchy.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/synchronizer_test.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/synchronizer_test.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/three_stage_synchronizer.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/three_stage_synchronizer.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/basic_clock_crossing.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/basic_clock_crossing.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/one_counter.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/one_counter.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/float_demo.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/float_demo.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/port_test.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/port_test.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/carrychain.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/carrychain.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/lfsr_kc705.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/lfsr_kc705.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/hierarchical_luts.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/hierarchical_luts.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/ports_diff_modules.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/ports_diff_modules.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/basic_synchronizer.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/basic_synchronizer.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/unique_challenge.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/unique_challenge.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/adder.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/adder.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/multi_port.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/multi_port.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/namespace.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/namespace.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/netlist_with_large_integer.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/netlist_with_large_integer.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/passthrough_test.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/passthrough_test.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/inverter.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/inverter.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/lfsr_zybo.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/lfsr_zybo.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/fourBitCounterWithAnd.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/fourBitCounterWithAnd.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/fourBitCounter.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/fourBitCounter.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/register_file.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/register_file.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/b13.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/b13.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/verilog_netlists/unique_different_modules.v.zip` & `spydrnet-1.9.0/spydrnet/support_files/verilog_netlists/unique_different_modules.v.zip`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/support_files/convert.tcl` & `spydrnet-1.9.0/spydrnet/support_files/convert.tcl`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_verilog_tokens.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_verilog_tokens.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_verilogParser.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_verilogParser.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_tokenizer.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/tests/test_token_factory.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/tests/test_token_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,23 @@
 
 multi line with extra white space
 
 
 */
 '''
 
+final_comments = '''
+module synth_th1_slaac
+   (XP_IN);
+  input [7:0]XP_IN;
+
+endmodule
+//* Final design comments
+'''
+
 
 class TestVerilogParser(unittest.TestCase):
 
     def run_token_count(self, string):
         tf = TokenFactory()
         running_total = 0
 
@@ -91,15 +100,15 @@
         token = tf.flush()
         if token is not None:
             running_total += 1
         return running_total
 
     def test_counts(self):
         to_run = [(very_simple_multi_line, 24, "very_simple_multi_line"), (very_simple, 35, "very_simple"),
-                  (port_remap, 74, "port_remap"), (comments, 11, "comments")]
+                  (port_remap, 74, "port_remap"), (comments, 11, "comments"), (final_comments, 16, "port_remap")]
         for p in to_run:
             s, c, n = p
             assert c == self.run_token_count(
                 s), "the number of expected tokens did not match up with the number parsed " + n
 
 
 if __name__ == '__main__':
```

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/verilog_token_factory.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/verilog_token_factory.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/tokenizer.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,20 +65,23 @@
         if self.next_token is not None:
             self.token = self.next_token
             self.next_token = None
         else:
             self.token = next(self.generator)
         return self.token
 
-
     def peek(self):
         if self.next_token is not None:
             return self.next_token
         else:
-            self.next_token = next(self.generator)
+            token = next(self.generator)
+            while len(token) >= 2 and (token[0:2] == vt.OPEN_LINE_COMMENT
+                                       or token[0:2] == vt.OPEN_BLOCK_COMMENT):
+                token = next(self.generator)
+            self.next_token = token
             return self.next_token
 
     def generate_tokens(self):
         '''give independent tokens from the token factory'''
 
         try:
             self.line_number = 1
@@ -89,19 +92,16 @@
                         self.line_number += 1
                     result = tf.add_character(ch)
                     if result is not None:
                         yield result
         finally:
             self.input_stream.close()
 
-        #if the input doesn't end in white space there will be one token left in the token factory try and get it.
+        # if the input doesn't end in white space there will be one token left in the token factory try and get it.
 
         result = tf.flush()
         if result != None:
             yield result
 
-    
-
     def close(self):
         if self.input_stream:
             self.input_stream.close()
-
```

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/parser.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,15 +676,15 @@
 
         token = self.next_token()
         assert token == vt.SEMI_COLON, self.error_string(
             vt.SEMI_COLON, "to end instatiation", token)
 
     def parse_defparam_parameters(self):
         '''parse a defparam structure and add the parameters to the associated instance
-        
+
         this looks like:
 
         defparam \\avs_s1_readdata[12]~output .bus_hold = "false"; //single backslash to escape name
 
         and must come after the associated instance (I'm not sure this is the verilog spec but
         it is the way quartus wrote my example and is much simpler)
         '''
@@ -706,15 +706,15 @@
         token = self.next_token()
         assert token == vt.EQUAL, self.error_string(vt.EQUAL, "separate the key from the value in a defparam statement", token)
         token = self.next_token()
         value = token
         token = self.next_token()
         assert token == vt.SEMI_COLON, self.error_string(vt.SEMI_COLON, "to end the defparam statement", token)
         self.set_instance_parameters(instance, params)
-        
+
 
     def parse_parameter_mapping(self):
         params = dict()
         token = self.next_token()
         assert token == vt.OCTOTHORP, self.error_string(
             vt.OCTOTHORP, "to begin parameter mapping", token)
 
@@ -772,15 +772,14 @@
     def parse_port_map_single(self):
         '''acutally does the mapping of the pins'''
         token = self.next_token()
         assert token == vt.DOT, self.error_string(
             vt.DOT, "to start a port mapping instance", token)
 
         token = self.next_token()
-        print(token)
         assert vt.is_valid_identifier(token), self.error_string(
             "valid port identifier", "for port in instantiation port map", token)
         port_name = token
 
         token = self.next_token()
         assert token == vt.OPEN_PARENTHESIS, self.error_string(
             vt.OPEN_PARENTHESIS, "to encapsulate cable name in port mapping", token)
@@ -830,15 +829,15 @@
             vt.SEMI_COLON, "to terminate assign statement", token)
 
         return l_cable, l_left, l_right, r_cable, r_left, r_right
 
     def parse_variable_instantiation(self):
         '''parse the cable name and its indicies if any
         if we are in Intel land then 2 other things can happen.
-        the "cable" is a constant, 
+        the "cable" is a constant,
             attach it to the \\<const0> or \\<const1> cable.
         the cable is inverted,
             create a new cable and an inverter block similar to the assign but with an inversion in the block
         '''
         token = self.next_token()
 
         if token[0] == "1":
```

### Comparing `spydrnet-1.8.3/spydrnet/parsers/verilog/verilog_tokens.py` & `spydrnet-1.9.0/spydrnet/parsers/verilog/verilog_tokens.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/__init__.py` & `spydrnet-1.9.0/spydrnet/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/primatives/parsetab.py` & `spydrnet-1.9.0/spydrnet/parsers/primatives/parsetab.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/primatives/parse_primatives.py` & `spydrnet-1.9.0/spydrnet/parsers/primatives/parse_primatives.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #Future capabilities
 #accept files from other locations for Xilinx
 #support intel/altera devices.
 #support for other vendors
 
 import os
-import SpyDrNet
+import spydrnet as SpyDrNet
 
 VERBOSE = True
 
 class PrimativeParser:
     '''
     Parses primative libraries for use with the tools
```

### Comparing `spydrnet-1.8.3/spydrnet/parsers/edif/tests/test_edif_parser.py` & `spydrnet-1.9.0/spydrnet/parsers/edif/tests/test_edif_parser.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/edif/tests/test_tokenizer.py` & `spydrnet-1.9.0/spydrnet/parsers/edif/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/edif/tokenizer.py` & `spydrnet-1.9.0/spydrnet/parsers/edif/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,12 +176,12 @@
                 "Parse error: Expecting stringToken on line {}, recieved {}".format(
                     self.line_number, self.token
                 )
             )
 
     def is_valid_stringToken(self):
         if re.match(
-            r'"(?:[a-zA-Z]|(?:%[ \t\n\r]*(?:(?:[-+]?\d+[ \t\n\r]+)*(?:[-+]?\d+))*[ \t\n\r]*%)|[0-9]|[\!\#\$\&\'\(\)\*\+\,\-\.\/\:\;\<\=\>\?\@\[\\\]\^\_\`\{\|\}\~]|[ \t\n\r])*"',
+            r'"(?:[a-zA-Z]|(?:%[ \t\n\r]*(?:(?:[-+]?\d+[ \t\n\r]+)*(?:[-+]?\d+))*[ \t\n\r]*%)|[0-9]|[\!\#\$\%\&\'\(\)\*\+\,\-\.\/\:\;\<\=\>\?\@\[\\\]\^\_\`\{\|\}\~]|[ \t\n\r])*"',
             self.token,
         ):
             return True
         return False
```

### Comparing `spydrnet-1.8.3/spydrnet/parsers/edif/parser.py` & `spydrnet-1.9.0/spydrnet/parsers/edif/parser.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/parsers/edif/edif_tokens.py` & `spydrnet-1.9.0/spydrnet/parsers/edif/edif_tokens.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/global_state/tests/test_global_callback.py` & `spydrnet-1.9.0/spydrnet/global_state/tests/test_global_callback.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/global_state/tests/test_global_service.py` & `spydrnet-1.9.0/spydrnet/global_state/tests/test_global_service.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/global_state/global_service.py` & `spydrnet-1.9.0/spydrnet/global_state/global_service.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/global_state/global_callback.py` & `spydrnet-1.9.0/spydrnet/global_state/global_callback.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/release.py` & `spydrnet-1.9.0/spydrnet/release.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/shortcuts/getter.py` & `spydrnet-1.9.0/spydrnet/shortcuts/getter.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_pins.py` & `spydrnet-1.9.0/spydrnet/util/get_pins.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_patterns.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_hierarchical_reference.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_hierarchical_reference.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_hwires.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_hwires.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_instances.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_instances.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_wires.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_wires.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_hinstances.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_hinstances.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_hports.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_hports.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_cables.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_cables.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_definitions.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_definitions.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_pins.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_pins.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_hcables.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_hcables.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_ports.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_ports.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_libraries.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_libraries.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_netlists.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_netlists.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/tests/test_get_hpins.py` & `spydrnet-1.9.0/spydrnet/util/tests/test_get_hpins.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/patterns.py` & `spydrnet-1.9.0/spydrnet/util/patterns.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_definitions.py` & `spydrnet-1.9.0/spydrnet/util/get_definitions.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/hierarchical_reference.py` & `spydrnet-1.9.0/spydrnet/util/hierarchical_reference.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/__init__.py` & `spydrnet-1.9.0/spydrnet/util/__init__.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_instances.py` & `spydrnet-1.9.0/spydrnet/util/get_instances.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_hports.py` & `spydrnet-1.9.0/spydrnet/util/get_hports.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_ports.py` & `spydrnet-1.9.0/spydrnet/util/get_ports.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_libraries.py` & `spydrnet-1.9.0/spydrnet/util/get_libraries.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_hpins.py` & `spydrnet-1.9.0/spydrnet/util/get_hpins.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_hwires.py` & `spydrnet-1.9.0/spydrnet/util/get_hwires.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_wires.py` & `spydrnet-1.9.0/spydrnet/util/get_wires.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_netlists.py` & `spydrnet-1.9.0/spydrnet/util/get_netlists.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_hcables.py` & `spydrnet-1.9.0/spydrnet/util/get_hcables.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_hinstances.py` & `spydrnet-1.9.0/spydrnet/util/get_hinstances.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/library.py` & `spydrnet-1.9.0/spydrnet/util/library.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/util/get_cables.py` & `spydrnet-1.9.0/spydrnet/util/get_cables.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/__init__.py` & `spydrnet-1.9.0/spydrnet/__init__.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/callback/callback_listener.py` & `spydrnet-1.9.0/spydrnet/callback/callback_listener.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/plugins/tests/test_namespace_manager.py` & `spydrnet-1.9.0/spydrnet/plugins/tests/test_namespace_manager.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/plugins/namespace_manager/tests/test_edif_namespace.py` & `spydrnet-1.9.0/spydrnet/plugins/namespace_manager/tests/test_edif_namespace.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/plugins/namespace_manager/default_namespace.py` & `spydrnet-1.9.0/spydrnet/plugins/namespace_manager/default_namespace.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/plugins/namespace_manager/__init__.py` & `spydrnet-1.9.0/spydrnet/plugins/namespace_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/plugins/namespace_manager/edif_namespace.py` & `spydrnet-1.9.0/spydrnet/plugins/namespace_manager/edif_namespace.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/uniquify.py` & `spydrnet-1.9.0/spydrnet/uniquify.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # Copyright 2020 Dallin Skouson, Andrew Keller, Michael Wirthlin
 
-from spydrnet.ir import *
 from collections import deque
+# from spydrnet.ir import *
 
 """Code to make definitions unique throughout a netlist.
 expected parameters,
 uniqify -- Makes all definitions unique below the top instance. definitions that are not referenced below the top instance will not be unique.
 """
 
 
-mod_name_uid = 0
+MOD_NAME_UID = 0
 
 
 def _get_unique_name_modifier():
-    global mod_name_uid
-    str_out = "_sdn_unique_" + str(mod_name_uid)
-    mod_name_uid += 1
+    global MOD_NAME_UID
+    str_out = "_sdn_unique_" + str(MOD_NAME_UID)
+    MOD_NAME_UID += 1
     return str_out
 
 
 def _make_instance_unique(instance):
     """clone the definition and point the reference to the new definition"""
     reference = instance.reference
     lib = instance.reference.library
     index = lib.definitions.index(reference)
     new_def = instance.reference.clone()
-    if instance.reference.name != None:
+    if instance.reference.name is not None:
         name = instance.reference.name
         unique_suffix = _get_unique_name_modifier()
         new_def.name = name + unique_suffix
         if 'EDIF.identifier' in new_def:
             new_def['EDIF.identifier'] = new_def['EDIF.identifier'] + \
                 unique_suffix
     lib.add_definition(new_def, index + 1)
@@ -43,19 +43,19 @@
 
 def uniquify(netlist):
     """Make the instances in the netlist unique
     uniqification is done in place. Each instance will correspond to exactly one definition and each definition will correspond to exactly one instance with the exception of leaf cells.
     Leaf cells are can be instanced unlimited numbers of times. Any netlist elements that are not instantiated by the top instance will not be modified and may retain duplicate instances
     Currently there is no guarantee that the original definition names will be maintained, but it is guaranteed that they will be unique within the scope of all hardware that is below the top instance.
 
-    Renameing is predictable. the string: _sdn_unique_# will be added to the end of the definition names.
+    Renaming is predictable. the string: _sdn_unique_# will be added to the end of the definition names.
 
-    parameter - netlist, the netlist that will be uniquified
+    :param netlist: the netlist that will be uniquified
 
-    returns - no returns
+    :return: void
 
     """
 
     # import pdb; pdb.set_trace()
     # starting with top.
     # top must be unique below top. otherwise we have infinite harware recursion which is does not make much sense.
     instance_queue = deque()
```

### Comparing `spydrnet-1.8.3/spydrnet/clone.py` & `spydrnet-1.9.0/spydrnet/clone.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/compare/tests/test_compare_netlists.py` & `spydrnet-1.9.0/spydrnet/compare/tests/test_compare_netlists.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/compare/compare_netlists.py` & `spydrnet-1.9.0/spydrnet/compare/compare_netlists.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/flatten.py` & `spydrnet-1.9.0/spydrnet/flatten.py`

 * *Files identical despite different names*

### Comparing `spydrnet-1.8.3/spydrnet/testing/test.py` & `spydrnet-1.9.0/spydrnet/testing/test.py`

 * *Files identical despite different names*

