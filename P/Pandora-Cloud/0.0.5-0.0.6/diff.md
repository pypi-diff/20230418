# Comparing `tmp/Pandora-Cloud-0.0.5.tar.gz` & `tmp/Pandora-Cloud-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-qmq7t_js/Pandora-Cloud-0.0.5.tar", last modified: Thu Apr  6 11:04:11 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-gr0r9gq2/Pandora-Cloud-0.0.6.tar", last modified: Tue Apr 18 02:07:40 2023, max compression
```

## Comparing `Pandora-Cloud-0.0.5.tar` & `Pandora-Cloud-0.0.6.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/Pandora_Cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/Pandora_Cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/Pandora_Cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/Pandora_Cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/Pandora_Cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105266 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305883 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-90236c4e04307644.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   154581 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-2b434f3f0b594dba.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/webpack-98709a717aa5cc1e.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108682 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/css/23406a6edf4b081a.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/ulp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/ulp/react-components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:04:11.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/flask/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-06 11:03:53.000000 Pandora-Cloud-0.0.5/src/pandora_cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/Pandora_Cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/Pandora_Cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/Pandora_Cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/Pandora_Cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/Pandora_Cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105266 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305883 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-90236c4e04307644.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   154581 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-2b434f3f0b594dba.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/webpack-98709a717aa5cc1e.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108682 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/css/23406a6edf4b081a.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/ulp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/ulp/react-components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:40.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/flask/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-18 02:07:29.000000 Pandora-Cloud-0.0.6/src/pandora_cloud/server.py
```

### Comparing `Pandora-Cloud-0.0.5/LICENSE` & `Pandora-Cloud-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/PKG-INFO` & `Pandora-Cloud-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-Cloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/pengzhile/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora-cloud
 Project-URL: Tracker, https://github.com/pengzhile/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `Pandora-Cloud-0.0.5/Pandora_Cloud.egg-info/PKG-INFO` & `Pandora-Cloud-0.0.6/Pandora_Cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-Cloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/pengzhile/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora-cloud
 Project-URL: Tracker, https://github.com/pengzhile/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `Pandora-Cloud-0.0.5/Pandora_Cloud.egg-info/SOURCES.txt` & `Pandora-Cloud-0.0.6/Pandora_Cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/README.md` & `Pandora-Cloud-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/setup.py` & `Pandora-Cloud-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-90236c4e04307644.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-90236c4e04307644.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-2b434f3f0b594dba.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-2b434f3f0b594dba.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/chunks/webpack-98709a717aa5cc1e.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/chunks/webpack-98709a717aa5cc1e.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/css/23406a6edf4b081a.css` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/css/23406a6edf4b081a.css`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/_buildManifest.js` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/_next/static/tTShkecJDS0nIc9faO2vC/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/apple-touch-icon.png` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/favicon-16x16.png` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/favicon-32x32.png` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff2` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff2` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff2` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff2` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Bold.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Italic.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Math-Italic.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Script-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/Signifier-Regular.otf` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/Sohne-Buch.otf` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/Sohne-Halbfett.otf` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/SohneMono-Buch.otf` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/fonts/SohneMono-Halbfett.otf` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/templates/chat.html` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/flask/templates/login.html` & `Pandora-Cloud-0.0.6/src/pandora_cloud/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.0.5/src/pandora_cloud/server.py` & `Pandora-Cloud-0.0.6/src/pandora_cloud/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def __init__(self, proxy, debug=False, sentry=False, login_local=False):
         self.proxy = proxy
         self.debug = debug
         self.sentry = sentry
         self.login_local = login_local
         self.log_level = logging.DEBUG if debug else logging.WARN
-        self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://chat.gateway.do')
+        self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://ai.fakeopen.com')
 
         hook_logging(level=self.log_level, format='[%(asctime)s] %(levelname)s in %(module)s: %(message)s')
         self.logger = logging.getLogger('waitress')
 
     def run(self, bind_str):
         host, port = self.__parse_bind(bind_str)
```

