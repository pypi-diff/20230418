# Comparing `tmp/jupyterlite-xeus-nelson-0.1.2.tar.gz` & `tmp/jupyterlite-xeus-nelson-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlite-xeus-nelson-0.1.2.tar", last modified: Wed Jan 25 13:24:39 2023, max compression
+gzip compressed data, was "jupyterlite-xeus-nelson-0.1.4.tar", last modified: Tue Apr 18 12:12:48 2023, max compression
```

## Comparing `jupyterlite-xeus-nelson-0.1.2.tar` & `jupyterlite-xeus-nelson-0.1.4.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.606679 jupyterlite-xeus-nelson-0.1.2/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)       13 2023-01-23 09:53:25.000000 jupyterlite-xeus-nelson-0.1.2/CHANGELOG.md
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     1555 2023-01-23 10:26:51.000000 jupyterlite-xeus-nelson-0.1.2/LICENSE
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      472 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/MANIFEST.in
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3143 2023-01-25 13:24:39.606679 jupyterlite-xeus-nelson-0.1.2/PKG-INFO
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     2086 2023-01-25 09:16:57.000000 jupyterlite-xeus-nelson-0.1.2/README.md
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     1905 2023-01-23 10:29:52.000000 jupyterlite-xeus-nelson-0.1.2/RELEASE.md
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      207 2023-01-23 10:26:40.000000 jupyterlite-xeus-nelson-0.1.2/install.json
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.596679 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      318 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/__init__.py
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      625 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/_version.py
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.596679 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    21411 2023-01-25 13:16:09.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/build_log.json
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4569 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/package.json
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.600012 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     6561 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/553002d543a9199df1e32348f99812205fb446205bd319f902ff7f8a27525f28.png
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     1995 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/69da0ac9a09126e3c01831219b74572f3b76533e342c72f8afa9fd8f01dcc8e8.png
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    12565 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/lib_index_js.8e45cbd5afbccccbdcb9.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     8715 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/lib_index_js.8e45cbd5afbccccbdcb9.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    20935 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/lib_worker_js.3177b3190a3b02deab39.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    23980 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/lib_worker_js.3177b3190a3b02deab39.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    33452 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/remoteEntry.f6c9feae2afb81a029cd.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    32550 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/remoteEntry.f6c9feae2afb81a029cd.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3365 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/service-worker-b2fb40a.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      174 2023-01-25 13:16:09.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/style.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     5233 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/style_index_js.690ac903a232d2819aff.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     2468 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/style_index_js.690ac903a232d2819aff.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    12278 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_comlink_dist_esm_comlink_mjs.df200806e63bae502a62.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    13760 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_comlink_dist_esm_comlink_mjs.df200806e63bae502a62.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    12092 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.ab85181109b3273b0f75.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    13841 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.ab85181109b3273b0f75.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    95966 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_jupyterlite_contents_lib_index_js.4f8c5efe8f97d253068f.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    98985 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_jupyterlite_contents_lib_index_js.4f8c5efe8f97d253068f.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    85061 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_jupyterlite_server_lib_index_js.6c84e851f3b29f475bc0.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)    94167 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/vendors-node_modules_jupyterlite_server_lib_index_js.6c84e851f3b29f475bc0.js.map
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)   124359 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/xnelson_wasm.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)  1929041 2023-01-25 13:16:11.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/xnelson_wasm.wasm
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.596679 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson.egg-info/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3143 2023-01-25 13:24:39.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson.egg-info/PKG-INFO
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3065 2023-01-25 13:24:39.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson.egg-info/SOURCES.txt
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)        1 2023-01-25 13:24:39.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson.egg-info/dependency_links.txt
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)        1 2023-01-25 13:24:39.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson.egg-info/not-zip-safe
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)       24 2023-01-25 13:24:39.000000 jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson.egg-info/top_level.txt
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4427 2023-01-25 13:23:33.000000 jupyterlite-xeus-nelson-0.1.2/package.json
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      738 2023-01-23 10:29:30.000000 jupyterlite-xeus-nelson-0.1.2/pyproject.toml
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)       38 2023-01-25 13:24:39.606679 jupyterlite-xeus-nelson-0.1.2/setup.cfg
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     2887 2023-01-23 10:30:04.000000 jupyterlite-xeus-nelson-0.1.2/setup.py
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.603346 jupyterlite-xeus-nelson-0.1.2/src/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      205 2023-01-23 10:33:05.000000 jupyterlite-xeus-nelson-0.1.2/src/declarations.d.ts
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     2082 2023-01-23 10:34:52.000000 jupyterlite-xeus-nelson-0.1.2/src/index.ts
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4213 2023-01-25 13:15:25.000000 jupyterlite-xeus-nelson-0.1.2/src/nelson_data.data
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     6325 2023-01-25 13:15:25.000000 jupyterlite-xeus-nelson-0.1.2/src/nelson_data.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4998 2023-01-25 13:15:25.000000 jupyterlite-xeus-nelson-0.1.2/src/web_worker_kernel.ts
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     5230 2023-01-25 13:15:51.000000 jupyterlite-xeus-nelson-0.1.2/src/worker.ts
--rwxr-xr-x   0 yoyo      (1000) yoyo      (1000)   124359 2023-01-25 13:15:25.000000 jupyterlite-xeus-nelson-0.1.2/src/xnelson_wasm.js
--rwxr-xr-x   0 yoyo      (1000) yoyo      (1000)  1929041 2023-01-25 13:15:25.000000 jupyterlite-xeus-nelson-0.1.2/src/xnelson_wasm.wasm
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.606679 jupyterlite-xeus-nelson-0.1.2/style/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      291 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/style/base.css
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      318 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/style/index.css
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      314 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/style/index.js
-drwxr-xr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-01-25 13:24:39.606679 jupyterlite-xeus-nelson-0.1.2/style/logos/
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     1995 2023-01-24 20:46:45.000000 jupyterlite-xeus-nelson-0.1.2/style/logos/nelson-logo-32x32.png
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     6561 2023-01-24 20:46:45.000000 jupyterlite-xeus-nelson-0.1.2/style/logos/nelson-logo-64x64.png
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      581 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/tsconfig.json
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      302 2023-01-23 10:30:16.000000 jupyterlite-xeus-nelson-0.1.2/webpack.config.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)      513 2023-01-23 09:52:16.000000 jupyterlite-xeus-nelson-0.1.2/worker.webpack.config.js
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)   160761 2023-01-24 10:39:43.000000 jupyterlite-xeus-nelson-0.1.2/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.151895 jupyterlite-xeus-nelson-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-18 12:10:35.000000 jupyterlite-xeus-nelson-0.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-18 12:12:48.151895 jupyterlite-xeus-nelson-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.143895 jupyterlite-xeus-nelson-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/docs/build-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/docs/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.143895 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.143895 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-18 12:12:48.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-18 12:12:48.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:12:48.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:12:47.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 12:12:48.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 12:12:48.000000 jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-18 12:10:32.000000 jupyterlite-xeus-nelson-0.1.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:12:48.151895 jupyterlite-xeus-nelson-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.139895 jupyterlite-xeus-nelson-0.1.4/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.139895 jupyterlite-xeus-nelson-0.1.4/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.139895 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.139895 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.143895 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.147895 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/213.f89a101850d49609bb95.js
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/213.f89a101850d49609bb95.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/553002d543a9199df1e32348f99812205fb446205bd319f902ff7f8a27525f28.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/69da0ac9a09126e3c01831219b74572f3b76533e342c72f8afa9fd8f01dcc8e8.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/708.7d4632730c6b1fa3bea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/747.b536d06e617484e9cba5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/870.a200ec1fdeec561413b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/870.a200ec1fdeec561413b1.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/remoteEntry.1d3ddca10c4c40c38bea.js
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-18 12:11:58.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)    75600 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/xnelson_wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4197908 2023-04-18 12:12:00.000000 jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/xnelson_wasm.wasm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.151895 jupyterlite-xeus-nelson-0.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/src/declarations.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/src/index.ts
+-rw-rw-r--   0 runner    (1001) docker     (123)     4998 2022-11-17 22:27:03.000000 jupyterlite-xeus-nelson-0.1.4/src/web_worker_kernel.ts
+-rw-rw-r--   0 runner    (1001) docker     (123)     5228 2023-04-18 12:11:42.000000 jupyterlite-xeus-nelson-0.1.4/src/worker.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.151895 jupyterlite-xeus-nelson-0.1.4/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:12:48.151895 jupyterlite-xeus-nelson-0.1.4/style/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/style/logos/nelson-logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/style/logos/nelson-logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/worker.webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-04-18 12:10:30.000000 jupyterlite-xeus-nelson-0.1.4/yarn.lock
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/LICENSE` & `jupyterlite-xeus-nelson-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/PKG-INFO` & `jupyterlite-xeus-nelson-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: jupyterlite-xeus-nelson
-Version: 0.1.2
-Summary: A Lua kernel for JupyterLite, powered by Xeus
+Version: 0.1.4
+Summary: A Nelson kernel for JupyterLite, powered by Xeus
 Home-page: https://github.com/jupyterlite/xeus-nelson-kernel
-Author: Thorsten Beier, JupyterLite Contributors
-Author-email: 
+Author: JupyterLite Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# jupyterlite-xeus-nelson-kernel
+# jupyterlite-xeus-nelson
 
-A NelSon kernel for JupyterLite running in the browser.
+The [xeus-nelson](https://github.com/jupyter-xeus/xeus-nelson) Nelson kernel for JupyterLite running in the browser.
 
 ## Requirements
 
-- JupyterLite >= 0.1.0b16
+- jupyterlite-core >= 0.1.0b20
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlite_xeus_nelson
+pip install jupyterlite-xeus-nelson
 ```
 
 Then build your JupyterLite site:
 
 ```bash
 jupyter lite build
 ```
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/README.md` & `jupyterlite-xeus-nelson-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# jupyterlite-xeus-nelson-kernel
+# jupyterlite-xeus-nelson
 
-A NelSon kernel for JupyterLite running in the browser.
+The [xeus-nelson](https://github.com/jupyter-xeus/xeus-nelson) Nelson kernel for JupyterLite running in the browser.
 
 ## Requirements
 
-- JupyterLite >= 0.1.0b16
+- jupyterlite-core >= 0.1.0b20
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlite_xeus_nelson
+pip install jupyterlite-xeus-nelson
 ```
 
 Then build your JupyterLite site:
 
 ```bash
 jupyter lite build
 ```
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/RELEASE.md` & `jupyterlite-xeus-nelson-0.1.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/package.json` & `jupyterlite-xeus-nelson-0.1.4/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8533633751306163%*

 * *Differences: {"'author'": "'JupyterLite Contributors'",*

 * * "'dependencies'": "{'@jupyterlite/server': '^0.1.0-beta.20', '@jupyterlite/kernel': "*

 * *                   "'^0.1.0-beta.20', delete: ['@jupyterlite/contents']}",*

 * * "'description'": "'A Nelson kernel for JupyterLite, powered by Xeus'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.4.1', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^5.57.1', '@typescript-eslint/parser': '^5.57.1', 'file-loader': '^6.2.0'}",*

 * * "'jupyterlab'": "{'outputDir': 'share/ […]*

```diff
@@ -1,62 +1,48 @@
 {
-    "author": {
-        "email": "",
-        "name": "Thorsten Beier, JupyterLite Contributors"
-    },
+    "author": "JupyterLite Contributors",
     "bugs": {
         "url": "https://github.com/jupyterlite/xeus-nelson-kernel/issues"
     },
     "dependencies": {
-        "@jupyterlite/contents": "^0.1.0-beta.16",
-        "@jupyterlite/server": "^0.1.0-beta.16",
+        "@jupyterlite/kernel": "^0.1.0-beta.20",
+        "@jupyterlite/server": "^0.1.0-beta.20",
         "comlink": "^4.3.1"
     },
-    "description": "A Lua kernel for JupyterLite, powered by Xeus",
+    "description": "A Nelson kernel for JupyterLite, powered by Xeus",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
+        "@jupyterlab/builder": "^3.4.1",
+        "@typescript-eslint/eslint-plugin": "^5.57.1",
+        "@typescript-eslint/parser": "^5.57.1",
         "copy-webpack-plugin": "^9.0.1",
         "copyfiles": "^2.4.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
+        "file-loader": "^6.2.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "shx": "^0.3.0",
         "source-map-loader": "^4.0.0",
         "typescript": "~4.2.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf,wasm}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlite/xeus-nelson-kernel",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
-            ]
-        },
-        "skip": [
-            "check-links"
-        ]
-    },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.f6c9feae2afb81a029cd.js",
-            "style": "./style"
-        },
         "extension": true,
-        "outputDir": "jupyterlite_xeus_nelson/labextension",
+        "outputDir": "share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel",
         "sharedPackages": {
+            "@jupyterlite/contents": {
+                "bundled": false,
+                "singleton": true
+            },
             "@jupyterlite/kernel": {
                 "bundled": false,
                 "singleton": true
             }
         },
         "webpackConfig": "./webpack.config.js"
     },
@@ -76,45 +62,40 @@
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterlite/xeus-nelson-kernel.git"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:worker && jlpm run copy-files && jlpm run build:labextension:dev",
-        "build:dockerimage": "docker build -t mydockerimage --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) . ",
-        "build:dockerimage_no_cache": "docker build -t mydockerimage  --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) --no-cache . ",
-        "build:emscripten": "echo $(pwd) && docker run --rm -v $(pwd):/src -u $(id -u):$(id -g) mydockerimage ./copy_output.sh",
+        "build": "jlpm run build:xeus-nelson && jlpm run build:lib && jlpm run build:worker && jlpm run copy-files && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": " jlpm run sed-worker && tsc",
-        "build:prod": "jlpm run clean && jlpm run build:wasm && jlpm run build:lib && jlpm run build:worker:prod && jlpm run copy-files && jlpm run build:labextension",
-        "build:wasm": "jlpm run build:dockerimage && jlpm run build:emscripten",
-        "build:wasm_no_cache": "jlpm run build:dockerimage_no_cache && jlpm run build:emscripten",
+        "build:lib": "tsc",
+        "build:prod": "jlpm run clean && jlpm run build build:xeus-nelson && jlpm run build:lib && jlpm run build:worker:prod && jlpm run copy-files && jlpm run build:labextension",
         "build:worker": "webpack --config worker.webpack.config.js --mode=development",
         "build:worker:prod": "webpack --config worker.webpack.config.js --mode=production",
+        "build:xeus-nelson": "python jupyterlite_xeus_nelson/build.py --output-path src --build-worker",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyterlite_xeus_nelson/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "copy-files": "copyfiles -u 1 src/xnelson_wasm.wasm src/xnelson_wasm.js lib",
+        "copy-files": "copyfiles -u 1 src/xnelson_wasm.wasm src/xnelson_wasm.js src/*.data src/*.js lib",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install:extension": "jlpm run build",
         "lint": "jlpm prettier && yarn eslint",
         "lint:check": "jlpm prettier:check && yarn eslint:check",
         "prettier": "prettier --list-different --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.html}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.html}\"",
-        "sed-worker": "shx sed -i \"s/XEUS_KERNEL_FILE/'.\\/xnelson_wasm.js'/\" src/worker.ts && shx sed -i \"s/LANGUAGE_DATA_FILE/''/\" src/worker.ts ",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.4"
 }
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/553002d543a9199df1e32348f99812205fb446205bd319f902ff7f8a27525f28.png` & `jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/553002d543a9199df1e32348f99812205fb446205bd319f902ff7f8a27525f28.png`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson/labextension/static/69da0ac9a09126e3c01831219b74572f3b76533e342c72f8afa9fd8f01dcc8e8.png` & `jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/static/69da0ac9a09126e3c01831219b74572f3b76533e342c72f8afa9fd8f01dcc8e8.png`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/jupyterlite_xeus_nelson.egg-info/PKG-INFO` & `jupyterlite-xeus-nelson-0.1.4/jupyterlite_xeus_nelson.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: jupyterlite-xeus-nelson
-Version: 0.1.2
-Summary: A Lua kernel for JupyterLite, powered by Xeus
+Version: 0.1.4
+Summary: A Nelson kernel for JupyterLite, powered by Xeus
 Home-page: https://github.com/jupyterlite/xeus-nelson-kernel
-Author: Thorsten Beier, JupyterLite Contributors
-Author-email: 
+Author: JupyterLite Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# jupyterlite-xeus-nelson-kernel
+# jupyterlite-xeus-nelson
 
-A NelSon kernel for JupyterLite running in the browser.
+The [xeus-nelson](https://github.com/jupyter-xeus/xeus-nelson) Nelson kernel for JupyterLite running in the browser.
 
 ## Requirements
 
-- JupyterLite >= 0.1.0b16
+- jupyterlite-core >= 0.1.0b20
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlite_xeus_nelson
+pip install jupyterlite-xeus-nelson
 ```
 
 Then build your JupyterLite site:
 
 ```bash
 jupyter lite build
 ```
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/package.json` & `jupyterlite-xeus-nelson-0.1.4/share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8533633751306163%*

 * *Differences: {"'author'": "'JupyterLite Contributors'",*

 * * "'dependencies'": "{'@jupyterlite/server': '^0.1.0-beta.20', '@jupyterlite/kernel': "*

 * *                   "'^0.1.0-beta.20', delete: ['@jupyterlite/contents']}",*

 * * "'description'": "'A Nelson kernel for JupyterLite, powered by Xeus'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.4.1', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^5.57.1', '@typescript-eslint/parser': '^5.57.1', 'file-loader': '^6.2.0'}",*

 * * "'jupyterlab'": "{'outputDir': 'share/ […]*

```diff
@@ -1,57 +1,53 @@
 {
-    "author": {
-        "email": "",
-        "name": "Thorsten Beier, JupyterLite Contributors"
-    },
+    "author": "JupyterLite Contributors",
     "bugs": {
         "url": "https://github.com/jupyterlite/xeus-nelson-kernel/issues"
     },
     "dependencies": {
-        "@jupyterlite/contents": "^0.1.0-beta.16",
-        "@jupyterlite/server": "^0.1.0-beta.16",
+        "@jupyterlite/kernel": "^0.1.0-beta.20",
+        "@jupyterlite/server": "^0.1.0-beta.20",
         "comlink": "^4.3.1"
     },
-    "description": "A Lua kernel for JupyterLite, powered by Xeus",
+    "description": "A Nelson kernel for JupyterLite, powered by Xeus",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
+        "@jupyterlab/builder": "^3.4.1",
+        "@typescript-eslint/eslint-plugin": "^5.57.1",
+        "@typescript-eslint/parser": "^5.57.1",
         "copy-webpack-plugin": "^9.0.1",
         "copyfiles": "^2.4.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
+        "file-loader": "^6.2.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "shx": "^0.3.0",
         "source-map-loader": "^4.0.0",
         "typescript": "~4.2.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf,wasm}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlite/xeus-nelson-kernel",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
-            ]
-        },
-        "skip": [
-            "check-links"
-        ]
-    },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.1d3ddca10c4c40c38bea.js",
+            "style": "./style"
+        },
         "extension": true,
-        "outputDir": "jupyterlite_xeus_nelson/labextension",
+        "outputDir": "share/jupyter/labextensions/@jupyterlite/xeus-nelson-kernel",
         "sharedPackages": {
+            "@jupyterlite/contents": {
+                "bundled": false,
+                "singleton": true
+            },
             "@jupyterlite/kernel": {
                 "bundled": false,
                 "singleton": true
             }
         },
         "webpackConfig": "./webpack.config.js"
     },
@@ -71,45 +67,40 @@
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterlite/xeus-nelson-kernel.git"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:worker && jlpm run copy-files && jlpm run build:labextension:dev",
-        "build:dockerimage": "docker build -t mydockerimage --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) . ",
-        "build:dockerimage_no_cache": "docker build -t mydockerimage  --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) --no-cache . ",
-        "build:emscripten": "echo $(pwd) && docker run --rm -v $(pwd):/src -u $(id -u):$(id -g) mydockerimage ./copy_output.sh",
+        "build": "jlpm run build:xeus-nelson && jlpm run build:lib && jlpm run build:worker && jlpm run copy-files && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": " jlpm run sed-worker && tsc",
-        "build:prod": "jlpm run clean && jlpm run build:wasm && jlpm run build:lib && jlpm run build:worker:prod && jlpm run copy-files && jlpm run build:labextension",
-        "build:wasm": "jlpm run build:dockerimage && jlpm run build:emscripten",
-        "build:wasm_no_cache": "jlpm run build:dockerimage_no_cache && jlpm run build:emscripten",
+        "build:lib": "tsc",
+        "build:prod": "jlpm run clean && jlpm run build build:xeus-nelson && jlpm run build:lib && jlpm run build:worker:prod && jlpm run copy-files && jlpm run build:labextension",
         "build:worker": "webpack --config worker.webpack.config.js --mode=development",
         "build:worker:prod": "webpack --config worker.webpack.config.js --mode=production",
+        "build:xeus-nelson": "python jupyterlite_xeus_nelson/build.py --output-path src --build-worker",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyterlite_xeus_nelson/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "copy-files": "copyfiles -u 1 src/xnelson_wasm.wasm src/xnelson_wasm.js lib",
+        "copy-files": "copyfiles -u 1 src/xnelson_wasm.wasm src/xnelson_wasm.js src/*.data src/*.js lib",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install:extension": "jlpm run build",
         "lint": "jlpm prettier && yarn eslint",
         "lint:check": "jlpm prettier:check && yarn eslint:check",
         "prettier": "prettier --list-different --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.html}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.html}\"",
-        "sed-worker": "shx sed -i \"s/XEUS_KERNEL_FILE/'.\\/xnelson_wasm.js'/\" src/worker.ts && shx sed -i \"s/LANGUAGE_DATA_FILE/''/\" src/worker.ts ",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.4"
 }
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/setup.py` & `jupyterlite-xeus-nelson-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,86 +8,104 @@
 import setuptools
 
 HERE = Path(__file__).parent.resolve()
 
 # The name of the project
 name = "jupyterlite-xeus-nelson"
 
-lab_path = (HERE / name.replace("-", "_") / "labextension")
+lab_path = (
+    HERE / "share" / "jupyter" / "labextensions" / "@jupyterlite" / "xeus-nelson-kernel"
+)
 
 # Representative files that should exist after a successful build
 ensured_targets = [
     str(lab_path / "package.json"),
-    str(lab_path / "static/style.js")
+#    str(lab_path / "static" / "nelson_data.js"),
+    str(lab_path / "static" / "xnelson_wasm.js"),
+    str(lab_path / "static" / "xnelson_wasm.wasm"),
+    str(lab_path / "static" / "style.js"),
 ]
 
 labext_name = "@jupyterlite/xeus-nelson-kernel"
 
 data_files_spec = [
-    ("share/jupyter/labextensions/%s" % labext_name, str(lab_path.relative_to(HERE)), "**"),
+    (
+        "share/jupyter/labextensions/%s" % labext_name,
+        str(lab_path.relative_to(HERE)),
+        "**",
+    ),
     ("share/jupyter/labextensions/%s" % labext_name, str("."), "install.json"),
 ]
 
 long_description = (HERE / "README.md").read_text()
 
 # Get the package info from package.json
 pkg_json = json.loads((HERE / "package.json").read_bytes())
 version = (
     pkg_json["version"]
     .replace("-alpha.", "a")
     .replace("-beta.", "b")
     .replace("-rc.", "rc")
-) 
+)
 
 setup_args = dict(
     name=name,
     version=version,
     url=pkg_json["homepage"],
-    author=pkg_json["author"]["name"],
-    author_email=pkg_json["author"]["email"],
+    author=pkg_json["author"],
     description=pkg_json["description"],
     license=pkg_json["license"],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
-    install_requires=[],
+    packages=setuptools.find_packages(exclude=["tests"]),
+    install_requires=[
+        "traitlets",
+        "jupyterlite-core>=0.1.0b20",
+        "requests",
+        "empack>=2.0.9,<3",
+        "typer",
+    ],
     zip_safe=False,
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Jupyter",
         "Framework :: Jupyter :: JupyterLab",
         "Framework :: Jupyter :: JupyterLab :: 3",
         "Framework :: Jupyter :: JupyterLab :: Extensions",
         "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     ],
 )
 
 try:
-    from jupyter_packaging import (
-        wrap_installers,
-        npm_builder,
-        get_data_files
-    )
+    from jupyter_packaging import wrap_installers, npm_builder, get_data_files
+
     post_develop = npm_builder(
-        build_cmd="build:prod", source_dir="src", build_dir=lab_path
+        build_cmd="build:prod", source_dir="src", build_dir=lab_path, npm=["jlpm"]
+    )
+    setup_args["cmdclass"] = wrap_installers(
+        post_develop=post_develop, ensured_targets=ensured_targets
     )
-    setup_args["cmdclass"] = wrap_installers(post_develop=post_develop, ensured_targets=ensured_targets)
     setup_args["data_files"] = get_data_files(data_files_spec)
 except ImportError as e:
     import logging
+
     logging.basicConfig(format="%(levelname)s: %(message)s")
-    logging.warning("Build tool `jupyter-packaging` is missing. Install it with pip or conda.")
+    logging.warning(
+        "Build tool `jupyter-packaging` is missing. Install it with pip or conda."
+    )
     if not ("--name" in sys.argv or "--version" in sys.argv):
         raise e
 
 if __name__ == "__main__":
     setuptools.setup(**setup_args)
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/src/web_worker_kernel.ts` & `jupyterlite-xeus-nelson-0.1.4/src/web_worker_kernel.ts`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/src/worker.ts` & `jupyterlite-xeus-nelson-0.1.4/src/worker.ts`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   IStats
 } from '@jupyterlite/contents';
 
 declare function createXeusModule(options: any): any;
 
 globalThis.Module = {};
 
-const WASM_KERNEL_FILE = './xnelson_wasm.js';
+const WASM_KERNEL_FILE = 'xnelson_wasm.js';
 const DATA_FILE = '';
 
 // TODO Remove this. This is to ensure we always perform node ops on Nodes and
 // not Streams, but why is it needed??? Why do we get Streams and not Nodes from
 // emscripten in the case of xeus-python???
 class StreamNodeOps extends DriveFSEmscriptenNodeOps {
   private getNode(nodeOrStream: any) {
```

### Comparing `jupyterlite-xeus-nelson-0.1.2/style/logos/nelson-logo-32x32.png` & `jupyterlite-xeus-nelson-0.1.4/style/logos/nelson-logo-32x32.png`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/style/logos/nelson-logo-64x64.png` & `jupyterlite-xeus-nelson-0.1.4/style/logos/nelson-logo-64x64.png`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/tsconfig.json` & `jupyterlite-xeus-nelson-0.1.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlite-xeus-nelson-0.1.2/worker.webpack.config.js` & `jupyterlite-xeus-nelson-0.1.4/worker.webpack.config.js`

 * *Files identical despite different names*

