# Comparing `tmp/nbtools-23.1.1.tar.gz` & `tmp/nbtools-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbtools-23.1.1.tar", last modified: Mon Feb 27 18:05:05 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nbtools-23.1.1.tar` & `nbtools-23.4.0.tar`

### file list

```diff
@@ -1,172 +1,105 @@
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.864316 nbtools-23.1.1/
--rw-r--r--   0 tmtabor    (501) staff       (20)     1556 2022-06-08 20:58:11.000000 nbtools-23.1.1/LICENSE.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)      460 2022-06-08 20:58:11.000000 nbtools-23.1.1/MANIFEST.in
--rw-r--r--   0 tmtabor    (501) staff       (20)     7098 2023-02-27 18:05:05.864456 nbtools-23.1.1/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)     6141 2022-12-02 20:34:56.000000 nbtools-23.1.1/README.md
--rw-r--r--   0 tmtabor    (501) staff       (20)      175 2022-06-08 20:58:11.000000 nbtools-23.1.1/install.json
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.754124 nbtools-23.1.1/jupyter-config/
--rw-r--r--   0 tmtabor    (501) staff       (20)       61 2022-06-08 20:58:11.000000 nbtools-23.1.1/jupyter-config/nbtools.json
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.763753 nbtools-23.1.1/nbtools/
--rw-r--r--   0 tmtabor    (501) staff       (20)      626 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/__init__.py
--rw-r--r--   0 tmtabor    (501) staff       (20)      342 2023-01-24 21:18:57.000000 nbtools-23.1.1/nbtools/_frontend.py
--rw-r--r--   0 tmtabor    (501) staff       (20)      583 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/_version.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     2243 2023-01-06 19:25:25.000000 nbtools-23.1.1/nbtools/basewidget.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     1081 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/event_manager.py
--rw-r--r--   0 tmtabor    (501) staff       (20)    19059 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/form.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.766415 nbtools-23.1.1/nbtools/labextension/
--rw-r--r--   0 tmtabor    (501) staff       (20)     4206 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/package.json
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.747924 nbtools-23.1.1/nbtools/labextension/schemas/
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.748003 nbtools-23.1.1/nbtools/labextension/schemas/@g2nb/
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.767613 nbtools-23.1.1/nbtools/labextension/schemas/@g2nb/nbtools/
--rw-r--r--   0 tmtabor    (501) staff       (20)     4064 2023-02-06 20:48:12.000000 nbtools-23.1.1/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig
--rw-r--r--   0 tmtabor    (501) staff       (20)      267 2023-02-06 20:48:12.000000 nbtools-23.1.1/nbtools/labextension/schemas/@g2nb/nbtools/plugin.json
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.773259 nbtools-23.1.1/nbtools/labextension/static/
--rw-r--r--   0 tmtabor    (501) staff       (20)     4352 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/static/130.0b2fd2702a0ba6ad38e3.js
--rw-r--r--   0 tmtabor    (501) staff       (20)     1622 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/static/480.a182ea7f38bfaebed329.js
--rw-r--r--   0 tmtabor    (501) staff       (20)    64237 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/static/548.c965df4564626efe18a1.js
--rw-r--r--   0 tmtabor    (501) staff       (20)    14801 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/static/562.af0994874442e869102f.js
--rw-r--r--   0 tmtabor    (501) staff       (20)      571 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/static/568.aa19fecfc2b9209cafb7.js
--rw-r--r--   0 tmtabor    (501) staff       (20)     3206 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png
--rw-r--r--   0 tmtabor    (501) staff       (20)     7320 2023-02-06 20:48:14.000000 nbtools-23.1.1/nbtools/labextension/static/remoteEntry.ba586b21563191547cfe.js
--rw-r--r--   0 tmtabor    (501) staff       (20)      156 2023-02-06 20:48:12.000000 nbtools-23.1.1/nbtools/labextension/static/style.js
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.773703 nbtools-23.1.1/nbtools/nbextension/
--rw-r--r--   0 tmtabor    (501) staff       (20)      366 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/nbextension/__init__.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.847178 nbtools-23.1.1/nbtools/nbextension/static/
--rw-r--r--   0 tmtabor    (501) staff       (20)     4156 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/06de3f6f47040a96e1b75f57ff2be41f.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      211 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/084b59edab2415645e3e81e6a715dc08.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      564 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/09f3e4106c73962f016e29bf9aa511c6.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      306 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/0b22fba7dd1dd7b9b2f5cc46d4e2343c.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      279 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/0fc6ae9cf3db8ad62b1ce50985ae4997.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      221 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/116f568bf7597e30d8360c2efe449b63.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      331 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/12d813858e2776ce290f56682563c552.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      237 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/130adcee3c98b618a4a668288c24587c.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      356 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/1423798505a006a4e17f17749ad544c8.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      260 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/198b0cf0a6d5a82f0ff877fe941f534c.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      190 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/1c5056ac7d7d8820327000a4251a5826.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      300 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/20879f46e732b69ab5942128421e7947.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      321 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/2384dc2d9b2863753727a0c5ce6f7150.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      777 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/27799b9c71f8384579c91c8fe5fd1bf5.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      385 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/34d7bda6b5659a7576b34d0ddf5dc3e4.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      323 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/362fbe231037c25f7a611caa3b4db579.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      262 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/3a8202097fde21c1e477844e5a557a19.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      231 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/3bdec8e12c2e28692a2db78902270546.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      366 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/3c8a45bbaff2e2ac75697967a09b7834.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      203 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/3f007ba20eb241c8ad4d3885ca3a352b.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     1086 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/3f78bae66f3f0c1bb80081518b2f39c3.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)   431066 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/449.index.js
--rw-r--r--   0 tmtabor    (501) staff       (20)  1366766 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/449.index.js.map
--rw-r--r--   0 tmtabor    (501) staff       (20)     2683 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/4599b3e5fdd4b9105f79eb4a00f47c31.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      236 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/4aedea2f17daa7bd6ad26be5331763dc.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      594 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/4b1725b52d8a822e36344458b5fe5d21.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      268 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/512f128cab9c739c699701eee8f3793e.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      176 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/52c3f961b1d3f000192f051a3684a1ea.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      424 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/553bb18bd5e7b736c4e015184ab4659d.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      200 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/560dc3e7f90903da1d8ba690861e5031.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      313 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/59d7657abe1de2d882d725d2567902ce.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      220 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/5b2e933b72dbbf17d658660a64c344c1.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      826 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/5b5c6a5e8f2bb307621f68a6f86cdd34.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      206 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/5f66ff2286ae93ec6e1aa351f8192436.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      551 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/5fcd922b694ea6ba66bc2960fc33e9be.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     1266 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/6499261858a1c577a146396bcec0ded0.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      308 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/654cfb1ad0d1d267b994b3480a06e062.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     3206 2022-06-06 19:44:48.000000 nbtools-23.1.1/nbtools/nbextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png
--rw-r--r--   0 tmtabor    (501) staff       (20)      273 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/6c6bea7d7d02889e8ca5e8d06572662e.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      379 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/6d224f40ca23b04df4e3619b6c4bba76.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      375 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/6fca189fa236cfe127e49a5a4d89a860.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      178 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/6fe3ac7034084b13fef2f013f5c91c76.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      257 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/7082b6a15061f93789daee98201dcb53.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)    18062 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/7185e29562cd28f9d8d94281ac8116b7.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     1100 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/71d43e4a5bed70955292e9cb3b54252f.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      283 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/7a030a96a5c1e4891b2224c5dd88f034.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     2505 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/7e458ac5b31b3a94a909999c9d70747b.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      187 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/80d0949ae699e14879ba3ae8e6f2a6d0.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      158 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/81b872ff2598dc3a8989392d609dabf9.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     2430 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/8285512701f34fba20e2c626bc81a4a4.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      265 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/86ab1f825a5f23edee9db1889dd7edf4.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     3417 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/87.index.js
--rw-r--r--   0 tmtabor    (501) staff       (20)     6655 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/87.index.js.map
--rw-r--r--   0 tmtabor    (501) staff       (20)      155 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/94d1b702584fc9bd2b81aaba489f1650.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      246 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/95be09dbb0dadec5c9458d5f59ab3ed1.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      303 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/994d08381f6d718120e7526de4fbdc4e.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      433 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/9c216b64d89f6684903be78ddb816ed8.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      287 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/9c45117a9835179b589c1df8b5b1f5bb.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      275 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/9d06218717b0c9f85dcf7a44aeca640f.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      805 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/9d0d4001a9b235942c9962bbb3018292.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      248 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/9ee14d53fd4d29d6d7da4378c5d4f58b.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      811 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/9f0a1870be9c8512bee453fa6cf99379.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      505 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/a2de8f17fb958dc14948d65fcf06f0d2.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      352 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/a3eb4b2533f34b214cb09246b3feba99.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      848 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/b02c48a8976a75e2d11253862d07238c.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      340 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/b3c5b742151f6d37ed698a49a8c223c9.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      515 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/bfe144422b33598a7b506119ba719e23.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      396 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/cfa17f017a507f1c597659d37c199855.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      182 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/d495187f3516bbd70b1cfdcd186e60c9.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     2023 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/d59b4f3a4c519168d6bcce403f5f7b26.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      335 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/d6a8fcf35b6351eb6a91e197f2997489.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      872 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/d7112020a283e16b607ba2fd4bed2236.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      290 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/d88d4e8d3803004667125335ba98ac03.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      388 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/dcfff0af3da94527c965e5d932983b0e.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      275 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/e098544173383fff5e2403c7892e5b1e.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      174 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/e233dfabe787204ac02ab110de74d361.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      401 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/e520596c09ddc274eb550505e54b5919.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      361 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/ebb2089a97a4145ccaaf60b2da44d32f.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      509 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/ec2f8802c23b01973deeff26ba6a6298.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     1018 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/nbextension/static/extension.js
--rw-r--r--   0 tmtabor    (501) staff       (20)      412 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/f58b1e4a203f8656c7afb4a41c3a4a39.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      768 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/f8e2df8e00acf84af2b02609f17ed5ae.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      231 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/fd28bf7cde6fee72fccabed8636573f9.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      211 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/feead08f9feb89ed83118ebe5cd6eb8a.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)     2720 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/ff62e89fb77dd8b83487167dc7c1e492.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)  1949402 2023-02-06 20:48:55.000000 nbtools-23.1.1/nbtools/nbextension/static/index.js
--rw-r--r--   0 tmtabor    (501) staff       (20)     2534 2022-12-13 16:26:48.000000 nbtools-23.1.1/nbtools/nbextension/static/index.js.LICENSE.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)  5162690 2023-02-06 20:48:55.000000 nbtools-23.1.1/nbtools/nbextension/static/index.js.map
--rw-r--r--   0 tmtabor    (501) staff       (20)    21002 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/nbextension/static/notebook.css
--rw-r--r--   0 tmtabor    (501) staff       (20)    10342 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/nbextension/static/toolbox.js
--rw-r--r--   0 tmtabor    (501) staff       (20)       25 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/nbtools.json
--rw-r--r--   0 tmtabor    (501) staff       (20)     3074 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/parsing_manager.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     2019 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/settings.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.850315 nbtools-23.1.1/nbtools/tests/
--rw-r--r--   0 tmtabor    (501) staff       (20)        0 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/tests/__init__.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     1459 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/tests/conftest.py
--rw-r--r--   0 tmtabor    (501) staff       (20)      319 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/tests/test_example.py
--rw-r--r--   0 tmtabor    (501) staff       (20)      508 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/tests/test_nbextension_path.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     7102 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/tool_manager.py
--rw-r--r--   0 tmtabor    (501) staff       (20)    10306 2022-11-16 18:08:48.000000 nbtools-23.1.1/nbtools/uibuilder.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     1142 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/uioutput.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     1496 2022-11-16 17:53:38.000000 nbtools-23.1.1/nbtools/utils.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.766176 nbtools-23.1.1/nbtools.egg-info/
--rw-r--r--   0 tmtabor    (501) staff       (20)     7098 2023-02-27 18:05:05.000000 nbtools-23.1.1/nbtools.egg-info/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)     7222 2023-02-27 18:05:05.000000 nbtools-23.1.1/nbtools.egg-info/SOURCES.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-02-27 18:05:05.000000 nbtools-23.1.1/nbtools.egg-info/dependency_links.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2022-02-16 22:17:06.000000 nbtools-23.1.1/nbtools.egg-info/not-zip-safe
--rw-r--r--   0 tmtabor    (501) staff       (20)       76 2023-02-27 18:05:05.000000 nbtools-23.1.1/nbtools.egg-info/requires.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        8 2023-02-27 18:05:05.000000 nbtools-23.1.1/nbtools.egg-info/top_level.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)     4064 2023-02-27 18:04:13.000000 nbtools-23.1.1/package.json
--rw-r--r--   0 tmtabor    (501) staff       (20)      613 2022-10-14 16:03:01.000000 nbtools-23.1.1/pyproject.toml
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.850904 nbtools-23.1.1/schema/
--rw-r--r--   0 tmtabor    (501) staff       (20)      267 2022-06-08 20:58:11.000000 nbtools-23.1.1/schema/plugin.json
--rw-r--r--   0 tmtabor    (501) staff       (20)      106 2023-02-27 18:05:05.864912 nbtools-23.1.1/setup.cfg
--rw-r--r--   0 tmtabor    (501) staff       (20)     3225 2023-02-27 18:03:01.000000 nbtools-23.1.1/setup.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.859337 nbtools-23.1.1/src/
--rw-r--r--   0 tmtabor    (501) staff       (20)    15822 2022-06-08 20:58:11.000000 nbtools-23.1.1/src/basewidget.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)    17444 2022-06-13 21:26:19.000000 nbtools-23.1.1/src/context.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)     5371 2022-09-06 18:11:55.000000 nbtools-23.1.1/src/dataregistry.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)      638 2022-06-08 20:58:11.000000 nbtools-23.1.1/src/extension.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)      335 2022-06-08 20:58:11.000000 nbtools-23.1.1/src/index.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)     5235 2022-06-08 20:58:11.000000 nbtools-23.1.1/src/plugin.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)     6498 2022-06-08 20:58:11.000000 nbtools-23.1.1/src/registry.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)     8870 2022-11-15 18:03:15.000000 nbtools-23.1.1/src/toolbox.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)    31412 2023-01-24 21:14:46.000000 nbtools-23.1.1/src/uibuilder.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)    12739 2023-01-04 18:29:04.000000 nbtools-23.1.1/src/uioutput.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)     4636 2022-10-03 20:20:30.000000 nbtools-23.1.1/src/utils.ts
--rw-r--r--   0 tmtabor    (501) staff       (20)      264 2022-06-08 20:58:11.000000 nbtools-23.1.1/src/version.ts
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-27 18:05:05.863813 nbtools-23.1.1/style/
--rw-r--r--   0 tmtabor    (501) staff       (20)     3944 2022-06-13 21:19:05.000000 nbtools-23.1.1/style/basewidget.css
--rw-r--r--   0 tmtabor    (501) staff       (20)     3206 2022-06-08 20:58:11.000000 nbtools-23.1.1/style/g2nb_logo.png
--rw-r--r--   0 tmtabor    (501) staff       (20)    18062 2022-06-08 20:58:11.000000 nbtools-23.1.1/style/icon.svg
--rw-r--r--   0 tmtabor    (501) staff       (20)      106 2022-06-08 20:58:11.000000 nbtools-23.1.1/style/index.css
--rw-r--r--   0 tmtabor    (501) staff       (20)       22 2022-06-08 20:58:11.000000 nbtools-23.1.1/style/index.js
--rw-r--r--   0 tmtabor    (501) staff       (20)     3658 2022-06-08 20:58:11.000000 nbtools-23.1.1/style/toolbox.css
--rw-r--r--   0 tmtabor    (501) staff       (20)     5302 2022-06-13 18:16:23.000000 nbtools-23.1.1/style/uibuilder.css
--rw-r--r--   0 tmtabor    (501) staff       (20)     1467 2022-06-13 18:08:49.000000 nbtools-23.1.1/style/uioutput.css
--rw-r--r--   0 tmtabor    (501) staff       (20)      587 2022-06-08 20:58:11.000000 nbtools-23.1.1/tsconfig.json
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbtools-23.4.0/.coveragerc
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nbtools-23.4.0/.eslintignore
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 nbtools-23.4.0/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nbtools-23.4.0/.npmignore
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nbtools-23.4.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbtools-23.4.0/.prettierrc
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 nbtools-23.4.0/DEPLOY.md
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 nbtools-23.4.0/Dockerfile
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nbtools-23.4.0/appveyor.yml
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 nbtools-23.4.0/codecov.yml
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbtools-23.4.0/dev.Dockerfile
+-rwxr-xr-x   0        0        0      827 2020-02-02 00:00:00.000000 nbtools-23.4.0/docker_build.sh
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nbtools-23.4.0/install.json
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 nbtools-23.4.0/package.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nbtools-23.4.0/postBuild
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbtools-23.4.0/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nbtools-23.4.0/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nbtools-23.4.0/setup.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nbtools-23.4.0/tsconfig.json
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 nbtools-23.4.0/webpack.config.js
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/.gitignore
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/compiler.xml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/modules.xml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/nbtools.iml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/rSettings.xml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nbtools-23.4.0/config/overrides.json
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/toolmanager.md
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/uibuilder.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/uioutput.md
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/wysiwyg.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbtools-23.4.0/jupyter-config/nbtools.json
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/_frontend.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/_version.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/basewidget.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/event_manager.py
+-rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/form.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbtools.json
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/parsing_manager.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/settings.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tool_manager.py
+-rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/uibuilder.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/uioutput.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/utils.py
+-rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/build_log.json
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/package.json
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/schemas/@g2nb/nbtools/plugin.json
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js.map
+-rw-r--r--   0        0        0   141481 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js
+-rw-r--r--   0        0        0   139488 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map
+-rw-r--r--   0        0        0    33507 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map
+-rw-r--r--   0        0        0    29361 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js
+-rw-r--r--   0        0        0    28197 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js.map
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/style.js
+-rw-r--r--   0        0        0    16904 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js
+-rw-r--r--   0        0        0    14914 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js
+-rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/static/extension.js
+-rw-r--r--   0        0        0    21002 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/static/notebook.css
+-rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/static/toolbox.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/conftest.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/test_example.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.4.0/schema/plugin.json
+-rw-r--r--   0        0        0    15823 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/basewidget.ts
+-rw-r--r--   0        0        0    17444 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/context.ts
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/dataregistry.ts
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/extension.ts
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/index.ts
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/plugin.ts
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/registry.ts
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/toolbox.ts
+-rw-r--r--   0        0        0    31309 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/uibuilder.ts
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/uioutput.ts
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/utils.ts
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/version.ts
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/basewidget.css
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/g2nb_logo.png
+-rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/icon.svg
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/index.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/index.js
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/toolbox.css
+-rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/uibuilder.css
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/uioutput.css
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/karma.conf.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/tsconfig.json
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/src/index.spec.ts
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/src/utils.spec.ts
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 nbtools-23.4.0/.gitignore
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 nbtools-23.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 nbtools-23.4.0/README.md
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 nbtools-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 nbtools-23.4.0/PKG-INFO
```

### Comparing `nbtools-23.1.1/LICENSE.txt` & `nbtools-23.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/PKG-INFO` & `nbtools-23.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,59 @@
 Metadata-Version: 2.1
 Name: nbtools
-Version: 23.1.1
+Version: 23.4.0
 Summary: Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.
-Home-page: https://github.com/g2nb/nbtools
-Author: Thorin Tabor
-Author-email: tmtabor@cloud.ucsd.edu
-License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/g2nb/nbtools
+Author-email: Thorin Tabor <tmtabor@cloud.ucsd.edu>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2021, Regents of the University of California & Broad Institute
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE.txt
 Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
+Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
 Requires-Python: >=3.6
+Requires-Dist: ipyuploads
+Requires-Dist: ipywidgets<9,>7
+Requires-Dist: jupyterlab>=3.4
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
 
 # nbtools for JupyterLab
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/g2nb/nbtools/lab?urlpath=lab)
 [![Build Status](https://travis-ci.org/g2nb/nbtools.svg?branch=lab)](https://travis-ci.org/genepattern/nbtools)
 [![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat)](https://gpnotebook-website-docs.readthedocs.io/en/latest/)
 [![Docker Pulls](https://img.shields.io/docker/pulls/genepattern/genepattern-notebook.svg)](https://hub.docker.com/r/genepattern/lab/)
```

### Comparing `nbtools-23.1.1/README.md` & `nbtools-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/__init__.py` & `nbtools-23.4.0/nbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/_version.py` & `nbtools-23.4.0/nbtools/_version.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/basewidget.py` & `nbtools-23.4.0/nbtools/basewidget.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/event_manager.py` & `nbtools-23.4.0/nbtools/event_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/form.py` & `nbtools-23.4.0/nbtools/form.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/labextension/package.json` & `nbtools-23.4.0/nbtools/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.963503086419753%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6', 'yarn': '^1.22.19'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ed7f531dbfb094c43618.js'}}",*

 * * "'version'": "'23.3.2'"}*

```diff
@@ -3,18 +3,19 @@
         "email": "tmtabor@cloud.ucsd.edu",
         "name": "Thorin Tabor"
     },
     "bugs": {
         "url": "https://github.com/g2nb/nbtools/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^4.0.0",
+        "@jupyter-widgets/base": "^6",
         "@jupyterlab/application": "^3.0.4",
         "@jupyterlab/mainmenu": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.4"
+        "@jupyterlab/notebook": "^3.0.4",
+        "yarn": "^1.22.19"
     },
     "description": "Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.",
     "devDependencies": {
         "@jupyterlab/apputils": "^3.0.3",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/ui-components": "^3.0.3",
         "@lumino/application": "^1.13.1",
@@ -52,15 +53,15 @@
         "dist/*.{js,css}",
         "style/index.js"
     ],
     "homepage": "https://github.com/g2nb/nbtools",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ba586b21563191547cfe.js",
+            "load": "static/remoteEntry.ed7f531dbfb094c43618.js",
             "style": "./style"
         },
         "discovery": {
             "kernel": [
                 {
                     "base": {
                         "name": "nbtools"
@@ -125,9 +126,9 @@
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch",
         "watch:src": "tsc -w"
     },
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "./lib/index.d.ts",
-    "version": "23.1.0"
+    "version": "23.3.2"
 }
```

### Comparing `nbtools-23.1.1/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig` & `nbtools-23.4.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6'}", "'version'": "'23.4.0'"}*

```diff
@@ -3,15 +3,15 @@
         "email": "tmtabor@cloud.ucsd.edu",
         "name": "Thorin Tabor"
     },
     "bugs": {
         "url": "https://github.com/g2nb/nbtools/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^4.0.0",
+        "@jupyter-widgets/base": "^6",
         "@jupyterlab/application": "^3.0.4",
         "@jupyterlab/mainmenu": "^3.0.3",
         "@jupyterlab/notebook": "^3.0.4"
     },
     "description": "Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.",
     "devDependencies": {
         "@jupyterlab/apputils": "^3.0.3",
@@ -120,9 +120,9 @@
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch",
         "watch:src": "tsc -w"
     },
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "./lib/index.d.ts",
-    "version": "23.1.0"
+    "version": "23.4.0"
 }
```

### Comparing `nbtools-23.1.1/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png` & `nbtools-23.4.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/nbextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png` & `nbtools-23.4.0/style/g2nb_logo.png`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/nbextension/static/7185e29562cd28f9d8d94281ac8116b7.svg` & `nbtools-23.4.0/style/icon.svg`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/nbextension/static/extension.js` & `nbtools-23.4.0/nbtools/nbextension/static/extension.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/nbextension/static/notebook.css` & `nbtools-23.4.0/nbtools/nbextension/static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/nbextension/static/toolbox.js` & `nbtools-23.4.0/nbtools/nbextension/static/toolbox.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/parsing_manager.py` & `nbtools-23.4.0/nbtools/parsing_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/settings.py` & `nbtools-23.4.0/nbtools/settings.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/tests/conftest.py` & `nbtools-23.4.0/nbtools/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/tool_manager.py` & `nbtools-23.4.0/nbtools/tool_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/uibuilder.py` & `nbtools-23.4.0/nbtools/uibuilder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import functools
 import warnings
 
 from IPython.core.display import display
 from traitlets import Unicode, List, Bool, Dict, Instance, observe
-from ipywidgets import widget_serialization, Output
+from ipywidgets import widget_serialization, Output, VBox
 from ._frontend import module_name, module_version
 from .form import InteractiveForm
 from .basewidget import BaseWidget
 from .tool_manager import ToolManager, NBTool
 
 
 class build_ui:
@@ -31,15 +31,15 @@
 
     def __init__(self, *args, **kwargs):
         # Display if decorator with no arguments
         if len(args) > 0:
             self.func = args[0]                                 # Set the function
             self.__widget__ = UIBuilder(self.func)              # Set the widget
             self.func.__dict__["__widget__"] = self.__widget__  # Ensure function has access to widget
-            if self.__widget__.register_tool:
+            if self.__widget__.form.register_tool:
                 ToolManager.instance().register(self.__widget__)
 
             # Display if defined directly in a notebook
             # Don't display if loading from a library
             if self.func.__module__ == "__main__":
                 display(self.__widget__)
         else:
@@ -53,15 +53,15 @@
         # Figure out what type of call this is
         if self.func is None:
             # This is a call at define time for a decorator with arguments
             self.func = args[0]                                                  # Set the function
             self.__widget__ = UIBuilder(self.func, **self.kwargs)                # Set the widget
             self.func.__dict__["__widget__"] = self.__widget__                   # Ensure function has access to widget
             self.func._ipython_display_ = self._ipython_display_                 # Render widget when function returned
-            if self.__widget__.register_tool:
+            if self.__widget__.form.register_tool:
                 ToolManager.instance().register(self.__widget__)
 
             if self.func.__module__ == "__main__":  # Don't automatically display if loaded from library
                 display(self.__widget__)            # Display if defined in a notebook
 
             # Return wrapped function
             @functools.wraps(self.func)
@@ -75,18 +75,61 @@
             return self.func(*args, **kwargs)
 
     def _ipython_display_(self):
         """Display widget when returned in a notebook cell"""
         display(self.__widget__)
 
 
-class UIBuilder(BaseWidget, NBTool):
-    """
-    Widget used to render Python output in a UI
-    """
+class UIBuilder(VBox, NBTool):
+    """Widget used to render Python output in a UI"""
+    origin = None
+    id = None
+    name = None
+    description = None
+
+    def __init__(self, function_or_method, **kwargs):
+        # Set the function and defaults
+        self.function_or_method = function_or_method
+        self._apply_defaults(function_or_method)
+        self._apply_overrides(**kwargs)
+
+        # Create the child widgets
+        self.form = UIBuilderBase(function_or_method, **kwargs)
+        self.output = self.form.output
+
+        # Call the super constructor
+        VBox.__init__(self, [self.form, self.output])
+
+        # Insert a copy of this UI Builder when added as a tool
+        self.load = lambda **override_kwargs: UIBuilder(self.function_or_method, **{**kwargs, **override_kwargs})
+
+    def _apply_defaults(self, function_or_method):
+        # Set the name based on the function name
+        self.name = function_or_method.__qualname__
+        self.id = function_or_method.__qualname__
+
+        # Set the description based on the docstring
+        self.description = inspect.getdoc(function_or_method) or ''
+
+        # Set the origin based on the package name or "Notebook"
+        self.origin = 'Notebook' if function_or_method.__module__ == '__main__' else function_or_method.__module__
+
+    def _apply_overrides(self, **kwargs):
+        # Assign keyword parameters to this object
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+    def id(self):
+        """Return the function name regardless of custom display name"""
+        return self.function_or_method.__qualname__
+
+
+class UIBuilderBase(BaseWidget):
+    """Widget that renders a function as a UI form"""
+
     _model_name = Unicode('UIBuilderModel').tag(sync=True)
     _model_module = Unicode(module_name).tag(sync=True)
     _model_module_version = Unicode(module_version).tag(sync=True)
 
     _view_name = Unicode('UIBuilderView').tag(sync=True)
     _view_module = Unicode(module_name).tag(sync=True)
     _view_module_version = Unicode(module_version).tag(sync=True)
@@ -129,17 +172,14 @@
         # This is a hack necessary to prevent interact from throwing an error if parameters override is given
         if not self.parameters: self.parameters = self.parameters
 
         # Create the form and output child widgets
         self.form = InteractiveForm(function_or_method, self.parameters, parent=self, upload_callback=self.upload_callback)
         self.output = self.form.out
 
-        # Display the output underneath the UI Builder widget
-        self.on_displayed(lambda widget: display(widget.output))
-
         # Insert a copy of this UI Builder when added as a tool
         self.load = lambda **override_kwargs: UIBuilder(self.function_or_method, **{ **kwargs, **override_kwargs})
 
     def _apply_defaults(self, function_or_method):
         # Set the name based on the function name
         self.name = function_or_method.__qualname__
         self.id = function_or_method.__qualname__
@@ -179,21 +219,21 @@
         params = []  # Return a list of parameter dicts
 
         for param in sig.parameters.values():
             params.append({
                 "name": param.name,
                 "label": param.name,
                 "optional": param.default != inspect.Signature.empty,
-                "default": UIBuilder._safe_default(param.default),
-                "value": UIBuilder._safe_default(param.default),
+                "default": UIBuilderBase._safe_default(param.default),
+                "value": UIBuilderBase._safe_default(param.default),
                 "description": param.annotation if param.annotation != inspect.Signature.empty else '',
                 "hide": False,
-                "type": UIBuilder._guess_type(param.default),
+                "type": UIBuilderBase._guess_type(param.default),
                 "kinds": None,
-                "choices": UIBuilder._choice_defaults(param),
+                "choices": UIBuilderBase._choice_defaults(param),
                 "id": None,
                 "events": None
             })
 
         # Special case for output_var
         params.append({
             "name": 'output_var',
```

### Comparing `nbtools-23.1.1/nbtools/uioutput.py` & `nbtools-23.4.0/nbtools/uioutput.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/nbtools/utils.py` & `nbtools-23.4.0/nbtools/utils.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/package.json` & `nbtools-23.4.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.963888888888889%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6', 'yarn': '^1.22.19'}", "'version'": "'23.3.2'"}*

```diff
@@ -3,18 +3,19 @@
         "email": "tmtabor@cloud.ucsd.edu",
         "name": "Thorin Tabor"
     },
     "bugs": {
         "url": "https://github.com/g2nb/nbtools/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^4.0.0",
+        "@jupyter-widgets/base": "^6",
         "@jupyterlab/application": "^3.0.4",
         "@jupyterlab/mainmenu": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.4"
+        "@jupyterlab/notebook": "^3.0.4",
+        "yarn": "^1.22.19"
     },
     "description": "Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.",
     "devDependencies": {
         "@jupyterlab/apputils": "^3.0.3",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/ui-components": "^3.0.3",
         "@lumino/application": "^1.13.1",
@@ -120,9 +121,9 @@
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch",
         "watch:src": "tsc -w"
     },
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "./lib/index.d.ts",
-    "version": "23.1.1"
+    "version": "23.3.2"
 }
```

### Comparing `nbtools-23.1.1/src/basewidget.ts` & `nbtools-23.4.0/src/basewidget.ts`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         this.attach_menu_options();
         this.model.on('change:extra_menu_items', this.attach_menu_options, this);
 
         // Allow menus to overflow the container
         this.float_menus();
 
         // Initialize the widget
-        this.initialize(<WidgetView.InitializeParameters>{ options: {} });
+        this.initialize(<WidgetView.IInitializeParameters>{ options: {} });
 
         // Call any post render events
         this.post_render();
     }
 
     build() {
         // Parse the template
```

### Comparing `nbtools-23.1.1/src/context.ts` & `nbtools-23.4.0/src/context.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/src/dataregistry.ts` & `nbtools-23.4.0/src/dataregistry.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/src/extension.ts` & `nbtools-23.4.0/src/extension.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/src/plugin.ts` & `nbtools-23.4.0/src/plugin.ts`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 import { MODULE_NAME, MODULE_VERSION } from './version';
 import * as base_exports from './basewidget';
 import * as uioutput_exports from './uioutput';
 import * as uibuilder_exports from './uibuilder';
 import { IMainMenu } from '@jupyterlab/mainmenu';
 import { ToolBrowser, Toolbox } from "./toolbox";
 import { IToolRegistry, ToolRegistry } from "./registry";
-import { pulse_red } from "./utils";
+import { pulse_red, usage_tracker } from "./utils";
 import { ILabShell, ILayoutRestorer, JupyterFrontEnd } from "@jupyterlab/application";
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { ContextManager } from "./context";
 import { DataRegistry, IDataRegistry } from "./dataregistry";
 
-
-const documentation = 'nbtools:documentation';
 const module_exports = { ...base_exports, ...uioutput_exports, ...uibuilder_exports };
 const EXTENSION_ID = '@g2nb/nbtools:plugin';
 const NAMESPACE = 'nbtools';
 
 
 /**
  * The nbtools plugin.
@@ -50,29 +48,32 @@
     init_context(app as JupyterFrontEnd, notebook_tracker);
 
     // Create the tool and data registries
     const tool_registry = new ToolRegistry();
     const data_registry = new DataRegistry();
 
     // Add items to the help menu
-    add_documentation_link(app as JupyterFrontEnd, mainmenu);
+    add_help_links(app as JupyterFrontEnd, mainmenu);
 
     // Add keyboard shortcuts
     add_keyboard_shortcuts(app as JupyterFrontEnd, tool_registry);
 
     // Add the toolbox
     add_tool_browser(app as JupyterFrontEnd, restorer);
 
     // Register the nbtools widgets with the widget registry
     widget_registry.registerWidget({
         name: MODULE_NAME,
         version: MODULE_VERSION,
         exports: module_exports,
     });
 
+    // Register the plugin as loaded
+    usage_tracker('labextension_load', location.protocol + '//' + location.host + location.pathname);
+
     // Return the tool registry so that it is provided to other extensions
     return [tool_registry, data_registry];
 }
 
 function init_context(app:JupyterFrontEnd, notebook_tracker: INotebookTracker|null) {
     ContextManager.jupyter_app = app;
     ContextManager.notebook_tracker = notebook_tracker;
@@ -106,20 +107,40 @@
 
     // Add the tool browser widget to the application restorer
     if (restorer) restorer.add(tool_browser, NAMESPACE);
     app.shell.add(tool_browser, 'left', { rank: 102 });
 }
 
 /**
- * Add the nbtools documentation link to the help menu
+ * Add the nbtools documentation and feedback links to the help menu
  *
  * @param {Application<Widget>} app
  * @param {IMainMenu} mainmenu
  */
-function add_documentation_link(app:JupyterFrontEnd, mainmenu:IMainMenu|null) {
+function add_help_links(app:JupyterFrontEnd, mainmenu:IMainMenu|null) {
+    const feedback = 'nbtools:feedback';
+    const documentation = 'nbtools:documentation';
+
+    // Add feedback command to the command palette
+    app.commands.addCommand(feedback, {
+        label: 'g2nb Help Forum',
+        caption: 'Open the g2nb help forum',
+        isEnabled: () => !!app.shell,
+        execute: () => {
+            const url = 'https://community.mesirovlab.org/c/g2nb/';
+            let element = document.createElement('a');
+            element.href = url;
+            element.target = '_blank';
+            document.body.appendChild(element);
+            element.click();
+            document.body.removeChild(element);
+            return void 0;
+        }
+    });
+
     // Add documentation command to the command palette
     app.commands.addCommand(documentation, {
         label: 'nbtools Documentation',
         caption: 'Open documentation for nbtools',
         isEnabled: () => !!app.shell,
         execute: () => {
             const url = 'https://github.com/g2nb/nbtools#nbtools';
@@ -130,9 +151,9 @@
             element.click();
             document.body.removeChild(element);
             return void 0;
         }
     });
 
     // Add documentation link to the help menu
-    if (mainmenu) mainmenu.helpMenu.addGroup([{command: documentation}], 2);
+    if (mainmenu) mainmenu.helpMenu.addGroup([{command: feedback}, {command: documentation}], 2);
 }
```

### Comparing `nbtools-23.1.1/src/registry.ts` & `nbtools-23.4.0/src/registry.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/src/toolbox.ts` & `nbtools-23.4.0/src/toolbox.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/src/uibuilder.ts` & `nbtools-23.4.0/src/uibuilder.ts`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  *
  * @author Thorin Tabor
  *
  * Copyright 2020 Regents of the University of California and the Broad Institute
  */
 import '../style/uibuilder.css'
 import { MODULE_NAME, MODULE_VERSION } from './version';
-import { ISerializers, ManagerBase, unpack_models } from "@jupyter-widgets/base";
+import { ISerializers, unpack_models } from "@jupyter-widgets/base";
 import { BaseWidgetModel, BaseWidgetView } from "./basewidget";
 import { element_rendered, toggle } from "./utils";
 import { ContextManager } from "./context";
 
 // noinspection JSAnnotator
 export class UIBuilderModel extends BaseWidgetModel {
     static model_name = 'UIBuilderModel';
@@ -19,46 +19,43 @@
     static model_module_version = MODULE_VERSION;
     static view_name = 'UIBuilderView';
     static view_module = MODULE_NAME;
     static view_module_version = MODULE_VERSION;
 
     static serializers: ISerializers = {
         ...BaseWidgetModel.serializers,
-        form: {
-            deserialize: (value: any, manager: ManagerBase<any>|undefined) =>
-                unpack_models(value, manager as ManagerBase<any>)
-        }
+        form: { deserialize: unpack_models }
     };
 
     defaults() {
         return {
             ...super.defaults(),
             _model_name: UIBuilderModel.model_name,
             _model_module: UIBuilderModel.model_module,
             _model_module_version: UIBuilderModel.model_module_version,
             _view_name: UIBuilderModel.view_name,
             _view_module: UIBuilderModel.view_module,
             _view_module_version: UIBuilderModel.view_module_version,
             name: 'Python Function',
             description: '',
-            _parameters: [],
-            parameter_groups: [],
-            accept_origins: [],
+            _parameters: [] as any,
+            parameter_groups: [] as any,
+            accept_origins: [] as any,
             function_import: '',
             register_tool: true,
             collapse: true,
             events: {},
             buttons: {},
             license: {},
             display_header: true,
             display_footer: true,
             busy: false,
             run_label: 'Run',
-            form: undefined,
-            output: undefined
+            form: undefined as any,
+            output: undefined as any
         };
     }
 }
 
 // noinspection JSAnnotator
 export class UIBuilderView extends BaseWidgetView {
     dom_class = 'nbtools-uibuilder';
```

### Comparing `nbtools-23.1.1/src/uioutput.ts` & `nbtools-23.4.0/src/uioutput.ts`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * Widget for representing Python output as an interactive interface
  *
  * @author Thorin Tabor
  *
  * Copyright 2020 Regents of the University of California and the Broad Institute
  */
 import '../style/uioutput.css'
-import { ISerializers, ManagerBase, unpack_models } from '@jupyter-widgets/base';
+import { ISerializers, unpack_models } from '@jupyter-widgets/base';
 import { MODULE_NAME, MODULE_VERSION } from './version';
 import { BaseWidgetModel, BaseWidgetView } from "./basewidget";
 import { extract_file_name, extract_file_type, get_absolute_url, is_absolute_path, is_url } from './utils';
 import { ContextManager } from "./context";
 import { Data } from "./dataregistry";
 
 // noinspection JSAnnotator
@@ -20,36 +20,33 @@
     static model_module_version = MODULE_VERSION;
     static view_name = 'UIOutputView';
     static view_module = MODULE_NAME;
     static view_module_version = MODULE_VERSION;
 
     static serializers: ISerializers = {
         ...BaseWidgetModel.serializers,
-        appendix: {
-            deserialize: (value: any, manager: ManagerBase<any>|undefined) =>
-                unpack_models(value, manager as ManagerBase<any>)
-        }
+        appendix: { deserialize: unpack_models }
     };
 
     defaults() {
         return {
             ...super.defaults(),
             _model_name: UIOutputModel.model_name,
             _model_module: UIOutputModel.model_module,
             _model_module_version: UIOutputModel.model_module_version,
             _view_name: UIOutputModel.view_name,
             _view_module: UIOutputModel.view_module,
             _view_module_version: UIOutputModel.view_module_version,
             name: 'Python Results',
             description: '',
             status: '',
-            files: [],
+            files: [] as any,
             text: '',
             visualization: '',
-            appendix: undefined,
+            appendix: undefined as any,
             extra_file_menu_items: {}
         };
     }
 }
 
 // noinspection JSAnnotator
 export class UIOutputView extends BaseWidgetView {
```

### Comparing `nbtools-23.1.1/src/utils.ts` & `nbtools-23.4.0/src/utils.ts`

 * *Files 22% similar despite different names*

```diff
@@ -96,14 +96,16 @@
 
 /**
  * Show an element
  *
  * @param {HTMLElement} elem
  */
 export function show(elem:HTMLElement) {
+    if (!elem) return; // Protect against null elements
+
 	// Get the natural height of the element
 	const getHeight = function () {
 		elem.style.display = 'block'; // Make it visible
 		const height = elem.scrollHeight + 'px'; // Get it's height
 		elem.style.display = ''; //  Hide it again
 		return height;
 	};
@@ -122,14 +124,15 @@
 /**
  * Hide an element
  *
  * @param elem
  * @param min_height
  */
 export function hide(elem:HTMLElement, min_height='0') {
+    if (!elem) return; // Protect against null elements
     elem.classList.add('nbtools-toggle');
 
 	// Give the element a height to change from
 	elem.style.height = elem.scrollHeight + 'px';
 
 	// Set the height back to 0
 	setTimeout(function () {
@@ -172,8 +175,23 @@
     setTimeout(() => {
         element.style.border = `rgba(255, 0, 0, ${count / 10}) solid ${Math.ceil(count / 2)}px`;
         if (count_up && count < 10) pulse_red(element, count+1, count_up);
         else if (count_up) pulse_red(element, count, false);
         else if (count > 0) pulse_red(element, count-1, count_up);
         else element.style.border = `none`;
     }, 25);
+}
+
+/**
+ * We maintain a basic counter of how many times our tools are used; this helps us secure funding.
+ * No identifying information is sent.
+ *
+ * @param event_token
+ * @param description
+ * @param endpoint
+ */
+export function usage_tracker(event_token:string, description='', endpoint='https://workspace.g2nb.org/services/usage/') {
+    fetch(`${endpoint}${event_token}/`, {
+        method: "POST",
+        body: description
+    }).then(r => r.text()).then(b => console.log(`usage response: ${b}`));
 }
```

### Comparing `nbtools-23.1.1/style/basewidget.css` & `nbtools-23.4.0/style/basewidget.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/style/toolbox.css` & `nbtools-23.4.0/style/toolbox.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/style/uibuilder.css` & `nbtools-23.4.0/style/uibuilder.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/style/uioutput.css` & `nbtools-23.4.0/style/uioutput.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.1.1/tsconfig.json` & `nbtools-23.4.0/tsconfig.json`

 * *Files identical despite different names*

