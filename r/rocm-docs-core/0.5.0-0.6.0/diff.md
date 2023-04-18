# Comparing `tmp/rocm-docs-core-0.5.0.tar.gz` & `tmp/rocm-docs-core-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocm-docs-core-0.5.0.tar", last modified: Fri Apr 14 20:50:20 2023, max compression
+gzip compressed data, was "rocm-docs-core-0.6.0.tar", last modified: Tue Apr 18 04:25:35 2023, max compression
```

## Comparing `rocm-docs-core-0.5.0.tar` & `rocm-docs-core-0.6.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.317810 rocm-docs-core-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-14 20:50:20.317810 rocm-docs-core-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:50:20.317810 rocm-docs-core-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.305810 rocm-docs-core-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.309810 rocm-docs-core-0.5.0/src/rocm_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.305810 rocm-docs-core-0.5.0/src/rocm_docs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.309810 rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/
--rw-r--r--   0 runner    (1001) docker     (123)    72387 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/header.html
--rw-r--r--   0 runner    (1001) docker     (123)    37264 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/doxygen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.309810 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.309810 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/components/social-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.309810 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/sections/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.309810 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.305810 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.317810 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20756 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16748 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21924 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17872 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20780 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16808 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21876 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17876 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20672 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16756 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21820 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17780 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20172 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16372 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21248 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17384 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20664 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16696 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21520 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17544 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27552 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22132 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29388 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23712 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27592 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22184 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29392 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23824 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27456 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22212 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29224 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23676 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    26652 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    21516 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    28292 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22904 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27376 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22040 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    28704 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23168 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29304 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23704 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27520 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22084 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21856 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20712 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16740 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts.css
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.317810 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    10074 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-04-14 20:50:09.000000 rocm-docs-core-0.5.0/src/rocm_docs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:50:20.317810 rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-14 20:50:20.000000 rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-14 20:50:20.000000 rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:50:20.000000 rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 20:50:20.000000 rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 20:50:20.000000 rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 20:50:20.000000 rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.016565 rocm-docs-core-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-18 04:25:35.016565 rocm-docs-core-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 04:25:35.016565 rocm-docs-core-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/rocm_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/rocm_docs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/
+-rw-r--r--   0 runner    (1001) docker     (123)    72387 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37264 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/doxygen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/components/social-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.008565 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.004565 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.012565 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20756 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16748 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21924 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17872 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20780 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16808 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21876 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17876 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20672 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16756 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21820 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17780 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20172 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16372 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21248 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17384 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20664 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16696 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21520 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17544 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27552 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22132 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29388 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23712 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27592 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22184 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29392 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23824 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27456 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22212 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29224 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23676 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26652 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21516 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28292 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22904 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27376 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22040 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28704 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23168 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29304 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23704 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27520 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22084 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21856 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20712 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16740 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.012565 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10074 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-04-18 04:25:24.000000 rocm-docs-core-0.6.0/src/rocm_docs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:25:35.016565 rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-18 04:25:34.000000 rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-18 04:25:35.000000 rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 04:25:34.000000 rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 04:25:34.000000 rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-18 04:25:34.000000 rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 04:25:34.000000 rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/top_level.txt
```

### Comparing `rocm-docs-core-0.5.0/LICENSE.txt` & `rocm-docs-core-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/PKG-INFO` & `rocm-docs-core-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 0.5.0
+Version: 0.6.0
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm-docs-core-0.5.0/README.md` & `rocm-docs-core-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/pyproject.toml` & `rocm-docs-core-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'rocm-docs-core'
-version = "0.5.0"
+version = "0.6.0"
 authors=[
   {name="Lauren Wrubleski", email="Lauren.Wrubleski@amd.com"}
 ]
 description ='Core utilities for all ROCm documentation on RTD'
 readme="README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -55,12 +55,12 @@
 where=["src"]
 
 [tool.setuptools.package-data]
 rocm_docs = ["data/**/*", "rocm_docs_theme/**/*"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0"
+version = "0.6.0"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 annotated_tag = true
 major_version_zero = true
```

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/__init__.py` & `rocm-docs-core-0.6.0/src/rocm_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/core.py` & `rocm-docs-core-0.6.0/src/rocm_docs/core.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css` & `rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/header.html` & `rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/header.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/data/_doxygen/stylesheet.css` & `rocm-docs-core-0.6.0/src/rocm_docs/data/_doxygen/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/doxygen.py` & `rocm-docs-core-0.6.0/src/rocm_docs/doxygen.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/components/social-links.html` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/components/social-links.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/sections/footer.html` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/sections/footer.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/sections/header.html` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/sections/header.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     <div class="rocm-header-buttons">
         <a href="https://www.amd.com" target="_blank" class="rocm-header-link">
             <img id="amd-logo" alt="Advanced Micro Devices, Inc." src="{{ pathto('_static/images/rocm-logo.png',1) }}"></img>
             <div class="glow-wrap">
                 <i class="glow"></i>
             </div>
         </a>
-        <a href="{{ theme_repository_url }}" target="_blank" class="rocm-header-link">
+        <a href="https://github.com/RadeonOpenCompute/ROCm" target="_blank" class="rocm-header-link">
             <div class="rocm-link-box">
                 <p>GitHub</p>
             </div>
             <div class="glow-wrap">
                 <i class="glow"></i>
             </div>
         </a>
```

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts.css` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     margin-top:15px;
 }
 
 .rocm-footer ul {
     display: flex;
     flex-direction: row;
     flex-wrap: wrap;
-    font-size: 12px;
+    font-size: 14px;
     padding: 0;
     padding-bottom: 12px;
     width:98vw;
     list-style: none inside none;
     margin: 0;
 }
```

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css` & `rocm-docs-core-0.6.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/theme.py` & `rocm-docs-core-0.6.0/src/rocm_docs/theme.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs/util.py` & `rocm-docs-core-0.6.0/src/rocm_docs/util.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/PKG-INFO` & `rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 0.5.0
+Version: 0.6.0
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm-docs-core-0.5.0/src/rocm_docs_core.egg-info/SOURCES.txt` & `rocm-docs-core-0.6.0/src/rocm_docs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

