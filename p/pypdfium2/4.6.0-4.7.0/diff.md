# Comparing `tmp/pypdfium2-4.6.0.tar.gz` & `tmp/pypdfium2-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfium2-4.6.0.tar", last modified: Tue Apr 11 04:01:21 2023, max compression
+gzip compressed data, was "pypdfium2-4.7.0.tar", last modified: Tue Apr 18 04:01:49 2023, max compression
```

## Comparing `pypdfium2-4.6.0.tar` & `pypdfium2-4.7.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/.reuse/dep5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40453 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39350 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/setupsrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/autorelease.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11023 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/build_pdfium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/craft_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/packaging_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/setup_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/update_pdfium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/sourcebuild/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/sourcebuild/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/public_headers.patch
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/shared_library.patch
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/syslibs_sourcebuild.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/sourcebuild/patches/win/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/win/build.patch
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/win/pdfium.patch
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/win/resources.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/src/pypdfium2/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/src/pypdfium2/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/arrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/extract_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/imgtopdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/pdfinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/toc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/src/pypdfium2/_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    26676 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/textpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 04:01:04.000000 pypdfium2-4.6.0/src/pypdfium2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/src/pypdfium2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40453 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.832905 pypdfium2-4.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/.reuse/dep5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40343 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39240 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 04:01:49.832905 pypdfium2-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/setupsrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/autorelease.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11023 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/build_pdfium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/craft_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/packaging_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/setup_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/setupsrc/pypdfium2_setup/update_pdfium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/sourcebuild/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/sourcebuild/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/public_headers.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/shared_library.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/syslibs_sourcebuild.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.820905 pypdfium2-4.7.0/sourcebuild/patches/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/win/build.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/win/pdfium.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/sourcebuild/patches/win/resources.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.816904 pypdfium2-4.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.824905 pypdfium2-4.7.0/src/pypdfium2/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/src/pypdfium2/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/arrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/extract_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/imgtopdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/pdfinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_cli/toc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/src/pypdfium2/_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.828905 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27011 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/textpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/_helpers/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 04:00:51.000000 pypdfium2-4.7.0/src/pypdfium2/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-18 04:01:24.000000 pypdfium2-4.7.0/src/pypdfium2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:01:49.824905 pypdfium2-4.7.0/src/pypdfium2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40343 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 04:01:49.000000 pypdfium2-4.7.0/src/pypdfium2.egg-info/top_level.txt
```

### Comparing `pypdfium2-4.6.0/.reuse/dep5` & `pypdfium2-4.7.0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/LICENSES/Apache-2.0.txt` & `pypdfium2-4.7.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/LICENSES/BSD-3-Clause.txt` & `pypdfium2-4.7.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/LICENSES/CC-BY-4.0.txt` & `pypdfium2-4.7.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/LICENSES/LicenseRef-PdfiumThirdParty.txt` & `pypdfium2-4.7.0/LICENSES/LicenseRef-PdfiumThirdParty.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/MANIFEST.in` & `pypdfium2-4.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/PKG-INFO` & `pypdfium2-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.6.0
+Version: 4.7.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
@@ -139,27 +139,16 @@
   for i, image in zip(page_indices, renderer):
       image.save("out_%0*d.jpg" % (n_digits, i))
   ```
 
 * Read the table of contents
   ```python
   for item in pdf.get_toc():
-    
-      if item.n_kids == 0:
-          state = "*"
-      elif item.is_closed:
-          state = "-"
-      else:
-          state = "+"
-      
-      if item.page_index is None:
-          target = "?"
-      else:
-          target = item.page_index + 1
-      
+      state = "*" if item.n_kids == 0 else "-" if item.is_closed else "+"
+      target = "?" if item.page_index is None else item.page_index+1
       print(
           "    " * item.level +
           "[%s] %s -> %s  # %s %s" % (
               state, item.title, target, item.view_mode,
               [round(c, n_digits) for c in item.view_pos],
           )
       )
@@ -198,15 +187,15 @@
   # Extract text from the whole page
   text_all = textpage.get_text_range()
   # Extract text from a specific rectangular area
   text_part = textpage.get_text_bounded(left=50, bottom=100, right=width-50, top=height-100)
   
   # Locate text on the page
   searcher = textpage.search("something", match_case=False, match_whole_word=False)
-  # This will be a list of bounding boxes of the form (left, bottom, right, top)
+  # This returns the next occurrence as (char_index, char_count), or None if not found
   first_occurrence = searcher.get_next()
   ```
 
 * Create a new PDF with an empty A4 sized page
   ```python
   pdf = pdfium.PdfDocument.new()
   width, height = (595, 842)
```

### Comparing `pypdfium2-4.6.0/README.md` & `pypdfium2-4.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,27 +112,16 @@
   for i, image in zip(page_indices, renderer):
       image.save("out_%0*d.jpg" % (n_digits, i))
   ```
 
 * Read the table of contents
   ```python
   for item in pdf.get_toc():
-    
-      if item.n_kids == 0:
-          state = "*"
-      elif item.is_closed:
-          state = "-"
-      else:
-          state = "+"
-      
-      if item.page_index is None:
-          target = "?"
-      else:
-          target = item.page_index + 1
-      
+      state = "*" if item.n_kids == 0 else "-" if item.is_closed else "+"
+      target = "?" if item.page_index is None else item.page_index+1
       print(
           "    " * item.level +
           "[%s] %s -> %s  # %s %s" % (
               state, item.title, target, item.view_mode,
               [round(c, n_digits) for c in item.view_pos],
           )
       )
@@ -171,15 +160,15 @@
   # Extract text from the whole page
   text_all = textpage.get_text_range()
   # Extract text from a specific rectangular area
   text_part = textpage.get_text_bounded(left=50, bottom=100, right=width-50, top=height-100)
   
   # Locate text on the page
   searcher = textpage.search("something", match_case=False, match_whole_word=False)
-  # This will be a list of bounding boxes of the form (left, bottom, right, top)
+  # This returns the next occurrence as (char_index, char_count), or None if not found
   first_occurrence = searcher.get_next()
   ```
 
 * Create a new PDF with an empty A4 sized page
   ```python
   pdf = pdfium.PdfDocument.new()
   width, height = (595, 842)
```

### Comparing `pypdfium2-4.6.0/pyproject.toml` & `pypdfium2-4.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/setup.py` & `pypdfium2-4.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/autorelease.py` & `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/autorelease.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/build_pdfium.py` & `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/build_pdfium.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/craft_packages.py` & `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/craft_packages.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/packaging_base.py` & `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/packaging_base.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/setup_base.py` & `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/setup_base.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/update_pdfium.py` & `pypdfium2-4.7.0/setupsrc/pypdfium2_setup/update_pdfium.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/sourcebuild/patches/public_headers.patch` & `pypdfium2-4.7.0/sourcebuild/patches/public_headers.patch`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/sourcebuild/patches/win/build.patch` & `pypdfium2-4.7.0/sourcebuild/patches/win/build.patch`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/sourcebuild/patches/win/resources.rc` & `pypdfium2-4.7.0/sourcebuild/patches/win/resources.rc`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/__main__.py` & `pypdfium2-4.7.0/src/pypdfium2/__main__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/_parsers.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/_parsers.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/arrange.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/arrange.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/attachments.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/attachments.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/extract_images.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/extract_images.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/extract_text.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/extract_text.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/imgtopdf.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/imgtopdf.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/pageobjects.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/pageobjects.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/pdfinfo.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/pdfinfo.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/render.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/render.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_cli/tile.py` & `pypdfium2-4.7.0/src/pypdfium2/_cli/tile.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/__init__.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/bases.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,13 @@
         # TODO add needs_parent safety check (if True, `parent` must be given)
         if (parent is not None) and parent._tree_closed():
             print(f"Parent closed before child - this is illegal ({parent}, {raw}).", file=sys.stderr)
         close_func(raw, *args, **kwargs)
     
     
     def close(self):
-        # TODO? issue a warning if needs_free=False ?
         if (self.raw is None):
             logger.warning(f"Duplicate close call suppressed on {self}.")
             return
         if self._finalizer is not None:
             self._finalizer()
             self.raw = None
```

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/consts.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/consts.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/utils.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/attachment.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/attachment.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/bitmap.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/bitmap.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/document.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,31 +159,34 @@
             config = pdfium_c.FPDF_FORMFILLINFO(version=2)
         raw = pdfium_c.FPDFDOC_InitFormFillEnvironment(self, config)
         if not raw:
             raise PdfiumError(f"Initializing form env failed for document {self}.")
         self.formenv = PdfFormEnv(raw, config, self)
     
     
+    # ?TODO(v5) consider cached property
     def get_formtype(self):
         """
         Returns:
             int: PDFium form type that applies to the document (:attr:`FORMTYPE_*`).
             :attr:`FORMTYPE_NONE` if the document has no forms.
         """
         return pdfium_c.FPDF_GetFormType(self)
     
     
+    # ?TODO(v5) consider cached property
     def get_pagemode(self):
         """
         Returns:
             int: Page displaying mode (:attr:`PAGEMODE_*`).
         """
         return pdfium_c.FPDFDoc_GetPageMode(self)
     
     
+    # ?TODO(v5) consider cached property
     def is_tagged(self):
         """
         Returns:
             bool: Whether the document is tagged (cf. PDF 1.7, 10.7 "Tagged PDF").
         """
         return bool( pdfium_c.FPDFCatalog_IsTagged(self) )
     
@@ -462,30 +465,27 @@
         
         return PdfXObject(
             raw = raw_xobject,
             pdf = dest_pdf,
         )
     
     
+    # TODO(v5) consider switching to a wrapper around the raw bookmark with on-demand cached properties
     def _get_bookmark(self, bookmark, level):
         
         n_bytes = pdfium_c.FPDFBookmark_GetTitle(bookmark, None, 0)
         buffer = ctypes.create_string_buffer(n_bytes)
         pdfium_c.FPDFBookmark_GetTitle(bookmark, buffer, n_bytes)
         title = buffer.raw[:n_bytes-2].decode('utf-16-le')
         
+        # TODO(v5) just expose count as-is rather than using two variables and doing extra work
         count = pdfium_c.FPDFBookmark_GetCount(bookmark)
-        if count < 0:
-            is_closed = True
-        elif count == 0:
-            is_closed = None
-        else:
-            is_closed = False
-        
+        is_closed = True if count < 0 else None if count == 0 else False
         n_kids = abs(count)
+        
         dest = pdfium_c.FPDFBookmark_GetDest(self, bookmark)
         page_index = pdfium_c.FPDFDest_GetDestPageIndex(self, dest)
         if page_index == -1:
             page_index = None
         
         n_params = ctypes.c_ulong()
         view_pos = (pdfium_c.FS_FLOAT * 4)()
@@ -499,14 +499,15 @@
             n_kids = n_kids,
             page_index = page_index,
             view_mode = view_mode,
             view_pos = view_pos,
         )
     
     
+    # TODO(v5) change outline API (see above)
     def get_toc(
             self,
             max_depth = 15,
             parent = None,
             level = 0,
             seen = None,
         ):
@@ -723,14 +724,15 @@
     if pdfium_c.FPDF_GetPageCount(pdf) < 1:
         err_code = pdfium_c.FPDF_GetLastError()
         raise PdfiumError(f"Failed to load document (PDFium: {consts.ErrorToStr.get(err_code)}).")
     
     return pdf, to_hold, to_close
 
 
+# TODO(v5) change outline API (see above)
 PdfOutlineItem = namedtuple("PdfOutlineItem", "level title is_closed n_kids page_index view_mode view_pos")
 """
 Bookmark information.
 
 Parameters:
     level (int):
         Number of parent items.
```

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/matrix.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         self.a, self.b, self.c, self.d, self.e, self.f = a, b, c, d, e, f
     
     
     def __repr__(self):
         return f"PdfMatrix{self.get()}"
     
     
-    def __eq__(self, matrix):
-        if type(self) is not type(matrix):
+    def __eq__(self, other):
+        if type(self) is not type(other):
             return False
-        return (self.get() == matrix.get())
+        return (self.get() == other.get())
     
     
     @property
     def _as_parameter_(self):
         return ctypes.byref( self.to_raw() )
```

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/page.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/page.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -224,16 +224,16 @@
             pageobj (PdfObject): The page object to remove.
         """
                 
         if pageobj.page is not self:
             raise ValueError("The page object you attempted to remove is not part of this page.")
         
         pdfium_c.FPDFPage_RemoveObject(self, pageobj)
-        pageobj._attach_finalizer()
         pageobj.page = None
+        pageobj._attach_finalizer()
     
     
     def gen_content(self):
         """
         Generate page content to apply additions, removals or modifications of page objects.
         
         If page content was changed, this function should be called once before saving the document or re-loading the page.
```

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/pageobjects.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/pageobjects.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/textpage.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/textpage.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/_helpers/unsupported.py` & `pypdfium2-4.7.0/src/pypdfium2/_helpers/unsupported.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.6.0/src/pypdfium2/version.py` & `pypdfium2-4.7.0/src/pypdfium2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-FileCopyrightText: 2023 geisserml <geisserml@gmail.com>
 # SPDX-License-Identifier: Apache-2.0 OR BSD-3-Clause
 
 __all__ = ["V_PYPDFIUM2", "V_LIBPDFIUM", "V_BUILDNAME", "V_PDFIUM_IS_V8"]
 
 V_MAJOR = 4
-V_MINOR = 6
+V_MINOR = 7
 V_PATCH = 0
 V_BETA = None
 
 #: pypdfium2 version string
 V_PYPDFIUM2 = f"{V_MAJOR}.{V_MINOR}.{V_PATCH}"
 if V_BETA is not None:
     V_PYPDFIUM2 += f"b{V_BETA}"
 
 #: PDFium library version string (git tag or commit hash)
-V_LIBPDFIUM = "5705"
+V_LIBPDFIUM = "5715"
 
 #: String describing the included PDFium binary's origin (pdfium-binaries, source)
 V_BUILDNAME = "pdfium-binaries"
 
 #: Whether the included PDFium binary was built with V8 support or not
 V_PDFIUM_IS_V8 = False
```

### Comparing `pypdfium2-4.6.0/src/pypdfium2.egg-info/PKG-INFO` & `pypdfium2-4.7.0/src/pypdfium2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.6.0
+Version: 4.7.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
@@ -139,27 +139,16 @@
   for i, image in zip(page_indices, renderer):
       image.save("out_%0*d.jpg" % (n_digits, i))
   ```
 
 * Read the table of contents
   ```python
   for item in pdf.get_toc():
-    
-      if item.n_kids == 0:
-          state = "*"
-      elif item.is_closed:
-          state = "-"
-      else:
-          state = "+"
-      
-      if item.page_index is None:
-          target = "?"
-      else:
-          target = item.page_index + 1
-      
+      state = "*" if item.n_kids == 0 else "-" if item.is_closed else "+"
+      target = "?" if item.page_index is None else item.page_index+1
       print(
           "    " * item.level +
           "[%s] %s -> %s  # %s %s" % (
               state, item.title, target, item.view_mode,
               [round(c, n_digits) for c in item.view_pos],
           )
       )
@@ -198,15 +187,15 @@
   # Extract text from the whole page
   text_all = textpage.get_text_range()
   # Extract text from a specific rectangular area
   text_part = textpage.get_text_bounded(left=50, bottom=100, right=width-50, top=height-100)
   
   # Locate text on the page
   searcher = textpage.search("something", match_case=False, match_whole_word=False)
-  # This will be a list of bounding boxes of the form (left, bottom, right, top)
+  # This returns the next occurrence as (char_index, char_count), or None if not found
   first_occurrence = searcher.get_next()
   ```
 
 * Create a new PDF with an empty A4 sized page
   ```python
   pdf = pdfium.PdfDocument.new()
   width, height = (595, 842)
```

### Comparing `pypdfium2-4.6.0/src/pypdfium2.egg-info/SOURCES.txt` & `pypdfium2-4.7.0/src/pypdfium2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

