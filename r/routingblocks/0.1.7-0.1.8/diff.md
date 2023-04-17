# Comparing `tmp/routingblocks-0.1.7.tar.gz` & `tmp/routingblocks-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingblocks-0.1.7.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "routingblocks-0.1.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `routingblocks-0.1.7.tar` & `routingblocks-0.1.8.tar`

### file list

```diff
@@ -1,294 +1,293 @@
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.clang-format
--rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.cmake-format
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.github/dependabot.yml
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.gitignore
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.readthedocs.yaml
--rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.7/CMakeLists.txt
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 routingblocks-0.1.7/README.md
--rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/CMakeLists.txt
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Evaluation.h
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Instance.hpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Labeling.h
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/LocalSearch.h
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Operators.h
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Solution.h
--rw-r--r--   0        0        0     4413 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/binding_helpers.hpp
--rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/large_neighborhood.h
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/specializations/ADPTW.h
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/specializations/NIFTW.h
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/utility.h
--rw-r--r--   0        0        0    15827 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Evaluation.cpp
--rw-r--r--   0        0        0     5098 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Instance.cpp
--rw-r--r--   0        0        0     4915 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Labeling.cpp
--rw-r--r--   0        0        0     4063 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/LocalSearch.cpp
--rw-r--r--   0        0        0    10884 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Operators.cpp
--rw-r--r--   0        0        0    22684 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Solution.cpp
--rw-r--r--   0        0        0     1345 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/bindings.cpp
--rw-r--r--   0        0        0    10720 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/large_neighborhood.cpp
--rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/specializations/ADPTW.cpp
--rw-r--r--   0        0        0     2104 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/specializations/NIFTW.cpp
--rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/utility.cpp
--rw-r--r--   0        0        0     3693 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_adptw.pyi
--rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_alns.pyi
--rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_arc.pyi
--rw-r--r--   0        0        0     8809 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_evaluation.pyi
--rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_frvcp.pyi
--rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_insertion_cache.pyi
--rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_instance.pyi
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_local_search.pyi
--rw-r--r--   0        0        0     3834 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_niftw.pyi
--rw-r--r--   0        0        0     4184 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_node.pyi
--rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_node_location.pyi
--rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_random.pyi
--rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_removal_cache.pyi
--rw-r--r--   0        0        0     8771 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_route.pyi
--rw-r--r--   0        0        0    10819 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_solution.pyi
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_types.pyi
--rw-r--r--   0        0        0     1961 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_vertex.pyi
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/make.bat
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/adptw.rst
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/alns.rst
--rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/auxilliary.rst
--rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/concepts.rst
--rw-r--r--   0        0        0     1774 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/conf.py
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/development.rst
--rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/evaluation.rst
--rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/examples.rst
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/extension.rst
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/frvcp.rst
--rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/full_api.rst
--rw-r--r--   0        0        0    28336 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/getting_started.rst
--rw-r--r--   0        0        0      626 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/index.rst
--rw-r--r--   0        0        0     4006 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/instance.rst
--rw-r--r--   0        0        0     2546 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/localsearch.rst
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/niftw.rst
--rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/references.bib
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/references.rst
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/solution.rst
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/__init__.py
--rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/__main__.py
--rw-r--r--   0        0        0     4884 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/alns.py
--rw-r--r--   0        0        0     2929 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/parsing.py
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/__init__.py
--rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/__main__.py
--rw-r--r--   0        0        0    18907 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/alns.py
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/config.json
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/__init__.py
--rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/parsing.py
--rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c101C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c104C10.txt
--rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c202C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c205C10.txt
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r102C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r103C10.txt
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r201C10.txt
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r203C10.txt
--rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc102C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc108C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc201C10.txt
--rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc205C10.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c109_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c201_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c203_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c204_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c205_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c206_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c207_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c208_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r105_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r109_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r110_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r111_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r112_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r208_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r209_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r210_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r211_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc108_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc202_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc208_21.txt
--rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c103C15.txt
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c106C15.txt
--rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c202C15.txt
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c208C15.txt
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r102C15.txt
--rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r105C15.txt
--rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r202C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r209C15.txt
--rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc103C15.txt
--rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc108C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc202C15.txt
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc204C15.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c101C5.txt
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c103C5.txt
--rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c206C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c208C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r104C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r105C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r202C5.txt
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r203C5.txt
--rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc105C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc108C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc204C5.txt
--rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc208C5.txt
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/README.txt
--rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/ShawMoveSelector.py
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/ShawRelatedness.py
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/SpatioTemporalRelatedness.py
--rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/__init__.py
--rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/parameters.py
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/requirements.txt
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/utility/__init__.py
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/utility/algorithms.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/__init__.py
--rw-r--r--   0        0        0     1454 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/__main__.py
--rw-r--r--   0        0        0     4250 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/ils.py
--rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/parsing.py
--rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/CMakeLists.txt
--rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/cmake/CPM.cmake
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/cmake/tools.cmake
--rw-r--r--   0        0        0    22838 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/ADPTWEvaluation.h
--rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/FRVCP.h
--rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/Instance.h
--rw-r--r--   0        0        0    11828 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/LocalSearch.h
--rw-r--r--   0        0        0    10459 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/NIFTWEvaluation.h
--rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/Solution.h
--rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/adaptive_large_neighborhood.hpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/arc.h
--rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/evaluation.h
--rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/insertion_cache.h
--rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/lns_operators.h
--rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/node.h
--rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/InsertStationOperator.h
--rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
--rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/RemoveStationOperator.h
--rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/SwapOperator.h
--rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators.h
--rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/removal_cache.h
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/types.h
--rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/adaptive_priority_list.h
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/algorithms.h
--rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/arc_set.h
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/heap.h
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/iterator_pair.h
--rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/random.h
--rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/vertex.h
--rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/CMakeLists.txt
--rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/CMakeLists.txt
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/LICENSE.txt
--rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
--rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/small_vector/CMakeLists.txt
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/small_vector/LICENSE.txt
--rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/small_vector/small_vector/small_vector.hpp
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/xoshiro/CMakeLists.txt
--rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/xoshiro/LICENSE.txt
--rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/xoshiro/xoshiro/xoshiro.h
--rw-r--r--   0        0        0     3299 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/ADPTWEvaluation.cpp
--rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/FRVCP.cpp
--rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/Instance.cpp
--rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/LocalSearch.cpp
--rw-r--r--   0        0        0     8321 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/NIFTWEvaluation.cpp
--rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/Solution.cpp
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/adaptive_large_neighborbood.cpp
--rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/lns_operators.cpp
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/node.cpp
--rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/operators/InsertStationOperator.cpp
--rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/operators/InterRouteTwoOptOperator.cpp
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/test/CMakeLists.txt
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/test/src/dummy.cpp
--rw-r--r--   0        0        0     1860 2022-11-09 12:37:21.000000 routingblocks-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/__init__.py
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/adptw/__init__.py
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/niftw/__init__.py
--rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/__init__.py
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/best_insert.py
--rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/cluster_removal.py
--rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/move_selectors.py
--rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/related_removal.py
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/route_removal.py
--rw-r--r--   0        0        0     3842 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/station_vicinity_removal.py
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/worst_removal.py
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/utility/__init__.py
--rw-r--r--   0        0        0     5849 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/utility/instance_builder.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/reference/insertion_cache.py
--rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/reference/removal_cache.py
--rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_frvcp.py
--rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_local_search.py
--rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_removal_cache.py
--rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_route_update.py
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/conftest.py
--rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/c101C5.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/r101_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/r201_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/rc101_21.txt
--rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/mock_evaluation.py
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/__init__.py
--rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/parsing.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/__init__.py
--rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_cluster_removal.py
--rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_random_insertion.py
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_random_removal.py
--rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_related_removal.py
--rw-r--r--   0        0        0     1782 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_station_insertion.py
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_station_removal.py
--rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_station_vicinity_removal.py
--rw-r--r--   0        0        0    20635 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_swap.py
--rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_evaluation.py
--rw-r--r--   0        0        0     4590 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_frvcp.py
--rw-r--r--   0        0        0     6422 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_insertion_cache.py
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_large_neighborhood.py
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_lns_helpers.py
--rw-r--r--   0        0        0     2644 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_local_search.py
--rw-r--r--   0        0        0     1990 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_node.py
--rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_removal_cache.py
--rw-r--r--   0        0        0    14114 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_route.py
--rw-r--r--   0        0        0    20300 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_solution.py
--rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 routingblocks-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.clang-format
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.cmake-format
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.gitignore
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.readthedocs.yaml
+-rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.8/CMakeLists.txt
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 routingblocks-0.1.8/README.md
+-rw-r--r--   0        0        0     2858 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/CMakeLists.txt
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Evaluation.h
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Instance.hpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Labeling.h
+-rw-r--r--   0        0        0      409 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/LocalSearch.h
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Operators.h
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Solution.h
+-rw-r--r--   0        0        0     4413 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/binding_helpers.hpp
+-rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/large_neighborhood.h
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/specializations/ADPTW.h
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/specializations/NIFTW.h
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/utility.h
+-rw-r--r--   0        0        0    15827 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Evaluation.cpp
+-rw-r--r--   0        0        0     5098 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Instance.cpp
+-rw-r--r--   0        0        0     4915 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Labeling.cpp
+-rw-r--r--   0        0        0     5942 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/LocalSearch.cpp
+-rw-r--r--   0        0        0    10884 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Operators.cpp
+-rw-r--r--   0        0        0    22684 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Solution.cpp
+-rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/bindings.cpp
+-rw-r--r--   0        0        0    10720 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/large_neighborhood.cpp
+-rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/specializations/ADPTW.cpp
+-rw-r--r--   0        0        0     2104 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/specializations/NIFTW.cpp
+-rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/utility.cpp
+-rw-r--r--   0        0        0     3693 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_adptw.pyi
+-rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_alns.pyi
+-rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_arc.pyi
+-rw-r--r--   0        0        0     8809 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_evaluation.pyi
+-rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_frvcp.pyi
+-rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_insertion_cache.pyi
+-rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_instance.pyi
+-rw-r--r--   0        0        0     6016 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_local_search.pyi
+-rw-r--r--   0        0        0     3834 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_niftw.pyi
+-rw-r--r--   0        0        0     4184 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_node.pyi
+-rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_node_location.pyi
+-rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_random.pyi
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_removal_cache.pyi
+-rw-r--r--   0        0        0     8771 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_route.pyi
+-rw-r--r--   0        0        0    10819 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_solution.pyi
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_types.pyi
+-rw-r--r--   0        0        0     1961 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_vertex.pyi
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/make.bat
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/adptw.rst
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/alns.rst
+-rw-r--r--   0        0        0      651 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/auxilliary.rst
+-rw-r--r--   0        0        0     1804 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/conf.py
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/development.rst
+-rw-r--r--   0        0        0     2690 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/evaluation.rst
+-rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/examples.rst
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/extension.rst
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/frvcp.rst
+-rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/full_api.rst
+-rw-r--r--   0        0        0    28951 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/index.rst
+-rw-r--r--   0        0        0     4006 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/instance.rst
+-rw-r--r--   0        0        0     9539 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/localsearch.rst
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/niftw.rst
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/references.bib
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/references.rst
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/solution.rst
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/__init__.py
+-rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/__main__.py
+-rw-r--r--   0        0        0     4797 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/alns.py
+-rw-r--r--   0        0        0     2929 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/parsing.py
+-rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/__init__.py
+-rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/__main__.py
+-rw-r--r--   0        0        0    18920 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/alns.py
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/config.json
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/__init__.py
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/parsing.py
+-rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c101C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c104C10.txt
+-rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c202C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c205C10.txt
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r102C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r103C10.txt
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r201C10.txt
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r203C10.txt
+-rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc102C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc108C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc201C10.txt
+-rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc205C10.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c109_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c201_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c203_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c204_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c205_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c206_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c207_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c208_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r105_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r109_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r110_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r111_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r112_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r208_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r209_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r210_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r211_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc108_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc202_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc208_21.txt
+-rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c103C15.txt
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c106C15.txt
+-rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c202C15.txt
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c208C15.txt
+-rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r102C15.txt
+-rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r105C15.txt
+-rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r202C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r209C15.txt
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc103C15.txt
+-rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc108C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc202C15.txt
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc204C15.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c101C5.txt
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c103C5.txt
+-rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c206C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c208C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r104C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r105C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r202C5.txt
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r203C5.txt
+-rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc105C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc108C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc204C5.txt
+-rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc208C5.txt
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/README.txt
+-rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/ShawMoveSelector.py
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/ShawRelatedness.py
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/SpatioTemporalRelatedness.py
+-rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/__init__.py
+-rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/parameters.py
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/requirements.txt
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/utility/__init__.py
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/utility/algorithms.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/__init__.py
+-rw-r--r--   0        0        0     1454 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/__main__.py
+-rw-r--r--   0        0        0     4236 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/ils.py
+-rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/parsing.py
+-rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/CMakeLists.txt
+-rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/cmake/CPM.cmake
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/cmake/tools.cmake
+-rw-r--r--   0        0        0    22838 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/ADPTWEvaluation.h
+-rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/FRVCP.h
+-rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/Instance.h
+-rw-r--r--   0        0        0    14652 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/LocalSearch.h
+-rw-r--r--   0        0        0    10459 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/NIFTWEvaluation.h
+-rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/Solution.h
+-rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/adaptive_large_neighborhood.hpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/arc.h
+-rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/evaluation.h
+-rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/insertion_cache.h
+-rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/lns_operators.h
+-rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/node.h
+-rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/InsertStationOperator.h
+-rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
+-rw-r--r--   0        0        0     3126 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/RemoveStationOperator.h
+-rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/SwapOperator.h
+-rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators.h
+-rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/removal_cache.h
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/types.h
+-rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/adaptive_priority_list.h
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/algorithms.h
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/arc_set.h
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/heap.h
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/iterator_pair.h
+-rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/random.h
+-rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/vertex.h
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/CMakeLists.txt
+-rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/LICENSE.txt
+-rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
+-rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/small_vector/CMakeLists.txt
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/small_vector/LICENSE.txt
+-rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/small_vector/small_vector/small_vector.hpp
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/xoshiro/CMakeLists.txt
+-rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/xoshiro/LICENSE.txt
+-rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/xoshiro/xoshiro/xoshiro.h
+-rw-r--r--   0        0        0     3299 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/ADPTWEvaluation.cpp
+-rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/FRVCP.cpp
+-rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/Instance.cpp
+-rw-r--r--   0        0        0     2289 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/LocalSearch.cpp
+-rw-r--r--   0        0        0     8321 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/NIFTWEvaluation.cpp
+-rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/Solution.cpp
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/adaptive_large_neighborbood.cpp
+-rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/lns_operators.cpp
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/node.cpp
+-rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/operators/InsertStationOperator.cpp
+-rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/operators/InterRouteTwoOptOperator.cpp
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/test/CMakeLists.txt
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/test/src/dummy.cpp
+-rw-r--r--   0        0        0     1946 2022-11-09 12:37:21.000000 routingblocks-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/__init__.py
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/adptw/__init__.py
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/niftw/__init__.py
+-rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/__init__.py
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/best_insert.py
+-rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/cluster_removal.py
+-rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/move_selectors.py
+-rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/related_removal.py
+-rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/route_removal.py
+-rw-r--r--   0        0        0     3842 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/station_vicinity_removal.py
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/worst_removal.py
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/utility/__init__.py
+-rw-r--r--   0        0        0     5849 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/utility/instance_builder.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/reference/insertion_cache.py
+-rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/reference/removal_cache.py
+-rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_frvcp.py
+-rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_local_search.py
+-rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_removal_cache.py
+-rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_route_update.py
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/conftest.py
+-rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/c101C5.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/r101_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/r201_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/rc101_21.txt
+-rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/mock_evaluation.py
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/parsing.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/__init__.py
+-rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_cluster_removal.py
+-rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_random_insertion.py
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_random_removal.py
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_related_removal.py
+-rw-r--r--   0        0        0     1821 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_station_insertion.py
+-rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_station_removal.py
+-rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_station_vicinity_removal.py
+-rw-r--r--   0        0        0    20635 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_swap.py
+-rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_evaluation.py
+-rw-r--r--   0        0        0     4629 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_frvcp.py
+-rw-r--r--   0        0        0     6422 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_insertion_cache.py
+-rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_large_neighborhood.py
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_lns_helpers.py
+-rw-r--r--   0        0        0     6343 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_local_search.py
+-rw-r--r--   0        0        0     1990 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_node.py
+-rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_removal_cache.py
+-rw-r--r--   0        0        0    14114 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_route.py
+-rw-r--r--   0        0        0    20300 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_solution.py
+-rw-r--r--   0        0        0     3226 2022-11-09 12:37:21.000000 routingblocks-0.1.8/PKG-INFO
```

### Comparing `routingblocks-0.1.7/.cmake-format` & `routingblocks-0.1.8/.cmake-format`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/.github/workflows/wheels.yml` & `routingblocks-0.1.8/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/.gitignore` & `routingblocks-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/CONTRIBUTING.md` & `routingblocks-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/README.md` & `routingblocks-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/CMakeLists.txt` & `routingblocks-0.1.8/bindings/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cmake_minimum_required(VERSION 3.15)
+cmake_minimum_required(VERSION 3.18)
 include(CheckIPOSupported)
 # To force building for a specific python version, set Python_ROOT_DIR to the respective path.
 # This can be a venv as well.
 # See the FIND_PACKAGE python cmake documentation for details.
 FIND_PACKAGE(Python COMPONENTS Interpreter Development.Module REQUIRED)
 
 message(STATUS "Found python binary: ${Python_EXECUTABLE} (Version ${Python_VERSION})")
@@ -45,22 +45,19 @@
 # Set the compiler standard
 #
 target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_20)
 
 # Create stub file
 file(GLOB stub_files CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/stubs/*.pyi")
 
-# Generate an empty target file
-file(WRITE ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi "")
-
 add_custom_command(
-    OUTPUT ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi
-    COMMAND ${CMAKE_COMMAND} -E echo "Concatenating files..."
-    COMMAND ${CMAKE_COMMAND} -E cat ${stub_files} > "${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi"
-    DEPENDS ${stub_files}
+        OUTPUT ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi
+        COMMAND ${CMAKE_COMMAND} -E echo "Concatenating files..."
+        COMMAND ${CMAKE_COMMAND} -E cat ${stub_files} > "${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi"
+        DEPENDS ${stub_files}
 )
 
 add_custom_target(stub_file ALL DEPENDS ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi)
 add_dependencies(${PROJECT_NAME} stub_file)
 
 INSTALL(TARGETS routingblocks DESTINATION routingblocks)
 INSTALL(FILES ${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks_bindings/binding_helpers.hpp DESTINATION routingblocks/include/routingblocks/)
```

### Comparing `routingblocks-0.1.7/bindings/include/routingblocks_bindings/binding_helpers.hpp` & `routingblocks-0.1.8/bindings/include/routingblocks_bindings/binding_helpers.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/Evaluation.cpp` & `routingblocks-0.1.8/bindings/src/Evaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/Instance.cpp` & `routingblocks-0.1.8/bindings/src/Instance.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/Labeling.cpp` & `routingblocks-0.1.8/bindings/src/Labeling.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/Operators.cpp` & `routingblocks-0.1.8/bindings/src/Operators.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/Solution.cpp` & `routingblocks-0.1.8/bindings/src/Solution.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/bindings.cpp` & `routingblocks-0.1.8/bindings/src/bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     // Evaluation
     bind_evaluation(m);
 
     // Local search
     bind_neighborhood_structures(m);
     bind_local_search(m);
+    bind_pivoting_rule(m);
     // LS Operators
     bind_operators(m);
 
     // Solution
     bind_node(m);
     bind_route(m);
     bind_solution(m);
```

### Comparing `routingblocks-0.1.7/bindings/src/large_neighborhood.cpp` & `routingblocks-0.1.8/bindings/src/large_neighborhood.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/specializations/ADPTW.cpp` & `routingblocks-0.1.8/bindings/src/specializations/ADPTW.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/specializations/NIFTW.cpp` & `routingblocks-0.1.8/bindings/src/specializations/NIFTW.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/src/utility.cpp` & `routingblocks-0.1.8/bindings/src/utility.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_adptw.pyi` & `routingblocks-0.1.8/bindings/stubs/_adptw.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_alns.pyi` & `routingblocks-0.1.8/bindings/stubs/_alns.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_arc.pyi` & `routingblocks-0.1.8/bindings/stubs/_arc.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_evaluation.pyi` & `routingblocks-0.1.8/bindings/stubs/_evaluation.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_frvcp.pyi` & `routingblocks-0.1.8/bindings/stubs/_frvcp.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_insertion_cache.pyi` & `routingblocks-0.1.8/bindings/stubs/_insertion_cache.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_instance.pyi` & `routingblocks-0.1.8/bindings/stubs/_instance.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_niftw.pyi` & `routingblocks-0.1.8/bindings/stubs/_niftw.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_node.pyi` & `routingblocks-0.1.8/bindings/stubs/_node.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_node_location.pyi` & `routingblocks-0.1.8/bindings/stubs/_node_location.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_removal_cache.pyi` & `routingblocks-0.1.8/bindings/stubs/_removal_cache.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_route.pyi` & `routingblocks-0.1.8/bindings/stubs/_route.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_solution.pyi` & `routingblocks-0.1.8/bindings/stubs/_solution.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/bindings/stubs/_vertex.pyi` & `routingblocks-0.1.8/bindings/stubs/_vertex.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/docs/make.bat` & `routingblocks-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/docs/source/alns.rst` & `routingblocks-0.1.8/docs/source/alns.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/docs/source/auxilliary.rst` & `routingblocks-0.1.8/docs/source/auxilliary.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     :undoc-members:
 
 Miscellaneous
 -------------
 
 .. autoapiclass:: routingblocks.Random
     :members:
-    :undoc-members:
+    :undoc-members:
```

### Comparing `routingblocks-0.1.7/docs/source/conf.py` & `routingblocks-0.1.8/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 extensions = [
     'autoapi.extension',
     'sphinx.ext.autodoc',
     'sphinx.ext.autodoc.typehints',
     'sphinx.ext.autosummary',
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
-    'sphinxcontrib.bibtex'
+    'sphinxcontrib.bibtex',
+    'sphinxcontrib.mermaid',
 ]
 
 # AutoAPI
 
 autosummary_generate = True
 autoapi_type = "python"
 autoapi_dirs = [str(routingblocks_import_path)]
```

### Comparing `routingblocks-0.1.7/docs/source/development.rst` & `routingblocks-0.1.8/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/docs/source/evaluation.rst` & `routingblocks-0.1.8/docs/source/evaluation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Note that this class is an interface: it's not meant to be instantiated or used directly. Please use the concrete
 implementations of this interface and helper functions instead. See e.g. :ref:`ADPTW` or :ref:`NIFTW` for examples of
 concrete implementations.
 
 .. warning::
 
-    We recommend implementing a custom Evaluation class by extending the native RoutingBlocks library instead of providing a python implementation for code used beyond prototyping. See `<extension>`_ for more information
+    We recommend implementing a custom Evaluation class by extending the native RoutingBlocks library instead of providing a python implementation for code used beyond prototyping. See `native extensions <https://github.com/tumBAIS/routingblocks-native-extension-example>`_ for an example.
 
 .. autoapiclass:: routingblocks.PyConcatenationBasedEvaluation
     :members:
     :undoc-members:
     :inherited-members:
 
 .. autoapiclass:: routingblocks.PyEvaluation
```

### Comparing `routingblocks-0.1.7/docs/source/getting_started.rst` & `routingblocks-0.1.8/docs/source/getting_started.rst`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 arcs[i['StringID'], j['StringID']] = dict(distance=distance, travel_time=travel_time,
                                                           consumption=consumption)
 
         return vertices, arcs, parameters
 
 .. note::
 
-    The instance format is described in the `supplemental material <https://data.mendeley.com/datasets/h3mrm5dhxw/1>`_ to `Schneider et. al (2014) <https://pubsonline.informs.org/doi/abs/10.1287/trsc.2013.0490>`_.
+    The instance format is described in the `supplemental material <https://data.mendeley.com/datasets/h3mrm5dhxw/1>`_ to :cite:t:`SchneiderStengerEtAl2014`.
 
 Next, we create a RoutingBlocks Instance object from the parsed data:
 
 .. code-block:: python
 
     def create_instance(serialized_vertices, serialized_arcs) -> rb.Instance:
         instance_builder = rb.utility.InstanceBuilder(create_vertex=rb.adptw.create_adptw_vertex,
@@ -105,15 +105,15 @@
 
 We utilize the InstanceBuilder class, offering a convenient way to construct a RoutingBlocks Instance from a set of vertices and arcs. It requires two functions as arguments: a vertex and an arc factory. These functions create a vertex or an arc object based on the data provided by the user. The InstanceBuilder class then handles the registration of vertices and arcs within the Instance object.
 
 Once the instance is created, we can proceed to implement the ILS algorithm. We initiate by creating an Evaluation object, which is responsible for cost calculation and efficient move evaluation. RoutingBlocks already includes an Evaluation class for the EVRP-TW-PR, allowing us to easily use it:
 
 .. note::
 
-        It is possible to implement a custom Evaluation class for custom problem settings (See `Custom problem settings <_custom_problem_settings>`_)
+        It is possible to implement a custom Evaluation class for custom problem settings (See :ref:`Custom problem settings <custom_problem_settings>`).
 
 .. code-block:: python
 
     vehicle_storage_capacity = params['C']
     # Vehicle battery capacity in units of time:
     # battery capacity * inverse refueling rate = battery capacity / refueling rate
     vehicle_battery_capacity_time = params['Q'] * params['g']
@@ -153,30 +153,39 @@
 
 Here, we begin by copying all customers into a single list, which is then shuffled and randomly split at various positions to generate a set of routes. We convert these into RoutingBlocks Route objects using the create_route helper function. This function takes the evaluation function, the instance, and a sequence of vertex IDs as arguments and creates a Route object, adding start and end depots as needed. Finally, we create and return a solution using the list of routes.
 
 Subsequently, we create and configure the local search solver:
 
 .. code-block:: python
 
-    local_search = rb.LocalSearch(instance, evaluation, None)
-    # Configure the local search to use a best-improvement pivoting rule
-    local_search.set_use_best_improvement(True)
+    # Create a best-improvement pivoting rule
+    pivoting_rule = rb.BestImprovementPivotingRule()
+    # Configure the local search - use the best-improvement pivoting rule
+    local_search = rb.LocalSearch(instance, evaluation, None, pivoting_rule)
     # Create a set of allowed arcs
     arc_set = rb.ArcSet(instance.number_of_vertices)
 
     # Create a set of operators that will be used later when calling the local search
     operators = [
         rb.operators.SwapOperator_0_1(instance, arc_set),
         rb.operators.SwapOperator_1_1(instance, arc_set),
         rb.operators.InsertStationOperator(instance),
         rb.operators.RemoveStationOperator(instance),
     ]
 
 
-The local search solver accepts three arguments: the instance, the evaluation used, and a second evaluation object that verifies moves deemed profitable by the first evaluation class. This is beneficial for problems like EVRP-TW-PR, where exact evaluation is costly. By default, the ADPTW Evaluation class implements approximate move evaluation. We can either pass an exact evaluation class here, or we can pass None, which prompts the local search to validate moves by applying them to a solution copy and evaluating the cost based on forward labels. This is what we do here.
+The local search solver accepts four arguments: the instance, the evaluation used, a second evaluation object that verifies moves deemed profitable by the first evaluation class, and a pivoting rule.
+Passing a second evaluation object for verification is beneficial for problems like EVRP-TW-PR, where exact evaluation is costly.
+By default, the ADPTW Evaluation class implements approximate move evaluation. We can either pass an exact evaluation class here,
+or we can pass None, which prompts the local search to validate moves by applying them to a solution copy and evaluating the cost based on forward labels.
+
+The pivoting rule implements the pivoting strategy used by the local search. RoutingBlocks provides three pivoting rules:
+`best improvement <best_improvement_pivoting_rule>`_, `k-best improvement <k_best_improvement_pivoting_rule>`_, and `first improvement <first_improvement_pivoting_rule>`_.
+It is also possible to implement custom pivoting rules (See :ref:`custom pivoting rules <_custom_pivoting_rules>`_).
+The former is the default and is the one we use here. The latter stops the local search as soon as a profitable move is found.
 
 Additionally, we create a set of operators to be used later when invoking the local search. The implementations provided by RoutingBlocks require a set of allowed arcs as an argument. The operator will only consider arcs within this set. By default, all arcs are allowed.
 Executing the local search procedure is as simple as calling
 
 .. code-block:: python
 
     local_search.optimize(solution, operators)
@@ -246,17 +255,16 @@
         evaluation = rb.adptw.Evaluation(vehicle_battery_capacity_time, vehicle_storage_capacity)
         # Set the penalty factors used to penalize violations of the time window, the
         # vehicle capacity, and the charge constraints
         evaluation.overload_penalty_factor = 100.
         evaluation.overcharge_penalty_factor = 100.
         evaluation.time_shift_penalty_factor = 100.
 
-        local_search = rb.LocalSearch(instance, evaluation, None)
-        # Configure the local search to use a best-improvement pivoting rule
-        local_search.set_use_best_improvement(True)
+        pivoting_rule = rb.BestImprovementPivotingRule()
+        local_search = rb.LocalSearch(instance, evaluation, None, pivoting_rule)
         # Create a set of allowed arcs
         arc_set = rb.ArcSet(instance.number_of_vertices)
 
         # Create a set of operators that will be used later when calling the local search
         operators = [
             rb.operators.SwapOperator_0_1(instance, arc_set),
             rb.operators.SwapOperator_1_1(instance, arc_set),
@@ -297,17 +305,16 @@
         evaluation = rb.adptw.Evaluation(vehicle_battery_capacity_time, vehicle_storage_capacity)
         # Set the penalty factors used to penalize violations of the time window, the
         # vehicle capacity, and the charge constraints
         evaluation.overload_penalty_factor = 100.
         evaluation.overcharge_penalty_factor = 100.
         evaluation.time_shift_penalty_factor = 100.
 
-        local_search = rb.LocalSearch(instance, evaluation, None)
-        # Configure the local search to use a best-improvement pivoting rule
-        local_search.set_use_best_improvement(True)
+        pivoting_rule = rb.BestImprovementPivotingRule()
+        local_search = rb.LocalSearch(instance, evaluation, None, pivoting_rule)
         # Create a set of allowed arcs
         arc_set = rb.ArcSet(instance.number_of_vertices)
 
         # Create a set of operators that will be used later when calling the local search
         operators = [
             rb.operators.SwapOperator_0_1(instance, arc_set),
             rb.operators.SwapOperator_1_1(instance, arc_set),
@@ -332,15 +339,15 @@
                                                                         blink_probability=0.1, randgen=randgen)))
         alns.add_destroy_operator(rb.operators.RandomRemovalOperator(randgen))
         alns.add_destroy_operator(rb.operators.WorstRemovalOperator(instance,
                                                                     rb.operators.blink_selector_factory(
                                                                         blink_probability=0.1, randgen=randgen)))
 
 
-We begin with the boilerplate code established for the ILS and add just a few lines to create and configure the ALNS solver. This class is responsible for operator selection and weight adaptation. It takes a random engine and a smoothing factor as arguments. The smoothing factor determines the weight of historical performance when selecting an operator. Next, we create and register destroy and repair operators with the ALNS solver. RoutingBlocks provides a `set of standard operators <alns_operators>`_ out of the box. In this case, we use RandomInsertion, BestInsertion, RandomRemoval, and WorstRemoval. We configure BestInsertion and WorstRemoval to select insertion/removal spots using a blink selection criterion.
+We begin with the boilerplate code established for the ILS and add just a few lines to create and configure the ALNS solver. This class is responsible for operator selection and weight adaptation. It takes a random engine and a smoothing factor as arguments. The smoothing factor determines the weight of historical performance when selecting an operator. Next, we create and register destroy and repair operators with the ALNS solver. RoutingBlocks provides a :ref:`set of standard operators <alns_operators>` out of the box. In this case, we use RandomInsertion, BestInsertion, RandomRemoval, and WorstRemoval. We configure BestInsertion and WorstRemoval to select insertion/removal spots using a blink selection criterion.
 
 We can now employ the ALNS solver to perturb the current solution within the main loop:
 
 
 .. code-block:: python
 
         # Generate a random starting solution
@@ -374,15 +381,15 @@
 
 We employ three essential methods of the ALNS solver:
 
 1. alns.generate: This method selects and applies a destroy and a repair operator to the current solution, modifying it in-place. It returns a tuple of the chosen operators.
 2. alns.collect_score: This method gathers scores for the provided operators. It requires the selected operators and a score as arguments.
 3. alns.adapt_operator_weights: This method adjusts the weights of the operators based on the scores collected during the last period.
 
-For more details on the ALNS solver, see the `documentation <alns>`_. The full code of the ALNS algorithm is available `here <alns_code>`_. A more sophisticated ALNS-based algorithm can be found in the `main repository <https://github.com/tumBAIS/RoutingBlocks/tree/main/examples/evrptw>`_.
+For more details on the ALNS solver, see the :ref:`documentation <alns>`. The full code of the ALNS algorithm is available :ref:`here <https://github.com/tumBAIS/RoutingBlocks/tree/main/examples/alns>`_. A more sophisticated ALNS-based algorithm can be found in the `main repository <https://github.com/tumBAIS/RoutingBlocks/tree/main/examples/evrptw>`_.
 
 Implementing custom operators
 ------------------------------------
 
 The RoutingBlocks library provides a set of standard operators out of the box. However, it is also possible to implement custom local search, destroy, and repair operators. We'll implement a simple RouteRemoval destroy operator as an example:
 
 .. code-block:: python
@@ -535,8 +542,8 @@
              number_of_iterations: int = 100, min_vertex_removal_factor: float = 0.2,
              max_vertex_removal_factor: float = 0.4):
         evaluation = CVRPEvaluation(vehicle_storage_capacity)
         evaluation.load_penalty = 1000.0
 
 .. warning::
 
-    We recommend implementing a custom Evaluation class by extending the native RoutingBlocks library instead of providing a python implementation for code used beyond prototyping. See `<extension>`_ for more information
+    We recommend implementing a custom Evaluation class by extending the native RoutingBlocks library instead of providing a python implementation for code used beyond prototyping. See `native extensions <https://github.com/tumBAIS/routingblocks-native-extension-example>`_ for an example.
```

### Comparing `routingblocks-0.1.7/docs/source/index.rst` & `routingblocks-0.1.8/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 ==========================================
 
 .. toctree::
     :maxdepth: 1
     :caption: Basics
 
     getting_started
-    concepts
 
 .. toctree::
     :maxdepth: 1
     :caption: Components
 
     instance
     solution
```

### Comparing `routingblocks-0.1.7/docs/source/instance.rst` & `routingblocks-0.1.8/docs/source/instance.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/docs/source/solution.rst` & `routingblocks-0.1.8/docs/source/solution.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/README.md` & `routingblocks-0.1.8/examples/README.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/alns/__main__.py` & `routingblocks-0.1.8/examples/alns/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/alns/alns.py` & `routingblocks-0.1.8/examples/alns/alns.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,15 @@
     evaluation = rb.adptw.Evaluation(vehicle_battery_capacity_time, vehicle_storage_capacity)
     # Set the penalty factors used to penalize violations of the time window, the
     # vehicle capacity, and the charge constraints
     evaluation.overload_penalty_factor = 100.
     evaluation.overcharge_penalty_factor = 100.
     evaluation.time_shift_penalty_factor = 100.
 
-    local_search = rb.LocalSearch(instance, evaluation, None)
-    # Configure the local search to use a best-improvement pivoting rule
-    local_search.set_use_best_improvement(True)
+    local_search = rb.LocalSearch(instance, evaluation, None, rb.BestImprovementPivotingRule())
     # Create a set of allowed arcs
     arc_set = rb.ArcSet(instance.number_of_vertices)
 
     # Create a set of operators that will be used later when calling the local search
     operators = [
         rb.operators.SwapOperator_0_1(instance, arc_set),
         rb.operators.SwapOperator_1_1(instance, arc_set),
```

### Comparing `routingblocks-0.1.7/examples/alns/parsing.py` & `routingblocks-0.1.8/examples/alns/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/__main__.py` & `routingblocks-0.1.8/examples/evrptw/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/alns.py` & `routingblocks-0.1.8/examples/evrptw/alns.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         # Initialize random engines
         self._random = routingblocks.Random(seed)
         self._py_random = random.Random(seed)
 
         # Create and configure algorithmic components
         self._adaptive_large_neighborhood = routingblocks.AdaptiveLargeNeighborhood(self._random,
                                                                                     self._params.adaptive_smoothing_factor)
-        self._local_search = routingblocks.LocalSearch(self._cpp_instance, evaluation, None)
-        self._local_search.set_use_best_improvement(self._params.use_best_improvement)
+        self._local_search = routingblocks.LocalSearch(self._cpp_instance, evaluation, None,
+                                                       routingblocks.BestImprovementPivotingRule())
 
         # Compute the granular neighborhood
         self._reduced_arc_set = create_reduced_arc_set(self._cpp_instance, self._py_instance, self._params.granularity)
 
         # Create specialized FRVCP solver
         self._frvcp = routingblocks.adptw.FRVCP(self._cpp_instance, self._py_instance.parameters.battery_capacity_time)
```

### Comparing `routingblocks-0.1.7/examples/evrptw/config.json` & `routingblocks-0.1.8/examples/evrptw/config.json`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instance/interface.py` & `routingblocks-0.1.8/examples/evrptw/instance/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instance/models.py` & `routingblocks-0.1.8/examples/evrptw/instance/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instance/parsing.py` & `routingblocks-0.1.8/examples/evrptw/instance/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c101C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c101C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c104C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c104C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c202C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c202C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c205C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r102C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r103C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r103C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r201C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r203C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r203C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc102C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc108C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc108C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc201C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc205C10.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c101_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c102_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c103_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c104_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c105_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c106_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c107_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c108_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c109_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c201_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c202_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c203_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c204_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c205_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c206_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c207_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c208_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r101_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r102_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r103_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r104_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r105_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r106_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r107_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r108_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r109_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r110_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r110_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r111_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r111_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r112_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r112_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r201_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r202_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r203_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r204_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r205_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r206_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r207_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r208_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r209_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r209_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r210_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r210_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r211_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r211_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc101_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc102_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc103_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc104_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc105_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc106_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc107_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc108_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc201_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc202_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc203_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc204_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc205_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc206_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc207_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc208_21.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c103C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c106C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c106C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c202C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c208C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c208C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r102C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r102C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r105C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r105C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r202C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r209C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r209C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc103C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc108C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc108C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc202C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc204C15.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc204C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c101C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c103C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c103C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c206C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c206C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c208C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r104C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r104C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r105C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r202C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r202C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r203C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r203C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc105C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc108C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc108C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc204C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc204C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc208C5.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/instances/evrptw/README.txt` & `routingblocks-0.1.8/examples/evrptw/instances/evrptw/README.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/operators/ShawMoveSelector.py` & `routingblocks-0.1.8/examples/evrptw/operators/ShawMoveSelector.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/operators/ShawRelatedness.py` & `routingblocks-0.1.8/examples/evrptw/operators/ShawRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/operators/SpatioTemporalRelatedness.py` & `routingblocks-0.1.8/examples/evrptw/operators/SpatioTemporalRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/operators/__init__.py` & `routingblocks-0.1.8/examples/evrptw/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/evrptw/parameters.py` & `routingblocks-0.1.8/examples/evrptw/parameters.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/ils/__main__.py` & `routingblocks-0.1.8/examples/ils/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/examples/ils/ils.py` & `routingblocks-0.1.8/examples/ils/ils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,16 @@
     evaluation = rb.adptw.Evaluation(vehicle_battery_capacity_time, vehicle_storage_capacity)
     # Set the penalty factors used to penalize violations of the time window, the
     # vehicle capacity, and the charge constraints
     evaluation.overload_penalty_factor = 100.
     evaluation.overcharge_penalty_factor = 100.0
     evaluation.time_shift_penalty_factor = 100.0
 
-    local_search = rb.LocalSearch(instance, evaluation, None)
     # Configure the local search to use a best-improvement pivoting rule
-    local_search.set_use_best_improvement(True)
+    local_search = rb.LocalSearch(instance, evaluation, None, rb.BestImprovementPivotingRule())
     # Create a set of allowed arcs
     arc_set = rb.ArcSet(instance.number_of_vertices)
 
     # Create a set of operators that will be used later when calling the local search
     operators = [
         rb.operators.SwapOperator_0_1(instance, arc_set),
         rb.operators.SwapOperator_1_1(instance, arc_set),
```

### Comparing `routingblocks-0.1.7/examples/ils/parsing.py` & `routingblocks-0.1.8/examples/ils/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/CMakeLists.txt` & `routingblocks-0.1.8/native/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/cmake/CPM.cmake` & `routingblocks-0.1.8/native/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/cmake/tools.cmake` & `routingblocks-0.1.8/native/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/ADPTWEvaluation.h` & `routingblocks-0.1.8/native/include/routingblocks/ADPTWEvaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/FRVCP.h` & `routingblocks-0.1.8/native/include/routingblocks/FRVCP.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/Instance.h` & `routingblocks-0.1.8/native/include/routingblocks/Instance.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/LocalSearch.h` & `routingblocks-0.1.8/native/include/routingblocks/LocalSearch.h`

 * *Files 23% similar despite different names*

```diff
@@ -65,25 +65,23 @@
 
         virtual void finalize_search() = 0;
 
         virtual ~Operator() = default;
     };
 
     template <class move_t>
-    concept specializes_exact_cost_computation
-        = requires(move_t move) {
-              move.evaluate_exact(std::declval<routingblocks::Evaluation&>(),
-                                  std::declval<const Instance&>(), std::declval<const Solution&>());
-          };
+    concept specializes_exact_cost_computation = requires(move_t move) {
+        move.evaluate_exact(std::declval<routingblocks::Evaluation&>(),
+                            std::declval<const Instance&>(), std::declval<const Solution&>());
+    };
 
     template <class operator_t>
-    concept specializes_move_construction
-        = requires(operator_t op) {
-              op.create_move(std::declval<NodeLocation>(), std::declval<NodeLocation>());
-          };
+    concept specializes_move_construction = requires(operator_t op) {
+        op.create_move(std::declval<NodeLocation>(), std::declval<NodeLocation>());
+    };
 
     template <class Impl> class GeneratorArcMove : public Move {
         NodeLocation _origin, _target;
 
       public:
         GeneratorArcMove(NodeLocation origin, NodeLocation target)
             : _origin(origin), _target(target) {}
@@ -236,39 +234,115 @@
         auto create_move(NodeLocation origin, NodeLocation target) const {
             return move_t(origin, target);
         }
 
         void finalize_search() override {}
     };
 
+    class PivotingRule {
+      public:
+        virtual ~PivotingRule() = default;
+        virtual bool continue_search(const std::shared_ptr<Move>& found_improving_move,
+                                     cost_t exact_cost, const Solution& solution)
+            = 0;
+        virtual std::shared_ptr<Move> select_move(const Solution& solution) = 0;
+    };
+
+    class FirstImprovementPivotingRule : public PivotingRule {
+      private:
+        std::shared_ptr<Move> _first_improving_move = nullptr;
+
+      public:
+        bool continue_search(const std::shared_ptr<Move>& found_improving_move, cost_t exact_cost,
+                             const Solution& solution) override {
+            _first_improving_move = found_improving_move;
+            return false;
+        }
+
+        std::shared_ptr<Move> select_move(const Solution& solution) override {
+            // Release the move
+            std::shared_ptr<Move> move = std::move(_first_improving_move);
+            return move;
+        }
+    };
+
+    class BestImprovementPivotingRule : public PivotingRule {
+      private:
+        std::shared_ptr<Move> _best_improving_move = nullptr;
+        cost_t _best_improving_move_cost = -1e-2;
+
+      public:
+        bool continue_search(const std::shared_ptr<Move>& found_improving_move, cost_t exact_cost,
+                             const Solution&) override {
+            if (exact_cost < _best_improving_move_cost) {
+                _best_improving_move = found_improving_move;
+                _best_improving_move_cost = exact_cost;
+            }
+            return true;
+        }
+
+        std::shared_ptr<Move> select_move(const Solution&) override {
+            // Release the move
+            std::shared_ptr<Move> move = std::move(_best_improving_move);
+            // Reset the cost
+            _best_improving_move_cost = std::numeric_limits<cost_t>::max();
+            return move;
+        }
+    };
+
+    class KBestImprovementPivotingRule : public PivotingRule {
+      private:
+        std::shared_ptr<Move> _best_improving_move = nullptr;
+        cost_t _best_improving_move_cost = -1e-2;
+        size_t _moves_seen = 0;
+        size_t _k;
+
+      public:
+        KBestImprovementPivotingRule(size_t k) : _k(k) {}
+
+        bool continue_search(const std::shared_ptr<Move>& found_improving_move, cost_t exact_cost,
+                             const Solution&) override {
+            if (exact_cost < _best_improving_move_cost) {
+                _best_improving_move = found_improving_move;
+                _best_improving_move_cost = exact_cost;
+            }
+            return (++_moves_seen) < _k;
+        }
+
+        std::shared_ptr<Move> select_move(const Solution&) override {
+            // Release the move
+            std::shared_ptr<Move> move = std::move(_best_improving_move);
+            // Reset the cost
+            _best_improving_move_cost = std::numeric_limits<cost_t>::max();
+            _moves_seen = 0;
+            return move;
+        }
+    };
+
     // Main local learch structure
     class LocalSearch {
         using eval_t = routingblocks::Evaluation;
         using solution_t = routingblocks::Solution;
 
       private:
         const routingblocks::Instance* _instance;  // Problem instance
         std::shared_ptr<eval_t> _evaluation;
         std::shared_ptr<eval_t> _exact_evaluation;
         std::vector<Operator*> _operators;
+        PivotingRule* _pivoting_rule;
 
         int loopID = 0;  // Current loop index
-        bool use_best_improvement = false;
 
         solution_t _current_solution;
 
         void _apply_move(const Move& move);
         cost_t _test_move(const Move& move);
         [[nodiscard]] std::shared_ptr<Move> _explore_neighborhood();
 
       public:
-        void set_use_best_improvement(bool best_improvement) {
-            this->use_best_improvement = best_improvement;
-        }
-
         // Run the local search with the specified penalty values
         template <class ForwardIterator>
             requires std::same_as<typename ForwardIterator::value_type, Operator*>
         void run(solution_t& sol, ForwardIterator operators_begin, ForwardIterator operators_end) {
             _current_solution = std::move(sol);
 
             // TODO Figure out a better way to do this.
@@ -284,15 +358,15 @@
             }
 
             sol = std::move(_current_solution);
         }
 
         // Constructor
         LocalSearch(const routingblocks::Instance& instance, std::shared_ptr<eval_t> evaluation,
-                    std::shared_ptr<eval_t> exact_evaluation);
+                    std::shared_ptr<eval_t> exact_evaluation, PivotingRule* pivoting_rule);
     };
 
 }  // namespace routingblocks
 
 std::ostream& operator<<(std::ostream& out, const routingblocks::Node& node);
 
 #endif
```

### Comparing `routingblocks-0.1.7/native/include/routingblocks/NIFTWEvaluation.h` & `routingblocks-0.1.8/native/include/routingblocks/NIFTWEvaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/Solution.h` & `routingblocks-0.1.8/native/include/routingblocks/Solution.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/adaptive_large_neighborhood.hpp` & `routingblocks-0.1.8/native/include/routingblocks/adaptive_large_neighborhood.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/arc.h` & `routingblocks-0.1.8/native/include/routingblocks/arc.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/evaluation.h` & `routingblocks-0.1.8/native/include/routingblocks/evaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/insertion_cache.h` & `routingblocks-0.1.8/native/include/routingblocks/insertion_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/lns_operators.h` & `routingblocks-0.1.8/native/include/routingblocks/lns_operators.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/node.h` & `routingblocks-0.1.8/native/include/routingblocks/node.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/operators/InsertStationOperator.h` & `routingblocks-0.1.8/native/include/routingblocks/operators/InsertStationOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/operators/InterRouteTwoOptOperator.h` & `routingblocks-0.1.8/native/include/routingblocks/operators/InterRouteTwoOptOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/operators/RemoveStationOperator.h` & `routingblocks-0.1.8/native/include/routingblocks/operators/RemoveStationOperator.h`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         const Instance& _instance;
 
         [[nodiscard]] SolutionArcIterator _recover_move(const Solution& solution,
                                                         const RemoveStationMove* move) const {
             if (move) {
                 auto [route, after_node] = to_iter(move->_node, solution);
                 auto arc_iterator = SolutionArcIterator(solution, {route, after_node});
-                ++arc_iterator;
                 return arc_iterator;
             } else {
                 return SolutionArcIterator(solution, {solution.begin(), solution.begin()->begin()});
             }
         };
 
       public:
```

### Comparing `routingblocks-0.1.7/native/include/routingblocks/operators/SwapOperator.h` & `routingblocks-0.1.8/native/include/routingblocks/operators/SwapOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/operators.h` & `routingblocks-0.1.8/native/include/routingblocks/operators.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/removal_cache.h` & `routingblocks-0.1.8/native/include/routingblocks/removal_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/utility/adaptive_priority_list.h` & `routingblocks-0.1.8/native/include/routingblocks/utility/adaptive_priority_list.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/utility/algorithms.h` & `routingblocks-0.1.8/native/include/routingblocks/utility/algorithms.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/utility/arc_set.h` & `routingblocks-0.1.8/native/include/routingblocks/utility/arc_set.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/utility/heap.h` & `routingblocks-0.1.8/native/include/routingblocks/utility/heap.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/utility/iterator_pair.h` & `routingblocks-0.1.8/native/include/routingblocks/utility/iterator_pair.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/utility/random.h` & `routingblocks-0.1.8/native/include/routingblocks/utility/random.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/include/routingblocks/vertex.h` & `routingblocks-0.1.8/native/include/routingblocks/vertex.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/lib/dynamic_bitset/LICENSE.txt` & `routingblocks-0.1.8/native/lib/dynamic_bitset/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp` & `routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h` & `routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/lib/small_vector/LICENSE.txt` & `routingblocks-0.1.8/native/lib/small_vector/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/lib/small_vector/small_vector/small_vector.hpp` & `routingblocks-0.1.8/native/lib/small_vector/small_vector/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/lib/xoshiro/LICENSE.txt` & `routingblocks-0.1.8/native/lib/xoshiro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/lib/xoshiro/xoshiro/xoshiro.h` & `routingblocks-0.1.8/native/lib/xoshiro/xoshiro/xoshiro.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/ADPTWEvaluation.cpp` & `routingblocks-0.1.8/native/src/ADPTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/Instance.cpp` & `routingblocks-0.1.8/native/src/Instance.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/LocalSearch.cpp` & `routingblocks-0.1.8/native/src/LocalSearch.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 #include <routingblocks/FRVCP.h>
 #include <routingblocks/LocalSearch.h>
 #include <routingblocks/Solution.h>
 
-#include <algorithm>
-#include <chrono>
 #include <set>
-#include <vector>
 
 namespace routingblocks {
     std::shared_ptr<Move> LocalSearch::_explore_neighborhood() {
-        std::shared_ptr<Move> next_move, best_move;
+        std::shared_ptr<Move> next_move;
         // Discard moves that do not have an impact on the objective function to avoid
         // routing errors.
-        auto best_cost = -1e-2;
+        bool skip_remaining_operators = false;
         for (auto& next_op : _operators) {
             next_op->prepare_search(_current_solution);
             while (true) {
                 next_move = next_op->find_next_improving_move(*_evaluation, _current_solution,
                                                               next_move.get());
                 if (next_move == nullptr) {
                     break;
-                } else if (auto cost = _test_move(*next_move); cost < best_cost) {
-                    if (!use_best_improvement) {
-                        return next_move;
+                } else if (auto cost = _test_move(*next_move); cost < -1e-2) {
+                    if (!_pivoting_rule->continue_search(next_move, cost, _current_solution)) {
+                        skip_remaining_operators = true;
+                        break;
                     }
-                    best_cost = cost;
-                    best_move = std::move(next_move);
                 }
             }
             next_op->finalize_search();
+            if (skip_remaining_operators) {
+                break;
+            }
         }
-        return best_move;
+        return _pivoting_rule->select_move(_current_solution);
     }
 
     cost_t LocalSearch::_test_move(const Move& move) {
         if (_exact_evaluation) {
             return move.get_cost_delta(*_exact_evaluation, *_instance, _current_solution);
         } else {
             Solution sol = _current_solution;
@@ -43,14 +42,15 @@
         }
     }
 
     void LocalSearch::_apply_move(const Move& move) { move.apply(*_instance, _current_solution); }
 
     LocalSearch::LocalSearch(const routingblocks::Instance& instance,
                              std::shared_ptr<eval_t> evaluation,
-                             std::shared_ptr<eval_t> exact_evaluation)
+                             std::shared_ptr<eval_t> exact_evaluation, PivotingRule* pivoting_rule)
         : _instance(&instance),
           _evaluation(std::move(evaluation)),
           _exact_evaluation(std::move(exact_evaluation)),
+          _pivoting_rule(pivoting_rule),
           _current_solution(_evaluation, *_instance, _instance->FleetSize()) {}
 
 }  // namespace routingblocks
```

### Comparing `routingblocks-0.1.7/native/src/NIFTWEvaluation.cpp` & `routingblocks-0.1.8/native/src/NIFTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/Solution.cpp` & `routingblocks-0.1.8/native/src/Solution.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/lns_operators.cpp` & `routingblocks-0.1.8/native/src/lns_operators.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/node.cpp` & `routingblocks-0.1.8/native/src/node.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/operators/InsertStationOperator.cpp` & `routingblocks-0.1.8/native/src/operators/InsertStationOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/src/operators/InterRouteTwoOptOperator.cpp` & `routingblocks-0.1.8/native/src/operators/InterRouteTwoOptOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/native/test/CMakeLists.txt` & `routingblocks-0.1.8/native/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/pyproject.toml` & `routingblocks-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core>=0.2.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "RoutingBlocks"
-version = "0.1.7"
+version = "0.1.8"
 description = "A package for the implementation of vehicle routing problems with intermediate stops"
 readme = "README.md"
 authors = [
     { name = "Patrick Sean Klein", email = "patrick.sean.klein@tum.de" },
 ]
 requires-python = ">=3.8"
 classifiers = [
@@ -20,20 +20,22 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-benchmark", "pytest-randomly", "pydantic"]
-docs = ["sphinx", "sphinx-rtd-theme", "sphinx-autodoc-typehints", "sphinx-autoapi"]
+docs = ["sphinx", "sphinx-rtd-theme", "sphinx-autodoc-typehints", "sphinx-autoapi", "sphinxcontrib-bibtex",
+    "sphinxcontrib-mermaid"]
 examples = ["click", "pydantic"]
 
 
 [tool.scikit-build]
 wheel.expand-macos-universal-tags = true
+cmake.minimum-version = "3.18.0"
 
 [tool.pytest.ini_options]
 testpaths = [
     "test/tests/",
 ]
 
 [tool.cibuildwheel]
```

### Comparing `routingblocks-0.1.7/routingblocks/operators/__init__.py` & `routingblocks-0.1.8/routingblocks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/operators/best_insert.py` & `routingblocks-0.1.8/routingblocks/operators/best_insert.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/operators/cluster_removal.py` & `routingblocks-0.1.8/routingblocks/operators/cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/operators/move_selectors.py` & `routingblocks-0.1.8/routingblocks/operators/move_selectors.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/operators/related_removal.py` & `routingblocks-0.1.8/routingblocks/operators/related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/operators/route_removal.py` & `routingblocks-0.1.8/routingblocks/operators/route_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/operators/station_vicinity_removal.py` & `routingblocks-0.1.8/routingblocks/operators/station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/operators/worst_removal.py` & `routingblocks-0.1.8/routingblocks/operators/worst_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/routingblocks/utility/instance_builder.py` & `routingblocks-0.1.8/routingblocks/utility/instance_builder.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/benchmarks/reference/insertion_cache.py` & `routingblocks-0.1.8/test/tests/benchmarks/reference/insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/benchmarks/reference/removal_cache.py` & `routingblocks-0.1.8/test/tests/benchmarks/reference/removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_frvcp.py` & `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_local_search.py` & `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_local_search.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_removal_cache.py` & `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_route_update.py` & `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_route_update.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/fixtures/__init__.py` & `routingblocks-0.1.8/test/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/fixtures/data/c101C5.txt` & `routingblocks-0.1.8/test/tests/fixtures/data/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/fixtures/data/c101_21.txt` & `routingblocks-0.1.8/test/tests/fixtures/data/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/fixtures/data/r101_21.txt` & `routingblocks-0.1.8/test/tests/fixtures/data/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/fixtures/data/r201_21.txt` & `routingblocks-0.1.8/test/tests/fixtures/data/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/fixtures/data/rc101_21.txt` & `routingblocks-0.1.8/test/tests/fixtures/data/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/fixtures/mock_evaluation.py` & `routingblocks-0.1.8/test/tests/fixtures/mock_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/helpers/interface.py` & `routingblocks-0.1.8/test/tests/helpers/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/helpers/models.py` & `routingblocks-0.1.8/test/tests/helpers/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/helpers/parsing.py` & `routingblocks-0.1.8/test/tests/helpers/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/operators/test_cluster_removal.py` & `routingblocks-0.1.8/test/tests/operators/test_cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/operators/test_random_insertion.py` & `routingblocks-0.1.8/test/tests/operators/test_random_insertion.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/operators/test_random_removal.py` & `routingblocks-0.1.8/test/tests/operators/test_random_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/operators/test_related_removal.py` & `routingblocks-0.1.8/test/tests/operators/test_related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/operators/test_station_insertion.py` & `routingblocks-0.1.8/test/tests/operators/test_station_insertion.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,11 +32,11 @@
     evaluation.time_shift_penalty_factor = 0.
 
     solution = recreate_solution(evaluation=evaluation, instance=instance)
     route = solution[0]
     assert not route.feasible
     assert route.cost_components[2] > 0
     station_insertion_operator = evrptw.operators.InsertStationOperator(instance)
-    ls = evrptw.LocalSearch(instance, evaluation, None)
+    ls = evrptw.LocalSearch(instance, evaluation, None, evrptw.FirstImprovementPivotingRule())
     ls.optimize(solution, [station_insertion_operator])
     # Charge penalty should be 0.
     assert route.cost_components[2] == 0.
```

### Comparing `routingblocks-0.1.7/test/tests/operators/test_station_vicinity_removal.py` & `routingblocks-0.1.8/test/tests/operators/test_station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/operators/test_swap.py` & `routingblocks-0.1.8/test/tests/operators/test_swap.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_evaluation.py` & `routingblocks-0.1.8/test/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_frvcp.py` & `routingblocks-0.1.8/test/tests/test_frvcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     # Generate test routes
     total_routes_considered = 0
     start_time = time.process_time()
     timeout = lambda: (time.process_time() - start_time) >= 30
     while True:
         picked_customers = random.choices([x.vertex_id for x in customers], k=random.randint(1, 10))
 
-        local_search = evrptw.LocalSearch(instance, evaluation, None)
+        local_search = evrptw.LocalSearch(instance, evaluation, None, evrptw.FirstImprovementPivotingRule())
         sol = evrptw.Solution(evaluation, instance,
                               [evrptw.create_route(evaluation, instance, picked_customers),
                                *(evrptw.Route(evaluation, instance) for _ in range(instance.fleet_size - 1))])
         local_search.optimize(sol, [routingblocks.operators.SwapOperator_0_1(instance, None)])
         for r in sol:
             if r.empty:
                 continue
```

### Comparing `routingblocks-0.1.7/test/tests/test_insertion_cache.py` & `routingblocks-0.1.8/test/tests/test_insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_large_neighborhood.py` & `routingblocks-0.1.8/test/tests/test_large_neighborhood.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_lns_helpers.py` & `routingblocks-0.1.8/test/tests/test_lns_helpers.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_node.py` & `routingblocks-0.1.8/test/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_removal_cache.py` & `routingblocks-0.1.8/test/tests/test_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_route.py` & `routingblocks-0.1.8/test/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/test/tests/test_solution.py` & `routingblocks-0.1.8/test/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.7/PKG-INFO` & `routingblocks-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingblocks
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for the implementation of vehicle routing problems with intermediate stops
 Author-Email: Patrick Sean Klein <patrick.sean.klein@tum.de>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,16 @@
 Requires-Dist: pytest-benchmark; extra == "test"
 Requires-Dist: pytest-randomly; extra == "test"
 Requires-Dist: pydantic; extra == "test"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: sphinxcontrib-mermaid; extra == "docs"
 Requires-Dist: click; extra == "examples"
 Requires-Dist: pydantic; extra == "examples"
 Description-Content-Type: text/markdown
 
 # RoutingBlocks
 
 `RoutingBlocks` is an open-source Python package for the implementation of algorithms for Vehicle Routing Problems with
```

