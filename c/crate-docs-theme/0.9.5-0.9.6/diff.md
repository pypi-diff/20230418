# Comparing `tmp/crate-docs-theme-0.9.5.tar.gz` & `tmp/crate-docs-theme-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".dist/crate-docs-theme-0.9.5.tar", last modified: Mon May 18 17:04:50 2020, max compression
+gzip compressed data, was ".dist/crate-docs-theme-0.9.6.tar", last modified: Fri Jun  5 14:20:33 2020, max compression
```

## Comparing `crate-docs-theme-0.9.5.tar` & `crate-docs-theme-0.9.6.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/
--rw-r--r--   0 nomi       (501) staff       (20)      107 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/MANIFEST.in
--rw-r--r--   0 nomi       (501) staff       (20)      760 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/PKG-INFO
--rw-r--r--   0 nomi       (501) staff       (20)     1575 2020-01-28 16:48:33.000000 crate-docs-theme-0.9.5/README.rst
--rw-r--r--   0 nomi       (501) staff       (20)       23 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/requirements.txt
--rw-r--r--   0 nomi       (501) staff       (20)       38 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/setup.cfg
--rw-r--r--   0 nomi       (501) staff       (20)     2451 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/setup.py
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate/
--rw-r--r--   0 nomi       (501) staff       (20)     1217 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/__init__.py
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate/theme/
--rw-r--r--   0 nomi       (501) staff       (20)        0 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/__init__.py
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/
--rw-r--r--   0 nomi       (501) staff       (20)     1690 2020-05-18 17:01:55.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/__init__.py
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/
--rw-r--r--   0 nomi       (501) staff       (20)     3340 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/__init__.py
--rw-r--r--   0 nomi       (501) staff       (20)     1316 2020-05-18 16:38:07.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_cli.py
--rw-r--r--   0 nomi       (501) staff       (20)     1323 2020-05-18 16:38:07.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_howtos.py
--rw-r--r--   0 nomi       (501) staff       (20)     1322 2020-05-18 16:38:07.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_reference.py
--rw-r--r--   0 nomi       (501) staff       (20)     1322 2020-05-18 16:38:07.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_tutorials.py
--rw-r--r--   0 nomi       (501) staff       (20)     1313 2020-05-18 16:38:08.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_admin_ui.py
--rw-r--r--   0 nomi       (501) staff       (20)     1327 2020-05-18 16:38:08.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_clients_tools.py
--rw-r--r--   0 nomi       (501) staff       (20)     1312 2020-05-18 16:38:08.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_crash.py
--rw-r--r--   0 nomi       (501) staff       (20)     1317 2020-05-18 16:38:08.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_howtos.py
--rw-r--r--   0 nomi       (501) staff       (20)     1316 2020-05-18 16:38:08.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_reference.py
--rw-r--r--   0 nomi       (501) staff       (20)     1317 2020-05-18 16:38:08.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_tutorials.py
--rw-r--r--   0 nomi       (501) staff       (20)     1299 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/dbal.py
--rw-r--r--   0 nomi       (501) staff       (20)     1304 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/fake.py
--rw-r--r--   0 nomi       (501) staff       (20)     1299 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/jdbc.py
--rw-r--r--   0 nomi       (501) staff       (20)     1303 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/npgsql.py
--rw-r--r--   0 nomi       (501) staff       (20)     1297 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/pdo.py
--rw-r--r--   0 nomi       (501) staff       (20)     1303 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/python.py
--rw-r--r--   0 nomi       (501) staff       (20)     1295 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/sql_99.py
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/
--rw-r--r--   0 nomi       (501) staff       (20)     8026 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/base.html
--rw-r--r--   0 nomi       (501) staff       (20)     5342 2020-01-28 16:48:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/footer.html
--rw-r--r--   0 nomi       (501) staff       (20)      508 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/globaltoc.html
--rw-r--r--   0 nomi       (501) staff       (20)    16070 2020-05-06 14:36:28.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/layout.html
--rw-r--r--   0 nomi       (501) staff       (20)       10 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/localtoc.html
--rw-r--r--   0 nomi       (501) staff       (20)     2933 2020-01-28 16:48:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/navbar.html
--rw-r--r--   0 nomi       (501) staff       (20)      532 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/navbarsearchbox.html
--rw-r--r--   0 nomi       (501) staff       (20)       36 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/navbartoc.html
--rw-r--r--   0 nomi       (501) staff       (20)      470 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/relations.html
--rw-r--r--   0 nomi       (501) staff       (20)     1927 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/search.html
--rw-r--r--   0 nomi       (501) staff       (20)      344 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/searchbox.html
--rw-r--r--   0 nomi       (501) staff       (20)     1201 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/searchresults.html
--rw-r--r--   0 nomi       (501) staff       (20)      801 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/sidebar.html
--rw-r--r--   0 nomi       (501) staff       (20)     6237 2020-05-18 16:38:08.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/sidebartoc.html
--rw-r--r--   0 nomi       (501) staff       (20)      195 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/sourcelink.html
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/
--rwxr-xr-x   0 nomi       (501) staff       (20)    30435 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/bootstrap.css
--rw-r--r--   0 nomi       (501) staff       (20)    36562 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/components.css
--rw-r--r--   0 nomi       (501) staff       (20)     3828 2020-01-28 16:48:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/crateio-rtd.css
--rw-r--r--   0 nomi       (501) staff       (20)    39353 2019-10-29 14:07:18.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/crateio.css
--rw-r--r--   0 nomi       (501) staff       (20)    15283 2020-05-06 11:47:32.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/custom.css
--rw-r--r--   0 nomi       (501) staff       (20)     7757 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/normalize.css
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/
--rw-r--r--   0 nomi       (501) staff       (20)   129668 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Bold.ttf
--rwxr-xr-x   0 nomi       (501) staff       (20)    63892 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/BlenderPro-BoldWeb.woff
--rw-r--r--   0 nomi       (501) staff       (20)   126080 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Thin.ttf
--rwxr-xr-x   0 nomi       (501) staff       (20)    25984 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.eot
--rwxr-xr-x   0 nomi       (501) staff       (20)   113254 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.svg
--rwxr-xr-x   0 nomi       (501) staff       (20)    61496 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.ttf
--rwxr-xr-x   0 nomi       (501) staff       (20)    29504 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff
--rwxr-xr-x   0 nomi       (501) staff       (20)    22916 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff2
--rwxr-xr-x   0 nomi       (501) staff       (20)    25494 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.eot
--rwxr-xr-x   0 nomi       (501) staff       (20)   117489 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.svg
--rwxr-xr-x   0 nomi       (501) staff       (20)    65196 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.ttf
--rwxr-xr-x   0 nomi       (501) staff       (20)    29140 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff
--rwxr-xr-x   0 nomi       (501) staff       (20)    22536 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff2
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/
--rwxr-xr-x   0 nomi       (501) staff       (20)    24376 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/5645e3972a73124134e9e237_hero-job.jpg
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/
--rw-r--r--   0 nomi       (501) staff       (20)     4968 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/caution.png
--rw-r--r--   0 nomi       (501) staff       (20)    10299 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/caution@2x.png
--rw-r--r--   0 nomi       (501) staff       (20)     6119 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/note.png
--rw-r--r--   0 nomi       (501) staff       (20)    12447 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/note@2x.png
--rw-r--r--   0 nomi       (501) staff       (20)     5482 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/seealso.png
--rw-r--r--   0 nomi       (501) staff       (20)    10184 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/seealso@2x.png
--rw-r--r--   0 nomi       (501) staff       (20)     6622 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/tip.png
--rw-r--r--   0 nomi       (501) staff       (20)    12537 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/tip@2x.png
--rw-r--r--   0 nomi       (501) staff       (20)     6393 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/warning.png
--rw-r--r--   0 nomi       (501) staff       (20)    13581 2019-06-03 16:52:33.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/warning@2x.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    24742 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/amazon-logo-182.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    42694 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/apple-touch-icon.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    50935 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/blog.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)     2817 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_admin.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     8716 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_everywhere.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     9225 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_open-source.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    12382 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_scale.png
--rwxr-xr-x   0 nomi       (501) staff       (20)   107294 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-drink.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   161450 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-food.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   164518 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-gear.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   117529 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-nutrition.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   109761 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-sleep.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   150196 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-sport.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   152606 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-testing.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   129490 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-together.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   124277 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-wild.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)    39015 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/documentation.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   113806 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/efre_logo_l.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   636967 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/efre_logo_s.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)      399 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-facebook.png
--rwxr-xr-x   0 nomi       (501) staff       (20)      924 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-github.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     1067 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-google.png
--rwxr-xr-x   0 nomi       (501) staff       (20)      613 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-linkedin.png
--rwxr-xr-x   0 nomi       (501) staff       (20)      842 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-twitter.png
--rwxr-xr-x   0 nomi       (501) staff       (20)      554 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-youtube.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     4646 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-cisco.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     4318 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom-launchpad.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     2915 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     1846 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-hacker-news.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     4231 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-inventures.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     4291 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-pioneers.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     4988 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-sxsw.png
--rwxr-xr-x   0 nomi       (501) staff       (20)      895 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-techcrunch.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    10061 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-cisco-top-15 .png
--rwxr-xr-x   0 nomi       (501) staff       (20)    10499 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-gigaom-launchpad.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     5272 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-gigaom.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     2666 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-hacker-news.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     7534 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-inventures.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     7050 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-pioneers-final-8.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     8113 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-sxsw.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     2688 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-techcrunch.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     1150 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/favicon.ico
--rwxr-xr-x   0 nomi       (501) staff       (20)      344 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/favicon.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    26277 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/google-logo-210.png
--rwxr-xr-x   0 nomi       (501) staff       (20)   164678 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/hero-bg-about.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   203194 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/hero-crates.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)     2947 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-docs@2x.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     5350 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-home-fast-x100.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     5166 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-home-playswell-x100.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     2242 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-home-simple-x100.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     3032 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-install.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     8047 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-performance@2x.png
--rw-r--r--   0 nomi       (501) staff       (20)      531 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-search2x.png
--rwxr-xr-x   0 nomi       (501) staff       (20)      531 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-search@2x.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     3599 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-start@2x.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    10841 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-support@2x.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     3110 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_analytics.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     1176 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_blob.png
--rwxr-xr-x   0 nomi       (501) staff       (20)      546 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_document.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     2961 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_restructure.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     2507 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_search.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     2043 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/logo-crate.png
--rw-r--r--   0 nomi       (501) staff       (20)     1150 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/logo-eu-optimized-1.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)    14800 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/microsoft-logo-210.png
--rwxr-xr-x   0 nomi       (501) staff       (20)    23294 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/notadev.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)   390839 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/robert-downey-jr-i-love-you-kisses.gif
--rw-r--r--   0 nomi       (501) staff       (20)     6553 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/slack.png
--rwxr-xr-x   0 nomi       (501) staff       (20)     5700 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/softlayer-logo-200.png
--rwxr-xr-x   0 nomi       (501) staff       (20)   169279 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/techcrunch-disrupt-winners.jpg
--rwxr-xr-x   0 nomi       (501) staff       (20)    20538 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/usecases.jpg
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/
--rw-r--r--   0 nomi       (501) staff       (20)    64841 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/bootstrap.js
--rw-r--r--   0 nomi       (501) staff       (20)        0 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/crate.js
--rw-r--r--   0 nomi       (501) staff       (20)     1984 2020-05-04 16:59:21.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/custom.js
--rw-r--r--   0 nomi       (501) staff       (20)     9495 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/fontawesome.js
--rwxr-xr-x   0 nomi       (501) staff       (20)     5267 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/modernizr.js
--rw-r--r--   0 nomi       (501) staff       (20)    25449 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/searchtools.js
--rw-r--r--   0 nomi       (501) staff       (20)    11896 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/sticky-sidebar.min.js
--rw-r--r--   0 nomi       (501) staff       (20)    16258 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/underscore.min.js
--rwxr-xr-x   0 nomi       (501) staff       (20)   139639 2019-07-05 12:28:44.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/webflow.js
--rw-r--r--   0 nomi       (501) staff       (20)     1373 2018-03-29 16:10:45.000000 crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/theme.conf
-drwxr-xr-x   0 nomi       (501) staff       (20)        0 2020-05-18 17:04:50.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/
--rw-r--r--   0 nomi       (501) staff       (20)      760 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/PKG-INFO
--rw-r--r--   0 nomi       (501) staff       (20)     8242 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/SOURCES.txt
--rw-r--r--   0 nomi       (501) staff       (20)        1 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/dependency_links.txt
--rw-r--r--   0 nomi       (501) staff       (20)        6 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/namespace_packages.txt
--rw-r--r--   0 nomi       (501) staff       (20)        1 2018-04-11 12:38:30.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/not-zip-safe
--rw-r--r--   0 nomi       (501) staff       (20)       65 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/requires.txt
--rw-r--r--   0 nomi       (501) staff       (20)        6 2020-05-18 17:04:49.000000 crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/top_level.txt
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/
+-rw-r--r--   0 daisyt     (501) staff       (20)      107 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/MANIFEST.in
+-rw-r--r--   0 daisyt     (501) staff       (20)      760 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/PKG-INFO
+-rw-r--r--   0 daisyt     (501) staff       (20)     1575 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/README.rst
+-rw-r--r--   0 daisyt     (501) staff       (20)       23 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/requirements.txt
+-rw-r--r--   0 daisyt     (501) staff       (20)       38 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/setup.cfg
+-rw-r--r--   0 daisyt     (501) staff       (20)     2451 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/setup.py
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/
+-rw-r--r--   0 daisyt     (501) staff       (20)     1217 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/__init__.py
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/
+-rw-r--r--   0 daisyt     (501) staff       (20)        0 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/__init__.py
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/
+-rw-r--r--   0 daisyt     (501) staff       (20)     1690 2020-06-04 13:18:44.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/__init__.py
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/
+-rw-r--r--   0 daisyt     (501) staff       (20)     3340 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/__init__.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1316 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_cli.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1323 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_howtos.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1322 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_reference.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1322 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_tutorials.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1313 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_admin_ui.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1327 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_clients_tools.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1312 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_crash.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1317 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_howtos.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1316 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_reference.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1317 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_tutorials.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1299 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/dbal.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1304 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/fake.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1299 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/jdbc.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1303 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/npgsql.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1297 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/pdo.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1303 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/python.py
+-rw-r--r--   0 daisyt     (501) staff       (20)     1295 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/sql_99.py
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/
+-rw-r--r--   0 daisyt     (501) staff       (20)     8026 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/base.html
+-rw-r--r--   0 daisyt     (501) staff       (20)     5342 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/footer.html
+-rw-r--r--   0 daisyt     (501) staff       (20)      508 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/globaltoc.html
+-rw-r--r--   0 daisyt     (501) staff       (20)    16022 2020-06-04 13:02:18.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/layout.html
+-rw-r--r--   0 daisyt     (501) staff       (20)       10 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/localtoc.html
+-rw-r--r--   0 daisyt     (501) staff       (20)     2933 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/navbar.html
+-rw-r--r--   0 daisyt     (501) staff       (20)      532 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/navbarsearchbox.html
+-rw-r--r--   0 daisyt     (501) staff       (20)       36 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/navbartoc.html
+-rw-r--r--   0 daisyt     (501) staff       (20)      470 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/relations.html
+-rw-r--r--   0 daisyt     (501) staff       (20)     1927 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/search.html
+-rw-r--r--   0 daisyt     (501) staff       (20)      344 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/searchbox.html
+-rw-r--r--   0 daisyt     (501) staff       (20)     1201 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/searchresults.html
+-rw-r--r--   0 daisyt     (501) staff       (20)      801 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/sidebar.html
+-rw-r--r--   0 daisyt     (501) staff       (20)     6237 2020-06-02 13:35:26.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/sidebartoc.html
+-rw-r--r--   0 daisyt     (501) staff       (20)      195 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/sourcelink.html
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    30435 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/bootstrap.css
+-rw-r--r--   0 daisyt     (501) staff       (20)    36562 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/components.css
+-rw-r--r--   0 daisyt     (501) staff       (20)     3828 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/crateio-rtd.css
+-rw-r--r--   0 daisyt     (501) staff       (20)    39353 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/crateio.css
+-rw-r--r--   0 daisyt     (501) staff       (20)    15283 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/custom.css
+-rw-r--r--   0 daisyt     (501) staff       (20)     7757 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/normalize.css
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/
+-rw-r--r--   0 daisyt     (501) staff       (20)   129668 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Bold.ttf
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    63892 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/BlenderPro-BoldWeb.woff
+-rw-r--r--   0 daisyt     (501) staff       (20)   126080 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Thin.ttf
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    25984 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.eot
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   113254 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.svg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    61496 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.ttf
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    29504 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    22916 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff2
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    25494 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.eot
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   117489 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.svg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    65196 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.ttf
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    29140 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    22536 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff2
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    24376 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/5645e3972a73124134e9e237_hero-job.jpg
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/
+-rw-r--r--   0 daisyt     (501) staff       (20)     4968 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/caution.png
+-rw-r--r--   0 daisyt     (501) staff       (20)    10299 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/caution@2x.png
+-rw-r--r--   0 daisyt     (501) staff       (20)     6119 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/note.png
+-rw-r--r--   0 daisyt     (501) staff       (20)    12447 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/note@2x.png
+-rw-r--r--   0 daisyt     (501) staff       (20)     5482 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/seealso.png
+-rw-r--r--   0 daisyt     (501) staff       (20)    10184 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/seealso@2x.png
+-rw-r--r--   0 daisyt     (501) staff       (20)     6622 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/tip.png
+-rw-r--r--   0 daisyt     (501) staff       (20)    12537 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/tip@2x.png
+-rw-r--r--   0 daisyt     (501) staff       (20)     6393 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/warning.png
+-rw-r--r--   0 daisyt     (501) staff       (20)    13581 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/warning@2x.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    24742 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/amazon-logo-182.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    42694 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/apple-touch-icon.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    50935 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/blog.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2817 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_admin.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     8716 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_everywhere.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     9225 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_open-source.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    12382 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_scale.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   107294 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-drink.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   161450 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-food.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   164518 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-gear.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   117529 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-nutrition.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   109761 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-sleep.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   150196 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-sport.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   152606 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-testing.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   129490 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-together.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   124277 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-wild.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    39015 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/documentation.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   113806 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/efre_logo_l.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   636967 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/efre_logo_s.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      399 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-facebook.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      924 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-github.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     1067 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-google.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      613 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-linkedin.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      842 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-twitter.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      554 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-youtube.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     4646 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-cisco.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     4318 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom-launchpad.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2915 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     1846 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-hacker-news.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     4231 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-inventures.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     4291 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-pioneers.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     4988 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-sxsw.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      895 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-techcrunch.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    10061 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-cisco-top-15 .png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    10499 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-gigaom-launchpad.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     5272 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-gigaom.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2666 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-hacker-news.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     7534 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-inventures.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     7050 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-pioneers-final-8.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     8113 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-sxsw.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2688 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-techcrunch.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     1150 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/favicon.ico
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      344 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/favicon.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    26277 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/google-logo-210.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   164678 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/hero-bg-about.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   203194 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/hero-crates.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2947 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-docs@2x.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     5350 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-home-fast-x100.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     5166 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-home-playswell-x100.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2242 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-home-simple-x100.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     3032 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-install.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     8047 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-performance@2x.png
+-rw-r--r--   0 daisyt     (501) staff       (20)      531 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-search2x.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      531 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-search@2x.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     3599 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-start@2x.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    10841 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-support@2x.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     3110 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_analytics.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     1176 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_blob.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)      546 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_document.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2961 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_restructure.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2507 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_search.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     2043 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/logo-crate.png
+-rw-r--r--   0 daisyt     (501) staff       (20)     1150 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/logo-eu-optimized-1.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    14800 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/microsoft-logo-210.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    23294 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/notadev.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   390839 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/robert-downey-jr-i-love-you-kisses.gif
+-rw-r--r--   0 daisyt     (501) staff       (20)     6553 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/slack.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     5700 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/softlayer-logo-200.png
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   169279 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/techcrunch-disrupt-winners.jpg
+-rwxr-xr-x   0 daisyt     (501) staff       (20)    20538 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/usecases.jpg
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/
+-rw-r--r--   0 daisyt     (501) staff       (20)    64841 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/bootstrap.js
+-rw-r--r--   0 daisyt     (501) staff       (20)        0 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/crate.js
+-rw-r--r--   0 daisyt     (501) staff       (20)     1984 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/custom.js
+-rw-r--r--   0 daisyt     (501) staff       (20)     9495 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/fontawesome.js
+-rwxr-xr-x   0 daisyt     (501) staff       (20)     5267 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/modernizr.js
+-rw-r--r--   0 daisyt     (501) staff       (20)    25449 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/searchtools.js
+-rw-r--r--   0 daisyt     (501) staff       (20)    11896 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/sticky-sidebar.min.js
+-rw-r--r--   0 daisyt     (501) staff       (20)    16258 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/underscore.min.js
+-rwxr-xr-x   0 daisyt     (501) staff       (20)   139639 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/webflow.js
+-rw-r--r--   0 daisyt     (501) staff       (20)     1373 2020-05-13 09:48:27.000000 crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/theme.conf
+drwxr-xr-x   0 daisyt     (501) staff       (20)        0 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/
+-rw-r--r--   0 daisyt     (501) staff       (20)      760 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/PKG-INFO
+-rw-r--r--   0 daisyt     (501) staff       (20)     8242 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 daisyt     (501) staff       (20)        1 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 daisyt     (501) staff       (20)        6 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/namespace_packages.txt
+-rw-r--r--   0 daisyt     (501) staff       (20)        1 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/not-zip-safe
+-rw-r--r--   0 daisyt     (501) staff       (20)       65 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/requires.txt
+-rw-r--r--   0 daisyt     (501) staff       (20)        6 2020-06-05 14:20:33.000000 crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/top_level.txt
```

### Comparing `crate-docs-theme-0.9.5/PKG-INFO` & `crate-docs-theme-0.9.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: crate-docs-theme
-Version: 0.9.5
+Version: 0.9.6
 Summary: Crate Docs Theme
 Home-page: https://github.com/crate/crate-docs-theme
 Author: Crate.IO GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Description: A Sphinx theme for the Crate Documentation
 Keywords: crate docs sphinx readthedocs
```

### Comparing `crate-docs-theme-0.9.5/README.rst` & `crate-docs-theme-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/setup.py` & `crate-docs-theme-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/__init__.py` & `crate-docs-theme-0.9.6/src/crate/__init__.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/__init__.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 
 """Crate Sphix Theme for ReadTheDocs"""
 
 import os
 
-VERSION = (0, 9, 5)
+VERSION = (0, 9, 6)
 
 __version__ = ".".join(str(v) for v in VERSION)
 __version_full__ = __version__
 
 def current_dir():
     return os.path.abspath(os.path.dirname(__file__))
```

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/__init__.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_cli.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_cli.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_howtos.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_howtos.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_reference.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_reference.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/cloud_tutorials.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/cloud_tutorials.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_admin_ui.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_admin_ui.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_clients_tools.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_clients_tools.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_crash.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_crash.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_howtos.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_howtos.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_reference.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_reference.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/crate_tutorials.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/crate_tutorials.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/dbal.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/dbal.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/fake.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/fake.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/jdbc.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/jdbc.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/npgsql.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/npgsql.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/pdo.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/pdo.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/python.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/python.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/conf/sql_99.py` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/conf/sql_99.py`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/base.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/base.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/footer.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/footer.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/layout.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/layout.html`

 * *Files 8% similar despite different names*

```diff
@@ -106,17 +106,17 @@
                             }}{{ '%0A'
                             }}{{
                               '<!--Please do not edit or remove the following information -->'|urlencode }}{{ '%0A '
                             }}{{ '%0A'
                             }}{{
                               '- Page title: '|urlencode }}{{ title|striptags|urlencode }}{{ '%0A'
                             }}{{
-                              '- Page URL: https://crate.io/'|urlencode }}{{ theme_canonical_url_path|urlencode }}{{ pagename|urlencode }}{{ suffix }}{{ '%0A'
+                              '- Page URL: https://crate.io/'|urlencode }}{{ theme_canonical_url_path|urlencode }}{{ pagename|urlencode }}.html{{ '%0A'
                             }}{{
-                              '- Source: https://'|urlencode }}{{ github_host|default('github.com') }}/{{ github_user }}/{{ github_repo }}/{{ theme_vcs_pageview_mode|default('blob') }}/{{ github_version }}{{ conf_py_path|urlencode }}{{ pagename|urlencode }}.html{{ '%0A'
+                              '- Source: https://'|urlencode }}{{ github_host|default('github.com') }}/{{ github_user }}/{{ github_repo }}/{{ theme_vcs_pageview_mode|default('blob') }}/{{ github_version }}{{ conf_py_path|urlencode }}{{ pagename|urlencode }}{{ suffix }}{{ '%0A'
                             }}{{ '%0A'
                             }}---{{ '%0A'
                             }}{{ '%0A'
                             }}{{
                               '<!-- Please add your comments here -->'|urlencode }}{{ '%0A'
                             }}{{ '%0A'
                             }}" target="_blank" title="New issue">New issue</a>
@@ -180,16 +180,15 @@
   </script>
 
   <!-- Segment -->
   <script>
     !function(){var analytics=window.analytics=window.analytics||[];if(!analytics.initialize)if(analytics.invoked)window.console&&console.error&&console.error("Segment snippet included twice.");else{analytics.invoked=!0;analytics.methods=["trackSubmit","trackClick","trackLink","trackForm","pageview","identify","reset","group","track","ready","alias","debug","page","once","off","on","setAnonymousId"];analytics.factory=function(t){return function(){var e=Array.prototype.slice.call(arguments);e.unshift(t);analytics.push(e);return analytics}};for(var t=0;t<analytics.methods.length;t++){var e=analytics.methods[t];analytics[e]=analytics.factory(e)}analytics.load=function(t){var e=document.createElement("script");e.type="text/javascript";e.async=!0;e.src=("https:"===document.location.protocol?"https://":"http://")+"cdn.segment.com/analytics.js/v1/"+t+"/analytics.min.js";var n=document.getElementsByTagName("script")[0];n.parentNode.insertBefore(e,n)};analytics.SNIPPET_VERSION="4.0.0";
       analytics.load("{{ theme_tracking_segment_id }}");
       analytics.setAnonymousId($.cookie('uid'));
-      analytics.page();
-      analytics.track('visited_section_docs', {
+      analytics.page('visited_section_docs', {
         project: '{{ theme_tracking_project }}',
         version: '{{ current_version }}'
       });
     }}();
   </script>
 
   <!-- GitHub feedback section -->
@@ -288,40 +287,43 @@
             async function fetchIssues(url) {
               const data = await fetch(url).then((response) => response.json());
               return data;
             }
 
             const content = document.getElementById('cr-feedback-content');
             content.innerHTML = '<p>Loading data...</p>';
-            Promise.all([
-              fetchIssues("https://api.{{ github_host|default('github.com') }}/search/issues?q=repo:{{ github_user }}/{{ github_repo }}+label:documentation+is:open+{{ pagename|urlencode }}.html"),
-              fetchIssues("https://api.{{ github_host|default('github.com') }}/search/issues?q=repo:{{ github_user }}/{{ github_repo }}+label:documentation+is:closed+{{ pagename|urlencode }}.html")
-              ]).then(function ([openIssues, closedIssues]) {
-                var html = makeIssueHeader(openIssues['items'], closedIssues['items']);
-                html += listIssues(openIssues['items']);
-                html += listIssues(closedIssues['items'], true);
-                content.innerHTML = html;
-                const openButton = document.getElementById('issues-open');
-                const closedButton = document.getElementById('issues-closed');
-                const openList = document.getElementById('cr-docs-issues-open-list');
-                const closedList = document.getElementById('cr-docs-issues-closed-list');
-                openButton.addEventListener('click', function (e) {
-                  openButton.classList.add('cr-fb-active');
-                  closedButton.classList.remove('cr-fb-active');
-                  openList.style.display = 'block';
-                  closedList.style.display = 'none';
-                });
-                closedButton.addEventListener('click', function (e) {
-                  openButton.classList.remove('cr-fb-active');
-                  closedButton.classList.add('cr-fb-active');
-                  openList.style.display = 'none';
-                  closedList.style.display = 'block';
-                });
-              }).catch(function() {
-            // if rate limit exceeded, throw this error
+            fetchIssues("https://api.{{ github_host|default('github.com') }}/search/issues?q=repo:{{ github_user }}/{{ github_repo }}+label:documentation+{{ pagename|urlencode }}.html")
+                .then(function (issues) {
+                  const openIssues = issues.items.filter(x => x.state == 'open');
+                  const closedIssues = issues.items.filter(x => x.state == 'closed');
+                  var html = makeIssueHeader(openIssues, closedIssues);
+                  html += listIssues(openIssues);
+                  html += listIssues(closedIssues, true);
+                  content.innerHTML = html;
+                  const openButton = document.getElementById('issues-open');
+                  const closedButton = document.getElementById('issues-closed');
+                  const openList = document.getElementById('cr-docs-issues-open-list');
+                  const closedList = document.getElementById('cr-docs-issues-closed-list');
+                  openButton.addEventListener('click', function (e) {
+                    openButton.classList.add('cr-fb-active');
+                    closedButton.classList.remove('cr-fb-active');
+                    openList.style.display = 'block';
+                    closedList.style.display = 'none';
+                  });
+                  closedButton.addEventListener('click', function (e) {
+                    openButton.classList.remove('cr-fb-active');
+                    closedButton.classList.add('cr-fb-active');
+                    openList.style.display = 'none';
+                    closedList.style.display = 'block';
+                  });
+
+                analytics.track('Feedback Opened');
+
+                }).catch(function() {
+                // if rate limit exceeded, throw this error
                 content.innerHTML = '<p>Error loading data, limit exceeded. Please try again later.</p>';
                 analytics.track('DOCS RATE LIMIT', {
                   location: 'Center',
                   text: 'Error loading data, limit exceeded. Please try again later.',
                   category: 'Docs',
                   type: 'Text',
                   pageTitle: document.title
```

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/navbar.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/navbar.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/navbarsearchbox.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/navbarsearchbox.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/search.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/search.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/searchresults.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/searchresults.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/sidebar.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/sidebar.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/sidebartoc.html` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/sidebartoc.html`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/bootstrap.css` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/components.css` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/components.css`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/crateio-rtd.css` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/crateio-rtd.css`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/crateio.css` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/crateio.css`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/custom.css` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/css/normalize.css` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Bold.ttf` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/BlenderPro-BoldWeb.woff` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/BlenderPro-BoldWeb.woff`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Thin.ttf` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/BlenderPro-Thin.ttf`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.eot` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.svg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.ttf` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff2` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.eot` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.eot`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.svg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.svg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.ttf` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff2` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/fonts/blenderpro-thin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/5645e3972a73124134e9e237_hero-job.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/5645e3972a73124134e9e237_hero-job.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/caution.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/caution.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/caution@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/caution@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/note.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/note.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/note@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/note@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/seealso.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/seealso.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/seealso@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/seealso@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/tip.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/tip.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/tip@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/tip@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/warning.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/warning.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/admonition/warning@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/admonition/warning@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/amazon-logo-182.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/amazon-logo-182.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/apple-touch-icon.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/blog.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/blog.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_admin.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_admin.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_everywhere.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_everywhere.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_open-source.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_open-source.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/cloud_scale.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/cloud_scale.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-drink.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-drink.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-food.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-food.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-gear.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-gear.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-nutrition.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-nutrition.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-sleep.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-sleep.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-sport.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-sport.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-testing.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-testing.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-together.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-together.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/culture-wild.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/culture-wild.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/documentation.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/documentation.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/efre_logo_l.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/efre_logo_l.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/efre_logo_s.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/efre_logo_s.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-github.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-github.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-google.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-google.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-linkedin.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-linkedin.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-twitter.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-twitter.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/f-logo-youtube.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/f-logo-youtube.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-cisco.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-cisco.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom-launchpad.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom-launchpad.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-gigaom.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-hacker-news.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-hacker-news.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-inventures.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-inventures.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-pioneers.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-pioneers.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-sxsw.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-sxsw.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-bw-techcrunch.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-bw-techcrunch.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-cisco-top-15 .png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-cisco-top-15 .png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-gigaom-launchpad.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-gigaom-launchpad.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-gigaom.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-gigaom.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-hacker-news.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-hacker-news.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-inventures.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-inventures.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-pioneers-final-8.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-pioneers-final-8.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-sxsw.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-sxsw.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/fa-techcrunch.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/fa-techcrunch.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/favicon.ico` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/google-logo-210.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/google-logo-210.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/hero-bg-about.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/hero-bg-about.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/hero-crates.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/hero-crates.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-docs@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-docs@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-home-fast-x100.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-home-fast-x100.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-home-playswell-x100.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-home-playswell-x100.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-home-simple-x100.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-home-simple-x100.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-install.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-install.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-performance@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-performance@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-search2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-search2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-search@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-search@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-start@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-start@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon-support@2x.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon-support@2x.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_analytics.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_analytics.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_blob.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_blob.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_document.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_document.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_restructure.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_restructure.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/icon_search.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/icon_search.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/logo-crate.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/logo-crate.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/logo-eu-optimized-1.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/logo-eu-optimized-1.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/microsoft-logo-210.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/microsoft-logo-210.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/notadev.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/notadev.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/robert-downey-jr-i-love-you-kisses.gif` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/robert-downey-jr-i-love-you-kisses.gif`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/slack.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/slack.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/softlayer-logo-200.png` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/softlayer-logo-200.png`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/techcrunch-disrupt-winners.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/techcrunch-disrupt-winners.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/images/usecases.jpg` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/images/usecases.jpg`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/bootstrap.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/custom.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/fontawesome.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/modernizr.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/modernizr.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/searchtools.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/searchtools.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/sticky-sidebar.min.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/sticky-sidebar.min.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/underscore.min.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/underscore.min.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/static/js/webflow.js` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/static/js/webflow.js`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate/theme/rtd/crate/theme.conf` & `crate-docs-theme-0.9.6/src/crate/theme/rtd/crate/theme.conf`

 * *Files identical despite different names*

### Comparing `crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/PKG-INFO` & `crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: crate-docs-theme
-Version: 0.9.5
+Version: 0.9.6
 Summary: Crate Docs Theme
 Home-page: https://github.com/crate/crate-docs-theme
 Author: Crate.IO GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Description: A Sphinx theme for the Crate Documentation
 Keywords: crate docs sphinx readthedocs
```

### Comparing `crate-docs-theme-0.9.5/src/crate_docs_theme.egg-info/SOURCES.txt` & `crate-docs-theme-0.9.6/src/crate_docs_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

