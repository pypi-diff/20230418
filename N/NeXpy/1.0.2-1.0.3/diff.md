# Comparing `tmp/NeXpy-1.0.2.tar.gz` & `tmp/NeXpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeXpy-1.0.2.tar", last modified: Tue Apr  4 21:07:54 2023, max compression
+gzip compressed data, was "NeXpy-1.0.3.tar", last modified: Tue Apr 18 15:01:55 2023, max compression
```

## Comparing `NeXpy-1.0.2.tar` & `NeXpy-1.0.3.tar`

### file list

```diff
@@ -1,254 +1,256 @@
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.786257 NeXpy-1.0.2/
--rw-r--r--   0 rosborn    (504) 660979062      672 2022-11-15 16:30:46.000000 NeXpy-1.0.2/.gitattributes
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.737340 NeXpy-1.0.2/.github/
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.741587 NeXpy-1.0.2/.github/workflows/
--rw-r--r--   0 rosborn    (504) 660979062      654 2023-02-27 16:28:59.000000 NeXpy-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 rosborn    (504) 660979062      577 2023-02-23 19:22:11.000000 NeXpy-1.0.2/.gitignore
--rw-r--r--   0 rosborn    (504) 660979062     2378 2022-11-15 16:30:46.000000 NeXpy-1.0.2/COPYING
--rw-r--r--   0 rosborn    (504) 660979062     5299 2023-04-04 21:07:54.786464 NeXpy-1.0.2/PKG-INFO
--rw-r--r--   0 rosborn    (504) 660979062     4283 2023-02-23 19:59:31.000000 NeXpy-1.0.2/README.md
--rw-r--r--   0 rosborn    (504) 660979062     7060 2023-02-23 19:59:31.000000 NeXpy-1.0.2/README.rst
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.742094 NeXpy-1.0.2/conda-recipe/
--rw-r--r--   0 rosborn    (504) 660979062       51 2022-11-15 16:30:46.000000 NeXpy-1.0.2/conda-recipe/bld.bat
--rw-r--r--   0 rosborn    (504) 660979062      103 2022-11-15 16:30:46.000000 NeXpy-1.0.2/conda-recipe/build.sh
--rw-r--r--   0 rosborn    (504) 660979062      999 2023-04-04 20:52:54.000000 NeXpy-1.0.2/conda-recipe/meta.yaml
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.742439 NeXpy-1.0.2/doc/
--rw-r--r--   0 rosborn    (504) 660979062     5643 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/Makefile
--rw-r--r--   0 rosborn    (504) 660979062     5103 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/make.bat
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.744019 NeXpy-1.0.2/doc/source/
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.744172 NeXpy-1.0.2/doc/source/_static/
--rw-r--r--   0 rosborn    (504) 660979062      102 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/_static/__ignore__.txt
--rw-r--r--   0 rosborn    (504) 660979062     8265 2023-02-23 19:59:31.000000 NeXpy-1.0.2/doc/source/conf.py
--rw-r--r--   0 rosborn    (504) 660979062      526 2023-02-23 19:59:31.000000 NeXpy-1.0.2/doc/source/examples.rst
--rw-r--r--   0 rosborn    (504) 660979062    90022 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/favicon.ico
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.749968 NeXpy-1.0.2/doc/source/images/
--rw-r--r--   0 rosborn    (504) 660979062    14509 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/axis-limits-bar.png
--rw-r--r--   0 rosborn    (504) 660979062   684819 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/customize-panel.png
--rw-r--r--   0 rosborn    (504) 660979062   432231 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/limits-panel.png
--rw-r--r--   0 rosborn    (504) 660979062   705341 2023-02-23 19:59:31.000000 NeXpy-1.0.2/doc/source/images/nexpy-fits.png
--rw-r--r--   0 rosborn    (504) 660979062   364457 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/nexpy-gui.png
--rw-r--r--   0 rosborn    (504) 660979062    40568 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/nexpy-logo.png
--rw-r--r--   0 rosborn    (504) 660979062    43638 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/options-tab.png
--rw-r--r--   0 rosborn    (504) 660979062   496144 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/projection-panel.png
--rw-r--r--   0 rosborn    (504) 660979062    20559 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/projection-tab.png
--rw-r--r--   0 rosborn    (504) 660979062   590841 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/scan-panel.png
--rw-r--r--   0 rosborn    (504) 660979062   598861 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/signal-tab.png
--rw-r--r--   0 rosborn    (504) 660979062    73587 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/simple-plot.png
--rw-r--r--   0 rosborn    (504) 660979062   308220 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/skewed-axis.png
--rw-r--r--   0 rosborn    (504) 660979062    19535 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/x-tab.png
--rw-r--r--   0 rosborn    (504) 660979062    29737 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/y-tab.png
--rw-r--r--   0 rosborn    (504) 660979062    20833 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/z-tab.png
--rw-r--r--   0 rosborn    (504) 660979062     8104 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/images/z-toolbar.png
--rw-r--r--   0 rosborn    (504) 660979062       30 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/includeme.rst
--rw-r--r--   0 rosborn    (504) 660979062     1093 2023-02-23 19:59:31.000000 NeXpy-1.0.2/doc/source/index.rst
--rw-r--r--   0 rosborn    (504) 660979062    59250 2023-03-23 22:41:46.000000 NeXpy-1.0.2/doc/source/pythongui.rst
--rw-r--r--   0 rosborn    (504) 660979062    44651 2023-02-23 19:59:31.000000 NeXpy-1.0.2/doc/source/pythonshell.rst
--rw-r--r--   0 rosborn    (504) 660979062     2845 2023-02-23 19:59:31.000000 NeXpy-1.0.2/doc/source/readers.rst
--rw-r--r--   0 rosborn    (504) 660979062      417 2022-11-15 16:30:46.000000 NeXpy-1.0.2/doc/source/treeapi.rst
--rw-r--r--   0 rosborn    (504) 660979062      181 2022-11-15 16:30:46.000000 NeXpy-1.0.2/pyproject.toml
--rw-r--r--   0 rosborn    (504) 660979062     1604 2023-04-04 21:07:54.787074 NeXpy-1.0.2/setup.cfg
--rwxr-xr-x   0 rosborn    (504) 660979062      410 2022-11-15 16:30:46.000000 NeXpy-1.0.2/setup.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.738127 NeXpy-1.0.2/src/
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.751342 NeXpy-1.0.2/src/NeXpy.egg-info/
--rw-r--r--   0 rosborn    (504) 660979062     5299 2023-04-04 21:07:54.000000 NeXpy-1.0.2/src/NeXpy.egg-info/PKG-INFO
--rw-r--r--   0 rosborn    (504) 660979062     9713 2023-04-04 21:07:54.000000 NeXpy-1.0.2/src/NeXpy.egg-info/SOURCES.txt
--rw-r--r--   0 rosborn    (504) 660979062        1 2023-04-04 21:07:54.000000 NeXpy-1.0.2/src/NeXpy.egg-info/dependency_links.txt
--rw-r--r--   0 rosborn    (504) 660979062       42 2023-04-04 21:07:54.000000 NeXpy-1.0.2/src/NeXpy.egg-info/entry_points.txt
--rw-r--r--   0 rosborn    (504) 660979062       47 2017-06-13 21:39:09.000000 NeXpy-1.0.2/src/NeXpy.egg-info/pbr.json
--rw-r--r--   0 rosborn    (504) 660979062      197 2023-04-04 21:07:54.000000 NeXpy-1.0.2/src/NeXpy.egg-info/requires.txt
--rw-r--r--   0 rosborn    (504) 660979062        6 2023-04-04 21:07:54.000000 NeXpy-1.0.2/src/NeXpy.egg-info/top_level.txt
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.751778 NeXpy-1.0.2/src/nexpy/
--rw-r--r--   0 rosborn    (504) 660979062      395 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062      160 2023-04-04 21:07:54.000000 NeXpy-1.0.2/src/nexpy/_version.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.751917 NeXpy-1.0.2/src/nexpy/api/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.752294 NeXpy-1.0.2/src/nexpy/api/frills/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/frills/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062     8480 2023-01-16 20:45:39.000000 NeXpy-1.0.2/src/nexpy/api/frills/fit.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.752505 NeXpy-1.0.2/src/nexpy/api/frills/functions/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/frills/functions/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.753887 NeXpy-1.0.2/src/nexpy/api/frills/models/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/frills/models/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062     1132 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/frills/models/bose.py
--rw-r--r--   0 rosborn    (504) 660979062      931 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/frills/models/critexp.py
--rw-r--r--   0 rosborn    (504) 660979062      916 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/frills/models/op.py
--rw-r--r--   0 rosborn    (504) 660979062      942 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/api/frills/models/pdfdecay.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.754035 NeXpy-1.0.2/src/nexpy/definitions/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/definitions/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.760921 NeXpy-1.0.2/src/nexpy/definitions/applications/
--rw-r--r--   0 rosborn    (504) 660979062     6656 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXarchive.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5051 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXarpes.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    50836 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2667 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3803 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXfluo.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2774 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5070 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXiqproc.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5557 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXlauetof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5500 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXmonopd.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    30950 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXmx.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4469 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXrefscan.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4919 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXreftof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7147 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXsas.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6974 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXsastof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4480 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXscan.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3495 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXspe.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4547 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXsqom.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    10592 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXstxm.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7230 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXtas.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5530 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6031 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXtofraw.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5772 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6441 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXtomo.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6800 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXtomophase.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5033 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4687 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxas.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3565 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxasproc.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7413 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxbase.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4034 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxeuler.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3899 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxkappa.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2671 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxlaue.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2066 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3632 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxnb.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3868 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/NXxrot.nxdl.xml
--rwxr-xr-x   0 rosborn    (504) 660979062     9850 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/applications/nxdlformat.xsl
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.771406 NeXpy-1.0.2/src/nexpy/definitions/base_classes/
--rw-r--r--   0 rosborn    (504) 660979062     2888 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3553 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6264 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3029 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3891 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3074 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2818 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcite.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2413 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3254 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    13934 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3997 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    16352 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdata.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    26917 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4068 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6385 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5447 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     8063 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXentry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2293 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5023 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3254 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6816 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3093 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3493 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3299 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3949 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7713 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXguide.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3606 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3459 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5749 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXlog.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6041 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3284 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5290 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3398 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2853 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXnote.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     1397 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXobject.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4413 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3058 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2196 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6173 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2499 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2419 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3770 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2847 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    20356 2021-11-21 23:11:32.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4090 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXroot.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    14403 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsample.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6404 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5297 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3723 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXshape.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2740 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXslit.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6942 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsource.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6964 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     8599 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2725 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2993 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXuser.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3107 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3830 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml
--rwxr-xr-x   0 rosborn    (504) 660979062     8463 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/base_classes/nxdlformat.xsl
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.773994 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/
--rw-r--r--   0 rosborn    (504) 660979062     6935 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2862 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    10240 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2498 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2506 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3113 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2143 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2725 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    13513 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    14352 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2137 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     1896 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    15240 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2719 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
--rwxr-xr-x   0 rosborn    (504) 660979062     9805 2022-11-21 17:33:01.000000 NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.774690 NeXpy-1.0.2/src/nexpy/examples/
--rw-r--r--   0 rosborn    (504) 660979062      615 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/README.rst
--rw-r--r--   0 rosborn    (504) 660979062   382712 2023-03-25 22:52:38.000000 NeXpy-1.0.2/src/nexpy/examples/chopper.nxs
--rw-r--r--   0 rosborn    (504) 660979062    53690 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/example.nxs
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.774890 NeXpy-1.0.2/src/nexpy/examples/plugins/
--rw-r--r--   0 rosborn    (504) 660979062     1250 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/plugins/README.rst
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.776609 NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/
--rw-r--r--   0 rosborn    (504) 660979062      244 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062      711 2016-08-04 20:27:34.000000 NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/__init__.pyc
--rw-r--r--   0 rosborn    (504) 660979062     4262 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/convert_qe.py
--rw-r--r--   0 rosborn    (504) 660979062     6571 2016-08-04 20:27:34.000000 NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/convert_qe.pyc
--rw-r--r--   0 rosborn    (504) 660979062     2383 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/get_ei.py
--rw-r--r--   0 rosborn    (504) 660979062     3888 2016-08-04 20:27:34.000000 NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/get_ei.pyc
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.777186 NeXpy-1.0.2/src/nexpy/examples/scripts/
--rw-r--r--   0 rosborn    (504) 660979062      634 2023-02-23 19:59:31.000000 NeXpy-1.0.2/src/nexpy/examples/scripts/README.rst
--rw-r--r--   0 rosborn    (504) 660979062      235 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/scripts/chopper_plot.py
--rw-r--r--   0 rosborn    (504) 660979062      203 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/examples/scripts/example.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.779323 NeXpy-1.0.2/src/nexpy/gui/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/gui/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062    13672 2023-03-23 22:41:46.000000 NeXpy-1.0.2/src/nexpy/gui/consoleapp.py
--rw-r--r--   0 rosborn    (504) 660979062   178429 2023-04-04 20:52:54.000000 NeXpy-1.0.2/src/nexpy/gui/datadialogs.py
--rwxr-xr-x   0 rosborn    (504) 660979062    55605 2022-12-30 18:26:23.000000 NeXpy-1.0.2/src/nexpy/gui/fitdialogs.py
--rw-r--r--   0 rosborn    (504) 660979062     1283 2022-11-15 16:30:46.000000 NeXpy-1.0.2/src/nexpy/gui/importdialog.py
--rw-r--r--   0 rosborn    (504) 660979062    91011 2023-04-03 20:37:28.000000 NeXpy-1.0.2/src/nexpy/gui/mainwindow.py
--rw-r--r--   0 rosborn    (504) 660979062   150779 2023-04-04 20:52:54.000000 NeXpy-1.0.2/src/nexpy/gui/plotview.py
--rw-r--r--   0 rosborn    (504) 660979062     1201 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/pyqt.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.784142 NeXpy-1.0.2/src/nexpy/gui/resources/
--rw-r--r--   0 rosborn    (504) 660979062     1465 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/back.png
--rw-r--r--   0 rosborn    (504) 660979062      401 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/backward-icon.png
--rw-r--r--   0 rosborn    (504) 660979062      905 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/customize.png
--rw-r--r--   0 rosborn    (504) 660979062      514 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/equal.png
--rw-r--r--   0 rosborn    (504) 660979062    37268 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/export-data.png
--rw-r--r--   0 rosborn    (504) 660979062    43660 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/export-figure.png
--rw-r--r--   0 rosborn    (504) 660979062     1121 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/filesave.png
--rw-r--r--   0 rosborn    (504) 660979062      410 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/forward-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1462 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/forward.png
--rw-r--r--   0 rosborn    (504) 660979062      979 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/hand.png
--rw-r--r--   0 rosborn    (504) 660979062     1338 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/home.png
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.784690 NeXpy-1.0.2/src/nexpy/gui/resources/icon/
--rw-r--r--   0 rosborn    (504) 660979062    95378 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/icon/NeXpy.png
--rw-r--r--   0 rosborn    (504) 660979062   127292 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/icon/NeXpy.svg
--rw-r--r--   0 rosborn    (504) 660979062      613 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/link-icon.png
--rw-r--r--   0 rosborn    (504) 660979062      241 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/lock-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1439 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/lock-red-icon.png
--rw-r--r--   0 rosborn    (504) 660979062      713 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/move.png
--rw-r--r--   0 rosborn    (504) 660979062      290 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/pause-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1617 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/refresh-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     2713 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/subplots.png
--rw-r--r--   0 rosborn    (504) 660979062      258 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/unlock-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1415 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/unlock-red-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1233 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/resources/zoom_to_rect.png
--rw-r--r--   0 rosborn    (504) 660979062     8546 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/gui/scripteditor.py
--rw-r--r--   0 rosborn    (504) 660979062    23583 2023-01-16 20:45:39.000000 NeXpy-1.0.2/src/nexpy/gui/treeview.py
--rw-r--r--   0 rosborn    (504) 660979062    28154 2023-04-04 20:52:54.000000 NeXpy-1.0.2/src/nexpy/gui/utils.py
--rw-r--r--   0 rosborn    (504) 660979062    42714 2023-04-01 21:24:50.000000 NeXpy-1.0.2/src/nexpy/gui/widgets.py
--rwxr-xr-x   0 rosborn    (504) 660979062     1281 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/nexpygui.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.784947 NeXpy-1.0.2/src/nexpy/plugins/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/plugins/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.785883 NeXpy-1.0.2/src/nexpy/readers/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/readers/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062    15851 2023-01-16 20:45:39.000000 NeXpy-1.0.2/src/nexpy/readers/readspec.py
--rw-r--r--   0 rosborn    (504) 660979062    10515 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/readers/readstack.py
--rw-r--r--   0 rosborn    (504) 660979062     1409 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/readers/readtiff.py
--rw-r--r--   0 rosborn    (504) 660979062     9571 2022-11-15 16:30:47.000000 NeXpy-1.0.2/src/nexpy/readers/readtxt.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-04 21:07:54.786080 NeXpy-1.0.2/tests/
--rw-r--r--   0 rosborn    (504) 660979062      997 2023-01-16 20:45:39.000000 NeXpy-1.0.2/tests/test_imports.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.635950 NeXpy-1.0.3/
+-rw-r--r--   0 rosborn    (504) 660979062      672 2023-04-15 18:57:55.000000 NeXpy-1.0.3/.gitattributes
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.567221 NeXpy-1.0.3/.github/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.572295 NeXpy-1.0.3/.github/workflows/
+-rw-r--r--   0 rosborn    (504) 660979062      654 2023-04-15 18:57:55.000000 NeXpy-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 rosborn    (504) 660979062      577 2023-04-15 18:57:55.000000 NeXpy-1.0.3/.gitignore
+-rw-r--r--   0 rosborn    (504) 660979062     2378 2023-04-15 18:57:55.000000 NeXpy-1.0.3/COPYING
+-rw-r--r--   0 rosborn    (504) 660979062     5299 2023-04-18 15:01:55.636113 NeXpy-1.0.3/PKG-INFO
+-rw-r--r--   0 rosborn    (504) 660979062     4283 2023-04-15 18:57:55.000000 NeXpy-1.0.3/README.md
+-rw-r--r--   0 rosborn    (504) 660979062     7060 2023-04-15 18:57:55.000000 NeXpy-1.0.3/README.rst
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.573353 NeXpy-1.0.3/conda-recipe/
+-rw-r--r--   0 rosborn    (504) 660979062       51 2022-11-15 16:30:46.000000 NeXpy-1.0.3/conda-recipe/bld.bat
+-rw-r--r--   0 rosborn    (504) 660979062      103 2022-11-15 16:30:46.000000 NeXpy-1.0.3/conda-recipe/build.sh
+-rw-r--r--   0 rosborn    (504) 660979062      999 2023-04-15 18:57:55.000000 NeXpy-1.0.3/conda-recipe/meta.yaml
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.574028 NeXpy-1.0.3/doc/
+-rw-r--r--   0 rosborn    (504) 660979062     5643 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/Makefile
+-rw-r--r--   0 rosborn    (504) 660979062     5103 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/make.bat
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.576472 NeXpy-1.0.3/doc/source/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.576727 NeXpy-1.0.3/doc/source/_static/
+-rw-r--r--   0 rosborn    (504) 660979062      102 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/_static/__ignore__.txt
+-rw-r--r--   0 rosborn    (504) 660979062     8265 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/conf.py
+-rw-r--r--   0 rosborn    (504) 660979062      526 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/examples.rst
+-rw-r--r--   0 rosborn    (504) 660979062    90022 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/favicon.ico
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.589111 NeXpy-1.0.3/doc/source/images/
+-rw-r--r--   0 rosborn    (504) 660979062    14509 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/axis-limits-bar.png
+-rw-r--r--   0 rosborn    (504) 660979062   684819 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/customize-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062   432231 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/limits-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062   705341 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/nexpy-fits.png
+-rw-r--r--   0 rosborn    (504) 660979062   364457 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/nexpy-gui.png
+-rw-r--r--   0 rosborn    (504) 660979062    40568 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/nexpy-logo.png
+-rw-r--r--   0 rosborn    (504) 660979062    43638 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/options-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062   496144 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/projection-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062    20559 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/projection-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062   590841 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/scan-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062   598861 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/signal-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062    73587 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/simple-plot.png
+-rw-r--r--   0 rosborn    (504) 660979062   308220 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/skewed-axis.png
+-rw-r--r--   0 rosborn    (504) 660979062    19535 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/x-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062    29737 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/y-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062    20833 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/z-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062     8104 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/z-toolbar.png
+-rw-r--r--   0 rosborn    (504) 660979062       30 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/includeme.rst
+-rw-r--r--   0 rosborn    (504) 660979062     1093 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/index.rst
+-rw-r--r--   0 rosborn    (504) 660979062    62301 2023-04-17 14:57:59.000000 NeXpy-1.0.3/doc/source/pythongui.rst
+-rw-r--r--   0 rosborn    (504) 660979062    44651 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/pythonshell.rst
+-rw-r--r--   0 rosborn    (504) 660979062     2845 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/readers.rst
+-rw-r--r--   0 rosborn    (504) 660979062      417 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/treeapi.rst
+-rw-r--r--   0 rosborn    (504) 660979062      181 2023-04-15 18:57:56.000000 NeXpy-1.0.3/pyproject.toml
+-rw-r--r--   0 rosborn    (504) 660979062     1667 2023-04-18 15:01:55.636650 NeXpy-1.0.3/setup.cfg
+-rwxr-xr-x   0 rosborn    (504) 660979062      410 2023-04-15 18:57:56.000000 NeXpy-1.0.3/setup.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.568241 NeXpy-1.0.3/src/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.590535 NeXpy-1.0.3/src/NeXpy.egg-info/
+-rw-r--r--   0 rosborn    (504) 660979062     5299 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/PKG-INFO
+-rw-r--r--   0 rosborn    (504) 660979062     9860 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/SOURCES.txt
+-rw-r--r--   0 rosborn    (504) 660979062        1 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/dependency_links.txt
+-rw-r--r--   0 rosborn    (504) 660979062       42 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/entry_points.txt
+-rw-r--r--   0 rosborn    (504) 660979062       47 2017-06-13 21:39:09.000000 NeXpy-1.0.3/src/NeXpy.egg-info/pbr.json
+-rw-r--r--   0 rosborn    (504) 660979062      244 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/requires.txt
+-rw-r--r--   0 rosborn    (504) 660979062        6 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/top_level.txt
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591076 NeXpy-1.0.3/src/nexpy/
+-rw-r--r--   0 rosborn    (504) 660979062      395 2023-04-15 19:28:11.000000 NeXpy-1.0.3/src/nexpy/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062      160 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/nexpy/_version.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591385 NeXpy-1.0.3/src/nexpy/api/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/api/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591678 NeXpy-1.0.3/src/nexpy/api/frills/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/api/frills/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062     8480 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/fit.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591869 NeXpy-1.0.3/src/nexpy/api/frills/functions/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/api/frills/functions/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.592698 NeXpy-1.0.3/src/nexpy/api/frills/models/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062     1132 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/bose.py
+-rw-r--r--   0 rosborn    (504) 660979062      931 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/critexp.py
+-rw-r--r--   0 rosborn    (504) 660979062      916 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/op.py
+-rw-r--r--   0 rosborn    (504) 660979062      942 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/pdfdecay.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.592896 NeXpy-1.0.3/src/nexpy/definitions/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/definitions/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.600331 NeXpy-1.0.3/src/nexpy/definitions/applications/
+-rw-r--r--   0 rosborn    (504) 660979062     6656 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXarchive.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5051 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXarpes.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    50836 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2667 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3803 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXfluo.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2774 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5070 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXiqproc.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5557 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXlauetof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5500 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXmonopd.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    30950 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXmx.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4469 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXrefscan.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4919 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXreftof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7147 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXsas.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6974 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXsastof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4480 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXscan.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3495 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXspe.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4547 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXsqom.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    10592 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXstxm.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7230 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtas.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5530 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6031 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofraw.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5772 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6441 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomo.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6800 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomophase.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5033 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4687 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxas.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3565 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxasproc.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7413 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxbase.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4034 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxeuler.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3899 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxkappa.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2671 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaue.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2066 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3632 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxnb.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3868 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxrot.nxdl.xml
+-rwxr-xr-x   0 rosborn    (504) 660979062     9850 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/nxdlformat.xsl
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.616618 NeXpy-1.0.3/src/nexpy/definitions/base_classes/
+-rw-r--r--   0 rosborn    (504) 660979062     2888 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3553 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6264 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3029 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3891 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3074 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2818 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcite.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2413 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3254 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    13934 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3997 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    16352 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdata.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    26917 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4068 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6385 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5447 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     8063 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXentry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2293 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5023 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3254 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6816 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3093 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3493 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3299 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3949 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7713 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXguide.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3606 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3459 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5749 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXlog.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6041 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3284 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5290 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3398 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2853 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXnote.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     1397 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXobject.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4413 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3058 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2196 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6173 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2499 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2419 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3770 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2847 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    20356 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4090 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXroot.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    14403 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6404 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5297 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3723 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXshape.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2740 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXslit.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6942 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsource.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6964 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     8599 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2725 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2993 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXuser.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3107 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3830 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml
+-rwxr-xr-x   0 rosborn    (504) 660979062     8463 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/nxdlformat.xsl
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.620176 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/
+-rw-r--r--   0 rosborn    (504) 660979062     6935 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2862 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    10240 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2498 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2506 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3113 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2143 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2725 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    13513 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    14352 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2137 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     1896 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    15240 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2719 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
+-rwxr-xr-x   0 rosborn    (504) 660979062     9805 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.621364 NeXpy-1.0.3/src/nexpy/examples/
+-rw-r--r--   0 rosborn    (504) 660979062      615 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/README.rst
+-rw-r--r--   0 rosborn    (504) 660979062   382712 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/chopper.nxs
+-rw-r--r--   0 rosborn    (504) 660979062    53690 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/example.nxs
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.621965 NeXpy-1.0.3/src/nexpy/examples/plugins/
+-rw-r--r--   0 rosborn    (504) 660979062     2026 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/README.rst
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.622315 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.624179 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/
+-rw-r--r--   0 rosborn    (504) 660979062      244 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062      711 2016-08-04 20:27:34.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.pyc
+-rw-r--r--   0 rosborn    (504) 660979062     4263 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.py
+-rw-r--r--   0 rosborn    (504) 660979062     6571 2016-08-04 20:27:34.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.pyc
+-rw-r--r--   0 rosborn    (504) 660979062     2383 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.py
+-rw-r--r--   0 rosborn    (504) 660979062     3888 2016-08-04 20:27:34.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.pyc
+-rw-r--r--   0 rosborn    (504) 660979062      255 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/pyproject.toml
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.624839 NeXpy-1.0.3/src/nexpy/examples/scripts/
+-rw-r--r--   0 rosborn    (504) 660979062      634 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/scripts/README.rst
+-rw-r--r--   0 rosborn    (504) 660979062      235 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/scripts/chopper_plot.py
+-rw-r--r--   0 rosborn    (504) 660979062      203 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/scripts/example.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.628288 NeXpy-1.0.3/src/nexpy/gui/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/gui/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062    14081 2023-04-17 15:50:34.000000 NeXpy-1.0.3/src/nexpy/gui/consoleapp.py
+-rw-r--r--   0 rosborn    (504) 660979062   178273 2023-04-17 20:23:53.000000 NeXpy-1.0.3/src/nexpy/gui/datadialogs.py
+-rwxr-xr-x   0 rosborn    (504) 660979062    55605 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/fitdialogs.py
+-rw-r--r--   0 rosborn    (504) 660979062     1283 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/importdialog.py
+-rw-r--r--   0 rosborn    (504) 660979062    92974 2023-04-17 16:33:37.000000 NeXpy-1.0.3/src/nexpy/gui/mainwindow.py
+-rw-r--r--   0 rosborn    (504) 660979062   150779 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/plotview.py
+-rw-r--r--   0 rosborn    (504) 660979062     1201 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/pyqt.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.633639 NeXpy-1.0.3/src/nexpy/gui/resources/
+-rw-r--r--   0 rosborn    (504) 660979062     1465 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/back.png
+-rw-r--r--   0 rosborn    (504) 660979062      401 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/backward-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062      905 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/customize.png
+-rw-r--r--   0 rosborn    (504) 660979062      514 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/equal.png
+-rw-r--r--   0 rosborn    (504) 660979062    37268 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/export-data.png
+-rw-r--r--   0 rosborn    (504) 660979062    43660 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/export-figure.png
+-rw-r--r--   0 rosborn    (504) 660979062     1121 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/filesave.png
+-rw-r--r--   0 rosborn    (504) 660979062      410 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/forward-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1462 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/forward.png
+-rw-r--r--   0 rosborn    (504) 660979062      979 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/hand.png
+-rw-r--r--   0 rosborn    (504) 660979062     1338 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/home.png
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.634315 NeXpy-1.0.3/src/nexpy/gui/resources/icon/
+-rw-r--r--   0 rosborn    (504) 660979062    95378 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.png
+-rw-r--r--   0 rosborn    (504) 660979062   127292 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.svg
+-rw-r--r--   0 rosborn    (504) 660979062      613 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/link-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062      241 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/lock-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1439 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/lock-red-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062      713 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/move.png
+-rw-r--r--   0 rosborn    (504) 660979062      290 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/pause-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1617 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/refresh-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     2713 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/subplots.png
+-rw-r--r--   0 rosborn    (504) 660979062      258 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/unlock-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1415 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/unlock-red-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1233 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/zoom_to_rect.png
+-rw-r--r--   0 rosborn    (504) 660979062     8546 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/scripteditor.py
+-rw-r--r--   0 rosborn    (504) 660979062    23583 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/treeview.py
+-rw-r--r--   0 rosborn    (504) 660979062    28172 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/utils.py
+-rw-r--r--   0 rosborn    (504) 660979062    42714 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/widgets.py
+-rwxr-xr-x   0 rosborn    (504) 660979062     1281 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/nexpygui.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.634644 NeXpy-1.0.3/src/nexpy/plugins/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/plugins/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.635505 NeXpy-1.0.3/src/nexpy/readers/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/readers/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062    15851 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readspec.py
+-rw-r--r--   0 rosborn    (504) 660979062    10515 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readstack.py
+-rw-r--r--   0 rosborn    (504) 660979062     1409 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readtiff.py
+-rw-r--r--   0 rosborn    (504) 660979062     9571 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readtxt.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.635746 NeXpy-1.0.3/tests/
+-rw-r--r--   0 rosborn    (504) 660979062      997 2023-04-15 18:57:56.000000 NeXpy-1.0.3/tests/test_imports.py
```

### Comparing `NeXpy-1.0.2/.gitattributes` & `NeXpy-1.0.3/.gitattributes`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/.github/workflows/ci.yml` & `NeXpy-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/.gitignore` & `NeXpy-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/COPYING` & `NeXpy-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/PKG-INFO` & `NeXpy-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeXpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python GUI to analyze NeXus data
 Home-page: https://nexpy.github.io/nexpy/
 Download-URL: https://github.com/nexpy/nexpy
 Author: Raymond Osborn
 Author-email: rayosborn@mac.com
 License: Modified BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `NeXpy-1.0.2/README.md` & `NeXpy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/README.rst` & `NeXpy-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/conda-recipe/meta.yaml` & `NeXpy-1.0.3/conda-recipe/meta.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 package:
   name: nexpy
-  version: "1.0.2"
+  version: "1.0.3"
 
 source:
   git_url: https://github.com/nexpy/nexpy.git
-  git_tag: v1.0.2
+  git_tag: v1.0.3
 
 build:
   entry_points:
     - nexpy = nexpy.nexpygui:main
   number: 0
   noarch: generic
```

### Comparing `NeXpy-1.0.2/doc/Makefile` & `NeXpy-1.0.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/make.bat` & `NeXpy-1.0.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/conf.py` & `NeXpy-1.0.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/examples.rst` & `NeXpy-1.0.3/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/favicon.ico` & `NeXpy-1.0.3/doc/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/axis-limits-bar.png` & `NeXpy-1.0.3/doc/source/images/axis-limits-bar.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/customize-panel.png` & `NeXpy-1.0.3/doc/source/images/customize-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/limits-panel.png` & `NeXpy-1.0.3/doc/source/images/limits-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/nexpy-fits.png` & `NeXpy-1.0.3/doc/source/images/nexpy-fits.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/nexpy-gui.png` & `NeXpy-1.0.3/doc/source/images/nexpy-gui.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/nexpy-logo.png` & `NeXpy-1.0.3/doc/source/images/nexpy-logo.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/options-tab.png` & `NeXpy-1.0.3/doc/source/images/options-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/projection-panel.png` & `NeXpy-1.0.3/doc/source/images/projection-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/projection-tab.png` & `NeXpy-1.0.3/doc/source/images/projection-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/scan-panel.png` & `NeXpy-1.0.3/doc/source/images/scan-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/signal-tab.png` & `NeXpy-1.0.3/doc/source/images/signal-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/simple-plot.png` & `NeXpy-1.0.3/doc/source/images/simple-plot.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/skewed-axis.png` & `NeXpy-1.0.3/doc/source/images/skewed-axis.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/x-tab.png` & `NeXpy-1.0.3/doc/source/images/x-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/y-tab.png` & `NeXpy-1.0.3/doc/source/images/y-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/z-tab.png` & `NeXpy-1.0.3/doc/source/images/z-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/images/z-toolbar.png` & `NeXpy-1.0.3/doc/source/images/z-toolbar.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/index.rst` & `NeXpy-1.0.3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/pythongui.rst` & `NeXpy-1.0.3/doc/source/pythongui.rst`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,18 @@
     if the user has the necessary privilege. The plugin menu is appended to
     the existing menus, but will be loaded in alphabetical order of the other
     plugins when NeXpy is restarted.
 
     .. note:: If a plugin of the same name exists in both directories, the 
               user's plugin is loaded.
 
+    .. note:: With NeXpy v1.0.3, plugins can also be loaded directly from
+              external packages, in which the plugin modules are declared
+              using the ``nexpy.readers`` entry point.
+
     .. seealso:: `NeXpy Plugins`_
     
 **Remove Plugin**
     The selected NeXpy plugin module is removed from either the user's
     NeXpy directory (``~/.nexpy/plugins``) or the package directory.
 
 **Restore Plugin**
@@ -1221,29 +1225,102 @@
          y = NXfield(range(z.shape[0]), name='y')      
          x = NXfield(range(z.shape[1]), name='x')
          return NXentry(NXdata(z,(y,x)))
 
 NeXpy Plugins
 -------------
 It is possible to customize NeXpy by adding new menus to the main menu bar 
-with sub-menus that open dialog boxes for operations that are specific to a 
-particular domain. These will be automatically loaded from either the 
-``nexpy.plugins`` directory within the installed NeXpy distribution or from the
-users' ``~/.nexpy/plugins`` directory.
-
-The new menu should be defined as a Python package, *i.e.*, by creating a 
-sub-directory within the plugins directory that contains ``__init__.py`` to 
-define the menu actions.
-
-There is an example package, ``chopper``, in the ``nexpy.examples`` directory,
-to show how plugins can work. It adds a top-level menu item, ``chopper``, that
-has a couple of menu items to perform data analysis on the example file, 
-``chopper.nxs``, which is distributed with NeXpy.
+with sub-menus that open GUI dialogs or perform operations that are 
+specific to a specialized application. 
+
+Installing Plugins
+^^^^^^^^^^^^^^^^^^
+NeXpy searches for plugin modules in two ways.
+
+1. The plugin code can be installed using the ``Install Plugin...`` dialog
+   either locally in the user's ``~/.nexpy/plugins``directory or in the 
+   ``nexpy.plugins`` directory within the installed NeXpy distribution.
+
+2. The plugin code can be contained within an external installed package,
+   which declares an entry point labelled ``nexpy.plugins``. An example 
+   package, that is installable using ``pip install .`` is available in 
+   the NeXpy package examples directory.
+
+   .. note:: The second method was introduced in NeXpy v1.0.3. It is 
+             recommended for new plugins. 
+
+Plugins are loaded from the users' directory, the NeXpy distribution's 
+plugin directory, and external package entry points, *in that order*,
+for backward compatibility with existing installations. Duplicate 
+plugins will not be loaded, but a warning will be added to the NeXpy log 
+file. If a previously installed plugin is now available in an external
+package, please remove the prior installation using the 
+``Remove Plugin...`` dialog.
 
-Here is the ``__init__.py`` file::
+Defining Plugins
+^^^^^^^^^^^^^^^^
+The modules that are accessed through the plugin menu should be defined
+as a Python package, *i.e.*, by creating a sub-directory that contains 
+``__init__.py``. This must contain a function, ``plugin_menu``, which returns
+the name to be added to the top-level NeXpy menu bar, and a list of tuples,
+each of which contains the sub-menu name and the corresponding function
+triggered by clicking on it.
+
+There is an example package, ``chopper_plugin``, in the ``nexpy.examples``
+directory, to show how plugins should be configured. It adds a top-level 
+menu item, ``Chopper``, that has a couple of sub-menu items to perform 
+data analysis on the example file, ``chopper.nxs``, which is also 
+distributed with NeXpy.
+
+Here is the structure of the ``chopper_plugin`` package::
+
+    chopper_plugin:
+    └── pyproject.toml
+    └── chopper
+        ├── __init.py__
+        ├── convert_qe.py
+        └── get_ei.py
+
+.. note:: If the plugin is to be installed using the ``Install Plugin...``
+          dialog, just select the ``chopper`` sub-directory in the above 
+          file tree.
+
+Here is the ``pyproject.toml`` file::
+
+    [build-system]
+    requires = ["setuptools", "setuptools-scm"]
+    build-backend = "setuptools.build_meta"
+
+    [project]
+    name = "chopper_plugin"
+    version = "1.0.0"
+    dependencies = [
+        "nexpy"
+    ]
+
+    [project.entry-points."nexpy.plugins"]
+    chopper = "chopper:plugin_menu"
+
+This is sufficient to install the plugin using ``pip`` and make it 
+discoverable by NeXpy through ``nexpy.plugins`` entry point. If the 
+plugin is embedded within a larger package, adjust the entry point so 
+that it points to the sub-directory containing the ``__init__.py`` file 
+that defines the ``plugin_menu`` function. For example, if the plugin 
+modules are contained within the ``plugins`` sub-directory of 
+``mypackage``, add the following entry point::
+
+    [project.entry-points."nexpy.plugins"]
+    plugin_name = "mypackage.plugins.plugin_name:plugin_menu"
+
+.. seealso:: Information on defining entry points in external packages
+             that do not use a ``pyproject.toml`` file is available in 
+             the `Setup Tools documentation
+             <https://setuptools.pypa.io/en/latest/userguide/entry_point.html>`_.
+
+Here is the ``__init__.py`` file, which defines the ``plugin_menu`` function::
 
   from . import get_ei, convert_qe
 
   def plugin_menu():
       menu = 'Chopper'
       actions = []
       actions.append(('Get Incident Energy', get_ei.show_dialog))
@@ -1267,17 +1344,15 @@
 analysis.
 
 In the simplest cases, no knowledge of PyQt is required. In the example below, 
 a grid defines a set of parameters, functions to read those parameters from
 the PySide text boxes (here, they are decorated with ``@property``, which
 means that the function can be called without an argument), a couple of
 buttons to activate different parts of the analysis, and finally the
-functions themselves.
-
-Here is the code::
+functions themselves::
 
   import numpy as np
   from nexpy.gui.datadialogs import GridParameters, NXDialog
   from nexpy.gui.mainwindow import report_error
   from nexusformat.nexus import NeXusError
```

### Comparing `NeXpy-1.0.2/doc/source/pythonshell.rst` & `NeXpy-1.0.3/doc/source/pythonshell.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/doc/source/readers.rst` & `NeXpy-1.0.3/doc/source/readers.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/setup.cfg` & `NeXpy-1.0.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -39,22 +39,23 @@
 	ipykernel >= 6.15.2
 	matplotlib
 	lmfit >= 1.0.3
 	pylatexenc
 	ansi2html
 	pillow
 	mplcursors
+	importlib-metadata; python_version<"3.10"
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 nexpy.gui = resources/*.*, resources/*/*.*
 nexpy.definitions = */*.xml
-nexpy = examples/*.*, examples/*/*.*, examples/*/*/*.*
+nexpy = examples/*.*, examples/*/*.*, examples/*/*/*.*, examples/*/*/*/*.*
 
 [options.entry_points]
 gui_scripts = 
 	nexpy = nexpy.nexpygui:main
 
 [options.extras_require]
 spec = spec2nexus
```

### Comparing `NeXpy-1.0.2/src/NeXpy.egg-info/PKG-INFO` & `NeXpy-1.0.3/src/NeXpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeXpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python GUI to analyze NeXus data
 Home-page: https://nexpy.github.io/nexpy/
 Download-URL: https://github.com/nexpy/nexpy
 Author: Raymond Osborn
 Author-email: rayosborn@mac.com
 License: Modified BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `NeXpy-1.0.2/src/NeXpy.egg-info/SOURCES.txt` & `NeXpy-1.0.3/src/NeXpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -167,20 +167,21 @@
 src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml
 src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
 src/nexpy/definitions/contributed_definitions/nxdlformat.xsl
 src/nexpy/examples/README.rst
 src/nexpy/examples/chopper.nxs
 src/nexpy/examples/example.nxs
 src/nexpy/examples/plugins/README.rst
-src/nexpy/examples/plugins/chopper/__init__.py
-src/nexpy/examples/plugins/chopper/__init__.pyc
-src/nexpy/examples/plugins/chopper/convert_qe.py
-src/nexpy/examples/plugins/chopper/convert_qe.pyc
-src/nexpy/examples/plugins/chopper/get_ei.py
-src/nexpy/examples/plugins/chopper/get_ei.pyc
+src/nexpy/examples/plugins/chopper_plugin/pyproject.toml
+src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.py
+src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.pyc
+src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.py
+src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.pyc
+src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.py
+src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.pyc
 src/nexpy/examples/scripts/README.rst
 src/nexpy/examples/scripts/chopper_plot.py
 src/nexpy/examples/scripts/example.py
 src/nexpy/gui/__init__.py
 src/nexpy/gui/consoleapp.py
 src/nexpy/gui/datadialogs.py
 src/nexpy/gui/fitdialogs.py
```

### Comparing `NeXpy-1.0.2/src/nexpy/api/frills/fit.py` & `NeXpy-1.0.3/src/nexpy/api/frills/fit.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/api/frills/models/bose.py` & `NeXpy-1.0.3/src/nexpy/api/frills/models/bose.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/api/frills/models/critexp.py` & `NeXpy-1.0.3/src/nexpy/api/frills/models/critexp.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/api/frills/models/op.py` & `NeXpy-1.0.3/src/nexpy/api/frills/models/op.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/api/frills/models/pdfdecay.py` & `NeXpy-1.0.3/src/nexpy/api/frills/models/pdfdecay.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXarchive.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXarchive.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXarpes.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXarpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXfluo.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXfluo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXiqproc.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXiqproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXlauetof.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXlauetof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXmonopd.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXmonopd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXmx.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXmx.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXrefscan.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXrefscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXreftof.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXreftof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXsas.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXsas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXsastof.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXsastof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXscan.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXspe.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXspe.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXsqom.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXsqom.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXstxm.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXstxm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXtas.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXtofraw.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofraw.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXtomo.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXtomophase.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomophase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxas.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxasproc.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxasproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxbase.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxbase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxeuler.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxeuler.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxkappa.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxkappa.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxlaue.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaue.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxnb.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxnb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/NXxrot.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxrot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/applications/nxdlformat.xsl` & `NeXpy-1.0.3/src/nexpy/definitions/applications/nxdlformat.xsl`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcite.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcite.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdata.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdata.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXentry.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXguide.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXguide.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXlog.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXlog.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXnote.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXnote.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXobject.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXobject.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXroot.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXroot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsample.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXshape.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXshape.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXslit.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXslit.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsource.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsource.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXuser.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXuser.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/base_classes/nxdlformat.xsl` & `NeXpy-1.0.3/src/nexpy/definitions/base_classes/nxdlformat.xsl`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl` & `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/README.rst` & `NeXpy-1.0.3/src/nexpy/examples/README.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/chopper.nxs` & `NeXpy-1.0.3/src/nexpy/examples/chopper.nxs`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/example.nxs` & `NeXpy-1.0.3/src/nexpy/examples/example.nxs`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/__init__.pyc` & `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.pyc`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/convert_qe.py` & `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     @property
     def dE(self):
         return self.parameters['dE'].value
 
     def read_parameters(self):
         self.L1 = - self.entry['sample/distance']
-        self.L2 = np.mean(self.entry['instrument/detector/distance'])
+        self.L2 = self.entry['instrument/detector/distance'].average()
         self.m1 = self.entry['monitor1']
         self.t_m1 = self.m1.moment()
         self.d_m1 = self.entry['monitor1/distance']
 
     def convert_tof(self, tof):
         ki = np.sqrt(self.Ei / 2.0721)
         ts = self.t_m1 + 1588.254 * (self.L1 - self.d_m1) / ki
```

### Comparing `NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/convert_qe.pyc` & `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.pyc`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/get_ei.py` & `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/plugins/chopper/get_ei.pyc` & `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.pyc`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/examples/scripts/README.rst` & `NeXpy-1.0.3/src/nexpy/examples/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/consoleapp.py` & `NeXpy-1.0.3/src/nexpy/gui/consoleapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,22 +170,30 @@
 
         def backup_age(backup):
             try:
                 return timestamp_age(os.path.basename(os.path.dirname(backup)))
             except ValueError:
                 return 0
         backups = self.settings.options('backups')
-        for backup in backups:
+        plugins = self.settings.options('plugins')
+        total_backups = backups + plugins
+        for backup in total_backups:
             if not (os.path.exists(backup) and
                     os.path.realpath(backup).startswith(self.backup_dir)):
-                self.settings.remove_option('backups', backup)
+                if backup in backups:
+                    self.settings.remove_option('backups', backup)
+                elif backup in plugins:
+                    self.settings.remove_option('plugins', backup)
             elif backup_age(backup) > 5:
                 try:
                     shutil.rmtree(os.path.dirname(os.path.realpath(backup)))
-                    self.settings.remove_option('backups', backup)
+                    if backup in backups:
+                        self.settings.remove_option('backups', backup)
+                    elif backup in plugins:
+                        self.settings.remove_option('plugins', backup)
                 except OSError:
                     pass
         self.settings.save()
 
     def init_log(self):
         """Initialize the NeXpy logger."""
         log_file = os.path.join(self.nexpy_dir, 'nexpy.log')
```

### Comparing `NeXpy-1.0.2/src/nexpy/gui/datadialogs.py` & `NeXpy-1.0.3/src/nexpy/gui/datadialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -----------------------------------------------------------------------------
 import bisect
 import logging
 import numbers
 import os
 import shutil
 from operator import attrgetter
-from pathlib import PosixPath as Path
+from pathlib import Path
 
 import matplotlib as mpl
 import numpy as np
 import pkg_resources
 from matplotlib.legend import Legend
 from matplotlib.rcsetup import validate_aspect, validate_float
 from nexusformat.nexus import (NeXusError, NXattr, NXdata, NXentry, NXfield,
@@ -4454,28 +4454,27 @@
             self.directorybox('Choose plugin directory'),
             self.radiobuttons(
                 ('local', 'Install locally', True),
                 ('nexpy', 'Install in NeXpy', False)),
             self.close_buttons())
         self.set_title('Installing Plugin')
 
-    def get_menu_name(self, plugin_name, plugin_path):
+    def get_menu_info(self, plugin_name, plugin_path):
         try:
             plugin_module = import_plugin(plugin_name, [plugin_path])
-            name, _ = plugin_module.plugin_menu()
-            return name
+            return plugin_module.plugin_menu()
         except Exception as error:
             report_error("Installing Plugin", error)
 
     def install_plugin(self):
         plugin_directory = self.get_directory()
         plugin_name = os.path.basename(os.path.normpath(plugin_directory))
         plugin_path = os.path.dirname(plugin_directory)
-        plugin_menu_name = self.get_menu_name(plugin_name, plugin_path)
-        if plugin_menu_name is None:
+        name, actions = self.get_menu_info(plugin_name, plugin_path)
+        if name is None:
             raise NeXusError("This directory does not contain a valid plugin")
         if self.radiobutton['local'].isChecked():
             plugin_path = self.local_directory
         else:
             plugin_path = self.nexpy_directory
         installed_path = os.path.join(plugin_path, plugin_name)
         if os.path.exists(installed_path):
@@ -4488,17 +4487,17 @@
                                              os.path.join(backup, plugin_name))
                 self.mainwindow.settings.save()
             else:
                 return
         shutil.copytree(plugin_directory, installed_path)
         for action in [action for action
                        in self.mainwindow.menuBar().actions()
-                       if action.text() == plugin_menu_name]:
+                       if action.text() == name]:
             self.mainwindow.menuBar().removeAction(action)
-        self.mainwindow.add_plugin_menu(plugin_name, [plugin_path])
+        self.mainwindow.add_plugin_menu(name, actions)
 
     def accept(self):
         try:
             self.install_plugin()
             super().accept()
         except NeXusError as error:
             report_error("Installing plugin", error)
@@ -4507,67 +4506,66 @@
 class RemovePluginDialog(NXDialog):
     """Dialog to remove a NeXus plugin"""
 
     def __init__(self, parent=None):
 
         super().__init__(parent=parent)
 
-        self.local_directory = self.mainwindow.plugin_dir
-        self.nexpy_directory = pkg_resources.resource_filename('nexpy',
-                                                               'plugins')
-        self.backup_dir = self.mainwindow.backup_dir
+        self.local_directory = Path(self.mainwindow.plugin_dir)
+        self.nexpy_directory = Path(pkg_resources.resource_filename('nexpy',
+                                                                    'plugins'))
+        self.backup_dir = Path(self.mainwindow.backup_dir)
+
+        local_plugins = []
+        for item in self.local_directory.iterdir():
+            if item.is_dir() and not item.name.startswith('_'):
+                local_plugins.append(
+                    self.checkboxes((str(item), '   ' + item.name, False),
+                                    align='left'))
+        nexpy_plugins = []
+        for item in self.nexpy_directory.iterdir():
+            if item.is_dir() and not item.name.startswith('_'):
+                nexpy_plugins.append(
+                    self.checkboxes((str(item), '   ' + item.name, False),
+                                    align='left'))
+
+        if len(local_plugins) == 0 and len(nexpy_plugins) == 0:
+            self.display_message('Removing Plugins', 'No plugins to remove')
+            self.reject()
+        elif len(local_plugins) == 0:
+            self.set_layout(NXLabel("NeXpy Plugins", bold=True),
+                            *nexpy_plugins,
+                            self.close_buttons())
+        elif len(nexpy_plugins) == 0:
+            self.set_layout(NXLabel("Local Plugins", bold=True),
+                            *local_plugins,
+                            self.close_buttons())
+        else:
+            self.set_layout(NXLabel("Local Plugins", bold=True),
+                            *local_plugins,
+                            NXLabel("NeXpy Plugins", bold=True),
+                            *nexpy_plugins,
+                            self.close_buttons())
 
-        self.setWindowTitle("Remove Plugin")
-
-        self.set_layout(self.directorybox('Choose plugin directory'),
-                        self.radiobuttons(('local', 'Local plugin', True),
-                                          ('nexpy', 'NeXpy plugin', False)),
-                        self.close_buttons())
         self.set_title('Removing Plugin')
-        self.radiobutton['local'].clicked.connect(self.set_local_directory)
-        self.radiobutton['nexpy'].clicked.connect(self.set_nexpy_directory)
-        self.set_local_directory()
-
-    def set_local_directory(self):
-        self.set_default_directory(self.local_directory)
-        self.directoryname.setText(self.local_directory)
-
-    def set_nexpy_directory(self):
-        self.set_default_directory(self.nexpy_directory)
-        self.directoryname.setText(self.nexpy_directory)
-
-    def get_menu_name(self, plugin_name, plugin_path):
-        try:
-            plugin_module = import_plugin(plugin_name, [plugin_path])
-            name, _ = plugin_module.plugin_menu()
-            return name
-        except Exception:
-            return None
 
     def remove_plugin(self):
-        plugin_directory = self.get_directory()
-        if (os.path.dirname(plugin_directory) != self.local_directory and
-                os.path.dirname(plugin_directory) != self.nexpy_directory):
-            raise NeXusError(
-                f"Directory '{plugin_directory}' not in plugins directory")
-        plugin_name = os.path.basename(os.path.normpath(plugin_directory))
-        plugin_menu_name = self.get_menu_name(plugin_name, plugin_directory)
-        if plugin_menu_name is None:
-            raise NeXusError("This directory does not contain a valid plugin")
-        if os.path.exists(plugin_directory):
-            if self.confirm_action(f"Remove '{plugin_directory}'?",
-                                   "This cannot be reversed"):
-                backup = os.path.join(self.backup_dir, timestamp())
-                os.mkdir(backup)
-                shutil.move(plugin_directory, backup)
-                self.mainwindow.settings.set('plugins',
-                                             os.path.join(backup, plugin_name))
+        for plugin_path in self.checkbox:
+            plugin_name = Path(plugin_path).name
+            if self.checkbox[plugin_path].isChecked():
+                if self.confirm_action(f"Remove '{plugin_path}'?",
+                                       "This cannot be reversed"):
+                    backup_path = self.backup_dir / timestamp()
+                    backup_path.mkdir()
+                    shutil.move(str(plugin_path), str(backup_path))
+                    self.mainwindow.settings.set(
+                        'plugins', str(backup_path.joinpath(plugin_name)))
                 self.mainwindow.settings.save()
             else:
-                return
+                continue
         for action in [action for action
                        in self.mainwindow.menuBar().actions()
                        if action.text().lower() == plugin_name.lower()]:
             self.mainwindow.menuBar().removeAction(action)
 
     def accept(self):
         try:
@@ -4617,21 +4615,20 @@
         self.set_layout(*items)
 
         self.set_title('Restore Plugin')
 
     def get_name(self, plugin):
         return os.path.basename(plugin)
 
-    def get_menu_name(self, plugin_name, plugin_path):
+    def get_menu_info(self, plugin_name, plugin_path):
         try:
             plugin_module = import_plugin(plugin_name, [plugin_path])
-            name, _ = plugin_module.plugin_menu()
-            return name
-        except Exception:
-            return None
+            return plugin_module.plugin_menu()
+        except Exception as error:
+            report_error("Restoring Plugin", error)
 
     def remove_backup(self, backup):
         shutil.rmtree(os.path.dirname(os.path.realpath(backup)))
         self.mainwindow.settings.remove_option('plugins', backup)
         self.mainwindow.settings.save()
 
     def restore(self):
@@ -4639,36 +4636,36 @@
         for plugin_directory in self.plugins:
             if self.radiobutton[plugin_directory].isChecked():
                 plugin_name = os.path.basename(plugin_directory)
                 break
         if plugin_name is None:
             return
         plugin_path = os.path.dirname(plugin_directory)
-        plugin_menu_name = self.get_menu_name(plugin_name, plugin_path)
-        if plugin_menu_name is None:
+        name, actions = self.get_menu_info(plugin_name, plugin_path)
+        if name is None:
             raise NeXusError("This directory does not contain a valid plugin")
         if self.radiobutton['local'].isChecked():
             plugin_path = self.local_directory
         else:
             plugin_path = self.nexpy_directory
         restored_path = os.path.join(plugin_path, plugin_name)
         if os.path.exists(restored_path):
             if self.confirm_action("Overwrite plugin?",
                                    f"Plugin '{plugin_name}' already exists"):
-                backup = os.path.join(self.backup_dir, timestamp())
-                os.mkdir(backup)
-                shutil.move(restored_path, backup)
-                self.mainwindow.settings.set('plugins',
-                                             os.path.join(backup, plugin_name))
+                backup_path = os.path.join(self.backup_dir, timestamp())
+                os.mkdir(backup_path)
+                shutil.move(restored_path, backup_path)
+                self.mainwindow.settings.set(
+                    'plugins', os.path.join(backup_path, plugin_name))
                 self.mainwindow.settings.save()
             else:
                 return
         shutil.copytree(plugin_directory, restored_path)
         self.remove_backup(plugin_directory)
 
         for action in [action for action
                        in self.mainwindow.menuBar().actions()
-                       if action.text() == plugin_menu_name]:
+                       if action.text() == name]:
             self.mainwindow.menuBar().removeAction(action)
-        self.mainwindow.add_plugin_menu(plugin_name, [plugin_path])
+        self.mainwindow.add_plugin_menu(name, actions)
 
         self.accept()
```

### Comparing `NeXpy-1.0.2/src/nexpy/gui/fitdialogs.py` & `NeXpy-1.0.3/src/nexpy/gui/fitdialogs.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/importdialog.py` & `NeXpy-1.0.3/src/nexpy/gui/importdialog.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/mainwindow.py` & `NeXpy-1.0.3/src/nexpy/gui/mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 import re
 import sys
 import webbrowser
 import xml.etree.ElementTree as ET
 from operator import attrgetter
 from pathlib import Path
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 import pkg_resources
 from nexusformat.nexus import (NeXusError, NXdata, NXentry, NXfield, NXFile,
                                NXgroup, NXlink, NXobject, NXprocess, NXroot,
                                nxcompleter, nxduplicate, nxgetconfig, nxload)
 from qtconsole.inprocess import QtInProcessKernelManager
 from qtconsole.rich_jupyter_widget import RichJupyterWidget
 
@@ -555,40 +560,76 @@
         self.fit_action = QtWidgets.QAction(
             "Fit Data", self, shortcut=QtGui.QKeySequence("Ctrl+Shift+F"),
             triggered=self.fit_data)
         self.add_menu_action(self.data_menu, self.fit_action)
 
     def init_plugin_menus(self):
         """Add an menu item for every module in the plugin menus"""
+        plugins = {}
         self.plugin_names = set()
-        private_path = self.plugin_dir
-        if os.path.isdir(private_path):
-            for name in os.listdir(private_path):
-                if (os.path.isdir(os.path.join(private_path, name)) and
-                        not (name.startswith('_') or name.startswith('.'))):
-                    self.plugin_names.add(name)
-        public_path = pkg_resources.resource_filename('nexpy', 'plugins')
-        for name in os.listdir(public_path):
-            if (os.path.isdir(os.path.join(public_path, name)) and
-                    not (name.startswith('_') or name.startswith('.'))):
-                self.plugin_names.add(name)
+        private_path = Path(self.plugin_dir)
+        for plugin_path in private_path.iterdir():
+            plugin_name = plugin_path.name
+            if (plugin_path.is_dir() and not (plugin_name.startswith('_') or
+                                              plugin_name.startswith('.'))):
+                self.plugin_names.add(plugin_name)
+                logging.info(
+                    f'Installing "{plugin_name}" plugin from "{plugin_path}"')
+        public_path = Path(pkg_resources.resource_filename('nexpy', 'plugins'))
+        for plugin_path in public_path.iterdir():
+            plugin_name = plugin_path.name
+            if plugin_name.lower() in [p.lower() for p in self.plugin_names]:
+                logging.warning(
+                    f'Duplicate plugin "{plugin_name}" not installed\n'
+                    + 36 * ' ' + f'located in "{plugin_path}"')
+                continue
+            if (plugin_path.is_dir() and not (plugin_name.startswith('_') or
+                                              plugin_name.startswith('.'))):
+                self.plugin_names.add(plugin_name)
+                logging.info(
+                    f'Installing "{plugin_name}" plugin from "{plugin_path}"')
         plugin_paths = [private_path, public_path]
         for plugin_name in set(sorted(self.plugin_names)):
             try:
-                self.add_plugin_menu(plugin_name, plugin_paths)
+                plugin_module = import_plugin(plugin_name, plugin_paths)
+                plugins[plugin_name] = plugin_module.plugin_menu
             except Exception as error:
-                logging.info(
+                logging.warning(
                     f'The "{plugin_name}" plugin could not be added '
-                    'to the main menu\n' + 33*' ' + f'{error}')
-
-    def add_plugin_menu(self, plugin_name, plugin_paths):
-        plugin_module = import_plugin(plugin_name, plugin_paths)
-        name, actions = plugin_module.plugin_menu()
-        plugin_menu = self.menu_bar.addMenu(name)
-        for action in actions:
+                    'to the main menu\n' + 36*' ' + f'Error: {error}')
+                self.plugin_names.remove(plugin_name)
+        for entry in entry_points(group='nexpy.plugins'):
+            plugin_name = entry.module.split('.')[-1]
+            if plugin_name.lower() in [p.lower() for p in self.plugin_names]:
+                logging.warning(
+                    f'Duplicate plugin "{entry.module}" not installed')
+                continue
+            else:
+                logging.info(
+                    f'Installing "{plugin_name}" '
+                    f'plugin from "{entry.module}" module')
+                self.plugin_names.add(plugin_name)
+            try:
+                plugins[plugin_name] = entry.load()
+            except Exception as error:
+                logging.warning(
+                    f'"{plugin_name}" could not be added to the main menu\n'
+                    + 36*' ' + f'Error: {error}')
+        for plugin in sorted(plugins):
+            try:
+                plugin_name, actions = plugins[plugin]()
+                self.add_plugin_menu(plugin_name, actions)
+            except Exception as error:
+                logging.warning(
+                    f'The "{plugin}" plugin could not be added '
+                    'to the main menu\n' + 36*' ' + f'Error: {error}')
+
+    def add_plugin_menu(self, plugin_name, plugin_actions):
+        plugin_menu = self.menu_bar.addMenu(plugin_name)
+        for action in plugin_actions:
             self.add_menu_action(plugin_menu, QtWidgets.QAction(
                 action[0], self, triggered=action[1]))
 
     def init_view_menu(self):
         self.view_menu = self.menu_bar.addMenu("&View")
 
         if sys.platform != 'darwin':
@@ -845,17 +886,17 @@
                 import_module = import_plugin(import_name, import_paths)
                 import_action = QtWidgets.QAction(
                     "Import "+import_module.filetype, self,
                     triggered=self.show_import_dialog)
                 self.add_menu_action(self.import_menu, import_action, self)
                 self.importer[import_action] = import_module
             except Exception as error:
-                logging.info(
+                logging.warning(
                     f'The "{import_name}" importer could not be added '
-                    'to the Import menu\n' + 33*' ' + f'{error}')
+                    'to the Import menu\n' + 36*' ' + f'Error: {error}')
 
     def new_workspace(self):
         try:
             dialog = NewDialog(parent=self)
             dialog.show()
         except NeXusError as error:
             report_error("Creating New Workspace", error)
```

### Comparing `NeXpy-1.0.2/src/nexpy/gui/plotview.py` & `NeXpy-1.0.3/src/nexpy/gui/plotview.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/pyqt.py` & `NeXpy-1.0.3/src/nexpy/gui/pyqt.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/back.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/back.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/customize.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/customize.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/equal.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/equal.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/export-data.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/export-data.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/export-figure.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/export-figure.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/filesave.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/filesave.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/forward.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/forward.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/hand.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/hand.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/home.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/home.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/icon/NeXpy.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/icon/NeXpy.svg` & `NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.svg`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/link-icon.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/link-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/lock-red-icon.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/lock-red-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/move.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/move.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/refresh-icon.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/refresh-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/subplots.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/subplots.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/unlock-red-icon.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/unlock-red-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/resources/zoom_to_rect.png` & `NeXpy-1.0.3/src/nexpy/gui/resources/zoom_to_rect.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/scripteditor.py` & `NeXpy-1.0.3/src/nexpy/gui/scripteditor.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/treeview.py` & `NeXpy-1.0.3/src/nexpy/gui/treeview.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/gui/utils.py` & `NeXpy-1.0.3/src/nexpy/gui/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,15 @@
         use(style)
     else:
         use('default')
 
 
 class NXimporter:
     def __init__(self, paths):
-        self.paths = paths
+        self.paths = [str(p) for p in paths]
 
     def __enter__(self):
         for path in reversed(self.paths):
             sys.path.insert(0, path)
 
     def __exit__(self, exc_type, exc_value, traceback):
         for path in self.paths:
```

### Comparing `NeXpy-1.0.2/src/nexpy/gui/widgets.py` & `NeXpy-1.0.3/src/nexpy/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/nexpygui.py` & `NeXpy-1.0.3/src/nexpy/nexpygui.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/readers/readspec.py` & `NeXpy-1.0.3/src/nexpy/readers/readspec.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/readers/readstack.py` & `NeXpy-1.0.3/src/nexpy/readers/readstack.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/readers/readtiff.py` & `NeXpy-1.0.3/src/nexpy/readers/readtiff.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/src/nexpy/readers/readtxt.py` & `NeXpy-1.0.3/src/nexpy/readers/readtxt.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.2/tests/test_imports.py` & `NeXpy-1.0.3/tests/test_imports.py`

 * *Files identical despite different names*

